# Comparing `tmp/rotop-1.0.4.tar.gz` & `tmp/rotop-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotop-1.0.4.tar", last modified: Fri Dec 15 07:41:43 2023, max compression
+gzip compressed data, was "rotop-1.0.5.tar", last modified: Fri May 10 10:08:22 2024, max compression
```

## Comparing `rotop-1.0.4.tar` & `rotop-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 07:41:43.603783 rotop-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 07:41:43.595784 rotop-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 07:41:43.599784 rotop-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2023-12-15 07:41:33.000000 rotop-1.0.4/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-12-15 07:41:33.000000 rotop-1.0.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 07:41:43.599784 rotop-1.0.4/00_doc/
--rw-r--r--   0 runner    (1001) docker     (127)   394789 2023-12-15 07:41:33.000000 rotop-1.0.4/00_doc/capture_00.png
--rw-r--r--   0 runner    (1001) docker     (127)   746799 2023-12-15 07:41:33.000000 rotop-1.0.4/00_doc/capture_01.png
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-15 07:41:33.000000 rotop-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2023-12-15 07:41:43.603783 rotop-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-12-15 07:41:33.000000 rotop-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-12-15 07:41:33.000000 rotop-1.0.4/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2023-12-15 07:41:33.000000 rotop-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-15 07:41:33.000000 rotop-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-15 07:41:43.603783 rotop-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 07:41:43.595784 rotop-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 07:41:43.599784 rotop-1.0.4/src/rotop/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-12-15 07:41:33.000000 rotop-1.0.4/src/rotop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-15 07:41:33.000000 rotop-1.0.4/src/rotop/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-15 07:41:43.000000 rotop-1.0.4/src/rotop/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2023-12-15 07:41:33.000000 rotop-1.0.4/src/rotop/data_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2023-12-15 07:41:33.000000 rotop-1.0.4/src/rotop/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2023-12-15 07:41:33.000000 rotop-1.0.4/src/rotop/rotop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2023-12-15 07:41:33.000000 rotop-1.0.4/src/rotop/top_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-12-15 07:41:33.000000 rotop-1.0.4/src/rotop/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-15 07:41:33.000000 rotop-1.0.4/src/rotop/version_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 07:41:43.603783 rotop-1.0.4/src/rotop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2023-12-15 07:41:43.000000 rotop-1.0.4/src/rotop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-15 07:41:43.000000 rotop-1.0.4/src/rotop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 07:41:43.000000 rotop-1.0.4/src/rotop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-15 07:41:43.000000 rotop-1.0.4/src/rotop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-15 07:41:43.000000 rotop-1.0.4/src/rotop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-15 07:41:43.000000 rotop-1.0.4/src/rotop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:08:22.276193 rotop-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:08:22.272193 rotop-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:08:22.272193 rotop-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-10 10:08:07.000000 rotop-1.0.5/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-10 10:08:07.000000 rotop-1.0.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:08:22.272193 rotop-1.0.5/00_doc/
+-rw-r--r--   0 runner    (1001) docker     (127)   394789 2024-05-10 10:08:07.000000 rotop-1.0.5/00_doc/capture_00.png
+-rw-r--r--   0 runner    (1001) docker     (127)   746799 2024-05-10 10:08:07.000000 rotop-1.0.5/00_doc/capture_01.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 10:08:07.000000 rotop-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-10 10:08:22.276193 rotop-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-10 10:08:07.000000 rotop-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 10:08:07.000000 rotop-1.0.5/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-10 10:08:07.000000 rotop-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 10:08:07.000000 rotop-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:08:22.276193 rotop-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:08:22.272193 rotop-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:08:22.276193 rotop-1.0.5/src/rotop/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-10 10:08:07.000000 rotop-1.0.5/src/rotop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-10 10:08:07.000000 rotop-1.0.5/src/rotop/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 10:08:22.000000 rotop-1.0.5/src/rotop/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-10 10:08:07.000000 rotop-1.0.5/src/rotop/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-05-10 10:08:07.000000 rotop-1.0.5/src/rotop/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-10 10:08:07.000000 rotop-1.0.5/src/rotop/rotop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-05-10 10:08:07.000000 rotop-1.0.5/src/rotop/top_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-10 10:08:07.000000 rotop-1.0.5/src/rotop/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 10:08:07.000000 rotop-1.0.5/src/rotop/version_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:08:22.276193 rotop-1.0.5/src/rotop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-10 10:08:22.000000 rotop-1.0.5/src/rotop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-10 10:08:22.000000 rotop-1.0.5/src/rotop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:08:22.000000 rotop-1.0.5/src/rotop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-10 10:08:22.000000 rotop-1.0.5/src/rotop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 10:08:22.000000 rotop-1.0.5/src/rotop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 10:08:22.000000 rotop-1.0.5/src/rotop.egg-info/top_level.txt
```

### Comparing `rotop-1.0.4/.github/workflows/pypi-publish.yml` & `rotop-1.0.5/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `rotop-1.0.4/.gitignore` & `rotop-1.0.5/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 _version.py
 .vscode/
+rotop*/total*.csv
 rotop*/cpu*.csv
 rotop*/mem*.csv
 
 ### https://raw.githubusercontent.com/github/gitignore/main/Python.gitignore ###
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
```

