# Comparing `tmp/pwrpy-1.1.4.tar.gz` & `tmp/pwrpy-5.0.5.tar.gz`

## Comparing `pwrpy-1.1.4.tar` & `pwrpy-5.0.5.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pwrpy-1.1.4/app.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 pwrpy-1.1.4/requirements.txt
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pwrpy-1.1.4/scripts.txt
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pwrpy-1.1.4/.vscode/launch.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/__init__.py
--rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/pwrapisdk.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/pwrwallet.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/signer.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/Block.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/Delegator.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/Transactions.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/TransferTxn.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/Validator.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/VmDataTxn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pwrpy-1.1.4/src/pwrpy/models/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 pwrpy-1.1.4/tests/test_pwrpy.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pwrpy-1.1.4/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pwrpy-1.1.4/LICENSE
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pwrpy-1.1.4/README.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pwrpy-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pwrpy-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pwrpy-5.0.5/scripts.txt
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pwrpy-5.0.5/.vscode/launch.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pwrpy-5.0.5/src/pwrpy/__init__.py
+-rw-r--r--   0        0        0    16444 2020-02-02 00:00:00.000000 pwrpy-5.0.5/src/pwrpy/pwrapisdk.py
+-rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 pwrpy-5.0.5/src/pwrpy/pwrwallet.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 pwrpy-5.0.5/src/pwrpy/signer.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 pwrpy-5.0.5/src/pwrpy/models/Block.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pwrpy-5.0.5/src/pwrpy/models/Delegator.py
+-rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 pwrpy-5.0.5/src/pwrpy/models/Transaction.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 pwrpy-5.0.5/src/pwrpy/models/Validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pwrpy-5.0.5/src/pwrpy/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pwrpy-5.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 pwrpy-5.0.5/tests/test_pwrpy.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 pwrpy-5.0.5/tests/test_wallet.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pwrpy-5.0.5/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pwrpy-5.0.5/LICENSE
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 pwrpy-5.0.5/README.md
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 pwrpy-5.0.5/pyproject.toml
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 pwrpy-5.0.5/PKG-INFO
```

### Comparing `pwrpy-1.1.4/src/pwrpy/pwrapisdk.py` & `pwrpy-5.0.5/src/pwrpy/pwrapisdk.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,333 +1,438 @@
-import os
-import requests
+import hashlib
 import json
+import requests
+from requests.exceptions import Timeout, RequestException
 from binascii import hexlify
 
+from pwrpy.models.Transaction import TxnForGuardianApproval
+from pwrpy.models.Transaction import Transaction
+from pwrpy.models.Transaction import VmDataTxn
 from pwrpy.models.Block import Block
-from pwrpy.models.Transactions import Transaction
 from pwrpy.models.Validator import Validator
 
 
 class ApiResponse:
     def __init__(self, success, message, data=None):
         self.success = success
         self.message = message
         self.data = data
 
 
+def get_response(url: str, timeout: int = 5):
+    """
+    Fetch a Response object from the given URL.
+
+    Args:
+        url (str): The URL to fetch the JSON object from.
+        timeout (int): Timeout for the HTTP request in seconds. Default is 10 seconds.
+
+    Returns:
+        Response: The response object containing the HTTP response from the server.
+    """
+    try:
+        headers = {
+            "Accept": "application/json",
+            "Content-type": "application/json"
+        }
+        response = requests.get(url, timeout=timeout, headers=headers)
+        response.raise_for_status()
+        return response
+    except Timeout:
+        print("Request timed out.")
+        # Handle timeout error as needed
+
+    except RequestException as e:
+        print("Request error:", e)
+        # Handle other request exceptions (e.g., connection errors)
+
+    except Exception as e:
+        print("An unexpected error occurred:", e)
+
+
 class PWRPY:
-    __rpc_node_url = "https://pwrrpc.pwrlabs.io/"
-    __fee_per_byte = 100
+    def __init__(self):
+        self.__rpc_node_url = "https://pwrrpc.pwrlabs.io/"
+        self.__chainId = b'-1'  # The chain ID is set to -1 until fetched from the rpc_node_url
+        self.__fee_per_byte = 0
+
+    def get_chainId(self):
+        if self.__chainId == b'-1':
+            url = self.__rpc_node_url + "/chainId/"
+            response = get_response(url)
+            chainID = response.json()["chainId"].to_bytes(1, byteorder='big')
+            return chainID
 
     def get_rpc_node_url(self):
         return self.__rpc_node_url
 
