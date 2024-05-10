# Comparing `tmp/tkosui-1.0.8.tar.gz` & `tmp/tkosui-1.0.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkosui-1.0.8.tar", last modified: Fri May 10 12:26:17 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

