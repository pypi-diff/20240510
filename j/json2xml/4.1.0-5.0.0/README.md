# Comparing `tmp/json2xml-4.1.0.tar.gz` & `tmp/json2xml-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json2xml-4.1.0.tar", last modified: Fri Nov 10 06:41:51 2023, max compression
+gzip compressed data, was "json2xml-5.0.0.tar", last modified: Fri May 10 19:20:13 2024, max compression
```

## Comparing `json2xml-4.1.0.tar` & `json2xml-5.0.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 06:41:51.102138 json2xml-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-11-10 06:41:32.000000 json2xml-4.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2023-11-10 06:41:32.000000 json2xml-4.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10098 2023-11-10 06:41:32.000000 json2xml-4.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)      583 2023-11-10 06:41:32.000000 json2xml-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-11-10 06:41:32.000000 json2xml-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16910 2023-11-10 06:41:51.102138 json2xml-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2023-11-10 06:41:32.000000 json2xml-4.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 06:41:51.098138 json2xml-4.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2023-11-10 06:41:32.000000 json2xml-4.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-10 06:41:32.000000 json2xml-4.1.0/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4840 2023-11-10 06:41:32.000000 json2xml-4.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-10 06:41:32.000000 json2xml-4.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-10 06:41:32.000000 json2xml-4.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-11-10 06:41:32.000000 json2xml-4.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-11-10 06:41:32.000000 json2xml-4.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-11-10 06:41:32.000000 json2xml-4.1.0/docs/json2xml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      770 2023-11-10 06:41:32.000000 json2xml-4.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-10 06:41:32.000000 json2xml-4.1.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-10 06:41:32.000000 json2xml-4.1.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-10 06:41:32.000000 json2xml-4.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 06:41:51.098138 json2xml-4.1.0/json2xml/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-11-10 06:41:32.000000 json2xml-4.1.0/json2xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20136 2023-11-10 06:41:32.000000 json2xml-4.1.0/json2xml/dicttoxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-11-10 06:41:32.000000 json2xml-4.1.0/json2xml/json2xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2023-11-10 06:41:32.000000 json2xml-4.1.0/json2xml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 06:41:51.098138 json2xml-4.1.0/json2xml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16910 2023-11-10 06:41:51.000000 json2xml-4.1.0/json2xml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-11-10 06:41:51.000000 json2xml-4.1.0/json2xml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-10 06:41:51.000000 json2xml-4.1.0/json2xml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-10 06:41:50.000000 json2xml-4.1.0/json2xml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-10 06:41:51.000000 json2xml-4.1.0/json2xml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-10 06:41:51.000000 json2xml-4.1.0/json2xml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-11-10 06:41:32.000000 json2xml-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-10 06:41:32.000000 json2xml-4.1.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-11-10 06:41:51.102138 json2xml-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2023-11-10 06:41:32.000000 json2xml-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 06:41:51.102138 json2xml-4.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-10 06:41:32.000000 json2xml-4.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14475 2023-11-10 06:41:32.000000 json2xml-4.1.0/tests/test_dict2xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2023-11-10 06:41:32.000000 json2xml-4.1.0/tests/test_json2xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:13.233901 json2xml-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-10 19:20:09.000000 json2xml-5.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-10 19:20:09.000000 json2xml-5.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-05-10 19:20:09.000000 json2xml-5.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-10 19:20:09.000000 json2xml-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 19:20:09.000000 json2xml-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16910 2024-05-10 19:20:13.233901 json2xml-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-10 19:20:09.000000 json2xml-5.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:13.233901 json2xml-5.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-10 19:20:09.000000 json2xml-5.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-10 19:20:09.000000 json2xml-5.0.0/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4840 2024-05-10 19:20:09.000000 json2xml-5.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-10 19:20:09.000000 json2xml-5.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-10 19:20:09.000000 json2xml-5.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-10 19:20:09.000000 json2xml-5.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-10 19:20:09.000000 json2xml-5.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-10 19:20:09.000000 json2xml-5.0.0/docs/json2xml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-10 19:20:09.000000 json2xml-5.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-10 19:20:09.000000 json2xml-5.0.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 19:20:09.000000 json2xml-5.0.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 19:20:09.000000 json2xml-5.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:13.233901 json2xml-5.0.0/json2xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-10 19:20:09.000000 json2xml-5.0.0/json2xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20141 2024-05-10 19:20:09.000000 json2xml-5.0.0/json2xml/dicttoxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-10 19:20:09.000000 json2xml-5.0.0/json2xml/json2xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-10 19:20:09.000000 json2xml-5.0.0/json2xml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:13.233901 json2xml-5.0.0/json2xml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16910 2024-05-10 19:20:13.000000 json2xml-5.0.0/json2xml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-10 19:20:13.000000 json2xml-5.0.0/json2xml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:20:13.000000 json2xml-5.0.0/json2xml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:20:13.000000 json2xml-5.0.0/json2xml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 19:20:13.000000 json2xml-5.0.0/json2xml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 19:20:13.000000 json2xml-5.0.0/json2xml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-10 19:20:09.000000 json2xml-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 19:20:09.000000 json2xml-5.0.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-10 19:20:13.233901 json2xml-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-10 19:20:09.000000 json2xml-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:20:13.233901 json2xml-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:20:09.000000 json2xml-5.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-05-10 19:20:09.000000 json2xml-5.0.0/tests/test_dict2xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-05-10 19:20:09.000000 json2xml-5.0.0/tests/test_json2xml.py
```

### Comparing `json2xml-4.1.0/CONTRIBUTING.rst` & `json2xml-5.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `json2xml-4.1.0/HISTORY.rst` & `json2xml-5.0.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `json2xml-4.1.0/LICENSE` & `json2xml-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `json2xml-4.1.0/PKG-INFO` & `json2xml-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json2xml
-Version: 4.1.0
+Version: 5.0.0
 Summary: Simple Python Library to convert JSON to XML
 Home-page: https://github.com/vinitkumar/json2xml
 Author: Vinit Kumar
 Author-email: mail@vinitkumar.me
 License: Apache Software License 2.0
 Keywords: json2xml
 Classifier: Development Status :: 6 - Mature
```

