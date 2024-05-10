# Comparing `tmp/frappe_manager-0.8.3.tar.gz` & `tmp/frappe_manager-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frappe_manager-0.8.3.tar", max compression
+gzip compressed data, was "frappe_manager-0.9.0.tar", max compression
```

## Comparing `frappe_manager-0.8.3.tar` & `frappe_manager-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,31 @@
--rw-r--r--   0        0        0     1063 2023-11-03 09:02:41.111245 frappe_manager-0.8.3/LICENSE
--rw-r--r--   0        0        0     1352 2023-11-03 09:02:41.111245 frappe_manager-0.8.3/README.md
--rw-r--r--   0        0        0        0 2023-11-03 09:02:41.111245 frappe_manager-0.8.3/frappe_manager/__init__.py
--rw-r--r--   0        0        0     1741 2023-11-03 09:02:41.111245 frappe_manager-0.8.3/frappe_manager/docker_wrapper/DockerClient.py
--rw-r--r--   0        0        0    27699 2023-11-03 09:02:41.111245 frappe_manager-0.8.3/frappe_manager/docker_wrapper/DockerCompose.py
--rw-r--r--   0        0        0     1688 2023-11-03 09:02:41.111245 frappe_manager-0.8.3/frappe_manager/docker_wrapper/DockerException.py
--rw-r--r--   0        0        0       84 2023-11-03 09:02:41.111245 frappe_manager-0.8.3/frappe_manager/docker_wrapper/__init__.py
--rw-r--r--   0        0        0     3576 2023-11-03 09:02:41.111245 frappe_manager-0.8.3/frappe_manager/docker_wrapper/utils.py
--rw-r--r--   0        0        0     9052 2023-11-09 13:51:05.185046 frappe_manager-0.8.3/frappe_manager/main.py
--rw-r--r--   0        0        0    10600 2023-11-03 09:02:41.114579 frappe_manager-0.8.3/frappe_manager/site_manager/Richprint.py
--rw-r--r--   0        0        0    10100 2023-11-03 09:02:41.114579 frappe_manager-0.8.3/frappe_manager/site_manager/SiteCompose.py
--rw-r--r--   0        0        0        0 2023-11-03 09:02:41.114579 frappe_manager-0.8.3/frappe_manager/site_manager/__init__.py
--rw-r--r--   0        0        0    19008 2023-11-03 09:02:41.114579 frappe_manager-0.8.3/frappe_manager/site_manager/manager.py
--rw-r--r--   0        0        0    13468 2023-11-03 09:02:41.114579 frappe_manager-0.8.3/frappe_manager/site_manager/site.py
--rw-r--r--   0        0        0     1515 2023-11-03 09:02:41.114579 frappe_manager-0.8.3/frappe_manager/site_manager/templates/docker-compose.tmpl
--rw-r--r--   0        0        0      714 2023-11-10 10:21:20.582642 frappe_manager-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 frappe_manager-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-11-28 09:55:55.759894 frappe_manager-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1110 2023-11-28 09:55:55.759894 frappe_manager-0.9.0/README.md
+-rw-r--r--   0        0        0       59 2023-12-04 08:32:30.620394 frappe_manager-0.9.0/frappe_manager/__init__.py
+-rw-r--r--   0        0        0     1741 2023-11-28 09:55:55.759894 frappe_manager-0.9.0/frappe_manager/docker_wrapper/DockerClient.py
+-rw-r--r--   0        0        0    27628 2023-12-04 08:32:30.620394 frappe_manager-0.9.0/frappe_manager/docker_wrapper/DockerCompose.py
+-rw-r--r--   0        0        0     1688 2023-11-28 09:55:55.759894 frappe_manager-0.9.0/frappe_manager/docker_wrapper/DockerException.py
+-rw-r--r--   0        0        0       84 2023-11-28 09:55:55.759894 frappe_manager-0.9.0/frappe_manager/docker_wrapper/__init__.py
+-rw-r--r--   0        0        0     2827 2023-11-29 10:47:56.411374 frappe_manager-0.9.0/frappe_manager/docker_wrapper/__pycache__/DockerClient.cpython-311.pyc
+-rw-r--r--   0        0        0    28107 2023-12-04 08:48:43.816304 frappe_manager-0.9.0/frappe_manager/docker_wrapper/__pycache__/DockerCompose.cpython-311.pyc
+-rw-r--r--   0        0        0     2954 2023-11-29 10:47:56.441373 frappe_manager-0.9.0/frappe_manager/docker_wrapper/__pycache__/DockerException.cpython-311.pyc
+-rw-r--r--   0        0        0      329 2023-11-29 10:47:56.408041 frappe_manager-0.9.0/frappe_manager/docker_wrapper/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7010 2023-12-04 08:48:43.819637 frappe_manager-0.9.0/frappe_manager/docker_wrapper/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     3808 2023-12-04 08:32:30.620394 frappe_manager-0.9.0/frappe_manager/docker_wrapper/utils.py
+-rw-r--r--   0        0        0       18 2023-12-04 08:32:30.623727 frappe_manager-0.9.0/frappe_manager/logger/__init__.py
+-rw-r--r--   0        0        0      260 2023-12-04 08:48:43.826304 frappe_manager-0.9.0/frappe_manager/logger/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2767 2023-12-04 08:48:43.826304 frappe_manager-0.9.0/frappe_manager/logger/__pycache__/log.cpython-311.pyc
+-rw-r--r--   0        0        0     1473 2023-12-04 08:32:30.623727 frappe_manager-0.9.0/frappe_manager/logger/log.py
+-rw-r--r--   0        0        0    11633 2023-12-04 08:32:30.623727 frappe_manager-0.9.0/frappe_manager/main.py
+-rw-r--r--   0        0        0    10600 2023-11-30 14:00:02.002822 frappe_manager-0.9.0/frappe_manager/site_manager/Richprint.py
+-rw-r--r--   0        0        0    10100 2023-12-04 09:02:40.646119 frappe_manager-0.9.0/frappe_manager/site_manager/SiteCompose.py
+-rw-r--r--   0        0        0        0 2023-11-28 09:55:55.759894 frappe_manager-0.9.0/frappe_manager/site_manager/__init__.py
+-rw-r--r--   0        0        0    14159 2023-11-30 14:15:05.370910 frappe_manager-0.9.0/frappe_manager/site_manager/__pycache__/Richprint.cpython-311.pyc
+-rw-r--r--   0        0        0    14760 2023-12-04 09:08:18.413885 frappe_manager-0.9.0/frappe_manager/site_manager/__pycache__/SiteCompose.cpython-311.pyc
+-rw-r--r--   0        0        0      224 2023-11-29 10:47:56.404708 frappe_manager-0.9.0/frappe_manager/site_manager/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    24514 2023-12-04 08:48:43.816304 frappe_manager-0.9.0/frappe_manager/site_manager/__pycache__/manager.cpython-311.pyc
+-rw-r--r--   0        0        0    19765 2023-12-04 08:48:43.836303 frappe_manager-0.9.0/frappe_manager/site_manager/__pycache__/site.cpython-311.pyc
+-rw-r--r--   0        0        0    17881 2023-12-04 08:32:30.623727 frappe_manager-0.9.0/frappe_manager/site_manager/manager.py
+-rw-r--r--   0        0        0    13450 2023-12-04 08:32:30.627061 frappe_manager-0.9.0/frappe_manager/site_manager/site.py
+-rw-r--r--   0        0        0     1515 2023-12-04 10:18:25.027090 frappe_manager-0.9.0/frappe_manager/site_manager/templates/docker-compose.tmpl
+-rw-r--r--   0        0        0      857 2023-12-04 10:17:58.097762 frappe_manager-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 frappe_manager-0.9.0/PKG-INFO
```

### Comparing `frappe_manager-0.8.3/LICENSE` & `frappe_manager-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frappe_manager-0.8.3/README.md` & `frappe_manager-0.9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -8,78 +8,63 @@
 00000070: 7461 626c 6520 666f 7220 6465 7665 6c6f  table for develo
 00000080: 706d 656e 7420 696e 206c 6f63 616c 206d  pment in local m
 00000090: 6163 6869 6e65 7320 7275 6e6e 696e 6720  achines running 
 000000a0: 6f6e 204d 6163 2061 6e64 204c 696e 7578  on Mac and Linux
 000000b0: 2062 6173 6564 204f 532e 0a0a 0a21 5b46   based OS....![F
 000000c0: 7261 7070 652d 4d61 6e61 6765 722d 4372  rappe-Manager-Cr
 000000d0: 6561 7465 2d53 6974 652e 7376 675d 2868  eate-Site.svg](h
-000000e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000000f0: 6d2f 7274 4361 6d70 2f46 7261 7070 652d  m/rtCamp/Frappe-
-00000100: 4d61 6e61 6765 722f 6173 7365 7473 2f32  Manager/assets/2
-00000110: 3632 3430 3738 302f 3738 3434 3138 6635  6240780/784418f5
-00000120: 2d37 3433 382d 3466 3231 2d61 6238 342d  -7438-4f21-ab84-
-00000130: 6432 6365 3434 6237 6438 6332 290a 0a0a  d2ce44b7d8c2)...
-00000140: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
-00000150: 2a2a 5265 7175 6972 656d 656e 7473 3a2a  **Requirements:*
-00000160: 2a20 5079 7468 6f6e 332e 3131 2b2c 2044  * Python3.11+, D
-00000170: 6f63 6b65 722c 2056 5343 6f64 6528 6f70  ocker, VSCode(op
-00000180: 7469 6f6e 616c 290a 0a60 6060 6261 7368  tional)..```bash
-00000190: 0a70 6970 2069 6e73 7461 6c6c 2066 7261  .pip install fra
-000001a0: 7070 652d 6d61 6e61 6765 720a 6060 600a  ppe-manager.```.
-000001b0: 0a23 2323 2053 6574 7570 2041 7574 6f63  .### Setup Autoc
-000001c0: 6f6d 706c 6574 696f 6e20 2020 200a 312e  ompletion    .1.
-000001d0: 2060 6060 6261 7368 0a20 2020 666d 202d   ```bash.   fm -
-000001e0: 2d69 6e73 7461 6c6c 2d63 6f6d 706c 6574  -install-complet
-000001f0: 696f 6e0a 2020 2060 6060 0a32 2e20 5265  ion.   ```.2. Re
-00000200: 7374 6172 7420 7368 656c 6c20 6f72 2074  start shell or t
-00000210: 6572 6d69 6e61 6c0a 0a0a 2323 2055 7361  erminal...## Usa
-00000220: 6765 0a23 2323 2043 7265 6174 6520 6120  ge.### Create a 
-00000230: 7369 7465 0a0a 6060 6062 6173 680a 2320  site..```bash.# 
-00000240: 6372 6561 7465 2065 7861 6d70 6c65 2e6c  create example.l
-00000250: 6f63 616c 686f 7374 2073 6974 6520 7769  ocalhost site wi
-00000260: 7468 206f 6e6c 7920 6672 6170 7065 2c20  th only frappe, 
-00000270: 7665 7273 696f 6e20 2d3e 2076 6572 7369  version -> versi
-00000280: 6f6e 2d31 350a 666d 2063 7265 6174 6520  on-15.fm create 
-00000290: 6578 616d 706c 650a 0a23 2063 7265 6174  example..# creat
-000002a0: 6520 6578 616d 706c 652e 6c6f 6361 6c68  e example.localh
-000002b0: 6f73 7420 7369 7465 2077 6974 6820 6f6e  ost site with on
-000002c0: 6c79 2066 7261 7070 652c 2076 6572 7369  ly frappe, versi
-000002d0: 6f6e 202d 3e20 6465 7665 6c6f 700a 666d  on -> develop.fm
-000002e0: 2063 7265 6174 6520 6578 616d 706c 6520   create example 
-000002f0: 2d2d 6672 6170 7065 2d62 7261 6e63 6820  --frappe-branch 
-00000300: 6465 7665 6c6f 700a 0a23 2063 7265 6174  develop..# creat
-00000310: 6520 6578 616d 706c 652e 6c6f 6361 6c68  e example.localh
-00000320: 6f73 7420 7369 7465 2077 6974 6820 6672  ost site with fr
-00000330: 6170 7065 2c20 6572 706e 6578 7420 616e  appe, erpnext an
-00000340: 6420 6872 6d73 2c20 7665 7273 696f 6e20  d hrms, version 
-00000350: 2d3e 2076 6572 7369 6f6e 2d31 350a 666d  -> version-15.fm
-00000360: 2063 7265 6174 6520 6578 616d 706c 6520   create example 
-00000370: 2d2d 6170 7073 2065 7270 6e65 7874 3a76  --apps erpnext:v
-00000380: 6572 7369 6f6e 2d31 3520 2d2d 6170 7073  ersion-15 --apps
-00000390: 2068 726d 733a 7665 7273 696f 6e2d 3135   hrms:version-15
-000003a0: 2020 2020 0a60 6060 0a0a 5669 7369 7420      .```..Visit 
-000003b0: 434c 4920 5b57 696b 695d 2868 7474 7073  CLI [Wiki](https
-000003c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7274  ://github.com/rt
-000003d0: 4361 6d70 2f46 7261 7070 652d 4d61 6e61  Camp/Frappe-Mana
-000003e0: 6765 722f 7769 6b69 2920 666f 7220 6d6f  ger/wiki) for mo
-000003f0: 7265 2065 7861 6d70 6c65 730a 0a23 2320  re examples..## 
-00000400: 4372 6564 6974 730a 446f 636b 6572 6669  Credits.Dockerfi
-00000410: 6c65 733a 205b 4672 6170 7065 2044 6f63  les: [Frappe Doc
-00000420: 6b65 725d 2868 7474 7073 3a2f 2f67 6974  ker](https://git
-00000430: 6875 622e 636f 6d2f 6672 6170 7065 2f66  hub.com/frappe/f
-00000440: 7261 7070 655f 646f 636b 6572 290a 0a23  rappe_docker)..#
-00000450: 2320 446f 6573 2074 6869 7320 696e 7465  # Does this inte
-00000460: 7265 7374 2079 6f75 3f0a 0a3c 6120 6872  rest you?..<a hr
-00000470: 6566 3d22 6874 7470 733a 2f2f 7274 6361  ef="https://rtca
-00000480: 6d70 2e63 6f6d 2f22 3e3c 696d 6720 7372  mp.com/"><img sr
-00000490: 633d 2268 7474 7073 3a2f 2f72 7463 616d  c="https://rtcam
-000004a0: 702e 636f 6d2f 7770 2d63 6f6e 7465 6e74  p.com/wp-content
-000004b0: 2f75 706c 6f61 6473 2f73 6974 6573 2f32  /uploads/sites/2
-000004c0: 2f32 3031 392f 3034 2f67 6974 6875 622d  /2019/04/github-
-000004d0: 6261 6e6e 6572 4032 782e 706e 6722 2061  banner@2x.png" a
-000004e0: 6c74 3d22 4a6f 696e 2075 7320 6174 2072  lt="Join us at r
-000004f0: 7443 616d 702c 2077 6520 7370 6563 6961  tCamp, we specia
-00000500: 6c69 7a65 2069 6e20 7072 6f76 6964 696e  lize in providin
-00000510: 6720 6869 6768 2070 6572 666f 726d 616e  g high performan
-00000520: 6365 2065 6e74 6572 7072 6973 6520 576f  ce enterprise Wo
-00000530: 7264 5072 6573 7320 736f 6c75 7469 6f6e  rdPress solution
-00000540: 7322 3e3c 2f61 3e0a                      s"></a>.
+000000e0: 7474 7073 3a2f 2f75 7365 722d 696d 6167  ttps://user-imag
+000000f0: 6573 2e67 6974 6875 6275 7365 7263 6f6e  es.githubusercon
+00000100: 7465 6e74 2e63 6f6d 2f32 3832 3934 3739  tent.com/2829479
+00000110: 352f 3238 3331 3038 3739 312d 3032 3337  5/283108791-0237
+00000120: 6430 3561 2d32 3536 322d 3438 6265 2d39  d05a-2562-48be-9
+00000130: 3837 622d 3033 3761 3230 3064 3731 6133  87b-037a200d71a3
+00000140: 2e73 7667 290a 0a0a 2323 2049 6e73 7461  .svg)...## Insta
+00000150: 6c6c 6174 696f 6e0a 2a2a 5265 7175 6972  llation.**Requir
+00000160: 656d 656e 7473 3a2a 2a20 5079 7468 6f6e  ements:** Python
+00000170: 332e 3131 2b2c 2044 6f63 6b65 722c 2056  3.11+, Docker, V
+00000180: 5343 6f64 6528 6f70 7469 6f6e 616c 290a  SCode(optional).
+00000190: 0a60 6060 6261 7368 0a70 6970 2069 6e73  .```bash.pip ins
+000001a0: 7461 6c6c 2066 7261 7070 652d 6d61 6e61  tall frappe-mana
+000001b0: 6765 720a 6060 600a 0a23 2323 2053 6574  ger.```..### Set
+000001c0: 7570 2041 7574 6f63 6f6d 706c 6574 696f  up Autocompletio
+000001d0: 6e20 2020 200a 312e 2060 6060 6261 7368  n    .1. ```bash
+000001e0: 0a20 2020 666d 202d 2d69 6e73 7461 6c6c  .   fm --install
+000001f0: 2d63 6f6d 706c 6574 696f 6e0a 2020 2060  -completion.   `
+00000200: 6060 0a32 2e20 5265 7374 6172 7420 7368  ``.2. Restart sh
+00000210: 656c 6c20 6f72 2074 6572 6d69 6e61 6c0a  ell or terminal.
+00000220: 0a0a 2323 2055 7361 6765 0a23 2323 2043  ..## Usage.### C
+00000230: 7265 6174 6520 6120 7369 7465 0a0a 6060  reate a site..``
+00000240: 6062 6173 680a 2320 6372 6561 7465 2065  `bash.# create e
+00000250: 7861 6d70 6c65 2e6c 6f63 616c 686f 7374  xample.localhost
+00000260: 2073 6974 6520 7769 7468 206f 6e6c 7920   site with only 
+00000270: 6672 6170 7065 2c20 7665 7273 696f 6e20  frappe, version 
+00000280: 2d3e 2076 6572 7369 6f6e 2d31 350a 666d  -> version-15.fm
+00000290: 2063 7265 6174 6520 6578 616d 706c 650a   create example.
+000002a0: 0a23 2063 7265 6174 6520 6578 616d 706c  .# create exampl
+000002b0: 652e 6c6f 6361 6c68 6f73 7420 7369 7465  e.localhost site
+000002c0: 2077 6974 6820 6f6e 6c79 2066 7261 7070   with only frapp
+000002d0: 652c 2076 6572 7369 6f6e 202d 3e20 6465  e, version -> de
+000002e0: 7665 6c6f 700a 666d 2063 7265 6174 6520  velop.fm create 
+000002f0: 6578 616d 706c 6520 2d2d 6672 6170 7065  example --frappe
+00000300: 2d62 7261 6e63 6820 6465 7665 6c6f 700a  -branch develop.
+00000310: 0a23 2063 7265 6174 6520 6578 616d 706c  .# create exampl
+00000320: 652e 6c6f 6361 6c68 6f73 7420 7369 7465  e.localhost site
+00000330: 2077 6974 6820 6672 6170 7065 2c20 6572   with frappe, er
+00000340: 706e 6578 7420 616e 6420 6872 6d73 2c20  pnext and hrms, 
+00000350: 7665 7273 696f 6e20 2d3e 2076 6572 7369  version -> versi
+00000360: 6f6e 2d31 350a 666d 2063 7265 6174 6520  on-15.fm create 
+00000370: 6578 616d 706c 6520 2d2d 6170 7073 2065  example --apps e
+00000380: 7270 6e65 7874 3a76 6572 7369 6f6e 2d31  rpnext:version-1
+00000390: 3520 2d2d 6170 7073 2068 726d 733a 7665  5 --apps hrms:ve
+000003a0: 7273 696f 6e2d 3135 2020 2020 0a60 6060  rsion-15    .```
+000003b0: 0a0a 5669 7369 7420 434c 4920 5b57 696b  ..Visit CLI [Wik
+000003c0: 695d 2868 7474 7073 3a2f 2f67 6974 6875  i](https://githu
+000003d0: 622e 636f 6d2f 7274 4361 6d70 2f46 7261  b.com/rtCamp/Fra
+000003e0: 7070 652d 4d61 6e61 6765 722f 7769 6b69  ppe-Manager/wiki
+000003f0: 2920 666f 7220 6d6f 7265 2065 7861 6d70  ) for more examp
+00000400: 6c65 730a 0a23 2320 4372 6564 6974 730a  les..## Credits.
+00000410: 446f 636b 6572 6669 6c65 733a 205b 4672  Dockerfiles: [Fr
+00000420: 6170 7065 2044 6f63 6b65 725d 2868 7474  appe Docker](htt
+00000430: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000440: 6672 6170 7065 2f66 7261 7070 655f 646f  frappe/frappe_do
+00000450: 636b 6572 290a                           cker).
```

### Comparing `frappe_manager-0.8.3/frappe_manager/docker_wrapper/DockerClient.py` & `frappe_manager-0.9.0/frappe_manager/docker_wrapper/DockerClient.py`

 * *Files identical despite different names*

### Comparing `frappe_manager-0.8.3/frappe_manager/docker_wrapper/DockerCompose.py` & `frappe_manager-0.9.0/frappe_manager/docker_wrapper/DockerCompose.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from subprocess import Popen, run, TimeoutExpired, CalledProcessError
 from pathlib import Path
