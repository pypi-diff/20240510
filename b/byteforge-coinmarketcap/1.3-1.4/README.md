# Comparing `tmp/byteforge_coinmarketcap-1.3.tar.gz` & `tmp/byteforge_coinmarketcap-1.4.tar.gz`

## Comparing `byteforge_coinmarketcap-1.3.tar` & `byteforge_coinmarketcap-1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/MANIFEST
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/.github/FUNDING.yml
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/__init__.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/types/__init__.py
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/types/token_state.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/v1/cryptocurrency/listings/common.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/v1/cryptocurrency/listings/latest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/v1/key/__init__.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/v1/key/info.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/coinmarketcap/v2/cryptocurrency/quotes/historical.py
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/doc/coinmarketcap.png
--rw-r--r--   0        0        0    21711 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/doc/coinmarketcap_original.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/tests/__init__.py
--rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/tests/test_coinmarketcap.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/.gitignore
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/LICENSE
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/README.md
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/pyproject.toml
--rw-r--r--   0        0        0    25988 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.3/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/MANIFEST
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/.github/FUNDING.yml
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/__init__.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/types/__init__.py
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/types/token_state.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/v1/cryptocurrency/listings/common.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/v1/cryptocurrency/listings/latest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/v1/key/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/v1/key/info.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/coinmarketcap/v2/cryptocurrency/quotes/historical.py
+-rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/doc/coinmarketcap.png
+-rw-r--r--   0        0        0    21711 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/doc/coinmarketcap_original.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/tests/__init__.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/tests/test_coinmarketcap.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/.gitignore
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/LICENSE
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/README.md
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/pyproject.toml
+-rw-r--r--   0        0        0    25988 2020-02-02 00:00:00.000000 byteforge_coinmarketcap-1.4/PKG-INFO
```

### Comparing `byteforge_coinmarketcap-1.3/coinmarketcap/core.py` & `byteforge_coinmarketcap-1.4/coinmarketcap/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .v1.cryptocurrency.listings.common import SortOption, AuxFields, SortDir, FilterOptions
 from .v1.key.info import _key_info
 from .v1.key.info import _calls_left_today
 
 class Market(object):
 
 	_session = None
+	_caching_session = None
 	_debug_mode = False
 	_api_key = None
 	__DEFAULT_BASE_URL = 'https://pro-api.coinmarketcap.com/'
 	__DEFAULT_TIMEOUT = 30
 	__TEMPDIR_CACHE = True
 
 	def __init__(self, api_key = None, base_url = __DEFAULT_BASE_URL, request_timeout = __DEFAULT_TIMEOUT, tempdir_cache = __TEMPDIR_CACHE, debug_mode = False):
@@ -29,38 +30,61 @@
 		self.request_timeout = request_timeout
 		self._debug_mode = debug_mode
 		self.cache_filename = 'coinmarketcap_cache'
 		self.cache_name = os.path.join(tempfile.gettempdir(), self.cache_filename) if tempdir_cache else self.cache_filename
 		if not self._api_key:
 			raise ValueError('An API key is required for using the coinmarketcap API. Please visit https://pro.coinmarketcap.com/signup/ for more information.')
 
+	@property
+	def caching_session(self):
+		if not self._caching_session:
+			# define a a session with caching
+			self._caching_session = requests_cache.CachedSession(
+			 	cache_name=self.cache_name,
+			 	backend='sqlite', 
+			 	expire_after=120)
+			
+			self._caching_session.headers.update({
+					'Accept': 'application/json',
+				  	'X-CMC_PRO_API_KEY': self._api_key,
+				})
+
+		return self._caching_session
 
 	@property
 	def session(self):
 		if not self._session:
-			self._session = requests_cache.CachedSession(cache_name=self.cache_name, backend='sqlite', expire_after=120)
+		
+			# and a normal (non-caching) session
+			self._session = requests.Session()
+
 			self._session.headers.update({
 					'Accept': 'application/json',
 				  	'X-CMC_PRO_API_KEY': self._api_key,
 				})
+			
 		return self._session
 	
 
-	def _request(self, endpoint, params = {}):
+	def _request(self, endpoint, params = {}, no_cache = False):
 		if self._debug_mode:
 			print('Request URL: ' + self.base_url + endpoint)
 			if params:
 				print("Request Payload:\n" + json.dumps(params, indent=4))
 
 		try:
-			response_object = self.session.get(self.base_url + endpoint, params = params, timeout = self.request_timeout)
+			if no_cache:
+				response_object = self.session.get(self.base_url + endpoint, params=params, timeout=self.request_timeout)
+			else:
+				response_object = self.caching_session.get(self.base_url + endpoint, params=params, timeout=self.request_timeout)
 			
 			if self._debug_mode:
 				print('Response Code: ' + str(response_object.status_code))
-				print('From Cache?: ' + str(response_object.from_cache))
+				if hasattr(response_object, 'from_cache'):
+					print('From Cache?: ' + str(response_object.from_cache))
 				print("Response Payload:\n" + json.dumps(response_object.json(), indent=4))
 
 			if response_object.status_code == requests.codes.ok:
 				return response_object.json()
 			else:
 				raise Exception(f"Server returned {response_object.status_code} - {response_object.text}")
 		except Exception as e:
