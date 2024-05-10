# Comparing `tmp/glue_plotly-0.7.1.tar.gz` & `tmp/glue_plotly-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_plotly-0.7.1.tar", last modified: Wed May  8 20:04:06 2024, max compression
+gzip compressed data, was "glue_plotly-0.7.2.tar", last modified: Fri May 10 20:36:50 2024, max compression
```

## Comparing `glue_plotly-0.7.1.tar` & `glue_plotly-0.7.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.711464 glue_plotly-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.695464 glue_plotly-0.7.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.695464 glue_plotly-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/.github/workflows/update-changelog.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-08 20:04:06.711464 glue_plotly-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.695464 glue_plotly-0.7.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/doc/BqplotToolbarHighlighted.png
--rw-r--r--   0 runner    (1001) docker     (127)    17060 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/doc/PlotlyViewerExample.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   151377 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/doc/QtChartStudioExport.gif
--rw-r--r--   0 runner    (1001) docker     (127)   221318 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/doc/QtToolbarExport.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.695464 glue_plotly-0.7.1/glue_plotly/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.699464 glue_plotly-0.7.1/glue_plotly/common/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/dotplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/scatter3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.699464 glue_plotly-0.7.1/glue_plotly/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/test_dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/test_dotplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/test_scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/common/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/export_dialog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.699464 glue_plotly-0.7.1/glue_plotly/html_exporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.703464 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/scatter2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.703464 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.703464 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/scatter3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_scatter2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_scatter3d.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/save_hover.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/save_hover.ui
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/sort_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/sort_components.ui
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/viewers/common/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/viewers/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/common/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/common/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/common/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/common/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/viewers/histogram/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/histogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/histogram/dotplot_layer_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/histogram/layer_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/histogram/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/viewers/scatter/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/scatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/scatter/layer_artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/viewers/scatter/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/export_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.707464 glue_plotly-0.7.1/glue_plotly/web/qt/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/qt/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/qt/exporter.ui
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.711464 glue_plotly-0.7.1/glue_plotly/web/qt/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/qt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/qt/tests/test_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/qt/tests/test_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.711464 glue_plotly-0.7.1/glue_plotly/web/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/glue_plotly/web/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:04:06.711464 glue_plotly-0.7.1/glue_plotly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 20:04:06.000000 glue_plotly-0.7.1/glue_plotly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 20:04:06.711464 glue_plotly-0.7.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      432 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-08 20:03:18.000000 glue_plotly-0.7.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.206228 glue_plotly-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.186228 glue_plotly-0.7.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.186228 glue_plotly-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/.github/workflows/update-changelog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-10 20:36:50.206228 glue_plotly-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.186228 glue_plotly-0.7.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)    14339 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/doc/BqplotToolbarHighlighted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17060 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/doc/PlotlyViewerExample.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   151377 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/doc/QtChartStudioExport.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   221318 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/doc/QtToolbarExport.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.190228 glue_plotly-0.7.2/glue_plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.190228 glue_plotly-0.7.2/glue_plotly/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/dotplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/scatter3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.194228 glue_plotly-0.7.2/glue_plotly/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/tests/test_dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/tests/test_dotplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/tests/test_scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/common/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/export_dialog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.194228 glue_plotly-0.7.2/glue_plotly/html_exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.194228 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/scatter2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.194228 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.198228 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/scatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.198228 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_scatter2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_scatter3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/save_hover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/save_hover.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/sort_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/sort_components.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.198228 glue_plotly-0.7.2/glue_plotly/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.198228 glue_plotly-0.7.2/glue_plotly/viewers/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.198228 glue_plotly-0.7.2/glue_plotly/viewers/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/common/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/common/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/common/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/common/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.202228 glue_plotly-0.7.2/glue_plotly/viewers/histogram/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/histogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/histogram/dotplot_layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/histogram/layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/histogram/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.202228 glue_plotly-0.7.2/glue_plotly/viewers/scatter/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/scatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/scatter/layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/viewers/scatter/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.202228 glue_plotly-0.7.2/glue_plotly/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/web/export_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.202228 glue_plotly-0.7.2/glue_plotly/web/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/web/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/web/qt/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/web/qt/exporter.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.202228 glue_plotly-0.7.2/glue_plotly/web/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/web/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6674 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/web/qt/tests/test_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/web/qt/tests/test_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.202228 glue_plotly-0.7.2/glue_plotly/web/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/glue_plotly/web/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:36:50.202228 glue_plotly-0.7.2/glue_plotly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-10 20:36:50.000000 glue_plotly-0.7.2/glue_plotly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-10 20:36:50.000000 glue_plotly-0.7.2/glue_plotly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:36:50.000000 glue_plotly-0.7.2/glue_plotly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 20:36:50.000000 glue_plotly-0.7.2/glue_plotly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:36:50.000000 glue_plotly-0.7.2/glue_plotly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-10 20:36:50.000000 glue_plotly-0.7.2/glue_plotly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 20:36:50.000000 glue_plotly-0.7.2/glue_plotly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-10 20:36:50.206228 glue_plotly-0.7.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      432 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-10 20:36:20.000000 glue_plotly-0.7.2/tox.ini
```

### Comparing `glue_plotly-0.7.1/.github/workflows/ci_workflows.yml` & `glue_plotly-0.7.2/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/.github/workflows/update-changelog.yaml` & `glue_plotly-0.7.2/.github/workflows/update-changelog.yaml`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/CHANGES.md` & `glue_plotly-0.7.2/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Full changelog
 
+## v0.7.1 - 2024-05-08
+
+<!-- Release notes generated using configuration in .github/release.yml at main -->
+### What's Changed
+
+#### Bug Fixes
+
+* Update how traces are removed from dotplot layer artist by @Carifio24 in https://github.com/glue-viz/glue-plotly/pull/61
+
+#### Documentation
+
+* Improve example notebook by @Carifio24 in https://github.com/glue-viz/glue-plotly/pull/60
+
+**Full Changelog**: https://github.com/glue-viz/glue-plotly/compare/v0.7.0...v0.7.1
+
 ## v0.7.0 - 2024-05-07
 
 <!-- Release notes generated using configuration in .github/release.yml at main -->
 ### What's Changed
 
 #### New Features
```

