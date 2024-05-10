# Comparing `tmp/vidsrc_search-0.2.4.tar.gz` & `tmp/vidsrc_search-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidsrc_search-0.2.4.tar", last modified: Tue Apr 16 20:02:59 2024, max compression
+gzip compressed data, was "vidsrc_search-0.2.5.tar", last modified: Fri May 10 17:28:19 2024, max compression
```

## Comparing `vidsrc_search-0.2.4.tar` & `vidsrc_search-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-16 20:02:59.502227 vidsrc_search-0.2.4/
--rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-04-15 17:13:28.000000 vidsrc_search-0.2.4/LICENSE
--rw-r--r--   0 Dev        (502) staff       (20)     2996 2024-04-16 20:02:59.501926 vidsrc_search-0.2.4/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)     2055 2024-04-16 07:34:13.000000 vidsrc_search-0.2.4/README.md
--rw-r--r--   0 Dev        (502) staff       (20)     1027 2024-04-16 02:37:13.000000 vidsrc_search-0.2.4/pyproject.toml
--rw-r--r--   0 Dev        (502) staff       (20)       38 2024-04-16 20:02:59.502297 vidsrc_search-0.2.4/setup.cfg
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-16 20:02:59.498072 vidsrc_search-0.2.4/src/
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-16 20:02:59.499738 vidsrc_search-0.2.4/src/vidsrc_search/
--rw-r--r--   0 Dev        (502) staff       (20)     1279 2024-04-16 19:24:15.000000 vidsrc_search-0.2.4/src/vidsrc_search/__main__.py
--rw-r--r--   0 Dev        (502) staff       (20)     2243 2024-04-16 02:57:09.000000 vidsrc_search-0.2.4/src/vidsrc_search/argparsing.py
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-16 20:02:59.501205 vidsrc_search-0.2.4/src/vidsrc_search/core/
--rw-r--r--   0 Dev        (502) staff       (20)     2884 2024-04-16 19:50:55.000000 vidsrc_search-0.2.4/src/vidsrc_search/core/help.py
--rw-r--r--   0 Dev        (502) staff       (20)    11007 2024-04-16 19:54:42.000000 vidsrc_search-0.2.4/src/vidsrc_search/core/library.py
--rw-r--r--   0 Dev        (502) staff       (20)    11526 2024-04-16 19:18:36.000000 vidsrc_search-0.2.4/src/vidsrc_search/core/search.py
--rw-r--r--   0 Dev        (502) staff       (20)      765 2024-04-16 19:17:32.000000 vidsrc_search-0.2.4/src/vidsrc_search/core/version.py
--rw-r--r--   0 Dev        (502) staff       (20)     1019 2024-04-16 19:17:40.000000 vidsrc_search-0.2.4/src/vidsrc_search/modules.py
--rw-r--r--   0 Dev        (502) staff       (20)     4946 2024-04-16 19:16:36.000000 vidsrc_search-0.2.4/src/vidsrc_search/term.py
--rw-r--r--   0 Dev        (502) staff       (20)     5874 2024-04-16 19:23:26.000000 vidsrc_search-0.2.4/src/vidsrc_search/utils.py
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-16 20:02:59.501663 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/
--rw-r--r--   0 Dev        (502) staff       (20)     2996 2024-04-16 20:02:59.000000 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)      556 2024-04-16 20:02:59.000000 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/SOURCES.txt
--rw-r--r--   0 Dev        (502) staff       (20)        1 2024-04-16 20:02:59.000000 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/dependency_links.txt
--rw-r--r--   0 Dev        (502) staff       (20)       62 2024-04-16 20:02:59.000000 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/entry_points.txt
--rw-r--r--   0 Dev        (502) staff       (20)       77 2024-04-16 20:02:59.000000 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/requires.txt
--rw-r--r--   0 Dev        (502) staff       (20)       14 2024-04-16 20:02:59.000000 vidsrc_search-0.2.4/src/vidsrc_search.egg-info/top_level.txt
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-05-10 17:28:19.354798 vidsrc_search-0.2.5/
+-rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-05-10 17:19:11.000000 vidsrc_search-0.2.5/LICENSE
+-rw-r--r--   0 Dev        (502) staff       (20)     2996 2024-05-10 17:28:19.354409 vidsrc_search-0.2.5/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)     2055 2024-05-10 17:19:11.000000 vidsrc_search-0.2.5/README.md
+-rw-r--r--   0 Dev        (502) staff       (20)     1027 2024-05-10 17:26:48.000000 vidsrc_search-0.2.5/pyproject.toml
+-rw-r--r--   0 Dev        (502) staff       (20)       38 2024-05-10 17:28:19.354870 vidsrc_search-0.2.5/setup.cfg
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-05-10 17:28:19.348381 vidsrc_search-0.2.5/src/
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-05-10 17:28:19.351162 vidsrc_search-0.2.5/src/vidsrc_search/
+-rw-r--r--   0 Dev        (502) staff       (20)     1279 2024-05-10 17:19:11.000000 vidsrc_search-0.2.5/src/vidsrc_search/__main__.py
+-rw-r--r--   0 Dev        (502) staff       (20)     2243 2024-05-10 17:19:11.000000 vidsrc_search-0.2.5/src/vidsrc_search/argparsing.py
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-05-10 17:28:19.353624 vidsrc_search-0.2.5/src/vidsrc_search/core/
+-rw-r--r--   0 Dev        (502) staff       (20)     2884 2024-05-10 17:19:11.000000 vidsrc_search-0.2.5/src/vidsrc_search/core/help.py
+-rw-r--r--   0 Dev        (502) staff       (20)    11249 2024-05-10 17:24:32.000000 vidsrc_search-0.2.5/src/vidsrc_search/core/library.py
+-rw-r--r--   0 Dev        (502) staff       (20)    11548 2024-05-10 17:25:35.000000 vidsrc_search-0.2.5/src/vidsrc_search/core/search.py
+-rw-r--r--   0 Dev        (502) staff       (20)      765 2024-05-10 17:26:38.000000 vidsrc_search-0.2.5/src/vidsrc_search/core/version.py
+-rw-r--r--   0 Dev        (502) staff       (20)     1019 2024-05-10 17:19:11.000000 vidsrc_search-0.2.5/src/vidsrc_search/modules.py
+-rw-r--r--   0 Dev        (502) staff       (20)     4901 2024-05-10 17:20:20.000000 vidsrc_search-0.2.5/src/vidsrc_search/term.py
+-rw-r--r--   0 Dev        (502) staff       (20)     5988 2024-05-10 17:22:14.000000 vidsrc_search-0.2.5/src/vidsrc_search/utils.py
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-05-10 17:28:19.353978 vidsrc_search-0.2.5/src/vidsrc_search.egg-info/
+-rw-r--r--   0 Dev        (502) staff       (20)     2996 2024-05-10 17:28:19.000000 vidsrc_search-0.2.5/src/vidsrc_search.egg-info/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)      556 2024-05-10 17:28:19.000000 vidsrc_search-0.2.5/src/vidsrc_search.egg-info/SOURCES.txt
+-rw-r--r--   0 Dev        (502) staff       (20)        1 2024-05-10 17:28:19.000000 vidsrc_search-0.2.5/src/vidsrc_search.egg-info/dependency_links.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       62 2024-05-10 17:28:19.000000 vidsrc_search-0.2.5/src/vidsrc_search.egg-info/entry_points.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       77 2024-05-10 17:28:19.000000 vidsrc_search-0.2.5/src/vidsrc_search.egg-info/requires.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       14 2024-05-10 17:28:19.000000 vidsrc_search-0.2.5/src/vidsrc_search.egg-info/top_level.txt
```

### Comparing `vidsrc_search-0.2.4/LICENSE` & `vidsrc_search-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vidsrc_search-0.2.4/PKG-INFO` & `vidsrc_search-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vidsrc-search
-Version: 0.2.4
+Version: 0.2.5
 Summary: A pirate movie watcher written in Python
 Project-URL: Homepage, https://github.com/SomedudeX/vidsrc-search
 Project-URL: License, https://github.com/SomedudeX/vidsrc-search/blob/main/LICENSE
 Project-URL: Changelog, https://github.com/SomedudeX/vidsrc-search/releases
 Keywords: movie,video,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `vidsrc_search-0.2.4/README.md` & `vidsrc_search-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `vidsrc_search-0.2.4/pyproject.toml` & `vidsrc_search-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vidsrc-search"
