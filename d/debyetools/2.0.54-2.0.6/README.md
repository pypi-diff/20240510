# Comparing `tmp/debyetools-2.0.54.tar.gz` & `tmp/debyetools-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debyetools-2.0.54.tar", last modified: Thu Dec 14 20:29:46 2023, max compression
+gzip compressed data, was "debyetools-2.0.6.tar", last modified: Fri May 10 16:22:04 2024, max compression
```

## Comparing `debyetools-2.0.54.tar` & `debyetools-2.0.6.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-12-14 20:29:46.976358 debyetools-2.0.54/
--rw-rw-r--   0 travis    (2000) travis    (2000)    34521 2023-12-14 20:28:05.000000 debyetools-2.0.54/LICENSE.md
--rw-r--r--   0 travis    (2000) travis    (2000)     4175 2023-12-14 20:29:46.972358 debyetools-2.0.54/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3294 2023-12-14 20:28:05.000000 debyetools-2.0.54/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-12-14 20:29:46.860350 debyetools-2.0.54/debyetools/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12478 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/anharmonicity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7880 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/aux_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3054 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/debfunct.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9511 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/defects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8553 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/electronic.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-12-14 20:29:46.860350 debyetools-2.0.54/debyetools/examples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-12-14 20:29:46.876351 debyetools-2.0.54/debyetools/examples/Ag_fcc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      732 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/CONTCAR.5
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.00
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)  1577236 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/OUTCAR.eps
--rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Ag_fcc/SUMMARY.fcc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-12-14 20:29:46.896352 debyetools-2.0.54/debyetools/examples/Al3Li_D022/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1144 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/CONTCAR.5
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.00
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)  4597169 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/OUTCAR.eps
--rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D022/SUMMARY.fcc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-12-14 20:29:46.928355 debyetools-2.0.54/debyetools/examples/Al3Li_D023/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2063 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/CONTCAR.5
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.00
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)  5101281 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/OUTCAR.eps
--rw-rw-r--   0 travis    (2000) travis    (2000)     1576 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_D023/SUMMARY.fcc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-12-14 20:29:46.948356 debyetools-2.0.54/debyetools/examples/Al3Li_L12/
--rw-rw-r--   0 travis    (2000) travis    (2000)      743 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/CONTCAR.5
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.00
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)  6488719 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/OUTCAR.eps
--rw-rw-r--   0 travis    (2000) travis    (2000)     1586 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al3Li_L12/SUMMARY.fcc
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-12-14 20:29:46.964357 debyetools-2.0.54/debyetools/examples/Al_fcc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      744 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/CONTCAR.5
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.00
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.10
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.01
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.02
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.03
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.04
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.05
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.06
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.07
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.08
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.09
--rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.1
--rw-rw-r--   0 travis    (2000) travis    (2000)  1485651 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/OUTCAR.eps
--rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/Al_fcc/SUMMARY.fcc
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/examples/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/fs_compound_db.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13605 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/ndeb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4340 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/pairanalysis.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3651 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/poisson.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   176909 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/potentials.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-12-14 20:29:46.972358 debyetools-2.0.54/debyetools/tpropsgui/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13556 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/atomtools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      688 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/dialog_doscar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1480 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/dialog_outcar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2079 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/dialog_summary.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      268 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/dialog_warning.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3019 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/elements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34358 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/events.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13883 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/functions0.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2272 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/get_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    43045 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/gui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      822 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/keygen.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10086 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/layout.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      876 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/lock.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10587 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/mainwindow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/plot_EV.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11627 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/plotter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4359 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/plotter_class.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      883 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/toolbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3416 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/ui_dialogSUMMARY.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2460 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/ui_dialog_doscar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2221 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/ui_dialog_outcar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16226 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/ui_heatcapacitywindow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18970 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/ui_interatomic_params.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22872 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/ui_mainwindow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/ui_missingkey.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1522 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/ui_warning.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8050 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/window_cp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6637 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/tpropsgui/window_interatomicparams.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26170 2023-12-14 20:28:05.000000 debyetools-2.0.54/debyetools/vibrational.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-12-14 20:29:46.972358 debyetools-2.0.54/debyetools.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     4175 2023-12-14 20:29:46.000000 debyetools-2.0.54/debyetools.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     6985 2023-12-14 20:29:46.000000 debyetools-2.0.54/debyetools.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-12-14 20:29:46.000000 debyetools-2.0.54/debyetools.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       35 2023-12-14 20:29:46.000000 debyetools-2.0.54/debyetools.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2023-12-14 20:29:46.000000 debyetools-2.0.54/debyetools.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-12-14 20:29:46.976358 debyetools-2.0.54/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1532 2023-12-14 20:28:05.000000 debyetools-2.0.54/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.591814 debyetools-2.0.6/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34521 2024-05-10 16:20:12.000000 debyetools-2.0.6/LICENSE.md
+-rw-r--r--   0 travis    (2000) travis    (2000)     4174 2024-05-10 16:22:04.591814 debyetools-2.0.6/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3294 2024-05-10 16:20:12.000000 debyetools-2.0.6/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.479803 debyetools-2.0.6/debyetools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12478 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/anharmonicity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7994 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/aux_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3054 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/debfunct.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9511 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/defects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8553 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/electronic.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.479803 debyetools-2.0.6/debyetools/examples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.495805 debyetools-2.0.6/debyetools/examples/Ag_fcc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      732 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/CONTCAR.5
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.00
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1577236 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/OUTCAR.eps
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Ag_fcc/SUMMARY.fcc
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.515807 debyetools-2.0.6/debyetools/examples/Al3Li_D022/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1144 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/CONTCAR.5
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.00
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   567881 2024-05-10 16:20:12.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)  4597169 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/OUTCAR.eps
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D022/SUMMARY.fcc
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.551810 debyetools-2.0.6/debyetools/examples/Al3Li_D023/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2063 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/CONTCAR.5
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.00
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1117465 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)  5101281 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/OUTCAR.eps
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1576 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_D023/SUMMARY.fcc
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.567812 debyetools-2.0.6/debyetools/examples/Al3Li_L12/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      743 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/CONTCAR.5
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.00
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)  6488719 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/OUTCAR.eps
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1586 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al3Li_L12/SUMMARY.fcc
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.583814 debyetools-2.0.6/debyetools/examples/Al_fcc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      744 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/CONTCAR.5
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.00
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.10
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.01
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.02
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.03
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.04
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.05
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.06
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.07
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.08
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.09
+-rw-rw-r--   0 travis    (2000) travis    (2000)   293089 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.1
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1485651 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/OUTCAR.eps
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1565 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/Al_fcc/SUMMARY.fcc
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/examples/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1532 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/fs_compound_db.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13605 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/ndeb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4340 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/pairanalysis.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3651 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/poisson.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   176909 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/potentials.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.587814 debyetools-2.0.6/debyetools/tpropsgui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13556 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/atomtools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      688 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/dialog_doscar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1480 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/dialog_outcar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2079 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/dialog_summary.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      268 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/dialog_warning.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3019 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/elements.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34358 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/events.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13883 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/functions0.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2272 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/get_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    43045 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/gui.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      822 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/keygen.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10086 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/layout.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      876 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/lock.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10587 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/mainwindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/plot_EV.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11627 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/plotter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4359 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/plotter_class.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      883 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/toolbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3416 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_dialogSUMMARY.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2460 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_dialog_doscar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2221 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_dialog_outcar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16226 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_heatcapacitywindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18970 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_interatomic_params.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22872 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_mainwindow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1444 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_missingkey.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1522 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/ui_warning.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8050 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/window_cp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6637 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/tpropsgui/window_interatomicparams.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26101 2024-05-10 16:20:13.000000 debyetools-2.0.6/debyetools/vibrational.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-10 16:22:04.591814 debyetools-2.0.6/debyetools.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     4174 2024-05-10 16:22:04.000000 debyetools-2.0.6/debyetools.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6985 2024-05-10 16:22:04.000000 debyetools-2.0.6/debyetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-10 16:22:04.000000 debyetools-2.0.6/debyetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       35 2024-05-10 16:22:04.000000 debyetools-2.0.6/debyetools.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2024-05-10 16:22:04.000000 debyetools-2.0.6/debyetools.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-05-10 16:22:04.591814 debyetools-2.0.6/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1531 2024-05-10 16:20:13.000000 debyetools-2.0.6/setup.py
```

### Comparing `debyetools-2.0.54/LICENSE.md` & `debyetools-2.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/PKG-INFO` & `debyetools-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debyetools
-Version: 2.0.54
+Version: 2.0.6
 Summary: Debye approximation implementation for the calculation of thermodynamic properties from ground-state atomistic simulations.
 Home-page: https://debyetools.readthedocs.io/
 Author: Javier Jofre
 Author-email: javier.jofre@polymtl.ca
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `debyetools-2.0.54/README.md` & `debyetools-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/anharmonicity.py` & `debyetools-2.0.6/debyetools/anharmonicity.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/aux_functions.py` & `debyetools-2.0.6/debyetools/aux_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 import itertools as it
 import re
 import numpy as np
 from typing import Tuple
 
+
 class logging(object):
     def __init__(self, *files: ...) -> None:
         self.files = files
+
     def write(self, obj: str) -> None:
         for f in self.files:
             f.write(obj)
             f.flush()
-    def flush(self)  -> None:
+
+    def flush(self) -> None:
         for f in self.files:
             f.flush()
+
+
 def c_types(atom_types: str) -> Tuple[list, list]:
     """
     returns all the pair types combinations.
 
     :param str atom_types: the types of each atom in the primitive cell in the same order as the basis vectors.
     :return: pair types and list wuth individual types.
     :rtype: Tuple[list, list]
     """
     types_all = re.findall('[A-Z][^A-Z]*', atom_types)
-    ptypes=list(set([s for s in types_all]))
+    ptypes = list(set([s for s in types_all]))
     ptypes.sort()
     combs_types = list(it.combinations_with_replacement(ptypes, r=2))
-    combs_types = [A[0]+'-'+A[1] for A in combs_types]
+    combs_types = [A[0] + '-' + A[1] for A in combs_types]
     return combs_types, types_all
 
+
 def generate_cells_coordinates(size: np.ndarray, primitive_cell: np.ndarray, center: np.ndarray) -> np.ndarray:
     """ generate the cell coordinates for which we are going
     to calculate the neighbor list.
 
     :param np.ndarray size: Number of times we are replicating the primitive cell
     :param np.ndarray primitive_cell: The primitive cell
     :param np.ndarray center: The position in space where the system of reference is
@@ -45,134 +51,140 @@
                                             np.arange(size[2])))))
 
     cell_coords_centered = cell_coords + center
     cell_coords_centered = np.dot(cell_coords_centered, primitive_cell)
 
     return cell_coords_centered
 
+
 def gen_Ts(Ti: float, Tf: float, nTs: int) -> np.ndarray:
     """
     Function to generate a range of temperatures.
 
     :param float Ti: Initial temperature. (Try not to use the value 0. Use 0.1 instead.)
     :param float Tf: Final temperature.
     :param int nTs: Number of values. This does not include room temperature, which is included anyways.
 
     :retun np.ndarray: Values of temperatures between Ti and Tf, inclusive, plus room temperature.
     """
-    minF_step = (Tf - Ti)/(nTs - 1.)
-    Ts = np.arange(Ti, Tf+minF_step, minF_step)
+    minF_step = (Tf - Ti) / (nTs - 1.)
+    Ts = np.arange(Ti, Tf + minF_step, minF_step)
     Ts = np.r_[Ts, [298.15]]
     Ts.sort()
     return Ts
-def gen_Ps(Pi,Pf,nPs):
+
+
+def gen_Ps(Pi, Pf, nPs):
     """
     Function to generate a range of pressures.
 
     :param float Pi: Initial pressure.
     :param float Pf: Final pressure.
     :param int nPs: Number of values. This does not include room pressure, which is included anyways.
 
     :retun: Values of pressures between Pi and Pf.
     :rtype: np.ndarray
     """
     if nPs <= 1: return np.array([Pi])
-    minF_step = (Pf - Pi)/(nPs - 1.)
-    Ps = np.arange(Pi, Pf+1, minF_step)
+    minF_step = (Pf - Pi) / (nPs - 1.)
+    Ps = np.arange(Pi, Pf + 1, minF_step)
 
     return Ps
 
-def load_doscar(filename_sufix: str, list_filetags: list = None) -> tuple[list,list,list]:
+
+def load_doscar(filename_sufix: str, list_filetags: list = None) -> tuple[list, list, list]:
     """
     Extract electronic density, energies and Fermi level as function of volume from DOSCAR's.
     :param filename_sufix: folder path.
     :type filename_sufix: str
     :param list_filetags: filename tags.
     :type list_filetags: list
     :return: E,N,Ef.
     :rtype: tuple[list,list,list]
     """
     if list_filetags is None:
-        list_filetags = ['-0.10', '-0.09','-0.08','-0.07','-0.06','-0.05','-0.04','-0.03',
-                         '-0.02','-0.01','-0.00','0.01','0.02','0.03','0.04','0.05','0.06',
-                         '0.07','0.08','0.09','0.10']
+        list_filetags = ['-0.10', '-0.09', '-0.08', '-0.07', '-0.06', '-0.05', '-0.04', '-0.03',
+                         '-0.02', '-0.01', '-0.00', '0.01', '0.02', '0.03', '0.04', '0.05', '0.06',
+                         '0.07', '0.08', '0.09', '0.10']
 
     list_filetags = [str(li) for li in list_filetags]
     E = []
     N = []
     Ef = []
     nat = 0
     for dosfile in list_filetags:
         countline = 0
         EN = []
 
-        filename = filename_sufix+dosfile
+        filename = filename_sufix + dosfile
         with open(filename) as infile:
-                for line in infile:
-                    if countline == 0:
-                        nat = float(line.split()[0])
-                    if countline == 5:
-                        Ef.append(float(line.split()[3]))
-                    if countline > 5:
-                        EN.append(line.split()[0:2])
+            for line in infile:
+                if countline == 0:
+                    nat = float(line.split()[0])
+                if countline == 5:
+                    Ef.append(float(line.split()[3]))
+                if countline > 5:
+                    EN.append(line.split()[0:2])
 
-                    countline +=1
+                countline += 1
         ENAl = np.array(EN)
         # print(dosfile, EN)
-        E.append([float(s) for s in list(ENAl[:,0])])
-        N.append([float(s)/nat for s in list(ENAl[:,1])])
+        E.append([float(s) for s in list(ENAl[:, 0])])
+        N.append([float(s) / nat for s in list(ENAl[:, 1])])
 
-    return E,N,Ef
+    return E, N, Ef
 
-def load_V_E(energy_dir_summary: str, energy_dir_contcar: str, units: str = 'eV/atom') -> tuple[np.ndarray,np.ndarray]:
+
+def load_V_E(energy_dir_summary: str, energy_dir_contcar: str, units: str = 'eV/atom') -> tuple[np.ndarray, np.ndarray]:
     """
     Loads Energy curve as function of volume from VASP outputs.
     :param energy_dir_summary: Summary file path.
     :type energy_dir_summary: str
     :param energy_dir_contcar: Atoms positions file path.
     :type energy_dir_contcar: str
     :param units: units.
     :type units: str
     :return: Energy as function of volume
     :rtype: tuple[np.ndarray,np.ndarray]
     """
-    with open(energy_dir_contcar,'r') as f_poscar:
+    with open(energy_dir_contcar, 'r') as f_poscar:
         f_poscar_lines = f_poscar.readlines()
         cell_poscar = f_poscar_lines[2:5]
 
         cell_lst = [c.split() for c in cell_poscar]
         diag_cell = [float(c[i]) for i, c in enumerate(cell_lst)]
 
         try:
             nat = sum([int(li) for li in np.fromstring(f_poscar_lines[5], dtype=int, sep=' ')])
-            1/nat
+            1 / nat
         except:
             nat = sum([int(li) for li in np.fromstring(f_poscar_lines[6], dtype=int, sep=' ')])
-            1/nat
+            1 / nat
     with open(energy_dir_summary) as f_summary:
         f_summary_lines = f_summary.readlines()
         f_summary_lines = list(dict.fromkeys(f_summary_lines))
         ds = []
         E = []
         for l in f_summary_lines:
             l_lst = l.split(' ')
             ds.append(float(l_lst[0]))
-            E.append(float(l_lst[3])/nat)
+            E.append(float(l_lst[3]) / nat)
 
     V = []
     for di in ds:
-        V.append(np.product(np.array(diag_cell)*(1+di))/nat)
+        V.append(np.product(np.array(diag_cell) * (1 + di)) / nat)
 
     uconvV, uconvE = None, None
-    if units=='J/mol':
-        uconvE=(0.160218e-18*6.02214e23)
-        uconvV=(1e-30*6.02e23)
-    elif units=='eV/atom':
-        uconvE,uconvV = 1,1
-    return np.array(V).T*uconvV, np.array(E).T*uconvE
+    if units == 'J/mol':
+        uconvE = (0.160218e-18 * 6.02214e23)
+        uconvV = (1e-30 * 6.02e23)
+    elif units == 'eV/atom':
+        uconvE, uconvV = 1, 1
+    return np.array(V).T * uconvV, np.array(E).T * uconvE
+
 
 def load_EM(filename_outcar_eps: str) -> np.ndarray:
     """
     Extract the stiffness tensor from the VASP output (OUTCAR for IBRION=6).
     :param filename_outcar_eps: file path.
     :type filename_outcar_eps: str
     :return: Stiffness tensor.
@@ -181,46 +193,48 @@
     EM = []
 
     with open(filename_outcar_eps) as f:
         lines = f.readlines()
         for i, line in enumerate(lines):
             if line.startswith('  SYMMETRIZED ELASTIC MODULI (kBar)'):
                 j = i + 3
-                data = lines[j:j+6]
+                data = lines[j:j + 6]
                 break
 
     for line in data:
         EM += [[float(x) for x in line.split()[1:]]]
     EM = np.array(EM)
 
     return EM
 
-def load_cell(filename_contcar: str) -> tuple[str,np.ndarray,np.ndarray]:
+
+def load_cell(filename_contcar: str) -> tuple[str, np.ndarray, np.ndarray]:
     """
     Extract crystal structure from file in VASP format (POSCAR or CONTCAR).
     :param filename_contcar: File path
     :type filename_contcar: str
     :return: formula,, cell, and basis.
     :rtype: tuple[str,np.ndarray,np.ndarray]
     """
     with open(filename_contcar) as f:
-        poscar_lines=f.readlines()
+        poscar_lines = f.readlines()
     mult = float(poscar_lines[1])
-    cell = np.array([np.fromstring(line_i, dtype=float,sep=' ') for line_i in poscar_lines[2:5]])
-    cell = cell*mult
+    cell = np.array([np.fromstring(line_i, dtype=float, sep=' ') for line_i in poscar_lines[2:5]])
+    cell = cell * mult
 
-    ix_nats=6
+    ix_nats = 6
     re.findall('[A-Z][^A-Z]*', 'ABC')
-    ats_types = re.findall('[A-Z][^A-Z]*', poscar_lines[ix_nats-1].replace('  ','').replace(' ','').replace('\n',''))
-    ats_types = [ai+'x' for ai in ats_types]
-    nats = np.fromstring(poscar_lines[ix_nats], dtype=int,sep=' ')
-
-    formula_lst=[]
-    for at_i, na_i in zip(ats_types,nats):
-        formula_lst.append(at_i*na_i)
-    formula=''.join(formula_lst)
-    tots_nats=sum(nats)
+    ats_types = re.findall('[A-Z][^A-Z]*',
+                           poscar_lines[ix_nats - 1].replace('  ', '').replace(' ', '').replace('\n', ''))
+    ats_types = [ai + 'x' for ai in ats_types]
+    nats = np.fromstring(poscar_lines[ix_nats], dtype=int, sep=' ')
+
+    formula_lst = []
+    for at_i, na_i in zip(ats_types, nats):
+        formula_lst.append(at_i * na_i)
+    formula = ''.join(formula_lst)
+    tots_nats = sum(nats)
 
-    basis = np.array([np.fromstring(line_i, dtype=float,sep=' ') for line_i in poscar_lines[8:8+tots_nats]])
+    basis = np.array([np.fromstring(line_i, dtype=float, sep=' ') for line_i in poscar_lines[8:8 + tots_nats]])
     # basis = np.dot(basis,cell)
 
     return formula.replace('x', ''), cell, basis
```

