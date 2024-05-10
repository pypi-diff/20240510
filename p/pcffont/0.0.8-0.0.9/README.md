# Comparing `tmp/pcffont-0.0.8.tar.gz` & `tmp/pcffont-0.0.9.tar.gz`

## Comparing `pcffont-0.0.8.tar` & `pcffont-0.0.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pcffont-0.0.8/requirements.txt
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pcffont-0.0.8/.github/workflows/test.yml
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/README.md
--rw-r--r--   0        0        0    16275 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-2.bdf
--rw-r--r--   0        0        0   123960 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-2.pcf
--rw-r--r--   0        0        0   154104 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-lsbyte-lsbit-p2-u4.pcf
--rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-lsbyte-lsbit-p4-u2.pcf
--rw-r--r--   0        0        0   154104 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-lsbyte-msbit-p2-u4.pcf
--rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-lsbyte-msbit-p4-u2.pcf
--rw-r--r--   0        0        0   154104 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-msbyte-lsbit-p2-u4.pcf
--rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-msbyte-lsbit-p4-u2.pcf
--rw-r--r--   0        0        0   154104 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-msbyte-msbit-p2-u4.pcf
--rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo-msbyte-msbit-p4-u2.pcf
--rw-r--r--   0        0        0    84057 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo.bdf
--rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/demo/demo.pcf
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/LICENSE
--rw-r--r--   0        0        0   230552 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/spleen-12x24.pcf
--rw-r--r--   0        0        0   268184 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/spleen-16x32.pcf
--rw-r--r--   0        0        0   392216 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/spleen-32x64.pcf
--rw-r--r--   0        0        0   145220 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/spleen-5x8.pcf
--rw-r--r--   0        0        0   158776 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/spleen-6x12.pcf
--rw-r--r--   0        0        0   206164 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/spleen/spleen-8x16.pcf
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/unifont/OFL.txt
--rw-r--r--   0        0        0  9385540 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/unifont/unifont-15.1.05.bdf
--rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.8/assets/unifont/unifont-15.1.05.pcf
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.8/examples/__init__.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 pcffont-0.0.8/examples/create.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 pcffont-0.0.8/examples/load.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/__init__.py
--rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/builder.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/error.py
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/font.py
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/format.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/glyph.py
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/header.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/metric.py
--rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_accelerators.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_bitmaps.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_encodings.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_glyph_names.py
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_metrics.py
--rw-r--r--   0        0        0    12296 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_properties.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/t_scalable_widths.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/table.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/internal/__init__.py
--rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pcffont-0.0.8/src/pcffont/internal/buffer.py
--rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_buffer.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_builder.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_example.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_load_save.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_no_compat.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_type.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pcffont-0.0.8/tests/test_validity.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.8/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.8/LICENSE
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 pcffont-0.0.8/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 pcffont-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pcffont-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pcffont-0.0.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/demo/README.md
+-rw-r--r--   0        0        0    16275 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/demo/demo-2.bdf
+-rw-r--r--   0        0        0   123960 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/demo/demo-2.pcf
+-rw-r--r--   0        0        0   154104 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/demo/demo-lsbyte-lsbit-p2-u4.pcf
+-rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/demo/demo-lsbyte-lsbit-p4-u2.pcf
+-rw-r--r--   0        0        0   154104 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/demo/demo-lsbyte-msbit-p2-u4.pcf
+-rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/demo/demo-lsbyte-msbit-p4-u2.pcf
+-rw-r--r--   0        0        0   154104 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/demo/demo-msbyte-lsbit-p2-u4.pcf
+-rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/demo/demo-msbyte-lsbit-p4-u2.pcf
+-rw-r--r--   0        0        0   154104 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/demo/demo-msbyte-msbit-p2-u4.pcf
+-rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/demo/demo-msbyte-msbit-p4-u2.pcf
+-rw-r--r--   0        0        0    84057 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/demo/demo.bdf
+-rw-r--r--   0        0        0   165624 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/demo/demo.pcf
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/spleen/LICENSE
+-rw-r--r--   0        0        0   230552 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/spleen/spleen-12x24.pcf
+-rw-r--r--   0        0        0   268184 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/spleen/spleen-16x32.pcf
+-rw-r--r--   0        0        0   392216 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/spleen/spleen-32x64.pcf
+-rw-r--r--   0        0        0   145220 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/spleen/spleen-5x8.pcf
+-rw-r--r--   0        0        0   158776 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/spleen/spleen-6x12.pcf
+-rw-r--r--   0        0        0   206164 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/spleen/spleen-8x16.pcf
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/unifont/OFL.txt
+-rw-r--r--   0        0        0  9385540 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/unifont/unifont-15.1.05.bdf
+-rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.9/assets/unifont/unifont-15.1.05.pcf
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.9/examples/__init__.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pcffont-0.0.9/examples/create.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 pcffont-0.0.9/examples/load.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/__init__.py
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/builder.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/error.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/font.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/format.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/glyph.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/header.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/metric.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/t_accelerators.py
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/t_bitmaps.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/t_encodings.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/t_glyph_names.py
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/t_metrics.py
+-rw-r--r--   0        0        0    12296 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/t_properties.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/t_scalable_widths.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/table.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/internal/__init__.py
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 pcffont-0.0.9/src/pcffont/internal/buffer.py
+-rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 pcffont-0.0.9/tests/test_buffer.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 pcffont-0.0.9/tests/test_builder.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 pcffont-0.0.9/tests/test_example.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pcffont-0.0.9/tests/test_load_save.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 pcffont-0.0.9/tests/test_no_compat.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 pcffont-0.0.9/tests/test_type.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pcffont-0.0.9/tests/test_validity.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 pcffont-0.0.9/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 pcffont-0.0.9/PKG-INFO
```

### Comparing `pcffont-0.0.8/.github/workflows/publish.yml` & `pcffont-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/.github/workflows/test.yml` & `pcffont-0.0.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/demo/README.md` & `pcffont-0.0.9/assets/demo/README.md`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/demo/demo-2.bdf` & `pcffont-0.0.9/assets/demo/demo-2.bdf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/demo/demo-2.pcf` & `pcffont-0.0.9/assets/demo/demo-2.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/demo/demo-lsbyte-lsbit-p2-u4.pcf` & `pcffont-0.0.9/assets/demo/demo-lsbyte-lsbit-p2-u4.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/demo/demo-lsbyte-lsbit-p4-u2.pcf` & `pcffont-0.0.9/assets/demo/demo-lsbyte-lsbit-p4-u2.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/demo/demo-lsbyte-msbit-p2-u4.pcf` & `pcffont-0.0.9/assets/demo/demo-lsbyte-msbit-p2-u4.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/demo/demo-lsbyte-msbit-p4-u2.pcf` & `pcffont-0.0.9/assets/demo/demo-lsbyte-msbit-p4-u2.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/demo/demo-msbyte-lsbit-p2-u4.pcf` & `pcffont-0.0.9/assets/demo/demo-msbyte-lsbit-p2-u4.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/demo/demo-msbyte-lsbit-p4-u2.pcf` & `pcffont-0.0.9/assets/demo/demo-msbyte-lsbit-p4-u2.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/demo/demo-msbyte-msbit-p2-u4.pcf` & `pcffont-0.0.9/assets/demo/demo-msbyte-msbit-p2-u4.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/demo/demo-msbyte-msbit-p4-u2.pcf` & `pcffont-0.0.9/assets/demo/demo-msbyte-msbit-p4-u2.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/demo/demo.bdf` & `pcffont-0.0.9/assets/demo/demo.bdf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/demo/demo.pcf` & `pcffont-0.0.9/assets/demo/demo.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/spleen/LICENSE` & `pcffont-0.0.9/assets/spleen/LICENSE`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/spleen/spleen-12x24.pcf` & `pcffont-0.0.9/assets/spleen/spleen-12x24.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/spleen/spleen-16x32.pcf` & `pcffont-0.0.9/assets/spleen/spleen-16x32.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/spleen/spleen-32x64.pcf` & `pcffont-0.0.9/assets/spleen/spleen-32x64.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/spleen/spleen-5x8.pcf` & `pcffont-0.0.9/assets/spleen/spleen-5x8.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/spleen/spleen-6x12.pcf` & `pcffont-0.0.9/assets/spleen/spleen-6x12.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/spleen/spleen-8x16.pcf` & `pcffont-0.0.9/assets/spleen/spleen-8x16.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/unifont/OFL.txt` & `pcffont-0.0.9/assets/unifont/OFL.txt`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/unifont/unifont-15.1.05.bdf` & `pcffont-0.0.9/assets/unifont/unifont-15.1.05.bdf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/assets/unifont/unifont-15.1.05.pcf` & `pcffont-0.0.9/assets/unifont/unifont-15.1.05.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/examples/create.py` & `pcffont-0.0.9/examples/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,13 +60,12 @@
 
     builder.properties.x_height = 5
     builder.properties.cap_height = 7
 
     builder.properties.font_version = '1.0.0'
     builder.properties.copyright = 'Copyright (c) TakWolf'
 
-    font = builder.build()
-    font.save(os.path.join(outputs_dir, 'my-font.pcf'))
+    builder.save(os.path.join(outputs_dir, 'my-font.pcf'))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pcffont-0.0.8/examples/load.py` & `pcffont-0.0.9/examples/load.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/src/pcffont/__init__.py` & `pcffont-0.0.9/src/pcffont/__init__.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/src/pcffont/builder.py` & `pcffont-0.0.9/src/pcffont/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 from pcffont.font import PcfFont
 from pcffont.format import PcfTableFormat
 from pcffont.glyph import PcfGlyph
 from pcffont.t_properties import PcfProperties
 from pcffont.t_accelerators import PcfAccelerators
 from pcffont.t_metrics import PcfMetrics
 from pcffont.t_bitmaps import PcfBitmaps
@@ -126,7 +128,10 @@
         font.metrics = metrics
         font.ink_metrics = ink_metrics
         font.bitmaps = bitmaps
         font.accelerators = accelerators
         font.bdf_accelerators = accelerators
         font.properties = self.properties
         return font
+
+    def save(self, file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes]):
+        self.build().save(file_path)
```