### Comparing `glue_plotly-0.7.1/LICENSE` & `glue_plotly-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/PKG-INFO` & `glue_plotly-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-plotly
-Version: 0.7.1
+Version: 0.7.2
 Summary: Experimental plot.ly exporters for glue
 Home-page: https://github.com/glue-viz/glue-plotly
 Author: Thomas Robitaille and Catherine Zucker
 Author-email: glue.viz@gmail.com
 License: BSD 3-Clause License
 Provides: glue_plotly
 Requires-Python: >=3.8
```

### Comparing `glue_plotly-0.7.1/README.rst` & `glue_plotly-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/doc/BqplotToolbarHighlighted.png` & `glue_plotly-0.7.2/doc/BqplotToolbarHighlighted.png`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/doc/PlotlyViewerExample.ipynb` & `glue_plotly-0.7.2/doc/PlotlyViewerExample.ipynb`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/doc/QtChartStudioExport.gif` & `glue_plotly-0.7.2/doc/QtChartStudioExport.gif`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/doc/QtToolbarExport.gif` & `glue_plotly-0.7.2/doc/QtToolbarExport.gif`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/__init__.py` & `glue_plotly-0.7.2/glue_plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/common.py` & `glue_plotly-0.7.2/glue_plotly/common/common.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/dendrogram.py` & `glue_plotly-0.7.2/glue_plotly/common/dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/dotplot.py` & `glue_plotly-0.7.2/glue_plotly/common/dotplot.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/histogram.py` & `glue_plotly-0.7.2/glue_plotly/common/histogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/image.py` & `glue_plotly-0.7.2/glue_plotly/common/image.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/profile.py` & `glue_plotly-0.7.2/glue_plotly/common/profile.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/scatter2d.py` & `glue_plotly-0.7.2/glue_plotly/common/scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/scatter3d.py` & `glue_plotly-0.7.2/glue_plotly/common/scatter3d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/tests/test_dendrogram.py` & `glue_plotly-0.7.2/glue_plotly/common/tests/test_dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/tests/test_dotplot.py` & `glue_plotly-0.7.2/glue_plotly/common/tests/test_dotplot.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/tests/test_histogram.py` & `glue_plotly-0.7.2/glue_plotly/common/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/tests/test_profile.py` & `glue_plotly-0.7.2/glue_plotly/common/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/tests/test_scatter2d.py` & `glue_plotly-0.7.2/glue_plotly/common/tests/test_scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/common/tests/utils.py` & `glue_plotly-0.7.2/glue_plotly/common/tests/utils.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/export_dialog.py` & `glue_plotly-0.7.2/glue_plotly/export_dialog.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/base.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/base.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/histogram.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/histogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/image.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/image.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/profile.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/profile.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/scatter2d.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_base.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_histogram.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_image.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_profile.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/bqplot/tests/test_scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/dendrogram.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/histogram.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/histogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/image.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/image.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/profile.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/profile.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/scatter2d.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/scatter3d.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/scatter3d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/table.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/table.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_base.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_dendrogram.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_dendrogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_histogram.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_image.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_profile.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_scatter2d.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_scatter2d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_scatter3d.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_scatter3d.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/html_exporters/qt/tests/test_table.py` & `glue_plotly-0.7.2/glue_plotly/html_exporters/qt/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/logo.png` & `glue_plotly-0.7.2/glue_plotly/logo.png`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/logo.svg` & `glue_plotly-0.7.2/glue_plotly/logo.svg`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/save_hover.py` & `glue_plotly-0.7.2/glue_plotly/save_hover.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/save_hover.ui` & `glue_plotly-0.7.2/glue_plotly/save_hover.ui`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/sort_components.py` & `glue_plotly-0.7.2/glue_plotly/sort_components.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/sort_components.ui` & `glue_plotly-0.7.2/glue_plotly/sort_components.ui`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/utils.py` & `glue_plotly-0.7.2/glue_plotly/utils.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/viewers/common/tests/test_tools.py` & `glue_plotly-0.7.2/glue_plotly/viewers/common/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/viewers/common/tests/utils.py` & `glue_plotly-0.7.2/glue_plotly/viewers/common/tests/utils.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/viewers/common/tools.py` & `glue_plotly-0.7.2/glue_plotly/viewers/common/tools.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/viewers/common/viewer.py` & `glue_plotly-0.7.2/glue_plotly/viewers/common/viewer.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/viewers/histogram/dotplot_layer_artist.py` & `glue_plotly-0.7.2/glue_plotly/viewers/histogram/dotplot_layer_artist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # NB: This dot plot layer artist shouldn't be used together with the
 # normalized mode, as a dotplot only makes sense when the heights are integral.
 
 import numpy as np
