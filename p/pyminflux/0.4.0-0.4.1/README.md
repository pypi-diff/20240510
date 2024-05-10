# Comparing `tmp/pyminflux-0.4.0.tar.gz` & `tmp/pyminflux-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyminflux-0.4.0.tar", max compression
+gzip compressed data, was "pyminflux-0.4.1.tar", max compression
```

## Comparing `pyminflux-0.4.0.tar` & `pyminflux-0.4.1.tar`

### file list

```diff
@@ -1,89 +1,93 @@
--rw-r--r--   0        0        0    11358 2024-02-08 14:57:56.991424 pyminflux-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     3072 2024-03-27 11:21:44.082029 pyminflux-0.4.0/README.md
--rw-r--r--   0        0        0     1455 2024-03-27 11:37:58.933900 pyminflux-0.4.0/pyminflux/__init__.py
--rw-r--r--   0        0        0     1390 2024-03-27 11:21:44.082029 pyminflux-0.4.0/pyminflux/analysis/__init__.py
--rw-r--r--   0        0        0    22710 2024-03-27 11:21:44.082029 pyminflux-0.4.0/pyminflux/analysis/_analysis.py
--rw-r--r--   0        0        0      638 2024-03-27 11:21:44.082029 pyminflux-0.4.0/pyminflux/base/__init__.py
--rw-r--r--   0        0        0      918 2024-03-27 11:21:44.082029 pyminflux-0.4.0/pyminflux/base/_base.py
--rw-r--r--   0        0        0      837 2024-03-27 11:21:44.082029 pyminflux-0.4.0/pyminflux/correct/__init__.py
--rw-r--r--   0        0        0    14374 2024-03-27 11:21:44.082029 pyminflux-0.4.0/pyminflux/correct/_correct.py
--rw-r--r--   0        0        0      935 2024-03-27 11:21:44.082029 pyminflux-0.4.0/pyminflux/fourier/__init__.py
--rw-r--r--   0        0        0    12913 2024-03-27 11:21:44.082029 pyminflux-0.4.0/pyminflux/fourier/_fourier.py
--rw-r--r--   0        0        0     1081 2024-03-27 11:21:44.082029 pyminflux-0.4.0/pyminflux/main.py
--rw-r--r--   0        0        0      728 2024-03-27 11:21:44.082029 pyminflux-0.4.0/pyminflux/processor/__init__.py
--rw-r--r--   0        0        0    35151 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/processor/_processor.py
--rw-r--r--   0        0        0      906 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/reader/__init__.py
--rw-r--r--   0        0        0     6103 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/reader/_native_reader.py
--rw-r--r--   0        0        0    21701 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/reader/_reader.py
--rw-r--r--   0        0        0      645 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/reader/metadata/__init__.py
--rw-r--r--   0        0        0     2157 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/reader/metadata/_metadata.py
--rw-r--r--   0        0        0      735 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/reader/util/__init__.py
--rw-r--r--   0        0        0    10998 2024-03-27 11:37:58.933900 pyminflux-0.4.0/pyminflux/reader/util/_util.py
--rw-r--r--   0        0        0      733 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/render/__init__.py
--rw-r--r--   0        0        0    12315 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/render/_render.py
--rw-r--r--   0        0        0   139482 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/resources.py
--rw-r--r--   0        0        0      747 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/resources.qrc
--rw-r--r--   0        0        0      641 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/settings/__init__.py
--rw-r--r--   0        0        0     1584 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/settings/_settings.py
--rw-r--r--   0        0        0      725 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/state/__init__.py
--rw-r--r--   0        0        0    10405 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/state/_state.py
--rw-r--r--   0        0        0      633 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/threads/__init__.py
--rw-r--r--   0        0        0      875 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/threads/_threads.py
--rw-r--r--   0        0        0      608 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/ui/__init__.py
--rw-r--r--   0        0        0    41718 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/ui/analyzer.py
--rw-r--r--   0        0        0    10913 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/ui/analyzer.ui
--rw-r--r--   0        0        0   216854 2024-02-08 14:57:57.235427 pyminflux-0.4.0/pyminflux/ui/assets/Logo_v3.icns
--rw-r--r--   0        0        0  1143198 2024-02-08 14:57:57.235427 pyminflux-0.4.0/pyminflux/ui/assets/Logo_v3.ico
--rwxr-xr-x   0        0        0    43531 2024-02-08 14:57:57.235427 pyminflux-0.4.0/pyminflux/ui/assets/Logo_v3.png
--rw-r--r--   0        0        0     8998 2024-02-08 14:57:57.235427 pyminflux-0.4.0/pyminflux/ui/assets/Logo_v3_small.png
--rwxr-xr-x   0        0        0      670 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/ui/assets/create_resources.sh
--rwxr-xr-x   0        0        0     1805 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/ui/assets/png_to_icns.sh
--rw-r--r--   0        0        0    11887 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/ui/color_unmixer.py
--rw-r--r--   0        0        0     8732 2024-02-08 14:57:57.235427 pyminflux-0.4.0/pyminflux/ui/color_unmixer.ui
--rw-r--r--   0        0        0     2661 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/ui/dataviewer.py
--rw-r--r--   0        0        0     1008 2024-03-27 11:21:44.086029 pyminflux-0.4.0/pyminflux/ui/emittingstream.py
--rw-r--r--   0        0        0    20152 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/frc_tool.py
--rw-r--r--   0        0        0     5267 2024-02-08 14:57:57.239427 pyminflux-0.4.0/pyminflux/ui/frc_tool.ui
--rw-r--r--   0        0        0      783 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/helpers/__init__.py
--rw-r--r--   0        0        0    15009 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/helpers/_helpers.py
--rw-r--r--   0        0        0     6135 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/histogram_plotter.py
--rw-r--r--   0        0        0     2988 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/histogram_plotter.ui
--rwxr-xr-x   0        0        0    43531 2024-02-08 14:57:57.239427 pyminflux-0.4.0/pyminflux/ui/icons/icon.png
--rw-r--r--   0        0        0     8030 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/importer.py
--rw-r--r--   0        0        0    33212 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/importer.ui
--rw-r--r--   0        0        0    47397 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/main_window.py
--rw-r--r--   0        0        0     6320 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/main_window.ui
--rw-r--r--   0        0        0    19753 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/options.py
--rw-r--r--   0        0        0    19896 2024-02-08 14:57:57.239427 pyminflux-0.4.0/pyminflux/ui/options.ui
--rw-r--r--   0        0        0     2618 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/pandas_datamodel.py
--rw-r--r--   0        0        0    17723 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/plotter.py
--rw-r--r--   0        0        0     4703 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/plotter_toolbar.py
--rw-r--r--   0        0        0     3254 2024-02-08 14:57:57.239427 pyminflux-0.4.0/pyminflux/ui/plotter_toolbar.ui
--rw-r--r--   0        0        0    10909 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/roi_ranges.py
--rw-r--r--   0        0        0     5257 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/roi_ranges.ui
--rw-r--r--   0        0        0    21307 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/time_inspector.py
--rw-r--r--   0        0        0     3128 2024-02-08 14:57:57.239427 pyminflux-0.4.0/pyminflux/ui/time_inspector.ui
--rw-r--r--   0        0        0     2683 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/trace_dataviewer.py
--rw-r--r--   0        0        0     2336 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/trace_stats_viewer.py
--rw-r--r--   0        0        0     1552 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/trace_stats_viewer.ui
--rw-r--r--   0        0        0    12947 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/ui_analyzer.py
--rw-r--r--   0        0        0     9840 2024-02-08 14:57:57.239427 pyminflux-0.4.0/pyminflux/ui/ui_color_unmixer.py
--rw-r--r--   0        0        0     6478 2024-02-08 14:57:57.239427 pyminflux-0.4.0/pyminflux/ui/ui_frc_tool.py
--rw-r--r--   0        0        0     3704 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/ui_histogram_plotter.py
--rw-r--r--   0        0        0    30910 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/ui_importer.py
--rw-r--r--   0        0        0    11237 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/ui_main_window.py
--rw-r--r--   0        0        0    24387 2024-02-08 14:57:57.239427 pyminflux-0.4.0/pyminflux/ui/ui_options.py
--rw-r--r--   0        0        0     5670 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/ui_plotter_toolbar.py
--rw-r--r--   0        0        0     6875 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/ui_roi_ranges.py
--rw-r--r--   0        0        0     5795 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/ui_time_inspector.py
--rw-r--r--   0        0        0     2654 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/ui_trace_stats_viewer.py
--rw-r--r--   0        0        0    13312 2024-02-08 14:57:57.239427 pyminflux-0.4.0/pyminflux/ui/ui_wizard.py
--rw-r--r--   0        0        0    20970 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/ui/wizard.py
--rw-r--r--   0        0        0     9919 2024-02-08 14:57:57.239427 pyminflux-0.4.0/pyminflux/ui/wizard.ui
--rw-r--r--   0        0        0      668 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/utils/__init__.py
--rw-r--r--   0        0        0     2799 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/utils/_utils.py
--rw-r--r--   0        0        0      794 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/writer/__init__.py
--rw-r--r--   0        0        0     5191 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/writer/_native_writer.py
--rw-r--r--   0        0        0     1907 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyminflux/writer/_writer.py
--rw-r--r--   0        0        0     1976 2024-03-27 11:21:44.090029 pyminflux-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4616 1970-01-01 00:00:00.000000 pyminflux-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-26 17:23:32.506519 pyminflux-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     3519 2024-05-10 08:05:07.811851 pyminflux-0.4.1/README.md
+-rw-r--r--   0        0        0     1455 2024-05-10 08:05:07.811851 pyminflux-0.4.1/pyminflux/__init__.py
+-rw-r--r--   0        0        0     1390 2024-05-10 08:04:49.924078 pyminflux-0.4.1/pyminflux/analysis/__init__.py
+-rw-r--r--   0        0        0    22673 2024-05-10 08:05:07.811851 pyminflux-0.4.1/pyminflux/analysis/_analysis.py
+-rw-r--r--   0        0        0      638 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/base/__init__.py
+-rw-r--r--   0        0        0      918 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/base/_base.py
+-rw-r--r--   0        0        0      837 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/correct/__init__.py
+-rw-r--r--   0        0        0    14374 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/correct/_correct.py
+-rw-r--r--   0        0        0      935 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/fourier/__init__.py
+-rw-r--r--   0        0        0    12913 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/fourier/_fourier.py
+-rw-r--r--   0        0        0     1081 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/main.py
+-rw-r--r--   0        0        0      728 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/processor/__init__.py
+-rw-r--r--   0        0        0    36842 2024-05-10 08:05:07.811851 pyminflux-0.4.1/pyminflux/processor/_processor.py
+-rw-r--r--   0        0        0      906 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/reader/__init__.py
+-rw-r--r--   0        0        0     6469 2024-05-10 08:05:07.811851 pyminflux-0.4.1/pyminflux/reader/_native_reader.py
+-rw-r--r--   0        0        0    25024 2024-05-10 08:05:07.811851 pyminflux-0.4.1/pyminflux/reader/_reader.py
+-rw-r--r--   0        0        0      645 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/reader/metadata/__init__.py
+-rw-r--r--   0        0        0     2199 2024-05-10 08:05:07.811851 pyminflux-0.4.1/pyminflux/reader/metadata/_metadata.py
+-rw-r--r--   0        0        0      735 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/reader/util/__init__.py
+-rw-r--r--   0        0        0    10998 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/reader/util/_util.py
+-rw-r--r--   0        0        0      733 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/render/__init__.py
+-rw-r--r--   0        0        0    12315 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/render/_render.py
+-rw-r--r--   0        0        0   139482 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/resources.py
+-rw-r--r--   0        0        0      747 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/resources.qrc
+-rw-r--r--   0        0        0      686 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/settings/__init__.py
+-rw-r--r--   0        0        0     1584 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/settings/_settings.py
+-rw-r--r--   0        0        0     3050 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/settings/_update_settings.py
+-rw-r--r--   0        0        0      725 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/state/__init__.py
+-rw-r--r--   0        0        0    10845 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/state/_state.py
+-rw-r--r--   0        0        0      631 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/threads/__init__.py
+-rw-r--r--   0        0        0      432 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/threads/common.py
+-rw-r--r--   0        0        0     5282 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/threads/frc.py
+-rw-r--r--   0        0        0     2126 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/threads/update.py
+-rw-r--r--   0        0        0      608 2024-05-10 08:04:49.928078 pyminflux-0.4.1/pyminflux/ui/__init__.py
+-rw-r--r--   0        0        0    43248 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/analyzer.py
+-rw-r--r--   0        0        0    10913 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/analyzer.ui
+-rw-r--r--   0        0        0   216854 2024-03-26 17:23:32.766521 pyminflux-0.4.1/pyminflux/ui/assets/Logo_v3.icns
+-rw-r--r--   0        0        0  1143198 2024-03-26 17:23:32.766521 pyminflux-0.4.1/pyminflux/ui/assets/Logo_v3.ico
+-rwxr-xr-x   0        0        0    43531 2024-03-26 17:23:32.766521 pyminflux-0.4.1/pyminflux/ui/assets/Logo_v3.png
+-rw-r--r--   0        0        0     8998 2024-03-26 17:23:32.766521 pyminflux-0.4.1/pyminflux/ui/assets/Logo_v3_small.png
+-rwxr-xr-x   0        0        0      670 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/assets/create_resources.sh
+-rwxr-xr-x   0        0        0     1805 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/assets/png_to_icns.sh
+-rw-r--r--   0        0        0    11731 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/color_unmixer.py
+-rw-r--r--   0        0        0     8732 2024-03-26 17:23:32.766521 pyminflux-0.4.1/pyminflux/ui/color_unmixer.ui
+-rw-r--r--   0        0        0     2661 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/dataviewer.py
+-rw-r--r--   0        0        0      983 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/emittingstream.py
+-rw-r--r--   0        0        0    14895 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/frc_tool.py
+-rw-r--r--   0        0        0     5267 2024-03-26 17:23:32.770521 pyminflux-0.4.1/pyminflux/ui/frc_tool.ui
+-rw-r--r--   0        0        0      817 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/helpers/__init__.py
+-rw-r--r--   0        0        0    17420 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/helpers/_helpers.py
+-rw-r--r--   0        0        0     6082 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/histogram_plotter.py
+-rw-r--r--   0        0        0     2988 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/histogram_plotter.ui
+-rwxr-xr-x   0        0        0    43531 2024-03-26 17:23:32.770521 pyminflux-0.4.1/pyminflux/ui/icons/icon.png
+-rw-r--r--   0        0        0     8341 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/importer.py
+-rw-r--r--   0        0        0    34085 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/importer.ui
+-rw-r--r--   0        0        0    46091 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/main_window.py
+-rw-r--r--   0        0        0     6320 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/main_window.ui
+-rw-r--r--   0        0        0    15088 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/mediator.py
+-rw-r--r--   0        0        0    19253 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/options.py
+-rw-r--r--   0        0        0    19896 2024-03-26 17:23:32.770521 pyminflux-0.4.1/pyminflux/ui/options.ui
+-rw-r--r--   0        0        0     2618 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/pandas_datamodel.py
+-rw-r--r--   0        0        0    18417 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/plotter.py
+-rw-r--r--   0        0        0     4825 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/plotter_toolbar.py
+-rw-r--r--   0        0        0     3254 2024-03-26 17:23:32.770521 pyminflux-0.4.1/pyminflux/ui/plotter_toolbar.ui
+-rw-r--r--   0        0        0    10877 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/roi_ranges.py
+-rw-r--r--   0        0        0     5257 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/roi_ranges.ui
+-rw-r--r--   0        0        0    21102 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/time_inspector.py
+-rw-r--r--   0        0        0     3128 2024-03-26 17:23:32.770521 pyminflux-0.4.1/pyminflux/ui/time_inspector.ui
+-rw-r--r--   0        0        0     2683 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/trace_dataviewer.py
+-rw-r--r--   0        0        0     2276 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/trace_stats_viewer.py
+-rw-r--r--   0        0        0     1552 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/trace_stats_viewer.ui
+-rw-r--r--   0        0        0    12947 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/ui_analyzer.py
+-rw-r--r--   0        0        0     9840 2024-03-26 17:23:32.770521 pyminflux-0.4.1/pyminflux/ui/ui_color_unmixer.py
+-rw-r--r--   0        0        0     6478 2024-03-26 17:23:32.770521 pyminflux-0.4.1/pyminflux/ui/ui_frc_tool.py
+-rw-r--r--   0        0        0     3704 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/ui_histogram_plotter.py
+-rw-r--r--   0        0        0    31828 2024-05-10 08:05:07.815851 pyminflux-0.4.1/pyminflux/ui/ui_importer.py
+-rw-r--r--   0        0        0    11237 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/ui_main_window.py
+-rw-r--r--   0        0        0    24387 2024-03-26 17:23:32.770521 pyminflux-0.4.1/pyminflux/ui/ui_options.py
+-rw-r--r--   0        0        0     5670 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/ui_plotter_toolbar.py
+-rw-r--r--   0        0        0     6875 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/ui_roi_ranges.py
+-rw-r--r--   0        0        0     5795 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/ui_time_inspector.py
+-rw-r--r--   0        0        0     2654 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/ui/ui_trace_stats_viewer.py
+-rw-r--r--   0        0        0    13312 2024-03-26 17:23:32.770521 pyminflux-0.4.1/pyminflux/ui/ui_wizard.py
+-rw-r--r--   0        0        0    20954 2024-05-10 08:05:07.819851 pyminflux-0.4.1/pyminflux/ui/wizard.py
+-rw-r--r--   0        0        0     9919 2024-03-26 17:23:32.770521 pyminflux-0.4.1/pyminflux/ui/wizard.ui
+-rw-r--r--   0        0        0      668 2024-05-10 08:04:49.932078 pyminflux-0.4.1/pyminflux/utils/__init__.py
+-rw-r--r--   0        0        0     3026 2024-05-10 08:05:07.819851 pyminflux-0.4.1/pyminflux/utils/_utils.py
+-rw-r--r--   0        0        0      794 2024-05-10 08:04:49.936078 pyminflux-0.4.1/pyminflux/writer/__init__.py
+-rw-r--r--   0        0        0     5341 2024-05-10 08:05:07.819851 pyminflux-0.4.1/pyminflux/writer/_native_writer.py
+-rw-r--r--   0        0        0     1907 2024-05-10 08:04:49.936078 pyminflux-0.4.1/pyminflux/writer/_writer.py
+-rw-r--r--   0        0        0     2016 2024-05-10 08:05:07.819851 pyminflux-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5063 1970-01-01 00:00:00.000000 pyminflux-0.4.1/PKG-INFO
```

### Comparing `pyminflux-0.4.0/LICENSE.txt` & `pyminflux-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/README.md` & `pyminflux-0.4.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 $ conda activate pyminflux-env
 $ git clone https://github.com/bsse-scf/pyMINFLUX /path/to/pyminflux
 $ cd /path/to/pyminflux
 $ python -m pip install -e .
 $ pip install -r dev-requirements.txt
 ```
 
+If you want to participate to the development of pyMINFLUX, please have a look at [how you can contribute](CONTRIBUTING.md) and at our [code of conduct](CODE_OF_CONDUCT.md).
+
 ### Running pyMINFLUX from console
 
 ```sh
 $ cd /path/to/pyminflux
 $ python pyminflux/main.py  # As a Python script, or
 $ pyminflux                 # as a standalone tool
 ```
@@ -63,14 +65,18 @@
 
 The official pyMINFLUX website is on https://pyminflux.ethz.ch.
 
 ## pyMINFLUX mailing list
 
 Join the [pyMINFLUX mailing list](https://sympa.ethz.ch/sympa/subscribe/pyminflux) for release announcements and further discussions.
 
+## Contributing to pyMINFLUX
+
+We value the contribution of our community members, and to make sure that everyone can profit from this collaboration, we ask you to have a look at our [CONTRIBUTING](./CONTRIBUTING.md) and [CODE OF CONDUCT](./CODE_OF_CONDUCT.md) documents.
+
 ## Citing pyMINFLUX
 
 If you use pyMINFLUX in your research, please cite this repository as follows:
 
 > Aaron Ponti, Javier Casares Arias, & Thomas Horn. (2023). pyMINFLUX. Zenodo. [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7895501.svg)](https://doi.org/10.5281/zenodo.7895501)
```

### Comparing `pyminflux-0.4.0/pyminflux/__init__.py` & `pyminflux-0.4.1/pyminflux/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 import pyqtgraph as pg
 
 __APP_NAME__ = "pyMINFLUX"
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 # PyQtGraph settings
 pg.setConfigOption("imageAxisOrder", "row-major")  # For best performance
 
 # Documentation
 __doc__ = f"""
 This is the **development** documentation of the `pyminflux` core command-line API (version {__version__}).
```

### Comparing `pyminflux-0.4.0/pyminflux/analysis/__init__.py` & `pyminflux-0.4.1/pyminflux/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/analysis/_analysis.py` & `pyminflux-0.4.1/pyminflux/analysis/_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,23 +48,23 @@
 
     mad: float
         Median absolute deviation of the time resolution from tim_diff (divided by 0.67449 to bring it to the
         scale of the standard deviation)
     """
 
     # Work on a shallow copy
-    df_copy = df.copy()
+    df_copy = df[["tid", "tim"]].copy()
 
     # Calculate time differences and apply unit factor
-    df_copy["tim_diff"] = df_copy.groupby("tid")["tim"].diff() * unit_factor
+    df_copy.loc[:, "tim_diff"] = df_copy.groupby("tid")["tim"].diff() * unit_factor
 
     # Calculate the median and the mad
-    med = np.nanmedian(df_copy["tim_diff"].values)
+    med = np.nanmedian(df_copy["tim_diff"].to_numpy())
     mad = stats.median_abs_deviation(
-        df_copy["tim_diff"].values, scale=0.67449, nan_policy="omit"
+        df_copy["tim_diff"].to_numpy(), scale=0.67449, nan_policy="omit"
     )
 
     return df_copy[["tid", "tim_diff"]], med, mad
 
 
 def calculate_trace_time(df: pd.DataFrame, unit_factor: float = 1e3):
     """Calculate total trace time.
@@ -97,17 +97,17 @@
     # Get the time steps
     tim_diff, _, _ = calculate_time_steps(df, unit_factor)
 
     # Calculate total time per trace
     tim_tot = tim_diff.groupby("tid")["tim_diff"].sum().reset_index(name="tim_tot")
 
     # Calculate median and mad per trace
-    med_tot = np.nanmedian(tim_tot["tim_tot"].values)
+    med_tot = np.nanmedian(tim_tot["tim_tot"].to_numpy())
     mad_tot = stats.median_abs_deviation(
-        tim_tot["tim_tot"].values, scale=0.67449, nan_policy="omit"
+        tim_tot["tim_tot"].to_numpy(), scale=0.67449, nan_policy="omit"
     )
 
     return tim_tot, med_tot, mad_tot
 
 
 def calculate_displacements(df: pd.DataFrame, is_3d: Optional[bool] = None):
     """Calculate displacement resolution.
@@ -133,37 +133,37 @@
     mad_displ: float
         Median absolute deviation of the displacements (steps), divided by 0.67449 to bring it to the scale of the
         standard deviation.
     """
 
     # Determine if 3D calculations are needed
     if is_3d is None:
-        is_3d = np.any(df["z"] != 0)
+        is_3d = bool(np.any(df["z"] != 0))
 
-    def calculate_displacements(group):
-        """Calculate displacements per tid."""
-        diffs = group[["x", "y", "z"]].diff() if is_3d else group[["x", "y"]].diff()
-        group["displacement"] = np.sqrt(np.sum(diffs.values**2, axis=1))
-        return group
+    # Selecting columns based on whether the data is 3D
+    cols = ["tid", "x", "y", "z"] if is_3d else ["tid", "x", "y"]
+    df_subset = df[cols].copy()
+
+    # Calculate translations per tid
+    diffs = df_subset.groupby("tid").diff()
 
     # Calculate displacements per tid
-    displacements = df.groupby("tid").apply(calculate_displacements)
-    displacements.reset_index(drop=True, inplace=True)
+    df_subset.loc[:, "displacement"] = np.linalg.norm(diffs.to_numpy(), axis=1)
 
     # Do we have data?
-    if len(displacements.index) == 0 or "displacement" not in displacements.columns:
-        displacements["displacement"] = []
-    med = float(np.nanmedian(displacements["displacement"].values))
+    if len(df_subset.index) == 0 or "displacement" not in df_subset.columns:
+        df_subset["displacement"] = []
+    med = float(np.nanmedian(df_subset["displacement"].to_numpy()))
     mad = float(
         stats.median_abs_deviation(
-            displacements["displacement"].values, scale=0.67449, nan_policy="omit"
+            df_subset["displacement"].to_numpy(), scale=0.67449, nan_policy="omit"
         )
     )
 
-    return displacements[["tid", "displacement"]], med, mad
+    return df_subset[["tid", "displacement"]], med, mad
 
 
 def calculate_total_distance_traveled(df: pd.DataFrame, is_3d: Optional[bool] = None):
     """Calculate total distance traveled for each tid in a dataframe.
 
     Parameters
     ----------
@@ -191,18 +191,18 @@
     # Get the displacements
     displacements, _, _ = calculate_displacements(df)
 
     # Calculate total distance per tid
     total_distance = displacements.groupby("tid")["displacement"].sum().reset_index()
 
     # Calculate median and mad of the total distance
-    med = float(np.nanmedian(total_distance["displacement"].values))
+    med = float(np.nanmedian(total_distance["displacement"].to_numpy()))
     mad = float(
         stats.median_abs_deviation(
-            total_distance["displacement"].values, scale=0.67449, nan_policy="omit"
+            total_distance["displacement"].to_numpy(), scale=0.67449, nan_policy="omit"
         )
     )
 
     return total_distance, med, mad
 
 
 def hist_bins(values: np.ndarray, bin_size: float) -> tuple:
```

### Comparing `pyminflux-0.4.0/pyminflux/base/__init__.py` & `pyminflux-0.4.1/pyminflux/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/base/_base.py` & `pyminflux-0.4.1/pyminflux/base/_base.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/correct/__init__.py` & `pyminflux-0.4.1/pyminflux/correct/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/correct/_correct.py` & `pyminflux-0.4.1/pyminflux/correct/_correct.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/fourier/__init__.py` & `pyminflux-0.4.1/pyminflux/fourier/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/fourier/_fourier.py` & `pyminflux-0.4.1/pyminflux/fourier/_fourier.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/main.py` & `pyminflux-0.4.1/pyminflux/main.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/processor/__init__.py` & `pyminflux-0.4.1/pyminflux/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/processor/_processor.py` & `pyminflux-0.4.1/pyminflux/processor/_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,15 @@
 from pathlib import Path
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 from scipy.stats import mode
 
-from pyminflux.analysis import (
-    calculate_time_steps,
-    calculate_total_distance_traveled,
-    calculate_trace_time,
-)
+from pyminflux.analysis import calculate_total_distance_traveled, calculate_trace_time
 from pyminflux.reader import MinFluxReader
 
 
 class MinFluxProcessor:
     """Processor of MINFLUX data."""
 
     __doc__ = """Allows for filtering and selecting data read by the underlying `MinFluxReader`. Please notice that
@@ -91,14 +87,17 @@
         self._use_weighted_localizations = False
 
         # Apply the global filters
         self._apply_global_filters()
 
     def _init_selected_rows_dict(self):
         """Initialize the selected rows array."""
+        if self.full_dataframe is None:
+            return
+
         # How many fluorophores do we have?
         self._selected_rows_dict = {
             1: pd.Series(
                 data=np.ones(len(self.full_dataframe.index), dtype=bool),
                 index=self.full_dataframe.index,
             ),
             2: pd.Series(
@@ -177,25 +176,30 @@
 
         # Flag stats to be recomputed
         self._stats_to_be_recomputed = True
 
     @property
     def num_fluorophores(self) -> int:
         """Return the number of fluorophores."""
-        return len(np.unique(self.full_dataframe["fluo"].values))
+        if self.full_dataframe is None:
+            return 0
+        return len(np.unique(self.full_dataframe["fluo"].to_numpy()))
 
     @property
     def filtered_numpy_array_all(self):
         """Return the raw NumPy array with applied filters (for all fluorophores)."""
 
         # Copy the raw NumPy array
         raw_array = self.reader.valid_raw_data
         if raw_array is None:
             return None
 
+        if self.full_dataframe is None or self._selected_rows_dict is None:
+            return None
+
         # Append the fluorophore ID data
         raw_array["fluo"] = self.full_dataframe["fluo"].astype(np.uint8)
 
         # Extract combination of fluorophore 1 and 2 filtered dataframes
         mask_1 = (self.full_dataframe["fluo"] == 1) & self._selected_rows_dict[1]
         mask_2 = (self.full_dataframe["fluo"] == 2) & self._selected_rows_dict[2]
         return raw_array[mask_1 | mask_2]
@@ -244,15 +248,15 @@
 
         Returns
         -------
 
         filtered_dataframe_all: Union[None, pd.DataFrame]
             A Pandas dataframe or None if no file was loaded.
         """
-        if self.full_dataframe is None:
+        if self.full_dataframe is None or self._selected_rows_dict is None:
             return None
 
         # Extract combination of fluorophore 1 and 2 filtered dataframes
         mask_1 = (self.full_dataframe["fluo"] == 1) & self._selected_rows_dict[1]
         mask_2 = (self.full_dataframe["fluo"] == 2) & self._selected_rows_dict[2]
         return self.full_dataframe.loc[mask_1 | mask_2]
 
@@ -270,14 +274,16 @@
             return None
         if self.current_fluorophore_id == 0:
             return self._filtered_dataframe_all()
         else:
             df = self.full_dataframe.loc[
                 self.full_dataframe["fluo"] == self.current_fluorophore_id
             ]
+            if self._selected_rows_dict is None:
+                return None
             return df.loc[self._selected_rows_dict[self.current_fluorophore_id]]
 
     @property
     def filtered_dataframe_stats(self) -> Union[None, pd.DataFrame]:
         """Return dataframe stats with all filters applied.
 
         Returns
@@ -326,14 +332,20 @@
             "sy",
             "sxy",
             "exy",
             "rms_xy",
             "sz",
             "ez",
             "fluo",
+        ]
+
+    @classmethod
+    def trace_stats_with_tracking_properties(cls):
+        """Return the columns of the filtered_dataframe_stats with tracking columns."""
+        return MinFluxProcessor.trace_stats_properties() + [
             "tim_tot",
             "avg_speed",
             "total_dist",
         ]
 
     def reset(self):
         """Drops all dynamic filters and resets the data to the processed data frame with global filters."""
@@ -368,15 +380,20 @@
             Array of y coordinates.
 
         z: np.ndarray (Optional)
             Optional array of z coordinates. Omit it to skip.
             If the acquisition is 2D, it will be ignored in any case.
         """
 
-        if self.full_dataframe is None:
+        if (
+            self.full_dataframe is None
+            or self._selected_rows_dict is None
+            or self.reader._data_df is None
+            or self.reader._valid_entries is None
+        ):
             return
 
         # Make sure to work with NumPy arrays
         x = np.array(x)
         y = np.array(y)
         if z is not None and self.is_3d:
             z = np.array(z)
@@ -388,18 +405,20 @@
             mask = mask_1 | mask_2
         elif self.current_fluorophore_id == 1:
             mask = (self.full_dataframe["fluo"] == 1) & self._selected_rows_dict[1]
         else:
             mask = (self.full_dataframe["fluo"] == 2) & self._selected_rows_dict[2]
 
         # Make sure that the lengths match
-        assert np.sum(mask.values) == len(x), "Unexpected number of elements in x."
-        assert np.sum(mask.values) == len(y), "Unexpected number of elements in y."
+        assert np.sum(mask.to_numpy()) == len(x), "Unexpected number of elements in x."
+        assert np.sum(mask.to_numpy()) == len(y), "Unexpected number of elements in y."
         if z is not None and self.is_3d:
-            assert np.sum(mask.values) == len(z), "Unexpected number of elements in z."
+            assert np.sum(mask.to_numpy()) == len(
+                z
+            ), "Unexpected number of elements in z."
 
         # Re-assign the data at the reader level
         self.reader._data_df.loc[mask, "x"] = x
         self.reader._data_df.loc[mask, "y"] = y
         if z is not None and self.is_3d:
             self.reader._data_df.loc[mask, "z"] = z
 
@@ -426,14 +445,16 @@
 
         # Mark derived data to be recomputed
         self._stats_to_be_recomputed = True
         self._weighted_localizations_to_be_recomputed = True
 
     def set_fluorophore_ids(self, fluorophore_ids: np.ndarray[int]):
         """Assign the fluorophore IDs."""
+        if self.full_dataframe is None:
+            return
         if len(fluorophore_ids) != len(self.full_dataframe.index):
             raise ValueError(
                 "The number of fluorophore IDs does not match the number of entries in the dataframe."
             )
         self.full_dataframe["fluo"] = fluorophore_ids
         self._init_selected_rows_dict()
         self._apply_global_filters()
@@ -499,22 +520,25 @@
         # Make sure that the range is increasing
         x_min = x_range[0]
         x_max = x_range[1]
         if x_max < x_min:
             x_max, x_min = x_min, x_max
 
         if from_weighted_locs:
+            if self._weighted_localizations is None:
+                return None
             return self._weighted_localizations.loc[
                 (self._weighted_localizations[x_prop] >= x_min)
                 & (self._weighted_localizations[x_prop] < x_max)
             ]
         else:
             # Work with currently selected rows
+            if self.filtered_dataframe is None:
+                return None
             df = self.filtered_dataframe
