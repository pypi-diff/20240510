# Comparing `tmp/enhanceezqq-1.0.2.tar.gz` & `tmp/enhanceezqq-1.0.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhanceezqq-1.0.2.tar", last modified: Sun Mar 17 12:38:08 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