-version = "0.2.4"
+version = "0.2.5"
 description = "A pirate movie watcher written in Python"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `vidsrc_search-0.2.4/src/vidsrc_search/__main__.py` & `vidsrc_search-0.2.5/src/vidsrc_search/__main__.py`

 * *Files identical despite different names*

### Comparing `vidsrc_search-0.2.4/src/vidsrc_search/argparsing.py` & `vidsrc_search-0.2.5/src/vidsrc_search/argparsing.py`

 * *Files identical despite different names*

### Comparing `vidsrc_search-0.2.4/src/vidsrc_search/core/help.py` & `vidsrc_search-0.2.5/src/vidsrc_search/core/help.py`

 * *Files identical despite different names*

### Comparing `vidsrc_search-0.2.4/src/vidsrc_search/core/library.py` & `vidsrc_search-0.2.5/src/vidsrc_search/core/library.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     def set_description_str(*args, **kwargs) -> None: ...
     def update(*args, **kwargs) -> Union[bool, None]: ...
     def close(*args, **kwargs) -> None: ...
 
 
 class Library:
     """Properties of the library"""
-    root_path = os.path.expanduser("~/.local/vidsrc-search")
-    lib_path = os.path.expanduser("~/.local/vidsrc-search/lib.json")
-    cache_path = os.path.expanduser("~/.local/vidsrc-search/cache")
+    root_path = os.path.expanduser("~/.local/share/vidsrc-search")
+    lib_path = os.path.expanduser("~/.local/share/vidsrc-search/lib.json")
+    cache_path = os.path.expanduser("~/.local/share/vidsrc-search/cache")
 
     def check_library(
         self,
         exit_on_false: bool = True
     ) -> bool:
         """Checks whether the library exist or not"""
         if os.path.exists(self.lib_path):
