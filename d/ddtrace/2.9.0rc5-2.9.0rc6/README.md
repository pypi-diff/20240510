# Comparing `tmp/ddtrace-2.9.0rc5.tar.gz` & `tmp/ddtrace-2.9.0rc6-cp312-cp312-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ddtrace-2.9.0rc5.tar", last modified: Fri May 10 15:02:53 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

