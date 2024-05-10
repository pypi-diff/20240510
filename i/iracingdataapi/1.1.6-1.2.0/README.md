# Comparing `tmp/iracingdataapi-1.1.6.tar.gz` & `tmp/iracingdataapi-1.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iracingdataapi-1.1.6.tar", last modified: Sun Mar 17 16:54:00 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

