# Comparing `tmp/geneea-nlp-client-1.4.4.tar.gz` & `tmp/geneea-nlp-client-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneea-nlp-client-1.4.4.tar", last modified: Fri May  3 08:50:28 2024, max compression
+gzip compressed data, was "geneea-nlp-client-1.5.0.tar", last modified: Fri May 10 09:34:46 2024, max compression
```

## Comparing `geneea-nlp-client-1.4.4.tar` & `geneea-nlp-client-1.5.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.077193 geneea-nlp-client-1.4.4/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.077193 geneea-nlp-client-1.4.4/examples/g3/
--rw-rw-rw-   0 root         (0) root         (0)        2 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2392 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/entitiesToExcel.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/languageToExcel.py
--rw-rw-rw-   0 root         (0) root         (0)     1485 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/quickStart.py
--rw-rw-rw-   0 root         (0) root         (0)     2890 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/quickStartAll.py
--rw-rw-rw-   0 root         (0) root         (0)     2034 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/quickStartEntities.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/relationsToExcel.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/examples/g3/sentimentToExcel.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.077193 geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-03 08:50:27.000000 geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1570 2024-05-03 08:50:27.000000 geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-03 08:50:27.000000 geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-03 08:50:27.000000 geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-03 08:50:27.000000 geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.077193 geneea-nlp-client-1.4.4/geneeanlpclient/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.077193 geneea-nlp-client-1.4.4/geneeanlpclient/common/
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/common/common.py
--rw-rw-rw-   0 root         (0) root         (0)     3734 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/common/dictutil.py
--rw-rw-rw-   0 root         (0) root         (0)     2809 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/common/restutil.py
--rw-rw-rw-   0 root         (0) root         (0)     5410 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/common/ud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/geneeanlpclient/g3/
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2952 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/client.py
--rw-rw-rw-   0 root         (0) root         (0)    29568 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/f2converter.py
--rw-rw-rw-   0 root         (0) root         (0)    54885 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/model.py
--rw-rw-rw-   0 root         (0) root         (0)    15903 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/reader.py
--rw-rw-rw-   0 root         (0) root         (0)    18574 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/request.py
--rw-rw-rw-   0 root         (0) root         (0)     7541 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/geneeanlpclient/g3/writer.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1481 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/tests/geneeanlpclient/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2743 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/test_common.py
--rw-rw-rw-   0 root         (0) root         (0)     4103 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/test_jsonutil.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/test_ud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-03 08:50:28.081193 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/examples.py
--rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/generate.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_charSpan.py
--rw-rw-rw-   0 root         (0) root         (0)     5186 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_f2converter.py
--rw-rw-rw-   0 root         (0) root         (0)     2839 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     9166 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_rw.py
--rw-rw-rw-   0 root         (0) root         (0)     3674 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_tokenSupport.py
--rw-rw-rw-   0 root         (0) root         (0)     5342 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_tokenutils.py
--rw-rw-rw-   0 root         (0) root         (0)     5447 2024-05-03 08:50:17.000000 geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_treeBuilder.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.902675 geneea-nlp-client-1.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-10 09:34:46.902675 geneea-nlp-client-1.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      502 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.882675 geneea-nlp-client-1.5.0/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.886675 geneea-nlp-client-1.5.0/examples/g3/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/entitiesToExcel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/languageToExcel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1485 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/quickStart.py
+-rw-rw-rw-   0 root         (0) root         (0)     2890 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/quickStartAll.py
+-rw-rw-rw-   0 root         (0) root         (0)     2034 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/quickStartEntities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/relationsToExcel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/examples/g3/sentimentToExcel.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.886675 geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-05-10 09:34:46.000000 geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2024-05-10 09:34:46.000000 geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-10 09:34:46.000000 geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-10 09:34:46.000000 geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-05-10 09:34:46.000000 geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.886675 geneea-nlp-client-1.5.0/geneeanlpclient/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.890675 geneea-nlp-client-1.5.0/geneeanlpclient/common/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/common/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     3734 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/common/dictutil.py
+-rw-rw-rw-   0 root         (0) root         (0)     2809 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/common/restutil.py
+-rw-rw-rw-   0 root         (0) root         (0)     5410 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/common/ud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.894675 geneea-nlp-client-1.5.0/geneeanlpclient/g3/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/client.py
+-rw-rw-rw-   0 root         (0) root         (0)    29568 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/f2converter.py
+-rw-rw-rw-   0 root         (0) root         (0)    57073 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/model.py
+-rw-rw-rw-   0 root         (0) root         (0)    16707 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)    18574 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     8244 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/geneeanlpclient/g3/writer.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-10 09:34:46.902675 geneea-nlp-client-1.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.894675 geneea-nlp-client-1.5.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.894675 geneea-nlp-client-1.5.0/tests/geneeanlpclient/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.898675 geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2743 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/test_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     4103 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/test_jsonutil.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/test_ud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 09:34:46.902675 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/generate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_charSpan.py
+-rw-rw-rw-   0 root         (0) root         (0)     5186 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_f2converter.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     9172 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_rw.py
+-rw-rw-rw-   0 root         (0) root         (0)     3674 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_tokenSupport.py
+-rw-rw-rw-   0 root         (0) root         (0)     5342 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_tokenutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5447 2024-05-10 09:34:35.000000 geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_treeBuilder.py
```

### Comparing `geneea-nlp-client-1.4.4/LICENSE` & `geneea-nlp-client-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/PKG-INFO` & `geneea-nlp-client-1.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneea-nlp-client
-Version: 1.4.4
+Version: 1.5.0
 Summary: The SDK library and command-line interface to Geneea Interpretor, an NLP REST API.
 Home-page: https://geneea.com
 Author: Geneea Analytics s.r.o
 Author-email: support@geneea.com
 License: UNKNOWN
 Project-URL: Documentation, https://help.geneea.com/sdk/index.html
 Project-URL: Source Code, https://bitbucket.org/geneea/sdk
