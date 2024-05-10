# Comparing `tmp/nwb4fp-0.6.2.3.tar.gz` & `tmp/nwb4fp-0.6.2.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.2.3.tar", last modified: Fri May 10 13:38:22 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

