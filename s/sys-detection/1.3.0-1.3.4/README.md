# Comparing `tmp/sys-detection-1.3.0.tar.gz` & `tmp/sys_detection-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sys-detection-1.3.0.tar", last modified: Sat Apr 23 04:36:06 2022, max compression
+gzip compressed data, was "sys_detection-1.3.4.tar", last modified: Fri May 10 19:04:59 2024, max compression
```

## Comparing `sys-detection-1.3.0.tar` & `sys_detection-1.3.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 mbautin  (19778) mbautin  (19778)        0 2022-04-23 04:36:06.261181 sys-detection-1.3.0/
--rw-rw-r--   0 mbautin  (19778) mbautin  (19778)     1771 2022-04-23 04:36:06.261181 sys-detection-1.3.0/PKG-INFO
--rw-rw-r--   0 mbautin  (19778) mbautin  (19778)     1111 2022-03-22 05:03:53.000000 sys-detection-1.3.0/README.md
--rw-rw-r--   0 mbautin  (19778) mbautin  (19778)       38 2022-04-23 04:36:06.261181 sys-detection-1.3.0/setup.cfg
--rw-rw-r--   0 mbautin  (19778) mbautin  (19778)     1991 2022-04-23 01:36:02.000000 sys-detection-1.3.0/setup.py
-drwxrwxr-x   0 mbautin  (19778) mbautin  (19778)        0 2022-04-23 04:36:06.259181 sys-detection-1.3.0/src/
-drwxrwxr-x   0 mbautin  (19778) mbautin  (19778)        0 2022-04-23 04:36:06.260181 sys-detection-1.3.0/src/sys_detection/
--rw-rw-r--   0 mbautin  (19778) mbautin  (19778)     8002 2022-04-23 01:37:03.000000 sys-detection-1.3.0/src/sys_detection/__init__.py
--rw-rw-r--   0 mbautin  (19778) mbautin  (19778)      896 2022-03-22 05:03:53.000000 sys-detection-1.3.0/src/sys_detection/__main__.py
--rw-rw-r--   0 mbautin  (19778) mbautin  (19778)     1329 2022-04-23 01:37:12.000000 sys-detection-1.3.0/src/sys_detection/os_compatibility.py
--rw-rw-r--   0 mbautin  (19778) mbautin  (19778)        0 2022-03-22 05:03:53.000000 sys-detection-1.3.0/src/sys_detection/py.typed
-drwxrwxr-x   0 mbautin  (19778) mbautin  (19778)        0 2022-04-23 04:36:06.261181 sys-detection-1.3.0/src/sys_detection.egg-info/
--rw-rw-r--   0 mbautin  (19778) mbautin  (19778)     1771 2022-04-23 04:36:06.000000 sys-detection-1.3.0/src/sys_detection.egg-info/PKG-INFO
--rw-rw-r--   0 mbautin  (19778) mbautin  (19778)      347 2022-04-23 04:36:06.000000 sys-detection-1.3.0/src/sys_detection.egg-info/SOURCES.txt
--rw-rw-r--   0 mbautin  (19778) mbautin  (19778)        1 2022-04-23 04:36:06.000000 sys-detection-1.3.0/src/sys_detection.egg-info/dependency_links.txt
--rw-rw-r--   0 mbautin  (19778) mbautin  (19778)       50 2022-04-23 04:36:06.000000 sys-detection-1.3.0/src/sys_detection.egg-info/requires.txt
--rw-rw-r--   0 mbautin  (19778) mbautin  (19778)       14 2022-04-23 04:36:06.000000 sys-detection-1.3.0/src/sys_detection.egg-info/top_level.txt
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-05-10 19:04:59.678699 sys_detection-1.3.4/
+-rw-r--r--   0 mikhail    (503) staff       (20)    11358 2021-09-18 18:25:06.000000 sys_detection-1.3.4/LICENSE
+-rw-r--r--   0 mikhail    (503) staff       (20)     1676 2024-05-10 19:04:59.678451 sys_detection-1.3.4/PKG-INFO
+-rw-r--r--   0 mikhail    (503) staff       (20)     1111 2021-09-18 18:35:43.000000 sys_detection-1.3.4/README.md
+-rw-r--r--   0 mikhail    (503) staff       (20)       38 2024-05-10 19:04:59.678752 sys_detection-1.3.4/setup.cfg
+-rw-r--r--   0 mikhail    (503) staff       (20)     2016 2024-05-10 19:04:39.000000 sys_detection-1.3.4/setup.py
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-05-10 19:04:59.675588 sys_detection-1.3.4/src/
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-05-10 19:04:59.676736 sys_detection-1.3.4/src/sys_detection/
+-rw-r--r--   0 mikhail    (503) staff       (20)     8022 2024-05-10 18:50:03.000000 sys_detection-1.3.4/src/sys_detection/__init__.py
+-rw-r--r--   0 mikhail    (503) staff       (20)      896 2021-09-18 18:25:06.000000 sys_detection-1.3.4/src/sys_detection/__main__.py
+-rw-r--r--   0 mikhail    (503) staff       (20)     1329 2024-05-10 18:48:38.000000 sys_detection-1.3.4/src/sys_detection/os_compatibility.py
+-rw-r--r--   0 mikhail    (503) staff       (20)        0 2021-09-18 18:25:06.000000 sys_detection-1.3.4/src/sys_detection/py.typed
+drwxr-xr-x   0 mikhail    (503) staff       (20)        0 2024-05-10 19:04:59.677788 sys_detection-1.3.4/src/sys_detection.egg-info/
+-rw-r--r--   0 mikhail    (503) staff       (20)     1676 2024-05-10 19:04:59.000000 sys_detection-1.3.4/src/sys_detection.egg-info/PKG-INFO
+-rw-r--r--   0 mikhail    (503) staff       (20)      355 2024-05-10 19:04:59.000000 sys_detection-1.3.4/src/sys_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)        1 2024-05-10 19:04:59.000000 sys_detection-1.3.4/src/sys_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       56 2024-05-10 19:04:59.000000 sys_detection-1.3.4/src/sys_detection.egg-info/requires.txt
+-rw-r--r--   0 mikhail    (503) staff       (20)       14 2024-05-10 19:04:59.000000 sys_detection-1.3.4/src/sys_detection.egg-info/top_level.txt
```

### Comparing `sys-detection-1.3.0/PKG-INFO` & `sys_detection-1.3.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 Metadata-Version: 2.1
 Name: sys-detection
