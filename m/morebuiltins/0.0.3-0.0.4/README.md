# Comparing `tmp/morebuiltins-0.0.3.tar.gz` & `tmp/morebuiltins-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morebuiltins-0.0.3.tar", last modified: Mon Apr 22 14:20:15 2024, max compression
+gzip compressed data, was "morebuiltins-0.0.4.tar", last modified: Fri May 10 16:17:19 2024, max compression
```

## Comparing `morebuiltins-0.0.3.tar` & `morebuiltins-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     1706 2024-04-21 11:23:27.856963 morebuiltins-0.0.3/.github/workflows/pythonpackage.yml
--rw-r--r--   0        0        0     1834 2024-04-22 13:47:51.525102 morebuiltins-0.0.3/.gitignore
--rw-r--r--   0        0        0     1065 2022-09-17 08:54:27.628835 morebuiltins-0.0.3/LICENSE
--rw-r--r--   0        0        0     5443 2024-04-22 14:20:02.091700 morebuiltins-0.0.3/README.md
--rw-r--r--   0        0        0    22158 2024-04-22 14:15:49.073472 morebuiltins-0.0.3/doc.md
--rw-r--r--   0        0        0     1686 2024-04-21 11:23:27.859926 morebuiltins-0.0.3/doc.py
--rw-r--r--   0        0        0      144 2024-04-22 14:09:40.059334 morebuiltins-0.0.3/morebuiltins/__init__.py
--rw-r--r--   0        0        0     5771 2024-04-22 14:07:46.467244 morebuiltins-0.0.3/morebuiltins/functools.py
--rw-r--r--   0        0        0    12448 2024-04-21 13:01:37.832092 morebuiltins-0.0.3/morebuiltins/ipc.py
--rw-r--r--   0        0        0    11610 2024-04-21 11:23:27.863238 morebuiltins-0.0.3/morebuiltins/request.py
--rw-r--r--   0        0        0    24097 2024-04-21 13:01:53.699477 morebuiltins-0.0.3/morebuiltins/utils.py
--rw-r--r--   0        0        0      176 2022-03-07 14:38:12.014153 morebuiltins-0.0.3/morebuiltins/zipapps/__init__.py
--rw-r--r--   0        0        0    15752 2023-09-12 15:05:46.088631 morebuiltins-0.0.3/morebuiltins/zipapps/__main__.py
--rw-r--r--   0        0        0      561 2022-10-29 14:52:39.536246 morebuiltins-0.0.3/morebuiltins/zipapps/activate_zipapps.py
--rw-r--r--   0        0        0     8426 2022-08-29 13:51:35.635512 morebuiltins-0.0.3/morebuiltins/zipapps/ensure_zipapps.py.template
--rw-r--r--   0        0        0     3385 2022-10-29 14:52:39.538241 morebuiltins-0.0.3/morebuiltins/zipapps/entry_point.py.template
--rw-r--r--   0        0        0     4640 2022-04-28 09:03:53.129989 morebuiltins-0.0.3/morebuiltins/zipapps/freezing.py
--rw-r--r--   0        0        0    26417 2024-04-22 14:18:00.799845 morebuiltins-0.0.3/morebuiltins/zipapps/main.py
--rw-r--r--   0        0        0       68 2024-04-22 13:58:01.690978 morebuiltins-0.0.3/publish.py
--rw-r--r--   0        0        0      468 2024-04-21 11:23:27.864237 morebuiltins-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1449 2024-04-22 14:03:35.884406 morebuiltins-0.0.3/test.py
--rw-r--r--   0        0        0     5655 1970-01-01 00:00:00.000000 morebuiltins-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1706 2024-04-21 11:23:27.856963 morebuiltins-0.0.4/.github/workflows/pythonpackage.yml
+-rw-r--r--   0        0        0     1834 2024-04-22 13:47:51.525102 morebuiltins-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1065 2022-09-17 08:54:27.628835 morebuiltins-0.0.4/LICENSE
+-rw-r--r--   0        0        0     6023 2024-05-10 16:16:04.000525 morebuiltins-0.0.4/README.md
+-rw-r--r--   0        0        0    28108 2024-05-10 16:14:53.022118 morebuiltins-0.0.4/doc.md
+-rw-r--r--   0        0        0      180 2024-05-10 16:14:50.495134 morebuiltins-0.0.4/morebuiltins/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-10 16:13:40.348340 morebuiltins-0.0.4/morebuiltins/download_python/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-10 16:13:40.348340 morebuiltins-0.0.4/morebuiltins/download_python/__main__.py
+-rw-r--r--   0        0        0     6175 2024-05-10 16:14:38.208022 morebuiltins-0.0.4/morebuiltins/download_python/main.py
+-rw-r--r--   0        0        0    14315 2024-04-26 09:30:43.977671 morebuiltins-0.0.4/morebuiltins/functools.py
+-rw-r--r--   0        0        0    12448 2024-04-21 13:01:37.832092 morebuiltins-0.0.4/morebuiltins/ipc.py
+-rw-r--r--   0        0        0    11610 2024-04-25 07:08:52.621056 morebuiltins-0.0.4/morebuiltins/request.py
+-rw-r--r--   0        0        0    24097 2024-04-21 13:01:53.699477 morebuiltins-0.0.4/morebuiltins/utils.py
+-rw-r--r--   0        0        0      176 2022-03-07 14:38:12.014153 morebuiltins-0.0.4/morebuiltins/zipapps/__init__.py
+-rw-r--r--   0        0        0    15752 2023-09-12 15:05:46.088631 morebuiltins-0.0.4/morebuiltins/zipapps/__main__.py
+-rw-r--r--   0        0        0      561 2022-10-29 14:52:39.536246 morebuiltins-0.0.4/morebuiltins/zipapps/activate_zipapps.py
+-rw-r--r--   0        0        0     8426 2022-08-29 13:51:35.635512 morebuiltins-0.0.4/morebuiltins/zipapps/ensure_zipapps.py.template
+-rw-r--r--   0        0        0     3385 2022-10-29 14:52:39.538241 morebuiltins-0.0.4/morebuiltins/zipapps/entry_point.py.template
+-rw-r--r--   0        0        0     4640 2022-04-28 09:03:53.129989 morebuiltins-0.0.4/morebuiltins/zipapps/freezing.py
+-rw-r--r--   0        0        0    26417 2024-04-22 14:18:00.799845 morebuiltins-0.0.4/morebuiltins/zipapps/main.py
+-rw-r--r--   0        0        0       68 2024-05-10 13:38:10.738314 morebuiltins-0.0.4/publish.py
+-rw-r--r--   0        0        0      468 2024-04-21 11:23:27.864237 morebuiltins-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3018 2024-04-25 07:10:55.980268 morebuiltins-0.0.4/test.py
+-rw-r--r--   0        0        0     6224 1970-01-01 00:00:00.000000 morebuiltins-0.0.4/PKG-INFO
```

### Comparing `morebuiltins-0.0.3/.github/workflows/pythonpackage.yml` & `morebuiltins-0.0.4/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `morebuiltins-0.0.3/.gitignore` & `morebuiltins-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `morebuiltins-0.0.3/LICENSE` & `morebuiltins-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `morebuiltins-0.0.3/README.md` & `morebuiltins-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 
 2.1 `lru_cache_ttl` - A Least Recently Used (LRU) cache with a Time To Live (TTL) feature.
 
 2.2 `threads` - Quickly convert synchronous functions to be concurrency-able. (similar to madisonmay/Tomorrow)
 
 2.3 `bg_task` - Avoid asyncio free-flying tasks, better to use the new asyncio.TaskGroup to avoid this in 3.11+. https://github.com/python/cpython/issues/91887
 
+2.4 `NamedLock` - Reusable named locks, support for timeouts, support for multiple concurrent locks.
+
+2.5 `FuncSchema` - Parse the parameters and types required by a function into a dictionary, and convert an incoming parameter into the appropriate type.
+
 
 ## 3. morebuiltins.ipc
 
 3.1 `IPCEncoder` - An abstract base class for all encoders; implementing the necessary communication protocol requires only the definition of two abstract methods. Be mindful that varying header lengths will impact the maximum packaging size.
 
 3.4 `SocketLogHandlerEncoder` - For a practical demonstration, refer to the test code: morebuiltins/ipc.py:_test_ipc_logging.
 
@@ -103,21 +107,28 @@
 4.2 `DomainParser` - Extracts the Second-level domain (SLD) from a provided hostname or URL.
 
 4.3 `unparse_qsl` - Provides the inverse operation of parse_qsl, converting query string lists back into a URL-encoded string.
 
 4.4 `update_url` - Organizes the query arguments within a URL to standardize its format.
 
 
+## 5. morebuiltins.download_python
+
+5.1 `download_python` - Usage: python -m morebuiltins.download_python
+
+
 <!-- end -->
 
 ## On the way
 
 - [x] add zipapps as a submodule(https://github.com/ClericPy/zipapps) - v0.0.3
 - [x] asyncio free-flying tasks(bg_task) - v0.0.3
+- [x] named lock with timeout - v0.0.4
+- [x] functools.FuncSchema (parse function to get the query-dict) - v0.0.4
+- [x] morebuiltins.download_python [standalone python](https://github.com/indygreg/python-build-standalone/releases/latest) downloader - v0.0.4
+- [ ] pip.pip_install
 - [ ] progress_bar
 - [ ] http.server (upload)
-- [ ] function parser (signature.parameters)
 - [ ] time reach syntax
 - [ ] quick tkinter
 - [ ] http request/response parser
-- [ ] named lock with timeout
 - [ ] TimeSizeRotatingHandler of logging.handlers
```

### Comparing `morebuiltins-0.0.3/doc.md` & `morebuiltins-0.0.4/doc.md`

 * *Files 14% similar despite different names*

