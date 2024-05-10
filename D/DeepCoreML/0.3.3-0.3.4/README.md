# Comparing `tmp/DeepCoreML-0.3.3.tar.gz` & `tmp/DeepCoreML-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepCoreML-0.3.3.tar", last modified: Thu Jan 11 08:36:47 2024, max compression
+gzip compressed data, was "DeepCoreML-0.3.4.tar", last modified: Fri May 10 21:44:05 2024, max compression
```

## Comparing `DeepCoreML-0.3.3.tar` & `DeepCoreML-0.3.4.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-01-11 08:36:47.494681 DeepCoreML-0.3.3/
-drwxrwxrwx   0        0        0        0 2024-01-11 08:36:47.475743 DeepCoreML-0.3.3/DeepCoreML/
--rw-rw-rw-   0        0        0     8802 2023-05-03 07:57:42.000000 DeepCoreML-0.3.3/DeepCoreML/BERTModels.py
--rw-rw-rw-   0        0        0     1824 2023-12-24 20:39:31.000000 DeepCoreML-0.3.3/DeepCoreML/Classifiers.py
--rw-rw-rw-   0        0        0     1786 2023-10-15 22:04:41.000000 DeepCoreML-0.3.3/DeepCoreML/DataAnimator.py
--rw-rw-rw-   0        0        0     7358 2024-01-10 10:54:14.000000 DeepCoreML-0.3.3/DeepCoreML/DataSamplers.py
--rw-rw-rw-   0        0        0     3479 2023-12-22 10:52:03.000000 DeepCoreML-0.3.3/DeepCoreML/DataTools.py
--rw-rw-rw-   0        0        0     8318 2023-12-24 23:46:55.000000 DeepCoreML-0.3.3/DeepCoreML/Datasets.py
--rw-rw-rw-   0        0        0     8521 2023-12-21 00:50:49.000000 DeepCoreML-0.3.3/DeepCoreML/DimensionalityReducers.py
--rw-rw-rw-   0        0        0     1933 2024-01-09 21:59:20.000000 DeepCoreML-0.3.3/DeepCoreML/ResultHandler.py
--rw-rw-rw-   0        0        0     3208 2023-11-27 23:36:07.000000 DeepCoreML-0.3.3/DeepCoreML/TextDatasets.py
--rw-rw-rw-   0        0        0     2672 2023-11-21 23:44:25.000000 DeepCoreML-0.3.3/DeepCoreML/TextPreprocessor.py
--rw-rw-rw-   0        0        0     8624 2023-11-26 21:21:04.000000 DeepCoreML-0.3.3/DeepCoreML/TextVectorizers.py
--rw-rw-rw-   0        0        0        0 2023-11-29 21:54:47.000000 DeepCoreML-0.3.3/DeepCoreML/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-11 08:36:47.493684 DeepCoreML-0.3.3/DeepCoreML/generators/
--rw-rw-rw-   0        0        0     8563 2024-01-08 14:37:07.000000 DeepCoreML-0.3.3/DeepCoreML/generators/BaseGenerators.py
--rw-rw-rw-   0        0        0    13353 2024-01-09 23:15:36.000000 DeepCoreML-0.3.3/DeepCoreML/generators/DataTransformers.py
--rw-rw-rw-   0        0        0    14448 2024-01-09 23:15:36.000000 DeepCoreML-0.3.3/DeepCoreML/generators/c_gan.py
--rw-rw-rw-   0        0        0    10022 2023-12-25 08:59:25.000000 DeepCoreML-0.3.3/DeepCoreML/generators/cbr.py
--rw-rw-rw-   0        0        0    19794 2024-01-11 08:31:22.000000 DeepCoreML-0.3.3/DeepCoreML/generators/cluster_gan.py
--rw-rw-rw-   0        0        0    23310 2024-01-08 16:30:02.000000 DeepCoreML-0.3.3/DeepCoreML/generators/ct_gan.py
--rw-rw-rw-   0        0        0     7136 2024-01-08 15:55:27.000000 DeepCoreML-0.3.3/DeepCoreML/generators/gan_discriminators.py
--rw-rw-rw-   0        0        0     4165 2024-01-10 00:41:18.000000 DeepCoreML-0.3.3/DeepCoreML/generators/gan_generators.py
--rw-rw-rw-   0        0        0    17790 2024-01-09 22:22:17.000000 DeepCoreML-0.3.3/DeepCoreML/generators/sb_gan.py
--rw-rw-rw-   0        0        0     8945 2024-01-11 08:31:22.000000 DeepCoreML-0.3.3/DeepCoreML/main_imbalanced.py
--rw-rw-rw-   0        0        0     2135 2023-11-29 10:27:00.000000 DeepCoreML-0.3.3/DeepCoreML/main_sentiment.py
-drwxrwxrwx   0        0        0        0 2024-01-11 08:36:47.478734 DeepCoreML-0.3.3/DeepCoreML.egg-info/
--rw-rw-rw-   0        0        0     2054 2024-01-11 08:36:47.000000 DeepCoreML-0.3.3/DeepCoreML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      909 2024-01-11 08:36:47.000000 DeepCoreML-0.3.3/DeepCoreML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-11 08:36:47.000000 DeepCoreML-0.3.3/DeepCoreML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2024-01-11 08:36:47.000000 DeepCoreML-0.3.3/DeepCoreML.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-01-11 08:36:47.000000 DeepCoreML-0.3.3/DeepCoreML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      559 2022-06-20 23:55:01.000000 DeepCoreML-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     2054 2024-01-11 08:36:47.494681 DeepCoreML-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-11-29 21:58:29.000000 DeepCoreML-0.3.3/README.md
--rw-rw-rw-   0        0        0       42 2024-01-11 08:36:47.494681 DeepCoreML-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     3044 2023-12-24 23:56:26.000000 DeepCoreML-0.3.3/setup.py
+drwxrwxrwx   0 leo       (1000) leo       (1000)        0 2024-05-10 21:44:05.970985 DeepCoreML-0.3.4/
+drwxrwxrwx   0 leo       (1000) leo       (1000)        0 2024-05-10 21:44:05.966434 DeepCoreML-0.3.4/DeepCoreML/
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     9101 2024-02-28 21:17:26.000000 DeepCoreML-0.3.4/DeepCoreML/BERTModels.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     1829 2024-04-10 20:17:03.000000 DeepCoreML-0.3.4/DeepCoreML/Classifiers.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     1714 2024-02-28 21:17:26.000000 DeepCoreML-0.3.4/DeepCoreML/DataAnimator.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     7255 2024-05-10 21:40:09.000000 DeepCoreML-0.3.4/DeepCoreML/DataSamplers.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     3455 2024-02-28 21:17:26.000000 DeepCoreML-0.3.4/DeepCoreML/DataTools.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)    14005 2024-05-07 10:40:05.000000 DeepCoreML-0.3.4/DeepCoreML/Datasets.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     8521 2023-12-21 00:50:49.000000 DeepCoreML-0.3.4/DeepCoreML/DimensionalityReducers.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     3200 2024-04-14 08:47:49.000000 DeepCoreML-0.3.4/DeepCoreML/ResultHandler.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     1239 2024-01-18 21:48:26.000000 DeepCoreML-0.3.4/DeepCoreML/Tests.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     3208 2024-02-28 21:17:26.000000 DeepCoreML-0.3.4/DeepCoreML/TextDatasets.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     2672 2023-11-21 23:44:25.000000 DeepCoreML-0.3.4/DeepCoreML/TextPreprocessor.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     8629 2024-02-28 21:17:26.000000 DeepCoreML-0.3.4/DeepCoreML/TextVectorizers.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)        0 2023-11-29 21:54:47.000000 DeepCoreML-0.3.4/DeepCoreML/__init__.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     4472 2024-05-10 21:40:09.000000 DeepCoreML-0.3.4/DeepCoreML/eval.py
+drwxrwxrwx   0 leo       (1000) leo       (1000)        0 2024-05-10 21:44:05.970328 DeepCoreML-0.3.4/DeepCoreML/generators/
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     6890 2024-01-30 10:48:11.000000 DeepCoreML-0.3.4/DeepCoreML/generators/BaseGenerators.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)    14053 2024-01-31 09:55:35.000000 DeepCoreML-0.3.4/DeepCoreML/generators/DataTransformers.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)    19096 2024-01-29 16:01:26.000000 DeepCoreML-0.3.4/DeepCoreML/generators/c_gan.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)    10298 2024-05-07 10:02:32.000000 DeepCoreML-0.3.4/DeepCoreML/generators/cbr.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)    26397 2024-01-31 23:31:07.000000 DeepCoreML-0.3.4/DeepCoreML/generators/ct_gan.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     7136 2024-01-08 15:55:27.000000 DeepCoreML-0.3.4/DeepCoreML/generators/gan_discriminators.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     4165 2024-01-10 00:41:18.000000 DeepCoreML-0.3.4/DeepCoreML/generators/gan_generators.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)    17981 2024-05-07 10:02:32.000000 DeepCoreML-0.3.4/DeepCoreML/generators/sb_gan.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     3498 2024-05-10 21:36:15.000000 DeepCoreML-0.3.4/DeepCoreML/main_imbalanced.py
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     2135 2023-11-29 10:27:00.000000 DeepCoreML-0.3.4/DeepCoreML/main_sentiment.py
+drwxrwxrwx   0 leo       (1000) leo       (1000)        0 2024-05-10 21:44:05.968068 DeepCoreML-0.3.4/DeepCoreML.egg-info/
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     2352 2024-05-10 21:44:05.000000 DeepCoreML-0.3.4/DeepCoreML.egg-info/PKG-INFO
+-rwxrwxrwx   0 leo       (1000) leo       (1000)      911 2024-05-10 21:44:05.000000 DeepCoreML-0.3.4/DeepCoreML.egg-info/SOURCES.txt
+-rwxrwxrwx   0 leo       (1000) leo       (1000)        1 2024-05-10 21:44:05.000000 DeepCoreML-0.3.4/DeepCoreML.egg-info/dependency_links.txt
+-rwxrwxrwx   0 leo       (1000) leo       (1000)      139 2024-05-10 21:44:05.000000 DeepCoreML-0.3.4/DeepCoreML.egg-info/requires.txt
+-rwxrwxrwx   0 leo       (1000) leo       (1000)       11 2024-05-10 21:44:05.000000 DeepCoreML-0.3.4/DeepCoreML.egg-info/top_level.txt
+-rwxrwxrwx   0 leo       (1000) leo       (1000)      559 2022-06-20 23:55:01.000000 DeepCoreML-0.3.4/LICENSE
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     2352 2024-05-10 21:44:05.970734 DeepCoreML-0.3.4/PKG-INFO
+-rwxrwxrwx   0 leo       (1000) leo       (1000)      466 2023-11-29 21:58:29.000000 DeepCoreML-0.3.4/README.md
+-rwxrwxrwx   0 leo       (1000) leo       (1000)       38 2024-05-10 21:44:05.971027 DeepCoreML-0.3.4/setup.cfg
+-rwxrwxrwx   0 leo       (1000) leo       (1000)     3044 2024-05-10 21:42:42.000000 DeepCoreML-0.3.4/setup.py
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/BERTModels.py` & `DeepCoreML-0.3.4/DeepCoreML/BERTModels.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,74 @@
 map_name_to_handle = {
-    'bert_en_uncased_L-12_H-768_A-12': 'https://tfhub.dev/tensorflow/bert_en_uncased_L-12_H-768_A-12/3',
-    'bert_en_cased_L-12_H-768_A-12': 'https://tfhub.dev/tensorflow/bert_en_cased_L-12_H-768_A-12/3',
-    'bert_multi_cased_L-12_H-768_A-12': 'https://tfhub.dev/tensorflow/bert_multi_cased_L-12_H-768_A-12/3',
-    'small_bert/bert_en_uncased_L-2_H-128_A-2': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-2_H-128_A-2/1',
-    'small_bert/bert_en_uncased_L-2_H-256_A-4': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-2_H-256_A-4/1',
-    'small_bert/bert_en_uncased_L-2_H-512_A-8': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-2_H-512_A-8/1',
-    'small_bert/bert_en_uncased_L-2_H-768_A-12': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-2_H-768_A-12/1',
-    'small_bert/bert_en_uncased_L-4_H-128_A-2': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-4_H-128_A-2/1',
-    'small_bert/bert_en_uncased_L-4_H-256_A-4': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-4_H-256_A-4/1',
-    'small_bert/bert_en_uncased_L-4_H-512_A-8': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-4_H-512_A-8/1',
-    'small_bert/bert_en_uncased_L-4_H-768_A-12': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-4_H-768_A-12/1',
-    'small_bert/bert_en_uncased_L-6_H-128_A-2': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-6_H-128_A-2/1',
-    'small_bert/bert_en_uncased_L-6_H-256_A-4': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-6_H-256_A-4/1',
-    'small_bert/bert_en_uncased_L-6_H-512_A-8': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-6_H-512_A-8/1',
-    'small_bert/bert_en_uncased_L-6_H-768_A-12': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-6_H-768_A-12/1',
-    'small_bert/bert_en_uncased_L-8_H-128_A-2': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-8_H-128_A-2/1',
-    'small_bert/bert_en_uncased_L-8_H-256_A-4': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-8_H-256_A-4/1',
-    'small_bert/bert_en_uncased_L-8_H-512_A-8': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-8_H-512_A-8/1',
-    'small_bert/bert_en_uncased_L-8_H-768_A-12': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-8_H-768_A-12/1',
-    'small_bert/bert_en_uncased_L-10_H-128_A-2': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-10_H-128_A-2/1',
-    'small_bert/bert_en_uncased_L-10_H-256_A-4': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-10_H-256_A-4/1',
-    'small_bert/bert_en_uncased_L-10_H-512_A-8': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-10_H-512_A-8/1',
-    'small_bert/bert_en_uncased_L-10_H-768_A-12': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-10_H-768_A-12/1',
-    'small_bert/bert_en_uncased_L-12_H-128_A-2': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-12_H-128_A-2/1',
-    'small_bert/bert_en_uncased_L-12_H-256_A-4': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-12_H-256_A-4/1',
-    'small_bert/bert_en_uncased_L-12_H-512_A-8': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-12_H-512_A-8/1',
-    'small_bert/bert_en_uncased_L-12_H-768_A-12': 'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-12_H-768_A-12/1',
-    'albert_en_base': 'https://tfhub.dev/tensorflow/albert_en_base/2',
-    'electra_small': 'https://tfhub.dev/google/electra_small/2',
-    'electra_base': 'https://tfhub.dev/google/electra_base/2',
-    'experts_pubmed': 'https://tfhub.dev/google/experts/bert/pubmed/2',
-    'experts_wiki_books': 'https://tfhub.dev/google/experts/bert/wiki_books/2',
-    'talking-heads_base': 'https://tfhub.dev/tensorflow/talkheads_ggelu_bert_en_base/1',
+    'bert_en_uncased_L-12_H-768_A-12':
+        'https://tfhub.dev/tensorflow/bert_en_uncased_L-12_H-768_A-12/3',
+    'bert_en_cased_L-12_H-768_A-12':
+        'https://tfhub.dev/tensorflow/bert_en_cased_L-12_H-768_A-12/3',
+    'bert_multi_cased_L-12_H-768_A-12':
+        'https://tfhub.dev/tensorflow/bert_multi_cased_L-12_H-768_A-12/3',
+    'small_bert/bert_en_uncased_L-2_H-128_A-2':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-2_H-128_A-2/1',
+    'small_bert/bert_en_uncased_L-2_H-256_A-4':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-2_H-256_A-4/1',
+    'small_bert/bert_en_uncased_L-2_H-512_A-8':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-2_H-512_A-8/1',
+    'small_bert/bert_en_uncased_L-2_H-768_A-12':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-2_H-768_A-12/1',
+    'small_bert/bert_en_uncased_L-4_H-128_A-2':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-4_H-128_A-2/1',
+    'small_bert/bert_en_uncased_L-4_H-256_A-4':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-4_H-256_A-4/1',
+    'small_bert/bert_en_uncased_L-4_H-512_A-8':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-4_H-512_A-8/1',
+    'small_bert/bert_en_uncased_L-4_H-768_A-12':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-4_H-768_A-12/1',
+    'small_bert/bert_en_uncased_L-6_H-128_A-2':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-6_H-128_A-2/1',
+    'small_bert/bert_en_uncased_L-6_H-256_A-4':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-6_H-256_A-4/1',
+    'small_bert/bert_en_uncased_L-6_H-512_A-8':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-6_H-512_A-8/1',
+    'small_bert/bert_en_uncased_L-6_H-768_A-12':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-6_H-768_A-12/1',
+    'small_bert/bert_en_uncased_L-8_H-128_A-2':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-8_H-128_A-2/1',
+    'small_bert/bert_en_uncased_L-8_H-256_A-4':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-8_H-256_A-4/1',
+    'small_bert/bert_en_uncased_L-8_H-512_A-8':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-8_H-512_A-8/1',
+    'small_bert/bert_en_uncased_L-8_H-768_A-12':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-8_H-768_A-12/1',
+    'small_bert/bert_en_uncased_L-10_H-128_A-2':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-10_H-128_A-2/1',
+    'small_bert/bert_en_uncased_L-10_H-256_A-4':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-10_H-256_A-4/1',
+    'small_bert/bert_en_uncased_L-10_H-512_A-8':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-10_H-512_A-8/1',
+    'small_bert/bert_en_uncased_L-10_H-768_A-12':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-10_H-768_A-12/1',
+    'small_bert/bert_en_uncased_L-12_H-128_A-2':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-12_H-128_A-2/1',
+    'small_bert/bert_en_uncased_L-12_H-256_A-4':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-12_H-256_A-4/1',
+    'small_bert/bert_en_uncased_L-12_H-512_A-8':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-12_H-512_A-8/1',
+    'small_bert/bert_en_uncased_L-12_H-768_A-12':
+        'https://tfhub.dev/tensorflow/small_bert/bert_en_uncased_L-12_H-768_A-12/1',
+    'albert_en_base':
+        'https://tfhub.dev/tensorflow/albert_en_base/2',
+    'electra_small':
+        'https://tfhub.dev/google/electra_small/2',
+    'electra_base':
+        'https://tfhub.dev/google/electra_base/2',
+    'experts_pubmed':
+        'https://tfhub.dev/google/experts/bert/pubmed/2',
+    'experts_wiki_books':
+        'https://tfhub.dev/google/experts/bert/wiki_books/2',
+    'talking-heads_base':
+        'https://tfhub.dev/tensorflow/talkheads_ggelu_bert_en_base/1',
 }
 
 map_model_to_preprocess = {
     'bert_en_uncased_L-12_H-768_A-12': 'https://tfhub.dev/tensorflow/bert_en_uncased_preprocess/3',
     'bert_en_cased_L-12_H-768_A-12': 'https://tfhub.dev/tensorflow/bert_en_cased_preprocess/3',
     'small_bert/bert_en_uncased_L-2_H-128_A-2': 'https://tfhub.dev/tensorflow/bert_en_uncased_preprocess/3',
     'small_bert/bert_en_uncased_L-2_H-256_A-4': 'https://tfhub.dev/tensorflow/bert_en_uncased_preprocess/3',
@@ -92,8 +125,8 @@
     'BERT-L2-H128': 'google/bert_uncased_L-2_H-128_A-2',
     'BERT-L4-H128': 'google/bert_uncased_L-4_H-128_A-2',
     'BERT-L6-H128': 'google/bert_uncased_L-6_H-128_A-2',
     'BERT-L8-H128': 'google/bert_uncased_L-8_H-128_A-2',
     'BERT-L10-H128': 'google/bert_uncased_L-10_H-128_A-2',
     'BERT-L12-H128': 'google/bert_uncased_L-12_H-128_A-2',
     'BERT-SEQUENCE-GEN': 'google/bert_for_seq_generation_L-24_bbc_encoder'
-}
+}
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/Classifiers.py` & `DeepCoreML-0.3.4/DeepCoreML/Classifiers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from sklearn.svm import SVC
 from sklearn.neural_network import MLPClassifier