### Comparing `json2xml-4.1.0/README.rst` & `json2xml-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `json2xml-4.1.0/docs/Makefile` & `json2xml-5.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `json2xml-4.1.0/docs/conf.py` & `json2xml-5.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `json2xml-4.1.0/docs/installation.rst` & `json2xml-5.0.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `json2xml-4.1.0/docs/json2xml.rst` & `json2xml-5.0.0/docs/json2xml.rst`

 * *Files identical despite different names*

### Comparing `json2xml-4.1.0/docs/make.bat` & `json2xml-5.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `json2xml-4.1.0/json2xml/dicttoxml.py` & `json2xml-5.0.0/json2xml/dicttoxml.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,19 +55,19 @@
 
 ELEMENT = Union[
     str,
     int,
     float,
     bool,
     numbers.Number,
-    Sequence,
+    Sequence[str],
     datetime.datetime,
     datetime.date,
     None,
-    Dict[str, Any],
+    dict[str, Any],
 ]
 
 
 def get_xml_type(val: ELEMENT) -> str:
     """
     Get the XML type of a given value.
```

### Comparing `json2xml-4.1.0/json2xml/json2xml.py` & `json2xml-5.0.0/json2xml/json2xml.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 
 class Json2xml:
     """
     Wrapper class to convert the data to xml
     """
     def __init__(
         self,
-        data: Optional[Dict[str, Any]] = None,
+        data: dict[str, Any] | None = None,
         wrapper: str = "all",
         root: bool = True,
         pretty: bool = True,
         attr_type: bool = True,
         item_wrap: bool = True,
     ):
         self.data = data
         self.pretty = pretty
         self.wrapper = wrapper
         self.attr_type = attr_type
         self.root = root
         self.item_wrap = item_wrap
 
-    def to_xml(self) -> Optional[Any]:
+    def to_xml(self) -> Any | None:
         """
         Convert to xml using dicttoxml.dicttoxml and then pretty print it.
         """
         if self.data:
             xml_data = dicttoxml.dicttoxml(
                 self.data,
                 root=self.root,
```

### Comparing `json2xml-4.1.0/json2xml/utils.py` & `json2xml-5.0.0/json2xml/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,35 +21,35 @@
 
 
 class StringReadError(Exception):
     """Raised when there is an error reading from a string."""
     pass
 
 
-def readfromjson(filename: str) -> Dict[str, str]:
+def readfromjson(filename: str) -> dict[str, str]:
     """Reads a JSON file and returns a dictionary."""
     try:
         with open(filename, encoding="utf-8") as jsondata:
             return json.load(jsondata)
     except ValueError:
         raise JSONReadError("Invalid JSON File")
     except OSError:
         raise JSONReadError("Invalid JSON File")
 
 
-def readfromurl(url: str, params: Optional[Dict[str, str]] = None) -> Dict[str, str]:
+def readfromurl(url: str, params: dict[str, str] | None = None) -> dict[str, str]:
     """Loads JSON data from a URL and returns a dictionary."""
     http = urllib3.PoolManager()
     response = http.request("GET", url, fields=params)
     if response.status == 200:
         return json.loads(response.data.decode('utf-8'))
     raise URLReadError("URL is not returning correct response")
 
 
-def readfromstring(jsondata: str) -> Dict[str, str]:
+def readfromstring(jsondata: str) -> dict[str, str]:
     """Loads JSON data from a string and returns a dictionary."""
     if not isinstance(jsondata, str):
         raise StringReadError("Input is not a proper JSON string")
     try:
         return json.loads(jsondata)
     except ValueError:
         raise StringReadError("Input is not a proper JSON string")
```

### Comparing `json2xml-4.1.0/json2xml.egg-info/PKG-INFO` & `json2xml-5.0.0/json2xml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json2xml
-Version: 4.1.0
+Version: 5.0.0
 Summary: Simple Python Library to convert JSON to XML
 Home-page: https://github.com/vinitkumar/json2xml
 Author: Vinit Kumar
 Author-email: mail@vinitkumar.me
 License: Apache Software License 2.0
 Keywords: json2xml
 Classifier: Development Status :: 6 - Mature
```

### Comparing `json2xml-4.1.0/json2xml.egg-info/SOURCES.txt` & `json2xml-5.0.0/json2xml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `json2xml-4.1.0/setup.cfg` & `json2xml-5.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `json2xml-4.1.0/setup.py` & `json2xml-5.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `json2xml-4.1.0/tests/test_dict2xml.py` & `json2xml-5.0.0/tests/test_dict2xml.py`

 * *Files identical despite different names*

### Comparing `json2xml-4.1.0/tests/test_json2xml.py` & `json2xml-5.0.0/tests/test_json2xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,23 +46,14 @@
         assert pytest_wrapped_e.type == JSONReadError
 
     def test_read_from_invalid_json2(self):
         with pytest.raises(JSONReadError) as pytest_wrapped_e:
             readfromjson("examples/wrongjson.json")
         assert pytest_wrapped_e.type == JSONReadError
 
-    def test_read_from_url(self):
-        data = readfromurl("https://api.publicapis.org/entries")
-        assert isinstance(data, dict)
-
-    def test_read_from_wrong_url(self):
-        with pytest.raises(URLReadError) as pytest_wrapped_e:
-            readfromurl("https://api.publicapis.org/entriesi")
-        assert pytest_wrapped_e.type == URLReadError
-
     def test_read_from_jsonstring(self):
         data = readfromstring(
             '{"login":"mojombo","id":1,"avatar_url":"https://avatars0.githubusercontent.com/u/1?v=4"}'
         )
         assert isinstance(data, dict)
 
     def test_read_from_invalid_string1(self):
```