-import subprocess
 from typing import Union, Literal
-from rich import print
 
 import shlex
 from frappe_manager.docker_wrapper.utils import (
-    stream_stdout_and_stderr,
     parameters_to_options,
     run_command_with_exit_code,
 )
 
 # Docker Compose version 2.18.1
 class DockerComposeWrapper:
     """
```

### Comparing `frappe_manager-0.8.3/frappe_manager/docker_wrapper/DockerException.py` & `frappe_manager-0.9.0/frappe_manager/docker_wrapper/DockerException.py`

 * *Files identical despite different names*

### Comparing `frappe_manager-0.8.3/frappe_manager/docker_wrapper/utils.py` & `frappe_manager-0.9.0/frappe_manager/docker_wrapper/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,44 +7,45 @@
 from datetime import datetime, timedelta
 from importlib.metadata import version
 from pathlib import Path
 from queue import Queue
 from subprocess import PIPE, Popen, run
 from threading import Thread
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, overload
-
+from frappe_manager.logger import log
 from rich import control
-
 from frappe_manager.docker_wrapper.DockerException import DockerException
 
+logger = log.get_logger()
 
 def reader(pipe, pipe_name, queue):
     try:
         with pipe:
             for line in iter(pipe.readline, b""):
-                # queue.put((pipe_name, line))
-                queue.put((pipe_name, str(line.decode().strip('\n')).encode()))
+                queue_line = line.decode().strip('\n')
+                logger.debug(queue_line)
+                queue.put((pipe_name, str(queue_line).encode()))
     finally:
         queue.put(None)
 
 
 
 def stream_stdout_and_stderr(
     full_cmd: list,
     env: Dict[str, str] = None,
 ) -> Iterable[Tuple[str, bytes]]:
-
+    logger.debug('- -'*10)
+    logger.debug(f"DOCKER COMMAND: {' '.join(full_cmd)}")
     if env is None:
         subprocess_env = None
     else:
         subprocess_env = dict(os.environ)
         subprocess_env.update(env)
 
     full_cmd = list(map(str, full_cmd))
-    #print(full_cmd)
     process = Popen(full_cmd, stdout=PIPE, stderr=PIPE, env=subprocess_env)
     q = Queue()
     full_stderr = b""  # for the error message
     # we use deamon threads to avoid hanging if the user uses ctrl+c
     th = Thread(target=reader, args=[process.stdout, "stdout", q])
     th.daemon = True
     th.start()
@@ -56,14 +57,16 @@
         for source, line in iter(q.get, None):
             yield source, line
             if source == "stderr":
                 full_stderr += line
 
     exit_code = process.wait()
 
+    logger.debug(f"RETURN CODE: {exit_code}")
+    logger.debug('- -'*10)
     if exit_code != 0:
         raise DockerException(full_cmd, exit_code, stderr=full_stderr)
 
     yield ("exit_code", str(exit_code).encode())
 
 def run_command_with_exit_code(
     full_cmd: list,
```

### Comparing `frappe_manager-0.8.3/frappe_manager/main.py` & `frappe_manager-0.9.0/frappe_manager/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,114 @@
 import typer
 import importlib
+import os
+import requests
+import sys
+import shutil
+import atexit
 from typing import Annotated, List, Optional, Set
-from pathlib import Path
 from frappe_manager.site_manager.manager import SiteManager
 from frappe_manager.site_manager.Richprint import richprint
-import os
-import requests
+from frappe_manager import CLI_DIR
+from frappe_manager.logger import log
 
 app = typer.Typer(no_args_is_help=True,rich_markup_mode='rich')
 
 # TODO configure this using config
 #sites_dir = Path().home() / __name__.split(".")[0]
 
-sites_dir = Path.home() / 'frappe'
-sites = SiteManager(sites_dir)
+def exit_cleanup():
+    """
+    This function is used to perform cleanup at the exit.
+    """
+    richprint.stop()
+
+def cli_entrypoint():
+    # logging
+    logger = log.get_logger()
+    logger.info('')
+    logger.info(f"{':'*20}FM Invoked{':'*20}")
+    logger.info('')
+
+    # logging command provided by user
+    logger.info(f"RUNNING COMMAND: {' '.join(sys.argv[1:])}")
+    logger.info('-'*20)
+    try:
+        app()
+    except Exception as e:
+        logger.exception(f"Exception:  : {e}")
+        raise e
+    finally:
+        atexit.register(exit_cleanup)
 
+# this will be initiated later in the app_callback
+sites: Optional[SiteManager] = None
 
 def version_callback(version: Optional[bool] = None):
     if version:
         fm_version = importlib.metadata.version('frappe_manager')
         richprint.print(fm_version,emoji_code='')
         raise typer.Exit()
 
-
 @app.callback()
 def app_callback(
         ctx: typer.Context,
         verbose: Annotated[Optional[bool], typer.Option('--verbose','-v',help="Enable verbose output.")] = None,
         version: Annotated[
             Optional[bool], typer.Option("--version",help="Show Version.",callback=version_callback)
         ] = None,
 ):
     """
     FrappeManager for creating frappe development envrionments.
     """
+    richprint.start(f"Working")
+
+    # Checks for cli directory
+    if not CLI_DIR.exists():
+        # creating the sites dir
+        # TODO check if it's writeable and readable -> by writing a file to it and catching exception
+        CLI_DIR.mkdir(parents=True, exist_ok=True)
+        richprint.print(f"fm directory doesn't exists! Created at -> {str(CLI_DIR)}")
+    else:
+        if not CLI_DIR.is_dir():
+            richprint.exit("Sites directory is not a directory! Aborting!")
+
+    # migration for directory change from CLI_DIR to CLI_DIR/sites
+    # TODO remove when not required, introduced in 0.8.4
+    sitesdir = CLI_DIR / 'sites'
+    if not sitesdir.exists():
+        richprint.change_head("Site directory migration")
+        move_directory_list = []
+        for site_dir in CLI_DIR.iterdir():
+            if site_dir.is_dir():
+                docker_compose_path = site_dir / "docker-compose.yml"
+                if docker_compose_path.exists():
+                    move_directory_list.append(site_dir)
+
+        # stop all the sites
+        sitesdir.mkdir(parents=True, exist_ok=True)
+        sites_mananger = SiteManager(CLI_DIR)
+        sites_mananger.stop_sites()
+        # move all the directories
+        for site in move_directory_list:
+            site_name = site.parts[-1]
+            new_path = sitesdir / site_name
+            try:
+                shutil.move(site,new_path)
+                richprint.print(f"Directory migrated: {site_name}")
+            except:
+                logger.debug(f'Site Directory migration failed: {site}')
+                richprint.warning(f"Unable to site directory migration for {site}\nPlease manually move it to {new_path}")
+        richprint.print("Site directory migration: Done")
+
+    global sites
+    sites = SiteManager(sitesdir)
+
     sites.set_typer_context(ctx)
+
     if verbose:
         sites.set_verbose()
 
 
 default_extension = [
     "dbaeumer.vscode-eslint",
     "esbenp.prettier-vscode",
@@ -48,26 +118,29 @@
     "visualstudioexptteam.vscodeintellicode",
     "VisualStudioExptTeam.intellicode-api-usage-examples"
 ]
 
 
 def check_frappe_app_exists(appname: str, branchname: str | None = None):
     # check appname
-    app_url = f"https://github.com/frappe/{appname}"
-    app = requests.get(app_url).status_code
-
-    if branchname:
-        branch_url = f"https://github.com/frappe/{appname}/tree/{branchname}"
-        # check branch
-        branch = requests.get(branch_url).status_code
-        return {
-            "app": True if app == 200 else False,
-            "branch": True if branch == 200 else False,
-        }
-    return {"app": True if app == 200 else False}
+    try:
+        app_url = f"https://github.com/frappe/{appname}"
+        app = requests.get(app_url).status_code
+
+        if branchname:
+            branch_url = f"https://github.com/frappe/{appname}/tree/{branchname}"
+            # check branch
+            branch = requests.get(branch_url).status_code
+            return {
+                "app": True if app == 200 else False,
+                "branch": True if branch == 200 else False,
+            }
+        return {"app": True if app == 200 else False}
+    except Exception:
+        richprint.exit("Not able to connect to github.com.")
 
 
 def apps_validation(value: List[str] | None):
     # don't allow frappe the be included throw error
     if value:
         for app in value:
             appx = app.split(":")
@@ -139,15 +212,15 @@
     [bold]# Install frappe\[version-14], erpnext\[version-14] and hrms\[version-14][/bold]
     $ [blue]fm create example --apps erpnext:version-14 --apps hrms:version-14[/blue]
 
     [bold]# Install frappe\[version-15-beta], erpnext\[version-15-beta] and hrms\[version-15-beta][/bold]
     $ [blue]fm create example --frappe-branch version-15-beta --apps erpnext:version-15-beta --apps hrms:version-15-beta[/blue]
     """
 