-
             return df.loc[(df[x_prop] >= x_min) & (df[x_prop] < x_max)]
 
     def select_by_2d_range(
         self, x_prop, y_prop, x_range, y_range, from_weighted_locs: bool = False
     ) -> Union[None, pd.DataFrame]:
         """Return a view on a subset of the filtered dataset or the weighted localisations defined by the passed
         parameters and corresponding ranges.
@@ -555,24 +579,27 @@
 
         y_min = y_range[0]
         y_max = y_range[1]
         if y_max < y_min:
             y_max, y_min = y_min, y_max
 
         if from_weighted_locs:
+            if self._weighted_localizations is None:
+                return None
             return self._weighted_localizations.loc[
                 (self._weighted_localizations[x_prop] >= x_min)
                 & (self._weighted_localizations[x_prop] < x_max)
                 & (self._weighted_localizations[y_prop] >= y_min)
                 & (self._weighted_localizations[y_prop] < y_max)
             ]
         else:
             # Work with currently selected rows
+            if self.filtered_dataframe is None:
+                return None
             df = self.filtered_dataframe
-
             return df.loc[
                 (df[x_prop] >= x_min)
                 & (df[x_prop] < x_max)
                 & (df[y_prop] >= y_min)
                 & (df[y_prop] < y_max)
             ]
 
@@ -794,15 +821,15 @@
 
         # Find all TIDs for current fluorophore ID by which the requested stats property is inside the range
         tids_to_keep = self.filtered_dataframe_stats[
             (
                 (self.filtered_dataframe_stats[x_prop_stats] >= x_min)
                 & (self.filtered_dataframe_stats[x_prop_stats] <= x_max)
             )
-        ]["tid"].values
+        ]["tid"].to_numpy()
 
         # Rows of the filtered dataframe to keep
         rows_to_keep = self.filtered_dataframe["tid"].isin(tids_to_keep)
 
         # Apply filter
         if self.current_fluorophore_id == 0 or self.current_fluorophore_id == 1:
             self._selected_rows_dict[1] = self._selected_rows_dict[1] & rows_to_keep
@@ -828,61 +855,75 @@
         if not self._stats_to_be_recomputed:
             return
 
         # Work with currently selected rows
         df = self.filtered_dataframe
 
         # Calculate the statistics
-        df_tid = self.calculate_statistics_on(df)
+        df_tid = self.calculate_statistics_on(df, self.reader.is_tracking)
 
         # Store the results
         self._filtered_stats_dataframe = df_tid
 
         # Flag the statistics to be computed
         self._stats_to_be_recomputed = False
 
     @staticmethod
-    def calculate_statistics_on(df: pd.DataFrame) -> pd.DataFrame:
+    def calculate_statistics_on(
+        df: pd.DataFrame, is_tracking: bool = False
+    ) -> pd.DataFrame:
         """Calculate per-trace statistics for the selected dataframe.
 
         Parameters
         ----------
 
         df: pd.DataFrame
             DataFrame (view) generated by one of the `select_by_*` methods.
 
         Returns
         -------
         df_stats: pd.DataFrame
             Per-trace statistics calculated on the passed DataFrame selection (view).
         """
 
+        # Prepare a dataframe with the statistics
+        if is_tracking:
+            df_tid = pd.DataFrame(
+                columns=MinFluxProcessor.trace_stats_with_tracking_properties()
+            )
+        else:
+            df_tid = pd.DataFrame(columns=MinFluxProcessor.trace_stats_properties())
+
         # Calculate some statistics per TID on the passed dataframe
         df_grouped = df.groupby("tid")
 
-        tid = df_grouped["tid"].first().values
-        n = df_grouped["tid"].count().values
-        mx = df_grouped["x"].mean().values
-        my = df_grouped["y"].mean().values
-        mz = df_grouped["z"].mean().values
-        sx = df_grouped["x"].std().values
-        sy = df_grouped["y"].std().values
-        sz = df_grouped["z"].std().values
+        # Base statistics
+        tid = df_grouped["tid"].first().to_numpy()
+        n = df_grouped["tid"].count().to_numpy()
+        mx = df_grouped["x"].mean().to_numpy()
+        my = df_grouped["y"].mean().to_numpy()
+        mz = df_grouped["z"].mean().to_numpy()
+        sx = df_grouped["x"].std().to_numpy()
+        sy = df_grouped["y"].std().to_numpy()
+        sz = df_grouped["z"].std().to_numpy()
         tmp = np.power(sx, 2) + np.power(sy, 2)
         sxy = np.sqrt(tmp)
         rms_xy = np.sqrt(tmp / 2)
         exy = sxy / np.sqrt(n)
         ez = sz / np.sqrt(n)
-        fluo = df_grouped["fluo"].agg(lambda x: mode(x, keepdims=True)[0][0]).values
-        tot_tim, _, _ = calculate_trace_time(df)
-        total_distance, _, _ = calculate_total_distance_traveled(df)
-        speeds = total_distance["displacement"].values / tot_tim["tim_tot"].values
+        fluo = df_grouped["fluo"].agg(lambda x: mode(x, keepdims=True)[0][0]).to_numpy()
 
-        # Prepare a dataframe with the statistics
-        df_tid = pd.DataFrame(columns=MinFluxProcessor.trace_stats_properties())
+        # Optional tracking statistics
+        if is_tracking:
+            tot_tim, _, _ = calculate_trace_time(df)
+            total_distance, _, _ = calculate_total_distance_traveled(df)
+            speeds = (
+                total_distance["displacement"].to_numpy()
+                / tot_tim["tim_tot"].to_numpy()
+            )
 
         # Store trace stats
         df_tid["tid"] = tid  # Trace ID
         df_tid["n"] = n  # Number of localizations for given trace ID
         df_tid["mx"] = mx  # x mean localization
         df_tid["my"] = my  # y mean localization
         df_tid["mz"] = mz  # z mean localization
@@ -890,83 +931,87 @@
         df_tid["sy"] = sy  # y localization precision
         df_tid["sxy"] = sxy  # Lateral (x, y) localization precision
         df_tid["rms_xy"] = rms_xy  # Lateral root mean square
         df_tid["exy"] = exy  # Standard error of sxy
         df_tid["sz"] = sz  # z localization precision
         df_tid["ez"] = ez  # Standard error of ez
         df_tid["fluo"] = fluo  # Assigned fluorophore ID
-        df_tid["tim_tot"] = tot_tim["tim_tot"].values  # Total time per trace
-        df_tid["avg_speed"] = speeds  # Average speed per trace
-        df_tid["total_dist"] = total_distance[
-            "displacement"
-        ].values  # Total travelled distance per trace
+        if is_tracking:
+            df_tid["tim_tot"] = tot_tim["tim_tot"].to_numpy()  # Total time per trace
+            df_tid["avg_speed"] = speeds  # Average speed per trace
+            df_tid["total_dist"] = total_distance[
+                "displacement"
+            ].to_numpy()  # Total travelled distance per trace
 
         # ["sx", "sy", "sxy", "rms_xy", "exy", "sz", "ez"] columns will contain
         # np.nan if n == 1: we replace them with 0.0.
         # @TODO: should this be changed? It could be a global option.
         df_tid[["sx", "sy", "sxy", "rms_xy", "exy", "sz", "ez"]] = df_tid[
             ["sx", "sy", "sxy", "rms_xy", "exy", "sz", "ez"]
         ].fillna(value=0.0)
 
         # Return the results
         return df_tid
 
     def _calculate_weighted_positions(self):
         """Calculate per-trace localization weighted by relative photon count."""
 
-        # Make sure we have processed dataframe to work on
-        if self.full_dataframe is None:
+        if self.filtered_dataframe is None:
             return
 
-        # Only recompute weighted localizations if needed
         if not self._weighted_localizations_to_be_recomputed:
             return
 
-        # Work with currently selected rows
-        df = self.filtered_dataframe
+        # Work with a copy of a subset of current filtered dataframe
+        df = self.filtered_dataframe[["tid", "eco", "x", "y", "z", "fluo"]].copy()
 
-        # Normal or weighted averaging?
         if self._use_weighted_localizations:
-            # Calculate weighing factors for TIDs
-            df = df.assign(
-                eco_rel=df["eco"].groupby(df["tid"]).transform(lambda x: x / x.sum())
-            )
-
-            # Calculate relative contributions of (x, y, z)_i for each TID
-            df["x_rel"] = df["x"] * df["eco_rel"]
-            df["y_rel"] = df["y"] * df["eco_rel"]
-            df["z_rel"] = df["z"] * df["eco_rel"]
+            # Calculate weights for each coordinate based on 'eco'
+            total_eco_per_tid = df.groupby("tid")["eco"].transform("sum")
+            eco_rel = df["eco"] / total_eco_per_tid
+
+            # Calculate weighted positions
+            df.loc[:, "x_rel"] = df["x"] * eco_rel
+            df.loc[:, "y_rel"] = df["y"] * eco_rel
+            df.loc[:, "z_rel"] = df["z"] * eco_rel
 
-            # Calculate the weighted localizations
+            # Summing up the relative contributions
             df_grouped = df.groupby("tid")
-            tid = df_grouped["tid"].first().values
-            x_w = df_grouped["x_rel"].sum().values
-            y_w = df_grouped["y_rel"].sum().values
-            z_w = df_grouped["z_rel"].sum().values
-            fluo = (
-                df_grouped["fluo"].agg(lambda x: mode(x, keepdims=True)[0][0]).values
-            )  # Return the most frequent fluo ID
+            x_w = df_grouped["x_rel"].sum()
+            y_w = df_grouped["y_rel"].sum()
+            z_w = df_grouped["z_rel"].sum()
+
+            # Return the most frequent fluo ID: traces should be homogeneous with respect
+            # to their fluorophore assignment, but we search anyway for safety.
+            fluo_mode = df_grouped["fluo"].agg(
+                lambda x: x.mode()[0] if not x.empty else np.nan
+            )
 
         else:
             # Calculate simple average of localizations by TID
-            df_grouped = df.groupby(df["tid"])
-            tid = df_grouped["tid"].first().values
-            x_w = df_grouped["x"].mean().values
-            y_w = df_grouped["y"].mean().values
-            z_w = df_grouped["z"].mean().values
-            fluo = (
-                df_grouped["fluo"].agg(lambda x: mode(x, keepdims=True)[0][0]).values
-            )  # Return the most frequent fluo ID
+            df_grouped = df.groupby("tid")
+            x_w = df_grouped["x"].mean()
+            y_w = df_grouped["y"].mean()
+            z_w = df_grouped["z"].mean()
+
+            # Return the most frequent fluo ID: traces should be homogeneous with respect
+            # to their fluorophore assignment, but we search anyway for safety.
+            fluo_mode = df_grouped["fluo"].agg(
+                lambda x: x.mode()[0] if not x.empty else np.nan
+            )
 
         # Prepare a dataframe with the weighted localizations
-        df_loc = pd.DataFrame(columns=["tid", "x", "y", "z", "fluo"])
-        df_loc["tid"] = tid
-        df_loc["x"] = x_w
-        df_loc["y"] = y_w
-        df_loc["z"] = z_w
-        df_loc["fluo"] = fluo
+        df_loc = pd.DataFrame(
+            {
+                "tid": x_w.index,
+                "x": x_w.to_numpy(),
+                "y": y_w.to_numpy(),
+                "z": z_w.to_numpy(),
+                "fluo": fluo_mode.to_numpy(),
+            }
+        )
 
-        # Store the results
+        # Update the weighted localization dataframe
         self._weighted_localizations = df_loc
 
-        # Make sure to flag the derived data to be recomputed
+        # Flag the results as up-to-date
         self._weighted_localizations_to_be_recomputed = False
```

### Comparing `pyminflux-0.4.0/pyminflux/reader/__init__.py` & `pyminflux-0.4.1/pyminflux/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/reader/_native_reader.py` & `pyminflux-0.4.1/pyminflux/reader/_native_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,37 +94,46 @@
                 # back to boolean on read.
                 try:
                     is_tracking = bool(f["parameters/is_tracking"][()])
                 except KeyError as e:
                     return None
 
                 try:
+                    pool_dcr = bool(f["parameters/pool_dcr"][()])
+                except KeyError as e:
+                    # This is an addendum to version 2.0, and we allow it to be missing.
+                    # It will fall back to False.
+                    pool_dcr = False
+
+                try:
                     scale_bar_size = float(f["parameters/scale_bar_size"][()])
                 except KeyError as e:
                     return None
 
             else:
                 tr_len_thresholds = None
                 time_thresholds = None
                 dwell_time = 1.0
                 is_tracking = False
+                pool_dcr = False
                 scale_bar_size = 500
 
         # Store and return
         metadata = NativeMetadata(
-            z_scaling_factor=z_scaling_factor,
-            min_trace_length=min_trace_length,
-            efo_thresholds=efo_thresholds,
+            pool_dcr=pool_dcr,
             cfr_thresholds=cfr_thresholds,
-            time_thresholds=time_thresholds,
-            tr_len_thresholds=tr_len_thresholds,
-            num_fluorophores=num_fluorophores,
             dwell_time=dwell_time,
+            efo_thresholds=efo_thresholds,
             is_tracking=is_tracking,
+            min_trace_length=min_trace_length,
+            num_fluorophores=num_fluorophores,
             scale_bar_size=scale_bar_size,
+            time_thresholds=time_thresholds,
+            tr_len_thresholds=tr_len_thresholds,
+            z_scaling_factor=z_scaling_factor,
         )
 
         return metadata
 
 
 class NativeArrayReader:
     """Reads the native NumPy array from `.pmx` files."""
```

### Comparing `pyminflux-0.4.0/pyminflux/reader/_reader.py` & `pyminflux-0.4.1/pyminflux/reader/_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,49 +29,51 @@
 )
 
 
 class MinFluxReader:
     __docs__ = "Reader of MINFLUX data in `.pmx`, `.npy` or `.mat` formats."
 
     __slots__ = [
-        "_filename",
-        "_last_valid_cfr",
-        "_last_valid",
-        "_is_last_valid",
-        "_valid",
-        "_unit_scaling_factor",
+        "_pool_dcr",
+        "_cfr_index",
         "_data_array",
         "_data_df",
         "_data_full_df",
-        "_valid_entries",
+        "_dcr_index",
+        "_dwell_time",
+        "_eco_index",
+        "_efo_index",
+        "_filename",
         "_is_3d",
         "_is_aggregated",
+        "_is_last_valid",
         "_is_tracking",
-        "_reps",
-        "_efo_index",
-        "_cfr_index",
-        "_eco_index",
-        "_dcr_index",
+        "_last_valid",
+        "_last_valid_cfr",
         "_loc_index",
+        "_relocalizations",
+        "_reps",
         "_tid_index",
         "_tim_index",
+        "_unit_scaling_factor",
+        "_valid",
+        "_valid_cfr",
+        "_valid_entries",
         "_vld_index",
         "_z_scaling_factor",
-        "_dwell_time",
-        "_valid_cfr",
-        "_relocalizations",
     ]
 
     def __init__(
         self,
         filename: Union[Path, str],
         valid: bool = True,
         z_scaling_factor: float = 1.0,
         is_tracking: bool = False,
-        dwell_time: bool = 1.0,
+        pool_dcr: bool = False,
+        dwell_time: float = 1.0,
     ):
         """Constructor.
 
         Parameters
         ----------
 
         filename: Union[Path, str]
@@ -83,14 +85,17 @@
         z_scaling_factor: float (optional, default = 1.0)
             Refractive index mismatch correction factor to apply to the z coordinates.
 
         is_tracking: bool (optional, default = False)
             Whether the dataset comes from a tracking experiment; otherwise, it is considered as a
             localization experiment.
 
+        pool_dcr: bool (optional, default = False)
+            Whether to pool DCR values weighted by the relative ECO of all relocalized iterations.
+
         dwell_time: float (optional, default 1.0)
             Dwell time in milliseconds.
         """
 
         # Store the filename
         self._filename: Path = Path(filename)
         if not self._filename.is_file():
@@ -120,14 +125,17 @@
 
         # Whether the acquisition is 2D or 3D
         self._is_3d: bool = False
 
         # Whether the acquisition is a tracking dataset
         self._is_tracking: bool = is_tracking
 
+        # Whether to pool the dcr values
+        self._pool_dcr = pool_dcr
+
         # Whether the file contains aggregate measurements
         self._is_aggregated: bool = False
 
         # Indices dependent on 2D or 3D acquisition and whether the
         # data comes from a localization or a tracking experiment.
         self._reps: int = -1
         self._efo_index: int = -1
@@ -149,16 +157,19 @@
         self._last_valid_cfr: int = -1
 
         # Load the file
         if not self._load():
             raise IOError(f"The file {self._filename} is not a valid MINFLUX file.")
 
     @property
-    def is_last_valid(self) -> bool:
-        """Return True if the selected iterations are the "last valid", False otherwise."""
+    def is_last_valid(self) -> Union[bool, None]:
+        """Return True if the selected iteration is the "last valid", False otherwise.
+        If the dataframe has not been processed yet, `is_last_valid` will be None."""
+        if self._data_df is None:
+            return None
         return self._is_last_valid
 
     @property
     def z_scaling_factor(self) -> float:
         """Returns the scaling factor for the z coordinates."""
         return self._z_scaling_factor
 
@@ -174,14 +185,24 @@
 
     @property
     def is_tracking(self) -> bool:
         """Returns True for a tracking acquisition, False otherwise."""
         return self._is_tracking
 
     @property
+    def is_pool_dcr(self) -> bool:
+        """Returns True if the DCR values over all relocalized iterations (to use all photons)."""
+        return self._pool_dcr
+
+    @property
+    def dwell_time(self) -> float:
+        """Returns the dwell time."""
+        return self._dwell_time
+
+    @property
     def num_valid_entries(self) -> int:
         """Number of valid entries."""
         if self._data_array is None:
             return 0
         return self._valid_entries.sum()
 
     @property
@@ -265,14 +286,18 @@
             Iteration index for cfr
 
         process: bool (Optional, default = True)
             By default, when setting the indices, the data is rescanned
             and the dataframe is rebuilt. In case several properties of
             the MinFluxReader are modified sequentially, the processing
             can be disabled and run only once after the last change.
+            However, this only applies after the first load/scan, when
+            the processed dataframe has not been created yet. If the
+            dataframe already exists, this flag will be ignored and the
+            processing will take place.
         """
 
         # Make sure there is loaded data
         if self._data_array is None:
             raise ValueError("No data loaded.")
 
         if self._reps == -1:
@@ -302,63 +327,99 @@
         self._cfr_index = cfr_index
 
         # Constant indices
         self._tid_index: int = 0
         self._tim_index: int = 0
         self._vld_index: int = 0
 
-        # Re-process the file?
-        if process:
+        # Re-process the file? If the processed dataframe already exists,
+        # the processing will take place anyway.
+        if process or self._data_df is not None:
             self._process()
 
     def set_tracking(self, is_tracking: bool, process: bool = True):
         """Sets whether the acquisition is tracking or localization.
 
         Parameters
         ----------
 
         is_tracking: bool
             Set to True for a tracking acquisition, False for a localization
             acquisition.
 
         process: bool (Optional, default = True)
-            By default, when setting the indices, the data is rescanned
+            By default, when setting the tracking flag, the data is rescanned
             and the dataframe is rebuilt. In case several properties of
             the MinFluxReader are modified sequentially, the processing
             can be disabled and run only once after the last change.
+            However, this only applies after the first load/scan, when
+            the processed dataframe has not been created yet. If the
+            dataframe already exists, this flag will be ignored and the
+            processing will take place.
         """
 
         # Update the flag
         self._is_tracking = is_tracking
 
         # Re-process the file?
-        if process:
+        if process or self._data_df is not None:
             self._process()
 
     def set_dwell_time(self, dwell_time: float, process: bool = True):
         """
         Sets the dwell time.
 
         Parameters
         ----------
         dwell_time: float
             Dwell time.
 
         process: bool (Optional, default = True)
-            By default, when setting the indices, the data is rescanned
+            By default, when setting the dwell time, the data is rescanned
             and the dataframe is rebuilt. In case several properties of
             the MinFluxReader are modified sequentially, the processing
             can be disabled and run only once after the last change.
+            However, this only applies after the first load/scan, when
+            the processed dataframe has not been created yet. If the
+            dataframe already exists, this flag will be ignored and the
+            processing will take place.
         """
 
         # Update the flag
         self._dwell_time = dwell_time
 
         # Re-process the file?
