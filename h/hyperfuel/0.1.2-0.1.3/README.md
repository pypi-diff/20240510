# Comparing `tmp/hyperfuel-0.1.2.tar.gz` & `tmp/hyperfuel-0.1.3.tar.gz`

## Comparing `hyperfuel-0.1.2.tar` & `hyperfuel-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 hyperfuel-0.1.2/Cargo.toml
--rw-r--r--   0     1001      127     2983 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      699 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/.gitignore
--rw-r--r--   0     1001      127    16725 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/LICENSE
--rw-r--r--   0     1001      127      924 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/README.md
--rw-r--r--   0     1001      127     1108 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/examples/asset-id.py
--rw-r--r--   0     1001      127     1316 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/examples/predicate-root.py
--rw-r--r--   0     1001      127      517 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/examples/simple-logs.py
--rw-r--r--   0     1001      127    11709 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/hyperfuel/__init__.py
--rw-r--r--   0     1001      127      814 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/src/config.rs
--rw-r--r--   0     1001      127    14946 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/src/lib.rs
--rw-r--r--   0     1001      127     6551 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/src/query.rs
--rw-r--r--   0     1001      127     7753 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/src/response.rs
--rw-r--r--   0     1001      127    18503 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/src/types.rs
--rw-r--r--   0     1001      127     2921 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/test.py
--rw-r--r--   0     1001      127    75317 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/Cargo.lock
--rw-r--r--   0     1001      127      604 2024-05-09 11:32:32.000000 hyperfuel-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 hyperfuel-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 hyperfuel-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      127     2983 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      699 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/.gitignore
+-rw-r--r--   0     1001      127    16725 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/LICENSE
+-rw-r--r--   0     1001      127      924 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/README.md
+-rw-r--r--   0     1001      127     1068 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/examples/asset-id.py
+-rw-r--r--   0     1001      127     1316 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/examples/predicate-root.py
+-rw-r--r--   0     1001      127      517 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/examples/simple-logs.py
+-rw-r--r--   0     1001      127    11709 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/hyperfuel/__init__.py
+-rw-r--r--   0     1001      127      814 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/src/config.rs
+-rw-r--r--   0     1001      127    14946 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      127     6561 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/src/query.rs
+-rw-r--r--   0     1001      127     7753 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/src/response.rs
+-rw-r--r--   0     1001      127    18503 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/src/types.rs
+-rw-r--r--   0     1001      127     2921 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/test.py
+-rw-r--r--   0     1001      127    75317 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/Cargo.lock
+-rw-r--r--   0     1001      127      604 2024-05-10 14:51:25.000000 hyperfuel-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 hyperfuel-0.1.3/PKG-INFO
```

### Comparing `hyperfuel-0.1.2/.github/workflows/CI.yml` & `hyperfuel-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `hyperfuel-0.1.2/.gitignore` & `hyperfuel-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperfuel-0.1.2/LICENSE` & `hyperfuel-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfuel-0.1.2/README.md` & `hyperfuel-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperfuel-0.1.2/examples/asset-id.py` & `hyperfuel-0.1.3/examples/asset-id.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import hyperfuel
 from hyperfuel import InputField
 import asyncio
 
 async def main():
     client = hyperfuel.HyperfuelClient()
-    query = hyperfuel.HyperfuelClient()
 
     query = hyperfuel.Query(
         from_block=7980000,
         to_block=7980100,
         inputs=[
             hyperfuel.InputSelection(
                 asset_id=["0x0000000000000000000000000000000000000000000000000000000000000000"]
```

### Comparing `hyperfuel-0.1.2/examples/predicate-root.py` & `hyperfuel-0.1.3/examples/predicate-root.py`

 * *Files identical despite different names*

### Comparing `hyperfuel-0.1.2/examples/simple-logs.py` & `hyperfuel-0.1.3/examples/simple-logs.py`

 * *Files identical despite different names*

### Comparing `hyperfuel-0.1.2/hyperfuel/__init__.py` & `hyperfuel-0.1.3/hyperfuel/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperfuel-0.1.2/src/config.rs` & `hyperfuel-0.1.3/src/config.rs`

 * *Files 8% similar despite different names*

```diff
@@ -10,12 +10,12 @@
     pub bearer_token: Option<String>,
     /// Timout treshold for a single http request in milliseconds, default is 30 seconds (30_000ms)
     #[serde(skip_serializing_if = "Option::is_none")]
     pub http_req_timeout_millis: Option<i64>,
 }
 
 impl Config {
-    pub fn try_convert(&self) -> Result<skar_client_fuel::Config> {
+    pub fn try_convert(&self) -> Result<hyperfuel_client::Config> {
         let json = serde_json::to_vec(self).context("serialize to json")?;
         serde_json::from_slice(&json).context("parse json")
     }
 }
```

