# Comparing `tmp/pyinstaller_hooks_contrib-2024.5.tar.gz` & `tmp/pyinstaller_hooks_contrib-2024.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinstaller_hooks_contrib-2024.5.tar", last modified: Tue Apr 23 20:51:25 2024, max compression
+gzip compressed data, was "pyinstaller_hooks_contrib-2024.6.tar", last modified: Fri May 10 14:23:44 2024, max compression
```

## Comparing `pyinstaller_hooks_contrib-2024.5.tar` & `pyinstaller_hooks_contrib-2024.6.tar`

### file list

```diff
@@ -1,492 +1,493 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:25.040809 pyinstaller_hooks_contrib-2024.5/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/LICENSE.APL.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/LICENSE.GPL.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-04-23 20:51:25.040809 pyinstaller_hooks_contrib-2024.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15157 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-23 20:51:25.040809 pyinstaller_hooks_contrib-2024.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:24.944807 pyinstaller_hooks_contrib-2024.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:24.944807 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:24.944807 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:24.944807 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/pre_find_module_path/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/pre_find_module_path/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:24.948807 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-win32com.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:24.948807 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_cryptography_openssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_enchant.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_ffpyplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_nltk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_osgeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pygraphviz.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyproj.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyqtgraph_multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pythoncom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pywintypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_traitlets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_usb.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:25.032808 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-BTrees.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-CTkMessagebox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Cryptodome.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-HtmlTestRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-IPython.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL_accelerate.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-PyTaskbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Xlib.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-_mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-accessible_output2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adbutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adios.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-afmformats.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-aliyunsdkcore.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-altair.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-amazonproduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appdirs.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appy.pod.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-apscheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-argon2.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy_iers_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-av.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-avro.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-azurerm.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-backports.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-backports.zoneinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bacon.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bcrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bitsandbytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bleak.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-blspy.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bokeh.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-botocore.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-branca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairocffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairosvg.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cassandra.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-celpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-certifi.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cf_units.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cftime.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-charset_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cloudpickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cloudscraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-compliance_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countrycode.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countryinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cryptography.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-customtkinter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cx_Oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cytoolz.itertoolz.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_bootstrap_components.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_core_components.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_html_components.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dask.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dateparser.utils.strptime.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dclab.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-detectron2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-discid.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-distorm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dns.rdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx2pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dynaconf.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-easyocr.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enchant.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eng_to_ipa.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ens.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enzyme.parsers.ebml.core.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_keyfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_rlp.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_utils.network.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-exchangelib.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fairscale.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-faker.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fastai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fastparquet.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ffpyplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fiona.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_restx.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flex.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flirpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fmpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-folium.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-freetype.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fvcore.nn.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gadfly.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-geopandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gmplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gmsh.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gooey.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.api_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.core.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.kms_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.pubsub_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.speech.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.translate.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-googleapiclient.model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      684 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-graphql_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-great_expectations.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gst._gst.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gtk.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-h5py.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hdf5plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hexbytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-httplib2.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-humanize.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hydra.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ijson.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio_ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-iminuit.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-iso639.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jaraco.text.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jedi.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jinja2.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jinxed.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jira.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonpath_rw_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonrpcserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema_specifications.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jupyterlab.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kaleido.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-khmernltk.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kinterbasdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langdetect.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-laonlp.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lark.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ldfparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lensfunpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-libaudioverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-librosa.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-limits.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lingua.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-litestar.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-llvmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-logilab.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.etree.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.isoschematron.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.objectify.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lz4.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-magic.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mako.codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mariadb.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mecab.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-metpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mimesis.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-minecraft_launcher_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mistune.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mnemonic.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.audio.fx.all.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.video.fx.all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mpl_toolkits.basemap.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-msoffcrypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nacl.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-names.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nanite.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbconvert.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbdime.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbformat.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbt.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ncclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-netCDF4.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nltk.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nnpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numba.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numcodecs.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cublas.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_cupti.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_nvcc.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_nvrtc.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cudnn.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cufft.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.curand.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cusolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cusparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.nccl.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.nvjitlink.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.nvtx.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-office365.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-opencc.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-openpyxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-opentelemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-orjson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-osgeo.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pandas_flavor.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-panel.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parsedatetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parso.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-passlib.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-paste.exceptions.reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-patsy.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pdfminer.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pendulum.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-phonenumbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pingouin.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pint.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pinyin.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-platformdirs.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-plotly.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pptx.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-prettytable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psutil.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psychopy.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-publicsuffix2.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pubsub.core.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-puremagic.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-py.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycountry.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycparser.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycrfsuite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydivert.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-io.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods3.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-odsr.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xls.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsx.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsxw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods3.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_odsr.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xls.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsxw.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcelerate.Writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pygraphviz.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pygwalker.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylibmagic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylsl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymediainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymorphy3.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymssql.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pynput.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyodbc.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyopencl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1545 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypemicro.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyphen.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyppeteer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyproj.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypsexec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypylon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyqtgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyshark.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pysnmp.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pystray.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pythainlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pythoncom.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx3.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyviz_comms.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyvjoy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywintypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywt.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-qtmodern.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-radicale.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-raven.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rawpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rdflib.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-redmine.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-regex.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.lib.utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.pdfbase._fontdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-resampy.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rlp.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rpy2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rtree.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sacremoses.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-seedir.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-selenium.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sentry_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shapely.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shotgun_api3.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-simplemma.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.color.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.data.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.draw.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.future.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.io.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.measure.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.registration.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.restoration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.linear_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.pairwise.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1264 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skyfield.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sound_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sounddevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-soundfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spacy.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-speech_recognition.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spiceypy.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spnego.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-srsly.msgpack._packer.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sspilib.raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-statsmodels.tsa.statespace.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-stdnum.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-storm.database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sudachipy.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sunpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-swagger_spec_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sympy.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tableauhyperapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tcod.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-text_unidecode.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-textdistance.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.backends.numpy_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-timezonefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-timm.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tinycss2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torch.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchaudio.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchtext.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchvision.io.image.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchvision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-trimesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkthemes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkwidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tzdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-u1db.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-umap.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-unidecode.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uniseg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-usb.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvicorn.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvloop.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-vaderSentiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-vtkpython.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wavefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-weasyprint.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-web3.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webassets.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webrtcvad.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webview.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-win32com.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wordcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.activex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.xrc.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.dom.html.HTMLDocument.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.sax.saxexts.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xmldiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xsge_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xyzservices.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-z3c.rml.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zeep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zmq.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zoneinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:25.032808 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/utils/nvidia_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:25.036808 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:24.944807 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:25.036808 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/data/test_hydra/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/data/test_hydra/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:25.036808 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_boto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_enchant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_pycparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_deep_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)    53328 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_scikit_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_scikit_learn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-23 20:51:11.000000 pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_wx_lib_pubsub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:51:25.040809 pyinstaller_hooks_contrib-2024.5/src/pyinstaller_hooks_contrib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-04-23 20:51:24.000000 pyinstaller_hooks_contrib-2024.5/src/pyinstaller_hooks_contrib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30249 2024-04-23 20:51:24.000000 pyinstaller_hooks_contrib-2024.5/src/pyinstaller_hooks_contrib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:51:24.000000 pyinstaller_hooks_contrib-2024.5/src/pyinstaller_hooks_contrib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 20:51:24.000000 pyinstaller_hooks_contrib-2024.5/src/pyinstaller_hooks_contrib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:51:24.000000 pyinstaller_hooks_contrib-2024.5/src/pyinstaller_hooks_contrib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 20:51:24.000000 pyinstaller_hooks_contrib-2024.5/src/pyinstaller_hooks_contrib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 20:51:24.000000 pyinstaller_hooks_contrib-2024.5/src/pyinstaller_hooks_contrib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:44.009632 pyinstaller_hooks_contrib-2024.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/LICENSE.APL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/LICENSE.GPL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-05-10 14:23:44.009632 pyinstaller_hooks_contrib-2024.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15157 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-10 14:23:44.009632 pyinstaller_hooks_contrib-2024.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:43.929632 pyinstaller_hooks_contrib-2024.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:43.929632 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:43.929632 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:43.929632 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/pre_find_module_path/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/pre_find_module_path/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:43.929632 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-win32com.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:43.933632 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_cryptography_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_enchant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_ffpyplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_osgeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pygraphviz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyproj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyqtgraph_multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pythoncom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pywintypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_traitlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:44.005632 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-BTrees.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-CTkMessagebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Cryptodome.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-HtmlTestRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-IPython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL_accelerate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-PyTaskbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Xlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-_mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-accessible_output2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adbutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adios.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-afmformats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-aliyunsdkcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-altair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-amazonproduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appy.pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-apscheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-argon2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy_iers_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-av.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-avro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-azurerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-backports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-backports.zoneinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bcrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bitsandbytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bleak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-blspy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-botocore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-branca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairocffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairosvg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cassandra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-celpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-certifi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cf_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cftime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-charset_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cloudpickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cloudscraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-compliance_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countrycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countryinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cryptography.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-customtkinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cx_Oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cytoolz.itertoolz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_bootstrap_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_core_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_html_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dateparser.utils.strptime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dclab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-discid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-distorm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dns.rdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx2pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dynaconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-easyocr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enchant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eng_to_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enzyme.parsers.ebml.core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_keyfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_rlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_utils.network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-exchangelib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fairscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-faker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fastai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fastparquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ffpyplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fiona.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_restx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flirpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fmpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-folium.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-freetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fvcore.nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gadfly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gmplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gooey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.api_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.kms_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.pubsub_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.speech.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-googleapiclient.model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      684 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-graphql_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-great_expectations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gst._gst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gtk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-h5py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hdf5plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hexbytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-httplib2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-humanize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hydra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ijson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio_ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-iminuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-iso639.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jaraco.text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jedi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jinxed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonpath_rw_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonrpcserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema_specifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jupyterlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kaleido.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-khmernltk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kinterbasdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langdetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-laonlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ldfparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lensfunpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-libaudioverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-librosa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lingua.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-litestar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-llvmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-logilab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.etree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.isoschematron.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.objectify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lz4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mako.codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mariadb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mecab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-metpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mimesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-minecraft_launcher_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mistune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mnemonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.audio.fx.all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.video.fx.all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mpl_toolkits.basemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-msoffcrypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nanite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbconvert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbdime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ncclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-netCDF4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nltk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nnpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numcodecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cublas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_cupti.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_nvcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_nvrtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cudnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.curand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cusolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cusparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.nccl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.nvjitlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-office365.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-opencc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-openpyxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-opentelemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-orjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-osgeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pandas_flavor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parsedatetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parso.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-passlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-paste.exceptions.reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-patsy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pdfminer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-phonenumbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pingouin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pinyin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-platformdirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-plotly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pptx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-prettytable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psychopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psycopg2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-publicsuffix2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pubsub.core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-puremagic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycountry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycrfsuite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydivert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-odsr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsxw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_odsr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsxw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcelerate.Writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pygraphviz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pygwalker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylibmagic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymediainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymorphy3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pynput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyodbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyopencl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1545 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypemicro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyphen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyppeteer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyproj.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypsexec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypylon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyqtgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyshark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pysnmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pystray.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pythainlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pythoncom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyviz_comms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyvjoy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywintypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-qtmodern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-radicale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-raven.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rawpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rdflib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-redmine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.lib.utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.pdfbase._fontdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-resampy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rpy2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sacremoses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-schwifty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-seedir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-selenium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sentry_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shapely.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shotgun_api3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-simplemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.restoration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1264 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skyfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sound_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sounddevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-soundfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-speech_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spiceypy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spnego.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-srsly.msgpack._packer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sspilib.raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-statsmodels.tsa.statespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-stdnum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-storm.database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sudachipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sunpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-swagger_spec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sympy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tableauhyperapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tcod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-text_unidecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-textdistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.backends.numpy_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-timezonefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-timm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tinycss2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchaudio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchtext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchvision.io.image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-trimesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkthemes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkwidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tzdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-u1db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-umap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-unidecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uniseg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvicorn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-vaderSentiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-vtkpython.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wavefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-weasyprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-web3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webassets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webrtcvad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-win32com.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wordcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.activex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.xrc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.dom.html.HTMLDocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.sax.saxexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xmldiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xsge_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xyzservices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-z3c.rml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zeep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zoneinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:44.005632 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/utils/nvidia_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:44.005632 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:43.925632 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:44.005632 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/data/test_hydra/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/data/test_hydra/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:44.005632 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_boto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_enchant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_pycparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11391 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_deep_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53610 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_scikit_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_scikit_learn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-10 14:23:31.000000 pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_wx_lib_pubsub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:23:44.009632 pyinstaller_hooks_contrib-2024.6/src/pyinstaller_hooks_contrib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-05-10 14:23:43.000000 pyinstaller_hooks_contrib-2024.6/src/pyinstaller_hooks_contrib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30312 2024-05-10 14:23:43.000000 pyinstaller_hooks_contrib-2024.6/src/pyinstaller_hooks_contrib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:23:43.000000 pyinstaller_hooks_contrib-2024.6/src/pyinstaller_hooks_contrib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 14:23:43.000000 pyinstaller_hooks_contrib-2024.6/src/pyinstaller_hooks_contrib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:23:43.000000 pyinstaller_hooks_contrib-2024.6/src/pyinstaller_hooks_contrib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 14:23:43.000000 pyinstaller_hooks_contrib-2024.6/src/pyinstaller_hooks_contrib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 14:23:43.000000 pyinstaller_hooks_contrib-2024.6/src/pyinstaller_hooks_contrib.egg-info/top_level.txt
```

### Comparing `pyinstaller_hooks_contrib-2024.5/LICENSE` & `pyinstaller_hooks_contrib-2024.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/LICENSE.APL.txt` & `pyinstaller_hooks_contrib-2024.6/LICENSE.APL.txt`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/LICENSE.GPL.txt` & `pyinstaller_hooks_contrib-2024.6/LICENSE.GPL.txt`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/PKG-INFO` & `pyinstaller_hooks_contrib-2024.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinstaller-hooks-contrib
-Version: 2024.5
+Version: 2024.6
 Summary: Community maintained hooks for PyInstaller
 Home-page: https://github.com/pyinstaller/pyinstaller-hooks-contrib
 Download-URL: https://pypi.org/project/pyinstaller-hooks-contrib
 Maintainer: Legorooj
 Maintainer-email: legorooj@protonmail.com
 Keywords: pyinstaller development hooks
 Classifier: Intended Audience :: Developers
