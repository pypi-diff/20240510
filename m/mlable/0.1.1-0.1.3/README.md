# Comparing `tmp/mlable-0.1.1.tar.gz` & `tmp/mlable-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlable-0.1.1.tar", max compression
+gzip compressed data, was "mlable-0.1.3.tar", max compression
```

## Comparing `mlable-0.1.1.tar` & `mlable-0.1.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      360 2023-12-27 16:49:58.465979 mlable-0.1.1/.github/README.md
--rw-r--r--   0        0        0        0 2024-01-25 21:43:22.740044 mlable-0.1.1/mlable/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 20:33:11.034995 mlable-0.1.1/mlable/keras/__init__.py
--rw-r--r--   0        0        0     5219 2024-03-17 15:32:31.801607 mlable-0.1.1/mlable/keras/models.py
--rw-r--r--   0        0        0        0 2024-01-26 10:57:37.881478 mlable-0.1.1/mlable/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 15:44:53.795021 mlable-0.1.1/mlable/models/colonel/__init__.py
--rw-r--r--   0        0        0    17241 2024-03-12 20:42:42.653388 mlable-0.1.1/mlable/models/gpm/README.md
--rw-r--r--   0        0        0        0 2024-02-04 22:08:59.205764 mlable-0.1.1/mlable/models/gpm/__init__.py
--rw-r--r--   0        0        0     9345 2024-03-12 21:16:09.662821 mlable-0.1.1/mlable/models/gpm/main.py
--rw-r--r--   0        0        0        0 2024-01-25 11:56:28.560613 mlable-0.1.1/mlable/models/gpt/__init__.py
--rw-r--r--   0        0        0     4609 2024-03-15 20:59:30.682559 mlable-0.1.1/mlable/models/gpt/rnn.torch.py
--rw-r--r--   0        0        0    33483 2024-02-05 23:20:39.711787 mlable-0.1.1/mlable/models/gpt/sat.keras.ipynb
--rw-r--r--   0        0        0     5407 2024-03-17 15:46:00.373875 mlable-0.1.1/mlable/models/gpt/sat.keras.py
--rw-r--r--   0        0        0     4642 2024-03-12 21:21:28.151800 mlable-0.1.1/mlable/models/gpt/sat.tensorflow.py
--rw-r--r--   0        0        0     4859 2024-03-16 16:19:19.458786 mlable-0.1.1/mlable/models/gpt/sat.torch.py
--rw-r--r--   0        0        0     8689 2024-01-07 22:39:32.640751 mlable-0.1.1/mlable/models/makemore/.old/mlp.batch.tensorflow.py
--rw-r--r--   0        0        0    11306 2024-01-07 22:39:21.714118 mlable-0.1.1/mlable/models/makemore/.old/mlp.regularization.tensorflow.py
--rw-r--r--   0        0        0    10543 2024-01-07 22:38:57.034242 mlable-0.1.1/mlable/models/makemore/.old/mlp.viz.tensorflow.py
--rw-r--r--   0        0        0        0 2024-01-25 21:44:14.973726 mlable-0.1.1/mlable/models/makemore/__init__.py
--rw-r--r--   0        0        0     7600 2024-01-14 14:50:05.071077 mlable-0.1.1/mlable/models/makemore/cnn.keras.py
--rw-r--r--   0        0        0    15313 2024-02-17 10:48:33.230500 mlable-0.1.1/mlable/models/makemore/cnn.tensorflow.py
--rw-r--r--   0        0        0    10039 2024-03-14 22:06:01.118763 mlable-0.1.1/mlable/models/makemore/cnn.torch.py
--rw-r--r--   0        0        0     6271 2024-01-22 21:19:30.047231 mlable-0.1.1/mlable/models/makemore/mlp.keras.py
--rw-r--r--   0        0        0    14087 2024-02-16 15:05:52.419701 mlable-0.1.1/mlable/models/makemore/mlp.tensorflow.py
--rw-r--r--   0        0        0        0 2024-04-09 09:50:53.069681 mlable-0.1.1/mlable/models/sold/__init__.py
--rw-r--r--   0        0        0     7419 2024-04-09 09:52:25.100652 mlable-0.1.1/mlable/models/sold/bytecode.py
--rw-r--r--   0        0        0     6669 2024-04-09 09:50:53.069681 mlable-0.1.1/mlable/models/sold/main.keras.py
--rw-r--r--   0        0        0     2387 2024-04-09 09:56:41.383364 mlable-0.1.1/mlable/models/sold/solidity.py
--rw-r--r--   0        0        0        0 2024-03-18 18:34:21.653083 mlable-0.1.1/mlable/models/tokun/__init__.py
--rw-r--r--   0        0        0     4321 2024-04-29 07:09:43.479546 mlable-0.1.1/mlable/models/tokun/layers.py
--rw-r--r--   0        0        0     4020 2024-05-02 07:00:17.075570 mlable-0.1.1/mlable/models/tokun/pipeline.py
--rw-r--r--   0        0        0 12878918 2024-05-02 11:01:32.760077 mlable-0.1.1/mlable/models/tokun/tokun.1.keras.ipynb
--rw-r--r--   0        0        0     9022 2024-05-04 08:39:42.186247 mlable-0.1.1/mlable/models/tokun/tokun.1.keras.py
--rw-r--r--   0        0        0 10227709 2024-05-02 11:01:26.420055 mlable-0.1.1/mlable/models/tokun/tokun.4.keras.ipynb
--rw-r--r--   0        0        0    10621 2024-05-02 09:26:01.860244 mlable-0.1.1/mlable/models/tokun/tokun.4.keras.py
--rw-r--r--   0        0        0   832982 2024-05-02 11:00:57.733286 mlable-0.1.1/mlable/models/tokun/tokun.4x4.keras.ipynb
--rw-r--r--   0        0        0    11288 2024-05-02 09:26:23.383872 mlable-0.1.1/mlable/models/tokun/tokun.4x4.keras.py
--rw-r--r--   0        0        0        0 2024-01-26 10:57:25.344821 mlable-0.1.1/mlable/tensorflow/__init__.py
--rw-r--r--   0        0        0      309 2024-02-16 18:02:23.195647 mlable-0.1.1/mlable/tensorflow/data.py
--rw-r--r--   0        0        0      532 2024-01-26 13:14:45.749598 mlable-0.1.1/mlable/tensorflow/initializers.py
--rw-r--r--   0        0        0      559 2024-04-29 12:29:16.563921 mlable-0.1.1/mlable/tensorflow/io.py
--rw-r--r--   0        0        0    17551 2024-05-07 16:55:57.231436 mlable-0.1.1/mlable/tensorflow/layers.py
--rw-r--r--   0        0        0        0 2024-01-26 12:54:06.355191 mlable-0.1.1/mlable/tensorflow/losses.py
--rw-r--r--   0        0        0     4622 2024-01-31 18:01:34.815819 mlable-0.1.1/mlable/tensorflow/models.py
--rw-r--r--   0        0        0     2843 2024-03-17 13:27:55.811876 mlable-0.1.1/mlable/tensorflow/optimizers.py
--rw-r--r--   0        0        0      608 2024-03-17 15:55:26.628912 mlable-0.1.1/mlable/tensorflow/sampling.py
--rw-r--r--   0        0        0     1073 2024-01-28 22:11:41.354437 mlable-0.1.1/mlable/tensorflow/summary.py
--rw-r--r--   0        0        0        0 2024-01-14 17:50:09.526979 mlable-0.1.1/mlable/tokens/__init__.py
--rw-r--r--   0        0        0     2387 2024-02-26 22:53:48.809185 mlable-0.1.1/mlable/tokens/bpe.py
--rw-r--r--   0        0        0     1743 2024-02-24 20:47:30.328705 mlable-0.1.1/mlable/tokens/ngrams.py
--rw-r--r--   0        0        0        0 2024-02-25 16:24:42.204319 mlable-0.1.1/mlable/torch/__init__.py
--rw-r--r--   0        0        0      252 2024-03-14 21:37:39.458099 mlable-0.1.1/mlable/torch/data.py
--rw-r--r--   0        0        0     9425 2024-03-16 16:18:40.985183 mlable-0.1.1/mlable/torch/layers.py
--rw-r--r--   0        0        0     2565 2024-03-16 16:03:36.844134 mlable-0.1.1/mlable/torch/optimizers.py
--rw-r--r--   0        0        0      612 2024-03-14 12:49:57.500345 mlable-0.1.1/mlable/torch/sampling.py
--rw-r--r--   0        0        0      453 2024-05-07 16:56:51.438470 mlable-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 mlable-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      360 2023-12-27 16:49:58.465979 mlable-0.1.3/.github/README.md
+-rw-r--r--   0        0        0        0 2024-01-25 21:43:22.740044 mlable-0.1.3/mlable/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 20:33:11.034995 mlable-0.1.3/mlable/keras/__init__.py
+-rw-r--r--   0        0        0     5219 2024-03-17 15:32:31.801607 mlable-0.1.3/mlable/keras/models.py
+-rw-r--r--   0        0        0        0 2024-01-26 10:57:37.881478 mlable-0.1.3/mlable/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 15:44:53.795021 mlable-0.1.3/mlable/models/colonel/__init__.py
+-rw-r--r--   0        0        0    17241 2024-03-12 20:42:42.653388 mlable-0.1.3/mlable/models/gpm/README.md
+-rw-r--r--   0        0        0        0 2024-02-04 22:08:59.205764 mlable-0.1.3/mlable/models/gpm/__init__.py
+-rw-r--r--   0        0        0     9345 2024-03-12 21:16:09.662821 mlable-0.1.3/mlable/models/gpm/main.py
+-rw-r--r--   0        0        0        0 2024-01-25 11:56:28.560613 mlable-0.1.3/mlable/models/gpt/__init__.py
+-rw-r--r--   0        0        0     4609 2024-03-15 20:59:30.682559 mlable-0.1.3/mlable/models/gpt/rnn.torch.py
+-rw-r--r--   0        0        0    33483 2024-02-05 23:20:39.711787 mlable-0.1.3/mlable/models/gpt/sat.keras.ipynb
+-rw-r--r--   0        0        0     5407 2024-03-17 15:46:00.373875 mlable-0.1.3/mlable/models/gpt/sat.keras.py
+-rw-r--r--   0        0        0     4642 2024-03-12 21:21:28.151800 mlable-0.1.3/mlable/models/gpt/sat.tensorflow.py
+-rw-r--r--   0        0        0     4859 2024-03-16 16:19:19.458786 mlable-0.1.3/mlable/models/gpt/sat.torch.py
+-rw-r--r--   0        0        0     8689 2024-01-07 22:39:32.640751 mlable-0.1.3/mlable/models/makemore/.old/mlp.batch.tensorflow.py
+-rw-r--r--   0        0        0    11306 2024-01-07 22:39:21.714118 mlable-0.1.3/mlable/models/makemore/.old/mlp.regularization.tensorflow.py
+-rw-r--r--   0        0        0    10543 2024-01-07 22:38:57.034242 mlable-0.1.3/mlable/models/makemore/.old/mlp.viz.tensorflow.py
+-rw-r--r--   0        0        0        0 2024-01-25 21:44:14.973726 mlable-0.1.3/mlable/models/makemore/__init__.py
+-rw-r--r--   0        0        0     7600 2024-01-14 14:50:05.071077 mlable-0.1.3/mlable/models/makemore/cnn.keras.py
+-rw-r--r--   0        0        0    15313 2024-02-17 10:48:33.230500 mlable-0.1.3/mlable/models/makemore/cnn.tensorflow.py
+-rw-r--r--   0        0        0    10039 2024-03-14 22:06:01.118763 mlable-0.1.3/mlable/models/makemore/cnn.torch.py
+-rw-r--r--   0        0        0     6271 2024-01-22 21:19:30.047231 mlable-0.1.3/mlable/models/makemore/mlp.keras.py
+-rw-r--r--   0        0        0    14087 2024-02-16 15:05:52.419701 mlable-0.1.3/mlable/models/makemore/mlp.tensorflow.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:50:53.069681 mlable-0.1.3/mlable/models/sold/__init__.py
+-rw-r--r--   0        0        0     7419 2024-04-09 09:52:25.100652 mlable-0.1.3/mlable/models/sold/bytecode.py
+-rw-r--r--   0        0        0     6669 2024-04-09 09:50:53.069681 mlable-0.1.3/mlable/models/sold/main.keras.py
+-rw-r--r--   0        0        0     2387 2024-04-09 09:56:41.383364 mlable-0.1.3/mlable/models/sold/solidity.py
+-rw-r--r--   0        0        0        0 2024-03-18 18:34:21.653083 mlable-0.1.3/mlable/models/tokun/__init__.py
+-rw-r--r--   0        0        0     4321 2024-04-29 07:09:43.479546 mlable-0.1.3/mlable/models/tokun/layers.py
+-rw-r--r--   0        0        0     4020 2024-05-02 07:00:17.075570 mlable-0.1.3/mlable/models/tokun/pipeline.py
+-rw-r--r--   0        0        0 12878918 2024-05-02 11:01:32.760077 mlable-0.1.3/mlable/models/tokun/tokun.1.keras.ipynb
+-rw-r--r--   0        0        0     9022 2024-05-04 08:39:42.186247 mlable-0.1.3/mlable/models/tokun/tokun.1.keras.py
+-rw-r--r--   0        0        0 10227709 2024-05-02 11:01:26.420055 mlable-0.1.3/mlable/models/tokun/tokun.4.keras.ipynb
+-rw-r--r--   0        0        0    10621 2024-05-02 09:26:01.860244 mlable-0.1.3/mlable/models/tokun/tokun.4.keras.py
+-rw-r--r--   0        0        0   832982 2024-05-02 11:00:57.733286 mlable-0.1.3/mlable/models/tokun/tokun.4x4.keras.ipynb
+-rw-r--r--   0        0        0    11288 2024-05-02 09:26:23.383872 mlable-0.1.3/mlable/models/tokun/tokun.4x4.keras.py
+-rw-r--r--   0        0        0        0 2024-01-26 10:57:25.344821 mlable-0.1.3/mlable/tensorflow/__init__.py
+-rw-r--r--   0        0        0      309 2024-02-16 18:02:23.195647 mlable-0.1.3/mlable/tensorflow/data.py
+-rw-r--r--   0        0        0      532 2024-01-26 13:14:45.749598 mlable-0.1.3/mlable/tensorflow/initializers.py
+-rw-r--r--   0        0        0      594 2024-05-10 08:46:46.358956 mlable-0.1.3/mlable/tensorflow/io.py
+-rw-r--r--   0        0        0    17551 2024-05-07 16:55:57.231436 mlable-0.1.3/mlable/tensorflow/layers.py
+-rw-r--r--   0        0        0        0 2024-01-26 12:54:06.355191 mlable-0.1.3/mlable/tensorflow/losses.py
+-rw-r--r--   0        0        0     4622 2024-01-31 18:01:34.815819 mlable-0.1.3/mlable/tensorflow/models.py
+-rw-r--r--   0        0        0     2843 2024-03-17 13:27:55.811876 mlable-0.1.3/mlable/tensorflow/optimizers.py
+-rw-r--r--   0        0        0      608 2024-03-17 15:55:26.628912 mlable-0.1.3/mlable/tensorflow/sampling.py
+-rw-r--r--   0        0        0     1073 2024-01-28 22:11:41.354437 mlable-0.1.3/mlable/tensorflow/summary.py
+-rw-r--r--   0        0        0        0 2024-01-14 17:50:09.526979 mlable-0.1.3/mlable/tokens/__init__.py
+-rw-r--r--   0        0        0     2387 2024-02-26 22:53:48.809185 mlable-0.1.3/mlable/tokens/bpe.py
+-rw-r--r--   0        0        0     1743 2024-02-24 20:47:30.328705 mlable-0.1.3/mlable/tokens/ngrams.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:24:42.204319 mlable-0.1.3/mlable/torch/__init__.py
+-rw-r--r--   0        0        0      252 2024-03-14 21:37:39.458099 mlable-0.1.3/mlable/torch/data.py
+-rw-r--r--   0        0        0     9425 2024-03-16 16:18:40.985183 mlable-0.1.3/mlable/torch/layers.py
+-rw-r--r--   0        0        0     2565 2024-03-16 16:03:36.844134 mlable-0.1.3/mlable/torch/optimizers.py
+-rw-r--r--   0        0        0      612 2024-03-14 12:49:57.500345 mlable-0.1.3/mlable/torch/sampling.py
+-rw-r--r--   0        0        0      453 2024-05-10 08:48:20.550589 mlable-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 mlable-0.1.3/PKG-INFO
```

### Comparing `mlable-0.1.1/mlable/keras/models.py` & `mlable-0.1.3/mlable/keras/models.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/gpm/README.md` & `mlable-0.1.3/mlable/models/gpm/README.md`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/gpm/main.py` & `mlable-0.1.3/mlable/models/gpm/main.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/gpt/rnn.torch.py` & `mlable-0.1.3/mlable/models/gpt/rnn.torch.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/gpt/sat.keras.ipynb` & `mlable-0.1.3/mlable/models/gpt/sat.keras.ipynb`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/gpt/sat.keras.py` & `mlable-0.1.3/mlable/models/gpt/sat.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/gpt/sat.tensorflow.py` & `mlable-0.1.3/mlable/models/gpt/sat.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/gpt/sat.torch.py` & `mlable-0.1.3/mlable/models/gpt/sat.torch.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/makemore/.old/mlp.batch.tensorflow.py` & `mlable-0.1.3/mlable/models/makemore/.old/mlp.batch.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/makemore/.old/mlp.regularization.tensorflow.py` & `mlable-0.1.3/mlable/models/makemore/.old/mlp.regularization.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/makemore/.old/mlp.viz.tensorflow.py` & `mlable-0.1.3/mlable/models/makemore/.old/mlp.viz.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/makemore/cnn.keras.py` & `mlable-0.1.3/mlable/models/makemore/cnn.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/makemore/cnn.tensorflow.py` & `mlable-0.1.3/mlable/models/makemore/cnn.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/makemore/cnn.torch.py` & `mlable-0.1.3/mlable/models/makemore/cnn.torch.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/makemore/mlp.keras.py` & `mlable-0.1.3/mlable/models/makemore/mlp.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/makemore/mlp.tensorflow.py` & `mlable-0.1.3/mlable/models/makemore/mlp.tensorflow.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/sold/bytecode.py` & `mlable-0.1.3/mlable/models/sold/bytecode.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/sold/main.keras.py` & `mlable-0.1.3/mlable/models/sold/main.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/sold/solidity.py` & `mlable-0.1.3/mlable/models/sold/solidity.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/tokun/layers.py` & `mlable-0.1.3/mlable/models/tokun/layers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/tokun/pipeline.py` & `mlable-0.1.3/mlable/models/tokun/pipeline.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/tokun/tokun.1.keras.ipynb` & `mlable-0.1.3/mlable/models/tokun/tokun.1.keras.ipynb`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/tokun/tokun.1.keras.py` & `mlable-0.1.3/mlable/models/tokun/tokun.1.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/tokun/tokun.4.keras.ipynb` & `mlable-0.1.3/mlable/models/tokun/tokun.4.keras.ipynb`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/tokun/tokun.4.keras.py` & `mlable-0.1.3/mlable/models/tokun/tokun.4.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/tokun/tokun.4x4.keras.ipynb` & `mlable-0.1.3/mlable/models/tokun/tokun.4x4.keras.ipynb`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/models/tokun/tokun.4x4.keras.py` & `mlable-0.1.3/mlable/models/tokun/tokun.4x4.keras.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/tensorflow/initializers.py` & `mlable-0.1.3/mlable/tensorflow/initializers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/tensorflow/io.py` & `mlable-0.1.3/mlable/tensorflow/io.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,9 +7,9 @@
     return ' '.join(_label(__c) for __c in token)
 
 # SERIALIZE ###################################################################
 
 def write(data: any, path: str, tsv: bool=True) -> None:
     with open(path, 'w') as __f:
         for __row in data:
-            __line = '\t'.join(str(__v) for __v in __row) if tsv else str(__row)
-            __f.write(__line + '\n')
+            __line = '\t'.join(str(__v) for __v in __row) if tsv else repr(__row)[1:-1]
+            __f.write(__line + '\n') # escape special characters
```

