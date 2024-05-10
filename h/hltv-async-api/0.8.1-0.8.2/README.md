# Comparing `tmp/hltv_async_api-0.8.1.tar.gz` & `tmp/hltv_async_api-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.8.1.tar", max compression
+gzip compressed data, was "hltv_async_api-0.8.2.tar", max compression
```

## Comparing `hltv_async_api-0.8.1.tar` & `hltv_async_api-0.8.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      124 2024-05-01 22:56:01.696170 hltv_async_api-0.8.1/hltv_async_api/__init__.py
--rw-r--r--   0        0        0    47390 2024-05-01 22:48:30.590801 hltv_async_api-0.8.1/hltv_async_api/aiohltv.py
--rw-r--r--   0        0        0     4147 2024-05-01 22:43:55.467443 hltv_async_api-0.8.1/hltv_async_api/unreleased.py
--rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.8.1/LICENSE
--rw-r--r--   0        0        0      627 2024-05-01 22:56:01.679888 hltv_async_api-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    16713 2024-05-01 22:52:56.932867 hltv_async_api-0.8.1/README.md
--rw-r--r--   0        0        0    17156 1970-01-01 00:00:00.000000 hltv_async_api-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      124 2024-05-10 11:59:09.773309 hltv_async_api-0.8.2/hltv_async_api/__init__.py
+-rw-r--r--   0        0        0    48503 2024-05-10 12:26:03.278178 hltv_async_api-0.8.2/hltv_async_api/aiohltv.py
+-rw-r--r--   0        0        0     4147 2024-05-01 22:43:55.467443 hltv_async_api-0.8.2/hltv_async_api/unreleased.py
+-rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.8.2/LICENSE
+-rw-r--r--   0        0        0      627 2024-05-10 11:59:09.764323 hltv_async_api-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0    17437 2024-05-10 12:26:03.291482 hltv_async_api-0.8.2/README.md
+-rw-r--r--   0        0        0    17855 1970-01-01 00:00:00.000000 hltv_async_api-0.8.2/PKG-INFO
```

### Comparing `hltv_async_api-0.8.1/hltv_async_api/aiohltv.py` & `hltv_async_api-0.8.2/hltv_async_api/aiohltv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 import pytz
 import asyncio
 import re
 import logging
-from typing import Any, List
+import random
+from typing import Any, List, Optional
 from datetime import date, datetime, timedelta
 from bs4 import BeautifulSoup
 from functools import partial
 from aiohttp import ClientSession, ClientTimeout
 from aiohttp.client_exceptions import ClientProxyConnectionError, ClientResponseError, ClientOSError, \
-    ServerDisconnectedError, ClientHttpProxyError
+    ServerDisconnectedError, ClientHttpProxyError, ClientConnectorError
 
 
 class Hltv:
-    def __init__(self, max_delay: int = 10,
+    def __init__(self,
+                 min_delay: float | int= -1.0,
+                 max_delay: float | int= 10.0,
                  timeout: int = 5,
+                 max_retries: int = 10,
                  proxy_path: str | None = None,
                  proxy_list: list | None = None,
-                 debug: bool = False,
-                 max_retries: int = 10,
+                 proxy_delay: bool = False,
                  proxy_protocol: str | None = None,
                  remove_proxy: bool = False,
                  tz: str | None = None,
                  safe_mode: bool = True,
+                 debug: bool = False,
                  ):
         self.headers = {
             "referer": "https://www.hltv.org/stats",
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)",
             "hltvTimeZone": "Europe/Copenhagen"
         }
         self.DEBUG = debug
         self._configure_logging()
         self.logger = logging.getLogger(__name__)
 
-        self.MAX_DELAY = max_delay
+        self.MIN_DELAY = float(min_delay)
+        self.MAX_DELAY = float(max_delay)
+        self._init_delay()
+
         self.timeout = timeout
         self.max_retries = max_retries
 
         self.TIMEZONE = tz
         self._init_tz(tz)
 
         self.PROXY_PATH = proxy_path
         self.PROXY_LIST = proxy_list
         self.PROXY_PROTOCOL = proxy_protocol
         self.PROXY_ONCE = remove_proxy
+        self.PROXY_DELAY = proxy_delay
 
         if self.PROXY_PATH:
             with open(self.PROXY_PATH, "r") as file:
                 self.PROXY_LIST = [line.strip() for line in file.readlines()]
 
         if self.PROXY_PROTOCOL:
             self.PROXY_LIST = [self.PROXY_PROTOCOL + '://' + proxy for i, proxy in enumerate(self.PROXY_LIST, start=0)]
@@ -77,31 +85,48 @@
     async def close(self):
         if self.session:
             self.logger.debug('Closing Session')
             await self.session.close()
             self.session = None
 
     def _configure_logging(self):
-        level = logging.DEBUG if self.DEBUG else logging.INFO
-        logging.basicConfig(level=level, format="%(message)s")
+        def get_logger(name, **kwargs):
+            import logging
 
