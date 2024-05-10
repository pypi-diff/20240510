# Comparing `tmp/python-HackMD-1.0.1.tar.gz` & `tmp/python_HackMD-1.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-HackMD-1.0.1.tar", last modified: Sun Oct 30 14:43:41 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