### Comparing `rotop-1.0.4/00_doc/capture_00.png` & `rotop-1.0.5/00_doc/capture_00.png`

 * *Files identical despite different names*

### Comparing `rotop-1.0.4/00_doc/capture_01.png` & `rotop-1.0.5/00_doc/capture_01.png`

 * *Files identical despite different names*

### Comparing `rotop-1.0.4/LICENSE` & `rotop-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rotop-1.0.4/PKG-INFO` & `rotop-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotop
-Version: 1.0.4
+Version: 1.0.5
 Summary: top command for ROS 2
 Author-email: iwatake2222 <take.iwiw2222@gmail.com>
 Maintainer-email: iwatake2222 <take.iwiw2222@gmail.com>
 Project-URL: Homepage, https://github.com/iwatake2222/rotop
 Project-URL: Bug Reports, https://github.com/iwatake2222/rotop/issues
 Project-URL: Source, https://github.com/iwatake2222/rotop
 Keywords: ros,ros2,tool,cpu,performance,monitoring
```

### Comparing `rotop-1.0.4/README.md` & `rotop-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rotop-1.0.4/main.py` & `rotop-1.0.5/main.py`

 * *Files identical despite different names*

### Comparing `rotop-1.0.4/pyproject.toml` & `rotop-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rotop-1.0.4/src/rotop/__init__.py` & `rotop-1.0.5/src/rotop/__init__.py`

 * *Files identical despite different names*

### Comparing `rotop-1.0.4/src/rotop/__main__.py` & `rotop-1.0.5/src/rotop/__main__.py`

 * *Files identical despite different names*

### Comparing `rotop-1.0.4/src/rotop/data_container.py` & `rotop-1.0.5/src/rotop/data_container.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,52 +21,59 @@
 from .utility import create_logger
 
 
 logger = create_logger(__name__, log_filename='rotop.log')
 
 
 class DataContainer:
-  MAX_ROW_CSV = 600
+  MAX_ROW_CSV = 1000
   MAX_NUM_HISTORY = 100
 
   def __init__(self, write_csv=False):
     now = datetime.datetime.now()
     if write_csv:
       self.csv_dir_name = now.strftime('./rotop_%Y%m%d_%H%M%S')
       os.mkdir(self.csv_dir_name)
     else:
       self.csv_dir_name = None
     self.csv_index = 0
+    self.df_total = pd.DataFrame()
     self.df_cpu = pd.DataFrame()
     self.df_mem = pd.DataFrame()
+    self.df_total_history = pd.DataFrame()
     self.df_cpu_history = pd.DataFrame()
     self.df_mem_history = pd.DataFrame()
 
   def run(self, top_runner: TopRunner, lines: list[str], num_process: int):
     if top_runner.col_range_command and top_runner.col_range_command[0] > 0:
-      df_cpu_current, df_mem_current = self.create_df_from_top(top_runner, lines, num_process)
+      df_total_current, df_cpu_current, df_mem_current = self.create_df_from_top(top_runner, lines, num_process)
+      self.df_total = pd.concat([self.df_total, df_total_current], axis=0)
       self.df_cpu = pd.concat([self.df_cpu, df_cpu_current], axis=0)
       self.df_mem = pd.concat([self.df_mem, df_mem_current], axis=0)
+      self.df_total_history = pd.concat([self.df_total_history, df_cpu_current], axis=0, ignore_index=True)
       self.df_cpu_history = pd.concat([self.df_cpu_history, df_cpu_current], axis=0, ignore_index=True)
       self.df_mem_history = pd.concat([self.df_mem_history, df_mem_current], axis=0, ignore_index=True)
       if self.csv_dir_name:
+        self.df_total.to_csv(os.path.join(self.csv_dir_name, f'total_{self.csv_index:03d}.csv'), index=False)
         self.df_cpu.to_csv(os.path.join(self.csv_dir_name, f'cpu_{self.csv_index:03d}.csv'), index=False)
         self.df_mem.to_csv(os.path.join(self.csv_dir_name, f'mem_{self.csv_index:03d}.csv'), index=False)
-        if len(self.df_cpu) >= self.MAX_ROW_CSV:
+        if len(self.df_total) >= self.MAX_ROW_CSV:
+          self.df_total = pd.DataFrame()
           self.df_cpu = pd.DataFrame()
           self.df_mem = pd.DataFrame()
           self.csv_index += 1
