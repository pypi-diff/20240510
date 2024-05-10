# Comparing `tmp/dhuodata_lib-0.3.6.tar.gz` & `tmp/dhuodata_lib-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata_lib-0.3.6.tar", last modified: Wed May  8 16:43:13 2024, max compression
+gzip compressed data, was "dhuodata_lib-0.3.7.tar", last modified: Fri May 10 14:25:06 2024, max compression
```

## Comparing `dhuodata_lib-0.3.6.tar` & `dhuodata_lib-0.3.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 16:43:13.387906 dhuodata_lib-0.3.6/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 16:43:13.387906 dhuodata_lib-0.3.6/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.6/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-08 16:43:13.387906 dhuodata_lib-0.3.6/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-08 16:43:09.000000 dhuodata_lib-0.3.6/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 16:43:13.383906 dhuodata_lib-0.3.6/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 16:43:13.387906 dhuodata_lib-0.3.6/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-08 16:43:13.000000 dhuodata_lib-0.3.6/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      424 2024-05-08 16:43:13.000000 dhuodata_lib-0.3.6/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-08 16:43:13.000000 dhuodata_lib-0.3.6/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-08 16:43:13.000000 dhuodata_lib-0.3.6/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-08 16:43:13.000000 dhuodata_lib-0.3.6/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 16:43:13.387906 dhuodata_lib-0.3.6/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.6/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-04-23 16:50:53.000000 dhuodata_lib-0.3.6/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     7128 2024-05-08 16:41:21.000000 dhuodata_lib-0.3.6/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-04-25 14:26:18.000000 dhuodata_lib-0.3.6/src/dhuolib/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-04-24 18:22:52.000000 dhuodata_lib-0.3.6/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1943 2024-05-08 16:42:11.000000 dhuodata_lib-0.3.6/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      790 2024-05-08 01:22:24.000000 dhuodata_lib-0.3.6/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-04-23 16:51:15.000000 dhuodata_lib-0.3.6/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-08 16:43:13.387906 dhuodata_lib-0.3.6/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     3550 2024-05-07 16:59:04.000000 dhuodata_lib-0.3.6/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.7/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-10 14:24:24.000000 dhuodata_lib-0.3.7/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-10 14:25:06.000000 dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      445 2024-05-10 14:25:06.000000 dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-10 14:25:06.000000 dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-10 14:25:06.000000 dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-10 14:25:06.000000 dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.7/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.7/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     8143 2024-05-10 14:10:57.000000 dhuodata_lib-0.3.7/src/dhuolib/clients.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.7/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)       95 2024-05-09 16:59:36.000000 dhuodata_lib-0.3.7/src/dhuolib/enums.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.7/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3341 2024-05-10 13:47:21.000000 dhuodata_lib-0.3.7/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      790 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.7/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.7/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-10 14:25:06.038252 dhuodata_lib-0.3.7/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     5207 2024-05-10 14:23:03.000000 dhuodata_lib-0.3.7/tests/test_dhuolib.py
```

### Comparing `dhuodata_lib-0.3.6/PKG-INFO` & `dhuodata_lib-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.3.6
+Version: 0.3.7
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.3.6/README.md` & `dhuodata_lib-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.6/setup.py` & `dhuodata_lib-0.3.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.3.6",
+    version="0.3.7",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata_lib-0.3.6/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata_lib-0.3.7/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.3.6
+Version: 0.3.7
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
```

### Comparing `dhuodata_lib-0.3.6/src/dhuolib/clients.py` & `dhuodata_lib-0.3.7/src/dhuolib/clients.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,117 @@
 from pydantic import ValidationError
 import json
+import time
+import base64
 from dhuolib.config import logger
 from dhuolib.services import ServiceAPIML
 from dhuolib.validations import ExperimentBody, RunExperimentBody, PredictModelBody
 from werkzeug.datastructures import FileStorage
 
 
 class DhuolibClient:
-    def __init__(self, service_endpoint=None):
+    def __init__(self, service_endpoint=None, project_name=None):
         if not service_endpoint:
             raise ValueError("service_endpoint is required")
 
         self.service = ServiceAPIML(service_endpoint)
+        self.project_name = project_name   
 
     def create_experiment(self, experiment_params: dict) -> dict:
         params = {}
         response = None
 
         try:
             ExperimentBody.parse_obj(experiment_params)
         except ValidationError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
