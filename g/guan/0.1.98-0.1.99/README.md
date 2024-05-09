# Comparing `tmp/guan-0.1.98.tar.gz` & `tmp/guan-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guan-0.1.98.tar", last modified: Wed May  8 21:21:38 2024, max compression
+gzip compressed data, was "guan-0.1.99.tar", last modified: Thu May  9 21:58:48 2024, max compression
```

## Comparing `guan-0.1.98.tar` & `guan-0.1.99.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 21:21:38.012875 guan-0.1.98/
--rw-rw-rw-   0        0        0    35821 2021-07-19 21:39:06.000000 guan-0.1.98/LICENSE
--rw-rw-rw-   0        0        0      798 2024-05-08 21:21:38.012875 guan-0.1.98/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-11-04 17:18:16.000000 guan-0.1.98/README.md
--rw-rw-rw-   0        0        0      108 2021-05-22 13:59:00.000000 guan-0.1.98/pyproject.toml
--rw-rw-rw-   0        0        0      641 2024-05-08 21:21:38.025410 guan-0.1.98/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 21:21:37.848793 guan-0.1.98/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 21:21:37.992855 guan-0.1.98/src/guan/
--rw-rw-rw-   0        0        0     5294 2024-02-22 19:01:32.000000 guan-0.1.98/src/guan/Fourier_transform.py
--rw-rw-rw-   0        0        0     6769 2024-05-07 14:06:47.000000 guan-0.1.98/src/guan/Green_functions.py
--rw-rw-rw-   0        0        0    24114 2024-02-22 19:01:51.000000 guan-0.1.98/src/guan/Hamiltonian_of_examples.py
--rw-rw-rw-   0        0        0      811 2024-02-22 19:43:08.000000 guan-0.1.98/src/guan/__init__.py
--rw-rw-rw-   0        0        0    10438 2024-02-22 18:58:28.000000 guan-0.1.98/src/guan/band_structures_and_wave_functions.py
--rw-rw-rw-   0        0        0     2388 2024-02-22 19:00:04.000000 guan-0.1.98/src/guan/basic_functions.py
--rw-rw-rw-   0        0        0     4809 2024-05-07 14:16:28.000000 guan-0.1.98/src/guan/data_processing.py
--rw-rw-rw-   0        0        0     1398 2024-02-22 19:14:25.000000 guan-0.1.98/src/guan/decorators.py
--rw-rw-rw-   0        0        0    10300 2024-02-22 19:01:02.000000 guan-0.1.98/src/guan/density_of_states.py
--rw-rw-rw-   0        0        0    21680 2024-02-22 19:01:14.000000 guan-0.1.98/src/guan/figure_plotting.py
--rw-rw-rw-   0        0        0    12813 2024-02-28 01:45:12.000000 guan-0.1.98/src/guan/file_reading_and_writing.py
--rw-rw-rw-   0        0        0    14014 2024-04-10 14:29:46.000000 guan-0.1.98/src/guan/machine_learning.py
--rw-rw-rw-   0        0        0    41346 2024-03-12 18:43:39.000000 guan-0.1.98/src/guan/others.py
--rw-rw-rw-   0        0        0    43385 2024-05-08 21:20:46.000000 guan-0.1.98/src/guan/quantum_transport.py
--rw-rw-rw-   0        0        0    27324 2024-02-22 19:02:31.000000 guan-0.1.98/src/guan/topological_invariant.py
-drwxrwxrwx   0        0        0        0 2024-05-08 21:21:38.012875 guan-0.1.98/src/guan.egg-info/
--rw-rw-rw-   0        0        0      798 2024-05-08 21:21:37.000000 guan-0.1.98/src/guan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      618 2024-05-08 21:21:37.000000 guan-0.1.98/src/guan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 21:21:37.000000 guan-0.1.98/src/guan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-08 21:21:37.000000 guan-0.1.98/src/guan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 21:58:48.822169 guan-0.1.99/
+-rw-rw-rw-   0        0        0    35821 2021-07-19 21:39:06.000000 guan-0.1.99/LICENSE
+-rw-rw-rw-   0        0        0      798 2024-05-09 21:58:48.822169 guan-0.1.99/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-11-04 17:18:16.000000 guan-0.1.99/README.md
+-rw-rw-rw-   0        0        0      108 2021-05-22 13:59:00.000000 guan-0.1.99/pyproject.toml
+-rw-rw-rw-   0        0        0      641 2024-05-09 21:58:48.825140 guan-0.1.99/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 21:58:48.678220 guan-0.1.99/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 21:58:48.800669 guan-0.1.99/src/guan/
+-rw-rw-rw-   0        0        0     5294 2024-02-22 19:01:32.000000 guan-0.1.99/src/guan/Fourier_transform.py
+-rw-rw-rw-   0        0        0     6769 2024-05-07 14:06:47.000000 guan-0.1.99/src/guan/Green_functions.py
+-rw-rw-rw-   0        0        0    24114 2024-02-22 19:01:51.000000 guan-0.1.99/src/guan/Hamiltonian_of_examples.py
+-rw-rw-rw-   0        0        0      811 2024-02-22 19:43:08.000000 guan-0.1.99/src/guan/__init__.py
+-rw-rw-rw-   0        0        0    10438 2024-02-22 18:58:28.000000 guan-0.1.99/src/guan/band_structures_and_wave_functions.py
+-rw-rw-rw-   0        0        0     2388 2024-02-22 19:00:04.000000 guan-0.1.99/src/guan/basic_functions.py
+-rw-rw-rw-   0        0        0     4809 2024-05-07 14:16:28.000000 guan-0.1.99/src/guan/data_processing.py
+-rw-rw-rw-   0        0        0     1398 2024-02-22 19:14:25.000000 guan-0.1.99/src/guan/decorators.py
+-rw-rw-rw-   0        0        0    10300 2024-02-22 19:01:02.000000 guan-0.1.99/src/guan/density_of_states.py
+-rw-rw-rw-   0        0        0    21680 2024-02-22 19:01:14.000000 guan-0.1.99/src/guan/figure_plotting.py
+-rw-rw-rw-   0        0        0    12813 2024-02-28 01:45:12.000000 guan-0.1.99/src/guan/file_reading_and_writing.py
+-rw-rw-rw-   0        0        0    15598 2024-05-09 21:57:30.000000 guan-0.1.99/src/guan/machine_learning.py
+-rw-rw-rw-   0        0        0    41346 2024-03-12 18:43:39.000000 guan-0.1.99/src/guan/others.py
+-rw-rw-rw-   0        0        0    43385 2024-05-08 21:20:46.000000 guan-0.1.99/src/guan/quantum_transport.py
+-rw-rw-rw-   0        0        0    27324 2024-02-22 19:02:31.000000 guan-0.1.99/src/guan/topological_invariant.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:58:48.821161 guan-0.1.99/src/guan.egg-info/
+-rw-rw-rw-   0        0        0      798 2024-05-09 21:58:48.000000 guan-0.1.99/src/guan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      618 2024-05-09 21:58:48.000000 guan-0.1.99/src/guan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 21:58:48.000000 guan-0.1.99/src/guan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-09 21:58:48.000000 guan-0.1.99/src/guan.egg-info/top_level.txt
```

### Comparing `guan-0.1.98/LICENSE` & `guan-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/PKG-INFO` & `guan-0.1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guan
-Version: 0.1.98
+Version: 0.1.99
 Summary: An open source python package
 Home-page: https://py.guanjihuan.com
 Author: guanjihuan
 Author-email: guanjihuan@163.com
 Project-URL: Bug Tracker, https://py.guanjihuan.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `guan-0.1.98/setup.cfg` & `guan-0.1.99/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 7561 6e0d 0a76 6572 7369 6f6e   = guan..version