-      if len(self.df_cpu_history) >= self.MAX_NUM_HISTORY:
+      if len(self.df_total_history) >= self.MAX_NUM_HISTORY:
+        self.df_total_history = self.df_total_history[1:]
         self.df_cpu_history = self.df_cpu_history[1:]
         self.df_mem_history = self.df_mem_history[1:]
 
     self.df_cpu_history = self.sort_df_in_column(self.df_cpu_history)
     self.df_mem_history = self.sort_df_in_column(self.df_mem_history)
 
-    return self.df_cpu_history, self.df_mem_history
+    return self.df_total_history, self.df_cpu_history, self.df_mem_history
 
 
   def reset_history(self):
     self.df_cpu_history = pd.DataFrame()
     self.df_mem_history = pd.DataFrame()
 
 
@@ -76,19 +83,37 @@
     return df
 
 
   @staticmethod
   def create_df_from_top(top_runner: TopRunner, lines: list[str], num_process: int):
     # now = datetime.datetime.now()
     now = int(time.time())
+
+    # Get total info
+    total_line = None
+    total_user = ''
+    total_sys = ''
+    total_idle = ''
+    for i, line in enumerate(lines):
+      if '%Cpu' in line:
+        total_line = line
+        break
+    if total_line:
+      total_user = total_line.split('us')[0].split()[-1].strip()
+      total_sys = total_line.split('sy')[0].split()[-1].strip()
+      total_idle = total_line.split('id')[0].split()[-1].strip()
+    df_total_current = pd.DataFrame([[now, total_user, total_sys, total_idle]], columns=['datetime', 'user', 'sys', 'idle'])
+
+    # Move to line containing process info
     for i, line in enumerate(lines):
       if 'PID' in line:
         lines = lines[i + 1:]
         break
 
+    # Get process info
     process_list = []
     cpu_list = []
     mem_list = []
     for i, line in enumerate(lines):
       if i >= num_process:
         break
       pid = line[top_runner.col_range_pid[0]:top_runner.col_range_pid[1]].strip()
@@ -99,8 +124,8 @@
       cpu_list.append(cpu)
       mem = float(line[top_runner.col_range_MEM[0]:top_runner.col_range_MEM[1]].strip())
       mem_list.append(mem)
 
     df_cpu_current = pd.DataFrame([[now] + cpu_list], columns=['datetime'] + process_list)
     df_mem_current = pd.DataFrame([[now] + mem_list], columns=['datetime'] + process_list)
 
-    return df_cpu_current, df_mem_current
+    return df_total_current, df_cpu_current, df_mem_current
```

### Comparing `rotop-1.0.4/src/rotop/gui_main.py` & `rotop-1.0.5/src/rotop/gui_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         g_reset_history_df = False
 
       result_lines, result_show_all_lines = top_runner.run(args.num_process, True, args.only_ros)
       if result_show_all_lines is None:
         time.sleep(0.1)
         continue
 
-      df_cpu_history, df_mem_history = data_container.run(top_runner, result_show_all_lines, args.num_process)
+      _, df_cpu_history, df_mem_history = data_container.run(top_runner, result_show_all_lines, args.num_process)
       df_cpu_history = df_cpu_history.iloc[:, :min(args.num_process, len(df_cpu_history.columns))]
       df_mem_history = df_mem_history.iloc[:, :min(args.num_process, len(df_mem_history.columns))]
 
       if gui_thread.is_alive():
         view.update_gui(result_lines, df_cpu_history, df_mem_history)
       else:
         break
```

### Comparing `rotop-1.0.4/src/rotop/rotop.py` & `rotop-1.0.5/src/rotop/rotop.py`

 * *Files identical despite different names*

### Comparing `rotop-1.0.4/src/rotop/top_runner.py` & `rotop-1.0.5/src/rotop/top_runner.py`

 * *Files identical despite different names*

### Comparing `rotop-1.0.4/src/rotop/utility.py` & `rotop-1.0.5/src/rotop/utility.py`

 * *Files identical despite different names*

### Comparing `rotop-1.0.4/src/rotop.egg-info/PKG-INFO` & `rotop-1.0.5/src/rotop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotop
-Version: 1.0.4
+Version: 1.0.5
 Summary: top command for ROS 2
 Author-email: iwatake2222 <take.iwiw2222@gmail.com>
 Maintainer-email: iwatake2222 <take.iwiw2222@gmail.com>
 Project-URL: Homepage, https://github.com/iwatake2222/rotop
 Project-URL: Bug Reports, https://github.com/iwatake2222/rotop/issues
 Project-URL: Source, https://github.com/iwatake2222/rotop
 Keywords: ros,ros2,tool,cpu,performance,monitoring
```

### Comparing `rotop-1.0.4/src/rotop.egg-info/SOURCES.txt` & `rotop-1.0.5/src/rotop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

