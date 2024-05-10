# Comparing `tmp/nexus_scraper-0.2.0.tar.gz` & `tmp/nexus_scraper-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus_scraper-0.2.0.tar", max compression
+gzip compressed data, was "nexus_scraper-0.2.2.tar", max compression
```

## Comparing `nexus_scraper-0.2.0.tar` & `nexus_scraper-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2024-05-03 04:37:29.166091 nexus_scraper-0.2.0/LICENSE
--rw-r--r--   0        0        0     1540 2024-05-06 05:59:50.677752 nexus_scraper-0.2.0/Nexus/__init__.py
--rw-r--r--   0        0        0      832 2024-05-06 05:51:40.167842 nexus_scraper-0.2.0/Nexus/exceptions.py
--rw-r--r--   0        0        0     4317 2024-05-07 11:58:16.129014 nexus_scraper-0.2.0/Nexus/models.py
--rw-r--r--   0        0        0     5043 2024-05-07 21:12:53.192842 nexus_scraper-0.2.0/Nexus/scraper.py
--rw-r--r--   0        0        0        0 2024-05-04 17:38:42.456288 nexus_scraper-0.2.0/Nexus/scrapers/__init__.py
--rw-r--r--   0        0        0     2718 2024-05-07 11:56:49.419030 nexus_scraper-0.2.0/Nexus/scrapers/annatar.py
--rw-r--r--   0        0        0     2731 2024-05-07 11:57:08.859026 nexus_scraper-0.2.0/Nexus/scrapers/jackett.py
--rw-r--r--   0        0        0     5245 2024-05-07 22:35:06.623835 nexus_scraper-0.2.0/Nexus/scrapers/orionoid.py
--rw-r--r--   0        0        0     3862 2024-05-07 11:57:22.469024 nexus_scraper-0.2.0/Nexus/scrapers/prowlarr.py
--rw-r--r--   0        0        0     2185 2024-05-07 11:57:29.909022 nexus_scraper-0.2.0/Nexus/scrapers/torbox.py
--rw-r--r--   0        0        0     2572 2024-05-07 11:58:35.879011 nexus_scraper-0.2.0/Nexus/scrapers/torrentio.py
--rw-r--r--   0        0        0       14 2024-05-03 04:37:29.166091 nexus_scraper-0.2.0/README.md
--rw-r--r--   0        0        0      594 2024-05-07 22:43:27.673742 nexus_scraper-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 nexus_scraper-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-03 04:37:29.166091 nexus_scraper-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1540 2024-05-06 05:59:50.677752 nexus_scraper-0.2.2/Nexus/__init__.py
+-rw-r--r--   0        0        0      832 2024-05-06 05:51:40.167842 nexus_scraper-0.2.2/Nexus/exceptions.py
+-rw-r--r--   0        0        0     4317 2024-05-07 11:58:16.129014 nexus_scraper-0.2.2/Nexus/models.py
+-rw-r--r--   0        0        0     4783 2024-05-09 05:38:52.766485 nexus_scraper-0.2.2/Nexus/scraper.py
+-rw-r--r--   0        0        0        0 2024-05-04 17:38:42.456288 nexus_scraper-0.2.2/Nexus/scrapers/__init__.py
+-rw-r--r--   0        0        0     2718 2024-05-07 11:56:49.419030 nexus_scraper-0.2.2/Nexus/scrapers/annatar.py
+-rw-r--r--   0        0        0     2691 2024-05-09 05:33:49.846542 nexus_scraper-0.2.2/Nexus/scrapers/jackett.py
+-rw-r--r--   0        0        0     5245 2024-05-07 22:35:06.623835 nexus_scraper-0.2.2/Nexus/scrapers/orionoid.py
+-rw-r--r--   0        0        0     3812 2024-05-09 05:33:32.846546 nexus_scraper-0.2.2/Nexus/scrapers/prowlarr.py
+-rw-r--r--   0        0        0     2185 2024-05-07 11:57:29.909022 nexus_scraper-0.2.2/Nexus/scrapers/torbox.py
+-rw-r--r--   0        0        0     2572 2024-05-07 11:58:35.879011 nexus_scraper-0.2.2/Nexus/scrapers/torrentio.py
+-rw-r--r--   0        0        0       14 2024-05-03 04:37:29.166091 nexus_scraper-0.2.2/README.md
+-rw-r--r--   0        0        0      594 2024-05-09 05:43:44.016430 nexus_scraper-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 nexus_scraper-0.2.2/PKG-INFO
```

### Comparing `nexus_scraper-0.2.0/LICENSE` & `nexus_scraper-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nexus_scraper-0.2.0/Nexus/__init__.py` & `nexus_scraper-0.2.2/Nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `nexus_scraper-0.2.0/Nexus/exceptions.py` & `nexus_scraper-0.2.2/Nexus/exceptions.py`

 * *Files identical despite different names*