-    def get_fee_per_byte(self):
-        return self.__fee_per_byte
-
     def set_rpc_node_url(self, url):
         self.__rpc_node_url = url
 
+    def get_fee_per_byte(self):
+        if self.__fee_per_byte == 0:
+            url = self.__rpc_node_url + "/feePerByte/"
+            response = get_response(url)
+            data = response.json()
+            fee = data.get('feePerByte')
+            self.__fee_per_byte = fee
+            return fee
+
+    def get_blockchain_version(self):
+        url = f"{self.__rpc_node_url}/blockchainVersion/"
+        response = get_response(url)
+        data = response.json()
+        version = data.get('blockchainVersion')
+        return version
+
     def broadcast_txn(self, txn):
         try:
-            url = self.get_rpc_node_url() + "/broadcast/"
-            headers = {
-                "Accept": "application/json",
-                "Content-type": "application/json"
+            timeout = 3
+            url = self.__rpc_node_url + "/broadcast/"
+            data = {
+                "txn": txn.hex()
             }
-            payload = json.dumps({"txn": hexlify(txn).decode()})
-
-            responseRaw = requests.post(url, data=payload, headers=headers)
 
-            response = responseRaw.json()
-            is_ok = responseRaw.status_code == 200
-
-            return ApiResponse(is_ok, response.get("message"))
-
-        except Exception as e:
-            return ApiResponse(False, str(e))
-
-    def get_nonce_of_address(self, address):
-        try:
-            url = self.get_rpc_node_url() + "/nonceOfUser/?userAddress=" + address
             headers = {
                 "Accept": "application/json",
-                "Content-type": "application/json"
+                "Content-Type": "application/json"
             }
 
-            responseRaw = requests.get(url, headers=headers)
-
-            response = responseRaw.json()
+            response = requests.post(url, json=data, headers=headers, timeout=timeout)
 
-            if responseRaw.status_code != 200:
-                return ApiResponse(False, response.get("message"))
+            if response.status_code == 200:
+                txnHash = "0x" + hashlib.sha3_256(txn).hexdigest()
+                return ApiResponse(True,  None, bytes.fromhex(txnHash[2:]))
+            elif response.status_code == 400:
+                error_message = json.loads(response.text)["message"]
+                print("broadcast response:", response.text)
+                return ApiResponse(False, error_message, None, )
             else:
-                return ApiResponse(True, response.get("message"), response.get("nonce"))
+                raise RuntimeError("Failed with HTTP error code: " + str(response.status_code))
 
         except Exception as e:
-            return ApiResponse(False, str(e))
+            return ApiResponse(False, None, str(e))
 
-    def get_balance_of_address(self, address):
+    def get_nonce_of_address(self, address: str):
         try:
-            url = self.get_rpc_node_url() + "/balanceOf/?userAddress=" + address
-            headers = {
-                "Accept": "application/json",
-                "Content-type": "application/json"
-            }
-
-            responseRaw = requests.get(url, headers=headers)
-
+            url = self.get_rpc_node_url() + "/nonceOfUser/?userAddress=" + address
+            responseRaw = get_response(url)
             response = responseRaw.json()
 
             if responseRaw.status_code != 200:
                 return ApiResponse(False, response.get("message"))
             else:
-                return ApiResponse(True, response.get("message"), response.get("balance"))
+                return ApiResponse(True, response.get("message"), response.get("nonce"))
 
         except Exception as e:
             return ApiResponse(False, str(e))
 
+    def get_balance_of_address(self, address: str):
+        url = self.get_rpc_node_url() + "/balanceOf/?userAddress=" + address
+        response = get_response(url)
+        data = response.json()
+        balance = data.get('balance') / (10 ** 9)
+        return balance
+
+    def get_guardian_of_address(self, address: str):
+        url = f"{self.__rpc_node_url}/guardianOf/?userAddress={address}"
+        response = get_response(url)
+        data = response.json()
+        if data.get('isGuarded') == 'true':
+            return data.get('guardian')
+        else:
+            return None
+
     def get_blocks_count(self):
-        try:
-            url = self.get_rpc_node_url() + "/blocksCount/"
-            headers = {
-                "Accept": "application/json",
-                "Content-type": "application/json"
-            }
+        url = self.get_rpc_node_url() + "/blocksCount/"
+        response = get_response(url)
+        data = response.json()
+        return data.get('blocksCount')
 
-            responseRaw = requests.get(url, headers=headers)
+    def get_block_by_number(self, block_number):
+        url = f"{self.__rpc_node_url}/block/?blockNumber={block_number}"
+        response = get_response(url)
+        data = response.json()
+        block = Block.from_json(data)
+        return block
 
+    def get_total_validators_count(self):
+        try:
+            url = self.get_rpc_node_url() + "/totalValidatorsCount/"
+            responseRaw = get_response(url)
             response = responseRaw.json()
 
             if responseRaw.status_code != 200:
-                return ApiResponse(False, response.get("message"))
+                return response.get("message")
             else:
-                return ApiResponse(True, response.get("message"), response.get("blocksCount"))
+                return response.get("validatorsCount")
 
         except Exception as e:
-            return ApiResponse(False, str(e))
-
-    def get_block_by_number(self, block_number):
-        try:
-            url = self.get_rpc_node_url()
-            response = requests.get(
-                f"{url}/block/?blockNumber={block_number}")
-
-            if response.status_code == 200:
-                json_data = response.json().get('block')
-                # Assuming the Block constructor takes the JSON data directly
-
-                block_instance = Block(
-                    transaction_count=json_data['transactionCount'],
-                    size=json_data['blockSize'],
-                    number=json_data['blockNumber'],
-                    reward=json_data['blockReward'],
-                    timestamp=json_data['timestamp'],
-                    hash=json_data['blockHash'],
-                    submitter=json_data['blockSubmitter'],
-                    success=json_data['success'],
-                    transactions=[Transaction(size=txn['size'], hash=txn['hash'], fee=txn['fee'], from_address=txn['from'], to=txn['to'],
-                                              nonce_or_validation_hash=txn['nonceOrValidationHash'], position_in_the_block=txn['positionInTheBlock'], type=txn['type']) for txn in json_data['transactions']]
-                )
-
-                return block_instance
-            elif response.status_code == 400:
-                error_data = response.json()
-                raise RuntimeError(f"Failed with HTTP error 400 and message: {
-                                   error_data.get('message')}")
-            else:
-                raise RuntimeError(f"Failed with HTTP error code : {
-                                   response.status_code}")
-
-        except requests.HTTPError as http_err:
-            raise RuntimeError(f"HTTP error occurred: {http_err}")
-        except Exception as err:
-            raise RuntimeError(f"An error occurred: {err}")
+            return str(e)
 
-    def get_total_validators_count(self):
+    def get_total_delegators_count(self):
         try:
-            url = self.get_rpc_node_url() + "/totalValidatorsCount/"
-            headers = {
-                "Accept": "application/json",
-                "Content-type": "application/json"
-            }
-
-            responseRaw = requests.get(url, headers=headers)
-
+            url = self.get_rpc_node_url() + "/totalDelegatorsCount/"
+            responseRaw = get_response(url)
             response = responseRaw.json()
 
             if responseRaw.status_code != 200:
-                return ApiResponse(False, response.get("message"))
+                return response.get("message")
             else:
-                return ApiResponse(True, response.get("message"), response.get("validatorsCount"))
+                return response.get("validatorsCount")
 
         except Exception as e:
-            return ApiResponse(False, str(e))
+            return str(e)
 
     def get_standby_validators_count(self):
         try:
             url = self.get_rpc_node_url() + "/standbyValidatorsCount/"
-            headers = {
-                "Accept": "application/json",
-                "Content-type": "application/json"
-            }
-
-            responseRaw = requests.get(url, headers=headers)
-
+            responseRaw = get_response(url)
             response = responseRaw.json()
 
             if responseRaw.status_code != 200:
-                return ApiResponse(False, response.get("message"))
+                return response.get("message")
             else:
-                return ApiResponse(True, response.get("message"), response.get("validatorsCount"))
+                return response.get("validatorsCount")
 
         except Exception as e:
-            return ApiResponse(False, str(e))
+            return str(e)
 
     def get_active_validators_count(self):
         try:
             url = self.get_rpc_node_url() + "/activeValidatorsCount/"
-            headers = {
-                "Accept": "application/json",
-                "Content-type": "application/json"
-            }
-
-            responseRaw = requests.get(url, headers=headers)
-
+            responseRaw = requests.get(url)
             response = responseRaw.json()
 
             if responseRaw.status_code != 200:
-                return ApiResponse(False, response.get("message"))
+                return response.get("message")
             else:
-                return ApiResponse(True, response.get("message"), response.get("validatorsCount"))
+                return response.get("validatorsCount")
 
         except Exception as e:
-            return ApiResponse(False, str(e))
+            return str(e)
 
     def get_all_validators(self):
         try:
-            response = requests.get(
-                self.get_rpc_node_url() + "/allValidators/")
-
+            url = self.get_rpc_node_url() + "/allValidators/"
+            response = get_response(url)
             if response.status_code == 200:
                 data = response.json()
                 validators = data['validators']
                 validators_list = []
 
                 for validator_data in validators:
-                    # Assuming Validator is a class you have defined elsewhere
                     validator = Validator(
-                        "0x" + validator_data.get("address"),
+                        validator_data.get("address"),
                         validator_data.get("ip"),
-                        validator_data.get("badActor"),
-                        validator_data.get("votingPower"),
-                        validator_data.get("totalShares"),
-                        validator_data.get("delegatorsCount"),
-                        validator_data.get("status")
+                        validator_data.get("badActor", False),
+                        validator_data.get("votingPower", 0),
+                        validator_data.get("totalShares", 0),
+                        validator_data.get("delegatorsCount", 0),
+                        validator_data.get("status", 'unknown')
                     )
                     validators_list.append(validator)
 
                 return validators_list
             else:
-                return ApiResponse(False, response.get("message"))
+                return response.get("message")
 
         except Exception as e:
-            return ApiResponse(False, str(e))
+            return str(e)
 
     def get_standby_validators(self):
         try:
-            url = self.get_rpc_node_url()
-            response = requests.get(url + "/standbyValidators/")
-
+            url = self.get_rpc_node_url() + "/standbyValidators/"
+            response = get_response(url)
             if response.status_code == 200:
                 data = response.json()
                 validators = data['validators']
                 validators_list = []
-
                 for validator_data in validators:
                     # Assuming Validator is a class you have defined elsewhere
                     validator = Validator(
-                        "0x" + validator_data.get("address"),
+                        validator_data.get("address"),
                         validator_data.get("ip"),
-                        validator_data.get("badActor"),
-                        validator_data.get("votingPower"),
-                        validator_data.get("totalShares"),
-                        validator_data.get("delegatorsCount"),
-                        validator_data.get("status")
+                        validator_data.get("badActor", False),
+                        validator_data.get("votingPower", 0),
+                        validator_data.get("totalShares", 0),
+                        validator_data.get("delegatorsCount", 0),
+                        validator_data.get("status", 'unknown')
                     )
                     validators_list.append(validator)
-
                 return validators_list
             else:
-                return ApiResponse(False, response.get("message"))
+                return response.get('message')
 
         except Exception as e:
-            return ApiResponse(False, str(e))
+            return str(e)
 
     def get_active_validators(self):
         try:
-            url = self.get_rpc_node_url()
-            response = requests.get(
-                url + "/activeValidators/")
+            url = self.get_rpc_node_url() + "/activeValidators/"
+            response = get_response(url)
 
             if response.status_code == 200:
                 data = response.json()
                 validators = data['validators']
                 validators_list = []
 
                 for validator_data in validators:
                     # Assuming Validator is a class you have defined elsewhere
                     validator = Validator(
-                        "0x" + validator_data.get("address"),
+                        validator_data.get("address"),
                         validator_data.get("ip"),
-                        validator_data.get("badActor"),
-                        validator_data.get("votingPower"),
-                        validator_data.get("totalShares"),
-                        validator_data.get("delegatorsCount"),
-                        validator_data.get("status")
+                        validator_data.get("badActor", False),
+                        validator_data.get("votingPower", 0),
+                        validator_data.get("totalShares", 0),
+                        validator_data.get("delegatorsCount", 0),
+                        validator_data.get("status", 'unknown')
                     )
                     validators_list.append(validator)
 
                 return validators_list
             else:
-                return ApiResponse(False, response.get("message"))
+                return response.get("message")
 
         except Exception as e:
-            return ApiResponse(False, str(e))
+            return str(e)
 
     def get_owner_of_vm(self, vm_id):
         try:
-            url = self.get_rpc_node_url()
-            response = requests.get(
-                f"{url}/ownerOfVmId/?vmId={vm_id}")
+            url = f"{self.__rpc_node_url}/ownerOfVmId/?vmId={vm_id}"
+            response = get_response(url)
 
             if response.status_code == 200:
                 data = response.json()
                 return data["owner"]
             else:
-                return ApiResponse(False, response.get("message"))
+                return response.get("message")
 
         except Exception as e:
-            return ApiResponse(False, str(e))
+            return str(e)
 
     def update_fee_per_byte(self):
         try:
-            url = self.get_rpc_node_url()
-            response = requests.get(f"{url}/feePerByte/")
+            url = f"{self.get_rpc_node_url()}/feePerByte/"
+            response = get_response(url)
 
             if response.status_code == 200:
                 data = response.json()
                 self.__fee_per_byte = data["feePerByte"]
                 return self.__fee_per_byte
             else:
-                return ApiResponse(False, response.get("message"))
+                return response.get("message")
 
         except Exception as e:
-            return ApiResponse(False, str(e))
+            return str(e)
 
     def get_latest_block_number(self):
-        response = self.get_blocks_count()
-        if not response.success:
-            return ApiResponse(False, response.get("message"))
+        latest_block_number = self.get_blocks_count() - 1
+        return latest_block_number
+
+    def get_vm_data_txns(self, starting_block: int, ending_block: int, vm_id: int):
+        url = f"{self.__rpc_node_url}/getVmTransactions/?startingBlock={starting_block}&endingBlock={ending_block}&vmId={vm_id}"
+        response = get_response(url)
+        if response.status_code == 200:
+            data = response.json()
+            vmDataTxn = data.get('transactions')
+            txn_array = []
+            for txn_object in vmDataTxn:
+                txn = VmDataTxn.from_json(txn_object)
+                txn_array.append(txn)
+            return txn_array
+
+    def get_vm_data_txns_filter_by_byte_prefix(self, starting_block: int, ending_block: int, vm_id: int,
+                                               prefix: bytearray):
+        url = f"{self.get_rpc_node_url()}/getVmTransactionsSortByBytePrefix/?startingBlock={starting_block}&endingBlock={ending_block}&vmId={vm_id}&bytePrefix={hexlify(prefix).decode()}"
+        response = get_response(url)
+
+        if response.status_code == 200:
+            data = response.json()
+            vmDataTxn = data.get('transactions')
+            txn_array = []
+            for txn_object in vmDataTxn:
+                txn = VmDataTxn.from_json(txn_object)
+                txn_array.append(txn)
+
+            return txn_array
+        else:
+            return response.message
+
+    def get_active_voting_power(self):
+        url = f"{self.__rpc_node_url}/activeVotingPower/"
+        response = get_response(url)
+        data = response.json()
+        return data.get('activeVotingPower')
+
+    def get_delegatees(self, address: str):
+        url = f"{self.__rpc_node_url}/delegateesOfUser/?userAddress={address}"
+        response = get_response(url)
+        data = response.json()
+        validator_objects = data.get('delegatees')
+        delegatees = []
+        for validator_object in validator_objects:
+            validator = Validator(
+                address= validator_object.get('address'),
+                ip=validator_object.get('ip'),
+                bad_actor=validator_object.get('badActor'),
+                voting_power=validator_object.get('votingPower'),
+                shares=validator_object.get('totalShares'),
+                delegators_count=validator_object.get('delegatorsCount'),
+                status=validator_object.get('status')
+            )
+            delegatees.append(validator)
+        return delegatees
+
+    def get_validator(self, address: str):
+        url = f"{self.__rpc_node_url}/validator/?validatorAddress={address}"
+        response = get_response(url)
+        data = response.json()
+        validator_object = data.get('validator')
+        validator = Validator(
+            address= validator_object.get('address'),
+            ip=validator_object.get('ip'),
+            bad_actor=validator_object.get('badActor'),
+            voting_power=validator_object.get('votingPower'),
+            shares=validator_object.get('totalShares'),
+            delegators_count=validator_object.get('delegatorsCount'),
+            status=validator_object.get('status')
+        )
+        return validator
+
+    def get_delegated_pwr(self, delegator_address: str, validator_address: str):
+        url = f"{self.__rpc_node_url}/validator/delegator/delegatedPWROfAddress/?userAddress={delegator_address}&validatorAddress={validator_address}"
+        response = get_response(url)
+        data = response.json()
+        return data.get('delegatedPWR')
+
+    def get_share_value(self, validator_address: str):
+        url = f"{self.__rpc_node_url}/validator/shareValue/?validatorAddress={validator_address}"
+        response = get_response(url)
+        data = response.json()
+        return data.get('shareValue')
+
+    def is_transaction_valid_for_guardian_approval(self, txn):
+        try:
+            if type(txn) in [bytes, bytearray]:
+                txn = txn.hex()
+
+            timeout = 3
+            url = f"{self.__rpc_node_url}/isTransactionValidForGuardianApproval/"
+            data = {
+                "txn": txn
+            }
+            headers = {
+                "Accept": "application/json",
+                "Content-Type": "application/json"
+            }
 
-        return ApiResponse(True, None, response.data - 1)
+            response = requests.post(url, json=data, headers=headers, timeout=timeout)
+            data = response.json()
+            is_valid = data.get('valid')
+            if is_valid:
+                return TxnForGuardianApproval(is_valid, None, Transaction.from_json(data))
+            else:
+                raise RuntimeError("Failed with HTTP error code: " + str(response.status_code))
+
+        except Exception as e:
+            print(f"An error occurred: {e}")
```

### Comparing `pwrpy-1.1.4/src/pwrpy/signer.py` & `pwrpy-5.0.5/src/pwrpy/signer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import coincurve
-from Crypto.Hash import keccak
+from crypto.Hash import keccak
 
 
 class Signature:
 
     @staticmethod
     def sign_message_hex(private_key_hex, message):
         private_key_bytes = bytes.fromhex(private_key_hex)
```

### Comparing `pwrpy-1.1.4/src/pwrpy/models/Delegator.py` & `pwrpy-5.0.5/src/pwrpy/models/Delegator.py`

 * *Files identical despite different names*

### Comparing `pwrpy-1.1.4/src/pwrpy/models/Validator.py` & `pwrpy-5.0.5/src/pwrpy/models/Validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,18 +59,16 @@
                         "0x" + delegator_address, self._address, shares, delegated_pwr)
                     delegators_list.append(delegator)
 
                 return delegators_list
             elif response.status_code == 400:
                 # If the response was a client error, raise an exception
                 data = response.json()
