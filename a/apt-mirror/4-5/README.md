# Comparing `tmp/apt-mirror-4.tar.gz` & `tmp/apt_mirror-5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apt-mirror-4.tar", last modified: Sat Apr  6 12:46:47 2024, max compression
+gzip compressed data, was "apt_mirror-5.tar", last modified: Thu May  9 14:32:09 2024, max compression
```

## Comparing `apt-mirror-4.tar` & `apt_mirror-5.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 12:46:47.563371 apt-mirror-4/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2024-04-06 12:46:36.000000 apt-mirror-4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    45480 2024-04-06 12:46:47.563371 apt-mirror-4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3476 2024-04-06 12:46:36.000000 apt-mirror-4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 12:46:47.558371 apt-mirror-4/apt_mirror/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25466 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/apt_mirror.py
--rw-rw-rw-   0 root         (0) root         (0)    18418 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 12:46:47.560371 apt-mirror-4/apt_mirror/download/
--rw-rw-rw-   0 root         (0) root         (0)      491 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5120 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/download_file.py
--rw-rw-rw-   0 root         (0) root         (0)    15148 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/downloader.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 12:46:47.561371 apt-mirror-4/apt_mirror/download/protocols/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/protocols/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5040 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/protocols/ftp.py
--rw-rw-rw-   0 root         (0) root         (0)     4204 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/protocols/http.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/response.py
--rw-rw-rw-   0 root         (0) root         (0)     2312 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/download/url.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/logs.py
--rw-rw-rw-   0 root         (0) root         (0)     2722 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/prometheus.py
--rw-rw-rw-   0 root         (0) root         (0)    28434 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/repository.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2024-04-06 12:46:36.000000 apt-mirror-4/apt_mirror/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 12:46:47.562371 apt-mirror-4/apt_mirror.egg-info/
--rw-r--r--   0 root         (0) root         (0)    45480 2024-04-06 12:46:47.000000 apt-mirror-4/apt_mirror.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      845 2024-04-06 12:46:47.000000 apt-mirror-4/apt_mirror.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 12:46:47.000000 apt-mirror-4/apt_mirror.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-04-06 12:46:47.000000 apt-mirror-4/apt_mirror.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      250 2024-04-06 12:46:47.000000 apt-mirror-4/apt_mirror.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-06 12:46:47.000000 apt-mirror-4/apt_mirror.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2127 2024-04-06 12:46:36.000000 apt-mirror-4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-06 12:46:47.564371 apt-mirror-4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      104 2024-04-06 12:46:36.000000 apt-mirror-4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 12:46:47.562371 apt-mirror-4/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1141 2024-04-06 12:46:36.000000 apt-mirror-4/tests/test_clean.py
--rw-rw-rw-   0 root         (0) root         (0)     8286 2024-04-06 12:46:36.000000 apt-mirror-4/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-04-06 12:46:36.000000 apt-mirror-4/tests/test_download.py
--rw-rw-rw-   0 root         (0) root         (0)     2979 2024-04-06 12:46:36.000000 apt-mirror-4/tests/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 14:32:09.269260 apt_mirror-5/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2024-05-09 14:31:55.000000 apt_mirror-5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    45766 2024-05-09 14:32:09.269260 apt_mirror-5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3684 2024-05-09 14:31:55.000000 apt_mirror-5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 14:32:09.261260 apt_mirror-5/apt_mirror/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/aiofile.py
+-rw-rw-rw-   0 root         (0) root         (0)    25895 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/apt_mirror.py
+-rw-rw-rw-   0 root         (0) root         (0)    18578 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 14:32:09.265260 apt_mirror-5/apt_mirror/download/
+-rw-rw-rw-   0 root         (0) root         (0)      491 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5120 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/download/download_file.py
+-rw-rw-rw-   0 root         (0) root         (0)    15146 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/download/downloader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/download/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 14:32:09.266260 apt_mirror-5/apt_mirror/download/protocols/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/download/protocols/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5040 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/download/protocols/ftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4204 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/download/protocols/http.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/download/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/download/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2312 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/download/url.py
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/logs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/prometheus.py
+-rw-rw-rw-   0 root         (0) root         (0)    28895 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2024-05-09 14:31:55.000000 apt_mirror-5/apt_mirror/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 14:32:09.267260 apt_mirror-5/apt_mirror.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    45766 2024-05-09 14:32:09.000000 apt_mirror-5/apt_mirror.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      867 2024-05-09 14:32:09.000000 apt_mirror-5/apt_mirror.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 14:32:09.000000 apt_mirror-5/apt_mirror.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-09 14:32:09.000000 apt_mirror-5/apt_mirror.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-09 14:32:09.000000 apt_mirror-5/apt_mirror.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-09 14:32:09.000000 apt_mirror-5/apt_mirror.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2024-05-09 14:31:55.000000 apt_mirror-5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-05-09 14:32:09.270260 apt_mirror-5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      104 2024-05-09 14:31:55.000000 apt_mirror-5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 14:32:09.267260 apt_mirror-5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1141 2024-05-09 14:31:55.000000 apt_mirror-5/tests/test_clean.py
+-rw-rw-rw-   0 root         (0) root         (0)     8286 2024-05-09 14:31:55.000000 apt_mirror-5/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-09 14:31:55.000000 apt_mirror-5/tests/test_download.py
+-rw-rw-rw-   0 root         (0) root         (0)     5295 2024-05-09 14:31:55.000000 apt_mirror-5/tests/test_repository.py
```

### Comparing `apt-mirror-4/LICENSE` & `apt_mirror-5/LICENSE`

 * *Files identical despite different names*

### Comparing `apt-mirror-4/PKG-INFO` & `apt_mirror-5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apt-mirror
-Version: 4
+Version: 5
 Summary: apt-mirror Python reimplementation
 Author-email: Yuri Konotopov <ykonotopov@gnome.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,27 +696,32 @@
 Requires-Dist: aioftp==0.21.4
 Requires-Dist: httpx[http2]==0.26.0
 Requires-Dist: python-debian==0.1.49
 Provides-Extra: dev
 Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: flake8==6.0.0; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
