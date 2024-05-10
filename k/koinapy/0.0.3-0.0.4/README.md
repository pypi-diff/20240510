# Comparing `tmp/koinapy-0.0.3.tar.gz` & `tmp/koinapy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koinapy-0.0.3.tar", max compression
+gzip compressed data, was "koinapy-0.0.4.tar", max compression
```

## Comparing `koinapy-0.0.3.tar` & `koinapy-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       37 2024-03-05 16:36:54.655226 koinapy-0.0.3/README.md
--rw-r--r--   0        0        0       24 2024-03-05 16:36:54.655226 koinapy-0.0.3/koinapy/__init__.py
--rw-r--r--   0        0        0      930 2024-03-05 16:36:54.655226 koinapy-0.0.3/koinapy/__main__.py
--rw-r--r--   0        0        0    27722 2024-03-05 16:36:54.655226 koinapy-0.0.3/koinapy/grpc.py
--rw-r--r--   0        0        0      783 2024-03-05 16:36:54.659226 koinapy-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 koinapy-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-10 11:43:41.840293 koinapy-0.0.4/README.md
+-rw-r--r--   0        0        0       24 2024-05-10 11:43:41.840293 koinapy-0.0.4/koinapy/__init__.py
+-rw-r--r--   0        0        0      930 2024-05-10 11:43:41.840293 koinapy-0.0.4/koinapy/__main__.py
+-rw-r--r--   0        0        0    28557 2024-05-10 11:43:41.840293 koinapy-0.0.4/koinapy/grpc.py
+-rw-r--r--   0        0        0      783 2024-05-10 11:43:41.840293 koinapy-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 koinapy-0.0.4/PKG-INFO
```

### Comparing `koinapy-0.0.3/koinapy/__main__.py` & `koinapy-0.0.4/koinapy/__main__.py`

 * *Files identical despite different names*

### Comparing `koinapy-0.0.3/koinapy/grpc.py` & `koinapy-0.0.4/koinapy/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
     def __init__(
         self,
         model_name: str,
         server_url: str = "koina.wilhelmlab.org:443",
         ssl: bool = True,
         targets: Optional[List[str]] = None,
-        disable_progress_bar: bool = False,
     ):
         """
         Initialize a KoinaModel instance with the specified parameters.
 
         This constructor initializes the KoinaModel instance, connecting it to the specified Inference Server.
         It checks the availability of the server, the specified model, retrieves input and output information,
         and determines the maximum batch size supported by the model's configuration.
@@ -50,15 +49,14 @@
         self.model_inputs = {}
         self.model_outputs = {}
         self._response_dict = {}
 
         self.model_name = model_name
         self.url = server_url
         self.ssl = ssl
-        self.disable_progress_bar = disable_progress_bar
         self.client = InferenceServerClient(url=server_url, ssl=ssl)
 
         self.type_convert = {
             "FP32": np.dtype("float32"),
             "BYTES": np.dtype("O"),
             "INT16": np.dtype("int16"),
             "INT32": np.dtype("int32"),
@@ -465,15 +463,15 @@
                 client_timeout=timeout,
             )
             yield
 
     def predict(
         self,
         data: Union[Dict[str, np.ndarray], pd.DataFrame],
-        _async: bool = True,
+        mode="semi_async",
         debug=False,
     ) -> Dict[str, np.ndarray]:
         """
         Perform inference on the given data using the Koina model.
 
         This method allows you to perform inference on the provided input data using the configured Koina model. You can
         choose to perform inference asynchronously (in parallel) or sequentially, depending on the value of the '_async'