```

### Comparing `pyinstaller_hooks_contrib-2024.5/README.md` & `pyinstaller_hooks_contrib-2024.6/README.md`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/pyproject.toml` & `pyinstaller_hooks_contrib-2024.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/setup.cfg` & `pyinstaller_hooks_contrib-2024.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/setup.py` & `pyinstaller_hooks_contrib-2024.6/setup.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/__init__.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-io.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,10 +6,11 @@
 #
 # The full license is available in LICENSE.GPL.txt, distributed with
 # this software.
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 # ------------------------------------------------------------------
 
-__version__ = '2024.5'
-__maintainer__ = 'Legorooj, bwoodsend'
-__uri__ = 'https://github.com/pyinstaller/pyinstaller-hooks-contrib'
+# This hook was tested with pyexcel-io 0.5.18:
+# https://github.com/pyexcel/pyexcel-io
+
+hiddenimports = ['pyexcel_io']
```

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/compat.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/compat.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/__init__.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-tensorflow.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-tensorflow.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-win32com.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/pre_safe_import_module/hook-win32com.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_cryptography_openssl.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_cryptography_openssl.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_enchant.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_enchant.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_ffpyplayer.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_ffpyplayer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_nltk.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_nltk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_osgeo.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_osgeo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pygraphviz.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pygraphviz.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyproj.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyproj.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyqtgraph_multiprocess.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pyqtgraph_multiprocess.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pythoncom.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pythoncom.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pywintypes.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_pywintypes.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_tensorflow.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_tensorflow.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_traitlets.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_traitlets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_usb.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks/pyi_rth_usb.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/rthooks.dat` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/rthooks.dat`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-BTrees.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-BTrees.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-CTkMessagebox.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-CTkMessagebox.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Crypto.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Crypto.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Cryptodome.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Cryptodome.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-HtmlTestRunner.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-HtmlTestRunner.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-IPython.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-IPython.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL_accelerate.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-OpenGL_accelerate.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-PyTaskbar.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-PyTaskbar.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Xlib.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-Xlib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-_mysql.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-_mysql.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-accessible_output2.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-accessible_output2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adbutils.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adbutils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adios.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-adios.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-afmformats.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-afmformats.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-aliyunsdkcore.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-aliyunsdkcore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-altair.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-altair.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-amazonproduct.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-amazonproduct.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-anyio.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-anyio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appdirs.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appdirs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appy.pod.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-appy.pod.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-apscheduler.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-apscheduler.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astor.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astor.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astroid.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astroid.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy_iers_data.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-astropy_iers_data.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-av.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-av.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-avro.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-avro.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-azurerm.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-azurerm.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-backports.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-backports.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-backports.zoneinfo.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-backports.zoneinfo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bacon.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bacon.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bcrypt.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bcrypt.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bitsandbytes.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bitsandbytes.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bleak.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bleak.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-blspy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-blspy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bokeh.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-bokeh.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto3.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-boto3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-botocore.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-botocore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-branca.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-branca.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairocffi.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairocffi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairosvg.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cairosvg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cassandra.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cassandra.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-celpy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-celpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-certifi.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-certifi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cf_units.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cf_units.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cftime.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cftime.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-charset_normalizer.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-charset_normalizer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cloudpickle.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cloudpickle.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cloudscraper.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cloudscraper.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr_loader.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-clr_loader.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-compliance_checker.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-compliance_checker.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countrycode.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countrycode.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countryinfo.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-countryinfo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cryptography.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cryptography.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-customtkinter.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-customtkinter.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cv2.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cv2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cytoolz.itertoolz.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-cytoolz.itertoolz.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_bootstrap_components.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_bootstrap_components.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_core_components.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_core_components.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_html_components.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_html_components.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_renderer.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_renderer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_table.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_table.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_uploader.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dash_uploader.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dask.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dask.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-datasets.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-datasets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dateparser.utils.strptime.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dateparser.utils.strptime.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dclab.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dclab.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-detectron2.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-detectron2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-discid.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-discid.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-distorm3.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-distorm3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dns.rdata.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dns.rdata.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docutils.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docutils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx2pdf.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-docx2pdf.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dynaconf.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-dynaconf.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-easyocr.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-easyocr.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eel.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eel.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enchant.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enchant.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eng_to_ipa.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eng_to_ipa.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ens.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ens.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enzyme.parsers.ebml.core.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-enzyme.parsers.ebml.core.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_abi.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_abi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_account.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_account.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_hash.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_hash.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_keyfile.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_keyfile.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_keys.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_keys.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_rlp.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_rlp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_typing.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_typing.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_utils.network.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_utils.network.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_utils.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-eth_utils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fabric.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fabric.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fairscale.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fairscale.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-faker.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-faker.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-falcon.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-falcon.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fastai.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fastai.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fastparquet.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fastparquet.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ffpyplayer.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ffpyplayer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fiona.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fiona.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_compress.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_compress.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_restx.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flask_restx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flex.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flex.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flirpy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-flirpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fmpy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fmpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-folium.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-folium.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-freetype.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-freetype.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fvcore.nn.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-fvcore.nn.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gcloud.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gcloud.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-geopandas.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-geopandas.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gitlab.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gitlab.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gmplot.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gmplot.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gmsh.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gmsh.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gooey.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gooey.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.api_core.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.api_core.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.bigquery.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.bigquery.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.core.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.core.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.kms_v1.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.kms_v1.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.pubsub_v1.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.pubsub_v1.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.speech.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.speech.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.storage.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.storage.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.translate.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-google.cloud.translate.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-googleapiclient.model.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-googleapiclient.model.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-graphql_query.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-graphql_query.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-great_expectations.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-great_expectations.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-grpc.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-grpc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gst._gst.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gst._gst.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gtk.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-gtk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-h5py.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-h5py.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hdf5plugin.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hdf5plugin.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hexbytes.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hexbytes.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-httplib2.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-httplib2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-humanize.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-humanize.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hydra.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-hydra.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ijson.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ijson.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio_ffmpeg.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-imageio_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-iminuit.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-iminuit.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-iso639.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-iso639.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jaraco.text.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jaraco.text.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jedi.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jedi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jieba.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jieba.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jira.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jira.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonpath_rw_ext.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonpath_rw_ext.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonrpcserver.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonrpcserver.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema_specifications.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jsonschema_specifications.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jupyterlab.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-jupyterlab.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kaleido.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kaleido.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-khmernltk.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-khmernltk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kinterbasdb.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-kinterbasdb.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langchain.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langchain.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langcodes.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langcodes.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langdetect.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-langdetect.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-laonlp.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-laonlp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lark.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lark.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ldfparser.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ldfparser.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lensfunpy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lensfunpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-libaudioverse.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-libaudioverse.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-librosa.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-librosa.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lightgbm.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lightning.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lightning.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-limits.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-limits.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-linear_operator.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-linear_operator.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lingua.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lingua.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-litestar.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-litestar.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-llvmlite.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-llvmlite.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-logilab.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-logilab.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.isoschematron.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.isoschematron.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lxml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lz4.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-lz4.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-magic.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-magic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mako.codegen.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mako.codegen.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mariadb.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mariadb.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-markdown.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-markdown.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mecab.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mecab.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-metpy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-metpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-migrate.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-migrate.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mimesis.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mimesis.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-minecraft_launcher_lib.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-minecraft_launcher_lib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mistune.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mistune.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mnemonic.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mnemonic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.audio.fx.all.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.audio.fx.all.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.video.fx.all.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-moviepy.video.fx.all.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mpl_toolkits.basemap.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-mpl_toolkits.basemap.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-msoffcrypto.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-msoffcrypto.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nacl.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nacl.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-names.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-names.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nanite.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nanite.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbconvert.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbconvert.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbdime.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbdime.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbformat.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nbformat.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ncclient.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ncclient.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-netCDF4.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-netCDF4.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nltk.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nltk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-notebook.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-notebook.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numba.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numba.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numcodecs.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-numcodecs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cublas.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cublas.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_cupti.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_cupti.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_nvcc.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_nvcc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_nvrtc.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_nvrtc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_runtime.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cuda_runtime.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cudnn.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cudnn.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cufft.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cufft.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.curand.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.curand.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cusolver.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cusolver.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cusparse.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.cusparse.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.nccl.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.nccl.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.nvjitlink.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.nvjitlink.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.nvtx.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-nvidia.nvtx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-office365.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-office365.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-opencc.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-opencc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-openpyxl.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-openpyxl.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-opentelemetry.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-opentelemetry.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-orjson.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-orjson.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-osgeo.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-osgeo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pandas_flavor.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pandas_flavor.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-panel.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-panel.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parsedatetime.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parsedatetime.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parso.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-parso.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-passlib.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-passlib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-paste.exceptions.reporter.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-paste.exceptions.reporter.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pdfminer.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pdfminer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pendulum.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pendulum.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-phonenumbers.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-phonenumbers.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pingouin.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pingouin.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pint.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pint.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pinyin.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pinyin.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-platformdirs.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-platformdirs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-plotly.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-plotly.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pptx.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pptx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-prettytable.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-prettytable.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psutil.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psutil.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psychopy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-psychopy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-publicsuffix2.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-publicsuffix2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pubsub.core.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pubsub.core.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-puremagic.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-puremagic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-py.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-py.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyarrow.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyarrow.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycountry.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycountry.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycparser.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pycparser.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydantic.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydantic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydivert.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pydivert.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-io.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods3.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 #
 # The full license is available in LICENSE.GPL.txt, distributed with
 # this software.
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 # ------------------------------------------------------------------
 
