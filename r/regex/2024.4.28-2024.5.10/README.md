# Comparing `tmp/regex-2024.4.28.tar.gz` & `tmp/regex-2024.5.10-cp311-cp311-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-2024.4.28.tar", last modified: Sun Apr 28 19:12:39 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