```

### Comparing `geneea-nlp-client-1.4.4/examples/g3/entitiesToExcel.py` & `geneea-nlp-client-1.5.0/examples/g3/entitiesToExcel.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/examples/g3/languageToExcel.py` & `geneea-nlp-client-1.5.0/examples/g3/languageToExcel.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/examples/g3/quickStart.py` & `geneea-nlp-client-1.5.0/examples/g3/quickStart.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/examples/g3/quickStartAll.py` & `geneea-nlp-client-1.5.0/examples/g3/quickStartAll.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/examples/g3/quickStartEntities.py` & `geneea-nlp-client-1.5.0/examples/g3/quickStartEntities.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/examples/g3/relationsToExcel.py` & `geneea-nlp-client-1.5.0/examples/g3/relationsToExcel.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/examples/g3/sentimentToExcel.py` & `geneea-nlp-client-1.5.0/examples/g3/sentimentToExcel.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/PKG-INFO` & `geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneea-nlp-client
-Version: 1.4.4
+Version: 1.5.0
 Summary: The SDK library and command-line interface to Geneea Interpretor, an NLP REST API.
 Home-page: https://geneea.com
 Author: Geneea Analytics s.r.o
 Author-email: support@geneea.com
 License: UNKNOWN
 Project-URL: Documentation, https://help.geneea.com/sdk/index.html
 Project-URL: Source Code, https://bitbucket.org/geneea/sdk
```

### Comparing `geneea-nlp-client-1.4.4/geneea_nlp_client.egg-info/SOURCES.txt` & `geneea-nlp-client-1.5.0/geneea_nlp_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,12 +36,13 @@
 tests/geneeanlpclient/common/test_ud.py
 tests/geneeanlpclient/g3/__init__.py
 tests/geneeanlpclient/g3/examples.py
 tests/geneeanlpclient/g3/generate.py
 tests/geneeanlpclient/g3/test_analysis.py
 tests/geneeanlpclient/g3/test_charSpan.py
 tests/geneeanlpclient/g3/test_f2converter.py
