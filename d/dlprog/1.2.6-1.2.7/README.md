# Comparing `tmp/dlprog-1.2.6.tar.gz` & `tmp/dlprog-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlprog-1.2.6.tar", last modified: Thu Jan 18 05:18:18 2024, max compression
+gzip compressed data, was "dlprog-1.2.7.tar", last modified: Fri May 10 06:22:05 2024, max compression
```

## Comparing `dlprog-1.2.6.tar` & `dlprog-1.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 komiya     (501) staff       (20)        0 2024-01-18 05:18:18.952621 dlprog-1.2.6/
--rw-r--r--   0 komiya     (501) staff       (20)     1091 2023-07-12 16:15:21.000000 dlprog-1.2.6/LICENSE
--rw-r--r--   0 komiya     (501) staff       (20)     8201 2024-01-18 05:18:18.952532 dlprog-1.2.6/PKG-INFO
--rw-r--r--   0 komiya     (501) staff       (20)     7534 2024-01-18 05:18:00.000000 dlprog-1.2.6/README.md
-drwxr-xr-x   0 komiya     (501) staff       (20)        0 2024-01-18 05:18:18.951801 dlprog-1.2.6/dlprog/
--rw-r--r--   0 komiya     (501) staff       (20)      123 2024-01-18 05:18:00.000000 dlprog-1.2.6/dlprog/__init__.py
--rw-r--r--   0 komiya     (501) staff       (20)    16707 2024-01-17 07:17:09.000000 dlprog-1.2.6/dlprog/progress.py
--rw-r--r--   0 komiya     (501) staff       (20)      748 2024-01-18 05:18:00.000000 dlprog-1.2.6/dlprog/utils.py
-drwxr-xr-x   0 komiya     (501) staff       (20)        0 2024-01-18 05:18:18.952298 dlprog-1.2.6/dlprog.egg-info/
--rw-r--r--   0 komiya     (501) staff       (20)     8201 2024-01-18 05:18:18.000000 dlprog-1.2.6/dlprog.egg-info/PKG-INFO
--rw-r--r--   0 komiya     (501) staff       (20)      210 2024-01-18 05:18:18.000000 dlprog-1.2.6/dlprog.egg-info/SOURCES.txt
--rw-r--r--   0 komiya     (501) staff       (20)        1 2024-01-18 05:18:18.000000 dlprog-1.2.6/dlprog.egg-info/dependency_links.txt
--rw-r--r--   0 komiya     (501) staff       (20)        7 2024-01-18 05:18:18.000000 dlprog-1.2.6/dlprog.egg-info/top_level.txt
--rw-r--r--   0 komiya     (501) staff       (20)       85 2024-01-18 05:18:18.952816 dlprog-1.2.6/setup.cfg
--rw-r--r--   0 komiya     (501) staff       (20)      912 2023-07-12 16:19:33.000000 dlprog-1.2.6/setup.py
+drwxr-xr-x   0 komiya     (501) staff       (20)        0 2024-05-10 06:22:05.548375 dlprog-1.2.7/
+-rw-r--r--   0 komiya     (501) staff       (20)     1091 2023-07-12 16:15:21.000000 dlprog-1.2.7/LICENSE
+-rw-r--r--   0 komiya     (501) staff       (20)     8326 2024-05-10 06:22:05.548242 dlprog-1.2.7/PKG-INFO
+-rw-r--r--   0 komiya     (501) staff       (20)     7659 2024-05-10 06:21:20.000000 dlprog-1.2.7/README.md
+drwxr-xr-x   0 komiya     (501) staff       (20)        0 2024-05-10 06:22:05.547412 dlprog-1.2.7/dlprog/
+-rw-r--r--   0 komiya     (501) staff       (20)      123 2024-05-10 06:21:20.000000 dlprog-1.2.7/dlprog/__init__.py
+-rw-r--r--   0 komiya     (501) staff       (20)    17627 2024-05-10 06:21:20.000000 dlprog-1.2.7/dlprog/progress.py
+-rw-r--r--   0 komiya     (501) staff       (20)      748 2024-05-10 04:34:19.000000 dlprog-1.2.7/dlprog/utils.py
+drwxr-xr-x   0 komiya     (501) staff       (20)        0 2024-05-10 06:22:05.548002 dlprog-1.2.7/dlprog.egg-info/
+-rw-r--r--   0 komiya     (501) staff       (20)     8326 2024-05-10 06:22:05.000000 dlprog-1.2.7/dlprog.egg-info/PKG-INFO
+-rw-r--r--   0 komiya     (501) staff       (20)      210 2024-05-10 06:22:05.000000 dlprog-1.2.7/dlprog.egg-info/SOURCES.txt
+-rw-r--r--   0 komiya     (501) staff       (20)        1 2024-05-10 06:22:05.000000 dlprog-1.2.7/dlprog.egg-info/dependency_links.txt
+-rw-r--r--   0 komiya     (501) staff       (20)        7 2024-05-10 06:22:05.000000 dlprog-1.2.7/dlprog.egg-info/top_level.txt
+-rw-r--r--   0 komiya     (501) staff       (20)       85 2024-05-10 06:22:05.548570 dlprog-1.2.7/setup.cfg
+-rw-r--r--   0 komiya     (501) staff       (20)      912 2023-07-12 16:19:33.000000 dlprog-1.2.7/setup.py
```

### Comparing `dlprog-1.2.6/LICENSE` & `dlprog-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dlprog-1.2.6/PKG-INFO` & `dlprog-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlprog
-Version: 1.2.6
+Version: 1.2.7
 Summary: A progress bar that aggregates the values of each iteration.
 Home-page: https://github.com/misya11p/dlprog
 Author: misya11p
 License: MIT
 Project-URL: Repository, https://github.com/misya11p/dlprog
 Keywords: iterator progress bar aggregate deep-learning machine-learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -303,10 +303,14 @@
 - Fix bug that argument `width` is not available when `with_test=True` in `train_progress()`.
 
 ### [1.2.5](https://pypi.org/project/dlprog/1.2.5/) (2024-01-17)
 
 - Add `get_all_values()` method.
 - Add `get_all_times()` method.
 