### Comparing `debyetools-2.0.54/debyetools/debfunct.py` & `debyetools-2.0.6/debyetools/debfunct.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/defects.py` & `debyetools-2.0.6/debyetools/defects.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/electronic.py` & `debyetools-2.0.6/debyetools/electronic.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/CONTCAR.5` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/CONTCAR.5`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.00` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.00`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.01` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.02` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.03` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.04` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.05` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.06` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.07` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.08` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.09` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.10` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.-0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.01` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.02` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.03` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.04` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.05` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.06` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.07` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.08` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.09` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.10` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/DOSCAR.EvV.0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/OUTCAR.eps` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/OUTCAR.eps`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Ag_fcc/SUMMARY.fcc` & `debyetools-2.0.6/debyetools/examples/Ag_fcc/SUMMARY.fcc`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/CONTCAR.5` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/CONTCAR.5`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.00` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.00`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.01` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.02` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.03` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.04` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.05` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.06` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.07` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.08` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.09` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.10` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.-0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.01` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.02` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.03` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.04` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.05` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.06` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.07` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.08` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.09` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.10` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/DOSCAR.EvV.0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/OUTCAR.eps` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/OUTCAR.eps`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D022/SUMMARY.fcc` & `debyetools-2.0.6/debyetools/examples/Al3Li_D022/SUMMARY.fcc`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/CONTCAR.5` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/CONTCAR.5`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.00` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.00`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.01` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.02` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.03` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.04` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.05` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.06` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.07` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.08` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.09` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.10` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.-0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.01` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.02` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.03` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.04` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.05` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.06` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.07` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.08` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.09` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.10` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/DOSCAR.EvV.0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/OUTCAR.eps` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/OUTCAR.eps`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_D023/SUMMARY.fcc` & `debyetools-2.0.6/debyetools/examples/Al3Li_D023/SUMMARY.fcc`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/CONTCAR.5` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/CONTCAR.5`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.00` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.00`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.01` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.02` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.03` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.04` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.05` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.06` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.07` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.08` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.09` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.10` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.-0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.01` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.02` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.03` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.04` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.05` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.06` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.07` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.08` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.09` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.10` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/DOSCAR.EvV.0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/OUTCAR.eps` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/OUTCAR.eps`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al3Li_L12/SUMMARY.fcc` & `debyetools-2.0.6/debyetools/examples/Al3Li_L12/SUMMARY.fcc`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/CONTCAR.5` & `debyetools-2.0.6/debyetools/examples/Al_fcc/CONTCAR.5`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.00` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.00`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.01` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.02` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.03` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.04` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.05` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.06` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.07` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.08` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.09` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.10` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.-0.10`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.01` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.01`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.02` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.02`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.03` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.03`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.04` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.04`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.05` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.05`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.06` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.06`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.07` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.07`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.08` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.08`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.09` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.09`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/DOSCAR.EvV.0.1` & `debyetools-2.0.6/debyetools/examples/Al_fcc/DOSCAR.EvV.0.1`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/OUTCAR.eps` & `debyetools-2.0.6/debyetools/examples/Al_fcc/OUTCAR.eps`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/examples/Al_fcc/SUMMARY.fcc` & `debyetools-2.0.6/debyetools/examples/Al_fcc/SUMMARY.fcc`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/fs_compound_db.py` & `debyetools-2.0.6/debyetools/fs_compound_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import numpy as np
 from scipy.optimize import curve_fit
 
