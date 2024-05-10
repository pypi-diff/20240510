# Comparing `tmp/pysarpro-0.1.2.tar.gz` & `tmp/pysarpro-0.1.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysarpro-0.1.2.tar", last modified: Fri Apr  5 11:11:48 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

