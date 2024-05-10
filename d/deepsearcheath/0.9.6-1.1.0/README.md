# Comparing `tmp/deepsearcheath-0.9.6-py3-none-any.whl.zip` & `tmp/deepsearcheath-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 13878 bytes, number of entries: 7
--rw-r--r--  2.0 unx       18 b- defN 22-Jan-23 07:47 deepsearcheath/__init__.py
--rw-r--r--  2.0 unx    49843 b- defN 23-Jun-20 09:25 deepsearcheath/deepsearch.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-20 09:27 deepsearcheath-0.9.6.dist-info/LICENSE
--rw-r--r--  2.0 unx      742 b- defN 23-Jun-20 09:27 deepsearcheath-0.9.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 09:27 deepsearcheath-0.9.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-20 09:27 deepsearcheath-0.9.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      588 b- defN 23-Jun-20 09:27 deepsearcheath-0.9.6.dist-info/RECORD
-7 files, 62655 bytes uncompressed, 12828 bytes compressed:  79.5%
+Zip file size: 15386 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       19 b- defN 24-May-10 07:39 deepsearcheath/__init__.py
+-rw-rw-rw-  2.0 fat    56920 b- defN 24-May-10 08:55 deepsearcheath/deepsearch.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-May-10 09:11 deepsearcheath-1.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1086 b- defN 24-May-10 09:11 deepsearcheath-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-10 09:11 deepsearcheath-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-May-10 09:11 deepsearcheath-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      589 b- defN 24-May-10 09:11 deepsearcheath-1.1.0.dist-info/RECORD
+7 files, 70279 bytes uncompressed, 14336 bytes compressed:  79.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: deepsearcheath/__init__.py
 Comment: 
 
 Filename: deepsearcheath/deepsearch.py
 Comment: 
 
