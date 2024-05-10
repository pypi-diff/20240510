# Comparing `tmp/aiida_bader-0.0.4.tar.gz` & `tmp/aiida_bader-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_bader-0.0.4.tar", last modified: Wed Apr 24 14:50:59 2024, max compression
+gzip compressed data, was "aiida_bader-0.0.5.tar", last modified: Wed Apr 24 20:38:04 2024, max compression
```

## Comparing `aiida_bader-0.0.4.tar` & `aiida_bader-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/
--rw-rw-r--   0 xing      (1000) xing      (1000)     1066 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/LICENSE
--rw-r--r--   0 xing      (1000) xing      (1000)     2136 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)     1606 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/README.md
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/calculations/
--rw-rw-r--   0 xing      (1000) xing      (1000)     3680 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/calculations/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/parsers/
--rw-rw-r--   0 xing      (1000) xing      (1000)     2005 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/parsers/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/qeapp/
--rw-rw-r--   0 xing      (1000) xing      (1000)      657 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/qeapp/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     3858 2024-04-10 19:56:14.000000 aiida_bader-0.0.4/aiida_bader/qeapp/result.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2857 2024-04-10 19:56:14.000000 aiida_bader-0.0.4/aiida_bader/qeapp/widget.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     2758 2024-04-10 19:56:14.000000 aiida_bader-0.0.4/aiida_bader/qeapp/workchain.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/workchains/
--rw-rw-r--   0 xing      (1000) xing      (1000)       93 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/workchains/__init__.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/workchains/protocols/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/workchains/protocols/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)     1196 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/workchains/protocols/bader.yaml
--rw-rw-r--   0 xing      (1000) xing      (1000)     8003 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/workchains/qe_bader.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader/worktrees/
--rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/worktrees/__init__.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      635 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/aiida_bader/worktrees/cp2k_bader.py
--rw-rw-r--   0 xing      (1000) xing      (1000)      903 2024-04-10 19:55:50.000000 aiida_bader-0.0.4/aiida_bader/worktrees/qe_bader.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/aiida_bader.egg-info/
--rw-r--r--   0 xing      (1000) xing      (1000)     2136 2024-04-24 14:50:59.000000 aiida_bader-0.0.4/aiida_bader.egg-info/PKG-INFO
--rw-rw-r--   0 xing      (1000) xing      (1000)      731 2024-04-24 14:50:59.000000 aiida_bader-0.0.4/aiida_bader.egg-info/SOURCES.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-04-24 14:50:59.000000 aiida_bader-0.0.4/aiida_bader.egg-info/dependency_links.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      256 2024-04-24 14:50:59.000000 aiida_bader-0.0.4/aiida_bader.egg-info/entry_points.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)      100 2024-04-24 14:50:59.000000 aiida_bader-0.0.4/aiida_bader.egg-info/requires.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       12 2024-04-24 14:50:59.000000 aiida_bader-0.0.4/aiida_bader.egg-info/top_level.txt
--rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/setup.cfg
--rw-rw-r--   0 xing      (1000) xing      (1000)     1556 2024-04-24 14:50:48.000000 aiida_bader-0.0.4/setup.py
-drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 14:50:59.706954 aiida_bader-0.0.4/tests/
--rw-rw-r--   0 xing      (1000) xing      (1000)      122 2024-03-25 15:26:07.000000 aiida_bader-0.0.4/tests/test_bader.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 20:38:04.049686 aiida_bader-0.0.5/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1066 2024-03-25 15:26:07.000000 aiida_bader-0.0.5/LICENSE
+-rw-r--r--   0 xing      (1000) xing      (1000)     2141 2024-04-24 20:38:04.049686 aiida_bader-0.0.5/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1606 2024-03-25 15:26:07.000000 aiida_bader-0.0.5/README.md
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 20:38:04.049686 aiida_bader-0.0.5/aiida_bader/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.5/aiida_bader/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 20:38:04.049686 aiida_bader-0.0.5/aiida_bader/calculations/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3680 2024-03-25 15:26:07.000000 aiida_bader-0.0.5/aiida_bader/calculations/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 20:38:04.049686 aiida_bader-0.0.5/aiida_bader/parsers/
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2005 2024-03-25 15:26:07.000000 aiida_bader-0.0.5/aiida_bader/parsers/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 20:38:04.049686 aiida_bader-0.0.5/aiida_bader/qeapp/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      708 2024-04-24 20:36:37.000000 aiida_bader-0.0.5/aiida_bader/qeapp/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     3858 2024-04-10 19:56:14.000000 aiida_bader-0.0.5/aiida_bader/qeapp/result.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2857 2024-04-10 19:56:14.000000 aiida_bader-0.0.5/aiida_bader/qeapp/widget.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     2758 2024-04-10 19:56:14.000000 aiida_bader-0.0.5/aiida_bader/qeapp/workchain.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 20:38:04.049686 aiida_bader-0.0.5/aiida_bader/workchains/
+-rw-rw-r--   0 xing      (1000) xing      (1000)       93 2024-03-25 15:26:07.000000 aiida_bader-0.0.5/aiida_bader/workchains/__init__.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 20:38:04.049686 aiida_bader-0.0.5/aiida_bader/workchains/protocols/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.5/aiida_bader/workchains/protocols/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1196 2024-03-25 15:26:07.000000 aiida_bader-0.0.5/aiida_bader/workchains/protocols/bader.yaml
+-rw-rw-r--   0 xing      (1000) xing      (1000)     8003 2024-03-25 15:26:07.000000 aiida_bader-0.0.5/aiida_bader/workchains/qe_bader.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 20:38:04.049686 aiida_bader-0.0.5/aiida_bader/worktrees/
+-rw-rw-r--   0 xing      (1000) xing      (1000)        0 2024-03-25 15:26:07.000000 aiida_bader-0.0.5/aiida_bader/worktrees/__init__.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      635 2024-03-25 15:26:07.000000 aiida_bader-0.0.5/aiida_bader/worktrees/cp2k_bader.py
+-rw-rw-r--   0 xing      (1000) xing      (1000)      903 2024-04-10 19:55:50.000000 aiida_bader-0.0.5/aiida_bader/worktrees/qe_bader.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 20:38:04.049686 aiida_bader-0.0.5/aiida_bader.egg-info/
+-rw-r--r--   0 xing      (1000) xing      (1000)     2141 2024-04-24 20:38:04.000000 aiida_bader-0.0.5/aiida_bader.egg-info/PKG-INFO
+-rw-rw-r--   0 xing      (1000) xing      (1000)      731 2024-04-24 20:38:04.000000 aiida_bader-0.0.5/aiida_bader.egg-info/SOURCES.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)        1 2024-04-24 20:38:04.000000 aiida_bader-0.0.5/aiida_bader.egg-info/dependency_links.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      256 2024-04-24 20:38:04.000000 aiida_bader-0.0.5/aiida_bader.egg-info/entry_points.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)      105 2024-04-24 20:38:04.000000 aiida_bader-0.0.5/aiida_bader.egg-info/requires.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       12 2024-04-24 20:38:04.000000 aiida_bader-0.0.5/aiida_bader.egg-info/top_level.txt
+-rw-rw-r--   0 xing      (1000) xing      (1000)       38 2024-04-24 20:38:04.049686 aiida_bader-0.0.5/setup.cfg
+-rw-rw-r--   0 xing      (1000) xing      (1000)     1561 2024-04-24 20:37:32.000000 aiida_bader-0.0.5/setup.py
+drwxrwxr-x   0 xing      (1000) xing      (1000)        0 2024-04-24 20:38:04.049686 aiida_bader-0.0.5/tests/
+-rw-rw-r--   0 xing      (1000) xing      (1000)      122 2024-03-25 15:26:07.000000 aiida_bader-0.0.5/tests/test_bader.py
```

### Comparing `aiida_bader-0.0.4/LICENSE` & `aiida_bader-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.4/PKG-INFO` & `aiida_bader-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: aiida-bader
-Version: 0.0.4
+Version: 0.0.5
 Summary: AiiDA plugin for bader code.
 Home-page: https://github.com/superstart54/aiida-bader
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiida-core
 Requires-Dist: aiida-worktree
