# Comparing `tmp/docrawl-1.3.0.tar.gz` & `tmp/docrawl-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrawl-1.3.0.tar", last modified: Fri May  3 13:11:26 2024, max compression
+gzip compressed data, was "docrawl-1.3.1.tar", last modified: Fri May 10 08:27:04 2024, max compression
```

## Comparing `docrawl-1.3.0.tar` & `docrawl-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 13:11:26.472505 docrawl-1.3.0/
--rw-rw-rw-   0        0        0     1090 2024-03-01 01:29:38.000000 docrawl-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      527 2024-05-03 13:11:26.471185 docrawl-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-03-01 01:29:38.000000 docrawl-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 13:11:26.424036 docrawl-1.3.0/docrawl/
--rw-rw-rw-   0        0        0        0 2024-03-01 01:29:38.000000 docrawl-1.3.0/docrawl/__init__.py
--rw-rw-rw-   0        0        0    12660 2024-05-03 13:10:38.000000 docrawl-1.3.0/docrawl/docrawl_client.py
--rw-rw-rw-   0        0        0    42929 2024-05-03 13:10:38.000000 docrawl-1.3.0/docrawl/docrawl_core.py
--rw-rw-rw-   0        0        0     6847 2024-03-01 01:29:38.000000 docrawl-1.3.0/docrawl/docrawl_launcher.py
--rw-rw-rw-   0        0        0     1108 2024-03-01 01:29:38.000000 docrawl-1.3.0/docrawl/docrawl_logger.py
--rw-rw-rw-   0        0        0     2674 2024-03-01 01:29:38.000000 docrawl-1.3.0/docrawl/elements.py
-drwxrwxrwx   0        0        0        0 2024-05-03 13:11:26.470185 docrawl-1.3.0/docrawl.egg-info/
--rw-rw-rw-   0        0        0      527 2024-05-03 13:11:26.000000 docrawl-1.3.0/docrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2024-05-03 13:11:26.000000 docrawl-1.3.0/docrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 13:11:26.000000 docrawl-1.3.0/docrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2024-05-03 13:11:26.000000 docrawl-1.3.0/docrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-03 13:11:26.000000 docrawl-1.3.0/docrawl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 13:11:26.472505 docrawl-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      834 2024-05-03 13:11:11.000000 docrawl-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:27:04.495024 docrawl-1.3.1/
+-rw-rw-rw-   0        0        0     1090 2024-03-01 01:29:38.000000 docrawl-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0      527 2024-05-10 08:27:04.493512 docrawl-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-03-01 01:29:38.000000 docrawl-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 08:27:04.430213 docrawl-1.3.1/docrawl/
+-rw-rw-rw-   0        0        0        0 2024-03-01 01:29:38.000000 docrawl-1.3.1/docrawl/__init__.py
+-rw-rw-rw-   0        0        0    13103 2024-05-10 08:26:51.000000 docrawl-1.3.1/docrawl/docrawl_client.py
+-rw-rw-rw-   0        0        0    43228 2024-05-10 08:26:51.000000 docrawl-1.3.1/docrawl/docrawl_core.py
+-rw-rw-rw-   0        0        0     6847 2024-03-01 01:29:38.000000 docrawl-1.3.1/docrawl/docrawl_launcher.py
+-rw-rw-rw-   0        0        0     1108 2024-03-01 01:29:38.000000 docrawl-1.3.1/docrawl/docrawl_logger.py
+-rw-rw-rw-   0        0        0     2674 2024-03-01 01:29:38.000000 docrawl-1.3.1/docrawl/elements.py
+-rw-rw-rw-   0        0        0       49 2024-05-10 08:26:51.000000 docrawl-1.3.1/docrawl/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-10 08:27:04.492520 docrawl-1.3.1/docrawl.egg-info/
+-rw-rw-rw-   0        0        0      527 2024-05-10 08:27:04.000000 docrawl-1.3.1/docrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-10 08:27:04.000000 docrawl-1.3.1/docrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 08:27:04.000000 docrawl-1.3.1/docrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2024-05-10 08:27:04.000000 docrawl-1.3.1/docrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-10 08:27:04.000000 docrawl-1.3.1/docrawl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 08:27:04.495024 docrawl-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      834 2024-05-10 08:26:31.000000 docrawl-1.3.1/setup.py
```

### Comparing `docrawl-1.3.0/LICENSE` & `docrawl-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docrawl-1.3.0/PKG-INFO` & `docrawl-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.3.0
+Version: 1.3.1
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `docrawl-1.3.0/docrawl/docrawl_client.py` & `docrawl-1.3.1/docrawl/docrawl_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import psutil
 import itertools
 import time
-
-from scrapy.crawler import CrawlerRunner
-from dataclasses import dataclass
 from contextlib import suppress
+from dataclasses import dataclass
+
+import psutil
 from crochet import setup
+from scrapy.crawler import CrawlerRunner
 
-from docrawl.docrawl_logger import docrawl_logger
 from docrawl.docrawl_core import DocrawlSpider
-
+from docrawl.docrawl_logger import docrawl_logger
+from docrawl.errors import SpiderFunctionError
 from keepvariable.keepvariable_core import KeepVariableDummyRedisServer
 
 
 @dataclass
 class DocrawlSettings:
     pid: int
     driver: str
@@ -21,28 +21,28 @@
     last_function: str
 
 
 class DocrawlClient:
     id_iter = itertools.count()
 
     def __init__(self, kv_redis=None, kv_redis_keys=None, number_of_spawn_browsers=0, redis_key_prefix=""):
-        """number of spawn browsers = how many browser processes are ready in standby mode to not initialize + close the browser, currently support 0 and 1"""
+        """Number of spawn browsers = how many browser processes are ready in standby mode to not initialize + close the browser, currently support 0 and 1."""
         self._client_id = redis_key_prefix.split(':')[1] or next(self.id_iter)
 
         self.kv_redis = kv_redis or KeepVariableDummyRedisServer()
         self.kv_redis_keys = kv_redis_keys or {}
         self.redis_key_prefix = redis_key_prefix
 
         self._kv_redis_key_browser_metadata = self.kv_redis_keys.get('browser_meta_data', f'{self.redis_key_prefix}:browser_meta_data')
         self._kv_redis_key_scanned_elements = self.kv_redis_keys.get('elements', f'{self.redis_key_prefix}:elements')
         self._kv_redis_key_screenshot = self.kv_redis_keys.get('screenshot', f'{self.redis_key_prefix}:screenshot')
-        
-        
+
+
         docrawl_logger.info(f'Initialised DocrawlClient with ID {self._client_id}')
-        
+
         if number_of_spawn_browsers > 0: #TODO: increase number of spawned browsers, support just 1 standby browser at this moment
             self.run_spider()
 
     def set_browser_meta_data(self, browser_meta_data: dict):
         self.kv_redis.set(key=self._kv_redis_key_browser_metadata, value=browser_meta_data)
 
     def get_browser_meta_data(self):
@@ -65,15 +65,15 @@
         pid = self.get_browser_meta_data()['browser'].get('pid', 0)
 
         return psutil.pid_exists(pid)
 
     def _initialize_browser_metadata(self, driver, headless, proxy=None):
         browser_meta_data = {
             "browser": {"driver": driver, "headless": headless, "proxy": proxy},
-            "function": {"name": "init_function", "input": None, "done": False}
+            "function": {"name": "init_function", "input": None, "done": False, "error": None},
         }
 
         self.set_browser_meta_data(browser_meta_data)
 
     def _wait_until_page_is_loaded(self, timeout=20):
         # Load spider_requests and spider_functions
         try:
@@ -96,15 +96,17 @@
             docrawl_logger.success('Page loaded')
         else:
             docrawl_logger.error('Page was not loaded')
 
     def _wait_until_function_is_done(self, timeout):
         # Load spider_requests and spider_functions
         try:
-            is_function_done = self.get_browser_meta_data()['function']['done']
+            spider_function = self.get_browser_meta_data()['function']
+            is_function_done = spider_function['done']
+            function_error_message = spider_function['error']
         except Exception as e:
             docrawl_logger.error(f'Error while loading is_function_done: {e}')
             is_function_done = True
 
         # Then check if function is done
         timeout_start = time.time()
         while not is_function_done and time.time() < timeout_start + timeout:
@@ -112,24 +114,29 @@
                 is_function_done = self.get_browser_meta_data()['function']['done']
             except:
                 is_function_done = False
             time.sleep(0.5)
             # docrawl_logger.info('Function is still running, waiting 0.5 sec ...')
 
         if is_function_done:
-            docrawl_logger.success('Function finished')
+            if function_error_message is None:
+                docrawl_logger.success('Spider function finished successfully')
+            else:
+                docrawl_logger.error(f'Spider function failed: {function_error_message}')
+                raise SpiderFunctionError(spider_function['error'])
         else:
             docrawl_logger.error('Function was not finished')
+            raise TimeoutError('Spider function timed out')
 
     def _execute_function(self, function, function_input=None, timeout=30):
-        docrawl_logger.info(f'Running function {function} with input: {function_input}')
+        # docrawl_logger.info(f'Running function {function} with input: {function_input}')
 
         if True:#self.is_browser_active(): #The browser seemed inactive but it was actually active
             browser_meta_data = self.get_browser_meta_data()
-            function = {"name": function, "input": function_input, "done": False}
+            function = {"name": function, "input": function_input, "done": False, "error": None}
             browser_meta_data['function'] = function
             self.set_browser_meta_data(browser_meta_data)
 
             # self._wait_until_page_is_loaded()
             self._wait_until_function_is_done(timeout)
         else:
             docrawl_logger.warning('Browser instance is not active / crashed, function '+str(function)+' could not be executed')
@@ -140,15 +147,15 @@
 
         self.active_browser = "browser1"
 
         docrawl_logger.warning(f"Acquired browser {self.active_browser}")
 
     def release_browser(self):
         self.active_browser = None
-        
+
 
     def run_spider(self, driver='Firefox', in_browser: bool = False, proxy: dict = None):
         self._initialize_browser_metadata(driver=driver, headless=not in_browser, proxy=proxy)
 
         setup()
         crawler = CrawlerRunner()
         crawler.crawl(DocrawlSpider, docrawl_client=self)
@@ -166,29 +173,27 @@
 
     def take_screenshot(self, timeout=20):
         self._execute_function('take_screenshot', None, timeout)
 
     def take_png_screenshot(self, filename, timeout=20):
         """
         Launches take_screenshot from core.
-            :param filename: string, output filename (where to save the screenshot)
+            :param filename: string, output filename (where to save the screenshot).
         """
-
         inp = {
             'filename': str(filename)  # Cast to str, e.g. when Path object is passed
         }
 
         self._execute_function('take_png_screenshot', inp, timeout)
 
     def extract_page_source(self, filename, timeout=20):
         """
         Launches extract_page_source from core.
-            :param filename: string, name of file that will be used for storing page source
+            :param filename: string, name of file that will be used for storing page source.
         """
-
         inp = {
             'filename': filename
         }
 
         self._execute_function('extract_page_source', inp, timeout)
 
     def scan_web_page(self, incl_tables=False, incl_bullets=False, incl_texts=False, incl_headlines=False,
@@ -201,17 +206,16 @@
             :param incl_bullets: boolean, search for bullet lists
             :param incl_texts: boolean, search for text elements
             :param incl_headlines: boolean, search for headlines
             :param incl_links: boolean, search for links
             :param incl_images: boolean, search for images
             :param incl_buttons: boolean, search for buttons
             :param by_xpath: str, search elements by custom XPath
-            :param output_folder: str, path to output folder
+            :param output_folder: str, path to output folder.
         """
-
         inp = {
             'incl_tables': incl_tables,
             'incl_bullets': incl_bullets,
             'incl_texts': incl_texts,
             'incl_headlines': incl_headlines,
             'incl_links': incl_links,
             'incl_images': incl_images,
@@ -223,39 +227,35 @@
         }
 
         self._execute_function('scan_web_page', inp, timeout)
 
     def wait_until_element_is_located(self, xpath, timeout=20):
         """
         Launches wait_until_element_is_located function from core.
-            :param xpath: str, xpath of element to be located
+            :param xpath: str, xpath of element to be located.
         """
-
         inp = {
             'xpath': xpath
         }
 
         self._execute_function('wait_until_element_is_located', inp, timeout)
 
     def get_current_url(self, filename, timeout=20):
         """
         Launches get_current_url function from core.
-            :param filename: string, name of file that will be used for storing the URL
+            :param filename: string, name of file that will be used for storing the URL.
         """
-
         inp = {
             'filename': filename
         }
 
         self._execute_function('get_current_url', inp, timeout)
 
     def close_browser(self, timeout=10):
-        """
-        Launches close_browser function from core.
-        """
+        """Launch close_browser function from core."""
 
         self._execute_function('close_browser', None, timeout)
 
         pid = self.get_browser_meta_data()['browser']['pid']
 
         with suppress(Exception):
             psutil.Process(pid).terminate()
```