@@ -104,21 +104,28 @@
 
         start_time = time.time()
         for item in self.types:
             size = self.get_download_size(item)
             asyncio.run(self.download(size, item))
 
             self.final_size += size * 15
-            self.expected_size += utils.unite_jsons(f"~/.local/vidsrc-search/{item}_buffer/", f"~/.local/vidsrc-search/{item}.json")
+            self.expected_size += utils.unite_jsons(
+                f"~/.local/share/vidsrc-search/{item}_buffer/", 
+                f"~/.local/share/vidsrc-search/{item}.json"
+            )
         end_time = time.time()
 
         self.progress.set_description_str("cleaning files")
         RemovalManager.remove_library()   # Removing previously downloaded library
         LogLibrary.log("moving new library in place")
-        utils.unite_jsons(f"~/.local/vidsrc-search/", f"~/.local/vidsrc-search/lib.json", raw=False)
+        utils.unite_jsons(
+            f"~/.local/share/vidsrc-search/", 
+            f"~/.local/share/vidsrc-search/lib.json", 
+            raw=False
+        )
 
         self.progress.update(1)
         self.time = end_time - start_time
         self.progress.set_description_str("library download complete")
         self.progress.close()
         return
 
@@ -129,15 +136,18 @@
             loss = 0
         print(f" • total number of links to movies downloaded: {self.expected_size}")
         print(f" • estimated link loss from connection issues: ~{loss:.2f}%")
         print(f" • operation took {self.time:.2f} seconds to complete")
         print(f" • vidsrc library has been downloaded")
         return
 
-    def get_download_size(self, kind: str) -> int:
+    def get_download_size(
+        self, 
+        kind: str
+    ) -> int:
         """Estimates the number of pages (links) of a download using binary
         search.
         """
         self.progress.set_description_str(f"calculating {kind} items")
         LogLibrary.log(f"starting download size estimation for {kind}")
 
         requests_errors = 0
@@ -170,31 +180,39 @@
             if len(file.content) < 50:
                 last_direction = this_direction
                 this_direction = -1
                 index += width * -1
         return index
 
     @staticmethod