### Comparing `mlable-0.1.1/mlable/tensorflow/layers.py` & `mlable-0.1.3/mlable/tensorflow/layers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/tensorflow/models.py` & `mlable-0.1.3/mlable/tensorflow/models.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/tensorflow/optimizers.py` & `mlable-0.1.3/mlable/tensorflow/optimizers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/tensorflow/sampling.py` & `mlable-0.1.3/mlable/tensorflow/sampling.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/tensorflow/summary.py` & `mlable-0.1.3/mlable/tensorflow/summary.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/tokens/bpe.py` & `mlable-0.1.3/mlable/tokens/bpe.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/tokens/ngrams.py` & `mlable-0.1.3/mlable/tokens/ngrams.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/torch/layers.py` & `mlable-0.1.3/mlable/torch/layers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/torch/optimizers.py` & `mlable-0.1.3/mlable/torch/optimizers.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/mlable/torch/sampling.py` & `mlable-0.1.3/mlable/torch/sampling.py`

 * *Files identical despite different names*

### Comparing `mlable-0.1.1/PKG-INFO` & `mlable-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlable
-Version: 0.1.1
+Version: 0.1.3
 Summary: Tensorflow and pyTorch libs + atomic projects and drafts.
 Author: apehex
 Author-email: apehex@protonmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