-    def config(self, max_delay: int | None = None,
-               timeout: int | None = None,
-               use_proxy: bool | None = None,
-               proxy_file_path: str | None = None,
-               proxy_list: list | None = None,
-               debug: bool | None = None,
-               max_retries: int | None = None,
-               proxy_protocol: str | None = None,
-               remove_proxy: bool | None = None,
-               tz: str | None = None,
-               safe_mode: bool | None = None,
+            logging.basicConfig(**kwargs)
+            logger = logging.getLogger(name)
+            logger.debug(f"start logging '{name}'")
+            return logger
+
+        self.logger = get_logger(
+            __name__,
+            **{
+                "level": "DEBUG" if self.DEBUG else "INFO",
+                "format": "[%(levelname)s] %(message)s ",
+            },
+        )
+
+    def config(self,
+               min_delay: Optional[float | int] = None,
+               max_delay: Optional[float | int] = None,
+               timeout: Optional[int] = None,
+               use_proxy: Optional[bool] = None,
+               proxy_file_path: Optional[str] = None,
+               proxy_list: Optional[list] = None,
+               debug: Optional[bool] = None,
+               max_retries: Optional[int] = None,
+               proxy_protocol: Optional[str] = None,
+               remove_proxy: Optional[bool] = None,
+               tz: Optional[str] = None,
+               safe_mode: Optional[bool] = None,
                ):
-        if max_delay:
-            self.MAX_DELAY = max_delay
+        if min_delay or max_delay:
+            self.MIN_DELAY = float(min_delay)
+            self.MAX_DELAY = float(max_delay)
+            self._init_delay()
         if timeout:
             self.timeout = timeout
         if use_proxy is not None:
             self.USE_PROXY = use_proxy
         if proxy_list:
             self.PROXY_LIST = proxy_list
         if max_retries:
@@ -131,38 +156,44 @@
                 self.logger.error('UnknownTimeZoneError, Using default timezone: Europe/Copenhagen')
                 self.TIMEZONE = None
 
     def _init_safe(self):
         if not self.SAFE:
             self.logger.warning('Safe mode deactivated.')
 
+    def _init_delay(self):
+        if self.MIN_DELAY != -1.0:
+            if self.MAX_DELAY >= self.MIN_DELAY >= 0.0 and self.MAX_DELAY >= 0.0:
+                return
+            self.logger.warning(f'Invalid min/max delay. Delay will be increasing by 1 sec')
+        self.MIN_DELAY = None
+
     def _get_proxy(self):
         try:
             proxy = self.PROXY_LIST[0]
 
             if self.PROXY_PROTOCOL and proxy != '' and self.PROXY_PROTOCOL not in proxy:
                 proxy = self.PROXY_PROTOCOL + '://' + proxy
 
             return proxy
         except IndexError:
             self.logger.error('No proxies left')
 
-    async def _switch_proxy(self):
+    def _switch_proxy(self):
         try:
             if self.PROXY_ONCE:
                 self.logger.debug(f'Removing proxy {self.PROXY_LIST[0]}')
                 self.PROXY_LIST = self.PROXY_LIST[1:]
             else:
                 self.logger.debug(f"Switching proxy {self.PROXY_LIST[0] if self.PROXY_LIST[0] else 'No Proxy'}")
                 self.PROXY_LIST = self.PROXY_LIST[1:] + [(self.PROXY_LIST[0])]
                 self.logger.info(f"New proxy: {self.PROXY_LIST[0] if self.PROXY_LIST[0] else 'No Proxy'}")
         except IndexError:
             self.logger.error('No proxies left')
 
-
     @staticmethod
     def _f(result):
         return BeautifulSoup(result, "lxml")
 
     def _cloudflare_check(self, page) -> bool:
         challenge_page = page.find(id="challenge-error-title")
         if challenge_page is not None:
@@ -170,20 +201,24 @@
                 self.logger.debug("Got cloudflare challenge page")
                 return True
         return False
 
     def _parse_error_handler(self, delay: int = 0) -> int:
         if self.USE_PROXY:
             self._switch_proxy()
+            if not self.PROXY_DELAY:
+                return 0
+
+        if self.MIN_DELAY:
+            delay = random.uniform(self.MIN_DELAY, self.MAX_DELAY)
+            self.logger.debug(f'Random delay {round(delay, 2)}s')
         else:
             if delay < self.MAX_DELAY:
                 delay += 1
-            else:
-                self.logger.debug("Reached max delay limit, try to use proxy")
-            self.logger.info(f"Calling again, increasing delay to {delay}s")
+                self.logger.info(f"Increasing delay to {delay}s")
 
         return delay
 
     async def _parse(self, url, delay):
         proxy = ''
         # setup new proxy, cuz old one was switched
         if self.USE_PROXY:
@@ -194,32 +229,32 @@
         try:
             async with self.session.get(url, headers=self.headers, proxy=proxy, timeout=self.timeout) as response:
                 self.logger.info(f"Fetching {url}, code: {response.status}")
                 if response.status == 200:
                     result = await response.text()
                     page = await self.loop.run_in_executor(None, partial(self._f, result))
                     forbitten = await self.loop.run_in_executor(None, partial(self._cloudflare_check, page))
-
-                    if forbitten:
-                        return False, await self.loop.run_in_executor(None, partial(self._parse_error_handler, delay))
-                    return True, page
+                    if not forbitten:
+                        return True, page
 
                 self.logger.debug(f"Error, Code {response.status=}")
                 return False, await self.loop.run_in_executor(None, partial(self._parse_error_handler, delay))
 
-        except ClientHttpProxyError as e:
+        except TimeoutError as e:
             self.logger.debug(e)
-            delay = self._parse_error_handler(delay)
-            return False, delay
 
-        except (ClientProxyConnectionError, ClientResponseError, ClientOSError,
-                ServerDisconnectedError, ClientTimeout, Exception) as e:
+        except (ClientProxyConnectionError, ClientResponseError, ClientOSError, ClientConnectorError,
+                ServerDisconnectedError, ClientTimeout, asyncio.TimeoutError, ClientHttpProxyError) as e:
             self.logger.debug(e)
-            delay = self._parse_error_handler(delay)
-            return False, delay
+
+        except Exception as e:
+            self.logger.debug(e)
+
+        delay = self._parse_error_handler(delay)
+        return False, delay
 
     async def _fetch(self, url, delay: int = 0):
         if not self.session:
             self._create_session()
         status = False
         try_ = 1
         result = None
@@ -1170,14 +1205,13 @@
             if only_today:
                 break
 
         return news
 
 
 async def main():
-    async with Hltv(debug=True, safe_mode=False,
-                    remove_proxy=True) as hltv:
-        print(await hltv.get_team_info(6667, 'faze'))
+    async with Hltv(debug=True, safe_mode=False, min_delay=2) as hltv:
+        print(await hltv.get_matches())
 
 
 if __name__ == '__main__':
     asyncio.run(main())
```

### Comparing `hltv_async_api-0.8.1/hltv_async_api/unreleased.py` & `hltv_async_api-0.8.2/hltv_async_api/unreleased.py`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.8.1/LICENSE` & `hltv_async_api-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.8.1/pyproject.toml` & `hltv_async_api-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hltv_async_api"
-version = "0.8.1"
+version = "0.8.2"
 authors = ["Akim Slys <akimslys2003@gmail.com>"]
 description = "An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `hltv_async_api-0.8.1/README.md` & `hltv_async_api-0.8.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # hltv-async-api an **unofficial** asynchronous HLTV API Wrapper for Python.
 
 # Future
 
-* **0.8** more event info data (winners, stats, groups, teams), refactor last_matches in player_info. Optimize proxy functions. Coverage. (?) Rotating user agent (exp. till 20.05)
+* **0.8** more event info data (winners, stats, groups, teams), refactor last_matches in player_info. Optimize proxy functions. Coverage.(?) Rotating user agent (exp. till 20.05)
 * **0.9.0** stats & images update, more stats scrapers, team logos, player photos, images, more data, team_map stats, map stats, more functions such as get_news_id, get_team_logo, get_player_photo, get_demo_id, get_match_stats...
 * **0.10.0** synchronous update, reformatting the library as a synchronous, move async parser as an extension. (JULY-AUGUST 2024)
-* **0.11.0** ...
+* **0.11.0 - 1.0.0** Provide to use Hltv-async-api on any system, language, by creating a RESTful service.
 
 
 # Features
 
 
 * **Simple Usage** (its really simple)
 
@@ -35,67 +35,92 @@
 ```
 
 ---
 
 
 # Simple Usage
 
-    ```
+  ```
 
     from hltv_async_api import Hltv
     
     async with Hltv() as hltv:
       print(await hltv.get_event_info(7148, 'PGL CS2 Major Copenhagen2024'))
 
-    ```
+  ```
 
   **OR**
 
-    ```
+  ```
 
     from hltv_async_api import Hltv
     
     hltv = Hltv()
     print(await hltv.get_event_info(7148, 'PGL CS2 Major Copenhagen2024'))
     await hltv.close()
 
-    ```
+  ```
 
 
 ---
 
 # Configs
 
-* max_delay: int = 15
+* max_delay: float = 10.0
 
-    Automatically increasing reconnecting delay by 1 sec to max_delay (from 1s to 5s)
+  Automatically increasing delay by 1 sec to 10s
 
-    ```
+  ```
     hltv = Hltv(max_delay=5)
     
     >>>Fetching https://www.hltv.org/matches/2370727/faze-vs-natus-vincere-pgl-cs2-major-copenhagen-2024, code: 403
     >>>Got 403 forbitten
     >>>Calling again, increasing delay to 4s
     >>>Fetching https://www.hltv.org/matches/2370727/faze-vs-natus-vincere-pgl-cs2-major-copenhagen-2024, code: 403
     >>>Got 403 forbitten
     >>>Calling again, increasing delay to 5s
-    ```
+  ```
+
+* min_delay: float = -1
+
+``` 
+  [DEBUG] Random delay 9.55s 
+  [DEBUG] Trying connect to https://www.hltv.org/matches, try 3/10
+  [DEBUG] Random delay 3.9s 
+  [DEBUG] Trying connect to https://www.hltv.org/matches, try 4/10
+```
+
+
+
+* proxy_delay: bool = False
+
+    Delay for proxy uses.
+* 
+  ```
+  [INFO] New proxy: http://123.123.123.123:123 
+  [DEBUG] Random delay 9.55s 
+  [DEBUG] Trying connect to https://www.hltv.org/matches, try 3/10
+  [DEBUG] Switching proxy http://123.123.123.123:123 
+  [INFO] New proxy: http://111.111.111.11:111 
+  [DEBUG] Random delay 3.9s 
+  [DEBUG] Trying connect to https://www.hltv.org/matches, try 4/10
+  ```
 
 * max_retries: int = 10
 
     0 for infinity retries
     
     ```
     hltv = Hltv(max_retries=2, debug=True)
     print(await hltv.get_best_players())
     
-    Creating Session
-    Trying connect to https://www.hltv.org/stats/players?startDate=2024-01-01&endDate=2024-12-31&rankingFilter=Top20, try 1/2
-    Trying connect to https://www.hltv.org/stats/players?startDate=2024-01-01&endDate=2024-12-31&rankingFilter=Top20, try 2/2
-    Connection failed
+    >>>Creating Session
+    >>>Trying connect to https://www.hltv.org/stats/players?startDate=2024-01-01&endDate=2024-12-31&rankingFilter=Top20, try 1/2
+    >>>Trying connect to https://www.hltv.org/stats/players?startDate=2024-01-01&endDate=2024-12-31&rankingFilter=Top20, try 2/2
+    >>>Connection failed
     ```
 
 * proxy_list: list | None = None
 
     automatic rotating proxies, if your proxies doesnt have any protocol you can use proxy_protocol.
     Note: To add non-proxy to list just put '' to it, you can find example with ar
```

#### html2text {}

```diff
@@ -1,40 +1,49 @@
 # hltv-async-api an **unofficial** asynchronous HLTV API Wrapper for Python. #
 Future * **0.8** more event info data (winners, stats, groups, teams), refactor
-last_matches in player_info. Optimize proxy functions. Coverage. (?) Rotating
+last_matches in player_info. Optimize proxy functions. Coverage.(?) Rotating
 user agent (exp. till 20.05) * **0.9.0** stats & images update, more stats
 scrapers, team logos, player photos, images, more data, team_map stats, map
 stats, more functions such as get_news_id, get_team_logo, get_player_photo,
 get_demo_id, get_match_stats... * **0.10.0** synchronous update, reformatting
 the library as a synchronous, move async parser as an extension. (JULY-AUGUST
-2024) * **0.11.0** ... # Features * **Simple Usage** (its really simple) *
-**New and modern fully async library** * **Huge amount of options** *
-**Supports proxy usage** * **Made with love <3** --- # Installation ``` pip
-install hltv-async-api ``` --- # Simple Usage ``` from hltv_async_api import
-Hltv async with Hltv() as hltv: print(await hltv.get_event_info(7148, 'PGL CS2
-Major Copenhagen2024')) ``` **OR** ``` from hltv_async_api import Hltv hltv =
-Hltv() print(await hltv.get_event_info(7148, 'PGL CS2 Major Copenhagen2024'))
-await hltv.close() ``` --- # Configs * max_delay: int = 15 Automatically
-increasing reconnecting delay by 1 sec to max_delay (from 1s to 5s) ``` hltv =
-Hltv(max_delay=5) >>>Fetching https://www.hltv.org/matches/2370727/faze-vs-
-natus-vincere-pgl-cs2-major-copenhagen-2024, code: 403 >>>Got 403 forbitten
+2024) * **0.11.0 - 1.0.0** Provide to use Hltv-async-api on any system,
+language, by creating a RESTful service. # Features * **Simple Usage** (its
+really simple) * **New and modern fully async library** * **Huge amount of
+options** * **Supports proxy usage** * **Made with love <3** --- # Installation
+``` pip install hltv-async-api ``` --- # Simple Usage ``` from hltv_async_api
+import Hltv async with Hltv() as hltv: print(await hltv.get_event_info(7148,
+'PGL CS2 Major Copenhagen2024')) ``` **OR** ``` from hltv_async_api import Hltv
+hltv = Hltv() print(await hltv.get_event_info(7148, 'PGL CS2 Major
+Copenhagen2024')) await hltv.close() ``` --- # Configs * max_delay: float =
+10.0 Automatically increasing delay by 1 sec to 10s ``` hltv = Hltv
+(max_delay=5) >>>Fetching https://www.hltv.org/matches/2370727/faze-vs-natus-
+vincere-pgl-cs2-major-copenhagen-2024, code: 403 >>>Got 403 forbitten
 >>>Calling again, increasing delay to 4s >>>Fetching https://www.hltv.org/
 matches/2370727/faze-vs-natus-vincere-pgl-cs2-major-copenhagen-2024, code: 403
->>>Got 403 forbitten >>>Calling again, increasing delay to 5s ``` *
-max_retries: int = 10 0 for infinity retries ``` hltv = Hltv(max_retries=2,
-debug=True) print(await hltv.get_best_players()) Creating Session Trying
-connect to https://www.hltv.org/stats/players?startDate=2024-01-
-01&endDate=2024-12-31&rankingFilter=Top20, try 1/2 Trying connect to https://
+>>>Got 403 forbitten >>>Calling again, increasing delay to 5s ``` * min_delay:
+float = -1 ``` [DEBUG] Random delay 9.55s [DEBUG] Trying connect to https://
+www.hltv.org/matches, try 3/10 [DEBUG] Random delay 3.9s [DEBUG] Trying connect
+to https://www.hltv.org/matches, try 4/10 ``` * proxy_delay: bool = False Delay
+for proxy uses. * ``` [INFO] New proxy: http://123.123.123.123:123 [DEBUG]
+Random delay 9.55s [DEBUG] Trying connect to https://www.hltv.org/matches, try
+3/10 [DEBUG] Switching proxy http://123.123.123.123:123 [INFO] New proxy: http:
+//111.111.111.11:111 [DEBUG] Random delay 3.9s [DEBUG] Trying connect to https:
+//www.hltv.org/matches, try 4/10 ``` * max_retries: int = 10 0 for infinity
+retries ``` hltv = Hltv(max_retries=2, debug=True) print(await
+hltv.get_best_players()) >>>Creating Session >>>Trying connect to https://
 www.hltv.org/stats/players?startDate=2024-01-01&endDate=2024-12-
-31&rankingFilter=Top20, try 2/2 Connection failed ``` * proxy_list: list | None
-= None automatic rotating proxies, if your proxies doesnt have any protocol you
-can use proxy_protocol. Note: To add non-proxy to list just put '' to it, you
-can find example with ar * proxy_path: str | None = None Path to your proxy
-(proxy_list will be ignored). If your proxies doesn't have any protocol you can
-use proxy_protocol * proxy_protocol: str | None = None, Proxy protocol. Your
+31&rankingFilter=Top20, try 1/2 >>>Trying connect to https://www.hltv.org/
+stats/players?startDate=2024-01-01&endDate=2024-12-31&rankingFilter=Top20, try
+2/2 >>>Connection failed ``` * proxy_list: list | None = None automatic
+rotating proxies, if your proxies doesnt have any protocol you can use
+proxy_protocol. Note: To add non-proxy to list just put '' to it, you can find
+example with ar * proxy_path: str | None = None Path to your proxy (proxy_list
+will be ignored). If your proxies doesn't have any protocol you can use
+proxy_protocol * proxy_protocol: str | None = None, Proxy protocol. Your
 proxies ```hltv = Hltv(proxy_protocol='http' ...) -> '11.11.11.11:1111' -
 > 'http://11.11.11.11:1111' * remove_proxy: bool = False Removes proxy from
 list (proxy_path included) if connection unsuccessfully * timeout: int = 5 Max
 time to close connection. Recommended to use timeout=1 if you are using random
 proxies. * debug: bool = False * tz: str = 'Europe/Copenhagen': Timezone
 config. _T_a_p_ _h_e_r_e_ to see all available timezones * safe_mode: bool = True
 Disallow to wrap restricted data. Switch to False only at your own risk. --- #
```

### Comparing `hltv_async_api-0.8.1/PKG-INFO` & `hltv_async_api-0.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 686c 7476  : 2.1.Name: hltv
 00000020: 5f61 7379 6e63 5f61 7069 0a56 6572 7369  _async_api.Versi
-00000030: 6f6e 3a20 302e 382e 310a 5375 6d6d 6172  on: 0.8.1.Summar
+00000030: 6f6e 3a20 302e 382e 320a 5375 6d6d 6172  on: 0.8.2.Summar
 00000040: 793a 2041 6e20 756e 6f66 6669 6369 616c  y: An unofficial
 00000050: 2061 7379 6e63 6872 6f6e 6f75 7320 484c   asynchronous HL
 00000060: 5456 2041 5049 2057 7261 7070 6572 2066  TV API Wrapper f
 00000070: 6f72 2050 7974 686f 6e0a 4175 7468 6f72  or Python.Author
 00000080: 3a20 416b 696d 2053 6c79 730a 4175 7468  : Akim Slys.Auth
 00000090: 6f72 2d65 6d61 696c 3a20 616b 696d 736c  or-email: akimsl
 000000a0: 7973 3230 3033 4067 6d61 696c 2e63 6f6d  ys2003@gmail.com
@@ -63,1011 +63,1054 @@
 000003e0: 7265 2065 7665 6e74 2069 6e66 6f20 6461  re event info da
 000003f0: 7461 2028 7769 6e6e 6572 732c 2073 7461  ta (winners, sta
 00000400: 7473 2c20 6772 6f75 7073 2c20 7465 616d  ts, groups, team
 00000410: 7329 2c20 7265 6661 6374 6f72 206c 6173  s), refactor las
 00000420: 745f 6d61 7463 6865 7320 696e 2070 6c61  t_matches in pla
 00000430: 7965 725f 696e 666f 2e20 4f70 7469 6d69  yer_info. Optimi
 00000440: 7a65 2070 726f 7879 2066 756e 6374 696f  ze proxy functio
-00000450: 6e73 2e20 436f 7665 7261 6765 2e20 283f  ns. Coverage. (?
-00000460: 2920 526f 7461 7469 6e67 2075 7365 7220  ) Rotating user 
-00000470: 6167 656e 7420 2865 7870 2e20 7469 6c6c  agent (exp. till
-00000480: 2032 302e 3035 290a 2a20 2a2a 302e 392e   20.05).* **0.9.
-00000490: 302a 2a20 7374 6174 7320 2620 696d 6167  0** stats & imag
-000004a0: 6573 2075 7064 6174 652c 206d 6f72 6520  es update, more 
-000004b0: 7374 6174 7320 7363 7261 7065 7273 2c20  stats scrapers, 
-000004c0: 7465 616d 206c 6f67 6f73 2c20 706c 6179  team logos, play
-000004d0: 6572 2070 686f 746f 732c 2069 6d61 6765  er photos, image
-000004e0: 732c 206d 6f72 6520 6461 7461 2c20 7465  s, more data, te
-000004f0: 616d 5f6d 6170 2073 7461 7473 2c20 6d61  am_map stats, ma
-00000500: 7020 7374 6174 732c 206d 6f72 6520 6675  p stats, more fu
-00000510: 6e63 7469 6f6e 7320 7375 6368 2061 7320  nctions such as 
-00000520: 6765 745f 6e65 7773 5f69 642c 2067 6574  get_news_id, get
-00000530: 5f74 6561 6d5f 6c6f 676f 2c20 6765 745f  _team_logo, get_
-00000540: 706c 6179 6572 5f70 686f 746f 2c20 6765  player_photo, ge
-00000550: 745f 6465 6d6f 5f69 642c 2067 6574 5f6d  t_demo_id, get_m
-00000560: 6174 6368 5f73 7461 7473 2e2e 2e0a 2a20  atch_stats....* 
-00000570: 2a2a 302e 3130 2e30 2a2a 2073 796e 6368  **0.10.0** synch
-00000580: 726f 6e6f 7573 2075 7064 6174 652c 2072  ronous update, r
-00000590: 6566 6f72 6d61 7474 696e 6720 7468 6520  eformatting the 
-000005a0: 6c69 6272 6172 7920 6173 2061 2073 796e  library as a syn
-000005b0: 6368 726f 6e6f 7573 2c20 6d6f 7665 2061  chronous, move a
-000005c0: 7379 6e63 2070 6172 7365 7220 6173 2061  sync parser as a
-000005d0: 6e20 6578 7465 6e73 696f 6e2e 2028 4a55  n extension. (JU
-000005e0: 4c59 2d41 5547 5553 5420 3230 3234 290a  LY-AUGUST 2024).
-000005f0: 2a20 2a2a 302e 3131 2e30 2a2a 202e 2e2e  * **0.11.0** ...
-00000600: 0a0a 0a23 2046 6561 7475 7265 730a 0a0a  ...# Features...
-00000610: 2a20 2a2a 5369 6d70 6c65 2055 7361 6765  * **Simple Usage
-00000620: 2a2a 2028 6974 7320 7265 616c 6c79 2073  ** (its really s
-00000630: 696d 706c 6529 0a0a 0a2a 202a 2a4e 6577  imple)...* **New
-00000640: 2061 6e64 206d 6f64 6572 6e20 6675 6c6c   and modern full
-00000650: 7920 6173 796e 6320 6c69 6272 6172 792a  y async library*
-00000660: 2a0a 0a0a 2a20 2a2a 4875 6765 2061 6d6f  *...* **Huge amo
-00000670: 756e 7420 6f66 206f 7074 696f 6e73 2a2a  unt of options**
-00000680: 0a0a 0a2a 202a 2a53 7570 706f 7274 7320  ...* **Supports 
-00000690: 7072 6f78 7920 7573 6167 652a 2a0a 0a0a  proxy usage**...
-000006a0: 2a20 2a2a 4d61 6465 2077 6974 6820 6c6f  * **Made with lo
-000006b0: 7665 203c 332a 2a0a 0a0a 2d2d 2d0a 0a23  ve <3**...---..#
-000006c0: 2049 6e73 7461 6c6c 6174 696f 6e0a 0a60   Installation..`
-000006d0: 6060 0a70 6970 2069 6e73 7461 6c6c 2068  ``.pip install h
-000006e0: 6c74 762d 6173 796e 632d 6170 690a 6060  ltv-async-api.``
-000006f0: 600a 0a2d 2d2d 0a0a 0a23 2053 696d 706c  `..---...# Simpl
-00000700: 6520 5573 6167 650a 0a20 2020 2060 6060  e Usage..    ```
-00000710: 0a0a 2020 2020 6672 6f6d 2068 6c74 765f  ..    from hltv_
-00000720: 6173 796e 635f 6170 6920 696d 706f 7274  async_api import
-00000730: 2048 6c74 760a 2020 2020 0a20 2020 2061   Hltv.    .    a
-00000740: 7379 6e63 2077 6974 6820 486c 7476 2829  sync with Hltv()
-00000750: 2061 7320 686c 7476 3a0a 2020 2020 2020   as hltv:.      
-00000760: 7072 696e 7428 6177 6169 7420 686c 7476  print(await hltv
-00000770: 2e67 6574 5f65 7665 6e74 5f69 6e66 6f28  .get_event_info(
-00000780: 3731 3438 2c20 2750 474c 2043 5332 204d  7148, 'PGL CS2 M
-00000790: 616a 6f72 2043 6f70 656e 6861 6765 6e32  ajor Copenhagen2
-000007a0: 3032 3427 2929 0a0a 2020 2020 6060 600a  024'))..    ```.
-000007b0: 0a20 202a 2a4f 522a 2a0a 0a20 2020 2060  .  **OR**..    `
-000007c0: 6060 0a0a 2020 2020 6672 6f6d 2068 6c74  ``..    from hlt
-000007d0: 765f 6173 796e 635f 6170 6920 696d 706f  v_async_api impo
-000007e0: 7274 2048 6c74 760a 2020 2020 0a20 2020  rt Hltv.    .   
-000007f0: 2068 6c74 7620 3d20 486c 7476 2829 0a20   hltv = Hltv(). 
-00000800: 2020 2070 7269 6e74 2861 7761 6974 2068     print(await h
-00000810: 6c74 762e 6765 745f 6576 656e 745f 696e  ltv.get_event_in
-00000820: 666f 2837 3134 382c 2027 5047 4c20 4353  fo(7148, 'PGL CS
-00000830: 3220 4d61 6a6f 7220 436f 7065 6e68 6167  2 Major Copenhag
-00000840: 656e 3230 3234 2729 290a 2020 2020 6177  en2024')).    aw
-00000850: 6169 7420 686c 7476 2e63 6c6f 7365 2829  ait hltv.close()
-00000860: 0a0a 2020 2020 6060 600a 0a0a 2d2d 2d0a  ..    ```...---.
-00000870: 0a23 2043 6f6e 6669 6773 0a0a 2a20 6d61  .# Configs..* ma
-00000880: 785f 6465 6c61 793a 2069 6e74 203d 2031  x_delay: int = 1
-00000890: 350a 0a20 2020 2041 7574 6f6d 6174 6963  5..    Automatic
-000008a0: 616c 6c79 2069 6e63 7265 6173 696e 6720  ally increasing 
-000008b0: 7265 636f 6e6e 6563 7469 6e67 2064 656c  reconnecting del
-000008c0: 6179 2062 7920 3120 7365 6320 746f 206d  ay by 1 sec to m
-000008d0: 6178 5f64 656c 6179 2028 6672 6f6d 2031  ax_delay (from 1
-000008e0: 7320 746f 2035 7329 0a0a 2020 2020 6060  s to 5s)..    ``
-000008f0: 600a 2020 2020 686c 7476 203d 2048 6c74  `.    hltv = Hlt
-00000900: 7628 6d61 785f 6465 6c61 793d 3529 0a20  v(max_delay=5). 
-00000910: 2020 200a 2020 2020 3e3e 3e46 6574 6368     .    >>>Fetch
-00000920: 696e 6720 6874 7470 733a 2f2f 7777 772e  ing https://www.
-00000930: 686c 7476 2e6f 7267 2f6d 6174 6368 6573  hltv.org/matches
-00000940: 2f32 3337 3037 3237 2f66 617a 652d 7673  /2370727/faze-vs
-00000950: 2d6e 6174 7573 2d76 696e 6365 7265 2d70  -natus-vincere-p
-00000960: 676c 2d63 7332 2d6d 616a 6f72 2d63 6f70  gl-cs2-major-cop
-00000970: 656e 6861 6765 6e2d 3230 3234 2c20 636f  enhagen-2024, co
-00000980: 6465 3a20 3430 330a 2020 2020 3e3e 3e47  de: 403.    >>>G
-00000990: 6f74 2034 3033 2066 6f72 6269 7474 656e  ot 403 forbitten
-000009a0: 0a20 2020 203e 3e3e 4361 6c6c 696e 6720  .    >>>Calling 
-000009b0: 6167 6169 6e2c 2069 6e63 7265 6173 696e  again, increasin
-000009c0: 6720 6465 6c61 7920 746f 2034 730a 2020  g delay to 4s.  
-000009d0: 2020 3e3e 3e46 6574 6368 696e 6720 6874    >>>Fetching ht
-000009e0: 7470 733a 2f2f 7777 772e 686c 7476 2e6f  tps://www.hltv.o
-000009f0: 7267 2f6d 6174 6368 6573 2f32 3337 3037  rg/matches/23707
-00000a00: 3237 2f66 617a 652d 7673 2d6e 6174 7573  27/faze-vs-natus
-00000a10: 2d76 696e 6365 7265 2d70 676c 2d63 7332  -vincere-pgl-cs2
-00000a20: 2d6d 616a 6f72 2d63 6f70 656e 6861 6765  -major-copenhage
-00000a30: 6e2d 3230 3234 2c20 636f 6465 3a20 3430  n-2024, code: 40
-00000a40: 330a 2020 2020 3e3e 3e47 6f74 2034 3033  3.    >>>Got 403
-00000a50: 2066 6f72 6269 7474 656e 0a20 2020 203e   forbitten.    >
-00000a60: 3e3e 4361 6c6c 696e 6720 6167 6169 6e2c  >>Calling again,
-00000a70: 2069 6e63 7265 6173 696e 6720 6465 6c61   increasing dela
-00000a80: 7920 746f 2035 730a 2020 2020 6060 600a  y to 5s.    ```.
-00000a90: 0a2a 206d 6178 5f72 6574 7269 6573 3a20  .* max_retries: 
-00000aa0: 696e 7420 3d20 3130 0a0a 2020 2020 3020  int = 10..    0 
-00000ab0: 666f 7220 696e 6669 6e69 7479 2072 6574  for infinity ret
-00000ac0: 7269 6573 0a20 2020 200a 2020 2020 6060  ries.    .    ``
-00000ad0: 600a 2020 2020 686c 7476 203d 2048 6c74  `.    hltv = Hlt
-00000ae0: 7628 6d61 785f 7265 7472 6965 733d 322c  v(max_retries=2,
-00000af0: 2064 6562 7567 3d54 7275 6529 0a20 2020   debug=True).   
-00000b00: 2070 7269 6e74 2861 7761 6974 2068 6c74   print(await hlt
-00000b10: 762e 6765 745f 6265 7374 5f70 6c61 7965  v.get_best_playe
-00000b20: 7273 2829 290a 2020 2020 0a20 2020 2043  rs()).    .    C
-00000b30: 7265 6174 696e 6720 5365 7373 696f 6e0a  reating Session.
-00000b40: 2020 2020 5472 7969 6e67 2063 6f6e 6e65      Trying conne
-00000b50: 6374 2074 6f20 6874 7470 733a 2f2f 7777  ct to https://ww
-00000b60: 772e 686c 7476 2e6f 7267 2f73 7461 7473  w.hltv.org/stats
-00000b70: 2f70 6c61 7965 7273 3f73 7461 7274 4461  /players?startDa
-00000b80: 7465 3d32 3032 342d 3031 2d30 3126 656e  te=2024-01-01&en
-00000b90: 6444 6174 653d 3230 3234 2d31 322d 3331  dDate=2024-12-31
-00000ba0: 2672 616e 6b69 6e67 4669 6c74 6572 3d54  &rankingFilter=T
-00000bb0: 6f70 3230 2c20 7472 7920 312f 320a 2020  op20, try 1/2.  
-00000bc0: 2020 5472 7969 6e67 2063 6f6e 6e65 6374    Trying connect
-00000bd0: 2074 6f20 6874 7470 733a 2f2f 7777 772e   to https://www.
-00000be0: 686c 7476 2e6f 7267 2f73 7461 7473 2f70  hltv.org/stats/p
-00000bf0: 6c61 7965 7273 3f73 7461 7274 4461 7465  layers?startDate
-00000c00: 3d32 3032 342d 3031 2d30 3126 656e 6444  =2024-01-01&endD
-00000c10: 6174 653d 3230 3234 2d31 322d 3331 2672  ate=2024-12-31&r
-00000c20: 616e 6b69 6e67 4669 6c74 6572 3d54 6f70  ankingFilter=Top
-00000c30: 3230 2c20 7472 7920 322f 320a 2020 2020  20, try 2/2.    
-00000c40: 436f 6e6e 6563 7469 6f6e 2066 6169 6c65  Connection faile
-00000c50: 640a 2020 2020 6060 600a 0a2a 2070 726f  d.    ```..* pro
-00000c60: 7879 5f6c 6973 743a 206c 6973 7420 7c20  xy_list: list | 
-00000c70: 4e6f 6e65 203d 204e 6f6e 650a 0a20 2020  None = None..   
-00000c80: 2061 7574 6f6d 6174 6963 2072 6f74 6174   automatic rotat
-00000c90: 696e 6720 7072 6f78 6965 732c 2069 6620  ing proxies, if 
-00000ca0: 796f 7572 2070 726f 7869 6573 2064 6f65  your proxies doe
-00000cb0: 736e 7420 6861 7665 2061 6e79 2070 726f  snt have any pro
-00000cc0: 746f 636f 6c20 796f 7520 6361 6e20 7573  tocol you can us
-00000cd0: 6520 7072 6f78 795f 7072 6f74 6f63 6f6c  e proxy_protocol
-00000ce0: 2e0a 2020 2020 4e6f 7465 3a20 546f 2061  ..    Note: To a
-00000cf0: 6464 206e 6f6e 2d70 726f 7879 2074 6f20  dd non-proxy to 
-00000d00: 6c69 7374 206a 7573 7420 7075 7420 2727  list just put ''
-00000d10: 2074 6f20 6974 2c20 796f 7520 6361 6e20   to it, you can 
-00000d20: 6669 6e64 2065 7861 6d70 6c65 2077 6974  find example wit
-00000d30: 6820 6172 0a0a 2a20 7072 6f78 795f 7061  h ar..* proxy_pa
-00000d40: 7468 3a20 7374 7220 7c20 4e6f 6e65 203d  th: str | None =
-00000d50: 204e 6f6e 650a 0a20 2020 2050 6174 6820   None..    Path 
-00000d60: 746f 2079 6f75 7220 7072 6f78 7920 2870  to your proxy (p
-00000d70: 726f 7879 5f6c 6973 7420 7769 6c6c 2062  roxy_list will b
-00000d80: 6520 6967 6e6f 7265 6429 2e20 4966 2079  e ignored). If y
-00000d90: 6f75 7220 7072 6f78 6965 7320 646f 6573  our proxies does
-00000da0: 6e27 7420 6861 7665 2061 6e79 2070 726f  n't have any pro
-00000db0: 746f 636f 6c20 796f 7520 6361 6e20 7573  tocol you can us
-00000dc0: 6520 7072 6f78 795f 7072 6f74 6f63 6f6c  e proxy_protocol
-00000dd0: 0a0a 2a20 7072 6f78 795f 7072 6f74 6f63  ..* proxy_protoc
-00000de0: 6f6c 3a20 7374 7220 7c20 4e6f 6e65 203d  ol: str | None =
-00000df0: 204e 6f6e 652c 0a0a 2020 2020 5072 6f78   None,..    Prox
-00000e00: 7920 7072 6f74 6f63 6f6c 2e20 596f 7572  y protocol. Your
-00000e10: 2070 726f 7869 6573 2060 6060 686c 7476   proxies ```hltv
-00000e20: 203d 2048 6c74 7628 7072 6f78 795f 7072   = Hltv(proxy_pr
-00000e30: 6f74 6f63 6f6c 3d27 6874 7470 2720 2e2e  otocol='http' ..
-00000e40: 2e29 202d 3e20 2731 312e 3131 2e31 312e  .) -> '11.11.11.
-00000e50: 3131 3a31 3131 3127 202d 3e20 2768 7474  11:1111' -> 'htt
-00000e60: 703a 2f2f 3131 2e31 312e 3131 2e31 313a  p://11.11.11.11:
-00000e70: 3131 3131 270a 0a2a 2072 656d 6f76 655f  1111'..* remove_
-00000e80: 7072 6f78 793a 2062 6f6f 6c20 3d20 4661  proxy: bool = Fa
-00000e90: 6c73 650a 0a20 2020 2052 656d 6f76 6573  lse..    Removes
-00000ea0: 2070 726f 7879 2066 726f 6d20 6c69 7374   proxy from list
-00000eb0: 2028 7072 6f78 795f 7061 7468 2069 6e63   (proxy_path inc
-00000ec0: 6c75 6465 6429 2069 6620 636f 6e6e 6563  luded) if connec
-00000ed0: 7469 6f6e 2075 6e73 7563 6365 7373 6675  tion unsuccessfu
-00000ee0: 6c6c 790a 0a2a 2074 696d 656f 7574 3a20  lly..* timeout: 
-00000ef0: 696e 7420 3d20 350a 0a20 2020 204d 6178  int = 5..    Max
-00000f00: 2074 696d 6520 746f 2063 6c6f 7365 2063   time to close c
-00000f10: 6f6e 6e65 6374 696f 6e2e 2052 6563 6f6d  onnection. Recom
-00000f20: 6d65 6e64 6564 2074 6f20 7573 6520 7469  mended to use ti
-00000f30: 6d65 6f75 743d 3120 6966 2079 6f75 2061  meout=1 if you a
-00000f40: 7265 2075 7369 6e67 2072 616e 646f 6d20  re using random 
-00000f50: 7072 6f78 6965 732e 0a0a 2a20 6465 6275  proxies...* debu
-00000f60: 673a 2062 6f6f 6c20 3d20 4661 6c73 650a  g: bool = False.
-00000f70: 0a2a 2074 7a3a 2073 7472 203d 2027 4575  .* tz: str = 'Eu
-00000f80: 726f 7065 2f43 6f70 656e 6861 6765 6e27  rope/Copenhagen'
-00000f90: 3a0a 2020 2020 0a20 2020 2054 696d 657a  :.    .    Timez
-00000fa0: 6f6e 6520 636f 6e66 6967 2e20 0a20 0a20  one config. . . 
-00000fb0: 2020 203c 6120 6872 6566 3d27 6874 7470     <a href='http
-00000fc0: 733a 2f2f 6769 7374 2e67 6974 6875 622e  s://gist.github.
-00000fd0: 636f 6d2f 6865 7961 6c65 7865 6a2f 3862  com/heyalexej/8b
-00000fe0: 6636 3838 6664 3637 6437 3139 3962 6534  f688fd67d7199be4
-00000ff0: 6131 3638 3262 3365 6563 3735 3638 273e  a1682b3eec7568'>
-00001000: 5461 7020 6865 7265 203c 2f61 3e20 746f  Tap here </a> to
-00001010: 2073 6565 2061 6c6c 2061 7661 696c 6162   see all availab
-00001020: 6c65 2074 696d 657a 6f6e 6573 0a0a 2a20  le timezones..* 
-00001030: 7361 6665 5f6d 6f64 653a 2062 6f6f 6c20  safe_mode: bool 
-00001040: 3d20 5472 7565 0a0a 2020 2020 4469 7361  = True..    Disa
-00001050: 6c6c 6f77 2074 6f20 7772 6170 2072 6573  llow to wrap res
-00001060: 7472 6963 7465 6420 6461 7461 2e20 5377  tricted data. Sw
-00001070: 6974 6368 2074 6f20 4661 6c73 6520 6f6e  itch to False on
-00001080: 6c79 2061 7420 796f 7572 206f 776e 2072  ly at your own r
-00001090: 6973 6b2e 0a0a 0a2d 2d2d 0a0a 2320 5072  isk....---..# Pr
-000010a0: 6f78 7920 5573 6167 650a 0a2a 2a4c 6f61  oxy Usage..**Loa
-000010b0: 6420 5072 6f78 6965 7320 6672 6f6d 206c  d Proxies from l
-000010c0: 6973 742a 2a0a 2020 2020 0a20 2020 2060  ist**.    .    `
-000010d0: 6060 0a20 2020 2070 726f 7879 5f6c 6973  ``.    proxy_lis
-000010e0: 7420 3d20 5b27 6874 7470 3a2f 2f31 3230  t = ['http://120
-000010f0: 2e32 3334 2e32 3033 2e31 3731 3a39 3030  .234.203.171:900
-00001100: 3227 2c20 2768 7474 703a 2f2f 3131 302e  2', 'http://110.
-00001110: 3338 2e36 382e 3338 3a38 3027 5d0a 2020  38.68.38:80'].  
-00001120: 2020 0a20 2020 2068 6c74 7620 3d20 486c    .    hltv = Hl
-00001130: 7476 2870 726f 7879 5f6c 6973 743d 7072  tv(proxy_list=pr
-00001140: 6f78 795f 6c69 7374 290a 0a20 2020 2060  oxy_list)..    `
-00001150: 6060 0a0a 2a2a 4c6f 6164 2050 726f 7869  ``..**Load Proxi
-00001160: 6573 2066 726f 6d20 6669 6c65 2a2a 0a0a  es from file**..
-00001170: 2020 2020 6060 600a 2020 2020 686c 7476      ```.    hltv
-00001180: 203d 2048 6c74 7628 7072 6f78 795f 7061   = Hltv(proxy_pa
-00001190: 7468 3d27 5041 5448 5f54 4f5f 5052 4f58  th='PATH_TO_PROX
-000011a0: 592e 5458 5427 290a 2020 2020 6060 600a  Y.TXT').    ```.
-000011b0: 0a0a 2a2a 5265 6d6f 7665 2070 726f 7879  ..**Remove proxy
-000011c0: 2a2a 0a0a 2020 2020 5265 6d6f 7665 7320  **..    Removes 
-000011d0: 6261 6420 7072 6f78 6965 730a 2020 2020  bad proxies.    
-000011e0: 0a20 2020 2060 6060 0a20 2020 2068 6c74  .    ```.    hlt
-000011f0: 7620 3d20 486c 7476 2870 726f 7879 5f70  v = Hltv(proxy_p
-00001200: 6174 683d 2750 4154 485f 544f 5f50 524f  ath='PATH_TO_PRO
-00001210: 5859 2e54 5854 272c 2072 656d 6f76 655f  XY.TXT', remove_
-00001220: 7072 6f78 793d 5472 7565 290a 2020 2020  proxy=True).    
-00001230: 6060 600a 0a2a 2a50 726f 746f 636f 6c20  ```..**Protocol 
-00001240: 7573 6167 652a 2a0a 0a20 2020 2060 6060  usage**..    ```
-00001250: 0a20 2020 2070 726f 7879 5f6c 6973 7420  .    proxy_list 
-00001260: 3d20 5b27 3132 302e 3233 342e 3230 332e  = ['120.234.203.
-00001270: 3137 313a 3930 3032 272c 2027 3131 302e  171:9002', '110.
-00001280: 3338 2e36 382e 3338 3a38 3027 5d0a 2020  38.68.38:80'].  
-00001290: 2020 0a20 2020 2068 6c74 7620 3d20 486c    .    hltv = Hl
-000012a0: 7476 2870 726f 7879 5f6c 6973 743d 7072  tv(proxy_list=pr
-000012b0: 6f78 795f 6c69 7374 2c20 7072 6f78 795f  oxy_list, proxy_
-000012c0: 7072 6f74 6f63 6f6c 3d27 6874 7470 2729  protocol='http')
-000012d0: 0a20 2020 2060 6060 0a0a 2d2d 2d0a 0a23  .    ```..---..#
-000012e0: 204d 6574 686f 6473 0a0a 2a20 2a2a 6765   Methods..* **ge
-000012f0: 745f 6d61 7463 6865 7328 6461 7973 3a20  t_matches(days: 
-00001300: 696e 7420 3d20 312c 206d 696e 5f73 7461  int = 1, min_sta
-00001310: 725f 7261 7469 6e67 3a20 696e 7420 3d20  r_rating: int = 
-00001320: 312c 206c 6976 653a 2062 6f6f 6c20 3d20  1, live: bool = 
-00001330: 5472 7565 2c20 6675 7475 7265 3a20 626f  True, future: bo
-00001340: 6f6c 203d 2054 7275 6529 2a2a 0a0a 2020  ol = True)**..  
-00001350: 2020 2d64 6179 7320 2874 6865 206e 756d    -days (the num
-00001360: 6265 7220 6f66 2064 6179 7320 696e 746f  ber of days into
-00001370: 2074 6865 2066 7574 7572 6520 746f 2066   the future to f
-00001380: 6574 6368 206d 6174 6368 6573 2066 6f72  etch matches for
-00001390: 290a 2020 0a20 2020 202d 6d69 6e5f 7374  ).  .    -min_st
-000013a0: 6172 5f72 6174 696e 6720 2874 6865 206d  ar_rating (the m
-000013b0: 696e 696d 756d 2073 7461 7220 7261 7469  inimum star rati
-000013c0: 6e67 2066 6f72 206d 6174 6368 6573 2074  ng for matches t
-000013d0: 6f20 696e 636c 7564 6529 0a20 200a 2020  o include).  .  
-000013e0: 2020 6060 600a 2020 2020 6177 6169 7420    ```.    await 
-000013f0: 686c 7476 2e67 6574 5f6d 6174 6368 6573  hltv.get_matches
-00001400: 2864 6179 733d 3129 0a20 2020 200a 2020  (days=1).    .  
-00001410: 2020 3e3e 3e20 5b7b 2769 6427 3a20 2732    >>> [{'id': '2
-00001420: 3337 3132 3031 272c 2027 6461 7465 273a  371201', 'date':
-00001430: 2027 4c49 5645 272c 2027 7469 6d65 273a   'LIVE', 'time':
-00001440: 2027 4c49 5645 272c 2027 7465 616d 3127   'LIVE', 'team1'
-00001450: 3a20 2749 6d70 6572 6961 6c27 2c20 2774  : 'Imperial', 't
-00001460: 6561 6d32 273a 2027 4d49 4252 272c 2027  eam2': 'MIBR', '
-00001470: 7431 5f69 6427 3a20 2739 3435 3527 2c20  t1_id': '9455', 
-00001480: 2774 325f 6964 273a 2027 3932 3135 272c  't2_id': '9215',
-00001490: 2027 6d61 7073 273a 2027 3327 2c20 2772   'maps': '3', 'r
-000014a0: 6174 696e 6727 3a20 312c 2027 6576 656e  ating': 1, 'even
-000014b0: 7427 3a20 2752 4553 2052 6567 696f 6e61  t': 'RES Regiona
-000014c0: 6c20 5365 7269 6573 2033 204c 4154 414d  l Series 3 LATAM
-000014d0: 277d 2c20 7b27 6964 273a 2027 3233 3730  '}, {'id': '2370
-000014e0: 3936 3427 2c20 2764 6174 6527 3a20 2732  964', 'date': '2
-000014f0: 3032 342d 3034 2d31 3627 2c20 2774 696d  024-04-16', 'tim
-00001500: 6527 3a20 2731 323a 3330 272c 2027 7465  e': '12:30', 'te
-00001510: 616d 3127 3a20 2753 4157 272c 2027 7465  am1': 'SAW', 'te
-00001520: 616d 3227 3a20 2753 616d 7069 272c 2027  am2': 'Sampi', '
-00001530: 7431 5f69 6427 3a20 2731 3035 3637 272c  t1_id': '10567',
-00001540: 2027 7432 5f69 6427 3a20 2731 3036 3935   't2_id': '10695
-00001550: 272c 2027 6d61 7073 273a 2027 3327 2c20  ', 'maps': '3', 
-00001560: 2772 6174 696e 6727 3a20 312c 2027 6576  'rating': 1, 'ev
-00001570: 656e 7427 3a20 2754 6875 6e64 6572 7069  ent': 'Thunderpi
-00001580: 636b 2057 6f72 6c64 2043 6861 6d70 696f  ck World Champio
-00001590: 6e73 6869 7020 3230 3234 2045 5520 436c  nship 2024 EU Cl
-000015a0: 6f73 6564 2051 7561 6c69 6669 6572 2031  osed Qualifier 1
-000015b0: 277d 2c20 7b27 6964 273a 2027 3233 3731  '}, {'id': '2371
-000015c0: 3336 3727 2c20 2764 6174 6527 3a20 2732  367', 'date': '2
-000015d0: 3032 342d 3034 2d31 3627 2c20 2774 696d  024-04-16', 'tim
-000015e0: 6527 3a20 2731 343a 3030 272c 2027 7465  e': '14:00', 'te
-000015f0: 616d 3127 3a20 2747 6169 6d69 6e20 476c  am1': 'Gaimin Gl
-00001600: 6164 6961 746f 7273 272c 2027 7465 616d  adiators', 'team
-00001610: 3227 3a20 2750 6572 6d69 7474 6127 2c20  2': 'Permitta', 
-00001620: 2774 315f 6964 273a 2027 3131 3537 3127  't1_id': '11571'
-00001630: 2c20 2774 325f 6964 273a 2027 3132 3030  , 't2_id': '1200
-00001640: 3927 2c20 276d 6170 7327 3a20 2733 272c  9', 'maps': '3',
-00001650: 2027 7261 7469 6e67 273a 2031 2c20 2765   'rating': 1, 'e
-00001660: 7665 6e74 273a 2027 456c 6973 6120 496e  vent': 'Elisa In
-00001670: 7669 7461 7469 6f6e 616c 2053 7072 696e  vitational Sprin
-00001680: 6720 3230 3234 277d 5d0a 2020 2020 0a20  g 2024'}].    . 
-00001690: 2020 2060 6060 0a0a 2a20 2a2a 6765 745f     ```..* **get_
-000016a0: 6d61 7463 685f 696e 666f 286d 6174 6368  match_info(match
-000016b0: 5f69 643a 2069 6e74 207c 2073 7472 2c20  _id: int | str, 
-000016c0: 7465 616d 312c 2074 6561 6d32 2c20 6576  team1, team2, ev
-000016d0: 656e 745f 7469 746c 652c 2073 7461 7473  ent_title, stats
-000016e0: 3a20 626f 6f6c 203d 2054 7275 652c 2070  : bool = True, p
-000016f0: 7265 6469 6374 733a 2062 6f6f 6c20 3d20  redicts: bool = 
-00001700: 5472 7565 292a 2a0a 2020 0a20 2020 2060  True)**.  .    `
-00001710: 6060 0a20 2020 2061 7761 6974 2068 6c74  ``.    await hlt
-00001720: 762e 6765 745f 6d61 7463 685f 696e 666f  v.get_match_info
-00001730: 2832 3337 3039 3331 2c20 274d 6f75 7a27  (2370931, 'Mouz'
-00001740: 2c20 2766 617a 6527 2c20 2769 656d 2d63  , 'faze', 'iem-c
-00001750: 6865 6e67 6475 2d32 3032 3427 2920 200a  hengdu-2024')  .
-00001760: 2020 0a20 2020 203e 3e3e 2832 3337 3039    .    >>>(23709
-00001770: 3331 2c20 2730 272c 2027 3227 2c20 274d  31, '0', '2', 'M
-00001780: 6174 6368 206f 7665 7227 2c20 5b7b 276d  atch over', [{'m
-00001790: 6170 6e61 6d65 273a 2027 4f76 6572 7061  apname': 'Overpa
-000017a0: 7373 272c 2027 725f 7465 616d 3127 3a20  ss', 'r_team1': 
-000017b0: 2731 3027 2c20 2772 5f74 6561 6d32 273a  '10', 'r_team2':
-000017c0: 2027 3133 277d 2c20 7b27 6d61 706e 616d   '13'}, {'mapnam
-000017d0: 6527 3a20 274e 756b 6527 2c20 2772 5f74  e': 'Nuke', 'r_t
-000017e0: 6561 6d31 273a 2027 3627 2c20 2772 5f74  eam1': '6', 'r_t
-000017f0: 6561 6d32 273a 2027 3133 277d 2c20 7b27  eam2': '13'}, {'
-00001800: 6d61 706e 616d 6527 3a20 274d 6972 6167  mapname': 'Mirag
-00001810: 6527 2c20 2772 5f74 6561 6d31 273a 2027  e', 'r_team1': '
-00001820: 2d27 2c20 2772 5f74 6561 6d32 273a 2027  -', 'r_team2': '
-00001830: 2d27 7d5d 2c20 5b7b 2769 6427 3a20 2731  -'}], [{'id': '1
-00001840: 3838 3530 272c 2027 6e69 636b 6e61 6d65  8850', 'nickname
-00001850: 273a 2027 4a69 6d70 7068 6174 272c 2027  ': 'Jimpphat', '
-00001860: 6b64 273a 2027 3333 2d32 3927 2c20 2761  kd': '33-29', 'a
-00001870: 6472 273a 2027 3830 2e39 272c 2027 7261  dr': '80.9', 'ra
-00001880: 7469 6e67 273a 2027 312e 3038 277d 2c20  ting': '1.08'}, 
-00001890: 0a20 200a 2020 2020 7b27 6964 273a 2027  .  .    {'id': '
-000018a0: 3138 3037 3227 2c20 276e 6963 6b6e 616d  18072', 'nicknam
-000018b0: 6527 3a20 2774 6f72 7a73 6927 2c20 276b  e': 'torzsi', 'k
-000018c0: 6427 3a20 2732 362d 3235 272c 2027 6164  d': '26-25', 'ad
-000018d0: 7227 3a20 2737 302e 3527 2c20 2772 6174  r': '70.5', 'rat
-000018e0: 696e 6727 3a20 2731 2e30 3227 7d2c 207b  ing': '1.02'}, {
-000018f0: 2769 6427 3a20 2731 3336 3636 272c 2027  'id': '13666', '
-00001900: 6e69 636b 6e61 6d65 273a 2027 4272 6f6c  nickname': 'Brol
-00001910: 6c61 6e27 2c20 276b 6427 3a20 2732 352d  lan', 'kd': '25-
-00001920: 3331 272c 2027 6164 7227 3a20 2736 382e  31', 'adr': '68.
-00001930: 3427 2c20 2772 6174 696e 6727 3a20 2730  4', 'rating': '0
-00001940: 2e39 3027 7d2c 207b 2769 6427 3a20 2732  .90'}, {'id': '2
-00001950: 3033 3132 272c 2027 6e69 636b 6e61 6d65  0312', 'nickname
-00001960: 273a 2027 7865 7274 696f 4e27 2c20 276b  ': 'xertioN', 'k
-00001970: 6427 3a20 2732 332d 3331 272c 2027 6164  d': '23-31', 'ad
-00001980: 7227 3a20 2736 322e 3427 2c20 2772 6174  r': '62.4', 'rat
-00001990: 696e 6727 3a20 2730 2e38 3227 7d2c 207b  ing': '0.82'}, {
-000019a0: 2769 6427 3a20 2731 3638 3230 272c 2027  'id': '16820', '
-000019b0: 6e69 636b 6e61 6d65 273a 2027 7369 7568  nickname': 'siuh
-000019c0: 7927 2c20 276b 6427 3a20 2731 372d 3330  y', 'kd': '17-30
-000019d0: 272c 2027 6164 7227 3a20 2735 312e 3627  ', 'adr': '51.6'
-000019e0: 2c20 2772 6174 696e 6727 3a20 2730 2e37  , 'rating': '0.7
-000019f0: 3027 7d2c 207b 2769 6427 3a20 2731 3830  0'}, {'id': '180
-00001a00: 3533 272c 2027 6e69 636b 6e61 6d65 273a  53', 'nickname':
-00001a10: 2027 6272 6f6b 7927 2c20 276b 6427 3a20   'broky', 'kd': 
-00001a20: 2733 342d 3232 272c 2027 6164 7227 3a20  '34-22', 'adr': 
-00001a30: 2737 392e 3327 2c20 2772 6174 696e 6727  '79.3', 'rating'
-00001a40: 3a20 2731 2e33 3327 7d2c 207b 2769 6427  : '1.33'}, {'id'
-00001a50: 3a20 2739 3936 3027 2c20 276e 6963 6b6e  : '9960', 'nickn
-00001a60: 616d 6527 3a20 2766 726f 7a65 6e27 2c20  ame': 'frozen', 
-00001a70: 276b 6427 3a20 2733 332d 3233 272c 2027  'kd': '33-23', '
-00001a80: 6164 7227 3a20 2738 352e 3527 2c20 2772  adr': '85.5', 'r
-00001a90: 6174 696e 6727 3a20 2731 2e33 3127 7d2c  ating': '1.31'},
-00001aa0: 207b 2769 6427 3a20 2731 3138 3136 272c   {'id': '11816',
-00001ab0: 2027 6e69 636b 6e61 6d65 273a 2027 726f   'nickname': 'ro
-00001ac0: 707a 272c 2027 6b64 273a 2027 3331 2d32  pz', 'kd': '31-2
-00001ad0: 3627 2c20 2761 6472 273a 2027 3733 2e30  6', 'adr': '73.0
-00001ae0: 272c 2027 7261 7469 6e67 273a 2027 312e  ', 'rating': '1.
-00001af0: 3230 277d 2c20 7b27 6964 273a 2027 3831  20'}, {'id': '81
-00001b00: 3833 272c 2027 6e69 636b 6e61 6d65 273a  83', 'nickname':
-00001b10: 2027 7261 696e 272c 2027 6b64 273a 2027   'rain', 'kd': '
-00001b20: 3237 2d32 3627 2c20 2761 6472 273a 2027  27-26', 'adr': '
-00001b30: 3832 2e30 272c 2027 7261 7469 6e67 273a  82.0', 'rating':
-00001b40: 2027 312e 3138 277d 2c20 7b27 6964 273a   '1.18'}, {'id':
-00001b50: 2027 3432 3927 2c20 276e 6963 6b6e 616d   '429', 'nicknam
-00001b60: 6527 3a20 276b 6172 7269 6761 6e27 2c20  e': 'karrigan', 
-00001b70: 276b 6427 3a20 2732 302d 3238 272c 2027  'kd': '20-28', '
-00001b80: 6164 7227 3a20 2734 392e 3727 2c20 2772  adr': '49.7', 'r
-00001b90: 6174 696e 6727 3a20 2730 2e38 3127 7d5d  ating': '0.81'}]
-00001ba0: 2920 200a 2020 2020 0a20 2020 2060 6060  )  .    .    ```
-00001bb0: 0a20 200a 2a20 2a2a 6765 745f 7265 7375  .  .* **get_resu
-00001bc0: 6c74 7328 6461 7973 3a20 696e 7420 3d20  lts(days: int = 
-00001bd0: 312c 206d 696e 5f72 6174 696e 673a 2069  1, min_rating: i
-00001be0: 6e74 203d 2031 2c20 6d61 783a 2069 6e74  nt = 1, max: int
-00001bf0: 203d 2033 302c 2066 6561 7475 7265 643a   = 30, featured:
-00001c00: 2062 6f6f 6c20 3d20 5472 7565 2c20 7265   bool = True, re
-00001c10: 6775 6c61 723a 2062 6f6f 6c20 3d20 5472  gular: bool = Tr
-00001c20: 7565 2929 202d 3e2a 2a0a 2020 2020 0a20  ue)) ->**.    . 
-00001c30: 2020 2060 6060 0a20 2020 2070 7269 6e74     ```.    print
-00001c40: 2861 7761 6974 2068 6c74 762e 6765 745f  (await hltv.get_
-00001c50: 7265 7375 6c74 7328 2929 0a20 200a 2020  results()).  .  
-00001c60: 2020 5b7b 2769 6427 3a20 2732 3337 3039    [{'id': '23709
-00001c70: 3331 272c 2027 7465 616d 3127 3a20 274d  31', 'team1': 'M
-00001c80: 4f55 5a27 2c20 2774 6561 6d32 273a 2027  OUZ', 'team2': '
-00001c90: 4661 5a65 272c 2027 7363 6f72 6531 273a  FaZe', 'score1':
-00001ca0: 2027 3027 2c20 2773 636f 7265 3227 3a20   '0', 'score2': 
-00001cb0: 2732 272c 2027 7261 7469 6e67 273a 2030  '2', 'rating': 0
-00001cc0: 2c20 2765 7665 6e74 273a 2027 4945 4d20  , 'event': 'IEM 
-00001cd0: 4368 656e 6764 7520 3230 3234 277d 5d0a  Chengdu 2024'}].
-00001ce0: 2020 2020 6060 600a 2020 0a2a 202a 2a67      ```.  .* **g
-00001cf0: 6574 5f65 7665 6e74 7328 6f75 7467 6f69  et_events(outgoi
-00001d00: 6e67 3d54 7275 652c 2066 7574 7572 653d  ng=True, future=
-00001d10: 5472 7565 2c20 6d61 785f 6576 656e 7473  True, max_events
-00001d20: 3d31 3029 202d 3e20 5b28 2769 6427 2c20  =10) -> [('id', 
-00001d30: 2774 6974 6c65 272c 2027 7374 6172 7464  'title', 'startd
-00001d40: 6174 6527 2c20 2765 6e64 6461 7465 2729  ate', 'enddate')
-00001d50: 5d2a 2a0a 0a20 2020 2060 6060 0a20 2020  ]**..    ```.   
-00001d60: 2061 7761 6974 2068 6c74 762e 6765 745f   await hltv.get_
-00001d70: 6576 656e 7473 2866 7574 7572 653d 4661  events(future=Fa
-00001d80: 6c73 6529 0a20 2020 200a 2020 2020 3e3e  lse).    .    >>
-00001d90: 3e5b 7b27 6964 273a 2027 3737 3439 272c  >[{'id': '7749',
-00001da0: 2027 7469 746c 6527 3a20 2754 6875 6e64   'title': 'Thund
-00001db0: 6572 7069 636b 2057 6f72 6c64 2043 6861  erpick World Cha
-00001dc0: 6d70 696f 6e73 6869 7020 3230 3234 2045  mpionship 2024 E
-00001dd0: 5520 436c 6f73 6564 2051 7561 6c69 6669  U Closed Qualifi
-00001de0: 6572 2031 272c 2027 7374 6172 745f 6461  er 1', 'start_da
-00001df0: 7465 273a 2027 312d 3427 2c20 2765 6e64  te': '1-4', 'end
-00001e00: 5f64 6174 6527 3a20 2732 322d 3427 7d2c  _date': '22-4'},
-00001e10: 207b 2769 6427 3a20 2737 3632 3127 2c20   {'id': '7621', 
-00001e20: 2774 6974 6c65 273a 2027 4553 4c20 4368  'title': 'ESL Ch
-00001e30: 616c 6c65 6e67 6572 204c 6561 6775 6520  allenger League 
-00001e40: 5365 6173 6f6e 2034 3720 4e6f 7274 6820  Season 47 North 
-00001e50: 416d 6572 6963 6127 2c20 2773 7461 7274  America', 'start
-00001e60: 5f64 6174 6527 3a20 2731 332d 3227 2c20  _date': '13-2', 
-00001e70: 2765 6e64 5f64 6174 6527 3a20 2731 362d  'end_date': '16-
-00001e80: 3627 7d5d 0a20 2020 2020 200a 2020 2020  6'}].      .    
-00001e90: 6060 600a 0a2a 202a 2a67 6574 5f65 7665  ```..* **get_eve
-00001ea0: 6e74 5f72 6573 756c 7473 2865 7665 6e74  nt_results(event
-00001eb0: 5f69 643a 2069 6e74 207c 2073 7472 2c20  _id: int | str, 
-00001ec0: 6461 7973 3a20 696e 7420 3d20 312c 206d  days: int = 1, m
-00001ed0: 6178 5f3a 2069 6e74 203d 2031 3029 2a2a  ax_: int = 10)**
-00001ee0: 0a0a 2020 0a20 2020 2060 6060 0a20 2020  ..  .    ```.   
-00001ef0: 2061 7761 6974 2067 6574 5f65 7665 6e74   await get_event
-00001f00: 5f72 6573 756c 7473 2837 3134 3829 0a20  _results(7148). 
-00001f10: 2020 200a 2020 2020 3e3e 3e5b 7b27 6964     .    >>>[{'id
-00001f20: 273a 2027 3233 3730 3933 3127 2c20 2764  ': '2370931', 'd
-00001f30: 6174 6527 3a20 2731 342d 3034 2d32 3032  ate': '14-04-202
-00001f40: 3427 2c20 2774 6561 6d31 273a 2027 4d4f  4', 'team1': 'MO
-00001f50: 555a 272c 2027 7465 616d 3227 3a20 2746  UZ', 'team2': 'F
-00001f60: 615a 6527 2c20 2773 636f 7265 3127 3a20  aZe', 'score1': 
-00001f70: 2730 272c 2027 7363 6f72 6532 273a 2027  '0', 'score2': '
-00001f80: 3227 7d5d 0a0a 2020 2020 6060 600a 0a2a  2'}]..    ```..*
-00001f90: 202a 2a67 6574 5f65 7665 6e74 5f6d 6174   **get_event_mat
-00001fa0: 6368 6573 2865 7665 6e74 5f69 643a 2073  ches(event_id: s
-00001fb0: 7472 207c 2069 6e74 2c20 6461 7973 3a20  tr | int, days: 
-00001fc0: 696e 7420 3d20 3129 3a2a 2a0a 2020 0a20  int = 1):**.  . 
-00001fd0: 2020 2060 6060 0a20 2020 2061 7761 6974     ```.    await
-00001fe0: 2068 6c74 762e 6765 745f 6576 656e 745f   hltv.get_event_
-00001ff0: 6d61 7463 6865 7328 3731 3438 290a 2020  matches(7148).  
-00002000: 2020 0a20 2020 203e 3e3e 5b7b 2769 6427    .    >>>[{'id'
-00002010: 3a20 2732 3337 3037 3731 272c 2027 6461  : '2370771', 'da
-00002020: 7465 273a 2027 3230 3234 2d30 342d 3138  te': '2024-04-18
-00002030: 272c 2027 7469 6d65 273a 2027 3135 3a33  ', 'time': '15:3
-00002040: 3027 2c20 2774 6561 6d31 273a 2027 4d6f  0', 'team1': 'Mo
-00002050: 6e74 6527 2c20 2774 6561 6d32 273a 2027  nte', 'team2': '
-00002060: 7061 694e 272c 2027 7431 5f69 6427 3a20  paiN', 't1_id': 
-00002070: 2731 3138 3131 272c 2027 7432 5f69 6427  '11811', 't2_id'
-00002080: 3a20 2734 3737 3327 7d2c 207b 2769 6427  : '4773'}, {'id'
-00002090: 3a20 2732 3337 3037 3732 272c 2027 6461  : '2370772', 'da
-000020a0: 7465 273a 2027 3230 3234 2d30 342d 3138  te': '2024-04-18
-000020b0: 272c 2027 7469 6d65 273a 2027 3137 3a30  ', 'time': '17:0
-000020c0: 3027 2c20 2774 6561 6d31 273a 2027 496d  0', 'team1': 'Im
-000020d0: 7065 7269 616c 272c 2027 7465 616d 3227  perial', 'team2'
-000020e0: 3a20 274d 6574 697a 706f 7274 272c 2027  : 'Metizport', '
-000020f0: 7431 5f69 6427 3a20 2739 3435 3527 2c20  t1_id': '9455', 
-00002100: 2774 325f 6964 273a 2027 3131 3634 3127  't2_id': '11641'
-00002110: 7d2c 207b 2769 6427 3a20 2732 3337 3037  }, {'id': '23707
-00002120: 3733 272c 2027 6461 7465 273a 2027 3230  73', 'date': '20
-00002130: 3234 2d30 342d 3138 272c 2027 7469 6d65  24-04-18', 'time
-00002140: 273a 2027 3138 3a33 3027 2c20 2774 6561  ': '18:30', 'tea
-00002150: 6d31 273a 2027 4655 5249 4127 2c20 2774  m1': 'FURIA', 't
-00002160: 6561 6d32 273a 2027 397a 272c 2027 7431  eam2': '9z', 't1
-00002170: 5f69 6427 3a20 2738 3239 3727 2c20 2774  _id': '8297', 't
-00002180: 325f 6964 273a 2027 3939 3936 277d 2c20  2_id': '9996'}, 
-00002190: 7b27 6964 273a 2027 3233 3730 3737 3427  {'id': '2370774'
-000021a0: 2c20 2764 6174 6527 3a20 2732 3032 342d  , 'date': '2024-
-000021b0: 3034 2d31 3827 2c20 2774 696d 6527 3a20  04-18', 'time': 
-000021c0: 2732 303a 3030 272c 2027 7465 616d 3127  '20:00', 'team1'
-000021d0: 3a20 274d 4942 5227 2c20 2774 6561 6d32  : 'MIBR', 'team2
-000021e0: 273a 2027 4f47 272c 2027 7431 5f69 6427  ': 'OG', 't1_id'
-000021f0: 3a20 2739 3231 3527 2c20 2774 325f 6964  : '9215', 't2_id
-00002200: 273a 2027 3130 3530 3327 7d2c 207b 2769  ': '10503'}, {'i
-00002210: 6427 3a20 2732 3337 3037 3735 272c 2027  d': '2370775', '
-00002220: 6461 7465 273a 2027 3230 3234 2d30 342d  date': '2024-04-
-00002230: 3138 272c 2027 7469 6d65 273a 2027 3231  18', 'time': '21
-00002240: 3a33 3027 2c20 2774 6561 6d31 273a 2027  :30', 'team1': '
-00002250: 5442 4427 2c20 2774 6561 6d32 273a 2027  TBD', 'team2': '
-00002260: 5442 4427 2c20 2774 315f 6964 273a 2030  TBD', 't1_id': 0
-00002270: 2c20 2774 325f 6964 273a 2030 7d2c 207b  , 't2_id': 0}, {
-00002280: 2769 6427 3a20 2732 3337 3037 3736 272c  'id': '2370776',
-00002290: 2027 6461 7465 273a 2027 3230 3234 2d30   'date': '2024-0
-000022a0: 342d 3138 272c 2027 7469 6d65 273a 2027  4-18', 'time': '
-000022b0: 3233 3a30 3027 2c20 2774 6561 6d31 273a  23:00', 'team1':
-000022c0: 2027 5442 4427 2c20 2774 6561 6d32 273a   'TBD', 'team2':
-000022d0: 2027 5442 4427 2c20 2774 315f 6964 273a   'TBD', 't1_id':
-000022e0: 2030 2c20 2774 325f 6964 273a 2030 7d2c   0, 't2_id': 0},
-000022f0: 207b 2769 6427 3a20 2732 3337 3037 3737   {'id': '2370777
-00002300: 272c 2027 6461 7465 273a 2027 3230 3234  ', 'date': '2024
-00002310: 2d30 342d 3139 272c 2027 7469 6d65 273a  -04-19', 'time':
-00002320: 2027 3030 3a30 3027 2c20 2774 6561 6d31   '00:00', 'team1
-00002330: 273a 2027 5442 4427 2c20 2774 6561 6d32  ': 'TBD', 'team2
-00002340: 273a 2027 5442 4427 2c20 2774 315f 6964  ': 'TBD', 't1_id
-00002350: 273a 2030 2c20 2774 325f 6964 273a 2030  ': 0, 't2_id': 0
-00002360: 7d2c 207b 2769 6427 3a20 2732 3337 3037  }, {'id': '23707
-00002370: 3738 272c 2027 6461 7465 273a 2027 3230  78', 'date': '20
-00002380: 3234 2d30 342d 3139 272c 2027 7469 6d65  24-04-19', 'time
-00002390: 273a 2027 3135 3a30 3027 2c20 2774 6561  ': '15:00', 'tea
-000023a0: 6d31 273a 2027 5442 4427 2c20 2774 6561  m1': 'TBD', 'tea
-000023b0: 6d32 273a 2027 5442 4427 2c20 2774 315f  m2': 'TBD', 't1_
-000023c0: 6964 273a 2030 2c20 2774 325f 6964 273a  id': 0, 't2_id':
-000023d0: 2030 7d2c 207b 2769 6427 3a20 2732 3337   0}, {'id': '237
-000023e0: 3037 3739 272c 2027 6461 7465 273a 2027  0779', 'date': '
-000023f0: 3230 3234 2d30 342d 3139 272c 2027 7469  2024-04-19', 'ti
-00002400: 6d65 273a 2027 3137 3a33 3027 2c20 2774  me': '17:30', 't
-00002410: 6561 6d31 273a 2027 5442 4427 2c20 2774  eam1': 'TBD', 't
-00002420: 6561 6d32 273a 2027 5442 4427 2c20 2774  eam2': 'TBD', 't
-00002430: 315f 6964 273a 2030 2c20 2774 325f 6964  1_id': 0, 't2_id
-00002440: 273a 2030 7d2c 207b 2769 6427 3a20 2732  ': 0}, {'id': '2
-00002450: 3337 3037 3830 272c 2027 6461 7465 273a  370780', 'date':
-00002460: 2027 3230 3234 2d30 342d 3139 272c 2027   '2024-04-19', '
-00002470: 7469 6d65 273a 2027 3230 3a30 3027 2c20  time': '20:00', 
-00002480: 2774 6561 6d31 273a 2027 5442 4427 2c20  'team1': 'TBD', 
-00002490: 2774 6561 6d32 273a 2027 5442 4427 2c20  'team2': 'TBD', 
-000024a0: 2774 315f 6964 273a 2030 2c20 2774 325f  't1_id': 0, 't2_
-000024b0: 6964 273a 2030 7d2c 207b 2769 6427 3a20  id': 0}, {'id': 
-000024c0: 2732 3337 3037 3831 272c 2027 6461 7465  '2370781', 'date
-000024d0: 273a 2027 3230 3234 2d30 342d 3139 272c  ': '2024-04-19',
-000024e0: 2027 7469 6d65 273a 2027 3232 3a33 3027   'time': '22:30'
-000024f0: 2c20 2774 6561 6d31 273a 2027 5442 4427  , 'team1': 'TBD'
-00002500: 2c20 2774 6561 6d32 273a 2027 5442 4427  , 'team2': 'TBD'
-00002510: 2c20 2774 315f 6964 273a 2030 2c20 2774  , 't1_id': 0, 't
-00002520: 325f 6964 273a 2030 7d2c 207b 2769 6427  2_id': 0}, {'id'
-00002530: 3a20 2732 3337 3037 3832 272c 2027 6461  : '2370782', 'da
-00002540: 7465 273a 2027 3230 3234 2d30 342d 3230  te': '2024-04-20
-00002550: 272c 2027 7469 6d65 273a 2027 3030 3a33  ', 'time': '00:3
-00002560: 3027 2c20 2774 6561 6d31 273a 2027 5442  0', 'team1': 'TB
-00002570: 4427 2c20 2774 6561 6d32 273a 2027 5442  D', 'team2': 'TB
-00002580: 4427 2c20 2774 315f 6964 273a 2030 2c20  D', 't1_id': 0, 
-00002590: 2774 325f 6964 273a 2030 7d2c 207b 2769  't2_id': 0}, {'i
-000025a0: 6427 3a20 2732 3337 3037 3833 272c 2027  d': '2370783', '
-000025b0: 6461 7465 273a 2027 3230 3234 2d30 342d  date': '2024-04-
-000025c0: 3230 272c 2027 7469 6d65 273a 2027 3135  20', 'time': '15
-000025d0: 3a30 3027 2c20 2774 6561 6d31 273a 2027  :00', 'team1': '
-000025e0: 5442 4427 2c20 2774 6561 6d32 273a 2027  TBD', 'team2': '
-000025f0: 5442 4427 2c20 2774 315f 6964 273a 2030  TBD', 't1_id': 0
-00002600: 2c20 2774 325f 6964 273a 2030 7d2c 207b  , 't2_id': 0}, {
-00002610: 2769 6427 3a20 2732 3337 3037 3834 272c  'id': '2370784',
-00002620: 2027 6461 7465 273a 2027 3230 3234 2d30   'date': '2024-0
-00002630: 342d 3230 272c 2027 7469 6d65 273a 2027  4-20', 'time': '
-00002640: 3138 3a30 3027 2c20 2774 6561 6d31 273a  18:00', 'team1':
-00002650: 2027 5442 4427 2c20 2774 6561 6d32 273a   'TBD', 'team2':
-00002660: 2027 5442 4427 2c20 2774 315f 6964 273a   'TBD', 't1_id':
-00002670: 2030 2c20 2774 325f 6964 273a 2030 7d5d   0, 't2_id': 0}]
-00002680: 0a20 200a 2020 2020 6060 600a 0a2a 202a  .  .    ```..* *
-00002690: 2a67 6574 5f65 7665 6e74 5f69 6e66 6f28  *get_event_info(
-000026a0: 6576 656e 745f 6964 3a20 7374 7220 7c20  event_id: str | 
-000026b0: 696e 742c 2065 7665 6e74 5f74 6974 6c65  int, event_title
-000026c0: 3a20 7374 7229 202d 3e20 2865 7665 6e74  : str) -> (event
-000026d0: 5f69 642c 2065 7665 6e74 5f74 6974 6c65  _id, event_title
-000026e0: 2c20 6576 656e 745f 7374 6172 742c 2065  , event_start, e
-000026f0: 7665 6e74 5f65 6e64 2c20 7072 697a 652c  vent_end, prize,
-00002700: 2074 6561 6d5f 6e75 6d2c 206c 6f63 6174   team_num, locat
-00002710: 696f 6e2c 2067 726f 7570 7329 2a2a 0a0a  ion, groups)**..
-00002720: 2020 2020 6060 600a 2020 2020 6177 6169      ```.    awai
-00002730: 7420 686c 7476 2e67 6574 5f65 7665 6e74  t hltv.get_event
-00002740: 5f69 6e66 6f28 3731 3438 2c20 2750 474c  _info(7148, 'PGL
-00002750: 2043 5332 204d 616a 6f72 2043 6f70 656e   CS2 Major Copen
-00002760: 6861 6765 6e32 3032 3427 290a 2020 2020  hagen2024').    
-00002770: 0a20 2020 207b 2769 6427 3a20 3731 3438  .    {'id': 7148
-00002780: 2c20 2774 6974 6c65 273a 2027 5047 4c20  , 'title': 'PGL 
-00002790: 4353 3220 4d61 6a6f 7220 436f 7065 6e68  CS2 Major Copenh
-000027a0: 6167 656e 3230 3234 272c 2027 7374 6172  agen2024', 'star
-000027b0: 7427 3a20 2732 312d 3327 2c20 2765 6e64  t': '21-3', 'end
-000027c0: 273a 2027 3331 2d33 272c 2027 7072 697a  ': '31-3', 'priz
-000027d0: 6527 3a20 2724 312c 3235 302c 3030 3027  e': '$1,250,000'
-000027e0: 2c20 2774 6561 6d73 273a 2027 3136 272c  , 'teams': '16',
-000027f0: 2027 6c6f 6361 7469 6f6e 273a 2027 436f   'location': 'Co
-00002800: 7065 6e68 6167 656e 2c20 4465 6e6d 6172  penhagen, Denmar
-00002810: 6b27 2c20 2767 726f 7570 273a 205b 5d7d  k', 'group': []}
-00002820: 0a20 2020 0a20 2020 2060 6060 0a0a 0a2a  .   .    ```...*
-00002830: 202a 2a67 6574 5f74 6f70 5f74 6561 6d73   **get_top_teams
-00002840: 286d 6178 5f74 6561 6d73 3d33 3029 202d  (max_teams=30) -
-00002850: 3e20 5b27 7261 6e6b 272c 2027 7469 746c  > ['rank', 'titl
-00002860: 6527 2c20 2770 6f69 6e74 7327 2c20 2763  e', 'points', 'c
-00002870: 6861 6e67 6527 2c20 2769 6427 5d2a 2a0a  hange', 'id']**.
-00002880: 0a20 2020 2060 6060 0a20 2020 2061 7761  .    ```.    awa
-00002890: 6974 2068 6c74 762e 6765 745f 746f 705f  it hltv.get_top_
-000028a0: 7465 616d 7328 3229 0a20 2020 200a 2020  teams(2).    .  
-000028b0: 2020 3e3e 3e5b 7b27 6964 273a 2027 3131    >>>[{'id': '11
-000028c0: 3131 272c 2027 7261 6e6b 273a 2027 3127  11', 'rank': '1'
-000028d0: 2c20 2774 6974 6c65 273a 2027 4661 5a65  , 'title': 'FaZe
-000028e0: 272c 2027 706f 696e 7473 273a 2027 3933  ', 'points': '93
-000028f0: 3927 2c20 2763 6861 6e67 6527 3a20 272d  9', 'change': '-
-00002900: 272c 2027 6964 273a 2027 3636 3637 277d  ', 'id': '6667'}
-00002910: 2c20 7b27 6964 273a 2027 3131 3131 272c  , {'id': '1111',
-00002920: 2027 7261 6e6b 273a 2027 3227 2c20 2774   'rank': '2', 't
-00002930: 6974 6c65 273a 2027 4e61 7475 7320 5669  itle': 'Natus Vi
-00002940: 6e63 6572 6527 2c20 2770 6f69 6e74 7327  ncere', 'points'
-00002950: 3a20 2737 3537 272c 2027 6368 616e 6765  : '757', 'change
-00002960: 273a 2027 2b34 272c 2027 6964 273a 2027  ': '+4', 'id': '
-00002970: 3436 3038 277d 5d0a 2020 2020 6060 600a  4608'}].    ```.
-00002980: 0a2a 202a 2a67 6574 5f74 6561 6d5f 696e  .* **get_team_in
-00002990: 666f 2874 6561 6d5f 6964 3a20 696e 7420  fo(team_id: int 
-000029a0: 7c20 7374 722c 2074 6974 6c65 3a20 7374  | str, title: st
-000029b0: 7229 202d 3e20 2874 6561 6d5f 6964 2c20  r) -> (team_id, 
-000029c0: 7465 616d 5f74 6974 6c65 2c20 7261 6e6b  team_title, rank
-000029d0: 2c20 7b27 706c 6179 6572 273a 706c 6179  , {'player':play
-000029e0: 6572 5f69 647d 2c20 636f 6163 682c 2061  er_id}, coach, a
-000029f0: 7665 7261 6765 5f61 6765 2c20 7765 656b  verage_age, week
-00002a00: 735f 696e 5f74 6f70 5f32 302c 206c 6173  s_in_top_20, las
-00002a10: 745f 7472 6f70 6879 2c20 746f 7461 6c5f  t_trophy, total_
-00002a20: 7472 6f70 6879 7329 2a2a 0a0a 2020 2020  trophys)**..    
-00002a30: 6060 600a 2020 2020 6177 6169 7420 686c  ```.    await hl
-00002a40: 7476 2e67 6574 5f74 6561 6d5f 696e 666f  tv.get_team_info
-00002a50: 2836 3636 372c 2027 6661 7a65 2729 0a20  (6667, 'faze'). 
-00002a60: 2020 200a 2020 2020 3e3e 3e7b 2769 6427     .    >>>{'id'
-00002a70: 3a20 3636 3637 2c20 2774 6974 6c65 273a  : 6667, 'title':
-00002a80: 2027 6661 7a65 272c 2027 7261 6e6b 273a   'faze', 'rank':
-00002a90: 2027 3127 2c20 2770 6c61 7965 7273 273a   '1', 'players':
-00002aa0: 207b 276b 6172 7269 6761 6e27 3a20 3432   {'karrigan': 42
-00002ab0: 392c 2027 7261 696e 273a 2038 3138 332c  9, 'rain': 8183,
-00002ac0: 2027 6672 6f7a 656e 273a 2039 3936 302c   'frozen': 9960,
-00002ad0: 2027 726f 707a 273a 2031 3138 3136 2c20   'ropz': 11816, 
-00002ae0: 2762 726f 6b79 273a 2031 3830 3533 7d2c  'broky': 18053},
-00002af0: 2027 636f 6163 6827 3a20 274e 454f 272c   'coach': 'NEO',
-00002b00: 2027 6167 6527 3a20 2732 362e 3627 2c20   'age': '26.6', 
-00002b10: 2777 6565 6b73 746f 7033 3027 3a20 2732  'weekstop30': '2
-00002b20: 3630 272c 2027 6c61 7374 5f74 726f 7068  60', 'last_troph
-00002b30: 7927 3a20 2749 454d 2043 6865 6e67 6475  y': 'IEM Chengdu
-00002b40: 2032 3032 3427 2c20 2774 6f74 616c 5f74   2024', 'total_t
-00002b50: 726f 7068 6965 7327 3a20 3232 7d0a 2020  rophies': 22}.  
-00002b60: 2020 6060 600a 0a2a 202a 2a67 6574 5f6c    ```..* **get_l
-00002b70: 6173 745f 6e65 7773 286d 6178 5f72 6567  ast_news(max_reg
-00002b80: 5f6e 6577 733d 322c 206f 6e6c 795f 746f  _news=2, only_to
-00002b90: 6461 793d 5472 7565 2c20 6f6e 6c79 5f66  day=True, only_f
-00002ba0: 6561 7475 7265 643d 4661 6c73 6529 202d  eatured=False) -
-00002bb0: 3e20 5b64 6174 652c 205b 6665 6174 7572  > [date, [featur
-00002bc0: 6564 5f69 642c 2066 6561 7475 7265 645f  ed_id, featured_
-00002bd0: 7469 746c 652c 2066 6561 7475 7265 645f  title, featured_
-00002be0: 6465 7363 6970 7469 6f6e 5d2c 205b 7265  desciption], [re
-00002bf0: 6775 6c61 725f 6964 2c20 7265 675f 7469  gular_id, reg_ti
-00002c00: 746c 652c 2072 6567 5f74 696d 655d 5d2a  tle, reg_time]]*
-00002c10: 2a0a 0a20 2020 2060 6060 0a20 2020 2061  *..    ```.    a
-00002c20: 7761 6974 2068 6c74 762e 6765 745f 6c61  wait hltv.get_la
-00002c30: 7374 5f6e 6577 7328 6f6e 6c79 5f74 6f64  st_news(only_tod
-00002c40: 6179 3d54 7275 6529 0a20 2020 200a 2020  ay=True).    .  
-00002c50: 2020 3e3e 3e5b 7b27 6461 7465 273a 2027    >>>[{'date': '
-00002c60: 3135 2d30 3427 2c20 2766 5f6e 6577 7327  15-04', 'f_news'
-00002c70: 3a20 5b5d 2c20 276e 6577 7327 3a20 5b7b  : [], 'news': [{
-00002c80: 2769 6427 3a20 2733 3837 3834 272c 2027  'id': '38784', '
-00002c90: 7469 746c 6527 3a20 274d 6564 6961 3a20  title': 'Media: 
-00002ca0: 4655 5249 4120 7072 6163 7469 6369 6e67  FURIA practicing
-00002cb0: 2077 6974 6820 6b79 6520 696e 2070 6c61   with kye in pla
-00002cc0: 6365 206f 6620 6172 5427 2c20 2770 6f73  ce of arT', 'pos
-00002cd0: 7465 6427 3a20 2761 6e20 686f 7572 2061  ted': 'an hour a
-00002ce0: 676f 277d 2c20 7b27 6964 273a 2027 3338  go'}, {'id': '38
-00002cf0: 3738 3327 2c20 2774 6974 6c65 273a 2027  783', 'title': '
-00002d00: 656c 6563 7472 6f4e 6963 2074 6f20 706c  electroNic to pl
-00002d10: 6179 2066 6f72 2056 6972 7475 732e 7072  ay for Virtus.pr
-00002d20: 6f20 6174 2045 534c 2050 726f 204c 6561  o at ESL Pro Lea
-00002d30: 6775 6520 5331 3927 2c20 2770 6f73 7465  gue S19', 'poste
-00002d40: 6427 3a20 2732 2068 6f75 7273 2061 676f  d': '2 hours ago
-00002d50: 277d 2c20 7b27 6964 273a 2027 3338 3738  '}, {'id': '3878
-00002d60: 3127 2c20 2774 6974 6c65 273a 2027 5468  1', 'title': 'Th
-00002d70: 6520 4556 5073 2061 6e64 2042 6573 7420  e EVPs and Best 
-00002d80: 4669 7665 206f 6620 4945 4d20 4368 656e  Five of IEM Chen
-00002d90: 6764 7527 2c20 2770 6f73 7465 6427 3a20  gdu', 'posted': 
-00002da0: 2737 2068 6f75 7273 2061 676f 277d 5d7d  '7 hours ago'}]}
-00002db0: 5d0a 2020 0a20 2020 2060 6060 0a0a 2a20  ].  .    ```..* 
-00002dc0: 2a2a 6765 745f 6265 7374 5f70 6c61 7965  **get_best_playe
-00002dd0: 7273 2874 6f70 3a20 696e 7420 3d20 3430  rs(top: int = 40
-00002de0: 2920 2d3e 2028 2772 616e 6b27 2c20 276e  ) -> ('rank', 'n
-00002df0: 616d 6527 2c20 2774 6561 6d27 2c20 276d  ame', 'team', 'm
-00002e00: 6170 7327 2c20 2772 6174 696e 6727 292a  aps', 'rating')*
-00002e10: 2a0a 0a20 2020 2060 6060 0a20 2020 2061  *..    ```.    a
-00002e20: 7761 6974 2068 6c74 762e 6765 745f 6265  wait hltv.get_be
-00002e30: 7374 5f70 6c61 7965 7273 2832 290a 2020  st_players(2).  
-00002e40: 2020 0a20 2020 203e 3e3e 5b7b 2769 6427    .    >>>[{'id'
-00002e50: 3a20 2731 3932 3330 272c 2027 7261 6e6b  : '19230', 'rank
-00002e60: 273a 2031 2c20 276e 616d 6527 3a20 276d  ': 1, 'name': 'm
-00002e70: 304e 4553 5927 2c20 2774 6561 6d27 3a20  0NESY', 'team': 
-00002e80: 2747 3227 2c20 276d 6170 7327 3a20 2734  'G2', 'maps': '4
-00002e90: 3427 2c20 2772 6174 696e 6727 3a20 2731  4', 'rating': '1
-00002ea0: 2e33 3727 7d2c 207b 2769 6427 3a20 2731  .37'}, {'id': '1
-00002eb0: 3830 3533 272c 2027 7261 6e6b 273a 2032  8053', 'rank': 2
-00002ec0: 2c20 276e 616d 6527 3a20 2762 726f 6b79  , 'name': 'broky
-00002ed0: 272c 2027 7465 616d 273a 2027 4661 5a65  ', 'team': 'FaZe
-00002ee0: 272c 2027 6d61 7073 273a 2027 3534 272c  ', 'maps': '54',
-00002ef0: 2027 7261 7469 6e67 273a 2027 312e 3139   'rating': '1.19
-00002f00: 277d 5d0a 2020 2020 6060 600a 0a2a 202a  '}].    ```..* *
-00002f10: 2a67 6574 5f70 6c61 7965 725f 696e 666f  *get_player_info
-00002f20: 2869 643a 2073 7472 207c 2069 6e74 2c20  (id: str | int, 
-00002f30: 6e69 636b 6e61 6d65 3a20 7374 7229 2a2a  nickname: str)**
-00002f40: 0a20 200a 2020 6060 600a 2020 6177 6169  .  .  ```.  awai
-00002f50: 7420 686c 7476 2e67 6574 5f70 6c61 7965  t hltv.get_playe
-00002f60: 725f 696e 666f 2837 3939 382c 2027 7331  r_info(7998, 's1
-00002f70: 6d70 6c65 2729 0a20 200a 2020 7b27 6964  mple').  .  {'id
-00002f80: 273a 2037 3939 382c 2027 6e69 636b 6e61  ': 7998, 'nickna
-00002f90: 6d65 273a 2027 7331 6d70 6c65 272c 2027  me': 's1mple', '
-00002fa0: 7465 616d 273a 2027 4e61 7475 7320 5669  team': 'Natus Vi
-00002fb0: 6e63 6572 6527 2c20 2774 6561 6d5f 6964  ncere', 'team_id
-00002fc0: 273a 2034 3630 382c 2027 6e61 6d65 273a  ': 4608, 'name':
-00002fd0: 2027 4f6c 656b 7361 6e64 7220 4b6f 7374   'Oleksandr Kost
-00002fe0: 796c 6965 7627 2c20 276e 6174 696f 6e61  yliev', 'nationa
-00002ff0: 6c69 7479 273a 2027 556b 7261 696e 6527  lity': 'Ukraine'
-00003000: 2c20 2761 6765 273a 2032 362c 2027 7261  , 'age': 26, 'ra
-00003010: 7469 6e67 273a 2027 302e 3934 272c 2027  ting': '0.94', '
-00003020: 6b70 7227 3a20 2730 2e36 3027 2c20 2768  kpr': '0.60', 'h
-00003030: 7327 3a20 2735 372e 3925 272c 2027 6c61  s': '57.9%', 'la
-00003040: 7374 5f6d 6174 6368 6573 273a 205b 3130  st_matches': [10
-00003050: 3330 3539 2c20 3939 3734 352c 2039 3937  3059, 99745, 997
-00003060: 3238 2c20 3939 3639 362c 2039 3934 3731  28, 99696, 99471
-00003070: 2c20 3939 3336 345d 2c20 276c 6173 745f  , 99364], 'last_
-00003080: 7472 6f70 6879 273a 2027 424c 4153 5420  trophy': 'BLAST 
-00003090: 5072 656d 6965 7220 5370 7269 6e67 2046  Premier Spring F
-000030a0: 696e 616c 2032 3032 3227 2c20 2774 6f74  inal 2022', 'tot
-000030b0: 616c 5f74 726f 7068 6965 7327 3a20 3330  al_trophies': 30
-000030c0: 2c20 2774 6f74 616c 5f6d 7670 7327 3a20  , 'total_mvps': 
-000030d0: 3231 7d0a 2020 6060 600a 0a2a 202a 2a67  21}.  ```..* **g
-000030e0: 6574 2874 7970 653a 2073 7472 2c20 6964  et(type: str, id
-000030f0: 3a20 696e 7420 7c20 7374 7220 7c20 4e6f  : int | str | No
-00003100: 6e65 203d 204e 6f6e 652c 2074 6974 6c65  ne = None, title
-00003110: 3a20 7374 7220 7c20 4e6f 6e65 203d 204e  : str | None = N
-00003120: 6f6e 652c 2074 6561 6d31 3a20 7374 7220  one, team1: str 
-00003130: 7c20 4e6f 6e65 203d 204e 6f6e 652c 2074  | None = None, t
-00003140: 6561 6d32 3a20 7374 7220 7c20 4e6f 6e65  eam2: str | None
-00003150: 203d 204e 6f6e 6529 3a2a 2a0a 2020 2842   = None):**.  (B
-00003160: 4554 4129 2054 6869 7320 6d65 7468 6f64  ETA) This method
-00003170: 2069 7320 6e6f 7420 6669 6e69 7368 6564   is not finished
-00003180: 2e20 506f 7373 6962 6c65 2074 7970 6573  . Possible types
-00003190: 2027 6576 656e 7473 272c 2027 6d61 7463   'events', 'matc
-000031a0: 6865 7327 2c20 2774 6561 6d73 272c 2061  hes', 'teams', a
-000031b0: 6c73 6f20 7520 6361 6e20 6164 6420 6964  lso u can add id
-000031c0: 207c 2074 6974 6c65 207c 2074 6561 6d31   | title | team1
-000031d0: 207c 2074 6561 6d32 2c20 746f 2070 6172   | team2, to par
-000031e0: 7365 206d 6f72 652e 0a20 200a 2020 6060  se more..  .  ``
-000031f0: 600a 2020 0a20 2061 7761 6974 2068 6c74  `.  .  await hlt
-00003200: 762e 6765 7428 276d 6174 6368 6573 272c  v.get('matches',
-00003210: 2032 3337 3132 3031 2c20 2772 6573 2d72   2371201, 'res-r
-00003220: 6567 696f 6e61 6c2d 7365 7269 6573 2d33  egional-series-3
-00003230: 2d6c 6174 616d 272c 2027 494d 5045 5249  -latam', 'IMPERI
-00003240: 414c 272c 2027 4d49 4252 2729 0a20 200a  AL', 'MIBR').  .
-00003250: 2020 3e3e 3e20 2832 3337 3132 3031 2c20    >>> (2371201, 
-00003260: 302c 2030 2c20 274c 4956 4527 2c20 5b7b  0, 0, 'LIVE', [{
-00003270: 276d 6170 6e61 6d65 273a 2027 5665 7274  'mapname': 'Vert
-00003280: 6967 6f27 2c20 2772 5f74 6561 6d31 273a  igo', 'r_team1':
-00003290: 2027 3627 2c20 2772 5f74 6561 6d32 273a   '6', 'r_team2':
-000032a0: 2027 3133 277d 2c20 7b27 6d61 706e 616d   '13'}, {'mapnam
-000032b0: 6527 3a20 274d 6972 6167 6527 2c20 2772  e': 'Mirage', 'r
-000032c0: 5f74 6561 6d31 273a 2027 2d27 2c20 2772  _team1': '-', 'r
-000032d0: 5f74 6561 6d32 273a 2027 2d27 7d2c 207b  _team2': '-'}, {
-000032e0: 276d 6170 6e61 6d65 273a 2027 416e 7562  'mapname': 'Anub
-000032f0: 6973 272c 2027 725f 7465 616d 3127 3a20  is', 'r_team1': 
-00003300: 272d 272c 2027 725f 7465 616d 3227 3a20  '-', 'r_team2': 
-00003310: 272d 277d 5d2c 205b 5d29 0a20 200a 2020  '-'}], []).  .  
-00003320: 6060 600a 0a0a 2d2d 2d0a 2320 4578 616d  ```...---.# Exam
-00003330: 706c 6573 0a0a 2a2a 2a2a 5369 6d70 6c65  ples..****Simple
-00003340: 2045 7861 6d70 6c65 2a2a 2a2a 0a0a 6060   Example****..``
-00003350: 600a 6672 6f6d 2068 6c74 765f 6173 796e  `.from hltv_asyn
-00003360: 635f 6170 6920 696d 706f 7274 2048 6c74  c_api import Hlt
-00003370: 760a 0a0a 6173 796e 6320 6465 6620 7465  v...async def te
-00003380: 7374 2829 3a0a 0a20 2020 2061 7379 6e63  st():..    async
-00003390: 2077 6974 6820 486c 7476 2829 2061 7320   with Hltv() as 
-000033a0: 686c 7476 3a0a 2020 2020 2020 7072 696e  hltv:.      prin
-000033b0: 7428 6177 6169 7420 686c 7476 2e67 6574  t(await hltv.get
-000033c0: 5f65 7665 6e74 5f69 6e66 6f28 3731 3438  _event_info(7148
-000033d0: 2c20 2770 676c 2d63 7332 2d6d 616a 6f72  , 'pgl-cs2-major
-000033e0: 2d63 6f70 656e 6861 6765 6e2d 3230 3234  -copenhagen-2024
-000033f0: 2729 290a 0a69 6620 5f5f 6e61 6d65 5f5f  '))..if __name__
-00003400: 203d 3d20 225f 5f6d 6169 6e5f 5f22 3a0a   == "__main__":.
-00003410: 2020 2020 6173 796e 6369 6f2e 7275 6e28      asyncio.run(
-00003420: 7465 7374 2829 290a 6060 600a 0a2a 2a2a  test()).```..***
-00003430: 2a50 726f 7879 2050 6172 7365 722a 2a2a  *Proxy Parser***
-00003440: 2a0a 0a60 6060 0a66 726f 6d20 686c 7476  *..```.from hltv
-00003450: 5f61 7379 6e63 5f61 7069 2069 6d70 6f72  _async_api impor
-00003460: 7420 486c 7476 0a0a 0a61 7379 6e63 2064  t Hltv...async d
-00003470: 6566 2074 6573 7428 293a 0a0a 2020 2020  ef test():..    
-00003480: 686c 7476 203d 2048 6c74 7628 6465 6275  hltv = Hltv(debu
-00003490: 673d 5472 7565 2c20 7072 6f78 795f 7061  g=True, proxy_pa
-000034a0: 7468 3d27 7072 6f78 795f 7465 7374 2e74  th='proxy_test.t
-000034b0: 7874 272c 2074 696d 656f 7574 3d31 2c20  xt', timeout=1, 
-000034c0: 7265 6d6f 7665 5f70 726f 7879 3d54 7275  remove_proxy=Tru
-000034d0: 652c 2070 726f 7879 5f70 726f 746f 636f  e, proxy_protoco
-000034e0: 6c3d 2768 7474 7027 290a 2020 2020 0a20  l='http').    . 
-000034f0: 2020 2070 7269 6e74 2861 7761 6974 2068     print(await h
-00003500: 6c74 762e 6765 745f 6576 656e 745f 696e  ltv.get_event_in
-00003510: 666f 2837 3134 382c 2027 7067 6c2d 6373  fo(7148, 'pgl-cs
-00003520: 322d 6d61 6a6f 722d 636f 7065 6e68 6167  2-major-copenhag
-00003530: 656e 2d32 3032 3427 2929 0a0a 6966 205f  en-2024'))..if _
-00003540: 5f6e 616d 655f 5f20 3d3d 2022 5f5f 6d61  _name__ == "__ma
-00003550: 696e 5f5f 223a 0a20 2020 2061 7379 6e63  in__":.    async
-00003560: 696f 2e72 756e 2874 6573 7428 2929 0a60  io.run(test()).`
-00003570: 6060 0a0a 2a2a 2a2a 4175 746f 6d61 7469  ``..****Automati
-00003580: 6320 7061 7273 6572 2077 6974 6820 6172  c parser with ar
-00003590: 7120 616e 6420 7265 6469 732a 2a2a 2a0a  q and redis****.
-000035a0: 0a2d 2074 6f20 7275 6e20 7479 7065 2022  .- to run type "
-000035b0: 6172 7120 5041 5448 5f54 4f5f 4649 4c45  arq PATH_TO_FILE
-000035c0: 2e57 6f72 6b65 7253 6574 7469 6e67 7322  .WorkerSettings"
-000035d0: 0a0a 2020 2020 6060 600a 2020 2020 696d  ..    ```.    im
-000035e0: 706f 7274 2075 6a73 6f6e 0a20 2020 2069  port ujson.    i
-000035f0: 6d70 6f72 7420 6173 796e 6369 6f0a 2020  mport asyncio.  
-00003600: 2020 6672 6f6d 2061 7271 2069 6d70 6f72    from arq impor
-00003610: 7420 6372 6f6e 0a20 2020 2066 726f 6d20  t cron.    from 
-00003620: 7265 6469 732e 6173 796e 6369 6f20 696d  redis.asyncio im
-00003630: 706f 7274 2052 6564 6973 2c20 436f 6e6e  port Redis, Conn
-00003640: 6563 7469 6f6e 506f 6f6c 0a20 2020 200a  ectionPool.    .
-00003650: 2020 2020 6672 6f6d 2068 6c74 765f 6173      from hltv_as
-00003660: 796e 635f 6170 6920 696d 706f 7274 2048  ync_api import H
-00003670: 6c74 760a 2020 2020 0a20 2020 200a 2020  ltv.    .    .  
-00003680: 2020 0a20 2020 2061 7379 6e63 2064 6566    .    async def
-00003690: 2073 7461 7274 7570 2863 7478 293a 0a20   startup(ctx):. 
-000036a0: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
-000036b0: 6820 486c 7476 286d 6178 5f64 656c 6179  h Hltv(max_delay
-000036c0: 3d35 2c20 7072 6f78 795f 7061 7468 3d27  =5, proxy_path='
-000036d0: 7072 6f78 6965 732e 7478 7427 2c20 6465  proxies.txt', de
-000036e0: 6275 673d 5472 7565 2920 6173 2068 6c74  bug=True) as hlt
-000036f0: 763a 0a20 2020 2020 2020 2020 2020 2020  v:.             
-00003700: 2063 7478 5b22 686c 7476 225d 203d 2068   ctx["hltv"] = h
-00003710: 6c74 760a 2020 0a20 2020 2020 2020 2063  ltv.  .        c
-00003720: 7478 5b22 7265 6469 7322 5d20 3d20 7265  tx["redis"] = re
-00003730: 6469 735f 636c 6965 6e74 203d 2052 6564  dis_client = Red
-00003740: 6973 280a 2020 2020 2020 2020 2020 2020  is(.            
-00003750: 636f 6e6e 6563 7469 6f6e 5f70 6f6f 6c3d  connection_pool=
-00003760: 436f 6e6e 6563 7469 6f6e 506f 6f6c 2e66  ConnectionPool.f
-00003770: 726f 6d5f 7572 6c28 7365 7474 696e 6773  rom_url(settings
-00003780: 2e72 6564 6973 5f75 726c 2929 0a20 2020  .redis_url)).   
-00003790: 2020 2020 206c 6f67 6765 722e 7375 6363       logger.succ
-000037a0: 6573 7328 6622 5363 6865 6475 6c65 7220  ess(f"Scheduler 
-000037b0: 7374 6172 7465 642e 2055 5443 2074 696d  started. UTC tim
-000037c0: 6520 7b64 6174 6574 696d 652e 7574 636e  e {datetime.utcn
-000037d0: 6f77 2829 7d22 290a 2020 2020 0a20 2020  ow()}").    .   
-000037e0: 200a 2020 2020 6173 796e 6320 6465 6620   .    async def 
-000037f0: 7368 7574 646f 776e 2863 7478 293a 0a20  shutdown(ctx):. 
-00003800: 2020 2020 2020 2061 7761 6974 2063 7478         await ctx
-00003810: 5b22 7265 6469 7322 5d2e 636c 6f73 6528  ["redis"].close(
-00003820: 290a 2020 2020 0a20 2020 200a 2020 2020  ).    .    .    
-00003830: 6173 796e 6320 6465 6620 7061 7273 655f  async def parse_
-00003840: 6d61 7463 6865 7328 6374 7829 3a0a 2020  matches(ctx):.  
-00003850: 2020 2020 2020 686c 7476 203d 2063 7478        hltv = ctx
-00003860: 5b22 686c 7476 225d 0a20 2020 2020 2020  ["hltv"].       
-00003870: 2072 6564 6973 203d 2063 7478 5b22 7265   redis = ctx["re
-00003880: 6469 7322 5d0a 2020 2020 2020 2020 6d61  dis"].        ma
-00003890: 7463 6865 7320 3d20 6177 6169 7420 686c  tches = await hl
-000038a0: 7476 2e67 6574 5f75 7063 6f6d 696e 675f  tv.get_upcoming_
-000038b0: 6d61 7463 6865 7328 312c 2031 290a 2020  matches(1, 1).  
-000038c0: 2020 2020 2020 6966 206d 6174 6368 6573        if matches
-000038d0: 3a0a 2020 2020 2020 2020 2020 2020 6177  :.            aw
-000038e0: 6169 7420 7265 6469 732e 7365 7428 226d  ait redis.set("m
-000038f0: 6174 6368 6573 222c 2075 6a73 6f6e 2e64  atches", ujson.d
-00003900: 756d 7073 286d 6174 6368 6573 2929 0a20  umps(matches)). 
-00003910: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00003920: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00003930: 6572 726f 7228 2265 7272 6f72 2070 6172  error("error par
-00003940: 7369 6e67 206d 6174 6368 6573 2229 0a20  sing matches"). 
-00003950: 2020 200a 2020 2020 6173 796e 6320 6465     .    async de
-00003960: 6620 7061 7273 655f 6576 656e 7473 2863  f parse_events(c
-00003970: 7478 293a 0a20 2020 2020 2020 2068 6c74  tx):.        hlt
-00003980: 7620 3d20 6374 785b 2268 6c74 7622 5d0a  v = ctx["hltv"].
-00003990: 2020 2020 2020 2020 7265 6469 7320 3d20          redis = 
-000039a0: 6374 785b 2272 6564 6973 225d 0a20 2020  ctx["redis"].   
-000039b0: 2020 2020 2065 7665 6e74 7320 3d20 6177       events = aw
-000039c0: 6169 7420 686c 7476 2e67 6574 5f65 7665  ait hltv.get_eve
-000039d0: 6e74 7328 290a 2020 2020 2020 2020 6966  nts().        if
-000039e0: 2065 7665 6e74 733a 0a20 2020 2020 2020   events:.       
-000039f0: 2020 2020 2061 7761 6974 2072 6564 6973       await redis
-00003a00: 2e73 6574 2822 6576 656e 7473 222c 2075  .set("events", u
-00003a10: 6a73 6f6e 2e64 756d 7073 2865 7665 6e74  json.dumps(event
-00003a20: 7329 290a 2020 2020 2020 2020 656c 7365  s)).        else
-00003a30: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-00003a40: 6767 6572 2e65 7272 6f72 2822 6572 726f  gger.error("erro
-00003a50: 7220 7061 7273 696e 6720 6576 656e 7473  r parsing events
-00003a60: 2229 0a20 2020 200a 2020 2020 0a20 2020  ").    .    .   
-00003a70: 2061 7379 6e63 2064 6566 2070 6172 7365   async def parse
-00003a80: 5f74 6f70 5f74 6561 6d73 2863 7478 293a  _top_teams(ctx):
-00003a90: 0a20 2020 2020 2020 2068 6c74 7620 3d20  .        hltv = 
-00003aa0: 6374 785b 2268 6c74 7622 5d0a 2020 2020  ctx["hltv"].    
-00003ab0: 2020 2020 7265 6469 7320 3d20 6374 785b      redis = ctx[
-00003ac0: 2272 6564 6973 225d 0a20 2020 2020 2020  "redis"].       
-00003ad0: 2074 6f70 5f74 6561 6d73 203d 2061 7761   top_teams = awa
-00003ae0: 6974 2068 6c74 762e 6765 745f 746f 705f  it hltv.get_top_
-00003af0: 7465 616d 7328 3330 290a 2020 2020 2020  teams(30).      
-00003b00: 2020 6966 2074 6f70 5f74 6561 6d73 3a0a    if top_teams:.
-00003b10: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00003b20: 7420 7265 6469 732e 7365 7428 2274 6f70  t redis.set("top
-00003b30: 5f74 6561 6d73 222c 2075 6a73 6f6e 2e64  _teams", ujson.d
-00003b40: 756d 7073 2874 6f70 5f74 6561 6d73 2929  umps(top_teams))
-00003b50: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00003b60: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00003b70: 722e 6572 726f 7228 2265 7272 6f72 2070  r.error("error p
-00003b80: 6172 7369 6e67 2074 6f70 2074 6561 6d73  arsing top teams
-00003b90: 2229 0a20 2020 200a 2020 2020 0a20 2020  ").    .    .   
-00003ba0: 2061 7379 6e63 2064 6566 2070 6172 7365   async def parse
-00003bb0: 5f74 6f70 5f70 6c61 7965 7273 2863 7478  _top_players(ctx
-00003bc0: 293a 0a20 2020 2020 2020 2068 6c74 7620  ):.        hltv 
-00003bd0: 3d20 6374 785b 2268 6c74 7622 5d0a 2020  = ctx["hltv"].  
-00003be0: 2020 2020 2020 7265 6469 7320 3d20 6374        redis = ct
-00003bf0: 785b 2272 6564 6973 225d 0a20 2020 2020  x["redis"].     
-00003c00: 2020 2074 6f70 5f70 6c61 7965 7273 203d     top_players =
-00003c10: 2061 7761 6974 2068 6c74 762e 6765 745f   await hltv.get_
-00003c20: 6265 7374 5f70 6c61 7965 7273 2833 3029  best_players(30)
-00003c30: 0a20 2020 2020 2020 2069 6620 746f 705f  .        if top_
-00003c40: 706c 6179 6572 733a 0a20 2020 2020 2020  players:.       
-00003c50: 2020 2020 2061 7761 6974 2072 6564 6973       await redis
-00003c60: 2e73 6574 2822 746f 705f 7465 616d 7322  .set("top_teams"
-00003c70: 2c20 756a 736f 6e2e 6475 6d70 7328 746f  , ujson.dumps(to
-00003c80: 705f 706c 6179 6572 7329 290a 2020 2020  p_players)).    
-00003c90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00003ca0: 2020 2020 2020 6c6f 6767 6572 2e65 7272        logger.err
-00003cb0: 6f72 2822 6572 726f 7220 7061 7273 696e  or("error parsin
-00003cc0: 6720 746f 7020 706c 6179 6572 7322 290a  g top players").
-00003cd0: 2020 2020 0a20 2020 200a 2020 2020 6173      .    .    as
-00003ce0: 796e 6320 6465 6620 7061 7273 655f 6c61  ync def parse_la
-00003cf0: 7374 5f6e 6577 7328 6374 7829 3a0a 2020  st_news(ctx):.  
-00003d00: 2020 2020 2020 686c 7476 203d 2063 7478        hltv = ctx
-00003d10: 5b22 686c 7476 225d 0a20 2020 2020 2020  ["hltv"].       
-00003d20: 2072 6564 6973 203d 2063 7478 5b22 7265   redis = ctx["re
-00003d30: 6469 7322 5d0a 2020 2020 2020 2020 6e65  dis"].        ne
-00003d40: 7773 203d 2061 7761 6974 2068 6c74 762e  ws = await hltv.
-00003d50: 6765 745f 6c61 7374 5f6e 6577 7328 6f6e  get_last_news(on
-00003d60: 6c79 5f74 6f64 6179 3d54 7275 652c 206d  ly_today=True, m
-00003d70: 6178 5f72 6567 5f6e 6577 733d 3429 0a20  ax_reg_news=4). 
-00003d80: 2020 2020 2020 2069 6620 6e65 7773 3a0a         if news:.
-00003d90: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00003da0: 7420 7265 6469 732e 7365 7428 226e 6577  t redis.set("new
-00003db0: 7322 2c20 756a 736f 6e2e 6475 6d70 7328  s", ujson.dumps(
-00003dc0: 6e65 7773 2929 0a20 2020 2020 2020 2065  news)).        e
-00003dd0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00003de0: 206c 6f67 6765 722e 6572 726f 7228 2265   logger.error("e
-00003df0: 7272 6f72 2070 6172 7369 6e67 206e 6577  rror parsing new
-00003e00: 7322 290a 2020 2020 0a20 2020 200a 2020  s").    .    .  
-00003e10: 2020 636c 6173 7320 576f 726b 6572 5365    class WorkerSe
-00003e20: 7474 696e 6773 3a0a 2020 2020 2020 2020  ttings:.        
-00003e30: 7265 6469 735f 7365 7474 696e 6773 203d  redis_settings =
-00003e40: 2073 6574 7469 6e67 732e 7265 6469 735f   settings.redis_
-00003e50: 706f 6f6c 0a20 2020 2020 2020 206f 6e5f  pool.        on_
-00003e60: 7374 6172 7475 7020 3d20 7374 6172 7475  startup = startu
-00003e70: 700a 2020 2020 2020 2020 6f6e 5f73 6875  p.        on_shu
-00003e80: 7464 6f77 6e20 3d20 7368 7574 646f 776e  tdown = shutdown
-00003e90: 0a20 2020 2020 2020 2066 756e 6374 696f  .        functio
-00003ea0: 6e73 203d 205b 7061 7273 655f 6d61 7463  ns = [parse_matc
-00003eb0: 6865 732c 0a20 2020 2020 2020 2020 2020  hes,.           
-00003ec0: 2020 2020 2020 2020 2020 7061 7273 655f            parse_
-00003ed0: 6576 656e 7473 2c0a 2020 2020 2020 2020  events,.        
-00003ee0: 2020 2020 2020 2020 2020 2020 2070 6172               par
-00003ef0: 7365 5f74 6f70 5f74 6561 6d73 2c0a 2020  se_top_teams,.  
-00003f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f10: 2020 2070 6172 7365 5f74 6f70 5f70 6c61     parse_top_pla
-00003f20: 7965 7273 2c0a 2020 2020 2020 2020 2020  yers,.          
-00003f30: 2020 2020 2020 2020 2020 2070 6172 7365             parse
-00003f40: 5f6c 6173 745f 6e65 7773 2c0a 2020 2020  _last_news,.    
-00003f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f60: 205d 0a20 2020 2020 2020 2063 726f 6e5f   ].        cron_
-00003f70: 6a6f 6273 203d 205b 0a20 2020 2020 2020  jobs = [.       
-00003f80: 2020 2020 2063 726f 6e28 7061 7273 655f       cron(parse_
-00003f90: 6d61 7463 6865 732c 206d 696e 7574 653d  matches, minute=
-00003fa0: 3539 292c 0a20 2020 2020 2020 2020 2020  59),.           
-00003fb0: 2063 726f 6e28 7061 7273 655f 6576 656e   cron(parse_even
-00003fc0: 7473 2c20 686f 7572 3d30 2c20 6d69 6e75  ts, hour=0, minu
-00003fd0: 7465 3d30 2c20 7365 636f 6e64 3d30 292c  te=0, second=0),
-00003fe0: 0a20 2020 2020 2020 2020 2020 2063 726f  .            cro
-00003ff0: 6e28 7061 7273 655f 746f 705f 7465 616d  n(parse_top_team
-00004000: 732c 2064 6179 3d30 2c20 686f 7572 3d31  s, day=0, hour=1
-00004010: 382c 206d 696e 7574 653d 312c 2073 6563  8, minute=1, sec
-00004020: 6f6e 643d 3330 292c 0a20 2020 2020 2020  ond=30),.       
-00004030: 2020 2020 2063 726f 6e28 7061 7273 655f       cron(parse_
-00004040: 746f 705f 706c 6179 6572 732c 2064 6179  top_players, day
-00004050: 3d30 2c20 686f 7572 3d32 302c 206d 696e  =0, hour=20, min
-00004060: 7574 653d 302c 2073 6563 6f6e 643d 3029  ute=0, second=0)
-00004070: 2c0a 2020 2020 2020 2020 2020 2020 6372  ,.            cr
-00004080: 6f6e 2870 6172 7365 5f6c 6173 745f 6e65  on(parse_last_ne
-00004090: 7773 2c20 6d69 6e75 7465 3d35 3529 2c0a  ws, minute=55),.
-000040a0: 2020 2020 2020 2020 5d0a 0a20 2020 2060          ]..    `
-000040b0: 6060 0a0a 2320 5465 7374 733a 0a0a 2a2a  ``..# Tests:..**
-000040c0: 3c61 2068 7265 663d 2768 7474 7073 3a2f  <a href='https:/
-000040d0: 2f67 6974 6875 622e 636f 6d2f 616b 696d  /github.com/akim
-000040e0: 6572 736c 7973 2f68 6c74 762d 6173 796e  erslys/hltv-asyn
-000040f0: 632d 6170 692f 626c 6f62 2f6d 6169 6e2f  c-api/blob/main/
-00004100: 7465 7374 2f68 6172 645f 7465 7374 2e70  test/hard_test.p
-00004110: 7927 3e54 6f20 7465 7374 206c 6962 7261  y'>To test libra
-00004120: 7279 2079 6f75 2063 616e 2075 7365 2074  ry you can use t
-00004130: 656d 706f 7261 7269 6c79 2074 6573 7420  emporarily test 
-00004140: 6669 6c65 3c2f 613e 2a2a 0a0a 6060 600a  file</a>**..```.
-00004150: 0a50 6172 7365 6420 3230 3820 6d61 7463  .Parsed 208 matc
-00004160: 6865 732e 2839 3773 2920 4552 524f 5253  hes.(97s) ERRORS
-00004170: 3a20 302f 3230 380a 5061 7273 6564 2032  : 0/208.Parsed 2
-00004180: 3520 6576 656e 7473 2e28 3233 7329 2045  5 events.(23s) E
-00004190: 5252 4f52 533a 2030 2f32 350a 5061 7273  RRORS: 0/25.Pars
-000041a0: 6564 2033 3120 7465 616d 732e 2834 3173  ed 31 teams.(41s
-000041b0: 2920 4552 524f 5253 3a20 302f 3331 0a50  ) ERRORS: 0/31.P
-000041c0: 6172 7365 6420 3331 2070 6c61 7965 7273  arsed 31 players
-000041d0: 2e28 3238 7329 2045 5252 4f52 533a 2030  .(28s) ERRORS: 0
-000041e0: 2f33 310a 4552 524f 5253 3d30 0a53 5543  /31.ERRORS=0.SUC
-000041f0: 4345 5353 3d32 3834 0a54 6f74 616c 2070  CESS=284.Total p
-00004200: 6172 7365 643d 3238 340a 546f 7461 6c20  arsed=284.Total 
-00004210: 7469 6d65 2039 362e 3833 3638 0a0a 6060  time 96.8368..``
-00004220: 600a 0a23 2042 6574 6120 2f20 556e 7265  `..# Beta / Unre
-00004230: 6c65 6173 6564 0a0a 6672 6f6d 2068 6c74  leased..from hlt
-00004240: 765f 6173 796e 635f 6170 692e 756e 7265  v_async_api.unre
-00004250: 6c65 6173 6564 2069 6d70 6f72 7420 556e  leased import Un
-00004260: 7265 6c65 6173 6564 0a0a 2320 5265 7175  released..# Requ
-00004270: 6972 656d 656e 7473 3a0a 0a50 7974 686f  irements:..Pytho
-00004280: 6e20 332e 392b 0a0a 4c69 6365 6e73 653a  n 3.9+..License:
-00004290: 0a48 4c54 5620 4173 796e 6320 6973 206c  .HLTV Async is l
-000042a0: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
-000042b0: 6520 4d49 5420 4c69 6365 6e73 652c 2061  e MIT License, a
-000042c0: 6c6c 6f77 696e 6720 666f 7220 7065 7273  llowing for pers
-000042d0: 6f6e 616c 2061 6e64 2063 6f6d 6d65 7263  onal and commerc
-000042e0: 6961 6c20 7573 6520 7769 7468 206d 696e  ial use with min
-000042f0: 696d 616c 2072 6573 7472 6963 7469 6f6e  imal restriction
-00004300: 732e 0a0a                                s...
+00000450: 6e73 2e20 436f 7665 7261 6765 2e28 3f29  ns. Coverage.(?)
+00000460: 2052 6f74 6174 696e 6720 7573 6572 2061   Rotating user a
+00000470: 6765 6e74 2028 6578 702e 2074 696c 6c20  gent (exp. till 
+00000480: 3230 2e30 3529 0a2a 202a 2a30 2e39 2e30  20.05).* **0.9.0
+00000490: 2a2a 2073 7461 7473 2026 2069 6d61 6765  ** stats & image
+000004a0: 7320 7570 6461 7465 2c20 6d6f 7265 2073  s update, more s
+000004b0: 7461 7473 2073 6372 6170 6572 732c 2074  tats scrapers, t
+000004c0: 6561 6d20 6c6f 676f 732c 2070 6c61 7965  eam logos, playe
+000004d0: 7220 7068 6f74 6f73 2c20 696d 6167 6573  r photos, images
+000004e0: 2c20 6d6f 7265 2064 6174 612c 2074 6561  , more data, tea
+000004f0: 6d5f 6d61 7020 7374 6174 732c 206d 6170  m_map stats, map
+00000500: 2073 7461 7473 2c20 6d6f 7265 2066 756e   stats, more fun
+00000510: 6374 696f 6e73 2073 7563 6820 6173 2067  ctions such as g
+00000520: 6574 5f6e 6577 735f 6964 2c20 6765 745f  et_news_id, get_
+00000530: 7465 616d 5f6c 6f67 6f2c 2067 6574 5f70  team_logo, get_p
+00000540: 6c61 7965 725f 7068 6f74 6f2c 2067 6574  layer_photo, get
+00000550: 5f64 656d 6f5f 6964 2c20 6765 745f 6d61  _demo_id, get_ma
+00000560: 7463 685f 7374 6174 732e 2e2e 0a2a 202a  tch_stats....* *
+00000570: 2a30 2e31 302e 302a 2a20 7379 6e63 6872  *0.10.0** synchr
+00000580: 6f6e 6f75 7320 7570 6461 7465 2c20 7265  onous update, re
+00000590: 666f 726d 6174 7469 6e67 2074 6865 206c  formatting the l
+000005a0: 6962 7261 7279 2061 7320 6120 7379 6e63  ibrary as a sync
+000005b0: 6872 6f6e 6f75 732c 206d 6f76 6520 6173  hronous, move as
+000005c0: 796e 6320 7061 7273 6572 2061 7320 616e  ync parser as an
+000005d0: 2065 7874 656e 7369 6f6e 2e20 284a 554c   extension. (JUL
+000005e0: 592d 4155 4755 5354 2032 3032 3429 0a2a  Y-AUGUST 2024).*
+000005f0: 202a 2a30 2e31 312e 3020 2d20 312e 302e   **0.11.0 - 1.0.
+00000600: 302a 2a20 5072 6f76 6964 6520 746f 2075  0** Provide to u
+00000610: 7365 2048 6c74 762d 6173 796e 632d 6170  se Hltv-async-ap
+00000620: 6920 6f6e 2061 6e79 2073 7973 7465 6d2c  i on any system,
+00000630: 206c 616e 6775 6167 652c 2062 7920 6372   language, by cr
+00000640: 6561 7469 6e67 2061 2052 4553 5466 756c  eating a RESTful
+00000650: 2073 6572 7669 6365 2e0a 0a0a 2320 4665   service....# Fe
+00000660: 6174 7572 6573 0a0a 0a2a 202a 2a53 696d  atures...* **Sim
+00000670: 706c 6520 5573 6167 652a 2a20 2869 7473  ple Usage** (its
+00000680: 2072 6561 6c6c 7920 7369 6d70 6c65 290a   really simple).
+00000690: 0a0a 2a20 2a2a 4e65 7720 616e 6420 6d6f  ..* **New and mo
+000006a0: 6465 726e 2066 756c 6c79 2061 7379 6e63  dern fully async
+000006b0: 206c 6962 7261 7279 2a2a 0a0a 0a2a 202a   library**...* *
+000006c0: 2a48 7567 6520 616d 6f75 6e74 206f 6620  *Huge amount of 
+000006d0: 6f70 7469 6f6e 732a 2a0a 0a0a 2a20 2a2a  options**...* **
+000006e0: 5375 7070 6f72 7473 2070 726f 7879 2075  Supports proxy u
+000006f0: 7361 6765 2a2a 0a0a 0a2a 202a 2a4d 6164  sage**...* **Mad
+00000700: 6520 7769 7468 206c 6f76 6520 3c33 2a2a  e with love <3**
+00000710: 0a0a 0a2d 2d2d 0a0a 2320 496e 7374 616c  ...---..# Instal
+00000720: 6c61 7469 6f6e 0a0a 6060 600a 7069 7020  lation..```.pip 
+00000730: 696e 7374 616c 6c20 686c 7476 2d61 7379  install hltv-asy
+00000740: 6e63 2d61 7069 0a60 6060 0a0a 2d2d 2d0a  nc-api.```..---.
+00000750: 0a0a 2320 5369 6d70 6c65 2055 7361 6765  ..# Simple Usage
+00000760: 0a0a 2020 6060 600a 0a20 2020 2066 726f  ..  ```..    fro
+00000770: 6d20 686c 7476 5f61 7379 6e63 5f61 7069  m hltv_async_api
+00000780: 2069 6d70 6f72 7420 486c 7476 0a20 2020   import Hltv.   
+00000790: 200a 2020 2020 6173 796e 6320 7769 7468   .    async with
+000007a0: 2048 6c74 7628 2920 6173 2068 6c74 763a   Hltv() as hltv:
+000007b0: 0a20 2020 2020 2070 7269 6e74 2861 7761  .      print(awa
+000007c0: 6974 2068 6c74 762e 6765 745f 6576 656e  it hltv.get_even
+000007d0: 745f 696e 666f 2837 3134 382c 2027 5047  t_info(7148, 'PG
+000007e0: 4c20 4353 3220 4d61 6a6f 7220 436f 7065  L CS2 Major Cope
+000007f0: 6e68 6167 656e 3230 3234 2729 290a 0a20  nhagen2024')).. 
+00000800: 2060 6060 0a0a 2020 2a2a 4f52 2a2a 0a0a   ```..  **OR**..
+00000810: 2020 6060 600a 0a20 2020 2066 726f 6d20    ```..    from 
+00000820: 686c 7476 5f61 7379 6e63 5f61 7069 2069  hltv_async_api i
+00000830: 6d70 6f72 7420 486c 7476 0a20 2020 200a  mport Hltv.    .
+00000840: 2020 2020 686c 7476 203d 2048 6c74 7628      hltv = Hltv(
+00000850: 290a 2020 2020 7072 696e 7428 6177 6169  ).    print(awai
+00000860: 7420 686c 7476 2e67 6574 5f65 7665 6e74  t hltv.get_event
+00000870: 5f69 6e66 6f28 3731 3438 2c20 2750 474c  _info(7148, 'PGL
+00000880: 2043 5332 204d 616a 6f72 2043 6f70 656e   CS2 Major Copen
+00000890: 6861 6765 6e32 3032 3427 2929 0a20 2020  hagen2024')).   
+000008a0: 2061 7761 6974 2068 6c74 762e 636c 6f73   await hltv.clos
+000008b0: 6528 290a 0a20 2060 6060 0a0a 0a2d 2d2d  e()..  ```...---
+000008c0: 0a0a 2320 436f 6e66 6967 730a 0a2a 206d  ..# Configs..* m
+000008d0: 6178 5f64 656c 6179 3a20 666c 6f61 7420  ax_delay: float 
+000008e0: 3d20 3130 2e30 0a0a 2020 4175 746f 6d61  = 10.0..  Automa
+000008f0: 7469 6361 6c6c 7920 696e 6372 6561 7369  tically increasi
+00000900: 6e67 2064 656c 6179 2062 7920 3120 7365  ng delay by 1 se
+00000910: 6320 746f 2031 3073 0a0a 2020 6060 600a  c to 10s..  ```.
+00000920: 2020 2020 686c 7476 203d 2048 6c74 7628      hltv = Hltv(
+00000930: 6d61 785f 6465 6c61 793d 3529 0a20 2020  max_delay=5).   
+00000940: 200a 2020 2020 3e3e 3e46 6574 6368 696e   .    >>>Fetchin
+00000950: 6720 6874 7470 733a 2f2f 7777 772e 686c  g https://www.hl
+00000960: 7476 2e6f 7267 2f6d 6174 6368 6573 2f32  tv.org/matches/2
+00000970: 3337 3037 3237 2f66 617a 652d 7673 2d6e  370727/faze-vs-n
+00000980: 6174 7573 2d76 696e 6365 7265 2d70 676c  atus-vincere-pgl
+00000990: 2d63 7332 2d6d 616a 6f72 2d63 6f70 656e  -cs2-major-copen
+000009a0: 6861 6765 6e2d 3230 3234 2c20 636f 6465  hagen-2024, code
+000009b0: 3a20 3430 330a 2020 2020 3e3e 3e47 6f74  : 403.    >>>Got
+000009c0: 2034 3033 2066 6f72 6269 7474 656e 0a20   403 forbitten. 
+000009d0: 2020 203e 3e3e 4361 6c6c 696e 6720 6167     >>>Calling ag
+000009e0: 6169 6e2c 2069 6e63 7265 6173 696e 6720  ain, increasing 
+000009f0: 6465 6c61 7920 746f 2034 730a 2020 2020  delay to 4s.    
+00000a00: 3e3e 3e46 6574 6368 696e 6720 6874 7470  >>>Fetching http
+00000a10: 733a 2f2f 7777 772e 686c 7476 2e6f 7267  s://www.hltv.org
+00000a20: 2f6d 6174 6368 6573 2f32 3337 3037 3237  /matches/2370727
+00000a30: 2f66 617a 652d 7673 2d6e 6174 7573 2d76  /faze-vs-natus-v
+00000a40: 696e 6365 7265 2d70 676c 2d63 7332 2d6d  incere-pgl-cs2-m
+00000a50: 616a 6f72 2d63 6f70 656e 6861 6765 6e2d  ajor-copenhagen-
+00000a60: 3230 3234 2c20 636f 6465 3a20 3430 330a  2024, code: 403.
+00000a70: 2020 2020 3e3e 3e47 6f74 2034 3033 2066      >>>Got 403 f
+00000a80: 6f72 6269 7474 656e 0a20 2020 203e 3e3e  orbitten.    >>>
+00000a90: 4361 6c6c 696e 6720 6167 6169 6e2c 2069  Calling again, i
+00000aa0: 6e63 7265 6173 696e 6720 6465 6c61 7920  ncreasing delay 
+00000ab0: 746f 2035 730a 2020 6060 600a 0a2a 206d  to 5s.  ```..* m
+00000ac0: 696e 5f64 656c 6179 3a20 666c 6f61 7420  in_delay: float 
+00000ad0: 3d20 2d31 0a0a 6060 6020 0a20 205b 4445  = -1..``` .  [DE
+00000ae0: 4255 475d 2052 616e 646f 6d20 6465 6c61  BUG] Random dela
+00000af0: 7920 392e 3535 7320 0a20 205b 4445 4255  y 9.55s .  [DEBU
+00000b00: 475d 2054 7279 696e 6720 636f 6e6e 6563  G] Trying connec
+00000b10: 7420 746f 2068 7474 7073 3a2f 2f77 7777  t to https://www
+00000b20: 2e68 6c74 762e 6f72 672f 6d61 7463 6865  .hltv.org/matche
+00000b30: 732c 2074 7279 2033 2f31 300a 2020 5b44  s, try 3/10.  [D
+00000b40: 4542 5547 5d20 5261 6e64 6f6d 2064 656c  EBUG] Random del
+00000b50: 6179 2033 2e39 7320 0a20 205b 4445 4255  ay 3.9s .  [DEBU
+00000b60: 475d 2054 7279 696e 6720 636f 6e6e 6563  G] Trying connec
+00000b70: 7420 746f 2068 7474 7073 3a2f 2f77 7777  t to https://www
+00000b80: 2e68 6c74 762e 6f72 672f 6d61 7463 6865  .hltv.org/matche
+00000b90: 732c 2074 7279 2034 2f31 300a 6060 600a  s, try 4/10.```.
+00000ba0: 0a0a 0a2a 2070 726f 7879 5f64 656c 6179  ...* proxy_delay
+00000bb0: 3a20 626f 6f6c 203d 2046 616c 7365 0a0a  : bool = False..
+00000bc0: 2020 2020 4465 6c61 7920 666f 7220 7072      Delay for pr
+00000bd0: 6f78 7920 7573 6573 2e0a 2a20 0a20 2060  oxy uses..* .  `
+00000be0: 6060 0a20 205b 494e 464f 5d20 4e65 7720  ``.  [INFO] New 
+00000bf0: 7072 6f78 793a 2068 7474 703a 2f2f 3132  proxy: http://12
+00000c00: 332e 3132 332e 3132 332e 3132 333a 3132  3.123.123.123:12
+00000c10: 3320 0a20 205b 4445 4255 475d 2052 616e  3 .  [DEBUG] Ran
+00000c20: 646f 6d20 6465 6c61 7920 392e 3535 7320  dom delay 9.55s 
+00000c30: 0a20 205b 4445 4255 475d 2054 7279 696e  .  [DEBUG] Tryin
+00000c40: 6720 636f 6e6e 6563 7420 746f 2068 7474  g connect to htt
+00000c50: 7073 3a2f 2f77 7777 2e68 6c74 762e 6f72  ps://www.hltv.or
+00000c60: 672f 6d61 7463 6865 732c 2074 7279 2033  g/matches, try 3
+00000c70: 2f31 300a 2020 5b44 4542 5547 5d20 5377  /10.  [DEBUG] Sw
+00000c80: 6974 6368 696e 6720 7072 6f78 7920 6874  itching proxy ht
+00000c90: 7470 3a2f 2f31 3233 2e31 3233 2e31 3233  tp://123.123.123
+00000ca0: 2e31 3233 3a31 3233 200a 2020 5b49 4e46  .123:123 .  [INF
+00000cb0: 4f5d 204e 6577 2070 726f 7879 3a20 6874  O] New proxy: ht
+00000cc0: 7470 3a2f 2f31 3131 2e31 3131 2e31 3131  tp://111.111.111
+00000cd0: 2e31 313a 3131 3120 0a20 205b 4445 4255  .11:111 .  [DEBU
+00000ce0: 475d 2052 616e 646f 6d20 6465 6c61 7920  G] Random delay 
+00000cf0: 332e 3973 200a 2020 5b44 4542 5547 5d20  3.9s .  [DEBUG] 
+00000d00: 5472 7969 6e67 2063 6f6e 6e65 6374 2074  Trying connect t
+00000d10: 6f20 6874 7470 733a 2f2f 7777 772e 686c  o https://www.hl
+00000d20: 7476 2e6f 7267 2f6d 6174 6368 6573 2c20  tv.org/matches, 
+00000d30: 7472 7920 342f 3130 0a20 2060 6060 0a0a  try 4/10.  ```..
+00000d40: 2a20 6d61 785f 7265 7472 6965 733a 2069  * max_retries: i
+00000d50: 6e74 203d 2031 300a 0a20 2020 2030 2066  nt = 10..    0 f
+00000d60: 6f72 2069 6e66 696e 6974 7920 7265 7472  or infinity retr
+00000d70: 6965 730a 2020 2020 0a20 2020 2060 6060  ies.    .    ```
+00000d80: 0a20 2020 2068 6c74 7620 3d20 486c 7476  .    hltv = Hltv
+00000d90: 286d 6178 5f72 6574 7269 6573 3d32 2c20  (max_retries=2, 
+00000da0: 6465 6275 673d 5472 7565 290a 2020 2020  debug=True).    
+00000db0: 7072 696e 7428 6177 6169 7420 686c 7476  print(await hltv
+00000dc0: 2e67 6574 5f62 6573 745f 706c 6179 6572  .get_best_player
+00000dd0: 7328 2929 0a20 2020 200a 2020 2020 3e3e  s()).    .    >>
+00000de0: 3e43 7265 6174 696e 6720 5365 7373 696f  >Creating Sessio
+00000df0: 6e0a 2020 2020 3e3e 3e54 7279 696e 6720  n.    >>>Trying 
+00000e00: 636f 6e6e 6563 7420 746f 2068 7474 7073  connect to https
+00000e10: 3a2f 2f77 7777 2e68 6c74 762e 6f72 672f  ://www.hltv.org/
+00000e20: 7374 6174 732f 706c 6179 6572 733f 7374  stats/players?st
+00000e30: 6172 7444 6174 653d 3230 3234 2d30 312d  artDate=2024-01-
+00000e40: 3031 2665 6e64 4461 7465 3d32 3032 342d  01&endDate=2024-
+00000e50: 3132 2d33 3126 7261 6e6b 696e 6746 696c  12-31&rankingFil
+00000e60: 7465 723d 546f 7032 302c 2074 7279 2031  ter=Top20, try 1
+00000e70: 2f32 0a20 2020 203e 3e3e 5472 7969 6e67  /2.    >>>Trying
+00000e80: 2063 6f6e 6e65 6374 2074 6f20 6874 7470   connect to http
+00000e90: 733a 2f2f 7777 772e 686c 7476 2e6f 7267  s://www.hltv.org
+00000ea0: 2f73 7461 7473 2f70 6c61 7965 7273 3f73  /stats/players?s
+00000eb0: 7461 7274 4461 7465 3d32 3032 342d 3031  tartDate=2024-01
+00000ec0: 2d30 3126 656e 6444 6174 653d 3230 3234  -01&endDate=2024
+00000ed0: 2d31 322d 3331 2672 616e 6b69 6e67 4669  -12-31&rankingFi
+00000ee0: 6c74 6572 3d54 6f70 3230 2c20 7472 7920  lter=Top20, try 
+00000ef0: 322f 320a 2020 2020 3e3e 3e43 6f6e 6e65  2/2.    >>>Conne
+00000f00: 6374 696f 6e20 6661 696c 6564 0a20 2020  ction failed.   
+00000f10: 2060 6060 0a0a 2a20 7072 6f78 795f 6c69   ```..* proxy_li
+00000f20: 7374 3a20 6c69 7374 207c 204e 6f6e 6520  st: list | None 
+00000f30: 3d20 4e6f 6e65 0a0a 2020 2020 6175 746f  = None..    auto
+00000f40: 6d61 7469 6320 726f 7461 7469 6e67 2070  matic rotating p
+00000f50: 726f 7869 6573 2c20 6966 2079 6f75 7220  roxies, if your 
+00000f60: 7072 6f78 6965 7320 646f 6573 6e74 2068  proxies doesnt h
+00000f70: 6176 6520 616e 7920 7072 6f74 6f63 6f6c  ave any protocol
+00000f80: 2079 6f75 2063 616e 2075 7365 2070 726f   you can use pro
+00000f90: 7879 5f70 726f 746f 636f 6c2e 0a20 2020  xy_protocol..   
+00000fa0: 204e 6f74 653a 2054 6f20 6164 6420 6e6f   Note: To add no
+00000fb0: 6e2d 7072 6f78 7920 746f 206c 6973 7420  n-proxy to list 
+00000fc0: 6a75 7374 2070 7574 2027 2720 746f 2069  just put '' to i
+00000fd0: 742c 2079 6f75 2063 616e 2066 696e 6420  t, you can find 
+00000fe0: 6578 616d 706c 6520 7769 7468 2061 720a  example with ar.
+00000ff0: 0a2a 2070 726f 7879 5f70 6174 683a 2073  .* proxy_path: s
+00001000: 7472 207c 204e 6f6e 6520 3d20 4e6f 6e65  tr | None = None
+00001010: 0a0a 2020 2020 5061 7468 2074 6f20 796f  ..    Path to yo
+00001020: 7572 2070 726f 7879 2028 7072 6f78 795f  ur proxy (proxy_
+00001030: 6c69 7374 2077 696c 6c20 6265 2069 676e  list will be ign
+00001040: 6f72 6564 292e 2049 6620 796f 7572 2070  ored). If your p
+00001050: 726f 7869 6573 2064 6f65 736e 2774 2068  roxies doesn't h
+00001060: 6176 6520 616e 7920 7072 6f74 6f63 6f6c  ave any protocol
+00001070: 2079 6f75 2063 616e 2075 7365 2070 726f   you can use pro
+00001080: 7879 5f70 726f 746f 636f 6c0a 0a2a 2070  xy_protocol..* p
+00001090: 726f 7879 5f70 726f 746f 636f 6c3a 2073  roxy_protocol: s
+000010a0: 7472 207c 204e 6f6e 6520 3d20 4e6f 6e65  tr | None = None
+000010b0: 2c0a 0a20 2020 2050 726f 7879 2070 726f  ,..    Proxy pro
+000010c0: 746f 636f 6c2e 2059 6f75 7220 7072 6f78  tocol. Your prox
+000010d0: 6965 7320 6060 6068 6c74 7620 3d20 486c  ies ```hltv = Hl
+000010e0: 7476 2870 726f 7879 5f70 726f 746f 636f  tv(proxy_protoco
+000010f0: 6c3d 2768 7474 7027 202e 2e2e 2920 2d3e  l='http' ...) ->
+00001100: 2027 3131 2e31 312e 3131 2e31 313a 3131   '11.11.11.11:11
+00001110: 3131 2720 2d3e 2027 6874 7470 3a2f 2f31  11' -> 'http://1
+00001120: 312e 3131 2e31 312e 3131 3a31 3131 3127  1.11.11.11:1111'
+00001130: 0a0a 2a20 7265 6d6f 7665 5f70 726f 7879  ..* remove_proxy
+00001140: 3a20 626f 6f6c 203d 2046 616c 7365 0a0a  : bool = False..
+00001150: 2020 2020 5265 6d6f 7665 7320 7072 6f78      Removes prox
+00001160: 7920 6672 6f6d 206c 6973 7420 2870 726f  y from list (pro
+00001170: 7879 5f70 6174 6820 696e 636c 7564 6564  xy_path included
+00001180: 2920 6966 2063 6f6e 6e65 6374 696f 6e20  ) if connection 
+00001190: 756e 7375 6363 6573 7366 756c 6c79 0a0a  unsuccessfully..
+000011a0: 2a20 7469 6d65 6f75 743a 2069 6e74 203d  * timeout: int =
+000011b0: 2035 0a0a 2020 2020 4d61 7820 7469 6d65   5..    Max time
+000011c0: 2074 6f20 636c 6f73 6520 636f 6e6e 6563   to close connec
+000011d0: 7469 6f6e 2e20 5265 636f 6d6d 656e 6465  tion. Recommende
+000011e0: 6420 746f 2075 7365 2074 696d 656f 7574  d to use timeout
+000011f0: 3d31 2069 6620 796f 7520 6172 6520 7573  =1 if you are us
+00001200: 696e 6720 7261 6e64 6f6d 2070 726f 7869  ing random proxi
+00001210: 6573 2e0a 0a2a 2064 6562 7567 3a20 626f  es...* debug: bo
+00001220: 6f6c 203d 2046 616c 7365 0a0a 2a20 747a  ol = False..* tz
+00001230: 3a20 7374 7220 3d20 2745 7572 6f70 652f  : str = 'Europe/
+00001240: 436f 7065 6e68 6167 656e 273a 0a20 2020  Copenhagen':.   
+00001250: 200a 2020 2020 5469 6d65 7a6f 6e65 2063   .    Timezone c
+00001260: 6f6e 6669 672e 200a 200a 2020 2020 3c61  onfig. . .    <a
+00001270: 2068 7265 663d 2768 7474 7073 3a2f 2f67   href='https://g
+00001280: 6973 742e 6769 7468 7562 2e63 6f6d 2f68  ist.github.com/h
+00001290: 6579 616c 6578 656a 2f38 6266 3638 3866  eyalexej/8bf688f
+000012a0: 6436 3764 3731 3939 6265 3461 3136 3832  d67d7199be4a1682
+000012b0: 6233 6565 6337 3536 3827 3e54 6170 2068  b3eec7568'>Tap h
+000012c0: 6572 6520 3c2f 613e 2074 6f20 7365 6520  ere </a> to see 
+000012d0: 616c 6c20 6176 6169 6c61 626c 6520 7469  all available ti
+000012e0: 6d65 7a6f 6e65 730a 0a2a 2073 6166 655f  mezones..* safe_
+000012f0: 6d6f 6465 3a20 626f 6f6c 203d 2054 7275  mode: bool = Tru
+00001300: 650a 0a20 2020 2044 6973 616c 6c6f 7720  e..    Disallow 
+00001310: 746f 2077 7261 7020 7265 7374 7269 6374  to wrap restrict
+00001320: 6564 2064 6174 612e 2053 7769 7463 6820  ed data. Switch 
+00001330: 746f 2046 616c 7365 206f 6e6c 7920 6174  to False only at
+00001340: 2079 6f75 7220 6f77 6e20 7269 736b 2e0a   your own risk..
+00001350: 0a0a 2d2d 2d0a 0a23 2050 726f 7879 2055  ..---..# Proxy U
+00001360: 7361 6765 0a0a 2a2a 4c6f 6164 2050 726f  sage..**Load Pro
+00001370: 7869 6573 2066 726f 6d20 6c69 7374 2a2a  xies from list**
+00001380: 0a20 2020 200a 2020 2020 6060 600a 2020  .    .    ```.  
+00001390: 2020 7072 6f78 795f 6c69 7374 203d 205b    proxy_list = [
+000013a0: 2768 7474 703a 2f2f 3132 302e 3233 342e  'http://120.234.
+000013b0: 3230 332e 3137 313a 3930 3032 272c 2027  203.171:9002', '
+000013c0: 6874 7470 3a2f 2f31 3130 2e33 382e 3638  http://110.38.68
+000013d0: 2e33 383a 3830 275d 0a20 2020 200a 2020  .38:80'].    .  
+000013e0: 2020 686c 7476 203d 2048 6c74 7628 7072    hltv = Hltv(pr
+000013f0: 6f78 795f 6c69 7374 3d70 726f 7879 5f6c  oxy_list=proxy_l
+00001400: 6973 7429 0a0a 2020 2020 6060 600a 0a2a  ist)..    ```..*
+00001410: 2a4c 6f61 6420 5072 6f78 6965 7320 6672  *Load Proxies fr
+00001420: 6f6d 2066 696c 652a 2a0a 0a20 2020 2060  om file**..    `
+00001430: 6060 0a20 2020 2068 6c74 7620 3d20 486c  ``.    hltv = Hl
+00001440: 7476 2870 726f 7879 5f70 6174 683d 2750  tv(proxy_path='P
+00001450: 4154 485f 544f 5f50 524f 5859 2e54 5854  ATH_TO_PROXY.TXT
+00001460: 2729 0a20 2020 2060 6060 0a0a 0a2a 2a52  ').    ```...**R
+00001470: 656d 6f76 6520 7072 6f78 792a 2a0a 0a20  emove proxy**.. 
+00001480: 2020 2052 656d 6f76 6573 2062 6164 2070     Removes bad p
+00001490: 726f 7869 6573 0a20 2020 200a 2020 2020  roxies.    .    
+000014a0: 6060 600a 2020 2020 686c 7476 203d 2048  ```.    hltv = H
+000014b0: 6c74 7628 7072 6f78 795f 7061 7468 3d27  ltv(proxy_path='
+000014c0: 5041 5448 5f54 4f5f 5052 4f58 592e 5458  PATH_TO_PROXY.TX
+000014d0: 5427 2c20 7265 6d6f 7665 5f70 726f 7879  T', remove_proxy
+000014e0: 3d54 7275 6529 0a20 2020 2060 6060 0a0a  =True).    ```..
+000014f0: 2a2a 5072 6f74 6f63 6f6c 2075 7361 6765  **Protocol usage
+00001500: 2a2a 0a0a 2020 2020 6060 600a 2020 2020  **..    ```.    
+00001510: 7072 6f78 795f 6c69 7374 203d 205b 2731  proxy_list = ['1
+00001520: 3230 2e32 3334 2e32 3033 2e31 3731 3a39  20.234.203.171:9
+00001530: 3030 3227 2c20 2731 3130 2e33 382e 3638  002', '110.38.68
+00001540: 2e33 383a 3830 275d 0a20 2020 200a 2020  .38:80'].    .  
+00001550: 2020 686c 7476 203d 2048 6c74 7628 7072    hltv = Hltv(pr
+00001560: 6f78 795f 6c69 7374 3d70 726f 7879 5f6c  oxy_list=proxy_l
+00001570: 6973 742c 2070 726f 7879 5f70 726f 746f  ist, proxy_proto
+00001580: 636f 6c3d 2768 7474 7027 290a 2020 2020  col='http').    
+00001590: 6060 600a 0a2d 2d2d 0a0a 2320 4d65 7468  ```..---..# Meth
+000015a0: 6f64 730a 0a2a 202a 2a67 6574 5f6d 6174  ods..* **get_mat
+000015b0: 6368 6573 2864 6179 733a 2069 6e74 203d  ches(days: int =
+000015c0: 2031 2c20 6d69 6e5f 7374 6172 5f72 6174   1, min_star_rat
+000015d0: 696e 673a 2069 6e74 203d 2031 2c20 6c69  ing: int = 1, li
+000015e0: 7665 3a20 626f 6f6c 203d 2054 7275 652c  ve: bool = True,
+000015f0: 2066 7574 7572 653a 2062 6f6f 6c20 3d20   future: bool = 
+00001600: 5472 7565 292a 2a0a 0a20 2020 202d 6461  True)**..    -da
+00001610: 7973 2028 7468 6520 6e75 6d62 6572 206f  ys (the number o
+00001620: 6620 6461 7973 2069 6e74 6f20 7468 6520  f days into the 
+00001630: 6675 7475 7265 2074 6f20 6665 7463 6820  future to fetch 
+00001640: 6d61 7463 6865 7320 666f 7229 0a20 200a  matches for).  .
+00001650: 2020 2020 2d6d 696e 5f73 7461 725f 7261      -min_star_ra
+00001660: 7469 6e67 2028 7468 6520 6d69 6e69 6d75  ting (the minimu
+00001670: 6d20 7374 6172 2072 6174 696e 6720 666f  m star rating fo
+00001680: 7220 6d61 7463 6865 7320 746f 2069 6e63  r matches to inc
+00001690: 6c75 6465 290a 2020 0a20 2020 2060 6060  lude).  .    ```
+000016a0: 0a20 2020 2061 7761 6974 2068 6c74 762e  .    await hltv.
+000016b0: 6765 745f 6d61 7463 6865 7328 6461 7973  get_matches(days
+000016c0: 3d31 290a 2020 2020 0a20 2020 203e 3e3e  =1).    .    >>>
+000016d0: 205b 7b27 6964 273a 2027 3233 3731 3230   [{'id': '237120
+000016e0: 3127 2c20 2764 6174 6527 3a20 274c 4956  1', 'date': 'LIV
+000016f0: 4527 2c20 2774 696d 6527 3a20 274c 4956  E', 'time': 'LIV
+00001700: 4527 2c20 2774 6561 6d31 273a 2027 496d  E', 'team1': 'Im
+00001710: 7065 7269 616c 272c 2027 7465 616d 3227  perial', 'team2'
+00001720: 3a20 274d 4942 5227 2c20 2774 315f 6964  : 'MIBR', 't1_id
+00001730: 273a 2027 3934 3535 272c 2027 7432 5f69  ': '9455', 't2_i
+00001740: 6427 3a20 2739 3231 3527 2c20 276d 6170  d': '9215', 'map
+00001750: 7327 3a20 2733 272c 2027 7261 7469 6e67  s': '3', 'rating
+00001760: 273a 2031 2c20 2765 7665 6e74 273a 2027  ': 1, 'event': '
+00001770: 5245 5320 5265 6769 6f6e 616c 2053 6572  RES Regional Ser
+00001780: 6965 7320 3320 4c41 5441 4d27 7d2c 207b  ies 3 LATAM'}, {
+00001790: 2769 6427 3a20 2732 3337 3039 3634 272c  'id': '2370964',
+000017a0: 2027 6461 7465 273a 2027 3230 3234 2d30   'date': '2024-0
+000017b0: 342d 3136 272c 2027 7469 6d65 273a 2027  4-16', 'time': '
+000017c0: 3132 3a33 3027 2c20 2774 6561 6d31 273a  12:30', 'team1':
+000017d0: 2027 5341 5727 2c20 2774 6561 6d32 273a   'SAW', 'team2':
+000017e0: 2027 5361 6d70 6927 2c20 2774 315f 6964   'Sampi', 't1_id
+000017f0: 273a 2027 3130 3536 3727 2c20 2774 325f  ': '10567', 't2_
+00001800: 6964 273a 2027 3130 3639 3527 2c20 276d  id': '10695', 'm
+00001810: 6170 7327 3a20 2733 272c 2027 7261 7469  aps': '3', 'rati
+00001820: 6e67 273a 2031 2c20 2765 7665 6e74 273a  ng': 1, 'event':
+00001830: 2027 5468 756e 6465 7270 6963 6b20 576f   'Thunderpick Wo
+00001840: 726c 6420 4368 616d 7069 6f6e 7368 6970  rld Championship
+00001850: 2032 3032 3420 4555 2043 6c6f 7365 6420   2024 EU Closed 
+00001860: 5175 616c 6966 6965 7220 3127 7d2c 207b  Qualifier 1'}, {
+00001870: 2769 6427 3a20 2732 3337 3133 3637 272c  'id': '2371367',
+00001880: 2027 6461 7465 273a 2027 3230 3234 2d30   'date': '2024-0
+00001890: 342d 3136 272c 2027 7469 6d65 273a 2027  4-16', 'time': '
+000018a0: 3134 3a30 3027 2c20 2774 6561 6d31 273a  14:00', 'team1':
+000018b0: 2027 4761 696d 696e 2047 6c61 6469 6174   'Gaimin Gladiat
+000018c0: 6f72 7327 2c20 2774 6561 6d32 273a 2027  ors', 'team2': '
+000018d0: 5065 726d 6974 7461 272c 2027 7431 5f69  Permitta', 't1_i
+000018e0: 6427 3a20 2731 3135 3731 272c 2027 7432  d': '11571', 't2
+000018f0: 5f69 6427 3a20 2731 3230 3039 272c 2027  _id': '12009', '
+00001900: 6d61 7073 273a 2027 3327 2c20 2772 6174  maps': '3', 'rat
+00001910: 696e 6727 3a20 312c 2027 6576 656e 7427  ing': 1, 'event'
+00001920: 3a20 2745 6c69 7361 2049 6e76 6974 6174  : 'Elisa Invitat
+00001930: 696f 6e61 6c20 5370 7269 6e67 2032 3032  ional Spring 202
+00001940: 3427 7d5d 0a20 2020 200a 2020 2020 6060  4'}].    .    ``
+00001950: 600a 0a2a 202a 2a67 6574 5f6d 6174 6368  `..* **get_match
+00001960: 5f69 6e66 6f28 6d61 7463 685f 6964 3a20  _info(match_id: 
+00001970: 696e 7420 7c20 7374 722c 2074 6561 6d31  int | str, team1
+00001980: 2c20 7465 616d 322c 2065 7665 6e74 5f74  , team2, event_t
+00001990: 6974 6c65 2c20 7374 6174 733a 2062 6f6f  itle, stats: boo
+000019a0: 6c20 3d20 5472 7565 2c20 7072 6564 6963  l = True, predic
+000019b0: 7473 3a20 626f 6f6c 203d 2054 7275 6529  ts: bool = True)
+000019c0: 2a2a 0a20 200a 2020 2020 6060 600a 2020  **.  .    ```.  
+000019d0: 2020 6177 6169 7420 686c 7476 2e67 6574    await hltv.get
+000019e0: 5f6d 6174 6368 5f69 6e66 6f28 3233 3730  _match_info(2370
+000019f0: 3933 312c 2027 4d6f 757a 272c 2027 6661  931, 'Mouz', 'fa
+00001a00: 7a65 272c 2027 6965 6d2d 6368 656e 6764  ze', 'iem-chengd
+00001a10: 752d 3230 3234 2729 2020 0a20 200a 2020  u-2024')  .  .  
+00001a20: 2020 3e3e 3e28 3233 3730 3933 312c 2027    >>>(2370931, '
+00001a30: 3027 2c20 2732 272c 2027 4d61 7463 6820  0', '2', 'Match 
+00001a40: 6f76 6572 272c 205b 7b27 6d61 706e 616d  over', [{'mapnam
+00001a50: 6527 3a20 274f 7665 7270 6173 7327 2c20  e': 'Overpass', 
+00001a60: 2772 5f74 6561 6d31 273a 2027 3130 272c  'r_team1': '10',
+00001a70: 2027 725f 7465 616d 3227 3a20 2731 3327   'r_team2': '13'
+00001a80: 7d2c 207b 276d 6170 6e61 6d65 273a 2027  }, {'mapname': '
+00001a90: 4e75 6b65 272c 2027 725f 7465 616d 3127  Nuke', 'r_team1'
+00001aa0: 3a20 2736 272c 2027 725f 7465 616d 3227  : '6', 'r_team2'
+00001ab0: 3a20 2731 3327 7d2c 207b 276d 6170 6e61  : '13'}, {'mapna
+00001ac0: 6d65 273a 2027 4d69 7261 6765 272c 2027  me': 'Mirage', '
+00001ad0: 725f 7465 616d 3127 3a20 272d 272c 2027  r_team1': '-', '
+00001ae0: 725f 7465 616d 3227 3a20 272d 277d 5d2c  r_team2': '-'}],
+00001af0: 205b 7b27 6964 273a 2027 3138 3835 3027   [{'id': '18850'
+00001b00: 2c20 276e 6963 6b6e 616d 6527 3a20 274a  , 'nickname': 'J
+00001b10: 696d 7070 6861 7427 2c20 276b 6427 3a20  impphat', 'kd': 
+00001b20: 2733 332d 3239 272c 2027 6164 7227 3a20  '33-29', 'adr': 
+00001b30: 2738 302e 3927 2c20 2772 6174 696e 6727  '80.9', 'rating'
+00001b40: 3a20 2731 2e30 3827 7d2c 200a 2020 0a20  : '1.08'}, .  . 
+00001b50: 2020 207b 2769 6427 3a20 2731 3830 3732     {'id': '18072
+00001b60: 272c 2027 6e69 636b 6e61 6d65 273a 2027  ', 'nickname': '
+00001b70: 746f 727a 7369 272c 2027 6b64 273a 2027  torzsi', 'kd': '
+00001b80: 3236 2d32 3527 2c20 2761 6472 273a 2027  26-25', 'adr': '
+00001b90: 3730 2e35 272c 2027 7261 7469 6e67 273a  70.5', 'rating':
+00001ba0: 2027 312e 3032 277d 2c20 7b27 6964 273a   '1.02'}, {'id':
+00001bb0: 2027 3133 3636 3627 2c20 276e 6963 6b6e   '13666', 'nickn
+00001bc0: 616d 6527 3a20 2742 726f 6c6c 616e 272c  ame': 'Brollan',
+00001bd0: 2027 6b64 273a 2027 3235 2d33 3127 2c20   'kd': '25-31', 
+00001be0: 2761 6472 273a 2027 3638 2e34 272c 2027  'adr': '68.4', '
+00001bf0: 7261 7469 6e67 273a 2027 302e 3930 277d  rating': '0.90'}
+00001c00: 2c20 7b27 6964 273a 2027 3230 3331 3227  , {'id': '20312'
+00001c10: 2c20 276e 6963 6b6e 616d 6527 3a20 2778  , 'nickname': 'x
+00001c20: 6572 7469 6f4e 272c 2027 6b64 273a 2027  ertioN', 'kd': '
+00001c30: 3233 2d33 3127 2c20 2761 6472 273a 2027  23-31', 'adr': '
+00001c40: 3632 2e34 272c 2027 7261 7469 6e67 273a  62.4', 'rating':
+00001c50: 2027 302e 3832 277d 2c20 7b27 6964 273a   '0.82'}, {'id':
+00001c60: 2027 3136 3832 3027 2c20 276e 6963 6b6e   '16820', 'nickn
+00001c70: 616d 6527 3a20 2773 6975 6879 272c 2027  ame': 'siuhy', '
+00001c80: 6b64 273a 2027 3137 2d33 3027 2c20 2761  kd': '17-30', 'a
+00001c90: 6472 273a 2027 3531 2e36 272c 2027 7261  dr': '51.6', 'ra
+00001ca0: 7469 6e67 273a 2027 302e 3730 277d 2c20  ting': '0.70'}, 
+00001cb0: 7b27 6964 273a 2027 3138 3035 3327 2c20  {'id': '18053', 
+00001cc0: 276e 6963 6b6e 616d 6527 3a20 2762 726f  'nickname': 'bro
+00001cd0: 6b79 272c 2027 6b64 273a 2027 3334 2d32  ky', 'kd': '34-2
+00001ce0: 3227 2c20 2761 6472 273a 2027 3739 2e33  2', 'adr': '79.3
+00001cf0: 272c 2027 7261 7469 6e67 273a 2027 312e  ', 'rating': '1.
+00001d00: 3333 277d 2c20 7b27 6964 273a 2027 3939  33'}, {'id': '99
+00001d10: 3630 272c 2027 6e69 636b 6e61 6d65 273a  60', 'nickname':
+00001d20: 2027 6672 6f7a 656e 272c 2027 6b64 273a   'frozen', 'kd':
+00001d30: 2027 3333 2d32 3327 2c20 2761 6472 273a   '33-23', 'adr':
+00001d40: 2027 3835 2e35 272c 2027 7261 7469 6e67   '85.5', 'rating
+00001d50: 273a 2027 312e 3331 277d 2c20 7b27 6964  ': '1.31'}, {'id
+00001d60: 273a 2027 3131 3831 3627 2c20 276e 6963  ': '11816', 'nic
+00001d70: 6b6e 616d 6527 3a20 2772 6f70 7a27 2c20  kname': 'ropz', 
+00001d80: 276b 6427 3a20 2733 312d 3236 272c 2027  'kd': '31-26', '
+00001d90: 6164 7227 3a20 2737 332e 3027 2c20 2772  adr': '73.0', 'r
+00001da0: 6174 696e 6727 3a20 2731 2e32 3027 7d2c  ating': '1.20'},
+00001db0: 207b 2769 6427 3a20 2738 3138 3327 2c20   {'id': '8183', 
+00001dc0: 276e 6963 6b6e 616d 6527 3a20 2772 6169  'nickname': 'rai
+00001dd0: 6e27 2c20 276b 6427 3a20 2732 372d 3236  n', 'kd': '27-26
+00001de0: 272c 2027 6164 7227 3a20 2738 322e 3027  ', 'adr': '82.0'
+00001df0: 2c20 2772 6174 696e 6727 3a20 2731 2e31  , 'rating': '1.1
+00001e00: 3827 7d2c 207b 2769 6427 3a20 2734 3239  8'}, {'id': '429
+00001e10: 272c 2027 6e69 636b 6e61 6d65 273a 2027  ', 'nickname': '
+00001e20: 6b61 7272 6967 616e 272c 2027 6b64 273a  karrigan', 'kd':
+00001e30: 2027 3230 2d32 3827 2c20 2761 6472 273a   '20-28', 'adr':
+00001e40: 2027 3439 2e37 272c 2027 7261 7469 6e67   '49.7', 'rating
+00001e50: 273a 2027 302e 3831 277d 5d29 2020 0a20  ': '0.81'}])  . 
+00001e60: 2020 200a 2020 2020 6060 600a 2020 0a2a     .    ```.  .*
+00001e70: 202a 2a67 6574 5f72 6573 756c 7473 2864   **get_results(d
+00001e80: 6179 733a 2069 6e74 203d 2031 2c20 6d69  ays: int = 1, mi
+00001e90: 6e5f 7261 7469 6e67 3a20 696e 7420 3d20  n_rating: int = 
+00001ea0: 312c 206d 6178 3a20 696e 7420 3d20 3330  1, max: int = 30
+00001eb0: 2c20 6665 6174 7572 6564 3a20 626f 6f6c  , featured: bool
+00001ec0: 203d 2054 7275 652c 2072 6567 756c 6172   = True, regular
+00001ed0: 3a20 626f 6f6c 203d 2054 7275 6529 2920  : bool = True)) 
+00001ee0: 2d3e 2a2a 0a20 2020 200a 2020 2020 6060  ->**.    .    ``
+00001ef0: 600a 2020 2020 7072 696e 7428 6177 6169  `.    print(awai
+00001f00: 7420 686c 7476 2e67 6574 5f72 6573 756c  t hltv.get_resul
+00001f10: 7473 2829 290a 2020 0a20 2020 205b 7b27  ts()).  .    [{'
+00001f20: 6964 273a 2027 3233 3730 3933 3127 2c20  id': '2370931', 
+00001f30: 2774 6561 6d31 273a 2027 4d4f 555a 272c  'team1': 'MOUZ',
+00001f40: 2027 7465 616d 3227 3a20 2746 615a 6527   'team2': 'FaZe'
+00001f50: 2c20 2773 636f 7265 3127 3a20 2730 272c  , 'score1': '0',
+00001f60: 2027 7363 6f72 6532 273a 2027 3227 2c20   'score2': '2', 
+00001f70: 2772 6174 696e 6727 3a20 302c 2027 6576  'rating': 0, 'ev
+00001f80: 656e 7427 3a20 2749 454d 2043 6865 6e67  ent': 'IEM Cheng
+00001f90: 6475 2032 3032 3427 7d5d 0a20 2020 2060  du 2024'}].    `
+00001fa0: 6060 0a20 200a 2a20 2a2a 6765 745f 6576  ``.  .* **get_ev
+00001fb0: 656e 7473 286f 7574 676f 696e 673d 5472  ents(outgoing=Tr
+00001fc0: 7565 2c20 6675 7475 7265 3d54 7275 652c  ue, future=True,
+00001fd0: 206d 6178 5f65 7665 6e74 733d 3130 2920   max_events=10) 
+00001fe0: 2d3e 205b 2827 6964 272c 2027 7469 746c  -> [('id', 'titl
+00001ff0: 6527 2c20 2773 7461 7274 6461 7465 272c  e', 'startdate',
+00002000: 2027 656e 6464 6174 6527 295d 2a2a 0a0a   'enddate')]**..
+00002010: 2020 2020 6060 600a 2020 2020 6177 6169      ```.    awai
+00002020: 7420 686c 7476 2e67 6574 5f65 7665 6e74  t hltv.get_event
+00002030: 7328 6675 7475 7265 3d46 616c 7365 290a  s(future=False).
+00002040: 2020 2020 0a20 2020 203e 3e3e 5b7b 2769      .    >>>[{'i
+00002050: 6427 3a20 2737 3734 3927 2c20 2774 6974  d': '7749', 'tit
+00002060: 6c65 273a 2027 5468 756e 6465 7270 6963  le': 'Thunderpic
+00002070: 6b20 576f 726c 6420 4368 616d 7069 6f6e  k World Champion
+00002080: 7368 6970 2032 3032 3420 4555 2043 6c6f  ship 2024 EU Clo
+00002090: 7365 6420 5175 616c 6966 6965 7220 3127  sed Qualifier 1'
+000020a0: 2c20 2773 7461 7274 5f64 6174 6527 3a20  , 'start_date': 
+000020b0: 2731 2d34 272c 2027 656e 645f 6461 7465  '1-4', 'end_date
+000020c0: 273a 2027 3232 2d34 277d 2c20 7b27 6964  ': '22-4'}, {'id
+000020d0: 273a 2027 3736 3231 272c 2027 7469 746c  ': '7621', 'titl
+000020e0: 6527 3a20 2745 534c 2043 6861 6c6c 656e  e': 'ESL Challen
+000020f0: 6765 7220 4c65 6167 7565 2053 6561 736f  ger League Seaso
+00002100: 6e20 3437 204e 6f72 7468 2041 6d65 7269  n 47 North Ameri
+00002110: 6361 272c 2027 7374 6172 745f 6461 7465  ca', 'start_date
+00002120: 273a 2027 3133 2d32 272c 2027 656e 645f  ': '13-2', 'end_
+00002130: 6461 7465 273a 2027 3136 2d36 277d 5d0a  date': '16-6'}].
+00002140: 2020 2020 2020 0a20 2020 2060 6060 0a0a        .    ```..
+00002150: 2a20 2a2a 6765 745f 6576 656e 745f 7265  * **get_event_re
+00002160: 7375 6c74 7328 6576 656e 745f 6964 3a20  sults(event_id: 
+00002170: 696e 7420 7c20 7374 722c 2064 6179 733a  int | str, days:
+00002180: 2069 6e74 203d 2031 2c20 6d61 785f 3a20   int = 1, max_: 
+00002190: 696e 7420 3d20 3130 292a 2a0a 0a20 200a  int = 10)**..  .
+000021a0: 2020 2020 6060 600a 2020 2020 6177 6169      ```.    awai
+000021b0: 7420 6765 745f 6576 656e 745f 7265 7375  t get_event_resu
+000021c0: 6c74 7328 3731 3438 290a 2020 2020 0a20  lts(7148).    . 
+000021d0: 2020 203e 3e3e 5b7b 2769 6427 3a20 2732     >>>[{'id': '2
+000021e0: 3337 3039 3331 272c 2027 6461 7465 273a  370931', 'date':
+000021f0: 2027 3134 2d30 342d 3230 3234 272c 2027   '14-04-2024', '
+00002200: 7465 616d 3127 3a20 274d 4f55 5a27 2c20  team1': 'MOUZ', 
+00002210: 2774 6561 6d32 273a 2027 4661 5a65 272c  'team2': 'FaZe',
+00002220: 2027 7363 6f72 6531 273a 2027 3027 2c20   'score1': '0', 
+00002230: 2773 636f 7265 3227 3a20 2732 277d 5d0a  'score2': '2'}].
+00002240: 0a20 2020 2060 6060 0a0a 2a20 2a2a 6765  .    ```..* **ge
+00002250: 745f 6576 656e 745f 6d61 7463 6865 7328  t_event_matches(
+00002260: 6576 656e 745f 6964 3a20 7374 7220 7c20  event_id: str | 
+00002270: 696e 742c 2064 6179 733a 2069 6e74 203d  int, days: int =
+00002280: 2031 293a 2a2a 0a20 200a 2020 2020 6060   1):**.  .    ``
+00002290: 600a 2020 2020 6177 6169 7420 686c 7476  `.    await hltv
+000022a0: 2e67 6574 5f65 7665 6e74 5f6d 6174 6368  .get_event_match
+000022b0: 6573 2837 3134 3829 0a20 2020 200a 2020  es(7148).    .  
+000022c0: 2020 3e3e 3e5b 7b27 6964 273a 2027 3233    >>>[{'id': '23
+000022d0: 3730 3737 3127 2c20 2764 6174 6527 3a20  70771', 'date': 
+000022e0: 2732 3032 342d 3034 2d31 3827 2c20 2774  '2024-04-18', 't
+000022f0: 696d 6527 3a20 2731 353a 3330 272c 2027  ime': '15:30', '
+00002300: 7465 616d 3127 3a20 274d 6f6e 7465 272c  team1': 'Monte',
+00002310: 2027 7465 616d 3227 3a20 2770 6169 4e27   'team2': 'paiN'
+00002320: 2c20 2774 315f 6964 273a 2027 3131 3831  , 't1_id': '1181
+00002330: 3127 2c20 2774 325f 6964 273a 2027 3437  1', 't2_id': '47
+00002340: 3733 277d 2c20 7b27 6964 273a 2027 3233  73'}, {'id': '23
+00002350: 3730 3737 3227 2c20 2764 6174 6527 3a20  70772', 'date': 
+00002360: 2732 3032 342d 3034 2d31 3827 2c20 2774  '2024-04-18', 't
+00002370: 696d 6527 3a20 2731 373a 3030 272c 2027  ime': '17:00', '
+00002380: 7465 616d 3127 3a20 2749 6d70 6572 6961  team1': 'Imperia
+00002390: 6c27 2c20 2774 6561 6d32 273a 2027 4d65  l', 'team2': 'Me
+000023a0: 7469 7a70 6f72 7427 2c20 2774 315f 6964  tizport', 't1_id
+000023b0: 273a 2027 3934 3535 272c 2027 7432 5f69  ': '9455', 't2_i
+000023c0: 6427 3a20 2731 3136 3431 277d 2c20 7b27  d': '11641'}, {'
+000023d0: 6964 273a 2027 3233 3730 3737 3327 2c20  id': '2370773', 
+000023e0: 2764 6174 6527 3a20 2732 3032 342d 3034  'date': '2024-04
+000023f0: 2d31 3827 2c20 2774 696d 6527 3a20 2731  -18', 'time': '1
+00002400: 383a 3330 272c 2027 7465 616d 3127 3a20  8:30', 'team1': 
+00002410: 2746 5552 4941 272c 2027 7465 616d 3227  'FURIA', 'team2'
+00002420: 3a20 2739 7a27 2c20 2774 315f 6964 273a  : '9z', 't1_id':
+00002430: 2027 3832 3937 272c 2027 7432 5f69 6427   '8297', 't2_id'
+00002440: 3a20 2739 3939 3627 7d2c 207b 2769 6427  : '9996'}, {'id'
+00002450: 3a20 2732 3337 3037 3734 272c 2027 6461  : '2370774', 'da
+00002460: 7465 273a 2027 3230 3234 2d30 342d 3138  te': '2024-04-18
+00002470: 272c 2027 7469 6d65 273a 2027 3230 3a30  ', 'time': '20:0
+00002480: 3027 2c20 2774 6561 6d31 273a 2027 4d49  0', 'team1': 'MI
+00002490: 4252 272c 2027 7465 616d 3227 3a20 274f  BR', 'team2': 'O
+000024a0: 4727 2c20 2774 315f 6964 273a 2027 3932  G', 't1_id': '92
+000024b0: 3135 272c 2027 7432 5f69 6427 3a20 2731  15', 't2_id': '1
+000024c0: 3035 3033 277d 2c20 7b27 6964 273a 2027  0503'}, {'id': '
+000024d0: 3233 3730 3737 3527 2c20 2764 6174 6527  2370775', 'date'
+000024e0: 3a20 2732 3032 342d 3034 2d31 3827 2c20  : '2024-04-18', 
+000024f0: 2774 696d 6527 3a20 2732 313a 3330 272c  'time': '21:30',
+00002500: 2027 7465 616d 3127 3a20 2754 4244 272c   'team1': 'TBD',
+00002510: 2027 7465 616d 3227 3a20 2754 4244 272c   'team2': 'TBD',
+00002520: 2027 7431 5f69 6427 3a20 302c 2027 7432   't1_id': 0, 't2
+00002530: 5f69 6427 3a20 307d 2c20 7b27 6964 273a  _id': 0}, {'id':
+00002540: 2027 3233 3730 3737 3627 2c20 2764 6174   '2370776', 'dat
+00002550: 6527 3a20 2732 3032 342d 3034 2d31 3827  e': '2024-04-18'
+00002560: 2c20 2774 696d 6527 3a20 2732 333a 3030  , 'time': '23:00
+00002570: 272c 2027 7465 616d 3127 3a20 2754 4244  ', 'team1': 'TBD
+00002580: 272c 2027 7465 616d 3227 3a20 2754 4244  ', 'team2': 'TBD
+00002590: 272c 2027 7431 5f69 6427 3a20 302c 2027  ', 't1_id': 0, '
+000025a0: 7432 5f69 6427 3a20 307d 2c20 7b27 6964  t2_id': 0}, {'id
+000025b0: 273a 2027 3233 3730 3737 3727 2c20 2764  ': '2370777', 'd
+000025c0: 6174 6527 3a20 2732 3032 342d 3034 2d31  ate': '2024-04-1
+000025d0: 3927 2c20 2774 696d 6527 3a20 2730 303a  9', 'time': '00:
+000025e0: 3030 272c 2027 7465 616d 3127 3a20 2754  00', 'team1': 'T
+000025f0: 4244 272c 2027 7465 616d 3227 3a20 2754  BD', 'team2': 'T
+00002600: 4244 272c 2027 7431 5f69 6427 3a20 302c  BD', 't1_id': 0,
+00002610: 2027 7432 5f69 6427 3a20 307d 2c20 7b27   't2_id': 0}, {'
+00002620: 6964 273a 2027 3233 3730 3737 3827 2c20  id': '2370778', 
+00002630: 2764 6174 6527 3a20 2732 3032 342d 3034  'date': '2024-04
+00002640: 2d31 3927 2c20 2774 696d 6527 3a20 2731  -19', 'time': '1
+00002650: 353a 3030 272c 2027 7465 616d 3127 3a20  5:00', 'team1': 
+00002660: 2754 4244 272c 2027 7465 616d 3227 3a20  'TBD', 'team2': 
+00002670: 2754 4244 272c 2027 7431 5f69 6427 3a20  'TBD', 't1_id': 
+00002680: 302c 2027 7432 5f69 6427 3a20 307d 2c20  0, 't2_id': 0}, 
+00002690: 7b27 6964 273a 2027 3233 3730 3737 3927  {'id': '2370779'
+000026a0: 2c20 2764 6174 6527 3a20 2732 3032 342d  , 'date': '2024-
+000026b0: 3034 2d31 3927 2c20 2774 696d 6527 3a20  04-19', 'time': 
+000026c0: 2731 373a 3330 272c 2027 7465 616d 3127  '17:30', 'team1'
+000026d0: 3a20 2754 4244 272c 2027 7465 616d 3227  : 'TBD', 'team2'
+000026e0: 3a20 2754 4244 272c 2027 7431 5f69 6427  : 'TBD', 't1_id'
+000026f0: 3a20 302c 2027 7432 5f69 6427 3a20 307d  : 0, 't2_id': 0}
+00002700: 2c20 7b27 6964 273a 2027 3233 3730 3738  , {'id': '237078
+00002710: 3027 2c20 2764 6174 6527 3a20 2732 3032  0', 'date': '202
+00002720: 342d 3034 2d31 3927 2c20 2774 696d 6527  4-04-19', 'time'
+00002730: 3a20 2732 303a 3030 272c 2027 7465 616d  : '20:00', 'team
+00002740: 3127 3a20 2754 4244 272c 2027 7465 616d  1': 'TBD', 'team
+00002750: 3227 3a20 2754 4244 272c 2027 7431 5f69  2': 'TBD', 't1_i
+00002760: 6427 3a20 302c 2027 7432 5f69 6427 3a20  d': 0, 't2_id': 
+00002770: 307d 2c20 7b27 6964 273a 2027 3233 3730  0}, {'id': '2370
+00002780: 3738 3127 2c20 2764 6174 6527 3a20 2732  781', 'date': '2
+00002790: 3032 342d 3034 2d31 3927 2c20 2774 696d  024-04-19', 'tim
+000027a0: 6527 3a20 2732 323a 3330 272c 2027 7465  e': '22:30', 'te
+000027b0: 616d 3127 3a20 2754 4244 272c 2027 7465  am1': 'TBD', 'te
+000027c0: 616d 3227 3a20 2754 4244 272c 2027 7431  am2': 'TBD', 't1
+000027d0: 5f69 6427 3a20 302c 2027 7432 5f69 6427  _id': 0, 't2_id'
+000027e0: 3a20 307d 2c20 7b27 6964 273a 2027 3233  : 0}, {'id': '23
+000027f0: 3730 3738 3227 2c20 2764 6174 6527 3a20  70782', 'date': 
+00002800: 2732 3032 342d 3034 2d32 3027 2c20 2774  '2024-04-20', 't
+00002810: 696d 6527 3a20 2730 303a 3330 272c 2027  ime': '00:30', '
+00002820: 7465 616d 3127 3a20 2754 4244 272c 2027  team1': 'TBD', '
+00002830: 7465 616d 3227 3a20 2754 4244 272c 2027  team2': 'TBD', '
+00002840: 7431 5f69 6427 3a20 302c 2027 7432 5f69  t1_id': 0, 't2_i
+00002850: 6427 3a20 307d 2c20 7b27 6964 273a 2027  d': 0}, {'id': '
+00002860: 3233 3730 3738 3327 2c20 2764 6174 6527  2370783', 'date'
+00002870: 3a20 2732 3032 342d 3034 2d32 3027 2c20  : '2024-04-20', 
+00002880: 2774 696d 6527 3a20 2731 353a 3030 272c  'time': '15:00',
+00002890: 2027 7465 616d 3127 3a20 2754 4244 272c   'team1': 'TBD',
+000028a0: 2027 7465 616d 3227 3a20 2754 4244 272c   'team2': 'TBD',
+000028b0: 2027 7431 5f69 6427 3a20 302c 2027 7432   't1_id': 0, 't2
+000028c0: 5f69 6427 3a20 307d 2c20 7b27 6964 273a  _id': 0}, {'id':
+000028d0: 2027 3233 3730 3738 3427 2c20 2764 6174   '2370784', 'dat
+000028e0: 6527 3a20 2732 3032 342d 3034 2d32 3027  e': '2024-04-20'
+000028f0: 2c20 2774 696d 6527 3a20 2731 383a 3030  , 'time': '18:00
+00002900: 272c 2027 7465 616d 3127 3a20 2754 4244  ', 'team1': 'TBD
+00002910: 272c 2027 7465 616d 3227 3a20 2754 4244  ', 'team2': 'TBD
+00002920: 272c 2027 7431 5f69 6427 3a20 302c 2027  ', 't1_id': 0, '
+00002930: 7432 5f69 6427 3a20 307d 5d0a 2020 0a20  t2_id': 0}].  . 
+00002940: 2020 2060 6060 0a0a 2a20 2a2a 6765 745f     ```..* **get_
+00002950: 6576 656e 745f 696e 666f 2865 7665 6e74  event_info(event
+00002960: 5f69 643a 2073 7472 207c 2069 6e74 2c20  _id: str | int, 
+00002970: 6576 656e 745f 7469 746c 653a 2073 7472  event_title: str
+00002980: 2920 2d3e 2028 6576 656e 745f 6964 2c20  ) -> (event_id, 
+00002990: 6576 656e 745f 7469 746c 652c 2065 7665  event_title, eve
+000029a0: 6e74 5f73 7461 7274 2c20 6576 656e 745f  nt_start, event_
+000029b0: 656e 642c 2070 7269 7a65 2c20 7465 616d  end, prize, team
+000029c0: 5f6e 756d 2c20 6c6f 6361 7469 6f6e 2c20  _num, location, 
+000029d0: 6772 6f75 7073 292a 2a0a 0a20 2020 2060  groups)**..    `
+000029e0: 6060 0a20 2020 2061 7761 6974 2068 6c74  ``.    await hlt
+000029f0: 762e 6765 745f 6576 656e 745f 696e 666f  v.get_event_info
+00002a00: 2837 3134 382c 2027 5047 4c20 4353 3220  (7148, 'PGL CS2 
+00002a10: 4d61 6a6f 7220 436f 7065 6e68 6167 656e  Major Copenhagen
+00002a20: 3230 3234 2729 0a20 2020 200a 2020 2020  2024').    .    
+00002a30: 7b27 6964 273a 2037 3134 382c 2027 7469  {'id': 7148, 'ti
+00002a40: 746c 6527 3a20 2750 474c 2043 5332 204d  tle': 'PGL CS2 M
+00002a50: 616a 6f72 2043 6f70 656e 6861 6765 6e32  ajor Copenhagen2
+00002a60: 3032 3427 2c20 2773 7461 7274 273a 2027  024', 'start': '
+00002a70: 3231 2d33 272c 2027 656e 6427 3a20 2733  21-3', 'end': '3
+00002a80: 312d 3327 2c20 2770 7269 7a65 273a 2027  1-3', 'prize': '
+00002a90: 2431 2c32 3530 2c30 3030 272c 2027 7465  $1,250,000', 'te
+00002aa0: 616d 7327 3a20 2731 3627 2c20 276c 6f63  ams': '16', 'loc
+00002ab0: 6174 696f 6e27 3a20 2743 6f70 656e 6861  ation': 'Copenha
+00002ac0: 6765 6e2c 2044 656e 6d61 726b 272c 2027  gen, Denmark', '
+00002ad0: 6772 6f75 7027 3a20 5b5d 7d0a 2020 200a  group': []}.   .
+00002ae0: 2020 2020 6060 600a 0a0a 2a20 2a2a 6765      ```...* **ge
+00002af0: 745f 746f 705f 7465 616d 7328 6d61 785f  t_top_teams(max_
+00002b00: 7465 616d 733d 3330 2920 2d3e 205b 2772  teams=30) -> ['r
+00002b10: 616e 6b27 2c20 2774 6974 6c65 272c 2027  ank', 'title', '
+00002b20: 706f 696e 7473 272c 2027 6368 616e 6765  points', 'change
+00002b30: 272c 2027 6964 275d 2a2a 0a0a 2020 2020  ', 'id']**..    
+00002b40: 6060 600a 2020 2020 6177 6169 7420 686c  ```.    await hl
+00002b50: 7476 2e67 6574 5f74 6f70 5f74 6561 6d73  tv.get_top_teams
+00002b60: 2832 290a 2020 2020 0a20 2020 203e 3e3e  (2).    .    >>>
+00002b70: 5b7b 2769 6427 3a20 2731 3131 3127 2c20  [{'id': '1111', 
+00002b80: 2772 616e 6b27 3a20 2731 272c 2027 7469  'rank': '1', 'ti
+00002b90: 746c 6527 3a20 2746 615a 6527 2c20 2770  tle': 'FaZe', 'p
+00002ba0: 6f69 6e74 7327 3a20 2739 3339 272c 2027  oints': '939', '
+00002bb0: 6368 616e 6765 273a 2027 2d27 2c20 2769  change': '-', 'i
+00002bc0: 6427 3a20 2736 3636 3727 7d2c 207b 2769  d': '6667'}, {'i
+00002bd0: 6427 3a20 2731 3131 3127 2c20 2772 616e  d': '1111', 'ran
+00002be0: 6b27 3a20 2732 272c 2027 7469 746c 6527  k': '2', 'title'
+00002bf0: 3a20 274e 6174 7573 2056 696e 6365 7265  : 'Natus Vincere
+00002c00: 272c 2027 706f 696e 7473 273a 2027 3735  ', 'points': '75
+00002c10: 3727 2c20 2763 6861 6e67 6527 3a20 272b  7', 'change': '+
+00002c20: 3427 2c20 2769 6427 3a20 2734 3630 3827  4', 'id': '4608'
+00002c30: 7d5d 0a20 2020 2060 6060 0a0a 2a20 2a2a  }].    ```..* **
+00002c40: 6765 745f 7465 616d 5f69 6e66 6f28 7465  get_team_info(te
+00002c50: 616d 5f69 643a 2069 6e74 207c 2073 7472  am_id: int | str
+00002c60: 2c20 7469 746c 653a 2073 7472 2920 2d3e  , title: str) ->
+00002c70: 2028 7465 616d 5f69 642c 2074 6561 6d5f   (team_id, team_
+00002c80: 7469 746c 652c 2072 616e 6b2c 207b 2770  title, rank, {'p
+00002c90: 6c61 7965 7227 3a70 6c61 7965 725f 6964  layer':player_id
+00002ca0: 7d2c 2063 6f61 6368 2c20 6176 6572 6167  }, coach, averag
+00002cb0: 655f 6167 652c 2077 6565 6b73 5f69 6e5f  e_age, weeks_in_
+00002cc0: 746f 705f 3230 2c20 6c61 7374 5f74 726f  top_20, last_tro
+00002cd0: 7068 792c 2074 6f74 616c 5f74 726f 7068  phy, total_troph
+00002ce0: 7973 292a 2a0a 0a20 2020 2060 6060 0a20  ys)**..    ```. 
+00002cf0: 2020 2061 7761 6974 2068 6c74 762e 6765     await hltv.ge
+00002d00: 745f 7465 616d 5f69 6e66 6f28 3636 3637  t_team_info(6667
+00002d10: 2c20 2766 617a 6527 290a 2020 2020 0a20  , 'faze').    . 
+00002d20: 2020 203e 3e3e 7b27 6964 273a 2036 3636     >>>{'id': 666
+00002d30: 372c 2027 7469 746c 6527 3a20 2766 617a  7, 'title': 'faz
+00002d40: 6527 2c20 2772 616e 6b27 3a20 2731 272c  e', 'rank': '1',
+00002d50: 2027 706c 6179 6572 7327 3a20 7b27 6b61   'players': {'ka
+00002d60: 7272 6967 616e 273a 2034 3239 2c20 2772  rrigan': 429, 'r
+00002d70: 6169 6e27 3a20 3831 3833 2c20 2766 726f  ain': 8183, 'fro
+00002d80: 7a65 6e27 3a20 3939 3630 2c20 2772 6f70  zen': 9960, 'rop
+00002d90: 7a27 3a20 3131 3831 362c 2027 6272 6f6b  z': 11816, 'brok
+00002da0: 7927 3a20 3138 3035 337d 2c20 2763 6f61  y': 18053}, 'coa
+00002db0: 6368 273a 2027 4e45 4f27 2c20 2761 6765  ch': 'NEO', 'age
+00002dc0: 273a 2027 3236 2e36 272c 2027 7765 656b  ': '26.6', 'week
+00002dd0: 7374 6f70 3330 273a 2027 3236 3027 2c20  stop30': '260', 
+00002de0: 276c 6173 745f 7472 6f70 6879 273a 2027  'last_trophy': '
+00002df0: 4945 4d20 4368 656e 6764 7520 3230 3234  IEM Chengdu 2024
+00002e00: 272c 2027 746f 7461 6c5f 7472 6f70 6869  ', 'total_trophi
+00002e10: 6573 273a 2032 327d 0a20 2020 2060 6060  es': 22}.    ```
+00002e20: 0a0a 2a20 2a2a 6765 745f 6c61 7374 5f6e  ..* **get_last_n
+00002e30: 6577 7328 6d61 785f 7265 675f 6e65 7773  ews(max_reg_news
+00002e40: 3d32 2c20 6f6e 6c79 5f74 6f64 6179 3d54  =2, only_today=T
+00002e50: 7275 652c 206f 6e6c 795f 6665 6174 7572  rue, only_featur
+00002e60: 6564 3d46 616c 7365 2920 2d3e 205b 6461  ed=False) -> [da
+00002e70: 7465 2c20 5b66 6561 7475 7265 645f 6964  te, [featured_id
+00002e80: 2c20 6665 6174 7572 6564 5f74 6974 6c65  , featured_title
+00002e90: 2c20 6665 6174 7572 6564 5f64 6573 6369  , featured_desci
+00002ea0: 7074 696f 6e5d 2c20 5b72 6567 756c 6172  ption], [regular
+00002eb0: 5f69 642c 2072 6567 5f74 6974 6c65 2c20  _id, reg_title, 
+00002ec0: 7265 675f 7469 6d65 5d5d 2a2a 0a0a 2020  reg_time]]**..  
+00002ed0: 2020 6060 600a 2020 2020 6177 6169 7420    ```.    await 
+00002ee0: 686c 7476 2e67 6574 5f6c 6173 745f 6e65  hltv.get_last_ne
+00002ef0: 7773 286f 6e6c 795f 746f 6461 793d 5472  ws(only_today=Tr
+00002f00: 7565 290a 2020 2020 0a20 2020 203e 3e3e  ue).    .    >>>
+00002f10: 5b7b 2764 6174 6527 3a20 2731 352d 3034  [{'date': '15-04
+00002f20: 272c 2027 665f 6e65 7773 273a 205b 5d2c  ', 'f_news': [],
+00002f30: 2027 6e65 7773 273a 205b 7b27 6964 273a   'news': [{'id':
+00002f40: 2027 3338 3738 3427 2c20 2774 6974 6c65   '38784', 'title
+00002f50: 273a 2027 4d65 6469 613a 2046 5552 4941  ': 'Media: FURIA
+00002f60: 2070 7261 6374 6963 696e 6720 7769 7468   practicing with
+00002f70: 206b 7965 2069 6e20 706c 6163 6520 6f66   kye in place of
+00002f80: 2061 7254 272c 2027 706f 7374 6564 273a   arT', 'posted':
+00002f90: 2027 616e 2068 6f75 7220 6167 6f27 7d2c   'an hour ago'},
+00002fa0: 207b 2769 6427 3a20 2733 3837 3833 272c   {'id': '38783',
+00002fb0: 2027 7469 746c 6527 3a20 2765 6c65 6374   'title': 'elect
+00002fc0: 726f 4e69 6320 746f 2070 6c61 7920 666f  roNic to play fo
+00002fd0: 7220 5669 7274 7573 2e70 726f 2061 7420  r Virtus.pro at 
+00002fe0: 4553 4c20 5072 6f20 4c65 6167 7565 2053  ESL Pro League S
+00002ff0: 3139 272c 2027 706f 7374 6564 273a 2027  19', 'posted': '
+00003000: 3220 686f 7572 7320 6167 6f27 7d2c 207b  2 hours ago'}, {
+00003010: 2769 6427 3a20 2733 3837 3831 272c 2027  'id': '38781', '
+00003020: 7469 746c 6527 3a20 2754 6865 2045 5650  title': 'The EVP
+00003030: 7320 616e 6420 4265 7374 2046 6976 6520  s and Best Five 
+00003040: 6f66 2049 454d 2043 6865 6e67 6475 272c  of IEM Chengdu',
+00003050: 2027 706f 7374 6564 273a 2027 3720 686f   'posted': '7 ho
+00003060: 7572 7320 6167 6f27 7d5d 7d5d 0a20 200a  urs ago'}]}].  .
+00003070: 2020 2020 6060 600a 0a2a 202a 2a67 6574      ```..* **get
+00003080: 5f62 6573 745f 706c 6179 6572 7328 746f  _best_players(to
+00003090: 703a 2069 6e74 203d 2034 3029 202d 3e20  p: int = 40) -> 
+000030a0: 2827 7261 6e6b 272c 2027 6e61 6d65 272c  ('rank', 'name',
+000030b0: 2027 7465 616d 272c 2027 6d61 7073 272c   'team', 'maps',
+000030c0: 2027 7261 7469 6e67 2729 2a2a 0a0a 2020   'rating')**..  
+000030d0: 2020 6060 600a 2020 2020 6177 6169 7420    ```.    await 
+000030e0: 686c 7476 2e67 6574 5f62 6573 745f 706c  hltv.get_best_pl
+000030f0: 6179 6572 7328 3229 0a20 2020 200a 2020  ayers(2).    .  
+00003100: 2020 3e3e 3e5b 7b27 6964 273a 2027 3139    >>>[{'id': '19
+00003110: 3233 3027 2c20 2772 616e 6b27 3a20 312c  230', 'rank': 1,
+00003120: 2027 6e61 6d65 273a 2027 6d30 4e45 5359   'name': 'm0NESY
+00003130: 272c 2027 7465 616d 273a 2027 4732 272c  ', 'team': 'G2',
+00003140: 2027 6d61 7073 273a 2027 3434 272c 2027   'maps': '44', '
+00003150: 7261 7469 6e67 273a 2027 312e 3337 277d  rating': '1.37'}
+00003160: 2c20 7b27 6964 273a 2027 3138 3035 3327  , {'id': '18053'
+00003170: 2c20 2772 616e 6b27 3a20 322c 2027 6e61  , 'rank': 2, 'na
+00003180: 6d65 273a 2027 6272 6f6b 7927 2c20 2774  me': 'broky', 't
+00003190: 6561 6d27 3a20 2746 615a 6527 2c20 276d  eam': 'FaZe', 'm
+000031a0: 6170 7327 3a20 2735 3427 2c20 2772 6174  aps': '54', 'rat
+000031b0: 696e 6727 3a20 2731 2e31 3927 7d5d 0a20  ing': '1.19'}]. 
+000031c0: 2020 2060 6060 0a0a 2a20 2a2a 6765 745f     ```..* **get_
+000031d0: 706c 6179 6572 5f69 6e66 6f28 6964 3a20  player_info(id: 
+000031e0: 7374 7220 7c20 696e 742c 206e 6963 6b6e  str | int, nickn
+000031f0: 616d 653a 2073 7472 292a 2a0a 2020 0a20  ame: str)**.  . 
+00003200: 2060 6060 0a20 2061 7761 6974 2068 6c74   ```.  await hlt
+00003210: 762e 6765 745f 706c 6179 6572 5f69 6e66  v.get_player_inf
+00003220: 6f28 3739 3938 2c20 2773 316d 706c 6527  o(7998, 's1mple'
+00003230: 290a 2020 0a20 207b 2769 6427 3a20 3739  ).  .  {'id': 79
+00003240: 3938 2c20 276e 6963 6b6e 616d 6527 3a20  98, 'nickname': 
+00003250: 2773 316d 706c 6527 2c20 2774 6561 6d27  's1mple', 'team'
+00003260: 3a20 274e 6174 7573 2056 696e 6365 7265  : 'Natus Vincere
+00003270: 272c 2027 7465 616d 5f69 6427 3a20 3436  ', 'team_id': 46
+00003280: 3038 2c20 276e 616d 6527 3a20 274f 6c65  08, 'name': 'Ole
+00003290: 6b73 616e 6472 204b 6f73 7479 6c69 6576  ksandr Kostyliev
+000032a0: 272c 2027 6e61 7469 6f6e 616c 6974 7927  ', 'nationality'
+000032b0: 3a20 2755 6b72 6169 6e65 272c 2027 6167  : 'Ukraine', 'ag
+000032c0: 6527 3a20 3236 2c20 2772 6174 696e 6727  e': 26, 'rating'
+000032d0: 3a20 2730 2e39 3427 2c20 276b 7072 273a  : '0.94', 'kpr':
+000032e0: 2027 302e 3630 272c 2027 6873 273a 2027   '0.60', 'hs': '
+000032f0: 3537 2e39 2527 2c20 276c 6173 745f 6d61  57.9%', 'last_ma
+00003300: 7463 6865 7327 3a20 5b31 3033 3035 392c  tches': [103059,
+00003310: 2039 3937 3435 2c20 3939 3732 382c 2039   99745, 99728, 9
+00003320: 3936 3936 2c20 3939 3437 312c 2039 3933  9696, 99471, 993
+00003330: 3634 5d2c 2027 6c61 7374 5f74 726f 7068  64], 'last_troph
+00003340: 7927 3a20 2742 4c41 5354 2050 7265 6d69  y': 'BLAST Premi
+00003350: 6572 2053 7072 696e 6720 4669 6e61 6c20  er Spring Final 
+00003360: 3230 3232 272c 2027 746f 7461 6c5f 7472  2022', 'total_tr
+00003370: 6f70 6869 6573 273a 2033 302c 2027 746f  ophies': 30, 'to
+00003380: 7461 6c5f 6d76 7073 273a 2032 317d 0a20  tal_mvps': 21}. 
+00003390: 2060 6060 0a0a 2a20 2a2a 6765 7428 7479   ```..* **get(ty
+000033a0: 7065 3a20 7374 722c 2069 643a 2069 6e74  pe: str, id: int
+000033b0: 207c 2073 7472 207c 204e 6f6e 6520 3d20   | str | None = 
+000033c0: 4e6f 6e65 2c20 7469 746c 653a 2073 7472  None, title: str
+000033d0: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c20   | None = None, 
+000033e0: 7465 616d 313a 2073 7472 207c 204e 6f6e  team1: str | Non
+000033f0: 6520 3d20 4e6f 6e65 2c20 7465 616d 323a  e = None, team2:
+00003400: 2073 7472 207c 204e 6f6e 6520 3d20 4e6f   str | None = No
+00003410: 6e65 293a 2a2a 0a20 2028 4245 5441 2920  ne):**.  (BETA) 
+00003420: 5468 6973 206d 6574 686f 6420 6973 206e  This method is n
+00003430: 6f74 2066 696e 6973 6865 642e 2050 6f73  ot finished. Pos
+00003440: 7369 626c 6520 7479 7065 7320 2765 7665  sible types 'eve
+00003450: 6e74 7327 2c20 276d 6174 6368 6573 272c  nts', 'matches',
+00003460: 2027 7465 616d 7327 2c20 616c 736f 2075   'teams', also u
+00003470: 2063 616e 2061 6464 2069 6420 7c20 7469   can add id | ti
+00003480: 746c 6520 7c20 7465 616d 3120 7c20 7465  tle | team1 | te
+00003490: 616d 322c 2074 6f20 7061 7273 6520 6d6f  am2, to parse mo
+000034a0: 7265 2e0a 2020 0a20 2060 6060 0a20 200a  re..  .  ```.  .
+000034b0: 2020 6177 6169 7420 686c 7476 2e67 6574    await hltv.get
+000034c0: 2827 6d61 7463 6865 7327 2c20 3233 3731  ('matches', 2371
+000034d0: 3230 312c 2027 7265 732d 7265 6769 6f6e  201, 'res-region
+000034e0: 616c 2d73 6572 6965 732d 332d 6c61 7461  al-series-3-lata
+000034f0: 6d27 2c20 2749 4d50 4552 4941 4c27 2c20  m', 'IMPERIAL', 
+00003500: 274d 4942 5227 290a 2020 0a20 203e 3e3e  'MIBR').  .  >>>
+00003510: 2028 3233 3731 3230 312c 2030 2c20 302c   (2371201, 0, 0,
+00003520: 2027 4c49 5645 272c 205b 7b27 6d61 706e   'LIVE', [{'mapn
+00003530: 616d 6527 3a20 2756 6572 7469 676f 272c  ame': 'Vertigo',
+00003540: 2027 725f 7465 616d 3127 3a20 2736 272c   'r_team1': '6',
+00003550: 2027 725f 7465 616d 3227 3a20 2731 3327   'r_team2': '13'
+00003560: 7d2c 207b 276d 6170 6e61 6d65 273a 2027  }, {'mapname': '
+00003570: 4d69 7261 6765 272c 2027 725f 7465 616d  Mirage', 'r_team
+00003580: 3127 3a20 272d 272c 2027 725f 7465 616d  1': '-', 'r_team
+00003590: 3227 3a20 272d 277d 2c20 7b27 6d61 706e  2': '-'}, {'mapn
+000035a0: 616d 6527 3a20 2741 6e75 6269 7327 2c20  ame': 'Anubis', 
+000035b0: 2772 5f74 6561 6d31 273a 2027 2d27 2c20  'r_team1': '-', 
+000035c0: 2772 5f74 6561 6d32 273a 2027 2d27 7d5d  'r_team2': '-'}]
+000035d0: 2c20 5b5d 290a 2020 0a20 2060 6060 0a0a  , []).  .  ```..
+000035e0: 0a2d 2d2d 0a23 2045 7861 6d70 6c65 730a  .---.# Examples.
+000035f0: 0a2a 2a2a 2a53 696d 706c 6520 4578 616d  .****Simple Exam
+00003600: 706c 652a 2a2a 2a0a 0a60 6060 0a66 726f  ple****..```.fro
+00003610: 6d20 686c 7476 5f61 7379 6e63 5f61 7069  m hltv_async_api
+00003620: 2069 6d70 6f72 7420 486c 7476 0a0a 0a61   import Hltv...a
+00003630: 7379 6e63 2064 6566 2074 6573 7428 293a  sync def test():
+00003640: 0a0a 2020 2020 6173 796e 6320 7769 7468  ..    async with
+00003650: 2048 6c74 7628 2920 6173 2068 6c74 763a   Hltv() as hltv:
+00003660: 0a20 2020 2020 2070 7269 6e74 2861 7761  .      print(awa
+00003670: 6974 2068 6c74 762e 6765 745f 6576 656e  it hltv.get_even
+00003680: 745f 696e 666f 2837 3134 382c 2027 7067  t_info(7148, 'pg
+00003690: 6c2d 6373 322d 6d61 6a6f 722d 636f 7065  l-cs2-major-cope
+000036a0: 6e68 6167 656e 2d32 3032 3427 2929 0a0a  nhagen-2024'))..
+000036b0: 6966 205f 5f6e 616d 655f 5f20 3d3d 2022  if __name__ == "
+000036c0: 5f5f 6d61 696e 5f5f 223a 0a20 2020 2061  __main__":.    a
+000036d0: 7379 6e63 696f 2e72 756e 2874 6573 7428  syncio.run(test(
+000036e0: 2929 0a60 6060 0a0a 2a2a 2a2a 5072 6f78  )).```..****Prox
+000036f0: 7920 5061 7273 6572 2a2a 2a2a 0a0a 6060  y Parser****..``
+00003700: 600a 6672 6f6d 2068 6c74 765f 6173 796e  `.from hltv_asyn
+00003710: 635f 6170 6920 696d 706f 7274 2048 6c74  c_api import Hlt
+00003720: 760a 0a0a 6173 796e 6320 6465 6620 7465  v...async def te
+00003730: 7374 2829 3a0a 0a20 2020 2068 6c74 7620  st():..    hltv 
+00003740: 3d20 486c 7476 2864 6562 7567 3d54 7275  = Hltv(debug=Tru
+00003750: 652c 2070 726f 7879 5f70 6174 683d 2770  e, proxy_path='p
+00003760: 726f 7879 5f74 6573 742e 7478 7427 2c20  roxy_test.txt', 
+00003770: 7469 6d65 6f75 743d 312c 2072 656d 6f76  timeout=1, remov
+00003780: 655f 7072 6f78 793d 5472 7565 2c20 7072  e_proxy=True, pr
+00003790: 6f78 795f 7072 6f74 6f63 6f6c 3d27 6874  oxy_protocol='ht
+000037a0: 7470 2729 0a20 2020 200a 2020 2020 7072  tp').    .    pr
+000037b0: 696e 7428 6177 6169 7420 686c 7476 2e67  int(await hltv.g
+000037c0: 6574 5f65 7665 6e74 5f69 6e66 6f28 3731  et_event_info(71
+000037d0: 3438 2c20 2770 676c 2d63 7332 2d6d 616a  48, 'pgl-cs2-maj
+000037e0: 6f72 2d63 6f70 656e 6861 6765 6e2d 3230  or-copenhagen-20
+000037f0: 3234 2729 290a 0a69 6620 5f5f 6e61 6d65  24'))..if __name
+00003800: 5f5f 203d 3d20 225f 5f6d 6169 6e5f 5f22  __ == "__main__"
+00003810: 3a0a 2020 2020 6173 796e 6369 6f2e 7275  :.    asyncio.ru
+00003820: 6e28 7465 7374 2829 290a 6060 600a 0a2a  n(test()).```..*
+00003830: 2a2a 2a41 7574 6f6d 6174 6963 2070 6172  ***Automatic par
+00003840: 7365 7220 7769 7468 2061 7271 2061 6e64  ser with arq and
+00003850: 2072 6564 6973 2a2a 2a2a 0a0a 2d20 746f   redis****..- to
+00003860: 2072 756e 2074 7970 6520 2261 7271 2050   run type "arq P
+00003870: 4154 485f 544f 5f46 494c 452e 576f 726b  ATH_TO_FILE.Work
+00003880: 6572 5365 7474 696e 6773 220a 0a20 2020  erSettings"..   
+00003890: 2060 6060 0a20 2020 2069 6d70 6f72 7420   ```.    import 
+000038a0: 756a 736f 6e0a 2020 2020 696d 706f 7274  ujson.    import
+000038b0: 2061 7379 6e63 696f 0a20 2020 2066 726f   asyncio.    fro
+000038c0: 6d20 6172 7120 696d 706f 7274 2063 726f  m arq import cro
+000038d0: 6e0a 2020 2020 6672 6f6d 2072 6564 6973  n.    from redis
+000038e0: 2e61 7379 6e63 696f 2069 6d70 6f72 7420  .asyncio import 
+000038f0: 5265 6469 732c 2043 6f6e 6e65 6374 696f  Redis, Connectio
+00003900: 6e50 6f6f 6c0a 2020 2020 0a20 2020 2066  nPool.    .    f
+00003910: 726f 6d20 686c 7476 5f61 7379 6e63 5f61  rom hltv_async_a
+00003920: 7069 2069 6d70 6f72 7420 486c 7476 0a20  pi import Hltv. 
+00003930: 2020 200a 2020 2020 0a20 2020 200a 2020     .    .    .  
+00003940: 2020 6173 796e 6320 6465 6620 7374 6172    async def star
+00003950: 7475 7028 6374 7829 3a0a 2020 2020 2020  tup(ctx):.      
+00003960: 2020 6173 796e 6320 7769 7468 2048 6c74    async with Hlt
+00003970: 7628 6d61 785f 6465 6c61 793d 352c 2070  v(max_delay=5, p
+00003980: 726f 7879 5f70 6174 683d 2770 726f 7869  roxy_path='proxi
+00003990: 6573 2e74 7874 272c 2064 6562 7567 3d54  es.txt', debug=T
+000039a0: 7275 6529 2061 7320 686c 7476 3a0a 2020  rue) as hltv:.  
+000039b0: 2020 2020 2020 2020 2020 2020 6374 785b              ctx[
+000039c0: 2268 6c74 7622 5d20 3d20 686c 7476 0a20  "hltv"] = hltv. 
+000039d0: 200a 2020 2020 2020 2020 6374 785b 2272   .        ctx["r
+000039e0: 6564 6973 225d 203d 2072 6564 6973 5f63  edis"] = redis_c
+000039f0: 6c69 656e 7420 3d20 5265 6469 7328 0a20  lient = Redis(. 
+00003a00: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
+00003a10: 6374 696f 6e5f 706f 6f6c 3d43 6f6e 6e65  ction_pool=Conne
+00003a20: 6374 696f 6e50 6f6f 6c2e 6672 6f6d 5f75  ctionPool.from_u
+00003a30: 726c 2873 6574 7469 6e67 732e 7265 6469  rl(settings.redi
+00003a40: 735f 7572 6c29 290a 2020 2020 2020 2020  s_url)).        
+00003a50: 6c6f 6767 6572 2e73 7563 6365 7373 2866  logger.success(f
+00003a60: 2253 6368 6564 756c 6572 2073 7461 7274  "Scheduler start
+00003a70: 6564 2e20 5554 4320 7469 6d65 207b 6461  ed. UTC time {da
+00003a80: 7465 7469 6d65 2e75 7463 6e6f 7728 297d  tetime.utcnow()}
+00003a90: 2229 0a20 2020 200a 2020 2020 0a20 2020  ").    .    .   
+00003aa0: 2061 7379 6e63 2064 6566 2073 6875 7464   async def shutd
+00003ab0: 6f77 6e28 6374 7829 3a0a 2020 2020 2020  own(ctx):.      
+00003ac0: 2020 6177 6169 7420 6374 785b 2272 6564    await ctx["red
+00003ad0: 6973 225d 2e63 6c6f 7365 2829 0a20 2020  is"].close().   
+00003ae0: 200a 2020 2020 0a20 2020 2061 7379 6e63   .    .    async
+00003af0: 2064 6566 2070 6172 7365 5f6d 6174 6368   def parse_match
+00003b00: 6573 2863 7478 293a 0a20 2020 2020 2020  es(ctx):.       
+00003b10: 2068 6c74 7620 3d20 6374 785b 2268 6c74   hltv = ctx["hlt
+00003b20: 7622 5d0a 2020 2020 2020 2020 7265 6469  v"].        redi
+00003b30: 7320 3d20 6374 785b 2272 6564 6973 225d  s = ctx["redis"]
+00003b40: 0a20 2020 2020 2020 206d 6174 6368 6573  .        matches
+00003b50: 203d 2061 7761 6974 2068 6c74 762e 6765   = await hltv.ge
+00003b60: 745f 7570 636f 6d69 6e67 5f6d 6174 6368  t_upcoming_match
+00003b70: 6573 2831 2c20 3129 0a20 2020 2020 2020  es(1, 1).       
+00003b80: 2069 6620 6d61 7463 6865 733a 0a20 2020   if matches:.   
+00003b90: 2020 2020 2020 2020 2061 7761 6974 2072           await r
+00003ba0: 6564 6973 2e73 6574 2822 6d61 7463 6865  edis.set("matche
+00003bb0: 7322 2c20 756a 736f 6e2e 6475 6d70 7328  s", ujson.dumps(
+00003bc0: 6d61 7463 6865 7329 290a 2020 2020 2020  matches)).      
+00003bd0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00003be0: 2020 2020 6c6f 6767 6572 2e65 7272 6f72      logger.error
+00003bf0: 2822 6572 726f 7220 7061 7273 696e 6720  ("error parsing 
+00003c00: 6d61 7463 6865 7322 290a 2020 2020 0a20  matches").    . 
+00003c10: 2020 2061 7379 6e63 2064 6566 2070 6172     async def par
+00003c20: 7365 5f65 7665 6e74 7328 6374 7829 3a0a  se_events(ctx):.
+00003c30: 2020 2020 2020 2020 686c 7476 203d 2063          hltv = c
+00003c40: 7478 5b22 686c 7476 225d 0a20 2020 2020  tx["hltv"].     
+00003c50: 2020 2072 6564 6973 203d 2063 7478 5b22     redis = ctx["
+00003c60: 7265 6469 7322 5d0a 2020 2020 2020 2020  redis"].        
+00003c70: 6576 656e 7473 203d 2061 7761 6974 2068  events = await h
+00003c80: 6c74 762e 6765 745f 6576 656e 7473 2829  ltv.get_events()
+00003c90: 0a20 2020 2020 2020 2069 6620 6576 656e  .        if even
+00003ca0: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00003cb0: 6177 6169 7420 7265 6469 732e 7365 7428  await redis.set(
+00003cc0: 2265 7665 6e74 7322 2c20 756a 736f 6e2e  "events", ujson.
+00003cd0: 6475 6d70 7328 6576 656e 7473 2929 0a20  dumps(events)). 
+00003ce0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00003cf0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00003d00: 6572 726f 7228 2265 7272 6f72 2070 6172  error("error par
+00003d10: 7369 6e67 2065 7665 6e74 7322 290a 2020  sing events").  
+00003d20: 2020 0a20 2020 200a 2020 2020 6173 796e    .    .    asyn
+00003d30: 6320 6465 6620 7061 7273 655f 746f 705f  c def parse_top_
+00003d40: 7465 616d 7328 6374 7829 3a0a 2020 2020  teams(ctx):.    
+00003d50: 2020 2020 686c 7476 203d 2063 7478 5b22      hltv = ctx["
+00003d60: 686c 7476 225d 0a20 2020 2020 2020 2072  hltv"].        r
+00003d70: 6564 6973 203d 2063 7478 5b22 7265 6469  edis = ctx["redi
+00003d80: 7322 5d0a 2020 2020 2020 2020 746f 705f  s"].        top_
+00003d90: 7465 616d 7320 3d20 6177 6169 7420 686c  teams = await hl
+00003da0: 7476 2e67 6574 5f74 6f70 5f74 6561 6d73  tv.get_top_teams
+00003db0: 2833 3029 0a20 2020 2020 2020 2069 6620  (30).        if 
+00003dc0: 746f 705f 7465 616d 733a 0a20 2020 2020  top_teams:.     
+00003dd0: 2020 2020 2020 2061 7761 6974 2072 6564         await red
+00003de0: 6973 2e73 6574 2822 746f 705f 7465 616d  is.set("top_team
+00003df0: 7322 2c20 756a 736f 6e2e 6475 6d70 7328  s", ujson.dumps(
+00003e00: 746f 705f 7465 616d 7329 290a 2020 2020  top_teams)).    
+00003e10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00003e20: 2020 2020 2020 6c6f 6767 6572 2e65 7272        logger.err
+00003e30: 6f72 2822 6572 726f 7220 7061 7273 696e  or("error parsin
+00003e40: 6720 746f 7020 7465 616d 7322 290a 2020  g top teams").  
+00003e50: 2020 0a20 2020 200a 2020 2020 6173 796e    .    .    asyn
+00003e60: 6320 6465 6620 7061 7273 655f 746f 705f  c def parse_top_
+00003e70: 706c 6179 6572 7328 6374 7829 3a0a 2020  players(ctx):.  
+00003e80: 2020 2020 2020 686c 7476 203d 2063 7478        hltv = ctx
+00003e90: 5b22 686c 7476 225d 0a20 2020 2020 2020  ["hltv"].       
+00003ea0: 2072 6564 6973 203d 2063 7478 5b22 7265   redis = ctx["re
+00003eb0: 6469 7322 5d0a 2020 2020 2020 2020 746f  dis"].        to
+00003ec0: 705f 706c 6179 6572 7320 3d20 6177 6169  p_players = awai
+00003ed0: 7420 686c 7476 2e67 6574 5f62 6573 745f  t hltv.get_best_
+00003ee0: 706c 6179 6572 7328 3330 290a 2020 2020  players(30).    
+00003ef0: 2020 2020 6966 2074 6f70 5f70 6c61 7965      if top_playe
+00003f00: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+00003f10: 6177 6169 7420 7265 6469 732e 7365 7428  await redis.set(
+00003f20: 2274 6f70 5f74 6561 6d73 222c 2075 6a73  "top_teams", ujs
+00003f30: 6f6e 2e64 756d 7073 2874 6f70 5f70 6c61  on.dumps(top_pla
+00003f40: 7965 7273 2929 0a20 2020 2020 2020 2065  yers)).        e
+00003f50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00003f60: 206c 6f67 6765 722e 6572 726f 7228 2265   logger.error("e
+00003f70: 7272 6f72 2070 6172 7369 6e67 2074 6f70  rror parsing top
+00003f80: 2070 6c61 7965 7273 2229 0a20 2020 200a   players").    .
+00003f90: 2020 2020 0a20 2020 2061 7379 6e63 2064      .    async d
+00003fa0: 6566 2070 6172 7365 5f6c 6173 745f 6e65  ef parse_last_ne
+00003fb0: 7773 2863 7478 293a 0a20 2020 2020 2020  ws(ctx):.       
+00003fc0: 2068 6c74 7620 3d20 6374 785b 2268 6c74   hltv = ctx["hlt
+00003fd0: 7622 5d0a 2020 2020 2020 2020 7265 6469  v"].        redi
+00003fe0: 7320 3d20 6374 785b 2272 6564 6973 225d  s = ctx["redis"]
+00003ff0: 0a20 2020 2020 2020 206e 6577 7320 3d20  .        news = 
+00004000: 6177 6169 7420 686c 7476 2e67 6574 5f6c  await hltv.get_l
+00004010: 6173 745f 6e65 7773 286f 6e6c 795f 746f  ast_news(only_to
+00004020: 6461 793d 5472 7565 2c20 6d61 785f 7265  day=True, max_re
+00004030: 675f 6e65 7773 3d34 290a 2020 2020 2020  g_news=4).      
+00004040: 2020 6966 206e 6577 733a 0a20 2020 2020    if news:.     
+00004050: 2020 2020 2020 2061 7761 6974 2072 6564         await red
+00004060: 6973 2e73 6574 2822 6e65 7773 222c 2075  is.set("news", u
+00004070: 6a73 6f6e 2e64 756d 7073 286e 6577 7329  json.dumps(news)
+00004080: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00004090: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+000040a0: 6572 2e65 7272 6f72 2822 6572 726f 7220  er.error("error 
+000040b0: 7061 7273 696e 6720 6e65 7773 2229 0a20  parsing news"). 
+000040c0: 2020 200a 2020 2020 0a20 2020 2063 6c61     .    .    cla
+000040d0: 7373 2057 6f72 6b65 7253 6574 7469 6e67  ss WorkerSetting
+000040e0: 733a 0a20 2020 2020 2020 2072 6564 6973  s:.        redis
+000040f0: 5f73 6574 7469 6e67 7320 3d20 7365 7474  _settings = sett
+00004100: 696e 6773 2e72 6564 6973 5f70 6f6f 6c0a  ings.redis_pool.
+00004110: 2020 2020 2020 2020 6f6e 5f73 7461 7274          on_start
+00004120: 7570 203d 2073 7461 7274 7570 0a20 2020  up = startup.   
+00004130: 2020 2020 206f 6e5f 7368 7574 646f 776e       on_shutdown
+00004140: 203d 2073 6875 7464 6f77 6e0a 2020 2020   = shutdown.    
+00004150: 2020 2020 6675 6e63 7469 6f6e 7320 3d20      functions = 
+00004160: 5b70 6172 7365 5f6d 6174 6368 6573 2c0a  [parse_matches,.
+00004170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004180: 2020 2020 2070 6172 7365 5f65 7665 6e74       parse_event
+00004190: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+000041a0: 2020 2020 2020 2020 7061 7273 655f 746f          parse_to
+000041b0: 705f 7465 616d 732c 0a20 2020 2020 2020  p_teams,.       
+000041c0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+000041d0: 7273 655f 746f 705f 706c 6179 6572 732c  rse_top_players,
+000041e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000041f0: 2020 2020 2020 7061 7273 655f 6c61 7374        parse_last
+00004200: 5f6e 6577 732c 0a20 2020 2020 2020 2020  _news,.         
+00004210: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+00004220: 2020 2020 2020 6372 6f6e 5f6a 6f62 7320        cron_jobs 
+00004230: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
+00004240: 6372 6f6e 2870 6172 7365 5f6d 6174 6368  cron(parse_match
+00004250: 6573 2c20 6d69 6e75 7465 3d35 3929 2c0a  es, minute=59),.
+00004260: 2020 2020 2020 2020 2020 2020 6372 6f6e              cron
+00004270: 2870 6172 7365 5f65 7665 6e74 732c 2068  (parse_events, h
+00004280: 6f75 723d 302c 206d 696e 7574 653d 302c  our=0, minute=0,
+00004290: 2073 6563 6f6e 643d 3029 2c0a 2020 2020   second=0),.    
+000042a0: 2020 2020 2020 2020 6372 6f6e 2870 6172          cron(par
+000042b0: 7365 5f74 6f70 5f74 6561 6d73 2c20 6461  se_top_teams, da
+000042c0: 793d 302c 2068 6f75 723d 3138 2c20 6d69  y=0, hour=18, mi
+000042d0: 6e75 7465 3d31 2c20 7365 636f 6e64 3d33  nute=1, second=3
+000042e0: 3029 2c0a 2020 2020 2020 2020 2020 2020  0),.            
+000042f0: 6372 6f6e 2870 6172 7365 5f74 6f70 5f70  cron(parse_top_p
+00004300: 6c61 7965 7273 2c20 6461 793d 302c 2068  layers, day=0, h
+00004310: 6f75 723d 3230 2c20 6d69 6e75 7465 3d30  our=20, minute=0
+00004320: 2c20 7365 636f 6e64 3d30 292c 0a20 2020  , second=0),.   
+00004330: 2020 2020 2020 2020 2063 726f 6e28 7061           cron(pa
+00004340: 7273 655f 6c61 7374 5f6e 6577 732c 206d  rse_last_news, m
+00004350: 696e 7574 653d 3535 292c 0a20 2020 2020  inute=55),.     
+00004360: 2020 205d 0a0a 2020 2020 6060 600a 0a23     ]..    ```..#
+00004370: 2054 6573 7473 3a0a 0a2a 2a3c 6120 6872   Tests:..**<a hr
+00004380: 6566 3d27 6874 7470 733a 2f2f 6769 7468  ef='https://gith
+00004390: 7562 2e63 6f6d 2f61 6b69 6d65 7273 6c79  ub.com/akimersly
+000043a0: 732f 686c 7476 2d61 7379 6e63 2d61 7069  s/hltv-async-api
+000043b0: 2f62 6c6f 622f 6d61 696e 2f74 6573 742f  /blob/main/test/
+000043c0: 6861 7264 5f74 6573 742e 7079 273e 546f  hard_test.py'>To
+000043d0: 2074 6573 7420 6c69 6272 6172 7920 796f   test library yo
+000043e0: 7520 6361 6e20 7573 6520 7465 6d70 6f72  u can use tempor
+000043f0: 6172 696c 7920 7465 7374 2066 696c 653c  arily test file<
+00004400: 2f61 3e2a 2a0a 0a60 6060 0a0a 5061 7273  /a>**..```..Pars
+00004410: 6564 2032 3038 206d 6174 6368 6573 2e28  ed 208 matches.(
+00004420: 3937 7329 2045 5252 4f52 533a 2030 2f32  97s) ERRORS: 0/2
+00004430: 3038 0a50 6172 7365 6420 3235 2065 7665  08.Parsed 25 eve
+00004440: 6e74 732e 2832 3373 2920 4552 524f 5253  nts.(23s) ERRORS
+00004450: 3a20 302f 3235 0a50 6172 7365 6420 3331  : 0/25.Parsed 31
+00004460: 2074 6561 6d73 2e28 3431 7329 2045 5252   teams.(41s) ERR
+00004470: 4f52 533a 2030 2f33 310a 5061 7273 6564  ORS: 0/31.Parsed
+00004480: 2033 3120 706c 6179 6572 732e 2832 3873   31 players.(28s
+00004490: 2920 4552 524f 5253 3a20 302f 3331 0a45  ) ERRORS: 0/31.E
+000044a0: 5252 4f52 533d 300a 5355 4343 4553 533d  RRORS=0.SUCCESS=
+000044b0: 3238 340a 546f 7461 6c20 7061 7273 6564  284.Total parsed
+000044c0: 3d32 3834 0a54 6f74 616c 2074 696d 6520  =284.Total time 
+000044d0: 3936 2e38 3336 380a 0a60 6060 0a0a 2320  96.8368..```..# 
+000044e0: 4265 7461 202f 2055 6e72 656c 6561 7365  Beta / Unrelease
+000044f0: 640a 0a66 726f 6d20 686c 7476 5f61 7379  d..from hltv_asy
+00004500: 6e63 5f61 7069 2e75 6e72 656c 6561 7365  nc_api.unrelease
+00004510: 6420 696d 706f 7274 2055 6e72 656c 6561  d import Unrelea
+00004520: 7365 640a 0a23 2052 6571 7569 7265 6d65  sed..# Requireme
+00004530: 6e74 733a 0a0a 5079 7468 6f6e 2033 2e39  nts:..Python 3.9
+00004540: 2b0a 0a4c 6963 656e 7365 3a0a 484c 5456  +..License:.HLTV
+00004550: 2041 7379 6e63 2069 7320 6c69 6365 6e73   Async is licens
+00004560: 6564 2075 6e64 6572 2074 6865 204d 4954  ed under the MIT
+00004570: 204c 6963 656e 7365 2c20 616c 6c6f 7769   License, allowi
+00004580: 6e67 2066 6f72 2070 6572 736f 6e61 6c20  ng for personal 
+00004590: 616e 6420 636f 6d6d 6572 6369 616c 2075  and commercial u
+000045a0: 7365 2077 6974 6820 6d69 6e69 6d61 6c20  se with minimal 
+000045b0: 7265 7374 7269 6374 696f 6e73 2e0a 0a    restrictions...
```