```

### Comparing `byteforge_coinmarketcap-1.3/coinmarketcap/types/token_state.py` & `byteforge_coinmarketcap-1.4/coinmarketcap/types/token_state.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.3/coinmarketcap/v1/cryptocurrency/listings/common.py` & `byteforge_coinmarketcap-1.4/coinmarketcap/v1/cryptocurrency/listings/common.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.3/coinmarketcap/v1/cryptocurrency/listings/latest.py` & `byteforge_coinmarketcap-1.4/coinmarketcap/v1/cryptocurrency/listings/latest.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,11 +51,11 @@
 		if filters.percent_change_24h_min is not None:
 			params['percent_change_24h_min'] = filters.percent_change_24h_min
 		if filters.percent_change_24h_max is not None:
 			params['percent_change_24h_max'] = filters.percent_change_24h_max
 		if filters.tags:
 			params['tag'] = ','.join(filters.tags)
 
-	response = market._request('v1/cryptocurrency/listings/latest', params=params)
+	response = market._request('v1/cryptocurrency/listings/latest', params=params, no_cache=True)
 	token_states = [TokenState.from_dict(token) for token in response['data']]
 
 	return token_states
```

### Comparing `byteforge_coinmarketcap-1.3/coinmarketcap/v1/key/info.py` & `byteforge_coinmarketcap-1.4/coinmarketcap/v1/key/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     
     Parameters:
         market (Market): An instance of the Market class, configured for API access.
 
     Returns:
         dict: A dictionary containing detailed key configuration information such as API limits.
     """
-    dct_response = market._request('v1/key/info')  
+    dct_response = market._request('v1/key/info', ignore_cache=True)
     return dct_response['data']
 
 
 def _calls_left_today(market):
     """
     Calculates how many API calls are left for today, based on the service plan's monthly call limit.
 
@@ -29,22 +29,22 @@
     Parameters:
         market (Market): An instance of the Market class, which handles the API communications.
 
     Returns:
         int: Approximate number of API calls left for the current day, based on daily usage 
              till the reset date and a monthly limit.
     """
-    dct_response = market._request('v1/key/info')
+    dct_response = market._request('v1/key/info', no_cache=True)
     quota_reset_dt = parser.parse(dct_response['data']['plan']['credit_limit_monthly_reset_timestamp'])
-    monthly_call_limit = dct_response['data']['plan']['credit_limit_monthly']
+    monthly_calls_remaining = dct_response['data']['usage']['current_month']['credits_left']
     
     # Ensure the current datetime is timezone-aware with UTC timezone  
     now_datetime = datetime.now(timezone.utc)
 
     # Calculate the timedelta  
     time_difference = quota_reset_dt - now_datetime
 
     # Extract the number of days as an integer  
     number_of_days = time_difference.days
 
     # Convert daily calls calculation into an integer
-    return int(monthly_call_limit / number_of_days) if number_of_days > 0 else 0  # Added safety for division
+    return int(monthly_calls_remaining / number_of_days) if number_of_days > 0 else 0  # Added safety for division
```

### Comparing `byteforge_coinmarketcap-1.3/coinmarketcap/v2/cryptocurrency/quotes/historical.py` & `byteforge_coinmarketcap-1.4/coinmarketcap/v2/cryptocurrency/quotes/historical.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.3/doc/coinmarketcap.png` & `byteforge_coinmarketcap-1.4/doc/coinmarketcap.png`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.3/doc/coinmarketcap_original.png` & `byteforge_coinmarketcap-1.4/doc/coinmarketcap_original.png`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.3/tests/test_coinmarketcap.py` & `byteforge_coinmarketcap-1.4/tests/test_coinmarketcap.py`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.3/LICENSE` & `byteforge_coinmarketcap-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.3/README.md` & `byteforge_coinmarketcap-1.4/README.md`

 * *Files identical despite different names*

### Comparing `byteforge_coinmarketcap-1.3/pyproject.toml` & `byteforge_coinmarketcap-1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "byteforge-coinmarketcap"
-version = "1.3"
+version = "1.4"
 description = "Python SDK for the coinmarketcap.com API."
 readme = "README.md"
 license = { file="LICENSE" }
 keywords = ["cryptocurrency", "API", "coinmarketcap", "BTC", "Bitcoin", "LTC", "Litecoin", "XRP", "Ripple", "ETH", "Ethereum"]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `byteforge_coinmarketcap-1.3/PKG-INFO` & `byteforge_coinmarketcap-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: byteforge-coinmarketcap
-Version: 1.3
+Version: 1.4
 Summary: Python SDK for the coinmarketcap.com API.
 Project-URL: Homepage, https://github.com/jmazzahacks/byteforge-coinmarketcap/
 Project-URL: Issues, https://github.com/jmazzahacks/byteforge-coinmarketcap/issues
 Author: Jason Byteforgia
 License:                              Apache License
                                Version 2.0, January 2004
                             http://www.apache.org/licenses/
```

