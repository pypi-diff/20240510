# Comparing `tmp/sourmash_plugin_directsketch-0.2.1.tar.gz` & `tmp/sourmash_plugin_directsketch-0.2.2.tar.gz`

## Comparing `sourmash_plugin_directsketch-0.2.1.tar` & `sourmash_plugin_directsketch-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,37 @@
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.2.1/Cargo.toml
--rw-r--r--   0      501       20      405 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.1/.github/dependabot.yml
--rw-r--r--   0      501       20     1474 2024-05-08 16:20:14.000000 sourmash_plugin_directsketch-0.2.1/.github/workflows/build-test.yml
--rw-r--r--   0      501       20      718 2024-04-26 03:30:23.000000 sourmash_plugin_directsketch-0.2.1/.gitignore
--rw-r--r--   0      501       20     1540 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.1/LICENSE
--rw-r--r--   0      501       20      368 2024-05-01 15:59:57.000000 sourmash_plugin_directsketch-0.2.1/Makefile
--rw-r--r--   0      501       20     2417 2024-05-01 22:22:17.000000 sourmash_plugin_directsketch-0.2.1/README.md
--rw-r--r--   0      501       20      176 2024-04-30 23:49:37.000000 sourmash_plugin_directsketch-0.2.1/environment.yml
--rw-r--r--   0      501       20    51553 2024-05-02 00:08:24.000000 sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000175555.1_assembly_report.txt
--rw-r--r--   0      501       20   798402 2024-05-02 00:08:23.000000 sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000175555.1_genomic.fna.gz
--rw-r--r--   0      501       20    36700 2024-05-02 00:08:22.000000 sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000961135.2_assembly_report.txt
--rw-r--r--   0      501       20   526013 2024-05-02 00:08:22.000000 sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000961135.2_genomic.fna.gz
--rw-r--r--   0      501       20   314606 2024-05-02 00:08:22.000000 sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000961135.2_protein.faa.gz
--rw-r--r--   0      501       20    24921 2024-05-08 21:50:14.000000 sourmash_plugin_directsketch-0.2.1/src/directsketch.rs
--rw-r--r--   0      501       20     2359 2024-05-08 18:17:29.000000 sourmash_plugin_directsketch-0.2.1/src/lib.rs
--rw-r--r--   0      501       20     4597 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.1/src/python/sourmash_plugin_directsketch/__init__.py
--rw-r--r--   0      501       20     5730 2024-05-07 17:31:28.000000 sourmash_plugin_directsketch-0.2.1/src/utils.rs
--rw-r--r--   0      501       20    38326 2024-05-08 21:42:37.000000 sourmash_plugin_directsketch-0.2.1/test.zip
--rw-r--r--   0      501       20      410 2024-05-08 18:17:29.000000 sourmash_plugin_directsketch-0.2.1/tests/conftest.py
--rw-r--r--   0      501       20     6849 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.1/tests/sourmash_tst_utils.py
--rw-r--r--   0      501       20        0 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/.notempty
--rw-r--r--   0      501       20    44471 2024-04-26 18:22:33.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/GCA_000175555.1.sig.gz
--rw-r--r--   0      501       20    20407 2024-04-27 01:42:18.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/GCA_000961135.2.protein.sig.gz
--rw-r--r--   0      501       20    29259 2024-04-26 18:04:28.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/GCA_000961135.2.sig.gz
--rw-r--r--   0      501       20      497 2024-04-27 02:01:15.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/acc.csv
--rw-r--r--   0      501       20   798402 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/out_fastas/GCA_000175555.1_genomic.fna.gz
--rw-r--r--   0      501       20   526013 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/out_fastas/GCA_000961135.2_genomic.fna.gz
--rw-r--r--   0      501       20   314606 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/out_fastas/GCA_000961135.2_protein.faa.gz
--rw-r--r--   0      501       20   798402 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000175555.1_genomic.fna.gz
--rw-r--r--   0      501       20     7793 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_assembly_report.txt
--rw-r--r--   0      501       20  1118769 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_genomic.fna.gz
--rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_md5checksums.txt
--rw-r--r--   0      501       20   702342 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_protein.faa.gz
--rw-r--r--   0      501       20    36700 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000961135.2_assembly_report.txt
--rw-r--r--   0      501       20   526013 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000961135.2_genomic.fna.gz
--rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000961135.2_md5checksums.txt
--rw-r--r--   0      501       20   314606 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000961135.2_protein.faa.gz
--rw-r--r--   0      501       20   735547 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_001950595.1_genomic.fna.gz
--rw-r--r--   0      501       20   118778 2024-04-27 00:46:05.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/test.zip
--rw-r--r--   0      501       20    11413 2024-05-06 22:31:50.000000 sourmash_plugin_directsketch-0.2.1/tests/test_gbsketch.py
--rw-r--r--   0      501       20    63427 2024-05-08 21:52:08.000000 sourmash_plugin_directsketch-0.2.1/Cargo.lock
--rw-r--r--   0      501       20     1003 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.2.2/Cargo.toml
+-rw-r--r--   0      501       20      405 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.2/.github/dependabot.yml
+-rw-r--r--   0      501       20     1474 2024-05-08 16:20:14.000000 sourmash_plugin_directsketch-0.2.2/.github/workflows/build-test.yml
+-rw-r--r--   0      501       20      718 2024-04-26 03:30:23.000000 sourmash_plugin_directsketch-0.2.2/.gitignore
+-rw-r--r--   0      501       20     1540 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.2/LICENSE
+-rw-r--r--   0      501       20      368 2024-05-01 15:59:57.000000 sourmash_plugin_directsketch-0.2.2/Makefile
+-rw-r--r--   0      501       20     3126 2024-05-09 16:57:29.000000 sourmash_plugin_directsketch-0.2.2/README.md
+-rw-r--r--   0      501       20      176 2024-04-30 23:49:37.000000 sourmash_plugin_directsketch-0.2.2/environment.yml
+-rw-r--r--   0      501       20    25928 2024-05-09 16:48:31.000000 sourmash_plugin_directsketch-0.2.2/src/directsketch.rs
+-rw-r--r--   0      501       20     2359 2024-05-08 18:17:29.000000 sourmash_plugin_directsketch-0.2.2/src/lib.rs
+-rw-r--r--   0      501       20     4597 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.2/src/python/sourmash_plugin_directsketch/__init__.py
+-rw-r--r--   0      501       20     5730 2024-05-07 17:31:28.000000 sourmash_plugin_directsketch-0.2.2/src/utils.rs
+-rw-r--r--   0      501       20      410 2024-05-08 18:17:29.000000 sourmash_plugin_directsketch-0.2.2/tests/conftest.py
+-rw-r--r--   0      501       20     6849 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.2/tests/sourmash_tst_utils.py
+-rw-r--r--   0      501       20        0 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/.notempty
+-rw-r--r--   0      501       20    44471 2024-04-26 18:22:33.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/GCA_000175555.1.sig.gz
+-rw-r--r--   0      501       20    20407 2024-04-27 01:42:18.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/GCA_000961135.2.protein.sig.gz
+-rw-r--r--   0      501       20    29259 2024-04-26 18:04:28.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/GCA_000961135.2.sig.gz
+-rw-r--r--   0      501       20      497 2024-04-27 02:01:15.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/acc.csv
+-rw-r--r--   0      501       20   798402 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/out_fastas/GCA_000175555.1_genomic.fna.gz
+-rw-r--r--   0      501       20   526013 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/out_fastas/GCA_000961135.2_genomic.fna.gz
+-rw-r--r--   0      501       20   314606 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/out_fastas/GCA_000961135.2_protein.faa.gz
+-rw-r--r--   0      501       20   798402 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000175555.1_genomic.fna.gz
+-rw-r--r--   0      501       20     7793 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000337115.1_assembly_report.txt
+-rw-r--r--   0      501       20  1118769 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000337115.1_genomic.fna.gz
+-rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000337115.1_md5checksums.txt
+-rw-r--r--   0      501       20   702342 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000337115.1_protein.faa.gz
+-rw-r--r--   0      501       20    36700 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000961135.2_assembly_report.txt
+-rw-r--r--   0      501       20   526013 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000961135.2_genomic.fna.gz
+-rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000961135.2_md5checksums.txt
+-rw-r--r--   0      501       20   314606 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000961135.2_protein.faa.gz
+-rw-r--r--   0      501       20   735547 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_001950595.1_genomic.fna.gz
+-rw-r--r--   0      501       20   118778 2024-04-27 00:46:05.000000 sourmash_plugin_directsketch-0.2.2/tests/test-data/test.zip
+-rw-r--r--   0      501       20    11422 2024-05-09 16:48:31.000000 sourmash_plugin_directsketch-0.2.2/tests/test_gbsketch.py
+-rw-r--r--   0      501       20    63427 2024-05-09 16:49:31.000000 sourmash_plugin_directsketch-0.2.2/Cargo.lock
+-rw-r--r--   0      501       20     1003 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.2.2/PKG-INFO
```

### Comparing `sourmash_plugin_directsketch-0.2.1/Cargo.toml` & `sourmash_plugin_directsketch-0.2.2/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 
 [package]
 name = "sourmash_plugin_directsketch"
