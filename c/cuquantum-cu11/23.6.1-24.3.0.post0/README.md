# Comparing `tmp/cuquantum_cu11-23.6.1-py3-none-manylinux2014_x86_64.whl.zip` & `tmp/cuquantum_cu11-24.3.0.post0-py3-none-manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,162 +1,237 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                      7003 (0000000000001B5Bh)
-  Actual end-cent-dir record offset:          6981 (0000000000001B45h)
-  Expected end-cent-dir record offset:        6981 (0000000000001B45h)
+  Zip archive file size:                      7527 (0000000000001D67h)
+  Actual end-cent-dir record offset:          7505 (0000000000001D51h)
+  Expected end-cent-dir record offset:        7505 (0000000000001D51h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 5 entries.
-  The central directory is 429 (00000000000001ADh) bytes long,
+  central directory contains 6 entries.
+  The central directory is 687 (00000000000002AFh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 6552 (0000000000001998h).
+  is 6818 (0000000000001AA2h).
 
 
 Central directory entry #1:
 ---------------------------
 
-  cuquantum_cu11-23.6.1.dist-info/LICENSE
+  cuquantum_cu11-24.3.0.post0.dist-info/
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 May 9 14:51:22
+  file last modified on (UT extra field modtime): 2024 May 9 20:51:21 local
+  file last modified on (UT extra field modtime): 2024 May 9 20:51:21 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             38 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #2:
+---------------------------
+
+  cuquantum_cu11-24.3.0.post0.dist-info/LICENSE
+
+  offset of local header from start of archive:   96
+                                                  (0000000000000060h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 20 16:40:58
+  file last modified on (DOS date/time):          2024 May 7 20:33:42
+  file last modified on (UT extra field modtime): 2024 May 8 02:33:42 local
+  file last modified on (UT extra field modtime): 2024 May 8 02:33:42 UTC
   32-bit CRC value (hex):                         9bd5338b
   compressed size:                                4716 bytes
   uncompressed size:                              11004 bytes
-  length of filename:                             39 characters
-  length of extra field:                          0 bytes
+  length of filename:                             45 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
   There is no file comment.
 
-Central directory entry #2:
+Central directory entry #3:
 ---------------------------
 
-  cuquantum_cu11-23.6.1.dist-info/METADATA
+  cuquantum_cu11-24.3.0.post0.dist-info/top_level.txt
 
-  offset of local header from start of archive:   4785
-                                                  (00000000000012B1h) bytes
+  offset of local header from start of archive:   4915
+                                                  (0000000000001333h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 20 16:40:58
-  32-bit CRC value (hex):                         244d2ba3
-  compressed size:                                1118 bytes
-  uncompressed size:                              2678 bytes
-  length of filename:                             40 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 May 7 20:33:42
+  file last modified on (UT extra field modtime): 2024 May 8 02:33:42 local
+  file last modified on (UT extra field modtime): 2024 May 8 02:33:42 UTC
+  32-bit CRC value (hex):                         32d70693
+  compressed size:                                1 bytes
+  uncompressed size:                              1 bytes
+  length of filename:                             51 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
   There is no file comment.
 
-Central directory entry #3:
+Central directory entry #4:
 ---------------------------
 
-  cuquantum_cu11-23.6.1.dist-info/WHEEL
+  cuquantum_cu11-24.3.0.post0.dist-info/WHEEL
 
-  offset of local header from start of archive:   5973
-                                                  (0000000000001755h) bytes
+  offset of local header from start of archive:   5025
+                                                  (00000000000013A1h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 20 16:40:58
-  32-bit CRC value (hex):                         cecc00c9
-  compressed size:                                107 bytes
+  file last modified on (DOS date/time):          2024 May 7 20:33:42
+  file last modified on (UT extra field modtime): 2024 May 8 02:33:42 local
+  file last modified on (UT extra field modtime): 2024 May 8 02:33:42 UTC
+  32-bit CRC value (hex):                         3f19bfad
+  compressed size:                                108 bytes
   uncompressed size:                              109 bytes
-  length of filename:                             37 characters
-  length of extra field:                          0 bytes
+  length of filename:                             43 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
   There is no file comment.
 
-Central directory entry #4:
+Central directory entry #5:
 ---------------------------
 
-  cuquantum_cu11-23.6.1.dist-info/top_level.txt
+  cuquantum_cu11-24.3.0.post0.dist-info/RECORD
 
-  offset of local header from start of archive:   6147
-                                                  (0000000000001803h) bytes
+  offset of local header from start of archive:   5234
+                                                  (0000000000001472h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 20 16:40:58
-  32-bit CRC value (hex):                         32d70693
-  compressed size:                                3 bytes
-  uncompressed size:                              1 bytes
-  length of filename:                             45 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 May 9 14:51:22
+  file last modified on (UT extra field modtime): 2024 May 9 20:51:21 local
+  file last modified on (UT extra field modtime): 2024 May 9 20:51:21 UTC
+  32-bit CRC value (hex):                         707b418d
+  compressed size:                                257 bytes
+  uncompressed size:                              427 bytes
+  length of filename:                             44 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             text
+  Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
   There is no file comment.
 
-Central directory entry #5:
+Central directory entry #6:
 ---------------------------
 
-  cuquantum_cu11-23.6.1.dist-info/RECORD
+  cuquantum_cu11-24.3.0.post0.dist-info/METADATA
 
-  offset of local header from start of archive:   6225
-                                                  (0000000000001851h) bytes
+  offset of local header from start of archive:   5593
+                                                  (00000000000015D9h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 20 16:40:58
-  32-bit CRC value (hex):                         f3c52561
-  compressed size:                                259 bytes
-  uncompressed size:                              427 bytes
-  length of filename:                             38 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 May 9 14:06:12
+  file last modified on (UT extra field modtime): 2024 May 9 20:06:11 local
+  file last modified on (UT extra field modtime): 2024 May 9 20:06:11 UTC
+  32-bit CRC value (hex):                         08abd8a4
+  compressed size:                                1121 bytes
+  uncompressed size:                              2680 bytes
+  length of filename:                             46 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
-Filename: cuquantum_cu11-23.6.1.dist-info/LICENSE
+Filename: cuquantum_cu11-24.3.0.post0.dist-info/
 Comment: 
 
-Filename: cuquantum_cu11-23.6.1.dist-info/METADATA
+Filename: cuquantum_cu11-24.3.0.post0.dist-info/LICENSE
 Comment: 
 
-Filename: cuquantum_cu11-23.6.1.dist-info/WHEEL
+Filename: cuquantum_cu11-24.3.0.post0.dist-info/top_level.txt
 Comment: 
 
-Filename: cuquantum_cu11-23.6.1.dist-info/top_level.txt
+Filename: cuquantum_cu11-24.3.0.post0.dist-info/WHEEL
 Comment: 
 
-Filename: cuquantum_cu11-23.6.1.dist-info/RECORD
+Filename: cuquantum_cu11-24.3.0.post0.dist-info/RECORD
+Comment: 
+
+Filename: cuquantum_cu11-24.3.0.post0.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## Comparing `cuquantum_cu11-23.6.1.dist-info/LICENSE` & `cuquantum_cu11-24.3.0.post0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cuquantum_cu11-23.6.1.dist-info/METADATA` & `cuquantum_cu11-24.3.0.post0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: cuquantum-cu11
-Version: 23.6.1
+Version: 24.3.0.post0
 Summary: NVIDIA cuQuantum SDK
 Home-page: https://developer.nvidia.com/cuquantum-sdk
 Author: NVIDIA Corporation
 Author-email: cuda_installer@nvidia.com
 License: NVIDIA Proprietary Software
 Project-URL: Bug Tracker, https://github.com/NVIDIA/cuQuantum/issues
 Project-URL: User Forum, https://github.com/NVIDIA/cuQuantum/discussions
 Project-URL: Documentation, https://docs.nvidia.com/cuda/cuquantum/
 Keywords: cuda,nvidia,state vector,tensor network,high-performance computing,quantum computing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: custatevec-cu11 (==1.4.1)
-Requires-Dist: cutensornet-cu11 (==2.2.1)
+Requires-Dist: custatevec-cu11 ==1.6.0
+Requires-Dist: cutensornet-cu11 ==2.4.0
 
 **************************************************************************************
 cuQuantum SDK: A High-Performance Library for Accelerating Quantum Information Science
 **************************************************************************************
 
 `NVIDIA cuQuantum SDK <https://developer.nvidia.com/cuquantum-sdk>`_ is a high-performance library for quantum information science and beyond.
 Currently its primary target is *quantum circuit simulations* and it consists of two major components:
```

