# Comparing `tmp/pix2text-1.1.0.1.tar.gz` & `tmp/pix2text-1.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix2text-1.1.0.1.tar", last modified: Tue Apr 30 03:15:23 2024, max compression
+gzip compressed data, was "pix2text-1.1.0.2.tar", last modified: Fri May 10 08:29:54 2024, max compression
```

## Comparing `pix2text-1.1.0.1.tar` & `pix2text-1.1.0.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.758790 pix2text-1.1.0.1/
--rw-r--r--   0 king       (501) staff       (20)     1067 2022-09-07 14:44:50.000000 pix2text-1.1.0.1/LICENSE
--rw-r--r--   0 king       (501) staff       (20)    14122 2024-04-30 03:15:23.758627 pix2text-1.1.0.1/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)    12903 2024-04-28 15:49:28.000000 pix2text-1.1.0.1/README.md
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.745408 pix2text-1.1.0.1/pix2text/
--rw-r--r--   0 king       (501) staff       (20)      456 2024-04-02 11:11:40.000000 pix2text-1.1.0.1/pix2text/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      203 2024-04-30 03:00:46.000000 pix2text-1.1.0.1/pix2text/__version__.py
--rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-1.1.0.1/pix2text/app.py
--rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-1.1.0.1/pix2text/category_mapping.py
--rw-r--r--   0 king       (501) staff       (20)    10451 2024-04-22 00:51:42.000000 pix2text-1.1.0.1/pix2text/cli.py
--rw-r--r--   0 king       (501) staff       (20)     3710 2024-04-16 14:50:16.000000 pix2text-1.1.0.1/pix2text/consts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.750090 pix2text-1.1.0.1/pix2text/doc_xl_layout/
--rw-r--r--   0 king       (501) staff       (20)      192 2024-04-03 01:13:56.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/__init__.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.751016 pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     8390 2024-04-02 08:34:16.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/base_detector_subfield.py
--rw-r--r--   0 king       (501) staff       (20)     8722 2024-04-02 07:16:21.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/ctdet_subfield.py
--rw-r--r--   0 king       (501) staff       (20)      137 2024-04-02 06:45:51.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/detector_factory.py
--rw-r--r--   0 king       (501) staff       (20)    17861 2024-04-30 02:52:35.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/doc_xl_layout_parser.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.751358 pix2text-1.1.0.1/pix2text/doc_xl_layout/external/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/external/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     2510 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/external/shapelyNMS.py
--rw-r--r--   0 king       (501) staff       (20)      365 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/huntie_subfield.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.752794 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     5178 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/data_parallel.py
--rw-r--r--   0 king       (501) staff       (20)    23840 2024-04-02 07:32:06.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/decode.py
--rw-r--r--   0 king       (501) staff       (20)     3443 2024-04-10 11:32:17.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/model.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.753115 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/networks/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/networks/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    24395 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py
--rw-r--r--   0 king       (501) staff       (20)     1528 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/scatter_gather.py
--rw-r--r--   0 king       (501) staff       (20)     1800 2024-04-02 07:31:48.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/models/utils.py
--rw-r--r--   0 king       (501) staff       (20)    23801 2024-04-02 00:43:23.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/opts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.755031 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/
--rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     4818 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/ddd_utils.py
--rw-r--r--   0 king       (501) staff       (20)    26623 2024-04-02 06:59:29.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/debugger.py
--rw-r--r--   0 king       (501) staff       (20)    18383 2024-04-02 06:47:12.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/evaluation_bk.py
--rw-r--r--   0 king       (501) staff       (20)     7851 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/image.py
--rw-r--r--   0 king       (501) staff       (20)     5368 2024-04-02 06:47:54.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/post_process.py
--rw-r--r--   0 king       (501) staff       (20)      533 2024-04-01 15:18:57.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/utils.py
--rw-r--r--   0 king       (501) staff       (20)     8844 2024-04-02 06:20:49.000000 pix2text-1.1.0.1/pix2text/doc_xl_layout/wrapper.py
--rw-r--r--   0 king       (501) staff       (20)    12517 2024-03-27 09:59:17.000000 pix2text-1.1.0.1/pix2text/element.py
--rw-r--r--   0 king       (501) staff       (20)    17431 2024-04-22 02:21:39.000000 pix2text-1.1.0.1/pix2text/latex_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    13244 2024-01-11 04:27:38.000000 pix2text-1.1.0.1/pix2text/latex_ocr0.py
--rw-r--r--   0 king       (501) staff       (20)    22526 2024-01-10 13:35:10.000000 pix2text-1.1.0.1/pix2text/latex_recog.py
--rw-r--r--   0 king       (501) staff       (20)     4016 2024-04-06 13:32:28.000000 pix2text-1.1.0.1/pix2text/layout_parser.py
--rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-1.1.0.1/pix2text/object_detector.py
--rw-r--r--   0 king       (501) staff       (20)     7285 2024-04-27 13:58:01.000000 pix2text-1.1.0.1/pix2text/ocr_engine.py
--rw-r--r--   0 king       (501) staff       (20)    10497 2024-04-30 02:55:47.000000 pix2text-1.1.0.1/pix2text/page_elements.py
--rw-r--r--   0 king       (501) staff       (20)    28192 2024-04-24 14:01:37.000000 pix2text-1.1.0.1/pix2text/pix_to_text.py
--rw-r--r--   0 king       (501) staff       (20)     5413 2024-04-30 02:57:49.000000 pix2text-1.1.0.1/pix2text/render.py
--rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-1.1.0.1/pix2text/screenshot_daemon_with_server2.py
--rw-r--r--   0 king       (501) staff       (20)     2776 2024-04-21 15:29:44.000000 pix2text-1.1.0.1/pix2text/serve.py
--rw-r--r--   0 king       (501) staff       (20)    38505 2024-03-27 14:55:51.000000 pix2text-1.1.0.1/pix2text/table_inference.py
--rw-r--r--   0 king       (501) staff       (20)    38370 2024-04-30 02:58:35.000000 pix2text-1.1.0.1/pix2text/table_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    37328 2024-03-29 23:43:03.000000 pix2text-1.1.0.1/pix2text/table_postprocess.py
--rw-r--r--   0 king       (501) staff       (20)    24628 2024-04-22 00:24:28.000000 pix2text-1.1.0.1/pix2text/text_formula_ocr.py
--rw-r--r--   0 king       (501) staff       (20)    31700 2024-04-21 13:52:16.000000 pix2text-1.1.0.1/pix2text/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.746924 pix2text-1.1.0.1/pix2text.egg-info/
--rw-r--r--   0 king       (501) staff       (20)    14122 2024-04-30 03:15:23.000000 pix2text-1.1.0.1/pix2text.egg-info/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)     2405 2024-04-30 03:15:23.000000 pix2text-1.1.0.1/pix2text.egg-info/SOURCES.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2024-04-30 03:15:23.000000 pix2text-1.1.0.1/pix2text.egg-info/dependency_links.txt
--rw-r--r--   0 king       (501) staff       (20)       42 2024-04-30 03:15:23.000000 pix2text-1.1.0.1/pix2text.egg-info/entry_points.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-1.1.0.1/pix2text.egg-info/not-zip-safe
--rw-r--r--   0 king       (501) staff       (20)      269 2024-04-30 03:15:23.000000 pix2text-1.1.0.1/pix2text.egg-info/requires.txt
--rw-r--r--   0 king       (501) staff       (20)       17 2024-04-30 03:15:23.000000 pix2text-1.1.0.1/pix2text.egg-info/top_level.txt
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.757838 pix2text-1.1.0.1/scripts/
--rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-1.1.0.1/scripts/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     2586 2023-06-09 10:01:38.000000 pix2text-1.1.0.1/scripts/convert_label_studio_to_yolov7.py
--rw-r--r--   0 king       (501) staff       (20)     6678 2024-01-03 07:40:48.000000 pix2text-1.1.0.1/scripts/extract_p2t_results.py
--rw-r--r--   0 king       (501) staff       (20)     4198 2023-06-19 02:59:28.000000 pix2text-1.1.0.1/scripts/gen_label_studio_json.py
--rw-r--r--   0 king       (501) staff       (20)     1966 2023-06-09 09:46:06.000000 pix2text-1.1.0.1/scripts/gen_pure_formula_to_yolov7.py
--rw-r--r--   0 king       (501) staff       (20)     1609 2023-06-03 02:41:33.000000 pix2text-1.1.0.1/scripts/merge_label_studio_anno_pred_json.py
--rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-1.1.0.1/scripts/object_detection3.py
--rw-r--r--   0 king       (501) staff       (20)     2413 2023-07-03 03:10:18.000000 pix2text-1.1.0.1/scripts/screenshot_daemon.py
--rw-r--r--   0 king       (501) staff       (20)      143 2024-01-01 08:28:55.000000 pix2text-1.1.0.1/scripts/try_easyocr.py
--rw-r--r--   0 king       (501) staff       (20)      796 2024-03-13 15:31:39.000000 pix2text-1.1.0.1/scripts/try_latex_correction.py
--rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-1.1.0.1/scripts/try_layout.py
--rw-r--r--   0 king       (501) staff       (20)      861 2024-03-29 15:11:40.000000 pix2text-1.1.0.1/scripts/try_pix2text_mfr.py
--rw-r--r--   0 king       (501) staff       (20)      845 2024-04-21 15:31:13.000000 pix2text-1.1.0.1/scripts/try_service.py
--rw-r--r--   0 king       (501) staff       (20)     1614 2024-01-05 04:02:17.000000 pix2text-1.1.0.1/scripts/try_texify.py
--rw-r--r--   0 king       (501) staff       (20)       38 2024-04-30 03:15:23.758845 pix2text-1.1.0.1/setup.cfg
--rw-r--r--   0 king       (501) staff       (20)     2522 2024-04-30 03:06:08.000000 pix2text-1.1.0.1/setup.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2024-04-30 03:15:23.758424 pix2text-1.1.0.1/tests/
--rw-r--r--   0 king       (501) staff       (20)     5861 2024-04-10 11:52:24.000000 pix2text-1.1.0.1/tests/test_pix2text.py
--rw-r--r--   0 king       (501) staff       (20)     1761 2023-07-01 07:49:03.000000 pix2text-1.1.0.1/tests/test_sort_boxes.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.101494 pix2text-1.1.0.2/
+-rw-r--r--   0 king       (501) staff       (20)     1067 2022-09-07 14:44:50.000000 pix2text-1.1.0.2/LICENSE
+-rw-r--r--   0 king       (501) staff       (20)    14138 2024-05-10 08:29:54.101276 pix2text-1.1.0.2/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)    12919 2024-05-06 08:46:19.000000 pix2text-1.1.0.2/README.md
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.089170 pix2text-1.1.0.2/pix2text/
+-rw-r--r--   0 king       (501) staff       (20)      456 2024-04-02 11:11:40.000000 pix2text-1.1.0.2/pix2text/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      203 2024-05-10 08:21:55.000000 pix2text-1.1.0.2/pix2text/__version__.py
+-rw-r--r--   0 king       (501) staff       (20)     1709 2022-09-10 15:50:05.000000 pix2text-1.1.0.2/pix2text/app.py
+-rw-r--r--   0 king       (501) staff       (20)     2092 2022-09-08 07:30:17.000000 pix2text-1.1.0.2/pix2text/category_mapping.py
+-rw-r--r--   0 king       (501) staff       (20)    10451 2024-04-22 00:51:42.000000 pix2text-1.1.0.2/pix2text/cli.py
+-rw-r--r--   0 king       (501) staff       (20)     3710 2024-04-16 14:50:16.000000 pix2text-1.1.0.2/pix2text/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.091837 pix2text-1.1.0.2/pix2text/doc_xl_layout/
+-rw-r--r--   0 king       (501) staff       (20)      192 2024-04-03 01:13:56.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/__init__.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.092874 pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     8390 2024-04-02 08:34:16.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/base_detector_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)     8722 2024-04-02 07:16:21.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/ctdet_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)      137 2024-04-02 06:45:51.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/detector_factory.py
+-rw-r--r--   0 king       (501) staff       (20)    17861 2024-04-30 02:52:35.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/doc_xl_layout_parser.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.093174 pix2text-1.1.0.2/pix2text/doc_xl_layout/external/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/external/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     2510 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/external/shapelyNMS.py
+-rw-r--r--   0 king       (501) staff       (20)      365 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/huntie_subfield.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.094558 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     5178 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/data_parallel.py
+-rw-r--r--   0 king       (501) staff       (20)    23840 2024-04-02 07:32:06.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/decode.py
+-rw-r--r--   0 king       (501) staff       (20)     3443 2024-04-10 11:32:17.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/model.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.094873 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/networks/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/networks/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    24395 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py
+-rw-r--r--   0 king       (501) staff       (20)     1528 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/scatter_gather.py
+-rw-r--r--   0 king       (501) staff       (20)     1800 2024-04-02 07:31:48.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/models/utils.py
+-rw-r--r--   0 king       (501) staff       (20)    23801 2024-04-02 00:43:23.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/opts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.096803 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/
+-rw-r--r--   0 king       (501) staff       (20)        0 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     4818 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/ddd_utils.py
+-rw-r--r--   0 king       (501) staff       (20)    26623 2024-04-02 06:59:29.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/debugger.py
+-rw-r--r--   0 king       (501) staff       (20)    18383 2024-04-02 06:47:12.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/evaluation_bk.py
+-rw-r--r--   0 king       (501) staff       (20)     7851 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/image.py
+-rw-r--r--   0 king       (501) staff       (20)     5368 2024-04-02 06:47:54.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/post_process.py
+-rw-r--r--   0 king       (501) staff       (20)      533 2024-04-01 15:18:57.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/utils.py
+-rw-r--r--   0 king       (501) staff       (20)     8844 2024-04-02 06:20:49.000000 pix2text-1.1.0.2/pix2text/doc_xl_layout/wrapper.py
+-rw-r--r--   0 king       (501) staff       (20)    12517 2024-03-27 09:59:17.000000 pix2text-1.1.0.2/pix2text/element.py
+-rw-r--r--   0 king       (501) staff       (20)    17431 2024-04-22 02:21:39.000000 pix2text-1.1.0.2/pix2text/latex_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    13244 2024-01-11 04:27:38.000000 pix2text-1.1.0.2/pix2text/latex_ocr0.py
+-rw-r--r--   0 king       (501) staff       (20)    22526 2024-01-10 13:35:10.000000 pix2text-1.1.0.2/pix2text/latex_recog.py
+-rw-r--r--   0 king       (501) staff       (20)     4016 2024-04-06 13:32:28.000000 pix2text-1.1.0.2/pix2text/layout_parser.py
+-rw-r--r--   0 king       (501) staff       (20)     3567 2022-09-13 02:10:01.000000 pix2text-1.1.0.2/pix2text/object_detector.py
+-rw-r--r--   0 king       (501) staff       (20)     7285 2024-04-27 13:58:01.000000 pix2text-1.1.0.2/pix2text/ocr_engine.py
+-rw-r--r--   0 king       (501) staff       (20)    10497 2024-04-30 02:55:47.000000 pix2text-1.1.0.2/pix2text/page_elements.py
+-rw-r--r--   0 king       (501) staff       (20)    28192 2024-04-24 14:01:37.000000 pix2text-1.1.0.2/pix2text/pix_to_text.py
+-rw-r--r--   0 king       (501) staff       (20)     5413 2024-04-30 02:57:49.000000 pix2text-1.1.0.2/pix2text/render.py
+-rw-r--r--   0 king       (501) staff       (20)     8692 2022-09-07 08:30:37.000000 pix2text-1.1.0.2/pix2text/screenshot_daemon_with_server2.py
+-rw-r--r--   0 king       (501) staff       (20)     2776 2024-04-21 15:29:44.000000 pix2text-1.1.0.2/pix2text/serve.py
+-rw-r--r--   0 king       (501) staff       (20)    38505 2024-03-27 14:55:51.000000 pix2text-1.1.0.2/pix2text/table_inference.py
+-rw-r--r--   0 king       (501) staff       (20)    38370 2024-04-30 02:58:35.000000 pix2text-1.1.0.2/pix2text/table_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    37328 2024-03-29 23:43:03.000000 pix2text-1.1.0.2/pix2text/table_postprocess.py
+-rw-r--r--   0 king       (501) staff       (20)    24628 2024-04-22 00:24:28.000000 pix2text-1.1.0.2/pix2text/text_formula_ocr.py
+-rw-r--r--   0 king       (501) staff       (20)    31718 2024-05-10 08:12:46.000000 pix2text-1.1.0.2/pix2text/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.090366 pix2text-1.1.0.2/pix2text.egg-info/
+-rw-r--r--   0 king       (501) staff       (20)    14138 2024-05-10 08:29:54.000000 pix2text-1.1.0.2/pix2text.egg-info/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)     2405 2024-05-10 08:29:54.000000 pix2text-1.1.0.2/pix2text.egg-info/SOURCES.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2024-05-10 08:29:54.000000 pix2text-1.1.0.2/pix2text.egg-info/dependency_links.txt
+-rw-r--r--   0 king       (501) staff       (20)       42 2024-05-10 08:29:54.000000 pix2text-1.1.0.2/pix2text.egg-info/entry_points.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2022-09-07 15:32:44.000000 pix2text-1.1.0.2/pix2text.egg-info/not-zip-safe
+-rw-r--r--   0 king       (501) staff       (20)      269 2024-05-10 08:29:54.000000 pix2text-1.1.0.2/pix2text.egg-info/requires.txt
+-rw-r--r--   0 king       (501) staff       (20)       17 2024-05-10 08:29:54.000000 pix2text-1.1.0.2/pix2text.egg-info/top_level.txt
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.099933 pix2text-1.1.0.2/scripts/
+-rw-r--r--   0 king       (501) staff       (20)       16 2022-09-08 02:47:44.000000 pix2text-1.1.0.2/scripts/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     2586 2023-06-09 10:01:38.000000 pix2text-1.1.0.2/scripts/convert_label_studio_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     6678 2024-01-03 07:40:48.000000 pix2text-1.1.0.2/scripts/extract_p2t_results.py
+-rw-r--r--   0 king       (501) staff       (20)     4198 2023-06-19 02:59:28.000000 pix2text-1.1.0.2/scripts/gen_label_studio_json.py
+-rw-r--r--   0 king       (501) staff       (20)     1966 2023-06-09 09:46:06.000000 pix2text-1.1.0.2/scripts/gen_pure_formula_to_yolov7.py
+-rw-r--r--   0 king       (501) staff       (20)     1609 2023-06-03 02:41:33.000000 pix2text-1.1.0.2/scripts/merge_label_studio_anno_pred_json.py
+-rw-r--r--   0 king       (501) staff       (20)     4409 2022-09-08 06:37:58.000000 pix2text-1.1.0.2/scripts/object_detection3.py
+-rw-r--r--   0 king       (501) staff       (20)     2413 2023-07-03 03:10:18.000000 pix2text-1.1.0.2/scripts/screenshot_daemon.py
+-rw-r--r--   0 king       (501) staff       (20)      143 2024-01-01 08:28:55.000000 pix2text-1.1.0.2/scripts/try_easyocr.py
+-rw-r--r--   0 king       (501) staff       (20)      796 2024-03-13 15:31:39.000000 pix2text-1.1.0.2/scripts/try_latex_correction.py
+-rw-r--r--   0 king       (501) staff       (20)      787 2022-09-23 04:41:39.000000 pix2text-1.1.0.2/scripts/try_layout.py
+-rw-r--r--   0 king       (501) staff       (20)      861 2024-03-29 15:11:40.000000 pix2text-1.1.0.2/scripts/try_pix2text_mfr.py
+-rw-r--r--   0 king       (501) staff       (20)      845 2024-04-21 15:31:13.000000 pix2text-1.1.0.2/scripts/try_service.py
+-rw-r--r--   0 king       (501) staff       (20)     1614 2024-01-05 04:02:17.000000 pix2text-1.1.0.2/scripts/try_texify.py
+-rw-r--r--   0 king       (501) staff       (20)       38 2024-05-10 08:29:54.101539 pix2text-1.1.0.2/setup.cfg
+-rw-r--r--   0 king       (501) staff       (20)     2522 2024-04-30 03:06:08.000000 pix2text-1.1.0.2/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2024-05-10 08:29:54.100682 pix2text-1.1.0.2/tests/
+-rw-r--r--   0 king       (501) staff       (20)     5861 2024-04-10 11:52:24.000000 pix2text-1.1.0.2/tests/test_pix2text.py
+-rw-r--r--   0 king       (501) staff       (20)     1761 2023-07-01 07:49:03.000000 pix2text-1.1.0.2/tests/test_sort_boxes.py
```

### Comparing `pix2text-1.1.0.1/LICENSE` & `pix2text-1.1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/PKG-INFO` & `pix2text-1.1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix2text
-Version: 1.1.0.1
+Version: 1.1.0.2
 Summary: An Open-Source Python3 tool for recognizing layouts, tables, math formulas, and text in images, converting them into Markdown format. A free alternative to Mathpix, empowering seamless conversion of visual content into text-based representations.
 Home-page: https://github.com/breezedeus/pix2text
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: MIT
 Platform: Mac
 Platform: Linux