```diff
@@ -1002,384 +1002,756 @@
 00003e90: 7375 6573 2f39 3138 3837 0d0a 0d0a 2020  sues/91887....  
 00003ea0: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
 00003eb0: 2020 2020 2020 2020 2063 6f72 6f20 2843           coro (C
 00003ec0: 6f72 6f75 7469 6e65 290d 0a0d 0a20 2020  oroutine)....   
 00003ed0: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
 00003ee0: 2020 2020 2020 2020 2020 205f 7479 7065             _type
 00003ef0: 5f3a 2054 6173 6b0d 0a0d 0a20 2020 200d  _: Task....    .
-00003f00: 0a0d 0a2d 2d2d 0d0a 0d0a 3d3d 3d3d 3d3d  ...---....======
-00003f10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003f20: 0d0a 0d0a 2323 2033 2e20 6d6f 7265 6275  ....## 3. morebu
-00003f30: 696c 7469 6e73 2e69 7063 0d0a 0d0a 0d0a  iltins.ipc......
-00003f40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003f50: 3d3d 3d3d 3d3d 0d0a 0d0a 0d0a 2020 2020  ======......    
-00003f60: 332e 3120 6049 5043 456e 636f 6465 7260  3.1 `IPCEncoder`
-00003f70: 202d 2041 6e20 6162 7374 7261 6374 2062   - An abstract b
-00003f80: 6173 6520 636c 6173 7320 666f 7220 616c  ase class for al
-00003f90: 6c20 656e 636f 6465 7273 3b20 696d 706c  l encoders; impl
-00003fa0: 656d 656e 7469 6e67 2074 6865 206e 6563  ementing the nec
-00003fb0: 6573 7361 7279 2063 6f6d 6d75 6e69 6361  essary communica
-00003fc0: 7469 6f6e 2070 726f 746f 636f 6c20 7265  tion protocol re
-00003fd0: 7175 6972 6573 206f 6e6c 7920 7468 6520  quires only the 
-00003fe0: 6465 6669 6e69 7469 6f6e 206f 6620 7477  definition of tw
-00003ff0: 6f20 6162 7374 7261 6374 206d 6574 686f  o abstract metho
-00004000: 6473 2e20 4265 206d 696e 6466 756c 2074  ds. Be mindful t
-00004010: 6861 7420 7661 7279 696e 6720 6865 6164  hat varying head
-00004020: 6572 206c 656e 6774 6873 2077 696c 6c20  er lengths will 
-00004030: 696d 7061 6374 2074 6865 206d 6178 696d  impact the maxim
-00004040: 756d 2070 6163 6b61 6769 6e67 2073 697a  um packaging siz
-00004050: 652e 0d0a 0d0a 0d0a 2d2d 2d0d 0a0d 0a0d  e.......---.....
-00004060: 0a20 2020 2033 2e34 2060 536f 636b 6574  .    3.4 `Socket
-00004070: 4c6f 6748 616e 646c 6572 456e 636f 6465  LogHandlerEncode
-00004080: 7260 202d 2046 6f72 2061 2070 7261 6374  r` - For a pract
-00004090: 6963 616c 2064 656d 6f6e 7374 7261 7469  ical demonstrati
-000040a0: 6f6e 2c20 7265 6665 7220 746f 2074 6865  on, refer to the
-000040b0: 2074 6573 7420 636f 6465 3a20 6d6f 7265   test code: more
-000040c0: 6275 696c 7469 6e73 2f69 7063 2e70 793a  builtins/ipc.py:
-000040d0: 5f74 6573 745f 6970 635f 6c6f 6767 696e  _test_ipc_loggin
-000040e0: 672e 0d0a 0d0a 2020 2020 2020 2020 6060  g.....        ``
-000040f0: 600d 0a20 2020 2020 2020 2061 7379 6e63  `..        async
-00004100: 2064 6566 205f 7465 7374 5f69 7063 5f6c   def _test_ipc_l
-00004110: 6f67 6769 6e67 2829 3a0d 0a20 2020 2020  ogging():..     
-00004120: 2020 2020 2020 2069 6d70 6f72 7420 6c6f         import lo
-00004130: 6767 696e 670d 0a0d 0a20 2020 2020 2020  gging....       
-00004140: 2020 2020 2068 6f73 7420 3d20 2231 3237       host = "127
-00004150: 2e30 2e30 2e31 220d 0a20 2020 2020 2020  .0.0.1"..       
-00004160: 2020 2020 2070 6f72 7420 3d20 3830 3930       port = 8090
-00004170: 0d0a 2020 2020 2020 2020 2020 2020 6173  ..            as
-00004180: 796e 6320 7769 7468 2053 6f63 6b65 7453  ync with SocketS
-00004190: 6572 7665 7228 686f 7374 3d68 6f73 742c  erver(host=host,
-000041a0: 2070 6f72 743d 706f 7274 2c20 656e 636f   port=port, enco
-000041b0: 6465 723d 536f 636b 6574 4c6f 6748 616e  der=SocketLogHan
-000041c0: 646c 6572 456e 636f 6465 7228 2929 3a0d  dlerEncoder()):.
-000041d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000041e0: 2023 2073 6f63 6b65 7420 6c6f 6767 6572   # socket logger
-000041f0: 2064 656d 6f0d 0a20 2020 2020 2020 2020   demo..         
-00004200: 2020 2020 2020 2023 203d 3d3d 3d3d 3d3d         # =======
-00004210: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d 0a20 2020  ===========..   
-00004220: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00004230: 6765 7220 3d20 6c6f 6767 696e 672e 6765  ger = logging.ge
-00004240: 744c 6f67 6765 7228 2274 6573 745f 6c6f  tLogger("test_lo
-00004250: 6767 6572 2229 0d0a 2020 2020 2020 2020  gger")..        
-00004260: 2020 2020 2020 2020 6c6f 6767 6572 2e73          logger.s
-00004270: 6574 4c65 7665 6c28 6c6f 6767 696e 672e  etLevel(logging.
-00004280: 4445 4255 4729 0d0a 2020 2020 2020 2020  DEBUG)..        
-00004290: 2020 2020 2020 2020 6820 3d20 536f 636b          h = Sock
-000042a0: 6574 4861 6e64 6c65 7228 686f 7374 2c20  etHandler(host, 
-000042b0: 706f 7274 290d 0a20 2020 2020 2020 2020  port)..         
-000042c0: 2020 2020 2020 2068 2e73 6574 4c65 7665         h.setLeve
-000042d0: 6c28 6c6f 6767 696e 672e 4445 4255 4729  l(logging.DEBUG)
-000042e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000042f0: 2020 6c6f 6767 6572 2e61 6464 4861 6e64    logger.addHand
-00004300: 6c65 7228 6829 0d0a 2020 2020 2020 2020  ler(h)..        
-00004310: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00004320: 6e66 6f28 2274 6573 7420 736f 636b 6574  nfo("test socket
-00004330: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00004340: 2020 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d      # ==========
-00004350: 3d3d 3d3d 3d3d 3d3d 0d0a 0d0a 2020 2020  ========....    
-00004360: 2020 2020 2020 2020 2020 2020 2320 656e              # en
-00004370: 7375 7265 2074 6573 7420 6361 7365 0d0a  sure test case..
-00004380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004390: 6177 6169 7420 6173 796e 6369 6f2e 736c  await asyncio.sl
-000043a0: 6565 7028 302e 3129 0d0a 2020 2020 2020  eep(0.1)..      
-000043b0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-000043c0: 2070 6963 6b6c 652e 6c6f 6164 7328 682e   pickle.loads(h.
-000043d0: 736f 636b 2e72 6563 7628 3130 3030 3030  sock.recv(100000
-000043e0: 295b 343a 5d29 5b22 6e61 6d65 225d 203d  )[4:])["name"] =
-000043f0: 3d20 6c6f 6767 6572 2e6e 616d 650d 0a20  = logger.name.. 
-00004400: 2020 2020 2020 2060 6060 0d0a 2020 2020         ```..    
-00004410: 2020 2020 416e 6420 7072 6f76 6964 6520      And provide 
-00004420: 6120 7369 6d70 6c65 2069 6d70 6c65 6d65  a simple impleme
-00004430: 6e74 6174 696f 6e20 666f 7220 6765 6e65  ntation for gene
-00004440: 7261 7469 6e67 206c 6f67 7320 666f 7220  rating logs for 
-00004450: 636f 726f 7574 696e 6520 636f 6465 2077  coroutine code w
-00004460: 6974 6820 436c 6965 6e74 2075 7361 6765  ith Client usage
-00004470: 2e0d 0a20 2020 200d 0a0d 0a2d 2d2d 0d0a  ...    ....---..
-00004480: 0d0a 0d0a 2020 2020 332e 3520 6053 6f63  ....    3.5 `Soc
-00004490: 6b65 7453 6572 7665 7260 202d 2054 6f20  ketServer` - To 
-000044a0: 7365 6520 616e 2065 7861 6d70 6c65 2069  see an example i
-000044b0: 6e20 6163 7469 6f6e 2c20 7669 6577 2074  n action, view t
-000044c0: 6865 2074 6573 7420 636f 6465 3a20 6d6f  he test code: mo
-000044d0: 7265 6275 696c 7469 6e73 2f69 7063 2e70  rebuiltins/ipc.p
-000044e0: 793a 5f74 6573 745f 6970 632e 0d0a 0d0a  y:_test_ipc.....
-000044f0: 2020 2020 2020 2020 2020 2020 6060 600d              ```.
-00004500: 0a20 2020 2020 2020 2061 7379 6e63 2064  .        async d
-00004510: 6566 2074 6573 745f 636c 6965 6e74 2868  ef test_client(h
-00004520: 6f73 743d 2231 3237 2e30 2e30 2e31 222c  ost="127.0.0.1",
-00004530: 2070 6f72 743d 3830 3930 2c20 656e 636f   port=8090, enco
-00004540: 6465 723d 4e6f 6e65 2c20 6361 7365 733d  der=None, cases=
-00004550: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
-00004560: 2020 2020 6173 796e 6320 7769 7468 2053      async with S
-00004570: 6f63 6b65 7443 6c69 656e 7428 686f 7374  ocketClient(host
-00004580: 3d68 6f73 742c 2070 6f72 743d 706f 7274  =host, port=port
-00004590: 2c20 656e 636f 6465 723d 656e 636f 6465  , encoder=encode
-000045a0: 7229 2061 7320 633a 0d0a 2020 2020 2020  r) as c:..      
-000045b0: 2020 2020 2020 2020 2020 666f 7220 6361            for ca
-000045c0: 7365 2069 6e20 6361 7365 733a 0d0a 2020  se in cases:..  
-000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045e0: 2020 6177 6169 7420 632e 7365 6e64 2863    await c.send(c
-000045f0: 6173 6529 0d0a 2020 2020 2020 2020 2020  ase)..          
-00004600: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
-00004610: 7365 203d 2061 7761 6974 2063 2e72 6563  se = await c.rec
-00004620: 7628 290d 0a20 2020 2020 2020 2020 2020  v()..           
-00004630: 2020 2020 2020 2020 2069 6620 676c 6f62           if glob
-00004640: 616c 7328 292e 6765 7428 2270 7269 6e74  als().get("print
-00004650: 5f6c 6f67 2229 3a0d 0a20 2020 2020 2020  _log"):..       
-00004660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004670: 2070 7269 6e74 2822 5b43 6c69 656e 745d   print("[Client]
-00004680: 222c 2022 7365 6e64 3a22 2c20 7265 7072  ", "send:", repr
-00004690: 2863 6173 6529 2c20 223d 3e22 2c20 2272  (case), "=>", "r
-000046a0: 6563 763a 222c 2072 6570 7228 7265 7370  ecv:", repr(resp
-000046b0: 6f6e 7365 2929 0d0a 2020 2020 2020 2020  onse))..        
-000046c0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-000046d0: 7274 2063 6173 6520 3d3d 2072 6573 706f  rt case == respo
-000046e0: 6e73 6520 6f72 2073 7472 2863 6173 6529  nse or str(case)
-000046f0: 203d 3d20 7265 7370 6f6e 7365 2c20 5b63   == response, [c
-00004700: 6173 652c 2072 6573 706f 6e73 655d 0d0a  ase, response]..
-00004710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004720: 6177 6169 7420 632e 7365 6e64 2822 5b73  await c.send("[s
-00004730: 6875 7464 6f77 6e20 7365 7276 6572 5d22  hutdown server]"
-00004740: 290d 0a0d 0a0d 0a20 2020 2020 2020 2061  )......        a
-00004750: 7379 6e63 2064 6566 205f 7465 7374 5f69  sync def _test_i
-00004760: 7063 2829 3a0d 0a20 2020 2020 2020 2020  pc():..         
-00004770: 2020 2069 6d70 6f72 7420 706c 6174 666f     import platfo
-00004780: 726d 0d0a 0d0a 2020 2020 2020 2020 2020  rm....          
-00004790: 2020 4a53 4f4e 456e 636f 6465 722e 5f44    JSONEncoder._D
-000047a0: 554d 505f 4b57 4152 4753 5b22 6465 6661  UMP_KWARGS["defa
-000047b0: 756c 7422 5d20 3d20 7374 720d 0a20 2020  ult"] = str..   
-000047c0: 2020 2020 2020 2020 2066 6f72 2065 6e63           for enc
-000047d0: 2c20 6361 7365 7320 696e 205b 0d0a 2020  , cases in [..  
-000047e0: 2020 2020 2020 2020 2020 2020 2020 5b50                [P
-000047f0: 6963 6b6c 6545 6e63 6f64 6572 2c20 5b31  ickleEncoder, [1
-00004800: 3233 2c20 2231 3233 222c 204e 6f6e 652c  23, "123", None,
-00004810: 207b 2261 227d 2c20 5b22 6122 5d2c 2028   {"a"}, ["a"], (
-00004820: 2261 222c 292c 207b 2261 223a 2031 7d5d  "a",), {"a": 1}]
-00004830: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00004840: 2020 2020 5b4a 534f 4e45 6e63 6f64 6572      [JSONEncoder
-00004850: 2c20 5b31 3233 2c20 2231 3233 222c 204e  , [123, "123", N
-00004860: 6f6e 652c 207b 2261 227d 2c20 5b22 6122  one, {"a"}, ["a"
-00004870: 5d2c 207b 2261 223a 2031 7d5d 5d2c 0d0a  ], {"a": 1}]],..
-00004880: 2020 2020 2020 2020 2020 2020 5d3a 0d0a              ]:..
-00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048a0: 656e 636f 6465 7220 3d20 656e 6328 290d  encoder = enc().
-000048b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000048c0: 2069 6620 706c 6174 666f 726d 2e73 7973   if platform.sys
-000048d0: 7465 6d28 2920 3d3d 2022 4c69 6e75 7822  tem() == "Linux"
-000048e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000048f0: 2020 2020 2020 2023 2074 6573 7420 756e         # test un
-00004900: 6978 2064 6f6d 6169 6e20 736f 636b 6574  ix domain socket
-00004910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004920: 2020 2020 2020 7072 696e 7428 2254 6573        print("Tes
-00004930: 7420 4c69 6e75 7820 556e 6978 2044 6f6d  t Linux Unix Dom
-00004940: 6169 6e20 536f 636b 6574 2229 0d0a 2020  ain Socket")..  
+00003f00: 0a0d 0a2d 2d2d 0d0a 0d0a 0d0a 2020 2020  ...---......    
+00003f10: 322e 3420 604e 616d 6564 4c6f 636b 6020  2.4 `NamedLock` 
+00003f20: 2d20 5265 7573 6162 6c65 206e 616d 6564  - Reusable named
+00003f30: 206c 6f63 6b73 2c20 7375 7070 6f72 7420   locks, support 
+00003f40: 666f 7220 7469 6d65 6f75 7473 2c20 7375  for timeouts, su
+00003f50: 7070 6f72 7420 666f 7220 6d75 6c74 6970  pport for multip
+00003f60: 6c65 2063 6f6e 6375 7272 656e 7420 6c6f  le concurrent lo
+00003f70: 636b 732e 0d0a 0d0a 2020 2020 2020 2020  cks.....        
+00003f80: 2020 2020 2020 2020 6060 6070 7974 686f          ```pytho
+00003f90: 6e0d 0a0d 0a20 2020 2020 2020 2064 6566  n....        def
+00003fa0: 2074 6573 745f 6e61 6d65 645f 6c6f 636b   test_named_lock
+00003fb0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00003fc0: 2064 6566 2074 6573 745f 7379 6e63 2829   def test_sync()
+00003fd0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003fe0: 2020 2069 6d70 6f72 7420 7469 6d65 0d0a     import time..
+00003ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004000: 6672 6f6d 2063 6f6e 6375 7272 656e 742e  from concurrent.
+00004010: 6675 7475 7265 7320 696d 706f 7274 2054  futures import T
+00004020: 6872 6561 6450 6f6f 6c45 7865 6375 746f  hreadPoolExecuto
+00004030: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
+00004040: 2020 2066 726f 6d20 7468 7265 6164 696e     from threadin
+00004050: 6720 696d 706f 7274 204c 6f63 6b2c 2053  g import Lock, S
+00004060: 656d 6170 686f 7265 0d0a 0d0a 2020 2020  emaphore....    
+00004070: 2020 2020 2020 2020 2020 2020 6465 6620              def 
+00004080: 5f74 6573 7431 2829 3a0d 0a20 2020 2020  _test1():..     
+00004090: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+000040a0: 6974 6820 4e61 6d65 644c 6f63 6b28 225f  ith NamedLock("_
+000040b0: 7465 7374 3122 2c20 4c6f 636b 2c20 7469  test1", Lock, ti
+000040c0: 6d65 6f75 743d 302e 3035 2920 6173 206c  meout=0.05) as l
+000040d0: 6f63 6b3a 0d0a 2020 2020 2020 2020 2020  ock:..          
+000040e0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+000040f0: 6d65 2e73 6c65 6570 2830 2e31 290d 0a20  me.sleep(0.1).. 
+00004100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004110: 2020 2020 2020 2072 6574 7572 6e20 626f         return bo
+00004120: 6f6c 286c 6f63 6b29 0d0a 0d0a 2020 2020  ol(lock)....    
+00004130: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00004140: 2054 6872 6561 6450 6f6f 6c45 7865 6375   ThreadPoolExecu
+00004150: 746f 7228 3130 2920 6173 2070 6f6f 6c3a  tor(10) as pool:
+00004160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004170: 2020 2020 2020 7461 736b 7320 3d20 5b70        tasks = [p
+00004180: 6f6f 6c2e 7375 626d 6974 285f 7465 7374  ool.submit(_test
+00004190: 3129 2066 6f72 205f 2069 6e20 7261 6e67  1) for _ in rang
+000041a0: 6528 3329 5d0d 0a20 2020 2020 2020 2020  e(3)]..         
+000041b0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000041c0: 7420 3d20 5b69 2e72 6573 756c 7428 2920  t = [i.result() 
+000041d0: 666f 7220 6920 696e 2074 6173 6b73 5d0d  for i in tasks].
+000041e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000041f0: 2020 2020 2061 7373 6572 7420 7265 7375       assert resu
+00004200: 6c74 203d 3d20 5b54 7275 652c 2046 616c  lt == [True, Fal
+00004210: 7365 2c20 4661 6c73 655d 2c20 7265 7375  se, False], resu
+00004220: 6c74 0d0a 2020 2020 2020 2020 2020 2020  lt..            
+00004230: 2020 2020 6173 7365 7274 206c 656e 284e      assert len(N
+00004240: 616d 6564 4c6f 636b 2e5f 5359 4e43 5f43  amedLock._SYNC_C
+00004250: 4143 4845 2920 3d3d 2031 0d0a 2020 2020  ACHE) == 1..    
+00004260: 2020 2020 2020 2020 2020 2020 4e61 6d65              Name
+00004270: 644c 6f63 6b2e 636c 6561 725f 756e 6c6f  dLock.clear_unlo
+00004280: 636b 6564 2829 0d0a 2020 2020 2020 2020  cked()..        
+00004290: 2020 2020 2020 2020 6173 7365 7274 206c          assert l
+000042a0: 656e 284e 616d 6564 4c6f 636b 2e5f 5359  en(NamedLock._SY
+000042b0: 4e43 5f43 4143 4845 2920 3d3d 2030 0d0a  NC_CACHE) == 0..
+000042c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000042d0: 2020 6465 6620 5f74 6573 7432 2829 3a0d    def _test2():.
+000042e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000042f0: 2020 2020 2077 6974 6820 4e61 6d65 644c       with NamedL
+00004300: 6f63 6b28 225f 7465 7374 3222 2c20 6c61  ock("_test2", la
+00004310: 6d62 6461 3a20 5365 6d61 7068 6f72 6528  mbda: Semaphore(
+00004320: 3229 2c20 7469 6d65 6f75 743d 302e 3035  2), timeout=0.05
+00004330: 2920 6173 206c 6f63 6b3a 0d0a 2020 2020  ) as lock:..    
+00004340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004350: 2020 2020 7469 6d65 2e73 6c65 6570 2830      time.sleep(0
+00004360: 2e32 290d 0a20 2020 2020 2020 2020 2020  .2)..           
+00004370: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00004380: 7572 6e20 626f 6f6c 286c 6f63 6b29 0d0a  urn bool(lock)..
+00004390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000043a0: 2020 7769 7468 2054 6872 6561 6450 6f6f    with ThreadPoo
+000043b0: 6c45 7865 6375 746f 7228 3130 2920 6173  lExecutor(10) as
+000043c0: 2070 6f6f 6c3a 0d0a 2020 2020 2020 2020   pool:..        
+000043d0: 2020 2020 2020 2020 2020 2020 7461 736b              task
+000043e0: 7320 3d20 5b70 6f6f 6c2e 7375 626d 6974  s = [pool.submit
+000043f0: 285f 7465 7374 3229 2066 6f72 205f 2069  (_test2) for _ i
+00004400: 6e20 7261 6e67 6528 3329 5d0d 0a20 2020  n range(3)]..   
+00004410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004420: 2072 6573 756c 7420 3d20 5b69 2e72 6573   result = [i.res
+00004430: 756c 7428 2920 666f 7220 6920 696e 2074  ult() for i in t
+00004440: 6173 6b73 5d0d 0a20 2020 2020 2020 2020  asks]..         
+00004450: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00004460: 7420 7265 7375 6c74 203d 3d20 5b54 7275  t result == [Tru
+00004470: 652c 2054 7275 652c 2046 616c 7365 5d2c  e, True, False],
+00004480: 2072 6573 756c 740d 0a0d 0a20 2020 2020   result....     
+00004490: 2020 2020 2020 2064 6566 2074 6573 745f         def test_
+000044a0: 6173 796e 6328 293a 0d0a 2020 2020 2020  async():..      
+000044b0: 2020 2020 2020 2020 2020 696d 706f 7274            import
+000044c0: 2061 7379 6e63 696f 0d0a 0d0a 2020 2020   asyncio....    
+000044d0: 2020 2020 2020 2020 2020 2020 6173 796e              asyn
+000044e0: 6320 6465 6620 6d61 696e 2829 3a0d 0a20  c def main():.. 
+000044f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004500: 2020 2061 7379 6e63 2064 6566 205f 7465     async def _te
+00004510: 7374 3128 293a 0d0a 2020 2020 2020 2020  st1():..        
+00004520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004530: 6173 796e 6320 7769 7468 204e 616d 6564  async with Named
+00004540: 4c6f 636b 2822 5f74 6573 7431 222c 2061  Lock("_test1", a
+00004550: 7379 6e63 696f 2e4c 6f63 6b2c 2074 696d  syncio.Lock, tim
+00004560: 656f 7574 3d30 2e30 3529 2061 7320 6c6f  eout=0.05) as lo
+00004570: 636b 3a0d 0a20 2020 2020 2020 2020 2020  ck:..           
+00004580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004590: 2061 7761 6974 2061 7379 6e63 696f 2e73   await asyncio.s
+000045a0: 6c65 6570 2830 2e31 290d 0a20 2020 2020  leep(0.1)..     
+000045b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045c0: 2020 2020 2020 2072 6574 7572 6e20 626f         return bo
+000045d0: 6f6c 286c 6f63 6b29 0d0a 0d0a 2020 2020  ol(lock)....    
+000045e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045f0: 7461 736b 7320 3d20 5b61 7379 6e63 696f  tasks = [asyncio
+00004600: 2e63 7265 6174 655f 7461 736b 285f 7465  .create_task(_te
+00004610: 7374 3128 2929 2066 6f72 205f 2069 6e20  st1()) for _ in 
+00004620: 7261 6e67 6528 3329 5d0d 0a20 2020 2020  range(3)]..     
+00004630: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004640: 6573 756c 7420 3d20 5b61 7761 6974 2069  esult = [await i
+00004650: 2066 6f72 2069 2069 6e20 7461 736b 735d   for i in tasks]
+00004660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004670: 2020 2020 2020 6173 7365 7274 2072 6573        assert res
+00004680: 756c 7420 3d3d 205b 5472 7565 2c20 4661  ult == [True, Fa
+00004690: 6c73 652c 2046 616c 7365 5d2c 2072 6573  lse, False], res
+000046a0: 756c 740d 0a20 2020 2020 2020 2020 2020  ult..           
+000046b0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+000046c0: 6c65 6e28 4e61 6d65 644c 6f63 6b2e 5f41  len(NamedLock._A
+000046d0: 5359 4e43 5f43 4143 4845 2920 3d3d 2031  SYNC_CACHE) == 1
+000046e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000046f0: 2020 2020 2020 4e61 6d65 644c 6f63 6b2e        NamedLock.
+00004700: 636c 6561 725f 756e 6c6f 636b 6564 2829  clear_unlocked()
+00004710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004720: 2020 2020 2020 6173 7365 7274 206c 656e        assert len
+00004730: 284e 616d 6564 4c6f 636b 2e5f 4153 594e  (NamedLock._ASYN
+00004740: 435f 4341 4348 4529 203d 3d20 300d 0a0d  C_CACHE) == 0...
+00004750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004760: 2020 2020 2061 7379 6e63 2064 6566 205f       async def _
+00004770: 7465 7374 3228 293a 0d0a 2020 2020 2020  test2():..      
+00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004790: 2020 6173 796e 6320 7769 7468 204e 616d    async with Nam
+000047a0: 6564 4c6f 636b 280d 0a20 2020 2020 2020  edLock(..       
+000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047c0: 2020 2020 2022 5f74 6573 7432 222c 206c       "_test2", l
+000047d0: 616d 6264 613a 2061 7379 6e63 696f 2e53  ambda: asyncio.S
+000047e0: 656d 6170 686f 7265 2832 292c 2074 696d  emaphore(2), tim
+000047f0: 656f 7574 3d30 2e30 350d 0a20 2020 2020  eout=0.05..     
+00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004810: 2020 2029 2061 7320 6c6f 636b 3a0d 0a20     ) as lock:.. 
+00004820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004830: 2020 2020 2020 2020 2020 2061 7761 6974             await
+00004840: 2061 7379 6e63 696f 2e73 6c65 6570 2830   asyncio.sleep(0
+00004850: 2e31 290d 0a20 2020 2020 2020 2020 2020  .1)..           
+00004860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004870: 2072 6574 7572 6e20 626f 6f6c 286c 6f63   return bool(loc
+00004880: 6b29 0d0a 0d0a 2020 2020 2020 2020 2020  k)....          
+00004890: 2020 2020 2020 2020 2020 7461 736b 7320            tasks 
+000048a0: 3d20 5b61 7379 6e63 696f 2e63 7265 6174  = [asyncio.creat
+000048b0: 655f 7461 736b 285f 7465 7374 3228 2929  e_task(_test2())
+000048c0: 2066 6f72 205f 2069 6e20 7261 6e67 6528   for _ in range(
+000048d0: 3329 5d0d 0a20 2020 2020 2020 2020 2020  3)]..           
+000048e0: 2020 2020 2020 2020 2072 6573 756c 7420           result 
+000048f0: 3d20 5b61 7761 6974 2069 2066 6f72 2069  = [await i for i
+00004900: 2069 6e20 7461 736b 735d 0d0a 2020 2020   in tasks]..    
+00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004920: 6173 7365 7274 2072 6573 756c 7420 3d3d  assert result ==
+00004930: 205b 5472 7565 2c20 5472 7565 2c20 4661   [True, True, Fa
+00004940: 6c73 655d 2c20 7265 7375 6c74 0d0a 0d0a  lse], result....
 00004950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004960: 2020 686f 7374 203d 2022 2f74 6d70 2f75    host = "/tmp/u
-00004970: 6473 2e73 6f63 6b22 0d0a 2020 2020 2020  ds.sock"..      
-00004980: 2020 2020 2020 2020 2020 2020 2020 706f                po
-00004990: 7274 203d 204e 6f6e 650d 0a20 2020 2020  rt = None..     
-000049a0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000049b0: 7379 6e63 2077 6974 6820 536f 636b 6574  sync with Socket
-000049c0: 5365 7276 6572 2868 6f73 743d 686f 7374  Server(host=host
-000049d0: 2c20 706f 7274 3d70 6f72 742c 2065 6e63  , port=port, enc
-000049e0: 6f64 6572 3d65 6e63 6f64 6572 293a 0d0a  oder=encoder):..
-000049f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a00: 2020 2020 2020 2020 6177 6169 7420 7465          await te
-00004a10: 7374 5f63 6c69 656e 7428 686f 7374 2c20  st_client(host, 
-00004a20: 706f 7274 3d4e 6f6e 652c 2065 6e63 6f64  port=None, encod
-00004a30: 6572 3d65 6e63 6f64 6572 2c20 6361 7365  er=encoder, case
-00004a40: 733d 6361 7365 7329 0d0a 0d0a 2020 2020  s=cases)....    
-00004a50: 2020 2020 2020 2020 2020 2020 2320 7465              # te
-00004a60: 7374 2073 6f63 6b65 740d 0a20 2020 2020  st socket..     
-00004a70: 2020 2020 2020 2020 2020 2068 6f73 7420             host 
-00004a80: 3d20 2231 3237 2e30 2e30 2e31 220d 0a20  = "127.0.0.1".. 
-00004a90: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00004aa0: 6f72 7420 3d20 3830 3930 0d0a 2020 2020  ort = 8090..    
-00004ab0: 2020 2020 2020 2020 2020 2020 6173 796e              asyn
-00004ac0: 6320 7769 7468 2053 6f63 6b65 7453 6572  c with SocketSer
-00004ad0: 7665 7228 686f 7374 3d68 6f73 742c 2070  ver(host=host, p
-00004ae0: 6f72 743d 706f 7274 2c20 656e 636f 6465  ort=port, encode
-00004af0: 723d 656e 636f 6465 7229 3a0d 0a20 2020  r=encoder):..   
-00004b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b10: 2061 7761 6974 2074 6573 745f 636c 6965   await test_clie
-00004b20: 6e74 2868 6f73 743d 2231 3237 2e30 2e30  nt(host="127.0.0
-00004b30: 2e31 222c 2070 6f72 743d 3830 3930 2c20  .1", port=8090, 
-00004b40: 656e 636f 6465 723d 656e 636f 6465 722c  encoder=encoder,
-00004b50: 2063 6173 6573 3d63 6173 6573 290d 0a0d   cases=cases)...
-00004b60: 0a0d 0a20 2020 2020 2020 2020 2020 2060  ...            `
-00004b70: 6060 0d0a 2020 2020 0d0a 0d0a 2d2d 2d0d  ``..    ....---.
-00004b80: 0a0d 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ...=============
-00004b90: 3d3d 3d3d 3d3d 3d3d 3d0d 0a0d 0a23 2320  =========....## 
-00004ba0: 342e 206d 6f72 6562 7569 6c74 696e 732e  4. morebuiltins.
-00004bb0: 7265 7175 6573 740d 0a0d 0a0d 0a3d 3d3d  request......===
-00004bc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004bd0: 3d3d 3d0d 0a0d 0a0d 0a20 2020 2034 2e31  ===......    4.1
-00004be0: 2060 7265 7160 202d 2041 2062 6173 6963   `req` - A basic
-00004bf0: 206d 6f63 6b20 666f 7220 7265 7175 6573   mock for reques
-00004c00: 7473 2c20 7065 7266 6f72 6d61 6e74 2061  ts, performant a
-00004c10: 6c62 6569 7420 7369 6d70 6c69 7374 6963  lbeit simplistic
-00004c20: 2e0d 0a0d 0a20 2020 2020 2020 203e 3e3e  .....        >>>
-00004c30: 2069 6d70 6f72 7420 7469 6d65 0d0a 2020   import time..  
-00004c40: 2020 2020 2020 3e3e 3e20 7220 3d20 7265        >>> r = re
-00004c50: 712e 6765 7428 2268 7474 7073 3a2f 2f70  q.get("https://p
-00004c60: 6f73 746d 616e 2d65 6368 6f2e 636f 6d2f  ostman-echo.com/
-00004c70: 6765 743f 613d 3222 2c20 7469 6d65 6f75  get?a=2", timeou
-00004c80: 743d 332c 2070 6172 616d 733d 7b22 6222  t=3, params={"b"
-00004c90: 3a20 2233 227d 290d 0a20 2020 2020 2020  : "3"})..       
-00004ca0: 203e 3e3e 2072 2e75 726c 0d0a 2020 2020   >>> r.url..    
-00004cb0: 2020 2020 2768 7474 7073 3a2f 2f70 6f73      'https://pos
-00004cc0: 746d 616e 2d65 6368 6f2e 636f 6d2f 6765  tman-echo.com/ge
-00004cd0: 743f 613d 3226 623d 3327 0d0a 2020 2020  t?a=2&b=3'..    
-00004ce0: 2020 2020 3e3e 3e20 722e 6f6b 0d0a 2020      >>> r.ok..  
-00004cf0: 2020 2020 2020 5472 7565 0d0a 2020 2020        True..    
-00004d00: 2020 2020 3e3e 3e20 722e 7374 6174 7573      >>> r.status
-00004d10: 5f63 6f64 650d 0a20 2020 2020 2020 2032  _code..        2
-00004d20: 3030 0d0a 2020 2020 2020 2020 3e3e 3e20  00..        >>> 
-00004d30: 722e 7465 7874 2e73 7461 7274 7377 6974  r.text.startswit
-00004d40: 6828 277b 2729 0d0a 2020 2020 2020 2020  h('{')..        
-00004d50: 5472 7565 0d0a 2020 2020 2020 2020 3e3e  True..        >>
-00004d60: 3e20 7220 3d20 7265 712e 706f 7374 2822  > r = req.post("
-00004d70: 6874 7470 733a 2f2f 706f 7374 6d61 6e2d  https://postman-
-00004d80: 6563 686f 2e63 6f6d 2f70 6f73 743f 613d  echo.com/post?a=
-00004d90: 3222 2c20 7469 6d65 6f75 743d 332c 2070  2", timeout=3, p
-00004da0: 6172 616d 733d 7b22 6222 3a20 2233 227d  arams={"b": "3"}
-00004db0: 2c20 6461 7461 3d62 226d 6f63 6b20 6461  , data=b"mock da
-00004dc0: 7461 2229 0d0a 2020 2020 2020 2020 3e3e  ta")..        >>
-00004dd0: 3e20 722e 6a73 6f6e 2829 5b22 6461 7461  > r.json()["data
-00004de0: 225d 0d0a 2020 2020 2020 2020 276d 6f63  "]..        'moc
-00004df0: 6b20 6461 7461 270d 0a20 2020 2020 2020  k data'..       
-00004e00: 203e 3e3e 2072 2e6a 736f 6e28 295b 2261   >>> r.json()["a
-00004e10: 7267 7322 5d0d 0a20 2020 2020 2020 207b  rgs"]..        {
-00004e20: 2761 273a 2027 3227 2c20 2762 273a 2027  'a': '2', 'b': '
-00004e30: 3327 7d0d 0a20 2020 2020 2020 203e 3e3e  3'}..        >>>
-00004e40: 2072 203d 2072 6571 2e70 6f73 7428 2268   r = req.post("h
-00004e50: 7474 7073 3a2f 2f70 6f73 746d 616e 2d65  ttps://postman-e
-00004e60: 6368 6f2e 636f 6d2f 706f 7374 3f61 3d32  cho.com/post?a=2
-00004e70: 222c 2074 696d 656f 7574 3d33 2c20 6a73  ", timeout=3, js
-00004e80: 6f6e 3d7b 2264 6174 6122 3a20 2279 6573  on={"data": "yes
-00004e90: 206a 736f 6e22 7d29 0d0a 2020 2020 2020   json"})..      
-00004ea0: 2020 3e3e 3e20 722e 6a73 6f6e 2829 5b22    >>> r.json()["
-00004eb0: 6a73 6f6e 225d 0d0a 2020 2020 2020 2020  json"]..        
-00004ec0: 7b27 6461 7461 273a 2027 7965 7320 6a73  {'data': 'yes js
-00004ed0: 6f6e 277d 0d0a 2020 2020 0d0a 0d0a 2d2d  on'}..    ....--
-00004ee0: 2d0d 0a0d 0a0d 0a20 2020 2034 2e32 2060  -......    4.2 `
-00004ef0: 446f 6d61 696e 5061 7273 6572 6020 2d20  DomainParser` - 
-00004f00: 4578 7472 6163 7473 2074 6865 2053 6563  Extracts the Sec
-00004f10: 6f6e 642d 6c65 7665 6c20 646f 6d61 696e  ond-level domain
-00004f20: 2028 534c 4429 2066 726f 6d20 6120 7072   (SLD) from a pr
-00004f30: 6f76 6964 6564 2068 6f73 746e 616d 6520  ovided hostname 
-00004f40: 6f72 2055 524c 2e0d 0a0d 0a20 2020 2020  or URL.....     
-00004f50: 2020 203e 3e3e 2064 6f6d 6169 6e5f 7061     >>> domain_pa
-00004f60: 7273 6572 203d 2044 6f6d 6169 6e50 6172  rser = DomainPar
-00004f70: 7365 7228 290d 0a20 2020 2020 2020 203e  ser()..        >
-00004f80: 3e3e 2064 6f6d 6169 6e5f 7061 7273 6572  >> domain_parser
-00004f90: 2e70 6172 7365 5f68 6f73 746e 616d 6528  .parse_hostname(
-00004fa0: 2267 6974 6875 622e 636f 6d22 290d 0a20  "github.com").. 
-00004fb0: 2020 2020 2020 2027 6769 7468 7562 2e63         'github.c
-00004fc0: 6f6d 270d 0a20 2020 2020 2020 203e 3e3e  om'..        >>>
-00004fd0: 2064 6f6d 6169 6e5f 7061 7273 6572 2e70   domain_parser.p
-00004fe0: 6172 7365 5f68 6f73 746e 616d 6528 2277  arse_hostname("w
-00004ff0: 7777 2e67 6974 6875 622e 636f 6d22 290d  ww.github.com").
-00005000: 0a20 2020 2020 2020 2027 6769 7468 7562  .        'github
-00005010: 2e63 6f6d 270d 0a20 2020 2020 2020 203e  .com'..        >
-00005020: 3e3e 2064 6f6d 6169 6e5f 7061 7273 6572  >> domain_parser
-00005030: 2e70 6172 7365 5f68 6f73 746e 616d 6528  .parse_hostname(
-00005040: 2277 7777 2e61 7069 2e67 6974 6875 622e  "www.api.github.
-00005050: 636f 6d2e 636e 2229 0d0a 2020 2020 2020  com.cn")..      
-00005060: 2020 2767 6974 6875 622e 636f 6d2e 636e    'github.com.cn
-00005070: 270d 0a20 2020 2020 2020 203e 3e3e 2064  '..        >>> d
-00005080: 6f6d 6169 6e5f 7061 7273 6572 2e70 6172  omain_parser.par
-00005090: 7365 5f68 6f73 746e 616d 6528 2261 2e62  se_hostname("a.b
-000050a0: 2e63 2e6b 6177 6173 616b 692e 6a70 2229  .c.kawasaki.jp")
-000050b0: 0d0a 2020 2020 2020 2020 2763 2e6b 6177  ..        'c.kaw
-000050c0: 6173 616b 692e 6a70 270d 0a20 2020 2020  asaki.jp'..     
-000050d0: 2020 203e 3e3e 2064 6f6d 6169 6e5f 7061     >>> domain_pa
-000050e0: 7273 6572 2e70 6172 7365 5f68 6f73 746e  rser.parse_hostn
-000050f0: 616d 6528 2261 2e62 2e63 2e63 6974 792e  ame("a.b.c.city.
-00005100: 6b61 7761 7361 6b69 2e6a 7022 290d 0a20  kawasaki.jp").. 
-00005110: 2020 2020 2020 2027 632e 6369 7479 2e6b         'c.city.k
-00005120: 6177 6173 616b 692e 6a70 270d 0a20 2020  awasaki.jp'..   
-00005130: 2020 2020 203e 3e3e 2064 6f6d 6169 6e5f       >>> domain_
-00005140: 7061 7273 6572 2e70 6172 7365 5f68 6f73  parser.parse_hos
-00005150: 746e 616d 6528 2261 2e62 6262 6262 622e  tname("a.bbbbbb.
-00005160: 6363 6363 6363 2229 0d0a 2020 2020 2020  cccccc")..      
-00005170: 2020 2727 0d0a 2020 2020 2020 2020 3e3e    ''..        >>
-00005180: 3e20 646f 6d61 696e 5f70 6172 7365 722e  > domain_parser.
-00005190: 7061 7273 655f 686f 7374 6e61 6d65 2822  parse_hostname("
-000051a0: 612e 6262 6262 6262 2e63 6363 6363 6322  a.bbbbbb.cccccc"
-000051b0: 2c20 6465 6661 756c 743d 2262 2e63 2229  , default="b.c")
-000051c0: 0d0a 2020 2020 2020 2020 2762 2e63 270d  ..        'b.c'.
-000051d0: 0a20 2020 2020 2020 203e 3e3e 2064 6f6d  .        >>> dom
-000051e0: 6169 6e5f 7061 7273 6572 2e70 6172 7365  ain_parser.parse
-000051f0: 5f75 726c 2822 6874 7470 733a 2f2f 6769  _url("https://gi
-00005200: 7468 7562 2e63 6f6d 2f43 6c65 7269 6350  thub.com/ClericP
-00005210: 792f 6d6f 7265 6275 696c 7469 6e73 2229  y/morebuiltins")
-00005220: 0d0a 2020 2020 2020 2020 2767 6974 6875  ..        'githu
-00005230: 622e 636f 6d27 0d0a 0d0a 2020 2020 0d0a  b.com'....    ..
-00005240: 0d0a 2d2d 2d0d 0a0d 0a0d 0a20 2020 2034  ..---......    4
-00005250: 2e33 2060 756e 7061 7273 655f 7173 6c60  .3 `unparse_qsl`
-00005260: 202d 2050 726f 7669 6465 7320 7468 6520   - Provides the 
-00005270: 696e 7665 7273 6520 6f70 6572 6174 696f  inverse operatio
-00005280: 6e20 6f66 2070 6172 7365 5f71 736c 2c20  n of parse_qsl, 
-00005290: 636f 6e76 6572 7469 6e67 2071 7565 7279  converting query
-000052a0: 2073 7472 696e 6720 6c69 7374 7320 6261   string lists ba
-000052b0: 636b 2069 6e74 6f20 6120 5552 4c2d 656e  ck into a URL-en
-000052c0: 636f 6465 6420 7374 7269 6e67 2e0d 0a0d  coded string....
-000052d0: 0a0d 0a2d 2d2d 0d0a 0d0a 0d0a 2020 2020  ...---......    
-000052e0: 342e 3420 6075 7064 6174 655f 7572 6c60  4.4 `update_url`
-000052f0: 202d 204f 7267 616e 697a 6573 2074 6865   - Organizes the
-00005300: 2071 7565 7279 2061 7267 756d 656e 7473   query arguments
-00005310: 2077 6974 6869 6e20 6120 5552 4c20 746f   within a URL to
-00005320: 2073 7461 6e64 6172 6469 7a65 2069 7473   standardize its
-00005330: 2066 6f72 6d61 742e 0d0a 0d0a 2020 2020   format.....    
-00005340: 2020 2020 3e3e 3e20 7570 6461 7465 5f75      >>> update_u
-00005350: 726c 2827 6874 7470 3a2f 2f77 7777 2e67  rl('http://www.g
-00005360: 6974 6875 622e 636f 6d3f 623d 3126 633d  ithub.com?b=1&c=
-00005370: 3126 613d 3127 2c20 7b22 6222 3a20 4e6f  1&a=1', {"b": No
-00005380: 6e65 2c20 2263 223a 204e 6f6e 657d 2920  ne, "c": None}) 
-00005390: 2023 2072 656d 6f76 6520 7061 7261 6d73   # remove params
-000053a0: 0d0a 2020 2020 2020 2020 2768 7474 703a  ..        'http:
-000053b0: 2f2f 7777 772e 6769 7468 7562 2e63 6f6d  //www.github.com
-000053c0: 3f61 3d31 270d 0a20 2020 2020 2020 203e  ?a=1'..        >
-000053d0: 3e3e 2075 7064 6174 655f 7572 6c28 2268  >> update_url("h
-000053e0: 7474 703a 2f2f 7777 772e 6769 7468 7562  ttp://www.github
-000053f0: 2e63 6f6d 3f62 3d31 2663 3d31 2661 3d31  .com?b=1&c=1&a=1
-00005400: 222c 2061 3d22 3132 3322 2c20 623d 4e6f  ", a="123", b=No
-00005410: 6e65 2920 2023 2075 7064 6174 6520 7061  ne)  # update pa
-00005420: 7261 6d73 2077 6974 6820 6b77 6172 6773  rams with kwargs
-00005430: 0d0a 2020 2020 2020 2020 2768 7474 703a  ..        'http:
-00005440: 2f2f 7777 772e 6769 7468 7562 2e63 6f6d  //www.github.com
-00005450: 3f63 3d31 2661 3d31 3233 270d 0a20 2020  ?c=1&a=123'..   
-00005460: 2020 2020 203e 3e3e 2075 7064 6174 655f       >>> update_
-00005470: 7572 6c28 2768 7474 703a 2f2f 7777 772e  url('http://www.
-00005480: 6769 7468 7562 2e63 6f6d 3f62 3d31 2663  github.com?b=1&c
-00005490: 3d31 2661 3d31 272c 2073 6f72 743d 5472  =1&a=1', sort=Tr
-000054a0: 7565 2920 2023 2073 6f72 7420 7061 7261  ue)  # sort para
-000054b0: 6d73 0d0a 2020 2020 2020 2020 2768 7474  ms..        'htt
-000054c0: 703a 2f2f 7777 772e 6769 7468 7562 2e63  p://www.github.c
-000054d0: 6f6d 3f61 3d31 2662 3d31 2663 3d31 270d  om?a=1&b=1&c=1'.
-000054e0: 0a20 2020 2020 2020 203e 3e3e 2075 7064  .        >>> upd
-000054f0: 6174 655f 7572 6c28 2268 7474 703a 2f2f  ate_url("http://
-00005500: 7777 772e 6769 7468 7562 2e63 6f6d 3f62  www.github.com?b
-00005510: 3d31 2663 3d31 2661 3d31 222c 207b 2261  =1&c=1&a=1", {"a
-00005520: 223a 2022 3939 3922 7d29 2020 2320 7570  ": "999"})  # up
-00005530: 6461 7465 2070 6172 616d 730d 0a20 2020  date params..   
-00005540: 2020 2020 2027 6874 7470 3a2f 2f77 7777       'http://www
-00005550: 2e67 6974 6875 622e 636f 6d3f 623d 3126  .github.com?b=1&
-00005560: 633d 3126 613d 3939 3927 0d0a 2020 2020  c=1&a=999'..    
-00005570: 2020 2020 3e3e 3e20 7570 6461 7465 5f75      >>> update_u
-00005580: 726c 2822 6874 7470 3a2f 2f77 7777 2e67  rl("http://www.g
-00005590: 6974 6875 622e 636f 6d3f 623d 3126 633d  ithub.com?b=1&c=
-000055a0: 3126 613d 3122 2c20 7265 706c 6163 655f  1&a=1", replace_
-000055b0: 6b77 6172 6773 3d7b 226e 6574 6c6f 6322  kwargs={"netloc"
-000055c0: 3a20 2277 7777 2e6e 6577 5f68 6f73 742e  : "www.new_host.
-000055d0: 636f 6d22 7d29 2020 2320 7570 6461 7465  com"})  # update
-000055e0: 206e 6574 6c6f 630d 0a20 2020 2020 2020   netloc..       
-000055f0: 2027 6874 7470 3a2f 2f77 7777 2e6e 6577   'http://www.new
-00005600: 5f68 6f73 742e 636f 6d3f 623d 3126 633d  _host.com?b=1&c=
-00005610: 3126 613d 3127 0d0a 0d0a 2020 2020 2020  1&a=1'....      
-00005620: 2020 7265 706c 6163 655f 6b77 6172 6773    replace_kwargs
-00005630: 2069 7320 6120 6469 6374 2074 6f20 7570   is a dict to up
-00005640: 6461 7465 2061 7474 7269 6275 7465 7320  date attributes 
-00005650: 6265 666f 7265 2073 6f72 7469 6e67 2020  before sorting  
-00005660: 2873 7563 6820 6173 2073 6368 656d 6520  (such as scheme 
-00005670: 2f20 6e65 746c 6f63 2e2e 2e29 2e0d 0a20  / netloc...)... 
-00005680: 2020 200d 0a0d 0a2d 2d2d 0d0a 0d0a          ....---....
+00004960: 6173 796e 6369 6f2e 6765 745f 6576 656e  asyncio.get_even
+00004970: 745f 6c6f 6f70 2829 2e72 756e 5f75 6e74  t_loop().run_unt
+00004980: 696c 5f63 6f6d 706c 6574 6528 6d61 696e  il_complete(main
+00004990: 2829 290d 0a0d 0a20 2020 2020 2020 2020  ())....         
+000049a0: 2020 2074 6573 745f 7379 6e63 2829 0d0a     test_sync()..
+000049b0: 2020 2020 2020 2020 2020 2020 7465 7374              test
+000049c0: 5f61 7379 6e63 2829 0d0a 0d0a 2020 2020  _async()....    
+000049d0: 2020 2020 2020 2020 2020 2020 6060 600d              ```.
+000049e0: 0a20 2020 200d 0a0d 0a2d 2d2d 0d0a 0d0a  .    ....---....
+000049f0: 0d0a 2020 2020 322e 3520 6046 756e 6353  ..    2.5 `FuncS
+00004a00: 6368 656d 6160 202d 2050 6172 7365 2074  chema` - Parse t
+00004a10: 6865 2070 6172 616d 6574 6572 7320 616e  he parameters an
+00004a20: 6420 7479 7065 7320 7265 7175 6972 6564  d types required
+00004a30: 2062 7920 6120 6675 6e63 7469 6f6e 2069   by a function i
+00004a40: 6e74 6f20 6120 6469 6374 696f 6e61 7279  nto a dictionary
+00004a50: 2c20 616e 6420 636f 6e76 6572 7420 616e  , and convert an
+00004a60: 2069 6e63 6f6d 696e 6720 7061 7261 6d65   incoming parame
+00004a70: 7465 7220 696e 746f 2074 6865 2061 7070  ter into the app
+00004a80: 726f 7072 6961 7465 2074 7970 652e 0d0a  ropriate type...
+00004a90: 0d0a 2020 2020 2020 2020 3e3e 3e20 6465  ..        >>> de
+00004aa0: 6620 7465 7374 2861 2c20 623a 2073 7472  f test(a, b: str
+00004ab0: 2c20 2f2c 2063 3d31 2c20 2a2c 2064 3d5b  , /, c=1, *, d=[
+00004ac0: 2264 225d 2c20 653d 302e 312c 2066 3d7b  "d"], e=0.1, f={
+00004ad0: 2266 227d 2c20 673d 2831 2c20 3229 2c20  "f"}, g=(1, 2), 
+00004ae0: 683d 5472 7565 2c20 693d 7b31 7d2c 202a  h=True, i={1}, *
+00004af0: 2a6b 7773 293a 0d0a 2020 2020 2020 2020  *kws):..        
+00004b00: 2e2e 2e20 2020 2020 7265 7475 726e 0d0a  ...     return..
+00004b10: 2020 2020 2020 2020 3e3e 3e20 4675 6e63          >>> Func
+00004b20: 5363 6865 6d61 2e70 6172 7365 2874 6573  Schema.parse(tes
+00004b30: 7429 0d0a 2020 2020 2020 2020 7b27 6227  t)..        {'b'
+00004b40: 3a20 7b27 7479 7065 273a 203c 636c 6173  : {'type': <clas
+00004b50: 7320 2773 7472 273e 2c20 2764 6566 6175  s 'str'>, 'defau
+00004b60: 6c74 273a 203c 636c 6173 7320 2769 6e73  lt': <class 'ins
+00004b70: 7065 6374 2e5f 656d 7074 7927 3e7d 2c20  pect._empty'>}, 
+00004b80: 2763 273a 207b 2774 7970 6527 3a20 3c63  'c': {'type': <c
+00004b90: 6c61 7373 2027 696e 7427 3e2c 2027 6465  lass 'int'>, 'de
+00004ba0: 6661 756c 7427 3a20 317d 2c20 2764 273a  fault': 1}, 'd':
+00004bb0: 207b 2774 7970 6527 3a20 3c63 6c61 7373   {'type': <class
+00004bc0: 2027 6c69 7374 273e 2c20 2764 6566 6175   'list'>, 'defau
+00004bd0: 6c74 273a 205b 2764 275d 7d2c 2027 6527  lt': ['d']}, 'e'
+00004be0: 3a20 7b27 7479 7065 273a 203c 636c 6173  : {'type': <clas
+00004bf0: 7320 2766 6c6f 6174 273e 2c20 2764 6566  s 'float'>, 'def
+00004c00: 6175 6c74 273a 2030 2e31 7d2c 2027 6627  ault': 0.1}, 'f'
+00004c10: 3a20 7b27 7479 7065 273a 203c 636c 6173  : {'type': <clas
+00004c20: 7320 2773 6574 273e 2c20 2764 6566 6175  s 'set'>, 'defau
+00004c30: 6c74 273a 207b 2766 277d 7d2c 2027 6727  lt': {'f'}}, 'g'
+00004c40: 3a20 7b27 7479 7065 273a 203c 636c 6173  : {'type': <clas
+00004c50: 7320 2774 7570 6c65 273e 2c20 2764 6566  s 'tuple'>, 'def
+00004c60: 6175 6c74 273a 2028 312c 2032 297d 2c20  ault': (1, 2)}, 
+00004c70: 2768 273a 207b 2774 7970 6527 3a20 3c63  'h': {'type': <c
+00004c80: 6c61 7373 2027 626f 6f6c 273e 2c20 2764  lass 'bool'>, 'd
+00004c90: 6566 6175 6c74 273a 2054 7275 657d 2c20  efault': True}, 
+00004ca0: 2769 273a 207b 2774 7970 6527 3a20 3c63  'i': {'type': <c
+00004cb0: 6c61 7373 2027 7365 7427 3e2c 2027 6465  lass 'set'>, 'de
+00004cc0: 6661 756c 7427 3a20 7b31 7d7d 7d0d 0a20  fault': {1}}}.. 
+00004cd0: 2020 2020 2020 203e 3e3e 2046 756e 6353         >>> FuncS
+00004ce0: 6368 656d 612e 636f 6e76 6572 7428 2231  chema.convert("1
+00004cf0: 222c 2069 6e74 290d 0a20 2020 2020 2020  ", int)..       
+00004d00: 2031 0d0a 2020 2020 2020 2020 3e3e 3e20   1..        >>> 
+00004d10: 4675 6e63 5363 6865 6d61 2e63 6f6e 7665  FuncSchema.conve
+00004d20: 7274 2822 3122 2c20 7374 7229 0d0a 2020  rt("1", str)..  
+00004d30: 2020 2020 2020 2731 270d 0a20 2020 2020        '1'..     
+00004d40: 2020 203e 3e3e 2046 756e 6353 6368 656d     >>> FuncSchem
+00004d50: 612e 636f 6e76 6572 7428 2231 222c 2066  a.convert("1", f
+00004d60: 6c6f 6174 290d 0a20 2020 2020 2020 2031  loat)..        1
+00004d70: 2e30 0d0a 2020 2020 2020 2020 3e3e 3e20  .0..        >>> 
+00004d80: 4675 6e63 5363 6865 6d61 2e63 6f6e 7665  FuncSchema.conve
+00004d90: 7274 2830 2c20 626f 6f6c 290d 0a20 2020  rt(0, bool)..   
+00004da0: 2020 2020 2046 616c 7365 0d0a 2020 2020       False..    
+00004db0: 2020 2020 3e3e 3e20 4675 6e63 5363 6865      >>> FuncSche
+00004dc0: 6d61 2e63 6f6e 7665 7274 2827 3127 2c20  ma.convert('1', 
+00004dd0: 626f 6f6c 290d 0a20 2020 2020 2020 2054  bool)..        T
+00004de0: 7275 650d 0a20 2020 2020 2020 203e 3e3e  rue..        >>>
+00004df0: 2046 756e 6353 6368 656d 612e 636f 6e76   FuncSchema.conv
+00004e00: 6572 7428 275b 5b31 2c20 315d 5d27 2c20  ert('[[1, 1]]', 
+00004e10: 6469 6374 290d 0a20 2020 2020 2020 207b  dict)..        {
+00004e20: 313a 2031 7d0d 0a20 2020 2020 2020 203e  1: 1}..        >
+00004e30: 3e3e 2046 756e 6353 6368 656d 612e 636f  >> FuncSchema.co
+00004e40: 6e76 6572 7428 275b 312c 2031 5d27 2c20  nvert('[1, 1]', 
+00004e50: 7365 7429 0d0a 2020 2020 2020 2020 7b31  set)..        {1
+00004e60: 7d0d 0a20 2020 2020 2020 203e 3e3e 2046  }..        >>> F
+00004e70: 756e 6353 6368 656d 612e 636f 6e76 6572  uncSchema.conver
+00004e80: 7428 275b 312c 2031 5d27 2c20 7475 706c  t('[1, 1]', tupl
+00004e90: 6529 0d0a 2020 2020 2020 2020 2831 2c20  e)..        (1, 
+00004ea0: 3129 0d0a 2020 2020 0d0a 0d0a 2d2d 2d0d  1)..    ....---.
+00004eb0: 0a0d 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ...=============
+00004ec0: 3d3d 3d3d 3d3d 3d3d 3d0d 0a0d 0a23 2320  =========....## 
+00004ed0: 332e 206d 6f72 6562 7569 6c74 696e 732e  3. morebuiltins.
+00004ee0: 6970 630d 0a0d 0a0d 0a3d 3d3d 3d3d 3d3d  ipc......=======
+00004ef0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d  ===============.
+00004f00: 0a0d 0a0d 0a20 2020 2033 2e31 2060 4950  .....    3.1 `IP
+00004f10: 4345 6e63 6f64 6572 6020 2d20 416e 2061  CEncoder` - An a
+00004f20: 6273 7472 6163 7420 6261 7365 2063 6c61  bstract base cla
+00004f30: 7373 2066 6f72 2061 6c6c 2065 6e63 6f64  ss for all encod
+00004f40: 6572 733b 2069 6d70 6c65 6d65 6e74 696e  ers; implementin
+00004f50: 6720 7468 6520 6e65 6365 7373 6172 7920  g the necessary 
+00004f60: 636f 6d6d 756e 6963 6174 696f 6e20 7072  communication pr
+00004f70: 6f74 6f63 6f6c 2072 6571 7569 7265 7320  otocol requires 
+00004f80: 6f6e 6c79 2074 6865 2064 6566 696e 6974  only the definit
+00004f90: 696f 6e20 6f66 2074 776f 2061 6273 7472  ion of two abstr
+00004fa0: 6163 7420 6d65 7468 6f64 732e 2042 6520  act methods. Be 
+00004fb0: 6d69 6e64 6675 6c20 7468 6174 2076 6172  mindful that var
+00004fc0: 7969 6e67 2068 6561 6465 7220 6c65 6e67  ying header leng
+00004fd0: 7468 7320 7769 6c6c 2069 6d70 6163 7420  ths will impact 
+00004fe0: 7468 6520 6d61 7869 6d75 6d20 7061 636b  the maximum pack
+00004ff0: 6167 696e 6720 7369 7a65 2e0d 0a0d 0a0d  aging size......
+00005000: 0a2d 2d2d 0d0a 0d0a 0d0a 2020 2020 332e  .---......    3.
+00005010: 3420 6053 6f63 6b65 744c 6f67 4861 6e64  4 `SocketLogHand
+00005020: 6c65 7245 6e63 6f64 6572 6020 2d20 466f  lerEncoder` - Fo
+00005030: 7220 6120 7072 6163 7469 6361 6c20 6465  r a practical de
+00005040: 6d6f 6e73 7472 6174 696f 6e2c 2072 6566  monstration, ref
+00005050: 6572 2074 6f20 7468 6520 7465 7374 2063  er to the test c
+00005060: 6f64 653a 206d 6f72 6562 7569 6c74 696e  ode: morebuiltin
+00005070: 732f 6970 632e 7079 3a5f 7465 7374 5f69  s/ipc.py:_test_i
+00005080: 7063 5f6c 6f67 6769 6e67 2e0d 0a0d 0a20  pc_logging..... 
+00005090: 2020 2020 2020 2060 6060 0d0a 2020 2020         ```..    
+000050a0: 2020 2020 6173 796e 6320 6465 6620 5f74      async def _t
+000050b0: 6573 745f 6970 635f 6c6f 6767 696e 6728  est_ipc_logging(
+000050c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000050d0: 696d 706f 7274 206c 6f67 6769 6e67 0d0a  import logging..
+000050e0: 0d0a 2020 2020 2020 2020 2020 2020 686f  ..            ho
+000050f0: 7374 203d 2022 3132 372e 302e 302e 3122  st = "127.0.0.1"
+00005100: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
+00005110: 7274 203d 2038 3039 300d 0a20 2020 2020  rt = 8090..     
+00005120: 2020 2020 2020 2061 7379 6e63 2077 6974         async wit
+00005130: 6820 536f 636b 6574 5365 7276 6572 2868  h SocketServer(h
+00005140: 6f73 743d 686f 7374 2c20 706f 7274 3d70  ost=host, port=p
+00005150: 6f72 742c 2065 6e63 6f64 6572 3d53 6f63  ort, encoder=Soc
+00005160: 6b65 744c 6f67 4861 6e64 6c65 7245 6e63  ketLogHandlerEnc
+00005170: 6f64 6572 2829 293a 0d0a 2020 2020 2020  oder()):..      
+00005180: 2020 2020 2020 2020 2020 2320 736f 636b            # sock
+00005190: 6574 206c 6f67 6765 7220 6465 6d6f 0d0a  et logger demo..
+000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051b0: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
+000051c0: 3d3d 3d3d 0d0a 2020 2020 2020 2020 2020  ====..          
+000051d0: 2020 2020 2020 6c6f 6767 6572 203d 206c        logger = l
+000051e0: 6f67 6769 6e67 2e67 6574 4c6f 6767 6572  ogging.getLogger
+000051f0: 2822 7465 7374 5f6c 6f67 6765 7222 290d  ("test_logger").
+00005200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005210: 206c 6f67 6765 722e 7365 744c 6576 656c   logger.setLevel
+00005220: 286c 6f67 6769 6e67 2e44 4542 5547 290d  (logging.DEBUG).
+00005230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005240: 2068 203d 2053 6f63 6b65 7448 616e 646c   h = SocketHandl
+00005250: 6572 2868 6f73 742c 2070 6f72 7429 0d0a  er(host, port)..
+00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005270: 682e 7365 744c 6576 656c 286c 6f67 6769  h.setLevel(loggi
+00005280: 6e67 2e44 4542 5547 290d 0a20 2020 2020  ng.DEBUG)..     
+00005290: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+000052a0: 722e 6164 6448 616e 646c 6572 2868 290d  r.addHandler(h).
+000052b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000052c0: 206c 6f67 6765 722e 696e 666f 2822 7465   logger.info("te
+000052d0: 7374 2073 6f63 6b65 7422 290d 0a20 2020  st socket")..   
+000052e0: 2020 2020 2020 2020 2020 2020 2023 203d               # =
+000052f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005300: 3d0d 0a0d 0a20 2020 2020 2020 2020 2020  =....           
+00005310: 2020 2020 2023 2065 6e73 7572 6520 7465       # ensure te
+00005320: 7374 2063 6173 650d 0a20 2020 2020 2020  st case..       
+00005330: 2020 2020 2020 2020 2061 7761 6974 2061           await a
+00005340: 7379 6e63 696f 2e73 6c65 6570 2830 2e31  syncio.sleep(0.1
+00005350: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00005360: 2020 2061 7373 6572 7420 7069 636b 6c65     assert pickle
+00005370: 2e6c 6f61 6473 2868 2e73 6f63 6b2e 7265  .loads(h.sock.re
+00005380: 6376 2831 3030 3030 3029 5b34 3a5d 295b  cv(100000)[4:])[
+00005390: 226e 616d 6522 5d20 3d3d 206c 6f67 6765  "name"] == logge
+000053a0: 722e 6e61 6d65 0d0a 2020 2020 2020 2020  r.name..        
+000053b0: 6060 600d 0a20 2020 2020 2020 2041 6e64  ```..        And
+000053c0: 2070 726f 7669 6465 2061 2073 696d 706c   provide a simpl
+000053d0: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+000053e0: 2066 6f72 2067 656e 6572 6174 696e 6720   for generating 
+000053f0: 6c6f 6773 2066 6f72 2063 6f72 6f75 7469  logs for corouti
+00005400: 6e65 2063 6f64 6520 7769 7468 2043 6c69  ne code with Cli
+00005410: 656e 7420 7573 6167 652e 0d0a 2020 2020  ent usage...    
+00005420: 0d0a 0d0a 2d2d 2d0d 0a0d 0a0d 0a20 2020  ....---......   
+00005430: 2033 2e35 2060 536f 636b 6574 5365 7276   3.5 `SocketServ
+00005440: 6572 6020 2d20 546f 2073 6565 2061 6e20  er` - To see an 
+00005450: 6578 616d 706c 6520 696e 2061 6374 696f  example in actio
+00005460: 6e2c 2076 6965 7720 7468 6520 7465 7374  n, view the test
+00005470: 2063 6f64 653a 206d 6f72 6562 7569 6c74   code: morebuilt
+00005480: 696e 732f 6970 632e 7079 3a5f 7465 7374  ins/ipc.py:_test
+00005490: 5f69 7063 2e0d 0a0d 0a20 2020 2020 2020  _ipc.....       
+000054a0: 2020 2020 2060 6060 0d0a 2020 2020 2020       ```..      
+000054b0: 2020 6173 796e 6320 6465 6620 7465 7374    async def test
+000054c0: 5f63 6c69 656e 7428 686f 7374 3d22 3132  _client(host="12
+000054d0: 372e 302e 302e 3122 2c20 706f 7274 3d38  7.0.0.1", port=8
+000054e0: 3039 302c 2065 6e63 6f64 6572 3d4e 6f6e  090, encoder=Non
+000054f0: 652c 2063 6173 6573 3d4e 6f6e 6529 3a0d  e, cases=None):.
+00005500: 0a20 2020 2020 2020 2020 2020 2061 7379  .            asy
+00005510: 6e63 2077 6974 6820 536f 636b 6574 436c  nc with SocketCl
+00005520: 6965 6e74 2868 6f73 743d 686f 7374 2c20  ient(host=host, 
+00005530: 706f 7274 3d70 6f72 742c 2065 6e63 6f64  port=port, encod
+00005540: 6572 3d65 6e63 6f64 6572 2920 6173 2063  er=encoder) as c
+00005550: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00005560: 2020 2066 6f72 2063 6173 6520 696e 2063     for case in c
+00005570: 6173 6573 3a0d 0a20 2020 2020 2020 2020  ases:..         
+00005580: 2020 2020 2020 2020 2020 2061 7761 6974             await
+00005590: 2063 2e73 656e 6428 6361 7365 290d 0a20   c.send(case).. 
+000055a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055b0: 2020 2072 6573 706f 6e73 6520 3d20 6177     response = aw
+000055c0: 6169 7420 632e 7265 6376 2829 0d0a 2020  ait c.recv()..  
+000055d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055e0: 2020 6966 2067 6c6f 6261 6c73 2829 2e67    if globals().g
+000055f0: 6574 2822 7072 696e 745f 6c6f 6722 293a  et("print_log"):
+00005600: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005610: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00005620: 225b 436c 6965 6e74 5d22 2c20 2273 656e  "[Client]", "sen
+00005630: 643a 222c 2072 6570 7228 6361 7365 292c  d:", repr(case),
+00005640: 2022 3d3e 222c 2022 7265 6376 3a22 2c20   "=>", "recv:", 
+00005650: 7265 7072 2872 6573 706f 6e73 6529 290d  repr(response)).
+00005660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005670: 2020 2020 2061 7373 6572 7420 6361 7365       assert case
+00005680: 203d 3d20 7265 7370 6f6e 7365 206f 7220   == response or 
+00005690: 7374 7228 6361 7365 2920 3d3d 2072 6573  str(case) == res
+000056a0: 706f 6e73 652c 205b 6361 7365 2c20 7265  ponse, [case, re
+000056b0: 7370 6f6e 7365 5d0d 0a20 2020 2020 2020  sponse]..       
+000056c0: 2020 2020 2020 2020 2061 7761 6974 2063           await c
+000056d0: 2e73 656e 6428 225b 7368 7574 646f 776e  .send("[shutdown
+000056e0: 2073 6572 7665 725d 2229 0d0a 0d0a 0d0a   server]")......
+000056f0: 2020 2020 2020 2020 6173 796e 6320 6465          async de
+00005700: 6620 5f74 6573 745f 6970 6328 293a 0d0a  f _test_ipc():..
+00005710: 2020 2020 2020 2020 2020 2020 696d 706f              impo
+00005720: 7274 2070 6c61 7466 6f72 6d0d 0a0d 0a20  rt platform.... 
+00005730: 2020 2020 2020 2020 2020 204a 534f 4e45             JSONE
+00005740: 6e63 6f64 6572 2e5f 4455 4d50 5f4b 5741  ncoder._DUMP_KWA
+00005750: 5247 535b 2264 6566 6175 6c74 225d 203d  RGS["default"] =
+00005760: 2073 7472 0d0a 2020 2020 2020 2020 2020   str..          
+00005770: 2020 666f 7220 656e 632c 2063 6173 6573    for enc, cases
+00005780: 2069 6e20 5b0d 0a20 2020 2020 2020 2020   in [..         
+00005790: 2020 2020 2020 205b 5069 636b 6c65 456e         [PickleEn
+000057a0: 636f 6465 722c 205b 3132 332c 2022 3132  coder, [123, "12
+000057b0: 3322 2c20 4e6f 6e65 2c20 7b22 6122 7d2c  3", None, {"a"},
+000057c0: 205b 2261 225d 2c20 2822 6122 2c29 2c20   ["a"], ("a",), 
+000057d0: 7b22 6122 3a20 317d 5d5d 2c0d 0a20 2020  {"a": 1}]],..   
+000057e0: 2020 2020 2020 2020 2020 2020 205b 4a53               [JS
+000057f0: 4f4e 456e 636f 6465 722c 205b 3132 332c  ONEncoder, [123,
+00005800: 2022 3132 3322 2c20 4e6f 6e65 2c20 7b22   "123", None, {"
+00005810: 6122 7d2c 205b 2261 225d 2c20 7b22 6122  a"}, ["a"], {"a"
+00005820: 3a20 317d 5d5d 2c0d 0a20 2020 2020 2020  : 1}]],..       
+00005830: 2020 2020 205d 3a0d 0a20 2020 2020 2020       ]:..       
+00005840: 2020 2020 2020 2020 2065 6e63 6f64 6572           encoder
+00005850: 203d 2065 6e63 2829 0d0a 2020 2020 2020   = enc()..      
+00005860: 2020 2020 2020 2020 2020 6966 2070 6c61            if pla
+00005870: 7466 6f72 6d2e 7379 7374 656d 2829 203d  tform.system() =
+00005880: 3d20 224c 696e 7578 223a 0d0a 2020 2020  = "Linux":..    
+00005890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058a0: 2320 7465 7374 2075 6e69 7820 646f 6d61  # test unix doma
+000058b0: 696e 2073 6f63 6b65 740d 0a20 2020 2020  in socket..     
+000058c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000058d0: 7269 6e74 2822 5465 7374 204c 696e 7578  rint("Test Linux
+000058e0: 2055 6e69 7820 446f 6d61 696e 2053 6f63   Unix Domain Soc
+000058f0: 6b65 7422 290d 0a20 2020 2020 2020 2020  ket")..         
+00005900: 2020 2020 2020 2020 2020 2068 6f73 7420             host 
+00005910: 3d20 222f 746d 702f 7564 732e 736f 636b  = "/tmp/uds.sock
+00005920: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00005930: 2020 2020 2020 2070 6f72 7420 3d20 4e6f         port = No
+00005940: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
+00005950: 2020 2020 2020 2020 6173 796e 6320 7769          async wi
+00005960: 7468 2053 6f63 6b65 7453 6572 7665 7228  th SocketServer(
+00005970: 686f 7374 3d68 6f73 742c 2070 6f72 743d  host=host, port=
+00005980: 706f 7274 2c20 656e 636f 6465 723d 656e  port, encoder=en
+00005990: 636f 6465 7229 3a0d 0a20 2020 2020 2020  coder):..       
+000059a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059b0: 2061 7761 6974 2074 6573 745f 636c 6965   await test_clie
+000059c0: 6e74 2868 6f73 742c 2070 6f72 743d 4e6f  nt(host, port=No
+000059d0: 6e65 2c20 656e 636f 6465 723d 656e 636f  ne, encoder=enco
+000059e0: 6465 722c 2063 6173 6573 3d63 6173 6573  der, cases=cases
+000059f0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00005a00: 2020 2020 2023 2074 6573 7420 736f 636b       # test sock
+00005a10: 6574 0d0a 2020 2020 2020 2020 2020 2020  et..            
+00005a20: 2020 2020 686f 7374 203d 2022 3132 372e      host = "127.
+00005a30: 302e 302e 3122 0d0a 2020 2020 2020 2020  0.0.1"..        
+00005a40: 2020 2020 2020 2020 706f 7274 203d 2038          port = 8
+00005a50: 3039 300d 0a20 2020 2020 2020 2020 2020  090..           
+00005a60: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
+00005a70: 536f 636b 6574 5365 7276 6572 2868 6f73  SocketServer(hos
+00005a80: 743d 686f 7374 2c20 706f 7274 3d70 6f72  t=host, port=por
+00005a90: 742c 2065 6e63 6f64 6572 3d65 6e63 6f64  t, encoder=encod
+00005aa0: 6572 293a 0d0a 2020 2020 2020 2020 2020  er):..          
+00005ab0: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00005ac0: 7465 7374 5f63 6c69 656e 7428 686f 7374  test_client(host
+00005ad0: 3d22 3132 372e 302e 302e 3122 2c20 706f  ="127.0.0.1", po
+00005ae0: 7274 3d38 3039 302c 2065 6e63 6f64 6572  rt=8090, encoder
+00005af0: 3d65 6e63 6f64 6572 2c20 6361 7365 733d  =encoder, cases=
+00005b00: 6361 7365 7329 0d0a 0d0a 0d0a 2020 2020  cases)......    
+00005b10: 2020 2020 2020 2020 6060 600d 0a20 2020          ```..   
+00005b20: 200d 0a0d 0a2d 2d2d 0d0a 0d0a 3d3d 3d3d   ....---....====
+00005b30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005b40: 3d3d 0d0a 0d0a 2323 2034 2e20 6d6f 7265  ==....## 4. more
+00005b50: 6275 696c 7469 6e73 2e72 6571 7565 7374  builtins.request
+00005b60: 0d0a 0d0a 0d0a 3d3d 3d3d 3d3d 3d3d 3d3d  ......==========
+00005b70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 0d0a  ============....
+00005b80: 0d0a 2020 2020 342e 3120 6072 6571 6020  ..    4.1 `req` 
+00005b90: 2d20 4120 6261 7369 6320 6d6f 636b 2066  - A basic mock f
+00005ba0: 6f72 2072 6571 7565 7374 732c 2070 6572  or requests, per
+00005bb0: 666f 726d 616e 7420 616c 6265 6974 2073  formant albeit s
+00005bc0: 696d 706c 6973 7469 632e 0d0a 0d0a 2020  implistic.....  
+00005bd0: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
+00005be0: 2074 696d 650d 0a20 2020 2020 2020 203e   time..        >
+00005bf0: 3e3e 2072 203d 2072 6571 2e67 6574 2822  >> r = req.get("
+00005c00: 6874 7470 733a 2f2f 706f 7374 6d61 6e2d  https://postman-
+00005c10: 6563 686f 2e63 6f6d 2f67 6574 3f61 3d32  echo.com/get?a=2
+00005c20: 222c 2074 696d 656f 7574 3d33 2c20 7061  ", timeout=3, pa
+00005c30: 7261 6d73 3d7b 2262 223a 2022 3322 7d29  rams={"b": "3"})
+00005c40: 0d0a 2020 2020 2020 2020 3e3e 3e20 722e  ..        >>> r.
+00005c50: 7572 6c0d 0a20 2020 2020 2020 2027 6874  url..        'ht
+00005c60: 7470 733a 2f2f 706f 7374 6d61 6e2d 6563  tps://postman-ec
+00005c70: 686f 2e63 6f6d 2f67 6574 3f61 3d32 2662  ho.com/get?a=2&b
+00005c80: 3d33 270d 0a20 2020 2020 2020 203e 3e3e  =3'..        >>>
+00005c90: 2072 2e6f 6b0d 0a20 2020 2020 2020 2054   r.ok..        T
+00005ca0: 7275 650d 0a20 2020 2020 2020 203e 3e3e  rue..        >>>
+00005cb0: 2072 2e73 7461 7475 735f 636f 6465 0d0a   r.status_code..
+00005cc0: 2020 2020 2020 2020 3230 300d 0a20 2020          200..   
+00005cd0: 2020 2020 203e 3e3e 2072 2e74 6578 742e       >>> r.text.
+00005ce0: 7374 6172 7473 7769 7468 2827 7b27 290d  startswith('{').
+00005cf0: 0a20 2020 2020 2020 2054 7275 650d 0a20  .        True.. 
+00005d00: 2020 2020 2020 203e 3e3e 2072 203d 2072         >>> r = r
+00005d10: 6571 2e70 6f73 7428 2268 7474 7073 3a2f  eq.post("https:/
+00005d20: 2f70 6f73 746d 616e 2d65 6368 6f2e 636f  /postman-echo.co
+00005d30: 6d2f 706f 7374 3f61 3d32 222c 2074 696d  m/post?a=2", tim
+00005d40: 656f 7574 3d33 2c20 7061 7261 6d73 3d7b  eout=3, params={
+00005d50: 2262 223a 2022 3322 7d2c 2064 6174 613d  "b": "3"}, data=
+00005d60: 6222 6d6f 636b 2064 6174 6122 290d 0a20  b"mock data").. 
+00005d70: 2020 2020 2020 203e 3e3e 2072 2e6a 736f         >>> r.jso
+00005d80: 6e28 295b 2264 6174 6122 5d0d 0a20 2020  n()["data"]..   
+00005d90: 2020 2020 2027 6d6f 636b 2064 6174 6127       'mock data'
+00005da0: 0d0a 2020 2020 2020 2020 3e3e 3e20 722e  ..        >>> r.
+00005db0: 6a73 6f6e 2829 5b22 6172 6773 225d 0d0a  json()["args"]..
+00005dc0: 2020 2020 2020 2020 7b27 6127 3a20 2732          {'a': '2
+00005dd0: 272c 2027 6227 3a20 2733 277d 0d0a 2020  ', 'b': '3'}..  
+00005de0: 2020 2020 2020 3e3e 3e20 7220 3d20 7265        >>> r = re
+00005df0: 712e 706f 7374 2822 6874 7470 733a 2f2f  q.post("https://
+00005e00: 706f 7374 6d61 6e2d 6563 686f 2e63 6f6d  postman-echo.com
+00005e10: 2f70 6f73 743f 613d 3222 2c20 7469 6d65  /post?a=2", time
+00005e20: 6f75 743d 332c 206a 736f 6e3d 7b22 6461  out=3, json={"da
+00005e30: 7461 223a 2022 7965 7320 6a73 6f6e 227d  ta": "yes json"}
+00005e40: 290d 0a20 2020 2020 2020 203e 3e3e 2072  )..        >>> r
+00005e50: 2e6a 736f 6e28 295b 226a 736f 6e22 5d0d  .json()["json"].
+00005e60: 0a20 2020 2020 2020 207b 2764 6174 6127  .        {'data'
+00005e70: 3a20 2779 6573 206a 736f 6e27 7d0d 0a20  : 'yes json'}.. 
+00005e80: 2020 200d 0a0d 0a2d 2d2d 0d0a 0d0a 0d0a     ....---......
+00005e90: 2020 2020 342e 3220 6044 6f6d 6169 6e50      4.2 `DomainP
+00005ea0: 6172 7365 7260 202d 2045 7874 7261 6374  arser` - Extract
+00005eb0: 7320 7468 6520 5365 636f 6e64 2d6c 6576  s the Second-lev
+00005ec0: 656c 2064 6f6d 6169 6e20 2853 4c44 2920  el domain (SLD) 
+00005ed0: 6672 6f6d 2061 2070 726f 7669 6465 6420  from a provided 
+00005ee0: 686f 7374 6e61 6d65 206f 7220 5552 4c2e  hostname or URL.
+00005ef0: 0d0a 0d0a 2020 2020 2020 2020 3e3e 3e20  ....        >>> 
+00005f00: 646f 6d61 696e 5f70 6172 7365 7220 3d20  domain_parser = 
+00005f10: 446f 6d61 696e 5061 7273 6572 2829 0d0a  DomainParser()..
+00005f20: 2020 2020 2020 2020 3e3e 3e20 646f 6d61          >>> doma
+00005f30: 696e 5f70 6172 7365 722e 7061 7273 655f  in_parser.parse_
+00005f40: 686f 7374 6e61 6d65 2822 6769 7468 7562  hostname("github
+00005f50: 2e63 6f6d 2229 0d0a 2020 2020 2020 2020  .com")..        
+00005f60: 2767 6974 6875 622e 636f 6d27 0d0a 2020  'github.com'..  
+00005f70: 2020 2020 2020 3e3e 3e20 646f 6d61 696e        >>> domain
+00005f80: 5f70 6172 7365 722e 7061 7273 655f 686f  _parser.parse_ho
+00005f90: 7374 6e61 6d65 2822 7777 772e 6769 7468  stname("www.gith
+00005fa0: 7562 2e63 6f6d 2229 0d0a 2020 2020 2020  ub.com")..      
+00005fb0: 2020 2767 6974 6875 622e 636f 6d27 0d0a    'github.com'..
+00005fc0: 2020 2020 2020 2020 3e3e 3e20 646f 6d61          >>> doma
+00005fd0: 696e 5f70 6172 7365 722e 7061 7273 655f  in_parser.parse_
+00005fe0: 686f 7374 6e61 6d65 2822 7777 772e 6170  hostname("www.ap
+00005ff0: 692e 6769 7468 7562 2e63 6f6d 2e63 6e22  i.github.com.cn"
+00006000: 290d 0a20 2020 2020 2020 2027 6769 7468  )..        'gith
+00006010: 7562 2e63 6f6d 2e63 6e27 0d0a 2020 2020  ub.com.cn'..    
+00006020: 2020 2020 3e3e 3e20 646f 6d61 696e 5f70      >>> domain_p
+00006030: 6172 7365 722e 7061 7273 655f 686f 7374  arser.parse_host
+00006040: 6e61 6d65 2822 612e 622e 632e 6b61 7761  name("a.b.c.kawa
+00006050: 7361 6b69 2e6a 7022 290d 0a20 2020 2020  saki.jp")..     
+00006060: 2020 2027 632e 6b61 7761 7361 6b69 2e6a     'c.kawasaki.j
+00006070: 7027 0d0a 2020 2020 2020 2020 3e3e 3e20  p'..        >>> 
+00006080: 646f 6d61 696e 5f70 6172 7365 722e 7061  domain_parser.pa
+00006090: 7273 655f 686f 7374 6e61 6d65 2822 612e  rse_hostname("a.
+000060a0: 622e 632e 6369 7479 2e6b 6177 6173 616b  b.c.city.kawasak
+000060b0: 692e 6a70 2229 0d0a 2020 2020 2020 2020  i.jp")..        
+000060c0: 2763 2e63 6974 792e 6b61 7761 7361 6b69  'c.city.kawasaki
+000060d0: 2e6a 7027 0d0a 2020 2020 2020 2020 3e3e  .jp'..        >>
+000060e0: 3e20 646f 6d61 696e 5f70 6172 7365 722e  > domain_parser.
+000060f0: 7061 7273 655f 686f 7374 6e61 6d65 2822  parse_hostname("
+00006100: 612e 6262 6262 6262 2e63 6363 6363 6322  a.bbbbbb.cccccc"
+00006110: 290d 0a20 2020 2020 2020 2027 270d 0a20  )..        ''.. 
+00006120: 2020 2020 2020 203e 3e3e 2064 6f6d 6169         >>> domai
+00006130: 6e5f 7061 7273 6572 2e70 6172 7365 5f68  n_parser.parse_h
+00006140: 6f73 746e 616d 6528 2261 2e62 6262 6262  ostname("a.bbbbb
+00006150: 622e 6363 6363 6363 222c 2064 6566 6175  b.cccccc", defau
+00006160: 6c74 3d22 622e 6322 290d 0a20 2020 2020  lt="b.c")..     
+00006170: 2020 2027 622e 6327 0d0a 2020 2020 2020     'b.c'..      
+00006180: 2020 3e3e 3e20 646f 6d61 696e 5f70 6172    >>> domain_par
+00006190: 7365 722e 7061 7273 655f 7572 6c28 2268  ser.parse_url("h
+000061a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000061b0: 6d2f 436c 6572 6963 5079 2f6d 6f72 6562  m/ClericPy/moreb
+000061c0: 7569 6c74 696e 7322 290d 0a20 2020 2020  uiltins")..     
+000061d0: 2020 2027 6769 7468 7562 2e63 6f6d 270d     'github.com'.
+000061e0: 0a0d 0a20 2020 200d 0a0d 0a2d 2d2d 0d0a  ...    ....---..
+000061f0: 0d0a 0d0a 2020 2020 342e 3320 6075 6e70  ....    4.3 `unp
+00006200: 6172 7365 5f71 736c 6020 2d20 5072 6f76  arse_qsl` - Prov
+00006210: 6964 6573 2074 6865 2069 6e76 6572 7365  ides the inverse
+00006220: 206f 7065 7261 7469 6f6e 206f 6620 7061   operation of pa
+00006230: 7273 655f 7173 6c2c 2063 6f6e 7665 7274  rse_qsl, convert
+00006240: 696e 6720 7175 6572 7920 7374 7269 6e67  ing query string
+00006250: 206c 6973 7473 2062 6163 6b20 696e 746f   lists back into
+00006260: 2061 2055 524c 2d65 6e63 6f64 6564 2073   a URL-encoded s
+00006270: 7472 696e 672e 0d0a 0d0a 0d0a 2d2d 2d0d  tring.......---.
+00006280: 0a0d 0a0d 0a20 2020 2034 2e34 2060 7570  .....    4.4 `up
+00006290: 6461 7465 5f75 726c 6020 2d20 4f72 6761  date_url` - Orga
+000062a0: 6e69 7a65 7320 7468 6520 7175 6572 7920  nizes the query 
+000062b0: 6172 6775 6d65 6e74 7320 7769 7468 696e  arguments within
+000062c0: 2061 2055 524c 2074 6f20 7374 616e 6461   a URL to standa
+000062d0: 7264 697a 6520 6974 7320 666f 726d 6174  rdize its format
+000062e0: 2e0d 0a0d 0a20 2020 2020 2020 203e 3e3e  .....        >>>
+000062f0: 2075 7064 6174 655f 7572 6c28 2768 7474   update_url('htt
+00006300: 703a 2f2f 7777 772e 6769 7468 7562 2e63  p://www.github.c
+00006310: 6f6d 3f62 3d31 2663 3d31 2661 3d31 272c  om?b=1&c=1&a=1',
+00006320: 207b 2262 223a 204e 6f6e 652c 2022 6322   {"b": None, "c"
+00006330: 3a20 4e6f 6e65 7d29 2020 2320 7265 6d6f  : None})  # remo
+00006340: 7665 2070 6172 616d 730d 0a20 2020 2020  ve params..     
+00006350: 2020 2027 6874 7470 3a2f 2f77 7777 2e67     'http://www.g
+00006360: 6974 6875 622e 636f 6d3f 613d 3127 0d0a  ithub.com?a=1'..
+00006370: 2020 2020 2020 2020 3e3e 3e20 7570 6461          >>> upda
+00006380: 7465 5f75 726c 2822 6874 7470 3a2f 2f77  te_url("http://w
+00006390: 7777 2e67 6974 6875 622e 636f 6d3f 623d  ww.github.com?b=
+000063a0: 3126 633d 3126 613d 3122 2c20 613d 2231  1&c=1&a=1", a="1
+000063b0: 3233 222c 2062 3d4e 6f6e 6529 2020 2320  23", b=None)  # 
+000063c0: 7570 6461 7465 2070 6172 616d 7320 7769  update params wi
+000063d0: 7468 206b 7761 7267 730d 0a20 2020 2020  th kwargs..     
+000063e0: 2020 2027 6874 7470 3a2f 2f77 7777 2e67     'http://www.g
+000063f0: 6974 6875 622e 636f 6d3f 633d 3126 613d  ithub.com?c=1&a=
+00006400: 3132 3327 0d0a 2020 2020 2020 2020 3e3e  123'..        >>
+00006410: 3e20 7570 6461 7465 5f75 726c 2827 6874  > update_url('ht
+00006420: 7470 3a2f 2f77 7777 2e67 6974 6875 622e  tp://www.github.
+00006430: 636f 6d3f 623d 3126 633d 3126 613d 3127  com?b=1&c=1&a=1'
+00006440: 2c20 736f 7274 3d54 7275 6529 2020 2320  , sort=True)  # 
+00006450: 736f 7274 2070 6172 616d 730d 0a20 2020  sort params..   
+00006460: 2020 2020 2027 6874 7470 3a2f 2f77 7777       'http://www
+00006470: 2e67 6974 6875 622e 636f 6d3f 613d 3126  .github.com?a=1&
+00006480: 623d 3126 633d 3127 0d0a 2020 2020 2020  b=1&c=1'..      
+00006490: 2020 3e3e 3e20 7570 6461 7465 5f75 726c    >>> update_url
+000064a0: 2822 6874 7470 3a2f 2f77 7777 2e67 6974  ("http://www.git
+000064b0: 6875 622e 636f 6d3f 623d 3126 633d 3126  hub.com?b=1&c=1&
+000064c0: 613d 3122 2c20 7b22 6122 3a20 2239 3939  a=1", {"a": "999
+000064d0: 227d 2920 2023 2075 7064 6174 6520 7061  "})  # update pa
+000064e0: 7261 6d73 0d0a 2020 2020 2020 2020 2768  rams..        'h
+000064f0: 7474 703a 2f2f 7777 772e 6769 7468 7562  ttp://www.github
+00006500: 2e63 6f6d 3f62 3d31 2663 3d31 2661 3d39  .com?b=1&c=1&a=9
+00006510: 3939 270d 0a20 2020 2020 2020 203e 3e3e  99'..        >>>
+00006520: 2075 7064 6174 655f 7572 6c28 2268 7474   update_url("htt
+00006530: 703a 2f2f 7777 772e 6769 7468 7562 2e63  p://www.github.c
+00006540: 6f6d 3f62 3d31 2663 3d31 2661 3d31 222c  om?b=1&c=1&a=1",
+00006550: 2072 6570 6c61 6365 5f6b 7761 7267 733d   replace_kwargs=
+00006560: 7b22 6e65 746c 6f63 223a 2022 7777 772e  {"netloc": "www.
+00006570: 6e65 775f 686f 7374 2e63 6f6d 227d 2920  new_host.com"}) 
+00006580: 2023 2075 7064 6174 6520 6e65 746c 6f63   # update netloc
+00006590: 0d0a 2020 2020 2020 2020 2768 7474 703a  ..        'http:
+000065a0: 2f2f 7777 772e 6e65 775f 686f 7374 2e63  //www.new_host.c
+000065b0: 6f6d 3f62 3d31 2663 3d31 2661 3d31 270d  om?b=1&c=1&a=1'.
+000065c0: 0a0d 0a20 2020 2020 2020 2072 6570 6c61  ...        repla
+000065d0: 6365 5f6b 7761 7267 7320 6973 2061 2064  ce_kwargs is a d
+000065e0: 6963 7420 746f 2075 7064 6174 6520 6174  ict to update at
+000065f0: 7472 6962 7574 6573 2062 6566 6f72 6520  tributes before 
+00006600: 736f 7274 696e 6720 2028 7375 6368 2061  sorting  (such a
+00006610: 7320 7363 6865 6d65 202f 206e 6574 6c6f  s scheme / netlo
+00006620: 632e 2e2e 292e 0d0a 2020 2020 0d0a 0d0a  c...)...    ....
+00006630: 2d2d 2d0d 0a0d 0a3d 3d3d 3d3d 3d3d 3d3d  ---....=========
+00006640: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d 0a0d  =============...
+00006650: 0a23 2320 352e 206d 6f72 6562 7569 6c74  .## 5. morebuilt
+00006660: 696e 732e 646f 776e 6c6f 6164 5f70 7974  ins.download_pyt
+00006670: 686f 6e0d 0a0d 0a0d 0a3d 3d3d 3d3d 3d3d  hon......=======
+00006680: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d  ===============.
+00006690: 0a0d 0a0d 0a20 2020 2035 2e31 2060 646f  .....    5.1 `do
+000066a0: 776e 6c6f 6164 5f70 7974 686f 6e60 202d  wnload_python` -
+000066b0: 2055 7361 6765 3a20 7079 7468 6f6e 202d   Usage: python -
+000066c0: 6d20 6d6f 7265 6275 696c 7469 6e73 2e64  m morebuiltins.d
+000066d0: 6f77 6e6c 6f61 645f 7079 7468 6f6e 0d0a  ownload_python..
+000066e0: 0d0a 2020 2020 2020 2020 cebb 2070 7974  ..        .. pyt
+000066f0: 686f 6e20 2d6d 206d 6f72 6562 7569 6c74  hon -m morebuilt
+00006700: 696e 732e 646f 776e 6c6f 6164 5f70 7974  ins.download_pyt
+00006710: 686f 6e0d 0a20 2020 2020 2020 2056 6965  hon..        Vie
+00006720: 7720 7468 6520 7275 6c65 733a 0d0a 2020  w the rules:..  
+00006730: 2020 2020 2020 6874 7470 733a 2f2f 6772        https://gr
+00006740: 6567 6f72 7973 7a6f 7263 2e63 6f6d 2f64  egoryszorc.com/d
+00006750: 6f63 732f 7079 7468 6f6e 2d62 7569 6c64  ocs/python-build
+00006760: 2d73 7461 6e64 616c 6f6e 652f 6d61 696e  -standalone/main
+00006770: 2f72 756e 6e69 6e67 2e68 746d 6c23 6f62  /running.html#ob
+00006780: 7461 696e 696e 672d 6469 7374 7269 6275  taining-distribu
+00006790: 7469 6f6e 730d 0a0d 0a20 2020 2020 2020  tions....       
+000067a0: 2047 6f74 2032 3930 2075 726c 7320 6672   Got 290 urls fr
+000067b0: 6f6d 2067 6974 6875 622e 0d0a 0d0a 2020  om github.....  
+000067c0: 2020 2020 2020 5b32 3930 5d20 456e 7465        [290] Ente
+000067d0: 7220 6b65 7977 6f72 6473 2028 6361 6e20  r keywords (can 
+000067e0: 6265 2069 6e74 2069 6e64 6578 206f 7220  be int index or 
+000067f0: 7061 7274 6961 6c20 6d61 7463 682c 2064  partial match, d
+00006800: 6566 6175 6c74 7320 746f 2030 293a 0d0a  efaults to 0):..
+00006810: 2020 2020 2020 2020 302e 2077 696e 646f          0. windo
+00006820: 7773 0d0a 2020 2020 2020 2020 312e 206c  ws..        1. l
+00006830: 696e 7578 0d0a 2020 2020 2020 2020 322e  inux..        2.
+00006840: 2064 6172 7769 6e0d 0a0d 0a20 2020 2020   darwin....     
+00006850: 2020 2046 696c 7420 7769 7468 206b 6579     Filt with key
+00006860: 776f 7264 3a20 2277 696e 646f 7773 222e  word: "windows".
+00006870: 2032 3930 203d 3e20 3430 0d0a 0d0a 2020   290 => 40....  
+00006880: 2020 2020 2020 5b34 305d 2045 6e74 6572        [40] Enter
+00006890: 206b 6579 776f 7264 7320 2863 616e 2062   keywords (can b
+000068a0: 6520 696e 7420 696e 6465 7820 6f72 2070  e int index or p
+000068b0: 6172 7469 616c 206d 6174 6368 2c20 6465  artial match, de
+000068c0: 6661 756c 7473 2074 6f20 3029 3a0d 0a20  faults to 0):.. 
+000068d0: 2020 2020 2020 2030 2e20 332e 3132 2e33         0. 3.12.3
+000068e0: 0d0a 2020 2020 2020 2020 312e 2033 2e31  ..        1. 3.1
+000068f0: 312e 390d 0a20 2020 2020 2020 2032 2e20  1.9..        2. 
+00006900: 332e 3130 2e31 340d 0a20 2020 2020 2020  3.10.14..       
+00006910: 2033 2e20 332e 392e 3139 0d0a 2020 2020   3. 3.9.19..    
+00006920: 2020 2020 342e 2033 2e38 2e31 390d 0a0d      4. 3.8.19...
+00006930: 0a20 2020 2020 2020 2046 696c 7420 7769  .        Filt wi
+00006940: 7468 206b 6579 776f 7264 3a20 2233 2e31  th keyword: "3.1
+00006950: 322e 3322 2e20 3430 203d 3e20 380d 0a0d  2.3". 40 => 8...
+00006960: 0a20 2020 2020 2020 205b 385d 2045 6e74  .        [8] Ent
+00006970: 6572 206b 6579 776f 7264 7320 2863 616e  er keywords (can
+00006980: 2062 6520 696e 7420 696e 6465 7820 6f72   be int index or
+00006990: 2070 6172 7469 616c 206d 6174 6368 2c20   partial match, 
+000069a0: 6465 6661 756c 7473 2074 6f20 3029 3a0d  defaults to 0):.
+000069b0: 0a20 2020 2020 2020 2030 2e20 7838 365f  .        0. x86_
+000069c0: 3634 0d0a 2020 2020 2020 2020 312e 2069  64..        1. i
+000069d0: 3638 360d 0a0d 0a20 2020 2020 2020 2046  686....        F
+000069e0: 696c 7420 7769 7468 206b 6579 776f 7264  ilt with keyword
+000069f0: 3a20 2278 3836 5f36 3422 2e20 3820 3d3e  : "x86_64". 8 =>
+00006a00: 2034 0d0a 0d0a 2020 2020 2020 2020 5b34   4....        [4
+00006a10: 5d20 456e 7465 7220 6b65 7977 6f72 6473  ] Enter keywords
+00006a20: 2028 6361 6e20 6265 2069 6e74 2069 6e64   (can be int ind
+00006a30: 6578 206f 7220 7061 7274 6961 6c20 6d61  ex or partial ma
+00006a40: 7463 682c 2064 6566 6175 6c74 7320 746f  tch, defaults to
+00006a50: 2030 293a 0d0a 2020 2020 2020 2020 302e   0):..        0.
+00006a60: 2073 6861 7265 642d 7067 6f2d 6675 6c6c   shared-pgo-full
+00006a70: 2e74 6172 2e7a 7374 0d0a 2020 2020 2020  .tar.zst..      
+00006a80: 2020 312e 2073 6861 7265 642d 696e 7374    1. shared-inst
+00006a90: 616c 6c5f 6f6e 6c79 2e74 6172 2e67 7a0d  all_only.tar.gz.
+00006aa0: 0a20 2020 2020 2020 2032 2e20 7067 6f2d  .        2. pgo-
+00006ab0: 6675 6c6c 2e74 6172 2e7a 7374 0d0a 2020  full.tar.zst..  
+00006ac0: 2020 2020 2020 332e 2069 6e73 7461 6c6c        3. install
+00006ad0: 5f6f 6e6c 792e 7461 722e 677a 0d0a 0d0a  _only.tar.gz....
+00006ae0: 2020 2020 2020 2020 4669 6c74 2077 6974          Filt wit
+00006af0: 6820 6b65 7977 6f72 643a 2022 7368 6172  h keyword: "shar
+00006b00: 6564 2d70 676f 2d66 756c 6c2e 7461 722e  ed-pgo-full.tar.
+00006b10: 7a73 7422 2e20 3420 3d3e 2031 0d0a 2020  zst". 4 => 1..  
+00006b20: 2020 2020 2020 446f 776e 6c6f 6164 2055        Download U
+00006b30: 524c 3a20 3430 2e34 204d 420d 0a20 2020  RL: 40.4 MB..   
+00006b40: 2020 2020 2068 7474 7073 3a2f 2f67 6974       https://git
+00006b50: 6875 622e 636f 6d2f 696e 6479 6772 6567  hub.com/indygreg
+00006b60: 2f70 7974 686f 6e2d 6275 696c 642d 7374  /python-build-st
+00006b70: 616e 6461 6c6f 6e65 2f72 656c 6561 7365  andalone/release
+00006b80: 732f 646f 776e 6c6f 6164 2f32 3032 3430  s/download/20240
+00006b90: 3431 352f 6370 7974 686f 6e2d 332e 3132  415/cpython-3.12
+00006ba0: 2e33 2532 4232 3032 3430 3431 352d 7838  .3%2B20240415-x8
+00006bb0: 365f 3634 2d70 632d 7769 6e64 6f77 732d  6_64-pc-windows-
+00006bc0: 6d73 7663 2d73 6861 7265 642d 7067 6f2d  msvc-shared-pgo-
+00006bd0: 6675 6c6c 2e74 6172 2e7a 7374 0d0a 2020  full.tar.zst..  
+00006be0: 2020 2020 2020 4669 6c65 2070 6174 6820        File path 
+00006bf0: 746f 2073 6176 6528 6465 6661 756c 7473  to save(defaults
+00006c00: 2074 6f20 602e 2f63 7079 7468 6f6e 2d33   to `./cpython-3
+00006c10: 2e31 322e 332b 3230 3234 3034 3135 2d78  .12.3+20240415-x
+00006c20: 3836 5f36 342d 7063 2d77 696e 646f 7773  86_64-pc-windows
+00006c30: 2d6d 7376 632d 7368 6172 6564 2d70 676f  -msvc-shared-pgo
+00006c40: 2d66 756c 6c2e 7461 722e 7a73 7460 293f  -full.tar.zst`)?
+00006c50: 0d0a 2020 2020 2020 2020 6f72 2060 7160  ..        or `q`
+00006c60: 2074 6f20 6578 6974 2e0d 0a0d 0a20 2020   to exit.....   
+00006c70: 2020 2020 2053 7461 7274 2064 6f77 6e6c       Start downl
+00006c80: 6f61 6469 6e67 2e2e 2e0d 0a20 2020 2020  oading.....     
+00006c90: 2020 2068 7474 7073 3a2f 2f67 6974 6875     https://githu
+00006ca0: 622e 636f 6d2f 696e 6479 6772 6567 2f70  b.com/indygreg/p
+00006cb0: 7974 686f 6e2d 6275 696c 642d 7374 616e  ython-build-stan
+00006cc0: 6461 6c6f 6e65 2f72 656c 6561 7365 732f  dalone/releases/
+00006cd0: 646f 776e 6c6f 6164 2f32 3032 3430 3431  download/2024041
+00006ce0: 352f 6370 7974 686f 6e2d 332e 3132 2e33  5/cpython-3.12.3
+00006cf0: 2532 4232 3032 3430 3431 352d 7838 365f  %2B20240415-x86_
+00006d00: 3634 2d70 632d 7769 6e64 6f77 732d 6d73  64-pc-windows-ms
+00006d10: 7663 2d73 6861 7265 642d 7067 6f2d 6675  vc-shared-pgo-fu
+00006d20: 6c6c 2e74 6172 2e7a 7374 0d0a 2020 2020  ll.tar.zst..    
+00006d30: 2020 2020 443a 5c67 6974 6875 625c 6d6f      D:\github\mo
+00006d40: 7265 6275 696c 7469 6e73 5c63 7079 7468  rebuiltins\cpyth
+00006d50: 6f6e 2d33 2e31 322e 332b 3230 3234 3034  on-3.12.3+202404
+00006d60: 3135 2d78 3836 5f36 342d 7063 2d77 696e  15-x86_64-pc-win
+00006d70: 646f 7773 2d6d 7376 632d 7368 6172 6564  dows-msvc-shared
+00006d80: 2d70 676f 2d66 756c 6c2e 7461 722e 7a73  -pgo-full.tar.zs
+00006d90: 740d 0a20 2020 2020 2020 205b 446f 776e  t..        [Down
+00006da0: 6c6f 6164 696e 675d 3a20 322e 3231 202f  loading]: 2.21 /
+00006db0: 2034 302e 3434 204d 4220 7c20 352e 3437   40.44 MB | 5.47
+00006dc0: 250d 0a0d 0a2d 2d2d 0d0a 0d0a            %....---....
```

### Comparing `morebuiltins-0.0.3/morebuiltins/ipc.py` & `morebuiltins-0.0.4/morebuiltins/ipc.py`

 * *Files identical despite different names*

### Comparing `morebuiltins-0.0.3/morebuiltins/request.py` & `morebuiltins-0.0.4/morebuiltins/request.py`

 * *Files identical despite different names*

### Comparing `morebuiltins-0.0.3/morebuiltins/utils.py` & `morebuiltins-0.0.4/morebuiltins/utils.py`

 * *Files identical despite different names*

### Comparing `morebuiltins-0.0.3/morebuiltins/zipapps/__main__.py` & `morebuiltins-0.0.4/morebuiltins/zipapps/__main__.py`

 * *Files identical despite different names*

### Comparing `morebuiltins-0.0.3/morebuiltins/zipapps/activate_zipapps.py` & `morebuiltins-0.0.4/morebuiltins/zipapps/activate_zipapps.py`

 * *Files identical despite different names*

### Comparing `morebuiltins-0.0.3/morebuiltins/zipapps/ensure_zipapps.py.template` & `morebuiltins-0.0.4/morebuiltins/zipapps/ensure_zipapps.py.template`

 * *Files identical despite different names*

### Comparing `morebuiltins-0.0.3/morebuiltins/zipapps/entry_point.py.template` & `morebuiltins-0.0.4/morebuiltins/zipapps/entry_point.py.template`

 * *Files identical despite different names*

### Comparing `morebuiltins-0.0.3/morebuiltins/zipapps/freezing.py` & `morebuiltins-0.0.4/morebuiltins/zipapps/freezing.py`

 * *Files identical despite different names*

### Comparing `morebuiltins-0.0.3/morebuiltins/zipapps/main.py` & `morebuiltins-0.0.4/morebuiltins/zipapps/main.py`

 * *Files identical despite different names*

### Comparing `morebuiltins-0.0.3/PKG-INFO` & `morebuiltins-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morebuiltins
-Version: 0.0.3
+Version: 0.0.4
 Summary: Things which I thought should be set in builtins.
 Author-email: ClericPy <clericpy@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/ClericPy/morebuiltins
 
@@ -92,14 +92,18 @@
 
 2.1 `lru_cache_ttl` - A Least Recently Used (LRU) cache with a Time To Live (TTL) feature.
 
 2.2 `threads` - Quickly convert synchronous functions to be concurrency-able. (similar to madisonmay/Tomorrow)
 
 2.3 `bg_task` - Avoid asyncio free-flying tasks, better to use the new asyncio.TaskGroup to avoid this in 3.11+. https://github.com/python/cpython/issues/91887
 
+2.4 `NamedLock` - Reusable named locks, support for timeouts, support for multiple concurrent locks.
+
+2.5 `FuncSchema` - Parse the parameters and types required by a function into a dictionary, and convert an incoming parameter into the appropriate type.
+
 
 ## 3. morebuiltins.ipc
 
 3.1 `IPCEncoder` - An abstract base class for all encoders; implementing the necessary communication protocol requires only the definition of two abstract methods. Be mindful that varying header lengths will impact the maximum packaging size.
 
 3.4 `SocketLogHandlerEncoder` - For a practical demonstration, refer to the test code: morebuiltins/ipc.py:_test_ipc_logging.
 
@@ -113,22 +117,29 @@
 4.2 `DomainParser` - Extracts the Second-level domain (SLD) from a provided hostname or URL.
 
 4.3 `unparse_qsl` - Provides the inverse operation of parse_qsl, converting query string lists back into a URL-encoded string.
 
 4.4 `update_url` - Organizes the query arguments within a URL to standardize its format.
 
 
+## 5. morebuiltins.download_python
+
+5.1 `download_python` - Usage: python -m morebuiltins.download_python
+
+
 <!-- end -->
 
 ## On the way
 
 - [x] add zipapps as a submodule(https://github.com/ClericPy/zipapps) - v0.0.3
 - [x] asyncio free-flying tasks(bg_task) - v0.0.3
+- [x] named lock with timeout - v0.0.4
+- [x] functools.FuncSchema (parse function to get the query-dict) - v0.0.4
+- [x] morebuiltins.download_python [standalone python](https://github.com/indygreg/python-build-standalone/releases/latest) downloader - v0.0.4
+- [ ] pip.pip_install
 - [ ] progress_bar
 - [ ] http.server (upload)
-- [ ] function parser (signature.parameters)
 - [ ] time reach syntax
 - [ ] quick tkinter
 - [ ] http request/response parser
-- [ ] named lock with timeout
 - [ ] TimeSizeRotatingHandler of logging.handlers
```

