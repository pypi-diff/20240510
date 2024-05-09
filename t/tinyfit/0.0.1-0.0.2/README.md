# Comparing `tmp/tinyfit-0.0.1.tar.gz` & `tmp/tinyfit-0.0.2.tar.gz`

## Comparing `tinyfit-0.0.1.tar` & `tinyfit-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 tinyfit-0.0.1/test.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tinyfit-0.0.1/src/tinyfit/__init__.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 tinyfit-0.0.1/src/tinyfit/linreg.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 tinyfit-0.0.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 tinyfit-0.0.1/LICENSE
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyfit-0.0.1/README.md
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 tinyfit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tinyfit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 tinyfit-0.0.2/test.ipynb
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 tinyfit-0.0.2/test.py
+-rw-r--r--   0        0        0   113301 2020-02-02 00:00:00.000000 tinyfit-0.0.2/test_nb.ipynb
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 tinyfit-0.0.2/src/tinyfit/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tinyfit-0.0.2/src/tinyfit/linreg.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 tinyfit-0.0.2/src/tinyfit/scaling.py
+-rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 tinyfit-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 tinyfit-0.0.2/LICENSE
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 tinyfit-0.0.2/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tinyfit-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 tinyfit-0.0.2/PKG-INFO
```

### Comparing `tinyfit-0.0.1/src/tinyfit/linreg.py` & `tinyfit-0.0.2/src/tinyfit/linreg.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,25 +15,29 @@
 
         for i in range(iter):
             x = x.reshape(-1,self.n_features)
             y = y.reshape(-1,1)
             pred = x.dot(self.W) + self.b
             diff = pred - y
             square = diff.T.dot(diff)
-            mse = square/self.n_features
+            mse = square/x.shape[0]
             
-            grad_W = x.T.dot(diff)/self.n_features
-            self.W += - self.lr*grad_W
+            grad_W = x.T.dot(diff)/x.shape[0]
+            self.W += -self.lr*grad_W
             if self.bias:
-                grad_b = 2*np.sum(diff,keepdims=True)/self.n_features
+                grad_b = 2*np.sum(diff,keepdims=True)/x.shape[0]
                 self.b += - self.lr*grad_b
                 
-        print(f'{mse=}')
+        print(f'mse= {mse.item():.4f}')
+
+    def predict(self, x):
+        x = x.reshape(-1,self.n_features)
+        return x.dot(self.W) + self.b
 
     def calculate_mse(self, x, y):
         x = x.reshape(-1,self.n_features)
         y = y.reshape(-1,1)
         pred = x.dot(self.W) + self.b
         diff = pred - y
         square = diff.T.dot(diff)
-        mse = square/self.n_features
+        mse = square/x.shape[0]
         return mse
```

### Comparing `tinyfit-0.0.1/LICENSE` & `tinyfit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyfit-0.0.1/pyproject.toml` & `tinyfit-0.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["hatchling", "numpy"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tinyfit"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Morne van Wyk", email="morn.vanwyk@gmail.com" },
 ]
 description = "A small regression library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://example.com"
-Documentation = "https://readthedocs.org"
-Repository = "https://github.com/me/spam.git"
-Issues = "https://github.com/me/spam/issues"
-Changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
+Homepage = "https://github.com/mornevwyk/tinyfit"
+Documentation = "https://github.com/mornevwyk/tinyfit"
+Repository = "https://github.com/mornevwyk/tinyfit"
+Issues = "https://github.com/mornevwyk/tinyfit/issues"
+Changelog = "https://github.com/mornevwyk/tinyfit"
```

### Comparing `tinyfit-0.0.1/PKG-INFO` & `tinyfit-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: tinyfit
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small regression library
-Project-URL: Homepage, https://example.com
-Project-URL: Documentation, https://readthedocs.org
-Project-URL: Repository, https://github.com/me/spam.git
-Project-URL: Issues, https://github.com/me/spam/issues
-Project-URL: Changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
+Project-URL: Homepage, https://github.com/mornevwyk/tinyfit
+Project-URL: Documentation, https://github.com/mornevwyk/tinyfit
+Project-URL: Repository, https://github.com/mornevwyk/tinyfit
+Project-URL: Issues, https://github.com/mornevwyk/tinyfit/issues
+Project-URL: Changelog, https://github.com/mornevwyk/tinyfit
 Author-email: Morne van Wyk <morn.vanwyk@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