-# This hook was tested with pyexcel-io 0.5.18:
-# https://github.com/pyexcel/pyexcel-io
+# This hook was tested with pyexcel-ods3 0.5.3:
+# https://github.com/pyexcel/pyexcel-ods3
 
-hiddenimports = ['pyexcel_io']
+hiddenimports = ['pyexcel_ods3']
```

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-ods3.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsx.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 #
 # The full license is available in LICENSE.GPL.txt, distributed with
 # this software.
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 # ------------------------------------------------------------------
 
-# This hook was tested with pyexcel-ods3 0.5.3:
-# https://github.com/pyexcel/pyexcel-ods3
+# This hook was tested with pyexcel-xlsx 0.4.2:
+# https://github.com/pyexcel/pyexcel-xlsx
 
-hiddenimports = ['pyexcel_ods3']
+hiddenimports = ['pyexcel_xlsx']
```

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-odsr.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-odsr.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xls.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xls.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsx.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-timm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # ------------------------------------------------------------------
-# Copyright (c) 2020 PyInstaller Development Team.
+# Copyright (c) 2023 PyInstaller Development Team.
 #
 # This file is distributed under the terms of the GNU General Public
 # License (version 2.0 or later).
 #
 # The full license is available in LICENSE.GPL.txt, distributed with
 # this software.
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 # ------------------------------------------------------------------
 