-version = "0.2.1"
+version = "0.2.2"
 edition = "2021"
 
 [lib]
 name = "sourmash_plugin_directsketch"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.21.2", features = ["extension-module", "anyhow"] }
 rayon = "1.10.0"
-serde = { version = "1.0.200", features = ["derive"] }
+serde = { version = "1.0.201", features = ["derive"] }
 sourmash = { version = "0.13.1"}
-serde_json = "1.0.116"
+serde_json = "1.0.117"
 niffler = "2.4.0"
 needletail = "0.5.1"
 #zip = { version = "0.6", default-features = false, features = ["deflate"] }
 async_zip={version="0.0.17", features=["full"]}
 simple-error = "0.3.0"
-anyhow = "1.0.82"
+anyhow = "1.0.83"
 camino = "1.1.6"
 csv = "1.3.0"
 reqwest = { version = "0.12.4", features = ["json", "stream"] }
 tokio = { version = "1.37.0", features = ["full"] }
 tokio-util = "0.7.11"
 regex = "1.10.4"
 chrono = "0.4.32"
```

### Comparing `sourmash_plugin_directsketch-0.2.1/.github/workflows/build-test.yml` & `sourmash_plugin_directsketch-0.2.2/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/.gitignore` & `sourmash_plugin_directsketch-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/LICENSE` & `sourmash_plugin_directsketch-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/README.md` & `sourmash_plugin_directsketch-0.2.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # sourmash_plugin_directsketch
 