-Version: 1.3.0
+Version: 1.3.4
 Summary: A library to detect the operating system, its version, architecture, etc.
 Home-page: https://github.com/yugabyte/sys-detection
 Author: Mikhail Bautin
 Author-email: mbautin@users.noreply.github.com
-License: UNKNOWN
-Description: # sys-detection
-        
-        https://pypi.org/project/sys-detection/
-        
-        Allows identifiying the current operating system, which is helpful when
-        building and packaging cross-platform software.
-        
-        ## Usage as module
-        
-        ```
-        >>> from sys_detection import local_sys_conf
-        
-        >>> local_sys_conf()
-         <sys_detection.SysConfiguration system='Linux' architecture='x86_64' linux_os_release={'NAME': 'CentOS Stream', 'VERSION': '8', 'ID': 'centos', 'ID_LIKE': 'rhel fedora', 'VERSION_ID': '8', 'PLATFORM_ID': 'platform:el8', 'PRETTY_NAME': 'CentOS Stream 8', 'ANSI_COLOR': '0;31', 'CPE_NAME': 'cpe:/o:centos:centos:8', 'HOME_URL': 'https://centos.org/', 'BUG_REPORT_URL': 'https://bugzilla.redhat.com/', 'REDHAT_SUPPORT_PRODUCT': 'Red Hat Enterprise Linux 8', 'REDHAT_SUPPORT_PRODUCT_VERSION': 'CentOS Stream'} at 0x7f0123456789>
-        
-        >>> local_sys_conf().id_for_packaging()
-        'centos8-x86_64'
-        
-        >>> local_sys_conf().id_for_packaging(mid_part=['moreinfo'])
-        'centos8-moreinfo-x86_64'
-        
-        >>> local_sys_conf().id_for_packaging(separator='_')
-        'centos8_x86_64'
-        ```
-        
-        ## Command-line usage
-        
-        ```bash
-        python3 -m sys_detection
-        ```
-        
-        Output:
-        
-        ```
-        centos8-x86_64
-        ```
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: autorepr
 Provides-Extra: dev