+tests/geneeanlpclient/g3/test_model.py
 tests/geneeanlpclient/g3/test_request.py
 tests/geneeanlpclient/g3/test_rw.py
 tests/geneeanlpclient/g3/test_tokenSupport.py
 tests/geneeanlpclient/g3/test_tokenutils.py
 tests/geneeanlpclient/g3/test_treeBuilder.py
```

### Comparing `geneea-nlp-client-1.4.4/geneeanlpclient/common/common.py` & `geneea-nlp-client-1.5.0/geneeanlpclient/common/common.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/geneeanlpclient/common/dictutil.py` & `geneea-nlp-client-1.5.0/geneeanlpclient/common/dictutil.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/geneeanlpclient/common/restutil.py` & `geneea-nlp-client-1.5.0/geneeanlpclient/common/restutil.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/geneeanlpclient/common/ud.py` & `geneea-nlp-client-1.5.0/geneeanlpclient/common/ud.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/geneeanlpclient/g3/__init__.py` & `geneea-nlp-client-1.5.0/geneeanlpclient/g3/__init__.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/geneeanlpclient/g3/client.py` & `geneea-nlp-client-1.5.0/geneeanlpclient/g3/client.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/geneeanlpclient/g3/f2converter.py` & `geneea-nlp-client-1.5.0/geneeanlpclient/g3/f2converter.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/geneeanlpclient/g3/model.py` & `geneea-nlp-client-1.5.0/geneeanlpclient/g3/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -897,14 +897,54 @@
         self._fillParents()
         root = self._findRoot()  # exactly one root check; addDependency checks for multiple parents => tree
         self._fillChildren()
 
         return Tree[Node](tokens=self._nodes, root=root)
 
 