-    async def fetch_downloads(session: aiohttp.ClientSession, url: str, _tries: int = 3) -> Union[Any, None]:
+    async def fetch_downloads(
+        session: aiohttp.ClientSession, 
+        url: str, 
+        _tries: int = 3
+    ) -> Union[Any, None]:
         """Asynchronously fetch a json file from a url, retrying if the response is not a json"""
         async with session.get(url) as response:
             if response.content_type == "application/json":
                 if _tries != 3:
                     LogLibrary.log(f"retry succesful")
                 return await response.json()
             LogLibrary.log(f"bad connection detected: retrying ({_tries})")
             if _tries != 0:
                 return await DownloadManager.fetch_downloads(session, url, _tries - 1)
             LogLibrary.log(f"too many retries: omitting current link")
             return
 
-    async def download(self, total: int, type: str):
+    async def download(
+        self, 
+        total: int, 
+        type: str
+    ):
         """Downloads the movie library into a buffer folder on disk"""
         domain = f"https://vidsrc.to/vapi/{type}/new/"
-        folder = f"~/.local/vidsrc-search/{type}_buffer/"
+        folder = f"~/.local/share/vidsrc-search/{type}_buffer/"
         urls = [f"{domain}{i}" for i in range(total)]
         LogLibrary.log(f"initiating downloads with {total} links to {type}s")
 
         self.progress.update(1)
         async with aiohttp.ClientSession() as session:
             self.progress.set_description_str("waiting for server responses")
             LogLibrary.log(f"adding fetch_downloads() tasks to task list")
@@ -229,17 +247,17 @@
         utils.rmdir_recurse(Library.cache_path)
         return
 
     @staticmethod
     def remove_buffer() -> None:
         """Removes the buffer storage"""
         LogLibrary.log(f"removing download buffering folders")
-        folders = utils.get_file(f"~/.local/vidsrc-search", "_buffer")
+        folders = utils.get_file(f"~/.local/share/vidsrc-search", "_buffer")
         for folder in folders:
-            utils.rmdir_recurse(f"~/.local/vidsrc-search/" + folder)
+            utils.rmdir_recurse(f"~/.local/share/vidsrc-search/" + folder)
         return
 
     def handle_remove_library(self) -> None:
         """Handles the removal of library"""
         LogLibrary.log(f"initiating handle_remove_libary()")
         if not os.path.exists(Library.lib_path):
             print(" • library does not exist")
```

### Comparing `vidsrc_search-0.2.4/src/vidsrc_search/core/search.py` & `vidsrc_search-0.2.5/src/vidsrc_search/core/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,19 +235,19 @@
 
         if self.raw:
             LogSearch.log("directly opening vidsrc link in browser")
             print(f" • opening '{title}' in new browser tab")
             webbrowser.open(url)
             return
 
