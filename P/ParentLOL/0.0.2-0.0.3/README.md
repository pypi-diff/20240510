# Comparing `tmp/parentlol-0.0.2.tar.gz` & `tmp/parentlol-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parentlol-0.0.2.tar", last modified: Fri May 10 03:03:34 2024, max compression
+gzip compressed data, was "parentlol-0.0.3.tar", last modified: Fri May 10 03:56:33 2024, max compression
```

## Comparing `parentlol-0.0.2.tar` & `parentlol-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 03:03:34.957087 parentlol-0.0.2/
--rw-rw-rw-   0        0        0      374 2024-05-10 03:03:34.955062 parentlol-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 03:03:34.942048 parentlol-0.0.2/ParentLOL/
--rw-rw-rw-   0        0        0     1158 2024-05-10 03:01:41.000000 parentlol-0.0.2/ParentLOL/ParentLOL.py
--rw-rw-rw-   0        0        0       33 2024-05-10 03:02:22.000000 parentlol-0.0.2/ParentLOL/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 03:03:34.953558 parentlol-0.0.2/ParentLOL.egg-info/
--rw-rw-rw-   0        0        0      374 2024-05-10 03:03:34.000000 parentlol-0.0.2/ParentLOL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-05-10 03:03:34.000000 parentlol-0.0.2/ParentLOL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 03:03:34.000000 parentlol-0.0.2/ParentLOL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-10 03:03:34.000000 parentlol-0.0.2/ParentLOL.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-10 03:03:34.000000 parentlol-0.0.2/ParentLOL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 03:03:34.957087 parentlol-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      521 2024-05-10 03:03:09.000000 parentlol-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:56:33.949166 parentlol-0.0.3/
+-rw-rw-rw-   0        0        0      374 2024-05-10 03:56:33.947659 parentlol-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 03:56:33.927806 parentlol-0.0.3/ParentLOL/
+-rw-rw-rw-   0        0        0     1276 2024-05-10 03:56:02.000000 parentlol-0.0.3/ParentLOL/ParentLOL.py
+-rw-rw-rw-   0        0        0       33 2024-05-10 03:02:22.000000 parentlol-0.0.3/ParentLOL/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 03:56:33.945659 parentlol-0.0.3/ParentLOL.egg-info/
+-rw-rw-rw-   0        0        0      374 2024-05-10 03:56:33.000000 parentlol-0.0.3/ParentLOL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-05-10 03:56:33.000000 parentlol-0.0.3/ParentLOL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 03:56:33.000000 parentlol-0.0.3/ParentLOL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 03:56:33.000000 parentlol-0.0.3/ParentLOL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-10 03:56:33.000000 parentlol-0.0.3/ParentLOL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 03:56:33.950211 parentlol-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      521 2024-05-10 03:56:12.000000 parentlol-0.0.3/setup.py
```

### Comparing `parentlol-0.0.2/ParentLOL/ParentLOL.py` & `parentlol-0.0.3/ParentLOL/ParentLOL.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 init()
 
 class ParPrint:
     SUCCESS = Fore.GREEN
     FAILED = Fore.RED
     WARNING = Fore.YELLOW
+    INFO = Fore.BLUE
     CYAN = Fore.CYAN
     END = Style.RESET_ALL
 
     @staticmethod
     def _get_current_time():
         return datetime.now().strftime("[%H:%M:%S]")
 
@@ -22,14 +23,16 @@
             
         if status == "Success":
             print(f"{time_prefix}{self.SUCCESS}{text}{self.END}")
         elif status == "Failed":
             print(f"{time_prefix}{self.FAILED}{text}{self.END}")
         elif status == "Warning":
             print(f"{time_prefix}{self.WARNING}{text}{self.END}")
+        elif status == "Info":
+            print(f"{time_prefix}{self.INFO}{text}{self.END}")
         else:
             print(f"{time_prefix}{text}")
 
 # Example usage
 if __name__ == "__main__":
     ParPrint("This is a test", "Success", time=True)
     ParPrint("This is a test", "Failed", time=True)
```

### Comparing `parentlol-0.0.2/setup.py` & `parentlol-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ParentLOL',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[
         "colorama",
         "datetime"
     ],
     description='Printing with Ease.',
     author='parent',
```