+[![PyPI](https://img.shields.io/pypi/v/sourmash_plugin_directsketch)](https://pypi.org/project/sourmash_plugin_directsketch/)
+
+
+tl;dr - download and sketch NCBI Assembly Datasets by accession
+
+## About
+
+This plugin is an attempt to improve database generation by downloading assemblies, checking md5sum, and sketching to a sourmash zipfile. FASTA files can also be saved if desired. It's quite fast, but still very much at alpha level. Here be dragons.
+
 ## Installation
 
 ```
 pip install sourmash_plugin_directsketch
 ```
 
 ## Usage
@@ -47,17 +56,25 @@
                         parameter string for sketching (default: k=31,scaled=1000)
   -c CORES, --cores CORES
                         number of cores to use (default is all available)
   -r RETRY_TIMES, --retry-times RETRY_TIMES
                         number of times to retry failed downloads
 ```
 
+## Code of Conduct
+
+This project is under the [sourmash Code of Conduct](https://github.com/sourmash-bio/sourmash/blob/latest/CODE_OF_CONDUCT.rst).
+
 ## Support
 
-We suggest filing issues in [the main sourmash issue tracker](https://github.com/dib-lab/sourmash/issues) as that receives more attention!
+We suggest filing issues in [the directsketch issue tracker](https://github.com/bluegenes/sourmash_plugin_directsketch/issues) or [the main sourmash issue tracker](https://github.com/dib-lab/sourmash/issues).
+
+## Authors
+
+* N. Tessa Pierce-Ward
 
 ## Dev docs
 
 `sourmash_plugin_directsketch` is developed at https://github.com/sourmash-bio/sourmash_plugin_directsketch.
 
 ### Testing
```

### Comparing `sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000175555.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/out_fastas/GCA_000175555.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000961135.2_assembly_report.txt` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000961135.2_assembly_report.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000961135.2_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/out_fastas/GCA_000961135.2_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000961135.2_protein.faa.gz` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/out_fastas/GCA_000961135.2_protein.faa.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/src/directsketch.rs` & `sourmash_plugin_directsketch-0.2.2/src/directsketch.rs`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 use needletail::parse_fastx_reader;
 use regex::Regex;
 use reqwest::Client;
 use std::collections::HashMap;
 use std::fs::{self, create_dir_all};
 use std::io::Cursor;
 use std::path::Path;
+use std::sync::atomic::{AtomicBool, Ordering};
 use std::sync::Arc;
 use tokio::fs::File;
 use tokio::io::{AsyncWriteExt, BufWriter};
 use tokio::sync::Semaphore;
 use tokio_util::compat::Compat;
 
 use pyo3::prelude::*;
@@ -175,14 +176,15 @@
 async fn download_with_retry(
     client: &Client,
     url: &str,
     expected_md5: Option<&str>,
     retry_count: u32,
 ) -> Result<Vec<u8>> {
     let mut attempts = retry_count;
+    let mut last_error: Option<anyhow::Error> = None;
 
     while attempts > 0 {
         let response = client.get(url).send().await;
 
         match response {
             Ok(resp) if resp.status().is_success() => {
                 let data = resp
@@ -191,39 +193,48 @@
                     .context("Failed to read bytes from response")?;
 
                 if let Some(md5) = expected_md5 {
                     let computed_hash = format!("{:x}", md5::compute(&data));
                     if computed_hash == md5 {
                         return Ok(data.to_vec());
                     } else {
-                        eprintln!(
-                            "MD5 hash does not match. Expected: {}, Found: {}. Retrying...",
-                            md5, computed_hash
-                        );
+                        last_error = Some(anyhow!(
+                            "MD5 hash does not match. Expected: {}, Found: {}",
+                            md5,
+                            computed_hash
+                        ));
                     }
                 } else {
                     return Ok(data.to_vec()); // If no expected MD5 is provided, just return the data
                 }
             }
-            _ => {
-                eprintln!("Failed to download file: {}. Retrying...", url);
+            Ok(resp) => {
+                last_error = Some(anyhow!(
+                    "Server error status code {}: {}. Retrying...",
+                    resp.status(),
+                    url
+                ));
+            }
+            Err(e) => {
+                last_error = Some(anyhow!("Failed to download file: {}. Error: {}.", url, e));
             }
         }
 
         attempts -= 1;
         if attempts == 0 {
             break;
         }
     }
-
-    Err(anyhow!(
-        "Failed to download file after {} retries: {}",
-        retry_count,
-        url
-    ))
+    Err(last_error.unwrap_or_else(|| {
+        anyhow!(
+            "Failed to download file after {} retries: {}",
+            url,
+            retry_count
+        )
+    }))
 }
 
 async fn sketch_data(
     name: String,
     filename: String,
     compressed_data: Vec<u8>,
     mut sigs: Vec<Signature>,
@@ -567,14 +578,29 @@
                 let _ = error_sender.send(error).await;
             }
         }
         drop(error_sender);
     })
 }
 
