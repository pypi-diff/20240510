# Comparing `tmp/mongojet-0.1.2.tar.gz` & `tmp/mongojet-0.1.3-pp39-pypy39_pp73-manylinux_2_28_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