-        if process:
+        if process or self._data_df is not None:
+            self._process()
+
+    def set_pool_dcr(self, pool_dcr: bool, process: bool = True):
+        """
+        Sets whether the DCR values should be pooled (and weighted by ECO).
+
+        Parameters
+        ----------
+        pool_dcr: bool
+            Whether the DCR values should be pooled (and weighted by ECO).
+
+        process: bool (Optional, default = True)
+            By default, when setting the DCR binning flag, the data is rescanned
+            and the dataframe is rebuilt. In case several properties of
+            the MinFluxReader are modified sequentially, the processing
+            can be disabled and run only once after the last change.
+            However, this only applies after the first load/scan, when
+            the processed dataframe has not been created yet. If the
+            dataframe already exists, this flag will be ignored and the
+            processing will take place.
+        """
+
+        # Update the flag
+        self._pool_dcr = pool_dcr
+
+        # Re-process the file?
+        if process or self._data_df is not None:
             self._process()
 
     @classmethod
     def processed_properties(cls) -> list:
         """Returns the properties read from the file that correspond to the processed dataframe column names."""
         return [
             "tid",
@@ -524,16 +585,31 @@
 
             # Extract CFR
             cfr = itr[:, self._cfr_index]["cfr"]
 
             # Extract ECO
             eco = itr[:, self._eco_index]["eco"]
 
-            # Extract DCR
-            dcr = itr[:, self._dcr_index]["dcr"]
+            # Pool DCR values?
+            if self._pool_dcr and np.sum(self._relocalizations) > 1:
+
+                # Calculate ECO contributions
+                eco_all = itr[:, self._relocalizations]["eco"]
+                eco_sum = eco_all.sum(axis=1)
+                eco_all_norm = eco_all / eco_sum.reshape(-1, 1)
+
+                # Extract DCR values and weigh them by the relative ECO contributions
+                dcr = itr[:, self._relocalizations]["dcr"]
+                dcr = dcr * eco_all_norm
+                dcr = dcr.sum(axis=1)
+
+            else:
+
+                # Extract DCR
+                dcr = itr[:, self._dcr_index]["dcr"]
 
             # Calculate dwell
             dwell = np.around((eco / (efo / 1000)) / self._dwell_time, decimals=0)
 
         # Create a Pandas dataframe for the results
         df = pd.DataFrame(
             index=pd.RangeIndex(start=0, stop=len(tid)),
@@ -553,15 +629,15 @@
         df["dwell"] = dwell
         df["fluo"] = fluo
 
         # Remove rows with NaNs in the loc matrix
         df = df.dropna(subset=["x"])
 
         # Check if the selected indices correspond to the last valid iteration
-        self._is_last_valid = (
+        self._is_last_valid = bool(
             self._cfr_index == self._last_valid_cfr
             and self._efo_index == self._last_valid
         )
 
         return df
 
     def _raw_data_to_full_dataframe(self) -> Union[None, pd.DataFrame]:
```

### Comparing `pyminflux-0.4.0/pyminflux/reader/metadata/__init__.py` & `pyminflux-0.4.1/pyminflux/reader/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/reader/metadata/_metadata.py` & `pyminflux-0.4.1/pyminflux/reader/metadata/_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,30 +29,32 @@
 
 @dataclass
 class NativeMetadata:
     """Metadata associated to `.pmx` native pyMINFLUX file format.
 
     Version 2.0
     -----------
-        time_thresholds: Union[None, tuple[float, float]]
-        tr_len_thresholds: Union[None, tuple[int, int]]
+        pool_dcr: bool
         dwell_time: float
         is_tracking: bool
         scale_bar_size: float
+        time_thresholds: Union[None, tuple[float, float]]
+        tr_len_thresholds: Union[None, tuple[int, int]]
         (+ version 1.0)
 
     Version 1.0
     -----------
-        z_scaling_factor: float
-        min_trace_length: int
-        efo_thresholds: tuple[int, int]
         cfr_thresholds: tuple[float, float]
+        efo_thresholds: tuple[int, int]
+        min_trace_length: int
         num_fluorophores: int
+        z_scaling_factor: float
     """
 
+    pool_dcr: bool
     cfr_thresholds: Union[None, tuple[float, float]]
     dwell_time: float
     efo_thresholds: Union[None, tuple[int, int]]
     is_tracking: bool
     min_trace_length: int
     num_fluorophores: int
     scale_bar_size: float
```

### Comparing `pyminflux-0.4.0/pyminflux/reader/util/__init__.py` & `pyminflux-0.4.1/pyminflux/reader/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/reader/util/_util.py` & `pyminflux-0.4.1/pyminflux/reader/util/_util.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/render/__init__.py` & `pyminflux-0.4.1/pyminflux/render/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/render/_render.py` & `pyminflux-0.4.1/pyminflux/render/_render.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/resources.py` & `pyminflux-0.4.1/pyminflux/resources.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/resources.qrc` & `pyminflux-0.4.1/pyminflux/resources.qrc`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/settings/__init__.py` & `pyminflux-0.4.1/pyminflux/settings/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,7 +10,8 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 from ._settings import Settings
+from ._update_settings import UpdateSettings
```

### Comparing `pyminflux-0.4.0/pyminflux/settings/_settings.py` & `pyminflux-0.4.1/pyminflux/settings/_settings.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/state/__init__.py` & `pyminflux-0.4.1/pyminflux/state/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/state/_state.py` & `pyminflux-0.4.1/pyminflux/state/_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 from enum import IntEnum
+from pathlib import Path
 from typing import Union
 
 from ..base import Singleton
 from ..reader.metadata import NativeMetadata
 
 
 class ColorCode(IntEnum):
@@ -34,14 +35,15 @@
     """
 
     __SLOTS__ = [
         "applied_cfr_thresholds",
         "applied_efo_thresholds",
         "applied_time_thresholds",
         "applied_tr_len_thresholds",
+        "pool_dcr",
         "cfr_range",
         "cfr_threshold_factor",
         "cfr_thresholds",
         "color_code",
         "dcr_bin_size",
         "dcr_manual_threshold",
         "dwell_time",
@@ -52,14 +54,15 @@
         "enable_cfr_lower_threshold",
         "enable_cfr_upper_threshold",
         "frc_endpoint_only",
         "frc_lateral_resolution",
         "frc_num_repeats",
         "frc_temporal_resolution",
         "is_tracking",
+        "last_selected_path",
         "loc_precision_range",
         "min_trace_length",
         "num_fluorophores",
         "open_console_at_start",
         "plot_average_localisations",
         "plot_export_dpi",
         "scale_bar_size",
@@ -129,19 +132,22 @@
         self.y_param: str = "y"
 
         # Number of fluorophores in the sample
         self.num_fluorophores: int = 1
         self.dcr_bin_size: float = 0.0
         self.dcr_manual_threshold: float = 0.0
 
+        # Pool DCR (weighted by ECO)
+        self.pool_dcr = False
+
         # Z scaling factor
         self.z_scaling_factor: float = 0.7
 
         # Resolution for exporting plots as images
-        self.plot_export_dpi: int = 600
+        self.plot_export_dpi: int = 300
 
         # FRC analysis
         self.frc_lateral_resolution: float = 4.0
         self.frc_temporal_resolution: float = 1800.0
         self.frc_num_repeats: int = 5
         self.frc_endpoint_only: bool = False
 
@@ -153,21 +159,25 @@
 
         # Is the dataset a tracking acquisition?
         self.is_tracking: bool = False
 
         # Scale bar size in um
         self.scale_bar_size: float = 500.0
 
+        # Last selected path
+        self.last_selected_path: Union[None, Path] = None
+
     def asdict(self) -> dict:
         """Return class as dictionary."""
         return {
             "applied_cfr_threshold": self.applied_cfr_thresholds,
             "applied_efo_thresholds": self.applied_efo_thresholds,
             "applied_time_thresholds": self.applied_time_thresholds,
             "applied_tr_len_thresholds": self.applied_tr_len_thresholds,
+            "pool_dcr": self.pool_dcr,
             "cfr_range": self.cfr_range,
             "cfr_threshold_factor": self.cfr_threshold_factor,
             "cfr_thresholds": self.cfr_thresholds,
             "color_code": str(ColorCode(self.color_code)),
             "dcr_bin_size": self.dcr_bin_size,
             "dcr_manual_threshold": self.dcr_manual_threshold,
             "dwell_time": self.dwell_time,
@@ -178,14 +188,15 @@
             "enable_cfr_lower_threshold": self.enable_cfr_lower_threshold,
             "enable_cfr_upper_threshold": self.enable_cfr_upper_threshold,
             "frc_endpoint_only": self.frc_endpoint_only,
             "frc_lateral_resolution": self.frc_lateral_resolution,
             "frc_num_repeats": self.frc_num_repeats,
             "frc_temporal_resolution": self.frc_temporal_resolution,
             "is_tracking": self.is_tracking,
+            "last_selected_path": self.last_selected_path,
             "loc_precision_range": self.loc_precision_range,
             "min_trace_length": self.min_trace_length,
             "num_fluorophores": self.num_fluorophores,
             "open_console_at_start": self.open_console_at_start,
             "plot_average_localisations": self.plot_average_localisations,
             "plot_export_dpi": self.plot_export_dpi,
             "scale_bar_size": self.scale_bar_size,
@@ -214,14 +225,15 @@
     def full_reset(self):
         """Reset to defaults."""
 
         self.applied_cfr_thresholds = None
         self.applied_efo_thresholds = None
         self.applied_time_thresholds = None
         self.applied_tr_len_thresholds = None
+        self.pool_dcr = False
         self.cfr_range = None
         self.cfr_threshold_factor = 2.0
         self.cfr_thresholds = None
         self.color_code: ColorCode = ColorCode.NONE
         self.dcr_bin_size = 0.0
         self.dcr_manual_threshold = 0.0
         self.dwell_time = 1.0
@@ -232,14 +244,15 @@
         self.enable_cfr_lower_threshold = False
         self.enable_cfr_upper_threshold = True
         self.frc_endpoint_only = False
         self.frc_lateral_resolution = 4.0
         self.frc_num_repeats = 5
         self.frc_temporal_resolution = 1800.0
         self.is_tracking = False
+        self.last_selected_path = None
         self.loc_precision_range = None
         self.min_trace_length = 1
         self.num_fluorophores = 1
         self.open_console_at_start = False
         self.plot_average_localisations = False
         self.plot_export_dpi = 300
         self.scale_bar_size = 500.0
@@ -253,14 +266,15 @@
         self.z_scaling_factor = 0.7
 
     def update_from_metadata(self, metadata: NativeMetadata):
         """Update State from the NativeMetadata parameters from a `.pmx` file."""
         self.applied_cfr_thresholds = metadata.cfr_thresholds
         self.applied_efo_thresholds = metadata.efo_thresholds
         self.applied_tr_len_thresholds = metadata.tr_len_thresholds
+        self.pool_dcr = metadata.pool_dcr
         self.cfr_thresholds = metadata.cfr_thresholds
         self.dwell_time = metadata.dwell_time
         self.efo_thresholds = metadata.efo_thresholds
         self.is_tracking = metadata.is_tracking
         self.min_trace_length = metadata.min_trace_length
         self.num_fluorophores = metadata.num_fluorophores
         self.scale_bar_size = metadata.scale_bar_size
```

### Comparing `pyminflux-0.4.0/pyminflux/threads/__init__.py` & `pyminflux-0.4.1/pyminflux/threads/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-from ._threads import *
+from .update import *
```

### Comparing `pyminflux-0.4.0/pyminflux/threads/_threads.py` & `pyminflux-0.4.1/pyminflux/ui/assets/create_resources.sh`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,20 @@
-#  Copyright (c) 2022 - 2024 D-BSSE, ETH Zurich.
+#!/bin/bash
+#
+# Copyright (c) 2022 - 2024 D-BSSE, ETH Zurich.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#      http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+#  limitations under the License.
 #
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#       http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#   limitations under the License.
 #
 
-from PySide6 import QtCore
-
-
-class BaseThread(QtCore.QThread):
-    """
-    Thread that runs the tracker without blocking the UI.
-    """
-
-    def __init__(self, *args):
-        super().__init__()
-
-        self._args = args
+pyside6-rcc ../../resources.qrc -o ../../resources.py
 
-    def run(self):
-        print("Done.")
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/__init__.py` & `pyminflux-0.4.1/pyminflux/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/analyzer.py` & `pyminflux-0.4.1/pyminflux/ui/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,30 +28,34 @@
     find_cutoff_near_value,
     get_robust_threshold,
     prepare_histogram,
 )
 from ..processor import MinFluxProcessor
 from ..state import State
 from ..utils import intersect_2d_ranges
-from .helpers import add_median_line, export_plot_interactive
+from .helpers import (
+    add_median_line,
+    export_all_plots_interactive,
+    export_plot_interactive,
+)
 from .roi_ranges import ROIRanges
 from .ui_analyzer import Ui_Analyzer
 
 
 class Analyzer(QDialog, Ui_Analyzer):
     # Signal that the data viewers should be updated
-    data_filters_changed = Signal(name="data_filters_changed")
-    plotting_started = Signal(name="plotting_started")
-    plotting_completed = Signal(name="plotting_completed")
-    efo_bounds_changed = Signal(name="efo_bounds_changed")
-    cfr_bounds_changed = Signal(name="cfr_bounds_changed")
-    cfr_threshold_factor_changed = Signal(name="cfr_threshold_factor_changed")
-    cfr_lower_bound_state_changed = Signal(name="cfr_lower_bound_state_changed")
-    cfr_upper_bound_state_changed = Signal(name="cfr_upper_bound_state_changed")
-    tr_len_bounds_changed = Signal(name="tr_len_bounds_changed")
+    data_filters_changed = Signal()
+    plotting_started = Signal()
+    plotting_completed = Signal()
+    efo_bounds_changed = Signal()
+    cfr_bounds_changed = Signal()
+    cfr_threshold_factor_changed = Signal()
+    cfr_lower_bound_state_changed = Signal()
+    cfr_upper_bound_state_changed = Signal()
+    tr_len_bounds_changed = Signal()
 
     def __init__(self, processor: MinFluxProcessor, parent=None):
         """Constructor."""
 
         # Call the base class
         super().__init__()
 
@@ -92,15 +96,15 @@
         #
         # Set defaults
         #
 
         # EFO cutoff frequency tab
         self.ui.leEFOExpectedCutoff.setText(str(self.state.efo_expected_frequency))
         self.ui.leEFOExpectedCutoff.setValidator(
-            QDoubleValidator(bottom=0.0, decimals=2)
+            QDoubleValidator(bottom=0.0, top=np.Inf, decimals=2)
         )
 
         # CFR filtering tab
         self.ui.checkCFRLowerThreshold.setChecked(self.state.enable_cfr_lower_threshold)
         self.ui.checkCFRUpperThreshold.setChecked(self.state.enable_cfr_upper_threshold)
         self.ui.leCFRFilterThreshFactor.setText(str(self.state.cfr_threshold_factor))
         self.ui.leCFRFilterThreshFactor.setValidator(
@@ -246,147 +250,150 @@
         self.cfr_region = None
         self.tr_len = None
         self.efo_range = self.state.efo_range
         self.cfr_range = self.state.cfr_range
         self.tr_len_range = self.state.tr_len_range
         self.loc_precision_range = self.state.loc_precision_range
 
-    @Slot(name="run_efo_cutoff_frequency_detection")
+    @Slot()
     def run_efo_cutoff_frequency_detection(self):
         """Run EFO cutoff frequency detection."""
 
         # Get the approximate frequency
         frequency = 2.0 * float(self.ui.leEFOExpectedCutoff.text())
 
         # Histogram bin settings
         efo_auto_bins = self.state.efo_bin_size_hz == 0
 
         # Calculate thresholds for EFO
         n_efo, _, b_efo, _ = prepare_histogram(
-            self.processor.filtered_dataframe["efo"].values,
+            self.processor.filtered_dataframe["efo"].to_numpy(),
             auto_bins=efo_auto_bins,
             bin_size=self.state.efo_bin_size_hz,
         )
         cutoff_frequency = find_cutoff_near_value(
             counts=n_efo,
             bins=b_efo,
             expected_value=frequency,
         )
 
         # If the search failed, we return
         if cutoff_frequency is None:
             return
 
         # Set the new upper bound and reset the lower bound
-        min_efo = self.processor.filtered_dataframe["efo"].values.min()
+        min_efo = self.processor.filtered_dataframe["efo"].to_numpy().min()
         max_efo = cutoff_frequency
         self.state.efo_thresholds = (min_efo, max_efo)
 
         # Update plot
         self.efo_region.setRegion(self.state.efo_thresholds)
 
-    @Slot(name="run_cfr_auto_threshold")
+    @Slot()
     def run_cfr_auto_threshold(self):
         """Run auto-threshold on CFR values and update the plots."""
 
         # Is there something to calculate?
         if (
             not self.state.enable_cfr_lower_threshold
             and not self.state.enable_cfr_upper_threshold
         ):
             print("Both lower and upper CFR thresholds are disabled.")
             return
 
+        if self.processor.filtered_dataframe is None:
+            return
+
         # Initialize values
         if self.state.cfr_thresholds is None:
-            min_cfr = self.processor.filtered_dataframe["cfr"].values.min()
-            max_cfr = self.processor.filtered_dataframe["cfr"].values.max()
+            min_cfr = self.processor.filtered_dataframe["cfr"].to_numpy().min()
+            max_cfr = self.processor.filtered_dataframe["cfr"].to_numpy().max()
         else:
             min_cfr = self.state.cfr_thresholds[0]
             max_cfr = self.state.cfr_thresholds[1]
 
         # Calculate thresholds for CFR
         upper_thresh_cfr, lower_thresh_cfr, _, _ = get_robust_threshold(
-            self.processor.filtered_dataframe["cfr"].values,
+            self.processor.filtered_dataframe["cfr"].to_numpy(),
             factor=self.state.cfr_threshold_factor,
         )
         if self.state.enable_cfr_lower_threshold:
             min_cfr = lower_thresh_cfr
         if self.state.enable_cfr_upper_threshold:
             max_cfr = upper_thresh_cfr
         self.state.cfr_thresholds = (min_cfr, max_cfr)
 
         # Update plot
         self.cfr_region.setRegion(self.state.cfr_thresholds)
 
-    @Slot(name="run_tr_len_auto_threshold")
+    @Slot()
     def run_tr_len_auto_threshold(self):
         """Run auto-run_tr_len_auto_threshold on Trace Length values and update the plots."""
 
         # Calculate the top percentile
-        n = self.processor.filtered_dataframe_stats["n"].values
+        n = self.processor.filtered_dataframe_stats["n"].to_numpy()
 
         # Get the value of the percentile
         percentile = float(self.ui.leTrLenTopPercentile.text())
 
         # Calculate the value
         p = np.percentile(n, percentile)
 
         # Update the thresholds
         thresholds = self.state.tr_len_thresholds
         self.state.tr_len_thresholds = (thresholds[0], p)
 
         # Update plot
         self.tr_len_region.setRegion(self.state.tr_len_thresholds)
 
-    @Slot(int, name="persist_cfr_lower_threshold")
+    @Slot(int)
     def persist_cfr_lower_threshold(self, state):
         self.state.enable_cfr_lower_threshold = state != 0
         self.cfr_lower_bound_state_changed.emit()
 
-    @Slot(int, name="persist_cfr_upper_threshold")
+    @Slot(int)
     def persist_cfr_upper_threshold(self, state):
         self.state.enable_cfr_upper_threshold = state != 0
         self.cfr_upper_bound_state_changed.emit()
 
-    @Slot(str, name="persist_efo_expected_frequency")
+    @Slot(str)
     def persist_efo_expected_frequency(self, text):
         try:
             efo_expected_frequency = float(text)
         except ValueError as _:
             return
 
         self.state.efo_expected_frequency = efo_expected_frequency
 
-    @Slot(str, name="persist_cfr_threshold_factor")
+    @Slot(str)
     def persist_cfr_threshold_factor(self, text):
         try:
             cfr_threshold_factor = float(text)
         except ValueError as _:
             return
         self.state.cfr_threshold_factor = cfr_threshold_factor
 
         # Broadcast
         self.cfr_threshold_factor_changed.emit()
 
-    @Slot(str, name="persist_tr_len_top_percentile")
+    @Slot(str)
     def persist_tr_len_top_percentile(self, text):
         try:
             tr_len_top_percentile = float(text)
         except ValueError as _:
             return
         if tr_len_top_percentile <= 0.0:
             tr_len_top_percentile = 0.0
             self.ui.leTrLenTopPercentile.setText(str(tr_len_top_percentile))
         if tr_len_top_percentile > 100.0:
             tr_len_top_percentile = 100.0
             self.ui.leTrLenTopPercentile.setText(str(tr_len_top_percentile))
         self.state.tr_len_top_percentile = tr_len_top_percentile
 
-    @Slot(name="run_efo_filter_and_broadcast_viewers_update")
+    @Slot()
     def run_efo_filter_and_broadcast_viewers_update(self):
         """Apply the EFO filter and inform the rest of the application that the data viewers should be updated."""
 
         # Apply the EFO filter if needed
         if self.state.efo_thresholds is not None:
             self.processor.filter_by_1d_range(
                 "efo", (self.state.efo_thresholds[0], self.state.efo_thresholds[1])
@@ -402,15 +409,15 @@
 
         # Update the histograms
         self.plot()
 
         # Signal that the external viewers should be updated
         self.data_filters_changed.emit()
 
-    @Slot(name="run_cfr_filter_and_broadcast_viewers_update")
+    @Slot()
     def run_cfr_filter_and_broadcast_viewers_update(self):
         """Apply the CFR filter and inform the rest of the application that the data viewers should be updated."""
 
         # Apply the CFR filter if needed
         if self.state.cfr_thresholds is not None:
             self.processor.filter_by_1d_range(
                 "cfr", (self.state.cfr_thresholds[0], self.state.cfr_thresholds[1])
@@ -426,15 +433,15 @@
 
         # Update the histograms
         self.plot()
 
         # Signal that the external viewers should be updated
         self.data_filters_changed.emit()
 
-    @Slot(name="run_tr_len_filter_and_broadcast_viewers_update")
+    @Slot()
     def run_tr_len_filter_and_broadcast_viewers_update(self):
         """Apply the Trace Length filter and inform the rest of the application that the data viewers should be updated."""
 
         # Apply the trace length filter if needed
         if self.state.tr_len_thresholds is not None:
             self.processor.filter_by_1d_stats(
                 "n", (self.state.tr_len_thresholds[0], self.state.tr_len_thresholds[1])
@@ -450,31 +457,44 @@
 
         # Update the histograms
         self.plot()
 
         # Signal that the external viewers should be updated
         self.data_filters_changed.emit()
 
-    @Slot(name="disable_buttons")
+    @Slot()
     def disable_buttons(self):
         self.ui.pbDetectCutoffFrequency.setEnabled(False)
         self.ui.pbCFRRunAutoThreshold.setEnabled(False)
         self.ui.pbEFORunFilter.setEnabled(False)
         self.ui.pbCFRRunFilter.setEnabled(False)
 
-    @Slot(name="enable_buttons")
+    @Slot()
     def enable_buttons(self):
         self.ui.pbDetectCutoffFrequency.setEnabled(True)
         self.ui.pbCFRRunAutoThreshold.setEnabled(True)
         self.ui.pbEFORunFilter.setEnabled(True)
         self.ui.pbCFRRunFilter.setEnabled(True)
 
     def plot(self):
         """Plot histograms."""
 
+        # Check that the necessary objects exist
+        if (
+            self.communication_label is None
+            or self.efo_plot is None
+            or self.cfr_plot is None
+            or self.tr_len_plot is None
+            or self.sx_plot is None
+            or self.sy_plot is None
+            or self.sz_plot is None
+            or self.processor.filtered_dataframe is None
+        ):
+            return
+
         # Hide the communications label
         self.communication_label.hide()
 
         # Make sure there is data to plot
         is_data = True
         if self.processor is None:
             is_data = False
@@ -512,20 +532,20 @@
             return
 
         # Histogram bin settings
         efo_auto_bins = self.state.efo_bin_size_hz == 0
 
         # Calculate the proper aspect ratio and view ranges for the relevant plots
         n_efo, efo_bin_edges, efo_bin_centers, efo_bin_width = prepare_histogram(
-            self.processor.filtered_dataframe["efo"].values,
+            self.processor.filtered_dataframe["efo"].to_numpy(),
             auto_bins=efo_auto_bins,
             bin_size=self.state.efo_bin_size_hz,
         )
         n_cfr, cfr_bin_edges, cfr_bin_centers, cfr_bin_width = prepare_histogram(
-            self.processor.filtered_dataframe["cfr"].values,
+            self.processor.filtered_dataframe["cfr"].to_numpy(),
             auto_bins=True,
             bin_size=0.0,
         )
 
         # Trace length distribution
         (
             n_tr_len,
@@ -632,15 +652,15 @@
             tim, _, _ = calculate_time_steps(self.processor.filtered_dataframe)
             (
                 n_tim,
                 n_tim_bin_edges,
                 n_tim_bin_centers,
                 n_tim_bin_width,
             ) = prepare_histogram(
-                tim["tim_diff"].values,
+                tim["tim_diff"].to_numpy(),
                 normalize=False,
                 auto_bins=True,
             )
 
             _ = self._create_histogram_plot(
                 "time_res",
                 self.sx_plot,
@@ -648,26 +668,26 @@
                 n_tim_bin_edges,
                 n_tim_bin_centers,
                 n_tim_bin_width,
                 axis_range=None,
                 brush="k",
                 support_thresholding=False,
             )
-            add_median_line(self.sx_plot, tim["tim_diff"].values, unit="ms")
+            add_median_line(self.sx_plot, tim["tim_diff"].to_numpy(), unit="ms")
             self.sx_plot.setTitle("Time resolution")
             self.sx_plot.show()
 
             # Displacement steps
             (
                 n_speeds,
                 n_speeds_bin_edges,
                 n_speeds_bin_centers,
                 n_speeds_bin_width,
             ) = prepare_histogram(
-                self.processor.filtered_dataframe_stats["avg_speed"].values,
+                self.processor.filtered_dataframe_stats["avg_speed"].to_numpy(),
                 normalize=False,
                 auto_bins=True,
             )
             _ = self._create_histogram_plot(
                 "speed",
                 self.sy_plot,
                 n_speeds,
@@ -676,28 +696,28 @@
                 n_speeds_bin_width,
                 axis_range=None,
                 brush="k",
                 support_thresholding=False,
             )
             add_median_line(
                 self.sy_plot,
-                self.processor.filtered_dataframe_stats["avg_speed"].values,
+                self.processor.filtered_dataframe_stats["avg_speed"].to_numpy(),
                 unit="nm/ms",
             )
             self.sy_plot.setTitle("Average speed per trace")
             self.sy_plot.show()
 
             # Total distance traveled per TID
             (
                 n_trav,
                 n_trav_bin_edges,
                 n_trav_bin_centers,
                 n_trav_bin_width,
             ) = prepare_histogram(
-                self.processor.filtered_dataframe_stats["total_dist"].values,
+                self.processor.filtered_dataframe_stats["total_dist"].to_numpy(),
                 normalize=False,
                 auto_bins=True,
             )
 
             # Remove distance traveled
             to_keep = n_trav > 0
             n_trav = n_trav[to_keep]
@@ -715,29 +735,29 @@
                 n_trav_bin_width,
                 axis_range=None,
                 brush="k",
                 support_thresholding=False,
             )
             add_median_line(
                 self.sz_plot,
-                self.processor.filtered_dataframe_stats["total_dist"].values,
+                self.processor.filtered_dataframe_stats["total_dist"].to_numpy(),
                 unit="nm",
             )
             self.sz_plot.setTitle("Total distance traveled per trace")
             self.sz_plot.show()
 
         else:
 
             #
             # Plot various statistics for localization datasets
             #
 
             # sx
             n_sx, sx_bin_edges, sx_bin_centers, sx_bin_width = prepare_histogram(
-                self.processor.filtered_dataframe_stats["sx"].values,
+                self.processor.filtered_dataframe_stats["sx"].to_numpy(),
                 auto_bins=True,
                 bin_size=0.0,
             )
             _ = self._create_histogram_plot(
                 "sx",
                 self.sx_plot,
                 n_sx,
@@ -745,22 +765,22 @@
                 sx_bin_centers,
                 sx_bin_width,
                 axis_range=self.loc_precision_range,
                 brush="k",
                 support_thresholding=False,
             )
             add_median_line(
-                self.sx_plot, self.processor.filtered_dataframe_stats["sx"].values
+                self.sx_plot, self.processor.filtered_dataframe_stats["sx"].to_numpy()
             )
             self.sx_plot.setTitle("σx")
             self.sx_plot.show()
 
             # sy
             n_sy, sy_bin_edges, sy_bin_centers, sy_bin_width = prepare_histogram(
-                self.processor.filtered_dataframe_stats["sy"].values,
+                self.processor.filtered_dataframe_stats["sy"].to_numpy(),
                 auto_bins=True,
                 bin_size=0.0,
             )
             _ = self._create_histogram_plot(
                 "sy",
                 self.sy_plot,
                 n_sy,
@@ -768,23 +788,23 @@
                 sy_bin_centers,
                 sy_bin_width,
                 axis_range=self.loc_precision_range,
                 brush="k",
                 support_thresholding=False,
             )
             add_median_line(
-                self.sy_plot, self.processor.filtered_dataframe_stats["sy"].values
+                self.sy_plot, self.processor.filtered_dataframe_stats["sy"].to_numpy()
             )
             self.sy_plot.setTitle("σy")
             self.sy_plot.show()
 
             # sz
             if self.processor.is_3d:
                 n_sz, sz_bin_edges, sz_bin_centers, sz_bin_width = prepare_histogram(
-                    self.processor.filtered_dataframe_stats["sz"].values,
+                    self.processor.filtered_dataframe_stats["sz"].to_numpy(),
                     auto_bins=True,
                     bin_size=0.0,
                 )
                 _ = self._create_histogram_plot(
                     "sz",
                     self.sz_plot,
                     n_sz,
@@ -793,15 +813,15 @@
                     sz_bin_width,
                     axis_range=self.loc_precision_range,
                     brush="k",
                     support_thresholding=False,
                 )
                 add_median_line(
                     self.sz_plot,
-                    self.processor.filtered_dataframe_stats["sz"].values,
+                    self.processor.filtered_dataframe_stats["sz"].to_numpy(),
                 )
                 self.sz_plot.setTitle("σz")
                 self.sz_plot.show()
             else:
                 self.sz_plot.hide()
 
         # Announce that the plotting has completed
@@ -929,47 +949,78 @@
             return
         if not hasattr(ev.currentItem, "data_label"):
             ev.ignore()
             return
 
         if ev.button() == Qt.MouseButton.RightButton:
             menu = QMenu()
+
             ranges_action = QAction("Set range")
             ranges_action.triggered.connect(
                 lambda checked: self.roi_open_ranges_dialog(ev.currentItem.data_label)
             )
             menu.addAction(ranges_action)
+
             filter_action = QAction("Filter")
             filter_action.triggered.connect(
                 lambda checked: self.trigger_filter_action(ev.currentItem)
             )
             menu.addAction(filter_action)
             menu.addSeparator()
+
             reset_action = QAction("Reset default axis range")
             reset_action.triggered.connect(
                 lambda checked: self.reset_default_axis_range(ev.currentItem)
             )
             menu.addAction(reset_action)
+
             shift_action = QAction("Move x axis origin to 0")
             shift_action.triggered.connect(
                 lambda checked: self.shift_x_axis_origin_to_zero(ev.currentItem)
             )
             menu.addAction(shift_action)
             menu.addSeparator()
+
             export_action = QAction("Export plot")
             export_action.triggered.connect(
                 lambda checked: export_plot_interactive(ev.currentItem)
             )
             menu.addAction(export_action)
+
+            export_all_action = QAction("Export all plots")
+            export_all_action.triggered.connect(self.collect_and_export_all_plots)
+            menu.addAction(export_all_action)
+
             pos = ev.screenPos()
             menu.exec(QPoint(int(pos.x()), int(pos.y())))
             ev.accept()
         else:
             ev.ignore()
 
+    def collect_and_export_all_plots(self):
+        items = {
+            "efo": self.efo_plot.getPlotItem().getViewBox(),
+            "cfr": self.cfr_plot.getPlotItem().getViewBox(),
+            "tr_len": self.tr_len_plot.getPlotItem().getViewBox(),
+            self.sx_plot.getPlotItem()
+            .getViewBox()
+            .data_label: self.sx_plot.getPlotItem()
+            .getViewBox(),
+            self.sy_plot.getPlotItem()
+            .getViewBox()
+            .data_label: self.sy_plot.getPlotItem()
+            .getViewBox(),
+        }
+        if self.processor.is_tracking or self.processor.is_3d:
+            items[
+                self.sz_plot.getPlotItem().getViewBox().data_label
+            ] = self.sz_plot.getPlotItem().getViewBox()
+
+        export_all_plots_interactive(items)
+
     def roi_open_ranges_dialog(self, item):
         """Open dialog to manually set the filter ranges"""
         if self.roi_ranges_dialog is None:
             self.roi_ranges_dialog = ROIRanges()
             self.roi_ranges_dialog.data_ranges_changed.connect(
                 self.roi_changes_finished
             )
@@ -983,36 +1034,43 @@
         """Set the lower range of the x axis of the passed viewbox to 0."""
         if isinstance(item, ViewBox):
             view_box = item
         elif isinstance(item, AxisItem):
             view_box = item.getViewBox()
         else:
             return
+        if view_box is None:
+            return
         view_range = view_box.viewRange()
         view_box.setRange(xRange=(0.0, view_range[0][1]))
 
     def reset_default_axis_range(self, item):
         if isinstance(item, ViewBox):
             view_box = item
         elif isinstance(item, AxisItem):
             view_box = item.getViewBox()
         else:
             return
-        if item.data_label == "efo":
+        if view_box is None:
+            return
+        if item.data_label == "efo" and self.state.efo_range is not None:
             view_box.setRange(xRange=(self.state.efo_range[0], self.state.efo_range[1]))
             self.efo_range = self.state.efo_range
-        elif item.data_label == "cfr":
+        elif item.data_label == "cfr" and self.state.cfr_range is not None:
             view_box.setRange(xRange=(self.state.cfr_range[0], self.state.cfr_range[1]))
             self.cfr_range = self.state.cfr_range
-        elif item.data_label == "tr_len":
+        elif item.data_label == "tr_len" and self.state.tr_len_range is not None:
             view_box.setRange(
                 xRange=(self.state.tr_len_range[0], self.state.tr_len_range[1])
             )
             self.tr_len_range = self.state.tr_len_range
-        elif item.data_label in ["sx", "sy", "sz"]:
+        elif (
+            item.data_label in ["sx", "sy", "sz"]
+            and self.state.loc_precision_range is not None
+        ):
             view_box.setRange(
                 xRange=(
                     self.state.loc_precision_range[0],
                     self.state.loc_precision_range[1],
                 )
             )
         else:
@@ -1022,14 +1080,18 @@
         """Set the lower range of the x axis of the passed viewbox to 0."""
         if isinstance(item, ViewBox):
             view_box = item
         elif isinstance(item, AxisItem):
             view_box = item.getViewBox()
         else:
             return
+        if view_box is None:
+            return
+        if not hasattr(view_box, "data_label"):
+            return
         plot_id = view_box.data_label
         if plot_id == "efo":
             self.run_efo_filter_and_broadcast_viewers_update()
         elif plot_id == "cfr":
             self.run_cfr_filter_and_broadcast_viewers_update()
         elif plot_id == "tr_len":
             self.run_tr_len_filter_and_broadcast_viewers_update()
@@ -1048,18 +1110,25 @@
             value = f"{min(region):.2f}"
         elif low_thresh_label.format == "{value:.0f}":
             value = f"{min(region):.0f}"
         else:
             value = f"{min(region)}"
         low_thresh_label.textItem.setPlainText(value)
 
-    @Slot(None, name="roi_changes_finished")
+    @Slot()
     def roi_changes_finished(self):
         """Called when the ROIChanges dialog has accepted the changes."""
 
+        if (
+            self.efo_region is None
+            or self.cfr_region is None
+            or self.tr_len_region is None
+        ):
+            return
+
         # Signal blocker on self.efo_plot, self.cfr_plot and self.tr_len_plot
         cfr_plot_blocker = QSignalBlocker(self.cfr_plot)
         efo_plot_blocker = QSignalBlocker(self.efo_plot)
         tr_len_plot_blocker = QSignalBlocker(self.tr_len_plot)
 
         # Block signals from self.efo_plot, self.cfr_plot and self.tr_len_plot
         cfr_plot_blocker.reblock()
@@ -1107,14 +1176,17 @@
         """Reset the y axis range whenever the x range changes."""
         viewbox.setYRange(viewbox.y_min, viewbox.y_max)
         viewbox.setAutoVisible(y=True)
 
     def change_efo_bounds(self):
         """Update the efo bounds on the histogram (without broadcasting any events)."""
 
+        if self.efo_region is None:
+            return
+
         # Signal blocker on self.efo_plot
         efo_plot_blocker = QSignalBlocker(self.efo_plot)
 
         # Block signals from self.efo_plot and self.cfr_plot
         efo_plot_blocker.reblock()
 
         # Update the thresholds in the EFO and CFR histograms.
@@ -1122,14 +1194,17 @@
 
         # Unblock the self.efo_plot and self.cfr_plot signals
         efo_plot_blocker.unblock()
 
     def change_cfr_bounds(self):
         """Update the cfr bounds on the histogram (without broadcasting any events)."""
 
+        if self.cfr_region is None:
+            return
+
         # Signal blocker on self.efo_plot
         cfr_plot_blocker = QSignalBlocker(self.cfr_plot)
 
         # Block signals from self.efo_plot and self.cfr_plot
         cfr_plot_blocker.reblock()
 
         # Update the thresholds in the EFO and CFR histograms.
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/analyzer.ui` & `pyminflux-0.4.1/pyminflux/ui/analyzer.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/assets/Logo_v3.icns` & `pyminflux-0.4.1/pyminflux/ui/assets/Logo_v3.icns`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/assets/Logo_v3.ico` & `pyminflux-0.4.1/pyminflux/ui/assets/Logo_v3.ico`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/assets/Logo_v3.png` & `pyminflux-0.4.1/pyminflux/ui/assets/Logo_v3.png`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/assets/Logo_v3_small.png` & `pyminflux-0.4.1/pyminflux/ui/assets/Logo_v3_small.png`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/assets/create_resources.sh` & `pyminflux-0.4.1/pyminflux/writer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-#!/bin/bash
-#
-# Copyright (c) 2022 - 2024 D-BSSE, ETH Zurich.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-#  limitations under the License.
+#  Copyright (c) 2022 - 2024 D-BSSE, ETH Zurich.
 #
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#   limitations under the License.
 #
 
-pyside6-rcc ../../resources.qrc -o ../../resources.py
+__doc__ = "Writer of processed MINFLUX data."
+__all__ = ["MinFluxWriter", "PyMinFluxNativeWriter"]
 
+from ._native_writer import PyMinFluxNativeWriter
+from ._writer import MinFluxWriter
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/assets/png_to_icns.sh` & `pyminflux-0.4.1/pyminflux/ui/assets/png_to_icns.sh`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/color_unmixer.py` & `pyminflux-0.4.1/pyminflux/ui/color_unmixer.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 class ColorUnmixer(QDialog, Ui_ColorUnmixer):
     """
     A QDialog to display the dcr histogram and to assigning the fluorophore ids.
     """
 
     # Signal that the fluorophore IDs have been assigned
-    fluorophore_ids_assigned = Signal(int, name="fluorophore_ids_assigned")
+    fluorophore_ids_assigned = Signal(int)
 
     def __init__(self, processor: MinFluxProcessor):
         # Call the base class
         super().__init__()
 
         # Initialize the dialog
         self.ui = Ui_ColorUnmixer()
@@ -91,54 +91,54 @@
         self.ui.leBinSize.editingFinished.connect(self.plot_dcr_histogram)
         self.ui.leManualThreshold.textChanged.connect(self.persist_dcr_manual_threshold)
         self.ui.pbDetect.clicked.connect(self.detect_fluorophores)
         self.ui.pbAssign.clicked.connect(self.assign_fluorophores_ids)
         self.ui.pbPreview.clicked.connect(self.preview_manual_assignment)
         self.ui.pbManualAssign.clicked.connect(self.assign_fluorophores_ids)
 
-    @Slot(str, name="persist_dcr_bin_size")
+    @Slot(str)
     def persist_dcr_bin_size(self, text):
         try:
             dcr_bin_size = float(text)
         except ValueError as _:
             return
         self.state.dcr_bin_size = dcr_bin_size
 
-    @Slot(str, name="persist_num_fluorophores")
+    @Slot(str)
     def persist_num_fluorophores(self, text):
         num_fluorophores = self.ui.cbNumFluorophores.currentIndex() + 1
         self.state.num_fluorophores = num_fluorophores
         self.ui.pbAssign.setEnabled(False)
 
-    @Slot(str, name="persist_dcr_manual_threshold")
+    @Slot(str)
     def persist_dcr_manual_threshold(self, text):
         try:
             dcr_manual_threshold = float(text)
         except ValueError as _:
             return
         self.state.dcr_manual_threshold = float(dcr_manual_threshold)
 
-    @Slot(None, name="plot_dcr_histogram")
+    @Slot()
     def plot_dcr_histogram(self):
         """Plot the dcr histogram. This is always performed assuming all data belongs to one fluorophore."""
 
         # Do we have something to plot?
         if self.processor is None or self.processor.full_dataframe is None:
             return
 
         if self.state.dcr_bin_size == 0:
             # Calculate the dcr histogram
             n_dcr, dcr_bin_edges, dcr_bin_centers, dcr_bin_width = prepare_histogram(
-                self.processor.full_dataframe["dcr"].values,
+                self.processor.full_dataframe["dcr"].to_numpy(),
                 auto_bins=True,
             )
         else:
             # Calculate the dcr histogram
             n_dcr, dcr_bin_edges, dcr_bin_centers, dcr_bin_width = prepare_histogram(
-                self.processor.full_dataframe["dcr"].values,
+                self.processor.full_dataframe["dcr"].to_numpy(),
                 auto_bins=False,
                 bin_size=self.state.dcr_bin_size,
             )
 
         # Remember the global histogram range and step
         self.n_dcr_max = n_dcr.max()
         self.dcr_bin_edges = dcr_bin_edges
@@ -166,20 +166,23 @@
         self.plot_widget.setLabel("bottom", "Complete dataset")
         self.plot_widget.setMenuEnabled(False)
         self.plot_widget.addItem(chart)
         self.plot_widget.scene().sigMouseClicked.connect(
             self.histogram_raise_context_menu
         )
 
-    @Slot(None, name="preview_manual_assignment")
+    @Slot()
     def preview_manual_assignment(self):
         """Preview the manual assignment."""
 
+        if self.processor is None or self.processor.full_dataframe is None:
+            return
+
         # Get the data
-        dcr = self.processor.full_dataframe["dcr"].values
+        dcr = self.processor.full_dataframe["dcr"].to_numpy()
         if len(dcr) == 0:
             return
 
         # Get the threshold
         threshold = float(self.ui.leManualThreshold.text())
 
         # Keep track of the total number of elements for normalisation
@@ -232,20 +235,20 @@
 
         # Store the predictions (1-shifted)
         self.assigned_fluorophore_ids = fluo_ids
 
         # Make sure to enable the assign button
         self.ui.pbManualAssign.setEnabled(True)
 
-    @Slot(None, name="detect_fluorophores")
+    @Slot()
     def detect_fluorophores(self):
         """Detect fluorophores."""
 
         # Get the data
-        dcr = self.processor.full_dataframe["dcr"].values
+        dcr = self.processor.full_dataframe["dcr"].to_numpy()
         if len(dcr) == 0:
             return
 
         # Fit the data to the requested number of clusters
         fluo_ids = assign_data_to_clusters(dcr, self.state.num_fluorophores, seed=42)
 
         # Reassign fluorophore IDs majority vote if necessary
@@ -261,15 +264,15 @@
         # Prepare some colors
         brushes = ["g", "m", "b", "r", "c"]
 
         # Calculate the bar width as a function of the number of fluorophores
         bar_width = 0.9 / self.state.num_fluorophores
         offset = self.dcr_bin_width / self.state.num_fluorophores
 
-        # Keep track of the total number of values for histogrm normalization
+        # Keep track of the total number of values for histogram normalization
         n_values = len(dcr)
 
         # Create new histograms
         for f in range(1, self.state.num_fluorophores + 1):
             data = dcr[fluo_ids == f]
             if len(data) == 0:
                 continue
@@ -292,15 +295,15 @@
 
         # Store the predictions (1-shifted)
         self.assigned_fluorophore_ids = fluo_ids
 
         # Make sure to enable the assign button
         self.ui.pbAssign.setEnabled(True)
 
-    @Slot(None, name="assign_fluorophores_ids")
+    @Slot()
     def assign_fluorophores_ids(self):
         """Assign the fluorophores ids."""
 
         if self.assigned_fluorophore_ids is None:
             return
 
         # Assign the IDs via the processor
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/color_unmixer.ui` & `pyminflux-0.4.1/pyminflux/ui/color_unmixer.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/dataviewer.py` & `pyminflux-0.4.1/pyminflux/ui/dataviewer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/emittingstream.py` & `pyminflux-0.4.1/pyminflux/ui/emittingstream.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 class EmittingStream(QObject):
     """
     Redirect standard output and error to be displayed by a QWidget.
     """
 
-    signal_textWritten = Signal(str, name="signal_textWritten")
+    signal_text_written = Signal(str)
 
     def write(self, text):
-        self.signal_textWritten.emit(str(text))
+        self.signal_text_written.emit(str(text))
 
     def flush(self):
         sys.stdout = sys.__stdout__
         sys.stdout.flush()
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/frc_tool.py` & `pyminflux-0.4.1/pyminflux/ui/frc_tool.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,224 +8,29 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
-import os
 import warnings
 
 import numpy as np
 import pyqtgraph as pg
-from PySide6.QtCore import (
-    QMutex,
-    QMutexLocker,
-    QObject,
-    QPoint,
-    QRunnable,
-    QThread,
-    QThreadPool,
-    Signal,
-    Slot,
-)
+from PySide6.QtCore import QPoint, Slot
 from PySide6.QtGui import QAction, QDoubleValidator, QIntValidator, Qt
 from PySide6.QtWidgets import QDialog, QMenu
 
-from ..fourier import estimate_resolution_by_frc
 from ..processor import MinFluxProcessor
 from ..state import State
+from ..threads.frc import FRCProcessorThread
 from .helpers import export_plot_interactive
 from .ui_frc_tool import Ui_FRCTool
 
 
-class CancelFlag:
-    """Encapulates a Mutex to communicate state change to the Workers."""
-
-    def __init__(self):
-        self._cancelled = False
-        self._mutex = QMutex()
-
-    def is_cancelled(self):
-        with QMutexLocker(self._mutex):
-            return self._cancelled
-
-    def cancel(self):
-        with QMutexLocker(self._mutex):
-            self._cancelled = True
-
-
-class WorkerSignals(QObject):
-    """Encapsulates Signals to be used by the Workers."""
-
-    # Signal progress, completion, and request for stop
-    progress = Signal(int)
-    result = Signal(int, np.ndarray)
-
-
-class Worker(QRunnable):
-    """Worker to run the FRC analysis in parallel over all bins."""
-
-    def __init__(
-        self, index, processor, start_time, end_time, sxy, rx, ry, n_reps, cancel_flag
-    ):
-        """Constructor."""
-
-        super().__init__()
-        self.index = index
-        self.processor = processor
-        self.start_time = start_time
-        self.end_time = end_time
-        self.sxy = sxy
-        self.rx = rx
-        self.ry = ry
-        self.n_reps = n_reps
-        self.signals = WorkerSignals()
-        self.cancel_flag = cancel_flag
-
-    def run(self):
-        # Check that the processing has not been interrupted
-        if self.cancel_flag.is_cancelled():
-            # Signal completion
-            self.signals.result.emit(self.index, None)
-            self.signals.progress.emit(1)
-            return
-
-        # Extract the data
-        df = self.processor.select_by_1d_range(
-            "tim", x_range=(self.start_time, self.end_time)
-        )
-        df_gr = df.groupby("tid")
-        mx = df_gr["x"].mean()
-        my = df_gr["y"].mean()
-
-        # Estimate the resolution by FRC
-        _, _, _, resolutions, _ = estimate_resolution_by_frc(
-            x=mx,
-            y=my,
-            sx=self.sxy,
-            sy=self.sxy,
-            rx=self.rx,
-            ry=self.ry,
-            num_reps=self.n_reps,
-            seed=None,
-            return_all=True,
-        )
-
-        # Convert to nm
-        resolutions = 1e9 * np.array(resolutions)
-
-        # Signal completion
-        self.signals.result.emit(self.index, resolutions)
-        self.signals.progress.emit(1)
-
-
-class ProcessorThread(QThread):
-    # Signal progress and completion
-    processing_started = Signal()
-    processing_progress_updated = Signal(int)
-    processing_interrupted = Signal()
-    processing_finished = Signal()
-
-    def __init__(self, processor, t_start, t_steps, sxy, rx, ry, n_reps):
-        """Constructor."""
-        super().__init__()
-
-        # Set arguments
-        self.processor = processor
-        self.t_start = t_start
-        self.t_steps = t_steps
-        self.sxy = sxy
-        self.rx = rx
-        self.ry = ry
-        self.n_reps = n_reps
-
-        # Initialize a thread pool
-        self.thread_pool = QThreadPool.globalInstance()
-        self.thread_pool.setMaxThreadCount(os.cpu_count())
-
-        # Keep track of the progress of the various threads
-        self.progress = 0
-
-        # Initialize output
-        self.all_resolutions = None
-
-        # Initialize CancelFlag to communicate to Worker in a thread-safe manner
-        self.cancel_flag = CancelFlag()
-
-    def run(self):
-        """Run the computation."""
-
-        # Signal start
-        self.processing_started.emit()
-
-        # Allocate space for the results
-        self.all_resolutions = np.empty(
-            (len(self.t_steps), self.n_reps), dtype=np.float32
-        )
-        self.all_resolutions.fill(np.nan)
-
-        # Reset the progress counter
-        self.progress = 0
-
-        # Create the workers and add them to the thread pool
-        for i, t in enumerate(self.t_steps):
-            if self.cancel_flag.is_cancelled():
-                # This is unlikely: threads are added very fast to the QThreadPool's queue
-                self.processing_interrupted.emit()
-                break
-
-            # Create the processor_thread
-            worker = Worker(
-                index=i,
-                processor=self.processor,
-                start_time=self.t_start,
-                end_time=t,
-                sxy=self.sxy,
-                rx=self.rx,
-                ry=self.ry,
-                n_reps=self.n_reps,
-                cancel_flag=self.cancel_flag,
-            )
-
-            # Attach all signals
-            worker.signals.result.connect(self.store_result)
-            worker.signals.progress.connect(self.broadcast_update_progress)
-
-            # Add the thread to the pool and start it
-            self.thread_pool.start(
-                worker
-            )  # Add the processor_thread to the thread pool
-
-        # Wait for all threads to finish
-        self.thread_pool.waitForDone()
-
-        # Signal completion
-        self.processing_finished.emit()
-
-    def stop(self):
-        # Inform the queued Workers to skip computation
-        self.cancel_flag.cancel()
-
-        # Clear the ThreadPool queue
-        self.thread_pool.clear()
-
-    @Slot(int, np.ndarray, name="store_result")
-    def store_result(self, index, result):
-        if result is not None:
-            self.all_resolutions[index, :] = result
-
-    def broadcast_update_progress(self, value):
-        # Signal progress
-        self.progress += value
-        self.processing_progress_updated.emit(
-            int(np.round(100 * (self.progress + 1) / len(self.t_steps)))
-        )
-
-
 class FRCTool(QDialog, Ui_FRCTool):
     def __init__(self, processor: MinFluxProcessor):
         """Constructor."""
 
         # Call the base class
         super().__init__()
 
@@ -258,20 +63,22 @@
 
         #
         # Set defaults
         #
 
         # Lateral (xy) resolution
         self.ui.leLateralResolution.setText(str(self.state.frc_lateral_resolution))
-        self.ui.leNumRepeats.setValidator(QDoubleValidator(bottom=0.0, decimals=2))
+        self.ui.leNumRepeats.setValidator(
+            QDoubleValidator(bottom=0.0, top=np.Inf, decimals=2)
+        )
 
         # Temporal (s) resolution
         self.ui.leTemporalResolution.setText(str(self.state.frc_temporal_resolution))
         self.ui.leTemporalResolution.setValidator(
-            QDoubleValidator(bottom=0.0, decimals=1)
+            QDoubleValidator(bottom=0.0, top=np.Inf, decimals=1)
         )
 
         # Endpoint estimation
         self.ui.cbEndpoint.setChecked(self.state.frc_endpoint_only)
         self.ui.lbTemporalResolution.setEnabled(True)
         self.ui.leTemporalResolution.setEnabled(True)
         if self.state.frc_endpoint_only:
@@ -319,30 +126,36 @@
         # Do not capture key events for now
         ev.ignore()
 
     def set_processor(self, processor: MinFluxProcessor):
         """Reset the internal state."""
         self.processor = processor
 
-    @Slot(int, name="persist_frc_endpoint_only")
+    @Slot(int)
     def persist_frc_endpoint_only(self, value):
         """Persist the selection for plotting average positions."""
         if value == Qt.CheckState.Checked.value:
             self.state.frc_endpoint_only = True
             self.ui.lbTemporalResolution.setEnabled(False)
             self.ui.leTemporalResolution.setEnabled(False)
         else:
             self.state.frc_endpoint_only = False
             self.ui.lbTemporalResolution.setEnabled(True)
             self.ui.leTemporalResolution.setEnabled(True)
 
-    @Slot(name="run_frc_analysis")
+    @Slot()
     def run_frc_analysis(self):
         """Run FRC analysis to estimate signal resolution."""
 
+        if self.frc_plot is None:
+            raise Exception("The PlotWidget object is not ready!")
+
+        if self.processor is None or self.processor.filtered_dataframe is None:
+            return
+
         # Mark that there is no plot ready to export
         self.plot_ready_to_export = False
 
         # Is there data to process?
         if len(self.processor.filtered_dataframe.index) == 0:
             self.frc_plot.setTitle("No data.")
             return
@@ -357,15 +170,15 @@
             self.processor.filtered_dataframe["x"].max(),
         )
         ry = (
             self.processor.filtered_dataframe["y"].min(),
             self.processor.filtered_dataframe["y"].max(),
         )
 
-        # Prepare the arguments for the Worker
+        # Prepare the arguments for the AutoUpdateCheckerWorker
         t_start = self.processor.filtered_dataframe["tim"].min()
         t_end = self.processor.filtered_dataframe["tim"].max()
 
         # Run temporal analysis or endpoint estimation?
         if self.state.frc_endpoint_only:
             # We only consider one step with the whole data
             t_steps = [t_end + 1.0]
@@ -376,15 +189,15 @@
             n_steps = int(np.round((t_end - t_start) / t_step))
             t_steps = np.linspace(t_start, t_end, n_steps)
             t_steps = t_steps[1:]
 
         # Create the new processor_thread
         if self.processor_thread is not None:
             del self.processor_thread
-        self.processor_thread = ProcessorThread(
+        self.processor_thread = FRCProcessorThread(
             self.processor, t_start, t_steps, sxy, rx, ry, n_reps
         )
         self.processor_thread.processing_started.connect(
             self.update_ui_on_process_start
         )
         self.processor_thread.processing_progress_updated.connect(
             self.update_progress_bar
@@ -397,51 +210,54 @@
         )
         self.processor_thread.processing_finished.connect(self.update_ui_on_process_end)
         self.processor_thread.processing_finished.connect(self.collect_results_and_plot)
 
         # Now process in the local processor_thread
         self.processor_thread.start()
 
-    @Slot(name="stop_frc_analysis")
+    @Slot()
     def stop_frc_analysis(self):
         if self.processor_thread is None:
             return
         self.processor_thread.stop()
 
-    @Slot(str, name="persist_frc_lateral_resolution")
+    @Slot(str)
     def persist_frc_lateral_resolution(self, text):
         try:
             frc_lateral_resolution = float(text)
         except ValueError as _:
             return
         self.state.frc_lateral_resolution = frc_lateral_resolution
 
-    @Slot(str, name="persist_frc_temporal_resolution")
+    @Slot(str)
     def persist_frc_temporal_resolution(self, text):
         try:
             frc_temporal_resolution = float(text)
         except ValueError as _:
             return
         self.state.frc_temporal_resolution = frc_temporal_resolution
 
-    @Slot(str, name="persist_frc_num_repeats")
+    @Slot(str)
     def persist_frc_num_repeats(self, text):
         try:
             frc_num_repeats = int(text)
         except ValueError as _:
             return
         self.state.frc_num_repeats = frc_num_repeats
 
-    @Slot(int, name="update_progress_bar")
+    @Slot(int)
     def update_progress_bar(self, value):
         self.ui.progress_bar.setValue(value)
 
     def plot(self, time_steps, resolutions):
         """Plot histograms."""
 
+        if self.frc_plot is None:
+            raise Exception("The PlotWidget object is not ready!")
+
         # Clear the plot
         self.clear_plot()
 
         # Show x and y grids
         self.frc_plot.showGrid(x=True, y=True)
 
         # Set properties of the label for y-axis
@@ -524,14 +340,17 @@
             self.frc_plot.setTitle(
                 f"Endpoint resolution = {res:.1f} ± {se:.1f}nm", size="16px"
             )
 
     def clear_plot(self):
         """Clear the plot."""
 
+        if self.frc_plot is None:
+            raise Exception("The PlotWidget object ois not ready!")
+
         for item in self.frc_plot.allChildItems():
             self.frc_plot.removeItem(item)
 
     def update_ui_on_process_start(self):
         """Disable elements and inform that a processing is ongoing."""
 
         # Disable all parameter widgets
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/frc_tool.ui` & `pyminflux-0.4.1/pyminflux/ui/frc_tool.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/helpers/__init__.py` & `pyminflux-0.4.1/pyminflux/ui/helpers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 
 from ._helpers import (
     BottomLeftAnchoredScaleBar,
     add_median_line,
     create_brushes_by,
+    export_all_plots_interactive,
     export_plot_interactive,
     export_to_image,
     update_brushes_by_,
 )
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/helpers/_helpers.py` & `pyminflux-0.4.1/pyminflux/ui/helpers/_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+import time
+from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pyqtgraph as pg
 from pyqtgraph import AxisItem, ViewBox
 from PySide6.QtCore import QPointF, QRect, QRectF
@@ -32,37 +34,101 @@
     elif isinstance(item, AxisItem):
         view_box = item.getViewBox()
     elif isinstance(item, pg.PlotItem):
         view_box = item.getViewBox()
     else:
         return
 
+    # Get the State
+    state = State()
+
+    # Default to the input data path
+    if state.last_selected_path is not None:
+        save_path = str(state.last_selected_path)
+    else:
+        save_path = str(Path(".").absolute())
+
     # Ask the user to pick a file name
     filename, ext = QFileDialog.getSaveFileName(
         parent,
-        "Export filtered data",
-        ".",
+        "Export current plot",
+        save_path,
         "PNG images (*.png)",
     )
 
     # Did the user cancel?
     if filename == "":
         return
 
     # Make sure to add the extension
     if not filename.lower().endswith(".png"):
         filename += ".png"
 
-    # Get the dpi from the State
-    state = State()
-
     # Save the scene to file
     export_to_image(view_box, filename, dpi=state.plot_export_dpi)
 
 
+def export_all_plots_interactive(items: dict, parent=None):
+    """Save the content of the current scene to a PNG image."""
+
+    if len(items) == 0:
+        return
+
+    # Get the State
+    state = State()
+
+    # Default to the input data path
+    if state.last_selected_path is not None:
+        save_path = str(state.last_selected_path)
+    else:
+        save_path = str(Path(".").absolute())
+
+    # Ask the user to pick a file name
+    filename, ext = QFileDialog.getSaveFileName(
+        parent,
+        "Set plots common name",
+        save_path,
+        "PNG images (*.png)",
+    )
+
+    # Did the user cancel?
+    if filename == "":
+        return
+
+    # Turn filename into a Path object
+    filename = Path(filename)
+
+    # Test if any of the output file names already exists
+    timestamp = ""
+    for name, item in items.items():
+        # Build the filename
+        test_filename = filename.parent / f"{filename.stem}_{name}.png"
+        if test_filename.exists():
+            timestamp = "_" + datetime.fromtimestamp(time.time()).strftime(
+                "%Y%m%d_%H%M%S"
+            )
+            break
+
+    for name, item in items.items():
+        if isinstance(item, ViewBox):
+            view_box = item
+        elif isinstance(item, AxisItem):
+            view_box = item.getViewBox()
+        elif isinstance(item, pg.PlotItem):
+            view_box = item.getViewBox()
+        else:
+            return
+
+        # Build the filename
+        out_filename = str(filename.parent / f"{filename.stem}_{name}{timestamp}.png")
+
+        # Save the scene to file
+        export_to_image(view_box, out_filename, dpi=state.plot_export_dpi)
+
+
 def export_to_image(item: pg.ViewBox, out_file_name: Union[Path, str], dpi: int = 600):
     """Export current QGraphicsScene to file."""
 
     # Get the scene from the viewBox
     if isinstance(item, pg.ViewBox):
         plot_item = item.parentItem()
         plot_widget = plot_item.getViewWidget()
@@ -223,15 +289,17 @@
     brushes_for_ids = [id_to_brush[identifier] for identifier in identifiers]
 
     # Return the list of brushes (and references) and the mapping between id and brush
     return brushes_for_ids, id_to_brush
 
 
 def update_brushes_by_(
-    identifiers: np.ndarray, id_to_brush: dict[tuple[int, Any], Any]
+    identifiers: np.ndarray,
+    id_to_brush: dict[tuple[int, Any], Any],
+    color_scheme: Optional[str] = None,
 ) -> tuple[list[Any], dict[tuple[int, Any], Any]]:
     """Updated the QBrush instances to be used in a ScatterPlotItem my mapping
     an (updated) list to identifier to the dictionary of cached unique ID to QBrush
     map.
 
     Parameters
     ----------
@@ -239,14 +307,23 @@
     identifiers: np.ndarray
         Identifiers to be used to re-assign colors.
 
     id_to_brush: dict[tuple[int, Any], Any]
         Cached map of unique ID to QBrush associations. This map is returned
         by `pyminflux.ui.helpers.create_brushes_by()`.
 
+    color_scheme: Optional[str] = None
+        Pre-defined color scheme for the QBrush creation. The color scheme
+        presupposes a fixed number of unique identifiers (as for instance,
+        when the spots are labeled by fluorophore ID (either, 1 or 2).
+        Currently supported color schemes:
+
+        "blue-red": two-color scheme := [[ 0, 0, 255], [255, 0, 0]]
+        "green-magenta": two-color scheme := [[ 0, 255, 0], [255, 0, 255]]
+
     Returns
     -------
 
     brushes_for_ids: list[QBrush]
         List of brushes corresponding to the list of identifiers. Each identifier references
         a unique QBrush instance.
 
@@ -254,15 +331,17 @@
         Possibly updated map between unique identifier and corresponding QBrush.
     """
 
     # Check that all identifies are in the cache
     if not np.isin(np.unique(identifiers), np.array(list(id_to_brush.keys()))).all():
         # Recreate the brushes
         # @TODO: Just recreate the missing ones
-        brushes_for_ids, id_to_brush = create_brushes_by(identifiers)
+        brushes_for_ids, id_to_brush = create_brushes_by(
+            identifiers, color_scheme=color_scheme
+        )
     else:
         # Update the mapping from each identifier in the full array to its corresponding QBrush for fast lookup
         brushes_for_ids = [id_to_brush[identifier] for identifier in identifiers]
 
     # Return the list of brushes (and references)
     return brushes_for_ids, id_to_brush
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/histogram_plotter.py` & `pyminflux-0.4.1/pyminflux/ui/histogram_plotter.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,36 +81,36 @@
         self.hist_plot.setMenuEnabled(False)
         self.hist_plot.hideAxis("bottom")
         self.hist_plot.hideAxis("left")
         self.hist_plot.scene().sigMouseClicked.connect(self.raise_context_menu)
         self.ui.hlPlot.addWidget(self.hist_plot)
         self.hist_plot.show()
 
-    @Slot(int, name="persist_selected_param")
+    @Slot(int)
     def persist_selected_param(self, index):
         """Persist the selection for the parameter."""
 
         # Persist the selection
         self.selected_parameter = self.plotting_parameters[index]
 
     def keyPressEvent(self, ev):
         """Key press event."""
 
         # Do not capture key events for now
         ev.ignore()
 
-    @Slot(name="plot_histogram")
+    @Slot()
     def plot_histogram(self):
         """Plot the histogram of the selected parameter."""
 
         # Mark that there is no plot ready to export
         self.plot_ready_to_export = False
 
         # Get the data for the histogram
-        data = self.processor.filtered_dataframe[self.selected_parameter].values
+        data = self.processor.filtered_dataframe[self.selected_parameter].to_numpy()
 
         # Is there data?
         if len(data) == 0:
             self.clear_plot()
             return
 
         # Calculate the histogram
@@ -140,15 +140,15 @@
         # Show x and y grids
         self.hist_plot.showGrid(x=True, y=True)
 
         # Set properties of the label for y-axis
         self.hist_plot.setLabel("left", f"{param} frequencies")
 
         # Set properties of the label for x-axis
-        self.hist_plot.setLabel("bottom", f"{param} bins")
+        self.hist_plot.setLabel("bottom", f"{param}")
 
         # Make sure to have valid ranges and widths
         x_range = [bins[0], bins[-1]]
         if x_range[1] - x_range[0] == 0:
             x_range = [bins[0] - 0.1, bins[0] + 0.1]
             bin_width = 0.05
         else:
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/histogram_plotter.ui` & `pyminflux-0.4.1/pyminflux/ui/histogram_plotter.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/icons/icon.png` & `pyminflux-0.4.1/pyminflux/ui/icons/icon.png`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/importer.py` & `pyminflux-0.4.1/pyminflux/ui/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,35 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
+from typing import Sequence
+
 from PySide6.QtCore import Slot
 from PySide6.QtWidgets import QDialog
 
 from pyminflux.ui.ui_importer import Ui_Importer
 
 
 class Importer(QDialog, Ui_Importer):
     """
     A QDialog to support custom loading.
     """
 
-    def __init__(self, valid_cfr, relocalizations, dwell_time):
+    def __init__(
+        self,
+        valid_cfr: Sequence,
+        relocalizations: Sequence,
+        dwell_time: float,
+        is_tracking: bool,
+        pool_dcr: bool,
+    ):
         # Call the base class
         super().__init__()
 
         # Initialize the dialog
         self.ui = Ui_Importer()
         self.ui.setupUi(self)
 
@@ -35,24 +44,26 @@
         self._num_iterations = len(valid_cfr)
         self._last_valid_cfr = self.find_last_valid_cfr(valid_cfr)
         self._iteration = self._num_iterations - 1
         self._cfr_iteration = self._last_valid_cfr
         self._valid_cfr = valid_cfr
         self._relocalizations = relocalizations
         self._dwell_time = dwell_time
-
-        # Keep track of whether the dataset is a tracking dataset
-        self._is_tracking = False
+        self._is_tracking = is_tracking
+        self._pool_dcr = pool_dcr
 
         # Set the dwell time
         self.ui.leDwellTime.setText(f"{self._dwell_time}")
 
         # Set the tracking checkbox
         self.ui.cbTracking.setChecked(self._is_tracking)
 
+        # Set the pool DCR checkbox
+        self.ui.cbPoolDCR.setChecked(self._pool_dcr)
+
         # Characters
         self.valid_char = "✓"
         self.invalid_char = "⨯"
 
         # Organize the widgets to hide in lists
         self.widgets_list = [
             (self.ui.pbIter_0, self.ui.lbIter_0, self.ui.lbReloc_0),
@@ -84,15 +95,15 @@
 
         # Highlight global _iteration
         self.highlight_iteration(self._num_iterations - 1)
 
         # Highlight cfr index
         self.highlight_cfr(self._cfr_iteration)
 
-        # Highlight relocalize index
+        # Highlight relocalization index
         self.highlight_relocalization(self._cfr_iteration)
 
         # Adjust the size of the dialog
         self.adjustSize()
 
         # Set the connections
         self.set_connections()
@@ -103,32 +114,37 @@
             if valid_cfr[i]:
                 return i
         return None
 
     def set_connections(self):
         self.ui.leDwellTime.textChanged.connect(self.persist_dwell_time)
         self.ui.cbTracking.stateChanged.connect(self.persist_is_tracking)
+        self.ui.cbPoolDCR.stateChanged.connect(self.persist_pool_dcr)
         self.ui.pb_last_valid.clicked.connect(self.set_last_valid)
         for i in range(len(self.widgets_list)):
             self.widgets_list[i][0].setProperty("index", i)
             self.widgets_list[i][0].clicked.connect(self.set_all_iterations)
 
-    @Slot(str, name="persist_dwell_time")
+    @Slot(str)
     def persist_dwell_time(self, text):
         try:
             dwell_time = float(text)
         except ValueError as _:
             return
         self._dwell_time = dwell_time
 
-    @Slot(int, name="persist_is_tracking")
+    @Slot(int)
     def persist_is_tracking(self, state):
         self._is_tracking = state != 0
 
-    @Slot(name="set_last_valid")
+    @Slot(int)
+    def persist_pool_dcr(self, state):
+        self._pool_dcr = state != 0
+
+    @Slot()
     def set_last_valid(self):
         """Set the indices to correspond to the last valid index
         for the general iteration and the cfr iteration."""
 
         # Reset indices
         self._iteration = self._num_iterations - 1
         self._cfr_iteration = self._last_valid_cfr
@@ -141,15 +157,15 @@
 
         # Highlight cfr index
         self.highlight_cfr(self._cfr_iteration)
 
         # Highlight relocalized field
         self.highlight_relocalization(self._cfr_iteration)
 
-    @Slot(int, name="set_all_iterations")
+    @Slot(int)
     def set_all_iterations(self, checked):
 
         # Get the index of the button
         index = self.sender().property("index")
 
         # Update selections
         self._iteration = index
@@ -170,14 +186,15 @@
     def get_selection(self) -> dict:
         """Return the selected options."""
         return {
             "iteration": self._iteration,
             "cfr_iteration": self._cfr_iteration,
             "is_tracking": self._is_tracking,
             "dwell_time": self._dwell_time,
+            "pool_dcr": self._pool_dcr,
         }
 
     def hide_to(self, to_value: int):
         """Hide all buttons and labels."""
         for i in range(len(self.widgets_list) - 1, to_value - 1, -1):
             self.widgets_list[i][0].setVisible(False)
             self.widgets_list[i][1].setVisible(False)
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/importer.ui` & `pyminflux-0.4.1/pyminflux/ui/importer.ui`

 * *Files 3% similar despite different names*

#### Comparing `pyminflux-0.4.0/pyminflux/ui/importer.ui` & `pyminflux-0.4.1/pyminflux/ui/importer.ui`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
   <class>Importer</class>
   <widget class="QDialog" name="Importer">
     <property name="windowModality">
-      <enum>Qt::NonModal</enum>
+      <enum>Qt::WindowModality::NonModal</enum>
     </property>
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>417</width>
         <height>813</height>
@@ -28,101 +28,137 @@
     <property name="windowTitle">
       <string>Importer</string>
     </property>
     <property name="modal">
       <bool>true</bool>
     </property>
     <layout class="QGridLayout" name="gridLayout">
-      <item row="14" column="1">
-        <widget class="QLabel" name="lbIter_13">
+      <item row="21" column="0" colspan="3">
+        <widget class="QLabel" name="lbRelocInfo">
+          <property name="text">
+            <string>Non-relocalized iterations contain one valid measurement per trace.</string>
+          </property>
+        </widget>
+      </item>
+      <item row="9" column="0">
+        <widget class="QPushButton" name="pbIter_8">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
-            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
+            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
-          <property name="font">
-            <font>
-              <bold>true</bold>
-            </font>
+          <property name="text">
+            <string>Iteration 8</string>
+          </property>
+          <property name="checkable">
+            <bool>false</bool>
+          </property>
+        </widget>
+      </item>
+      <item row="4" column="0">
+        <widget class="QPushButton" name="pbIter_3">
+          <property name="enabled">
+            <bool>true</bool>
+          </property>
+          <property name="sizePolicy">
+            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+              <horstretch>0</horstretch>
+              <verstretch>0</verstretch>
+            </sizepolicy>
           </property>
           <property name="text">
-            <string>⨯</string>
+            <string>Iteration 3</string>
           </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
+          <property name="checkable">
+            <bool>false</bool>
           </property>
         </widget>
       </item>
-      <item row="1" column="2">
-        <widget class="QLabel" name="lbReloc_0">
+      <item row="11" column="0">
+        <widget class="QPushButton" name="pbIter_10">
+          <property name="enabled">
+            <bool>true</bool>
+          </property>
           <property name="sizePolicy">
-            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
+            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
+          <property name="text">
+            <string>Iteration 10</string>
+          </property>
+          <property name="checkable">
+            <bool>false</bool>
+          </property>
+        </widget>
+      </item>
+      <item row="0" column="2">
+        <widget class="QLabel" name="lbReloc">
           <property name="font">
             <font>
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
-            <string>⨯</string>
+            <string>Relocalized</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="16" column="2">
-        <widget class="QLabel" name="lbReloc_15">
+      <item row="12" column="2">
+        <widget class="QLabel" name="lbReloc_11">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
             <font>
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
-            <string>⨯</string>
+            <string>✓</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="8" column="0">
-        <widget class="QPushButton" name="pbIter_7">
-          <property name="enabled">
-            <bool>true</bool>
-          </property>
+      <item row="6" column="2">
+        <widget class="QLabel" name="lbReloc_5">
           <property name="sizePolicy">
-            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
+          <property name="font">
+            <font>
+              <bold>true</bold>
+            </font>
+          </property>
           <property name="text">
-            <string>Iteration 7</string>
+            <string>⨯</string>
           </property>
-          <property name="checkable">
-            <bool>false</bool>
+          <property name="alignment">
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="6" column="1">
-        <widget class="QLabel" name="lbIter_5">
+      <item row="1" column="1">
+        <widget class="QLabel" name="lbIter_0">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
@@ -133,51 +169,39 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-        </widget>
-      </item>
-      <item row="25" column="0">
-        <widget class="QCheckBox" name="cbTracking">
-          <property name="text">
-            <string>Tracking dataset</string>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="9" column="1">
-        <widget class="QLabel" name="lbIter_8">
+      <item row="1" column="0">
+        <widget class="QPushButton" name="pbIter_0">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
-            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
+            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
-          <property name="font">
-            <font>
-              <bold>true</bold>
-            </font>
-          </property>
           <property name="text">
-            <string>⨯</string>
+            <string>Iteration 0</string>
           </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
+          <property name="checkable">
+            <bool>false</bool>
           </property>
         </widget>
       </item>
-      <item row="7" column="2">
-        <widget class="QLabel" name="lbReloc_6">
+      <item row="16" column="2">
+        <widget class="QLabel" name="lbReloc_15">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -185,68 +209,54 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="0" column="1">
-        <widget class="QLabel" name="lbCFRValues">
+      <item row="0" column="0">
+        <widget class="QLabel" name="lbIteration">
           <property name="font">
             <font>
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
-            <string>CFR values</string>
+            <string>Iteration number</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="21" column="0" colspan="3">
-        <widget class="QLabel" name="lbRelocInfo">
-          <property name="text">
-            <string>Non-relocalized iterations contain one valid measurement per trace.</string>
-          </property>
-        </widget>
-      </item>
-      <item row="24" column="0" colspan="3">
-        <widget class="Line" name="line">
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-        </widget>
-      </item>
-      <item row="9" column="0">
-        <widget class="QPushButton" name="pbIter_8">
+      <item row="16" column="0">
+        <widget class="QPushButton" name="pbIter_15">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="text">
-            <string>Iteration 8</string>
+            <string>Iteration 15</string>
           </property>
           <property name="checkable">
             <bool>false</bool>
           </property>
         </widget>
       </item>
-      <item row="4" column="2">
-        <widget class="QLabel" name="lbReloc_3">
+      <item row="14" column="2">
+        <widget class="QLabel" name="lbReloc_13">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -254,23 +264,20 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="15" column="1">
-        <widget class="QLabel" name="lbIter_14">
-          <property name="enabled">
-            <bool>true</bool>
-          </property>
+      <item row="9" column="2">
+        <widget class="QLabel" name="lbReloc_8">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -278,20 +285,20 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="1" column="1">
-        <widget class="QLabel" name="lbIter_0">
+      <item row="5" column="1">
+        <widget class="QLabel" name="lbIter_4">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
@@ -302,108 +309,110 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="11" column="1">
-        <widget class="QLabel" name="lbIter_10">
+      <item row="18" column="0" colspan="3">
+        <widget class="Line" name="line_2">
+          <property name="orientation">
+            <enum>Qt::Orientation::Horizontal</enum>
+          </property>
+        </widget>
+      </item>
+      <item row="7" column="0">
+        <widget class="QPushButton" name="pbIter_6">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
+            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+              <horstretch>0</horstretch>
+              <verstretch>0</verstretch>
+            </sizepolicy>
+          </property>
+          <property name="text">
+            <string>Iteration 6</string>
+          </property>
+          <property name="checkable">
+            <bool>false</bool>
+          </property>
+        </widget>
+      </item>
+      <item row="10" column="2">
+        <widget class="QLabel" name="lbReloc_9">
+          <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
             <font>
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="7" column="0">
-        <widget class="QPushButton" name="pbIter_6">
+      <item row="15" column="0">
+        <widget class="QPushButton" name="pbIter_14">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="text">
-            <string>Iteration 6</string>
+            <string>Iteration 14</string>
           </property>
           <property name="checkable">
             <bool>false</bool>
           </property>
         </widget>
       </item>
-      <item row="28" column="0" colspan="3">
-        <widget class="QDialogButtonBox" name="buttonBox">
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
-          </property>
-          <property name="standardButtons">
-            <set>QDialogButtonBox::Cancel|QDialogButtonBox::Ok</set>
-          </property>
-        </widget>
-      </item>
-      <item row="27" column="0">
-        <spacer name="verticalSpacer">
-          <property name="orientation">
-            <enum>Qt::Vertical</enum>
-          </property>
-          <property name="sizeHint" stdset="0">
-            <size>
-              <width>20</width>
-              <height>40</height>
-            </size>
+      <item row="9" column="1">
+        <widget class="QLabel" name="lbIter_8">
+          <property name="enabled">
+            <bool>true</bool>
           </property>
-        </spacer>
-      </item>
-      <item row="18" column="0" colspan="3">
-        <widget class="Line" name="line_2">
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
+          <property name="sizePolicy">
+            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
+              <horstretch>0</horstretch>
+              <verstretch>0</verstretch>
+            </sizepolicy>
           </property>
-        </widget>
-      </item>
-      <item row="0" column="0">
-        <widget class="QLabel" name="lbIteration">
           <property name="font">
             <font>
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
-            <string>Iteration number</string>
+            <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="3" column="2">
-        <widget class="QLabel" name="lbReloc_2">
+      <item row="5" column="2">
+        <widget class="QLabel" name="lbReloc_4">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -411,51 +420,60 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="4" column="1">
-        <widget class="QLabel" name="lbIter_3">
+      <item row="10" column="0">
+        <widget class="QPushButton" name="pbIter_9">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
+            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+              <horstretch>0</horstretch>
+              <verstretch>0</verstretch>
+            </sizepolicy>
+          </property>
+          <property name="text">
+            <string>Iteration 9</string>
+          </property>
+          <property name="checkable">
+            <bool>false</bool>
+          </property>
+        </widget>
+      </item>
+      <item row="7" column="2">
+        <widget class="QLabel" name="lbReloc_6">
+          <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
             <font>
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-        </widget>
-      </item>
-      <item row="20" column="0" colspan="3">
-        <widget class="QLabel" name="lbLastValidInfo">
-          <property name="text">
-            <string>Only &quot;last valid&quot; iteration can be saved.</string>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="5" column="2">
-        <widget class="QLabel" name="lbReloc_4">
+      <item row="4" column="2">
+        <widget class="QLabel" name="lbReloc_3">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -463,23 +481,20 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="13" column="1">
-        <widget class="QLabel" name="lbIter_12">
-          <property name="enabled">
-            <bool>true</bool>
-          </property>
+      <item row="13" column="2">
+        <widget class="QLabel" name="lbReloc_12">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -487,39 +502,65 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="1" column="0">
-        <widget class="QPushButton" name="pbIter_0">
+      <item row="27" column="0">
+        <widget class="QLabel" name="lbDwellTime">
+          <property name="sizePolicy">
+            <sizepolicy hsizetype="MinimumExpanding" vsizetype="Fixed">
+              <horstretch>0</horstretch>
+              <verstretch>0</verstretch>
+            </sizepolicy>
+          </property>
+          <property name="text">
+            <string>Dwell time (ms)</string>
+          </property>
+        </widget>
+      </item>
+      <item row="29" column="0" colspan="3">
+        <widget class="QDialogButtonBox" name="buttonBox">
+          <property name="orientation">
+            <enum>Qt::Orientation::Horizontal</enum>
+          </property>
+          <property name="standardButtons">
+            <set>QDialogButtonBox::StandardButton::Cancel|QDialogButtonBox::StandardButton::Ok</set>
+          </property>
+        </widget>
+      </item>
+      <item row="14" column="0">
+        <widget class="QPushButton" name="pbIter_13">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="text">
-            <string>Iteration 0</string>
+            <string>Iteration 13</string>
           </property>
           <property name="checkable">
             <bool>false</bool>
           </property>
         </widget>
       </item>
-      <item row="9" column="2">
-        <widget class="QLabel" name="lbReloc_8">
+      <item row="3" column="1">
+        <widget class="QLabel" name="lbIter_2">
+          <property name="enabled">
+            <bool>true</bool>
+          </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -527,119 +568,80 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="15" column="0">
-        <widget class="QPushButton" name="pbIter_14">
+      <item row="3" column="0">
+        <widget class="QPushButton" name="pbIter_2">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="text">
-            <string>Iteration 14</string>
+            <string>Iteration 2</string>
           </property>
           <property name="checkable">
             <bool>false</bool>
           </property>
         </widget>
       </item>
-      <item row="3" column="0">
-        <widget class="QPushButton" name="pbIter_2">
+      <item row="5" column="0">
+        <widget class="QPushButton" name="pbIter_4">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="text">
-            <string>Iteration 2</string>
+            <string>Iteration 4</string>
           </property>
           <property name="checkable">
             <bool>false</bool>
           </property>
         </widget>
       </item>
-      <item row="15" column="2">
-        <widget class="QLabel" name="lbReloc_14">
-          <property name="sizePolicy">
-            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
-              <horstretch>0</horstretch>
-              <verstretch>0</verstretch>
-            </sizepolicy>
-          </property>
-          <property name="font">
-            <font>
-              <bold>true</bold>
-            </font>
-          </property>
-          <property name="text">
-            <string>⨯</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-        </widget>
-      </item>
-      <item row="14" column="0">
-        <widget class="QPushButton" name="pbIter_13">
+      <item row="2" column="0">
+        <widget class="QPushButton" name="pbIter_1">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="text">
-            <string>Iteration 13</string>
+            <string>Iteration 1</string>
           </property>
           <property name="checkable">
             <bool>false</bool>
           </property>
         </widget>
       </item>
-      <item row="2" column="2">
-        <widget class="QLabel" name="lbReloc_1">
-          <property name="sizePolicy">
-            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
-              <horstretch>0</horstretch>
-              <verstretch>0</verstretch>
-            </sizepolicy>
-          </property>
-          <property name="font">
-            <font>
-              <bold>true</bold>
-            </font>
-          </property>
-          <property name="text">
-            <string>⨯</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
+      <item row="6" column="1">
+        <widget class="QLabel" name="lbIter_5">
+          <property name="enabled">
+            <bool>true</bool>
           </property>
-        </widget>
-      </item>
-      <item row="10" column="2">
-        <widget class="QLabel" name="lbReloc_9">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -647,39 +649,39 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="12" column="0">
-        <widget class="QPushButton" name="pbIter_11">
+      <item row="8" column="0">
+        <widget class="QPushButton" name="pbIter_7">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="text">
-            <string>Iteration 11</string>
+            <string>Iteration 7</string>
           </property>
           <property name="checkable">
             <bool>false</bool>
           </property>
         </widget>
       </item>
-      <item row="16" column="1">
-        <widget class="QLabel" name="lbIter_15">
+      <item row="11" column="1">
+        <widget class="QLabel" name="lbIter_10">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
@@ -690,39 +692,20 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-        </widget>
-      </item>
-      <item row="11" column="0">
-        <widget class="QPushButton" name="pbIter_10">
-          <property name="enabled">
-            <bool>true</bool>
-          </property>
-          <property name="sizePolicy">
-            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
-              <horstretch>0</horstretch>
-              <verstretch>0</verstretch>
-            </sizepolicy>
-          </property>
-          <property name="text">
-            <string>Iteration 10</string>
-          </property>
-          <property name="checkable">
-            <bool>false</bool>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="12" column="1">
-        <widget class="QLabel" name="lbIter_11">
+      <item row="7" column="1">
+        <widget class="QLabel" name="lbIter_6">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
@@ -730,55 +713,61 @@
           </property>
           <property name="font">
             <font>
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
-            <string>✓</string>
+            <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="26" column="1" colspan="2">
-        <widget class="QLineEdit" name="leDwellTime">
+      <item row="6" column="0">
+        <widget class="QPushButton" name="pbIter_5">
+          <property name="enabled">
+            <bool>true</bool>
+          </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
+          <property name="text">
+            <string>Iteration 5</string>
+          </property>
+          <property name="checkable">
+            <bool>false</bool>
+          </property>
         </widget>
       </item>
-      <item row="4" column="0">
-        <widget class="QPushButton" name="pbIter_3">
+      <item row="13" column="0">
+        <widget class="QPushButton" name="pbIter_12">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="text">
-            <string>Iteration 3</string>
+            <string>Iteration 12</string>
           </property>
           <property name="checkable">
             <bool>false</bool>
           </property>
         </widget>
       </item>
-      <item row="5" column="1">
-        <widget class="QLabel" name="lbIter_4">
-          <property name="enabled">
-            <bool>true</bool>
-          </property>
+      <item row="1" column="2">
+        <widget class="QLabel" name="lbReloc_0">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -786,76 +775,65 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="5" column="0">
-        <widget class="QPushButton" name="pbIter_4">
-          <property name="enabled">
-            <bool>true</bool>
-          </property>
+      <item row="11" column="2">
+        <widget class="QLabel" name="lbReloc_10">
           <property name="sizePolicy">
-            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
-          <property name="text">
-            <string>Iteration 4</string>
-          </property>
-          <property name="checkable">
-            <bool>false</bool>
-          </property>
-        </widget>
-      </item>
-      <item row="0" column="2">
-        <widget class="QLabel" name="lbReloc">
           <property name="font">
             <font>
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
-            <string>Relocalized</string>
+            <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="13" column="0">
-        <widget class="QPushButton" name="pbIter_12">
+      <item row="15" column="1">
+        <widget class="QLabel" name="lbIter_14">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
-            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
+          <property name="font">
+            <font>
+              <bold>true</bold>
+            </font>
+          </property>
           <property name="text">
-            <string>Iteration 12</string>
+            <string>⨯</string>
           </property>
-          <property name="checkable">
-            <bool>false</bool>
+          <property name="alignment">
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="7" column="1">
-        <widget class="QLabel" name="lbIter_6">
-          <property name="enabled">
-            <bool>true</bool>
-          </property>
+      <item row="15" column="2">
+        <widget class="QLabel" name="lbReloc_14">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -863,58 +841,67 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="6" column="0">
-        <widget class="QPushButton" name="pbIter_5">
-          <property name="enabled">
-            <bool>true</bool>
-          </property>
+      <item row="2" column="2">
+        <widget class="QLabel" name="lbReloc_1">
           <property name="sizePolicy">
-            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
+          <property name="font">
+            <font>
+              <bold>true</bold>
+            </font>
+          </property>
           <property name="text">
-            <string>Iteration 5</string>
+            <string>⨯</string>
           </property>
-          <property name="checkable">
-            <bool>false</bool>
+          <property name="alignment">
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="16" column="0">
-        <widget class="QPushButton" name="pbIter_15">
-          <property name="enabled">
-            <bool>true</bool>
+      <item row="17" column="0">
+        <spacer name="verticalSpacer_2">
+          <property name="orientation">
+            <enum>Qt::Orientation::Vertical</enum>
           </property>
-          <property name="sizePolicy">
-            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
-              <horstretch>0</horstretch>
-              <verstretch>0</verstretch>
-            </sizepolicy>
+          <property name="sizeHint" stdset="0">
+            <size>
+              <width>20</width>
+              <height>20</height>
+            </size>
           </property>
-          <property name="text">
-            <string>Iteration 15</string>
+        </spacer>
+      </item>
+      <item row="28" column="0">
+        <spacer name="verticalSpacer">
+          <property name="orientation">
+            <enum>Qt::Orientation::Vertical</enum>
           </property>
-          <property name="checkable">
-            <bool>false</bool>
+          <property name="sizeHint" stdset="0">
+            <size>
+              <width>20</width>
+              <height>40</height>
+            </size>
           </property>
-        </widget>
+        </spacer>
       </item>
-      <item row="2" column="1">
-        <widget class="QLabel" name="lbIter_1">
+      <item row="10" column="1">
+        <widget class="QLabel" name="lbIter_9">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
@@ -925,30 +912,27 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="19" column="0" colspan="3">
-        <widget class="QPushButton" name="pb_last_valid">
-          <property name="text">
-            <string>Pick last valid iteration</string>
-          </property>
-          <property name="checkable">
-            <bool>false</bool>
+      <item row="24" column="0" colspan="3">
+        <widget class="Line" name="line">
+          <property name="orientation">
+            <enum>Qt::Orientation::Horizontal</enum>
           </property>
         </widget>
       </item>
-      <item row="10" column="1">
-        <widget class="QLabel" name="lbIter_9">
+      <item row="13" column="1">
+        <widget class="QLabel" name="lbIter_12">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
@@ -959,39 +943,41 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="2" column="0">
-        <widget class="QPushButton" name="pbIter_1">
-          <property name="enabled">
-            <bool>true</bool>
-          </property>
+      <item row="3" column="2">
+        <widget class="QLabel" name="lbReloc_2">
           <property name="sizePolicy">
-            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
+          <property name="font">
+            <font>
+              <bold>true</bold>
+            </font>
+          </property>
           <property name="text">
-            <string>Iteration 1</string>
+            <string>⨯</string>
           </property>
-          <property name="checkable">
-            <bool>false</bool>
+          <property name="alignment">
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="14" column="2">
-        <widget class="QLabel" name="lbReloc_13">
+      <item row="8" column="2">
+        <widget class="QLabel" name="lbReloc_7">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -999,73 +985,73 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="10" column="0">
-        <widget class="QPushButton" name="pbIter_9">
+      <item row="2" column="1">
+        <widget class="QLabel" name="lbIter_1">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
-            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
+          <property name="font">
+            <font>
+              <bold>true</bold>
+            </font>
+          </property>
           <property name="text">
-            <string>Iteration 9</string>
+            <string>⨯</string>
           </property>
-          <property name="checkable">
-            <bool>false</bool>
+          <property name="alignment">
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="26" column="0">
-        <widget class="QLabel" name="lbDwellTime">
-          <property name="sizePolicy">
-            <sizepolicy hsizetype="MinimumExpanding" vsizetype="Fixed">
-              <horstretch>0</horstretch>
-              <verstretch>0</verstretch>
-            </sizepolicy>
-          </property>
+      <item row="20" column="0" colspan="3">
+        <widget class="QLabel" name="lbLastValidInfo">
           <property name="text">
-            <string>Dwell time (ms)</string>
+            <string>Only &quot;last valid&quot; iteration can be saved.</string>
           </property>
         </widget>
       </item>
-      <item row="13" column="2">
-        <widget class="QLabel" name="lbReloc_12">
-          <property name="sizePolicy">
-            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
-              <horstretch>0</horstretch>
-              <verstretch>0</verstretch>
-            </sizepolicy>
-          </property>
+      <item row="0" column="1">
+        <widget class="QLabel" name="lbCFRValues">
           <property name="font">
             <font>
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
-            <string>⨯</string>
+            <string>CFR values</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="8" column="1">
-        <widget class="QLabel" name="lbIter_7">
+      <item row="25" column="0">
+        <widget class="QCheckBox" name="cbTracking">
+          <property name="text">
+            <string>Tracking dataset</string>
+          </property>
+        </widget>
+      </item>
+      <item row="16" column="1">
+        <widget class="QLabel" name="lbIter_15">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
@@ -1076,20 +1062,23 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="6" column="2">
-        <widget class="QLabel" name="lbReloc_5">
+      <item row="4" column="1">
+        <widget class="QLabel" name="lbIter_3">
+          <property name="enabled">
+            <bool>true</bool>
+          </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -1097,20 +1086,23 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="12" column="2">
-        <widget class="QLabel" name="lbReloc_11">
+      <item row="12" column="1">
+        <widget class="QLabel" name="lbIter_11">
+          <property name="enabled">
+            <bool>true</bool>
+          </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -1118,20 +1110,23 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>✓</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="8" column="2">
-        <widget class="QLabel" name="lbReloc_7">
+      <item row="8" column="1">
+        <widget class="QLabel" name="lbIter_7">
+          <property name="enabled">
+            <bool>true</bool>
+          </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="font">
@@ -1139,20 +1134,30 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
           </property>
         </widget>
       </item>
-      <item row="3" column="1">
-        <widget class="QLabel" name="lbIter_2">
+      <item row="19" column="0" colspan="3">
+        <widget class="QPushButton" name="pb_last_valid">
+          <property name="text">
+            <string>Pick last valid iteration</string>
+          </property>
+          <property name="checkable">
+            <bool>false</bool>
+          </property>
+        </widget>
+      </item>
+      <item row="14" column="1">
+        <widget class="QLabel" name="lbIter_13">
           <property name="enabled">
             <bool>true</bool>
           </property>
           <property name="sizePolicy">
             <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
@@ -1163,67 +1168,69 @@
               <bold>true</bold>
             </font>
           </property>
           <property name="text">
             <string>⨯</string>
           </property>
           <property name="alignment">
-            <set>Qt::AlignCenter</set>
+            <set>Qt::AlignmentFlag::AlignCenter</set>
+          </property>
+        </widget>
+      </item>
+      <item row="27" column="1" colspan="2">
+        <widget class="QLineEdit" name="leDwellTime">
+          <property name="sizePolicy">
+            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+              <horstretch>0</horstretch>
+              <verstretch>0</verstretch>
+            </sizepolicy>
           </property>
         </widget>
       </item>
       <item row="22" column="0">
         <spacer name="fixedVerticalSpacer">
           <property name="orientation">
-            <enum>Qt::Vertical</enum>
+            <enum>Qt::Orientation::Vertical</enum>
           </property>
           <property name="sizeType">
-            <enum>QSizePolicy::Fixed</enum>
+            <enum>QSizePolicy::Policy::Fixed</enum>
           </property>
           <property name="sizeHint" stdset="0">
             <size>
               <width>20</width>
               <height>20</height>
             </size>
           </property>
         </spacer>
       </item>
-      <item row="11" column="2">
-        <widget class="QLabel" name="lbReloc_10">
+      <item row="12" column="0">
+        <widget class="QPushButton" name="pbIter_11">
+          <property name="enabled">
+            <bool>true</bool>
+          </property>
           <property name="sizePolicy">
-            <sizepolicy hsizetype="Preferred" vsizetype="Fixed">
+            <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
-          <property name="font">
-            <font>
-              <bold>true</bold>
-            </font>
-          </property>
           <property name="text">
-            <string>⨯</string>
+            <string>Iteration 11</string>
           </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
+          <property name="checkable">
+            <bool>false</bool>
           </property>
         </widget>
       </item>
-      <item row="17" column="0">
-        <spacer name="verticalSpacer_2">
-          <property name="orientation">
-            <enum>Qt::Vertical</enum>
-          </property>
-          <property name="sizeHint" stdset="0">
-            <size>
-              <width>20</width>
-              <height>20</height>
-            </size>
+      <item row="26" column="0" colspan="3">
+        <widget class="QCheckBox" name="cbPoolDCR">
+          <property name="text">
+            <string>Pool DCR values (ECO-weighted)</string>
           </property>
-        </spacer>
+        </widget>
       </item>
     </layout>
   </widget>
   <resources/>
   <connections>
     <connection>
       <sender>buttonBox</sender>
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/main_window.py` & `pyminflux-0.4.1/pyminflux/ui/main_window.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
-
 import sys
 from datetime import datetime
 from pathlib import Path
+from typing import Optional
 
 from pyqtgraph import ViewBox
 from PySide6 import QtGui
 from PySide6.QtCore import Qt, Signal, Slot
 from PySide6.QtGui import QDesktopServices, QIcon
 from PySide6.QtWidgets import (
     QDialog,
@@ -33,23 +33,24 @@
     QVBoxLayout,
 )
 
 import pyminflux.resources
 from pyminflux import __APP_NAME__, __version__
 from pyminflux.processor import MinFluxProcessor
 from pyminflux.reader import MinFluxReader, NativeMetadataReader
-from pyminflux.settings import Settings
+from pyminflux.settings import Settings, UpdateSettings
 from pyminflux.state import State
+from pyminflux.threads import AutoUpdateCheckerWorker
 from pyminflux.ui.analyzer import Analyzer
 from pyminflux.ui.color_unmixer import ColorUnmixer
 from pyminflux.ui.dataviewer import DataViewer
-from pyminflux.ui.emittingstream import EmittingStream
 from pyminflux.ui.frc_tool import FRCTool
 from pyminflux.ui.histogram_plotter import HistogramPlotter
 from pyminflux.ui.importer import Importer
+from pyminflux.ui.mediator import Mediator
 from pyminflux.ui.options import Options
 from pyminflux.ui.plotter import Plotter
 from pyminflux.ui.plotter_toolbar import PlotterToolbar
 from pyminflux.ui.time_inspector import TimeInspector
 from pyminflux.ui.trace_stats_viewer import TraceStatsViewer
 from pyminflux.ui.ui_main_window import Ui_MainWindow
 from pyminflux.ui.wizard import WizardDialog
@@ -58,15 +59,15 @@
 
 
 class PyMinFluxMainWindow(QMainWindow, Ui_MainWindow):
     """
     Main application window.
     """
 
-    request_sync_external_tools = Signal(None, name="request_sync_external_tools")
+    request_sync_external_tools = Signal()
 
     def __init__(self, parent=None):
         """
         Constructor.
         """
 
         # Call the base constructor
@@ -82,111 +83,112 @@
         # Set the window icon
         icon = QIcon(":/icons/icon.png")
         self.setWindowIcon(icon)
 
         # Keep a reference to the state machine
         self.state = State()
 
-        # Keep track of the last selected path
-        self.last_selected_path = ""
+        # Keep a reference to the AutoUpdateCheckWorker
+        self.update_worker = None
+
+        # Interval in seconds since last check for updates
+        self._check_interval_in_seconds = 60 * 60 * 24 * 7
 
         # Keep a reference to the MinFluxProcessor
         self.processor = None
 
         # Read the application settings and update the state
         self.load_and_apply_settings()
 
         # Set the menu state based on the settings
         self.ui.actionConsole.setChecked(self.state.open_console_at_start)
 
+        # Initialize Mediator
+        self.mediator = Mediator()
+        self.mediator.register_dialog("main_window", self)
+
         # Dialogs and widgets
         self.data_viewer = None
         self.analyzer = None
         self.plotter = None
         self.histogram_plotter = None
         self.color_unmixer = None
         self.time_inspector = None
         self.trace_stats_viewer = None
-        self.trace_length_viewer = None
         self.frc_tool = None
         self.options = Options()
+        self.mediator.register_dialog("options", self.options)
 
         # Initialize widget and its dock
         self.wizard = WizardDialog()
         self.wizard_dock = QDockWidget("", self)
         self.wizard_dock.setAllowedAreas(Qt.LeftDockWidgetArea | Qt.RightDockWidgetArea)
         self.wizard_dock.setFeatures(
             QDockWidget.DockWidgetMovable | QDockWidget.DockWidgetFloatable
         )
         self.wizard_dock.setWidget(self.wizard)
         self.addDockWidget(Qt.LeftDockWidgetArea, self.wizard_dock)
+        self.mediator.register_dialog("wizard", self.wizard)
 
         # Initialize Plotter and DataViewer
         self.plotter = Plotter()
+        self.mediator.register_dialog("plotter", self.plotter)
         self.plotter_toolbar = PlotterToolbar()
+        self.mediator.register_dialog("plotter_toolbar", self.plotter_toolbar)
         self.data_viewer = DataViewer()
+        self.mediator.register_dialog("data_viewer", self.data_viewer)
 
         # Create the output console
-        self.txConsole = QTextEdit()
-        self.txConsole.setReadOnly(True)
-        self.txConsole.setMinimumHeight(100)
-        self.txConsole.setMaximumHeight(500)
-        self.txConsole.setLineWrapMode(QTextEdit.NoWrap)
-        self.txConsole.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOn)
+        self.txt_console = QTextEdit()
+        self.txt_console.setReadOnly(True)
+        self.txt_console.setMinimumHeight(100)
+        self.txt_console.setMaximumHeight(500)
+        self.txt_console.setLineWrapMode(QTextEdit.NoWrap)
+        self.txt_console.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOn)
+        self.mediator.register_dialog("txt_console", self.txt_console)
 
         # Add them to the splitter
         self.ui.splitter_layout.addWidget(self.plotter)
         self.ui.splitter_layout.addWidget(self.plotter_toolbar)
         self.ui.splitter_layout.addWidget(self.data_viewer)
-        self.ui.splitter_layout.addWidget(self.txConsole)
+        self.ui.splitter_layout.addWidget(self.txt_console)
 
         # Make sure to only show the console if requested
         self.toggle_console_visibility()
 
         # Set initial visibility and enabled states
         self.enable_ui_components(False)
 
         # Set up signals and slots
-        self.setup_conn()
-
-        # Install the custom output stream
-        sys.stdout = EmittingStream()
-        sys.stdout.signal_textWritten.connect(self.print_to_console)
+        self.setup_actions_conn()
 
         # Print a welcome message to the console
         print(f"Welcome to {__APP_NAME__} v{__version__}.")
 
+        # Check for updates
+        self.auto_check_remote_for_updates()
+
     def load_and_apply_settings(self):
         """Read the application settings and update the State."""
 
         # Open settings file
         settings = Settings()
 
-        # Read and set 'last_selected_path' option
-        self.last_selected_path = Path(
+        # Read and set "last_selected_path" option
+        self.state.last_selected_path = Path(
             settings.instance.value("io/last_selected_path", ".")
         )
 
         # Read and set 'min_trace_length' option
         self.state.min_trace_length = int(
             settings.instance.value(
                 "options/min_trace_length", self.state.min_trace_length
             )
         )
 
-        # @SUPERSEDED: Read 'min_trace_length' and set as 'min_trace_length'
-        # This property will be removed from the file the next time the user hits
-        # the "Set as new default" in the Options dialog.
-        if settings.instance.contains("options/min_trace_length"):
-            self.state.min_trace_length = int(
-                settings.instance.value(
-                    "options/min_trace_length", self.state.min_trace_length
-                )
-            )
-
         # Current option name: "options/min_trace_length"
         if settings.instance.contains("options/min_trace_length"):
             self.state.min_trace_length = int(
                 settings.instance.value(
                     "options/min_trace_length", self.state.min_trace_length
                 )
             )
@@ -262,15 +264,15 @@
             self.state.open_console_at_start,
         )
         open_console_at_start = (
             value.lower() == "true" if isinstance(value, str) else bool(value)
         )
         self.state.open_console_at_start = open_console_at_start
 
-    def setup_conn(self):
+    def setup_actions_conn(self):
         """Set up signals and slots."""
 
         # Menu actions
         self.ui.actionLoad.triggered.connect(self.select_and_load_or_import_data_file)
         self.ui.actionSave.triggered.connect(self.save_native_file)
         self.ui.actionExport_data.triggered.connect(self.export_filtered_data)
         self.ui.actionExport_stats.triggered.connect(self.export_filtered_stats)
@@ -310,63 +312,23 @@
             lambda _: QDesktopServices.openUrl(
                 "https://github.com/bsse-scf/pyMINFLUX/blob/master/CHANGELOG.md"
             )
         )
         self.ui.actionCheck_for_updates.triggered.connect(self.check_remote_for_updates)
         self.ui.actionAbout.triggered.connect(self.about)
 
-        # Plotter toolbar
-        self.plotter_toolbar.plot_requested_parameters.connect(
-            self.plot_selected_parameters
-        )
-        self.plotter_toolbar.plot_average_positions_state_changed.connect(
-            self.full_update_ui
-        )
-
-        # Plotter
-        self.plotter.locations_selected.connect(
-            self.show_selected_points_by_indices_in_dataviewer
-        )
-        self.plotter.locations_selected_by_range.connect(
-            self.show_selected_points_by_range_in_dataviewer
-        )
-        self.plotter.crop_region_selected.connect(self.crop_data_by_range)
-        self.plotter_toolbar.color_code_locs_changed.connect(
-            self.plot_selected_parameters
-        )
+    def enable_ui_components(self, enabled: bool):
+        """Enable/disable UI components."""
 
-        # Options
-        self.options.weigh_avg_localization_by_eco_option_changed.connect(
-            self.update_weighted_average_localization_option_and_plot
-        )
-        self.options.min_trace_length_option_changed.connect(
-            self.update_min_trace_length
-        )
+        if self.plotter is None:
+            raise Exception("Plotter object not ready!")
 
-        # Wizard
-        self.wizard.load_data_triggered.connect(
-            self.select_and_load_or_import_data_file
-        )
-        self.wizard.reset_filters_triggered.connect(self.reset_filters_and_broadcast)
-        self.wizard.open_unmixer_triggered.connect(self.open_color_unmixer)
-        self.wizard.open_time_inspector_triggered.connect(self.open_time_inspector)
-        self.wizard.open_analyzer_triggered.connect(self.open_analyzer)
-        self.wizard.fluorophore_id_changed.connect(
-            self.update_fluorophore_id_in_processor_and_broadcast
-        )
-        self.wizard.request_fluorophore_ids_reset.connect(self.reset_fluorophore_ids)
-        self.wizard.wizard_filters_run.connect(self.full_update_ui)
-        self.wizard.save_data_triggered.connect(self.save_native_file)
-        self.wizard.export_data_triggered.connect(self.export_filtered_data)
-        self.wizard.load_filename_triggered.connect(
-            self.select_and_load_or_import_data_file
-        )
+        if self.data_viewer is None:
+            raise Exception("DataViewer object not ready!")
 
-    def enable_ui_components(self, enabled: bool):
-        """Enable/disable UI components."""
         self.plotter.show()  # Always show
         if enabled:
             self.plotter_toolbar.show()
             self.data_viewer.show()
             self.plotter_toolbar.show()
         else:
             self.plotter_toolbar.hide()
@@ -383,28 +345,35 @@
         self.ui.actionFRC_analyzer.setEnabled(enabled)
 
     def full_update_ui(self):
         """
         Updates the UI completely (after a project load, for instance).
         :return:
         """
+
+        if self.plotter is None:
+            raise Exception("Plotter object not ready!")
+
+        if self.data_viewer is None:
+            raise Exception("DataViewer object not ready!")
+
         self.plotter.clear()
         self.plot_selected_parameters()
         self.data_viewer.clear()
         if self.processor is not None and self.processor.filtered_dataframe is not None:
             print(f"Retrieved {len(self.processor.filtered_dataframe.index)} events.")
 
     def print_to_console(self, text):
         """
         Append text to the QTextEdit.
         """
-        cursor = self.txConsole.textCursor()
+        cursor = self.txt_console.textCursor()
         cursor.movePosition(QtGui.QTextCursor.MoveOperation.End)
         cursor.insertText(text)
-        self.txConsole.setTextCursor(cursor)
+        self.txt_console.setTextCursor(cursor)
 
     def closeEvent(self, event):
         """Application close event."""
 
         # Ask the user
         button = QMessageBox.question(
             self,
@@ -416,109 +385,121 @@
 
         if button != QMessageBox.StandardButton.Yes:
             event.ignore()
         else:
             # @TODO Shutdown threads if any are running
 
             if self.options is not None:
+                self.mediator.unregister_dialog("options")
                 self.options.close()
                 self.options = None
 
             if self.histogram_plotter is not None:
+                self.mediator.unregister_dialog("histogram_plotter")
                 self.histogram_plotter.close()
                 self.histogram_plotter = None
 
             if self.analyzer is not None:
+                self.mediator.unregister_dialog("analyzer")
                 self.analyzer.close()
                 self.analyzer = None
 
             if self.color_unmixer is not None:
+                self.mediator.unregister_dialog("color_unmixer")
                 self.color_unmixer.close()
                 self.color_unmixer = None
 
             if self.time_inspector is not None:
+                self.mediator.unregister_dialog("time_inspector")
                 self.time_inspector.close()
                 self.time_inspector = None
 
             if self.options is not None:
+                self.mediator.unregister_dialog("options")
                 self.options.close()
                 self.options = None
 
             if self.trace_stats_viewer is not None:
+                self.mediator.unregister_dialog("trace_stats_viewer")
                 self.trace_stats_viewer.close()
                 self.trace_stats_viewer = None
 
-            if self.trace_length_viewer is not None:
-                self.trace_length_viewer.close()
-                self.trace_length_viewer = None
-
             if self.frc_tool is not None:
+                self.mediator.unregister_dialog("frc_tool")
                 self.frc_tool.close()
                 self.frc_tool = None
 
             # Store the application settings
-            if self.last_selected_path != "":
+            if self.state.last_selected_path is not None:
                 settings = Settings()
                 settings.instance.setValue(
-                    "io/last_selected_path", str(self.last_selected_path)
+                    "io/last_selected_path", str(self.state.last_selected_path)
                 )
 
-            # # Restore sys.stdout
-            # sys.stdout = sys.__stdout__
-            # sys.stdout.flush()
+            # Unregister the text console and the Main Window
+            self.mediator.unregister_dialog("txt_console")
+            self.mediator.unregister_dialog("main_window")
 
             # Now exit
             event.accept()
 
-    @Slot(None, name="reset_filters_and_broadcast")
+    @Slot()
     def reset_filters_and_broadcast(self):
         """Reset all filters and broadcast changes."""
 
+        if self.processor is None:
+            return
+
         # Reset filters and data
         self.processor.reset()
         self.state.efo_thresholds = None
         self.state.cfr_thresholds = None
 
         # Update main window
         self.full_update_ui()
 
         # Signal that the external viewers and tools should be updated
         self.request_sync_external_tools.emit()
 
-    @Slot(None, name="quit_application")
+    @Slot()
     def quit_application(self):
         """Quit the application."""
         self.close()
 
-    @Slot(bool, name="toggle_console_visibility")
+    @Slot(bool)
     def toggle_console_visibility(self):
         """Toggle the visibility of the console widget."""
         if self.ui.actionConsole.isChecked():
-            self.txConsole.show()
+            self.txt_console.show()
         else:
-            self.txConsole.hide()
+            self.txt_console.hide()
 
-    @Slot(bool, name="toggle_dataviewer_visibility")
+    @Slot(bool)
     def toggle_dataviewer_visibility(self):
         """Toggle the visibility of the console dock widget."""
         if self.data_viewer is not None:
             if self.ui.actionData_viewer.isChecked():
                 self.data_viewer.show()
             else:
                 self.data_viewer.hide()
 
-    @Slot(None, name="save_native_file")
+    @Slot()
     def save_native_file(self):
         """Save data to native pyMINFLUX `.pmx` file."""
-        if self.processor is None or len(self.processor.filtered_dataframe.index) == 0:
+        if (
+            self.processor is None
+            or self.processor.filtered_dataframe is None
+            or len(self.processor.filtered_dataframe.index) == 0
+        ):
             return
 
         # Get current filename to build the suggestion output
         if self.processor.filename is None:
-            out_filename = str(self.last_selected_path)
+            # Just use the path
+            out_filename = str(self.state.last_selected_path)
         else:
             out_filename = str(
                 self.processor.filename.parent / f"{self.processor.filename.stem}.pmx"
             )
 
         # Ask the user to pick a name (and format)
         filename, ext = QFileDialog.getSaveFileName(
@@ -547,28 +528,33 @@
         else:
             QMessageBox.critical(
                 self,
                 "Error",
                 f"Could not save file {Path(filename).name}!\n\nThe error was:\n{writer.message}",
             )
 
-    @Slot(None, name="select_and_load_or_import_data_file")
-    def select_and_load_or_import_data_file(self, filename: str = None):
+    @Slot()
+    def select_and_load_or_import_data_file(self, filename: Optional[str] = None):
         """
         Pick a MINFLUX `.pmx` file to load, or an Imspector `.npy' or '.mat' file to import.
         :return: void
         """
 
         # Do we have a filename?
         if filename is None or not filename:
             # Open a file dialog for the user to pick a .pmx, .npy or .mat file
+            if self.state.last_selected_path is not None:
+                save_path = str(self.state.last_selected_path)
+            else:
+                save_path = str(Path(".").absolute())
+
             res = QFileDialog.getOpenFileName(
                 self,
                 "Load file",
-                str(self.last_selected_path),
+                save_path,
                 "All Supported Files (*.pmx *.npy *.mat);;"
                 "pyMINFLUX file (*.pmx);;"
                 "Imspector NumPy files (*.npy);;"
                 "Imspector MATLAB mat files (*.mat)",
             )
             filename = res[0]
 
@@ -611,15 +597,15 @@
                     )
                     return
 
                 # Update the State from the read metadata
                 self.state.update_from_metadata(metadata)
 
                 # Inform
-                print("Applied settings from file.")
+                print(f"Loaded settings from {Path(filename).name}.")
 
             # Now pass the filename to the MinFluxReader
             try:
                 reader = MinFluxReader(
                     filename, z_scaling_factor=self.state.z_scaling_factor
                 )
             except IOError as e:
@@ -628,15 +614,19 @@
                     "Error",
                     f"{e}",
                 )
                 return
 
             # Open the Importer
             importer = Importer(
-                reader.valid_cfr, reader.relocalizations, self.state.dwell_time
+                valid_cfr=reader.valid_cfr,
+                relocalizations=reader.relocalizations,
+                dwell_time=self.state.dwell_time,
+                is_tracking=self.state.is_tracking,
+                pool_dcr=self.state.pool_dcr,
             )
             if importer.exec_() != QDialog.Accepted:
                 # The user cancelled the dialog
                 print("Loading cancelled.")
                 return
 
             # Retrieve the selected options from the Importer
@@ -646,24 +636,28 @@
             # trigger the creation of the dataframe, hence the
             # process=False argument everywhere).
             reader.set_tracking(selection["is_tracking"], process=False)
             reader.set_indices(
                 selection["iteration"], selection["cfr_iteration"], process=False
             )
             reader.set_dwell_time(selection["dwell_time"], process=False)
+            reader.set_pool_dcr(selection["pool_dcr"], process=False)
 
             # Update the state as well
             self.state.is_tracking = selection["is_tracking"]
             self.state.dwell_time = selection["dwell_time"]
+            if self.state.is_tracking:
+                self.state.plot_average_localisations = False
+            self.state.pool_dcr = selection["pool_dcr"]
 
             # Show some info
             print(reader)
 
             # Process the file
-            self.last_selected_path = Path(filename).parent
+            self.state.last_selected_path = Path(filename).parent
 
             # Add initialize the processor with the reader
             self.processor = MinFluxProcessor(reader, self.state.min_trace_length)
 
             # Make sure to set current value of use_weighted_localizations
             self.processor.use_weighted_localizations = (
                 self.state.weigh_avg_localization_by_eco
@@ -671,48 +665,56 @@
 
             # Show the filename on the main window
             self.setWindowTitle(
                 f"{__APP_NAME__} v{__version__} - [{Path(filename).name}]"
             )
 
             # Reset the plotter
-            if self.plotter is not None:
-                self.plotter.reset()
+            if self.plotter is None:
+                raise Exception("Plotter object not ready!")
+            self.plotter.reset()
+
+            # Reset the plotter toolbar
+            if self.plotter_toolbar is None:
+                raise Exception("Plotter Toolbar object not ready!")
+            self.plotter_toolbar.reset()
 
             # Close the Options
             if self.options is not None:
+                self.mediator.unregister_dialog("options")
                 self.options.close()
                 self.options = None
 
             # Close the Histogram Plotter
             if self.histogram_plotter is not None:
+                self.mediator.unregister_dialog("histogram_plotter")
                 self.histogram_plotter.close()
                 self.histogram_plotter = None
 
             # Close the Color Unmixer
             if self.color_unmixer is not None:
+                self.mediator.unregister_dialog("color_unmixer")
                 self.color_unmixer.close()
                 self.color_unmixer = None
 
             # Close the Temporal Inspector
             if self.time_inspector is not None:
+                self.mediator.unregister_dialog("time_inspector")
                 self.time_inspector.close()
                 self.time_inspector = None
 
             # Close the Trace Stats Viewer
             if self.trace_stats_viewer is not None:
+                self.mediator.unregister_dialog("trace_stats_viewer")
                 self.trace_stats_viewer.close()
                 self.trace_stats_viewer = None
 
-            if self.trace_length_viewer is not None:
-                self.trace_length_viewer.close()
-                self.trace_length_viewer = None
-
             # Close the FRC Tool
             if self.frc_tool is not None:
+                self.mediator.unregister_dialog("frc_tool")
                 self.frc_tool.close()
                 self.frc_tool = None
 
             # Update the ui
             self.full_update_ui()
 
             # Make sure to autoupdate the axis on load
@@ -750,23 +752,27 @@
             self.wizard.enable_controls(True)
 
         else:
             # If nothing is loaded (even from earlier), disable wizard
             if self.processor is None:
                 self.wizard.enable_controls(False)
 
-    @Slot(None, name="export_filtered_data")
+    @Slot()
     def export_filtered_data(self):
         """Export filtered data as CSV file."""
-        if self.processor is None or len(self.processor.filtered_dataframe.index) == 0:
+        if (
+            self.processor is None
+            or self.processor.filtered_dataframe is None
+            or len(self.processor.filtered_dataframe.index) == 0
+        ):
             return
 
         # Get current filename to build the suggestion output
         if self.processor.filename is None:
-            out_filename = str(self.last_selected_path)
+            out_filename = str(f"{Path('.') / self.processor.filename.stem}.csv")
         else:
             out_filename = str(
                 self.processor.filename.parent / f"{self.processor.filename.stem}.csv"
             )
 
         # Ask the user to pick a name (and format)
         filename, ext = QFileDialog.getSaveFileName(
@@ -800,29 +806,33 @@
         else:
             QMessageBox.critical(
                 self,
                 "Error",
                 f"Could not export filtered data to {Path(filename).name}.",
             )
 
-    @Slot(None, name="export_filtered_stats")
+    @Slot()
     def export_filtered_stats(self):
         """Export filtered, per-trace statistics as CSV file."""
-        if self.processor is None or len(self.processor.filtered_dataframe.index) == 0:
+        if (
+            self.processor is None
+            or self.processor.filtered_dataframe is None
+            or len(self.processor.filtered_dataframe.index) == 0
+        ):
             # Inform and return
             QMessageBox.information(
                 self,
                 "Info",
                 f"Sorry, nothing to export.",
             )
             return
 
         # Get current filename to build the suggestion output
         if self.processor.filename is None:
-            out_filename = str(self.last_selected_path)
+            out_filename = str(f"{Path('.') / self.processor.filename.stem}.csv")
         else:
             out_filename = str(
                 self.processor.filename.parent
                 / f"{self.processor.filename.stem}_stats.csv"
             )
 
         # Ask the user to pick a name
@@ -859,26 +869,26 @@
                 "Error",
                 f"Could not export trace statistics to {Path(filename).name}.\n\n{str(e)}.",
             )
             return
 
         print(f"Successfully exported statistics for {len(stats.index)} traces.")
 
-    @Slot(None, name="print_current_state")
+    @Slot()
     def print_current_state(self):
         """Print current contents of the state machine (DEBUG)."""
-        if self.txConsole.isHidden():
-            self.txConsole.show()
+        if self.txt_console.isHidden():
+            self.txt_console.show()
             self.ui.actionConsole.setChecked(True)
         state_dict = self.state.asdict()
         print("[DEBUG] Internal state:")
         for s in state_dict:
             print(f'  ∟ "{s}": {state_dict[s]}')
 
-    @Slot(None, name="about")
+    @Slot()
     def about(self):
         """Show simple About dialog."""
         from h5py import __version__ as h5py_version
         from numpy import __version__ as numpy_version
         from pandas import __version__ as pandas_version
         from pyarrow import __version__ as pyarrow_version
         from pyqtgraph import __version__ as pg_version
@@ -902,37 +912,103 @@
             f"NumPy {numpy_version}\n"
             f"SciPy {scipy_version}\n"
             f"Pandas {pandas_version}\n"
             f"PyArrow {pyarrow_version}\n"
             f"h5py {h5py_version}\n",
         )
 
-    @Slot(None, name="check_remote_for_updates")
+    @Slot()
     def check_remote_for_updates(self):
         """Check for application updates."""
 
         # Check for updates
         code, version, error = check_for_updates()
 
         # Process the output
         if code == -1:
             # Something went wrong: report
-            html = f"<b>Error! {error}</b><br /><br /><br />Please make sure you are connected to the internet.<br />If this error persists, please <a href='https://github.com/bsse-scf/pyMINFLUX/issues/'>report it</a>."
+            html = (
+                f"<b>Error! {error}</b><br /><br /><br />Please make sure you are connected to the internet.<br />"
+                f"If this error persists, please <a href='https://github.com/bsse-scf/pyMINFLUX/issues/'>report it</a>."
+            )
 
         elif code == 0:
             # No new version
-            html = f"<b>Congratulations!</b><br /><br />You are running the latest version ({pyminflux.__version__}) of {pyminflux.__APP_NAME__}."
+            html = (
+                f"<b>Congratulations!</b><br /><br />You are running the latest version ({pyminflux.__version__}) "
+                f"of {pyminflux.__APP_NAME__}."
+            )
 
         elif code == 1:
             # Show a dialog with a link to the download page
-            html = f"<b>There is a new version ({version}) of {pyminflux.__APP_NAME__}!</b><br /><br />You can download it from the <a href='https://github.com/bsse-scf/pyMINFLUX/releases/latest'>release page</a>."
+            html = (
+                f"<b>There is a new version ({version}) of {pyminflux.__APP_NAME__}!</b><br /><br />"
+                f"You can download it from the <a href='https://github.com/bsse-scf/pyMINFLUX/releases/latest'>release page</a>."
+            )
 
         else:
             raise ValueError("Unexpected code!")
 
+        # Update last check time
+        update_settings = UpdateSettings(self._check_interval_in_seconds)
+        update_settings.update_last_check_time()
+
+        # Show the dialog
+        self.show_update_result_dialog(html)
+
+    def auto_check_remote_for_updates(self):
+        """Automatic check for application updates."""
+
+        # Check if it is time to check
+        update_settings = UpdateSettings(self._check_interval_in_seconds)
+        if not update_settings.is_elapsed():
+            return
+
+        # For simplicity, we already update the last check timestamp
+        update_settings.update_last_check_time()
+
+        # Create the worker
+        self.update_worker = AutoUpdateCheckerWorker()
+
+        # Connect the signals
+        self.update_worker.result.connect(self.complete_check_remote_for_updates)
+
+        # Start the worker
+        self.update_worker.start()
+
+    def complete_check_remote_for_updates(self, is_update, version):
+        """Automatic check for application updates."""
+
+        # Only display the dialog if there is an update
+        if not is_update:
+            return
+
+        # Show a dialog with a link to the download page
+        html = (
+            f"<b>There is a new version ({version}) of {pyminflux.__APP_NAME__}!</b><br /><br />"
+            f"You can download it from the <a href='https://github.com/bsse-scf/pyMINFLUX/releases/latest'>release page</a>."
+        )
+
+        # Show the dialog
+        self.show_update_result_dialog(html)
+
+    @Slot()
+    def open_analyzer(self):
+        """Initialize and open the analyzer."""
+        if self.processor is None:
+            return
+        if self.analyzer is None:
+            self.analyzer = Analyzer(self.processor)
+            self.mediator.register_dialog("analyzer", self.analyzer)
+        self.analyzer.plot()
+        self.analyzer.show()
+        self.analyzer.activateWindow()
+
+    def show_update_result_dialog(self, html):
+        """Display the outcome of the update check in a dialog."""
         # Show the dialog
         dialog = QDialog()
         dialog.setWindowTitle("Check for updates")
         dialog.setMinimumSize(400, 180)
         dialog.setFixedHeight(180)
         layout = QVBoxLayout(dialog)
         text_browser = QTextBrowser()
@@ -941,169 +1017,91 @@
         text_browser.insertHtml(html)
         layout.addWidget(text_browser)
         button = QPushButton("OK")
         button.clicked.connect(dialog.close)
         layout.addWidget(button)
         dialog.exec_()
 
-    @Slot(None, name="open_analyzer")
-    def open_analyzer(self):
-        """Initialize and open the analyzer."""
-        if self.analyzer is None:
-            self.analyzer = Analyzer(self.processor)
-            self.wizard.wizard_filters_run.connect(self.analyzer.plot)
-            self.request_sync_external_tools.connect(self.analyzer.plot)
-            self.wizard.efo_bounds_modified.connect(self.analyzer.change_efo_bounds)
-            self.wizard.cfr_bounds_modified.connect(self.analyzer.change_cfr_bounds)
-            self.analyzer.data_filters_changed.connect(self.full_update_ui)
-            self.analyzer.efo_bounds_changed.connect(self.wizard.change_efo_bounds)
-            self.analyzer.cfr_bounds_changed.connect(self.wizard.change_cfr_bounds)
-        if self.histogram_plotter is not None:
-            self.analyzer.data_filters_changed.connect(
-                self.histogram_plotter.plot_histogram
-            )
-        if self.time_inspector is not None:
-            self.analyzer.data_filters_changed.connect(self.time_inspector.update)
-        if self.trace_stats_viewer is not None:
-            self.analyzer.data_filters_changed.connect(self.trace_stats_viewer.update)
-        if self.trace_length_viewer is not None:
-            self.analyzer.data_filters_changed.connect(self.trace_length_viewer.update)
-        self.analyzer.plot()
-        self.analyzer.show()
-        self.analyzer.activateWindow()
-
-    @Slot(None, name="open_time_inspector")
+    @Slot()
     def open_time_inspector(self):
         """Initialize and open the Time Inspector."""
         if self.time_inspector is None:
             self.time_inspector = TimeInspector(self.processor)
-            self.time_inspector.dataset_time_filtered.connect(self.full_update_ui)
-            self.wizard.wizard_filters_run.connect(self.time_inspector.update)
-            self.request_sync_external_tools.connect(self.time_inspector.update)
-        if self.analyzer is not None:
-            self.analyzer.data_filters_changed.connect(self.time_inspector.update)
-            self.time_inspector.dataset_time_filtered.connect(self.analyzer.plot)
-        if self.histogram_plotter is not None:
-            self.time_inspector.dataset_time_filtered.connect(
-                self.histogram_plotter.plot_histogram
-            )
-        if self.trace_stats_viewer is not None:
-            self.time_inspector.dataset_time_filtered.connect(
-                self.trace_stats_viewer.update
-            )
-        if self.trace_length_viewer is not None:
-            self.time_inspector.dataset_time_filtered.connect(
-                self.trace_length_viewer.update
-            )
+            self.mediator.register_dialog("time_inspector", self.time_inspector)
         self.time_inspector.show()
         self.time_inspector.activateWindow()
 
-    @Slot(None, name="open_histogram_plotter")
+    @Slot()
     def open_histogram_plotter(self):
         """Initialize and open the histogram plotter."""
+        if self.processor is None:
+            return
         if self.histogram_plotter is None:
             self.histogram_plotter = HistogramPlotter(self.processor)
-            self.request_sync_external_tools.connect(
-                self.histogram_plotter.plot_histogram
-            )
-            self.wizard.wizard_filters_run.connect(
-                self.histogram_plotter.plot_histogram
-            )
-            self.wizard.fluorophore_id_changed.connect(
-                self.histogram_plotter.plot_histogram
-            )
-        if self.analyzer is not None:
-            self.analyzer.data_filters_changed.connect(
-                self.histogram_plotter.plot_histogram
-            )
-        if self.color_unmixer is not None:
-            self.color_unmixer.fluorophore_ids_assigned.connect(
-                self.histogram_plotter.plot_histogram
-            )
-        if self.time_inspector is not None:
-            self.time_inspector.dataset_time_filtered.connect(
-                self.histogram_plotter.plot_histogram
-            )
+            self.mediator.register_dialog("histogram_plotter", self.histogram_plotter)
         self.histogram_plotter.show()
         self.histogram_plotter.activateWindow()
 
-    @Slot(None, name="open_color_unmixer")
+    @Slot()
     def open_color_unmixer(self):
         """Initialize and open the color unmixer."""
+        if self.processor is None:
+            return
         if self.color_unmixer is None:
             self.color_unmixer = ColorUnmixer(self.processor)
-            self.color_unmixer.fluorophore_ids_assigned.connect(
-                self.wizard.set_fluorophore_list
-            )
-            self.color_unmixer.fluorophore_ids_assigned.connect(
-                self.plot_selected_parameters
-            )
-            self.wizard.wizard_filters_run.connect(self.plot_selected_parameters)
-        if self.trace_stats_viewer is not None:
-            self.color_unmixer.fluorophore_ids_assigned.connect(
-                self.trace_stats_viewer.update
-            )
-        if self.trace_length_viewer is not None:
-            self.color_unmixer.fluorophore_ids_assigned.connect(
-                self.trace_length_viewer.update
-            )
+            self.mediator.register_dialog("color_unmixer", self.color_unmixer)
         self.color_unmixer.show()
         self.color_unmixer.activateWindow()
 
-    @Slot(None, name="open_options_dialog")
+    @Slot()
     def open_options_dialog(self):
         """Open the options dialog."""
         if self.options is None:
             self.options = Options()
-            self.options.min_trace_length_option_changed.connect(
-                self.update_min_trace_length
-            )
+            self.mediator.register_dialog("options", self.options)
         self.options.show()
         self.options.activateWindow()
 
-    @Slot(None, name="update_min_trace_length")
+    @Slot()
     def update_min_trace_length(self):
         if self.processor is not None:
             self.processor.min_trace_length = self.state.min_trace_length
 
-    @Slot(None, name="open_trace_stats_viewer")
+    @Slot()
     def open_trace_stats_viewer(self):
         """Open the trace stats viewer."""
+        if self.processor is None:
+            return
         if self.trace_stats_viewer is None:
             self.trace_stats_viewer = TraceStatsViewer(self.processor)
-            self.request_sync_external_tools.connect(self.trace_stats_viewer.update)
-            self.wizard.request_fluorophore_ids_reset.connect(
-                self.trace_stats_viewer.update
-            )
-            self.wizard.wizard_filters_run.connect(self.trace_stats_viewer.update)
-            self.trace_stats_viewer.export_trace_stats_requested.connect(
-                self.export_filtered_stats
-            )
-            self.wizard.fluorophore_id_changed.connect(self.trace_stats_viewer.update)
-        if self.color_unmixer is not None:
-            self.color_unmixer.fluorophore_ids_assigned.connect(
-                self.trace_stats_viewer.update
-            )
-        if self.analyzer is not None:
-            self.analyzer.data_filters_changed.connect(self.trace_stats_viewer.update)
+            self.mediator.register_dialog("trace_stats_viewer", self.trace_stats_viewer)
         self.trace_stats_viewer.show()
         self.trace_stats_viewer.activateWindow()
 
-    @Slot(None, name="open_frc_tool")
+    @Slot()
     def open_frc_tool(self):
         """Open the FRC tool."""
+        if self.processor is None:
+            return
         if self.frc_tool is None:
             self.frc_tool = FRCTool(self.processor)
+            self.mediator.register_dialog("frc_tool", self.frc_tool)
         self.frc_tool.show()
         self.frc_tool.activateWindow()
 
-    @Slot(list, name="show_selected_points_by_indices_in_dataviewer")
+    @Slot(list)
     def show_selected_points_by_indices_in_dataviewer(self, points):
         """Show the data for the selected points in the dataframe viewer."""
 
+        if self.data_viewer is None:
+            raise Exception("DataViewer object not ready!")
+
+        if self.processor is None:
+            return
+
         # Extract indices of the rows corresponding to the selected points
         indices = []
         for p in points:
             indices.append(p.index())
 
         # Sort the indices
         indices = sorted(indices)
@@ -1116,40 +1114,55 @@
         # Update the dataviewer
         self.data_viewer.set_data(df)
 
         # Inform
         point_str = "event" if len(indices) == 1 else "events"
         print(f"Selected {len(indices)} {point_str}.")
 
-    @Slot(tuple, tuple, name="show_selected_points_by_range_in_dataviewer")
+    @Slot(tuple, tuple)
     def show_selected_points_by_range_in_dataviewer(
         self, x_param, y_param, x_range, y_range
     ):
         """Select the data by x and y range and show in the dataframe viewer."""
 
+        if self.data_viewer is None:
+            raise Exception("DataViewer object not ready!")
+
+        if self.processor is None:
+            return
+
         # Get the filtered dataframe subset contained in the provided x and y ranges
         df = self.processor.select_by_2d_range(
             x_param,
             y_param,
             x_range,
             y_range,
             from_weighted_locs=self.state.plot_average_localisations,
         )
 
         # Update the dataviewer
         self.data_viewer.set_data(df)
 
         # Inform
-        point_str = "event" if len(df.index) == 1 else "events"
-        print(f"Selected {len(df.index)} {point_str}.")
+        if df is not None:
+            point_str = "event" if len(df.index) == 1 else "events"
+            print(f"Selected {len(df.index)} {point_str}.")
+        else:
+            print(f"Selected 0 events.")
 
-    @Slot(tuple, tuple, name="crop_data_by_range")
+    @Slot(tuple, tuple)
     def crop_data_by_range(self, x_param, y_param, x_range, y_range):
         """Filter the data by x and y range and show in the dataframe viewer."""
 
+        if self.plotter is None:
+            raise Exception("Plotter object not ready!")
+
+        if self.processor is None:
+            return
+
         # Filter the dataframe by the passed x and y ranges
         self.processor.filter_by_2d_range(x_param, y_param, x_range, y_range)
 
         # Update the Analyzer
         if self.analyzer is not None:
             self.analyzer.plot()
 
@@ -1179,19 +1192,26 @@
                 self.state.weigh_avg_localization_by_eco
             )
         self.plot_selected_parameters()
 
     def plot_selected_parameters(self):
         """Plot the localizations."""
 
+        if self.plotter is None:
+            raise Exception("Plotter object not ready!")
+
         # Remove the previous plots
         self.plotter.remove_points()
 
         # If there is nothing to plot, return here
-        if self.processor is None or len(self.processor.filtered_dataframe.index) == 0:
+        if (
+            self.processor is None
+            or self.processor.filtered_dataframe is None
+            or len(self.processor.filtered_dataframe.index) == 0
+        ):
             print("No data to process.")
             return
 
         # If an only if the requested parameters are "x" and "y" (in any order),
         # we consider the State.plot_average_localisations property.
         if (self.state.x_param == "x" and self.state.y_param == "y") or (
             self.state.x_param == "y" and self.state.y_param == "x"
@@ -1203,19 +1223,23 @@
                 # Get the (potentially filtered) full dataframe
                 dataframe = self.processor.filtered_dataframe
 
         else:
             # Get the (potentially filtered) full dataframe
             dataframe = self.processor.filtered_dataframe
 
+        # Do we have data to plot
+        if dataframe is None:
+            return
+
         # Extract values
-        x = dataframe[self.state.x_param].values
-        y = dataframe[self.state.y_param].values
-        tid = dataframe["tid"].values
-        fid = dataframe["fluo"].values
+        x = dataframe[self.state.x_param].to_numpy()
+        y = dataframe[self.state.y_param].to_numpy()
+        tid = dataframe["tid"].to_numpy()
+        fid = dataframe["fluo"].to_numpy()
 
         # Always plot the (x, y) coordinates in the 2D plotter
         self.plotter.plot_parameters(
             tid=tid,
             fid=fid,
             x=x,
             y=y,
@@ -1224,41 +1248,50 @@
         )
 
     def show_processed_dataframe(self, dataframe=None):
         """
         Displays the results for current frame in the data viewer.
         """
 
+        if self.data_viewer is None:
+            raise Exception("DataViewer object not ready!")
+
         # Is there data to process?
         if self.processor is None:
             self.data_viewer.clear()
             return
 
         if dataframe is None:
             # Get the (potentially filtered) dataframe
-            dataframe = self.processor.filtered_dataframe()
+            dataframe = self.processor.filtered_dataframe
 
         # Pass the dataframe to the pdDataViewer
         self.data_viewer.set_data(dataframe)
 
-    @Slot(int, name="update_fluorophore_id_in_processor_and_broadcast")
+    @Slot(int)
     def update_fluorophore_id_in_processor_and_broadcast(self, index):
         """Update the fluorophore ID in the processor and broadcast the change to all parties."""
 
+        if self.processor is None:
+            return
+
         # Update the processor
         self.processor.current_fluorophore_id = index
 
         # Update all views
         self.full_update_ui()
 
         # Update the analyzer as well
         if self.analyzer is not None:
             self.analyzer.plot()
 
     def reset_fluorophore_ids(self):
         """Reset the fluorophore IDs."""
 
+        if self.processor is None:
+            return
+
         # Reset
         self.processor.reset()
 
         # Update UI
         self.update_fluorophore_id_in_processor_and_broadcast(0)
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/main_window.ui` & `pyminflux-0.4.1/pyminflux/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/options.py` & `pyminflux-0.4.1/pyminflux/ui/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,19 +22,17 @@
 
 from ..settings import Settings
 from .ui_options import Ui_Options
 
 
 class Options(QDialog, Ui_Options):
     # Signal that the options have changed
-    min_trace_length_option_changed = Signal(name="min_trace_length_option_changed")
-    efo_bin_size_hz_option_changed = Signal(name="efo_bin_size_hz_option_changed")
-    weigh_avg_localization_by_eco_option_changed = Signal(
-        name="weigh_avg_localization_by_eco_option_changed"
-    )
+    min_trace_length_option_changed = Signal()
+    efo_bin_size_hz_option_changed = Signal()
+    weigh_avg_localization_by_eco_option_changed = Signal()
 
     def __init__(self, parent=None):
         """Constructor."""
 
         # Call the base class
         super().__init__()
 
@@ -206,81 +204,81 @@
         )
         self.ui.pbOpenConsoleAtStartHelp.clicked.connect(
             lambda _: self.ui.teHelp.setText(
                 "Whether to open the console at application start."
             )
         )
 
-    @Slot(str, name="persist_min_trace_length")
+    @Slot(str)
     def persist_min_trace_length(self, text):
         try:
             min_trace_length = int(text)
         except Exception as _:
             self.ui.leMinTIDNum.setStyleSheet("background-color: red;")
             self.valid["leMinTIDNum"] = False
             return
         self.ui.leMinTIDNum.setStyleSheet("")
         self.valid["leMinTIDNum"] = True
         self.state.min_trace_length = min_trace_length
 
         # Signal the change
         self.min_trace_length_option_changed.emit()
 
-    @Slot(str, name="persist_z_scaling_factor")
+    @Slot(str)
     def persist_z_scaling_factor(self, text):
         try:
             z_scaling_factor = float(text)
         except Exception as _:
             self.ui.leZScalingFactor.setStyleSheet("background-color: red;")
             self.valid["leZScalingFactor"] = False
             return
         self.ui.leZScalingFactor.setStyleSheet("")
         self.valid["leZScalingFactor"] = True
         self.state.z_scaling_factor = z_scaling_factor
 
-    @Slot(str, name="persist_plot_export_dpi")
+    @Slot(str)
     def persist_plot_export_dpi(self, text):
         try:
             plot_export_dpi = int(text)
         except Exception as _:
             self.ui.lePlotExportDPI.setStyleSheet("background-color: red;")
             self.valid["lePlotExportDPI"] = False
             return
         self.ui.lePlotExportDPI.setStyleSheet("")
         self.valid["lePlotExportDPI"] = True
         self.state.plot_export_dpi = plot_export_dpi
 
-    @Slot(str, name="persist_efo_bin_size_hz")
+    @Slot(str)
     def persist_efo_bin_size_hz(self, text):
         try:
             efo_bin_size_hz = float(text)
         except Exception as _:
             self.ui.leEFOBinSize.setStyleSheet("background-color: red;")
             self.valid["hlEFOBinSize"] = False
             return
         self.ui.leEFOBinSize.setStyleSheet("")
         self.valid["hlEFOBinSize"] = True
         self.state.efo_bin_size_hz = efo_bin_size_hz
 
         # Signal the change
         self.efo_bin_size_hz_option_changed.emit()
 
-    @Slot(str, name="persist_efo_expected_cutoff")
+    @Slot(str)
     def persist_efo_expected_cutoff(self, text):
         try:
             efo_expected_frequency = float(text)
         except Exception as _:
             self.ui.leEFOSingleEmitterFrequency.setStyleSheet("background-color: red;")
             self.valid["leEFOSingleEmitterFrequency"] = False
             return
         self.ui.leEFOSingleEmitterFrequency.setStyleSheet("")
         self.valid["leEFOSingleEmitterFrequency"] = True
         self.state.efo_expected_frequency = efo_expected_frequency
 
-    @Slot(str, name="persist_cfr_range")
+    @Slot(str)
     def persist_cfr_range(self, _):
         """Persist CFR range."""
 
         # Initialize the status to valid
         self.valid["leCFRRangeMin"] = True
         self.valid["leCFRRangeMax"] = True
 
@@ -311,15 +309,15 @@
             if cfr_min == "":
                 self.ui.leCFRRangeMin.setStyleSheet("background-color: red;")
                 self.valid["leCFRRangeMin"] = False
             if cfr_max == "":
                 self.ui.leCFRRangeMax.setStyleSheet("background-color: red;")
                 self.valid["leCFRRangeMax"] = False
 
-    @Slot(str, name="persist_efo_range")
+    @Slot(str)
     def persist_efo_range(self, _):
         """Persist EFO range."""
 
         # Initialize the status to valid
         self.valid["leEFORangeMin"] = True
         self.valid["leEFORangeMax"] = True
 
@@ -350,15 +348,15 @@
             if efo_min == "":
                 self.ui.leEFORangeMin.setStyleSheet("background-color: red;")
                 self.valid["leEFORangeMin"] = False
             if efo_max == "":
                 self.ui.leEFORangeMax.setStyleSheet("background-color: red;")
                 self.valid["leEFORangeMax"] = False
 
-    @Slot(str, name="persist_loc_prec_range")
+    @Slot(str)
     def persist_loc_prec_range(self, _):
         """Persist localization precision range."""
 
         # Initialize the status to valid
         self.valid["leLocPrecRangeMin"] = True
         self.valid["leLocPrecRangeMax"] = True
 
@@ -389,26 +387,26 @@
             if loc_prec_min == "":
                 self.ui.leLocPrecRangeMin.setStyleSheet("background-color: red;")
                 self.valid["leLocPrecRangeMin"] = False
             if loc_prec_max == "":
                 self.ui.leLocPrecRangeMax.setStyleSheet("background-color: red;")
                 self.valid["leLocPrecRangeMax"] = False
 
-    @Slot(str, name="persist_weigh_avg_localization_by_eco")
+    @Slot(str)
     def persist_weigh_avg_localization_by_eco(self, state):
         self.state.weigh_avg_localization_by_eco = state != 0
 
         # Signal the change
         self.weigh_avg_localization_by_eco_option_changed.emit()
 
-    @Slot(str, name="persist_open_console_at_start")
+    @Slot(str)
     def persist_open_console_at_start(self, state):
         self.state.open_console_at_start = state != 0
 
-    @Slot(str, name="set_as_new_default")
+    @Slot(str)
     def set_as_new_default(self, text):
         """Persist current selection as new default options."""
 
         # Only save if all fields are properly set
         all_true = all(self.valid.values())
 
         if not all_true:
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/options.ui` & `pyminflux-0.4.1/pyminflux/ui/options.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/pandas_datamodel.py` & `pyminflux-0.4.1/pyminflux/ui/pandas_datamodel.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/plotter.py` & `pyminflux-0.4.1/pyminflux/ui/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,17 @@
     export_plot_interactive,
     update_brushes_by_,
 )
 
 
 class Plotter(PlotWidget):
     # Signals
-    locations_selected = Signal(list, name="locations_selected")
-    locations_selected_by_range = Signal(
-        str, str, tuple, tuple, name="locations_selected_by_range"
-    )
-    crop_region_selected = Signal(str, str, tuple, tuple, name="crop_region_selected")
+    locations_selected = Signal(list)
+    locations_selected_by_range = Signal(str, str, tuple, tuple)
+    crop_region_selected = Signal(str, str, tuple, tuple)
 
     def __init__(self):
         super().__init__()
         self.setBackground("w")
         self.brush = pg.mkBrush(255, 255, 255, 128)
         self.pen = pg.mkPen(None)
         self.remove_points()
@@ -123,16 +121,16 @@
             # Accept the event
             ev.accept()
 
         elif (
             self.scatter_plot is not None
             and ev.button() == Qt.MouseButton.LeftButton
             and ev.modifiers() == QtCore.Qt.ControlModifier
-            and self.state.x_param in ("x", "y")
-            and self.state.y_param in ("x", "y")
+            and self.state.x_param in ("x", "y", "z")
+            and self.state.y_param in ("x", "y", "z")
         ):
             # Is the user trying to initiate drawing a line?
 
             # Remove previous line if it exists
             if self.line is not None:
                 self.removeItem(self.line)
                 self.line.deleteLater()
@@ -190,28 +188,30 @@
                 super().mousePressEvent(ev)
 
     def mouseMoveEvent(self, ev):
         # Is the user drawing an ROI?
         if (
             self.scatter_plot is not None
             and ev.buttons() == Qt.MouseButton.LeftButton
+            and self.ROI is not None
             and self._roi_is_being_drawn
         ):
             # Resize the ROI
             current_point = (
                 self.getPlotItem().getViewBox().mapSceneToView(ev.position())
             )
             self.ROI.setSize(current_point - self._roi_start_point)
 
             # Accept the event
             ev.accept()
 
         elif (
             self.scatter_plot is not None
             and ev.buttons() == Qt.MouseButton.LeftButton
+            and self.line is not None
             and self._line_is_being_drawn
         ):
             # Is the user drawing a line?
 
             # Resize the ROI
             current_point = (
                 self.getPlotItem().getViewBox().mapSceneToView(ev.position())
@@ -225,91 +225,101 @@
             ev.accept()
         else:
             # Call the parent method
             ev.ignore()
             super().mouseMoveEvent(ev)
 
     def mouseReleaseEvent(self, ev):
-        if (
-            self.scatter_plot is not None
-            and ev.button() == Qt.MouseButton.LeftButton
-            and self._roi_is_being_drawn
-        ):
-            # Extract the ranges
-            x_range, y_range = self._get_ranges_from_roi()
-
-            # Get current parameters
-            x_param = self.state.x_param
-            y_param = self.state.y_param
+        if self.scatter_plot is not None and ev.button() == Qt.MouseButton.LeftButton:
+            if self._roi_is_being_drawn:
+                # Extract the ranges
+                x_range, y_range = self._get_ranges_from_roi()
+                if x_range is None or y_range is None:
+                    # Handle the case where ranges are None
+                    return
+
+                # Get current parameters
+                x_param = self.state.x_param
+                y_param = self.state.y_param
 
-            # Update the DataViewer with current selection
-            if x_range is not None and y_range is not None:
+                # Update the DataViewer with current selection
                 self.locations_selected_by_range.emit(
                     x_param, y_param, x_range, y_range
                 )
 
-            # Reset flags
-            self._roi_start_point = None
-            self._roi_is_being_drawn = False
+                # Reset flags
+                self._roi_start_point = None
+                self._roi_is_being_drawn = False
+
+                # Check if the ROI has 0 size
+                if (
+                    np.abs(x_range[1] - x_range[0]) < 1e-4
+                    or np.abs(y_range[1] - y_range[0]) < 1e-4
+                ):
+                    if hasattr(self, "ROI") and self.ROI:
+                        self.removeItem(self.ROI)
+                        self.ROI.deleteLater()
+                        self.ROI = None
 
-            # If the ROI has 0 size (when a shift-click has been used to remove a previous ROI),
-            # clean it up properly.
-            if (
-                np.abs(x_range[1] - x_range[0]) < 1e-4
-                or np.abs(y_range[1] - y_range[0]) < 1e-4
-            ):
-                self.removeItem(self.ROI)
-                self.ROI.deleteLater()
-                self.ROI = None
+                # Accept the event
+                ev.accept()
 
-            # Accept the event
-            ev.accept()
+            elif self._line_is_being_drawn:
+                if self.line:
+                    # Display the measurement
+                    x_data, y_data = self.line.getData()
+                    if (
+                        x_data is None
+                        or len(x_data) < 2
+                        or y_data is None
+                        or len(y_data) < 2
+                    ):  # Check if data is incomplete
+                        return
+
+                    center = np.array(
+                        [0.5 * (x_data[0] + x_data[1]), 0.5 * (y_data[0] + y_data[1])]
+                    )
+                    delta_y = y_data[1] - y_data[0]
+                    delta_x = x_data[1] - x_data[0]
+                    v = np.array([-1.0 * delta_y, delta_x])
+                    norm = np.linalg.norm(v)
+
+                    if norm >= 1e-4:
+                        v_norm = v / norm
+                        length = np.sqrt(delta_x**2 + delta_y**2)
+                        pos = center + 1.0 * v_norm
+                        clr = (
+                            (255, 255, 0)
+                            if self.state.color_code == ColorCode.NONE
+                            else (255, 255, 255)
+                        )
+                        self.line_text = TextItem(text=f"{length:.2f} nm", color=clr)
+                        self.line_text.setPos(pos[0], pos[1])
+                        self.addItem(self.line_text)
+                    else:
+                        self.removeItem(self.line)
+                        self.line.deleteLater()
+                        self.line = None
+
+                    # Reset flags
+                    self._line_start_point = None
+                    self._line_is_being_drawn = False
 
-        elif (
-            self.scatter_plot is not None
-            and ev.button() == Qt.MouseButton.LeftButton
-            and self._line_is_being_drawn
-        ):
-            # Display the measurement
-            x_data, y_data = self.line.getData()
-            center = np.array(
-                [0.5 * (x_data[0] + x_data[1]), 0.5 * (y_data[0] + y_data[1])]
-            )
-            delta_y = np.array(y_data[1] - y_data[0])
-            delta_x = np.array(x_data[1] - x_data[0])
-            v = np.array([-1.0 * delta_y, delta_x])
-            norm = np.linalg.norm(v)
-            if np.abs(norm) >= 1e-4:
-                v_norm = v / norm
-                length = np.sqrt(delta_x * delta_x + delta_y * delta_y)
-                pos = center + 1.0 * v_norm
-                if self.state.color_code == ColorCode.NONE:
-                    clr = (255, 255, 0)
+                    # Accept the event
+                    ev.accept()
                 else:
-                    clr = (255, 255, 255)
-                self.line_text = TextItem(text=f"{length:.2f} nm", color=clr)
-                self.line_text.setPos(pos[0], pos[1])
-                self.addItem(self.line_text)
-            else:
-                if self.line is not None:
-                    self.removeItem(self.line)
-                    self.line.deleteLater()
-                    self.line = None
-
-            # Reset flags
-            self._line_start_point = None
-            self._line_is_being_drawn = False
-
-            # Accept the event
-            ev.accept()
+                    # If line is None, safely ignore the operation
+                    ev.ignore()
 
+            else:
+                # Call the parent method if no conditions are met
+                super().mouseReleaseEvent(ev)
         else:
-            # Call the parent method
+            # Properly ignore the event if conditions are not met
             ev.ignore()
-            super().mouseReleaseEvent(ev)
 
     def reset(self):
         # Forget last plot
         self._last_x_param = None
         self._last_y_param = None
         self.remove_points()
 
@@ -335,15 +345,15 @@
         elif self.state.color_code == ColorCode.BY_FLUO:
             if self._fid_to_brush is None:
                 brushes, self._fid_to_brush = create_brushes_by(
                     fid, color_scheme="green-magenta"
                 )
             else:
                 brushes, self._fid_to_brush = update_brushes_by_(
-                    fid, self._fid_to_brush
+                    fid, self._fid_to_brush, color_scheme="green-magenta"
                 )
         else:
             raise ValueError("Unexpected request for color-coding the localizations!")
 
         # Create the scatter_plot plot
         self.scatter_plot = pg.ScatterPlotItem(
             x=x,
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/plotter_toolbar.py` & `pyminflux-0.4.1/pyminflux/ui/plotter_toolbar.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,19 +18,17 @@
 
 from ..reader import MinFluxReader
 from ..state import ColorCode, State
 from .ui_plotter_toolbar import Ui_PlotterToolbar
 
 
 class PlotterToolbar(QWidget, Ui_PlotterToolbar):
-    plot_requested_parameters = Signal(None, name="plot_requested_parameters")
-    color_code_locs_changed = Signal(int, name="color_code_locs_changed")
-    plot_average_positions_state_changed = Signal(
-        None, name="plot_average_positions_state_changed"
-    )
+    plot_requested_parameters = Signal()
+    color_code_locs_changed = Signal(int)
+    plot_average_positions_state_changed = Signal()
 
     def __init__(self):
         """Constructor."""
 
         # Call the base class
         super().__init__()
 
@@ -66,54 +64,67 @@
 
         # Set the state of the average checkbox
         self.ui.cbPlotAveragePos.setChecked(self.state.plot_average_localisations)
         self.ui.cbPlotAveragePos.stateChanged.connect(
             self.persist_plot_average_localisations_and_broadcast
         )
 
-    @Slot(int, name="persist_plot_average_localisations_and_broadcast")
+    @Slot(int)
     def persist_plot_average_localisations_and_broadcast(self, value):
         """Persist the selection for plotting average positions."""
         if value == Qt.CheckState.Checked.value:
             self.state.plot_average_localisations = True
         else:
             self.state.plot_average_localisations = False
         self.plot_average_positions_state_changed.emit()
 
-    @Slot(int, name="toggle_average_state")
+    @Slot(int)
     def toggle_average_state(self, index):
         """Persist the selection for the second parameter."""
 
         # Enable the Average checkbox only for x, y plots
-        if self.state.x_param in ["x", "y"] and self.state.y_param in ["x", "y"]:
+        if (
+            not self.state.is_tracking
+            and self.state.x_param in ["x", "y"]
+            and self.state.y_param in ["x", "y"]
+        ):
             self.ui.cbPlotAveragePos.setEnabled(True)
         else:
             self.ui.cbPlotAveragePos.setEnabled(False)
 
-    @Slot(int, name="persist_color_code_and_broadcast")
+    @Slot(int)
     def persist_color_code_and_broadcast(self, index):
         """Persist the selection of the color code and broadcast a change."""
         self.state.color_code = ColorCode(index)
 
         # Broadcast the change
         self.color_code_locs_changed.emit(self.state.color_code.value)
 
-    @Slot(int, name="persist_first_param")
+    @Slot(int)
     def persist_first_param(self, index):
         """Persist the selection for the first parameter."""
 
         # Persist the selection
         self.state.x_param = self.plotting_parameters[index]
 
-    @Slot(int, name="persist_second_param")
+    @Slot(int)
     def persist_second_param(self, index):
         """Persist the selection for the second parameter."""
 
         # Persist the selection
         self.state.y_param = self.plotting_parameters[index]
 
-    @Slot(None, name="emit_plot_requested")
+    @Slot()
     def emit_plot_requested(self):
         """Plot the requested parameters."""
 
         # Emit signal
         self.plot_requested_parameters.emit()
+
+    def reset(self):
+        """Reset the toolbar."""
+        if self.state.is_tracking and self.state.plot_average_localisations:
+            print(
+                "DEBUG: Inconsistent state! Both `self.state.is_tracking` and `self.state.plot_average_localisations` are true!"
+            )
+            self.state.plot_average_localisations = False
+        self.toggle_average_state(None)
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/plotter_toolbar.ui` & `pyminflux-0.4.1/pyminflux/ui/plotter_toolbar.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/roi_ranges.py` & `pyminflux-0.4.1/pyminflux/ui/roi_ranges.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from ..state import State
 from .ui_roi_ranges import Ui_ROIRanges
 
 
 class ROIRanges(QDialog, Ui_ROIRanges):
     # Signal that the data viewers should be updated
-    data_ranges_changed = Signal(None, name="data_ranges_changed")
+    data_ranges_changed = Signal()
 
     def __init__(self, parent=None):
         """Constructor."""
 
         # Call the base class
         super().__init__()
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/roi_ranges.ui` & `pyminflux-0.4.1/pyminflux/ui/roi_ranges.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/time_inspector.py` & `pyminflux-0.4.1/pyminflux/ui/time_inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 
 class TimeInspector(QDialog, Ui_TimeInspector):
     """
     A QDialog to perform temporal analysis and selection.
     """
 
     # Signal that the fluorophore IDs have been assigned
-    fluorophore_ids_assigned = Signal(int, name="fluorophore_ids_assigned")
-    processing_started = Signal(None, name="processing_started")
-    processing_completed = Signal(None, name="processing_completed")
-    dataset_time_filtered = Signal(None, name="dataset_time_filtered")
+    fluorophore_ids_assigned = Signal(int)
+    processing_started = Signal()
+    processing_completed = Signal()
+    dataset_time_filtered = Signal()
 
     def __init__(self, processor):
         # Call the base class
         super().__init__()
 
         # Initialize the dialog
         self.ui = Ui_TimeInspector()
@@ -115,28 +115,28 @@
         self.localization_precision_per_unit_time_cache_x = None
         self.localization_precision_per_unit_time_cache_y = None
         self.localization_precision_per_unit_time_cache_z = None
         self.localization_precision_stderr_per_unit_time_cache_x = None
         self.localization_precision_stderr_per_unit_time_cache_y = None
         self.localization_precision_stderr_per_unit_time_cache_z = None
 
-    @Slot(None, name="update")
+    @Slot()
     def update(self):
         """Update the plots as response to data changes."""
 
         # Invalidate cache
         self.invalidate_cache()
 
         # Switch back to the fastest plot
         self.ui.cbAnalysisSelection.setCurrentIndex(0)
 
         # Plot
         self.plot_selected()
 
-    @Slot(None, name="plot_selected")
+    @Slot()
     def plot_selected(self):
         """Perform and plot the results of the selected analysis."""
 
         # Do we have something to plot?
         if (
             self.processor is None
             or self.processor.filtered_dataframe is None
@@ -233,15 +233,15 @@
                 step=self.time_resolution_sec,
             )
             bin_centers = bin_edges[:-1] + 0.5 * self.time_resolution_sec
             bin_width = self.time_resolution_sec
 
             # Calculate the histogram of localizations per unit time
             self.localizations_per_unit_time_cache, _ = np.histogram(
-                self.processor.filtered_dataframe["tim"].values,
+                self.processor.filtered_dataframe["tim"].to_numpy(),
                 bins=bin_edges,
                 density=False,
             )
 
             # Cache the x range
             self.x_axis = (bin_centers - 0.5 * bin_width) / self.time_resolution_sec
 
@@ -554,15 +554,15 @@
             )
         else:
             self.roi_ranges_dialog.update_fields()
         self.roi_ranges_dialog.set_target(item)
         self.roi_ranges_dialog.show()
         self.roi_ranges_dialog.activateWindow()
 
-    @Slot(None, name="roi_changes_finished")
+    @Slot()
     def roi_changes_finished(self):
         """Called when the ROIChanges dialog has accepted the changes."""
 
         # Signal blocker on self.efo_plot, self.cfr_plot and self.tr_len_plot
         plot_blocker = QSignalBlocker(self.plot_widget)
 
         # Block signals from the plot widget
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/time_inspector.ui` & `pyminflux-0.4.1/pyminflux/ui/time_inspector.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/trace_dataviewer.py` & `pyminflux-0.4.1/pyminflux/ui/trace_dataviewer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/trace_stats_viewer.py` & `pyminflux-0.4.1/pyminflux/ui/trace_stats_viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 class TraceStatsViewer(QDialog, Ui_TraceStatsViewer):
     """
     A QDialog to display trace statistics.
     """
 
-    export_trace_stats_requested = Signal(None, name="export_trace_stats_requested")
+    export_trace_stats_requested = Signal()
 
     def __init__(self, processor: MinFluxProcessor):
         # Call the base class
         super().__init__()
 
         # Initialize the dialog
         self.ui = Ui_TraceStatsViewer()
@@ -61,13 +61,13 @@
 
         # Update the viewer
         self.update()
 
         # Show the data
         self.trace_dataviewer.show()
 
-    @Slot(None, name="update")
+    @Slot()
     def update(self):
         """Update the viewer."""
         if self.processor is None:
             return
         self.trace_dataviewer.set_data(self.processor.filtered_dataframe_stats)
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/trace_stats_viewer.ui` & `pyminflux-0.4.1/pyminflux/ui/trace_stats_viewer.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/ui_analyzer.py` & `pyminflux-0.4.1/pyminflux/ui/ui_analyzer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/ui_color_unmixer.py` & `pyminflux-0.4.1/pyminflux/ui/ui_color_unmixer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/ui_frc_tool.py` & `pyminflux-0.4.1/pyminflux/ui/ui_frc_tool.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/ui_histogram_plotter.py` & `pyminflux-0.4.1/pyminflux/ui/ui_histogram_plotter.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/ui_importer.py` & `pyminflux-0.4.1/pyminflux/ui/ui_importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'importer.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.2
+## Created by: Qt User Interface Compiler version 6.7.0
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (
     QCoreApplication,
     QDate,
@@ -57,702 +57,714 @@
 )
 
 
 class Ui_Importer(object):
     def setupUi(self, Importer):
         if not Importer.objectName():
             Importer.setObjectName("Importer")
-        Importer.setWindowModality(Qt.NonModal)
+        Importer.setWindowModality(Qt.WindowModality.NonModal)
         Importer.resize(417, 813)
         sizePolicy = QSizePolicy(
             QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Preferred
         )
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(Importer.sizePolicy().hasHeightForWidth())
         Importer.setSizePolicy(sizePolicy)
         Importer.setMinimumSize(QSize(260, 0))
         Importer.setModal(True)
         self.gridLayout = QGridLayout(Importer)
         self.gridLayout.setObjectName("gridLayout")
-        self.lbIter_13 = QLabel(Importer)
-        self.lbIter_13.setObjectName("lbIter_13")
-        self.lbIter_13.setEnabled(True)
-        sizePolicy1 = QSizePolicy(
-            QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Fixed
-        )
-        sizePolicy1.setHorizontalStretch(0)
-        sizePolicy1.setVerticalStretch(0)
-        sizePolicy1.setHeightForWidth(self.lbIter_13.sizePolicy().hasHeightForWidth())
-        self.lbIter_13.setSizePolicy(sizePolicy1)
-        font = QFont()
-        font.setBold(True)
-        self.lbIter_13.setFont(font)
-        self.lbIter_13.setAlignment(Qt.AlignCenter)
-
-        self.gridLayout.addWidget(self.lbIter_13, 14, 1, 1, 1)
-
-        self.lbReloc_0 = QLabel(Importer)
-        self.lbReloc_0.setObjectName("lbReloc_0")
-        sizePolicy1.setHeightForWidth(self.lbReloc_0.sizePolicy().hasHeightForWidth())
-        self.lbReloc_0.setSizePolicy(sizePolicy1)
-        self.lbReloc_0.setFont(font)
-        self.lbReloc_0.setAlignment(Qt.AlignCenter)
-
-        self.gridLayout.addWidget(self.lbReloc_0, 1, 2, 1, 1)
-
-        self.lbReloc_15 = QLabel(Importer)
-        self.lbReloc_15.setObjectName("lbReloc_15")
-        sizePolicy1.setHeightForWidth(self.lbReloc_15.sizePolicy().hasHeightForWidth())
-        self.lbReloc_15.setSizePolicy(sizePolicy1)
-        self.lbReloc_15.setFont(font)
-        self.lbReloc_15.setAlignment(Qt.AlignCenter)
-
-        self.gridLayout.addWidget(self.lbReloc_15, 16, 2, 1, 1)
-
-        self.pbIter_7 = QPushButton(Importer)
-        self.pbIter_7.setObjectName("pbIter_7")
-        self.pbIter_7.setEnabled(True)
-        sizePolicy2 = QSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Fixed)
-        sizePolicy2.setHorizontalStretch(0)
-        sizePolicy2.setVerticalStretch(0)
-        sizePolicy2.setHeightForWidth(self.pbIter_7.sizePolicy().hasHeightForWidth())
-        self.pbIter_7.setSizePolicy(sizePolicy2)
-        self.pbIter_7.setCheckable(False)
-
-        self.gridLayout.addWidget(self.pbIter_7, 8, 0, 1, 1)
-
-        self.lbIter_5 = QLabel(Importer)
-        self.lbIter_5.setObjectName("lbIter_5")
-        self.lbIter_5.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_5.sizePolicy().hasHeightForWidth())
-        self.lbIter_5.setSizePolicy(sizePolicy1)
-        self.lbIter_5.setFont(font)
-        self.lbIter_5.setAlignment(Qt.AlignCenter)
-
-        self.gridLayout.addWidget(self.lbIter_5, 6, 1, 1, 1)
-
-        self.cbTracking = QCheckBox(Importer)
-        self.cbTracking.setObjectName("cbTracking")
-
-        self.gridLayout.addWidget(self.cbTracking, 25, 0, 1, 1)
-
-        self.lbIter_8 = QLabel(Importer)
-        self.lbIter_8.setObjectName("lbIter_8")
-        self.lbIter_8.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_8.sizePolicy().hasHeightForWidth())
-        self.lbIter_8.setSizePolicy(sizePolicy1)
-        self.lbIter_8.setFont(font)
-        self.lbIter_8.setAlignment(Qt.AlignCenter)
-
-        self.gridLayout.addWidget(self.lbIter_8, 9, 1, 1, 1)
-
-        self.lbReloc_6 = QLabel(Importer)
-        self.lbReloc_6.setObjectName("lbReloc_6")
-        sizePolicy1.setHeightForWidth(self.lbReloc_6.sizePolicy().hasHeightForWidth())
-        self.lbReloc_6.setSizePolicy(sizePolicy1)
-        self.lbReloc_6.setFont(font)
-        self.lbReloc_6.setAlignment(Qt.AlignCenter)
-
-        self.gridLayout.addWidget(self.lbReloc_6, 7, 2, 1, 1)
-
-        self.lbCFRValues = QLabel(Importer)
-        self.lbCFRValues.setObjectName("lbCFRValues")
-        self.lbCFRValues.setFont(font)
-        self.lbCFRValues.setAlignment(Qt.AlignCenter)
-
-        self.gridLayout.addWidget(self.lbCFRValues, 0, 1, 1, 1)
-
         self.lbRelocInfo = QLabel(Importer)
         self.lbRelocInfo.setObjectName("lbRelocInfo")
 
         self.gridLayout.addWidget(self.lbRelocInfo, 21, 0, 1, 3)
 
-        self.line = QFrame(Importer)
-        self.line.setObjectName("line")
-        self.line.setFrameShape(QFrame.HLine)
-        self.line.setFrameShadow(QFrame.Sunken)
-
-        self.gridLayout.addWidget(self.line, 24, 0, 1, 3)
-
         self.pbIter_8 = QPushButton(Importer)
         self.pbIter_8.setObjectName("pbIter_8")
         self.pbIter_8.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_8.sizePolicy().hasHeightForWidth())
-        self.pbIter_8.setSizePolicy(sizePolicy2)
+        sizePolicy1 = QSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Fixed)
+        sizePolicy1.setHorizontalStretch(0)
+        sizePolicy1.setVerticalStretch(0)
+        sizePolicy1.setHeightForWidth(self.pbIter_8.sizePolicy().hasHeightForWidth())
+        self.pbIter_8.setSizePolicy(sizePolicy1)
         self.pbIter_8.setCheckable(False)
 
         self.gridLayout.addWidget(self.pbIter_8, 9, 0, 1, 1)
 
-        self.lbReloc_3 = QLabel(Importer)
-        self.lbReloc_3.setObjectName("lbReloc_3")
-        sizePolicy1.setHeightForWidth(self.lbReloc_3.sizePolicy().hasHeightForWidth())
-        self.lbReloc_3.setSizePolicy(sizePolicy1)
-        self.lbReloc_3.setFont(font)
-        self.lbReloc_3.setAlignment(Qt.AlignCenter)
+        self.pbIter_3 = QPushButton(Importer)
+        self.pbIter_3.setObjectName("pbIter_3")
+        self.pbIter_3.setEnabled(True)
+        sizePolicy1.setHeightForWidth(self.pbIter_3.sizePolicy().hasHeightForWidth())
+        self.pbIter_3.setSizePolicy(sizePolicy1)
+        self.pbIter_3.setCheckable(False)
 
-        self.gridLayout.addWidget(self.lbReloc_3, 4, 2, 1, 1)
+        self.gridLayout.addWidget(self.pbIter_3, 4, 0, 1, 1)
 
-        self.lbIter_14 = QLabel(Importer)
-        self.lbIter_14.setObjectName("lbIter_14")
-        self.lbIter_14.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_14.sizePolicy().hasHeightForWidth())
-        self.lbIter_14.setSizePolicy(sizePolicy1)
-        self.lbIter_14.setFont(font)
-        self.lbIter_14.setAlignment(Qt.AlignCenter)
+        self.pbIter_10 = QPushButton(Importer)
+        self.pbIter_10.setObjectName("pbIter_10")
+        self.pbIter_10.setEnabled(True)
+        sizePolicy1.setHeightForWidth(self.pbIter_10.sizePolicy().hasHeightForWidth())
+        self.pbIter_10.setSizePolicy(sizePolicy1)
+        self.pbIter_10.setCheckable(False)
 
-        self.gridLayout.addWidget(self.lbIter_14, 15, 1, 1, 1)
+        self.gridLayout.addWidget(self.pbIter_10, 11, 0, 1, 1)
 
-        self.lbIter_0 = QLabel(Importer)
-        self.lbIter_0.setObjectName("lbIter_0")
-        self.lbIter_0.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_0.sizePolicy().hasHeightForWidth())
-        self.lbIter_0.setSizePolicy(sizePolicy1)
-        self.lbIter_0.setFont(font)
-        self.lbIter_0.setAlignment(Qt.AlignCenter)
+        self.lbReloc = QLabel(Importer)
+        self.lbReloc.setObjectName("lbReloc")
+        font = QFont()
+        font.setBold(True)
+        self.lbReloc.setFont(font)
+        self.lbReloc.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbIter_0, 1, 1, 1, 1)
+        self.gridLayout.addWidget(self.lbReloc, 0, 2, 1, 1)
 
-        self.lbIter_10 = QLabel(Importer)
-        self.lbIter_10.setObjectName("lbIter_10")
-        self.lbIter_10.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_10.sizePolicy().hasHeightForWidth())
-        self.lbIter_10.setSizePolicy(sizePolicy1)
-        self.lbIter_10.setFont(font)
-        self.lbIter_10.setAlignment(Qt.AlignCenter)
+        self.lbReloc_11 = QLabel(Importer)
+        self.lbReloc_11.setObjectName("lbReloc_11")
+        sizePolicy2 = QSizePolicy(
+            QSizePolicy.Policy.Preferred, QSizePolicy.Policy.Fixed
+        )
+        sizePolicy2.setHorizontalStretch(0)
+        sizePolicy2.setVerticalStretch(0)
+        sizePolicy2.setHeightForWidth(self.lbReloc_11.sizePolicy().hasHeightForWidth())
+        self.lbReloc_11.setSizePolicy(sizePolicy2)
+        self.lbReloc_11.setFont(font)
+        self.lbReloc_11.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbIter_10, 11, 1, 1, 1)
+        self.gridLayout.addWidget(self.lbReloc_11, 12, 2, 1, 1)
 
-        self.pbIter_6 = QPushButton(Importer)
-        self.pbIter_6.setObjectName("pbIter_6")
-        self.pbIter_6.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_6.sizePolicy().hasHeightForWidth())
-        self.pbIter_6.setSizePolicy(sizePolicy2)
-        self.pbIter_6.setCheckable(False)
+        self.lbReloc_5 = QLabel(Importer)
+        self.lbReloc_5.setObjectName("lbReloc_5")
+        sizePolicy2.setHeightForWidth(self.lbReloc_5.sizePolicy().hasHeightForWidth())
+        self.lbReloc_5.setSizePolicy(sizePolicy2)
+        self.lbReloc_5.setFont(font)
+        self.lbReloc_5.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.pbIter_6, 7, 0, 1, 1)
+        self.gridLayout.addWidget(self.lbReloc_5, 6, 2, 1, 1)
 
-        self.buttonBox = QDialogButtonBox(Importer)
-        self.buttonBox.setObjectName("buttonBox")
-        self.buttonBox.setOrientation(Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel | QDialogButtonBox.Ok)
+        self.lbIter_0 = QLabel(Importer)
+        self.lbIter_0.setObjectName("lbIter_0")
+        self.lbIter_0.setEnabled(True)
+        sizePolicy2.setHeightForWidth(self.lbIter_0.sizePolicy().hasHeightForWidth())
+        self.lbIter_0.setSizePolicy(sizePolicy2)
+        self.lbIter_0.setFont(font)
+        self.lbIter_0.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.buttonBox, 28, 0, 1, 3)
+        self.gridLayout.addWidget(self.lbIter_0, 1, 1, 1, 1)
 
-        self.verticalSpacer = QSpacerItem(
-            20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding
-        )
+        self.pbIter_0 = QPushButton(Importer)
+        self.pbIter_0.setObjectName("pbIter_0")
+        self.pbIter_0.setEnabled(True)
+        sizePolicy1.setHeightForWidth(self.pbIter_0.sizePolicy().hasHeightForWidth())
+        self.pbIter_0.setSizePolicy(sizePolicy1)
+        self.pbIter_0.setCheckable(False)
 
-        self.gridLayout.addItem(self.verticalSpacer, 27, 0, 1, 1)
+        self.gridLayout.addWidget(self.pbIter_0, 1, 0, 1, 1)
 
-        self.line_2 = QFrame(Importer)
-        self.line_2.setObjectName("line_2")
-        self.line_2.setFrameShape(QFrame.HLine)
-        self.line_2.setFrameShadow(QFrame.Sunken)
+        self.lbReloc_15 = QLabel(Importer)
+        self.lbReloc_15.setObjectName("lbReloc_15")
+        sizePolicy2.setHeightForWidth(self.lbReloc_15.sizePolicy().hasHeightForWidth())
+        self.lbReloc_15.setSizePolicy(sizePolicy2)
+        self.lbReloc_15.setFont(font)
+        self.lbReloc_15.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.line_2, 18, 0, 1, 3)
+        self.gridLayout.addWidget(self.lbReloc_15, 16, 2, 1, 1)
 
         self.lbIteration = QLabel(Importer)
         self.lbIteration.setObjectName("lbIteration")
         self.lbIteration.setFont(font)
-        self.lbIteration.setAlignment(Qt.AlignCenter)
+        self.lbIteration.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
         self.gridLayout.addWidget(self.lbIteration, 0, 0, 1, 1)
 
-        self.lbReloc_2 = QLabel(Importer)
-        self.lbReloc_2.setObjectName("lbReloc_2")
-        sizePolicy1.setHeightForWidth(self.lbReloc_2.sizePolicy().hasHeightForWidth())
-        self.lbReloc_2.setSizePolicy(sizePolicy1)
-        self.lbReloc_2.setFont(font)
-        self.lbReloc_2.setAlignment(Qt.AlignCenter)
+        self.pbIter_15 = QPushButton(Importer)
+        self.pbIter_15.setObjectName("pbIter_15")
+        self.pbIter_15.setEnabled(True)
+        sizePolicy1.setHeightForWidth(self.pbIter_15.sizePolicy().hasHeightForWidth())
+        self.pbIter_15.setSizePolicy(sizePolicy1)
+        self.pbIter_15.setCheckable(False)
 
-        self.gridLayout.addWidget(self.lbReloc_2, 3, 2, 1, 1)
+        self.gridLayout.addWidget(self.pbIter_15, 16, 0, 1, 1)
 
-        self.lbIter_3 = QLabel(Importer)
-        self.lbIter_3.setObjectName("lbIter_3")
-        self.lbIter_3.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_3.sizePolicy().hasHeightForWidth())
-        self.lbIter_3.setSizePolicy(sizePolicy1)
-        self.lbIter_3.setFont(font)
-        self.lbIter_3.setAlignment(Qt.AlignCenter)
+        self.lbReloc_13 = QLabel(Importer)
+        self.lbReloc_13.setObjectName("lbReloc_13")
+        sizePolicy2.setHeightForWidth(self.lbReloc_13.sizePolicy().hasHeightForWidth())
+        self.lbReloc_13.setSizePolicy(sizePolicy2)
+        self.lbReloc_13.setFont(font)
+        self.lbReloc_13.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbIter_3, 4, 1, 1, 1)
+        self.gridLayout.addWidget(self.lbReloc_13, 14, 2, 1, 1)
 
-        self.lbLastValidInfo = QLabel(Importer)
-        self.lbLastValidInfo.setObjectName("lbLastValidInfo")
+        self.lbReloc_8 = QLabel(Importer)
+        self.lbReloc_8.setObjectName("lbReloc_8")
+        sizePolicy2.setHeightForWidth(self.lbReloc_8.sizePolicy().hasHeightForWidth())
+        self.lbReloc_8.setSizePolicy(sizePolicy2)
+        self.lbReloc_8.setFont(font)
+        self.lbReloc_8.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbLastValidInfo, 20, 0, 1, 3)
+        self.gridLayout.addWidget(self.lbReloc_8, 9, 2, 1, 1)
 
-        self.lbReloc_4 = QLabel(Importer)
-        self.lbReloc_4.setObjectName("lbReloc_4")
-        sizePolicy1.setHeightForWidth(self.lbReloc_4.sizePolicy().hasHeightForWidth())
-        self.lbReloc_4.setSizePolicy(sizePolicy1)
-        self.lbReloc_4.setFont(font)
-        self.lbReloc_4.setAlignment(Qt.AlignCenter)
+        self.lbIter_4 = QLabel(Importer)
+        self.lbIter_4.setObjectName("lbIter_4")
+        self.lbIter_4.setEnabled(True)
+        sizePolicy2.setHeightForWidth(self.lbIter_4.sizePolicy().hasHeightForWidth())
+        self.lbIter_4.setSizePolicy(sizePolicy2)
+        self.lbIter_4.setFont(font)
+        self.lbIter_4.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbReloc_4, 5, 2, 1, 1)
+        self.gridLayout.addWidget(self.lbIter_4, 5, 1, 1, 1)
 
-        self.lbIter_12 = QLabel(Importer)
-        self.lbIter_12.setObjectName("lbIter_12")
-        self.lbIter_12.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_12.sizePolicy().hasHeightForWidth())
-        self.lbIter_12.setSizePolicy(sizePolicy1)
-        self.lbIter_12.setFont(font)
-        self.lbIter_12.setAlignment(Qt.AlignCenter)
+        self.line_2 = QFrame(Importer)
+        self.line_2.setObjectName("line_2")
+        self.line_2.setFrameShape(QFrame.Shape.HLine)
+        self.line_2.setFrameShadow(QFrame.Shadow.Sunken)
 
-        self.gridLayout.addWidget(self.lbIter_12, 13, 1, 1, 1)
+        self.gridLayout.addWidget(self.line_2, 18, 0, 1, 3)
 
-        self.pbIter_0 = QPushButton(Importer)
-        self.pbIter_0.setObjectName("pbIter_0")
-        self.pbIter_0.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_0.sizePolicy().hasHeightForWidth())
-        self.pbIter_0.setSizePolicy(sizePolicy2)
-        self.pbIter_0.setCheckable(False)
+        self.pbIter_6 = QPushButton(Importer)
+        self.pbIter_6.setObjectName("pbIter_6")
+        self.pbIter_6.setEnabled(True)
+        sizePolicy1.setHeightForWidth(self.pbIter_6.sizePolicy().hasHeightForWidth())
+        self.pbIter_6.setSizePolicy(sizePolicy1)
+        self.pbIter_6.setCheckable(False)
 
-        self.gridLayout.addWidget(self.pbIter_0, 1, 0, 1, 1)
+        self.gridLayout.addWidget(self.pbIter_6, 7, 0, 1, 1)
 
-        self.lbReloc_8 = QLabel(Importer)
-        self.lbReloc_8.setObjectName("lbReloc_8")
-        sizePolicy1.setHeightForWidth(self.lbReloc_8.sizePolicy().hasHeightForWidth())
-        self.lbReloc_8.setSizePolicy(sizePolicy1)
-        self.lbReloc_8.setFont(font)
-        self.lbReloc_8.setAlignment(Qt.AlignCenter)
+        self.lbReloc_9 = QLabel(Importer)
+        self.lbReloc_9.setObjectName("lbReloc_9")
+        sizePolicy2.setHeightForWidth(self.lbReloc_9.sizePolicy().hasHeightForWidth())
+        self.lbReloc_9.setSizePolicy(sizePolicy2)
+        self.lbReloc_9.setFont(font)
+        self.lbReloc_9.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbReloc_8, 9, 2, 1, 1)
+        self.gridLayout.addWidget(self.lbReloc_9, 10, 2, 1, 1)
 
         self.pbIter_14 = QPushButton(Importer)
         self.pbIter_14.setObjectName("pbIter_14")
         self.pbIter_14.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_14.sizePolicy().hasHeightForWidth())
-        self.pbIter_14.setSizePolicy(sizePolicy2)
+        sizePolicy1.setHeightForWidth(self.pbIter_14.sizePolicy().hasHeightForWidth())
+        self.pbIter_14.setSizePolicy(sizePolicy1)
         self.pbIter_14.setCheckable(False)
 
         self.gridLayout.addWidget(self.pbIter_14, 15, 0, 1, 1)
 
-        self.pbIter_2 = QPushButton(Importer)
-        self.pbIter_2.setObjectName("pbIter_2")
-        self.pbIter_2.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_2.sizePolicy().hasHeightForWidth())
-        self.pbIter_2.setSizePolicy(sizePolicy2)
-        self.pbIter_2.setCheckable(False)
-
-        self.gridLayout.addWidget(self.pbIter_2, 3, 0, 1, 1)
-
-        self.lbReloc_14 = QLabel(Importer)
-        self.lbReloc_14.setObjectName("lbReloc_14")
-        sizePolicy1.setHeightForWidth(self.lbReloc_14.sizePolicy().hasHeightForWidth())
-        self.lbReloc_14.setSizePolicy(sizePolicy1)
-        self.lbReloc_14.setFont(font)
-        self.lbReloc_14.setAlignment(Qt.AlignCenter)
+        self.lbIter_8 = QLabel(Importer)
+        self.lbIter_8.setObjectName("lbIter_8")
+        self.lbIter_8.setEnabled(True)
+        sizePolicy2.setHeightForWidth(self.lbIter_8.sizePolicy().hasHeightForWidth())
+        self.lbIter_8.setSizePolicy(sizePolicy2)
+        self.lbIter_8.setFont(font)
+        self.lbIter_8.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbReloc_14, 15, 2, 1, 1)
+        self.gridLayout.addWidget(self.lbIter_8, 9, 1, 1, 1)
 
-        self.pbIter_13 = QPushButton(Importer)
-        self.pbIter_13.setObjectName("pbIter_13")
-        self.pbIter_13.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_13.sizePolicy().hasHeightForWidth())
-        self.pbIter_13.setSizePolicy(sizePolicy2)
-        self.pbIter_13.setCheckable(False)
+        self.lbReloc_4 = QLabel(Importer)
+        self.lbReloc_4.setObjectName("lbReloc_4")
+        sizePolicy2.setHeightForWidth(self.lbReloc_4.sizePolicy().hasHeightForWidth())
+        self.lbReloc_4.setSizePolicy(sizePolicy2)
+        self.lbReloc_4.setFont(font)
+        self.lbReloc_4.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.pbIter_13, 14, 0, 1, 1)
+        self.gridLayout.addWidget(self.lbReloc_4, 5, 2, 1, 1)
 
-        self.lbReloc_1 = QLabel(Importer)
-        self.lbReloc_1.setObjectName("lbReloc_1")
-        sizePolicy1.setHeightForWidth(self.lbReloc_1.sizePolicy().hasHeightForWidth())
-        self.lbReloc_1.setSizePolicy(sizePolicy1)
-        self.lbReloc_1.setFont(font)
-        self.lbReloc_1.setAlignment(Qt.AlignCenter)
+        self.pbIter_9 = QPushButton(Importer)
+        self.pbIter_9.setObjectName("pbIter_9")
+        self.pbIter_9.setEnabled(True)
+        sizePolicy1.setHeightForWidth(self.pbIter_9.sizePolicy().hasHeightForWidth())
+        self.pbIter_9.setSizePolicy(sizePolicy1)
+        self.pbIter_9.setCheckable(False)
 
-        self.gridLayout.addWidget(self.lbReloc_1, 2, 2, 1, 1)
+        self.gridLayout.addWidget(self.pbIter_9, 10, 0, 1, 1)
 
-        self.lbReloc_9 = QLabel(Importer)
-        self.lbReloc_9.setObjectName("lbReloc_9")
-        sizePolicy1.setHeightForWidth(self.lbReloc_9.sizePolicy().hasHeightForWidth())
-        self.lbReloc_9.setSizePolicy(sizePolicy1)
-        self.lbReloc_9.setFont(font)
-        self.lbReloc_9.setAlignment(Qt.AlignCenter)
+        self.lbReloc_6 = QLabel(Importer)
+        self.lbReloc_6.setObjectName("lbReloc_6")
+        sizePolicy2.setHeightForWidth(self.lbReloc_6.sizePolicy().hasHeightForWidth())
+        self.lbReloc_6.setSizePolicy(sizePolicy2)
+        self.lbReloc_6.setFont(font)
+        self.lbReloc_6.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbReloc_9, 10, 2, 1, 1)
+        self.gridLayout.addWidget(self.lbReloc_6, 7, 2, 1, 1)
 
-        self.pbIter_11 = QPushButton(Importer)
-        self.pbIter_11.setObjectName("pbIter_11")
-        self.pbIter_11.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_11.sizePolicy().hasHeightForWidth())
-        self.pbIter_11.setSizePolicy(sizePolicy2)
-        self.pbIter_11.setCheckable(False)
+        self.lbReloc_3 = QLabel(Importer)
+        self.lbReloc_3.setObjectName("lbReloc_3")
+        sizePolicy2.setHeightForWidth(self.lbReloc_3.sizePolicy().hasHeightForWidth())
+        self.lbReloc_3.setSizePolicy(sizePolicy2)
+        self.lbReloc_3.setFont(font)
+        self.lbReloc_3.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.pbIter_11, 12, 0, 1, 1)
+        self.gridLayout.addWidget(self.lbReloc_3, 4, 2, 1, 1)
 
-        self.lbIter_15 = QLabel(Importer)
-        self.lbIter_15.setObjectName("lbIter_15")
-        self.lbIter_15.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_15.sizePolicy().hasHeightForWidth())
-        self.lbIter_15.setSizePolicy(sizePolicy1)
-        self.lbIter_15.setFont(font)
-        self.lbIter_15.setAlignment(Qt.AlignCenter)
+        self.lbReloc_12 = QLabel(Importer)
+        self.lbReloc_12.setObjectName("lbReloc_12")
+        sizePolicy2.setHeightForWidth(self.lbReloc_12.sizePolicy().hasHeightForWidth())
+        self.lbReloc_12.setSizePolicy(sizePolicy2)
+        self.lbReloc_12.setFont(font)
+        self.lbReloc_12.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbIter_15, 16, 1, 1, 1)
+        self.gridLayout.addWidget(self.lbReloc_12, 13, 2, 1, 1)
 
-        self.pbIter_10 = QPushButton(Importer)
-        self.pbIter_10.setObjectName("pbIter_10")
-        self.pbIter_10.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_10.sizePolicy().hasHeightForWidth())
-        self.pbIter_10.setSizePolicy(sizePolicy2)
-        self.pbIter_10.setCheckable(False)
+        self.lbDwellTime = QLabel(Importer)
+        self.lbDwellTime.setObjectName("lbDwellTime")
+        sizePolicy3 = QSizePolicy(
+            QSizePolicy.Policy.MinimumExpanding, QSizePolicy.Policy.Fixed
+        )
+        sizePolicy3.setHorizontalStretch(0)
+        sizePolicy3.setVerticalStretch(0)
+        sizePolicy3.setHeightForWidth(self.lbDwellTime.sizePolicy().hasHeightForWidth())
+        self.lbDwellTime.setSizePolicy(sizePolicy3)
 
-        self.gridLayout.addWidget(self.pbIter_10, 11, 0, 1, 1)
+        self.gridLayout.addWidget(self.lbDwellTime, 27, 0, 1, 1)
 
-        self.lbIter_11 = QLabel(Importer)
-        self.lbIter_11.setObjectName("lbIter_11")
-        self.lbIter_11.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_11.sizePolicy().hasHeightForWidth())
-        self.lbIter_11.setSizePolicy(sizePolicy1)
-        self.lbIter_11.setFont(font)
-        self.lbIter_11.setAlignment(Qt.AlignCenter)
+        self.buttonBox = QDialogButtonBox(Importer)
+        self.buttonBox.setObjectName("buttonBox")
+        self.buttonBox.setOrientation(Qt.Orientation.Horizontal)
+        self.buttonBox.setStandardButtons(
+            QDialogButtonBox.StandardButton.Cancel | QDialogButtonBox.StandardButton.Ok
+        )
 
-        self.gridLayout.addWidget(self.lbIter_11, 12, 1, 1, 1)
+        self.gridLayout.addWidget(self.buttonBox, 29, 0, 1, 3)
 
-        self.leDwellTime = QLineEdit(Importer)
-        self.leDwellTime.setObjectName("leDwellTime")
-        sizePolicy2.setHeightForWidth(self.leDwellTime.sizePolicy().hasHeightForWidth())
-        self.leDwellTime.setSizePolicy(sizePolicy2)
+        self.pbIter_13 = QPushButton(Importer)
+        self.pbIter_13.setObjectName("pbIter_13")
+        self.pbIter_13.setEnabled(True)
+        sizePolicy1.setHeightForWidth(self.pbIter_13.sizePolicy().hasHeightForWidth())
+        self.pbIter_13.setSizePolicy(sizePolicy1)
+        self.pbIter_13.setCheckable(False)
 
-        self.gridLayout.addWidget(self.leDwellTime, 26, 1, 1, 2)
+        self.gridLayout.addWidget(self.pbIter_13, 14, 0, 1, 1)
 
-        self.pbIter_3 = QPushButton(Importer)
-        self.pbIter_3.setObjectName("pbIter_3")
-        self.pbIter_3.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_3.sizePolicy().hasHeightForWidth())
-        self.pbIter_3.setSizePolicy(sizePolicy2)
-        self.pbIter_3.setCheckable(False)
+        self.lbIter_2 = QLabel(Importer)
+        self.lbIter_2.setObjectName("lbIter_2")
+        self.lbIter_2.setEnabled(True)
+        sizePolicy2.setHeightForWidth(self.lbIter_2.sizePolicy().hasHeightForWidth())
+        self.lbIter_2.setSizePolicy(sizePolicy2)
+        self.lbIter_2.setFont(font)
+        self.lbIter_2.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.pbIter_3, 4, 0, 1, 1)
+        self.gridLayout.addWidget(self.lbIter_2, 3, 1, 1, 1)
 
-        self.lbIter_4 = QLabel(Importer)
-        self.lbIter_4.setObjectName("lbIter_4")
-        self.lbIter_4.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_4.sizePolicy().hasHeightForWidth())
-        self.lbIter_4.setSizePolicy(sizePolicy1)
-        self.lbIter_4.setFont(font)
-        self.lbIter_4.setAlignment(Qt.AlignCenter)
+        self.pbIter_2 = QPushButton(Importer)
+        self.pbIter_2.setObjectName("pbIter_2")
+        self.pbIter_2.setEnabled(True)
+        sizePolicy1.setHeightForWidth(self.pbIter_2.sizePolicy().hasHeightForWidth())
+        self.pbIter_2.setSizePolicy(sizePolicy1)
+        self.pbIter_2.setCheckable(False)
 
-        self.gridLayout.addWidget(self.lbIter_4, 5, 1, 1, 1)
+        self.gridLayout.addWidget(self.pbIter_2, 3, 0, 1, 1)
 
         self.pbIter_4 = QPushButton(Importer)
         self.pbIter_4.setObjectName("pbIter_4")
         self.pbIter_4.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_4.sizePolicy().hasHeightForWidth())
-        self.pbIter_4.setSizePolicy(sizePolicy2)
+        sizePolicy1.setHeightForWidth(self.pbIter_4.sizePolicy().hasHeightForWidth())
+        self.pbIter_4.setSizePolicy(sizePolicy1)
         self.pbIter_4.setCheckable(False)
 
         self.gridLayout.addWidget(self.pbIter_4, 5, 0, 1, 1)
 
-        self.lbReloc = QLabel(Importer)
-        self.lbReloc.setObjectName("lbReloc")
-        self.lbReloc.setFont(font)
-        self.lbReloc.setAlignment(Qt.AlignCenter)
+        self.pbIter_1 = QPushButton(Importer)
+        self.pbIter_1.setObjectName("pbIter_1")
+        self.pbIter_1.setEnabled(True)
+        sizePolicy1.setHeightForWidth(self.pbIter_1.sizePolicy().hasHeightForWidth())
+        self.pbIter_1.setSizePolicy(sizePolicy1)
+        self.pbIter_1.setCheckable(False)
 
-        self.gridLayout.addWidget(self.lbReloc, 0, 2, 1, 1)
+        self.gridLayout.addWidget(self.pbIter_1, 2, 0, 1, 1)
 
-        self.pbIter_12 = QPushButton(Importer)
-        self.pbIter_12.setObjectName("pbIter_12")
-        self.pbIter_12.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_12.sizePolicy().hasHeightForWidth())
-        self.pbIter_12.setSizePolicy(sizePolicy2)
-        self.pbIter_12.setCheckable(False)
+        self.lbIter_5 = QLabel(Importer)
+        self.lbIter_5.setObjectName("lbIter_5")
+        self.lbIter_5.setEnabled(True)
+        sizePolicy2.setHeightForWidth(self.lbIter_5.sizePolicy().hasHeightForWidth())
+        self.lbIter_5.setSizePolicy(sizePolicy2)
+        self.lbIter_5.setFont(font)
+        self.lbIter_5.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.pbIter_12, 13, 0, 1, 1)
+        self.gridLayout.addWidget(self.lbIter_5, 6, 1, 1, 1)
+
+        self.pbIter_7 = QPushButton(Importer)
+        self.pbIter_7.setObjectName("pbIter_7")
+        self.pbIter_7.setEnabled(True)
+        sizePolicy1.setHeightForWidth(self.pbIter_7.sizePolicy().hasHeightForWidth())
+        self.pbIter_7.setSizePolicy(sizePolicy1)
+        self.pbIter_7.setCheckable(False)
+
+        self.gridLayout.addWidget(self.pbIter_7, 8, 0, 1, 1)
+
+        self.lbIter_10 = QLabel(Importer)
+        self.lbIter_10.setObjectName("lbIter_10")
+        self.lbIter_10.setEnabled(True)
+        sizePolicy2.setHeightForWidth(self.lbIter_10.sizePolicy().hasHeightForWidth())
+        self.lbIter_10.setSizePolicy(sizePolicy2)
+        self.lbIter_10.setFont(font)
+        self.lbIter_10.setAlignment(Qt.AlignmentFlag.AlignCenter)
+
+        self.gridLayout.addWidget(self.lbIter_10, 11, 1, 1, 1)
 
         self.lbIter_6 = QLabel(Importer)
         self.lbIter_6.setObjectName("lbIter_6")
         self.lbIter_6.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_6.sizePolicy().hasHeightForWidth())
-        self.lbIter_6.setSizePolicy(sizePolicy1)
+        sizePolicy2.setHeightForWidth(self.lbIter_6.sizePolicy().hasHeightForWidth())
+        self.lbIter_6.setSizePolicy(sizePolicy2)
         self.lbIter_6.setFont(font)
-        self.lbIter_6.setAlignment(Qt.AlignCenter)
+        self.lbIter_6.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
         self.gridLayout.addWidget(self.lbIter_6, 7, 1, 1, 1)
 
         self.pbIter_5 = QPushButton(Importer)
         self.pbIter_5.setObjectName("pbIter_5")
         self.pbIter_5.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_5.sizePolicy().hasHeightForWidth())
-        self.pbIter_5.setSizePolicy(sizePolicy2)
+        sizePolicy1.setHeightForWidth(self.pbIter_5.sizePolicy().hasHeightForWidth())
+        self.pbIter_5.setSizePolicy(sizePolicy1)
         self.pbIter_5.setCheckable(False)
 
         self.gridLayout.addWidget(self.pbIter_5, 6, 0, 1, 1)
 
-        self.pbIter_15 = QPushButton(Importer)
-        self.pbIter_15.setObjectName("pbIter_15")
-        self.pbIter_15.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_15.sizePolicy().hasHeightForWidth())
-        self.pbIter_15.setSizePolicy(sizePolicy2)
-        self.pbIter_15.setCheckable(False)
+        self.pbIter_12 = QPushButton(Importer)
+        self.pbIter_12.setObjectName("pbIter_12")
+        self.pbIter_12.setEnabled(True)
+        sizePolicy1.setHeightForWidth(self.pbIter_12.sizePolicy().hasHeightForWidth())
+        self.pbIter_12.setSizePolicy(sizePolicy1)
+        self.pbIter_12.setCheckable(False)
 
-        self.gridLayout.addWidget(self.pbIter_15, 16, 0, 1, 1)
+        self.gridLayout.addWidget(self.pbIter_12, 13, 0, 1, 1)
 
-        self.lbIter_1 = QLabel(Importer)
-        self.lbIter_1.setObjectName("lbIter_1")
-        self.lbIter_1.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_1.sizePolicy().hasHeightForWidth())
-        self.lbIter_1.setSizePolicy(sizePolicy1)
-        self.lbIter_1.setFont(font)
-        self.lbIter_1.setAlignment(Qt.AlignCenter)
+        self.lbReloc_0 = QLabel(Importer)
+        self.lbReloc_0.setObjectName("lbReloc_0")
+        sizePolicy2.setHeightForWidth(self.lbReloc_0.sizePolicy().hasHeightForWidth())
+        self.lbReloc_0.setSizePolicy(sizePolicy2)
+        self.lbReloc_0.setFont(font)
+        self.lbReloc_0.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbIter_1, 2, 1, 1, 1)
+        self.gridLayout.addWidget(self.lbReloc_0, 1, 2, 1, 1)
 
-        self.pb_last_valid = QPushButton(Importer)
-        self.pb_last_valid.setObjectName("pb_last_valid")
-        self.pb_last_valid.setCheckable(False)
+        self.lbReloc_10 = QLabel(Importer)
+        self.lbReloc_10.setObjectName("lbReloc_10")
+        sizePolicy2.setHeightForWidth(self.lbReloc_10.sizePolicy().hasHeightForWidth())
+        self.lbReloc_10.setSizePolicy(sizePolicy2)
+        self.lbReloc_10.setFont(font)
+        self.lbReloc_10.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.pb_last_valid, 19, 0, 1, 3)
+        self.gridLayout.addWidget(self.lbReloc_10, 11, 2, 1, 1)
+
+        self.lbIter_14 = QLabel(Importer)
+        self.lbIter_14.setObjectName("lbIter_14")
+        self.lbIter_14.setEnabled(True)
+        sizePolicy2.setHeightForWidth(self.lbIter_14.sizePolicy().hasHeightForWidth())
+        self.lbIter_14.setSizePolicy(sizePolicy2)
+        self.lbIter_14.setFont(font)
+        self.lbIter_14.setAlignment(Qt.AlignmentFlag.AlignCenter)
+
+        self.gridLayout.addWidget(self.lbIter_14, 15, 1, 1, 1)
+
+        self.lbReloc_14 = QLabel(Importer)
+        self.lbReloc_14.setObjectName("lbReloc_14")
+        sizePolicy2.setHeightForWidth(self.lbReloc_14.sizePolicy().hasHeightForWidth())
+        self.lbReloc_14.setSizePolicy(sizePolicy2)
+        self.lbReloc_14.setFont(font)
+        self.lbReloc_14.setAlignment(Qt.AlignmentFlag.AlignCenter)
+
+        self.gridLayout.addWidget(self.lbReloc_14, 15, 2, 1, 1)
+
+        self.lbReloc_1 = QLabel(Importer)
+        self.lbReloc_1.setObjectName("lbReloc_1")
+        sizePolicy2.setHeightForWidth(self.lbReloc_1.sizePolicy().hasHeightForWidth())
+        self.lbReloc_1.setSizePolicy(sizePolicy2)
+        self.lbReloc_1.setFont(font)
+        self.lbReloc_1.setAlignment(Qt.AlignmentFlag.AlignCenter)
+
+        self.gridLayout.addWidget(self.lbReloc_1, 2, 2, 1, 1)
+
+        self.verticalSpacer_2 = QSpacerItem(
+            20, 20, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding
+        )
+
+        self.gridLayout.addItem(self.verticalSpacer_2, 17, 0, 1, 1)
+
+        self.verticalSpacer = QSpacerItem(
+            20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding
+        )
+
+        self.gridLayout.addItem(self.verticalSpacer, 28, 0, 1, 1)
 
         self.lbIter_9 = QLabel(Importer)
         self.lbIter_9.setObjectName("lbIter_9")
         self.lbIter_9.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_9.sizePolicy().hasHeightForWidth())
-        self.lbIter_9.setSizePolicy(sizePolicy1)
+        sizePolicy2.setHeightForWidth(self.lbIter_9.sizePolicy().hasHeightForWidth())
+        self.lbIter_9.setSizePolicy(sizePolicy2)
         self.lbIter_9.setFont(font)
-        self.lbIter_9.setAlignment(Qt.AlignCenter)
+        self.lbIter_9.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
         self.gridLayout.addWidget(self.lbIter_9, 10, 1, 1, 1)
 
-        self.pbIter_1 = QPushButton(Importer)
-        self.pbIter_1.setObjectName("pbIter_1")
-        self.pbIter_1.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_1.sizePolicy().hasHeightForWidth())
-        self.pbIter_1.setSizePolicy(sizePolicy2)
-        self.pbIter_1.setCheckable(False)
+        self.line = QFrame(Importer)
+        self.line.setObjectName("line")
+        self.line.setFrameShape(QFrame.Shape.HLine)
+        self.line.setFrameShadow(QFrame.Shadow.Sunken)
 
-        self.gridLayout.addWidget(self.pbIter_1, 2, 0, 1, 1)
+        self.gridLayout.addWidget(self.line, 24, 0, 1, 3)
 
-        self.lbReloc_13 = QLabel(Importer)
-        self.lbReloc_13.setObjectName("lbReloc_13")
-        sizePolicy1.setHeightForWidth(self.lbReloc_13.sizePolicy().hasHeightForWidth())
-        self.lbReloc_13.setSizePolicy(sizePolicy1)
-        self.lbReloc_13.setFont(font)
-        self.lbReloc_13.setAlignment(Qt.AlignCenter)
+        self.lbIter_12 = QLabel(Importer)
+        self.lbIter_12.setObjectName("lbIter_12")
+        self.lbIter_12.setEnabled(True)
+        sizePolicy2.setHeightForWidth(self.lbIter_12.sizePolicy().hasHeightForWidth())
+        self.lbIter_12.setSizePolicy(sizePolicy2)
+        self.lbIter_12.setFont(font)
+        self.lbIter_12.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbReloc_13, 14, 2, 1, 1)
+        self.gridLayout.addWidget(self.lbIter_12, 13, 1, 1, 1)
 
-        self.pbIter_9 = QPushButton(Importer)
-        self.pbIter_9.setObjectName("pbIter_9")
-        self.pbIter_9.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.pbIter_9.sizePolicy().hasHeightForWidth())
-        self.pbIter_9.setSizePolicy(sizePolicy2)
-        self.pbIter_9.setCheckable(False)
+        self.lbReloc_2 = QLabel(Importer)
+        self.lbReloc_2.setObjectName("lbReloc_2")
+        sizePolicy2.setHeightForWidth(self.lbReloc_2.sizePolicy().hasHeightForWidth())
+        self.lbReloc_2.setSizePolicy(sizePolicy2)
+        self.lbReloc_2.setFont(font)
+        self.lbReloc_2.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.pbIter_9, 10, 0, 1, 1)
+        self.gridLayout.addWidget(self.lbReloc_2, 3, 2, 1, 1)
 
-        self.lbDwellTime = QLabel(Importer)
-        self.lbDwellTime.setObjectName("lbDwellTime")
-        sizePolicy3 = QSizePolicy(
-            QSizePolicy.Policy.MinimumExpanding, QSizePolicy.Policy.Fixed
-        )
-        sizePolicy3.setHorizontalStretch(0)
-        sizePolicy3.setVerticalStretch(0)
-        sizePolicy3.setHeightForWidth(self.lbDwellTime.sizePolicy().hasHeightForWidth())
-        self.lbDwellTime.setSizePolicy(sizePolicy3)
+        self.lbReloc_7 = QLabel(Importer)
+        self.lbReloc_7.setObjectName("lbReloc_7")
+        sizePolicy2.setHeightForWidth(self.lbReloc_7.sizePolicy().hasHeightForWidth())
+        self.lbReloc_7.setSizePolicy(sizePolicy2)
+        self.lbReloc_7.setFont(font)
+        self.lbReloc_7.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbDwellTime, 26, 0, 1, 1)
+        self.gridLayout.addWidget(self.lbReloc_7, 8, 2, 1, 1)
 
-        self.lbReloc_12 = QLabel(Importer)
-        self.lbReloc_12.setObjectName("lbReloc_12")
-        sizePolicy1.setHeightForWidth(self.lbReloc_12.sizePolicy().hasHeightForWidth())
-        self.lbReloc_12.setSizePolicy(sizePolicy1)
-        self.lbReloc_12.setFont(font)
-        self.lbReloc_12.setAlignment(Qt.AlignCenter)
+        self.lbIter_1 = QLabel(Importer)
+        self.lbIter_1.setObjectName("lbIter_1")
+        self.lbIter_1.setEnabled(True)
+        sizePolicy2.setHeightForWidth(self.lbIter_1.sizePolicy().hasHeightForWidth())
+        self.lbIter_1.setSizePolicy(sizePolicy2)
+        self.lbIter_1.setFont(font)
+        self.lbIter_1.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbReloc_12, 13, 2, 1, 1)
+        self.gridLayout.addWidget(self.lbIter_1, 2, 1, 1, 1)
+
+        self.lbLastValidInfo = QLabel(Importer)
+        self.lbLastValidInfo.setObjectName("lbLastValidInfo")
+
+        self.gridLayout.addWidget(self.lbLastValidInfo, 20, 0, 1, 3)
+
+        self.lbCFRValues = QLabel(Importer)
+        self.lbCFRValues.setObjectName("lbCFRValues")
+        self.lbCFRValues.setFont(font)
+        self.lbCFRValues.setAlignment(Qt.AlignmentFlag.AlignCenter)
+
+        self.gridLayout.addWidget(self.lbCFRValues, 0, 1, 1, 1)
+
+        self.cbTracking = QCheckBox(Importer)
+        self.cbTracking.setObjectName("cbTracking")
+
+        self.gridLayout.addWidget(self.cbTracking, 25, 0, 1, 1)
+
+        self.lbIter_15 = QLabel(Importer)
+        self.lbIter_15.setObjectName("lbIter_15")
+        self.lbIter_15.setEnabled(True)
+        sizePolicy2.setHeightForWidth(self.lbIter_15.sizePolicy().hasHeightForWidth())
+        self.lbIter_15.setSizePolicy(sizePolicy2)
+        self.lbIter_15.setFont(font)
+        self.lbIter_15.setAlignment(Qt.AlignmentFlag.AlignCenter)
+
+        self.gridLayout.addWidget(self.lbIter_15, 16, 1, 1, 1)
+
+        self.lbIter_3 = QLabel(Importer)
+        self.lbIter_3.setObjectName("lbIter_3")
+        self.lbIter_3.setEnabled(True)
+        sizePolicy2.setHeightForWidth(self.lbIter_3.sizePolicy().hasHeightForWidth())
+        self.lbIter_3.setSizePolicy(sizePolicy2)
+        self.lbIter_3.setFont(font)
+        self.lbIter_3.setAlignment(Qt.AlignmentFlag.AlignCenter)
+
+        self.gridLayout.addWidget(self.lbIter_3, 4, 1, 1, 1)
+
+        self.lbIter_11 = QLabel(Importer)
+        self.lbIter_11.setObjectName("lbIter_11")
+        self.lbIter_11.setEnabled(True)
+        sizePolicy2.setHeightForWidth(self.lbIter_11.sizePolicy().hasHeightForWidth())
+        self.lbIter_11.setSizePolicy(sizePolicy2)
+        self.lbIter_11.setFont(font)
+        self.lbIter_11.setAlignment(Qt.AlignmentFlag.AlignCenter)
+
+        self.gridLayout.addWidget(self.lbIter_11, 12, 1, 1, 1)
 
         self.lbIter_7 = QLabel(Importer)
         self.lbIter_7.setObjectName("lbIter_7")
         self.lbIter_7.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_7.sizePolicy().hasHeightForWidth())
-        self.lbIter_7.setSizePolicy(sizePolicy1)
+        sizePolicy2.setHeightForWidth(self.lbIter_7.sizePolicy().hasHeightForWidth())
+        self.lbIter_7.setSizePolicy(sizePolicy2)
         self.lbIter_7.setFont(font)
-        self.lbIter_7.setAlignment(Qt.AlignCenter)
+        self.lbIter_7.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
         self.gridLayout.addWidget(self.lbIter_7, 8, 1, 1, 1)
 
-        self.lbReloc_5 = QLabel(Importer)
-        self.lbReloc_5.setObjectName("lbReloc_5")
-        sizePolicy1.setHeightForWidth(self.lbReloc_5.sizePolicy().hasHeightForWidth())
-        self.lbReloc_5.setSizePolicy(sizePolicy1)
-        self.lbReloc_5.setFont(font)
-        self.lbReloc_5.setAlignment(Qt.AlignCenter)
-
-        self.gridLayout.addWidget(self.lbReloc_5, 6, 2, 1, 1)
-
-        self.lbReloc_11 = QLabel(Importer)
-        self.lbReloc_11.setObjectName("lbReloc_11")
-        sizePolicy1.setHeightForWidth(self.lbReloc_11.sizePolicy().hasHeightForWidth())
-        self.lbReloc_11.setSizePolicy(sizePolicy1)
-        self.lbReloc_11.setFont(font)
-        self.lbReloc_11.setAlignment(Qt.AlignCenter)
+        self.pb_last_valid = QPushButton(Importer)
+        self.pb_last_valid.setObjectName("pb_last_valid")
+        self.pb_last_valid.setCheckable(False)
 
-        self.gridLayout.addWidget(self.lbReloc_11, 12, 2, 1, 1)
+        self.gridLayout.addWidget(self.pb_last_valid, 19, 0, 1, 3)
 
-        self.lbReloc_7 = QLabel(Importer)
-        self.lbReloc_7.setObjectName("lbReloc_7")
-        sizePolicy1.setHeightForWidth(self.lbReloc_7.sizePolicy().hasHeightForWidth())
-        self.lbReloc_7.setSizePolicy(sizePolicy1)
-        self.lbReloc_7.setFont(font)
-        self.lbReloc_7.setAlignment(Qt.AlignCenter)
+        self.lbIter_13 = QLabel(Importer)
+        self.lbIter_13.setObjectName("lbIter_13")
+        self.lbIter_13.setEnabled(True)
+        sizePolicy2.setHeightForWidth(self.lbIter_13.sizePolicy().hasHeightForWidth())
+        self.lbIter_13.setSizePolicy(sizePolicy2)
+        self.lbIter_13.setFont(font)
+        self.lbIter_13.setAlignment(Qt.AlignmentFlag.AlignCenter)
 
-        self.gridLayout.addWidget(self.lbReloc_7, 8, 2, 1, 1)
+        self.gridLayout.addWidget(self.lbIter_13, 14, 1, 1, 1)
 
-        self.lbIter_2 = QLabel(Importer)
-        self.lbIter_2.setObjectName("lbIter_2")
-        self.lbIter_2.setEnabled(True)
-        sizePolicy1.setHeightForWidth(self.lbIter_2.sizePolicy().hasHeightForWidth())
-        self.lbIter_2.setSizePolicy(sizePolicy1)
-        self.lbIter_2.setFont(font)
-        self.lbIter_2.setAlignment(Qt.AlignCenter)
+        self.leDwellTime = QLineEdit(Importer)
+        self.leDwellTime.setObjectName("leDwellTime")
+        sizePolicy1.setHeightForWidth(self.leDwellTime.sizePolicy().hasHeightForWidth())
+        self.leDwellTime.setSizePolicy(sizePolicy1)
 
-        self.gridLayout.addWidget(self.lbIter_2, 3, 1, 1, 1)
+        self.gridLayout.addWidget(self.leDwellTime, 27, 1, 1, 2)
 
         self.fixedVerticalSpacer = QSpacerItem(
             20, 20, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Fixed
         )
 
         self.gridLayout.addItem(self.fixedVerticalSpacer, 22, 0, 1, 1)
 
-        self.lbReloc_10 = QLabel(Importer)
-        self.lbReloc_10.setObjectName("lbReloc_10")
-        sizePolicy1.setHeightForWidth(self.lbReloc_10.sizePolicy().hasHeightForWidth())
-        self.lbReloc_10.setSizePolicy(sizePolicy1)
-        self.lbReloc_10.setFont(font)
-        self.lbReloc_10.setAlignment(Qt.AlignCenter)
+        self.pbIter_11 = QPushButton(Importer)
+        self.pbIter_11.setObjectName("pbIter_11")
+        self.pbIter_11.setEnabled(True)
+        sizePolicy1.setHeightForWidth(self.pbIter_11.sizePolicy().hasHeightForWidth())
+        self.pbIter_11.setSizePolicy(sizePolicy1)
+        self.pbIter_11.setCheckable(False)
 
-        self.gridLayout.addWidget(self.lbReloc_10, 11, 2, 1, 1)
+        self.gridLayout.addWidget(self.pbIter_11, 12, 0, 1, 1)
 
-        self.verticalSpacer_2 = QSpacerItem(
-            20, 20, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding
-        )
+        self.cbPoolDCR = QCheckBox(Importer)
+        self.cbPoolDCR.setObjectName("cbPoolDCR")
 
-        self.gridLayout.addItem(self.verticalSpacer_2, 17, 0, 1, 1)
+        self.gridLayout.addWidget(self.cbPoolDCR, 26, 0, 1, 3)
 
         self.retranslateUi(Importer)
         self.buttonBox.accepted.connect(Importer.accept)
         self.buttonBox.rejected.connect(Importer.reject)
 
         QMetaObject.connectSlotsByName(Importer)
 
     # setupUi
 
     def retranslateUi(self, Importer):
         Importer.setWindowTitle(
             QCoreApplication.translate("Importer", "Importer", None)
         )
-        self.lbIter_13.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbReloc_0.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbReloc_15.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.pbIter_7.setText(
-            QCoreApplication.translate("Importer", "Iteration 7", None)
-        )
-        self.lbIter_5.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.cbTracking.setText(
-            QCoreApplication.translate("Importer", "Tracking dataset", None)
-        )
-        self.lbIter_8.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbReloc_6.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbCFRValues.setText(
-            QCoreApplication.translate("Importer", "CFR values", None)
-        )
         self.lbRelocInfo.setText(
             QCoreApplication.translate(
                 "Importer",
                 "Non-relocalized iterations contain one valid measurement per trace.",
                 None,
             )
         )
         self.pbIter_8.setText(
             QCoreApplication.translate("Importer", "Iteration 8", None)
         )
-        self.lbReloc_3.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbIter_14.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbIter_0.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbIter_10.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.pbIter_6.setText(
-            QCoreApplication.translate("Importer", "Iteration 6", None)
+        self.pbIter_3.setText(
+            QCoreApplication.translate("Importer", "Iteration 3", None)
         )
-        self.lbIteration.setText(
-            QCoreApplication.translate("Importer", "Iteration number", None)
+        self.pbIter_10.setText(
+            QCoreApplication.translate("Importer", "Iteration 10", None)
         )
-        self.lbReloc_2.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbIter_3.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbLastValidInfo.setText(
-            QCoreApplication.translate(
-                "Importer", 'Only "last valid" iteration can be saved.', None
-            )
+        self.lbReloc.setText(
+            QCoreApplication.translate("Importer", "Relocalized", None)
         )
-        self.lbReloc_4.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbIter_12.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbReloc_11.setText(QCoreApplication.translate("Importer", "\u2713", None))
+        self.lbReloc_5.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbIter_0.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
         self.pbIter_0.setText(
             QCoreApplication.translate("Importer", "Iteration 0", None)
         )
+        self.lbReloc_15.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbIteration.setText(
+            QCoreApplication.translate("Importer", "Iteration number", None)
+        )
+        self.pbIter_15.setText(
+            QCoreApplication.translate("Importer", "Iteration 15", None)
+        )
+        self.lbReloc_13.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
         self.lbReloc_8.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbIter_4.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.pbIter_6.setText(
+            QCoreApplication.translate("Importer", "Iteration 6", None)
+        )
+        self.lbReloc_9.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
         self.pbIter_14.setText(
             QCoreApplication.translate("Importer", "Iteration 14", None)
         )
-        self.pbIter_2.setText(
-            QCoreApplication.translate("Importer", "Iteration 2", None)
+        self.lbIter_8.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbReloc_4.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.pbIter_9.setText(
+            QCoreApplication.translate("Importer", "Iteration 9", None)
+        )
+        self.lbReloc_6.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbReloc_3.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbReloc_12.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbDwellTime.setText(
+            QCoreApplication.translate("Importer", "Dwell time (ms)", None)
         )
-        self.lbReloc_14.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
         self.pbIter_13.setText(
             QCoreApplication.translate("Importer", "Iteration 13", None)
         )
-        self.lbReloc_1.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbReloc_9.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.pbIter_11.setText(
-            QCoreApplication.translate("Importer", "Iteration 11", None)
-        )
-        self.lbIter_15.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.pbIter_10.setText(
-            QCoreApplication.translate("Importer", "Iteration 10", None)
-        )
-        self.lbIter_11.setText(QCoreApplication.translate("Importer", "\u2713", None))
-        self.pbIter_3.setText(
-            QCoreApplication.translate("Importer", "Iteration 3", None)
+        self.lbIter_2.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.pbIter_2.setText(
+            QCoreApplication.translate("Importer", "Iteration 2", None)
         )
-        self.lbIter_4.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
         self.pbIter_4.setText(
             QCoreApplication.translate("Importer", "Iteration 4", None)
         )
-        self.lbReloc.setText(
-            QCoreApplication.translate("Importer", "Relocalized", None)
+        self.pbIter_1.setText(
+            QCoreApplication.translate("Importer", "Iteration 1", None)
         )
-        self.pbIter_12.setText(
-            QCoreApplication.translate("Importer", "Iteration 12", None)
+        self.lbIter_5.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.pbIter_7.setText(
+            QCoreApplication.translate("Importer", "Iteration 7", None)
         )
+        self.lbIter_10.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
         self.lbIter_6.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
         self.pbIter_5.setText(
             QCoreApplication.translate("Importer", "Iteration 5", None)
         )
-        self.pbIter_15.setText(
-            QCoreApplication.translate("Importer", "Iteration 15", None)
+        self.pbIter_12.setText(
+            QCoreApplication.translate("Importer", "Iteration 12", None)
         )
+        self.lbReloc_0.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbReloc_10.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbIter_14.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbReloc_14.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbReloc_1.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbIter_9.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbIter_12.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbReloc_2.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbReloc_7.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
         self.lbIter_1.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbLastValidInfo.setText(
+            QCoreApplication.translate(
+                "Importer", 'Only "last valid" iteration can be saved.', None
+            )
+        )
+        self.lbCFRValues.setText(
+            QCoreApplication.translate("Importer", "CFR values", None)
+        )
+        self.cbTracking.setText(
+            QCoreApplication.translate("Importer", "Tracking dataset", None)
+        )
+        self.lbIter_15.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbIter_3.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.lbIter_11.setText(QCoreApplication.translate("Importer", "\u2713", None))
+        self.lbIter_7.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
         self.pb_last_valid.setText(
             QCoreApplication.translate("Importer", "Pick last valid iteration", None)
         )
-        self.lbIter_9.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.pbIter_1.setText(
-            QCoreApplication.translate("Importer", "Iteration 1", None)
-        )
-        self.lbReloc_13.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.pbIter_9.setText(
-            QCoreApplication.translate("Importer", "Iteration 9", None)
+        self.lbIter_13.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
+        self.pbIter_11.setText(
+            QCoreApplication.translate("Importer", "Iteration 11", None)
         )
-        self.lbDwellTime.setText(
-            QCoreApplication.translate("Importer", "Dwell time (ms)", None)
+        self.cbPoolDCR.setText(
+            QCoreApplication.translate(
+                "Importer", "Pool DCR values (ECO-weighted)", None
+            )
         )
-        self.lbReloc_12.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbIter_7.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbReloc_5.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbReloc_11.setText(QCoreApplication.translate("Importer", "\u2713", None))
-        self.lbReloc_7.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbIter_2.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
-        self.lbReloc_10.setText(QCoreApplication.translate("Importer", "\u2a2f", None))
 
     # retranslateUi
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/ui_main_window.py` & `pyminflux-0.4.1/pyminflux/ui/ui_main_window.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/ui_options.py` & `pyminflux-0.4.1/pyminflux/ui/ui_options.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/ui_plotter_toolbar.py` & `pyminflux-0.4.1/pyminflux/ui/ui_plotter_toolbar.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/ui_roi_ranges.py` & `pyminflux-0.4.1/pyminflux/ui/ui_roi_ranges.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/ui_time_inspector.py` & `pyminflux-0.4.1/pyminflux/ui/ui_time_inspector.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/ui_trace_stats_viewer.py` & `pyminflux-0.4.1/pyminflux/ui/ui_trace_stats_viewer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/ui_wizard.py` & `pyminflux-0.4.1/pyminflux/ui/ui_wizard.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/ui/wizard.py` & `pyminflux-0.4.1/pyminflux/ui/wizard.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,40 +11,41 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 from pathlib import Path
 
+import numpy as np
 from PySide6.QtCore import QSignalBlocker, Qt, Signal, Slot
 from PySide6.QtGui import QDoubleValidator
 from PySide6.QtWidgets import QDialog, QMessageBox
 
 from pyminflux.state import State
 
 from ..analysis import prepare_histogram
 from ..utils import intersect_2d_ranges
 from .ui_wizard import Ui_WizardDialog
 
 
 class WizardDialog(QDialog, Ui_WizardDialog):
-    load_data_triggered = Signal(None, name="load_data_triggered")
-    load_filename_triggered = Signal(str, name="load_filename_triggered")
-    save_data_triggered = Signal(None, name="save_data_triggered")
-    reset_filters_triggered = Signal(None, name="reset_filters_triggered")
-    open_unmixer_triggered = Signal(None, name="open_unmixer_triggered")
-    open_time_inspector_triggered = Signal(None, name="open_time_inspector_triggered")
-    open_analyzer_triggered = Signal(None, name="open_analyzer_triggered")
-    fluorophore_id_changed = Signal(int, name="fluorophore_id_changed")
-    request_fluorophore_ids_reset = Signal(None, name="request_fluorophore_ids_reset")
-    efo_bounds_modified = Signal(None, name="efo_bounds_modified")
-    cfr_bounds_modified = Signal(None, name="cfr_bounds_modified")
-    cfr_robust_threshold_modified = Signal(float, name="cfr_robust_threshold_modified ")
-    wizard_filters_run = Signal(None, name="wizard_filters_run")
-    export_data_triggered = Signal(None, name="export_data_triggered")
+    load_data_triggered = Signal()
+    load_filename_triggered = Signal(str)
+    save_data_triggered = Signal()
+    reset_filters_triggered = Signal()
+    open_unmixer_triggered = Signal()
+    open_time_inspector_triggered = Signal()
+    open_analyzer_triggered = Signal()
+    fluorophore_id_changed = Signal(int)
+    request_fluorophore_ids_reset = Signal()
+    efo_bounds_modified = Signal()
+    cfr_bounds_modified = Signal()
+    cfr_robust_threshold_modified = Signal(float)
+    wizard_filters_run = Signal()
+    export_data_triggered = Signal()
 
     def __init__(self, parent=None):
         """Constructor."""
 
         # Call the base class
         super().__init__()
 
@@ -70,21 +71,29 @@
             "leEFOUpperBound": True,
             "leCFRLowerBound": True,
             "leCFRUpperBound": True,
         }
 
         # Fill the fields
         self.ui.leEFOLowerBound.setText("")
-        self.ui.leEFOLowerBound.setValidator(QDoubleValidator(decimals=0))
+        self.ui.leEFOLowerBound.setValidator(
+            QDoubleValidator(bottom=-np.Inf, top=np.Inf, decimals=0)
+        )
         self.ui.leEFOUpperBound.setText("")
-        self.ui.leEFOUpperBound.setValidator(QDoubleValidator(decimals=0))
+        self.ui.leEFOUpperBound.setValidator(
+            QDoubleValidator(bottom=-np.Inf, top=np.Inf, decimals=0)
+        )
         self.ui.leCFRLowerBound.setText("")
-        self.ui.leCFRLowerBound.setValidator(QDoubleValidator(decimals=2))
+        self.ui.leCFRLowerBound.setValidator(
+            QDoubleValidator(bottom=-np.Inf, top=np.Inf, decimals=2)
+        )
         self.ui.leCFRUpperBound.setText("")
-        self.ui.leCFRUpperBound.setValidator(QDoubleValidator(decimals=2))
+        self.ui.leCFRUpperBound.setValidator(
+            QDoubleValidator(bottom=-np.Inf, top=np.Inf, decimals=2)
+        )
 
         # Set up connections
         self.setup_conn()
 
     def dragEnterEvent(self, event):
         """Process drag events. Ignore drag events that are not file paths."""
 
@@ -185,23 +194,23 @@
 
         if self.processor is None or len(self.processor.filtered_dataframe.index) == 0:
             return
 
         # Get the range for the EFO data
         if self.state.efo_thresholds is None:
             _, efo_bin_edges, _, _ = prepare_histogram(
-                self.processor.filtered_dataframe["efo"].values,
+                self.processor.filtered_dataframe["efo"].to_numpy(),
                 auto_bins=self.state.efo_bin_size_hz == 0,
                 bin_size=self.state.efo_bin_size_hz,
             )
             self.state.efo_thresholds = (efo_bin_edges[0], efo_bin_edges[-1])
 
         # Get the range for the CFR data
         _, cfr_bin_edges, _, _ = prepare_histogram(
-            self.processor.filtered_dataframe["cfr"].values,
+            self.processor.filtered_dataframe["cfr"].to_numpy(),
             auto_bins=True,
             bin_size=0.0,
         )
         self.state.cfr_thresholds = (cfr_bin_edges[0], cfr_bin_edges[-1])
 
         # Set the filter ranges from {efo|cfr}_thresholds
         self.set_filter_ranges_from_state()
@@ -283,15 +292,15 @@
 
         # Reset the fluorophore ID assignment
         self.request_fluorophore_ids_reset.emit()
 
         # Update the color selection combo box
         self.set_fluorophore_list(1)
 
-    @Slot(int, name="set_fluorophore_list")
+    @Slot(int)
     def set_fluorophore_list(self, num_fluorophores):
         """Update the fluorophores pull-down menu."""
 
         # Signal blocker on self.efo_cfr_roi
         blocker = QSignalBlocker(self.ui.cmActiveColor)
 
         # Block signals from the combo box
@@ -311,69 +320,81 @@
         # Release the blocker
         blocker.unblock()
 
         # Fall back to no fluorophore id selected.
         # This is allowed to signal.
         self.ui.cmActiveColor.setCurrentIndex(0)
 
-    @Slot(int, name="fluorophore_index_changed")
+    @Slot(int)
     def fluorophore_index_changed(self, index):
         """Emit a signal informing that the fluorophore id has changed."""
 
         # If the items have just been added, the index will be -1
         if index == -1:
             return
 
         # The fluorophore index is 1 + the combobox current index
         self.fluorophore_id_changed.emit(index)
 
-    @Slot(None, name="change_efo_bounds")
+    @Slot()
     def change_efo_bounds(self):
         """Update the EFO bounds."""
 
+        if self.state.efo_thresholds is None:
+            raise Exception("self.state.efo_thresholds is None!")
+
         # Block signals from self.ui.leEFOLowerBound and self.ui.leEFOUpperBound
         efo_lower_bound_blocker = QSignalBlocker(self.ui.leEFOLowerBound)
         efo_upper_bound_blocker = QSignalBlocker(self.ui.leEFOUpperBound)
         efo_lower_bound_blocker.reblock()
         efo_upper_bound_blocker.reblock()
 
         # Update the thresholds for the EFO histogram.
         self.ui.leEFOLowerBound.setText(f"{self.state.efo_thresholds[0]:.0f}")
         self.ui.leEFOUpperBound.setText(f"{self.state.efo_thresholds[1]:.0f}")
 
         # Unblock the signals
         efo_lower_bound_blocker.unblock()
         efo_upper_bound_blocker.unblock()
 
-    @Slot(None, name="change_cfr_bounds")
+    @Slot()
     def change_cfr_bounds(self):
         """Update the CFR bounds."""
 
+        if self.state.cfr_thresholds is None:
+            raise Exception("self.state.cfr_thresholds is None!")
+
         # Block signals from self.ui.leEFOLowerBound and self.ui.leEFOUpperBound
         cfr_lower_bound_blocker = QSignalBlocker(self.ui.leCFRLowerBound)
         cfr_upper_bound_blocker = QSignalBlocker(self.ui.leCFRUpperBound)
         cfr_lower_bound_blocker.reblock()
         cfr_upper_bound_blocker.reblock()
 
         # Update the thresholds for the CFR histogram.
         self.ui.leCFRLowerBound.setText(f"{self.state.cfr_thresholds[0]:.2f}")
         self.ui.leCFRUpperBound.setText(f"{self.state.cfr_thresholds[1]:.2f}")
 
         # Unblock the signals
         cfr_lower_bound_blocker.unblock()
         cfr_upper_bound_blocker.unblock()
 
-    @Slot(None, name="run_efo_filter_and_broadcast")
+    @Slot()
     def run_efo_filter_and_broadcast(self):
         """Run the EFO filter and broadcast the changes."""
 
+        if self.processor is None:
+            return
+
         # Make sure that we have valid bounds
         if not (self.valid["leEFOLowerBound"] and self.valid["leEFOUpperBound"]):
             return
 
+        if self.state.efo_thresholds is None:
+            raise Exception("self.state.efo_thresholds is None!")
+
         # Apply the EFO filter if needed
         if self.state.efo_thresholds is not None:
             self.processor.filter_by_1d_range(
                 "efo", (self.state.efo_thresholds[0], self.state.efo_thresholds[1])
             )
 
         # Update State.applied_efo_thresholds
@@ -383,22 +404,28 @@
             self.state.applied_efo_thresholds = intersect_2d_ranges(
                 self.state.efo_thresholds, self.state.applied_efo_thresholds
             )
 
         # Signal that the external viewers should be updated
         self.wizard_filters_run.emit()
 
-    @Slot(None, name="run_cfr_filter_and_broadcast")
+    @Slot()
     def run_cfr_filter_and_broadcast(self):
         """Run the CFR filter and broadcast the changes."""
 
+        if self.processor is None:
+            return
+
         # Make sure that we have valid bounds
         if not (self.valid["leCFRLowerBound"] and self.valid["leCFRUpperBound"]):
             return
 
+        if self.state.cfr_thresholds is None:
+            raise Exception("self.state.cfr_thresholds is None!")
+
         # Apply the CFR filter if needed
         if self.state.cfr_thresholds is not None:
             self.processor.filter_by_1d_range(
                 "cfr", (self.state.cfr_thresholds[0], self.state.cfr_thresholds[1])
             )
 
         # Update State.applied_cfr_thresholds
@@ -408,15 +435,15 @@
             self.state.applied_cfr_thresholds = intersect_2d_ranges(
                 self.state.cfr_thresholds, self.state.applied_cfr_thresholds
             )
 
         # Signal that the external viewers should be updated
         self.wizard_filters_run.emit()
 
-    @Slot(None, name="efo_change_bounds_and_broadcast")
+    @Slot()
     def efo_change_bounds_and_broadcast(self, text):
         """Update the EFO bounds and broadcast changes."""
 
         # Initialize the status to valid
         self.valid["leEFOLowerBound"] = True
         self.valid["leEFOUpperBound"] = True
 
@@ -457,15 +484,15 @@
         if self.valid["leEFOLowerBound"] and self.valid["leEFOUpperBound"]:
             # Broadcast
             self.efo_bounds_modified.emit()
         else:
             # Disable the filter push button
             self.ui.pbEFOFilter.setEnabled(False)
 
-    @Slot(None, name="cfr_change_bounds_and_broadcast")
+    @Slot()
     def cfr_change_bounds_and_broadcast(self, text):
         """Update the CFR bounds and broadcast changes."""
 
         # Initialize the status to valid
         self.valid["leCFRLowerBound"] = True
         self.valid["leCFRUpperBound"] = True
 
@@ -506,15 +533,15 @@
         if self.valid["leCFRLowerBound"] and self.valid["leCFRUpperBound"]:
             # Broadcast
             self.cfr_bounds_modified.emit()
         else:
             # Disable the filter push button
             self.ui.pbCFRFilter.setEnabled(False)
 
-    @Slot(None, name="reset_filters")
+    @Slot()
     def reset_filters(self):
         """Reset fluorophores pull-down menu in the wizard and broadcast changes to other tools."""
 
         # Reset the fluorophore ID pull-down menu
         self.reset_fluorophores()
 
         # Broadcast change
```

### Comparing `pyminflux-0.4.0/pyminflux/ui/wizard.ui` & `pyminflux-0.4.1/pyminflux/ui/wizard.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/utils/__init__.py` & `pyminflux-0.4.1/pyminflux/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyminflux/utils/_utils.py` & `pyminflux-0.4.1/pyminflux/utils/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,23 +39,30 @@
 
     # Initialize outputs
     code = -1
     version = ""
     error = ""
 
     # Get the redirect from the latest release URL
-    response = requests.get(
-        "https://github.com/bsse-scf/pyMINFLUX/releases/latest", allow_redirects=False
-    )
+    try:
+        response = requests.get(
+            "https://github.com/bsse-scf/pyMINFLUX/releases/latest",
+            allow_redirects=False,
+        )
 
-    # This should redirect (status code 301 or 302)
-    if response.status_code in (301, 302):
-        redirect_url = response.headers["Location"]
-    else:
-        error = "Could not check for updates!"
+        # This should redirect (status code 301 or 302)
+        if response.status_code in (301, 302):
+            redirect_url = response.headers["Location"]
+        else:
+            error = "Could not check for updates!"
+            return code, version, error
+
+    except Exception as e:
+        # Could not connect at all
+        error = "Could not retrieve version information from server!"
         return code, version, error
 
     # Try retrieving the version string
     match = re.search(r"\b(\d+)\.(\d+)\.(\d+)$", redirect_url)
     if match:
         x, y, z = match.groups()
     else:
```

### Comparing `pyminflux-0.4.0/pyminflux/writer/_native_writer.py` & `pyminflux-0.4.1/pyminflux/writer/_native_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,17 @@
     def message(self):
         """Return last error message."""
         return self._message
 
     def _store_dataframe(self, group):
         """Write the Pandas DataFrame in a way that it can be reloaded without external dependencies."""
 
+        if self.processor.filtered_dataframe is None:
+            return
+
         dataset = group.create_dataset(
             "dataframe",
             data=self.processor.filtered_dataframe.to_numpy(),
             compression="gzip",
         )
 
         # Convert the column names to a list of strings
@@ -134,7 +137,8 @@
         group.create_dataset("num_fluorophores", data=self.processor.num_fluorophores)
         group.create_dataset("dwell_time", data=self.state.dwell_time)
         group.create_dataset("scale_bar_size", data=self.state.scale_bar_size)
 
         # HDF5 does not have a native boolean type, so we save as int8 and convert it
         # back to boolean on read.
         group.create_dataset("is_tracking", data=np.int8(self.state.is_tracking))
+        group.create_dataset("pool_dcr", data=np.int8(self.state.pool_dcr))
```

### Comparing `pyminflux-0.4.0/pyminflux/writer/_writer.py` & `pyminflux-0.4.1/pyminflux/writer/_writer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.4.0/pyproject.toml` & `pyminflux-0.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyminflux"
-version = "0.4.0"
+version = "0.4.1"
 description = "Reader, processor, and viewer of MINFLUX raw data."
 authors = ["Aaron Ponti <aaron.ponti@bsse.ethz.ch>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/bsse-scf/pyMINFLUX"
 documentation = "https://github.com/bsse-scf/pyMINFLUX/wiki"
 keywords = ["MINFLUX", "Visualization", "Filtering", "Analysis", "Python"]
@@ -67,14 +67,16 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 ordered-set = "^4.1.0"
 pytest-cov = "^4.1.0"
 pre-commit = "^3.6.0"
 pdoc3 = "^0.10.0"
 pyinstaller = "^6.3.0"
+nuitka = "^2.1.5"
+zstandard = "^0.22.0"
 
 [tool.poetry.scripts]
 pyminflux = "pyminflux.main:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyminflux-0.4.0/PKG-INFO` & `pyminflux-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyminflux
-Version: 0.4.0
+Version: 0.4.1
 Summary: Reader, processor, and viewer of MINFLUX raw data.
 Home-page: https://github.com/bsse-scf/pyMINFLUX
 License: Apache-2.0
 Keywords: MINFLUX,Visualization,Filtering,Analysis,Python
 Author: Aaron Ponti
 Author-email: aaron.ponti@bsse.ethz.ch
 Requires-Python: >=3.10,<3.12
@@ -75,14 +75,16 @@
 $ conda activate pyminflux-env
 $ git clone https://github.com/bsse-scf/pyMINFLUX /path/to/pyminflux
 $ cd /path/to/pyminflux
 $ python -m pip install -e .
 $ pip install -r dev-requirements.txt
 ```
 
+If you want to participate to the development of pyMINFLUX, please have a look at [how you can contribute](CONTRIBUTING.md) and at our [code of conduct](CODE_OF_CONDUCT.md).
+
 ### Running pyMINFLUX from console
 
 ```sh
 $ cd /path/to/pyminflux
 $ python pyminflux/main.py  # As a Python script, or
 $ pyminflux                 # as a standalone tool
 ```
@@ -99,14 +101,18 @@
 
 The official pyMINFLUX website is on https://pyminflux.ethz.ch.
 
 ## pyMINFLUX mailing list
 
 Join the [pyMINFLUX mailing list](https://sympa.ethz.ch/sympa/subscribe/pyminflux) for release announcements and further discussions.
 
+## Contributing to pyMINFLUX
+
+We value the contribution of our community members, and to make sure that everyone can profit from this collaboration, we ask you to have a look at our [CONTRIBUTING](./CONTRIBUTING.md) and [CODE OF CONDUCT](./CODE_OF_CONDUCT.md) documents.
+
 ## Citing pyMINFLUX
 
 If you use pyMINFLUX in your research, please cite this repository as follows:
 
 > Aaron Ponti, Javier Casares Arias, & Thomas Horn. (2023). pyMINFLUX. Zenodo. [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7895501.svg)](https://doi.org/10.5281/zenodo.7895501)
```