+from uuid import uuid4
 
 from glue.core.exceptions import IncompatibleAttribute
 from glue.viewers.common.layer_artist import LayerArtist
 from glue.viewers.histogram.state import HistogramLayerState
 from glue_plotly.common.common import fixed_color
 
 from glue_plotly.common.dotplot import dot_radius, traces_for_layer
@@ -31,18 +32,19 @@
             viewer_state,
             layer_state=layer_state,
             layer=layer
         )
 
         self.view = view
         self.bins = None
-        self._dots_id = None
+        self._dots_id = uuid4().hex
 
         self._viewer_state.add_global_callback(self._update_dotplot)
         self.state.add_global_callback(self._update_dotplot)
+        self.state.add_callback("zorder", self._update_zorder)
 
     def _get_dots(self):
         return self.view.figure.select_traces(dict(meta=self._dots_id))
 
     def traces(self):
         return self._get_dots()
 
@@ -121,19 +123,20 @@
 
         dots = traces_for_layer(self.view, self.state, add_data_label=True)
         for trace in dots:
             trace.update(hoverinfo='all', unselected=dict(marker=dict(opacity=self.state.alpha)))
         self._dots_id = dots[0].meta if dots else None
         self.view.figure.add_traces(dots)
 
-    def _update_zorder(self):
+    def _update_zorder(self, *args):
+        current_traces = self.view.figure.data
         traces = [self.view.selection_layer]
         for layer in self.view.layers:
             traces += list(layer.traces())
