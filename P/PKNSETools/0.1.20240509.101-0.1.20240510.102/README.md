# Comparing `tmp/PKNSETools-0.1.20240509.101.tar.gz` & `tmp/PKNSETools-0.1.20240510.102.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240509.101.tar", last modified: Thu May  9 11:18:23 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240510.102.tar", last modified: Fri May 10 12:01:21 2024, max compression
```

## Comparing `PKNSETools-0.1.20240509.101.tar` & `PKNSETools-0.1.20240510.102.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 11:18:23.615875 PKNSETools-0.1.20240509.101/
--rw-rw-rw-   0        0        0     2663 2024-05-09 11:18:23.615875 PKNSETools-0.1.20240509.101/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 11:18:23.600254 PKNSETools-0.1.20240509.101/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-05-09 11:18:23.600254 PKNSETools-0.1.20240509.101/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 11:18:23.600254 PKNSETools-0.1.20240509.101/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3386 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10770 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2635 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0     9360 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0    13763 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       31 2024-05-09 11:18:18.000000 PKNSETools-0.1.20240509.101/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 11:18:23.600254 PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61961 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22038 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29916 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-09 11:18:23.600254 PKNSETools-0.1.20240509.101/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2663 2024-05-09 11:18:23.000000 PKNSETools-0.1.20240509.101/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2024-05-09 11:18:23.000000 PKNSETools-0.1.20240509.101/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 11:18:23.000000 PKNSETools-0.1.20240509.101/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-09 11:18:16.000000 PKNSETools-0.1.20240509.101/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-05-09 11:18:23.000000 PKNSETools-0.1.20240509.101/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-09 11:18:23.000000 PKNSETools-0.1.20240509.101/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/README.md
--rw-rw-rw-   0        0        0       86 2024-05-09 11:18:23.615875 PKNSETools-0.1.20240509.101/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-05-09 11:16:02.000000 PKNSETools-0.1.20240509.101/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:01:21.725873 PKNSETools-0.1.20240510.102/
+-rw-rw-rw-   0        0        0     2663 2024-05-10 12:01:21.725873 PKNSETools-0.1.20240510.102/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 12:01:21.725873 PKNSETools-0.1.20240510.102/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-05-10 12:01:21.725873 PKNSETools-0.1.20240510.102/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:01:21.725873 PKNSETools-0.1.20240510.102/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3386 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10770 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2635 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0     9520 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0    13763 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       31 2024-05-10 12:01:16.000000 PKNSETools-0.1.20240510.102/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:01:21.725873 PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61961 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29916 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 12:01:21.725873 PKNSETools-0.1.20240510.102/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2663 2024-05-10 12:01:21.000000 PKNSETools-0.1.20240510.102/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2024-05-10 12:01:21.000000 PKNSETools-0.1.20240510.102/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 12:01:21.000000 PKNSETools-0.1.20240510.102/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-10 12:01:14.000000 PKNSETools-0.1.20240510.102/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-05-10 12:01:21.000000 PKNSETools-0.1.20240510.102/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-10 12:01:21.000000 PKNSETools-0.1.20240510.102/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-10 12:01:21.725873 PKNSETools-0.1.20240510.102/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-05-10 12:00:07.000000 PKNSETools-0.1.20240510.102/setup.py
```

### Comparing `PKNSETools-0.1.20240509.101/PKG-INFO` & `PKNSETools-0.1.20240510.102/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240509.101
+Version: 0.1.20240510.102
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240509.101.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240510.102.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240510.102/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240510.102/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240510.102/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240510.102/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240510.102/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240510.102/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240510.102/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240510.102/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240510.102/PKNSETools/PKIntraDay.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 
 """
+from time import sleep
 from datetime import datetime
 from mthrottle import Throttle
 
 import pandas as pd
 import requests
 
 from PKNSETools.PKConstants import (_base_domain, _chart_data_index_open_url,
@@ -139,14 +140,15 @@
         open_url = f'{_base_domain}{_quote_url_path_trade_info}'.format(self.symbol)
         trade_df = None
         try:
             trade_info = self.session.get(url=open_url, headers=_head)
             if trade_info.status_code == 429 or trade_info.status_code == 403:
                 print(f"{trade_info.status_code}: {trade_info.text}")
                 if (th.penalize()):
+                    sleep(5)
                     th.maxPenaltyCount += MAX_PENALTY_COUNT
             tradeInfoDict = trade_info.json()
             mCap = tradeInfoDict["marketDeptOrderBook"]["tradeInfo"]["totalMarketCap"]
             if mCap >= 1000000:
                 mCap = f"{int(mCap/1000000)}M"
             elif mCap >= 1000:
                 mCap = f"{int(mCap/1000)}k"
@@ -175,14 +177,15 @@
         get_details = f'{_base_domain}{_quote_url_path}'
         trade_df = None
         try:
             info = self.session.get(url=get_details.format(self.symbol), headers=_head)
             if info.status_code == 429 or info.status_code == 403:
                 print(f"{info.status_code}: {info.text}")
                 if (th.penalize()):
+                    sleep(5)
                     th.maxPenaltyCount += MAX_PENALTY_COUNT
             priceInfo = info.json()["priceInfo"]
             priceInfoDict = {
                 "Stock": self.symbol,
                 "LTP": priceInfo["lastPrice"],
                 "%Chng": round(priceInfo["pChange"],2),
                 "VWAP": priceInfo["vwap"],
@@ -192,14 +195,16 @@
             trade_df = pd.DataFrame([priceInfoDict])
         except:
             pass
         return trade_df
     
     def price_order_info(self):
         th.check()
+        if th._penaltyCount >= MAX_PENALTY_COUNT:
+            return None
         priceInfo = self.price_info()
         tradeInfo = self.order_trade_info()
         priceOrder_df = priceInfo.merge(tradeInfo, on='Stock', how='inner')
         return priceOrder_df
 
 # i = 0
 # while i <= 100:
```

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240510.102/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240510.102/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240510.102/PKNSETools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240509.101
+Version: 0.1.20240510.102
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240509.101.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240510.102.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240509.101/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240510.102/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/README.md` & `PKNSETools-0.1.20240510.102/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240509.101/setup.py` & `PKNSETools-0.1.20240510.102/setup.py`

 * *Files identical despite different names*