-        
-        if "requirements_file" in experiment_params.keys() and "model_pkl_file" in experiment_params.keys():
-            params["experiment_tags"] = json.dumps(
-                experiment_params["experiment_tags"]
-            )
+
+        if (
+            "requirements_file" in experiment_params.keys() 
+            and "model_pkl_file" in experiment_params.keys()
+        ):
+            params["experiment_tags"] = json.dumps(experiment_params["experiment_tags"])
             try:
                 with open(experiment_params["requirements_file"], "rb") as f1, open(
                     experiment_params["model_pkl_file"], "rb"
                 ) as f2:
-                    params = {
+                    files = {
                         "requirements_file": FileStorage(
-                            stream=f1, filename="requirements.txt", content_type="text/plain"
+                            stream=f1,
+                            filename="requirements.txt",
+                            content_type="text/plain",
                         ),
                         "model_pkl_file": FileStorage(
                             stream=f2,
                             filename="model.pkl",
                             content_type="application/octet-stream",
                         ),
                     }
-                    params = {**params, **experiment_params}
-    
-                    response = self.service.create_experiment_by_conf_json(params)
+                    response = self.service.create_experiment_by_conf_json(experiment_params, files)
 
                     experiment = response.json()
                     logger.info(
                         f"Experiment Name: {params['experiment_name']}"
                         f"Experiment ID: {experiment['experiment_id']} created"
                     )
                     return experiment
             except FileNotFoundError as e:
                 logger.error(f"Error: {e}")
                 return {"error": str(e)}
-        params = {**params, **experiment_params}
-        response = self.service.create_experiment_by_conf_json(params)
-        experiment = response.json()
+        response = self.service.create_experiment_by_conf_json(experiment_params)
         logger.info(
-            f"Experiment Name: {params['experiment_name']}"
-            f"Experiment ID: {experiment['experiment_id']} created"
+            f"Experiment Name: {experiment_params['experiment_name']}"
+            f"Experiment ID: {response['experiment_id']} created"
         )
-        return experiment
+        return response
 
     def run_experiment(self, params) -> dict:
         try:
             RunExperimentBody.parse_obj(params)
         except ValidationError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
-        
+
         try:
             with open(params["requirements_file"], "rb") as f1, open(
                 params["model_pkl_file"], "rb"
             ) as f2:
                 files = {
                     "requirements_file": FileStorage(
-                        stream=f1, filename="requirements.txt", content_type="text/plain"
+                        stream=f1,
+                        filename="requirements.txt",
+                        content_type="text/plain",
                     ),
                     "model_pkl_file": FileStorage(
                         stream=f2,
                         filename="model.pkl",
                         content_type="application/octet-stream",
                     ),
                 }
-             
+
                 if params["experiment_id"] is None:
                     experiment_id = self.create_experiment(params)
                     params["experiment_id"] = experiment_id
 
                 response = self.service.run_experiment(params=params, files=files)
                 logger.info(f"Experiment ID: {params['experiment_id']} running")
-                return response.json()
+                return response
         except FileNotFoundError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
 
     def create_model(self, model_params) -> dict:
         try:
             if model_params["stage"] is None:
                 model_params["stage"] = "STAGING"
 
             response = self.service.create_model(model_params)
             logger.info(f"Model Name: {model_params['modelname']} created")
-            return response.json()
+            return response
         except ValidationError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
 
     def predict_online(self, run_params) -> dict:
         try:
             PredictModelBody.parse_obj(run_params)
@@ -119,85 +123,82 @@
                 files = {
                     "data": FileStorage(
                         stream=f1, filename="data.csv", content_type="csv"
                     )
                 }
                 response = self.service.predict_online(params=run_params, files=files)
                 logger.info(f"Model Name: {run_params['modelname']} predictions")
-                return response.json()
+                return response
         except FileNotFoundError as e:
             logger.error(f"Error: {e}")
             return {"error": str(e)}
 
-    def load_model(self, model_name, tag) -> str:
-        print("loading model")
-        return "model_name.pkl"
-
-    def predict(self):
-        pass
-
-    def read_from_bucket(self, bucket: str, filename: str):
-        # OCI, GCP, AWS
-        return f"folder/{filename}"
-
-    # def read_from_bucket(self, filename: str):
-    #     default_bucket = "s3://default"
-    #     return self.read_from_bucket(default_bucket, filename)
-
-    def execute_select(self, statement: str):
-        # Acesso pela API ML Service
-        # Processo assíncrono
-        file = "s3://bucket/temp/file1.csv"
-        return file
-
-    def execute_dml(self, statement: str):
-        # rows_count - linhas afetadas
-
-        rows_count = 0
-        return rows_count
-
-    # Promover o model_name para "production"
-
-    # - [ ] criar cluster no Dataflow
-    # - [ ] informar o dado de schedule e criação de aplicação Dataflow
-    # - [ ] inserção de lista de dependencias: libs + zip + script.py
-
-    # @hydra.main(config_path="config", config_name="deploy")
-    def deploy(self, params):
-
-        # Enfileira o serviços
-
-        return None
-
-    def save_predictions(
-        self, dataset_predictions, inputs, predictions, model_name, tag
-    ):
-
-        return ""
-
-
-if __name__ == "__main__":
-    dhuolib = DhuolibClient()
-
-    experiment = "classificacao para recomendação"
-    experiment_id = dhuolib.create_experiment(experiment)
-
-    file = "pickle.file"
-    model_name = "model_decision_tree"
-    tag = "1.0.1"
-
-    save_status = dhuolib.save_model(experiment_id, file, model_name, tag)
-    print(save_status)
-
-    file = "pickle.file"
-    model_name = "model_logistic"
-    tag = "1.0.2"
-
-    save_status = dhuolib.save_model(experiment_id, file, model_name, tag)
-    print(save_status)
-
-    file = dhuolib.load_model("model_decision_tree", "1.0.1")
-
-    data_input = {"x": 1}
-    predictions = dhuolib.predict("model_decision_tree", "1.0.1", data_input)
+    def create_batch_project(self, project_name: str):
+        if project_name is None:
+            raise ValueError("project_name is required")
+        response = self.service.create_project(project_name)
+        return response
+
+    def deploy_batch_project(self, script_filename: str, requirements_filename: str):
+        if self.project_name is None:
+            raise ValueError("Batch project is required")
+
+        if script_filename is None or requirements_filename is None:
+            raise ValueError("script_filename and requirements_filename are required")
+
+        try:
+            with open(script_filename, "rb") as script_file, open(requirements_filename, "rb") as requirements_file:
+                encoded_script = base64.b64encode(script_file.read())
+                encoded_requirements = base64.b64encode(requirements_file.read())
+                response = self.service.deploy_script(
+                    self.project_name, encoded_script, encoded_requirements)
+                return response
+        except FileNotFoundError as e:
+            logger.error(f"Error: {e}")
+            return {"error": str(e)}
 
-    dhuolib.deploy()
+    def pipeline_status_report(self):
+        lst = []
+        if self.project_name is None:
+            raise ValueError("Batch project is required")
+        response = self.service.get_pipeline_status(self.project_name)
+        json_objects = json.loads(response.content)
+        for data in json_objects:
+            lst.append({
+                "date_log": data["date_log"],
+                "step": data["step"],
+                "status": data["status"]
+            })
+        return lst
+
+    def _create_cluster(self, cluster_size: int):
+        if self.project_name is None:
+            raise ValueError("Batch project is required")
+
+        if cluster_size not in [1, 2, 3]:
+            raise ValueError("cluster_size must be 1, 2 or 3")
+
+        response = self.service.create_cluster(self.project_name, cluster_size)
+        return response
+
+    def _batch_run(self):
+        if self.project_name is None:
+            raise ValueError("Batch project is required")
+
+        response = self.service.run_pipeline(self.project_name)
+        return response
+     
+    def predict_batch(self, cluster_size: int, script_filename: str, requirements_filename: str):
+        if self.project_name is None:
+            raise ValueError("Batch project is required")
+        response = self.deploy_batch_project(script_filename, requirements_filename)
+        logger.info(f"Deploy_batch_project {response} deployed")
+        while True:
+            status = self.pipeline_status_report()
+            if all([s["status"] == "DEPLOY COMPLETED SUCCESSFULLY" for s in status]):
+                break
+            time.sleep(30)
+        response = self._create_cluster(cluster_size)
+        logger.info(f"Create_cluster {response}")
+        response = self._batch_run()
+        logger.info(f"Batch Run {response}")
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dhuodata_lib-0.3.6/src/dhuolib/predict.py` & `dhuodata_lib-0.3.7/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.6/src/dhuolib/services.py` & `dhuodata_lib-0.3.7/src/dhuolib/services.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,48 +8,93 @@
 
         if not isinstance(service_endpoint, str):
             raise ValueError("service_endpoint must be a string")
 
         self.service_endpoint = f"{service_endpoint}/api/experiment"
         self.headers = {"Content-Type": "application/json"}
 
-    def create_experiment_by_conf_json(self, experiment_params):
+    def create_experiment_by_conf_json(self, experiment_params='', files=None):
         if experiment_params is None and isinstance(experiment_params, dict):
             raise ValueError("json_data must be a dict")
 
-        if 'model_pkl_file' in experiment_params.keys():
+        if files:
             return requests.post(
-                f"{self.service_endpoint}/save", data=experiment_params, headers={"Content-Type": "multipart/form-data"}
+                f"{self.service_endpoint}/save",
+                data=experiment_params,
+                files=files
             )
-            
-        return requests.post(f"{self.service_endpoint}/save", data=json.dumps(experiment_params), headers=self.headers)
+
+        response = requests.post(
+            f"{self.service_endpoint}/save",
+            data=json.dumps(experiment_params),
+            headers=self.headers,
+        )
+        return response.json()
 
     def run_experiment(self, params={}, files=None):
         if params is None and isinstance(params, str):
             raise ValueError("json_data must be a dict")
-        
+
         response = requests.post(
-            f"{self.service_endpoint}/run",
-            data=params,
-            files=files
+            f"{self.service_endpoint}/run", data=params, files=files
         )
-        return response
+        return response.json()
 
     def create_model(self, model_params):
         if model_params is None and not isinstance(model_params, dict):
             raise ValueError("json_data must be a dict")
         response = requests.post(
             f"{self.service_endpoint}/model",
             data=json.dumps(model_params),
             headers=self.headers,
         )
-        return response
+        return response.json()
 
     def predict_online(self, params={}, files=None):
         if params is None and not isinstance(params, dict):
             raise ValueError("json_data must be a dict")
         response = requests.post(
-            f"{self.service_endpoint}/predict_online",
-            data=params,
-            files=files
+            f"{self.service_endpoint}/predict_online", data=params, files=files
         )
-        return response
+        return response.json()
+
+    def create_project(self, project_name):
+        body = {
+            'name': project_name
+        }
+        response = requests.post(
+            f"{self.service_endpoint}/project", json=body)
+
+        return response.json()
+
+    def deploy_script(self, project_name: str, script_file_encode: str, requirements_file_enconde: str):
+        body = {
+            "project_name": project_name,
+            "requirements_content": requirements_file_enconde.decode("utf-8"),
+            "run_script_content": script_file_encode.decode("utf-8")
+        }
+        response = requests.post(f"{self.service_endpoint}/deploy", json=body)
+
+        return response.json()
+
+    def get_pipeline_status(self, project_name: str):
+        route = "deploy/{}".format(project_name)
+        response = requests.get(f"{self.service_endpoint}/{route}")
+
+        return response.json()
+
+    def create_cluster(self, project_name: str, cluster_size: int):
+        body = {
+            "project_name": project_name,
+            "cluster_size": cluster_size
+        }
+        response = requests.post(f"{self.service_endpoint}/cluster", json=body)
+
+        return response.json()
+
+    def run_pipeline(self, project_name: str):
+        body = {
+            "project_name": project_name
+        }
+        response = requests.post(f"{self.service_endpoint}/cluster/run", json=body)
+
+        return response.json()
```

### Comparing `dhuodata_lib-0.3.6/src/dhuolib/validations.py` & `dhuodata_lib-0.3.7/src/dhuolib/validations.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.6/tests/test_dhuolib.py` & `dhuodata_lib-0.3.7/tests/test_dhuolib.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from dhuolib.clients import DhuolibClient
 import sys
 import unittest
-from unittest.mock import patch
+from unittest.mock import patch, mock_open
+import base64
 
 sys.path.append("src")
 
 
 class TestDhuolibUtils(unittest.TestCase):
     def setUp(self):
         self.end_point = "http://localhost:8000"
-        self.dhuolib = DhuolibClient(service_endpoint=self.end_point)
+        self.dhuolib = DhuolibClient(
+            service_endpoint=self.end_point, project_name="TestProject")
         self.file_path = "tests/files/LogisticRegression_best.pickle"
 
-    def test_deve_lancar_excecao_com_valores_run_params_incorretos(self):
+    def test_1_deve_lancar_excecao_com_valores_run_params_incorretos(self):
         experiment_params = {
             "experiment_tags": {"version": "v1", "priority": "P1"},
         }
         response = self.dhuolib.create_experiment(experiment_params)
         self.assertEqual(list(response.keys()), ["error"])
 
     @patch("requests.post")
-    def test_deve_criar_o_experimento_com_run_params_corretos(self, mock_post):
-        client = DhuolibClient(service_endpoint=self.end_point)
-
+    def test_2_deve_criar_o_experimento_com_run_params_corretos(self, mock_post):
         mock_response = mock_post.return_value
         mock_response.status_code = 201
         mock_response.json.return_value = {"experiment_id": "1"}
 
         experiment_params = {
             "experiment_name": "test_experiment",
-            "experiment_tags": {"version": "v1", "priority": "P1"}
+            "experiment_tags": {"version": "v1", "priority": "P1"},
         }
 
-        response = client.create_experiment(experiment_params)
+        response = self.dhuolib.create_experiment(experiment_params)
         self.assertEqual(response, mock_response.json.return_value)
 
     @patch("requests.post")
-    def test_deve_executar_o_experimento_com_run_params_corretos(self, mock_post):
+    def test_3_deve_executar_o_experimento_com_run_params_corretos(self, mock_post):
         mock_response = mock_post.return_value
         mock_response.status_code = 201
         mock_response.json.return_value = {
             "experiment_id": "experiment_id",
             "run_id": "run_id",
             "model_uri": "model_uri",
         }
@@ -51,15 +51,15 @@
             "requirements_file": "tests/files/requirements.txt",
         }
         response = self.dhuolib.run_experiment(run_params)
 
         self.assertEqual(response, mock_response.json.return_value)
 
     @patch("requests.post")