@@ -41,15 +41,15 @@
 ![last-release](https://img.shields.io/github/release-date/breezedeus/pix2text)
 ![last-commit](https://img.shields.io/github/last-commit/breezedeus/pix2text)
 [![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
 
 [📖 Doc](https://pix2text.readthedocs.io) |
 [👩🏻‍💻 Online Service](https://p2t.breezedeus.com) |
 [👨🏻‍💻 Demo](https://huggingface.co/spaces/breezedeus/Pix2Text-Demo) |
-[💬 Contact](https://www.breezedeus.com/join-group)
+[💬 Contact](https://www.breezedeus.com/article/join-group)
 
 </div>
 
 <div align="center">
 
 [中文](./README_cn.md) | English
 
@@ -269,15 +269,15 @@
 <div align="center">
   <img src="https://github.com/breezedeus/Pix2Text-Mac/raw/main/assets/on_menu_bar.jpg" alt="Pix2Text Mac App" width="400px"/>
 </div>
 
 
 ## A cup of coffee for the author
 
-It is not easy to maintain and evolve the project, so if it is helpful to you, please consider [offering the author a cup of coffee 🥤](https://www.breezedeus.com/buy-me-coffee).
+It is not easy to maintain and evolve the project, so if it is helpful to you, please consider [offering the author a cup of coffee 🥤](https://www.breezedeus.com/article/buy-me-coffee).
 
 ---
 
 Official code base: [https://github.com/breezedeus/pix2text](https://github.com/breezedeus/pix2text). Please cite it properly.
 
 For more information on Pix2Text (P2T), visit: [https://www.breezedeus.com/article/pix2text](https://www.breezedeus.com/article/pix2text).
```

### Comparing `pix2text-1.1.0.1/README.md` & `pix2text-1.1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ![last-release](https://img.shields.io/github/release-date/breezedeus/pix2text)
 ![last-commit](https://img.shields.io/github/last-commit/breezedeus/pix2text)
 [![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
 
 [📖 Doc](https://pix2text.readthedocs.io) |
 [👩🏻‍💻 Online Service](https://p2t.breezedeus.com) |
 [👨🏻‍💻 Demo](https://huggingface.co/spaces/breezedeus/Pix2Text-Demo) |
-[💬 Contact](https://www.breezedeus.com/join-group)
+[💬 Contact](https://www.breezedeus.com/article/join-group)
 
 </div>
 
 <div align="center">
 
 [中文](./README_cn.md) | English
 
@@ -240,14 +240,14 @@
 <div align="center">
   <img src="https://github.com/breezedeus/Pix2Text-Mac/raw/main/assets/on_menu_bar.jpg" alt="Pix2Text Mac App" width="400px"/>
 </div>
 
 
 ## A cup of coffee for the author
 
-It is not easy to maintain and evolve the project, so if it is helpful to you, please consider [offering the author a cup of coffee 🥤](https://www.breezedeus.com/buy-me-coffee).
+It is not easy to maintain and evolve the project, so if it is helpful to you, please consider [offering the author a cup of coffee 🥤](https://www.breezedeus.com/article/buy-me-coffee).
 
 ---
 
 Official code base: [https://github.com/breezedeus/pix2text](https://github.com/breezedeus/pix2text). Please cite it properly.
 
 For more information on Pix2Text (P2T), visit: [https://www.breezedeus.com/article/pix2text](https://www.breezedeus.com/article/pix2text).
```

### Comparing `pix2text-1.1.0.1/pix2text/app.py` & `pix2text-1.1.0.2/pix2text/app.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/category_mapping.py` & `pix2text-1.1.0.2/pix2text/category_mapping.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/cli.py` & `pix2text-1.1.0.2/pix2text/cli.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/consts.py` & `pix2text-1.1.0.2/pix2text/consts.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/base_detector_subfield.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/base_detector_subfield.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/detectors/ctdet_subfield.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/detectors/ctdet_subfield.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/doc_xl_layout_parser.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/doc_xl_layout_parser.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/external/shapelyNMS.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/external/shapelyNMS.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/models/data_parallel.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/models/data_parallel.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/models/decode.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/models/decode.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/models/model.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/models/model.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/models/networks/dlav0_subfield.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/models/scatter_gather.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/models/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/models/utils.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/models/utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/opts.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/opts.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/ddd_utils.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/ddd_utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/debugger.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/debugger.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/evaluation_bk.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/evaluation_bk.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/image.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/image.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/post_process.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/post_process.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/utils/utils.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/doc_xl_layout/wrapper.py` & `pix2text-1.1.0.2/pix2text/doc_xl_layout/wrapper.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/element.py` & `pix2text-1.1.0.2/pix2text/element.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/latex_ocr.py` & `pix2text-1.1.0.2/pix2text/latex_ocr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/latex_ocr0.py` & `pix2text-1.1.0.2/pix2text/latex_ocr0.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/latex_recog.py` & `pix2text-1.1.0.2/pix2text/latex_recog.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/layout_parser.py` & `pix2text-1.1.0.2/pix2text/layout_parser.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/object_detector.py` & `pix2text-1.1.0.2/pix2text/object_detector.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/ocr_engine.py` & `pix2text-1.1.0.2/pix2text/ocr_engine.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/page_elements.py` & `pix2text-1.1.0.2/pix2text/page_elements.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/pix_to_text.py` & `pix2text-1.1.0.2/pix2text/pix_to_text.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/render.py` & `pix2text-1.1.0.2/pix2text/render.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/screenshot_daemon_with_server2.py` & `pix2text-1.1.0.2/pix2text/screenshot_daemon_with_server2.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/serve.py` & `pix2text-1.1.0.2/pix2text/serve.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/table_inference.py` & `pix2text-1.1.0.2/pix2text/table_inference.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/table_ocr.py` & `pix2text-1.1.0.2/pix2text/table_ocr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/table_postprocess.py` & `pix2text-1.1.0.2/pix2text/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/text_formula_ocr.py` & `pix2text-1.1.0.2/pix2text/text_formula_ocr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/pix2text/utils.py` & `pix2text-1.1.0.2/pix2text/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -910,16 +910,16 @@
 
     indentation_thrsh = (max_x - min_x) * 0.1
     if mean_height is not None:
         indentation_thrsh = 1.5 * mean_height
 
     min_x, max_x = cal_block_xmin_xmax(lines, indentation_thrsh)
 
-    line_text_list = [(idx, txt) for idx, txt in enumerate(line_text_list) if txt]
     res_line_texts = [''] * len(line_text_list)
+    line_text_list = [(idx, txt) for idx, txt in enumerate(line_text_list) if txt]
     for idx, (line_number, txt) in enumerate(line_text_list):
         if isolated_included[line_number]:
             res_line_texts[line_number] = line_sep + txt + line_sep
             continue
 
         tmp = txt
         if line_margin_list[line_number][0] > min_x + indentation_thrsh:
@@ -934,9 +934,9 @@
                 and line_ymin_ymax_list[next_line_number][0] < line_ymin_ymax_list[next_line_number][1]
                 and line_ymin_ymax_list[next_line_number][0] - line_ymin_ymax_list[line_number][1]
                 > cur_height
             ):  # 当前行与下一行的间距超过了一行的行高，则认为它们之间应该是不同的段落
                 tmp = tmp + line_sep
         res_line_texts[idx] = tmp
 
-    outs = smart_join(res_line_texts, spellchecker)
+    outs = smart_join([c for c in res_line_texts if c], spellchecker)
     return re.sub(rf'{line_sep}+', line_sep, outs)  # 把多个 '\n' 替换为 '\n'
```

### Comparing `pix2text-1.1.0.1/pix2text.egg-info/PKG-INFO` & `pix2text-1.1.0.2/pix2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix2text
-Version: 1.1.0.1
+Version: 1.1.0.2
 Summary: An Open-Source Python3 tool for recognizing layouts, tables, math formulas, and text in images, converting them into Markdown format. A free alternative to Mathpix, empowering seamless conversion of visual content into text-based representations.
 Home-page: https://github.com/breezedeus/pix2text
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: MIT
 Platform: Mac
 Platform: Linux
@@ -41,15 +41,15 @@
 ![last-release](https://img.shields.io/github/release-date/breezedeus/pix2text)
 ![last-commit](https://img.shields.io/github/last-commit/breezedeus/pix2text)
 [![Twitter](https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fbreezedeus)](https://twitter.com/breezedeus)
 
 [📖 Doc](https://pix2text.readthedocs.io) |
 [👩🏻‍💻 Online Service](https://p2t.breezedeus.com) |
 [👨🏻‍💻 Demo](https://huggingface.co/spaces/breezedeus/Pix2Text-Demo) |
-[💬 Contact](https://www.breezedeus.com/join-group)
+[💬 Contact](https://www.breezedeus.com/article/join-group)
 
 </div>
 
 <div align="center">
 
 [中文](./README_cn.md) | English
 
@@ -269,15 +269,15 @@
 <div align="center">
   <img src="https://github.com/breezedeus/Pix2Text-Mac/raw/main/assets/on_menu_bar.jpg" alt="Pix2Text Mac App" width="400px"/>
 </div>
 
 
 ## A cup of coffee for the author
 
-It is not easy to maintain and evolve the project, so if it is helpful to you, please consider [offering the author a cup of coffee 🥤](https://www.breezedeus.com/buy-me-coffee).
+It is not easy to maintain and evolve the project, so if it is helpful to you, please consider [offering the author a cup of coffee 🥤](https://www.breezedeus.com/article/buy-me-coffee).
 
 ---
 
 Official code base: [https://github.com/breezedeus/pix2text](https://github.com/breezedeus/pix2text). Please cite it properly.
 
 For more information on Pix2Text (P2T), visit: [https://www.breezedeus.com/article/pix2text](https://www.breezedeus.com/article/pix2text).
```

### Comparing `pix2text-1.1.0.1/pix2text.egg-info/SOURCES.txt` & `pix2text-1.1.0.2/pix2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/scripts/convert_label_studio_to_yolov7.py` & `pix2text-1.1.0.2/scripts/convert_label_studio_to_yolov7.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/scripts/extract_p2t_results.py` & `pix2text-1.1.0.2/scripts/extract_p2t_results.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/scripts/gen_label_studio_json.py` & `pix2text-1.1.0.2/scripts/gen_label_studio_json.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/scripts/gen_pure_formula_to_yolov7.py` & `pix2text-1.1.0.2/scripts/gen_pure_formula_to_yolov7.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/scripts/merge_label_studio_anno_pred_json.py` & `pix2text-1.1.0.2/scripts/merge_label_studio_anno_pred_json.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/scripts/object_detection3.py` & `pix2text-1.1.0.2/scripts/object_detection3.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/scripts/screenshot_daemon.py` & `pix2text-1.1.0.2/scripts/screenshot_daemon.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/scripts/try_latex_correction.py` & `pix2text-1.1.0.2/scripts/try_latex_correction.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/scripts/try_layout.py` & `pix2text-1.1.0.2/scripts/try_layout.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/scripts/try_pix2text_mfr.py` & `pix2text-1.1.0.2/scripts/try_pix2text_mfr.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/scripts/try_service.py` & `pix2text-1.1.0.2/scripts/try_service.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/scripts/try_texify.py` & `pix2text-1.1.0.2/scripts/try_texify.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/setup.py` & `pix2text-1.1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/tests/test_pix2text.py` & `pix2text-1.1.0.2/tests/test_pix2text.py`

 * *Files identical despite different names*

### Comparing `pix2text-1.1.0.1/tests/test_sort_boxes.py` & `pix2text-1.1.0.2/tests/test_sort_boxes.py`

 * *Files identical despite different names*

