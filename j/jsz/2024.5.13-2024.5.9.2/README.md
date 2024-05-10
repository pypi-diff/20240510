# Comparing `tmp/jsz-2024.5.13.tar.gz` & `tmp/jsz-2024.5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsz-2024.5.13.tar", last modified: Fri May 10 16:46:22 2024, max compression
+gzip compressed data, was "jsz-2024.5.9.2.tar", last modified: Thu May  9 15:40:15 2024, max compression
```

## Comparing `jsz-2024.5.13.tar` & `jsz-2024.5.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 16:46:22.878573 jsz-2024.5.13/
--rw-rw-rw-   0        0        0      884 2024-05-10 16:46:22.876560 jsz-2024.5.13/PKG-INFO
--rw-rw-rw-   0        0        0      128 2024-05-09 15:00:28.000000 jsz-2024.5.13/README.md
--rw-rw-rw-   0        0        0      675 2024-05-10 16:45:48.000000 jsz-2024.5.13/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 16:46:22.879644 jsz-2024.5.13/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 16:46:22.753969 jsz-2024.5.13/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 16:46:22.842126 jsz-2024.5.13/src/jsz/
--rw-rw-rw-   0        0        0      304 2024-04-29 13:27:07.000000 jsz-2024.5.13/src/jsz/__init__.py
--rw-rw-rw-   0        0        0     4366 2024-04-21 16:16:14.000000 jsz-2024.5.13/src/jsz/newpool.py
--rw-rw-rw-   0        0        0    20010 2024-05-10 16:44:49.000000 jsz-2024.5.13/src/jsz/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-10 16:46:22.871239 jsz-2024.5.13/src/jsz.egg-info/
--rw-rw-rw-   0        0        0      884 2024-05-10 16:46:22.000000 jsz-2024.5.13/src/jsz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-05-10 16:46:22.000000 jsz-2024.5.13/src/jsz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 16:46:22.000000 jsz-2024.5.13/src/jsz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2024-05-10 16:46:22.000000 jsz-2024.5.13/src/jsz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-10 16:46:22.000000 jsz-2024.5.13/src/jsz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 15:40:15.162739 jsz-2024.5.9.2/
+-rw-rw-rw-   0        0        0      854 2024-05-09 15:40:15.161749 jsz-2024.5.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0      128 2024-05-09 15:00:28.000000 jsz-2024.5.9.2/README.md
+-rw-rw-rw-   0        0        0      645 2024-05-09 15:17:28.000000 jsz-2024.5.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 15:40:15.163740 jsz-2024.5.9.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 15:40:15.140010 jsz-2024.5.9.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 15:40:15.145378 jsz-2024.5.9.2/src/jsz/
+-rw-rw-rw-   0        0        0      304 2024-04-29 13:27:07.000000 jsz-2024.5.9.2/src/jsz/__init__.py
+-rw-rw-rw-   0        0        0     4366 2024-04-21 16:16:14.000000 jsz-2024.5.9.2/src/jsz/newpool.py
+-rw-rw-rw-   0        0        0    19859 2024-05-09 14:59:07.000000 jsz-2024.5.9.2/src/jsz/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-09 15:40:15.160731 jsz-2024.5.9.2/src/jsz.egg-info/
+-rw-rw-rw-   0        0        0      854 2024-05-09 15:40:15.000000 jsz-2024.5.9.2/src/jsz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-05-09 15:40:15.000000 jsz-2024.5.9.2/src/jsz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 15:40:15.000000 jsz-2024.5.9.2/src/jsz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2024-05-09 15:40:15.000000 jsz-2024.5.9.2/src/jsz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-09 15:40:15.000000 jsz-2024.5.9.2/src/jsz.egg-info/top_level.txt
```

### Comparing `jsz-2024.5.13/PKG-INFO` & `jsz-2024.5.9.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: jsz
-Version: 2024.5.13
+Version: 2024.5.9.2
 Summary: 金手指
 Author: jiaosenvip
 Author-email: jiaosenvip <jiaosenvip@163.com>
 License: MIT
-Project-URL: Homepage, https://github.com/jiaosenvip/jsz
+Project-URL: homepage, https://github.com/jiaosenvip/jsz
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4
 Requires-Dist: lxml
 Requires-Dist: rich
 Requires-Dist: oss2
 Requires-Dist: pymongo
 Requires-Dist: pypdf
 Requires-Dist: html2text
 Requires-Dist: faker
 Requires-Dist: python-dateutil
-Requires-Dist: dateparser; platform_machine != "aarch64"
+Requires-Dist: dateparser
 Requires-Dist: loguru
 Requires-Dist: grequests
 Requires-Dist: httpx
 Requires-Dist: jsonpath
 Requires-Dist: parsel
 Requires-Dist: ipython
 Requires-Dist: js2py
