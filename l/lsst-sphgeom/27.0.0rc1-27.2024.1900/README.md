# Comparing `tmp/lsst_sphgeom-27.0.0rc1.tar.gz` & `tmp/lsst_sphgeom-27.2024.1900-cp39-cp39-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_sphgeom-27.0.0rc1.tar", last modified: Wed May  1 21:16:22 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