### Comparing `hyperfuel-0.1.2/src/lib.rs` & `hyperfuel-0.1.3/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use anyhow::{Context, Result};
 use arrow2::datatypes::Field;
 use arrow2::ffi;
 use arrow2::{array::StructArray, datatypes::DataType};
+use hyperfuel_client::ArrowBatch;
 use pyo3::ffi::Py_uintptr_t;
 use pyo3_asyncio::tokio::future_into_py;
 use response::{LogResponse, QueryResponseArrow, QueryResponseArrowData, QueryResponseTyped};
-use skar_client_fuel::ArrowBatch;
 use std::sync::Arc;
 
 mod config;
 mod query;
 mod response;
 mod types;
 
@@ -22,25 +22,25 @@
 
 #[pymodule]
 fn hyperfuel(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<HyperfuelClient>()
 }
 #[pyclass]
 pub struct HyperfuelClient {
-    inner: Arc<skar_client_fuel::Client>,
+    inner: Arc<hyperfuel_client::Client>,
 }
 
 impl HyperfuelClient {
     fn new_impl(config: Config) -> Result<HyperfuelClient> {
         env_logger::try_init().ok();
 
         let config = config.try_convert().context("parse config")?;
 
         Ok(HyperfuelClient {
-            inner: Arc::new(skar_client_fuel::Client::new(config).context("create client")?),
+            inner: Arc::new(hyperfuel_client::Client::new(config).context("create client")?),
         })
     }
 }
 
 #[pymethods]
 impl HyperfuelClient {
     /// Create a new client with given config
```

### Comparing `hyperfuel-0.1.2/src/query.rs` & `hyperfuel-0.1.3/src/query.rs`

 * *Files 2% similar despite different names*

```diff
@@ -149,21 +149,21 @@
     /// Maximum number of transactions that should be returned, the server might return more transactions than this number but
     ///  it won't overshoot by too much.
     #[serde(skip_serializing_if = "Option::is_none")]
     pub max_num_transactions: Option<usize>,
 }
 
 impl Query {
-    pub fn try_convert(&self) -> Result<skar_net_types_fuel::Query> {
+    pub fn try_convert(&self) -> Result<hyperfuel_net_types::Query> {
         let json = serde_json::to_vec(self).context("serialize to json")?;
         serde_json::from_slice(&json).context("parse json")
     }
 }
 
-impl TryFrom<skar_net_types_fuel::Query> for Query {
+impl TryFrom<hyperfuel_net_types::Query> for Query {
     type Error = anyhow::Error;
 
-    fn try_from(skar_query: skar_net_types_fuel::Query) -> Result<Self> {
-        let json = serde_json::to_vec(&skar_query).context("serialize query to json")?;
+    fn try_from(hyperfuel_query: hyperfuel_net_types::Query) -> Result<Self> {
+        let json = serde_json::to_vec(&hyperfuel_query).context("serialize query to json")?;
         serde_json::from_slice(&json).context("parse json")
     }
 }
```

### Comparing `hyperfuel-0.1.2/src/response.rs` & `hyperfuel-0.1.3/src/response.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+use hyperfuel_format::Hex;
 use pyo3::{pyclass, pymethods, PyObject, PyResult};
-use skar_format_fuel::Hex;
 
 use crate::types::{Block, Input, Output, Receipt, Transaction};
 
 #[pyclass]
 #[pyo3(get_all)]
 #[derive(Clone, Debug)]
 pub struct QueryResponseArrowData {
@@ -125,16 +125,16 @@
     }
 
     fn __str__(&self) -> PyResult<String> {
         Ok(format!("{:?}", self))
     }
 }
 
-impl From<skar_client_fuel::QueryResponseTyped> for QueryResponseTyped {
-    fn from(r: skar_client_fuel::QueryResponseTyped) -> Self {
+impl From<hyperfuel_client::QueryResponseTyped> for QueryResponseTyped {
+    fn from(r: hyperfuel_client::QueryResponseTyped) -> Self {
         let archive_height = r.archive_height;
         let next_block = r.next_block;
         let total_execution_time = r.total_execution_time;
         let data = QueryResponseDataTyped {
             blocks: r.data.blocks.into_iter().map(|b| b.into()).collect(),
             transactions: r.data.transactions.into_iter().map(|b| b.into()).collect(),
             receipts: r.data.receipts.into_iter().map(|b| b.into()).collect(),
@@ -222,16 +222,16 @@
     }
 
     fn __str__(&self) -> PyResult<String> {
         Ok(format!("{:?}", self))
     }
 }
 
-impl From<skar_client_fuel::LogResponse> for LogResponse {
-    fn from(r: skar_client_fuel::LogResponse) -> Self {
+impl From<hyperfuel_client::LogResponse> for LogResponse {
+    fn from(r: hyperfuel_client::LogResponse) -> Self {
         let archive_height = r.archive_height;
         let next_block = r.next_block;
         let total_execution_time = r.total_execution_time;
         let data = r
             .data
             .into_iter()
             .map(|c| LogContext {
```

### Comparing `hyperfuel-0.1.2/src/types.rs` & `hyperfuel-0.1.3/src/types.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+use hyperfuel_format::Hex;
 use pyo3::{pyclass, pymethods, PyResult};
-use skar_format_fuel::Hex;
 
 /// The block header contains metadata about a certain block.
 #[pyclass]
 #[pyo3(get_all)]
 #[derive(Debug, Default, Clone, PartialEq, Eq)]
 pub struct Block {
     /// String of the header
@@ -295,16 +295,16 @@
     }
 
     fn __str__(&self) -> PyResult<String> {
         Ok(format!("{:?}", self))
     }
 }
 
-impl From<skar_format_fuel::BlockHeader> for Block {
-    fn from(b: skar_format_fuel::BlockHeader) -> Self {
+impl From<hyperfuel_format::BlockHeader> for Block {
+    fn from(b: hyperfuel_format::BlockHeader) -> Self {
         Self {
             id: b.id.encode_hex(),
             da_height: b.da_height.into(),
             transactions_count: b.transactions_count.encode_hex(),
             message_receipt_count: b.message_receipt_count.encode_hex(),
             transactions_root: b.transactions_root.encode_hex(),
             message_receipt_root: b.message_receipt_root.encode_hex(),
@@ -312,16 +312,16 @@
             prev_root: b.prev_root.encode_hex(),
             time: b.time.into(),
             application_hash: b.application_hash.encode_hex(),
         }
     }
 }
 
-impl From<skar_format_fuel::Transaction> for Transaction {
-    fn from(t: skar_format_fuel::Transaction) -> Self {
+impl From<hyperfuel_format::Transaction> for Transaction {
+    fn from(t: hyperfuel_format::Transaction) -> Self {
         Self {
             block_height: t.block_height.into(),
             id: t.id.encode_hex(),
             input_asset_ids: t
                 .input_asset_ids
                 .map(|d| d.into_iter().map(|i| i.encode_hex()).collect()),
             input_contracts: t
@@ -358,16 +358,16 @@
             bytecode_witness_index: t.bytecode_witness_index.map(|d| d.into()),
             bytecode_length: t.bytecode_length.map(|d| d.into()),
             salt: t.salt.map(|d| d.encode_hex()),
         }
     }
 }
 
-impl From<skar_format_fuel::Receipt> for Receipt {
-    fn from(r: skar_format_fuel::Receipt) -> Self {
+impl From<hyperfuel_format::Receipt> for Receipt {
+    fn from(r: hyperfuel_format::Receipt) -> Self {
         Self {
             receipt_index: r.receipt_index.into(),
             root_contract_id: r.root_contract_id.map(|d| d.encode_hex()),
             tx_id: r.tx_id.encode_hex(),
             block_height: r.block_height.into(),
             pc: r.pc.map(|d| d.into()),
             is: r.is.map(|d| d.into()),
@@ -396,16 +396,16 @@
             nonce: r.nonce.map(|d| d.encode_hex()),
             contract_id: r.contract_id.map(|d| d.encode_hex()),
             sub_id: r.sub_id.map(|d| d.encode_hex()),
         }
     }
 }
 
-impl From<skar_format_fuel::Input> for Input {
-    fn from(i: skar_format_fuel::Input) -> Self {
+impl From<hyperfuel_format::Input> for Input {
+    fn from(i: hyperfuel_format::Input) -> Self {
         Self {
             tx_id: i.tx_id.encode_hex(),
             block_height: i.block_height.into(),
             input_type: i.input_type.as_u8(),
             utxo_id: i.utxo_id.map(|d| d.encode_hex()),
             owner: i.owner.map(|d| d.encode_hex()),
             amount: i.amount.map(|d| d.into()),
@@ -423,16 +423,16 @@
             recipient: i.recipient.map(|d| d.encode_hex()),
             nonce: i.nonce.map(|d| d.encode_hex()),
             data: i.data.map(|d| d.encode_hex()),
         }
     }
 }
 
-impl From<skar_format_fuel::Output> for Output {
-    fn from(r: skar_format_fuel::Output) -> Self {
+impl From<hyperfuel_format::Output> for Output {
+    fn from(r: hyperfuel_format::Output) -> Self {
         Self {
             tx_id: r.tx_id.encode_hex(),
             block_height: r.block_height.into(),
             output_type: r.output_type.as_u8(),
             to: r.to.map(|d| d.encode_hex()),
             amount: r.amount.map(|d| d.into()),
             asset_id: r.asset_id.map(|d| d.encode_hex()),
```

### Comparing `hyperfuel-0.1.2/test.py` & `hyperfuel-0.1.3/test.py`

 * *Files identical despite different names*

### Comparing `hyperfuel-0.1.2/Cargo.lock` & `hyperfuel-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1151,34 +1151,98 @@
  "rustls",
  "tokio",
  "tokio-rustls",
 ]
 
 [[package]]
 name = "hyperfuel"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "anyhow",
  "arrow2",
  "dict_derive",
  "env_logger",
  "faster-hex",
+ "hyperfuel-client",
+ "hyperfuel-format",
+ "hyperfuel-net-types",
  "itertools 0.12.1",
  "prefix-hex",
  "pyo3",
  "pyo3-asyncio",
  "serde",
  "serde_json",
- "skar-client-fuel",
- "skar-format-fuel",
- "skar-net-types-fuel",
  "tokio",
 ]
 
 [[package]]
+name = "hyperfuel-client"
+version = "0.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0fd01a1c647f1ed619c2b734e19db1cc5ba50da560f309fcd878b3b94babab5c"
+dependencies = [
+ "alloy-dyn-abi",
+ "alloy-json-abi",
+ "anyhow",
+ "arrayvec",
+ "arrow2",
+ "capnp",
+ "fastrange-rs",
+ "futures",
+ "hyperfuel-format",
+ "hyperfuel-net-types",
+ "hyperfuel-schema",
+ "log",
+ "rand",
+ "reqwest",
+ "serde",
+ "serde_json",
+ "tokio",
+ "tokio-util",
+ "url",
+ "xxhash-rust",
+]
+
+[[package]]
+name = "hyperfuel-format"
+version = "0.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "349dbdda23441b38f48555f72e82af522e34aa67072776ee6dbc99e5ff1ae614"
+dependencies = [
+ "arrayvec",
+ "derive_more",
+ "faster-hex",
+ "serde",
+ "thiserror",
+]
+
+[[package]]
+name = "hyperfuel-net-types"
+version = "0.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "daf7ac78f60db4327c69b2833bde4fc6c4304de068a798dec830560080179fbf"
+dependencies = [
+ "arrayvec",
+ "capnp",
+ "capnpc",
+ "hyperfuel-format",
+ "serde",
+]
+
+[[package]]
+name = "hyperfuel-schema"
+version = "0.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c4ee2a2ac4d968d73056a67395fd234bfb67a35571bc90e9cfa1ae2e735f696c"
+dependencies = [
+ "anyhow",
+ "arrow2",
+]
+
+[[package]]
 name = "idna"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
@@ -2203,78 +2267,14 @@
 [[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
-name = "skar-client-fuel"
-version = "0.0.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f575c142d1433dc4b45f390ce6592adca4bac974ebc64c3fb641699b8304d2b0"
-dependencies = [
- "alloy-dyn-abi",
- "alloy-json-abi",
- "anyhow",
- "arrayvec",
- "arrow2",
- "capnp",
- "fastrange-rs",
- "futures",
- "log",
- "rand",
- "reqwest",
- "serde",
- "serde_json",
- "skar-format-fuel",
- "skar-net-types-fuel",
- "skar-schema-fuel",
- "tokio",
- "tokio-util",
- "url",
- "xxhash-rust",
-]
-
-[[package]]
-name = "skar-format-fuel"
-version = "0.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a778e4a92ad675cc4dab3fdd6e3bc5773bd869b016981847810cd80420b52e68"
-dependencies = [
- "arrayvec",
- "derive_more",
- "faster-hex",
- "serde",
- "thiserror",
-]
-
-[[package]]
-name = "skar-net-types-fuel"
-version = "0.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db34cb9577e7f688d53f847591a9c09e41d9d938362a8ff0c4a5f8ef683df76"
-dependencies = [
- "arrayvec",
- "capnp",
- "capnpc",
- "serde",
- "skar-format-fuel",
-]
-
-[[package]]
-name = "skar-schema-fuel"
-version = "0.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e5d04f359bba0ce6410346eb31c3a8e78c6a6e7335202f23cbee92a38b63117"
-dependencies = [
- "anyhow",
- "arrow2",
-]
-
-[[package]]
 name = "slab"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
```

### Comparing `hyperfuel-0.1.2/pyproject.toml` & `hyperfuel-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyperfuel-0.1.2/PKG-INFO` & `hyperfuel-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hyperfuel
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: strenum >=0.4.15, <0.4.16
```