-### [1.2.6](https://pypi.org/project/dlprog/1.2.6/) (2024-01-18, Latest)
+### [1.2.6](https://pypi.org/project/dlprog/1.2.6/) (2024-01-18)
 
 - Fix bug that the time (minutes) is not displayed correctly.
+
+### [1.2.7](https://pypi.org/project/dlprog/1.2.7/) (2024-05-10, Latest)
+
+- Add `store_all_values` and `store_all_times` arguments.
```

### Comparing `dlprog-1.2.6/README.md` & `dlprog-1.2.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -285,10 +285,14 @@
 - Fix bug that argument `width` is not available when `with_test=True` in `train_progress()`.
 
 ### [1.2.5](https://pypi.org/project/dlprog/1.2.5/) (2024-01-17)
 
 - Add `get_all_values()` method.
 - Add `get_all_times()` method.
 
-### [1.2.6](https://pypi.org/project/dlprog/1.2.6/) (2024-01-18, Latest)
+### [1.2.6](https://pypi.org/project/dlprog/1.2.6/) (2024-01-18)
 
 - Fix bug that the time (minutes) is not displayed correctly.
+
+### [1.2.7](https://pypi.org/project/dlprog/1.2.7/) (2024-05-10, Latest)
+
+- Add `store_all_values` and `store_all_times` arguments.
```

### Comparing `dlprog-1.2.6/dlprog/progress.py` & `dlprog-1.2.7/dlprog/progress.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .utils import time_format, value_format
 import time
-from typing import Optional, Union, Callable, List, Dict
+from typing import Optional, Union, Callable, List
 import warnings
 
 
 Number = Union[int, float]
 Numbers = Union[Number, List[Number]]
 
 
@@ -22,14 +22,16 @@
         defer: bool = False,
         note: str = "",
         symbol: str = "#",
         round: int = 5,
         sep_label: str = ": ",
         sep_values: str = ", ",
         sep_note: str = ", ",