-from sklearn.tree import DecisionTreeClassifier
-from sklearn.linear_model import LogisticRegression
+# from sklearn.svm import SVC
+# from sklearn.tree import DecisionTreeClassifier
+# from sklearn.linear_model import LogisticRegression
 from sklearn.ensemble import RandomForestClassifier
 
 
 class BaseClassifier:
     def __init__(self, name, short_name, model, **kwargs):
         self.name_ = name
         self.short_name_ = short_name
@@ -28,14 +28,14 @@
             #                LogisticRegression(max_iter=300, random_state=random_state)),
             # BaseClassifier("Support Vector Machine", "SVM",
             #               SVC(kernel='rbf', C=1, random_state=random_state)),
             # BaseClassifier("Decision Tree", "DT",
             #               DecisionTreeClassifier(criterion='gini', max_depth=None,
             #                                      max_features=None, random_state=random_state)),
             # BaseClassifier("Random Forest", "RF",
-            #                RandomForestClassifier(n_estimators=50, criterion='gini', max_depth=None,
+            #               RandomForestClassifier(n_estimators=50, criterion='gini', max_depth=None,
             #                                      max_features='sqrt', n_jobs=1, random_state=random_state)),
             BaseClassifier("Multilayer Perceptron", "MLP",
                            MLPClassifier(activation='relu', hidden_layer_sizes=(128, 128), solver='adam', max_iter=300,
                                          random_state=random_state)),
         )
         self.num_classifiers_ = len(self.models_)
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/DataAnimator.py` & `DeepCoreML-0.3.4/DeepCoreML/DataAnimator.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,21 @@
 
 class DataAnimator:
     def __init__(self, data, num_classes, file_name):
         self.data = data
         self.num_classes = num_classes
         self.file_name = file_name
 
-        self.pt = [None for i in range(num_classes)]
-
         self.fig = plt.figure()
         self.ax = self.fig.add_subplot(111)
         self.ax.grid(True)
         self.ax.set_xlabel("x1")
         self.ax.set_ylabel("x2")
 