+Requires-Dist: codecheck; extra == "dev"
+Requires-Dist: pycodestyle; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
+# sys-detection
+
+https://pypi.org/project/sys-detection/
+
+Allows identifiying the current operating system, which is helpful when
+building and packaging cross-platform software.
+
+## Usage as module
+
+```
+>>> from sys_detection import local_sys_conf
+
+>>> local_sys_conf()
+ <sys_detection.SysConfiguration system='Linux' architecture='x86_64' linux_os_release={'NAME': 'CentOS Stream', 'VERSION': '8', 'ID': 'centos', 'ID_LIKE': 'rhel fedora', 'VERSION_ID': '8', 'PLATFORM_ID': 'platform:el8', 'PRETTY_NAME': 'CentOS Stream 8', 'ANSI_COLOR': '0;31', 'CPE_NAME': 'cpe:/o:centos:centos:8', 'HOME_URL': 'https://centos.org/', 'BUG_REPORT_URL': 'https://bugzilla.redhat.com/', 'REDHAT_SUPPORT_PRODUCT': 'Red Hat Enterprise Linux 8', 'REDHAT_SUPPORT_PRODUCT_VERSION': 'CentOS Stream'} at 0x7f0123456789>
+
+>>> local_sys_conf().id_for_packaging()
+'centos8-x86_64'
+
+>>> local_sys_conf().id_for_packaging(mid_part=['moreinfo'])
+'centos8-moreinfo-x86_64'
+
+>>> local_sys_conf().id_for_packaging(separator='_')
+'centos8_x86_64'
+```
+
+## Command-line usage
+
+```bash
+python3 -m sys_detection
+```
+
+Output:
+
+```
+centos8-x86_64
+```
```

### Comparing `sys-detection-1.3.0/README.md` & `sys_detection-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `sys-detection-1.3.0/setup.py` & `sys_detection-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from os import path
     this_directory = path.abspath(path.dirname(__file__))
     with open(path.join(this_directory, 'README.md'), encoding='utf-8') as readme_file:
         long_description = readme_file.read()
 
     setup(
         name='sys-detection',
-        version='1.3.0',
+        version='1.3.4',
         url='https://github.com/yugabyte/sys-detection',
         author='Mikhail Bautin',
         author_email='mbautin@users.noreply.github.com',
         description='A library to detect the operating system, its version, architecture, etc.',
         packages=find_packages(where='src'),
         package_dir={"": "src"},
         package_data={'sys_detection': ['py.typed']},
@@ -42,10 +42,11 @@
             #   . venv/bin/activate
             #   pip install --editable '.[dev]'
             'dev': [
                 'codecheck',
                 'pycodestyle',
                 'mypy',
                 'pytest',
+                'twine',
             ]
         }
     )
```

### Comparing `sys-detection-1.3.0/src/sys_detection/__init__.py` & `sys_detection-1.3.4/src/sys_detection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,26 @@
 
 
 VALID_ATTR_RE = re.compile('^[a-z_]+$')
 
 SHORT_LINUX_OS_NAMES = [
     'almalinux',
     'alpine',
+    'amazonlinux',
+    'amzn',
+    'arch',
     'centos',
     'debian',
     'fedora',
+    'manjaro',
     'ol',
-    'rocky',
-    'ubuntu',
     'opensuse-leap',
     'opensuse-tumbleweed',
-    'arch',
-    'manjaro',
-    'amzn'
+    'rocky',
+    'ubuntu',
 ]
 
 SHORT_OS_NAMES = ['macos'] + SHORT_LINUX_OS_NAMES
 
 SHORT_OS_NAME_REGEX_STR = '|'.join(SHORT_OS_NAMES)
 
 REDHAT_FAMILY_OS_NAMES = ['almalinux', 'centos', 'rhel', 'rocky', 'ol']
