# Comparing `tmp/pyneurons-0.1.0.tar.gz` & `tmp/pyneurons-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneurons-0.1.0.tar", max compression
+gzip compressed data, was "pyneurons-0.1.1.tar", max compression
```

## Comparing `pyneurons-0.1.0.tar` & `pyneurons-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rwxr-xr-x   0        0        0     1074 2023-04-03 04:18:42.795665 pyneurons-0.1.0/LICENSE
--rwxr-xr-x   0        0        0      905 2023-04-05 06:27:09.618795 pyneurons-0.1.0/README.md
--rwxr-xr-x   0        0        0     1356 2023-04-21 08:51:16.028124 pyneurons-0.1.0/pyneurons/__init__.py
--rwxr-xr-x   0        0        0       97 2023-04-21 04:24:18.627505 pyneurons-0.1.0/pyneurons/apply.py
--rwxr-xr-x   0        0        0      155 2023-04-21 04:10:57.606663 pyneurons-0.1.0/pyneurons/binary.py
--rwxr-xr-x   0        0        0      543 2023-04-21 04:51:42.492864 pyneurons-0.1.0/pyneurons/bind.py
--rwxr-xr-x   0        0        0      496 2023-04-21 08:24:50.922852 pyneurons-0.1.0/pyneurons/box.py
--rwxr-xr-x   0        0        0      181 2023-04-21 04:12:46.320420 pyneurons-0.1.0/pyneurons/brelu1.py
--rwxr-xr-x   0        0        0      225 2023-04-21 09:49:44.253645 pyneurons-0.1.0/pyneurons/compose.py
--rwxr-xr-x   0        0        0      182 2023-04-12 16:03:46.201744 pyneurons-0.1.0/pyneurons/concat.py
--rwxr-xr-x   0        0        0      511 2023-04-12 16:29:43.034885 pyneurons-0.1.0/pyneurons/explode.py
--rwxr-xr-x   0        0        0      296 2023-04-21 08:43:39.961421 pyneurons-0.1.0/pyneurons/fit.py
--rwxr-xr-x   0        0        0       92 2023-04-21 08:37:25.286610 pyneurons-0.1.0/pyneurons/gd.py
--rwxr-xr-x   0        0        0       32 2023-04-12 15:10:11.661346 pyneurons-0.1.0/pyneurons/identity.py
--rwxr-xr-x   0        0        0      144 2023-04-12 16:05:01.092875 pyneurons-0.1.0/pyneurons/implode.py
--rwxr-xr-x   0        0        0       96 2023-04-21 09:37:05.880556 pyneurons-0.1.0/pyneurons/loss.py
--rwxr-xr-x   0        0        0      812 2023-04-21 09:43:04.543242 pyneurons-0.1.0/pyneurons/model.py
--rwxr-xr-x   0        0        0       94 2023-04-21 08:29:46.661449 pyneurons-0.1.0/pyneurons/mse.py
--rwxr-xr-x   0        0        0      354 2023-04-21 09:49:44.275482 pyneurons-0.1.0/pyneurons/neuron.py
--rwxr-xr-x   0        0        0      255 2023-04-11 10:10:27.530077 pyneurons-0.1.0/pyneurons/random/__init__.py
--rwxr-xr-x   0        0        0      138 2023-04-19 10:10:42.695753 pyneurons-0.1.0/pyneurons/random/bias.py
--rwxr-xr-x   0        0        0      107 2023-04-08 06:47:31.914453 pyneurons-0.1.0/pyneurons/random/integer.py
--rwxr-xr-x   0        0        0      100 2023-04-08 06:48:25.109449 pyneurons-0.1.0/pyneurons/random/key.py
--rwxr-xr-x   0        0        0       96 2023-04-11 09:29:59.544583 pyneurons-0.1.0/pyneurons/random/param.py
--rwxr-xr-x   0        0        0       48 2023-04-08 06:47:51.865782 pyneurons-0.1.0/pyneurons/random/seed.py
--rwxr-xr-x   0        0        0      101 2023-04-11 10:07:07.222203 pyneurons-0.1.0/pyneurons/random/weight.py
--rwxr-xr-x   0        0        0      149 2023-04-21 04:11:21.802245 pyneurons-0.1.0/pyneurons/relu.py
--rwxr-xr-x   0        0        0      180 2023-04-21 04:11:48.596839 pyneurons-0.1.0/pyneurons/relu1.py
--rwxr-xr-x   0        0        0       46 2023-04-21 04:14:13.015824 pyneurons-0.1.0/pyneurons/spark.py
--rwxr-xr-x   0        0        0       46 2023-04-21 04:13:57.606997 pyneurons-0.1.0/pyneurons/spike.py
--rwxr-xr-x   0        0        0      208 2023-04-12 16:21:31.806473 pyneurons-0.1.0/pyneurons/split.py
--rwxr-xr-x   0        0        0      147 2023-04-12 16:04:00.337550 pyneurons-0.1.0/pyneurons/stack.py
--rwxr-xr-x   0        0        0      164 2023-04-20 16:12:10.942593 pyneurons-0.1.0/pyneurons/unstack.py
--rwxr-xr-x   0        0        0       58 2023-04-12 15:55:49.386788 pyneurons-0.1.0/pyneurons/vjp/__init__.py
--rwxr-xr-x   0        0        0      273 2023-04-10 11:48:26.156029 pyneurons-0.1.0/pyneurons/vjp/identity.py
--rwxr-xr-x   0        0        0      526 2023-04-21 09:56:56.985663 pyneurons-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1631 1970-01-01 00:00:00.000000 pyneurons-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-05-10 19:07:34.735375 pyneurons-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1356 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/__init__.py
+-rw-r--r--   0        0        0       97 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/apply.py
+-rw-r--r--   0        0        0      155 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/binary.py
+-rw-r--r--   0        0        0      543 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/bind.py
+-rw-r--r--   0        0        0      496 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/box.py
+-rw-r--r--   0        0        0      181 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/brelu1.py
+-rw-r--r--   0        0        0      225 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/compose.py
+-rw-r--r--   0        0        0      182 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/concat.py
+-rw-r--r--   0        0        0      511 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/explode.py
+-rw-r--r--   0        0        0      298 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/fit.py
+-rw-r--r--   0        0        0       92 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/gd.py
+-rw-r--r--   0        0        0       32 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/identity.py
+-rw-r--r--   0        0        0      144 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/implode.py
+-rw-r--r--   0        0        0       96 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/loss.py
+-rw-r--r--   0        0        0      812 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/model.py
+-rw-r--r--   0        0        0       94 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/mse.py
+-rw-r--r--   0        0        0      354 2024-05-10 19:07:34.735375 pyneurons-0.1.1/pyneurons/neuron.py
+-rw-r--r--   0        0        0      255 2024-05-10 19:07:34.743402 pyneurons-0.1.1/pyneurons/random/__init__.py
+-rw-r--r--   0        0        0      138 2024-05-10 19:07:34.743402 pyneurons-0.1.1/pyneurons/random/bias.py
+-rw-r--r--   0        0        0      107 2024-05-10 19:07:34.743402 pyneurons-0.1.1/pyneurons/random/integer.py
+-rw-r--r--   0        0        0      100 2024-05-10 19:07:34.743402 pyneurons-0.1.1/pyneurons/random/key.py
+-rw-r--r--   0        0        0       96 2024-05-10 19:07:34.744432 pyneurons-0.1.1/pyneurons/random/param.py
+-rw-r--r--   0        0        0       48 2024-05-10 19:07:34.744432 pyneurons-0.1.1/pyneurons/random/seed.py
+-rw-r--r--   0        0        0      101 2024-05-10 19:07:34.744432 pyneurons-0.1.1/pyneurons/random/weight.py
+-rw-r--r--   0        0        0      149 2024-05-10 19:07:34.745430 pyneurons-0.1.1/pyneurons/relu.py
+-rw-r--r--   0        0        0      180 2024-05-10 19:07:34.745430 pyneurons-0.1.1/pyneurons/relu1.py
+-rw-r--r--   0        0        0       46 2024-05-10 19:07:34.745430 pyneurons-0.1.1/pyneurons/spark.py
+-rw-r--r--   0        0        0       46 2024-05-10 19:07:34.745430 pyneurons-0.1.1/pyneurons/spike.py
+-rw-r--r--   0        0        0      208 2024-05-10 19:07:34.745430 pyneurons-0.1.1/pyneurons/split.py
+-rw-r--r--   0        0        0      147 2024-05-10 19:07:34.746430 pyneurons-0.1.1/pyneurons/stack.py
+-rw-r--r--   0        0        0      164 2024-05-10 19:07:34.746430 pyneurons-0.1.1/pyneurons/unstack.py
+-rw-r--r--   0        0        0       58 2024-05-10 19:07:34.746430 pyneurons-0.1.1/pyneurons/vjp/__init__.py
+-rw-r--r--   0        0        0      273 2024-05-10 19:07:34.747430 pyneurons-0.1.1/pyneurons/vjp/identity.py
+-rw-r--r--   0        0        0      549 2024-05-10 19:42:01.662910 pyneurons-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4545 2024-05-10 19:22:22.558651 pyneurons-0.1.1/README.md
+-rw-r--r--   0        0        0     5200 1970-01-01 00:00:00.000000 pyneurons-0.1.1/PKG-INFO
```

### Comparing `pyneurons-0.1.0/LICENSE` & `pyneurons-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Ivan Dustin Bilon
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Ivan Dustin Bilon
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pyneurons-0.1.0/pyneurons/__init__.py` & `pyneurons-0.1.1/pyneurons/__init__.py`

 * *Files identical despite different names*

### Comparing `pyneurons-0.1.0/pyneurons/bind.py` & `pyneurons-0.1.1/pyneurons/bind.py`

 * *Files identical despite different names*

### Comparing `pyneurons-0.1.0/pyneurons/model.py` & `pyneurons-0.1.1/pyneurons/model.py`

 * *Files identical despite different names*

