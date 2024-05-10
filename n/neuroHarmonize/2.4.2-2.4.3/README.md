# Comparing `tmp/neuroharmonize-2.4.2.tar.gz` & `tmp/neuroharmonize-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroharmonize-2.4.2.tar", last modified: Mon May  6 20:12:17 2024, max compression
+gzip compressed data, was "neuroharmonize-2.4.3.tar", last modified: Fri May 10 12:57:00 2024, max compression
```

## Comparing `neuroharmonize-2.4.2.tar` & `neuroharmonize-2.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-06 20:12:17.963958 neuroharmonize-2.4.2/
--rw-r--r--   0 pomponior   (501) staff       (20)     1069 2024-02-01 14:00:43.000000 neuroharmonize-2.4.2/LICENSE
--rw-r--r--   0 pomponior   (501) staff       (20)       18 2024-04-23 17:14:29.000000 neuroharmonize-2.4.2/MANIFEST.in
--rw-r--r--   0 pomponior   (501) staff       (20)    10859 2024-05-06 20:12:17.963859 neuroharmonize-2.4.2/PKG-INFO
--rw-r--r--   0 pomponior   (501) staff       (20)    10301 2024-05-06 20:08:17.000000 neuroharmonize-2.4.2/README.md
--rw-r--r--   0 pomponior   (501) staff       (20)      104 2024-02-01 14:00:43.000000 neuroharmonize-2.4.2/pyproject.toml
--rw-r--r--   0 pomponior   (501) staff       (20)      683 2024-05-06 20:12:17.964233 neuroharmonize-2.4.2/setup.cfg
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-06 20:12:17.961604 neuroharmonize-2.4.2/src/
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-06 20:12:17.962997 neuroharmonize-2.4.2/src/neuroHarmonize/
--rw-r--r--   0 pomponior   (501) staff       (20)      219 2024-05-06 20:11:20.000000 neuroharmonize-2.4.2/src/neuroHarmonize/__init__.py
--rwxr-xr-x   0 pomponior   (501) staff       (20)     9135 2024-05-06 20:11:20.000000 neuroharmonize-2.4.2/src/neuroHarmonize/harmonizationApply.py
--rwxr-xr-x   0 pomponior   (501) staff       (20)    18851 2024-05-06 20:11:20.000000 neuroharmonize-2.4.2/src/neuroHarmonize/harmonizationLearn.py
--rw-r--r--   0 pomponior   (501) staff       (20)     6701 2024-05-06 20:11:20.000000 neuroharmonize-2.4.2/src/neuroHarmonize/harmonizationNIFTI.py
-drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-06 20:12:17.963680 neuroharmonize-2.4.2/src/neuroHarmonize.egg-info/
--rw-r--r--   0 pomponior   (501) staff       (20)    10859 2024-05-06 20:12:17.000000 neuroharmonize-2.4.2/src/neuroHarmonize.egg-info/PKG-INFO
--rw-r--r--   0 pomponior   (501) staff       (20)      376 2024-05-06 20:12:17.000000 neuroharmonize-2.4.2/src/neuroHarmonize.egg-info/SOURCES.txt
--rw-r--r--   0 pomponior   (501) staff       (20)        1 2024-05-06 20:12:17.000000 neuroharmonize-2.4.2/src/neuroHarmonize.egg-info/dependency_links.txt
--rw-r--r--   0 pomponior   (501) staff       (20)       15 2024-05-06 20:12:17.000000 neuroharmonize-2.4.2/src/neuroHarmonize.egg-info/top_level.txt
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-10 12:57:00.001329 neuroharmonize-2.4.3/
+-rw-r--r--   0 pomponior   (501) staff       (20)     1069 2024-02-01 14:00:43.000000 neuroharmonize-2.4.3/LICENSE
+-rw-r--r--   0 pomponior   (501) staff       (20)       18 2024-04-23 17:14:29.000000 neuroharmonize-2.4.3/MANIFEST.in
+-rw-r--r--   0 pomponior   (501) staff       (20)    10838 2024-05-10 12:57:00.001242 neuroharmonize-2.4.3/PKG-INFO
+-rw-r--r--   0 pomponior   (501) staff       (20)    10280 2024-05-10 12:48:25.000000 neuroharmonize-2.4.3/README.md
+-rw-r--r--   0 pomponior   (501) staff       (20)      104 2024-02-01 14:00:43.000000 neuroharmonize-2.4.3/pyproject.toml
+-rw-r--r--   0 pomponior   (501) staff       (20)      683 2024-05-10 12:57:00.001598 neuroharmonize-2.4.3/setup.cfg
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-10 12:56:59.999295 neuroharmonize-2.4.3/src/
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-10 12:57:00.000405 neuroharmonize-2.4.3/src/neuroHarmonize/
+-rw-r--r--   0 pomponior   (501) staff       (20)      219 2024-05-10 12:56:43.000000 neuroharmonize-2.4.3/src/neuroHarmonize/__init__.py
+-rwxr-xr-x   0 pomponior   (501) staff       (20)     9135 2024-05-10 12:56:43.000000 neuroharmonize-2.4.3/src/neuroHarmonize/harmonizationApply.py
+-rwxr-xr-x   0 pomponior   (501) staff       (20)    18873 2024-05-10 12:56:43.000000 neuroharmonize-2.4.3/src/neuroHarmonize/harmonizationLearn.py
+-rw-r--r--   0 pomponior   (501) staff       (20)     6701 2024-05-10 12:56:43.000000 neuroharmonize-2.4.3/src/neuroHarmonize/harmonizationNIFTI.py
+drwxr-xr-x   0 pomponior   (501) staff       (20)        0 2024-05-10 12:57:00.001052 neuroharmonize-2.4.3/src/neuroHarmonize.egg-info/
+-rw-r--r--   0 pomponior   (501) staff       (20)    10838 2024-05-10 12:56:59.000000 neuroharmonize-2.4.3/src/neuroHarmonize.egg-info/PKG-INFO
+-rw-r--r--   0 pomponior   (501) staff       (20)      376 2024-05-10 12:56:59.000000 neuroharmonize-2.4.3/src/neuroHarmonize.egg-info/SOURCES.txt
+-rw-r--r--   0 pomponior   (501) staff       (20)        1 2024-05-10 12:56:59.000000 neuroharmonize-2.4.3/src/neuroHarmonize.egg-info/dependency_links.txt
+-rw-r--r--   0 pomponior   (501) staff       (20)       15 2024-05-10 12:56:59.000000 neuroharmonize-2.4.3/src/neuroHarmonize.egg-info/top_level.txt
```

### Comparing `neuroharmonize-2.4.2/LICENSE` & `neuroharmonize-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroharmonize-2.4.2/PKG-INFO` & `neuroharmonize-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroHarmonize
-Version: 2.4.2
+Version: 2.4.3
 Summary: Harmonization tools for multi-center neuroimaging studies.
 Home-page: https://github.com/rpomponio/neuroHarmonize
 Author: Raymond Pomponio
 Author-email: raymond.pomponio@outlook.com
 Project-URL: Bug Tracker, https://github.com/rpomponio/neuroHarmonize/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,17 +19,15 @@
 reported in our paper with data from the ISTAGING consoritum [^1].
 
 contact: raymond (dot) pomponio (at) outlook (dot) com
 
 Overview
 ---------
 