-00000020: 203d 2030 2e31 2e39 380d 0a61 7574 686f   = 0.1.98..autho
+00000020: 203d 2030 2e31 2e39 390d 0a61 7574 686f   = 0.1.99..autho
 00000030: 7220 3d20 6775 616e 6a69 6875 616e 0d0a  r = guanjihuan..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2067  author_email = g
 00000050: 7561 6e6a 6968 7561 6e40 3136 332e 636f  uanjihuan@163.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 2041 6e20 6f70 656e 2073 6f75 7263 6520   An open source 
 00000080: 7079 7468 6f6e 2070 6163 6b61 6765 0d0a  python package..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
```

### Comparing `guan-0.1.98/src/guan/Fourier_transform.py` & `guan-0.1.99/src/guan/Fourier_transform.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan/Green_functions.py` & `guan-0.1.99/src/guan/Green_functions.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan/Hamiltonian_of_examples.py` & `guan-0.1.99/src/guan/Hamiltonian_of_examples.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan/__init__.py` & `guan-0.1.99/src/guan/__init__.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan/band_structures_and_wave_functions.py` & `guan-0.1.99/src/guan/band_structures_and_wave_functions.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan/basic_functions.py` & `guan-0.1.99/src/guan/basic_functions.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan/data_processing.py` & `guan-0.1.99/src/guan/data_processing.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan/decorators.py` & `guan-0.1.99/src/guan/decorators.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan/density_of_states.py` & `guan-0.1.99/src/guan/density_of_states.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan/figure_plotting.py` & `guan-0.1.99/src/guan/figure_plotting.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan/file_reading_and_writing.py` & `guan-0.1.99/src/guan/file_reading_and_writing.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan/machine_learning.py` & `guan-0.1.99/src/guan/machine_learning.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,18 @@
                 hidden_output = torch.nn.functional.relu(self.hidden_layer(x))
             elif activation == 'leaky_relu':
                 hidden_output = torch.nn.functional.leaky_relu(self.hidden_layer(x))
             elif activation == 'sigmoid':
                 hidden_output = torch.nn.functional.sigmoid(self.hidden_layer(x))
             elif activation == 'tanh':
                 hidden_output = torch.nn.functional.tanh(self.hidden_layer(x))