```

### Comparing `jsz-2024.5.13/pyproject.toml` & `jsz-2024.5.9.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jsz"
-version = "2024.5.13"
+version = "2024.5.9.2"
 description = "金手指"
 authors = [
     { name = "jiaosenvip" },
     { name = "jiaosenvip", email = "jiaosenvip@163.com" },
 ]
 dependencies = [
     "beautifulsoup4",
@@ -12,23 +12,23 @@
     "rich",
     "oss2",
     "pymongo",
     "pypdf",
     "html2text",
     "faker",
     "python-dateutil",
-    "dateparser; platform_machine != 'aarch64'",
+    "dateparser",
     "loguru",
     "grequests",
     "httpx",
     "jsonpath",
     "parsel",
     "ipython",
     "js2py",
     "pandas[excel]",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 license = { text = "MIT" }
 
 [project.urls]
-Homepage = "https://github.com/jiaosenvip/jsz"
+homepage = "https://github.com/jiaosenvip/jsz"
```

### Comparing `jsz-2024.5.13/src/jsz/newpool.py` & `jsz-2024.5.9.2/src/jsz/newpool.py`

 * *Files identical despite different names*

### Comparing `jsz-2024.5.13/src/jsz/tools.py` & `jsz-2024.5.9.2/src/jsz/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,39 +22,35 @@
     unwrap,
     quote,
     parse_qs,
     parse_qsl,
 )
 from pypdf import PdfReader
 from faker import Faker
-from rich import print, print_json
+from rich import print
 from rich.progress import Progress, track
 from rich.console import Console
 from rich.columns import Columns
 from rich.markdown import Markdown
 from rich.panel import Panel
 from rich.rule import Rule
 from rich.status import Status
 from rich.table import Table
 from rich.pretty import pprint
 import datetime
 import time
-import platform
 from dateutil.parser import parse as timeparse
-
-if platform.machine() != "aarch64":
-    from dateparser import parse as timeparse2
-else:
-    timeparse2 = None
+from dateparser import parse as timeparse2
 from bs4 import BeautifulSoup, element
 import re
 import html2text
 import hashlib
 import base64
 from pymongo import MongoClient
+import oss2
 from parsel import Selector
 
 
 __all__ = [
     "base64_decode",
     "base64_encode",
     "bs_get_text",
@@ -78,34 +74,33 @@
     "oss2_find_file",
     "Panel",
     "parse_qs",
     "parse_qsl",
     "pdf2text",
     "pprint",
     "print",
-    "print_json",
     "print_exception",
     "printx",
     "Progress",
     "quote",
     "randint",
-    "random",
     "re",
     "read_json",
     "retry",
     "Rule",
     "send_bot",
     "sleep",
     "sleep_progress",
     "Status",
     "Selector",
     "Table",
     "time_next",
     "timeit",
     "timeparse",
+    "timeparse2",
     "timestamp",
     "to_excel",
     "to_json",
     "today",
     "tongji_content",
     "track",
     "ua",
@@ -117,16 +112,14 @@
     "urlparse",
     "urlsplit",
     "urlunsplit",
     "urlunparse",
     "wait",
 ]
 
-if timeparse2:
-    __all__.append("timeparse2")
 
 NON_BREAKING_ELEMENTS = [
     "a",
     "abbr",
     "acronym",
     "audio",
     "b",
@@ -812,28 +805,26 @@
         logger.success(f"MongoDB 成功连接到 {database}")
         return db
     except Exception as e:
         logger.error("MongoDB 连接失败:", str(e))
         return None
 
 
-def oss2_find_file(bucket, prefix, size1=0, size2=1048576000):
+def oss2_find_file(bucket: oss2.Bucket, prefix, size1=0, size2=1048576000):
     """
     寻找 oss 文件, 指定 size1 和 size2 可以筛选特定大小的文件。默认单位为 KB。返回值为字典。
 
     - 可以通过 len 统计文件数量。
     - 可以通过 sum 统计返回值字典的 values 统计文件夹文件的总大小, 单位为KB。
 
     bucket: oss2.Bucket 对象
     prefix: 文件夹路径, 例如 'etl/atk'
     size1: 文件大小下限,默认0
     size2: 文件大小上限,默认 1000G；如果需要筛选无用pdf, 可以设置上限20。
     """
-    import oss2
-
     if not isinstance(bucket, oss2.Bucket):
         print("bucket 不符合要求")
         return
     d = {}
     for obj in oss2.ObjectIterator(bucket, prefix):
         t = obj.size / 1024
         if size1 < t < size2 and not obj.is_prefix():
```

### Comparing `jsz-2024.5.13/src/jsz.egg-info/PKG-INFO` & `jsz-2024.5.9.2/src/jsz.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: jsz
-Version: 2024.5.13
+Version: 2024.5.9.2
 Summary: 金手指
 Author: jiaosenvip
 Author-email: jiaosenvip <jiaosenvip@163.com>
 License: MIT
-Project-URL: Homepage, https://github.com/jiaosenvip/jsz
+Project-URL: homepage, https://github.com/jiaosenvip/jsz
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: beautifulsoup4
 Requires-Dist: lxml
 Requires-Dist: rich
 Requires-Dist: oss2
 Requires-Dist: pymongo
 Requires-Dist: pypdf
 Requires-Dist: html2text
 Requires-Dist: faker
 Requires-Dist: python-dateutil
-Requires-Dist: dateparser; platform_machine != "aarch64"
+Requires-Dist: dateparser
 Requires-Dist: loguru
 Requires-Dist: grequests
 Requires-Dist: httpx
 Requires-Dist: jsonpath
 Requires-Dist: parsel
 Requires-Dist: ipython
 Requires-Dist: js2py
```