-    def test_deve_criar_modelo_com_run_params_corretos(self, mock_post):
+    def test_4_deve_criar_modelo_com_run_params_corretos(self, mock_post):
         mock_response = mock_post.return_value
         mock_response.status_code = 201
         mock_response.json.return_value = {
             "current_stage": "Production",
             "last_updated_timestamp": 1713582060414,
             "model_version": "1",
             "run_id": "9434e517ed104958b6f5f47d33c79184",
@@ -68,33 +68,63 @@
 
         run_params = {
             "stage": "Production",
             "modelname": "nlp_framework",
             "modeltag": "v1",
             "run_id": "9434e517ed104958b6f5f47d33c79184",
             "requirements_file": "tests/files/requirements.txt",
-            "model_uri": "model_uri"
+            "model_uri": "model_uri",
         }
 
         response = self.dhuolib.create_model(run_params)
 
         self.assertEqual(response, mock_response.json.return_value)
 
     @patch("requests.post")
-    def test_deve_fazer_o_predict_online_a_partir_de_um_dataset(self, mock_post):
+    def test_5_deve_fazer_o_predict_online_a_partir_de_um_dataset(self, mock_post):
         mock_response = mock_post.return_value
         mock_response.status_code = 201
         mock_response.json.return_value = {
             "model_name": "nlp_framework",
             "predictions": [0, 1, 0, 1, 0, 1, 0, 1, 0, 1],
         }
 
         run_params = {
             "stage": "Production",
             "data": "tests/files/data_predict.csv",
             "modelname": "nlp_framework",
-
         }
 
         response = self.dhuolib.predict_online(run_params)
 
         self.assertEqual(response, mock_response.json.return_value)
+
+    @patch("requests.post")
+    def test_6_create_batch_project_successful(self, mock_post):
+        project_name = "Test Project"
+        mock_response = mock_post.return_value
+        mock_response.status_code = 201
+        mock_response.json.return_value = {"status": "success", "project_id": 123}
+        response = self.dhuolib.create_batch_project(project_name)
+        self.assertEqual(response, {"status": "success", "project_id": 123})
+
+    def test_7_create_batch_project_raises_exception_on_none(self):
+        with self.assertRaises(ValueError) as context:
+            self.dhuolib.create_batch_project(None)
+        self.assertTrue("project_name is required" in str(context.exception))
+
+    def test_8_deploy_batch_project_no_project_name(self):
+        self.dhuolib = DhuolibClient(service_endpoint=self.end_point)
+        with self.assertRaises(ValueError) as context:
+            self.dhuolib.deploy_batch_project("script.py", "requirements.txt")
+        self.assertTrue("Batch project is required" in str(context.exception))
+
+    def test_9_deploy_batch_project_missing_files(self):
+        with self.assertRaises(ValueError) as context:
+            self.dhuolib.deploy_batch_project(None, None)
+        self.assertTrue(
+            "script_filename and requirements_filename are required" in str(context.exception))
+
+    def test_10_deploy_batch_project_file_not_found(self):
+        with patch("builtins.open", side_effect=FileNotFoundError("File not found")):
+            response = self.dhuolib.deploy_batch_project("script.py", "requirements.txt")
+            self.assertEqual(response, {"error": "File not found"})
```