-Filename: deepsearcheath-0.9.6.dist-info/LICENSE
+Filename: deepsearcheath-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: deepsearcheath-0.9.6.dist-info/METADATA
+Filename: deepsearcheath-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: deepsearcheath-0.9.6.dist-info/WHEEL
+Filename: deepsearcheath-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: deepsearcheath-0.9.6.dist-info/top_level.txt
+Filename: deepsearcheath-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: deepsearcheath-0.9.6.dist-info/RECORD
+Filename: deepsearcheath-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deepsearcheath/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-__all__ = ['api']
+__all__ = ['api']
```

## deepsearcheath/deepsearch.py

```diff
@@ -1,1024 +1,1098 @@
-import requests
-from datetime import datetime
-import time
-import os
-import asyncio
-import aiohttp
-import FinanceDataReader as fdr
-from pandas_datareader import data as pdr
-
-import pandas as pd
-import numpy as np
-
-from dotenv import load_dotenv
-from requests.auth import HTTPBasicAuth
-
-from dateutil.relativedelta import relativedelta
-
-load_dotenv(verbose=True)
-
-
-class asyncDeepSearchAPI(object):
-    _COMPUTE_API = "{}/v1/compute".format('https://api.deepsearch.com')
-    _AUTH_ID = os.getenv('_AUTH_ID')
-    _AUTH_PW = os.getenv('_AUTH_PW')
-    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
-    
-    @classmethod
-    async def compute(cls, query, locale='ko_KR'):
-        params = {
-            'input': query,
-            'locale': locale
-        } 
-        _count = 0
-        while True:
-            try:
-                async with aiohttp.ClientSession() as sess:
-
-                    async with sess.post( url=cls._COMPUTE_API, auth=aiohttp.BasicAuth(cls._AUTH_ID, cls._AUTH_PW), data=params, timeout=120 ) as co_resp:
-                        response_json = await co_resp.json()
-                        if (co_resp.status != 200) or (not response_json['success']):
-                            try:
-                                print("Response code, Success status:", co_resp.status, response_json['success'])
-                            except:
-                                print(response_json)
-                            print("Exception query log:", query)
-                            print(response_json)
-                            return None
-
-                        pods = response_json['data']['pods']  # pods[0]: input
-
-                        if pods[1]['class'] == 'Result:DataFrame':
-                            data    =    pods[1]['content']['data']
-                            index   =   pods[1]['content']['index']
-                            dtypes  =  pods[1]['content']['dtypes']
-                            columns = pods[1]['content']['columns']
-
-                            results = []
-
-                            no_obs = len(data[columns[0]])
-                            for i in range(no_obs):
-                                item = dict()
-                                for col in columns:
-                                    item[col] = data[col][i]
-                                results.append(item)
-
-                            df_results = pd.DataFrame(results)
-
-                            if df_results.empty:
-                                return None
-
-                            for col in dtypes.keys():  # pyarrow converting
-                                df_results[col] = df_results[col].astype(dtypes[col])
-
-                            df_results = df_results.set_index(index)  # 'symbol'
-                            df_results = df_results.sort_index()
-
-                            return df_results
-
-                        elif pods[1]['class'] == 'Result:DocumentTrendsResult':
-                            data    =    pods[1]['content']['data']
-                            trends  =   pods[1]['content']['data']['trends']
-                            total_matches = trends[0]['total_matches']
-                            buckets = trends[0]['buckets']
-
-                            df_results = pd.DataFrame(buckets)
-                            
-                            return df_results
-
-                        else:
-                            return pods[1]['content']
-            
-            except Exception as e:
-                print("Exception query log:", query)
-                print(e)
-                _count += 1
-                if _count > 5:
-                    return [None]
-                time.sleep(5)
-                continue
-
-
-
-class asyncDeepSearchAPI_mk2(object):
-    _COMPUTE_API = "{}/v1/compute".format('https://api.deepsearch.com')
-    _AUTH_ID = os.getenv('_AUTH_ID')
-    _AUTH_PW = os.getenv('_AUTH_PW')
-    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
-    
-    @classmethod
-    async def compute(cls, query, locale='ko_KR', timeout=120, max_count=5, sentiment=False):
-        params = {
-            'input': query,
-            'locale': locale
-        } 
-        _count = 0
-        retry = False
-        while True:
-            try:
-                async with aiohttp.ClientSession() as sess:
-
-                    async with sess.post( url=cls._COMPUTE_API, auth=aiohttp.BasicAuth(cls._AUTH_ID, cls._AUTH_PW), data=params, timeout=timeout ) as co_resp:
-                        response_json = await co_resp.json()
-                        if (co_resp.status != 200) or (not response_json['success']):
-                            print("Response code, Success status:", co_resp.status, response_json['success'])
-                            if sentiment:
-                                raise Exception("Response code, Success status:", co_resp.status, response_json['success'])
-                            return None, query
-                            return None
-
-                        pods = response_json['data']['pods']  # pods[0]: input
-
-                        if pods[1]['class'] == 'Result:DataFrame':
-                            data    =    pods[1]['content']['data']
-                            index   =   pods[1]['content']['index']
-                            dtypes  =  pods[1]['content']['dtypes']
-                            columns = pods[1]['content']['columns']
-
-                            results = []
-
-                            no_obs = len(data[columns[0]])
-                            for i in range(no_obs):
-                                item = dict()
-                                for col in columns:
-                                    item[col] = data[col][i]
-                                results.append(item)
-
-                            df_results = pd.DataFrame(results)
-
-                            if df_results.empty:
-                                print("Empty DataFrame:", query)
-                                return None, query
-                                return None
-
-                            for col in dtypes.keys():  # pyarrow converting
-                                df_results[col] = df_results[col].astype(dtypes[col])
-
-                            df_results = df_results.set_index(index)  # 'symbol'
-                            df_results = df_results.sort_index()
-
-                            if retry: print("retry success")
-                            return df_results, query
-                            return df_results
-
-                        elif pods[1]['class'] == 'Result:DocumentTrendsResult':
-                            data    =    pods[1]['content']['data']
-                            trends  =   pods[1]['content']['data']['trends']
-                            total_matches = trends[0]['total_matches']
-                            buckets = trends[0]['buckets']
-
-                            df_results = pd.DataFrame(buckets)
-                            
-                            if retry: print("retry success")
-                            return df_results, query
-                            return df_results
-
-                        else:
-                            if retry: print("retry success")
-                            return pods[1]['content'], query
-                            return pods[1]['content']
-            
-            except Exception as e:
-                retry = True
-                print("Exception query log:", query)
-                print(e)
-                _count += 1
-                print(_count)
-                if _count > max_count:
-                    print('max count exceeded')
-                    return [None], query
-                    return [None]
-                time.sleep(5)
-                continue
-
-
-
-
-class DeepSearchAPI(object):
-    _COMPUTE_API = "{}/v1/compute".format('https://api.deepsearch.com')
-    _AUTH_ID = os.getenv('_AUTH_ID')
-    _AUTH_PW = os.getenv('_AUTH_PW')
-    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
-
-    @classmethod
-    def compute(cls, query, locale='ko_KR'):
-        params = {
-            'input': query,
-            'locale': locale
-        } 
-
-        response = requests.post( url=cls._COMPUTE_API, auth=cls._AUTH, data=params, timeout=120 )
-
-        if (response.status_code != 200) or (not response.json()['success']):
-            print("Response code:", response.status_code)
-            print("AUTH info:", cls._AUTH_ID, cls._AUTH_PW)
-            print("Exception query log:", query)
-            return None
-
-        pods = response.json()['data']['pods']  # pods[0]: input
-
-        if pods[1]['class'] == 'Result:DataFrame':
-            data    =    pods[1]['content']['data']
-            index   =   pods[1]['content']['index']
-            dtypes  =  pods[1]['content']['dtypes']
-            columns = pods[1]['content']['columns']
-
-            results = []
-
-            no_obs = len(data[columns[0]])
-            for i in range(no_obs):
-                item = dict()
-                for col in columns:
-                    item[col] = data[col][i]
-                results.append(item)
-
-            df_results = pd.DataFrame(results)
-
-            if df_results.empty:
-                return None
-
-            for col in dtypes.keys():  # pyarrow converting
-                df_results[col] = df_results[col].astype(dtypes[col])
-
-            df_results = df_results.set_index(index)  # 'symbol'
-            df_results = df_results.sort_index()
-
-            return df_results
-
-        elif pods[1]['class'] == 'Result:DocumentTrendsResult':
-            data    =    pods[1]['content']['data']
-            trends  =   pods[1]['content']['data']['trends']
-            total_matches = trends[0]['total_matches']
-            buckets = trends[0]['buckets']
-
-            df_results = pd.DataFrame(buckets)
-            
-            return df_results
-
-        else:
-            return pods[1]['content']
-
-
-class WaveletAPI(object):
-    _COMPUTE_API_INDEX = 'https://api.ddi.deepsearch.com/wavelet/v1/indices' 
-    _COMPUTE_API = 'https://api.ddi.deepsearch.com/wavelet/v1/prices'
-    _AUTH_ID = os.getenv('_AUTH_ID')
-    _AUTH_PW = os.getenv('_AUTH_PW')
-    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
-
-    @classmethod
-    def compute(cls, symbol, date_from, date_to, interval=None):
-        assert type(symbol) == list
-        num_of_pdf = len(symbol)
-        symbol_str = ','.join(symbol)
-        return_dict = dict()
-        
-        if symbol in [['KOSPI'], ['KOSDAQ']]:
-            query = f'{cls._COMPUTE_API_INDEX}/{symbol_str}?from={date_from}&to={date_to}'
-        else:
-            query = f'{cls._COMPUTE_API}/{symbol_str}?from={date_from}&to={date_to}'
-
-        response = requests.get(query, auth=cls._AUTH)
-        
-        if (response.status_code != 200):
-            print("Response code:", response.status_code)
-            print("AUTH info:", cls._AUTH_ID, cls._AUTH_PW)
-            print("Exception query log:", query)
-            return None
-            
-        # print(query)
-
-        if symbol in [['KOSPI'], ['KOSDAQ']]:
-            data = response.json()['data'][0]
-            points = data['points']
-
-            df = pd.DataFrame.from_dict(points)
-            df = df.set_index(['timestamp'])
-            df.index = pd.to_datetime(df.index)
-
-            return_dict[symbol[0]] = df  #! 인덱스 리턴은 하나밖에 못한다가 됨
-            return return_dict
-
-        else:
-            for i in range(num_of_pdf):
-                try:
-                    data = response.json()['data'][i]
-                    points = data['points']
-
-                    df = pd.DataFrame.from_dict(points)
-                    df = df.set_index(['timestamp'])
-                    df.index = pd.to_datetime(df.index)
-
-                    if num_of_pdf == 1:
-                        return_dict[data['exchange'] + ':' + data['symbol']] = df
-                        return return_dict
-                
-                    return_dict[data['exchange'] + ':' + data['symbol']] = df
-                except:  
-                    print("Response code:", response.status_code)
-                    print("Exception query log:", query)
-                    break
-
-            return return_dict
-
-
-class asyncWaveletAPI(object):
-    _COMPUTE_API_INDEX = 'https://api.ddi.deepsearch.com/wavelet/v1/indices' 
-    _COMPUTE_API = 'https://api.ddi.deepsearch.com/wavelet/v1/prices'
-    _AUTH_ID = os.getenv('_AUTH_ID')
-    _AUTH_PW = os.getenv('_AUTH_PW')
-    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
-
-    @classmethod
-    def compute():
-        return
-
-
-class HaystackAPI(object):
-    """
-    api.ddi.deepsearch.com/haystack/v1/news/_search?query=삼성전자&count=1
-        - https://help.deepsearch.com/ddi/haystack/search
-
-    @category - section: 
-        - news
-            politics, economy, society, culture, world, tech, entertainment, opinion
-        - research
-            market, strategy, company, industry, economy, bond   
-        - company
-            ir, disclosure
-        - patent
-            patent
-    """
-    _COMPUTE_API = "{}/v1".format('https://api.ddi.deepsearch.com/haystack')
-    _AUTH_ID = os.getenv('_AUTH_ID')
-    _AUTH_PW = os.getenv('_AUTH_PW')
-    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
-
-    @classmethod
-    def compute(cls, category, section, params, module='_search?', group_by='securities.symbol', locale='ko_KR'):
-        assert type(params) is dict
-        url = os.path.join(cls._COMPUTE_API, category, section, module)
-        if module == '_aggregation?':
-            params['groupby'] = group_by
-        response = requests.get( url=url, auth=cls._AUTH, params=params, timeout=30 )
-
-        if (response.status_code != 200) or (not response.json()['found']):
-            print("Response code, Found status:", response.status_code, response.json()['found'])
-            print("Exception query log:", response.url)
-            return None
-
-        return response.json()['data']
-
-
-class asyncHaystackAPI(object):
-    """
-    api.ddi.deepsearch.com/haystack/v1/news/_search?query=삼성전자&count=1
-        - https://help.deepsearch.com/ddi/haystack/search
-
-    @category - section: 
-        - news
-            politics, economy, society, culture, world, tech, entertainment, opinion
-        - research
-            market, strategy, company, industry, economy, bond   
-        - company
-            ir, disclosure
-        - patent
-            patent
-    """
-    _COMPUTE_API = "{}/v1".format('https://api.ddi.deepsearch.com/haystack')
-    _AUTH_ID = os.getenv('_AUTH_ID')
-    _AUTH_PW = os.getenv('_AUTH_PW')
-    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
-
-    @classmethod
-    async def compute(cls, category, section, params, locale='ko_KR'):
-        assert type(params) is dict
-        url = os.path.join(cls._COMPUTE_API, category, section, '_search?')
-        async with aiohttp.ClientSession() as sess:
-            async with sess.get( url=url, auth=aiohttp.BasicAuth(cls._AUTH_ID, cls._AUTH_PW), params=params, timeout=120 ) as co_resp:
-                response_json = await co_resp.json()
-                if (co_resp.status != 200):# or (not response_json['found']):
-                    print("Response code, Success status:", co_resp.status)#, response_json['found'])
-                    print("Exception query log:", co_resp.url)
-                    print(response_json)
-                    return None
-        return response_json['data']
-
-
-
-class backtest(object):
-    _aum = 100_000_000_000.0
-    deepsearch = DeepSearchAPI()
-    async_deepsearch = asyncDeepSearchAPI()
-    wavelet = WaveletAPI()
-    
-    loop = asyncio.get_event_loop()
-    fdr_krx = fdr.StockListing('KRX')
-    fdr_krx_delisted = fdr.StockListing('KRX-DELISTING')
-
-    def _split_phases(cls, deepsearch_df:pd.DataFrame) -> dict:
-        return_dict = dict()
-        phases = deepsearch_df.index.unique()
-        for p in phases:
-            pdf = deepsearch_df.loc[p]
-            return_dict[p] = pdf
-        return return_dict
-
-    def _is_business_day(date) -> bool:
-        return bool(len(pd.bdate_range(date, date)))
-
-    def _datetime_reformer(date:str) -> datetime:
-        formats = [
-            "%Y-%m-%d", 
-            "%m/%d/%Y",
-        ]
-        checked = False
-        for i in formats:
-            try: _datetime = datetime.strptime(date, i)
-            except: _datetime = date
-            checked = True
-        if not checked:
-            print("Date format is not valid. Check the date format.")
-            print("Date format should be one of the following:")
-            print(formats)
-            print("Your date format is:")
-            print(date)
-        return _datetime  #! formats 에 없는 형식일 경우 에러 : "%Y-%m-%d", "%m/%d/%Y"
-
-    @classmethod
-    async def _async_main(cls, symbol_list, date_from, date_to, krx=True) -> list or None:
-        start = "'"
-        separator = "', '"
-        query = f"GetStockPrices(([{start + separator.join(symbol_list) + start}]), columns=['change_rate'], date_from={date_from}, date_to={date_to})"
-        task = [cls.async_deepsearch.compute(query)]
-        result = await asyncio.gather(*task)
-        return result
-        """
-        if krx:
-            if "NICE" in [i.split(":")[0] for i in symbol_list]:
-                query = ' '.join(symbol_list) + f' {date_from}-{date_to} 주가'  #! 주가수익률은 해당말일을 기준으로 한 점만 보여준다
-            else:
-            # print(query)
-                start = "'"
-                separator = "', '"
-                query = f"GetStockPrices(([{start + separator.join(symbol_list) + start}]), columns=['close'], date_from={date_from}, date_to={date_to})"
-            # query = ' '.join(symbol_list) + f' {date_from}-{date_to} 주가'  #! 주가수익률 계산 오류 있음. 상폐종목 나이스 티커 필요. 
-            # start = "'"
-            # separator = "', '"
-            # query = f'GetStockPrices(([{start + separator.join(symbol_list) + start}]), columns=["close"], date_from={date_from}, date_to={date_to})'
-        else:
-            start = "'"
-            separator = "', '"
-            query = f'Global.GetStockPrices(([{start + separator.join(symbol_list) + start}]), columns=["close"], date_from={date_from}, date_to={date_to})'
-        task = [cls.async_deepsearch.compute(query)]
-        result = await asyncio.gather(*task)
-        return result
-        """
-
-    def _async_main_wrapper(cls, chunk_krx, chunk_krx_not, _date_from, _date_to, krx=True):
-        async_data_krx = cls.loop.run_until_complete( cls._async_main( [i for i in chunk_krx], _date_from, _date_to ) )
-        if len(chunk_krx_not) > 0:
-            async_data_krx_not = cls.loop.run_until_complete( cls._async_main( [i for i in chunk_krx_not], _date_from, _date_to, krx=False) )
-            async_data_krx_not = [ cls._nonkrx_handler(async_data_krx_not[0], _date_from, _date_to) ]
-            async_data = [ pd.concat([async_data_krx[0], async_data_krx_not[0]]) ]
-        else:
-            async_data = async_data_krx
-        return async_data
-
-
-    @classmethod
-    def _nonkrx_handler(cls, async_data_krx_not_df, _date_from, _date_to) -> pd.DataFrame:
-        won_dollar = cls.deepsearch.compute('QueryBankOfKoreaSeriesData("BOK:731Y001.0000001")')
-        async_data_krx_not = async_data_krx_not_df.rename({'close':f'주가 {_date_from}-{_date_to}'}, axis=1)
-        wd_stockprice = pd.merge(async_data_krx_not.reset_index(), won_dollar.reset_index()).set_index(['date', 'symbol'])
-        wd_stockprice[f'주가 {_date_from}-{_date_to}'] = wd_stockprice.loc[:, f'주가 {_date_from}-{_date_to}'] * wd_stockprice.loc[:, 'QueryBankOfKoreaSeriesData(BOK:731Y001.0000001)']
-        async_data_krx_not[f'주가 {_date_from}-{_date_to}'] = wd_stockprice[f'주가 {_date_from}-{_date_to}']
-        return async_data_krx_not
-
-
-    @classmethod
-    def _fdr_handler(cls, symbol, _date_from, _date_to) -> pd.DataFrame:
-        if "KRX:" in symbol: symbol = symbol.split(":")[-1]
-        if "NICE:" in symbol: symbol = symbol.split(":")[-1]
-        _resp = fdr.DataReader(symbol,_date_from,_date_to)
-        if symbol in list(cls.fdr_krx["Symbol"]): 
-            _entity_name = cls.fdr_krx[cls.fdr_krx["Symbol"] == symbol]["Name"].values[0]
-        else: 
-            _entity_name = cls.fdr_krx_delisted[cls.fdr_krx_delisted["Symbol"] == symbol]["Name"].values[0]
-        _resp["symbol"] = "KRX:"+symbol
-        _resp["entity_name"] = _entity_name
-        _resp = _resp.reset_index()[["Date", "symbol", "entity_name", "Close"]].sort_values(by=["Date"])
-        _resp.columns = ["date", "symbol", "entity_name", f"주가 {_date_from}-{_date_to}"]
-        _resp = _resp.set_index(["date", "symbol"])
-        return _resp
-        """
-        _date_from, _date_to = str(_date_from), str(_date_to)
-        if "KRX:" in symbol: symbol = symbol.split(":")[-1]
-        if "NICE:" in symbol: symbol = symbol.split(":")[-1]
-        _resp = fdr.DataReader(symbol,_date_from,_date_to)
-        if symbol in list(cls.fdr_krx["Symbol"]): 
-            _entity_name = cls.fdr_krx[cls.fdr_krx["Symbol"] == symbol]["Name"].values[0]
-        else: 
-            _entity_name = cls.fdr_krx_delisted[cls.fdr_krx_delisted["Symbol"] == symbol]["Name"].values[0]
-        _resp["symbol"] = "KRX:"+symbol
-        _resp["entity_name"] = _entity_name
-        _resp = _resp.reset_index()[["Date", "symbol", "entity_name", "Close"]].sort_values(by=["Date"])
-        _resp.columns = ["date", "symbol", "entity_name", f"주가 {_date_from}-{_date_to}"]
-        _resp = _resp.set_index(["date", "symbol"])
-        return _resp
-        """
-
-
-    @classmethod
-    def _pdr_naver_handler(cls, chunk_krx, ticker_name_df, _date_from, _date_to) -> list:
-        """
-        _date_from 은 change_rate 과 호환되어야 한다. 
-        """
-        # 220630 맘스터치 상폐 / 007460 무증
-        resp_basket = pd.DataFrame()
-        for idx, ticker in enumerate(chunk_krx):
-            _ticker = ticker.replace("KRX:", "")
-            _resp = pdr.DataReader(_ticker, "naver", start=(pd.to_datetime(_date_from) -relativedelta(months=1)).strftime("%Y-%m-%d"), end=_date_to)[["Open", "High", "Low", "Close", "Volume"]]
-            _resp = _resp.rename(columns={'Open': 'open', 'High': 'high', 'Low': 'low', 'Close': 'close', 'Volume': 'volume'}).reset_index()
-            _resp['entity_name'] = ticker_name_df.loc["KRX:"+_ticker].values[-1][0]
-            _resp['symbol'] = "KRX:"+_ticker
-            _resp['date'] = _resp['Date']
-            _resp["change_rate"] = _resp["close"].astype(float).pct_change()
-            _resp = _resp[["date", "symbol", "entity_name", "change_rate"]]
-
-            date_for_change_rate = ((_resp["date"] < pd.to_datetime(_date_from))).replace(False, np.nan).dropna()
-            if len(date_for_change_rate) == 0: pass  # _start 이전 데이터가 없는 경우
-            else:
-                _resp = _resp.iloc[date_for_change_rate.index[-1] +1:]
-            resp_basket = pd.concat([resp_basket, _resp], axis=0)
-        async_data = [resp_basket.sort_values(["date", "symbol"]).set_index(["date", "symbol"])]
-        return async_data
-
-
-    @classmethod
-    def compute(cls, deepsearch_df, df_to_upload_bool=False, debug=False, fdr=False, naver=False):
-        
-        if naver:
-            ticker_name_dict = dict()
-            ticker_nice_dict = dict()
-            ticker_name_df = deepsearch_df.reset_index()[["symbol_listed", "entity_name"]].drop_duplicates().set_index("symbol_listed")
-            ticker_nice_df = deepsearch_df.reset_index()[["symbol_listed", "symbol"]].drop_duplicates().set_index("symbol_listed")
-
-
-        df = cls._split_phases(cls, deepsearch_df)
-        rebalancing_dates = list(df.keys())
-        for idx, date in enumerate(rebalancing_dates):
-            if datetime.today() < cls._datetime_reformer(date):
-                print(rebalancing_dates, rebalancing_dates[:idx])
-                rebalancing_dates = rebalancing_dates[:idx]
-                break
-        """ 종가매수 """
-        if (rebalancing_dates[-1] == datetime.today().strftime("%m/%d/%Y")): 
-            rebalancing_dates = rebalancing_dates[:-1]
-
-
-        _async_batch_size = 10
-
-        cls._aum = 100_000_000_000.0  #! 변수 초기화
-
-        total_return = pd.DataFrame()
-        for idx, date in enumerate(rebalancing_dates):  # idx starts from 0
-            async_result = pd.DataFrame()
-            if isinstance(df[date], pd.Series): _df = pd.DataFrame(df[date]).T
-            else: _df = df[date]
-            ratio = _df.reset_index().set_index(['symbol'])['weight'].astype(float)  # 단축코드, 비중(비중의합은1)
-            ratio.index = ratio.index.str.replace(" ", "")
-            pdf = list(_df['symbol'])  # 0 은 iter item (timestamp)
-
-            if naver: pdf = list(_df["symbol_listed"])
-
-            delisted_firm_dict = dict()
-            delisted_firm = _df[_df['symbol'] != _df['symbol_listed']]
-            for _, row in delisted_firm.iterrows(): delisted_firm_dict[row['symbol_listed']] = row['symbol']
-
-            date = cls._datetime_reformer(date)
-
-            b_days = 0
-            while True:
-                if not cls._is_business_day(date): date, b_days = date +relativedelta(days=1), b_days +1
-                else: break
-
-
-            if idx+1 != len(rebalancing_dates):  #* if not the last phase
-                # _date_from = datetime.strftime(date -relativedelta(days=1), "%Y-%m-%d")
-                _date_from_for_close_column = datetime.strftime(date -relativedelta(days=1), "%Y-%m-%d")  # close 기반 하루전날 데이터
-                _date_from = datetime.strftime(date, "%Y-%m-%d")  # change_rate 기반 당일 데이터
-                _date_to_for_close_column = datetime.strftime(cls._datetime_reformer(rebalancing_dates[idx+1]) -relativedelta(days=1), "%Y-%m-%d")  # 리밸런싱 전날
-                _date_to = datetime.strftime(cls._datetime_reformer(rebalancing_dates[idx+1]), "%Y-%m-%d")  # 리밸런싱 당일 종가가 수익률에 포함됨
-                
-                _async_data_fdr = pd.DataFrame()
-
-                for i in range(len(pdf)//_async_batch_size +1):
-                    chunk_start, chunk_end = i*_async_batch_size, (i+1)*_async_batch_size
-            
-                    chunk = pdf[chunk_start:chunk_end]
-                    chunk_krx = [i for i in chunk if (i.startswith('KRX:') | i.startswith('NICE:'))]  # ['KRX:007070', 'KRX:023530', 'KRX:139480', 'KRX:097950']
-                    chunk_krx_not = list(set(chunk) - set(chunk_krx))
-
-                    if len(chunk) != len(chunk_krx):
-                        print(chunk)
-                        print(chunk_krx)
-                        import pdb
-                        pdb.set_trace()
-
-                    if len(chunk) == 0: break
-                    if naver:
-                        async_data = []
-                        try: _async_data = cls._pdr_naver_handler(cls, chunk_krx, ticker_name_df, _date_from, _date_to)
-                        except: _async_data = cls._pdr_naver_handler(chunk_krx, ticker_name_df, _date_from, _date_to)
-                        async_data = async_data +_async_data
-                    else:   
-                        try: async_data = cls._async_main_wrapper( chunk_krx, chunk_krx_not, _date_from, _date_to)
-                        except: async_data = cls._async_main_wrapper(cls, chunk_krx, chunk_krx_not, _date_from, _date_to)
-
-
-                    for data in async_data: 
-                        # data.columns = ['entity_name', 'close']  #! 데이터가 안받아져 왔을 시 죽는다
-                        data.columns = ['entity_name', 'change_rate']  #! 데이터가 안받아져 왔을 시 죽는다
-                        async_result = pd.concat([async_result, data], axis=0)
-
-                '''
-                for i in range(len(pdf)//_async_batch_size +1):
-                    chunk_start, chunk_end = i*_async_batch_size, (i+1)*_async_batch_size
-            
-                    chunk = pdf[chunk_start:chunk_end]
-                    chunk_krx = [i for i in chunk if (i.startswith('KRX:') | i.startswith('NICE:'))]
-                    chunk_krx_not = list(set(chunk) - set(chunk_krx))
-
-                    # chunk_krx = chunk_krx[chunk_start:chunk_end]
-                    # chunk_krx_not = chunk_krx_not[chunk_start:chunk_end]
-
-
-                    if len(chunk) == 0: break
-                    #! 왜 다른가?
-                    """try: 
-                        async_data_krx = loop.run_until_complete( cls._async_main( cls, [i for i in chunk_krx], _date_from, _date_to ) )
-                        if len(chunk_krx_not) > 0:
-                            async_data_krx_not = loop.run_until_complete( cls._async_main( cls, [i for i in chunk_krx_not], _date_from, _date_to, krx=False) )
-                            async_data_krx_not = [ cls._nonkrx_handler(async_data_krx_not[0], _date_from, _date_to) ]
-                            async_data = [ pd.concat([async_data_krx[0], async_data_krx_not[0]]) ]
-                        else:
-                            async_data = async_data_krx
-                    except: 
-                        async_data_krx = loop.run_until_complete( cls._async_main( [i for i in chunk_krx], _date_from, _date_to ) )
-                        if len(chunk_krx_not) > 0:
-                            async_data_krx_not = loop.run_until_complete( cls._async_main( [i for i in chunk_krx_not], _date_from, _date_to, krx=False) )
-                            async_data_krx_not = [ cls._nonkrx_handler(async_data_krx_not[0], _date_from, _date_to) ]
-                            async_data = [ pd.concat([async_data_krx[0], async_data_krx_not[0]]) ]
-                        else:
-                            async_data = async_data_krx"""
-                    # if (datetime.strptime(_date_from, "%Y-%m-%d") < datetime(2022, 9, 28)) & (datetime(2022, 9, 28) < datetime.strptime(_date_to, "%Y-%m-%d")):
-                    #     for symbol in chunk_krx:
-                    #         try:
-                    #             _async_resp = cls._fdr_handler( symbol, _date_from, _date_to)
-                    #         except:
-                    #             _async_resp = cls._fdr_handler(cls, symbol, _date_from, _date_to)
-                    #         _async_data_fdr = pd.concat([_async_data_fdr, _async_resp]).sort_index()
-                    #     async_data = [_async_data_fdr]
-                    # else:  # 문제의 기간이 없다면
-                    try: 
-                        async_data = cls._async_main_wrapper( chunk_krx, chunk_krx_not, _date_from, _date_to)
-                    except:
-                        async_data = cls._async_main_wrapper(cls, chunk_krx, chunk_krx_not, _date_from, _date_to)
-
-
-                    for data in async_data: 
-                        data.columns = ['entity_name', 'close']  #! 데이터가 안받아져 왔을 시 죽는다
-                        async_result = pd.concat([async_result, data], axis=0)
-                '''
-            else:  #* if the last phase
-                _date_from_for_close_column = datetime.strftime(date -relativedelta(days=1), "%Y-%m-%d")  # close 기반 하루전날 데이터 
-                _date_from = datetime.strftime(date, "%Y-%m-%d")  # change_rate 기반 당일 데이터
-                _date_to = datetime.strftime(datetime.today().date(), "%Y-%m-%d")
-
-
-
-                for i in range(len(pdf)//_async_batch_size +1):
-                    chunk_start, chunk_end = i*_async_batch_size, (i+1)*_async_batch_size
-                    
-                    chunk = pdf[chunk_start:chunk_end]
-                    chunk_krx = [i for i in chunk if (i.startswith('KRX:') | i.startswith('NICE:'))]
-                    chunk_krx_not = set(chunk) - set(chunk_krx)
-
-                    if len(chunk) != len(chunk_krx):
-                        print(chunk)
-                        print(chunk_krx)
-
-                    if len(chunk) == 0: break
-                    if naver:
-                        async_data = []
-                        try: _async_data = cls._pdr_naver_handler(cls, chunk_krx, ticker_name_df, _date_from, _date_to)
-                        except: _async_data = cls._pdr_naver_handler(chunk_krx, ticker_name_df, _date_from, _date_to)
-                        async_data = async_data +_async_data
-                    else:   
-                        try: async_data = cls._async_main_wrapper(cls, chunk_krx, chunk_krx_not, _date_from, _date_to)
-                        except: async_data = cls._async_main_wrapper( chunk_krx, chunk_krx_not, _date_from, _date_to)
-
-
-                    for data in async_data:
-                        # data.columns = ['entity_name', 'close']
-                        data.columns = ['entity_name', 'change_rate']  #! 데이터가 안받아져 왔을 시 죽는다
-                        async_result = pd.concat([async_result, data], axis=0)
-                
-            async_result_reset = async_result.reset_index()
-
-            
-            #####################################################################################################################
-            #* close
-            # pdf_returns_ds = async_result_reset.drop_duplicates(subset=['date', 'symbol'], keep='first').pivot(index='date', columns='symbol', values='close').ffill()
-            # pdf_returns_async = (pdf_returns_ds.pct_change().fillna(0) +1).cumprod()  #! NICE가 없다
-
-            #* change_rate
-            pdf_returns_ds = async_result_reset.drop_duplicates(subset=['date', 'symbol'], keep='first').pivot(index='date', columns='symbol', values='change_rate').ffill()
-            pdf_returns_async = (pdf_returns_ds +1).cumprod()
-            #####################################################################################################################
-            
-            # pdf_returns_ds.iloc[0, :] = 0  #* 주가수익률로 계산했을 시기의 코드 
-            # pdf_returns_async = (pdf_returns_ds +1).cumprod()  #* 주가수익률로 계산했을 시기의 코드 
-            pdf_returns_async.columns = [ delisted_firm_dict[i] if i in delisted_firm_dict.keys() else i for i in pdf_returns_async.columns ]
-
-            inherited_budget = ratio * cls._aum  # 시작분배금  #! NICE가 있다 / ratio는 가장 최근의 리밸비중 / 여기서의 cls._aum 은 다음 값으로 업데이트 되기 전임
-            #* 시작일은 base_point를 남기고 그 이후부터는 첫날의 리밸런싱 무수익을 떨군다
-            
-            inherited_budget.index = inherited_budget.index.astype(str)
-            pdf_returns_async.columns = pdf_returns_async.columns.astype(str)
-            if idx > 0: 
-                _aum_change_async = pdf_returns_async[datetime.strptime(_date_from, "%Y-%m-%d").date() +relativedelta(days=1):] *inherited_budget
-            else: 
-                _aum_change_async = pdf_returns_async *inherited_budget
-
-            cls._aum = _aum_change_async.sum(axis=1)[-1]
-            total_return = pd.concat([total_return, _aum_change_async])
-            print(cls._aum)
-
-
-        if debug == True:
-            import pdb
-            pdb.set_trace()
-
-        total_return = total_return.groupby(total_return.index).first()
-
-        if df_to_upload_bool:
-            total_return = total_return.groupby(total_return.index).first()
-            base_point = 1000
-            daily_aum = total_return.sum(axis=1)
-            daily_aum.index = pd.to_datetime(daily_aum.index)
-            index_calc_start_date = cls._datetime_reformer(rebalancing_dates[0])
-
-            """
-            //2023-01-19//
-            close 기반 기존의 계산 -> 시가매수
-            change_rate 기반 계산 -> 종가매수 
-            """
-            import copy
-            daily_aum_for_change_rate = copy.deepcopy(daily_aum)
-            daily_aum_for_change_rate = dict(daily_aum_for_change_rate)
-            daily_aum_for_change_rate[index_calc_start_date] = 100_000_000_000
-            daily_aum_for_change_rate = pd.Series(daily_aum_for_change_rate).sort_index()
-
-            daily_aum = daily_aum_for_change_rate
-
-            try:
-                daily_idx = daily_aum / daily_aum[datetime.strftime(index_calc_start_date, "%Y-%m-%d")] *base_point
-            except:
-                print(f'error check [{rebalancing_dates[0]}] - date index not exists, call the most recent previous date')
-                daily_idx = daily_aum / daily_aum[:datetime.strftime(index_calc_start_date, "%Y-%m-%d")].iloc[-1] *base_point
-            daily_idx = daily_idx[datetime.strftime(index_calc_start_date, "%Y-%m-%d"):]
-
-
-            resp = pdr.DataReader("KOSPI", "naver", start=datetime.strftime(index_calc_start_date, '%Y-%m-%d'), end=datetime.strftime(datetime.today().date(), '%Y-%m-%d'))[["Open", "High", "Low", "Close", "Volume"]]
-            resp = resp.astype(float)
-            resp["symbol"] = "KRX:KOSPI"
-            resp["entity_name"] = "코스피"
-            resp = resp.reset_index()[["Date", "symbol", "entity_name", "Close"]].sort_values(by=["Date"])
-            resp.columns = ["date", "symbol", "entity_name", f"주가 {datetime.strftime(index_calc_start_date, '%Y-%m-%d')}-{datetime.strftime(datetime.today().date(), '%Y-%m-%d')}"]
-            resp = resp.set_index(["date", "symbol"])
-            kospi = resp.reset_index().set_index('date')
-            kospi.columns = ['symbol', 'entity_name', 'close']
-            kospi.index = pd.to_datetime(kospi.index).date
-
-            #! 한국주식과 미국주식을 섞으면 공휴일이 다르다 
-            _excel_date_format = "%Y-%m-%d"
-            try:
-                daily_idx_date_reviewed = daily_idx.loc[kospi.index]
-            except:
-                daily_idx.index = pd.to_datetime(daily_idx.index).date
-                daily_idx_date_reviewed = daily_idx
-            
-            df_to_upload = pd.concat([daily_idx_date_reviewed, kospi["close"]], axis=1).sort_index(ascending=True).bfill()
-            df_to_upload.columns = ['index', 'KOSPI']
-            df_to_upload.index = pd.to_datetime(df_to_upload.index, format="%Y-%m-%d")
-            df_to_upload.index = df_to_upload.index.strftime(_excel_date_format)
-            df_to_upload = df_to_upload.reset_index()
-            df_to_upload.columns = ['date', 'index', 'KOSPI']
-
-            df_to_upload["index"] = df_to_upload["index"] / df_to_upload["index"].iloc[0] * base_point
-            df_to_upload["KOSPI"] = df_to_upload["KOSPI"] / df_to_upload["KOSPI"].iloc[0] * base_point
-
-
-            df_to_upload['date'] = df_to_upload['date'].astype(str)
-
-            return df_to_upload
-        return total_return
-
-
-
-
-class _backtest(object):
-    _aum = 100_000_000_000.0
-    deepsearch = DeepSearchAPI()
-    async_deepsearch = asyncDeepSearchAPI()
-    wavelet = WaveletAPI()
-
-    def _split_phases(cls, deepsearch_df):
-        return_dict = dict()
-        phases = deepsearch_df.index.unique()
-        for p in phases:
-            pdf = deepsearch_df.loc[p]
-            return_dict[p] = pdf
-        return return_dict
-
-    def _is_business_day(date):
-        return bool(len(pd.bdate_range(date, date)))
-
-    @classmethod
-    async def _async_main(cls, symbol_list, date_from, date_to):
-        query = ' '.join(symbol_list) + f' {date_from}-{date_to} 주가'  #! 주가수익률은 해당말일을 기준으로 한 점만 보여준다
-        task = [cls.async_deepsearch.compute(query)]
-        result = await asyncio.gather(*task)
-        return result
-
-    @classmethod
-    def compute(cls, deepsearch_df, df_to_upload_bool=False, debug=False):
-        df = cls._split_phases(cls, deepsearch_df)
-        rebalancing_dates = list(df.keys())
-        for idx, date in enumerate(rebalancing_dates):
-            if datetime.today() < (datetime.strptime(date, "%m/%d/%Y")):
-                print(rebalancing_dates, rebalancing_dates[:idx])
-                rebalancing_dates = rebalancing_dates[:idx]
-                break
-
-
-
-        loop = asyncio.get_event_loop()
-        _async_batch_size = 10
-
-
-        total_return = pd.DataFrame()
-        for idx, date in enumerate(rebalancing_dates):  # idx starts from 0
-            async_result = pd.DataFrame()
-            if isinstance(df[date], pd.Series): _df = pd.DataFrame(df[date]).T
-            else: _df = df[date]
-            ratio = _df.reset_index().set_index(['symbol'])['weight'].astype(float)  # 단축코드, 비중(비중의합은1)
-            ratio.index = ratio.index.str.replace(" ", "")
-            pdf = list(_df['symbol'])  # 0 은 iter item (timestamp)
-
-            delisted_firm_dict = dict()
-            delisted_firm = _df[_df['symbol'] != _df['symbol_listed']]
-            for _, row in delisted_firm.iterrows(): delisted_firm_dict[row['symbol_listed']] = row['symbol']
-
-            date = datetime.strptime(date, "%m/%d/%Y")
-
-            b_days = 0
-            while True:
-                if not cls._is_business_day(date): date, b_days = date +relativedelta(days=1), b_days +1
-                else: break
-
-
-            if idx+1 != len(rebalancing_dates):  #* if not the last phase
-                _date_from = datetime.strftime(date -relativedelta(days=1), "%Y-%m-%d")
-                _date_to = datetime.strftime(datetime.strptime(rebalancing_dates[idx+1], "%m/%d/%Y") -relativedelta(days=1), "%Y-%m-%d")
-
-                for i in range(len(pdf)//_async_batch_size +1):
-                    chunk_start, chunk_end = i*_async_batch_size, (i+1)*_async_batch_size
-                    chunk = pdf[chunk_start:chunk_end]
-                    if len(chunk) == 0: break
-                    #! 왜 다른가?
-                    try: async_data = loop.run_until_complete( cls._async_main( cls, [i for i in chunk], _date_from, _date_to ) )
-                    except: async_data = loop.run_until_complete( cls._async_main( [i for i in chunk], _date_from, _date_to ) )
-                    for data in async_data: 
-                        data.columns = ['entity_name', 'close']  #! 데이터가 안받아져 왔을 시 죽는다
-                        async_result = pd.concat([async_result, data], axis=0)
-            else:  #* if the last phase
-                _date_from = datetime.strftime(date -relativedelta(days=1), "%Y-%m-%d")
-                _date_to = datetime.strftime(datetime.today().date(), "%Y-%m-%d")
-
-                for i in range(len(pdf)//_async_batch_size +1):
-                    chunk_start, chunk_end = i*_async_batch_size, (i+1)*_async_batch_size
-                    chunk = pdf[chunk_start:chunk_end]
-                    if len(chunk) == 0: break
-                    #! 왜 다른가?
-                    try: async_data = loop.run_until_complete( cls._async_main( cls, [i for i in chunk], _date_from, _date_to) )  # datetime.strftime(datetime.today(), "%Y-%m-%d")
-                    except: async_data = loop.run_until_complete( cls._async_main( [i for i in chunk], _date_from, _date_to) )  # datetime.strftime(datetime.today(), "%Y-%m-%d")
-                    for data in async_data:
-                        data.columns = ['entity_name', 'close']
-                        async_result = pd.concat([async_result, data], axis=0)
-
-            async_result_reset = async_result.reset_index()
-            pdf_returns_ds = async_result_reset.drop_duplicates(subset=['date', 'symbol'], keep='first').pivot(index='date', columns='symbol', values='close')
-            pdf_returns_async = (pdf_returns_ds.pct_change().fillna(0) +1).cumprod()  #! NICE가 없다
-            # pdf_returns_ds.iloc[0, :] = 0  #* 주가수익률로 계산했을 시기의 코드 
-            # pdf_returns_async = (pdf_returns_ds +1).cumprod()  #* 주가수익률로 계산했을 시기의 코드 
-            pdf_returns_async.columns = [ delisted_firm_dict[i] if i in delisted_firm_dict.keys() else i for i in pdf_returns_async.columns ]
-
-            inherited_budget = ratio * cls._aum  # 시작분배금  #! NICE가 있다 / ratio는 가장 최근의 리밸비중 / 여기서의 cls._aum 은 다음 값으로 업데이트 되기 전임
-            #* 시작일은 base_point를 남기고 그 이후부터는 첫날의 리밸런싱 무수익을 떨군다
-
-            try: _prev_aum_change_async = _aum_change_async
-            except: pass
-            inherited_budget.index = inherited_budget.index.astype(str)
-            pdf_returns_async.columns = pdf_returns_async.columns.astype(str)
-            if idx > 0: 
-                _aum_change_async = pdf_returns_async[datetime.strptime(_date_from, "%Y-%m-%d").date() +relativedelta(days=1):] *inherited_budget
-            else: _aum_change_async = pdf_returns_async *inherited_budget
-
-            cls._aum = _aum_change_async.sum(axis=1)[-1]
-            total_return = pd.concat([total_return, _aum_change_async])
-            print(cls._aum)
-
-            # total_return = pd.concat([total_return, _aum_change_wavelet])
-
-        if debug == True:
-            import pdb
-            pdb.set_trace()
-
-        total_return = total_return.groupby(total_return.index).first()
-
-        cls._aum = 100_000_000_000.0  #! 변수 초기화
-
-        if df_to_upload_bool:
-            total_return = total_return.groupby(total_return.index).first()
-            base_point = 1000
-            daily_aum = total_return.sum(axis=1)
-            try:
-                daily_idx = daily_aum / daily_aum[datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), "%Y-%m-%d")] *base_point
-            except:
-                print(f'error check [{rebalancing_dates[0]}] - date index not exists, call the most recent previous date')
-                daily_idx = daily_aum / daily_aum[:datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), "%Y-%m-%d")].iloc[-1] *base_point
-            daily_idx = daily_idx[datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), "%Y-%m-%d"):]
-            
-            """
-            daily_aum.index = pd.to_datetime(daily_aum.index)
-            daily_idx = daily_aum / daily_aum[datetime.strftime(datetime.strptime(rebalancing_dates[0], "%m/%d/%Y"), "%Y-%m-%d")] *base_point
-            daily_idx = daily_idx[datetime.strftime(datetime.strptime(rebalancing_dates[0], "%m/%d/%Y"), "%Y-%m-%d"):]
-            # daily_idx.index = daily_idx.index.date
-            """
-
-            #* rebalancing_dates[0] 은 해당일 종가매수를 의미한다.
-            #* 즉, 월요일부터의 수익률을 보고싶은 경우, 리밸런싱 날짜는 월요일이 아닌 직전 거래일(금요일)을 넣어야 한다.
-            _query_kospi = f"코스피 지수 {datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), '%Y-%m-%d')}-{datetime.strftime(datetime.today().date(), '%Y-%m-%d')}"
-            resp = cls.deepsearch.compute(_query_kospi).reset_index().set_index('date')
-            resp.columns = ['close' if '지수' in i else i for i in resp.columns]
-            kospi = resp
-
-            # import FinanceDataReader as fdr
-            # from pandas_datareader import data 
-            # resp = data.DataReader("KOSPI", "naver", start=datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), '%Y-%m-%d'), end=datetime.strftime(datetime.today().date(), '%Y-%m-%d'))[["Open", "High", "Low", "Close", "Volume"]]
-            # resp = resp.astype(float)
-            # resp["symbol"] = "KRX:KOSPI"
-            # resp["entity_name"] = "코스피"
-            # resp = resp.reset_index()[["Date", "symbol", "entity_name", "Close"]].sort_values(by=["Date"])
-            # resp.columns = ["date", "symbol", "entity_name", f"주가 {datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), '%Y-%m-%d')}-{datetime.strftime(datetime.today().date(), '%Y-%m-%d')}"]
-            # resp = resp.set_index(["date", "symbol"])
-            # kospi = resp.reset_index().set_index('date')
-            # kospi.columns = ['symbol', 'entity_name', 'close']
-            # kospi.index = pd.to_datetime(kospi.index).date
-
-            #! 한국주식과 미국주식을 섞으면 공휴일이 다르다 
-            try:
-                daily_idx_date_reviewed = daily_idx.loc[kospi.index]
-            except:
-                import pdb
-                pdb.set_trace()
-            # kospi_ret = kospi['close'].loc[daily_idx.index].pct_change()  # 당일의 종가수익률이 아니라 판다스에서 추가적으로 계산된 값이므로 첫날의 수익률은 누락 #! 그런데 첫날이 월요일이면 -1day때문에 길이가 안맞는다
-            kospi_ret = kospi['close'].pct_change()
-
-            daily_kospi = (kospi_ret+1).cumprod().fillna(1) *base_point  #* 엑셀 holdings 파일의 date 는 종가매수의 기준일이므로, 날짜를 월요일로 잡아도 월요일 종가매수를 의미한다. 
-            # daily_kospi.index = daily_kospi.index.date
-            #업로드용 파일 가공
-            _excel_date_format = "%Y-%m-%d"
-            # df_to_upload = pd.concat([daily_idx, daily_kospi], axis=1)
-            df_to_upload = pd.concat([daily_idx_date_reviewed, daily_kospi], axis=1)
-            df_to_upload.columns = ['index', 'KOSPI']
-            df_to_upload.index = pd.to_datetime(df_to_upload.index, format="%Y-%m-%d")
-            df_to_upload.index = df_to_upload.index.strftime(_excel_date_format)
-            df_to_upload = df_to_upload.reset_index()
-            df_to_upload.columns = ['date', 'index', 'KOSPI']
-            df_to_upload['date'] = df_to_upload['date'].astype(str)
-
-            """
-            _excel_date_format = "%d/%m/%Y"
-            df_to_upload = pd.concat([daily_idx, daily_kospi], axis=1)
-            df_to_upload.columns = ['index', 'KOSPI']
-            df_to_upload.index = pd.to_datetime(df_to_upload.index, format="%Y-%m-%d")
-            df_to_upload.index = df_to_upload.index.strftime(_excel_date_format)
-            df_to_upload = df_to_upload.reset_index()
-            """
-
-            return df_to_upload
-        return total_return
+import requests
+from datetime import datetime
+import time
+import os
+import asyncio
+import aiohttp
+import FinanceDataReader as fdr
+from pandas_datareader import data as pdr
+
+import pandas as pd
+import numpy as np
+
+from dotenv import load_dotenv
+from requests.auth import HTTPBasicAuth
+
+from dateutil.relativedelta import relativedelta
+
+load_dotenv(verbose=True)
+
+
+class asyncDeepSearchAPI(object):
+    _COMPUTE_API = "{}/v1/compute".format('https://api.deepsearch.com')
+    _AUTH_ID = os.getenv('_AUTH_ID')
+    _AUTH_PW = os.getenv('_AUTH_PW')
+    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
+    
+    @classmethod
+    async def compute(cls, query, locale='ko_KR'):
+        params = {
+            'input': query,
+            'locale': locale
+        } 
+        _count = 0
+        while True:
+            try:
+                async with aiohttp.ClientSession() as sess:
+
+                    async with sess.post( url=cls._COMPUTE_API, auth=aiohttp.BasicAuth(cls._AUTH_ID, cls._AUTH_PW), data=params, timeout=120 ) as co_resp:
+                        response_json = await co_resp.json()
+                        if (co_resp.status != 200) or (not response_json['success']):
+                            try:
+                                print("Response code, Success status:", co_resp.status, response_json['success'])
+                            except:
+                                print(response_json)
+                            print("Exception query log:", query)
+                            print(response_json)
+                            return None
+
+                        pods = response_json['data']['pods']  # pods[0]: input
+
+                        if pods[1]['class'] == 'Result:DataFrame':
+                            data    =    pods[1]['content']['data']
+                            index   =   pods[1]['content']['index']
+                            dtypes  =  pods[1]['content']['dtypes']
+                            columns = pods[1]['content']['columns']
+
+                            results = []
+
+                            no_obs = len(data[columns[0]])
+                            for i in range(no_obs):
+                                item = dict()
+                                for col in columns:
+                                    item[col] = data[col][i]
+                                results.append(item)
+
+                            df_results = pd.DataFrame(results)
+
+                            if df_results.empty:
+                                return None
+
+                            for col in dtypes.keys():  # pyarrow converting
+                                # df_results[col] = df_results[col].astype(dtypes[col])
+                                
+                                if dtypes[col] == 'datetime64':
+                                    df_results[col] = pd.to_datetime(df_results[col], errors='coerce')
+                                else:
+                                    df_results[col] = df_results[col].astype(dtypes[col])  # pandas 1.5.3 
+
+                            df_results = df_results.set_index(index)  # 'symbol'
+                            df_results = df_results.sort_index()
+
+                            return df_results
+
+                        elif pods[1]['class'] == 'Result:DocumentTrendsResult':
+                            data    =    pods[1]['content']['data']
+                            trends  =   pods[1]['content']['data']['trends']
+                            total_matches = trends[0]['total_matches']
+                            buckets = trends[0]['buckets']
+
+                            df_results = pd.DataFrame(buckets)
+                            
+                            return df_results
+
+                        else:
+                            return pods[1]['content']
+            
+            except Exception as e:
+                print("Exception query log:", query)
+                print(e)
+                _count += 1
+                if _count > 5:
+                    return [None]
+                time.sleep(5)
+                continue
+
+
+
+class asyncDeepSearchAPI_mk2(object):
+    _COMPUTE_API = "{}/v1/compute".format('https://api.deepsearch.com')
+    _AUTH_ID = os.getenv('_AUTH_ID')
+    _AUTH_PW = os.getenv('_AUTH_PW')
+    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
+    
+    @classmethod
+    async def compute(cls, query, locale='ko_KR', timeout=120, max_count=5, sentiment=False, verbose=False):
+        params = {
+            'input': query,
+            'locale': locale
+        } 
+        _count = 0
+        retry = False
+        while True:
+            try:
+                async with aiohttp.ClientSession() as sess:
+
+                    async with sess.post( url=cls._COMPUTE_API, auth=aiohttp.BasicAuth(cls._AUTH_ID, cls._AUTH_PW), data=params, timeout=timeout ) as co_resp:
+                        response_json = await co_resp.json()
+                        if (co_resp.status != 200) or (not response_json['success']):
+                            if verbose:
+                                print("Response code, Success status:", co_resp.status, response_json['success'])
+                            if sentiment:
+                                raise Exception("Response code, Success status:", co_resp.status, response_json['success'])
+                            
+                            raise Exception("Exception query log:", query)
+                            return None, query
+                            return None
+
+                        pods = response_json['data']['pods']  # pods[0]: input
+
+                        if pods[1]['class'] == 'Result:DataFrame':
+                            data    =    pods[1]['content']['data']
+                            index   =   pods[1]['content']['index']
+                            dtypes  =  pods[1]['content']['dtypes']
+                            columns = pods[1]['content']['columns']
+
+                            results = []
+
+                            no_obs = len(data[columns[0]])
+                            for i in range(no_obs):
+                                item = dict()
+                                for col in columns:
+                                    item[col] = data[col][i]
+                                results.append(item)
+
+                            df_results = pd.DataFrame(results)
+
+                            if df_results.empty:
+                                if verbose:
+                                    print("Empty DataFrame:", query)
+                                return None, query
+                                return None
+
+                            for col in dtypes.keys():  # pyarrow converting
+                                # df_results[col] = df_results[col].astype(dtypes[col])
+                                
+                                if dtypes[col] == 'datetime64':
+                                    df_results[col] = pd.to_datetime(df_results[col], errors='coerce')
+                                else:
+                                    df_results[col] = df_results[col].astype(dtypes[col])  # pandas 1.5.3 
+
+                            df_results = df_results.set_index(index)  # 'symbol'
+                            df_results = df_results.sort_index()
+
+                            if verbose:
+                                if retry: print("retry success")
+                            return df_results, query
+                            return df_results
+
+                        elif pods[1]['class'] == 'Result:DocumentTrendsResult':
+                            data    =    pods[1]['content']['data']
+                            trends  =   pods[1]['content']['data']['trends']
+                            total_matches = trends[0]['total_matches']
+                            buckets = trends[0]['buckets']
+
+                            df_results = pd.DataFrame(buckets)
+                            
+                            if verbose:
+                                if retry: print("retry success")
+                            return df_results, query
+                            return df_results
+
+                        else:
+                            if verbose:
+                                if retry: print("retry success")
+                            return pods[1]['content'], query
+                            return pods[1]['content']
+            
+            except Exception as e:
+                retry = True
+                _count += 1
+                if verbose:
+                    print("Exception query log:", query)
+                    print(e)
+                    print(_count)
+                if _count > max_count:
+                    print(f'max count exceeded: {query}')
+                    return [None], query
+                    return [None]
+                time.sleep(5)
+                continue
+
+
+
+
+
+    @classmethod
+    async def compute_legacy(cls, category, section, params, locale='ko_KR'):
+        assert type(params) is dict
+        # url = os.path.join(cls._COMPUTE_API, category, section, '_search?')
+        url = os.path.join('https://api.ddi.deepsearch.com/haystack/v1', category, section, '_search?')
+        async with aiohttp.ClientSession() as sess:
+            async with sess.get( url=url, auth=aiohttp.BasicAuth(cls._AUTH_ID, cls._AUTH_PW), params=params, timeout=120 ) as co_resp:
+                response_json = await co_resp.json()
+                if (co_resp.status != 200):# or (not response_json['found']):
+                    print("Response code, Success status:", co_resp.status)#, response_json['found'])
+                    print("Exception query log:", co_resp.url)
+                    print(response_json)
+                    return None
+        return response_json['data']
+
+
+
+
+class DeepSearchAPI(object):
+    _COMPUTE_API = "{}/v1/compute".format('https://api.deepsearch.com')
+    _AUTH_ID = os.getenv('_AUTH_ID')
+    _AUTH_PW = os.getenv('_AUTH_PW')
+    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
+
+    @classmethod
+    def compute(cls, query, locale='ko_KR', debug=False, timeout=120):
+        params = {
+            'input': query,
+            'locale': locale
+        } 
+
+        response = requests.post( url=cls._COMPUTE_API, auth=cls._AUTH, data=params, timeout=timeout )
+
+        if (response.status_code != 200) or (not response.json()['success']):
+            print("Response code:", response.status_code)
+            print("AUTH info:", cls._AUTH_ID, cls._AUTH_PW)
+            print("Exception query log:", query)
+            if debug:
+                return response
+            return None
+
+        pods = response.json()['data']['pods']  # pods[0]: input
+
+        if pods[1]['class'] == 'Result:DataFrame':
+            data    =    pods[1]['content']['data']
+            index   =   pods[1]['content']['index']
+            dtypes  =  pods[1]['content']['dtypes']
+            columns = pods[1]['content']['columns']
+
+            results = []
+
+            no_obs = len(data[columns[0]])
+            for i in range(no_obs):
+                item = dict()
+                for col in columns:
+                    item[col] = data[col][i]
+                results.append(item)
+
+            df_results = pd.DataFrame(results)
+
+            if df_results.empty:
+                return None
+
+            for col in dtypes.keys():  # pyarrow converting
+                if None in df_results[col].values:
+                    df_results[col] = df_results[col].ffill()
+                
+                if dtypes[col] == 'datetime64':
+                    df_results[col] = pd.to_datetime(df_results[col], errors='coerce')
+                else:
+                    df_results[col] = df_results[col].astype(dtypes[col])  # pandas 1.5.3 
+
+            df_results = df_results.set_index(index)  # 'symbol'
+            df_results = df_results.sort_index()
+
+            return df_results
+
+        elif pods[1]['class'] == 'Result:DocumentTrendsResult':
+            data    =    pods[1]['content']['data']
+            trends  =   pods[1]['content']['data']['trends']
+            total_matches = trends[0]['total_matches']
+            buckets = trends[0]['buckets']
+
+            df_results = pd.DataFrame(buckets)
+            
+            return df_results
+
+        else:
+            return pods[1]['content']
+
+
+class WaveletAPI(object):
+    _COMPUTE_API_INDEX = 'https://api.ddi.deepsearch.com/wavelet/v1/indices' 
+    _COMPUTE_API = 'https://api.ddi.deepsearch.com/wavelet/v1/prices'
+    _AUTH_ID = os.getenv('_AUTH_ID')
+    _AUTH_PW = os.getenv('_AUTH_PW')
+    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
+
+    @classmethod
+    def compute(cls, symbol, date_from, date_to, interval=None):
+        assert type(symbol) == list
+        num_of_pdf = len(symbol)
+        symbol_str = ','.join(symbol)
+        return_dict = dict()
+        
+        if symbol in [['KOSPI'], ['KOSDAQ']]:
+            query = f'{cls._COMPUTE_API_INDEX}/{symbol_str}?from={date_from}&to={date_to}'
+        else:
+            query = f'{cls._COMPUTE_API}/{symbol_str}?from={date_from}&to={date_to}'
+
+        response = requests.get(query, auth=cls._AUTH)
+        
+        if (response.status_code != 200):
+            print("Response code:", response.status_code)
+            print("AUTH info:", cls._AUTH_ID, cls._AUTH_PW)
+            print("Exception query log:", query)
+            return None
+            
+        # print(query)
+
+        if symbol in [['KOSPI'], ['KOSDAQ']]:
+            data = response.json()['data'][0]
+            points = data['points']
+
+            df = pd.DataFrame.from_dict(points)
+            df = df.set_index(['timestamp'])
+            df.index = pd.to_datetime(df.index)
+
+            return_dict[symbol[0]] = df  #! 인덱스 리턴은 하나밖에 못한다가 됨
+            return return_dict
+
+        else:
+            for i in range(num_of_pdf):
+                try:
+                    data = response.json()['data'][i]
+                    points = data['points']
+
+                    df = pd.DataFrame.from_dict(points)
+                    df = df.set_index(['timestamp'])
+                    df.index = pd.to_datetime(df.index)
+
+                    if num_of_pdf == 1:
+                        return_dict[data['exchange'] + ':' + data['symbol']] = df
+                        return return_dict
+                
+                    return_dict[data['exchange'] + ':' + data['symbol']] = df
+                except:  
+                    print("Response code:", response.status_code)
+                    print("Exception query log:", query)
+                    break
+
+            return return_dict
+
+
+class asyncWaveletAPI(object):
+    _COMPUTE_API_INDEX = 'https://api.ddi.deepsearch.com/wavelet/v1/indices' 
+    _COMPUTE_API = 'https://api.ddi.deepsearch.com/wavelet/v1/prices'
+    _AUTH_ID = os.getenv('_AUTH_ID')
+    _AUTH_PW = os.getenv('_AUTH_PW')
+    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
+
+    @classmethod
+    def compute():
+        return
+
+
+class HaystackAPI(object):
+    """
+    api.ddi.deepsearch.com/haystack/v1/news/_search?query=삼성전자&count=1
+        - https://help.deepsearch.com/ddi/haystack/search
+
+    @category - section: 
+        - news
+            politics, economy, society, culture, world, tech, entertainment, opinion
+        - research
+            market, strategy, company, industry, economy, bond   
+        - company
+            ir, disclosure
+        - patent
+            patent
+    """
+    _COMPUTE_API = "{}/v1".format('https://api.ddi.deepsearch.com/haystack')
+    _AUTH_ID = os.getenv('_AUTH_ID')
+    _AUTH_PW = os.getenv('_AUTH_PW')
+    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
+
+    @classmethod
+    def compute(cls, category, section, params, module='_search?', group_by='securities.symbol', locale='ko_KR'):
+        assert type(params) is dict
+        url = os.path.join(cls._COMPUTE_API, category, section, module)
+        if module == '_aggregation?':
+            params['groupby'] = group_by
+        response = requests.get( url=url, auth=cls._AUTH, params=params, timeout=30 )
+
+        if (response.status_code != 200) or (not response.json()['found']):
+            print("Response code, Found status:", response.status_code, response.json()['found'])
+            print("Exception query log:", response.url)
+            return None
+
+        return response.json()['data']
+
+
+class asyncHaystackAPI(object):
+    """
+    api.ddi.deepsearch.com/haystack/v1/news/_search?query=삼성전자&count=1
+        - https://help.deepsearch.com/ddi/haystack/search
+
+    @category - section: 
+        - news
+            politics, economy, society, culture, world, tech, entertainment, opinion
+        - research
+            market, strategy, company, industry, economy, bond   
+        - company
+            ir, disclosure
+        - patent
+            patent
+    """
+    _COMPUTE_API = "{}/v1".format('https://api.ddi.deepsearch.com/haystack')
+    _AUTH_ID = os.getenv('_AUTH_ID')
+    _AUTH_PW = os.getenv('_AUTH_PW')
+    _AUTH = HTTPBasicAuth(_AUTH_ID, _AUTH_PW)
+
+    @classmethod
+    async def compute(cls, category, section, params, locale='ko_KR'):
+        assert type(params) is dict
+        url = os.path.join(cls._COMPUTE_API, category, section, '_search?')
+        async with aiohttp.ClientSession() as sess:
+            async with sess.get( url=url, auth=aiohttp.BasicAuth(cls._AUTH_ID, cls._AUTH_PW), params=params, timeout=120 ) as co_resp:
+                response_json = await co_resp.json()
+                if (co_resp.status != 200):# or (not response_json['found']):
+                    print("Response code, Success status:", co_resp.status)#, response_json['found'])
+                    print("Exception query log:", co_resp.url)
+                    print(response_json)
+                    return None
+        return response_json['data']
+
+
+
+class backtest(object):
+    _aum = 100_000_000_000.0
+    deepsearch = DeepSearchAPI()
+    async_deepsearch = asyncDeepSearchAPI()
+    # wavelet = WaveletAPI()
+    loop = asyncio.get_event_loop()
+    # fdr_krx = fdr.StockListing('KRX')
+    # fdr_krx_delisted = fdr.StockListing('KRX-DELISTING')
+
+    def _split_phases(cls, deepsearch_df:pd.DataFrame) -> dict:
+        return_dict = dict()
+        phases = deepsearch_df.index.unique()
+        for p in phases:
+            pdf = deepsearch_df.loc[p]
+            return_dict[p] = pdf
+        return return_dict
+
+    def _is_business_day(date) -> bool:
+        return bool(len(pd.bdate_range(date, date)))
+
+    def _datetime_reformer(date:str) -> datetime:
+        formats = [
+            "%Y-%m-%d", 
+            "%m/%d/%Y",
+        ]
+        checked = False
+        for i in formats:
+            try: _datetime = datetime.strptime(date, i)
+            except: _datetime = date
+            checked = True
+        if not checked:
+            print("Date format is not valid. Check the date format.")
+            print("Date format should be one of the following:")
+            print(formats)
+            print("Your date format is:")
+            print(date)
+        return _datetime  #! formats 에 없는 형식일 경우 에러 : "%Y-%m-%d", "%m/%d/%Y"
+
+    @classmethod
+    async def _async_main(cls, symbol_list, date_from, date_to, krx=True) -> list or None:
+        start = "'"
+        separator = "', '"
+        query = f"GetStockPrices(([{start + separator.join(symbol_list) + start}]), columns=['change_rate'], date_from={date_from}, date_to={date_to})"
+        # if krx:
+        #     if "NICE" in [i.split(":")[0] for i in symbol_list]:
+        #         query = ' '.join(symbol_list) + f' {date_from}-{date_to} 주가'  #! 주가수익률은 해당말일을 기준으로 한 점만 보여준다
+        #     else:
+        #         start = "'"
+        #         separator = "', '"
+        #         # query = f"GetStockPrices(([{start + separator.join(symbol_list) + start}]), columns=['close'], date_from={date_from}, date_to={date_to})"
+        #         query = f"GetStockPrices(([{start + separator.join(symbol_list) + start}]), columns=['change_rate'], date_from={date_from}, date_to={date_to})"
+        #     # print(query)
+        # else:
+        #     start = "'"
+        #     separator = "', '"
+        #     # query = f'Global.GetStockPrices(([{start + separator.join(symbol_list) + start}]), columns=["close"], date_from={date_from}, date_to={date_to})'
+        #     query = f'Global.GetStockPrices(([{start + separator.join(symbol_list) + start}]), columns=["change_rate"], date_from={date_from}, date_to={date_to})'
+        #     # print(query)
+        task = [cls.async_deepsearch.compute(query)]
+        result = await asyncio.gather(*task)
+        return result
+
+    def _async_main_wrapper(cls, chunk_krx, chunk_krx_not, _date_from, _date_to, krx=True):
+        async_data_krx = cls.loop.run_until_complete( cls._async_main( [i for i in chunk_krx], _date_from, _date_to ) )
+        if len(chunk_krx_not) > 0:
+            async_data_krx_not = cls.loop.run_until_complete( cls._async_main( [i for i in chunk_krx_not], _date_from, _date_to, krx=False) )
+            async_data_krx_not = [ cls._nonkrx_handler(async_data_krx_not[0], _date_from, _date_to) ]
+            async_data = [ pd.concat([async_data_krx[0], async_data_krx_not[0]]) ]
+        else:
+            async_data = async_data_krx
+        return async_data
+
+
+    @classmethod
+    def _nonkrx_handler(cls, async_data_krx_not_df, _date_from, _date_to) -> pd.DataFrame:
+        won_dollar = cls.deepsearch.compute('QueryBankOfKoreaSeriesData("BOK:731Y001.0000001")')
+        async_data_krx_not = async_data_krx_not_df.rename({'close':f'주가 {_date_from}-{_date_to}'}, axis=1)
+        wd_stockprice = pd.merge(async_data_krx_not.reset_index(), won_dollar.reset_index()).set_index(['date', 'symbol'])
+        wd_stockprice[f'주가 {_date_from}-{_date_to}'] = wd_stockprice.loc[:, f'주가 {_date_from}-{_date_to}'] * wd_stockprice.loc[:, 'QueryBankOfKoreaSeriesData(BOK:731Y001.0000001)']
+        async_data_krx_not[f'주가 {_date_from}-{_date_to}'] = wd_stockprice[f'주가 {_date_from}-{_date_to}']
+        return async_data_krx_not
+
+
+    @classmethod
+    def _fdr_handler(cls, symbol, _date_from, _date_to):
+        if "KRX:" in symbol: symbol = symbol.split(":")[-1]
+        if "NICE:" in symbol: symbol = symbol.split(":")[-1]
+        _resp = fdr.DataReader(symbol,_date_from,_date_to)
+        if symbol in list(cls.fdr_krx["Symbol"]): 
+            _entity_name = cls.fdr_krx[cls.fdr_krx["Symbol"] == symbol]["Name"].values[0]
+        else: 
+            _entity_name = cls.fdr_krx_delisted[cls.fdr_krx_delisted["Symbol"] == symbol]["Name"].values[0]
+        _resp["symbol"] = "KRX:"+symbol
+        _resp["entity_name"] = _entity_name
+        _resp = _resp.reset_index()[["Date", "symbol", "entity_name", "Close"]].sort_values(by=["Date"])
+        _resp.columns = ["date", "symbol", "entity_name", f"주가 {_date_from}-{_date_to}"]
+        _resp = _resp.set_index(["date", "symbol"])
+        return _resp
+        """
+        _date_from, _date_to = str(_date_from), str(_date_to)
+        if "KRX:" in symbol: symbol = symbol.split(":")[-1]
+        if "NICE:" in symbol: symbol = symbol.split(":")[-1]
+        _resp = fdr.DataReader(symbol,_date_from,_date_to)
+        if symbol in list(cls.fdr_krx["Symbol"]): 
+            _entity_name = cls.fdr_krx[cls.fdr_krx["Symbol"] == symbol]["Name"].values[0]
+        else: 
+            _entity_name = cls.fdr_krx_delisted[cls.fdr_krx_delisted["Symbol"] == symbol]["Name"].values[0]
+        _resp["symbol"] = "KRX:"+symbol
+        _resp["entity_name"] = _entity_name
+        _resp = _resp.reset_index()[["Date", "symbol", "entity_name", "Close"]].sort_values(by=["Date"])
+        _resp.columns = ["date", "symbol", "entity_name", f"주가 {_date_from}-{_date_to}"]
+        _resp = _resp.set_index(["date", "symbol"])
+        return _resp
+        """
+
+
+    @classmethod
+    def _pdr_naver_handler(cls, chunk_krx, ticker_name_df, _date_from, _date_to) -> list:
+        """
+        _date_from 은 change_rate 과 호환되어야 한다. 
+        """
+        # 220630 맘스터치 상폐 / 007460 무증
+        resp_basket = pd.DataFrame()
+        for idx, ticker in enumerate(chunk_krx):
+            _ticker = ticker.replace("KRX:", "")#.replace(" ", "")
+
+            #!  XML or text declaration not at start of entity: line 3, column 0 : 없는 티커
+            _resp = pdr.DataReader(_ticker, "naver", start=(pd.to_datetime(_date_from) -relativedelta(months=1)).strftime("%Y-%m-%d"), end=_date_to)[["Open", "High", "Low", "Close", "Volume"]]
+            _resp = _resp.rename(columns={'Open': 'open', 'High': 'high', 'Low': 'low', 'Close': 'close', 'Volume': 'volume'}).reset_index()
+            _resp['entity_name'] = ticker_name_df.loc["KRX:"+_ticker].values[-1][0]
+            _resp['symbol'] = "KRX:"+_ticker
+            _resp['date'] = _resp['Date']
+            _resp["change_rate"] = _resp["close"].astype(float).pct_change()
+            _resp = _resp[["date", "symbol", "entity_name", "change_rate"]]
+
+            date_for_change_rate = ((_resp["date"] < pd.to_datetime(_date_from))).replace(False, np.nan).dropna()
+            if len(date_for_change_rate) == 0: pass  # _start 이전 데이터가 없는 경우
+            else:
+                # resp = resp.iloc[((resp["date"] > pd.to_datetime(_start))).replace(False, np.nan).dropna().index[0]:]
+                _resp = _resp.iloc[date_for_change_rate.index[-1] +1:]  #! ??? : resp = _resp.iloc[date_for_change_rate.index[-1] +1:] 이렇게 되어있었음
+            resp_basket = pd.concat([resp_basket, _resp], axis=0)  #! ??? : resp_basket = pd.concat([resp_basket, resp], axis=0) 이렇게 되어있었음
+        async_data = [resp_basket.sort_values(["date", "symbol"]).set_index(["date", "symbol"])]
+        return async_data
+
+
+    @classmethod
+    def compute(cls, deepsearch_df, df_to_upload_bool=False, debug=False, fdr=False, naver=False):
+        
+        if naver:
+            ticker_name_dict = dict()
+            ticker_nice_dict = dict()
+            ticker_name_df = deepsearch_df.reset_index()[["symbol_listed", "entity_name"]].drop_duplicates().set_index("symbol_listed")
+            ticker_nice_df = deepsearch_df.reset_index()[["symbol_listed", "symbol"]].drop_duplicates().set_index("symbol_listed")
+
+
+        df = cls._split_phases(cls, deepsearch_df)
+        _rebalancing_dates = list(df.keys())
+        for idx, date in enumerate(_rebalancing_dates):
+            if datetime.today() < cls._datetime_reformer(date):
+                print(_rebalancing_dates, _rebalancing_dates[:idx])
+                _rebalancing_dates = _rebalancing_dates[:idx]
+                break
+
+        """ 
+            종가매수 : 오늘 홀딩스 업데이트 한 경우, 종가매수 후 작업이 포트폴리오 계산에 반영되지 않으므로 제외한다.
+        """
+        if _rebalancing_dates[-1].strftime("%m/%d/%Y") == datetime.today().strftime("%m/%d/%Y"): 
+            rebalancing_dates = _rebalancing_dates[:-1]
+
+
+
+        cls._aum = 100_000_000_000.0  #! 변수 초기화
+
+        _async_batch_size = 10
+        total_return = pd.DataFrame()
+        for idx, date in enumerate(rebalancing_dates):  # idx starts from 0
+            print(idx, date, rebalancing_dates)
+            """
+                rebalancing_dates 는 holdings 파일의 날짜를 의미하며
+                date 는 종가리밸런싱이 수행되는 날짜를 의미한다.
+                바뀐 포트폴리오의 주가변동은 익일부터 적용된다. 
+                만약 홀딩스 파일 기준 date가 휴일이면, 해당 날짜가 휴일이 아닐 때까지 계속해서 다음날로 넘어간다.
+                    - ex 24.05.01
+                        24년 5월 1일 자 종가 매수 후, 포트폴리오 수익률은 익일은 5월 2일의 수익률부터 반영.
+                    - ex 24.05.05 
+                        24년 5월 5일은 일요일 휴일. 5월 6일은 대체공휴일. 리밸런싱 날짜는 5월 7일로 넘어간다.
+
+                05.10 수정내역
+                    - 05.01 , 05.05 , 05.10 으로 테스팅 한 결과, 
+                        첫 번째 페이즈는 2일부터 5일을 포함하고, 두 번째 페이즈는 7일부터 10일을 포함하고 있었다 (말일 종가매수 예외처리 적용). 
+                        즉, 1일의 종가에 매수하여 2일과 3일의 수익률을 반영하고, 3일의 종가에 매수하여 7일부터 10일의 수익률을 반영했다. 
+                        휴일 이슈를 제외하면, 7일의 수익률이 두 번째 페이즈에 반영되는 것이 옳으나,
+                        * 5월 5일이 리밸런싱 일자이므로 다음 거래일의 종가에 매수가 이루어지면, 첫번 째 페이즈는 2일부터 7일까지를 포함해야 한다.
+                        * 기존방식인 두 번쨰 페이즈가 7일을 포함한다는 것은, 5일이 휴일이므로 직전 거래일의 종가에 매수함을 의미한다. 
+                        ? 휴일의 종가에 매수한다는 것은 어떤 매매를 의도한 것인가? 포트폴리오 작성 시점에, 5일이 휴일이라는 것을 알지 않았다면?
+                        
+            """
+            async_result = pd.DataFrame()
+            if isinstance(df[date], pd.Series): _df = pd.DataFrame(df[date]).T
+            else: _df = df[date]
+            ratio = _df.reset_index().set_index(['symbol'])['weight'].astype(float)  # 단축코드, 비중(비중의합은1)
+            ratio.index = ratio.index.str.replace(" ", "")
+            pdf = list(_df['symbol'])  # 0 은 iter item (timestamp)
+
+            if naver: pdf = list(_df["symbol_listed"])
+
+            delisted_firm_dict = dict()
+            delisted_firm = _df[_df['symbol'] != _df['symbol_listed']]
+            for _, row in delisted_firm.iterrows(): delisted_firm_dict[row['symbol_listed']] = row['symbol']
+
+            date = cls._datetime_reformer(date)
+
+            b_days = 0
+            while True:
+                if not cls._is_business_day(date): date, b_days = date +relativedelta(days=1), b_days +1
+                else: break
+
+
+            if idx+1 != len(rebalancing_dates):  #* if not the last phase
+                # _date_from = datetime.strftime(date -relativedelta(days=1), "%Y-%m-%d")
+                _date_from_for_close_column = datetime.strftime(date -relativedelta(days=1), "%Y-%m-%d")  # close 기반 하루전날 데이터
+                #* 240307 변경(추가) 코드
+                # _date_from = datetime.strftime(date, "%Y-%m-%d")  # change_rate 기반 당일 데이터 (당일 수익률 데이터)
+                #* 익일의 당일수익률부터 반영
+                _date_from = datetime.strftime(date +relativedelta(days=1), "%Y-%m-%d")  #! 휴일이면 안된다 (api 별로 익일을 가져오는지 전일을 가져오는지가 다름). 
+
+                _date_to_for_close_column = datetime.strftime(cls._datetime_reformer(rebalancing_dates[idx+1]) -relativedelta(days=1), "%Y-%m-%d")  # 리밸런싱 전날
+                _date_to = datetime.strftime(cls._datetime_reformer(rebalancing_dates[idx+1])-relativedelta(days=0), "%Y-%m-%d")  # 리밸런싱 당일 종가가 기존포트의 수익률에 포함됨
+
+                for i in range(len(pdf)//_async_batch_size +1):
+                    chunk_start, chunk_end = i*_async_batch_size, (i+1)*_async_batch_size
+
+                    chunk = pdf[chunk_start:chunk_end]
+                    chunk_krx = [i for i in chunk if (i.startswith('KRX:') | i.startswith('NICE:'))]  # ['KRX:007070', 'KRX:023530', 'KRX:139480', 'KRX:097950']
+                    chunk_krx_not = list(set(chunk) - set(chunk_krx))
+
+                    if len(chunk) != len(chunk_krx):
+                        print(chunk)
+                        print(chunk_krx)
+
+                    if len(chunk) == 0: break
+                    if naver:
+                        async_data = []
+                        try: _async_data = cls._pdr_naver_handler(chunk_krx, ticker_name_df, _date_from, _date_to)
+                        except: _async_data = cls._pdr_naver_handler(cls, chunk_krx, ticker_name_df, _date_from, _date_to)
+                        async_data = async_data +_async_data
+                    else:   
+                        try: async_data = cls._async_main_wrapper( chunk_krx, chunk_krx_not, _date_from, _date_to)
+                        except: async_data = cls._async_main_wrapper(cls, chunk_krx, chunk_krx_not, _date_from, _date_to)
+
+
+                    for data in async_data:  # wrapper return datatype handler
+                        # data.columns = ['entity_name', 'close']  #! 데이터가 안받아져 왔을 시 죽는다
+                        try:
+                            data.columns = ['entity_name', 'change_rate']  #! 데이터가 안받아져 왔을 시 죽는다
+                        except:
+                            import pdb
+                            pdb.set_trace()
+                        async_result = pd.concat([async_result, data], axis=0)
+
+                '''
+                for i in range(len(pdf)//_async_batch_size +1):
+                    chunk_start, chunk_end = i*_async_batch_size, (i+1)*_async_batch_size
+            
+                    chunk = pdf[chunk_start:chunk_end]
+                    chunk_krx = [i for i in chunk if (i.startswith('KRX:') | i.startswith('NICE:'))]
+                    chunk_krx_not = list(set(chunk) - set(chunk_krx))
+
+                    # chunk_krx = chunk_krx[chunk_start:chunk_end]
+                    # chunk_krx_not = chunk_krx_not[chunk_start:chunk_end]
+
+
+                    if len(chunk) == 0: break
+                    #! 왜 다른가?
+                    """try: 
+                        async_data_krx = loop.run_until_complete( cls._async_main( cls, [i for i in chunk_krx], _date_from, _date_to ) )
+                        if len(chunk_krx_not) > 0:
+                            async_data_krx_not = loop.run_until_complete( cls._async_main( cls, [i for i in chunk_krx_not], _date_from, _date_to, krx=False) )
+                            async_data_krx_not = [ cls._nonkrx_handler(async_data_krx_not[0], _date_from, _date_to) ]
+                            async_data = [ pd.concat([async_data_krx[0], async_data_krx_not[0]]) ]
+                        else:
+                            async_data = async_data_krx
+                    except: 
+                        async_data_krx = loop.run_until_complete( cls._async_main( [i for i in chunk_krx], _date_from, _date_to ) )
+                        if len(chunk_krx_not) > 0:
+                            async_data_krx_not = loop.run_until_complete( cls._async_main( [i for i in chunk_krx_not], _date_from, _date_to, krx=False) )
+                            async_data_krx_not = [ cls._nonkrx_handler(async_data_krx_not[0], _date_from, _date_to) ]
+                            async_data = [ pd.concat([async_data_krx[0], async_data_krx_not[0]]) ]
+                        else:
+                            async_data = async_data_krx"""
+                    # if (datetime.strptime(_date_from, "%Y-%m-%d") < datetime(2022, 9, 28)) & (datetime(2022, 9, 28) < datetime.strptime(_date_to, "%Y-%m-%d")):
+                    #     for symbol in chunk_krx:
+                    #         try:
+                    #             _async_resp = cls._fdr_handler( symbol, _date_from, _date_to)
+                    #         except:
+                    #             _async_resp = cls._fdr_handler(cls, symbol, _date_from, _date_to)
+                    #         _async_data_fdr = pd.concat([_async_data_fdr, _async_resp]).sort_index()
+                    #     async_data = [_async_data_fdr]
+                    # else:  # 문제의 기간이 없다면
+                    try: 
+                        async_data = cls._async_main_wrapper( chunk_krx, chunk_krx_not, _date_from, _date_to)
+                    except:
+                        async_data = cls._async_main_wrapper(cls, chunk_krx, chunk_krx_not, _date_from, _date_to)
+
+
+                    for data in async_data: 
+                        data.columns = ['entity_name', 'close']  #! 데이터가 안받아져 왔을 시 죽는다
+                        async_result = pd.concat([async_result, data], axis=0)
+                '''
+            else:  #* if the last phase
+                _date_from_for_close_column = datetime.strftime(date -relativedelta(days=1), "%Y-%m-%d")  # close 기반 하루전날 데이터 
+                #* 240307 변경(추가) 코드
+                # _date_from = datetime.strftime(date, "%Y-%m-%d")  # change_rate 기반 당일 데이터
+                _date_from = datetime.strftime(date +relativedelta(days=1), "%Y-%m-%d")  #! 휴일이면 안된다 (api 별로 익일을 가져오는지 전일을 가져오는지가 다름). 
+                _date_to = datetime.strftime(datetime.today().date(), "%Y-%m-%d")
+
+                for i in range(len(pdf)//_async_batch_size +1):
+                    chunk_start, chunk_end = i*_async_batch_size, (i+1)*_async_batch_size
+                    
+                    chunk = pdf[chunk_start:chunk_end]
+                    chunk_krx = [i for i in chunk if (i.startswith('KRX:') | i.startswith('NICE:'))]
+                    chunk_krx_not = set(chunk) - set(chunk_krx)
+
+                    if len(chunk) != len(chunk_krx):
+                        print(chunk)
+                        print(chunk_krx)
+
+                    if len(chunk) == 0: break
+                    if naver:
+                        async_data = []
+                        try: _async_data = cls._pdr_naver_handler(chunk_krx, ticker_name_df, _date_from, _date_to)
+                        except: _async_data = cls._pdr_naver_handler(cls, chunk_krx, ticker_name_df, _date_from, _date_to)
+                        async_data = async_data +_async_data
+                    else:   
+                        try: async_data = cls._async_main_wrapper(chunk_krx, chunk_krx_not, _date_from, _date_to)
+                        except: async_data = cls._async_main_wrapper(cls,  chunk_krx, chunk_krx_not, _date_from, _date_to)
+
+
+                    for data in async_data:
+                        # data.columns = ['entity_name', 'close']
+                        data.columns = ['entity_name', 'change_rate']  #! 데이터가 안받아져 왔을 시 죽는다
+                        async_result = pd.concat([async_result, data], axis=0)
+
+            async_result_reset = async_result.reset_index()
+
+            
+            #####################################################################################################################
+            #* close
+            # pdf_returns_ds = async_result_reset.drop_duplicates(subset=['date', 'symbol'], keep='first').pivot(index='date', columns='symbol', values='close').ffill()
+            # pdf_returns_async = (pdf_returns_ds.pct_change().fillna(0) +1).cumprod()  #! NICE가 없다
+
+            #* change_rate
+            pdf_returns_ds = async_result_reset.drop_duplicates(subset=['date', 'symbol'], keep='first').pivot(index='date', columns='symbol', values='change_rate').ffill()
+            pdf_returns_async = (pdf_returns_ds +1).cumprod()
+            #####################################################################################################################
+            
+            # pdf_returns_ds.iloc[0, :] = 0  #* 주가수익률로 계산했을 시기의 코드 
+            # pdf_returns_async = (pdf_returns_ds +1).cumprod()  #* 주가수익률로 계산했을 시기의 코드 
+            pdf_returns_async.columns = [ delisted_firm_dict[i] if i in delisted_firm_dict.keys() else i for i in pdf_returns_async.columns ]
+
+            inherited_budget = ratio * cls._aum  # 시작분배금  #! NICE가 있다 / ratio는 가장 최근의 리밸비중 / 여기서의 cls._aum 은 다음 값으로 업데이트 되기 전임
+            #* 시작일은 base_point를 남기고 그 이후부터는 첫날의 리밸런싱 무수익을 떨군다
+
+            inherited_budget.index = inherited_budget.index.astype(str)
+            pdf_returns_async.columns = pdf_returns_async.columns.astype(str)
+            if idx > 0: 
+                #* 기존 코드 : 종가리밸런싱일자 익일 수익률부터 반영하지만, 종가리밸런싱일자의 하루치 수익률이 들어가 있다
+                # _aum_change_async = pdf_returns_async[datetime.strptime(_date_from, "%Y-%m-%d").date() +relativedelta(days=1):] *inherited_budget
+                #* 240307 변경 코드
+                _aum_change_async = pdf_returns_async[datetime.strptime(_date_from, "%Y-%m-%d").date() +relativedelta(days=0):] *inherited_budget
+            else:  # 최초 상장
+                _aum_change_async = pdf_returns_async *inherited_budget
+                
+
+            # cls._aum = _aum_change_async.sum(axis=1)[-1]  # deprecation caution informed
+            cls._aum = _aum_change_async.sum(axis=1).iloc[-1]
+            total_return = pd.concat([total_return, _aum_change_async])
+            print(cls._aum)
+
+
+        if debug == True:
+            import pdb
+            pdb.set_trace()
+
+        total_return = total_return.groupby(total_return.index).first()
+
+        if df_to_upload_bool:
+            total_return = total_return.groupby(total_return.index).first()
+            base_point = 1000
+            daily_aum = total_return.sum(axis=1)
+            daily_aum.index = pd.to_datetime(daily_aum.index)
+            index_calc_start_date = cls._datetime_reformer(rebalancing_dates[0])
+
+            """
+            //2023-01-19//
+            close 기반 기존의 계산 -> 시가매수
+            change_rate 기반 계산 -> 종가매수 
+            """
+            import copy
+            daily_aum_for_change_rate = copy.deepcopy(daily_aum)
+            daily_aum_for_change_rate = dict(daily_aum_for_change_rate)
+            daily_aum_for_change_rate[index_calc_start_date] = 100_000_000_000
+            daily_aum_for_change_rate = pd.Series(daily_aum_for_change_rate).sort_index()
+
+            daily_aum = daily_aum_for_change_rate
+
+            try:
+                daily_idx = daily_aum / daily_aum[datetime.strftime(index_calc_start_date, "%Y-%m-%d")] *base_point
+            except:
+                print(f'error check [{rebalancing_dates[0]}] - date index not exists, call the most recent previous date')
+                daily_idx = daily_aum / daily_aum[:datetime.strftime(index_calc_start_date, "%Y-%m-%d")].iloc[-1] *base_point
+            daily_idx = daily_idx[datetime.strftime(index_calc_start_date, "%Y-%m-%d"):]
+
+
+            resp = pdr.DataReader("KOSPI", "naver", start=datetime.strftime(index_calc_start_date, '%Y-%m-%d'), end=datetime.strftime(datetime.today().date(), '%Y-%m-%d'))[["Open", "High", "Low", "Close", "Volume"]]
+            resp = resp.astype(float)
+            resp["symbol"] = "KRX:KOSPI"
+            resp["entity_name"] = "코스피"
+            resp = resp.reset_index()[["Date", "symbol", "entity_name", "Close"]].sort_values(by=["Date"])
+            resp.columns = ["date", "symbol", "entity_name", f"주가 {datetime.strftime(index_calc_start_date, '%Y-%m-%d')}-{datetime.strftime(datetime.today().date(), '%Y-%m-%d')}"]
+            resp = resp.set_index(["date", "symbol"])
+            kospi = resp.reset_index().set_index('date')
+            kospi.columns = ['symbol', 'entity_name', 'close']
+            kospi.index = pd.to_datetime(kospi.index).date
+
+            #! 한국주식과 미국주식을 섞으면 공휴일이 다르다 
+            _excel_date_format = "%Y-%m-%d"
+            try:
+                daily_idx_date_reviewed = daily_idx.loc[kospi.index]
+            except:
+                daily_idx.index = pd.to_datetime(daily_idx.index).date
+                daily_idx_date_reviewed = daily_idx
+            
+            df_to_upload = pd.concat([daily_idx_date_reviewed, kospi["close"]], axis=1).sort_index(ascending=True).bfill()
+            df_to_upload.columns = ['index', 'KOSPI']
+            df_to_upload.index = pd.to_datetime(df_to_upload.index, format="%Y-%m-%d")
+            df_to_upload.index = df_to_upload.index.strftime(_excel_date_format)
+            df_to_upload = df_to_upload.reset_index()
+            df_to_upload.columns = ['date', 'index', 'KOSPI']
+
+            df_to_upload["index"] = df_to_upload["index"] / df_to_upload["index"].iloc[0] * base_point
+            df_to_upload["KOSPI"] = df_to_upload["KOSPI"] / df_to_upload["KOSPI"].iloc[0] * base_point
+
+
+            df_to_upload['date'] = df_to_upload['date'].astype(str)
+
+            return df_to_upload
+        return total_return
+
+
+
+
+class _backtest(object):
+    _aum = 100_000_000_000.0
+    deepsearch = DeepSearchAPI()
+    async_deepsearch = asyncDeepSearchAPI()
+    wavelet = WaveletAPI()
+
+    def _split_phases(cls, deepsearch_df):
+        return_dict = dict()
+        phases = deepsearch_df.index.unique()
+        for p in phases:
+            pdf = deepsearch_df.loc[p]
+            return_dict[p] = pdf
+        return return_dict
+
+    def _is_business_day(date):
+        return bool(len(pd.bdate_range(date, date)))
+
+    @classmethod
+    async def _async_main(cls, symbol_list, date_from, date_to):
+        query = ' '.join(symbol_list) + f' {date_from}-{date_to} 주가'  #! 주가수익률은 해당말일을 기준으로 한 점만 보여준다
+        task = [cls.async_deepsearch.compute(query)]
+        result = await asyncio.gather(*task)
+        return result
+
+    @classmethod
+    def compute(cls, deepsearch_df, df_to_upload_bool=False, debug=False):
+        df = cls._split_phases(cls, deepsearch_df)
+        rebalancing_dates = list(df.keys())
+        for idx, date in enumerate(rebalancing_dates):
+            if datetime.today() < (datetime.strptime(date, "%m/%d/%Y")):
+                print(rebalancing_dates, rebalancing_dates[:idx])
+                rebalancing_dates = rebalancing_dates[:idx]
+                break
+
+
+
+        loop = asyncio.get_event_loop()
+        _async_batch_size = 10
+
+
+        total_return = pd.DataFrame()
+        for idx, date in enumerate(rebalancing_dates):  # idx starts from 0
+            async_result = pd.DataFrame()
+            if isinstance(df[date], pd.Series): _df = pd.DataFrame(df[date]).T
+            else: _df = df[date]
+            ratio = _df.reset_index().set_index(['symbol'])['weight'].astype(float)  # 단축코드, 비중(비중의합은1)
+            ratio.index = ratio.index.str.replace(" ", "")
+            pdf = list(_df['symbol'])  # 0 은 iter item (timestamp)
+
+            delisted_firm_dict = dict()
+            delisted_firm = _df[_df['symbol'] != _df['symbol_listed']]
+            for _, row in delisted_firm.iterrows(): delisted_firm_dict[row['symbol_listed']] = row['symbol']
+
+            date = datetime.strptime(date, "%m/%d/%Y")
+
+            b_days = 0
+            while True:
+                if not cls._is_business_day(date): date, b_days = date +relativedelta(days=1), b_days +1
+                else: break
+
+
+            if idx+1 != len(rebalancing_dates):  #* if not the last phase
+                _date_from = datetime.strftime(date -relativedelta(days=1), "%Y-%m-%d")
+                _date_to = datetime.strftime(datetime.strptime(rebalancing_dates[idx+1], "%m/%d/%Y") -relativedelta(days=1), "%Y-%m-%d")
+
+                for i in range(len(pdf)//_async_batch_size +1):
+                    chunk_start, chunk_end = i*_async_batch_size, (i+1)*_async_batch_size
+                    chunk = pdf[chunk_start:chunk_end]
+                    if len(chunk) == 0: break
+                    #! 왜 다른가?
+                    try: async_data = loop.run_until_complete( cls._async_main( cls, [i for i in chunk], _date_from, _date_to ) )
+                    except: async_data = loop.run_until_complete( cls._async_main( [i for i in chunk], _date_from, _date_to ) )
+                    for data in async_data: 
+                        data.columns = ['entity_name', 'close']  #! 데이터가 안받아져 왔을 시 죽는다
+                        async_result = pd.concat([async_result, data], axis=0)
+            else:  #* if the last phase
+                _date_from = datetime.strftime(date -relativedelta(days=1), "%Y-%m-%d")
+                _date_to = datetime.strftime(datetime.today().date(), "%Y-%m-%d")
+
+                for i in range(len(pdf)//_async_batch_size +1):
+                    chunk_start, chunk_end = i*_async_batch_size, (i+1)*_async_batch_size
+                    chunk = pdf[chunk_start:chunk_end]
+                    if len(chunk) == 0: break
+                    #! 왜 다른가?
+                    try: async_data = loop.run_until_complete( cls._async_main( cls, [i for i in chunk], _date_from, _date_to) )  # datetime.strftime(datetime.today(), "%Y-%m-%d")
+                    except: async_data = loop.run_until_complete( cls._async_main( [i for i in chunk], _date_from, _date_to) )  # datetime.strftime(datetime.today(), "%Y-%m-%d")
+                    for data in async_data:
+                        data.columns = ['entity_name', 'close']
+                        async_result = pd.concat([async_result, data], axis=0)
+
+            async_result_reset = async_result.reset_index()
+            pdf_returns_ds = async_result_reset.drop_duplicates(subset=['date', 'symbol'], keep='first').pivot(index='date', columns='symbol', values='close')
+            pdf_returns_async = (pdf_returns_ds.pct_change().fillna(0) +1).cumprod()  #! NICE가 없다
+            # pdf_returns_ds.iloc[0, :] = 0  #* 주가수익률로 계산했을 시기의 코드 
+            # pdf_returns_async = (pdf_returns_ds +1).cumprod()  #* 주가수익률로 계산했을 시기의 코드 
+            pdf_returns_async.columns = [ delisted_firm_dict[i] if i in delisted_firm_dict.keys() else i for i in pdf_returns_async.columns ]
+
+            inherited_budget = ratio * cls._aum  # 시작분배금  #! NICE가 있다 / ratio는 가장 최근의 리밸비중 / 여기서의 cls._aum 은 다음 값으로 업데이트 되기 전임
+            #* 시작일은 base_point를 남기고 그 이후부터는 첫날의 리밸런싱 무수익을 떨군다
+
+            try: _prev_aum_change_async = _aum_change_async
+            except: pass
+            inherited_budget.index = inherited_budget.index.astype(str)
+            pdf_returns_async.columns = pdf_returns_async.columns.astype(str)
+            if idx > 0: 
+                _aum_change_async = pdf_returns_async[datetime.strptime(_date_from, "%Y-%m-%d").date() +relativedelta(days=1):] *inherited_budget
+            else: _aum_change_async = pdf_returns_async *inherited_budget
+
+            cls._aum = _aum_change_async.sum(axis=1)[-1]
+            total_return = pd.concat([total_return, _aum_change_async])
+            print(cls._aum)
+
+            # total_return = pd.concat([total_return, _aum_change_wavelet])
+
+        if debug == True:
+            import pdb
+            pdb.set_trace()
+
+        total_return = total_return.groupby(total_return.index).first()
+
+        cls._aum = 100_000_000_000.0  #! 변수 초기화
+
+        if df_to_upload_bool:
+            total_return = total_return.groupby(total_return.index).first()
+            base_point = 1000
+            daily_aum = total_return.sum(axis=1)
+            try:
+                daily_idx = daily_aum / daily_aum[datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), "%Y-%m-%d")] *base_point
+            except:
+                print(f'error check [{rebalancing_dates[0]}] - date index not exists, call the most recent previous date')
+                daily_idx = daily_aum / daily_aum[:datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), "%Y-%m-%d")].iloc[-1] *base_point
+            daily_idx = daily_idx[datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), "%Y-%m-%d"):]
+            
+            """
+            daily_aum.index = pd.to_datetime(daily_aum.index)
+            daily_idx = daily_aum / daily_aum[datetime.strftime(datetime.strptime(rebalancing_dates[0], "%m/%d/%Y"), "%Y-%m-%d")] *base_point
+            daily_idx = daily_idx[datetime.strftime(datetime.strptime(rebalancing_dates[0], "%m/%d/%Y"), "%Y-%m-%d"):]
+            # daily_idx.index = daily_idx.index.date
+            """
+
+            #* rebalancing_dates[0] 은 해당일 종가매수를 의미한다.
+            #* 즉, 월요일부터의 수익률을 보고싶은 경우, 리밸런싱 날짜는 월요일이 아닌 직전 거래일(금요일)을 넣어야 한다.
+            _query_kospi = f"코스피 지수 {datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), '%Y-%m-%d')}-{datetime.strftime(datetime.today().date(), '%Y-%m-%d')}"
+            resp = cls.deepsearch.compute(_query_kospi).reset_index().set_index('date')
+            resp.columns = ['close' if '지수' in i else i for i in resp.columns]
+            kospi = resp
+
+            # import FinanceDataReader as fdr
+            # from pandas_datareader import data 
+            # resp = data.DataReader("KOSPI", "naver", start=datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), '%Y-%m-%d'), end=datetime.strftime(datetime.today().date(), '%Y-%m-%d'))[["Open", "High", "Low", "Close", "Volume"]]
+            # resp = resp.astype(float)
+            # resp["symbol"] = "KRX:KOSPI"
+            # resp["entity_name"] = "코스피"
+            # resp = resp.reset_index()[["Date", "symbol", "entity_name", "Close"]].sort_values(by=["Date"])
+            # resp.columns = ["date", "symbol", "entity_name", f"주가 {datetime.strftime(cls._datetime_reformer(rebalancing_dates[0]), '%Y-%m-%d')}-{datetime.strftime(datetime.today().date(), '%Y-%m-%d')}"]
+            # resp = resp.set_index(["date", "symbol"])
+            # kospi = resp.reset_index().set_index('date')
+            # kospi.columns = ['symbol', 'entity_name', 'close']
+            # kospi.index = pd.to_datetime(kospi.index).date
+
+            #! 한국주식과 미국주식을 섞으면 공휴일이 다르다 
+            try:
+                daily_idx_date_reviewed = daily_idx.loc[kospi.index]
+            except:
+                import pdb
+                pdb.set_trace()
+            # kospi_ret = kospi['close'].loc[daily_idx.index].pct_change()  # 당일의 종가수익률이 아니라 판다스에서 추가적으로 계산된 값이므로 첫날의 수익률은 누락 #! 그런데 첫날이 월요일이면 -1day때문에 길이가 안맞는다
+            kospi_ret = kospi['close'].pct_change()
+
+            daily_kospi = (kospi_ret+1).cumprod().fillna(1) *base_point  #* 엑셀 holdings 파일의 date 는 종가매수의 기준일이므로, 날짜를 월요일로 잡아도 월요일 종가매수를 의미한다. 
+            # daily_kospi.index = daily_kospi.index.date
+            #업로드용 파일 가공
+            _excel_date_format = "%Y-%m-%d"
+            # df_to_upload = pd.concat([daily_idx, daily_kospi], axis=1)
+            df_to_upload = pd.concat([daily_idx_date_reviewed, daily_kospi], axis=1)
+            df_to_upload.columns = ['index', 'KOSPI']
+            df_to_upload.index = pd.to_datetime(df_to_upload.index, format="%Y-%m-%d")
+            df_to_upload.index = df_to_upload.index.strftime(_excel_date_format)
+            df_to_upload = df_to_upload.reset_index()
+            df_to_upload.columns = ['date', 'index', 'KOSPI']
+            df_to_upload['date'] = df_to_upload['date'].astype(str)
+
+            """
+            _excel_date_format = "%d/%m/%Y"
+            df_to_upload = pd.concat([daily_idx, daily_kospi], axis=1)
+            df_to_upload.columns = ['index', 'KOSPI']
+            df_to_upload.index = pd.to_datetime(df_to_upload.index, format="%Y-%m-%d")
+            df_to_upload.index = df_to_upload.index.strftime(_excel_date_format)
+            df_to_upload = df_to_upload.reset_index()
+            """
+
+            return df_to_upload
+        return total_return
```

## Comparing `deepsearcheath-0.9.6.dist-info/LICENSE` & `deepsearcheath-1.1.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