-# This hook was tested with pyexcel-xlsx 0.4.2:
-# https://github.com/pyexcel/pyexcel-xlsx
-
-hiddenimports = ['pyexcel_xlsx']
+# Collect source .py files for JIT/torchscript. Requires PyInstaller >= 5.3, no-op in older versions.
+module_collection_mode = 'pyz+py'
```

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsxw.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel-xlsxw.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_io.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_io.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods3.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_ods3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_odsr.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_odsr.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xls.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xls.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsx.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsxw.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcel_xlsxw.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcelerate.Writer.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyexcelerate.Writer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pygraphviz.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pygraphviz.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pygwalker.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pygwalker.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylibmagic.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylibmagic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylint.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylint.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylsl.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pylsl.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymediainfo.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymediainfo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymorphy3.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymorphy3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymssql.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pymssql.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pynput.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pynput.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyodbc.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyodbc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyopencl.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyopencl.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypemicro.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypemicro.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyphen.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyphen.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyppeteer.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyppeteer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyproj.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyproj.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypsexec.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypsexec.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypylon.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pypylon.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyqtgraph.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyshark.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyshark.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pysnmp.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pysnmp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pystray.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pystray.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pytest.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pytest.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pythainlp.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pythainlp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pythoncom.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pythoncom.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx3.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyttsx3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyviz_comms.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyviz_comms.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyvjoy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pyvjoy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywintypes.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywintypes.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywt.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-pywt.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-qtmodern.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-qtmodern.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-radicale.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-radicale.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rawpy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rawpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rdflib.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rdflib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.pdfbase._fontdata.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.pdfbase._fontdata.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-resampy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-resampy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rlp.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rlp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rpy2.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rpy2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rtree.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rtree.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sacremoses.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sacremoses.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-seedir.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-seedir.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-selenium.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-selenium.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sentry_sdk.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sentry_sdk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shapely.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shapely.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shotgun_api3.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shotgun_api3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-simplemma.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-simplemma.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.color.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.color.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.data.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.data.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.draw.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.draw.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.exposure.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.exposure.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.feature.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.feature.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.filters.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.filters.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.future.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.future.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.graph.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.graph.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.io.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.io.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.measure.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.measure.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.metrics.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.metrics.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.morphology.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.morphology.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.registration.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.registration.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.restoration.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.restoration.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.transform.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.transform.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.cluster.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.cluster.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.linear_model.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.linear_model.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.cluster.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.cluster.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.pairwise.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.pairwise.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.metrics.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.neighbors.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.neighbors.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sklearn.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skyfield.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skyfield.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sound_lib.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sound_lib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sounddevice.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sounddevice.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-soundfile.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-soundfile.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spacy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spacy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-speech_recognition.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spiceypy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spiceypy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spnego.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-spnego.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-srsly.msgpack._packer.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-srsly.msgpack._packer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sspilib.raw.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sspilib.raw.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-statsmodels.tsa.statespace.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-statsmodels.tsa.statespace.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-stdnum.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-stdnum.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-storm.database.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-storm.database.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sudachipy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sudachipy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sunpy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sunpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-swagger_spec_validator.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-swagger_spec_validator.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sympy.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sympy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tableauhyperapi.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tableauhyperapi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tables.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tables.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tcod.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tcod.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tensorflow.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tensorflow.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-text_unidecode.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-text_unidecode.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-textdistance.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-textdistance.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.backends.numpy_ops.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.backends.numpy_ops.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-thinc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-timezonefinder.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-timezonefinder.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-timm.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-websockets.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # ------------------------------------------------------------------
-# Copyright (c) 2023 PyInstaller Development Team.
+# Copyright (c) 2021 PyInstaller Development Team.
 #
 # This file is distributed under the terms of the GNU General Public
 # License (version 2.0 or later).
 #
 # The full license is available in LICENSE.GPL.txt, distributed with
 # this software.
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 # ------------------------------------------------------------------
 
-# Collect source .py files for JIT/torchscript. Requires PyInstaller >= 5.3, no-op in older versions.
-module_collection_mode = 'pyz+py'
+from PyInstaller.utils.hooks import collect_submodules
+
+# Websockets lazily loads its submodules.
+hiddenimports = collect_submodules("websockets")
```

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tinycss2.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tinycss2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torch.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torch.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchaudio.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchaudio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchtext.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchtext.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchvision.io.image.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchvision.io.image.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchvision.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-torchvision.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-transformers.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-transformers.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-trimesh.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-trimesh.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-triton.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-triton.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkthemes.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkthemes.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkwidgets.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-ttkwidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tzdata.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-tzdata.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-u1db.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-u1db.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-umap.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-umap.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-unidecode.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-unidecode.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uniseg.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uniseg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-usb.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-usb.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvicorn.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvicorn.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvloop.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-uvloop.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-vaderSentiment.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-vaderSentiment.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-vtkpython.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-vtkpython.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wavefile.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wavefile.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-weasyprint.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-weasyprint.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webassets.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webassets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webrtcvad.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webrtcvad.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-websockets.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # ------------------------------------------------------------------
-# Copyright (c) 2021 PyInstaller Development Team.
+# Copyright (c) 2020 PyInstaller Development Team.
 #
 # This file is distributed under the terms of the GNU General Public
 # License (version 2.0 or later).
 #
 # The full license is available in LICENSE.GPL.txt, distributed with
 # this software.
 #
 # SPDX-License-Identifier: GPL-2.0-or-later
 # ------------------------------------------------------------------
