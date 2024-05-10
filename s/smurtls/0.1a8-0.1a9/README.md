# Comparing `tmp/smurtls-0.1a8-py3-none-any.whl.zip` & `tmp/smurtls-0.1a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3567 bytes, number of entries: 6
--rw-r--r--  2.0 unx       19 b- defN 24-May-08 20:07 smurtls/__init__.py
--rw-r--r--  2.0 unx     7331 b- defN 24-May-08 20:07 smurtls/data.py
--rw-r--r--  2.0 unx      474 b- defN 24-May-08 20:07 smurtls-0.1a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-08 20:07 smurtls-0.1a8.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-08 20:07 smurtls-0.1a8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      442 b- defN 24-May-08 20:07 smurtls-0.1a8.dist-info/RECORD
-6 files, 8366 bytes uncompressed, 2765 bytes compressed:  66.9%
+Zip file size: 3639 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       19 b- defN 24-May-09 00:06 smurtls/__init__.py
+-rw-r--r--  2.0 unx     7758 b- defN 24-May-09 00:06 smurtls/data.py
+-rw-r--r--  2.0 unx      474 b- defN 24-May-09 00:06 smurtls-0.1a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-09 00:06 smurtls-0.1a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-09 00:06 smurtls-0.1a9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      442 b- defN 24-May-09 00:06 smurtls-0.1a9.dist-info/RECORD
+6 files, 8793 bytes uncompressed, 2837 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: smurtls/__init__.py
 Comment: 
 
 Filename: smurtls/data.py
 Comment: 
 
-Filename: smurtls-0.1a8.dist-info/METADATA
+Filename: smurtls-0.1a9.dist-info/METADATA
 Comment: 
 
-Filename: smurtls-0.1a8.dist-info/WHEEL
+Filename: smurtls-0.1a9.dist-info/WHEEL
 Comment: 
 
-Filename: smurtls-0.1a8.dist-info/top_level.txt
+Filename: smurtls-0.1a9.dist-info/top_level.txt
 Comment: 
 
-Filename: smurtls-0.1a8.dist-info/RECORD
+Filename: smurtls-0.1a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## smurtls/data.py

```diff
@@ -3,18 +3,23 @@
 from sklearn.preprocessing import MinMaxScaler
 from lifelines.utils import  concordance_index
 from datetime import datetime
 
 class Reader:
     @staticmethod 
     def read_csv(dataSetPath, columns = [], **params):
+        verbose = False
         df = pd.read_csv(dataSetPath)
         if len(columns) != 0:
             df = df[columns]
         # --------------------
+        if "verbose" in params and params["verbose"]:
+            if params["verbose"] == 1:
+                verbose = True
+            
         if "dropna_rows" in params and params["dropna_rows"]:
             na_mask = df.isna().any(axis=1)
             df = df[~na_mask]
             df.reset_index(drop=True, inplace=True)
 
         if "head" in params and params["head"]:
             num = params["head"]
@@ -27,15 +32,16 @@
                 num = df.shape[0]
             if num < 0:
                 Debug.puts(actor=Reader, status=418, message="Number of rows to display is negative. Displaying the entire dataset.")
                 num = df.shape[0]
             
             df = df.head(num)
         # --------------------
-        Reader.print_df_stats(df)
+        if verbose:
+            Reader.print_df_stats(df)
         return df
 
     @staticmethod
     def print_df_stats(df):
         state = "Shape: " + str(df.shape) + "\n"
         state += "NaN rows: " + str(len(df[df.isna().any(axis=1)])) + "\n"
         Debug.puts(actor=Reader, status=101, message=state)
@@ -115,15 +121,15 @@
         data = data.copy()
         for col in cols:
             uniqs = data[col].unique()
             if len(uniqs) == 2:
                 if data[col].dtype == bool:
                     data[col] = data[col].astype(float)
                 elif data[col].dtype == 'object' and any(value.lower() in {'yes', 'no', 'ja', 'nein'} for value in data[col].unique()):
-                    data[col] = data[col].str.lower().replace({"yes": 1.0, "no": 0.0, "ja": 1.0, "nein": 0.0})
+                    data[col] = data[col].infer_objects(copy=False).str.lower().replace({"yes": 1.0, "no": 0.0, "ja": 1.0, "nein": 0.0})
                 else:
                     data[col] = data[col].map({uniqs[0]: 0.0, uniqs[1]: 1.0})
         
         data.reset_index(drop=True, inplace=True)
         return data
 
     @staticmethod
@@ -195,17 +201,20 @@
     
     return res
 
 
 
 class Eval:
     @staticmethod
-    def hci(y_pred, labels, breaks, time):
+    def hci(y_pred, labels_time, labels_status, breaks, time):
         """
         y_pred: shape (n_samples, n_intervals) -> [Prediction_at_interval_1, ..., Prediction_at_interval_n]
         labels: shape (n_samples, 2) -> [Time_OS, Status_OS]
         breaks: shape (n_intervals+1,) -> [0, ..., n_intervals]
         time: point in time of interest in years
         """
-        return concordance_index(labels["Time_OS"], np.cumprod(y_pred[:,0:np.where(breaks>time*365)[0][0]], axis=1)[:,-1], labels["Status_OS"])
+        print(len(np.cumprod(y_pred[:,0:np.where(breaks>time*365)[0][0]], axis=1)[:,-1]))
+        print(len(labels_time))
+        #print(np.cumprod(y_pred[:,0:np.where(breaks>time*365)[0][0]], axis=1)[:,-1])
+        return concordance_index(labels_time, np.cumprod(y_pred[:,0:np.where(breaks>time*365)[0][0]], axis=1)[:,-1], labels_status)
```