-Requires-Dist: pip-tools==7.0.0; extra == "dev"
+Requires-Dist: pip-tools==7.4.1; extra == "dev"
 Requires-Dist: pylint==3.0.3; extra == "dev"
 Requires-Dist: pytest==7.4.4; extra == "dev"
+Provides-Extra: aiofiles
+Requires-Dist: aiofiles==23.2.1; extra == "aiofiles"
 Provides-Extra: prometheus
 Requires-Dist: prometheus-client==0.20.0; extra == "prometheus"
 Provides-Extra: uvloop
 Requires-Dist: uvloop==0.19.0; extra == "uvloop"
 
 # apt-mirror2
 
 [`apt-mirror2`](https://gitlab.com/apt-mirror2/apt-mirror2) is the Python/asyncio reimplementation of the
 [apt-mirror](https://github.com/apt-mirror/apt-mirror) developed as drop-in replacement for the latest.  
-This project should be suitable as general [apt-mirror](https://github.com/apt-mirror/apt-mirror) replacement.
+This project should be suitable as general [apt-mirror](https://github.com/apt-mirror/apt-mirror) replacement.  
+
+One of the main advantages of the `apt-mirror2` over the `apt-mirror` - you should never got broken mirror in case `apt-mirror2` returns 0 exit code.
+This is ensured by data integrity checks at all stages of mirroring.
 
 # Requirements
 
 Python 3.10 is the minimum supported version.  
 For additional dependencies look to the `pyproject.yml` and/or `requirements.txt`.
 
 # Installation
@@ -774,15 +779,15 @@
   configfile  Path to config file. Default /etc/apt/mirror.list
 
 options:
   -h, --help  show this help message and exit
   --version   Show version
 ```
 
-# apt-mirror configuration compatibility
+# apt-mirror compatibility
 
 Most of `apt-mirror` configuration directives are supported.  
 As of now proxy for FTP repositories is not supported.  
 
 File lists (ALL, NEW, MD5, SHA256, SHA512) are not written by default, but you can enable them with the `write_file_lists` option.
 
 In addition there are some enhancements available:
```

### Comparing `apt-mirror-4/README.md` & `apt_mirror-5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # apt-mirror2
 
 [`apt-mirror2`](https://gitlab.com/apt-mirror2/apt-mirror2) is the Python/asyncio reimplementation of the
 [apt-mirror](https://github.com/apt-mirror/apt-mirror) developed as drop-in replacement for the latest.  
-This project should be suitable as general [apt-mirror](https://github.com/apt-mirror/apt-mirror) replacement.
+This project should be suitable as general [apt-mirror](https://github.com/apt-mirror/apt-mirror) replacement.  
+
+One of the main advantages of the `apt-mirror2` over the `apt-mirror` - you should never got broken mirror in case `apt-mirror2` returns 0 exit code.
+This is ensured by data integrity checks at all stages of mirroring.
 
 # Requirements
 
 Python 3.10 is the minimum supported version.  
 For additional dependencies look to the `pyproject.yml` and/or `requirements.txt`.
 
 # Installation
@@ -64,15 +67,15 @@
   configfile  Path to config file. Default /etc/apt/mirror.list
 
 options:
   -h, --help  show this help message and exit
   --version   Show version
 ```
 
-# apt-mirror configuration compatibility
+# apt-mirror compatibility
 
 Most of `apt-mirror` configuration directives are supported.  
 As of now proxy for FTP repositories is not supported.  
 
 File lists (ALL, NEW, MD5, SHA256, SHA512) are not written by default, but you can enable them with the `write_file_lists` option.
 
 In addition there are some enhancements available:
```

### Comparing `apt-mirror-4/apt_mirror/apt_mirror.py` & `apt_mirror-5/apt_mirror/apt_mirror.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,35 +272,45 @@
                 - self._downloader.get_missing_sources(),
             )
 
             # Download remaining pool
             await self.download_pool_files()
 
             # Move skel to mirror
-            await self.move_metadata(downloaded_metadata_files)
+            if not self._error:
+                await self.move_metadata(downloaded_metadata_files)
+            else:
+                self._log.warning(
+                    "Metadata movement skipped because of download errors"
+                )
 
             if self._repository.clean:
-                await self.clean_repository(
-                    needed_files=self._downloader.get_downloaded_files_paths(),
-                    unlink=self._config.autoclean,
-                )
+                if not self._error:
+                    await self.clean_repository(
+                        needed_files=self._downloader.get_downloaded_files_paths(),
+                        unlink=self._config.autoclean,
+                    )
+                else:
+                    self._log.warning(
+                        "Repository cleanup skipped because of download errors"
+                    )
 
             self._log.info(f"Repository {self._repository} mirroring complete")
 
         return not self._error
 
     async def download_release_files(self) -> Sequence[DownloadFile]:
         # Download release files
         self._log.info(f"Downloading release files for repository {self._repository}")
         release_files = [
             DownloadFile.from_path(path, ignore_missing=True)
             for path in self._repository.release_files
         ]
 
-        tries = 15
+        tries = self._config.release_files_retries
         while True:
             self._downloader.reset_paths()
             self._downloader.add(*release_files)
             await self._downloader.download()
 
             # Drop release files in skel which we were unable to download
             downloaded_paths = self._downloader.get_downloaded_files_paths()
```

### Comparing `apt-mirror-4/apt_mirror/config.py` & `apt_mirror-5/apt_mirror/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,14 +259,15 @@
             "no_check_certificate": "0",
             "certificate": "",
             "private_key": "",
             "ca_certificate": "",
             "prometheus_enable": "off",
             "prometheus_host": "localhost",
             "prometheus_port": "8000",
+            "release_files_retries": "15",
         }
 
         self._parse_config_file()
         self._substitute_variables()
 
     def _parse_config_file(self):
         clean: list[str] = []
@@ -540,7 +541,11 @@
     @property
     def prometheus_host(self) -> str:
         return self["prometheus_host"]
 
     @property
     def prometheus_port(self) -> int:
         return int(self["prometheus_port"])
+
+    @property
+    def release_files_retries(self) -> int:
+        return max(1, int(self["release_files_retries"]))
```

### Comparing `apt-mirror-4/apt_mirror/download/download_file.py` & `apt_mirror-5/apt_mirror/download/download_file.py`

 * *Files identical despite different names*

### Comparing `apt-mirror-4/apt_mirror/download/downloader.py` & `apt_mirror-5/apt_mirror/download/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import shutil
 from abc import ABC, abstractmethod
 from contextlib import asynccontextmanager
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Any, AsyncGenerator
 
-from aiofile import async_open
 from aiolimiter import AsyncLimiter
 
+from ..aiofile import AsyncIOFile
 from ..logs import LoggerFactory
 from .download_file import DownloadFile, DownloadFileCompressionVariant
 from .proxy import Proxy
 from .response import DownloadResponse
 from .url import URL
 
 
@@ -326,15 +326,15 @@
                                 variant.get_all_paths()
                             )
 
                             return
 
                         size = 0
                         target_path.unlink(missing_ok=True)
-                        async with async_open(target_path, "wb") as fp:
+                        async with AsyncIOFile(target_path) as fp:
                             try:
                                 async for chunk in response.stream():
                                     if self._rate_limiter:
                                         await self._rate_limiter.acquire(
                                             min(len(chunk), self._rate_limiter.max_rate)
                                         )
```

### Comparing `apt-mirror-4/apt_mirror/download/factory.py` & `apt_mirror-5/apt_mirror/download/factory.py`

 * *Files identical despite different names*

### Comparing `apt-mirror-4/apt_mirror/download/protocols/ftp.py` & `apt_mirror-5/apt_mirror/download/protocols/ftp.py`

 * *Files identical despite different names*

### Comparing `apt-mirror-4/apt_mirror/download/protocols/http.py` & `apt_mirror-5/apt_mirror/download/protocols/http.py`

 * *Files identical despite different names*

### Comparing `apt-mirror-4/apt_mirror/download/proxy.py` & `apt_mirror-5/apt_mirror/download/proxy.py`

 * *Files identical despite different names*

### Comparing `apt-mirror-4/apt_mirror/download/response.py` & `apt_mirror-5/apt_mirror/download/response.py`

 * *Files identical despite different names*

### Comparing `apt-mirror-4/apt_mirror/download/url.py` & `apt_mirror-5/apt_mirror/download/url.py`

 * *Files identical despite different names*

### Comparing `apt-mirror-4/apt_mirror/logs.py` & `apt_mirror-5/apt_mirror/logs.py`

 * *Files identical despite different names*

### Comparing `apt-mirror-4/apt_mirror/prometheus.py` & `apt_mirror-5/apt_mirror/prometheus.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,21 @@
         pass
 
 
 try:
     from prometheus_client import Metric, start_http_server
     from prometheus_client.core import REGISTRY, GaugeMetricFamily
     from prometheus_client.registry import Collector
+except ImportError:
+
+    class DownloaderCollector(BaseDownloaderCollector):
+        def collect(self):
+            yield
+
+else:
 
     class DownloaderCollector(BaseDownloaderCollector, Collector):  # type: ignore
         def __init__(self, address: str, port: int) -> None:
             super().__init__(address, port)
 
             self._wsgi_server, self._wsgi_thread = start_http_server(
                 port=port, addr=address
@@ -73,13 +80,7 @@
             yield self._metric("downloaded_files_size")
             yield self._metric("error_files_count")
             yield self._metric("error_files_size")
             yield self._metric("missing_files_count")
             yield self._metric("missing_files_size")
             yield self._metric("unmodified_files_count")
             yield self._metric("unmodified_files_size")
-
-except ImportError:
-
-    class DownloaderCollector(BaseDownloaderCollector):
-        def collect(self):
-            yield
```

### Comparing `apt-mirror-4/apt_mirror/repository.py` & `apt_mirror-5/apt_mirror/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -650,29 +650,35 @@
         # Skip binary metadata if not needed
         if not codename.should_mirror_binaries() and any(
             part in file_path_str for part in ("/binary-", "/cnf/", "/dep11/", "/i18n/")
         ):
             return False
 
         # Skip redundand components
-        if file_path_str.count("/") >= 2:
-            file_component, _, _ = file_path_str.rsplit("/", maxsplit=2)
+        components_split = min(file_path_str.count("/"), 2)
+        if components_split >= 1:
+            file_component = file_path_str.rsplit("/", maxsplit=components_split)[0]
 
             if not any(
                 file_component == component.name
                 for component in codename.components.values()
             ):
                 return False
 
             if (
                 "/binary-" in file_path_str
                 and "source" not in file_path_str
-                and not any(
-                    arch in file_path_str
-                    for arch in codename.components[file_component].arches
+                and (
+                    not codename.should_mirror_binaries()
+                    or not any(
+                        arch in file_path_str
+                        for arch in itertools.chain(
+                            codename.components[file_component].arches, ["-all"]
+                        )
+                    )
                 )
             ):
                 return False
 
         all_arches = set(
             arch
             for component in codename.components.values()
@@ -685,14 +691,21 @@
                 for suffix in ("Commands-", "Components-", "Contents-")
             )
             and "source" not in file_path.name
             and not any(arch in file_path.name for arch in all_arches)
         ):
             return False
 
+        if (
+            "Contents-" in file_path_str
+            and ".diff" in file_path_str
+            and not any(arch in file_path.name for arch in all_arches)
+        ):
+            return False
+
         # Allow any metadata not explicitly disallowed
         return True
 
     @property
     def is_source_enabled(self) -> bool:
         return any(c.should_mirror_source() for c in self.codenames.values())
```

### Comparing `apt-mirror-4/apt_mirror.egg-info/PKG-INFO` & `apt_mirror-5/apt_mirror.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apt-mirror
-Version: 4
+Version: 5
 Summary: apt-mirror Python reimplementation
 Author-email: Yuri Konotopov <ykonotopov@gnome.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,27 +696,32 @@
 Requires-Dist: aioftp==0.21.4
 Requires-Dist: httpx[http2]==0.26.0
 Requires-Dist: python-debian==0.1.49
 Provides-Extra: dev
 Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: flake8==6.0.0; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
-Requires-Dist: pip-tools==7.0.0; extra == "dev"
+Requires-Dist: pip-tools==7.4.1; extra == "dev"
 Requires-Dist: pylint==3.0.3; extra == "dev"
 Requires-Dist: pytest==7.4.4; extra == "dev"
+Provides-Extra: aiofiles
+Requires-Dist: aiofiles==23.2.1; extra == "aiofiles"
 Provides-Extra: prometheus
 Requires-Dist: prometheus-client==0.20.0; extra == "prometheus"
 Provides-Extra: uvloop
 Requires-Dist: uvloop==0.19.0; extra == "uvloop"
 
 # apt-mirror2
 
 [`apt-mirror2`](https://gitlab.com/apt-mirror2/apt-mirror2) is the Python/asyncio reimplementation of the
 [apt-mirror](https://github.com/apt-mirror/apt-mirror) developed as drop-in replacement for the latest.  
-This project should be suitable as general [apt-mirror](https://github.com/apt-mirror/apt-mirror) replacement.
+This project should be suitable as general [apt-mirror](https://github.com/apt-mirror/apt-mirror) replacement.  
+
+One of the main advantages of the `apt-mirror2` over the `apt-mirror` - you should never got broken mirror in case `apt-mirror2` returns 0 exit code.
+This is ensured by data integrity checks at all stages of mirroring.
 
 # Requirements
 
 Python 3.10 is the minimum supported version.  
 For additional dependencies look to the `pyproject.yml` and/or `requirements.txt`.
 
 # Installation
@@ -774,15 +779,15 @@
   configfile  Path to config file. Default /etc/apt/mirror.list
 
 options:
   -h, --help  show this help message and exit
   --version   Show version
 ```
 
-# apt-mirror configuration compatibility
+# apt-mirror compatibility
 
 Most of `apt-mirror` configuration directives are supported.  
 As of now proxy for FTP repositories is not supported.  
 
 File lists (ALL, NEW, MD5, SHA256, SHA512) are not written by default, but you can enable them with the `write_file_lists` option.
 
 In addition there are some enhancements available:
```

### Comparing `apt-mirror-4/apt_mirror.egg-info/SOURCES.txt` & `apt_mirror-5/apt_mirror.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 apt_mirror/__init__.py
+apt_mirror/aiofile.py
 apt_mirror/apt_mirror.py
 apt_mirror/config.py
 apt_mirror/logs.py
 apt_mirror/prometheus.py
 apt_mirror/repository.py
 apt_mirror/version.py
 apt_mirror.egg-info/PKG-INFO
```

### Comparing `apt-mirror-4/pyproject.toml` & `apt_mirror-5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apt-mirror"
-version = "4"
+version = "5"
 authors = [
     {name = "Yuri Konotopov", email = "ykonotopov@gnome.org"},
 ]
 description = "apt-mirror Python reimplementation"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["apt", "debian"]
@@ -28,18 +28,21 @@
 ]
 
 [project.optional-dependencies]
 dev = [
     "black==24.3.0",
     "flake8==6.0.0",
     "isort==5.12.0",
-    "pip-tools==7.0.0",
+    "pip-tools==7.4.1",
     "pylint==3.0.3",
     "pytest==7.4.4",
 ]
+aiofiles = [
+    "aiofiles==23.2.1"
+]
 prometheus = [
     "prometheus-client==0.20.0"
 ]
 uvloop = [
     "uvloop==0.19.0",
 ]
```

### Comparing `apt-mirror-4/tests/test_clean.py` & `apt_mirror-5/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `apt-mirror-4/tests/test_config.py` & `apt_mirror-5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `apt-mirror-4/tests/test_download.py` & `apt_mirror-5/tests/test_download.py`

 * *Files identical despite different names*