+            elif activation == 'gelu':
+                hidden_output = torch.nn.functional.gelu(self.hidden_layer(x))
+            elif activation == 'silu':
+                hidden_output = torch.nn.functional.silu(self.hidden_layer(x))
             else:
                 hidden_output = self.hidden_layer(x)
             output = self.output_layer(hidden_output)
             return output
     model = model_class_of_fully_connected_neural_network_with_one_hidden_layer()
     return model
 
@@ -40,25 +44,33 @@
                 hidden_output_1 = torch.nn.functional.relu(self.hidden_layer_1(x))
             elif activation_1 == 'leaky_relu':
                 hidden_output_1 = torch.nn.functional.leaky_relu(self.hidden_layer_1(x))
             elif activation_1 == 'sigmoid':
                 hidden_output_1 = torch.nn.functional.sigmoid(self.hidden_layer_1(x))
             elif activation_1 == 'tanh':
                 hidden_output_1 = torch.nn.functional.tanh(self.hidden_layer_1(x))
+            elif activation_1 == 'gelu':
+                hidden_output_1 = torch.nn.functional.gelu(self.hidden_layer_1(x))
+            elif activation_1 == 'silu':
+                hidden_output_1 = torch.nn.functional.silu(self.hidden_layer_1(x))
             else:
                 hidden_output_1 = self.hidden_layer_1(x)
             
             if activation_2 == 'relu':
                 hidden_output_2 = torch.nn.functional.relu(self.hidden_layer_2(hidden_output_1))
             elif activation_2 == 'leaky_relu':
                 hidden_output_2 = torch.nn.functional.leaky_relu(self.hidden_layer_2(hidden_output_1))
             elif activation_2 == 'sigmoid':
                 hidden_output_2 = torch.nn.functional.sigmoid(self.hidden_layer_2(hidden_output_1))
             elif activation_2 == 'tanh':
                 hidden_output_2 = torch.nn.functional.tanh(self.hidden_layer_2(hidden_output_1))
+            elif activation_2 == 'gelu':
+                hidden_output_2 = torch.nn.functional.gelu(self.hidden_layer_2(hidden_output_1))
+            elif activation_2 == 'silu':
+                hidden_output_2 = torch.nn.functional.silu(self.hidden_layer_2(hidden_output_1))
             else:
                 hidden_output_2 = self.hidden_layer_2(hidden_output_1)
             
             output = self.output_layer(hidden_output_2)
             return output
     model = model_class_of_fully_connected_neural_network_with_two_hidden_layers()
     return model