-
-from PyInstaller.utils.hooks import collect_submodules
-
-# Websockets lazily loads its submodules.
-hiddenimports = collect_submodules("websockets")
+# Import all fixtures from PyInstaller into the tests.
+from PyInstaller.utils.conftest import *  # noqa: F401,F403
```

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webview.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-webview.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-win32com.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-win32com.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wordcloud.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wordcloud.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-workflow.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-workflow.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.activex.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.activex.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.pubsub.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-wx.lib.pubsub.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xarray.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xarray.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.dom.html.HTMLDocument.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.dom.html.HTMLDocument.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.sax.saxexts.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xml.sax.saxexts.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xmldiff.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xmldiff.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xsge_gui.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xsge_gui.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xyzservices.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-xyzservices.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-z3c.rml.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-z3c.rml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zeep.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zeep.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zmq.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zmq.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zoneinfo.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-zoneinfo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/hooks/utils/nvidia_cuda.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/hooks/utils/nvidia_cuda.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/__init__.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_boto.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_boto.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_enchant.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_enchant.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_pycparser.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_pycparser.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_layer.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_layer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_mnist.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/scripts/pyi_lib_tensorflow_mnist.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_deep_learning.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_deep_learning.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_libraries.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_libraries.py`

 * *Files 1% similar despite different names*