### Comparing `pcffont-0.0.8/src/pcffont/error.py` & `pcffont-0.0.9/src/pcffont/error.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/src/pcffont/font.py` & `pcffont-0.0.9/src/pcffont/font.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/src/pcffont/glyph.py` & `pcffont-0.0.9/src/pcffont/glyph.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/src/pcffont/header.py` & `pcffont-0.0.9/src/pcffont/header.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,27 +16,28 @@
     INK_METRICS = 1 << 4
     BDF_ENCODINGS = 1 << 5
     SWIDTHS = 1 << 6
     GLYPH_NAMES = 1 << 7
     BDF_ACCELERATORS = 1 << 8
 
 
-class PcfHeader:
-    _TABLE_PARSE_ORDER = [
-        PcfTableType.PROPERTIES,
-        PcfTableType.ACCELERATORS,
-        PcfTableType.BDF_ACCELERATORS,
-        PcfTableType.GLYPH_NAMES,
-        PcfTableType.METRICS,
-        PcfTableType.INK_METRICS,
-        PcfTableType.SWIDTHS,
-        PcfTableType.BITMAPS,
-        PcfTableType.BDF_ENCODINGS,
-    ]
+_TABLE_PARSE_ORDER = [
+    PcfTableType.PROPERTIES,
+    PcfTableType.ACCELERATORS,
+    PcfTableType.BDF_ACCELERATORS,
+    PcfTableType.GLYPH_NAMES,
+    PcfTableType.METRICS,
+    PcfTableType.INK_METRICS,
+    PcfTableType.SWIDTHS,
+    PcfTableType.BITMAPS,
+    PcfTableType.BDF_ENCODINGS,
+]
+
 
