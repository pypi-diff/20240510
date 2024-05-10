# Comparing `tmp/pwrpy-1.1.3.tar.gz` & `tmp/pwrpy-1.1.4.tar.gz`

## Comparing `pwrpy-1.1.3.tar` & `pwrpy-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pwrpy-1.1.3/app.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 pwrpy-1.1.3/requirements.txt
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pwrpy-1.1.3/scripts.txt
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pwrpy-1.1.3/.vscode/launch.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pwrpy-1.1.3/src/pwrpy/__init__.py
--rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 pwrpy-1.1.3/src/pwrpy/pwrapisdk.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 pwrpy-1.1.3/src/pwrpy/pwrwallet.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pwrpy-1.1.3/src/pwrpy/signer.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 pwrpy-1.1.3/src/pwrpy/models/Block.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pwrpy-1.1.3/src/pwrpy/models/Delegator.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pwrpy-1.1.3/src/pwrpy/models/Transactions.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 pwrpy-1.1.3/src/pwrpy/models/TransferTxn.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 pwrpy-1.1.3/src/pwrpy/models/Validator.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 pwrpy-1.1.3/src/pwrpy/models/VmDataTxn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pwrpy-1.1.3/src/pwrpy/models/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 pwrpy-1.1.3/tests/test_demo.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pwrpy-1.1.3/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pwrpy-1.1.3/LICENSE
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 pwrpy-1.1.3/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 pwrpy-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pwrpy-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pwrpy-1.1.4/app.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 pwrpy-1.1.4/requirements.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pwrpy-1.1.4/scripts.txt
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pwrpy-1.1.4/.vscode/launch.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/__init__.py
+-rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/pwrapisdk.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/pwrwallet.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/signer.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/Block.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/Delegator.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/Transactions.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/TransferTxn.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/Validator.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/VmDataTxn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 pwrpy-1.1.4/tests/test_pwrpy.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pwrpy-1.1.4/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pwrpy-1.1.4/LICENSE
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pwrpy-1.1.4/README.md
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pwrpy-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pwrpy-1.1.4/PKG-INFO
```

### Comparing `pwrpy-1.1.3/app.py` & `pwrpy-1.1.4/app.py`

 * *Files identical despite different names*

### Comparing `pwrpy-1.1.3/requirements.txt` & `pwrpy-1.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `pwrpy-1.1.3/src/pwrpy/pwrapisdk.py` & `pwrpy-1.1.4/src/pwrpy/pwrapisdk.py`

 * *Files identical despite different names*

### Comparing `pwrpy-1.1.3/src/pwrpy/pwrwallet.py` & `pwrpy-1.1.4/src/pwrpy/pwrwallet.py`

 * *Files identical despite different names*

### Comparing `pwrpy-1.1.3/src/pwrpy/signer.py` & `pwrpy-1.1.4/src/pwrpy/signer.py`

 * *Files identical despite different names*

### Comparing `pwrpy-1.1.3/src/pwrpy/models/Block.py` & `pwrpy-1.1.4/src/pwrpy/models/Block.py`

 * *Files identical despite different names*

### Comparing `pwrpy-1.1.3/src/pwrpy/models/Delegator.py` & `pwrpy-1.1.4/src/pwrpy/models/Delegator.py`

 * *Files identical despite different names*

### Comparing `pwrpy-1.1.3/src/pwrpy/models/Transactions.py` & `pwrpy-1.1.4/src/pwrpy/models/Transactions.py`

 * *Files identical despite different names*

### Comparing `pwrpy-1.1.3/src/pwrpy/models/Validator.py` & `pwrpy-1.1.4/src/pwrpy/models/Validator.py`

 * *Files identical despite different names*

### Comparing `pwrpy-1.1.3/tests/test_demo.py` & `pwrpy-1.1.4/tests/test_pwrpy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 import os
 from pwrpy.pwrapisdk import PWRPY
 from pwrpy.pwrwallet import PWRWallet
 
-wallet = PWRWallet(pwrsdk=PWRPY(os.environ.get("PRC_NODE_URL")),
+wallet = PWRWallet(pwrsdk=PWRPY(),
                    private_key_hex=os.environ.get("PRIVATE_KEY_HEX"))
 
 
 def test_get_address():
     assert wallet.get_address().startswith("0x") == True
 
 
@@ -25,15 +25,15 @@
 
 
 def test_get_nonce():
     assert wallet.get_nonce() != None
 
 
 def test_transfer_pwr():
-    wallet2 = PWRWallet(pwrsdk=PWRPY(os.environ.get("PRC_NODE_URL")))
+    wallet2 = PWRWallet(pwrsdk=PWRPY())
     r = wallet.transfer_pwr(wallet2.get_address(), 1)
 
     assert r.success == True
 
 
 def test_send_vm_data_txn():
     r = wallet.send_vm_data_txn(1, [1])
@@ -42,15 +42,15 @@
         print("Txn Hash: " + r.txnHash)
     if not r.success:
         print(r.error)
     assert r.success == True
 
 
 def test_delegate():
-    wallet2 = PWRWallet(pwrsdk=PWRPY(os.environ.get("PRC_NODE_URL")))
+    wallet2 = PWRWallet(pwrsdk=PWRPY())
 
     r = wallet.delegate(wallet2.get_address(), 10000000)
     print("Nonce: " + str(wallet.get_nonce()))
 
     if not r.success:
         print(r.error)
```

### Comparing `pwrpy-1.1.3/LICENSE` & `pwrpy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pwrpy-1.1.3/pyproject.toml` & `pwrpy-1.1.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pwrpy"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="PWR Labs", email="devservices@pwrlabs.io" },
 ]
 description = "PWRPY is a Python library for interacting with the PWR network. "
 readme = "README.md"
-requires-python = ">=3.12"
+requires-python = ">=3.7.2"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `pwrpy-1.1.3/PKG-INFO` & `pwrpy-1.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: pwrpy
-Version: 1.1.3
+Version: 1.1.4
 Summary: PWRPY is a Python library for interacting with the PWR network. 
 Project-URL: Homepage, https://github.com/pwrlabs/pwrpy
 Project-URL: Issues, https://github.com/pwrlabs/pwrpy/issues
 Author-email: PWR Labs <devservices@pwrlabs.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.12
+Requires-Python: >=3.7.2
 Description-Content-Type: text/markdown
 
 # PWRPY
 
 PWRPY is a Python library for interacting with the PWR network.
 It provides an easy interface for wallet management and sending transactions on PWR.
 
 ## Installation
 
 Run: `pip install pwrpy`
-
-The library needs the `PRC_NODE_URL` environment variable set to https://pwrrpc.pwrlabs.io/.
```