-        if self.new or not os.path.exists(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html")):
-            SearchHandler.cache_movie(url, f"~/.local/vidsrc-search/cache/{id}.html")
-        SearchHandler.process_html(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"))
+        if self.new or not os.path.exists(os.path.expanduser(f"~/.local/share/vidsrc-search/cache/{id}.html")):
+            SearchHandler.cache_movie(url, f"~/.local/share/vidsrc-search/cache/{id}.html")
+        SearchHandler.process_html(os.path.expanduser(f"~/.local/share/vidsrc-search/cache/{id}.html"))
         print(f" • opening '{title}' in new browser tab")
-        webbrowser.open("file://" + os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"))
+        webbrowser.open("file://" + os.path.expanduser(f"~/.local/share/vidsrc-search/cache/{id}.html"))
         return
 
     def process_query(self) -> None:
         if len(self.query) < 1:
             return
         if self.query[0] == "'" and self.query[len(self.query) - 1] == "'":
             self.query = self.query[1:-1]
@@ -259,15 +259,15 @@
         print()
         print(" • warning: the content of the movie is hosted on a third party site. the")
         print("            site is not endorsed by the author or checked for its quality, ")
         print("            content, or authenticity. the author of vidsrc-search disclaims")
         print("            any responsibility, express or implied, of the consequences ")
         print("            as a result your usage or dependence on the website provided ")
         print("            through this tool. ")
-        print(" • warning: the following window shown will be the cached contents of vidsrc.to\n")
+        print(" • warning: the following window shown will be the cached contents of vidsrc.to")
         affirm = input(" > i have read and understood the conditions above (Y/n) ")
         print()
         if not affirm == "Y":
             print(" • terminating per user request")
             raise UserWarning
         return
```

### Comparing `vidsrc_search-0.2.4/src/vidsrc_search/core/version.py` & `vidsrc_search-0.2.5/src/vidsrc_search/core/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import platform
 
 from typing import Any, Dict, List
 
 from ..argparsing import ArgumentsError
 from ..term import Logger
 
-__version__ = "v0.2.4"
+__version__ = "v0.2.5"
 LogVersion = Logger()
 
 
 def print_version() -> None:
     """Prints system information and the version of the program"""
     print(f" • vidsrc-search {__version__}")
     print(f" • {platform.python_implementation().lower()} {platform.python_version().lower()}")
```

### Comparing `vidsrc_search-0.2.4/src/vidsrc_search/modules.py` & `vidsrc_search-0.2.5/src/vidsrc_search/modules.py`

 * *Files identical despite different names*

### Comparing `vidsrc_search-0.2.4/src/vidsrc_search/term.py` & `vidsrc_search-0.2.5/src/vidsrc_search/term.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# We do not have logging in term.py because
-
 import os
 import sys
 import inspect
 
 
 class CallerInfo:
     """The info of the caller of the function"""
```

### Comparing `vidsrc_search-0.2.4/src/vidsrc_search/utils.py` & `vidsrc_search-0.2.5/src/vidsrc_search/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,16 +62,17 @@
     return f"{total_size:.2f} {units[len(units) - 1]}"
 
 
 def cleanup() -> None:
     """Removes buffer directories created during the execution of the program"""
     LogUtils.log(f"performing program cleanup sequence")
     rmdir_recurse(os.path.expanduser("~/.config/pymovie")) # Pre v0.1.4 folder
-    rmfile("~/.local/vidsrc-search/movie.json")
-    rmfile("~/.local/vidsrc-search/tv.json")
+    rmdir_recurse(os.path.expanduser("~/.local/vidsrc-search")) # Pre v0.2.4 folder
+    rmfile("~/.local/share/vidsrc-search/movie.json")
+    rmfile("~/.local/share/vidsrc-search/tv.json")
     RemovalManager.remove_buffer()
     return
 
 
 def initialize(args: Dict[str, Any]) -> None:
     """Called when the program first starts. Prepares program for execution"""
     if args["dbg"]:
@@ -81,17 +82,17 @@
         from .term import enable_debug
 
         enable_debug()
         LogUtils.log(f"vidsrc-search {__version__}")
         LogUtils.log(f"{platform.python_implementation().lower()} {platform.python_version().lower()}")
         LogUtils.log(f"{platform.platform(True, True).lower()} {platform.machine().lower()}")
     LogUtils.log("initializing directories")
-    required_path_one = os.path.expanduser("~/.local/vidsrc-search/movie_buffer")
-    required_path_two = os.path.expanduser("~/.local/vidsrc-search/tv_buffer")
-    required_path_three = os.path.expanduser("~/.local/vidsrc-search/cache")
+    required_path_one = os.path.expanduser("~/.local/share/vidsrc-search/movie_buffer")
+    required_path_two = os.path.expanduser("~/.local/share/vidsrc-search/tv_buffer")
+    required_path_three = os.path.expanduser("~/.local/share/vidsrc-search/cache")
     os.makedirs(required_path_one, exist_ok=True)
     os.makedirs(required_path_two, exist_ok=True)
     os.makedirs(required_path_three, exist_ok=True)
 
     if sys.platform in ["win32", "cygwin", "msys"]:  # Windows has some issues with asyncio
         LogUtils.log("patching windows asyncio")
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
```

### Comparing `vidsrc_search-0.2.4/src/vidsrc_search.egg-info/PKG-INFO` & `vidsrc_search-0.2.5/src/vidsrc_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vidsrc-search
-Version: 0.2.4
+Version: 0.2.5
 Summary: A pirate movie watcher written in Python
 Project-URL: Homepage, https://github.com/SomedudeX/vidsrc-search
 Project-URL: License, https://github.com/SomedudeX/vidsrc-search/blob/main/LICENSE
 Project-URL: Changelog, https://github.com/SomedudeX/vidsrc-search/releases
 Keywords: movie,video,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `vidsrc_search-0.2.4/src/vidsrc_search.egg-info/SOURCES.txt` & `vidsrc_search-0.2.5/src/vidsrc_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