-This package extends the functionality of the package developed by Jean-Philippe
-Fortin and Nick Cullen [^2], `neuroCombat`. **New in version 2.4.x:**
-`neuroCombat` is now a formal dependency for `neuroHarmonize`.
+This package extends the functionality of the package developed by Jean-Philippe Fortin and Nick Cullen [^2], `neuroCombat`. **New in version 2.4.x:** `neuroCombat` is now a formal dependency.
 
 The reference implementation, `neuroCombat`, allows the user to perform a
 harmonization procedure using the ComBat [^3] algorithm for correcting
 multi-site data.
 
 This package, `neuroHarmonize`, provides similar functionality, with
 additional features:
@@ -39,15 +37,15 @@
 3. Specify covariates with generic nonlinear effects. Implemented using
    Generalized Additive Models (GAMs) from the `statsmodels` package.
 4. Skip the empirical Bayes (EB) step of ComBat, if desired.
 
 Installation
 ------------
 
-Latest development version: `2.4.2` (May 2024)
+Latest development version: `2.4.3` (May 2024)
 
 Requirements:
 
 * `git >= 2.17.2`
 * `python >= 3.6.8`
 
 **Option 1: Install from PyPI (Stable Version)**
```

### Comparing `neuroharmonize-2.4.2/README.md` & `neuroharmonize-2.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 reported in our paper with data from the ISTAGING consoritum [^1].
 
 contact: raymond (dot) pomponio (at) outlook (dot) com
 
 Overview
 ---------
 
-This package extends the functionality of the package developed by Jean-Philippe
-Fortin and Nick Cullen [^2], `neuroCombat`. **New in version 2.4.x:**
-`neuroCombat` is now a formal dependency for `neuroHarmonize`.
+This package extends the functionality of the package developed by Jean-Philippe Fortin and Nick Cullen [^2], `neuroCombat`. **New in version 2.4.x:** `neuroCombat` is now a formal dependency.
 
 The reference implementation, `neuroCombat`, allows the user to perform a
 harmonization procedure using the ComBat [^3] algorithm for correcting
 multi-site data.
 
 This package, `neuroHarmonize`, provides similar functionality, with
 additional features:
@@ -24,15 +22,15 @@
 3. Specify covariates with generic nonlinear effects. Implemented using
    Generalized Additive Models (GAMs) from the `statsmodels` package.
 4. Skip the empirical Bayes (EB) step of ComBat, if desired.
 
 Installation
 ------------
 
