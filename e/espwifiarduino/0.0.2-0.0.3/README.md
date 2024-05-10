# Comparing `tmp/espwifiarduino-0.0.2.tar.gz` & `tmp/espwifiarduino-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espwifiarduino-0.0.2.tar", last modified: Fri Apr 26 21:37:43 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