-Cp2fit = lambda T, P0, P1, P2, P3: P0*T**0 + P1*T**1 + P2*T**(-2) + P3*T**2# + P4*T**(-.5) + P5*T**(-3)
+Cp2fit = lambda T, P0, P1, P2, P3, P4, P5: P0*T**0 + P1*T**1 + P2*T**(-2) + P3*T**2 + P4*T**(-.5) + P5*T**(-3)
 alpha2fit = lambda T, Q0, Q1, Q2, Q3: Q0*T**0 + Q1*T**1 + Q2*T**(-1) + Q3*T**(-2)
 Ksinv2fit = lambda T, R0, R1, R2, R3: R0*T**0 + R1*T**1 + R2*T**2 + R3*T**3
 Ksp2fit = lambda T, S0, S1: S0 + S1*(T-298.15)*np.log(T/298.15)
 
 def fit_FS(tprops: dict, T_from: float, T_to: float) -> dict:
     """
     Procedure for the fitting of FS compound database parametes to thermodynamic properties.
```

### Comparing `debyetools-2.0.54/debyetools/ndeb.py` & `debyetools-2.0.6/debyetools/ndeb.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/pairanalysis.py` & `debyetools-2.0.6/debyetools/pairanalysis.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/poisson.py` & `debyetools-2.0.6/debyetools/poisson.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/potentials.py` & `debyetools-2.0.6/debyetools/potentials.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/atomtools.py` & `debyetools-2.0.6/debyetools/tpropsgui/atomtools.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/dialog_doscar.py` & `debyetools-2.0.6/debyetools/tpropsgui/dialog_doscar.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/dialog_outcar.py` & `debyetools-2.0.6/debyetools/tpropsgui/dialog_outcar.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/dialog_summary.py` & `debyetools-2.0.6/debyetools/tpropsgui/dialog_summary.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/elements.py` & `debyetools-2.0.6/debyetools/tpropsgui/elements.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/events.py` & `debyetools-2.0.6/debyetools/tpropsgui/events.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/functions0.py` & `debyetools-2.0.6/debyetools/tpropsgui/functions0.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/get_functions.py` & `debyetools-2.0.6/debyetools/tpropsgui/get_functions.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/gui.py` & `debyetools-2.0.6/debyetools/tpropsgui/gui.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/keygen.py` & `debyetools-2.0.6/debyetools/tpropsgui/keygen.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/layout.py` & `debyetools-2.0.6/debyetools/tpropsgui/layout.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/lock.py` & `debyetools-2.0.6/debyetools/tpropsgui/lock.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/mainwindow.py` & `debyetools-2.0.6/debyetools/tpropsgui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/plot_EV.py` & `debyetools-2.0.6/debyetools/tpropsgui/plot_EV.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/plotter.py` & `debyetools-2.0.6/debyetools/tpropsgui/plotter.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/plotter_class.py` & `debyetools-2.0.6/debyetools/tpropsgui/plotter_class.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/toolbox.py` & `debyetools-2.0.6/debyetools/tpropsgui/toolbox.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/ui_dialogSUMMARY.py` & `debyetools-2.0.6/debyetools/tpropsgui/ui_dialogSUMMARY.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/ui_dialog_doscar.py` & `debyetools-2.0.6/debyetools/tpropsgui/ui_dialog_doscar.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/ui_dialog_outcar.py` & `debyetools-2.0.6/debyetools/tpropsgui/ui_dialog_outcar.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/ui_heatcapacitywindow.py` & `debyetools-2.0.6/debyetools/tpropsgui/ui_heatcapacitywindow.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/ui_interatomic_params.py` & `debyetools-2.0.6/debyetools/tpropsgui/ui_interatomic_params.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/ui_mainwindow.py` & `debyetools-2.0.6/debyetools/tpropsgui/ui_mainwindow.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/ui_missingkey.py` & `debyetools-2.0.6/debyetools/tpropsgui/ui_missingkey.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/ui_warning.py` & `debyetools-2.0.6/debyetools/tpropsgui/ui_warning.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/window_cp.py` & `debyetools-2.0.6/debyetools/tpropsgui/window_cp.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/tpropsgui/window_interatomicparams.py` & `debyetools-2.0.6/debyetools/tpropsgui/window_interatomicparams.py`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/debyetools/vibrational.py` & `debyetools-2.0.6/debyetools/vibrational.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,19 +85,15 @@
         elif mode == 'jjfv':
             self.V0_DM = 1
             self.b_DM = 0
             self.a_DM = 0
             self.lam = 1
 
         else:
-            hola
-            self.V0_DM = ''
-            self.b_DM = ''
-            self.a_DM = ''
-            self.lam = -1
+            raise Exception('This is an error message')
 
     def set_int_anh(self, T: float, V: float) -> None:
         """
         Calculates intrinsic anharmonicity correction to the Debye temperature and its derivatives.
 
         :param float T: Temperature.
         :param float V: Volume.
```

### Comparing `debyetools-2.0.54/debyetools.egg-info/PKG-INFO` & `debyetools-2.0.6/debyetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debyetools
-Version: 2.0.54
+Version: 2.0.6
 Summary: Debye approximation implementation for the calculation of thermodynamic properties from ground-state atomistic simulations.
 Home-page: https://debyetools.readthedocs.io/
 Author: Javier Jofre
 Author-email: javier.jofre@polymtl.ca
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `debyetools-2.0.54/debyetools.egg-info/SOURCES.txt` & `debyetools-2.0.6/debyetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `debyetools-2.0.54/setup.py` & `debyetools-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="debyetools",
-    version="2.0.54",
+    version="2.0.6",
     description="Debye approximation implementation for the calculation of thermodynamic properties from ground-state atomistic simulations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://debyetools.readthedocs.io/",
     author="Javier Jofre",
     author_email="javier.jofre@polymtl.ca",
     license="GPLv3",
```

