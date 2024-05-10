# Comparing `tmp/bio_curve_fit-0.1.11.tar.gz` & `tmp/bio_curve_fit-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio_curve_fit-0.1.11.tar", max compression
+gzip compressed data, was "bio_curve_fit-0.1.12.tar", max compression
```

## Comparing `bio_curve_fit-0.1.11.tar` & `bio_curve_fit-0.1.12.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-02-19 19:10:23.981259 bio_curve_fit-0.1.11/LICENSE
--rw-r--r--   0        0        0     1488 2024-02-19 19:10:23.981259 bio_curve_fit-0.1.11/README.md
--rw-r--r--   0        0        0        0 2024-02-19 19:10:23.981259 bio_curve_fit-0.1.11/bio_curve_fit/__init__.py
--rw-r--r--   0        0        0      876 2024-02-19 19:10:23.981259 bio_curve_fit-0.1.11/bio_curve_fit/base.py
--rw-r--r--   0        0        0    10426 2024-02-19 19:10:23.981259 bio_curve_fit-0.1.11/bio_curve_fit/logistic.py
--rw-r--r--   0        0        0     4371 2024-02-19 19:10:23.981259 bio_curve_fit-0.1.11/bio_curve_fit/plotting.py
--rw-r--r--   0        0        0      689 2024-02-19 19:10:23.985259 bio_curve_fit-0.1.11/pyproject.toml
--rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 bio_curve_fit-0.1.11/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-10 14:43:36.479522 bio_curve_fit-0.1.12/LICENSE
+-rw-r--r--   0        0        0     1488 2024-05-10 14:43:36.479522 bio_curve_fit-0.1.12/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 14:43:36.479522 bio_curve_fit-0.1.12/bio_curve_fit/__init__.py
+-rw-r--r--   0        0        0      876 2024-05-10 14:43:36.479522 bio_curve_fit-0.1.12/bio_curve_fit/base.py
+-rw-r--r--   0        0        0    10426 2024-05-10 14:43:36.479522 bio_curve_fit-0.1.12/bio_curve_fit/logistic.py
+-rw-r--r--   0        0        0     4487 2024-05-10 14:43:36.479522 bio_curve_fit-0.1.12/bio_curve_fit/plotting.py
+-rw-r--r--   0        0        0      689 2024-05-10 14:43:36.479522 bio_curve_fit-0.1.12/pyproject.toml
+-rw-r--r--   0        0        0     2164 1970-01-01 00:00:00.000000 bio_curve_fit-0.1.12/PKG-INFO
```

### Comparing `bio_curve_fit-0.1.11/LICENSE` & `bio_curve_fit-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `bio_curve_fit-0.1.11/README.md` & `bio_curve_fit-0.1.12/README.md`

 * *Files identical despite different names*

### Comparing `bio_curve_fit-0.1.11/bio_curve_fit/base.py` & `bio_curve_fit-0.1.12/bio_curve_fit/base.py`

 * *Files identical despite different names*

### Comparing `bio_curve_fit-0.1.11/bio_curve_fit/logistic.py` & `bio_curve_fit-0.1.12/bio_curve_fit/logistic.py`

 * *Files identical despite different names*

### Comparing `bio_curve_fit-0.1.11/bio_curve_fit/plotting.py` & `bio_curve_fit-0.1.12/bio_curve_fit/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     - x_label (str, optional): Label for the X-axis. Default is "Concentration".
     - y_label (str, optional): Label for the Y-axis. Default is "Response".
     - show_plot (bool, optional): If True, display the plot. Default is False.
     - curve_kwargs (dict, optional): Keyword arguments for the plot function for the fitted curve. Default is {'label': 'Fitted curve', 'color': 'red'}.
     - data_kwargs (dict, optional): Keyword arguments for the scatter function for data points. Default is {'label': 'Data', 's': 12}.
     - llod_kwargs (dict, optional): Keyword arguments for the axhline function for the Lower Limit of Detection line. Default is {'color': 'red', 'linestyle': '--', 'label': 'LLOD'}.
     - ulod_kwargs (dict, optional): Keyword arguments for the axhline function for the Upper Limit of Detection line. Default is {'color': 'blue', 'linestyle': '--', 'label': 'ULOD'}.
-    - plot_kwargs (dict, optional): General keyword arguments for further plot customizations. This can include 'title_kwargs' for title properties and 'savefig_kwargs' for savefig properties, and 'formatter' for the x-axis formatter. Default is Log.
+    - plot_kwargs (dict, optional): General keyword arguments for further plot customizations. This can include 'title_kwargs' for title properties and 'savefig_kwargs' for savefig properties, 'formatter' for the x-axis formatter (Default is Log), and 'xscale' and 'yscale' for the plot scale (Default is 'log').
 
     Returns:
     - bytes: A bytes object containing the plot image in PNG format.
 
     Example Usage:
     plot_standard_curve(x_data, y_data, fitted_model, show_plot=True, curve_kwargs={'color': 'green', 'linestyle': '--'}, data_kwargs={'color': 'blue', 'marker': 'o'}, llod_kwargs={'color': 'orange'}, ulod_kwargs={'color': 'purple'})
 
@@ -53,16 +53,16 @@
     if data_kwargs is None:
         data_kwargs = {"label": "Data", "s": 12}
     if llod_kwargs is None:
         llod_kwargs = {"color": "red", "linestyle": "--", "label": "LLOD"}
     if ulod_kwargs is None:
         ulod_kwargs = {"color": "blue", "linestyle": "--", "label": "ULOD"}
 
-    plt.xscale("log")
-    plt.yscale("log")
+    plt.xscale(plot_kwargs.get("xscale", "log"))
+    plt.yscale(plot_kwargs.get("yscale", "log"))
     data = pd.DataFrame({"x": x_data, "y": y_data})
     filtered_data = data[data["x"] > 0]
 
     epsilon = 0.01
     x_min = np.log10(max(min(x_data), epsilon))
     x_max = max(x_data) * 2
     x = np.logspace(x_min, np.log10(x_max), 100)  # type: ignore
```

### Comparing `bio_curve_fit-0.1.11/pyproject.toml` & `bio_curve_fit-0.1.12/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bio-curve-fit"
-version = "0.1.11"
+version = "0.1.12"
 description = "Curve fitting algorithms for bio-assays with scikit-learn api"
 authors = ["Luke Schiefelbein <luke@ganymede.bio>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bio_curve_fit"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bio_curve_fit-0.1.11/PKG-INFO` & `bio_curve_fit-0.1.12/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-curve-fit
-Version: 0.1.11
+Version: 0.1.12
 Summary: Curve fitting algorithms for bio-assays with scikit-learn api
 License: MIT
 Author: Luke Schiefelbein
 Author-email: luke@ganymede.bio
 Requires-Python: >=3.8.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