### Comparing `docrawl-1.3.0/docrawl/docrawl_core.py` & `docrawl-1.3.1/docrawl/docrawl_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1035,29 +1035,34 @@
 
                     self.docrawl_client.set_browser_meta_data(browser_meta_data)
 
                 if not spider_function['done']:
                     function_str = spider_function['name']
 
                     inp = spider_function['input']
-                    docrawl_logger.info(f'Function input from docrawl core: {inp}')
+                    # docrawl_logger.info(f'Function input from docrawl core: {inp}')
                     
                     
-                    docrawl_logger.warning("Preparing for finishing undone docrawl function")
+                    # docrawl_logger.warning("Preparing for finishing undone docrawl function")
                     if f'_{function_str}'=="_take_png_screenshot":
                         #skip standard execution and run in a different thread
                         self.initialize_screenshot_thread_if_not_existing(inp["filename"])
                     else: #Standard behaviour    
                         getattr(self, f'_{function_str}')(inp=inp)
                         
                         docrawl_logger.warning("Running docrawl function:"+f'_{function_str}')
 
                     spider_function['done'] = True
+                    spider_function['error'] = None
                     browser_meta_data['function'] = spider_function
-
                     self.docrawl_client.set_browser_meta_data(browser_meta_data)
 
             except KeyboardInterrupt:
                 break
             except Exception as e:
                 docrawl_logger.error(f'Error while executing docrawl loop: {e}')
                 docrawl_logger.error(traceback.format_exc())
+
+                spider_function['done'] = True
+                spider_function['error'] = str(e)
+                browser_meta_data['function'] = spider_function
+                self.docrawl_client.set_browser_meta_data(browser_meta_data)
```

### Comparing `docrawl-1.3.0/docrawl/docrawl_launcher.py` & `docrawl-1.3.1/docrawl/docrawl_launcher.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.3.0/docrawl/docrawl_logger.py` & `docrawl-1.3.1/docrawl/docrawl_logger.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.3.0/docrawl/elements.py` & `docrawl-1.3.1/docrawl/elements.py`

 * *Files identical despite different names*

### Comparing `docrawl-1.3.0/docrawl.egg-info/PKG-INFO` & `docrawl-1.3.1/docrawl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 1.3.0
+Version: 1.3.1
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `docrawl-1.3.0/setup.py` & `docrawl-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='docrawl',
-    version='1.3.0',
+    version='1.3.1',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Do automated crawling of pages using scrapy',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/docrawl',
     packages=setuptools.find_packages(),
```

