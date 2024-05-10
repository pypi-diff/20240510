# Comparing `tmp/mecode_viewer-0.3.8.tar.gz` & `tmp/mecode_viewer-0.3.9.tar.gz`

## Comparing `mecode_viewer-0.3.8.tar` & `mecode_viewer-0.3.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 mecode_viewer-0.3.8/mecode_viewer/__init__.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 mecode_viewer-0.3.8/mecode_viewer/cli.py
--rw-r--r--   0        0        0    38958 2020-02-02 00:00:00.000000 mecode_viewer-0.3.8/mecode_viewer/mecode_viewer.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 mecode_viewer-0.3.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mecode_viewer-0.3.8/LICENSE
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 mecode_viewer-0.3.8/README.md
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mecode_viewer-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 mecode_viewer-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 mecode_viewer-0.3.9/mecode_viewer/__init__.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 mecode_viewer-0.3.9/mecode_viewer/cli.py
+-rw-r--r--   0        0        0    39048 2020-02-02 00:00:00.000000 mecode_viewer-0.3.9/mecode_viewer/mecode_viewer.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 mecode_viewer-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 mecode_viewer-0.3.9/LICENSE
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 mecode_viewer-0.3.9/README.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mecode_viewer-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 mecode_viewer-0.3.9/PKG-INFO
```

### Comparing `mecode_viewer-0.3.8/mecode_viewer/mecode_viewer.py` & `mecode_viewer-0.3.9/mecode_viewer/mecode_viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -831,25 +831,27 @@
                     color_history.append(colors[0])
                 elif h['COLOR'] is not None:
                     color_history.append(h['COLOR'])
                 else:
                     color_history.append((1,0,0)) 
             elif len(keys) == 2:
                 ratio = h['PRINTING'][keys[0]]['value'] / (h['PRINTING'][keys[0]]['value'] + h['PRINTING'][keys[1]]['value'])
+                ratio = 0 if np.isnan(ratio) else ratio
+                
                 if colors is not None:
                     if h['PRINTING'][keys[0]]['printing'] and not h['PRINTING'][keys[1]]['printing']:
                         color_history.append(colors[0])
                     elif not h['PRINTING'][keys[0]]['printing'] and h['PRINTING'][keys[1]]['printing']:
                         color_history.append(colors[1])
                     else:
                         color_1 = colors[0]
                         color_2 = colors[1]
                         gradient_cmap = create_linear_gradient_colormap(color_1, color_2)
                         color_history.append(gradient_cmap(int(ratio * gradient_cmap.N)))
-                elif h['COLOR'] is not None:
+                elif 'COLOR' in h and h['COLOR'] is not None:
                     color_history.append(h['COLOR'])
                 else:
                     color_1 = (1,0,0)
                     color_2 = (0,0,1)
                     gradient_cmap = create_linear_gradient_colormap(color_1, color_2)
                     color_history.append(gradient_cmap(int(ratio * gradient_cmap.N)))
             elif len(keys) > 2:
```

### Comparing `mecode_viewer-0.3.8/.gitignore` & `mecode_viewer-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.3.8/LICENSE` & `mecode_viewer-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.3.8/README.md` & `mecode_viewer-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.3.8/pyproject.toml` & `mecode_viewer-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.3.8/PKG-INFO` & `mecode_viewer-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecode-viewer
-Version: 0.3.8
+Version: 0.3.9
 Summary: Simple GCode Viewer
 Project-URL: Homepage, https://github.com/rtellez700/mecode_viewer
 Author-email: Rodrigo Telles <rtelles@g.harvard.edu>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: mecode_viewer
 Classifier: Development Status :: 2 - Pre-Alpha
```

