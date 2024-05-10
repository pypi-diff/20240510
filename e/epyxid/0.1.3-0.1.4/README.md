# Comparing `tmp/epyxid-0.1.3.tar.gz` & `tmp/epyxid-0.1.4.tar.gz`

## Comparing `epyxid-0.1.3.tar` & `epyxid-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 epyxid-0.1.3/Cargo.toml
--rw-r--r--   0     1001      127      270 2024-03-05 15:58:17.000000 epyxid-0.1.3/.editorconfig
--rw-r--r--   0     1001      127     4113 2024-03-05 15:58:17.000000 epyxid-0.1.3/.github/workflows/ci.yml
--rw-r--r--   0     1001      127     1511 2024-03-05 15:58:17.000000 epyxid-0.1.3/.gitignore
--rw-r--r--   0     1001      127      516 2024-03-05 15:58:17.000000 epyxid-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     1036 2024-03-05 15:58:17.000000 epyxid-0.1.3/LICENSE.txt
--rw-r--r--   0     1001      127      490 2024-03-05 15:58:17.000000 epyxid-0.1.3/README.md
--rw-r--r--   0     1001      127     1226 2024-03-05 15:58:17.000000 epyxid-0.1.3/build.rs
--rw-r--r--   0     1001      127     1390 2024-03-05 15:58:17.000000 epyxid-0.1.3/epyxid.pyi
--rwxr-xr-x   0     1001      127      135 2024-03-05 15:58:17.000000 epyxid-0.1.3/justfile
--rw-r--r--   0     1001      127      118 2024-03-05 15:58:17.000000 epyxid-0.1.3/src/errors.rs
--rw-r--r--   0     1001      127      595 2024-03-05 15:58:17.000000 epyxid-0.1.3/src/lib.rs
--rw-r--r--   0     1001      127      926 2024-03-05 15:58:17.000000 epyxid-0.1.3/src/utils.rs
--rw-r--r--   0     1001      127     1746 2024-03-05 15:58:17.000000 epyxid-0.1.3/src/wrapper.rs
--rw-r--r--   0     1001      127      913 2024-03-05 15:58:17.000000 epyxid-0.1.3/test_xid.py
--rw-r--r--   0     1001      127    12933 2024-03-05 15:58:25.000000 epyxid-0.1.3/Cargo.lock
--rw-r--r--   0     1001      127     1168 2024-03-05 15:58:17.000000 epyxid-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1371 1970-01-01 00:00:00.000000 epyxid-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 epyxid-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      127      270 2024-05-10 13:39:34.000000 epyxid-0.1.4/.editorconfig
+-rw-r--r--   0     1001      127     4131 2024-05-10 13:39:34.000000 epyxid-0.1.4/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127     1511 2024-05-10 13:39:34.000000 epyxid-0.1.4/.gitignore
+-rw-r--r--   0     1001      127      516 2024-05-10 13:39:34.000000 epyxid-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     1036 2024-05-10 13:39:34.000000 epyxid-0.1.4/LICENSE.txt
+-rw-r--r--   0     1001      127      490 2024-05-10 13:39:34.000000 epyxid-0.1.4/README.md
+-rw-r--r--   0     1001      127     1390 2024-05-10 13:39:34.000000 epyxid-0.1.4/epyxid.pyi
+-rwxr-xr-x   0     1001      127      135 2024-05-10 13:39:34.000000 epyxid-0.1.4/justfile
+-rw-r--r--   0     1001      127      118 2024-05-10 13:39:34.000000 epyxid-0.1.4/src/errors.rs
+-rw-r--r--   0     1001      127      595 2024-05-10 13:39:34.000000 epyxid-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      127      926 2024-05-10 13:39:34.000000 epyxid-0.1.4/src/utils.rs
+-rw-r--r--   0     1001      127     1746 2024-05-10 13:39:34.000000 epyxid-0.1.4/src/wrapper.rs
+-rw-r--r--   0     1001      127      913 2024-05-10 13:39:34.000000 epyxid-0.1.4/test_xid.py
+-rw-r--r--   0     1001      127    13608 2024-05-10 13:39:40.000000 epyxid-0.1.4/Cargo.lock
+-rw-r--r--   0     1001      127     1168 2024-05-10 13:39:34.000000 epyxid-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1371 1970-01-01 00:00:00.000000 epyxid-0.1.4/PKG-INFO
```

### Comparing `epyxid-0.1.3/.github/workflows/ci.yml` & `epyxid-0.1.4/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
+          args: --release --out dist --interpreter python3.10
           sccache: 'true'
           manylinux: auto
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
@@ -76,15 +76,15 @@
         with:
           python-version: '3.10'
           architecture: ${{ matrix.target }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
+          args: --release --out dist --interpreter python3.10
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
       - name: pytest
@@ -106,15 +106,15 @@
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
+          args: --release --out dist --interpreter python3.10
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
       - name: pytest
```

### Comparing `epyxid-0.1.3/.gitignore` & `epyxid-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `epyxid-0.1.3/.pre-commit-config.yaml` & `epyxid-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `epyxid-0.1.3/LICENSE.txt` & `epyxid-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `epyxid-0.1.3/epyxid.pyi` & `epyxid-0.1.4/epyxid.pyi`

 * *Files identical despite different names*

### Comparing `epyxid-0.1.3/src/lib.rs` & `epyxid-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `epyxid-0.1.3/src/utils.rs` & `epyxid-0.1.4/src/utils.rs`

 * *Files identical despite different names*

### Comparing `epyxid-0.1.3/src/wrapper.rs` & `epyxid-0.1.4/src/wrapper.rs`

 * *Files identical despite different names*

### Comparing `epyxid-0.1.3/test_xid.py` & `epyxid-0.1.4/test_xid.py`

 * *Files identical despite different names*

### Comparing `epyxid-0.1.3/Cargo.lock` & `epyxid-0.1.4/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
+
+[[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "cfg-if"
@@ -41,17 +47,17 @@
 dependencies = [
  "pyo3",
  "xid",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -69,29 +75,29 @@
  "libc",
  "match_cfg",
  "winapi",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "match_cfg"
@@ -103,42 +109,42 @@
 name = "md5"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "490cc448043f947bae3cbee9c203358d62dbee0db12107a74be5c30ccfd09771"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
@@ -153,26 +159,26 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -180,62 +186,62 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -264,19 +270,19 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
@@ -288,62 +294,62 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sysctl"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "225e483f02d0ad107168dc57381a8a40c3aeea6abe47f37506931f861643cfa8"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "byteorder",
  "libc",
  "thiserror",
  "walkdir",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.57"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.57"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -388,98 +394,114 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
 name = "windows-targets"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winreg"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d107f8c6e916235c4c01cabb3e8acf7bea8ef6a63ca2e7fa0527c049badfc48c"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "xid"
-version = "1.0.3"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f9671fb9541acc3118f04c4a6768253091d55077653efed3a4b151493abfd4e"
+checksum = "3752a194518cdee5d019812fb7978c51d8f0b7cfe9ace5983df1780964bb84c0"
 dependencies = [
  "crc32fast",
  "hostname",
  "md5",
  "once_cell",
  "rand",
  "sysctl",
```

### Comparing `epyxid-0.1.3/pyproject.toml` & `epyxid-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "epyxid"
 description = "Python wrapper around Rust implementation of XID (Globally Unique ID Generator)"
 requires-python = ">=3.8"
 authors = [
   {name = "Aleksandr Shpak", email = "shpaker@gmail.com"},
 ]
-version = "0.1.3"
+version = "0.1.4"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 keywords = [
   "rust",
   "xid",
   "pyo3",
 ]
```

### Comparing `epyxid-0.1.3/PKG-INFO` & `epyxid-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: epyxid
-Version: 0.1.3
+Version: 0.1.4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
```

