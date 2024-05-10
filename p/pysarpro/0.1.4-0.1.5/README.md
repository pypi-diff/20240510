# Comparing `tmp/pysarpro-0.1.4.tar.gz` & `tmp/pysarpro-0.1.5-cp39-cp39-macosx_12_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysarpro-0.1.4.tar", last modified: Fri May 10 09:09:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