```diff
@@ -2020,7 +2020,19 @@
         # `tables` uses cpu_info package during initialization, which in turn uses `multiprocessing`, so we need to call
         # `multiprocessing.freeze_support()` before importing `tables`.
         import multiprocessing
         multiprocessing.freeze_support()
 
         import tables
     """, run_from_path=True)
+
+
+@importorskip('schwifty')
+def test_schwifty(pyi_builder):
+    pyi_builder.test_source("""
+        import schwifty
+
+        iban = schwifty.IBAN('DE89 3704 0044 0532 0130 00')
+        print(iban.country_code)
+        print(iban.bank_code)
+        print(iban.account_code)
+    """)
```

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_pytorch.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_scikit_image.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_scikit_image.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_scikit_learn.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_scikit_learn.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_tensorflow.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/_pyinstaller_hooks_contrib/tests/test_wx_lib_pubsub.py` & `pyinstaller_hooks_contrib-2024.6/src/_pyinstaller_hooks_contrib/tests/test_wx_lib_pubsub.py`

 * *Files identical despite different names*

### Comparing `pyinstaller_hooks_contrib-2024.5/src/pyinstaller_hooks_contrib.egg-info/PKG-INFO` & `pyinstaller_hooks_contrib-2024.6/src/pyinstaller_hooks_contrib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinstaller-hooks-contrib
-Version: 2024.5
+Version: 2024.6
 Summary: Community maintained hooks for PyInstaller
 Home-page: https://github.com/pyinstaller/pyinstaller-hooks-contrib
 Download-URL: https://pypi.org/project/pyinstaller-hooks-contrib
 Maintainer: Legorooj
 Maintainer-email: legorooj@protonmail.com
 Keywords: pyinstaller development hooks
 Classifier: Intended Audience :: Developers
```

### Comparing `pyinstaller_hooks_contrib-2024.5/src/pyinstaller_hooks_contrib.egg-info/SOURCES.txt` & `pyinstaller_hooks_contrib-2024.6/src/pyinstaller_hooks_contrib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -345,14 +345,15 @@
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.lib.utils.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-reportlab.pdfbase._fontdata.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-resampy.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rlp.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rpy2.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-rtree.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sacremoses.py
+src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-schwifty.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-seedir.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-selenium.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-sentry_sdk.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shapely.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-shotgun_api3.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-simplemma.py
 src/_pyinstaller_hooks_contrib/hooks/stdhooks/hook-skimage.color.py
```