-Requires-Dist: aiida-quantumespresso
+Requires-Dist: aiida-quantumespresso~=4.4
 Requires-Dist: aiida-cp2k
 Requires-Dist: weas-widget
 Requires-Dist: pytest
 Requires-Dist: pytest-cov
 Requires-Dist: pre-commit
 
 # AiiDA-Bader
```

### Comparing `aiida_bader-0.0.4/README.md` & `aiida_bader-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.4/aiida_bader/calculations/__init__.py` & `aiida_bader-0.0.5/aiida_bader/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.4/aiida_bader/parsers/__init__.py` & `aiida_bader-0.0.5/aiida_bader/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.4/aiida_bader/qeapp/__init__.py` & `aiida_bader-0.0.5/aiida_bader/qeapp/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from aiidalab_qe.common.panel import OutlinePanel
-from aiidalab_widgets_base import ComputationalResourcesWidget
+from aiidalab_qe.common.widgets import (
+    QEAppComputationalResourcesWidget as ComputationalResourcesWidget,
+)
 
 from .result import Result
 from .workchain import workchain_and_builder
 
 
 class BaderOutline(OutlinePanel):
     title = "Bader charge analysis"
```

### Comparing `aiida_bader-0.0.4/aiida_bader/qeapp/result.py` & `aiida_bader-0.0.5/aiida_bader/qeapp/result.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.4/aiida_bader/qeapp/widget.py` & `aiida_bader-0.0.5/aiida_bader/qeapp/widget.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.4/aiida_bader/qeapp/workchain.py` & `aiida_bader-0.0.5/aiida_bader/qeapp/workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.4/aiida_bader/workchains/protocols/bader.yaml` & `aiida_bader-0.0.5/aiida_bader/workchains/protocols/bader.yaml`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.4/aiida_bader/workchains/qe_bader.py` & `aiida_bader-0.0.5/aiida_bader/workchains/qe_bader.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.4/aiida_bader/worktrees/cp2k_bader.py` & `aiida_bader-0.0.5/aiida_bader/worktrees/cp2k_bader.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.4/aiida_bader/worktrees/qe_bader.py` & `aiida_bader-0.0.5/aiida_bader/worktrees/qe_bader.py`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.4/aiida_bader.egg-info/PKG-INFO` & `aiida_bader-0.0.5/aiida_bader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: aiida-bader
-Version: 0.0.4
+Version: 0.0.5
 Summary: AiiDA plugin for bader code.
 Home-page: https://github.com/superstart54/aiida-bader
 Author: Xing Wang
 Author-email: xingwang1991@gmail.com
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiida-core
 Requires-Dist: aiida-worktree
-Requires-Dist: aiida-quantumespresso
+Requires-Dist: aiida-quantumespresso~=4.4
 Requires-Dist: aiida-cp2k
 Requires-Dist: weas-widget
 Requires-Dist: pytest
 Requires-Dist: pytest-cov
 Requires-Dist: pre-commit
 
 # AiiDA-Bader
```

### Comparing `aiida_bader-0.0.4/aiida_bader.egg-info/SOURCES.txt` & `aiida_bader-0.0.5/aiida_bader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiida_bader-0.0.4/setup.py` & `aiida_bader-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name="aiida-bader",
-    version="0.0.4",
+    version="0.0.5",
     description="AiiDA plugin for bader code.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/superstart54/aiida-bader",
     author="Xing Wang",
     author_email="xingwang1991@gmail.com",
     license="MIT License",
     classifiers=[],
     packages=find_packages(),
     install_requires=[
         "aiida-core",
         "aiida-worktree",
-        "aiida-quantumespresso",
+        "aiida-quantumespresso~=4.4",
         "aiida-cp2k",
         "weas-widget",
         "pytest",
         "pytest-cov",
         "pre-commit",
     ],
     entry_points={
```