```

### Comparing `sys-detection-1.3.0/src/sys_detection/__main__.py` & `sys_detection-1.3.4/src/sys_detection/__main__.py`

 * *Files identical despite different names*

### Comparing `sys-detection-1.3.0/src/sys_detection/os_compatibility.py` & `sys_detection-1.3.4/src/sys_detection/os_compatibility.py`

 * *Files identical despite different names*

### Comparing `sys-detection-1.3.0/src/sys_detection.egg-info/PKG-INFO` & `sys_detection-1.3.4/src/sys_detection.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 Metadata-Version: 2.1
 Name: sys-detection
-Version: 1.3.0
+Version: 1.3.4
 Summary: A library to detect the operating system, its version, architecture, etc.
 Home-page: https://github.com/yugabyte/sys-detection
 Author: Mikhail Bautin
 Author-email: mbautin@users.noreply.github.com
-License: UNKNOWN
-Description: # sys-detection
-        
-        https://pypi.org/project/sys-detection/
-        
-        Allows identifiying the current operating system, which is helpful when
-        building and packaging cross-platform software.
-        
-        ## Usage as module
-        
-        ```
-        >>> from sys_detection import local_sys_conf
-        
-        >>> local_sys_conf()
-         <sys_detection.SysConfiguration system='Linux' architecture='x86_64' linux_os_release={'NAME': 'CentOS Stream', 'VERSION': '8', 'ID': 'centos', 'ID_LIKE': 'rhel fedora', 'VERSION_ID': '8', 'PLATFORM_ID': 'platform:el8', 'PRETTY_NAME': 'CentOS Stream 8', 'ANSI_COLOR': '0;31', 'CPE_NAME': 'cpe:/o:centos:centos:8', 'HOME_URL': 'https://centos.org/', 'BUG_REPORT_URL': 'https://bugzilla.redhat.com/', 'REDHAT_SUPPORT_PRODUCT': 'Red Hat Enterprise Linux 8', 'REDHAT_SUPPORT_PRODUCT_VERSION': 'CentOS Stream'} at 0x7f0123456789>
-        
-        >>> local_sys_conf().id_for_packaging()
-        'centos8-x86_64'
-        
-        >>> local_sys_conf().id_for_packaging(mid_part=['moreinfo'])
-        'centos8-moreinfo-x86_64'
-        
-        >>> local_sys_conf().id_for_packaging(separator='_')
-        'centos8_x86_64'
-        ```
-        
-        ## Command-line usage
-        
-        ```bash
-        python3 -m sys_detection
-        ```
-        
-        Output:
-        
-        ```
-        centos8-x86_64
-        ```
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: autorepr
 Provides-Extra: dev
+Requires-Dist: codecheck; extra == "dev"
+Requires-Dist: pycodestyle; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
+# sys-detection
+
+https://pypi.org/project/sys-detection/
+
+Allows identifiying the current operating system, which is helpful when
+building and packaging cross-platform software.
+
+## Usage as module
+
+```
+>>> from sys_detection import local_sys_conf
+
+>>> local_sys_conf()
+ <sys_detection.SysConfiguration system='Linux' architecture='x86_64' linux_os_release={'NAME': 'CentOS Stream', 'VERSION': '8', 'ID': 'centos', 'ID_LIKE': 'rhel fedora', 'VERSION_ID': '8', 'PLATFORM_ID': 'platform:el8', 'PRETTY_NAME': 'CentOS Stream 8', 'ANSI_COLOR': '0;31', 'CPE_NAME': 'cpe:/o:centos:centos:8', 'HOME_URL': 'https://centos.org/', 'BUG_REPORT_URL': 'https://bugzilla.redhat.com/', 'REDHAT_SUPPORT_PRODUCT': 'Red Hat Enterprise Linux 8', 'REDHAT_SUPPORT_PRODUCT_VERSION': 'CentOS Stream'} at 0x7f0123456789>
+
+>>> local_sys_conf().id_for_packaging()
+'centos8-x86_64'
+
+>>> local_sys_conf().id_for_packaging(mid_part=['moreinfo'])
+'centos8-moreinfo-x86_64'
+
+>>> local_sys_conf().id_for_packaging(separator='_')
+'centos8_x86_64'
+```
+
+## Command-line usage
+
+```bash
+python3 -m sys_detection
+```
+
+Output:
+
+```
+centos8-x86_64
+```
```

