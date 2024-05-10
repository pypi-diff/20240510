# Comparing `tmp/pymunk-6.7.0.tar.gz` & `tmp/pymunk-6.8.0-cp38-cp38-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\a\pymunk\pymunk\dist\.tmp-ye3b_e1l\pymunk-6.7.0.tar", last modified: Wed May  1 19:10:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