+class PcfHeader:
     @staticmethod
     def parse(buffer: Buffer) -> list['PcfHeader']:
         buffer.seek(0)
         if buffer.read(4) != _FILE_VERSION:
             raise PcfParseError('Not PCF format')
 
         tables_count = buffer.read_uint32()
@@ -44,15 +45,15 @@
         headers = []
         for _ in range(tables_count):
             table_type = PcfTableType(buffer.read_uint32())
             table_format = PcfTableFormat.parse(buffer.read_uint32())
             table_size = buffer.read_uint32()
             table_offset = buffer.read_uint32()
             headers.append(PcfHeader(table_type, table_format, table_size, table_offset))
-        headers.sort(key=lambda header: PcfHeader._TABLE_PARSE_ORDER.index(header.table_type))
+        headers.sort(key=lambda header: _TABLE_PARSE_ORDER.index(header.table_type))
 
         return headers
 
     @staticmethod
     def dump(buffer: Buffer, headers: list['PcfHeader']):
         buffer.seek(0)
         buffer.write(_FILE_VERSION)
```

### Comparing `pcffont-0.0.8/src/pcffont/metric.py` & `pcffont-0.0.9/src/pcffont/metric.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/src/pcffont/t_accelerators.py` & `pcffont-0.0.9/src/pcffont/t_accelerators.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/src/pcffont/t_bitmaps.py` & `pcffont-0.0.9/src/pcffont/t_bitmaps.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 
 import pcffont
 from pcffont.format import PcfTableFormat
 from pcffont.header import PcfHeader
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
 