### Comparing `nexus_scraper-0.2.0/Nexus/models.py` & `nexus_scraper-0.2.2/Nexus/models.py`

 * *Files identical despite different names*

### Comparing `nexus_scraper-0.2.0/Nexus/scraper.py` & `nexus_scraper-0.2.2/Nexus/scraper.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,21 +48,17 @@
         Returns:
         - A list of `ScrapeResult` objects.
         """
         if not query:
             raise NexusException("Query cannot be empty")
 
         if source not in self.scrapers:
-            if query.startswith("tt"):
-                return self.imdb_scrapers["torrentio"].scrape(query, **kwargs)
-            else:
-                return self.raw_scrapers["torbox"].scrape(query, **kwargs)
-        if query.startswith("tt"):
-            return self.imdb_scrapers[source].scrape(query, **kwargs)
-        return self.raw_scrapers[source].scrape(query, **kwargs)
+            raise NexusException("Invalid source")
+        
+        return self.scrapers[source].scrape(query, **kwargs)
 
     def scrape_raw(self, query="", **kwargs) -> List[ScrapeResult]:
         """
         Scrape all sources for a query.
 
         Parameters:
         - `query` (str): The search query.
```

### Comparing `nexus_scraper-0.2.0/Nexus/scrapers/annatar.py` & `nexus_scraper-0.2.2/Nexus/scrapers/annatar.py`

 * *Files identical despite different names*

### Comparing `nexus_scraper-0.2.0/Nexus/scrapers/jackett.py` & `nexus_scraper-0.2.2/Nexus/scrapers/jackett.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from Nexus.models import Guids, NexusSettings, ScrapeResult
 
 
 class Jackett:
     def __init__(self, settings: NexusSettings):
         self.settings = settings
         if not self.settings.jackett_url or not self.settings.jackett_apikey:
-            raise JackettException("URL and API key are required.")
+            return
+        
         self.base_url = self.settings.jackett_url
         self.api_key = self.settings.jackett_apikey
         self.session = requests.Session()
 
     def _request(self, endpoint, method="GET", params=None, data=None, timeout=60):
         """Private method to handle API requests."""
         url = f"{self.base_url}/{endpoint}"
```

### Comparing `nexus_scraper-0.2.0/Nexus/scrapers/orionoid.py` & `nexus_scraper-0.2.2/Nexus/scrapers/orionoid.py`

 * *Files identical despite different names*

### Comparing `nexus_scraper-0.2.0/Nexus/scrapers/prowlarr.py` & `nexus_scraper-0.2.2/Nexus/scrapers/prowlarr.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class Prowlarr:
     """Prowlarr class for Prowlarr API operations."""
 
     def __init__(self, settings: NexusSettings):
         if not settings.prowlarr_url or not settings.prowlarr_apikey:
-            raise ProwlarrException("URL and API key are required.")
+            return
         if len(settings.prowlarr_apikey) != 32:
             raise ProwlarrException("API key must be 32 characters long.")
 
         self.base_url = settings.prowlarr_url
         self.api_key = settings.prowlarr_apikey
         self.session = requests.Session()
         self.session.headers.update({"X-Api-Key": settings.prowlarr_apikey})
```

### Comparing `nexus_scraper-0.2.0/Nexus/scrapers/torbox.py` & `nexus_scraper-0.2.2/Nexus/scrapers/torbox.py`

 * *Files identical despite different names*

### Comparing `nexus_scraper-0.2.0/Nexus/scrapers/torrentio.py` & `nexus_scraper-0.2.2/Nexus/scrapers/torrentio.py`

 * *Files identical despite different names*

### Comparing `nexus_scraper-0.2.0/pyproject.toml` & `nexus_scraper-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nexus-scraper"
-version = "0.2.0"
+version = "0.2.2"
 description = ""
 authors = ["Spoked <dreu.lavelle@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `nexus_scraper-0.2.0/PKG-INFO` & `nexus_scraper-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-scraper
-Version: 0.2.0
+Version: 0.2.2
 Summary: 
 License: MIT
 Author: Spoked
 Author-email: dreu.lavelle@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

