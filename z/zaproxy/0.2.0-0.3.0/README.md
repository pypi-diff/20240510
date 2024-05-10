# Comparing `tmp/zaproxy-0.2.0.tar.gz` & `tmp/zaproxy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaproxy-0.2.0.tar", last modified: Fri Nov  3 18:32:58 2023, max compression
+gzip compressed data, was "zaproxy-0.3.0.tar", max compression
```

## Comparing `zaproxy-0.2.0.tar` & `zaproxy-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,45 @@
-drwxr-xr-x   0 thc202     (501) staff       (20)        0 2023-11-03 18:32:58.102354 zaproxy-0.2.0/
--rw-r--r--   0 thc202     (501) staff       (20)    11357 2023-11-03 18:32:19.000000 zaproxy-0.2.0/LICENSE
--rw-r--r--   0 thc202     (501) staff       (20)     1140 2023-11-03 18:32:58.101960 zaproxy-0.2.0/PKG-INFO
--rw-r--r--   0 thc202     (501) staff       (20)     2065 2023-11-03 18:32:19.000000 zaproxy-0.2.0/README.md
--rw-r--r--   0 thc202     (501) staff       (20)       38 2023-11-03 18:32:58.102429 zaproxy-0.2.0/setup.cfg
--rwxr-xr-x   0 thc202     (501) staff       (20)     1533 2023-11-03 18:32:19.000000 zaproxy-0.2.0/setup.py
-drwxr-xr-x   0 thc202     (501) staff       (20)        0 2023-11-03 18:32:58.081364 zaproxy-0.2.0/src/
-drwxr-xr-x   0 thc202     (501) staff       (20)        0 2023-11-03 18:32:58.086139 zaproxy-0.2.0/src/zaproxy.egg-info/
--rw-r--r--   0 thc202     (501) staff       (20)     1140 2023-11-03 18:32:58.000000 zaproxy-0.2.0/src/zaproxy.egg-info/PKG-INFO
--rw-r--r--   0 thc202     (501) staff       (20)     1071 2023-11-03 18:32:58.000000 zaproxy-0.2.0/src/zaproxy.egg-info/SOURCES.txt
--rw-r--r--   0 thc202     (501) staff       (20)        1 2023-11-03 18:32:58.000000 zaproxy-0.2.0/src/zaproxy.egg-info/dependency_links.txt
--rw-r--r--   0 thc202     (501) staff       (20)       66 2023-11-03 18:32:58.000000 zaproxy-0.2.0/src/zaproxy.egg-info/requires.txt
--rw-r--r--   0 thc202     (501) staff       (20)        6 2023-11-03 18:32:58.000000 zaproxy-0.2.0/src/zaproxy.egg-info/top_level.txt
-drwxr-xr-x   0 thc202     (501) staff       (20)        0 2023-11-03 18:32:58.101017 zaproxy-0.2.0/src/zapv2/
--rw-r--r--   0 thc202     (501) staff       (20)     7800 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/__init__.py
--rw-r--r--   0 thc202     (501) staff       (20)     3123 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/accessControl.py
--rw-r--r--   0 thc202     (501) staff       (20)     2610 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/acsrf.py
--rw-r--r--   0 thc202     (501) staff       (20)    16355 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/ajaxSpider.py
--rw-r--r--   0 thc202     (501) staff       (20)     7597 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/alert.py
--rw-r--r--   0 thc202     (501) staff       (20)     9098 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/alertFilter.py
--rw-r--r--   0 thc202     (501) staff       (20)    27498 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/ascan.py
--rw-r--r--   0 thc202     (501) staff       (20)     3694 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/authentication.py
--rw-r--r--   0 thc202     (501) staff       (20)     2266 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/authorization.py
--rw-r--r--   0 thc202     (501) staff       (20)     1693 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/automation.py
--rw-r--r--   0 thc202     (501) staff       (20)     8349 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/autoupdate.py
--rw-r--r--   0 thc202     (501) staff       (20)     4479 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/brk.py
--rw-r--r--   0 thc202     (501) staff       (20)     7885 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/context.py
--rw-r--r--   0 thc202     (501) staff       (20)    29662 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/core.py
--rw-r--r--   0 thc202     (501) staff       (20)     4089 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/exim.py
--rw-r--r--   0 thc202     (501) staff       (20)     2036 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/forcedUser.py
--rw-r--r--   0 thc202     (501) staff       (20)     8201 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/graphql.py
--rw-r--r--   0 thc202     (501) staff       (20)     5977 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/httpSessions.py
--rw-r--r--   0 thc202     (501) staff       (20)     2127 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/localProxies.py
--rw-r--r--   0 thc202     (501) staff       (20)    19754 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/network.py
--rw-r--r--   0 thc202     (501) staff       (20)     1938 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/openapi.py
--rw-r--r--   0 thc202     (501) staff       (20)     1195 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/params.py
--rw-r--r--   0 thc202     (501) staff       (20)     2921 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/pnh.py
--rw-r--r--   0 thc202     (501) staff       (20)     5392 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/pscan.py
--rw-r--r--   0 thc202     (501) staff       (20)     3296 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/replacer.py
--rw-r--r--   0 thc202     (501) staff       (20)     2988 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/reports.py
--rw-r--r--   0 thc202     (501) staff       (20)     1132 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/retest.py
--rw-r--r--   0 thc202     (501) staff       (20)     1512 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/reveal.py
--rw-r--r--   0 thc202     (501) staff       (20)     1754 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/revisit.py
--rw-r--r--   0 thc202     (501) staff       (20)     2229 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/ruleConfig.py
--rw-r--r--   0 thc202     (501) staff       (20)     8741 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/script.py
--rw-r--r--   0 thc202     (501) staff       (20)     8638 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/search.py
--rw-r--r--   0 thc202     (501) staff       (20)     8074 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/selenium.py
--rw-r--r--   0 thc202     (501) staff       (20)     2358 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/sessionManagement.py
--rw-r--r--   0 thc202     (501) staff       (20)     1493 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/soap.py
--rw-r--r--   0 thc202     (501) staff       (20)    26424 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/spider.py
--rw-r--r--   0 thc202     (501) staff       (20)     4617 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/stats.py
--rw-r--r--   0 thc202     (501) staff       (20)     7054 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/users.py
--rw-r--r--   0 thc202     (501) staff       (20)     1859 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/wappalyzer.py
--rw-r--r--   0 thc202     (501) staff       (20)     3906 2023-11-03 18:32:19.000000 zaproxy-0.2.0/src/zapv2/websocket.py
+-rw-r--r--   0        0        0    11357 2024-05-10 07:42:35.993695 zaproxy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1114 2024-05-10 07:42:35.993695 zaproxy-0.3.0/README.md
+-rw-r--r--   0        0        0     1467 2024-05-10 07:42:35.993695 zaproxy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7894 2024-05-10 07:42:35.993695 zaproxy-0.3.0/src/zapv2/__init__.py
+-rw-r--r--   0        0        0     3123 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/accessControl.py
+-rw-r--r--   0        0        0     2610 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/acsrf.py
+-rw-r--r--   0        0        0    16351 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/ajaxSpider.py
+-rw-r--r--   0        0        0     7597 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/alert.py
+-rw-r--r--   0        0        0     9098 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/alertFilter.py
+-rw-r--r--   0        0        0    28082 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/ascan.py
+-rw-r--r--   0        0        0     3694 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/authentication.py
+-rw-r--r--   0        0        0     2266 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/authorization.py
+-rw-r--r--   0        0        0     1693 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/automation.py
+-rw-r--r--   0        0        0     8349 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/autoupdate.py
+-rw-r--r--   0        0        0     4479 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/brk.py
+-rw-r--r--   0        0        0     7885 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/context.py
+-rw-r--r--   0        0        0    30289 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/core.py
+-rw-r--r--   0        0        0     4430 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/custompayloads.py
+-rw-r--r--   0        0        0     4089 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/exim.py
+-rw-r--r--   0        0        0     2036 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/forcedUser.py
+-rw-r--r--   0        0        0     8201 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/graphql.py
+-rw-r--r--   0        0        0     5977 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/httpSessions.py
+-rw-r--r--   0        0        0     2127 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/localProxies.py
+-rw-r--r--   0        0        0    19754 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/network.py
+-rw-r--r--   0        0        0     1938 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/openapi.py
+-rw-r--r--   0        0        0     1195 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/params.py
+-rw-r--r--   0        0        0     2921 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/pnh.py
+-rw-r--r--   0        0        0     5392 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/pscan.py
+-rw-r--r--   0        0        0     3296 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/replacer.py
+-rw-r--r--   0        0        0     2988 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/reports.py
+-rw-r--r--   0        0        0     1132 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/retest.py
+-rw-r--r--   0        0        0     1512 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/reveal.py
+-rw-r--r--   0        0        0     1754 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/revisit.py
+-rw-r--r--   0        0        0     2229 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/ruleConfig.py
+-rw-r--r--   0        0        0     8741 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/script.py
+-rw-r--r--   0        0        0    10589 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/search.py
+-rw-r--r--   0        0        0     8074 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/selenium.py
+-rw-r--r--   0        0        0     2358 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/sessionManagement.py
+-rw-r--r--   0        0        0     1493 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/soap.py
+-rw-r--r--   0        0        0    26424 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/spider.py
+-rw-r--r--   0        0        0     4617 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/stats.py
+-rw-r--r--   0        0        0     7030 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/users.py
+-rw-r--r--   0        0        0     1870 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/wappalyzer.py
+-rw-r--r--   0        0        0     3906 2024-05-10 07:42:35.997695 zaproxy-0.3.0/src/zapv2/websocket.py
+-rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 zaproxy-0.3.0/PKG-INFO
```

### Comparing `zaproxy-0.2.0/LICENSE` & `zaproxy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/__init__.py` & `zaproxy-0.3.0/src/zapv2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Client implementation for using the ZAP pentesting proxy remotely.
 """
 
 __docformat__ = 'restructuredtext'
-__version__ = '0.2.0'
+__version__ = '0.3.0'
 
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 
 from .accessControl import accessControl
 from .acsrf import acsrf
 from .alert import alert
@@ -34,14 +34,15 @@
 from .authentication import authentication
 from .authorization import authorization
 from .automation import automation
 from .autoupdate import autoupdate
 from .brk import brk
 from .context import context
 from .core import core
+from .custompayloads import custompayloads
 from .exim import exim
 from .forcedUser import forcedUser
 from .graphql import graphql
 from .httpSessions import httpSessions
 from .localProxies import localProxies
 from .network import network
 from .openapi import openapi
@@ -99,14 +100,15 @@
         self.authentication = authentication(self)
         self.authorization = authorization(self)
         self.automation = automation(self)
         self.autoupdate = autoupdate(self)
         self.brk = brk(self)
         self.context = context(self)
         self.core = core(self)
+        self.custompayloads = custompayloads(self)
         self.exim = exim(self)
         self.forcedUser = forcedUser(self)
         self.graphql = graphql(self)
         self.httpsessions = httpSessions(self)
         self.localProxies = localProxies(self)
         self.network = network(self)
         self.openapi = openapi(self)
```

### Comparing `zaproxy-0.2.0/src/zapv2/accessControl.py` & `zaproxy-0.3.0/src/zapv2/accessControl.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/acsrf.py` & `zaproxy-0.3.0/src/zapv2/acsrf.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/ajaxSpider.py` & `zaproxy-0.3.0/src/zapv2/ajaxSpider.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         Sets the configuration of the AJAX Spider to use one of the supported browsers.
         This component is optional and therefore the API will only work if it is installed
         """
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'ajaxSpider/action/setOptionBrowserId/', {'String': string})))
 
     def set_option_click_default_elems(self, boolean, apikey=''):
         """
-        Sets whether or not the the AJAX Spider will only click on the default HTML elements.
+        Sets whether or not the AJAX Spider will only click on the default HTML elements.
         This component is optional and therefore the API will only work if it is installed
         """
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'ajaxSpider/action/setOptionClickDefaultElems/', {'Boolean': boolean})))
 
     def set_option_click_elems_once(self, boolean, apikey=''):
         """
         When enabled, the crawler attempts to interact with each element (e.g., by clicking) only once.
```

### Comparing `zaproxy-0.2.0/src/zapv2/alert.py` & `zaproxy-0.3.0/src/zapv2/alert.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/alertFilter.py` & `zaproxy-0.3.0/src/zapv2/alertFilter.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/ascan.py` & `zaproxy-0.3.0/src/zapv2/ascan.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,21 @@
     def option_allow_attack_on_start(self):
         """
         
         """
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'ascan/view/optionAllowAttackOnStart/')))
 
     @property
+    def option_encode_cookie_values(self):
+        """
+        Tells whether or not the active scanner should encode cookie values.
+        """
+        return six.next(six.itervalues(self.zap._request(self.zap.base + 'ascan/view/optionEncodeCookieValues/')))
+
+    @property
     def option_inject_plugin_id_in_header(self):
         """
         Tells whether or not the active scanner should inject the HTTP request header X-ZAP-Scan-ID, with the ID of the scan rule that's sending the requests.
         """
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'ascan/view/optionInjectPluginIdInHeader/')))
 
     @property
@@ -568,14 +575,20 @@
 
     def set_option_delay_in_ms(self, integer, apikey=''):
         """
         
         """
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'ascan/action/setOptionDelayInMs/', {'Integer': integer})))
 
+    def set_option_encode_cookie_values(self, boolean, apikey=''):
+        """
+        Sets whether or not the active scanner should encode cookie values.
+        """
+        return six.next(six.itervalues(self.zap._request(self.zap.base + 'ascan/action/setOptionEncodeCookieValues/', {'Boolean': boolean})))
+
     def set_option_handle_anti_csrf_tokens(self, boolean, apikey=''):
         """
         
         """
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'ascan/action/setOptionHandleAntiCSRFTokens/', {'Boolean': boolean})))
 
     def set_option_host_per_scan(self, integer, apikey=''):
```

### Comparing `zaproxy-0.2.0/src/zapv2/authentication.py` & `zaproxy-0.3.0/src/zapv2/authentication.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/authorization.py` & `zaproxy-0.3.0/src/zapv2/authorization.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/automation.py` & `zaproxy-0.3.0/src/zapv2/automation.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/autoupdate.py` & `zaproxy-0.3.0/src/zapv2/autoupdate.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/brk.py` & `zaproxy-0.3.0/src/zapv2/brk.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/context.py` & `zaproxy-0.3.0/src/zapv2/context.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/core.py` & `zaproxy-0.3.0/src/zapv2/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,23 @@
         params = {}
         if baseurl is not None:
             params['baseurl'] = baseurl
         if riskid is not None:
             params['riskId'] = riskid
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'core/view/numberOfAlerts/', params)))
 
+    def get_log_level(self, name=None):
+        """
+        The detailed logging config, optionally filtered based on a name (ex: starts with).
+        """
+        params = {}
+        if name is not None:
+            params['name'] = name
+        return six.next(six.itervalues(self.zap._request(self.zap.base + 'core/view/getLogLevel/', params)))
+
     @property
     def option_default_user_agent(self):
         """
         Gets the user agent that ZAP should use when creating HTTP messages (for example, spider messages or CONNECT requests to outgoing proxy).
         """
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'core/view/optionDefaultUserAgent/')))
 
@@ -530,14 +539,20 @@
 
     def delete_alert(self, id, apikey=''):
         """
         Deletes the alert with the given ID. 
         """
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'core/action/deleteAlert/', {'id': id})))
 
+    def set_log_level(self, name, loglevel, apikey=''):
+        """
+        Sets the logging level for a given logger name.
+        """
+        return six.next(six.itervalues(self.zap._request(self.zap.base + 'core/action/setLogLevel/', {'name': name, 'logLevel': loglevel})))
+
     def set_option_default_user_agent(self, string, apikey=''):
         """
         Sets the user agent that ZAP should use when creating HTTP messages (for example, spider messages or CONNECT requests to outgoing proxy).
         """
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'core/action/setOptionDefaultUserAgent/', {'String': string})))
 
     def set_option_dns_ttl_successful_queries(self, integer, apikey=''):
```

### Comparing `zaproxy-0.2.0/src/zapv2/exim.py` & `zaproxy-0.3.0/src/zapv2/exim.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/forcedUser.py` & `zaproxy-0.3.0/src/zapv2/forcedUser.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/graphql.py` & `zaproxy-0.3.0/src/zapv2/graphql.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/httpSessions.py` & `zaproxy-0.3.0/src/zapv2/httpSessions.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/localProxies.py` & `zaproxy-0.3.0/src/zapv2/localProxies.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/network.py` & `zaproxy-0.3.0/src/zapv2/network.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/openapi.py` & `zaproxy-0.3.0/src/zapv2/openapi.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/params.py` & `zaproxy-0.3.0/src/zapv2/params.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/pnh.py` & `zaproxy-0.3.0/src/zapv2/pnh.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/pscan.py` & `zaproxy-0.3.0/src/zapv2/pscan.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/replacer.py` & `zaproxy-0.3.0/src/zapv2/replacer.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/reports.py` & `zaproxy-0.3.0/src/zapv2/reports.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/retest.py` & `zaproxy-0.3.0/src/zapv2/retest.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/reveal.py` & `zaproxy-0.3.0/src/zapv2/reveal.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/revisit.py` & `zaproxy-0.3.0/src/zapv2/revisit.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/ruleConfig.py` & `zaproxy-0.3.0/src/zapv2/ruleConfig.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/script.py` & `zaproxy-0.3.0/src/zapv2/script.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/search.py` & `zaproxy-0.3.0/src/zapv2/search.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,27 @@
             params['baseurl'] = baseurl
         if start is not None:
             params['start'] = start
         if count is not None:
             params['count'] = count
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'search/view/urlsByUrlRegex/', params)))
 
+    def urls_by_tag_regex(self, regex, baseurl=None, start=None, count=None):
+        """
+        Returns the URLs of the HTTP messages that match the given regular expression in their history Tags optionally filtered by URL and paginated with 'start' position and 'count' of messages.
+        """
+        params = {'regex': regex}
+        if baseurl is not None:
+            params['baseurl'] = baseurl
+        if start is not None:
+            params['start'] = start
+        if count is not None:
+            params['count'] = count
+        return six.next(six.itervalues(self.zap._request(self.zap.base + 'search/view/urlsByTagRegex/', params)))
+
     def urls_by_request_regex(self, regex, baseurl=None, start=None, count=None):
         """
         Returns the URLs of the HTTP messages that match the given regular expression in the request optionally filtered by URL and paginated with 'start' position and 'count' of messages.
         """
         params = {'regex': regex}
         if baseurl is not None:
             params['baseurl'] = baseurl
@@ -88,14 +101,27 @@
             params['baseurl'] = baseurl
         if start is not None:
             params['start'] = start
         if count is not None:
             params['count'] = count
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'search/view/messagesByUrlRegex/', params)))
 
+    def messages_by_tag_regex(self, regex, baseurl=None, start=None, count=None):
+        """
+        Returns the HTTP messages that match the given regular expression in their history Tags optionally filtered by URL and paginated with 'start' position and 'count' of messages.
+        """
+        params = {'regex': regex}
+        if baseurl is not None:
+            params['baseurl'] = baseurl
+        if start is not None:
+            params['start'] = start
+        if count is not None:
+            params['count'] = count
+        return six.next(six.itervalues(self.zap._request(self.zap.base + 'search/view/messagesByTagRegex/', params)))
+
     def messages_by_request_regex(self, regex, baseurl=None, start=None, count=None):
         """
         Returns the HTTP messages that match the given regular expression in the request optionally filtered by URL and paginated with 'start' position and 'count' of messages.
         """
         params = {'regex': regex}
         if baseurl is not None:
             params['baseurl'] = baseurl
@@ -140,14 +166,27 @@
             params['baseurl'] = baseurl
         if start is not None:
             params['start'] = start
         if count is not None:
             params['count'] = count
         return (self.zap._request_other(self.zap.base_other + 'search/other/harByUrlRegex/', params))
 
+    def har_by_tag_regex(self, regex, baseurl=None, start=None, count=None, apikey=''):
+        """
+        Returns the HTTP messages, in HAR format, that match the given regular expression in their history Tags optionally filtered by URL and paginated with 'start' position and 'count' of messages.
+        """
+        params = {'regex': regex}
+        if baseurl is not None:
+            params['baseurl'] = baseurl
+        if start is not None:
+            params['start'] = start
+        if count is not None:
+            params['count'] = count
+        return (self.zap._request_other(self.zap.base_other + 'search/other/harByTagRegex/', params))
+
     def har_by_request_regex(self, regex, baseurl=None, start=None, count=None, apikey=''):
         """
         Returns the HTTP messages, in HAR format, that match the given regular expression in the request optionally filtered by URL and paginated with 'start' position and 'count' of messages.
         """
         params = {'regex': regex}
         if baseurl is not None:
             params['baseurl'] = baseurl
```

### Comparing `zaproxy-0.2.0/src/zapv2/selenium.py` & `zaproxy-0.3.0/src/zapv2/selenium.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/sessionManagement.py` & `zaproxy-0.3.0/src/zapv2/sessionManagement.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/soap.py` & `zaproxy-0.3.0/src/zapv2/soap.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/spider.py` & `zaproxy-0.3.0/src/zapv2/spider.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/stats.py` & `zaproxy-0.3.0/src/zapv2/stats.py`

 * *Files identical despite different names*

### Comparing `zaproxy-0.2.0/src/zapv2/users.py` & `zaproxy-0.3.0/src/zapv2/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             params['contextId'] = contextid
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'users/view/usersList/', params)))
 
     def get_user_by_id(self, contextid, userid):
         """
         Gets the data of the user with the given ID that belongs to the context with the given ID.
         """
-        return six.next(six.itervalues(self.zap._request(self.zap.base + 'users/view/getUserById/', {'contextId': contextid, 'userId': userid})))
+        return (self.zap._request(self.zap.base + 'users/view/getUserById/', {'contextId': contextid, 'userId': userid}))
 
     def get_authentication_credentials_config_params(self, contextid):
         """
         Gets the configuration parameters for the credentials of the context with the given ID.
         """
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'users/view/getAuthenticationCredentialsConfigParams/', {'contextId': contextid})))
```

### Comparing `zaproxy-0.2.0/src/zapv2/wappalyzer.py` & `zaproxy-0.3.0/src/zapv2/wappalyzer.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     def __init__(self, zap):
         self.zap = zap
 
     @property
     def list_sites(self):
         """
-        Lists all the sites recognized by the wappalyzer addon.
+        Lists all the sites recognized by the Technology Detection add-on.
         This component is optional and therefore the API will only work if it is installed
         """
         return six.next(six.itervalues(self.zap._request(self.zap.base + 'wappalyzer/view/listSites/')))
 
     @property
     def list_all(self):
         """
```

### Comparing `zaproxy-0.2.0/src/zapv2/websocket.py` & `zaproxy-0.3.0/src/zapv2/websocket.py`

 * *Files identical despite different names*