-        for c in range(num_classes):
-            self.pt[c], = self.ax.plot([], [], 'o')
+        self.pt = [self.ax.plot([], [], 'o') for _ in range(num_classes)]
 
     def init(self):
         for c in range(self.num_classes):
             self.pt[c].set_data([], [])
 
         return self.pt,
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/DataSamplers.py` & `DeepCoreML-0.3.4/DeepCoreML/DataSamplers.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,20 @@
 from imblearn.under_sampling import ClusterCentroids
 
 from sklearn.cluster import MiniBatchKMeans
 
 from generators.c_gan import cGAN
 from generators.sb_gan import sbGAN
 from generators.ct_gan import ctGAN
-from generators.cluster_gan import clusterGAN
+
 from generators.cbr import CBR
 
+from sdv.single_table import GaussianCopulaSynthesizer
+from sdv.single_table import CTGANSynthesizer
+
 
 class BaseSampler:
     def __init__(self, name, short_name, model, **kwargs):
         """
         A data resampling technique for mitigating class imbalance. It may be an over-sampling or an under-sampling
         technique implementing fit(x, y) and fit_resample(x, y).
 
@@ -57,19 +60,19 @@
             return x
 
 
 class DataSamplers:
     """
     Array of data over-sampling and inder-sampling techniques.
     """
-    def __init__(self, sampling_strategy='auto', random_state=0, **kwargs):
+    def __init__(self, metadata, sampling_strategy='auto', random_state=0, **kwargs):
         """
-        :param sampling_strategy: float, str, dict or callable, default=auto
+        :param sampling_strategy: how fit_resample creates samples
         Sampling information to resample the data set.
-         * When float, it corresponds to the desired ratio of the number of samples in the minority class over the
+         * When is float, it corresponds to the desired ratio of the number of samples in the minority class over the
            number of samples in the majority class after resampling. float is only available for binary classification.
            An error is raised for multi-class classification.
          * When str, specify the class targeted by the resampling. The number of samples in the different classes will
            be equalized. Possible choices are:
            * 'minority': resample only the minority class;
            * 'not minority': resample all classes but the minority class;
            * 'not majority': resample all classes but the majority class;
@@ -85,60 +88,68 @@
         clus = MiniBatchKMeans(n_clusters=2, init='k-means++', n_init='auto')
 
         # Good for KC1 disc = (12, 6) gen = (32, 32)
         disc = (256, 256)
         gen = (256, 256)
         emb_dim = 32
         knn = 10
-        rad = 400
+        rad = 1
         pac = 1
         epochs = 300
         batch_size = 32