-                raise RuntimeError(f"Failed with HTTP error 400 and message: {
-                                   data['message']}")
+                raise RuntimeError(f"Failed with HTTP error 400 and message: {data['message']}")
             else:
                 # If the response was another kind of error, raise an exception
-                raise RuntimeError(f"Failed with HTTP error code: {
-                                   response.status_code}")
+                raise RuntimeError(f"Failed with HTTP error code: {response.status_code}")
 
         except requests.HTTPError as http_err:
             raise RuntimeError(f"HTTP error occurred: {http_err}")
         except Exception as err:
             raise RuntimeError(f"An error occurred: {err}")
```

### Comparing `pwrpy-1.1.4/LICENSE` & `pwrpy-5.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pwrpy-1.1.4/PKG-INFO` & `pwrpy-5.0.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pwrpy
-Version: 1.1.4
-Summary: PWRPY is a Python library for interacting with the PWR network. 
-Project-URL: Homepage, https://github.com/pwrlabs/pwrpy
-Project-URL: Issues, https://github.com/pwrlabs/pwrpy/issues
+Version: 5.0.5
+Summary: PWRPY is a Python library for interacting with the PWR network.
+Project-URL: homepage, https://github.com/pwrlabs/pwrpy
+Project-URL: documentation, https://pwrpy.readthedocs.io/
+Project-URL: issues, https://github.com/pwrlabs/pwrpy/issues
 Author-email: PWR Labs <devservices@pwrlabs.io>
+License-Expression: MIT
 License-File: LICENSE
+Keywords: library,network,pwr,python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.2
 Description-Content-Type: text/markdown
 
 # PWRPY
```

