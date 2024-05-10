# Comparing `tmp/redshift_data_api-1.2.4.tar.gz` & `tmp/redshift_data_api-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redshift_data_api-1.2.4.tar", max compression
+gzip compressed data, was "redshift_data_api-1.2.5.tar", max compression
```

## Comparing `redshift_data_api-1.2.4.tar` & `redshift_data_api-1.2.5.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      547 2024-02-14 16:41:09.071731 redshift_data_api-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     4182 2024-02-14 16:39:59.163560 redshift_data_api-1.2.4/redshift_data_api/__init__.py
--rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 redshift_data_api-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0      730 2024-05-10 18:54:42.008725 redshift_data_api-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     4182 2024-02-14 16:40:30.395888 redshift_data_api-1.2.5/redshift_data_api/__init__.py
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 redshift_data_api-1.2.5/PKG-INFO
```

### Comparing `redshift_data_api-1.2.4/redshift_data_api/__init__.py` & `redshift_data_api-1.2.5/redshift_data_api/__init__.py`

 * *Files identical despite different names*