+        max_clusters = 20
         act = 'tanh'
 
         self.over_samplers_ = (
             BaseSampler("None", "None", None),
 
             BaseSampler("Random Oversampling", "ROS",
                         RandomOverSampler(sampling_strategy=sampling_strategy, random_state=random_state)),
+
             BaseSampler("SMOTE", "SMOTE",
                         SMOTE(sampling_strategy=sampling_strategy, random_state=random_state)),
+
             BaseSampler("Borderline SMOTE", "B-SMOTE",
                         BorderlineSMOTE(sampling_strategy=sampling_strategy, random_state=random_state)),
+
             BaseSampler("SMOTE SVM", "SVM-SMOTE",
                         SVMSMOTE(sampling_strategy=sampling_strategy, random_state=random_state)),
+
             BaseSampler("KMeans SMOTE", "KMN-SMOTE",
                         KMeansSMOTE(sampling_strategy=sampling_strategy, kmeans_estimator=clus,
                                     cluster_balance_threshold=0.05, random_state=random_state)),
+
             BaseSampler("ADASYN", "ADASYN",
                         ADASYN(sampling_strategy=sampling_strategy, random_state=random_state)),
+
             BaseSampler("CBR", "CBR",
-                        CBR(verbose=False, random_state=random_state)),
-            BaseSampler("Conditional pac GAN", "cGAN",
+                        CBR(min_distance_factor=3, verbose=False, random_state=random_state)),
+
+            BaseSampler("Conditional GAN", "CGAN",
                         cGAN(embedding_dim=emb_dim, discriminator=disc, generator=gen, pac=pac, adaptive=False,
                              g_activation=act, epochs=epochs, batch_size=batch_size, random_state=random_state)),
 
-            # BaseSampler("Safe-Borderline GAN (KNN)", "SBGAN-KNN",
-            #             sbGAN(embedding_dim=emb_dim, discriminator=disc, generator=gen, pac=pac, adaptive=False,
-            #                   g_activation=act, epochs=epochs, batch_size=batch_size, method='knn', k=knn, r=rad,
-            #                   random_state=random_state)),
-
-            BaseSampler("Safe-Borderline GAN (RAD)", "SBGAN-RAD",
+            BaseSampler("Safe-Borderline GAN (KNN)", "SBGAN",
                         sbGAN(embedding_dim=emb_dim, discriminator=disc, generator=gen, pac=pac, adaptive=False,
-                              g_activation=act, epochs=epochs, batch_size=batch_size, method='rad', k=knn, r=rad,
+                              g_activation=act, epochs=epochs, batch_size=batch_size, method='knn', k=knn, r=rad,
                               random_state=random_state)),
 
-            BaseSampler("Cluster GAN", "ClusterGAN",
-                        clusterGAN(embedding_dim=emb_dim, discriminator=disc, generator=gen, pac=pac, adaptive=False,
-                                   g_activation=act, epochs=epochs, batch_size=batch_size, random_state=random_state)),
-
             BaseSampler("ctGAN", "ctGAN",
                         ctGAN(embedding_dim=emb_dim, discriminator=disc, generator=gen, pac=pac, adaptive=False,
                               g_activation=None, epochs=epochs, batch_size=batch_size, discriminator_steps=1,
                               log_frequency=True, verbose=False, random_state=random_state)),
+
+            BaseSampler("Gaussian Copula", "GCOP",
+                        GaussianCopulaSynthesizer(
+                            metadata, enforce_min_max_values=False, enforce_rounding=False)),
+
+            BaseSampler("CTGAN", "CTGAN",
+                        CTGANSynthesizer(
+                            metadata, enforce_min_max_values=False, enforce_rounding=False, epochs=epochs,
+                            verbose=False))
         )
 
         self.under_samplers_ = (
             BaseSampler("None", "None", None),
             BaseSampler("Random Oversampling", "RUS",
                         RandomUnderSampler(sampling_strategy=sampling_strategy, replacement=True,
                                            random_state=random_state)),
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/DataTools.py` & `DeepCoreML-0.3.4/DeepCoreML/DataTools.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,27 +55,27 @@
         torch.cuda.random.set_rng_state(cuda_random_state)
         torch.cuda.empty_cache()
 
     gc.collect()
 
 
 @contextlib.contextmanager
-def ct_set_random_states(random_state, set_model_random_state):
+def ct_set_random_states(seed, set_model_random_state):
     """Context manager for managing the random state.
 
     Args:
-        random_state (int or tuple):
+        seed (int or tuple):
             The random seed or a tuple of (numpy.random.RandomState, torch.Generator).
         set_model_random_state (function):
             Function to set the random state on the model.
     """
     original_np_state = np.random.get_state()
     original_torch_state = torch.get_rng_state()
 
-    random_np_state, random_torch_state = random_state
+    random_np_state, random_torch_state = seed
 
     np.random.set_state(random_np_state.get_state())
     torch.set_rng_state(random_torch_state.get_state())
 
     try:
         yield
     finally:
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/DimensionalityReducers.py` & `DeepCoreML-0.3.4/DeepCoreML/DimensionalityReducers.py`

 * *Files identical despite different names*

### Comparing `DeepCoreML-0.3.3/DeepCoreML/TextDatasets.py` & `DeepCoreML-0.3.4/DeepCoreML/TextDatasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
         In both cases, the following four filters are applied:
          * tokenization
          * case folding,
          * punctuation removal and
          * stopword removal.
         """
-        self.df_.columns.values[self.feature_columns_] = '_text_'
-        self.df_.columns.values[self.class_column_] = '_class_'
+        self.df_.columns.values[self._feature_columns] = '_text_'
+        self.df_.columns.values[self._class_column] = '_class_'
 
         self.df_['_text_'].replace('', np.nan, inplace=True)
         self.df_.dropna(subset=['_text_'], inplace=True)
 
         t0 = time.time()
         preprocessor = TextPreprocessor()
 
@@ -69,17 +69,17 @@
         """
         print("\tText Vectorization with", vectorizer, "... ", end="", flush=True)
 
         raw_data = self.df_['_clean_text_'].to_numpy()
 
         vector_data = vectorizer.fit_transform(raw_data)
         self.vectorization_time_ = vectorizer.vectorization_time_
-        self.dimensionality_ = vectorizer.get_dimensionality()
+        self._dimensionality = vectorizer.get_dimensionality()
 
-        print("completed in %5.2f sec (dimensionality = %d)." % (self.vectorization_time_, self.dimensionality_))
+        print("completed in %5.2f sec (dimensionality = %d)." % (self.vectorization_time_, self._dimensionality))
         return vector_data
 
     def get_preprocessing_time(self):
         """
         :return: The dataset preprocessing dataset
         """
         return self.preprocessing_time_
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/TextPreprocessor.py` & `DeepCoreML-0.3.4/DeepCoreML/TextPreprocessor.py`

 * *Files identical despite different names*

### Comparing `DeepCoreML-0.3.3/DeepCoreML/TextVectorizers.py` & `DeepCoreML-0.3.4/DeepCoreML/TextVectorizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         """
         A simple invocation to the transform method of sklearn's tfIdfvectorizer
         :param x: Input raw text to be transformed by the tfIdfvectorizer
         :return: text vectors of length self.latent_dimensionality_
         """
         return self.vectorizer_.transform(x)
 
-    def fit_transform(self, x, y):
+    def fit_transform(self, x, y=None):
         self.vectorizer_.fit(x)
         x_vec = self.vectorizer_.transform(x)
         return x_vec
 
 
 # ####################################################################################################################
 # word2vecVectorizer #################################################################################################
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/generators/BaseGenerators.py` & `DeepCoreML-0.3.4/DeepCoreML/generators/BaseGenerators.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 
 import torch
-import torch.nn as nn
 
 from sklearn.preprocessing import OneHotEncoder
 
 
 class BaseGenerator:
     """`BaseGenerator` provides the base class for all generative models.
 
@@ -40,30 +39,34 @@
         pac: Number of samples to group together when applying the discriminator.
         adaptive: boolean value to enable/disable adaptive training.
         g_activation: The activation function of the Generator's output layer.
         epochs: Number of training epochs.
         batch_size: Number of data instances per training batch.
         lr: Learning rate parameter for the Generator/Discriminator Adam optimizers.
         decay: Weight decay parameter for the Generator/Discriminator Adam optimizers.
+        sampling_mode:
+         - `balance`: perform oversampling on the minority classes to establish class imbalance in the dataset
+         - `reproduce`: create a new dataset with the same class distribution as the input dataset
         random_state: An integer for seeding the involved random number generators.
     """
-    def __init__(self, embedding_dim, discriminator, generator, pac, adaptive, g_activation, epochs, batch_size,
-                 lr, decay, random_state):
+    def __init__(self, embedding_dim, discriminator, generator, pac, g_activation, adaptive, epochs, batch_size,
+                 lr, decay, sampling_mode, random_state):
 
         super().__init__(epochs, batch_size, random_state)
 
         self.embedding_dim_ = embedding_dim     # Size of the random sample passed to the Generator.
         self.gen_activation_ = g_activation     # The activation function of the Generator's output layer
         self.batch_norm_ = True                 # Sets/unsets 1D-Batch Normalization in the Generator
         self.adaptive_ = adaptive               # Enables/Disables GAN adaptive training
         self.test_classifier_ = None            # Optional classification model for evaluating the GAN's effectiveness
         self.pac_ = pac                         # Number of samples to group together when applying the discriminator.
         self._lr = lr                           # Learning rate param for the Generator/Discriminator Adam optimizers.
         self._decay = decay                     # Weight decay param for the Generator/Discriminator Adam optimizers.
         self._transformer = None                # Input data transformer (normalizers)
+        self._sampling_mode = sampling_mode     # Used in `fit_resample`: Given an input dataset, how GAN generates data
 
         # Discriminator parameters (object, architecture, optimizer)
         self.D_ = None
         self.D_Arch_ = discriminator
         self.D_optimizer_ = None
 
         # Generator parameters (object, architecture, optimizer)
@@ -112,64 +115,26 @@
             x_class_data = np.array([x_train[r, :] for r in range(y_train.shape[0]) if y_train[r, y] == 1])
             x_class_data = torch.from_numpy(x_class_data).to(torch.float32).to(self._device)
 
             self._samples_per_class.append(x_class_data)
 
         return training_data
 
-    # Use GAN's Generator to create artificial samples i) either from a specific class, ii) or from a random class.
-    def sample(self, num_samples, y=None):
-        """ Create artificial samples using the GAN's Generator.
-
-        Args:
-            num_samples: The number of samples to generate.
-            y: The class of the generated samples. If `None`, then samples with random classes are generated.
-
-        Returns:
-            Artificial data instances created by the Generator.
-        """
-        if y is None:
-            latent_classes = torch.from_numpy(np.random.randint(0, self._n_classes, num_samples)).to(torch.int64)
-            latent_y = nn.functional.one_hot(latent_classes, num_classes=self._n_classes)
-        else:
-            latent_y = nn.functional.one_hot(torch.full(size=(num_samples,), fill_value=y), num_classes=self._n_classes)
-
-        latent_x = torch.randn((num_samples, self.embedding_dim_))
-
-        # concatenate, copy to device, and pass to generator
-        latent_data = torch.cat((latent_x, latent_y), dim=1).to(self._device)
-
-        # Generate data from the model's Generator - The feature values of the generated samples fall into the range:
-        # [-1,1]: if the activation function of the output layer of the Generator is nn.Tanh().
-        # [0,1]: if the activation function of the output layer of the Generator is nn.Sigmoid().
-
-        generated_samples = self.G_(latent_data).cpu().detach().numpy()
-        # print("Generated Samples:\n", generated_samples)
-        reconstructed_samples = self._transformer.inverse_transform(generated_samples)
-        # print("Reconstructed samples\n", reconstructed_samples)
-        return reconstructed_samples
-
-    def base_fit_resample(self, x_train, y_train):
-        generated_data = [None for _ in range(self._n_classes)]
-
-        majority_class = np.array(self._gen_samples_ratio).argmax()
-        num_majority_samples = np.max(np.array(self._gen_samples_ratio))
-
-        x_over_train = np.copy(x_train)
-        y_over_train = np.copy(y_train)
-
+    def synthesize_dataset(self):
+        i = 0
+        x_synthetic, y_synthetic = None, None
         for cls in range(self._n_classes):
-            if cls != majority_class:
-                samples_to_generate = num_majority_samples - self._gen_samples_ratio[cls]
-
-                # print("\tSampling Class y:", y, " Gen Samples ratio:", gen_samples_ratio[y])
-                generated_data[cls] = self.sample(samples_to_generate, cls)
-
-                min_classes = np.full(samples_to_generate, cls)
+            # print("Sampling class", cls, "Create", self._gen_samples_ratio[cls], "samples")
+            samples_to_generate = self._gen_samples_ratio[cls]
 
-                x_over_train = np.vstack((x_over_train, generated_data[cls]))
-                y_over_train = np.hstack((y_over_train, min_classes))
+            generated_samples = self.sample(samples_to_generate, cls)
+            generated_classes = np.full(samples_to_generate, cls)
 
-        # balanced_data = np.hstack((x_over_train, y_over_train.reshape((-1, 1))))
-        # return balanced_data
+            if i == 0:
+                x_synthetic = generated_samples
+                y_synthetic = generated_classes
+            else:
+                x_synthetic = np.vstack((x_synthetic, generated_samples))
+                y_synthetic = np.hstack((y_synthetic, generated_classes))
+            i += 1
 
-        return x_over_train, y_over_train
+        return x_synthetic, y_synthetic
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/generators/DataTransformers.py` & `DeepCoreML-0.3.4/DeepCoreML/generators/DataTransformers.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,39 +65,51 @@
         """
         column_name = data.columns[0]
         max_val = data.max()
         min_val = data.min()
 
         cti = None
         if self._cont_normalizer == 'gm':
-            gm = ClusterBasedNormalizer(model_missing_values=True, max_clusters=min(len(data), self._max_clusters))
-            gm.fit(data, column_name)
-            num_components = sum(gm.valid_component_indicator)
+            tran = ClusterBasedNormalizer(model_missing_values=True, max_clusters=min(len(data), self._max_clusters))
+            tran.fit(data, column_name)
+            num_components = sum(tran.valid_component_indicator)
 
-            cti = ColumnTransformInfo(column_name=column_name, column_type='continuous', transform=gm,
+            cti = ColumnTransformInfo(column_name=column_name, column_type='continuous', transform=tran,
                                       column_max=max_val, column_min=min_val,
                                       output_info=[SpanInfo(1, 'tanh'), SpanInfo(num_components, 'softmax')],
                                       output_dimensions=1 + num_components)
 
         elif self._cont_normalizer == 'gmo':
-            gm = ClusterBasedNormalizer(model_missing_values=True, max_clusters=min(len(data), self._max_clusters))
-            gm.fit(data, column_name)
+            tran = ClusterBasedNormalizer(model_missing_values=True, max_clusters=min(len(data), self._max_clusters))
+            tran.fit(data, column_name)
 
-            cti = ColumnTransformInfo(column_name=column_name, column_type='continuous', transform=gm,
+            cti = ColumnTransformInfo(column_name=column_name, column_type='continuous', transform=tran,
                                       column_max=max_val, column_min=min_val,
                                       output_info=[SpanInfo(1, 'tanh')], output_dimensions=1)
 
         elif self._cont_normalizer == 'ss':
+            tran = StandardScaler(with_mean=self._with_mean, with_std=self._with_std)
+            tran.fit(data)
+
+            cti = ColumnTransformInfo(column_name=column_name, column_type='continuous', transform=tran,
+                                      column_max=max_val, column_min=min_val,
+                                      output_info=[SpanInfo(1, 'tanh')], output_dimensions=1)
+        '''
+        elif self._cont_normalizer == 'ss-pca':
+            tran = Pipeline([
+                ('scaler', StandardScaler(with_mean=True, with_std=True)),
+                ('pca', PCA(n_components=self._input_dim, random_state=self._random_state))
+            ])
             ss = StandardScaler(with_mean=self._with_mean, with_std=self._with_std)
             ss.fit(data)
 
             cti = ColumnTransformInfo(column_name=column_name, column_type='continuous', transform=ss,
                                       column_max=max_val, column_min=min_val,
                                       output_info=[SpanInfo(1, 'tanh')], output_dimensions=1)
-
+        '''
         return cti
 
     def _fit_discrete(self, data):
         """Fit one hot encoder for discrete column.
 
         Args:
             data (pd.DataFrame): A dataframe containing a column.
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/generators/c_gan.py` & `DeepCoreML-0.3.4/DeepCoreML/generators/c_gan.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,16 +19,17 @@
     by providing both the Generator and the Discriminator the input feature vectors concatenated
     with their respective one-hot-encoded class labels.
 
     A Packed Conditional GAN (Pac cGAN) is a cGAN that accepts input samples in packs. Pac cGAN
     uses a Packed Discriminator to prevent the model from mode collapsing.
     """
 
-    def __init__(self, embedding_dim=128, discriminator=(128, 128), generator=(256, 256), pac=10, adaptive=False,
-                 g_activation='tanh', epochs=300, batch_size=32, lr=2e-4, decay=1e-6, random_state=0):
+    def __init__(self, embedding_dim=128, discriminator=(128, 128), generator=(256, 256), pac=10, g_activation='tanh',
+                 adaptive=False, epochs=300, batch_size=32, lr=2e-4, decay=1e-6, sampling_mode='balance',
+                 random_state=0):
 
         """Initializes a Packed Conditional GAN.
 
         Args:
             embedding_dim: Size of the random sample passed to the Generator.
             discriminator: a tuple with number of neurons in each fully connected layer of the Discriminator. Each
                 number determines the dimensionality of the output of each layer.
@@ -39,16 +40,16 @@
             g_activation: The activation function of the Generator's output layer.
             epochs: Number of training epochs.
             batch_size: Number of data instances per training batch.
             lr: Learning rate parameter for the Generator/Discriminator Adam optimizers.
             decay: Weight decay parameter for the Generator/Discriminator Adam optimizers.
             random_state: An integer for seeding the involved random number generators.
         """
-        super().__init__(embedding_dim, discriminator, generator, pac, adaptive, g_activation, epochs, batch_size,
-                         lr, decay, random_state)
+        super().__init__(embedding_dim, discriminator, generator, pac, g_activation, adaptive, epochs, batch_size,
+                         lr, decay, sampling_mode, random_state)
 
     def train_batch(self, real_data):
         """
         Given a batch of input data, `train_batch` updates the Discriminator and Generator weights using the respective
         optimizers and back propagation.
 
         Args:
@@ -268,27 +269,117 @@
 
             print("Epoch %4d \t Loss D.=%5.4f \t Loss G.=%5.4f \t Mean Acc=%5.4f \t Mean KLD=%5.4f" %
                   (epoch + 1, disc_loss, gen_loss, float(mean_met[epoch]), float(mean_kld[epoch])))
 
         return generated_data, (mean_met, mean_kld)
 
     def fit(self, x_train, y_train):
-        """`fit` invokes the GAN training process. `fit` renders the cGAN class compatible with `imblearn`'s interface,
+        """`fit` invokes the GAN training process. `fit` renders cGAN compatible with `imblearn`'s interface,
         allowing its usage in over-sampling/under-sampling pipelines.
 
         Args:
             x_train: The training data instances.
             y_train: The classes of the training data instances.
         """
         self.train(x_train, y_train)
 
+    # Use GAN's Generator to create artificial samples i) either from a specific class, ii) or from a random class.
+    def sample(self, num_samples, y=None):
+        """ Create artificial samples using the GAN's Generator.
+
+        Args:
+            num_samples: The number of samples to generate.
+            y: The class of the generated samples. If `None`, then samples with random classes are generated.
+
+        Returns:
+            Artificial data instances created by the Generator.
+        """
+        if y is None:
+            latent_classes = torch.from_numpy(np.random.randint(0, self._n_classes, num_samples)).to(torch.int64)
+            latent_y = nn.functional.one_hot(latent_classes, num_classes=self._n_classes)
+        else:
+            latent_y = nn.functional.one_hot(torch.full(size=(num_samples,), fill_value=y), num_classes=self._n_classes)
+
+        latent_x = torch.randn((num_samples, self.embedding_dim_))
+
+        # concatenate, copy to device, and pass to generator
+        latent_data = torch.cat((latent_x, latent_y), dim=1).to(self._device)
+
+        # Generate data from the model's Generator - The feature values of the generated samples fall into the range:
+        # [-1,1]: if the activation function of the output layer of the Generator is nn.Tanh().
+        # [0,1]: if the activation function of the output layer of the Generator is nn.Sigmoid().
+
+        generated_samples = self.G_(latent_data).cpu().detach().numpy()
+        # print("Generated Samples:\n", generated_samples)
+
+        reconstructed_samples = self._transformer.inverse_transform(generated_samples)
+        # print("Reconstructed samples\n", reconstructed_samples)
+        return reconstructed_samples
+
     def fit_resample(self, x_train, y_train):
-        """`fit_transform` invokes the GAN training process. `fit_transform` renders the cGAN class compatible with
-        `imblearn`'s interface, allowing its usage in over-sampling/under-sampling pipelines.
+        """`fit_resample` alleviates the problem of class imbalance in imbalanced datasets. The function renders cGAN
+        compatible with the `imblearn`'s interface, allowing its usage in over-sampling/under-sampling pipelines.
+
+        In the `fit` part, the input dataset is used to train cGAN. In the `resample` part, cGAN is employed to
+        generate synthetic data according to the value of `self._sampling_mode`:
+
+        - 'balance': the model equalizes the number of samples from each class by oversampling the minority classes.
+        - 'synthesize_similar': the model synthesizes a new dataset with identical class distribution as the train set.
 
         Args:
             x_train: The training data instances.
             y_train: The classes of the training data instances.
         """
+
+        # Train the GAN with the input data
         self.train(x_train, y_train)
 
-        return self.base_fit_resample(x_train, y_train)
+        # balance mode: Use the GAN to equalize the number of samples per class. This is achieved by generating
+        # samples of the minority classes (i.e. we perform oversampling).
+        if self._sampling_mode == 'balance':
+            majority_class = np.array(self._gen_samples_ratio).argmax()
+            num_majority_samples = np.max(np.array(self._gen_samples_ratio))
+
+            x_balanced = np.copy(x_train)
+            y_balanced = np.copy(y_train)
+
+            # Perform oversampling
+            for cls in range(self._n_classes):
+                if cls != majority_class:
+                    samples_to_generate = num_majority_samples - self._gen_samples_ratio[cls]
+
+                    # Generate the appropriate number of samples to equalize cls with the majority class.
+                    # print("\tSampling Class y:", cls, " Gen Samples ratio:", gen_samples_ratio[cls])
+                    generated_samples = self.sample(samples_to_generate, cls)
+                    generated_classes = np.full(samples_to_generate, cls)
+
+                    x_balanced = np.vstack((x_balanced, generated_samples))
+                    y_balanced = np.hstack((y_balanced, generated_classes))
+
+            # Return balanced_data
+            return x_balanced, y_balanced
+
+        # synthesize_similar mode: Use the GAN to create a new dataset with identical class distribution
+        # as the training set.
+        elif self._sampling_mode == 'synthesize_similar':
+            i = 0
+            x_synthetic = None
+            y_synthetic = None
+
+            # Perform oversampling
+            for cls in range(self._n_classes):
+                # print("Sampling class", cls, "Create", self._gen_samples_ratio[cls], "samples")
+                samples_to_generate = self._gen_samples_ratio[cls]
+
+                generated_samples = self.sample(samples_to_generate, cls)
+                generated_classes = np.full(samples_to_generate, cls)
+
+                if i == 0:
+                    x_synthetic = generated_samples
+                    y_synthetic = generated_classes
+                else:
+                    x_synthetic = np.vstack((x_synthetic, generated_samples))
+                    y_synthetic = np.hstack((y_synthetic, generated_classes))
+                i += 1
+
+            # Return balanced_data
+            return x_synthetic, y_synthetic
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/generators/cbr.py` & `DeepCoreML-0.3.4/DeepCoreML/generators/cbr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# CBR: Cluster-Based Resampler
+# This method was introduced in the following paper:
+# L. Akritidis, P. Bozanis, "A Clustering-Based Resampling Technique with Cluster Structure Analysis for Software Defect
+# Detection in Imbalanced Datasets", Information Sciences, 2024.
+
 import numpy as np
 
 from sklearn.cluster import DBSCAN, AgglomerativeClustering
 from sklearn.metrics.pairwise import euclidean_distances
 
 from imblearn.over_sampling import SMOTE
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/generators/cluster_gan.py` & `DeepCoreML-0.3.4/DeepCoreML/generators/sb_gan.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,42 @@
-# Conditional GAN Implementation
+# SB-GAN: Safe-Borderline Generative Adversarial Net
+# This generative model was introduced in the following paper:
+# L. Akritidis, A. Fevgas, M. Alamaniotis, P. Bozanis, "Conditional Data Synthesis with Deep Generative Models for
+# Imbalanced Dataset Oversampling", In Proceedings of the 35th IEEE International Conference on Tools with Artificial
+# Intelligence (ICTAI), pp. 444-451, 2023.
+
 import numpy as np
 import torch
 import torch.nn as nn
-from torch.distributions import Categorical
 
 from torch.utils.data import DataLoader
 
-from sklearn.cluster import AgglomerativeClustering
-from sklearn.metrics import accuracy_score
-from sklearn.metrics.pairwise import euclidean_distances
-
-from sklearn.mixture import GaussianMixture
-from sklearn.preprocessing import StandardScaler, OneHotEncoder
-from sklearn.decomposition import PCA
-from sklearn.pipeline import Pipeline
+from sklearn.neighbors import KDTree
 
 from .DataTransformers import DataTransformer
 from .gan_discriminators import PackedDiscriminator
 from .gan_generators import Generator
 from .BaseGenerators import BaseGAN
 
 
-class clusterGAN(BaseGAN):
+class sbGAN(BaseGAN):
     """
     Safe-Borderline GAN
 
     Conditional GANs (cGANs) conditionally generate data from a specific class. They are trained
     by providing both the Generator and the Discriminator the input feature vectors concatenated
     with their respective one-hot-encoded class labels.
 
     A Packed Conditional GAN (Pac cGAN) is a cGAN that accepts input samples in packs. Pac cGAN
     uses a Packed Discriminator to prevent the model from mode collapsing.
     """
 
-    def __init__(self, embedding_dim=128, discriminator=(128, 128), generator=(256, 256), pac=10, adaptive=False,
-                 g_activation='tanh', epochs=300, batch_size=32, lr=2e-4, decay=1e-6, min_distance_factor=2,
-                 random_state=0):
+    def __init__(self, embedding_dim=128, discriminator=(128, 128), generator=(256, 256), pac=10, g_activation='tanh',
+                 adaptive=False, epochs=300, batch_size=32, lr=2e-4, decay=1e-6, sampling_mode='balance',
+                 method='knn', k=5, r=10, random_state=0):
         """
         Initializes a Safe-Borderline Conditional GAN.
 
         Args:
             embedding_dim: Size of the random sample passed to the Generator.
             discriminator: a tuple with number of neurons in each fully connected layer of the Discriminator. It
                 determines the dimensionality of the output of each layer.
@@ -48,140 +45,97 @@
             pac: Number of samples to group together when applying the discriminator.
             adaptive: boolean value to enable/disable adaptive training.
             g_activation: The activation function of the Generator's output layer.
             epochs: Number of training epochs.
             batch_size: Number of data instances per training batch.
             lr: Learning rate parameter for the Generator/Discriminator Adam optimizers.
             decay: Weight decay parameter for the Generator/Discriminator Adam optimizers.
-            min_distance_factor:
+            method: 'knn': k-nearest neighbors / 'rad': neighbors inside a surrounding hypersphere.
+            k: The number of nearest neighbors to retrieve; applied when `method='knn'`.
+            r: The radius of the hypersphere that includes the neighboring samples; applied when `method='rad'`.
             random_state: An integer for seeding the involved random number generators.
         """
-        super().__init__(embedding_dim, discriminator, generator, pac, adaptive, g_activation, epochs, batch_size,
-                         lr, decay, random_state)
+        super().__init__(embedding_dim, discriminator, generator, pac, g_activation, adaptive, epochs, batch_size,
+                         lr, decay, sampling_mode, random_state)
 
-        self._min_distance_factor = min_distance_factor
-        self._n_clusters = 0
-        self._cluster_class_distribution = []
+        self._method = method
+        self._n_neighbors = k
+        self._radius = r
 
-    def cluster_prepare(self, x_train, y_train):
+    def select_prepare(self, x_train, y_train):
         """
         Refine the training set with sample filtering. It invokes `prepare` to return the preprocessed data.
 
         Args:
             x_train: The training data instances.
             y_train: The classes of the training data instances.
 
         Returns:
             A tensor with the preprocessed data.
         """
+        num_samples = x_train.shape[0]
 
-        self._n_classes = len(set(y_train))
+        # Array with the point labels.
+        pts_types = ['NotSet'] * num_samples
+        x_sample, y_sample = [], []
+
+        # Build an auxiliary KD-Tree accelerate spatial queries.
+        kd_tree = KDTree(x_train, metric='euclidean', leaf_size=40)
+
+        # Nearest-Neighbors method.
+        if self._method == 'knn':
+            # Query the KD-Tree to find the nearest neighbors. indices contains the indices of the nearest neighbors
+            # in the original dataset -> a row indices[r] contains the 5 nearest neighbors of x_train[r].
+            _, indices = kd_tree.query(x_train, k=self._n_neighbors)
+
+        elif self._method == 'rad':
+            # Query the KD-Tree to find the neighbors-within-hypersphere of radius=radius. indices contains the indices
+            # of the neighbors-within-hypersphere in the original dataset -> a row indices[r] contains the
+            # neighbors-within-hypersphere of x_train[r].
+            indices = kd_tree.query_radius(x_train, r=self._radius)
 
-        # ====== 1. Feature Transformation Step: First standardize, then project to a latent space of max variance.
-        self._input_dim = x_train.shape[1]
-        self._transformer = Pipeline([
-                ('scaler', StandardScaler(with_mean=True, with_std=True)),
-                ('pca', PCA(n_components=self._input_dim))
-            ])
+        else:
+            print("method should be 'knn' or 'rad'; returning the input dataset")
+            return self.prepare(x_train, y_train)
 
-        self._transformer.fit(x_train)
-        x_train_projected = self._transformer.transform(x_train)
+        # For each sample in the dataset
+        for m in range(num_samples):
+            pts_with_same_class = 0
+
+            # Examine its nearest neighbors and assign a label: core/border/outlier/isolated
+            num_neighbors = len(indices[m])
+            for k in range(num_neighbors):
+                nn_idx = indices[m][k]
+                if y_train[nn_idx] == y_train[m]:
+                    pts_with_same_class += 1
+
+            if num_neighbors == 1:
+                pts_types[m] = 'Isolated'
+            else:
+                t_high = 1.0 * num_neighbors
+                t_low = 0.2 * num_neighbors
+
+                if pts_with_same_class >= t_high:
+                    pts_types[m] = 'Core'
+                    # x_sample.append(x_train[m])
+                    # y_sample.append(y_train[m])
+                elif t_high > pts_with_same_class > t_low:
+                    pts_types[m] = 'Border'
+                    x_sample.append(x_train[m])
+                    y_sample.append(y_train[m])
+                else:
+                    pts_types[m] = 'Outlier'
 
-        # ====== 2. Clustering step
-        n_components = range(1, 30)
-        covariance_type = ['spherical', 'tied', 'diag', 'full']
-        score = []
-        for cov in covariance_type:
-            for n_comp in n_components:
-                gmm = GaussianMixture(n_components=n_comp, covariance_type=cov, random_state=self._random_state)
-                gmm.fit(x_train)
-                score.append((cov, n_comp, gmm.bic(x_train)))
-
-        best = min(score, key=lambda tup: tup[2])
-        self._n_clusters = best[1]
-        best_cov = best[0]
-        print(best)
-
-        gmm = GaussianMixture(n_components=self._n_clusters, covariance_type=best_cov, random_state=self._random_state)
-        gmm.fit(x_train)
-        cluster_labels = gmm.predict(x_train)
-
-        '''
-        # First, Apply a simple heuristic to get the max distance between two clusters.
-        # Compute the distances and get the median, then divide the median by self._min_distance_factor
-        e_dists = euclidean_distances(x_train, x_train)
-        med = np.median(e_dists)
-        eps = med / self._min_distance_factor
-
-        clustering_method = AgglomerativeClustering(distance_threshold=eps, n_clusters=None, affinity='euclidean',
-                                                    linkage='ward')
-        clustering_method.fit(x_train_projected)
-        cluster_labels = clustering_method.labels_
-
-        # 3. One hot encode the cluster labels
-        self._n_clusters = len(set(cluster_labels))
-        cluster_encoder = OneHotEncoder()
-        cluster_encoded_data = cluster_encoder.fit_transform(cluster_labels.reshape(-1, 1)).toarray()
-        # print(cluster_encoded_data)
-
-        clustering_method = AgglomerativeClustering(distance_threshold=eps, n_clusters=None, linkage='ward')
-        clustering_method.fit(x_train_projected)
-        self._n_clusters = len(set(clustering_method.labels_))
-        cluster_labels = clustering_method.labels_
-
-        while self._n_clusters < 50:
-            eps /= 2
-
-            clustering_method = AgglomerativeClustering(distance_threshold=eps, n_clusters=None, linkage='ward')
-            clustering_method.fit(x_train_projected)
-            self._n_clusters = len(set(cluster_labels))
-            print("\tNew num_clusters:", self._n_clusters)
-            cluster_labels = clustering_method.labels_
-        '''
-
-        # 3. One hot encode the cluster labels
-        cluster_encoder = OneHotEncoder()
-        cluster_encoded_data = cluster_encoder.fit_transform(cluster_labels.reshape(-1, 1)).toarray()
-        # print(cluster_encoded_data)
-
-        # 4. Get class distributions per cluster
-        # If a cluster has 10 samples from class 0 and 20 samples from class 1, then create the list lcd=[10, 20]
-        # self._cluster_class_distribution stores one such lcd list per cluster.
-        for cluster in range(self._n_clusters):
-            y_cluster_all = y_train[cluster_labels == cluster]
-
-            lcd = [len(y_cluster_all[y_cluster_all == c]) for c in range(self._n_classes)]
-            # print("Cluster:", cluster, " === Classes", y_cluster_all, " ==== ", lcd)
-            self._cluster_class_distribution.append(lcd)
-        # print("self._cluster_class_distribution", self._cluster_class_distribution)
-
-        # 5. One hot encode the class labels
-        class_encoder = OneHotEncoder()
-        y_train = class_encoder.fit_transform(y_train.reshape(-1, 1)).toarray()
-
-        # 6. Concatenate everything (x_train, ohe_clusters, ohe_classes)
-        train_data = np.concatenate((x_train_projected, cluster_encoded_data, y_train), axis=1)
-        training_data = torch.from_numpy(train_data).to(torch.float32)
-
-        # print(training_data)
-        # print("Shapes:\n\tClusters:", cluster_encoded_data.shape, "\n\tClasses:", y_train.shape,
-        #      "\n\tFeatures:", x_train_projected.shape, "\n\tTraining set:", training_data.shape)
-
-        # Determine how to draw samples from the GAN's Generator
-        self._gen_samples_ratio = [int(sum(y_train[:, c])) for c in range(self._n_classes)]
-
-        # Class specific training data
-        self._samples_per_class = []
-        for y in range(self._n_classes):
-            x_class_data = np.array([x_train_projected[r, :] for r in range(y_train.shape[0]) if y_train[r, y] == 1])
-            x_class_data = torch.from_numpy(x_class_data).to(torch.float32).to(self._device)
+            # print("Sample", m, ":", pts_types[m], "- Neighbors indices:", indices[m], "- Neighbors classes:",
+            #      [y_train[indices[m][k]] for k in range(num_neighbors)])
 
-            self._samples_per_class.append(x_class_data)
+        x_train = np.array(x_sample)
+        y_train = np.array(y_sample)
 
-        return training_data
+        return self.prepare(x_train, y_train)
 
     def train_batch(self, real_data):
         """
         Given a batch of input data, `train_batch` updates the Discriminator and Generator weights using the respective
         optimizers and back propagation.
 
         Args:
@@ -204,96 +158,93 @@
         self.D_optimizer_.zero_grad()
 
         # 1. Randomly take samples from a normal distribution
         # 2. Assign one-hot-encoded random classes
         # 3. Pass the fake data (samples + classes) to the Generator
         latent_x = torch.randn((num_samples, self.embedding_dim_))
         latent_classes = torch.from_numpy(np.random.randint(0, self._n_classes, num_samples)).to(torch.int64)
-        latent_classes_ohe = nn.functional.one_hot(latent_classes, num_classes=self._n_classes)
-        latent_clusters = torch.from_numpy(np.random.randint(0, self._n_clusters, num_samples)).to(torch.int64)
-        latent_clusters_ohe = nn.functional.one_hot(latent_clusters, num_classes=self._n_clusters)
-        latent_y = torch.cat((latent_clusters_ohe, latent_classes_ohe), dim=1)
+        latent_y = nn.functional.one_hot(latent_classes, num_classes=self._n_classes)
         latent_data = torch.cat((latent_x, latent_y), dim=1)
 
         # 4. The Generator produces fake samples (their labels are 0)
         fake_x = self.G_(latent_data.to(self._device))
         fake_labels = torch.zeros((packed_samples, 1))
 
         # 5. The real samples (coming from the dataset) with their one-hot-encoded classes are assigned labels eq. to 1.
         real_x = real_data[:, 0:self._input_dim]
-        real_y = real_data[:, self._input_dim:(self._input_dim + self._n_classes + self._n_clusters)]
+        real_y = real_data[:, self._input_dim:(self._input_dim + self._n_classes)]
         real_labels = torch.ones((packed_samples, 1))
         # print(real_x.shape, real_y.shape)
 
         # 6. Mix (concatenate) the fake samples (from Generator) with the real ones (from the dataset).
         all_x = torch.cat((real_x.to(self._device), fake_x))
         all_y = torch.cat((real_y, latent_y)).to(self._device)
         all_labels = torch.cat((real_labels, fake_labels)).to(self._device)
         all_data = torch.cat((all_x, all_y), dim=1)
 
         # 7. Reshape the data to feed it to Discriminator (num_samples, dimensionality) -> (-1, pac * dimensionality)
         # The samples are packed according to self.pac parameter.
-        all_data = all_data.reshape((-1, self.pac_ * (self._input_dim + self._n_classes + self._n_clusters)))
+        all_data = all_data.reshape((-1, self.pac_ * (self._input_dim + self._n_classes)))
 
         # 8. Pass the mixed data to the Discriminator and train the Discriminator (update its weights with backprop).
         # The loss function quantifies the Discriminator's ability to classify a real/fake sample as real/fake.
         d_predictions = self.D_(all_data)
         disc_loss = loss_function(d_predictions, all_labels)
         disc_loss.backward()
         self.D_optimizer_.step()
 
         # GENERATOR TRAINING
         self.G_optimizer_.zero_grad()
 
         latent_x = torch.randn((num_samples, self.embedding_dim_))
         latent_classes = torch.from_numpy(np.random.randint(0, self._n_classes, num_samples)).to(torch.int64)
-        latent_classes_ohe = nn.functional.one_hot(latent_classes, num_classes=self._n_classes)
-        latent_clusters = torch.from_numpy(np.random.randint(0, self._n_clusters, num_samples)).to(torch.int64)
-        latent_clusters_ohe = nn.functional.one_hot(latent_clusters, num_classes=self._n_clusters)
-        latent_y = torch.cat((latent_clusters_ohe, latent_classes_ohe), dim=1)
+        latent_y = nn.functional.one_hot(latent_classes, num_classes=self._n_classes)
         latent_data = torch.cat((latent_x, latent_y), dim=1)
 
         fake_x = self.G_(latent_data.to(self._device))
 
         all_data = torch.cat((fake_x, latent_y.to(self._device)), dim=1)
 
         # Reshape the data to feed it to Discriminator ( (num_samples, dimensionality) -> ( -1, pac * dimensionality )
-        all_data = all_data.reshape((-1, self.pac_ * (self._input_dim + self._n_classes + self._n_clusters)))
+        all_data = all_data.reshape((-1, self.pac_ * (self._input_dim + self._n_classes)))
 
         d_predictions = self.D_(all_data)
 
         gen_loss = loss_function(d_predictions, real_labels.to(self._device))
         gen_loss.backward()
         self.G_optimizer_.step()
 
         return disc_loss, gen_loss
 
     def train(self, x_train, y_train):
         """
-        Conventional training process of a Cluster GAN. The Generator and the Discriminator are trained
+        Conventional training process of a Packed SBGAN. The Generator and the Discriminator are trained
         simultaneously in the traditional adversarial fashion by optimizing `loss_function`.
 
         Args:
             x_train: The training data instances.
             y_train: The classes of the training data instances.
         """
         # Modify the size of the batch to align with self.pac_
         factor = self._batch_size // self.pac_
         batch_size = factor * self.pac_
 
+        self._transformer = DataTransformer(cont_normalizer='ss')
+        self._transformer.fit(x_train)
+        x_train = self._transformer.transform(x_train)
+
         # select_prepare: implemented in BaseGenerators.py
-        training_data = self.cluster_prepare(x_train, y_train)
+        training_data = self.select_prepare(x_train, y_train)
 
         train_dataloader = DataLoader(training_data, batch_size=batch_size, shuffle=True)
 
-        self.D_ = PackedDiscriminator(self.D_Arch_, input_dim=self._input_dim + self._n_classes + self._n_clusters,
+        self.D_ = PackedDiscriminator(self.D_Arch_, input_dim=self._input_dim + self._n_classes,
                                       pac=self.pac_).to(self._device)
-        self.G_ = (Generator(self.G_Arch_, input_dim=self.embedding_dim_ + self._n_classes + self._n_clusters,
-                             output_dim=self._input_dim, activation=self.gen_activation_, normalize=self.batch_norm_).
-                   to(self._device))
+        self.G_ = Generator(self.G_Arch_, input_dim=self.embedding_dim_ + self._n_classes, output_dim=self._input_dim,
+                            activation=self.gen_activation_, normalize=self.batch_norm_).to(self._device)
 
         self.D_optimizer_ = torch.optim.Adam(self.D_.parameters(),
                                              lr=self._lr, weight_decay=self._decay, betas=(0.5, 0.9))
         self.G_optimizer_ = torch.optim.Adam(self.G_.parameters(),
                                              lr=self._lr, weight_decay=self._decay, betas=(0.5, 0.9))
 
         disc_loss, gen_loss = 0, 0
@@ -313,88 +264,109 @@
 
         Args:
             x_train: The training data instances.
             y_train: The classes of the training data instances.
         """
         self.train(x_train, y_train)
 
-    def fit_resample(self, x_train, y_train):
-        """`fit_transform` invokes the GAN training process. `fit_transform` renders the CGAN class compatible with
-        `imblearn`'s interface, allowing its usage in over-sampling/under-sampling pipelines.
-
-        Args:
-            x_train: The training data instances.
-            y_train: The classes of the training data instances.
-        """
-        self.train(x_train, y_train)
-
-        generated_data = [None for _ in range(self._n_classes)]
-
-        majority_class = np.array(self._gen_samples_ratio).argmax()
-        num_majority_samples = np.max(np.array(self._gen_samples_ratio))
-
-        x_over_train = np.copy(x_train)
-        y_over_train = np.copy(y_train)
-
-        for cls in range(self._n_classes):
-            if cls != majority_class:
-                samples_to_generate = num_majority_samples - self._gen_samples_ratio[cls]
-
-                # print("\tSampling Class y:", y, " Gen Samples ratio:", self._gen_samples_ratio[y])
-                generated_data[cls] = self.sample(samples_to_generate, cls)
-
-                min_classes = np.full(samples_to_generate, cls)
-
-                x_over_train = np.vstack((x_over_train, generated_data[cls]))
-                y_over_train = np.hstack((y_over_train, min_classes))
-
-        return x_over_train, y_over_train
+        # Use GAN's Generator to create artificial samples i) either from a specific class, ii) or from a random class.
 
     def sample(self, num_samples, y=None):
         """ Create artificial samples using the GAN's Generator.
 
         Args:
             num_samples: The number of samples to generate.
             y: The class of the generated samples. If `None`, then samples with random classes are generated.
 
         Returns:
             Artificial data instances created by the Generator.
         """
-        probabilities = np.zeros((self._n_classes, self._n_clusters))
-        for clu in range(self._n_clusters):
-            for cls in range(self._n_classes):
-                probabilities[cls][clu] = self._cluster_class_distribution[clu][cls]/self._gen_samples_ratio[cls]
-        # print(probabilities)
-
         if y is None:
-            latent_clusters = torch.from_numpy(np.random.randint(0, self._n_clusters, num_samples)).to(torch.int64)
-            latent_clusters_ohe = nn.functional.one_hot(latent_clusters, num_classes=self._n_clusters)
-
             latent_classes = torch.from_numpy(np.random.randint(0, self._n_classes, num_samples)).to(torch.int64)
-            latent_classes_ohe = nn.functional.one_hot(latent_classes, num_classes=self._n_classes)
+            latent_y = nn.functional.one_hot(latent_classes, num_classes=self._n_classes)
         else:
-            # The part of the conditional vector that concerns the clusters
-            mix = Categorical(torch.tensor(probabilities[y]))
-            latent_clusters = mix.sample(sample_shape=torch.Size([num_samples]))
-            # print("Sampling class", y, latent_clusters)
-            latent_clusters_ohe = nn.functional.one_hot(
-                latent_clusters, num_classes=self._n_clusters)
-
-            # The part of the conditional vector that concerns the classes
-            latent_classes_ohe = nn.functional.one_hot(
-                torch.full(size=(num_samples,), fill_value=y), num_classes=self._n_classes)
+            latent_y = nn.functional.one_hot(torch.full(size=(num_samples,), fill_value=y), num_classes=self._n_classes)
 
-        latent_y = torch.cat((latent_clusters_ohe, latent_classes_ohe), dim=1)
         latent_x = torch.randn((num_samples, self.embedding_dim_))
 
         # concatenate, copy to device, and pass to generator
         latent_data = torch.cat((latent_x, latent_y), dim=1).to(self._device)
 
         # Generate data from the model's Generator - The feature values of the generated samples fall into the range:
         # [-1,1]: if the activation function of the output layer of the Generator is nn.Tanh().
         # [0,1]: if the activation function of the output layer of the Generator is nn.Sigmoid().
 
         generated_samples = self.G_(latent_data).cpu().detach().numpy()
         # print("Generated Samples:\n", generated_samples)
         reconstructed_samples = self._transformer.inverse_transform(generated_samples)
         # print("Reconstructed samples\n", reconstructed_samples)
         return reconstructed_samples
+
+    def fit_resample(self, x_train, y_train):
+        """`fit_resample` alleviates the problem of class imbalance in imbalanced datasets. In particular, this
+         resampling operation equalizes the number of samples from each class by oversampling the minority class.
+         The function renders sbGAN compatible with the `imblearn`'s interface, allowing its usage in
+         over-sampling/under-sampling pipelines.
+
+        Args:
+            x_train: The training data instances.
+            y_train: The classes of the training data instances.
+
+        Returns:
+            x_balanced: the balanced dataset samples
+            y_balanced: the classes of the samples of x_balanced
+        """
+
+        # Train the GAN with the input data
+        self.train(x_train, y_train)
+
+        # balance mode: Use the GAN to equalize the number of samples per class. This is achieved by generating
+        # samples of the minority classes (i.e. we perform oversampling).
+        if self._sampling_mode == 'balance':
+            majority_class = np.array(self._gen_samples_ratio).argmax()
+            num_majority_samples = np.max(np.array(self._gen_samples_ratio))
+
+            x_balanced = np.copy(x_train)
+            y_balanced = np.copy(y_train)
+
+            # Perform oversampling
+            for cls in range(self._n_classes):
+                if cls != majority_class:
+                    samples_to_generate = num_majority_samples - self._gen_samples_ratio[cls]
+
+                    if samples_to_generate > 1:
+                        # Generate the appropriate number of samples to equalize cls with the majority class.
+                        # print("\tSampling Class y:", cls, " Gen Samples ratio:", gen_samples_ratio[cls])
+                        generated_samples = self.sample(samples_to_generate, cls)
+                        generated_classes = np.full(samples_to_generate, cls)
+
+                        x_balanced = np.vstack((x_balanced, generated_samples))
+                        y_balanced = np.hstack((y_balanced, generated_classes))
+
+            # Return balanced_data
+            return x_balanced, y_balanced
+
+        # synthesize_similar mode: Use the GAN to create a new dataset with identical class distribution
+        # as the training set.
+        elif self._sampling_mode == 'synthesize_similar':
+            i = 0
+            x_synthetic = None
+            y_synthetic = None
+
+            # Perform oversampling
+            for cls in range(self._n_classes):
+                # print("Sampling class", cls, "Create", self._gen_samples_ratio[cls], "samples")
+                samples_to_generate = self._gen_samples_ratio[cls]
+
+                generated_samples = self.sample(samples_to_generate, cls)
+                generated_classes = np.full(samples_to_generate, cls)
+
+                if i == 0:
+                    x_synthetic = generated_samples
+                    y_synthetic = generated_classes
+                else:
+                    x_synthetic = np.vstack((x_synthetic, generated_samples))
+                    y_synthetic = np.hstack((y_synthetic, generated_classes))
+                i += 1
+
+            # Return balanced_data
+            return x_synthetic, y_synthetic
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/generators/ct_gan.py` & `DeepCoreML-0.3.4/DeepCoreML/generators/ct_gan.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 
 from .DataTransformers import DataTransformer
 # from .gan_discriminators import PackedDiscriminator
 from .gan_discriminators import ctDiscriminator
 from .gan_generators import ctGenerator
 from .BaseGenerators import BaseGAN
 
-np.set_printoptions(threshold=np.inf, linewidth=250, precision=3, suppress=True,)
-
 
 class DataSampler(object):
     """DataSampler samples the conditional vector and corresponding data for CTGAN."""
 
     def __init__(self, data, output_info, log_frequency):
         self._data = data
 
@@ -181,20 +179,20 @@
         verbose (boolean):
             Whether to have print statements for progress results. Defaults to ``False``.
         epochs (int):
             Number of training epochs. Defaults to 300.
         pac (int):
             Number of samples to group together when applying the discriminator. Defaults to 10.
     """
-    def __init__(self, embedding_dim=128, generator=(256, 256), discriminator=(256, 256), pac=10, adaptive=False,
-                 g_activation=None, epochs=300, batch_size=32, lr=2e-4, decay=1e-6, discriminator_steps=1,
-                 log_frequency=True, verbose=False, random_state=0):
+    def __init__(self, embedding_dim=128, generator=(256, 256), discriminator=(256, 256), pac=10, g_activation=None,
+                 adaptive=False, epochs=300, batch_size=32, lr=2e-4, decay=1e-6, sampling_mode='balance',
+                 discriminator_steps=1, log_frequency=True, verbose=False, random_state=0):
 
-        super().__init__(embedding_dim, discriminator, generator, pac, adaptive, g_activation, epochs, batch_size,
-                         lr, decay, random_state)
+        super().__init__(embedding_dim, discriminator, generator, pac, g_activation, adaptive, epochs, batch_size,
+                         lr, decay, sampling_mode, random_state)
 
         assert batch_size % 2 == 0
 
         self._discriminator_steps = discriminator_steps
         self._log_frequency = log_frequency
         self._verbose = verbose
 
@@ -419,15 +417,36 @@
                 loss_g.backward()
                 self.G_optimizer_.step()
 
             if self._verbose:
                 print(f'Epoch {i+1}, Loss G: {loss_g.detach().cpu(): .4f},'
                       f'Loss D: {loss_d.detach().cpu(): .4f}', flush=True)
 
-    def sample(self, n, condition_column=None, condition_value=None):
+    def fit(self, x_train, y_train):
+        """`fit` invokes the GAN training process. `fit` renders ctGAN compatible with `imblearn`'s interface,
+        allowing its usage in over-sampling/under-sampling pipelines.
+
+        Args:
+            x_train: The training data instances.
+            y_train: The classes of the training data instances.
+        """
+        training_data = np.concatenate((x_train, y_train.reshape((-1, 1))), axis=1)
+
+        self._input_dim = x_train.shape[1]
+
+        # One-hot-encode the class labels; Get the number of classes and the number of samples to generate per class.
+        class_encoder = OneHotEncoder()
+        y_encoded = class_encoder.fit_transform(y_train.reshape(-1, 1)).toarray()
+        self._n_classes = y_encoded.shape[1]
+        self._gen_samples_ratio = [int(sum(y_encoded[:, c])) for c in range(self._n_classes)]
+
+        # Train the ctGAN
+        self.train(training_data, discrete_columns=(self._input_dim,))
+
+    def sample_original(self, n, condition_column=None, condition_value=None):
         """Sample data similar to the training data.
 
         Choosing a condition_column and condition_value will increase the probability of the
         discrete condition_value happening in the condition_column.
 
         Args:
             n (int): Number of rows to sample.
@@ -471,54 +490,96 @@
             data.append(fakeact.detach().cpu().numpy())
 
         data = np.concatenate(data, axis=0)
         data = data[:n]
 
         return self._transformer.inverse_transform(data)
 
-    def set_device(self, device):
-        """Set the `device` to be used ('GPU' or 'CPU)."""
-        self._device = device
-        if self.G_ is not None:
-            self.G_.to(self._device)
+    def sample(self, num_samples, y=None):
+        """Wrapper to the `sample_original` function. It provides a unified interface, similar to the `sample` methods
+        of the other GANs.
+        """
+        return self.sample_original(n=num_samples, condition_column=str(self._input_dim),
+                                    condition_value=y)[:, 0:self._input_dim]
 
     def fit_resample(self, x_train, y_train):
+        """`fit_resample` alleviates the problem of class imbalance in imbalanced datasets. In particular, this
+         resampling operation equalizes the number of samples from each class by oversampling the minority class.
+         The function renders the ctGAN class compatible with the `imblearn`'s interface, allowing its usage in
+         over-sampling/under-sampling pipelines.
+
+        Args:
+            x_train: The training data instances.
+            y_train: The classes of the training data instances.
+
+        Returns:
+            x_balanced: the balanced dataset samples
+            y_balanced: the classes of the samples of x_balanced
+        """
+
         # Create the ctGAN training data
         training_data = np.concatenate((x_train, y_train.reshape((-1, 1))), axis=1)
 
         self._input_dim = x_train.shape[1]
 
         # Train the ctGAN
         self.train(training_data, discrete_columns=(self._input_dim,))
 
         # One-hot-encode the class labels; Get the number of classes and the number of samples to generate per class.
         class_encoder = OneHotEncoder()
         y_encoded = class_encoder.fit_transform(y_train.reshape(-1, 1)).toarray()
         self._n_classes = y_encoded.shape[1]
         self._gen_samples_ratio = [int(sum(y_encoded[:, c])) for c in range(self._n_classes)]
 
-        majority_class = np.array(self._gen_samples_ratio).argmax()
-        num_majority_samples = np.max(np.array(self._gen_samples_ratio))
-
-        # X and Y data to return
-        x_over_train = np.copy(x_train)
-        y_over_train = np.copy(y_train)
-
-        generated_data = [None for _ in range(self._n_classes)]
-        for cls in range(self._n_classes):
-            if cls != majority_class:
-                samples_to_generate = num_majority_samples - self._gen_samples_ratio[cls]
-
-                # print("\tSampling Class y:", y, " Gen Samples ratio:", gen_samples_ratio[y])
-                # generated_data[cls] = self.sample(samples_to_generate, cls).cpu().detach()
-                generated_data[cls] = self.sample(n=samples_to_generate, condition_column=str(self._input_dim),
-                                                  condition_value=cls)[:, 0:self._input_dim]
-
-                min_classes = np.full(samples_to_generate, cls)
-
-                x_over_train = np.vstack((x_over_train, generated_data[cls]))
-                y_over_train = np.hstack((y_over_train, min_classes))
-
-        # balanced_data = np.hstack((x_over_train, y_over_train.reshape((-1, 1))))
-        # return balanced_data
+        # balance mode: Use the GAN to equalize the number of samples per class. This is achieved by generating
+        # samples of the minority classes (i.e. we perform oversampling).
+        if self._sampling_mode == 'balance':
+            majority_class = np.array(self._gen_samples_ratio).argmax()
+            num_majority_samples = np.max(np.array(self._gen_samples_ratio))
+
+            x_balanced = np.copy(x_train)
+            y_balanced = np.copy(y_train)
+
+            # Perform oversampling
+            for cls in range(self._n_classes):
+                if cls != majority_class:
+                    samples_to_generate = num_majority_samples - self._gen_samples_ratio[cls]
+
+                    # Generate the appropriate number of samples to equalize cls with the majority class.
+                    # print("\tSampling Class y:", cls, " Gen Samples ratio:", gen_samples_ratio[cls])
+                    generated_samples = self.sample_original(n=samples_to_generate,
+                                                             condition_column=str(self._input_dim),
+                                                             condition_value=cls)[:, 0:self._input_dim]
+
+                    generated_classes = np.full(samples_to_generate, cls)
+
+                    x_balanced = np.vstack((x_balanced, generated_samples))
+                    y_balanced = np.hstack((y_balanced, generated_classes))
+
+            # Return balanced_data
+            return x_balanced, y_balanced
+
+        # synthesize_similar mode: Use the GAN to create a new dataset with identical class distribution
+        # as the training set.
+        elif self._sampling_mode == 'synthesize_similar':
+            i = 0
+            x_synthetic = None
+            y_synthetic = None
+
+            # Perform oversampling
+            for cls in range(self._n_classes):
+                # print("Sampling class", cls, "Create", self._gen_samples_ratio[cls], "samples")
+                samples_to_generate = self._gen_samples_ratio[cls]
+
+                generated_samples = self.sample(samples_to_generate, cls)
+                generated_classes = np.full(samples_to_generate, cls)
+
+                if i == 0:
+                    x_synthetic = generated_samples
+                    y_synthetic = generated_classes
+                else:
+                    x_synthetic = np.vstack((x_synthetic, generated_samples))
+                    y_synthetic = np.hstack((y_synthetic, generated_classes))
+                i += 1
 
-        return x_over_train, y_over_train
+            # Return balanced_data
+            return x_synthetic, y_synthetic
```

### Comparing `DeepCoreML-0.3.3/DeepCoreML/generators/gan_discriminators.py` & `DeepCoreML-0.3.4/DeepCoreML/generators/gan_discriminators.py`

 * *Files identical despite different names*

### Comparing `DeepCoreML-0.3.3/DeepCoreML/generators/gan_generators.py` & `DeepCoreML-0.3.4/DeepCoreML/generators/gan_generators.py`

 * *Files identical despite different names*

### Comparing `DeepCoreML-0.3.3/DeepCoreML/main_sentiment.py` & `DeepCoreML-0.3.4/DeepCoreML/main_sentiment.py`

 * *Files identical despite different names*

### Comparing `DeepCoreML-0.3.3/DeepCoreML.egg-info/SOURCES.txt` & `DeepCoreML-0.3.4/DeepCoreML.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 DeepCoreML/Classifiers.py
 DeepCoreML/DataAnimator.py
 DeepCoreML/DataSamplers.py
 DeepCoreML/DataTools.py
 DeepCoreML/Datasets.py
 DeepCoreML/DimensionalityReducers.py
 DeepCoreML/ResultHandler.py
+DeepCoreML/Tests.py
 DeepCoreML/TextDatasets.py
 DeepCoreML/TextPreprocessor.py
 DeepCoreML/TextVectorizers.py
 DeepCoreML/__init__.py
+DeepCoreML/eval.py
 DeepCoreML/main_imbalanced.py
 DeepCoreML/main_sentiment.py
 DeepCoreML.egg-info/PKG-INFO
 DeepCoreML.egg-info/SOURCES.txt
 DeepCoreML.egg-info/dependency_links.txt
 DeepCoreML.egg-info/requires.txt
 DeepCoreML.egg-info/top_level.txt
 DeepCoreML/generators/BaseGenerators.py
 DeepCoreML/generators/DataTransformers.py
 DeepCoreML/generators/c_gan.py
 DeepCoreML/generators/cbr.py
-DeepCoreML/generators/cluster_gan.py
 DeepCoreML/generators/ct_gan.py
 DeepCoreML/generators/gan_discriminators.py
 DeepCoreML/generators/gan_generators.py
 DeepCoreML/generators/sb_gan.py
```

### Comparing `DeepCoreML-0.3.3/LICENSE` & `DeepCoreML-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepCoreML-0.3.3/setup.py` & `DeepCoreML-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     '<li>L. Akritidis, P. Bozanis, "<a href="https://link.springer.com/article/10.1007/s42979-023-01913-y">' \
     'Low Dimensional Text Representations for Sentiment Analysis NLP Tasks</a>", Springer Nature (SN) Computer '\
     'Science, vol. 4, no. 5, 474, 2023.</li>' \
     '</ul></p>'
 
 setup(
     name='DeepCoreML',
-    version='0.3.3',
+    version='0.3.4',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author="Leonidas Akritidis",
     author_email="lakritidis@ihu.gr",
     maintainer="Leonidas Akritidis",
     maintainer_email="lakritidis@ihu.gr",
```

#### html2text {}

```diff
@@ -38,15 +38,15 @@
       Theory and Applications of Learning from Imbalanced Data, to appear,
       2023.
     * ' \ '
     * L. Akritidis, P. Bozanis, "_'_ _\_ _'_L_o_w_ _D_i_m_e_n_s_i_o_n_a_l_ _T_e_x_t_ _R_e_p_r_e_s_e_n_t_a_t_i_o_n_s_ _f_o_r
       _S_e_n_t_i_m_e_n_t_ _A_n_a_l_y_s_i_s_ _N_L_P_ _T_a_s_k_s", Springer Nature (SN) Computer '\ 'Science,
       vol. 4, no. 5, 474, 2023.
     * ' \ '
-' setup( name='DeepCoreML', version='0.3.3', description=DESCRIPTION,
+' setup( name='DeepCoreML', version='0.3.4', description=DESCRIPTION,
 long_description=LONG_DESCRIPTION, long_description_content_type='text/
 markdown', author="Leonidas Akritidis", author_email="lakritidis@ihu.gr",
 maintainer="Leonidas Akritidis", maintainer_email="lakritidis@ihu.gr",
 packages=find_packages(), package_data={'': ['generators/*']}, url='https://
 github.com/lakritidis/DeepCoreML', install_requires=["numpy", "pandas", "nltk",
 "matplotlib", "seaborn", "gensim", "bs4", "joblib", "torch>=2.0.0",
 "transformers>=4.29.0", "scikit-learn>=1.0.0", "imblearn>=0.0",
```