+_GLYPH_PAD_OPTIONS = [1, 2, 4, 8]
+_SCAN_UNIT_OPTIONS = [1, 2, 4, 8]
+
 
 def _swap_fragments(fragments: list[list[int]], scan_unit: int):
     if scan_unit == 2:
         for i in range(0, len(fragments), 2):
             fragments[i], fragments[i + 1] = fragments[i + 1], fragments[i]
     elif scan_unit == 4:
         for i in range(0, len(fragments), 4):
@@ -19,16 +22,16 @@
 
 
 class PcfBitmaps(PcfTable, UserList[list[list[int]]]):
     @staticmethod
     def parse(buffer: Buffer, font: 'pcffont.PcfFont', header: PcfHeader, strict_level: int) -> 'PcfBitmaps':
         table_format = header.read_and_check_table_format(buffer, strict_level)
 
-        glyph_pad = [1, 2, 4, 8][table_format.glyph_pad_index]
-        scan_unit = [1, 2, 4][table_format.scan_unit_index]
+        glyph_pad = _GLYPH_PAD_OPTIONS[table_format.glyph_pad_index]
+        scan_unit = _SCAN_UNIT_OPTIONS[table_format.scan_unit_index]
 
         glyphs_count = buffer.read_uint32(table_format.ms_byte_first)
         bitmap_offsets = buffer.read_uint32_list(glyphs_count, table_format.ms_byte_first)
         bitmaps_sizes = buffer.read_uint32_list(4, table_format.ms_byte_first)
         bitmaps_start = buffer.tell()
 
         bitmaps = PcfBitmaps(table_format)
@@ -70,16 +73,16 @@
         if not isinstance(other, PcfBitmaps):
             return False
         return (self.table_format == other.table_format and
                 self._compat_info == other._compat_info and
                 UserList.__eq__(self, other))
 
     def _dump(self, buffer: Buffer, font: 'pcffont.PcfFont', table_offset: int) -> int:
-        glyph_pad = [1, 2, 4, 8][self.table_format.glyph_pad_index]
-        scan_unit = [1, 2, 4][self.table_format.scan_unit_index]
+        glyph_pad = _GLYPH_PAD_OPTIONS[self.table_format.glyph_pad_index]
+        scan_unit = _SCAN_UNIT_OPTIONS[self.table_format.scan_unit_index]
 
         glyphs_count = len(self)
 
         bitmaps_start = table_offset + 4 + 4 + 4 * glyphs_count + 4 * 4
         bitmaps_size = 0
         bitmap_offsets = []
         buffer.seek(bitmaps_start)