@@ -79,36 +91,48 @@
                 hidden_output_1 = torch.nn.functional.relu(self.hidden_layer_1(x))
             elif activation_1 == 'leaky_relu':
                 hidden_output_1 = torch.nn.functional.leaky_relu(self.hidden_layer_1(x))
             elif activation_1 == 'sigmoid':
                 hidden_output_1 = torch.nn.functional.sigmoid(self.hidden_layer_1(x))
             elif activation_1 == 'tanh':
                 hidden_output_1 = torch.nn.functional.tanh(self.hidden_layer_1(x))
+            elif activation_1 == 'gelu':
+                hidden_output_1 = torch.nn.functional.gelu(self.hidden_layer_1(x))
+            elif activation_1 == 'silu':
+                hidden_output_1 = torch.nn.functional.silu(self.hidden_layer_1(x))
             else:
                 hidden_output_1 = self.hidden_layer_1(x)
             
             if activation_2 == 'relu':
                 hidden_output_2 = torch.nn.functional.relu(self.hidden_layer_2(hidden_output_1))
             elif activation_2 == 'leaky_relu':
                 hidden_output_2 = torch.nn.functional.leaky_relu(self.hidden_layer_2(hidden_output_1))
             elif activation_2 == 'sigmoid':
                 hidden_output_2 = torch.nn.functional.sigmoid(self.hidden_layer_2(hidden_output_1))
             elif activation_2 == 'tanh':
                 hidden_output_2 = torch.nn.functional.tanh(self.hidden_layer_2(hidden_output_1))
+            elif activation_2 == 'gelu':
+                hidden_output_2 = torch.nn.functional.gelu(self.hidden_layer_2(hidden_output_1))
+            elif activation_2 == 'silu':
+                hidden_output_2 = torch.nn.functional.silu(self.hidden_layer_2(hidden_output_1))
             else:
                 hidden_output_2 = self.hidden_layer_2(hidden_output_1)
 
             if activation_3 == 'relu':
                 hidden_output_3 = torch.nn.functional.relu(self.hidden_layer_3(hidden_output_2))
             elif activation_3 == 'leaky_relu':
                 hidden_output_3 = torch.nn.functional.leaky_relu(self.hidden_layer_3(hidden_output_2))
             elif activation_3 == 'sigmoid':
                 hidden_output_3 = torch.nn.functional.sigmoid(self.hidden_layer_3(hidden_output_2))
             elif activation_3 == 'tanh':
                 hidden_output_3 = torch.nn.functional.tanh(self.hidden_layer_3(hidden_output_2))
+            elif activation_3 == 'gelu':
+                hidden_output_3 = torch.nn.functional.gelu(self.hidden_layer_3(hidden_output_2))
+            elif activation_3 == 'silu':
+                hidden_output_3 = torch.nn.functional.silu(self.hidden_layer_3(hidden_output_2))
             else:
                 hidden_output_3 = self.hidden_layer_3(hidden_output_2)
             
             output = self.output_layer(hidden_output_3)
             return output
     model = model_class_of_fully_connected_neural_network_with_three_hidden_layers()
     return model
```

### Comparing `guan-0.1.98/src/guan/others.py` & `guan-0.1.99/src/guan/others.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan/quantum_transport.py` & `guan-0.1.99/src/guan/quantum_transport.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan/topological_invariant.py` & `guan-0.1.99/src/guan/topological_invariant.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.98/src/guan.egg-info/PKG-INFO` & `guan-0.1.99/src/guan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guan
-Version: 0.1.98
+Version: 0.1.99
 Summary: An open source python package
 Home-page: https://py.guanjihuan.com
 Author: guanjihuan
 Author-email: guanjihuan@163.com
 Project-URL: Bug Tracker, https://py.guanjihuan.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `guan-0.1.98/src/guan.egg-info/SOURCES.txt` & `guan-0.1.99/src/guan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