-        self.view.figure.data = traces
+        self.view.figure.data = traces + [t for t in current_traces if t not in traces]
 
     def _update_dotplot(self, force=False, **kwargs):
         if (self._viewer_state.hist_x_min is None or
                 self._viewer_state.hist_x_max is None or
                 self._viewer_state.hist_n_bin is None or
                 self._viewer_state.x_att is None or
                 self.state.layer is None):
@@ -151,13 +154,10 @@
 
         if force or len(changed & SCALE_PROPERTIES) > 0:
             self._scale_histogram()
 
         if force or len(changed & VISUAL_PROPERTIES) > 0:
             self._update_visual_attributes(changed, force=force)
 
-        if force or "zorder" in changed:
-            self._update_zorder()
-
     def update(self):
         self.state.reset_cache()
         self._update_dotplot(force=True)
```

### Comparing `glue_plotly-0.7.1/glue_plotly/viewers/histogram/layer_artist.py` & `glue_plotly-0.7.2/glue_plotly/viewers/histogram/layer_artist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from uuid import uuid4
 
 from glue.core.exceptions import IncompatibleAttribute
 from glue.viewers.common.layer_artist import LayerArtist
 from glue.viewers.histogram.state import HistogramLayerState
 from glue_plotly.common.common import fixed_color
 
 from glue_plotly.common.histogram import traces_for_layer
@@ -26,18 +27,19 @@
             viewer_state,
             layer_state=layer_state,
             layer=layer
         )
 
         self.view = view
         self.bins = None
-        self._bars_id = None
+        self._bars_id = uuid4().hex
 
         self._viewer_state.add_global_callback(self._update_histogram)
         self.state.add_global_callback(self._update_histogram)
+        self.state.add_callback("zorder", self._update_zorder)
 
     def _get_bars(self):
         return self.view.figure.select_traces(dict(meta=self._bars_id))
 
     def traces(self):
         return self._get_bars()
 
@@ -117,19 +119,20 @@
 
         bars = traces_for_layer(self.view.state, self.state, add_data_label=True)
         for bar in bars:
             bar.update(hoverinfo='all', unselected=dict(marker=dict(opacity=self.state.alpha)))
         self._bars_id = bars[0].meta if bars else None
         self.view.figure.add_traces(bars)
 
-    def _update_zorder(self):
+    def _update_zorder(self, *args):
+        current_traces = self.view.figure.data
         traces = [self.view.selection_layer]
         for layer in self.view.layers:
             traces += list(layer.traces())
-        self.view.figure.data = traces
+        self.view.figure.data = traces + [t for t in current_traces if t not in traces]
 
     def _update_histogram(self, force=False, **kwargs):
         if (self._viewer_state.hist_x_min is None or
                 self._viewer_state.hist_x_max is None or
                 self._viewer_state.hist_n_bin is None or
                 self._viewer_state.x_att is None or
                 self.state.layer is None):
@@ -147,13 +150,10 @@
 
         if force or len(changed & SCALE_PROPERTIES) > 0:
             self._scale_histogram()
 
         if force or len(changed & VISUAL_PROPERTIES) > 0:
             self._update_visual_attributes(changed, force=force)
 
-        if force or "zorder" in changed:
-            self._update_zorder()
-
     def update(self):
         self.state.reset_cache()
         self._update_histogram(force=True)
```

### Comparing `glue_plotly-0.7.1/glue_plotly/viewers/histogram/viewer.py` & `glue_plotly-0.7.2/glue_plotly/viewers/histogram/viewer.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/viewers/scatter/layer_artist.py` & `glue_plotly-0.7.2/glue_plotly/viewers/scatter/layer_artist.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,15 @@
             viewer_state,
             layer_state=layer_state,
             layer=layer
         )
 
         self._viewer_state.add_global_callback(self._update_display)
         self.state.add_global_callback(self._update_display)