+class GkbProperty:
+
+    def __init__(self, *,
+                 name: str,
+                 label: str,
+                 valueGkbId: Optional[str] = None,
+                 boolValue: Optional[bool] = None,
+                 floatValue: Optional[float] = None,
+                 intValue: Optional[int] = None,
+                 strValue: Optional[str] = None,
+                 ) -> None:
+        self.propertyOf: Union[Entity, Tag] = None
+        """ Entity this mention belongs to """
+        self.name: str = name
+        """ Property name """
+        self.label: str = label
+        """ Label describing the property (in presentation language of analysis """
+        self.valueGkbId: Optional[str] = valueGkbId
+        """ GKB identifier if any """
+        self.boolValue: Optional[bool] = boolValue
+        """ Actual value if the type is boolean """
+        self.floatValue: Optional[float] = floatValue
+        """ Actual value if the type is float """
+        self.intValue: Optional[int] = intValue
+        """ Actual value if the type is integer """
+        self.strValue: Optional[str] = strValue
+        """ Actual value if the type is string (including datetime values and GPS coordinates) """
+        if boolValue is None and floatValue is None and intValue is None and strValue is None:
+            raise ValueError(f'At least one value has to be set for GkbProperty {name} ({valueGkbId})')
+
+    def __hash__(self):
+        return hash((self.name, self.valueGkbId, self.boolValue, self.floatValue, self.intValue, self.strValue))
+
+    def __str__(self):
+        return objToStr(self, ('name', 'valueGkbId', 'boolValue', 'floatValue', 'intValue', 'strValue'))
+
+    def __repr__(self):
+        return objRepr(self, ('name', 'valueGkbId', 'boolValue', 'floatValue', 'intValue', 'strValue', 'label'))
+
+
 class Entity:
     """ A class encapsulating an Entity. """
 
     class Mention:
 
         def __init__(self, *,
             id: str,
@@ -964,43 +1004,46 @@
 
     def __init__(self, *,
         id: str,
         gkbId: str = None,
         stdForm: str,
         type: str,
         feats: Mapping[str, str] = None,
+        gkbProperties: List[GkbProperty] = None,
         mentions: List[Mention],
         sentiment: Sentiment = None,
         vectors: List[Vector] = None,
     ) -> None:
         self._id = id
         """ ID of the entity used to refer to it from other objects """
         self.gkbId: Optional[str] = gkbId
         """ Unique identifier of this entity in Geneea knowledge-base """
         self.stdForm: str = stdForm
         """ Standard form of the entity, abstracting from alternative names """
         self.type: str = type
         """ Basic type of this entity (e.g. person, location, ...)"""
         self.feats: Mapping[str, str] = feats or {}
         """ Custom features/properties. """
+        self.gkbProperties: List[GkbProperty] = gkbProperties or []
+        """ Custom GKB properties. """
         self.mentions: List[Entity.Mention] = mentions
         """ Actual occurrences of this entity in the text. Empty if not requested/supported."""
         self.sentiment: Optional[Sentiment] = sentiment
         """ Sentiment of this entity. None if not requested. """
         self.vectors: Optional[List[Vector]] = vectors
         """ Optional vectors for this entity. """
 
     def __hash__(self):
         return hash(self._id)
 
     def __str__(self):
-        return objToStr(self, ('gkbId', 'stdForm', 'type', 'feats', 'mentions', 'sentiment', 'vectors'))
+        return objToStr(self, ('gkbId', 'stdForm', 'type', 'feats', 'gkbProperties', 'mentions', 'sentiment', 'vectors'))
 
     def __repr__(self):
-        return objRepr(self, ('_id', 'gkbId', 'stdForm', 'type', 'feats', 'mentions', 'sentiment', 'vectors'))
+        return objRepr(self, ('_id', 'gkbId', 'stdForm', 'type', 'feats', 'gkbProperties', 'mentions', 'sentiment', 'vectors'))
 
 
 class Tag:
     TYPE_TOPIC = 'topic'
     """ Type of the tag with the main topic of the document """
     TYPE_TOPIC_DISTRIBUTION = 'topic.distribution'
     """ Type of the tags with the topic distribution of the document """
@@ -1052,14 +1095,15 @@
     def __init__(self, *,
         id: str,
         gkbId: str = None,
         stdForm: str,
         type: str,
         relevance: float,
         feats: Mapping[str, str] = None,
+        gkbProperties: List[GkbProperty] = None,
         mentions: List[Mention],
         sentiment: Sentiment = None,
         vectors: List[Vector] = None,
     ) -> None:
         self._id = id
         """ ID of the tag used to refer to it from other objects """
         self.gkbId: Optional[str] = gkbId
@@ -1068,29 +1112,31 @@
         """ Standard form of the tag, abstracting from its alternative names """
         self.type: str = type
         """ Domain-specific type (e.g. content, theme, iAB, department) """
         self.relevance: float = relevance
         """ Relevance of the tag relative to the content of the document """
         self.feats: Mapping[str, str] = feats or {}
         """ Custom features """
+        self.gkbProperties: List[GkbProperty] = gkbProperties or []
+        """ Custom GKB properties. """
         self.mentions: List[Tag.Mention] = mentions
         """ Text segments related to this tag. Empty if not appropriate/requested/supported. """
         self.sentiment: Optional[Sentiment] = sentiment
         """ Sentiment of this tag. Not supported yet.  """
         self.vectors: Optional[List[Vector]] = vectors
         """ Optional vectors for this tag. """
 
     def __hash__(self):
         return hash(self._id)
 
     def __str__(self):
-        return objToStr(self, ('gkbId', 'stdForm', 'type', 'relevance', 'feats', 'mentions', 'sentiment', 'vectors'))
+        return objToStr(self, ('gkbId', 'stdForm', 'type', 'relevance', 'feats', 'gkbProperties', 'mentions', 'sentiment', 'vectors'))
 
     def __repr__(self):
-        return objRepr(self, ('_id', 'gkbId', 'stdForm', 'type', 'relevance', 'feats', 'mentions', 'sentiment', 'vectors'))
+        return objRepr(self, ('_id', 'gkbId', 'stdForm', 'type', 'relevance', 'feats', 'gkbProperties', 'mentions', 'sentiment', 'vectors'))
 
 
 class Relation:
     TYPE_ATTR = 'ATTR'
     """ Attribute relation (e.g. `good(pizza)` for _good pizza_, _pizza is good_), the attribute is  """
     TYPE_VERB = 'VERB'
     """ Verbal relation (e.g. `eat(John,pizza)` for _John ate a pizza._"""
```

### Comparing `geneea-nlp-client-1.4.4/geneeanlpclient/g3/reader.py` & `geneea-nlp-client-1.5.0/geneeanlpclient/g3/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 import math
 import re
 import warnings
 from typing import Any, Dict, Iterable, List, Optional
 
 from geneeanlpclient.common import ud
 from geneeanlpclient.common.dictutil import JsonType, getValue
-from geneeanlpclient.g3.model import (Analysis, CharSpan, Language, Sentiment, Paragraph, Sentence, Relation, Entity, Tag,
-    TectoToken, Token, TreeBuilder, Tree, TokenSupport, Vector, Node)
+from geneeanlpclient.g3.model import (Analysis, CharSpan, GkbProperty, Language, Sentiment, Paragraph,
+                                      Sentence, Relation, Entity, Tag,
+                                      TectoToken, Token, TreeBuilder, Tree, TokenSupport, Vector, Node)
 
 STD_KEYS = frozenset([
     'id', 'language', 'paragraphs',
     'entities', 'tags', 'relations',
     'docSentiment', 'itemSentiments', 'docVectors', 'itemVectors',
     'usedChars', 'metadata', 'debugInfo', 'version'
 ])
@@ -133,15 +134,15 @@
         version = rawAnalysis.get('version', '3.0.0')
         verMatch = re.fullmatch(r'^([0-9]+)\.([0-9]+)\.([0-9]+)$', version)
         if not verMatch:
             raise ValueError(f'unsupported API version "{version}"')
         verMajor, verMinor, verFix = tuple(map(int, verMatch.groups()))
         if verMajor > 3:
             raise ValueError(f'unsupported API version "{version}", major ver.num > 3')
-        if verMajor != 3 or verMinor > 2:
+        if verMajor != 3 or verMinor > 3:
             LOG.warning(f'Reading analysis with version {version} '
                         f'(higher than {self.version}) is only partially supported')
         else:
             self.version = verMajor, verMinor, verFix
 
     def _readSentiment(self, rawSentiment: JsonType) -> Sentiment:
         return Sentiment(
@@ -284,14 +285,25 @@
             sentences=[self._readSentence(rawS, offMap) for rawS in rawPara['sentences']],
         )
         for s in para.sentences:
             s.paragraph = para
         self._register(para)
         return para
 
+    def _readGkbProperties(self, raw: JsonType) -> GkbProperty:
+        return GkbProperty(
+            name=raw['name'],
+            label=raw.get('label', ''),
+            valueGkbId=raw.get('valueGkbId'),
+            boolValue=raw.get('boolValue'),
+            floatValue=raw.get('floatValue'),
+            intValue=raw.get('intValue'),
+            strValue=raw.get('strValue'),
+        )
+
     def _readEntityMention(self, raw: JsonType) -> Entity.Mention:
         return Entity.Mention(
             id=raw['id'],
             mwl=raw['mwl'],
             text=raw['text'],
             tokens=TokenSupport.of(self.resolveIds(raw.get('tokenIds', []))),
             derivedFrom=raw.get('derivedFromEntityId'),  # will be replaced by entity obj. later
@@ -301,18 +313,21 @@
     def _readEntity(self, raw: JsonType) -> Entity:
         ent = Entity(
             id=raw['id'],
             gkbId=raw.get('gkbId'),
             stdForm=raw['stdForm'],
             type=raw['type'],
             feats=raw.get('feats'),
+            gkbProperties=[self._readGkbProperties(rp) for rp in raw.get('gkbProperties', [])],
             mentions=[self._readEntityMention(rm) for rm in raw.get('mentions', [])],
         )
         for m in ent.mentions:
             m.mentionOf = ent
+        for p in ent.gkbProperties:
+            p.propertyOf = ent
         self._register(ent)
         self._registerAll(ent.mentions)
         return ent
 
     def _readTagMention(self, raw: JsonType) -> Tag.Mention:
         return Tag.Mention(
             id=raw['id'],
@@ -324,18 +339,21 @@
         tag = Tag(
             id=raw['id'],
             gkbId=raw.get('gkbId'),
             stdForm=raw['stdForm'],
             type=raw['type'],
             relevance=raw['relevance'],
             feats=raw.get('feats'),
+            gkbProperties=[self._readGkbProperties(rp) for rp in raw.get('gkbProperties', [])],
             mentions=[self._readTagMention(rm) for rm in raw.get('mentions', [])],
         )
         for m in tag.mentions:
             m.mentionOf = tag
+        for p in tag.gkbProperties:
+            p.propertyOf = tag
         self._register(tag)
         self._registerAll(tag.mentions)
         return tag
 
     def _readRelationArg(self, raw: JsonType) -> Relation.Argument:
         return Relation.Argument(
             name=raw['name'],
```

### Comparing `geneea-nlp-client-1.4.4/geneeanlpclient/g3/request.py` & `geneea-nlp-client-1.5.0/geneeanlpclient/g3/request.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/geneeanlpclient/g3/writer.py` & `geneea-nlp-client-1.5.0/geneeanlpclient/g3/writer.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 
 # Except the toDict function, all functions and classes defined in this file are only internal helpers.
 
 
 from typing import Dict, List
 
 from geneeanlpclient.common.dictutil import JsonType, DictBuilder
-from geneeanlpclient.g3.model import Analysis, Relation, Paragraph, Entity, Tag, Token, TectoToken, Sentence, Sentiment, Vector
+from geneeanlpclient.g3.model import (Analysis, Relation, Paragraph, GkbProperty,
+                                      Entity, Tag, Token, TectoToken, Sentence, Sentiment, Vector)
 
 
 def toDict(obj: Analysis) -> JsonType:
     """
     Writes the Analysis to a JSON-based dictionary to a format as returned by Geneea G3 API.
     """
     builder = DictBuilder({
-        'version': '3.2.1',
+        'version': '3.3.0',
         'language': {'detected': obj.language.detected},
     })
     builder.addIfNotNone('id', obj.docId)
     builder.addIfNotNone('paragraphs', [_toRawPara(p) for p in obj.paragraphs])
     builder.addIfNotNone('entities', [_toRawEntity(e) for e in obj.entities])
     builder.addIfNotNone('tags', [_toRawTag(t) for t in obj.tags])
     builder.addIfNotNone('relations', [_toRawRelation(r) for r in obj.relations])
@@ -43,14 +44,27 @@
     builder.addIfNotNone('itemVectors', _toRawItemVectors(obj))
     builder.addIfNotNone('usedChars', obj.usedChars)
     builder.addIfNotNone('metadata', obj.metadata)
     builder.addIfNotNone('debugInfo', obj.debugInfo)
     return builder.build()
 
 
+def _toRawGkbProperty(prop: GkbProperty) -> JsonType:
+    builder = DictBuilder({
+        'name': prop.name,
+    })
+    builder.addIfNotNone('label', prop.label)
+    builder.addIfNotNone('valueGkbId', prop.valueGkbId)
+    builder.addIfNotNone('boolValue', prop.boolValue)
+    builder.addIfNotNone('floatValue', prop.floatValue)
+    builder.addIfNotNone('intValue', prop.intValue)
+    builder.addIfNotNone('strValue', prop.strValue)
+    return builder.build()
+
+
 def _toRawEntityMention(mention: Entity.Mention) -> JsonType:
     builder = DictBuilder({
         'text': mention.text,
         'mwl': mention.mwl,
     })
     builder.addId('id', mention)
     builder.addIds('tokenIds', mention.tokens)
@@ -63,14 +77,15 @@
     builder = DictBuilder({
         'stdForm': entity.stdForm,
         'type': entity.type,
     })
     builder.addId('id', entity)
     builder.addIfNotNone('gkbId', entity.gkbId)
     builder.addIfNotNone('feats', entity.feats)
+    builder.addIfNotNone('gkbProperties', [_toRawGkbProperty(p) for p in entity.gkbProperties])
     builder.addIfNotNone('mentions', [_toRawEntityMention(m) for m in entity.mentions])
     return builder.build()
 
 
 def _toRawTagMention(mention: Tag.Mention) -> JsonType:
     builder = DictBuilder({})
     builder.addId('id', mention)
@@ -84,14 +99,15 @@
         'stdForm': tag.stdForm,
         'type': tag.type,
         'relevance': tag.relevance,
     })
     builder.addId('id', tag)
     builder.addIfNotNone('gkbId', tag.gkbId)
     builder.addIfNotNone('feats', tag.feats)
+    builder.addIfNotNone('gkbProperties', [_toRawGkbProperty(p) for p in tag.gkbProperties])
     builder.addIfNotNone('mentions', [_toRawTagMention(m) for m in tag.mentions])
     return builder.build()
 
 
 def _toRawArg(arg: Relation.Argument) -> JsonType:
     builder = DictBuilder({
         "name": arg.name,
```

### Comparing `geneea-nlp-client-1.4.4/setup.py` & `geneea-nlp-client-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', mode='r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='geneea-nlp-client',
-    version='1.4.4',
+    version='1.5.0',
 
     author='Geneea Analytics s.r.o',
     author_email='support@geneea.com',
     description='The SDK library and command-line interface to Geneea Interpretor, an NLP REST API.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='geneea python interpretor nlp nlu api cli',
@@ -36,12 +36,11 @@
     # Dependencies
     install_requires=['requests~=2.25', 'retrying~=1.3'],
     dependency_links=[],
     extras_require={
         'examples':  ['pandas>=0.22']
     },
 
-
     packages=find_packages(),
 
     test_suite='tests'
 )
```

### Comparing `geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/test_common.py` & `geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/test_common.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/tests/geneeanlpclient/common/test_jsonutil.py` & `geneea-nlp-client-1.5.0/tests/geneeanlpclient/common/test_jsonutil.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/examples.py` & `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/examples.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/generate.py` & `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/generate.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_analysis.py` & `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_analysis.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_charSpan.py` & `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_charSpan.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_f2converter.py` & `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_f2converter.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_request.py` & `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_request.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_rw.py` & `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_rw.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                         token['fnc'] = 'root'
 
     def test_read_write(self):
         self.maxDiff = None
 
         examplesPath = Path(__file__).parent / 'examples'
         exampleFiles = list(examplesPath.glob('example*.json'))
-        self.assertEqual(127, len(exampleFiles))
+        self.assertEqual(129, len(exampleFiles))
 
         for exampleFile in exampleFiles:
             with exampleFile.open(encoding='utf8') as file:
                 obj = fromDict(json.load(file))
 
             actual = toDict(obj)
 
@@ -50,15 +50,15 @@
         """
         Test that we can read newer G3 with the same major version and write it again.
         It is assumed that after write some content can be lost.
         """
         self.maxDiff = None
 
         exampleFile = Path(__file__).parent / 'examples' / 'forward_example_ENTITIES_PROPS.json'
-        exampleExpectedFile = Path(__file__).parent / 'examples' / 'example_ENTITIES.json'
+        exampleExpectedFile = Path(__file__).parent / 'examples' / 'example_ENTITIES_PROPS.json'
 
         with exampleFile.open(encoding='utf8') as file:
             obj = fromDict(json.load(file))
 
         actual = toDict(obj)
 
         with exampleExpectedFile.open(encoding='utf8') as file:
```

### Comparing `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_tokenSupport.py` & `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_tokenSupport.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_tokenutils.py` & `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_tokenutils.py`

 * *Files identical despite different names*

### Comparing `geneea-nlp-client-1.4.4/tests/geneeanlpclient/g3/test_treeBuilder.py` & `geneea-nlp-client-1.5.0/tests/geneeanlpclient/g3/test_treeBuilder.py`

 * *Files identical despite different names*