-Latest development version: `2.4.2` (May 2024)
+Latest development version: `2.4.3` (May 2024)
 
 Requirements:
 
 * `git >= 2.17.2`
 * `python >= 3.6.8`
 
 **Option 1: Install from PyPI (Stable Version)**
```

### Comparing `neuroharmonize-2.4.2/setup.cfg` & `neuroharmonize-2.4.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = neuroHarmonize
-version = 2.4.2
+version = 2.4.3
 author = Raymond Pomponio
 author_email = raymond.pomponio@outlook.com
 description = Harmonization tools for multi-center neuroimaging studies.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rpomponio/neuroHarmonize
 project_urls =
```

### Comparing `neuroharmonize-2.4.2/src/neuroHarmonize/harmonizationApply.py` & `neuroharmonize-2.4.3/src/neuroHarmonize/harmonizationApply.py`

 * *Files identical despite different names*

### Comparing `neuroharmonize-2.4.2/src/neuroHarmonize/harmonizationLearn.py` & `neuroharmonize-2.4.3/src/neuroHarmonize/harmonizationLearn.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         By default, this function is non-deterministic. Setting the optional
         argument `seed` will make the function deterministic.
 
 
     Returns
     -------
     model : a dictionary of estimated model parameters
-        design, var_pooled, B_hat, grand_mean,
+        design, var_pooled, B_hat, stand_mean, mod_mean,
         gamma_star, delta_star, info_dict (a neuroCombat invention),
         gamma_hat, delta_hat, gamma_bar, t2, a_prior, b_prior, smooth_model
     
     bayes_data : a numpy array
         harmonized data, corrected for effects of SITE
         dimensions are N_samples x N_features
 
@@ -388,15 +388,15 @@
     by file_name, and store the model using the pickle package.
     
     """
     if os.path.exists(file_name):
         raise ValueError('Model file already exists: %s. Change name or delete to save.' % file_name)
     # estimate size of out_file
     est_size = 0
-    for key in ['design', 'B_hat', 'grand_mean', 'var_pooled',
+    for key in ['design', 'B_hat', 'stand_mean', 'mod_mean', 'var_pooled',
                 'gamma_star', 'delta_star', 'gamma_hat', 'delta_hat']:
         est_size += model[key].nbytes / 1e6
     print('\n[neuroHarmonize]: Saving model object, estimated size in MB: %4.2f' % est_size)
     out_file = open(file_name, 'wb')
     pickle.dump(model, out_file)
     out_file.close()
```

### Comparing `neuroharmonize-2.4.2/src/neuroHarmonize/harmonizationNIFTI.py` & `neuroharmonize-2.4.3/src/neuroHarmonize/harmonizationNIFTI.py`

 * *Files identical despite different names*

### Comparing `neuroharmonize-2.4.2/src/neuroHarmonize.egg-info/PKG-INFO` & `neuroharmonize-2.4.3/src/neuroHarmonize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroHarmonize
-Version: 2.4.2
+Version: 2.4.3
 Summary: Harmonization tools for multi-center neuroimaging studies.
 Home-page: https://github.com/rpomponio/neuroHarmonize
 Author: Raymond Pomponio
 Author-email: raymond.pomponio@outlook.com
 Project-URL: Bug Tracker, https://github.com/rpomponio/neuroHarmonize/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,17 +19,15 @@
 reported in our paper with data from the ISTAGING consoritum [^1].
 
 contact: raymond (dot) pomponio (at) outlook (dot) com
 
 Overview
 ---------
 
-This package extends the functionality of the package developed by Jean-Philippe
-Fortin and Nick Cullen [^2], `neuroCombat`. **New in version 2.4.x:**
-`neuroCombat` is now a formal dependency for `neuroHarmonize`.
+This package extends the functionality of the package developed by Jean-Philippe Fortin and Nick Cullen [^2], `neuroCombat`. **New in version 2.4.x:** `neuroCombat` is now a formal dependency.
 
 The reference implementation, `neuroCombat`, allows the user to perform a
 harmonization procedure using the ComBat [^3] algorithm for correcting
 multi-site data.
 
 This package, `neuroHarmonize`, provides similar functionality, with
 additional features:
@@ -39,15 +37,15 @@
 3. Specify covariates with generic nonlinear effects. Implemented using
    Generalized Additive Models (GAMs) from the `statsmodels` package.
 4. Skip the empirical Bayes (EB) step of ComBat, if desired.
 
 Installation
 ------------
 
-Latest development version: `2.4.2` (May 2024)
+Latest development version: `2.4.3` (May 2024)
 
 Requirements:
 
 * `git >= 2.17.2`
 * `python >= 3.6.8`
 
 **Option 1: Install from PyPI (Stable Version)**
```