+        self.state.add_callback("zorder", self._update_zorder)
 
         self.view = view
 
         # Somewhat annoyingly, the trace that we pass in to be added
         # is NOT the same instance that ends up living in the figure.
         # (see basedatatypes.py line 2251 in the Plotly package)
         # So we abuse the metadata entry of the trace to tag it with
@@ -80,17 +81,21 @@
         # Note that setting the UID directly (either in the Scatter
         # constructor or after) doesn't seem to work - it gets
         # overridden by Plotly
         self._scatter_id = uuid4().hex
         scatter = self._create_scatter()
         self.view.figure.add_trace(scatter)
 
-        self._lines_id = None
-        self._error_id = None
-        self._vector_id = None
+        # We want to initialize these to some dummy UUIDs so that
+        # _get_lines, _get_error_bars, _get_vectors, etc. don't pick up
+        # any other traces that tools have added to the viewer, which
+        # will happen if these IDs are None
+        self._lines_id = uuid4().hex
+        self._error_id = uuid4().hex
+        self._vector_id = uuid4().hex
 
     def remove(self):
         self.view._remove_traces([self._get_scatter()])
         self.view._remove_traces(self._get_lines())
         self.view._remove_traces(self._get_error_bars())
         self.view._remove_traces(self._get_vectors())
         return super().remove()
@@ -158,22 +163,20 @@
 
         if force or len(changed & VISUAL_PROPERTIES) > 0:
             self._update_visual_attributes(changed, force=force)
 
         if force or len(changed & LINE_PROPERTIES) > 0:
             self._update_lines(changed, force=force)
 
-        if force or "zorder" in changed:
-            self._update_zorder()
-
-    def _update_zorder(self):
+    def _update_zorder(self, *args):
+        current_traces = self.view.figure.data
         traces = [self.view.selection_layer]
         for layer in self.view.layers:
             traces += list(layer.traces())
-        self.view.figure.data = traces
+        self.view.figure.data = traces + [t for t in current_traces if t not in traces]
 
     def _update_lines(self, changed, force=False):
         scatter = self._get_scatter()
         fixed_color = self.state.cmap_mode == 'Fixed'
         lines = list(self._get_lines())
 
         with self.view.figure.batch_update():
```

### Comparing `glue_plotly-0.7.1/glue_plotly/viewers/scatter/viewer.py` & `glue_plotly-0.7.2/glue_plotly/viewers/scatter/viewer.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/web/export_plotly.py` & `glue_plotly-0.7.2/glue_plotly/web/export_plotly.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/web/qt/__init__.py` & `glue_plotly-0.7.2/glue_plotly/web/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/web/qt/exporter.py` & `glue_plotly-0.7.2/glue_plotly/web/qt/exporter.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/web/qt/exporter.ui` & `glue_plotly-0.7.2/glue_plotly/web/qt/exporter.ui`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/web/qt/tests/test_exporter.py` & `glue_plotly-0.7.2/glue_plotly/web/qt/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly/web/qt/tests/test_plotly.py` & `glue_plotly-0.7.2/glue_plotly/web/qt/tests/test_plotly.py`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/glue_plotly.egg-info/PKG-INFO` & `glue_plotly-0.7.2/glue_plotly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-plotly
-Version: 0.7.1
+Version: 0.7.2
 Summary: Experimental plot.ly exporters for glue
 Home-page: https://github.com/glue-viz/glue-plotly
 Author: Thomas Robitaille and Catherine Zucker
 Author-email: glue.viz@gmail.com
 License: BSD 3-Clause License
 Provides: glue_plotly
 Requires-Python: >=3.8
```

### Comparing `glue_plotly-0.7.1/glue_plotly.egg-info/SOURCES.txt` & `glue_plotly-0.7.2/glue_plotly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/setup.cfg` & `glue_plotly-0.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `glue_plotly-0.7.1/tox.ini` & `glue_plotly-0.7.2/tox.ini`

 * *Files identical despite different names*

