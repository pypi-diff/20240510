# Comparing `tmp/ddtrace-2.9.0rc4.tar.gz` & `tmp/ddtrace-2.9.0rc5-cp310-cp310-macosx_11_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ddtrace-2.9.0rc4.tar", last modified: Wed May  8 21:28:29 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