+        store_all_values: bool = True,
+        store_all_times: bool = True,
     ):
         """
         Progress bar class.
         When the following attributes are None, the progress bar is not 
         displayed correctly.
         Attributes defined in this constructor will be default values.
 
@@ -70,14 +72,20 @@
             sep_label (str):
                 Separator character for value and label.
                 Defaults to ': '.
             sep_values (str):
                 Separator character for values. Defaults to ', '.
             sep_note (str):
                 Separator character for note. Defaults to ', '.
+            store_all_values (bool):
+                If True, store values of all iterations. Set to False if
+                you want to reduce memory usage. Defaults to True.
+            store_all_times (bool):
+                If True, store times of all iterations. Set to False if
+                you want to reduce memory usage. Defaults to True.
         """
         self._defaults = {
             "n_iter": n_iter,
             "n_epochs": n_epochs,
             "label": label,
             "n_values": n_values,
             "agg_fn": agg_fn,
@@ -87,14 +95,16 @@
             "defer": defer,
             "note": note,
             "symbol": symbol,
             "round": round,
             "sep_label": sep_label,
             "sep_values": sep_values,
             "sep_note": sep_note,
+            "store_all_values": store_all_values,
+            "store_all_times": store_all_times,
         }
         self.reset()
 
     _agg_fns = {
         "mean": lambda s, w: s / w,
         "sum": lambda s, w: s,
     }
@@ -238,15 +248,15 @@
                 Separator character for note. Defaults to ', '.
         """
         self.reset(**kwargs)
         assert self.n_iter is not None, "'n_iter' is not set."
         if ("label" not in kwargs) and (self.label is None) \
                 and ("labels" in kwargs):
             warnings.warn(
-                "'labels' is not a valid argument."
+                "'labels' is not a valid argument. "
                 "Try using 'label' instead.",
             )
         self.is_running = True
         self.now_epoch = 1
         self.n_bar = 1
         self._keep_step = False
         self._bar_note = self.note
@@ -334,16 +344,20 @@
         if not self.is_running:
             self.start()
         self._update_values(advance, value, weight)
         self.prop = self.now_iter / self.n_iter
         if note is not None:
             self._bar_note = note
         self._draw()
-        self._epoch_all_values.append(value)
-        self._epoch_all_times.append(self.now_time - self._tmp_time)
+
+        if self.store_all_values:
+            self._epoch_all_values.append(value)
+        if self.store_all_times:
+            self._epoch_all_times.append(self.now_time - self._tmp_time)
+
         self._tmp_time = self.now_time
         if auto_step and self.prop >= 1.:
             bar_step = self._bar_prop >= 1.
             leave = not (self.n_bar % self.leave_freq)
             leave = self.leave_freq > 0 and leave
             if self.defer:
                 self._keep_step = True
@@ -376,16 +390,24 @@
         self.values.append(value)
         self.now_epoch += 1
         self._epoch_reset()
         self._keep_step = False
 
     def _get_data(self, data: str, flatten: bool = False):
         if data == "value":
+            if not self.store_all_values:
+                warnings.warn(
+                    "store_all_values is False. No values are stored."
+                )
             data = self._all_values
         elif data == "time":
+            if not self.store_all_times:
+                warnings.warn(
+                    "store_all_times is False. No times are stored."
+                )
             data = self._all_times
         data = [epoch for epoch in data if epoch]
         if flatten:
             return [v for epoch in data for v in epoch]
         else:
             return data
```

### Comparing `dlprog-1.2.6/dlprog/utils.py` & `dlprog-1.2.7/dlprog/utils.py`

 * *Files identical despite different names*

### Comparing `dlprog-1.2.6/dlprog.egg-info/PKG-INFO` & `dlprog-1.2.7/dlprog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlprog
-Version: 1.2.6
+Version: 1.2.7
 Summary: A progress bar that aggregates the values of each iteration.
 Home-page: https://github.com/misya11p/dlprog
 Author: misya11p
 License: MIT
 Project-URL: Repository, https://github.com/misya11p/dlprog
 Keywords: iterator progress bar aggregate deep-learning machine-learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -303,10 +303,14 @@
 - Fix bug that argument `width` is not available when `with_test=True` in `train_progress()`.
 
 ### [1.2.5](https://pypi.org/project/dlprog/1.2.5/) (2024-01-17)
 
 - Add `get_all_values()` method.
 - Add `get_all_times()` method.
 
-### [1.2.6](https://pypi.org/project/dlprog/1.2.6/) (2024-01-18, Latest)
+### [1.2.6](https://pypi.org/project/dlprog/1.2.6/) (2024-01-18)
 
 - Fix bug that the time (minutes) is not displayed correctly.
+
+### [1.2.7](https://pypi.org/project/dlprog/1.2.7/) (2024-05-10, Latest)
+
+- Add `store_all_values` and `store_all_times` arguments.
```

### Comparing `dlprog-1.2.6/setup.py` & `dlprog-1.2.7/setup.py`

 * *Files identical despite different names*