-    sites.init(sitename, createdir=True)
+    sites.init(sitename)
 
     uid: int = os.getuid()
     gid: int = os.getgid()
 
     frappe_env: dict = {
         "USERID": uid,
         "USERGROUP": gid,
```

### Comparing `frappe_manager-0.8.3/frappe_manager/site_manager/Richprint.py` & `frappe_manager-0.9.0/frappe_manager/site_manager/Richprint.py`

 * *Files identical despite different names*

### Comparing `frappe_manager-0.8.3/frappe_manager/site_manager/SiteCompose.py` & `frappe_manager-0.9.0/frappe_manager/site_manager/SiteCompose.py`

 * *Files identical despite different names*

### Comparing `frappe_manager-0.8.3/frappe_manager/site_manager/manager.py` & `frappe_manager-0.9.0/frappe_manager/site_manager/manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from frappe_manager.docker_wrapper import DockerClient, DockerException
-from typing import List, Optional, Type
+from typing import List, Optional
 from pathlib import Path
 import subprocess
 import json
 import shlex
 import typer
 import shutil
 
@@ -19,49 +19,44 @@
     def __init__(self, sitesdir: Path):
         self.sitesdir = sitesdir
         self.site = None
         self.sitepath = None
         self.verbose = False
         self.typer_context: Optional[typer.Context] = None
 
-    def init(self, sitename: str| None = None,createdir: bool = False):
+    def init(self, sitename: str| None = None):
         """
         The `init` function initializes a site by checking if the site directory exists, creating it if
         necessary, and setting the site name and path.
         
         :param sitename: The `sitename` parameter is a string that represents the name of the site. It is
         optional and can be set to `None`. If a value is provided, it will be used to create a site path by
         appending ".localhost" to the sitename
         :type sitename: str| None
-        :param createdir: The `createdir` parameter is a boolean flag that determines whether or not to
-        create the sites directory if it doesn't already exist. If `createdir` is set to `True`, the code
-        will create the directory. If it's set to `False`, the code will exit with an error, defaults to
-        False
-        :type createdir: bool (optional)
-        """
-        richprint.start(f"Working")
-
-        # check if the site name is correct
-        if not self.sitesdir.exists():
-            # creating the sites dir
-            # TODO check if it's writeable and readable
-            if createdir:
-                self.sitesdir.mkdir(parents=True, exist_ok=True)
-                richprint.print(f"Sites directory doesn't exists! Created at -> {str(self.sitesdir)}")
-            else:
-                richprint.exit(f"Sites directory doesn't exists!")
-
-        if not self.sitesdir.is_dir():
-            richprint.exit("Sites directory is not a directory! Aborting!")
+        """
 
         if sitename:
-            sitename = sitename + ".localhost"
+            if not '.localhost' in sitename:
+                sitename = sitename + ".localhost"
             sitepath: Path = self.sitesdir / sitename
+
+            site_directory_exits_check_for_commands = ['create']
+
+            if self.typer_context.invoked_subcommand in site_directory_exits_check_for_commands:
+                if sitepath.exists():
+                    richprint.exit(
+                        f"Site {sitename} already exists! Aborting! -> [bold cyan] {sitepath}[/bold cyan]"
+                    )
+            else:
+                if not sitepath.exists():
+                    richprint.exit(
+                        f"Site {sitename} doesn't exists! Aborting! -> [bold cyan] {sitepath}[/bold cyan]"
+                    )
+
             self.site: Site = Site(sitepath, sitename, verbose= self.verbose)
-            # self.migrate_site()
 
     def set_verbose(self):
         """
         The function sets the "verbose" attribute of an object to True.
         """
         self.verbose = True
 
@@ -113,16 +108,19 @@
     def stop_sites(self):
         """
         The `stop_sites` function stops all sites except the current site by halting their Docker
         containers.
         """
         status_text='Halting other sites'
         richprint.change_head(status_text)
-        exclude = [self.site.name]
-        site_compose: list = self.__get_all_sites_path(exclude)
+        if self.site:
+            exclude = [self.site.name]
+            site_compose: list = self.__get_all_sites_path(exclude)
+        else:
+            site_compose: list = self.__get_all_sites_path()
         if site_compose:
             for site_compose_path in site_compose:
                 docker = DockerClient(compose_file_path=site_compose_path)
                 try:
                     output = docker.compose.stop(timeout=10,stream=not self.verbose)
                     if not self.verbose:
                         richprint.live_lines(output, padding=(0,0,0,2))
@@ -136,18 +134,16 @@
         necessary images, starts the site, and displays information about the site.
         
         :param template_inputs: The `template_inputs` parameter is a dictionary that contains the inputs or
         configuration values required to generate the compose file for the site. These inputs can be used to
         customize the site's configuration, such as database settings, domain name, etc
         :type template_inputs: dict
         """
-        if self.site.exists():
-            richprint.exit(
-                f"Site {self.site.name} already exists! Aborting! -> [bold cyan] {self.site.path}[/bold cyan]"
-            )
+        # check if provided sitename is valid and only one level subdom of localhost
+        self.site.validate_sitename()
         self.stop_sites()
         # check if ports are available
         self.check_ports()
         richprint.change_head(f"Creating Site Directory")
         self.site.create_dirs()
         richprint.change_head(f"Generating Compose")
         self.site.generate_compose(template_inputs)
@@ -160,48 +156,42 @@
 
     def remove_site(self):
         """
         The `remove_site` function checks if a site exists, stops it if it is running, and then removes the
         site directory.
         """
         # TODO maybe the site is running and folder has been delted and all the containers are there. We need to clean it.
-        # check if it exits
-        if not self.site.exists():
-            richprint.exit(
-                f"Site {self.site.name} doesn't exists! Aborting! -> [bold cyan] {self.site.path}[/bold cyan]"
-            )
-
         richprint.change_head(f"Removing Site")
         # check if running -> stop it
         # remove dir
         self.site.remove()
-        richprint.stop()
 
     def list_sites(self):
         """
         The `list_sites` function retrieves a list of sites, categorizes them as either running or stale,
         and displays them in separate panels using the Rich library.
         """
         # format -> name , status [ 'stale', 'running' ]
         # sites_list = self.__get_all_sites_path()
         running = []
         stale = []
         sites_list = self.get_all_sites()
         if not sites_list:
-            richprint.error("No available sites!!")
+            richprint.error("No sites available !")
             typer.Exit(2)
         else:
             for name in sites_list.keys():
                 temppath = self.sitesdir / name
                 tempSite = Site(temppath,name)
                 if tempSite.running():
                     running.append({'name': name,'path':temppath.absolute()})
                 else:
                    stale.append({'name': name,'path':temppath.absolute()})
         richprint.stop()
+
         if running:
             columns_data = [ f"[b]{x['name']}[/b]\n[dim]{x['path']}[/dim]" for x in running ]
             panel = Panel(Columns(columns_data),title='Running',title_align='left',style='green')
             richprint.stdout.print(panel)
 
         if stale:
             columns_data = [ f"[b]{x['name']}[/b]\n[dim]{x['path']}[/dim]" for x in stale ]
@@ -209,42 +199,32 @@
             richprint.stdout.print(panel)
 
     def stop_site(self):
         """
         The function `stop_site` checks if a site exists, stops it if it does, and prints a message
         indicating that the site has been stopped.
         """
-        if not self.site.exists():
-            richprint.exit(
-                f"Site {self.site.name} doesn't exists! Aborting!"
-            )
         richprint.change_head(f"Stopping site")
         #self.stop_sites()
         self.site.stop()
         richprint.print(f"Stopped site")
-        richprint.stop()
 
     def start_site(self):
         """
         The function `start_site` checks if a site exists, stops all sites, checks ports, pulls the site,
         and starts it.
         """
-        if not self.site.exists():
-            richprint.exit(
-                f"Site {self.site.name} doesn't exists! Aborting!"
-            )
         # stop all sites
         self.stop_sites()
         if not self.site.running():
             self.check_ports()
         # start the provided site
         self.migrate_site()
         self.site.pull()
         self.site.start()
-        richprint.stop()
 
     def attach_to_site(self, user: str, extensions: List[str]):
         """
         The `attach_to_site` function attaches to a running site and opens it in Visual Studio Code with
         specified extensions.
         
         :param user: The `user` parameter is a string that represents the username of the user who wants to
@@ -299,41 +279,35 @@
             # TODO check if vscode exists
             richprint.change_head("Attaching to Container")
             output = subprocess.run(vscode_cmd,shell=True)
             if output.returncode != 0:
                 richprint.exit(f"Attaching to Container : Failed")
             richprint.print(f"Attaching to Container : Done")
         else:
-            print(f"Site: {self.site.name} is not running")
-        richprint.stop()
+            richprint.print(f"Site: {self.site.name} is not running")
 
     def logs(self,service:str,follow):
         """
         The `logs` function checks if a site exists, and if it does, it shows the logs for a specific
         service. If the site is not running, it displays an error message.
         
         :param service: The `service` parameter is a string that represents the specific service or
         component for which you want to view the logs. It could be the name of a specific container
         :type service: str
         :param follow: The "follow" parameter is a boolean value that determines whether to continuously
         follow the logs or not. If "follow" is set to True, the logs will be continuously displayed as they
         are generated. If "follow" is set to False, only the existing logs will be displayed
         """
-        if not self.site.exists():
-            richprint.exit(
-                f"Site {self.site.name} doesn't exists! Aborting!"
-            )
         richprint.change_head(f"Showing logs")
         if self.site.running():
             self.site.logs(service,follow)
         else:
             richprint.error(
                 f"Site {self.site.name} not running!"
             )
-        richprint.stop()
 
     def check_ports(self):
         """
         The `check_ports` function checks if certain ports are already bound by another process using the
         `lsof` command.
         """
         richprint.change_head("Checking Ports")
@@ -366,83 +340,82 @@
         :type container: str
         :param user: The `user` parameter in the `shell` method is an optional parameter that specifies the
         user for which the shell command should be executed. If no user is provided, the default user is set
         to 'frappe'
         :type user: str | None
         """
         richprint.change_head(f"Spawning shell")
-        if not self.site.exists():
-            richprint.exit(
-                f"Site {self.site.name} doesn't exists! Aborting!"
-            )
         if self.site.running():
             if container == 'frappe':
                 if not user:
                     user = 'frappe'
             self.site.shell(container,user)
         else:
             richprint.exit(
                 f"Site {self.site.name} not running!"
             )
-        richprint.stop()
 
     def info(self):
         """
         The `info` function retrieves information about a site, including its URL, root path, database
         details, Frappe username and password, and a list of installed apps.
         """
-        if not self.site.exists():
-            richprint.exit(
-                f"Site {self.site.name} doesn't exists! Aborting!"
-            )
         richprint.change_head(f"Getting site info")
         site_config_file = self.site.path / 'workspace' / 'frappe-bench' / 'sites' / self.site.name / 'site_config.json'
         db_user = None
         db_pass = None
         if site_config_file.exists():
             with open(site_config_file,'r') as f:
                 site_config = json.load(f)
                 db_user = site_config['db_name']
                 db_pass= site_config['db_password']
 
         frappe_password = self.site.composefile.get_envs('frappe')['ADMIN_PASS']
-        site_info_table = Table(box=box.ASCII2,show_lines=True,show_header=False)
+        root_db_password = self.site.composefile.get_envs('mariadb')['MYSQL_ROOT_PASSWORD']
+        site_info_table = Table(box=box.ASCII2,show_lines=True,show_header=False,highlight=True)
         data = {
             "Site Url":f"http://{self.site.name}",
             "Site Root":f"{self.site.path.absolute()}",
             "Mailhog Url":f"http://{self.site.name}/mailhog",
             "Adminer Url":f"http://{self.site.name}/adminer",
             "Frappe Username" : "administrator",
             "Frappe Password" : frappe_password,
-            "DB Host" : f"mariadb",
+            "Root DB User" : 'root',
+            "Root DB Password" : root_db_password,
+            "DB Host" : "mariadb",
             "DB Name" : db_user,
             "DB User" : db_user,
             "DB Password" : db_pass,
+
             }
         site_info_table.add_column()
         site_info_table.add_column()
         for key in data.keys():
             site_info_table.add_row(key,data[key])
-        richprint.stdout.print(site_info_table)
+
         # bench apps list
         richprint.stdout.print('')
-        bench_apps_list_table=Table(title="Bench Apps",box=box.ASCII2,show_lines=True)
+        # bench_apps_list_table=Table(title="Bench Apps",box=box.ASCII2,show_lines=True)
+        bench_apps_list_table=Table(box=box.ASCII2,show_lines=True,expand=True,show_edge=False,pad_edge=False)
         bench_apps_list_table.add_column("App")
         bench_apps_list_table.add_column("Version")
+
+
         apps_json_file = self.site.path / 'workspace' / 'frappe-bench' / 'sites' / 'apps.json'
         if apps_json_file.exists():
             with open(apps_json_file,'r') as f:
                 apps_json = json.load(f)
                 for app in apps_json.keys():
                     bench_apps_list_table.add_row(app,apps_json[app]['version'])
-                richprint.stdout.print(bench_apps_list_table)
-        richprint.stop()
+
+            site_info_table.add_row('Bench Apps',bench_apps_list_table)
+        richprint.stdout.print(site_info_table)
 
     def migrate_site(self):
         """
         The function `migrate_site` checks if the services name is the same as the template, if not, it
         brings down the site, migrates the site, and starts it.
         """
         richprint.change_head("Migrating Environment")
         if not self.site.composefile.is_services_name_same_as_template():
             self.site.down()
-        self.site.migrate_site()
+        self.site.migrate_site_compose()
```

### Comparing `frappe_manager-0.8.3/frappe_manager/site_manager/site.py` & `frappe_manager-0.9.0/frappe_manager/site_manager/site.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,32 +38,29 @@
         """
         The function `validate_sitename` checks if a given sitename is valid by using a regular expression
         pattern.
         :return: a boolean value. If the sitename is valid, it returns True. If the sitename is not valid,
         it returns False.
         """
         sitename = self.name
-        match = re.search(r'^[A-Za-z0-9](?:[A-Za-z0-9\-]{0,61}[A-Za-z0-9])?',sitename)
-        if len(sitename) != match.span()[-1]:
-            return False
-            # console.print(f"[bold red][ERROR] : [/bold red][bold cyan]Not a valid sitename.[/bold cyan]")
-            # exit(2)
-        return True
+        match = re.search(r'^[A-Za-z0-9](?:[A-Za-z0-9\-]{0,61}[A-Za-z0-9])?.localhost$',sitename)
+        if not match:
+            richprint.exit("The site name must follow a single-level subdomain Fully Qualified Domain Name (FQDN) format of localhost, such as 'suddomain.localhost'.")
 
     def get_frappe_container_hex(self) -> None | str:
         """
         The function `get_frappe_container_hex` searches for a Docker container with the name containing
         "-frappe" and returns its hexadecimal representation if found, otherwise returns None.
         :return: either a hexadecimal string representing the name of the Frappe container, or None if no
         Frappe container is found.
         """
         container_name = self.composefile.get_container_names()
         return container_name['frappe'].encode().hex()
 
-    def migrate_site(self) :
+    def migrate_site_compose(self) :
         """
         The `migrate_site` function checks the environment version and migrates it if necessary.
         :return: a boolean value,`True` if the site migrated else `False`.
         """
         if self.composefile.exists():
             richprint.change_head("Checking Environment Version")
             compose_version = self.composefile.get_version()
@@ -163,24 +160,25 @@
         """
         The function `frappe_logs_till_start` prints logs until a specific line is found and then stops.
         """
         status_text= 'Creating Site'
         richprint.change_head(status_text)
         try:
             output = self.docker.compose.logs(services=['frappe'],no_log_prefix=True,follow=True,stream=True)
+
             if self.quiet:
                 richprint.live_lines(output, padding=(0,0,0,2),stop_string="INFO spawned: 'bench-dev' with pid")
             else:
                 for source , line in self.docker.compose.logs(services=['frappe'],no_log_prefix=True,follow=True,stream=True):
                     if not source == 'exit_code':
                         line = line.decode()
                         if "[==".lower() in line.lower():
                             print(line)
                         else:
-                            richprint.stdout.print(line,end='')
+                            richprint.stdout.print(line)
                         if "INFO spawned: 'bench-dev' with pid".lower() in line.lower():
                             break
             richprint.print(f"{status_text}: Done")
         except DockerException as e:
             richprint.warning(f"{status_text}: Failed")
```

### Comparing `frappe_manager-0.8.3/frappe_manager/site_manager/templates/docker-compose.tmpl` & `frappe_manager-0.9.0/frappe_manager/site_manager/templates/docker-compose.tmpl`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 version: "3.9"
 services:
   frappe:
-    image: ghcr.io/rtcamp/frappe-manager-frappe:v0.8.3
+    image: ghcr.io/rtcamp/frappe-manager-frappe:v0.9.0
     environment:
       - SHELL=/bin/bash
     volumes:
       - ./workspace:/workspace:cached
     ports:
       - 80
       - 9000:9000
```

### Comparing `frappe_manager-0.8.3/PKG-INFO` & `frappe_manager-0.9.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6672 6170  : 2.1.Name: frap
 00000020: 7065 2d6d 616e 6167 6572 0a56 6572 7369  pe-manager.Versi
-00000030: 6f6e 3a20 302e 382e 330a 5375 6d6d 6172  on: 0.8.3.Summar
+00000030: 6f6e 3a20 302e 392e 300a 5375 6d6d 6172  on: 0.9.0.Summar
 00000040: 793a 2041 2043 4c49 2074 6f6f 6c20 6261  y: A CLI tool ba
 00000050: 7365 6420 6f6e 2044 6f63 6b65 7220 436f  sed on Docker Co
 00000060: 6d70 6f73 6520 746f 2065 6173 696c 7920  mpose to easily 
 00000070: 6d61 6e61 6765 2046 7261 7070 6520 6261  manage Frappe ba
 00000080: 7365 6420 7072 6f6a 6563 7473 2e20 4173  sed projects. As
 00000090: 206f 6620 6e6f 772c 206f 6e6c 7920 7375   of now, only su
 000000a0: 6974 6162 6c65 2066 6f72 2064 6576 656c  itable for devel
@@ -20,120 +20,115 @@
 00000130: 686f 723a 2072 7443 616d 700a 4175 7468  hor: rtCamp.Auth
 00000140: 6f72 2d65 6d61 696c 3a20 7379 7340 7274  or-email: sys@rt
 00000150: 6361 6d70 2e63 6f6d 0a4d 6169 6e74 6169  camp.com.Maintai
 00000160: 6e65 723a 2041 6c6f 6b20 5369 6e67 680a  ner: Alok Singh.
 00000170: 4d61 696e 7461 696e 6572 2d65 6d61 696c  Maintainer-email
 00000180: 3a20 616c 6f6b 2e73 696e 6768 4072 7463  : alok.singh@rtc
 00000190: 616d 702e 636f 6d0a 5265 7175 6972 6573  amp.com.Requires
-000001a0: 2d50 7974 686f 6e3a 203e 3d33 2e31 312c  -Python: >=3.11,
+000001a0: 2d50 7974 686f 6e3a 203e 3d33 2e31 302c  -Python: >=3.10,
 000001b0: 3c34 2e30 0a43 6c61 7373 6966 6965 723a  <4.0.Classifier:
 000001c0: 204c 6963 656e 7365 203a 3a20 4f53 4920   License :: OSI 
 000001d0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
 000001e0: 4c69 6365 6e73 650a 436c 6173 7369 6669  License.Classifi
 000001f0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
 00000200: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
 00000210: 6f6e 203a 3a20 330a 436c 6173 7369 6669  on :: 3.Classifi
 00000220: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
 00000230: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000240: 6f6e 203a 3a20 332e 3131 0a52 6571 7569  on :: 3.11.Requi
-00000250: 7265 732d 4469 7374 3a20 6a69 6e6a 6132  res-Dist: jinja2
-00000260: 2028 3e3d 332e 312e 322c 3c34 2e30 2e30   (>=3.1.2,<4.0.0
-00000270: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000280: 2070 7979 616d 6c20 283e 3d36 2e30 2e31   pyyaml (>=6.0.1
-00000290: 2c3c 372e 302e 3029 0a52 6571 7569 7265  ,<7.0.0).Require
-000002a0: 732d 4469 7374 3a20 7265 7175 6573 7473  s-Dist: requests
-000002b0: 2028 3e3d 322e 3331 2e30 2c3c 332e 302e   (>=2.31.0,<3.0.
-000002c0: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
-000002d0: 3a20 7479 7065 725b 616c 6c5d 2028 3e3d  : typer[all] (>=
-000002e0: 302e 392e 302c 3c30 2e31 302e 3029 0a50  0.9.0,<0.10.0).P
-000002f0: 726f 6a65 6374 2d55 524c 3a20 5265 706f  roject-URL: Repo
-00000300: 7369 746f 7279 2c20 6874 7470 733a 2f2f  sitory, https://
-00000310: 6769 7468 7562 2e63 6f6d 2f72 7463 616d  github.com/rtcam
-00000320: 702f 6672 6170 7065 2d6d 616e 6167 6572  p/frappe-manager
-00000330: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-00000340: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-00000350: 6d61 726b 646f 776e 0a0a 2320 4672 6170  markdown..# Frap
-00000360: 7065 2d4d 616e 6167 6572 0a0a 4120 434c  pe-Manager..A CL
-00000370: 4920 746f 6f6c 2062 6173 6564 206f 6e20  I tool based on 
-00000380: 446f 636b 6572 2043 6f6d 706f 7365 2074  Docker Compose t
-00000390: 6f20 6561 7369 6c79 206d 616e 6167 6520  o easily manage 
-000003a0: 4672 6170 7065 2062 6173 6564 2070 726f  Frappe based pro
-000003b0: 6a65 6374 732e 2041 7320 6f66 206e 6f77  jects. As of now
-000003c0: 2c20 6f6e 6c79 2073 7569 7461 626c 6520  , only suitable 
-000003d0: 666f 7220 6465 7665 6c6f 706d 656e 7420  for development 
-000003e0: 696e 206c 6f63 616c 206d 6163 6869 6e65  in local machine
-000003f0: 7320 7275 6e6e 696e 6720 6f6e 204d 6163  s running on Mac
-00000400: 2061 6e64 204c 696e 7578 2062 6173 6564   and Linux based
-00000410: 204f 532e 0a0a 0a21 5b46 7261 7070 652d   OS....![Frappe-
-00000420: 4d61 6e61 6765 722d 4372 6561 7465 2d53  Manager-Create-S
-00000430: 6974 652e 7376 675d 2868 7474 7073 3a2f  ite.svg](https:/
-00000440: 2f67 6974 6875 622e 636f 6d2f 7274 4361  /github.com/rtCa
-00000450: 6d70 2f46 7261 7070 652d 4d61 6e61 6765  mp/Frappe-Manage
-00000460: 722f 6173 7365 7473 2f32 3632 3430 3738  r/assets/2624078
-00000470: 302f 3738 3434 3138 6635 2d37 3433 382d  0/784418f5-7438-
-00000480: 3466 3231 2d61 6238 342d 6432 6365 3434  4f21-ab84-d2ce44
-00000490: 6237 6438 6332 290a 0a0a 2323 2049 6e73  b7d8c2)...## Ins
-000004a0: 7461 6c6c 6174 696f 6e0a 2a2a 5265 7175  tallation.**Requ
-000004b0: 6972 656d 656e 7473 3a2a 2a20 5079 7468  irements:** Pyth
-000004c0: 6f6e 332e 3131 2b2c 2044 6f63 6b65 722c  on3.11+, Docker,
-000004d0: 2056 5343 6f64 6528 6f70 7469 6f6e 616c   VSCode(optional
-000004e0: 290a 0a60 6060 6261 7368 0a70 6970 2069  )..```bash.pip i
-000004f0: 6e73 7461 6c6c 2066 7261 7070 652d 6d61  nstall frappe-ma
-00000500: 6e61 6765 720a 6060 600a 0a23 2323 2053  nager.```..### S
-00000510: 6574 7570 2041 7574 6f63 6f6d 706c 6574  etup Autocomplet
-00000520: 696f 6e20 2020 200a 312e 2060 6060 6261  ion    .1. ```ba
-00000530: 7368 0a20 2020 666d 202d 2d69 6e73 7461  sh.   fm --insta
-00000540: 6c6c 2d63 6f6d 706c 6574 696f 6e0a 2020  ll-completion.  
-00000550: 2060 6060 0a32 2e20 5265 7374 6172 7420   ```.2. Restart 
-00000560: 7368 656c 6c20 6f72 2074 6572 6d69 6e61  shell or termina
-00000570: 6c0a 0a0a 2323 2055 7361 6765 0a23 2323  l...## Usage.###
-00000580: 2043 7265 6174 6520 6120 7369 7465 0a0a   Create a site..
-00000590: 6060 6062 6173 680a 2320 6372 6561 7465  ```bash.# create
-000005a0: 2065 7861 6d70 6c65 2e6c 6f63 616c 686f   example.localho
-000005b0: 7374 2073 6974 6520 7769 7468 206f 6e6c  st site with onl
-000005c0: 7920 6672 6170 7065 2c20 7665 7273 696f  y frappe, versio
-000005d0: 6e20 2d3e 2076 6572 7369 6f6e 2d31 350a  n -> version-15.
-000005e0: 666d 2063 7265 6174 6520 6578 616d 706c  fm create exampl
-000005f0: 650a 0a23 2063 7265 6174 6520 6578 616d  e..# create exam
-00000600: 706c 652e 6c6f 6361 6c68 6f73 7420 7369  ple.localhost si
-00000610: 7465 2077 6974 6820 6f6e 6c79 2066 7261  te with only fra
-00000620: 7070 652c 2076 6572 7369 6f6e 202d 3e20  ppe, version -> 
-00000630: 6465 7665 6c6f 700a 666d 2063 7265 6174  develop.fm creat
-00000640: 6520 6578 616d 706c 6520 2d2d 6672 6170  e example --frap
-00000650: 7065 2d62 7261 6e63 6820 6465 7665 6c6f  pe-branch develo
-00000660: 700a 0a23 2063 7265 6174 6520 6578 616d  p..# create exam
-00000670: 706c 652e 6c6f 6361 6c68 6f73 7420 7369  ple.localhost si
-00000680: 7465 2077 6974 6820 6672 6170 7065 2c20  te with frappe, 
-00000690: 6572 706e 6578 7420 616e 6420 6872 6d73  erpnext and hrms
-000006a0: 2c20 7665 7273 696f 6e20 2d3e 2076 6572  , version -> ver
-000006b0: 7369 6f6e 2d31 350a 666d 2063 7265 6174  sion-15.fm creat
-000006c0: 6520 6578 616d 706c 6520 2d2d 6170 7073  e example --apps
-000006d0: 2065 7270 6e65 7874 3a76 6572 7369 6f6e   erpnext:version
-000006e0: 2d31 3520 2d2d 6170 7073 2068 726d 733a  -15 --apps hrms:
-000006f0: 7665 7273 696f 6e2d 3135 2020 2020 0a60  version-15    .`
-00000700: 6060 0a0a 5669 7369 7420 434c 4920 5b57  ``..Visit CLI [W
-00000710: 696b 695d 2868 7474 7073 3a2f 2f67 6974  iki](https://git
-00000720: 6875 622e 636f 6d2f 7274 4361 6d70 2f46  hub.com/rtCamp/F
-00000730: 7261 7070 652d 4d61 6e61 6765 722f 7769  rappe-Manager/wi
-00000740: 6b69 2920 666f 7220 6d6f 7265 2065 7861  ki) for more exa
-00000750: 6d70 6c65 730a 0a23 2320 4372 6564 6974  mples..## Credit
-00000760: 730a 446f 636b 6572 6669 6c65 733a 205b  s.Dockerfiles: [
-00000770: 4672 6170 7065 2044 6f63 6b65 725d 2868  Frappe Docker](h
-00000780: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000790: 6d2f 6672 6170 7065 2f66 7261 7070 655f  m/frappe/frappe_
-000007a0: 646f 636b 6572 290a 0a23 2320 446f 6573  docker)..## Does
-000007b0: 2074 6869 7320 696e 7465 7265 7374 2079   this interest y
-000007c0: 6f75 3f0a 0a3c 6120 6872 6566 3d22 6874  ou?..<a href="ht
-000007d0: 7470 733a 2f2f 7274 6361 6d70 2e63 6f6d  tps://rtcamp.com
-000007e0: 2f22 3e3c 696d 6720 7372 633d 2268 7474  /"><img src="htt
-000007f0: 7073 3a2f 2f72 7463 616d 702e 636f 6d2f  ps://rtcamp.com/
-00000800: 7770 2d63 6f6e 7465 6e74 2f75 706c 6f61  wp-content/uploa
-00000810: 6473 2f73 6974 6573 2f32 2f32 3031 392f  ds/sites/2/2019/
-00000820: 3034 2f67 6974 6875 622d 6261 6e6e 6572  04/github-banner
-00000830: 4032 782e 706e 6722 2061 6c74 3d22 4a6f  @2x.png" alt="Jo
-00000840: 696e 2075 7320 6174 2072 7443 616d 702c  in us at rtCamp,
-00000850: 2077 6520 7370 6563 6961 6c69 7a65 2069   we specialize i
-00000860: 6e20 7072 6f76 6964 696e 6720 6869 6768  n providing high
-00000870: 2070 6572 666f 726d 616e 6365 2065 6e74   performance ent
-00000880: 6572 7072 6973 6520 576f 7264 5072 6573  erprise WordPres
-00000890: 7320 736f 6c75 7469 6f6e 7322 3e3c 2f61  s solutions"></a
-000008a0: 3e0a 0a                                  >..
+00000240: 6f6e 203a 3a20 332e 3130 0a43 6c61 7373  on :: 3.10.Class
+00000250: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000260: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000270: 7974 686f 6e20 3a3a 2033 2e31 310a 5265  ython :: 3.11.Re
+00000280: 7175 6972 6573 2d44 6973 743a 2070 7979  quires-Dist: pyy
+00000290: 616d 6c20 283e 3d36 2e30 2e31 2c3c 372e  aml (>=6.0.1,<7.
+000002a0: 302e 3029 0a52 6571 7569 7265 732d 4469  0.0).Requires-Di
+000002b0: 7374 3a20 7265 7175 6573 7473 2028 3e3d  st: requests (>=
+000002c0: 322e 3331 2e30 2c3c 332e 302e 3029 0a52  2.31.0,<3.0.0).R
+000002d0: 6571 7569 7265 732d 4469 7374 3a20 7479  equires-Dist: ty
+000002e0: 7065 725b 616c 6c5d 2028 3e3d 302e 392e  per[all] (>=0.9.
+000002f0: 302c 3c30 2e31 302e 3029 0a50 726f 6a65  0,<0.10.0).Proje
+00000300: 6374 2d55 524c 3a20 4275 6720 5472 6163  ct-URL: Bug Trac
+00000310: 6b65 722c 2068 7474 7073 3a2f 2f67 6974  ker, https://git
+00000320: 6875 622e 636f 6d2f 7274 6361 6d70 2f66  hub.com/rtcamp/f
+00000330: 7261 7070 652d 6d61 6e61 6765 722f 6973  rappe-manager/is
+00000340: 7375 6573 0a50 726f 6a65 6374 2d55 524c  sues.Project-URL
+00000350: 3a20 446f 6375 6d65 6e74 6174 696f 6e2c  : Documentation,
+00000360: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000370: 636f 6d2f 7274 6361 6d70 2f66 7261 7070  com/rtcamp/frapp
+00000380: 652d 6d61 6e61 6765 722f 7769 6b69 0a50  e-manager/wiki.P
+00000390: 726f 6a65 6374 2d55 524c 3a20 5265 706f  roject-URL: Repo
+000003a0: 7369 746f 7279 2c20 6874 7470 733a 2f2f  sitory, https://
+000003b0: 6769 7468 7562 2e63 6f6d 2f72 7463 616d  github.com/rtcam
+000003c0: 702f 6672 6170 7065 2d6d 616e 6167 6572  p/frappe-manager
+000003d0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+000003e0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+000003f0: 6d61 726b 646f 776e 0a0a 2320 4672 6170  markdown..# Frap
+00000400: 7065 2d4d 616e 6167 6572 0a0a 4120 434c  pe-Manager..A CL
+00000410: 4920 746f 6f6c 2062 6173 6564 206f 6e20  I tool based on 
+00000420: 446f 636b 6572 2043 6f6d 706f 7365 2074  Docker Compose t
+00000430: 6f20 6561 7369 6c79 206d 616e 6167 6520  o easily manage 
+00000440: 4672 6170 7065 2062 6173 6564 2070 726f  Frappe based pro
+00000450: 6a65 6374 732e 2041 7320 6f66 206e 6f77  jects. As of now
+00000460: 2c20 6f6e 6c79 2073 7569 7461 626c 6520  , only suitable 
+00000470: 666f 7220 6465 7665 6c6f 706d 656e 7420  for development 
+00000480: 696e 206c 6f63 616c 206d 6163 6869 6e65  in local machine
+00000490: 7320 7275 6e6e 696e 6720 6f6e 204d 6163  s running on Mac
+000004a0: 2061 6e64 204c 696e 7578 2062 6173 6564   and Linux based
+000004b0: 204f 532e 0a0a 0a21 5b46 7261 7070 652d   OS....![Frappe-
+000004c0: 4d61 6e61 6765 722d 4372 6561 7465 2d53  Manager-Create-S
+000004d0: 6974 652e 7376 675d 2868 7474 7073 3a2f  ite.svg](https:/
+000004e0: 2f75 7365 722d 696d 6167 6573 2e67 6974  /user-images.git
+000004f0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000500: 6f6d 2f32 3832 3934 3739 352f 3238 3331  om/28294795/2831
+00000510: 3038 3739 312d 3032 3337 6430 3561 2d32  08791-0237d05a-2
+00000520: 3536 322d 3438 6265 2d39 3837 622d 3033  562-48be-987b-03
+00000530: 3761 3230 3064 3731 6133 2e73 7667 290a  7a200d71a3.svg).
+00000540: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+00000550: 6e0a 2a2a 5265 7175 6972 656d 656e 7473  n.**Requirements
+00000560: 3a2a 2a20 5079 7468 6f6e 332e 3131 2b2c  :** Python3.11+,
+00000570: 2044 6f63 6b65 722c 2056 5343 6f64 6528   Docker, VSCode(
+00000580: 6f70 7469 6f6e 616c 290a 0a60 6060 6261  optional)..```ba
+00000590: 7368 0a70 6970 2069 6e73 7461 6c6c 2066  sh.pip install f
+000005a0: 7261 7070 652d 6d61 6e61 6765 720a 6060  rappe-manager.``
+000005b0: 600a 0a23 2323 2053 6574 7570 2041 7574  `..### Setup Aut
+000005c0: 6f63 6f6d 706c 6574 696f 6e20 2020 200a  ocompletion    .
+000005d0: 312e 2060 6060 6261 7368 0a20 2020 666d  1. ```bash.   fm
+000005e0: 202d 2d69 6e73 7461 6c6c 2d63 6f6d 706c   --install-compl
+000005f0: 6574 696f 6e0a 2020 2060 6060 0a32 2e20  etion.   ```.2. 
+00000600: 5265 7374 6172 7420 7368 656c 6c20 6f72  Restart shell or
+00000610: 2074 6572 6d69 6e61 6c0a 0a0a 2323 2055   terminal...## U
+00000620: 7361 6765 0a23 2323 2043 7265 6174 6520  sage.### Create 
+00000630: 6120 7369 7465 0a0a 6060 6062 6173 680a  a site..```bash.
+00000640: 2320 6372 6561 7465 2065 7861 6d70 6c65  # create example
+00000650: 2e6c 6f63 616c 686f 7374 2073 6974 6520  .localhost site 
+00000660: 7769 7468 206f 6e6c 7920 6672 6170 7065  with only frappe
+00000670: 2c20 7665 7273 696f 6e20 2d3e 2076 6572  , version -> ver
+00000680: 7369 6f6e 2d31 350a 666d 2063 7265 6174  sion-15.fm creat
+00000690: 6520 6578 616d 706c 650a 0a23 2063 7265  e example..# cre
+000006a0: 6174 6520 6578 616d 706c 652e 6c6f 6361  ate example.loca
+000006b0: 6c68 6f73 7420 7369 7465 2077 6974 6820  lhost site with 
+000006c0: 6f6e 6c79 2066 7261 7070 652c 2076 6572  only frappe, ver
+000006d0: 7369 6f6e 202d 3e20 6465 7665 6c6f 700a  sion -> develop.
+000006e0: 666d 2063 7265 6174 6520 6578 616d 706c  fm create exampl
+000006f0: 6520 2d2d 6672 6170 7065 2d62 7261 6e63  e --frappe-branc
+00000700: 6820 6465 7665 6c6f 700a 0a23 2063 7265  h develop..# cre
+00000710: 6174 6520 6578 616d 706c 652e 6c6f 6361  ate example.loca
+00000720: 6c68 6f73 7420 7369 7465 2077 6974 6820  lhost site with 
+00000730: 6672 6170 7065 2c20 6572 706e 6578 7420  frappe, erpnext 
+00000740: 616e 6420 6872 6d73 2c20 7665 7273 696f  and hrms, versio
+00000750: 6e20 2d3e 2076 6572 7369 6f6e 2d31 350a  n -> version-15.
+00000760: 666d 2063 7265 6174 6520 6578 616d 706c  fm create exampl
+00000770: 6520 2d2d 6170 7073 2065 7270 6e65 7874  e --apps erpnext
+00000780: 3a76 6572 7369 6f6e 2d31 3520 2d2d 6170  :version-15 --ap
+00000790: 7073 2068 726d 733a 7665 7273 696f 6e2d  ps hrms:version-
+000007a0: 3135 2020 2020 0a60 6060 0a0a 5669 7369  15    .```..Visi
+000007b0: 7420 434c 4920 5b57 696b 695d 2868 7474  t CLI [Wiki](htt
+000007c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000007d0: 7274 4361 6d70 2f46 7261 7070 652d 4d61  rtCamp/Frappe-Ma
+000007e0: 6e61 6765 722f 7769 6b69 2920 666f 7220  nager/wiki) for 
+000007f0: 6d6f 7265 2065 7861 6d70 6c65 730a 0a23  more examples..#
+00000800: 2320 4372 6564 6974 730a 446f 636b 6572  # Credits.Docker
+00000810: 6669 6c65 733a 205b 4672 6170 7065 2044  files: [Frappe D
+00000820: 6f63 6b65 725d 2868 7474 7073 3a2f 2f67  ocker](https://g
+00000830: 6974 6875 622e 636f 6d2f 6672 6170 7065  ithub.com/frappe
+00000840: 2f66 7261 7070 655f 646f 636b 6572 290a  /frappe_docker).
+00000850: 0a                                       .
```