+pub fn error_handler(
+    mut recv_errors: tokio::sync::mpsc::Receiver<anyhow::Error>,
+    error_flag: Arc<AtomicBool>,
+) -> tokio::task::JoinHandle<()> {
+    tokio::spawn(async move {
+        while let Some(error) = recv_errors.recv().await {
+            eprintln!("Error: {}", error);
+            if error.to_string().contains("No signatures written") {
+                error_flag.store(true, Ordering::SeqCst);
+                break;
+            }
+        }
+    })
+}
+
 #[tokio::main]
 #[allow(clippy::too_many_arguments)]
 pub async fn download_and_sketch(
     py: Python,
     input_csv: String,
     output_sigs: String,
     param_str: String,
@@ -597,25 +623,28 @@
     let download_path = PathBuf::from(fasta_location);
     if !download_path.exists() {
         create_dir_all(&download_path)?;
     }
 
     // // create channels. buffer size can be changed - here it is 4 b/c we can do 3 downloads simultaneously
     // // to do: see whether increasing buffer size speeds things up
-    let (send_sigs, recv_sigs) = tokio::sync::mpsc::channel::<Vec<Signature>>(4);
-    let (send_failed, recv_failed) = tokio::sync::mpsc::channel::<FailedDownload>(4);
+    let (send_sigs, recv_sigs) = tokio::sync::mpsc::channel::<Vec<Signature>>(1000);
+    let (send_failed, recv_failed) = tokio::sync::mpsc::channel::<FailedDownload>(100);
     // // Error channel for handling task errors
-    let (error_sender, mut error_receiver) = tokio::sync::mpsc::channel::<anyhow::Error>(1);
+    let (error_sender, error_receiver) = tokio::sync::mpsc::channel::<anyhow::Error>(1);
 
     // //  // Set up collector/writing tasks
     let mut handles = Vec::new();
     let sig_handle = sigwriter_handle(recv_sigs, output_sigs, error_sender.clone());
     let failures_handle = failures_handle(failed_csv, recv_failed, error_sender.clone());
+    let critical_error_flag = Arc::new(AtomicBool::new(false));
+    let error_handle = error_handler(error_receiver, critical_error_flag.clone());
     handles.push(sig_handle);
     handles.push(failures_handle);
+    handles.push(error_handle);
 
     // // Worker tasks
     let semaphore = Arc::new(Semaphore::new(3)); // Limiting concurrent downloads
     let client = Arc::new(Client::new());
 
     // Open the file containing the accessions synchronously
     let (accession_info, n_accs) = load_accession_info(input_csv)?;
@@ -699,20 +728,18 @@
     // drop senders as we're done sending data
     drop(send_sigs);
     drop(send_failed);
     drop(error_sender);
     // Wait for all tasks to complete
     for handle in handles {
         if let Err(e) = handle.await {
-            eprintln!("A task encountered an error: {}", e);
+            eprintln!("Handle join error: {}.", e);
         }
     }
-    // // Handle errors received from the error channel
-    while let Some(error) = error_receiver.recv().await {
-        eprintln!("Error: {}", error);
-        // Check if the error message contains "No signatures written"
-        if error.to_string().contains("No signatures written") & !download_only {
-            bail!("{}.", error);
-        }
+    // since the only critical error is not having written any sigs
+    // check this here at end. Bail if we wrote expected sigs but wrote none.
+    if critical_error_flag.load(Ordering::SeqCst) & !download_only {
+        bail!("No signatures written, exiting.");
     }
+
     Ok(())
 }
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
 use anyhow::{anyhow, bail, Context, Error, Result}; use async_zip::base::
 write::ZipFileWriter; use async_zip::{Compression, ZipDateTime,
 ZipEntryBuilder}; use camino::Utf8PathBuf as PathBuf; use chrono::Utc; use
 needletail::parse_fastx_reader; use regex::Regex; use reqwest::Client; use
 std::collections::HashMap; use std::fs::{self, create_dir_all}; use std::io::
-Cursor; use std::path::Path; use std::sync::Arc; use tokio::fs::File; use
-tokio::io::{AsyncWriteExt, BufWriter}; use tokio::sync::Semaphore; use
-tokio_util::compat::Compat; use pyo3::prelude::*; use sourmash::manifest::
-{Manifest, Record}; use sourmash::signature::Signature; use crate::utils::
-{build_siginfo, load_accession_info, parse_params_str}; #[allow(dead_code)]
-enum GenBankFileType { Genomic, Protein, AssemblyReport, Checksum, } impl
-GenBankFileType { fn suffix(&self) -> &'static str { match self
-{ GenBankFileType::Genomic => "_genomic.fna.gz", GenBankFileType::Protein =>
-"_protein.faa.gz", GenBankFileType::AssemblyReport => "_assembly_report.txt",
-GenBankFileType::Checksum => "md5checksums.txt", } } //use for checksums fn
-server_filename(&self, full_name: &str) -> String { format!("{}{}", full_name,
-self.suffix()) } fn filename_to_write(&self, accession: &str) -> String { match
-self { GenBankFileType::Checksum => format!("{}_{}", accession, self.suffix()),
-_ => format!("{}{}", accession, self.suffix()), } } fn url(&self, base_url:
-&str, full_name: &str) -> String { match self { GenBankFileType::Checksum =>
-format!("{}/{}", base_url, self.suffix()), _ => format!("{}/{}{}", base_url,
-full_name, self.suffix()), } } fn moltype(&self) -> String { match self
-{ GenBankFileType::Genomic => "DNA".to_string(), GenBankFileType::Protein =>
-"protein".to_string(), _ => "".to_string(), } } } async fn
-fetch_genbank_filename(client: &Client, accession: &str) -> Result<(String,
-String)> { let (db, acc) = accession .trim() .split_once('_') .ok_or_else(||
-anyhow!("Invalid accession format"))?; let (number, _) = acc.split_once
-('.').unwrap_or((acc, "1")); let number_path = number .chars() .collect::
+Cursor; use std::path::Path; use std::sync::atomic::{AtomicBool, Ordering}; use
+std::sync::Arc; use tokio::fs::File; use tokio::io::{AsyncWriteExt, BufWriter};
+use tokio::sync::Semaphore; use tokio_util::compat::Compat; use pyo3::prelude::
+*; use sourmash::manifest::{Manifest, Record}; use sourmash::signature::
+Signature; use crate::utils::{build_siginfo, load_accession_info,
+parse_params_str}; #[allow(dead_code)] enum GenBankFileType { Genomic, Protein,
+AssemblyReport, Checksum, } impl GenBankFileType { fn suffix(&self) -> &'static
+str { match self { GenBankFileType::Genomic => "_genomic.fna.gz",
+GenBankFileType::Protein => "_protein.faa.gz", GenBankFileType::AssemblyReport
+=> "_assembly_report.txt", GenBankFileType::Checksum => "md5checksums.txt", } }
+//use for checksums fn server_filename(&self, full_name: &str) -> String
+{ format!("{}{}", full_name, self.suffix()) } fn filename_to_write(&self,
+accession: &str) -> String { match self { GenBankFileType::Checksum => format!
+("{}_{}", accession, self.suffix()), _ => format!("{}{}", accession,
+self.suffix()), } } fn url(&self, base_url: &str, full_name: &str) -> String
+{ match self { GenBankFileType::Checksum => format!("{}/{}", base_url,
+self.suffix()), _ => format!("{}/{}{}", base_url, full_name, self.suffix()), }
+} fn moltype(&self) -> String { match self { GenBankFileType::Genomic =>
+"DNA".to_string(), GenBankFileType::Protein => "protein".to_string(), _ =>
+"".to_string(), } } } async fn fetch_genbank_filename(client: &Client,
+accession: &str) -> Result<(String, String)> { let (db, acc) = accession .trim
+() .split_once('_') .ok_or_else(|| anyhow!("Invalid accession format"))?; let
+(number, _) = acc.split_once('.').unwrap_or((acc, "1")); let number_path =
+number .chars() .collect::
 _>>() .chunks(3) .map(|chunk| chunk.iter().collect::()) .collect::
 _>>() .join("/"); let base_url = format!( "https://ftp.ncbi.nlm.nih.gov/
 genomes/all/{}/{}", db, number_path ); let directory_response = client.get
 (&base_url).send().await; match directory_response { Ok(response) => { if
 !response.status().is_success() { return Err(anyhow!( "Failed to open genome
 directory: HTTP {}, {}", response.status(), response .status()
 .canonical_reason() .unwrap_or("Unknown reason") )); } let text = response.text
@@ -51,25 +52,28 @@
 / Trim the filename to remove any leading " ./" if present let filename = parts
 [1].trim_start_matches(" ./"); // remove any ' ', '.', '/' from front
 checksums.insert(filename.to_string(), parts[0].to_string()); } else { return
 Err(anyhow!( "Invalid checksum line format in URL {}: {}", url, line )); } } Ok
 (checksums) } // download and return data directly instead of saving to file
 async fn download_with_retry( client: &Client, url: &str, expected_md5:
 Option<&str>, retry_count: u32, ) -> Result
-u8>> { let mut attempts = retry_count; while attempts > 0 { let response =
-client.get(url).send().await; match response { Ok(resp) if resp.status
-().is_success() => { let data = resp .bytes() .await .context("Failed to read
-bytes from response")?; if let Some(md5) = expected_md5 { let computed_hash =
-format!("{:x}", md5::compute(&data)); if computed_hash == md5 { return Ok
-(data.to_vec()); } else { eprintln!( "MD5 hash does not match. Expected: {},
-Found: {}. Retrying...", md5, computed_hash ); } } else { return Ok(data.to_vec
-()); // If no expected MD5 is provided, just return the data } } _ =>
-{ eprintln!("Failed to download file: {}. Retrying...", url); } } attempts -
-= 1; if attempts == 0 { break; } } Err(anyhow!( "Failed to download file after
-{} retries: {}", retry_count, url )) } async fn sketch_data( name: String,
+u8>> { let mut attempts = retry_count; let mut last_error: Option = None; while
+attempts > 0 { let response = client.get(url).send().await; match response { Ok
+(resp) if resp.status().is_success() => { let data = resp .bytes() .await
+.context("Failed to read bytes from response")?; if let Some(md5) =
+expected_md5 { let computed_hash = format!("{:x}", md5::compute(&data)); if
+computed_hash == md5 { return Ok(data.to_vec()); } else { last_error = Some
+(anyhow!( "MD5 hash does not match. Expected: {}, Found: {}", md5,
+computed_hash )); } } else { return Ok(data.to_vec()); // If no expected MD5 is
+provided, just return the data } } Ok(resp) => { last_error = Some(anyhow!
+( "Server error status code {}: {}. Retrying...", resp.status(), url )); } Err
+(e) => { last_error = Some(anyhow!("Failed to download file: {}. Error: {}.",
+url, e)); } } attempts -= 1; if attempts == 0 { break; } } Err
+(last_error.unwrap_or_else(|| { anyhow!( "Failed to download file after {}
+retries: {}", url, retry_count ) })) } async fn sketch_data( name: String,
 filename: String, compressed_data: Vec, mut sigs: Vec, moltype: String, ) -
 > Result
 Signature>> { tokio::task::spawn_blocking(move || { let cursor = Cursor::new
 (compressed_data); let mut fastx_reader = parse_fastx_reader(cursor).context
 ("Failed to parse FASTA/FASTQ data")?; let mut set_name = false; while let Some
 (record) = fastx_reader.next() { let record = record.context("Failed to read
 record")?; sigs.iter_mut().for_each(|sig| { if !set_name { sig.set_name(&name);
@@ -177,46 +181,54 @@
 each record if let Err(e) = writer.write_all(record.as_bytes()).await { let
 error = Error::new(e).context("Failed to write record"); let _ =
 error_sender.send(error).await; continue; // Optionally continue to try to
 write next records } } // Attempt to flush the writer if let Err(e) =
 writer.flush().await { let error = Error::new(e).context("Failed to flush
 writer"); let _ = error_sender.send(error).await; } } Err(e) => { let error =
 Error::new(e).context("Failed to create file"); let _ = error_sender.send
-(error).await; } } drop(error_sender); }) } #[tokio::main] #[allow(clippy::
-too_many_arguments)] pub async fn download_and_sketch( py: Python, input_csv:
-String, output_sigs: String, param_str: String, failed_csv: String,
-retry_times: u32, fasta_location: String, keep_fastas: bool, genomes_only:
-bool, proteomes_only: bool, download_only: bool, ) -> Result<(), anyhow::Error>
-{ // if sig output doesn't end in zip, bail if Path::new(&output_sigs)
-.extension() .map_or(true, |ext| ext != "zip") { bail!("Output must be a zip
-file."); } // set up fasta download path let download_path = PathBuf::from
-(fasta_location); if !download_path.exists() { create_dir_all(&download_path)?;
-} // // create channels. buffer size can be changed - here it is 4 b/c we can
-do 3 downloads simultaneously // // to do: see whether increasing buffer size
-speeds things up let (send_sigs, recv_sigs) = tokio::sync::mpsc::channel::
-Signature>>(4); let (send_failed, recv_failed) = tokio::sync::mpsc::channel::
-(4); // // Error channel for handling task errors let (error_sender, mut
+(error).await; } } drop(error_sender); }) } pub fn error_handler( mut
+recv_errors: tokio::sync::mpsc::Receiver, error_flag: Arc, ) -> tokio::task::
+JoinHandle<()> { tokio::spawn(async move { while let Some(error) =
+recv_errors.recv().await { eprintln!("Error: {}", error); if error.to_string
+().contains("No signatures written") { error_flag.store(true, Ordering::
+SeqCst); break; } } }) } #[tokio::main] #[allow(clippy::too_many_arguments)]
+pub async fn download_and_sketch( py: Python, input_csv: String, output_sigs:
+String, param_str: String, failed_csv: String, retry_times: u32,
+fasta_location: String, keep_fastas: bool, genomes_only: bool, proteomes_only:
+bool, download_only: bool, ) -> Result<(), anyhow::Error> { // if sig output
+doesn't end in zip, bail if Path::new(&output_sigs) .extension() .map_or(true,
+|ext| ext != "zip") { bail!("Output must be a zip file."); } // set up fasta
+download path let download_path = PathBuf::from(fasta_location); if
+!download_path.exists() { create_dir_all(&download_path)?; } // // create
+channels. buffer size can be changed - here it is 4 b/c we can do 3 downloads
+simultaneously // // to do: see whether increasing buffer size speeds things up
+let (send_sigs, recv_sigs) = tokio::sync::mpsc::channel::
+Signature>>(1000); let (send_failed, recv_failed) = tokio::sync::mpsc::
+channel::(100); // // Error channel for handling task errors let (error_sender,
 error_receiver) = tokio::sync::mpsc::channel::(1); // // // Set up collector/
 writing tasks let mut handles = Vec::new(); let sig_handle = sigwriter_handle
 (recv_sigs, output_sigs, error_sender.clone()); let failures_handle =
-failures_handle(failed_csv, recv_failed, error_sender.clone()); handles.push
-(sig_handle); handles.push(failures_handle); // // Worker tasks let semaphore =
-Arc::new(Semaphore::new(3)); // Limiting concurrent downloads let client =
-Arc::new(Client::new()); // Open the file containing the accessions
-synchronously let (accession_info, n_accs) = load_accession_info(input_csv)?;
-if n_accs == 0 { bail!("No accessions to download and sketch.") } // // parse
-param string into params_vec, print error if fail let param_result =
-parse_params_str(param_str); let params_vec = match param_result { Ok(params)
-=> params, Err(e) => { bail!("Failed to parse params string: {}", e); } }; let
-dna_sig_templates = build_siginfo(&params_vec, "DNA"); let prot_sig_templates =
-build_siginfo(&params_vec, "protein"); // report every 1 percent (or every 1,
-whichever is larger) let reporting_threshold = std::cmp::max(n_accs / 100, 1);
-for (i, accinfo) in accession_info.into_iter().enumerate() { py.check_signals
-()?; // If interrupted, return an Err automatically let semaphore_clone = Arc::
-clone(&semaphore); let client_clone = Arc::clone(&client); let send_sigs =
+failures_handle(failed_csv, recv_failed, error_sender.clone()); let
+critical_error_flag = Arc::new(AtomicBool::new(false)); let error_handle =
+error_handler(error_receiver, critical_error_flag.clone()); handles.push
+(sig_handle); handles.push(failures_handle); handles.push(error_handle); // /
+/ Worker tasks let semaphore = Arc::new(Semaphore::new(3)); // Limiting
+concurrent downloads let client = Arc::new(Client::new()); // Open the file
+containing the accessions synchronously let (accession_info, n_accs) =
+load_accession_info(input_csv)?; if n_accs == 0 { bail!("No accessions to
+download and sketch.") } // // parse param string into params_vec, print error
+if fail let param_result = parse_params_str(param_str); let params_vec = match
+param_result { Ok(params) => params, Err(e) => { bail!("Failed to parse params
+string: {}", e); } }; let dna_sig_templates = build_siginfo(&params_vec,
+"DNA"); let prot_sig_templates = build_siginfo(&params_vec, "protein"); /
+/ report every 1 percent (or every 1, whichever is larger) let
+reporting_threshold = std::cmp::max(n_accs / 100, 1); for (i, accinfo) in
+accession_info.into_iter().enumerate() { py.check_signals()?; // If
+interrupted, return an Err automatically let semaphore_clone = Arc::clone
+(&semaphore); let client_clone = Arc::clone(&client); let send_sigs =
 send_sigs.clone(); let send_failed = send_failed.clone(); let
 download_path_clone = download_path.clone(); // Clone the path for each task
 let send_errors = error_sender.clone(); let dna_sigs = dna_sig_templates.clone
 (); let prot_sigs = prot_sig_templates.clone(); tokio::spawn(async move { let
 _permit = semaphore_clone.acquire().await; // Report when the permit is
 available and processing begins if (i + 1) % reporting_threshold == 0 { let
 percent_processed = (((i + 1) as f64 / n_accs as f64) * 100.0).round();
@@ -229,13 +241,12 @@
 ("Failed to send signatures: {}", e); let _ = send_errors.send(e.into()).await;
 // Send the error through the channel } for fail in failed_downloads { if let
 Err(e) = send_failed.send(fail).await { eprintln!("Failed to send failed
 download info: {}", e); let _ = send_errors.send(e.into()).await; // Send the
 error through the channel } } } Err(e) => { let _ = send_errors.send(e).await;
 } } drop(send_errors); }); } // drop senders as we're done sending data drop
 (send_sigs); drop(send_failed); drop(error_sender); // Wait for all tasks to
-complete for handle in handles { if let Err(e) = handle.await { eprintln!("A
-task encountered an error: {}", e); } } // // Handle errors received from the
-error channel while let Some(error) = error_receiver.recv().await { eprintln!
-("Error: {}", error); // Check if the error message contains "No signatures
-written" if error.to_string().contains("No signatures written") &
-!download_only { bail!("{}.", error); } } Ok(()) }
+complete for handle in handles { if let Err(e) = handle.await { eprintln!
+("Handle join error: {}.", e); } } // since the only critical error is not
+having written any sigs // check this here at end. Bail if we wrote expected
+sigs but wrote none. if critical_error_flag.load(Ordering::SeqCst) &
+!download_only { bail!("No signatures written, exiting."); } Ok(()) }
```

### Comparing `sourmash_plugin_directsketch-0.2.1/src/lib.rs` & `sourmash_plugin_directsketch-0.2.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/src/python/sourmash_plugin_directsketch/__init__.py` & `sourmash_plugin_directsketch-0.2.2/src/python/sourmash_plugin_directsketch/__init__.py`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/src/utils.rs` & `sourmash_plugin_directsketch-0.2.2/src/utils.rs`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/sourmash_tst_utils.py` & `sourmash_plugin_directsketch-0.2.2/tests/sourmash_tst_utils.py`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test-data/GCA_000175555.1.sig.gz` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/GCA_000175555.1.sig.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test-data/GCA_000961135.2.protein.sig.gz` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/GCA_000961135.2.protein.sig.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test-data/GCA_000961135.2.sig.gz` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/GCA_000961135.2.sig.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test-data/out_fastas/GCA_000175555.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000175555.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test-data/out_fastas/GCA_000961135.2_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000961135.2_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test-data/out_fastas/GCA_000961135.2_protein.faa.gz` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000961135.2_protein.faa.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_assembly_report.txt` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000337115.1_assembly_report.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000337115.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_md5checksums.txt` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000337115.1_md5checksums.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_protein.faa.gz` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000337115.1_protein.faa.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000961135.2_md5checksums.txt` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_000961135.2_md5checksums.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_001950595.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/outputs/GCA_001950595.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test-data/test.zip` & `sourmash_plugin_directsketch-0.2.2/tests/test-data/test.zip`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/tests/test_gbsketch.py` & `sourmash_plugin_directsketch-0.2.2/tests/test_gbsketch.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,8 +288,8 @@
         runtmp.sourmash('scripts', 'gbsketch', acc_mod, '-o', output,
                     '--failed', failed, '-r', '1',
                     '--param-str', "dna,k=31,scaled=1000")
         
     captured = capfd.readouterr()
     print(captured.out)
     print(captured.err)
-    assert "Error: No signatures written." in captured.err
+    assert "Error: No signatures written, exiting." in captured.err
```

### Comparing `sourmash_plugin_directsketch-0.2.1/Cargo.lock` & `sourmash_plugin_directsketch-0.2.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.82"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
+checksum = "25bdb32cbbdce2b519a9cd7df3a678443100e265d5e25ca763b7572a5104f5f3"
 
 [[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
@@ -1663,37 +1663,37 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
+checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
+checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.116"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1811,15 +1811,15 @@
  "vec-collections",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "sourmash_plugin_directsketch"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "anyhow",
  "async_zip",
  "camino",
  "chrono",
  "csv",
  "futures",
```

### Comparing `sourmash_plugin_directsketch-0.2.1/pyproject.toml` & `sourmash_plugin_directsketch-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.1/PKG-INFO` & `sourmash_plugin_directsketch-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sourmash_plugin_directsketch
-Version: 0.2.1
+Version: 0.2.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: sourmash >=4.8.5, <5
 Requires-Dist: pytest >=6.2.4, <8.3.0 ; extra == 'test'
 Requires-Dist: pytest-cov >=2.12, <6.0 ; extra == 'test'
 Requires-Dist: pytest-xdist ; extra == 'test'
@@ -13,14 +13,23 @@
 Summary: Download and Sketch GenBank Assembly Datasets
 Author: N. Tessa Pierce-Ward
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # sourmash_plugin_directsketch
 
+[![PyPI](https://img.shields.io/pypi/v/sourmash_plugin_directsketch)](https://pypi.org/project/sourmash_plugin_directsketch/)
+
+
+tl;dr - download and sketch NCBI Assembly Datasets by accession
+
+## About
+
+This plugin is an attempt to improve database generation by downloading assemblies, checking md5sum, and sketching to a sourmash zipfile. FASTA files can also be saved if desired. It's quite fast, but still very much at alpha level. Here be dragons.
+
 ## Installation
 
 ```
 pip install sourmash_plugin_directsketch
 ```
 
 ## Usage
@@ -64,17 +73,25 @@
                         parameter string for sketching (default: k=31,scaled=1000)
   -c CORES, --cores CORES
                         number of cores to use (default is all available)
   -r RETRY_TIMES, --retry-times RETRY_TIMES
                         number of times to retry failed downloads
 ```
 
+## Code of Conduct
+
+This project is under the [sourmash Code of Conduct](https://github.com/sourmash-bio/sourmash/blob/latest/CODE_OF_CONDUCT.rst).
+
 ## Support
 
-We suggest filing issues in [the main sourmash issue tracker](https://github.com/dib-lab/sourmash/issues) as that receives more attention!
+We suggest filing issues in [the directsketch issue tracker](https://github.com/bluegenes/sourmash_plugin_directsketch/issues) or [the main sourmash issue tracker](https://github.com/dib-lab/sourmash/issues).
+
+## Authors
+
+* N. Tessa Pierce-Ward
 
 ## Dev docs
 
 `sourmash_plugin_directsketch` is developed at https://github.com/sourmash-bio/sourmash_plugin_directsketch.
 
 ### Testing
```