@@ -103,21 +106,15 @@
             bitmaps_size += buffer.write_binary_list(fragments, self.table_format.ms_bit_first)
 
         # Compat
         if self._compat_info is not None:
             bitmaps_sizes = list(self._compat_info)
             bitmaps_sizes[self.table_format.glyph_pad_index] = bitmaps_size
         else:
-            unit_bitmaps_size = bitmaps_size // glyph_pad
-            bitmaps_sizes = [
-                unit_bitmaps_size,
-                unit_bitmaps_size * 2,
-                unit_bitmaps_size * 4,
-                unit_bitmaps_size * 8,
-            ]
+            bitmaps_sizes = [bitmaps_size // glyph_pad * glyph_pad_option for glyph_pad_option in _GLYPH_PAD_OPTIONS]
 
         buffer.seek(table_offset)
         buffer.write_uint32(self.table_format.value)
         buffer.write_uint32(glyphs_count, self.table_format.ms_byte_first)
         buffer.write_uint32_list(bitmap_offsets, self.table_format.ms_byte_first)
         buffer.write_uint32_list(bitmaps_sizes, self.table_format.ms_byte_first)
         buffer.skip(bitmaps_size)
```

### Comparing `pcffont-0.0.8/src/pcffont/t_encodings.py` & `pcffont-0.0.9/src/pcffont/t_encodings.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/src/pcffont/t_glyph_names.py` & `pcffont-0.0.9/src/pcffont/t_glyph_names.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/src/pcffont/t_metrics.py` & `pcffont-0.0.9/src/pcffont/t_metrics.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/src/pcffont/t_properties.py` & `pcffont-0.0.9/src/pcffont/t_properties.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/src/pcffont/t_scalable_widths.py` & `pcffont-0.0.9/src/pcffont/t_scalable_widths.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/src/pcffont/table.py` & `pcffont-0.0.9/src/pcffont/table.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/src/pcffont/internal/buffer.py` & `pcffont-0.0.9/src/pcffont/internal/buffer.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/tests/test_buffer.py` & `pcffont-0.0.9/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/tests/test_builder.py` & `pcffont-0.0.9/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/tests/test_load_save.py` & `pcffont-0.0.9/tests/test_load_save.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/tests/test_no_compat.py` & `pcffont-0.0.9/tests/test_no_compat.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/tests/test_type.py` & `pcffont-0.0.9/tests/test_type.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/tests/test_validity.py` & `pcffont-0.0.9/tests/test_validity.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/.gitignore` & `pcffont-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/LICENSE` & `pcffont-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.8/README.md` & `pcffont-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,15 @@
 
     builder.properties.x_height = 5
     builder.properties.cap_height = 7
 
     builder.properties.font_version = '1.0.0'
     builder.properties.copyright = 'Copyright (c) TakWolf'
 
-    font = builder.build()
-    font.save(os.path.join(outputs_dir, 'my-font.pcf'))
+    builder.save(os.path.join(outputs_dir, 'my-font.pcf'))
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Test Fonts
```

### Comparing `pcffont-0.0.8/pyproject.toml` & `pcffont-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pcffont"
-version = "0.0.8"
+version = "0.0.9"
 description = "A library for manipulating Portable Compiled Format (PCF) Fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `pcffont-0.0.8/PKG-INFO` & `pcffont-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pcffont
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for manipulating Portable Compiled Format (PCF) Fonts.
 Project-URL: homepage, https://github.com/TakWolf/pcffont
 Project-URL: source, https://github.com/TakWolf/pcffont
 Project-URL: issues, https://github.com/TakWolf/pcffont/issues
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
@@ -138,16 +138,15 @@
 
     builder.properties.x_height = 5
     builder.properties.cap_height = 7
 
     builder.properties.font_version = '1.0.0'
     builder.properties.copyright = 'Copyright (c) TakWolf'
 
-    font = builder.build()
-    font.save(os.path.join(outputs_dir, 'my-font.pcf'))
+    builder.save(os.path.join(outputs_dir, 'my-font.pcf'))
 
 
 if __name__ == '__main__':
     main()
 ```
 
 ## Test Fonts
```