@@ -502,21 +500,44 @@
             predictions = model.predict(input_data)
         """
         if isinstance(data, pd.DataFrame):
             data = {
                 input_field: data[input_field].to_numpy().reshape(-1, 1)
                 for input_field in self.model_inputs.keys()
             }
-        if _async:
+        if mode == "semi_async":
+            return self.__predict_semi_async(data, debug=debug)
+        elif mode == "async":
             return self.__predict_async(data, debug=debug)
-        else:
+        elif mode == "sync":
             return self.__predict_sequential(data)
+        else:
+            raise ValueError(f"mode must be one of 'semi_async', 'async' or 'sync'")
+
+    def __predict_semi_async(self, data, debug=False, disable_progress_bar=False):
+        results = []
+        data_subsets = list(self.__slice_dict(data, self.batchsize * 10))
+        pbar = tqdm(
+            total=len(data_subsets) * 10,
+            desc=f"{self.model_name}:",
+            disable=disable_progress_bar,
+        )
+        for data_batch in data_subsets:
+            results.append(
+                self.__predict_async(data_batch, debug=debug, pbar_input=pbar)
+            )
+        pbar.close()
+        return self.__merge_list_dict_array(results)
 
     def __predict_async(
-        self, data: Dict[str, np.ndarray], debug=False
+        self,
+        data: Dict[str, np.ndarray],
+        debug=False,
+        disable_progress_bar=False,
+        pbar_input=None,
     ) -> Dict[str, np.ndarray]:
         """
         Perform asynchronous inference on the given data using the Koina model.
 
         This method performs asynchronous inference on the provided input data using the configured Koina model.
         Asynchronous inference allows for parallel processing of input data, potentially leading to faster results.
         The method will return when all asynchronous inference tasks are complete. Note: Ensure that the model and server
@@ -537,36 +558,42 @@
                 self.__async_predict_batch(
                     data_batch, infer_results, request_id=i, retries=0
                 )
             )
             next(tasks[i])
 
         n_tasks = i + 1
-        with tqdm(
-            total=n_tasks, desc="Getting predictions", disable=self.disable_progress_bar
-        ) as pbar:
-            unfinished_tasks = [i for i in range(n_tasks)]
-            while pbar.n < n_tasks:
-                time.sleep(0.5)
-                new_unfinished_tasks = []
-                for j in unfinished_tasks:
-                    result = infer_results.get(j)
-                    if result is None:
+        if pbar_input is None:
+            pbar = tqdm(
+                total=n_tasks, desc=f"{self.model_name}:", disable=disable_progress_bar
+            )
+        else:
+            pbar = pbar_input
+        unfinished_tasks = [i for i in range(n_tasks)]
+        while len(unfinished_tasks) > 0:
+            time.sleep(0.5)
+            new_unfinished_tasks = []
+            for j in unfinished_tasks:
+                result = infer_results.get(j)
+                if result is None:
+                    new_unfinished_tasks.append(j)
+                elif isinstance(result, dict):
+                    pbar.n += 1
+                else:  # unexpected result / exception -> try again
+                    try:
+                        next(tasks[j])
                         new_unfinished_tasks.append(j)
-                    elif isinstance(result, dict):
+                    except StopIteration:
                         pbar.n += 1
-                    else:  # unexpected result / exception -> try again
-                        try:
-                            next(tasks[j])
-                            new_unfinished_tasks.append(j)
-                        except StopIteration:
-                            pbar.n += 1
 
-                unfinished_tasks = new_unfinished_tasks
-                pbar.refresh()
+            unfinished_tasks = new_unfinished_tasks
+            pbar.refresh()
+
+        if pbar_input is None:
+            pbar.close()
 
         return self.__handle_results(infer_results, debug)
 
     def __handle_results(
         self,
         infer_results: Dict[
             int, Union[Dict[str, np.ndarray], InferenceServerException]
```

### Comparing `koinapy-0.0.3/pyproject.toml` & `koinapy-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "koinapy"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python client to communicate with Koina."
 authors = ["Ludwig Lautenbacher <Ludwig.Lautenbacher@tum.de>"]
 license = "Apache 2.0"
 homepage = "https://koina.wilhelmlab.org/"
 repository = "https://github.com/wilhelm-lab/koina"
 documentation = "https://koina.wilhelmlab.org/docs"
 readme = "README.md"
```

### Comparing `koinapy-0.0.3/PKG-INFO` & `koinapy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koinapy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python client to communicate with Koina.
 Home-page: https://koina.wilhelmlab.org/
 License: Apache 2.0
 Author: Ludwig Lautenbacher
 Author-email: Ludwig.Lautenbacher@tum.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
```

