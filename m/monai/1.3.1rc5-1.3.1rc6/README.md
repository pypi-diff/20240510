# Comparing `tmp/monai-1.3.1rc5-py3-none-any.whl.zip` & `tmp/monai-1.3.1rc6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,62 +1,62 @@
-Zip file size: 1366611 bytes, number of entries: 387
--rw-rw-r--  2.0 unx     2663 b- defN 24-Apr-12 13:56 monai/__init__.py
--rw-rw-r--  2.0 unx      500 b- defN 24-Apr-19 06:53 monai/_version.py
+Zip file size: 1368313 bytes, number of entries: 387
+-rw-rw-r--  2.0 unx     2663 b- defN 24-Apr-22 04:57 monai/__init__.py
+-rw-rw-r--  2.0 unx      500 b- defN 24-Apr-26 07:07 monai/_version.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Dec-06 14:13 monai/py.typed
 -rw-rw-r--  2.0 unx      642 b- defN 23-Sep-05 03:43 monai/_extensions/__init__.py
 -rw-rw-r--  2.0 unx     3643 b- defN 23-Sep-05 03:43 monai/_extensions/loader.py
 -rw-rw-r--  2.0 unx     2931 b- defN 23-Jan-06 02:58 monai/_extensions/gmm/gmm.cpp
 -rw-rw-r--  2.0 unx     1760 b- defN 22-Dec-06 14:13 monai/_extensions/gmm/gmm.h
 -rw-rw-r--  2.0 unx     1118 b- defN 22-Dec-06 14:13 monai/_extensions/gmm/gmm_cpu.cpp
 -rw-rw-r--  2.0 unx    15983 b- defN 23-Sep-06 15:49 monai/_extensions/gmm/gmm_cuda.cu
 -rw-rw-r--  2.0 unx     3520 b- defN 22-Dec-06 14:13 monai/_extensions/gmm/gmm_cuda_linalg.cuh
 -rw-rw-r--  2.0 unx      908 b- defN 23-Sep-05 03:43 monai/apps/__init__.py
--rw-rw-r--  2.0 unx    35085 b- defN 24-Feb-29 16:07 monai/apps/datasets.py
--rw-rw-r--  2.0 unx    14297 b- defN 24-Feb-29 16:07 monai/apps/utils.py
+-rw-rw-r--  2.0 unx    35085 b- defN 24-Apr-22 05:03 monai/apps/datasets.py
+-rw-rw-r--  2.0 unx    14452 b- defN 24-Apr-26 07:06 monai/apps/utils.py
 -rw-rw-r--  2.0 unx     1016 b- defN 23-Sep-06 15:49 monai/apps/auto3dseg/__init__.py
 -rw-rw-r--  2.0 unx     1411 b- defN 23-Sep-06 15:49 monai/apps/auto3dseg/__main__.py
--rw-rw-r--  2.0 unx    40110 b- defN 24-Apr-18 13:58 monai/apps/auto3dseg/auto_runner.py
--rw-rw-r--  2.0 unx    28994 b- defN 24-Feb-29 16:07 monai/apps/auto3dseg/bundle_gen.py
+-rw-rw-r--  2.0 unx    40110 b- defN 24-Apr-22 04:57 monai/apps/auto3dseg/auto_runner.py
+-rw-rw-r--  2.0 unx    28994 b- defN 24-Apr-22 04:57 monai/apps/auto3dseg/bundle_gen.py
 -rw-rw-r--  2.0 unx    18628 b- defN 24-Feb-19 03:12 monai/apps/auto3dseg/data_analyzer.py
--rw-rw-r--  2.0 unx    27277 b- defN 24-Feb-29 16:07 monai/apps/auto3dseg/ensemble_builder.py
--rw-rw-r--  2.0 unx    16674 b- defN 24-Apr-12 13:56 monai/apps/auto3dseg/hpo_gen.py
+-rw-rw-r--  2.0 unx    27277 b- defN 24-Apr-22 04:57 monai/apps/auto3dseg/ensemble_builder.py
+-rw-rw-r--  2.0 unx    16674 b- defN 24-Apr-22 04:57 monai/apps/auto3dseg/hpo_gen.py
 -rw-rw-r--  2.0 unx     3991 b- defN 23-Sep-06 15:49 monai/apps/auto3dseg/transforms.py
 -rw-rw-r--  2.0 unx     3138 b- defN 24-Jan-17 03:03 monai/apps/auto3dseg/utils.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/apps/deepedit/__init__.py
 -rw-rw-r--  2.0 unx     4501 b- defN 23-Sep-05 03:43 monai/apps/deepedit/interaction.py
--rw-rw-r--  2.0 unx    38119 b- defN 24-Feb-29 16:07 monai/apps/deepedit/transforms.py
+-rw-rw-r--  2.0 unx    38119 b- defN 24-Apr-22 05:03 monai/apps/deepedit/transforms.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/apps/deepgrow/__init__.py
 -rw-rw-r--  2.0 unx    10054 b- defN 23-Sep-05 03:43 monai/apps/deepgrow/dataset.py
 -rw-rw-r--  2.0 unx     3748 b- defN 24-Feb-19 03:12 monai/apps/deepgrow/interaction.py
 -rw-rw-r--  2.0 unx    41884 b- defN 23-Nov-07 11:06 monai/apps/deepgrow/transforms.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/apps/detection/__init__.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/apps/detection/metrics/__init__.py
--rw-rw-r--  2.0 unx    26618 b- defN 24-Feb-29 16:07 monai/apps/detection/metrics/coco.py
+-rw-rw-r--  2.0 unx    26618 b- defN 24-Apr-22 05:03 monai/apps/detection/metrics/coco.py
 -rw-rw-r--  2.0 unx    17161 b- defN 23-Sep-05 03:43 monai/apps/detection/metrics/matching.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/apps/detection/networks/__init__.py
 -rw-rw-r--  2.0 unx    53640 b- defN 23-Sep-06 15:49 monai/apps/detection/networks/retinanet_detector.py
 -rw-rw-r--  2.0 unx    19044 b- defN 23-Nov-07 11:06 monai/apps/detection/networks/retinanet_network.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/apps/detection/transforms/__init__.py
 -rw-rw-r--  2.0 unx    24519 b- defN 23-Sep-05 03:43 monai/apps/detection/transforms/array.py
 -rw-rw-r--  2.0 unx    18035 b- defN 24-Feb-19 03:12 monai/apps/detection/transforms/box_ops.py
 -rw-rw-r--  2.0 unx    69282 b- defN 23-Sep-06 15:49 monai/apps/detection/transforms/dictionary.py
--rw-rw-r--  2.0 unx    13532 b- defN 24-Feb-29 16:07 monai/apps/detection/utils/ATSS_matcher.py
+-rw-rw-r--  2.0 unx    13532 b- defN 24-Apr-22 05:03 monai/apps/detection/utils/ATSS_matcher.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/apps/detection/utils/__init__.py
--rw-rw-r--  2.0 unx    18732 b- defN 24-Feb-23 07:18 monai/apps/detection/utils/anchor_utils.py
+-rw-rw-r--  2.0 unx    18732 b- defN 24-Apr-22 04:59 monai/apps/detection/utils/anchor_utils.py
 -rw-rw-r--  2.0 unx    11120 b- defN 23-Sep-05 03:43 monai/apps/detection/utils/box_coder.py
 -rw-rw-r--  2.0 unx     9031 b- defN 23-Sep-05 03:43 monai/apps/detection/utils/box_selector.py
 -rw-rw-r--  2.0 unx    10306 b- defN 23-Sep-05 03:43 monai/apps/detection/utils/detector_utils.py
 -rw-rw-r--  2.0 unx    13890 b- defN 23-Sep-05 03:43 monai/apps/detection/utils/hard_negative_sampler.py
 -rw-rw-r--  2.0 unx     5818 b- defN 23-Sep-06 15:49 monai/apps/detection/utils/predict_utils.py
 -rw-rw-r--  2.0 unx      726 b- defN 23-Sep-05 03:43 monai/apps/mmars/__init__.py
 -rw-rw-r--  2.0 unx    13115 b- defN 23-Sep-05 03:43 monai/apps/mmars/mmars.py
 -rw-rw-r--  2.0 unx     9996 b- defN 23-Sep-05 03:43 monai/apps/mmars/model_desc.py
 -rw-rw-r--  2.0 unx      745 b- defN 23-Sep-05 03:43 monai/apps/nnunet/__init__.py
 -rw-rw-r--  2.0 unx      832 b- defN 23-Sep-06 15:49 monai/apps/nnunet/__main__.py
--rw-rw-r--  2.0 unx    48001 b- defN 24-Apr-12 13:56 monai/apps/nnunet/nnunetv2_runner.py
+-rw-rw-r--  2.0 unx    48001 b- defN 24-Apr-22 04:57 monai/apps/nnunet/nnunetv2_runner.py
 -rw-rw-r--  2.0 unx     6761 b- defN 23-Dec-18 15:02 monai/apps/nnunet/utils.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/apps/nuclick/__init__.py
 -rw-rw-r--  2.0 unx    24948 b- defN 23-Sep-05 03:43 monai/apps/nuclick/transforms.py
 -rw-rw-r--  2.0 unx     1030 b- defN 23-Sep-06 15:49 monai/apps/pathology/__init__.py
 -rw-rw-r--  2.0 unx     2860 b- defN 23-Sep-05 03:43 monai/apps/pathology/utils.py
 -rw-rw-r--  2.0 unx      650 b- defN 23-Sep-05 03:43 monai/apps/pathology/engines/__init__.py
 -rw-rw-r--  2.0 unx     2397 b- defN 23-Sep-05 03:43 monai/apps/pathology/engines/utils.py
@@ -66,15 +66,15 @@
 -rw-rw-r--  2.0 unx     9167 b- defN 23-Nov-07 11:06 monai/apps/pathology/inferers/inferer.py
 -rw-rw-r--  2.0 unx      650 b- defN 23-Sep-05 03:43 monai/apps/pathology/losses/__init__.py
 -rw-rw-r--  2.0 unx     7293 b- defN 23-Sep-05 03:43 monai/apps/pathology/losses/hovernet_loss.py
 -rw-rw-r--  2.0 unx      646 b- defN 23-Sep-05 03:43 monai/apps/pathology/metrics/__init__.py
 -rw-rw-r--  2.0 unx     7331 b- defN 24-Feb-19 03:12 monai/apps/pathology/metrics/lesion_froc.py
 -rw-rw-r--  2.0 unx     2243 b- defN 23-Sep-06 15:49 monai/apps/pathology/transforms/__init__.py
 -rw-rw-r--  2.0 unx     1995 b- defN 23-Sep-05 03:43 monai/apps/pathology/transforms/post/__init__.py
--rw-rw-r--  2.0 unx    37258 b- defN 24-Feb-29 16:07 monai/apps/pathology/transforms/post/array.py
+-rw-rw-r--  2.0 unx    37258 b- defN 24-Apr-22 04:57 monai/apps/pathology/transforms/post/array.py
 -rw-rw-r--  2.0 unx    25928 b- defN 23-Sep-06 15:49 monai/apps/pathology/transforms/post/dictionary.py
 -rw-rw-r--  2.0 unx      836 b- defN 23-Sep-05 03:43 monai/apps/pathology/transforms/stain/__init__.py
 -rw-rw-r--  2.0 unx     8366 b- defN 23-Sep-05 03:43 monai/apps/pathology/transforms/stain/array.py
 -rw-rw-r--  2.0 unx     4761 b- defN 23-Sep-05 03:43 monai/apps/pathology/transforms/stain/dictionary.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/apps/reconstruction/__init__.py
 -rw-rw-r--  2.0 unx     8393 b- defN 23-Sep-05 03:43 monai/apps/reconstruction/complex_utils.py
 -rw-rw-r--  2.0 unx     3644 b- defN 23-Sep-05 03:43 monai/apps/reconstruction/fastmri_reader.py
@@ -91,65 +91,65 @@
 -rw-rw-r--  2.0 unx    12240 b- defN 23-Sep-05 03:43 monai/apps/reconstruction/transforms/array.py
 -rw-rw-r--  2.0 unx    15829 b- defN 23-Sep-06 15:49 monai/apps/reconstruction/transforms/dictionary.py
 -rw-rw-r--  2.0 unx      824 b- defN 24-Feb-19 03:12 monai/apps/tcia/__init__.py
 -rw-rw-r--  2.0 unx     1582 b- defN 23-Sep-05 03:43 monai/apps/tcia/label_desc.py
 -rw-rw-r--  2.0 unx     6303 b- defN 24-Feb-19 03:12 monai/apps/tcia/utils.py
 -rw-rw-r--  2.0 unx     1164 b- defN 23-Sep-05 03:43 monai/auto3dseg/__init__.py
 -rw-rw-r--  2.0 unx     4286 b- defN 23-Sep-06 15:49 monai/auto3dseg/algo_gen.py
--rw-rw-r--  2.0 unx    41323 b- defN 24-Apr-12 13:56 monai/auto3dseg/analyzer.py
+-rw-rw-r--  2.0 unx    41323 b- defN 24-Apr-22 04:57 monai/auto3dseg/analyzer.py
 -rw-rw-r--  2.0 unx     5110 b- defN 23-Sep-05 03:43 monai/auto3dseg/operations.py
 -rw-rw-r--  2.0 unx     8717 b- defN 23-Nov-07 11:06 monai/auto3dseg/seg_summarizer.py
 -rw-rw-r--  2.0 unx    18674 b- defN 23-Nov-07 11:06 monai/auto3dseg/utils.py
 -rw-rw-r--  2.0 unx     1443 b- defN 24-Feb-19 03:12 monai/bundle/__init__.py
 -rw-rw-r--  2.0 unx      952 b- defN 23-Nov-07 11:06 monai/bundle/__main__.py
--rw-rw-r--  2.0 unx    16151 b- defN 24-Apr-12 13:56 monai/bundle/config_item.py
+-rw-rw-r--  2.0 unx    16151 b- defN 24-Apr-22 04:57 monai/bundle/config_item.py
 -rw-rw-r--  2.0 unx    22895 b- defN 23-Nov-29 14:56 monai/bundle/config_parser.py
 -rw-rw-r--  2.0 unx    11582 b- defN 24-Mar-26 15:04 monai/bundle/properties.py
 -rw-rw-r--  2.0 unx    15747 b- defN 23-Nov-29 14:56 monai/bundle/reference_resolver.py
--rw-rw-r--  2.0 unx    80520 b- defN 24-Apr-12 14:52 monai/bundle/scripts.py
--rw-rw-r--  2.0 unx     8927 b- defN 24-Apr-12 14:52 monai/bundle/utils.py
--rw-rw-r--  2.0 unx    24580 b- defN 24-Apr-12 14:52 monai/bundle/workflows.py
+-rw-rw-r--  2.0 unx    80520 b- defN 24-Apr-22 04:57 monai/bundle/scripts.py
+-rw-rw-r--  2.0 unx     8927 b- defN 24-Apr-22 04:57 monai/bundle/utils.py
+-rw-rw-r--  2.0 unx    24580 b- defN 24-Apr-22 04:57 monai/bundle/workflows.py
 -rw-rw-r--  2.0 unx     1048 b- defN 23-Sep-05 03:43 monai/config/__init__.py
 -rw-rw-r--  2.0 unx    10315 b- defN 24-Jan-17 03:03 monai/config/deviceconfig.py
 -rw-rw-r--  2.0 unx     3485 b- defN 23-Sep-05 03:43 monai/config/type_definitions.py
 -rw-rw-r--  2.0 unx     5167 b- defN 23-Nov-07 11:06 monai/data/__init__.py
 -rw-rw-r--  2.0 unx    50102 b- defN 23-Sep-05 03:43 monai/data/box_utils.py
 -rw-rw-r--  2.0 unx     4952 b- defN 23-Sep-05 03:43 monai/data/csv_saver.py
 -rw-rw-r--  2.0 unx     4459 b- defN 23-Nov-07 11:06 monai/data/dataloader.py
--rw-rw-r--  2.0 unx    79098 b- defN 24-Apr-12 13:56 monai/data/dataset.py
+-rw-rw-r--  2.0 unx    79098 b- defN 24-Apr-22 05:03 monai/data/dataset.py
 -rw-rw-r--  2.0 unx    10216 b- defN 23-Sep-05 03:43 monai/data/dataset_summary.py
--rw-rw-r--  2.0 unx    10310 b- defN 24-Feb-23 07:18 monai/data/decathlon_datalist.py
+-rw-rw-r--  2.0 unx    10310 b- defN 24-Apr-22 04:59 monai/data/decathlon_datalist.py
 -rw-rw-r--  2.0 unx     4448 b- defN 23-Sep-05 03:43 monai/data/fft_utils.py
 -rw-rw-r--  2.0 unx     6344 b- defN 23-Sep-05 03:43 monai/data/folder_layout.py
 -rw-rw-r--  2.0 unx    19483 b- defN 24-Feb-19 03:12 monai/data/grid_dataset.py
 -rw-rw-r--  2.0 unx     7008 b- defN 23-Sep-05 03:43 monai/data/image_dataset.py
 -rw-rw-r--  2.0 unx    61767 b- defN 24-Feb-21 06:47 monai/data/image_reader.py
 -rw-rw-r--  2.0 unx    39856 b- defN 24-Feb-19 03:12 monai/data/image_writer.py
 -rw-rw-r--  2.0 unx    13100 b- defN 23-Nov-20 07:53 monai/data/iterable_dataset.py
 -rw-rw-r--  2.0 unx    14461 b- defN 23-Nov-07 11:06 monai/data/itk_torch_bridge.py
 -rw-rw-r--  2.0 unx     8800 b- defN 23-Sep-05 03:43 monai/data/meta_obj.py
--rw-rw-r--  2.0 unx    27478 b- defN 24-Apr-18 14:39 monai/data/meta_tensor.py
+-rw-rw-r--  2.0 unx    27478 b- defN 24-Apr-23 07:34 monai/data/meta_tensor.py
 -rw-rw-r--  2.0 unx     5102 b- defN 23-Nov-07 11:06 monai/data/samplers.py
 -rw-rw-r--  2.0 unx     7375 b- defN 23-Sep-05 03:43 monai/data/synthetic.py
 -rw-rw-r--  2.0 unx     9780 b- defN 23-Sep-05 03:43 monai/data/test_time_augmentation.py
 -rw-rw-r--  2.0 unx     8840 b- defN 23-Sep-05 03:43 monai/data/thread_buffer.py
 -rw-rw-r--  2.0 unx     5500 b- defN 23-Sep-05 03:43 monai/data/torchscript_utils.py
 -rw-rw-r--  2.0 unx    13201 b- defN 23-Nov-07 11:06 monai/data/ultrasound_confidence_map.py
 -rw-rw-r--  2.0 unx    66686 b- defN 24-Feb-19 03:12 monai/data/utils.py
--rw-rw-r--  2.0 unx     9105 b- defN 24-Apr-18 13:58 monai/data/video_dataset.py
+-rw-rw-r--  2.0 unx     9105 b- defN 24-Apr-22 04:57 monai/data/video_dataset.py
 -rw-rw-r--  2.0 unx    18619 b- defN 23-Sep-06 15:49 monai/data/wsi_datasets.py
 -rw-rw-r--  2.0 unx    49478 b- defN 24-Feb-19 03:12 monai/data/wsi_reader.py
--rw-rw-r--  2.0 unx     1018 b- defN 23-Nov-07 11:06 monai/engines/__init__.py
+-rw-rw-r--  2.0 unx     1018 b- defN 24-Apr-22 04:57 monai/engines/__init__.py
 -rw-rw-r--  2.0 unx    26934 b- defN 24-Feb-21 06:47 monai/engines/evaluator.py
--rw-rw-r--  2.0 unx    23793 b- defN 24-Mar-01 09:30 monai/engines/trainer.py
--rw-rw-r--  2.0 unx    11631 b- defN 24-Jan-23 04:22 monai/engines/utils.py
+-rw-rw-r--  2.0 unx    23793 b- defN 24-Apr-22 04:57 monai/engines/trainer.py
+-rw-rw-r--  2.0 unx    11631 b- defN 24-Apr-22 04:57 monai/engines/utils.py
 -rw-rw-r--  2.0 unx    15250 b- defN 24-Feb-22 06:31 monai/engines/workflow.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/fl/__init__.py
 -rw-rw-r--  2.0 unx      725 b- defN 23-Sep-05 03:43 monai/fl/client/__init__.py
--rw-rw-r--  2.0 unx     5098 b- defN 24-Feb-29 16:07 monai/fl/client/client_algo.py
+-rw-rw-r--  2.0 unx     5098 b- defN 24-Apr-22 05:03 monai/fl/client/client_algo.py
 -rw-rw-r--  2.0 unx    33623 b- defN 24-Mar-26 14:58 monai/fl/client/monai_algo.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/fl/utils/__init__.py
 -rw-rw-r--  2.0 unx     1750 b- defN 23-Nov-07 11:06 monai/fl/utils/constants.py
 -rw-rw-r--  2.0 unx     3527 b- defN 23-Sep-05 03:43 monai/fl/utils/exchange_object.py
 -rw-rw-r--  2.0 unx     1633 b- defN 23-Sep-06 15:49 monai/fl/utils/filters.py
 -rw-rw-r--  2.0 unx     2372 b- defN 23-Nov-07 11:06 monai/handlers/__init__.py
 -rw-rw-r--  2.0 unx     7456 b- defN 23-Nov-07 11:06 monai/handlers/checkpoint_loader.py
@@ -157,15 +157,15 @@
 -rw-rw-r--  2.0 unx     7606 b- defN 23-Sep-05 03:43 monai/handlers/classification_saver.py
 -rw-rw-r--  2.0 unx     7518 b- defN 23-Nov-07 11:06 monai/handlers/clearml_handlers.py
 -rw-rw-r--  2.0 unx     4006 b- defN 23-Nov-07 11:06 monai/handlers/confusion_matrix.py
 -rw-rw-r--  2.0 unx     4425 b- defN 23-Sep-05 03:43 monai/handlers/decollate_batch.py
 -rw-rw-r--  2.0 unx     5334 b- defN 23-Nov-07 11:06 monai/handlers/earlystop_handler.py
 -rw-rw-r--  2.0 unx     3645 b- defN 23-Nov-07 11:06 monai/handlers/garbage_collector.py
 -rw-rw-r--  2.0 unx     3594 b- defN 23-Nov-07 11:06 monai/handlers/hausdorff_distance.py
--rw-rw-r--  2.0 unx     7461 b- defN 24-Feb-29 16:07 monai/handlers/ignite_metric.py
+-rw-rw-r--  2.0 unx     7461 b- defN 24-Apr-22 05:03 monai/handlers/ignite_metric.py
 -rw-rw-r--  2.0 unx     3931 b- defN 23-Sep-05 03:43 monai/handlers/logfile_handler.py
 -rw-rw-r--  2.0 unx     3575 b- defN 23-Sep-05 03:43 monai/handlers/lr_schedule_handler.py
 -rw-rw-r--  2.0 unx     3785 b- defN 24-Feb-19 03:12 monai/handlers/mean_dice.py
 -rw-rw-r--  2.0 unx     2841 b- defN 23-Nov-07 11:06 monai/handlers/mean_iou.py
 -rw-rw-r--  2.0 unx     5477 b- defN 23-Sep-05 03:43 monai/handlers/metric_logger.py
 -rw-rw-r--  2.0 unx     6195 b- defN 23-Nov-07 11:06 monai/handlers/metrics_reloaded_handler.py
 -rw-rw-r--  2.0 unx     8560 b- defN 23-Oct-11 14:05 monai/handlers/metrics_saver.py
@@ -179,211 +179,211 @@
 -rw-rw-r--  2.0 unx     2744 b- defN 23-Nov-07 11:06 monai/handlers/roc_auc.py
 -rw-rw-r--  2.0 unx     3051 b- defN 23-Sep-05 03:43 monai/handlers/smartcache_handler.py
 -rw-rw-r--  2.0 unx    14126 b- defN 23-Nov-07 11:06 monai/handlers/stats_handler.py
 -rw-rw-r--  2.0 unx     3327 b- defN 23-Nov-07 11:06 monai/handlers/surface_distance.py
 -rw-rw-r--  2.0 unx    22615 b- defN 24-Feb-02 11:00 monai/handlers/tensorboard_handlers.py
 -rw-rw-r--  2.0 unx    10239 b- defN 24-Feb-19 03:12 monai/handlers/utils.py
 -rw-rw-r--  2.0 unx     3698 b- defN 23-Nov-07 11:06 monai/handlers/validation_handler.py
--rw-rw-r--  2.0 unx      958 b- defN 23-Nov-07 11:06 monai/inferers/__init__.py
--rw-rw-r--  2.0 unx    34219 b- defN 24-Feb-19 06:38 monai/inferers/inferer.py
+-rw-rw-r--  2.0 unx      958 b- defN 24-Apr-22 04:57 monai/inferers/__init__.py
+-rw-rw-r--  2.0 unx    34219 b- defN 24-Apr-22 04:57 monai/inferers/inferer.py
 -rw-rw-r--  2.0 unx    15566 b- defN 23-Nov-07 11:06 monai/inferers/merger.py
 -rw-rw-r--  2.0 unx    21149 b- defN 23-Sep-06 15:49 monai/inferers/splitter.py
 -rw-rw-r--  2.0 unx    20386 b- defN 23-Nov-07 11:06 monai/inferers/utils.py
--rw-rw-r--  2.0 unx     1746 b- defN 24-Apr-12 13:56 monai/losses/__init__.py
+-rw-rw-r--  2.0 unx     1746 b- defN 24-Apr-22 04:57 monai/losses/__init__.py
 -rw-rw-r--  2.0 unx     7722 b- defN 23-Nov-07 11:06 monai/losses/adversarial_loss.py
--rw-rw-r--  2.0 unx     3613 b- defN 24-Apr-12 13:56 monai/losses/barlow_twins.py
+-rw-rw-r--  2.0 unx     3613 b- defN 24-Apr-22 04:57 monai/losses/barlow_twins.py
 -rw-rw-r--  2.0 unx     6328 b- defN 23-Nov-07 11:06 monai/losses/cldice.py
 -rw-rw-r--  2.0 unx     3261 b- defN 23-Nov-07 11:06 monai/losses/contrastive.py
 -rw-rw-r--  2.0 unx     9701 b- defN 24-Feb-21 06:47 monai/losses/deform.py
--rw-rw-r--  2.0 unx    51627 b- defN 24-Apr-12 13:56 monai/losses/dice.py
+-rw-rw-r--  2.0 unx    51627 b- defN 24-Apr-22 04:57 monai/losses/dice.py
 -rw-rw-r--  2.0 unx     3854 b- defN 23-Sep-06 15:49 monai/losses/ds_loss.py
--rw-rw-r--  2.0 unx    11772 b- defN 24-Apr-12 13:56 monai/losses/focal_loss.py
+-rw-rw-r--  2.0 unx    11772 b- defN 24-Apr-22 04:57 monai/losses/focal_loss.py
 -rw-rw-r--  2.0 unx     2795 b- defN 23-Sep-05 03:43 monai/losses/giou_loss.py
 -rw-rw-r--  2.0 unx    10697 b- defN 24-Feb-23 05:41 monai/losses/hausdorff_loss.py
--rw-rw-r--  2.0 unx    15460 b- defN 24-Feb-23 07:18 monai/losses/image_dissimilarity.py
+-rw-rw-r--  2.0 unx    15460 b- defN 24-Apr-22 04:59 monai/losses/image_dissimilarity.py
 -rw-rw-r--  2.0 unx     3636 b- defN 23-Sep-05 03:43 monai/losses/multi_scale.py
--rw-rw-r--  2.0 unx    17586 b- defN 24-Apr-12 13:56 monai/losses/perceptual.py
+-rw-rw-r--  2.0 unx    19468 b- defN 24-Apr-23 03:52 monai/losses/perceptual.py
 -rw-rw-r--  2.0 unx     2955 b- defN 23-Oct-07 12:44 monai/losses/spatial_mask.py
 -rw-rw-r--  2.0 unx     3368 b- defN 23-Nov-07 11:06 monai/losses/spectral_loss.py
 -rw-rw-r--  2.0 unx     5058 b- defN 23-Nov-07 11:06 monai/losses/ssim_loss.py
--rw-rw-r--  2.0 unx     8179 b- defN 24-Apr-12 13:56 monai/losses/sure_loss.py
+-rw-rw-r--  2.0 unx     8179 b- defN 24-Apr-22 04:57 monai/losses/sure_loss.py
 -rw-rw-r--  2.0 unx     6645 b- defN 23-Sep-05 03:43 monai/losses/tversky.py
 -rw-rw-r--  2.0 unx    10224 b- defN 23-Sep-05 03:43 monai/losses/unified_focal_loss.py
 -rw-rw-r--  2.0 unx     2174 b- defN 23-Nov-07 11:06 monai/metrics/__init__.py
 -rw-rw-r--  2.0 unx     8211 b- defN 23-Nov-02 09:47 monai/metrics/active_learning_metrics.py
 -rw-rw-r--  2.0 unx    15064 b- defN 24-Feb-19 03:12 monai/metrics/confusion_matrix.py
 -rw-rw-r--  2.0 unx     5578 b- defN 23-Sep-05 03:43 monai/metrics/cumulative_average.py
--rw-rw-r--  2.0 unx     3984 b- defN 24-Feb-29 16:07 monai/metrics/f_beta_score.py
+-rw-rw-r--  2.0 unx     3984 b- defN 24-Apr-22 05:03 monai/metrics/f_beta_score.py
 -rw-rw-r--  2.0 unx     4794 b- defN 23-Nov-07 11:06 monai/metrics/fid.py
 -rw-rw-r--  2.0 unx     7981 b- defN 23-Sep-06 15:49 monai/metrics/froc.py
 -rw-rw-r--  2.0 unx     8265 b- defN 23-Sep-19 03:23 monai/metrics/generalized_dice.py
 -rw-rw-r--  2.0 unx    11844 b- defN 24-Feb-19 03:12 monai/metrics/hausdorff_distance.py
 -rw-rw-r--  2.0 unx     4907 b- defN 23-Sep-06 15:49 monai/metrics/loss_metric.py
 -rw-rw-r--  2.0 unx    13475 b- defN 24-Feb-29 16:03 monai/metrics/meandice.py
 -rw-rw-r--  2.0 unx     7004 b- defN 24-Feb-19 03:12 monai/metrics/meaniou.py
--rw-rw-r--  2.0 unx    15203 b- defN 24-Apr-12 13:56 monai/metrics/metric.py
+-rw-rw-r--  2.0 unx    15203 b- defN 24-Apr-22 04:57 monai/metrics/metric.py
 -rw-rw-r--  2.0 unx     3299 b- defN 23-Nov-07 11:06 monai/metrics/mmd.py
 -rw-rw-r--  2.0 unx    13679 b- defN 23-Sep-05 03:43 monai/metrics/panoptic_quality.py
--rw-rw-r--  2.0 unx    26218 b- defN 24-Apr-12 13:56 monai/metrics/regression.py
+-rw-rw-r--  2.0 unx    26218 b- defN 24-Apr-22 04:57 monai/metrics/regression.py
 -rw-rw-r--  2.0 unx     8038 b- defN 23-Sep-25 14:21 monai/metrics/rocauc.py
 -rw-rw-r--  2.0 unx    15149 b- defN 24-Feb-19 03:12 monai/metrics/surface_dice.py
 -rw-rw-r--  2.0 unx     9727 b- defN 24-Feb-19 03:12 monai/metrics/surface_distance.py
 -rw-rw-r--  2.0 unx    46947 b- defN 24-Feb-29 15:54 monai/metrics/utils.py
 -rw-rw-r--  2.0 unx    11781 b- defN 23-Nov-02 13:07 monai/metrics/wrapper.py
 -rw-rw-r--  2.0 unx     1020 b- defN 23-Sep-06 15:49 monai/networks/__init__.py
--rw-rw-r--  2.0 unx    49607 b- defN 24-Apr-18 13:58 monai/networks/utils.py
--rw-rw-r--  2.0 unx     2134 b- defN 23-Sep-05 03:43 monai/networks/blocks/__init__.py
+-rw-rw-r--  2.0 unx    49645 b- defN 24-Apr-26 07:06 monai/networks/utils.py
+-rw-rw-r--  2.0 unx     2134 b- defN 24-Apr-22 04:57 monai/networks/blocks/__init__.py
 -rw-rw-r--  2.0 unx     4275 b- defN 23-Sep-05 03:43 monai/networks/blocks/acti_norm.py
 -rw-rw-r--  2.0 unx     5839 b- defN 23-Sep-05 03:43 monai/networks/blocks/activation.py
 -rw-rw-r--  2.0 unx     4380 b- defN 23-Sep-05 03:43 monai/networks/blocks/aspp.py
 -rw-rw-r--  2.0 unx     7488 b- defN 23-Sep-06 15:49 monai/networks/blocks/backbone_fpn_utils.py
 -rw-rw-r--  2.0 unx    11686 b- defN 23-Sep-05 03:43 monai/networks/blocks/convolutions.py
 -rw-rw-r--  2.0 unx     5009 b- defN 23-Sep-05 03:43 monai/networks/blocks/crf.py
 -rw-rw-r--  2.0 unx     4747 b- defN 23-Nov-07 11:06 monai/networks/blocks/denseblock.py
 -rw-rw-r--  2.0 unx     9255 b- defN 23-Sep-05 03:43 monai/networks/blocks/dints_block.py
 -rw-rw-r--  2.0 unx     2413 b- defN 23-Sep-05 03:43 monai/networks/blocks/downsample.py
--rw-rw-r--  2.0 unx    11063 b- defN 24-Feb-29 16:07 monai/networks/blocks/dynunet_block.py
+-rw-rw-r--  2.0 unx    11063 b- defN 24-Apr-22 05:03 monai/networks/blocks/dynunet_block.py
 -rw-rw-r--  2.0 unx     3669 b- defN 23-Sep-05 03:43 monai/networks/blocks/encoder.py
 -rw-rw-r--  2.0 unx     9024 b- defN 23-Sep-05 03:43 monai/networks/blocks/fcn.py
 -rw-rw-r--  2.0 unx    10554 b- defN 23-Nov-07 11:06 monai/networks/blocks/feature_pyramid_network.py
 -rw-rw-r--  2.0 unx     8263 b- defN 23-Sep-05 03:43 monai/networks/blocks/fft_utils_t.py
--rw-rw-r--  2.0 unx    11456 b- defN 24-Feb-29 16:07 monai/networks/blocks/localnet_block.py
+-rw-rw-r--  2.0 unx    11456 b- defN 24-Apr-22 05:03 monai/networks/blocks/localnet_block.py
 -rw-rw-r--  2.0 unx     2814 b- defN 23-Nov-07 11:06 monai/networks/blocks/mlp.py
--rw-rw-r--  2.0 unx     9248 b- defN 24-Apr-12 13:56 monai/networks/blocks/patchembedding.py
--rw-rw-r--  2.0 unx     4070 b- defN 24-Apr-12 13:56 monai/networks/blocks/pos_embed_utils.py
+-rw-rw-r--  2.0 unx     9248 b- defN 24-Apr-22 04:57 monai/networks/blocks/patchembedding.py
+-rw-rw-r--  2.0 unx     4070 b- defN 24-Apr-22 05:03 monai/networks/blocks/pos_embed_utils.py
 -rw-rw-r--  2.0 unx     8825 b- defN 23-Sep-05 03:43 monai/networks/blocks/regunet_block.py
 -rw-rw-r--  2.0 unx     3339 b- defN 23-Nov-07 11:06 monai/networks/blocks/segresnet_block.py
--rw-rw-r--  2.0 unx     3100 b- defN 24-Feb-19 06:35 monai/networks/blocks/selfattention.py
+-rw-rw-r--  2.0 unx     3100 b- defN 24-Apr-22 04:57 monai/networks/blocks/selfattention.py
 -rw-rw-r--  2.0 unx    12752 b- defN 23-Sep-05 03:43 monai/networks/blocks/squeeze_and_excitation.py
 -rw-rw-r--  2.0 unx     3814 b- defN 23-Sep-06 15:49 monai/networks/blocks/text_embedding.py
 -rw-rw-r--  2.0 unx     2323 b- defN 23-Nov-07 11:06 monai/networks/blocks/transformerblock.py
 -rw-rw-r--  2.0 unx     9049 b- defN 23-Sep-05 03:43 monai/networks/blocks/unetr_block.py
 -rw-rw-r--  2.0 unx    13312 b- defN 23-Sep-05 03:43 monai/networks/blocks/upsample.py
 -rw-rw-r--  2.0 unx     7255 b- defN 23-Nov-07 11:06 monai/networks/blocks/warp.py
--rw-rw-r--  2.0 unx     1612 b- defN 24-Apr-12 13:56 monai/networks/layers/__init__.py
--rw-rw-r--  2.0 unx     3717 b- defN 24-Apr-12 13:56 monai/networks/layers/conjugate_gradient.py
+-rw-rw-r--  2.0 unx     1612 b- defN 24-Apr-22 04:57 monai/networks/layers/__init__.py
+-rw-rw-r--  2.0 unx     3717 b- defN 24-Apr-22 04:57 monai/networks/layers/conjugate_gradient.py
 -rw-rw-r--  2.0 unx     8288 b- defN 23-Sep-05 03:43 monai/networks/layers/convutils.py
 -rw-rw-r--  2.0 unx     1802 b- defN 23-Sep-05 03:43 monai/networks/layers/drop_path.py
--rw-rw-r--  2.0 unx    15380 b- defN 24-Feb-19 03:12 monai/networks/layers/factories.py
+-rw-rw-r--  2.0 unx    15380 b- defN 24-Apr-22 04:57 monai/networks/layers/factories.py
 -rw-rw-r--  2.0 unx    17992 b- defN 23-Sep-05 03:43 monai/networks/layers/filtering.py
--rw-rw-r--  2.0 unx     3325 b- defN 24-Feb-29 16:07 monai/networks/layers/gmm.py
--rw-rw-r--  2.0 unx    28472 b- defN 24-Feb-29 16:07 monai/networks/layers/simplelayers.py
--rw-rw-r--  2.0 unx    25581 b- defN 24-Mar-14 08:35 monai/networks/layers/spatial_transforms.py
--rw-rw-r--  2.0 unx     4296 b- defN 23-Sep-05 03:43 monai/networks/layers/utils.py
+-rw-rw-r--  2.0 unx     3325 b- defN 24-Apr-22 05:03 monai/networks/layers/gmm.py
+-rw-rw-r--  2.0 unx    28472 b- defN 24-Apr-22 05:03 monai/networks/layers/simplelayers.py
+-rw-rw-r--  2.0 unx    25581 b- defN 24-Apr-22 05:03 monai/networks/layers/spatial_transforms.py
+-rw-rw-r--  2.0 unx     4296 b- defN 24-Apr-22 04:57 monai/networks/layers/utils.py
 -rw-rw-r--  2.0 unx     2253 b- defN 23-Sep-05 03:43 monai/networks/layers/weight_init.py
--rw-rw-r--  2.0 unx     3329 b- defN 24-Feb-19 03:12 monai/networks/nets/__init__.py
--rw-rw-r--  2.0 unx    21570 b- defN 24-Feb-29 16:07 monai/networks/nets/ahnet.py
--rw-rw-r--  2.0 unx     9206 b- defN 24-Feb-29 16:07 monai/networks/nets/attentionunet.py
+-rw-rw-r--  2.0 unx     3368 b- defN 24-Apr-23 07:34 monai/networks/nets/__init__.py
+-rw-rw-r--  2.0 unx    21570 b- defN 24-Apr-22 05:03 monai/networks/nets/ahnet.py
+-rw-rw-r--  2.0 unx     9206 b- defN 24-Apr-22 05:03 monai/networks/nets/attentionunet.py
 -rw-rw-r--  2.0 unx    12586 b- defN 23-Nov-07 11:06 monai/networks/nets/autoencoder.py
--rw-rw-r--  2.0 unx    10951 b- defN 24-Feb-29 16:07 monai/networks/nets/basic_unet.py
--rw-rw-r--  2.0 unx     7961 b- defN 24-Feb-29 16:07 monai/networks/nets/basic_unetplusplus.py
+-rw-rw-r--  2.0 unx    10951 b- defN 24-Apr-22 05:03 monai/networks/nets/basic_unet.py
+-rw-rw-r--  2.0 unx     7961 b- defN 24-Apr-22 05:03 monai/networks/nets/basic_unetplusplus.py
 -rw-rw-r--  2.0 unx     6293 b- defN 23-Sep-05 03:43 monai/networks/nets/classifier.py
 -rw-rw-r--  2.0 unx    23786 b- defN 23-Nov-07 11:06 monai/networks/nets/daf3d.py
--rw-rw-r--  2.0 unx    15823 b- defN 24-Feb-29 16:07 monai/networks/nets/densenet.py
--rw-rw-r--  2.0 unx    44775 b- defN 24-Feb-29 16:07 monai/networks/nets/dints.py
+-rw-rw-r--  2.0 unx    15823 b- defN 24-Apr-22 05:03 monai/networks/nets/densenet.py
+-rw-rw-r--  2.0 unx    44775 b- defN 24-Apr-22 05:03 monai/networks/nets/dints.py
 -rw-rw-r--  2.0 unx    18210 b- defN 23-Sep-05 03:43 monai/networks/nets/dynunet.py
--rw-rw-r--  2.0 unx    40671 b- defN 24-Feb-29 16:07 monai/networks/nets/efficientnet.py
--rw-rw-r--  2.0 unx    14147 b- defN 23-Sep-05 03:43 monai/networks/nets/flexible_unet.py
+-rw-rw-r--  2.0 unx    40671 b- defN 24-Apr-22 05:03 monai/networks/nets/efficientnet.py
+-rw-rw-r--  2.0 unx    14435 b- defN 24-Apr-23 07:34 monai/networks/nets/flexible_unet.py
 -rw-rw-r--  2.0 unx     7212 b- defN 23-Sep-05 03:43 monai/networks/nets/fullyconnectednet.py
 -rw-rw-r--  2.0 unx     6581 b- defN 23-Sep-05 03:43 monai/networks/nets/generator.py
--rw-rw-r--  2.0 unx     8883 b- defN 24-Feb-29 16:07 monai/networks/nets/highresnet.py
--rw-rw-r--  2.0 unx    28684 b- defN 24-Feb-29 16:07 monai/networks/nets/hovernet.py
--rw-rw-r--  2.0 unx     9813 b- defN 24-Feb-29 16:07 monai/networks/nets/milmodel.py
+-rw-rw-r--  2.0 unx     8883 b- defN 24-Apr-22 05:03 monai/networks/nets/highresnet.py
+-rw-rw-r--  2.0 unx    28684 b- defN 24-Apr-22 05:03 monai/networks/nets/hovernet.py
+-rw-rw-r--  2.0 unx     9813 b- defN 24-Apr-22 05:03 monai/networks/nets/milmodel.py
 -rw-rw-r--  2.0 unx     6102 b- defN 23-Sep-05 03:43 monai/networks/nets/netadapter.py
 -rw-rw-r--  2.0 unx    20220 b- defN 24-Feb-19 09:52 monai/networks/nets/quicknat.py
 -rw-rw-r--  2.0 unx     6482 b- defN 23-Nov-07 11:06 monai/networks/nets/regressor.py
--rw-rw-r--  2.0 unx    18664 b- defN 24-Feb-29 16:07 monai/networks/nets/regunet.py
--rw-rw-r--  2.0 unx    22089 b- defN 24-Feb-19 03:12 monai/networks/nets/resnet.py
+-rw-rw-r--  2.0 unx    18664 b- defN 24-Apr-22 05:03 monai/networks/nets/regunet.py
+-rw-rw-r--  2.0 unx    27339 b- defN 24-Apr-23 07:34 monai/networks/nets/resnet.py
 -rw-rw-r--  2.0 unx    13994 b- defN 23-Sep-05 03:43 monai/networks/nets/segresnet.py
 -rw-rw-r--  2.0 unx    15703 b- defN 23-Nov-07 11:06 monai/networks/nets/segresnet_ds.py
 -rw-rw-r--  2.0 unx    19289 b- defN 23-Sep-05 03:43 monai/networks/nets/senet.py
 -rw-rw-r--  2.0 unx    44811 b- defN 24-Feb-19 03:12 monai/networks/nets/swin_unetr.py
 -rw-rw-r--  2.0 unx     6309 b- defN 24-Mar-22 13:10 monai/networks/nets/torchvision_fc.py
 -rw-rw-r--  2.0 unx    15726 b- defN 24-Feb-21 06:47 monai/networks/nets/transchex.py
 -rw-rw-r--  2.0 unx    13627 b- defN 23-Nov-07 11:06 monai/networks/nets/unet.py
 -rw-rw-r--  2.0 unx     8545 b- defN 23-Nov-09 02:51 monai/networks/nets/unetr.py
 -rw-rw-r--  2.0 unx     6282 b- defN 23-Nov-07 11:06 monai/networks/nets/varautoencoder.py
 -rw-rw-r--  2.0 unx     6250 b- defN 24-Feb-19 06:54 monai/networks/nets/vit.py
 -rw-rw-r--  2.0 unx     6033 b- defN 23-Nov-07 11:06 monai/networks/nets/vitautoenc.py
--rw-rw-r--  2.0 unx    10820 b- defN 24-Feb-29 16:07 monai/networks/nets/vnet.py
+-rw-rw-r--  2.0 unx    10820 b- defN 24-Apr-22 05:03 monai/networks/nets/vnet.py
 -rw-rw-r--  2.0 unx    20811 b- defN 24-Feb-19 03:12 monai/networks/nets/voxelmorph.py
 -rw-rw-r--  2.0 unx      796 b- defN 23-Sep-05 03:43 monai/optimizers/__init__.py
--rw-rw-r--  2.0 unx    21954 b- defN 24-Feb-29 16:07 monai/optimizers/lr_finder.py
+-rw-rw-r--  2.0 unx    21954 b- defN 24-Apr-22 05:03 monai/optimizers/lr_finder.py
 -rw-rw-r--  2.0 unx     4082 b- defN 23-Nov-07 11:06 monai/optimizers/lr_scheduler.py
 -rw-rw-r--  2.0 unx     5677 b- defN 23-Nov-07 11:06 monai/optimizers/novograd.py
--rw-rw-r--  2.0 unx     4133 b- defN 24-Feb-29 16:07 monai/optimizers/utils.py
--rw-rw-r--  2.0 unx    16052 b- defN 24-Apr-12 13:56 monai/transforms/__init__.py
--rw-rw-r--  2.0 unx     8950 b- defN 24-Feb-29 16:07 monai/transforms/adaptors.py
+-rw-rw-r--  2.0 unx     4133 b- defN 24-Apr-22 05:03 monai/optimizers/utils.py
+-rw-rw-r--  2.0 unx    16052 b- defN 24-Apr-22 04:57 monai/transforms/__init__.py
+-rw-rw-r--  2.0 unx     8950 b- defN 24-Apr-22 05:03 monai/transforms/adaptors.py
 -rw-rw-r--  2.0 unx    37663 b- defN 24-Feb-02 14:06 monai/transforms/compose.py
 -rw-rw-r--  2.0 unx    18746 b- defN 24-Mar-07 06:00 monai/transforms/inverse.py
--rw-rw-r--  2.0 unx     7055 b- defN 24-Feb-29 16:07 monai/transforms/inverse_batch_transform.py
+-rw-rw-r--  2.0 unx     7055 b- defN 24-Apr-22 05:03 monai/transforms/inverse_batch_transform.py
 -rw-rw-r--  2.0 unx     3386 b- defN 23-Sep-05 03:43 monai/transforms/nvtx.py
 -rw-rw-r--  2.0 unx     3563 b- defN 23-Sep-06 15:49 monai/transforms/traits.py
 -rw-rw-r--  2.0 unx    21532 b- defN 24-Feb-02 14:04 monai/transforms/transform.py
--rw-rw-r--  2.0 unx    91619 b- defN 24-Apr-19 06:29 monai/transforms/utils.py
+-rw-rw-r--  2.0 unx    91658 b- defN 24-Apr-23 03:52 monai/transforms/utils.py
 -rw-rw-r--  2.0 unx    31121 b- defN 23-Nov-07 11:06 monai/transforms/utils_create_transform_ims.py
--rw-rw-r--  2.0 unx    18779 b- defN 24-Apr-12 13:56 monai/transforms/utils_pytorch_numpy_unification.py
+-rw-rw-r--  2.0 unx    18779 b- defN 24-Apr-22 04:57 monai/transforms/utils_pytorch_numpy_unification.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/transforms/croppad/__init__.py
 -rw-rw-r--  2.0 unx    74745 b- defN 24-Feb-19 03:12 monai/transforms/croppad/array.py
 -rw-rw-r--  2.0 unx     6138 b- defN 23-Sep-06 15:49 monai/transforms/croppad/batch.py
 -rw-rw-r--  2.0 unx    60722 b- defN 24-Feb-19 03:12 monai/transforms/croppad/dictionary.py
 -rw-rw-r--  2.0 unx    12628 b- defN 23-Sep-06 15:49 monai/transforms/croppad/functional.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/transforms/intensity/__init__.py
--rw-rw-r--  2.0 unx   120755 b- defN 24-Apr-12 13:56 monai/transforms/intensity/array.py
--rw-rw-r--  2.0 unx    85059 b- defN 24-Apr-12 13:56 monai/transforms/intensity/dictionary.py
+-rw-rw-r--  2.0 unx   120755 b- defN 24-Apr-24 02:57 monai/transforms/intensity/array.py
+-rw-rw-r--  2.0 unx    85059 b- defN 24-Apr-22 04:57 monai/transforms/intensity/dictionary.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/transforms/io/__init__.py
--rw-rw-r--  2.0 unx    25636 b- defN 24-Apr-18 14:39 monai/transforms/io/array.py
+-rw-rw-r--  2.0 unx    25636 b- defN 24-Apr-23 07:34 monai/transforms/io/array.py
 -rw-rw-r--  2.0 unx    17602 b- defN 23-Nov-07 11:06 monai/transforms/io/dictionary.py
 -rw-rw-r--  2.0 unx      573 b- defN 23-Sep-06 15:49 monai/transforms/lazy/__init__.py
 -rw-rw-r--  2.0 unx     1211 b- defN 23-Sep-06 15:49 monai/transforms/lazy/array.py
 -rw-rw-r--  2.0 unx     1571 b- defN 23-Sep-06 15:49 monai/transforms/lazy/dictionary.py
 -rw-rw-r--  2.0 unx    15183 b- defN 24-Feb-29 16:10 monai/transforms/lazy/functional.py
 -rw-rw-r--  2.0 unx     9840 b- defN 24-Feb-29 16:10 monai/transforms/lazy/utils.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/transforms/meta_utility/__init__.py
 -rw-rw-r--  2.0 unx     4896 b- defN 23-Sep-05 03:43 monai/transforms/meta_utility/dictionary.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/transforms/post/__init__.py
--rw-rw-r--  2.0 unx    44998 b- defN 24-Feb-29 16:07 monai/transforms/post/array.py
+-rw-rw-r--  2.0 unx    44998 b- defN 24-Apr-22 05:03 monai/transforms/post/array.py
 -rw-rw-r--  2.0 unx    43042 b- defN 24-Feb-19 03:12 monai/transforms/post/dictionary.py
--rw-rw-r--  2.0 unx      573 b- defN 24-Apr-12 13:56 monai/transforms/regularization/__init__.py
--rw-rw-r--  2.0 unx     6870 b- defN 24-Apr-12 13:56 monai/transforms/regularization/array.py
--rw-rw-r--  2.0 unx     3241 b- defN 24-Apr-12 13:56 monai/transforms/regularization/dictionary.py
+-rw-rw-r--  2.0 unx      573 b- defN 24-Apr-22 04:57 monai/transforms/regularization/__init__.py
+-rw-rw-r--  2.0 unx     6870 b- defN 24-Apr-24 02:57 monai/transforms/regularization/array.py
+-rw-rw-r--  2.0 unx     3241 b- defN 24-Apr-24 02:57 monai/transforms/regularization/dictionary.py
 -rw-rw-r--  2.0 unx      573 b- defN 23-Jan-06 02:58 monai/transforms/signal/__init__.py
 -rw-rw-r--  2.0 unx    16339 b- defN 23-Nov-07 11:06 monai/transforms/signal/array.py
 -rw-rw-r--  2.0 unx     2085 b- defN 23-Nov-07 11:06 monai/transforms/signal/dictionary.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/transforms/smooth_field/__init__.py
--rw-rw-r--  2.0 unx    17856 b- defN 24-Feb-21 06:47 monai/transforms/smooth_field/array.py
+-rw-rw-r--  2.0 unx    17856 b- defN 24-Apr-22 04:57 monai/transforms/smooth_field/array.py
 -rw-rw-r--  2.0 unx    11194 b- defN 23-Sep-05 03:43 monai/transforms/smooth_field/dictionary.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/transforms/spatial/__init__.py
--rw-rw-r--  2.0 unx   183231 b- defN 24-Mar-14 08:35 monai/transforms/spatial/array.py
+-rw-rw-r--  2.0 unx   183231 b- defN 24-Apr-22 04:57 monai/transforms/spatial/array.py
 -rw-rw-r--  2.0 unx   131672 b- defN 24-Feb-29 16:10 monai/transforms/spatial/dictionary.py
 -rw-rw-r--  2.0 unx    31249 b- defN 24-Mar-07 10:48 monai/transforms/spatial/functional.py
 -rw-rw-r--  2.0 unx      573 b- defN 22-Dec-06 14:13 monai/transforms/utility/__init__.py
 -rw-rw-r--  2.0 unx    70600 b- defN 24-Feb-21 06:47 monai/transforms/utility/array.py
--rw-rw-r--  2.0 unx    73114 b- defN 24-Feb-29 16:07 monai/transforms/utility/dictionary.py
--rw-rw-r--  2.0 unx     3726 b- defN 24-Mar-15 17:05 monai/utils/__init__.py
+-rw-rw-r--  2.0 unx    73114 b- defN 24-Apr-22 05:03 monai/transforms/utility/dictionary.py
+-rw-rw-r--  2.0 unx     3726 b- defN 24-Apr-22 04:57 monai/utils/__init__.py
 -rw-rw-r--  2.0 unx     4096 b- defN 23-Sep-06 15:49 monai/utils/aliases.py
 -rw-rw-r--  2.0 unx     4498 b- defN 24-Feb-19 03:12 monai/utils/component_store.py
 -rw-rw-r--  2.0 unx     3129 b- defN 23-Sep-05 03:43 monai/utils/decorators.py
 -rw-rw-r--  2.0 unx    14759 b- defN 23-Sep-05 03:43 monai/utils/deprecate_utils.py
--rw-rw-r--  2.0 unx     8639 b- defN 24-Feb-23 07:18 monai/utils/dist.py
--rw-rw-r--  2.0 unx    19674 b- defN 24-Apr-18 14:39 monai/utils/enums.py
+-rw-rw-r--  2.0 unx     8639 b- defN 24-Apr-22 04:59 monai/utils/dist.py
+-rw-rw-r--  2.0 unx    19674 b- defN 24-Apr-23 07:34 monai/utils/enums.py
 -rw-rw-r--  2.0 unx    15651 b- defN 23-Nov-07 11:06 monai/utils/jupyter_utils.py
--rw-rw-r--  2.0 unx    30908 b- defN 24-Apr-19 05:52 monai/utils/misc.py
--rw-rw-r--  2.0 unx    25008 b- defN 24-Apr-12 13:56 monai/utils/module.py
+-rw-rw-r--  2.0 unx    30908 b- defN 24-Apr-24 02:57 monai/utils/misc.py
+-rw-rw-r--  2.0 unx    25008 b- defN 24-Apr-22 05:03 monai/utils/module.py
 -rw-rw-r--  2.0 unx     6876 b- defN 23-Sep-05 03:43 monai/utils/nvtx.py
--rw-rw-r--  2.0 unx    15937 b- defN 24-Feb-29 16:07 monai/utils/profiling.py
+-rw-rw-r--  2.0 unx    15937 b- defN 24-Apr-22 05:03 monai/utils/profiling.py
 -rw-rw-r--  2.0 unx     5955 b- defN 23-Sep-05 03:43 monai/utils/state_cacher.py
 -rw-rw-r--  2.0 unx     3141 b- defN 23-Nov-07 11:06 monai/utils/tf32.py
 -rw-rw-r--  2.0 unx    21520 b- defN 23-Nov-07 11:06 monai/utils/type_conversion.py
 -rw-rw-r--  2.0 unx     1038 b- defN 23-Sep-05 03:43 monai/visualize/__init__.py
--rw-rw-r--  2.0 unx    16158 b- defN 24-Mar-04 06:50 monai/visualize/class_activation_maps.py
--rw-rw-r--  2.0 unx     6278 b- defN 24-Feb-29 16:07 monai/visualize/gradient_based.py
+-rw-rw-r--  2.0 unx    16158 b- defN 24-Apr-22 05:03 monai/visualize/class_activation_maps.py
+-rw-rw-r--  2.0 unx     6278 b- defN 24-Apr-22 05:03 monai/visualize/gradient_based.py
 -rw-rw-r--  2.0 unx     9200 b- defN 23-Sep-05 03:43 monai/visualize/img2tensorboard.py
 -rw-rw-r--  2.0 unx    18160 b- defN 23-Nov-07 11:06 monai/visualize/occlusion_sensitivity.py
 -rw-rw-r--  2.0 unx     9966 b- defN 23-Sep-05 03:43 monai/visualize/utils.py
 -rw-rw-r--  2.0 unx     1377 b- defN 23-Sep-05 03:43 monai/visualize/visualizer.py
--rw-rw-r--  2.0 unx    11357 b- defN 24-Apr-19 06:53 monai-1.3.1rc5.dist-info/LICENSE
--rw-rw-r--  2.0 unx    10915 b- defN 24-Apr-19 06:53 monai-1.3.1rc5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-19 06:53 monai-1.3.1rc5.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-19 06:53 monai-1.3.1rc5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    34644 b- defN 24-Apr-19 06:53 monai-1.3.1rc5.dist-info/RECORD
-387 files, 5232835 bytes uncompressed, 1312107 bytes compressed:  74.9%
+-rw-rw-r--  2.0 unx    11357 b- defN 24-Apr-26 07:07 monai-1.3.1rc6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    10915 b- defN 24-Apr-26 07:07 monai-1.3.1rc6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-26 07:07 monai-1.3.1rc6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-26 07:07 monai-1.3.1rc6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    34644 b- defN 24-Apr-26 07:07 monai-1.3.1rc6.dist-info/RECORD
+387 files, 5240526 bytes uncompressed, 1313809 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -1140,23 +1140,23 @@
 
 Filename: monai/visualize/utils.py
 Comment: 
 
 Filename: monai/visualize/visualizer.py
 Comment: 
 
-Filename: monai-1.3.1rc5.dist-info/LICENSE
+Filename: monai-1.3.1rc6.dist-info/LICENSE
 Comment: 
 
-Filename: monai-1.3.1rc5.dist-info/METADATA
+Filename: monai-1.3.1rc6.dist-info/METADATA
 Comment: 
 
-Filename: monai-1.3.1rc5.dist-info/WHEEL
+Filename: monai-1.3.1rc6.dist-info/WHEEL
 Comment: 
 
-Filename: monai-1.3.1rc5.dist-info/top_level.txt
+Filename: monai-1.3.1rc6.dist-info/top_level.txt
 Comment: 
 
-Filename: monai-1.3.1rc5.dist-info/RECORD
+Filename: monai-1.3.1rc6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## monai/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-04-19T14:11:26+0800",
+ "date": "2024-04-26T13:18:06+0800",
  "dirty": false,
  "error": null,
- "full-revisionid": "224c47a5741f0e0b454b6ffda5a65bf598af6a7c",
- "version": "1.3.1rc5"
+ "full-revisionid": "6a130cc7f659efe66cf651369e35d4a93b2ec28a",
+ "version": "1.3.1rc6"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## monai/apps/utils.py

```diff
@@ -131,15 +131,20 @@
             See also: :py:data:`monai.apps.utils.SUPPORTED_HASH_TYPES`.
 
     """
     if val is None:
         logger.info(f"Expected {hash_type} is None, skip {hash_type} check for file {filepath}.")
         return True
     actual_hash_func = look_up_option(hash_type.lower(), SUPPORTED_HASH_TYPES)
-    actual_hash = actual_hash_func()
+
+    if sys.version_info >= (3, 9):
+        actual_hash = actual_hash_func(usedforsecurity=False)  # allows checks on FIPS enabled machines
+    else:
+        actual_hash = actual_hash_func()
+
     try:
         with open(filepath, "rb") as f:
             for chunk in iter(lambda: f.read(1024 * 1024), b""):
                 actual_hash.update(chunk)
     except Exception as e:
         logger.error(f"Exception in check_hash: {e}")
         return False
```

## monai/losses/perceptual.py

```diff
@@ -41,14 +41,15 @@
     Open Radiologic Deep Learning Research Dataset for Effective Transfer Learning"
     https://pubs.rsna.org/doi/full/10.1148/ryai.210315 ; MedicalNet from Chen et al. "Med3D: Transfer Learning for
     3D Medical Image Analysis" https://arxiv.org/abs/1904.00625 ;
     and ResNet50 from Torchvision: https://pytorch.org/vision/main/models/generated/torchvision.models.resnet50.html .
 
     The fake 3D implementation is based on a 2.5D approach where we calculate the 2D perceptual loss on slices from all
     three axes and average. The full 3D approach uses a 3D network to calculate the perceptual loss.
+    MedicalNet networks are only compatible with 3D inputs and support channel-wise loss.
 
     Args:
         spatial_dims: number of spatial dimensions.
         network_type: {``"alex"``, ``"vgg"``, ``"squeeze"``, ``"radimagenet_resnet50"``,
         ``"medicalnet_resnet10_23datasets"``, ``"medicalnet_resnet50_23datasets"``, ``"resnet50"``}
             Specifies the network architecture to use. Defaults to ``"alex"``.
         is_fake_3d: if True use 2.5D approach for a 3D perceptual loss.
@@ -58,38 +59,44 @@
             LIPIS or Torchvision. Defaults to ``"True"``.
         pretrained_path: if `pretrained` is `True`, users can specify a weights file to be loaded
             via using this argument. This argument only works when ``"network_type"`` is "resnet50".
             Defaults to `None`.
         pretrained_state_dict_key: if `pretrained_path` is not `None`, this argument is used to
             extract the expected state dict. This argument only works when ``"network_type"`` is "resnet50".
             Defaults to `None`.
+        channel_wise: if True, the loss is returned per channel. Otherwise the loss is averaged over the channels.
+                Defaults to ``False``.
     """
 
     def __init__(
         self,
         spatial_dims: int,
         network_type: str = PercetualNetworkType.alex,
         is_fake_3d: bool = True,
         fake_3d_ratio: float = 0.5,
         cache_dir: str | None = None,
         pretrained: bool = True,
         pretrained_path: str | None = None,
         pretrained_state_dict_key: str | None = None,
+        channel_wise: bool = False,
     ):
         super().__init__()
 
         if spatial_dims not in [2, 3]:
             raise NotImplementedError("Perceptual loss is implemented only in 2D and 3D.")
 
         if (spatial_dims == 2 or is_fake_3d) and "medicalnet_" in network_type:
             raise ValueError(
                 "MedicalNet networks are only compatible with ``spatial_dims=3``."
                 "Argument is_fake_3d must be set to False."
             )
 
+        if channel_wise and "medicalnet_" not in network_type:
+            raise ValueError("Channel-wise loss is only compatible with MedicalNet networks.")
+
         if network_type.lower() not in list(PercetualNetworkType):
             raise ValueError(
                 "Unrecognised criterion entered for Adversarial Loss. Must be one in: %s"
                 % ", ".join(PercetualNetworkType)
             )
 
         if cache_dir:
@@ -98,28 +105,31 @@
             warnings.warn(
                 f"Setting cache_dir to {cache_dir}, this may change the default cache dir for all torch.hub calls."
             )
 
         self.spatial_dims = spatial_dims
         self.perceptual_function: nn.Module
         if spatial_dims == 3 and is_fake_3d is False:
-            self.perceptual_function = MedicalNetPerceptualSimilarity(net=network_type, verbose=False)
+            self.perceptual_function = MedicalNetPerceptualSimilarity(
+                net=network_type, verbose=False, channel_wise=channel_wise
+            )
         elif "radimagenet_" in network_type:
             self.perceptual_function = RadImageNetPerceptualSimilarity(net=network_type, verbose=False)
         elif network_type == "resnet50":
             self.perceptual_function = TorchvisionModelPerceptualSimilarity(
                 net=network_type,
                 pretrained=pretrained,
                 pretrained_path=pretrained_path,
                 pretrained_state_dict_key=pretrained_state_dict_key,
             )
         else:
             self.perceptual_function = LPIPS(pretrained=pretrained, net=network_type, verbose=False)
         self.is_fake_3d = is_fake_3d
         self.fake_3d_ratio = fake_3d_ratio
+        self.channel_wise = channel_wise
 
     def _calculate_axis_loss(self, input: torch.Tensor, target: torch.Tensor, spatial_axis: int) -> torch.Tensor:
         """
         Calculate perceptual loss in one of the axis used in the 2.5D approach. After the slices of one spatial axis
         is transformed into different instances in the batch, we compute the loss using the 2D approach.
 
         Args:
@@ -168,62 +178,95 @@
             loss_coronal = self._calculate_axis_loss(input, target, spatial_axis=3)
             loss_axial = self._calculate_axis_loss(input, target, spatial_axis=4)
             loss = loss_sagittal + loss_axial + loss_coronal
         else:
             # 2D and real 3D cases
             loss = self.perceptual_function(input, target)
 
-        return torch.mean(loss)
+        if self.channel_wise:
+            loss = torch.mean(loss.squeeze(), dim=0)
+        else:
+            loss = torch.mean(loss)
+
+        return loss
 
 
 class MedicalNetPerceptualSimilarity(nn.Module):
     """
     Component to perform the perceptual evaluation with the networks pretrained by Chen, et al. "Med3D: Transfer
     Learning for 3D Medical Image Analysis". This class uses torch Hub to download the networks from
     "Warvito/MedicalNet-models".
 
     Args:
         net: {``"medicalnet_resnet10_23datasets"``, ``"medicalnet_resnet50_23datasets"``}
             Specifies the network architecture to use. Defaults to ``"medicalnet_resnet10_23datasets"``.
         verbose: if false, mute messages from torch Hub load function.
+        channel_wise: if True, the loss is returned per channel. Otherwise the loss is averaged over the channels.
+                Defaults to ``False``.
     """
 
-    def __init__(self, net: str = "medicalnet_resnet10_23datasets", verbose: bool = False) -> None:
+    def __init__(
+        self, net: str = "medicalnet_resnet10_23datasets", verbose: bool = False, channel_wise: bool = False
+    ) -> None:
         super().__init__()
         torch.hub._validate_not_a_forked_repo = lambda a, b, c: True
         self.model = torch.hub.load("warvito/MedicalNet-models", model=net, verbose=verbose)
         self.eval()
 
+        self.channel_wise = channel_wise
+
         for param in self.parameters():
             param.requires_grad = False
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         """
         Compute perceptual loss using MedicalNet 3D networks. The input and target tensors are inputted in the
         pre-trained MedicalNet that is used for feature extraction. Then, these extracted features are normalised across
         the channels. Finally, we compute the difference between the input and target features and calculate the mean
         value from the spatial dimensions to obtain the perceptual loss.
 
         Args:
             input: 3D input tensor with shape BCDHW.
             target: 3D target tensor with shape BCDHW.
+
         """
         input = medicalnet_intensity_normalisation(input)
         target = medicalnet_intensity_normalisation(target)
 
         # Get model outputs
-        outs_input = self.model.forward(input)
-        outs_target = self.model.forward(target)
+        feats_per_ch = 0
+        for ch_idx in range(input.shape[1]):
+            input_channel = input[:, ch_idx, ...].unsqueeze(1)
+            target_channel = target[:, ch_idx, ...].unsqueeze(1)
+
+            if ch_idx == 0:
+                outs_input = self.model.forward(input_channel)
+                outs_target = self.model.forward(target_channel)
+                feats_per_ch = outs_input.shape[1]
+            else:
+                outs_input = torch.cat([outs_input, self.model.forward(input_channel)], dim=1)
+                outs_target = torch.cat([outs_target, self.model.forward(target_channel)], dim=1)
 
         # Normalise through the channels
         feats_input = normalize_tensor(outs_input)
         feats_target = normalize_tensor(outs_target)
 
-        results: torch.Tensor = (feats_input - feats_target) ** 2
-        results = spatial_average_3d(results.sum(dim=1, keepdim=True), keepdim=True)
+        feats_diff: torch.Tensor = (feats_input - feats_target) ** 2
+        if self.channel_wise:
+            results = torch.zeros(
+                feats_diff.shape[0], input.shape[1], feats_diff.shape[2], feats_diff.shape[3], feats_diff.shape[4]
+            )
+            for i in range(input.shape[1]):
+                l_idx = i * feats_per_ch
+                r_idx = (i + 1) * feats_per_ch
+                results[:, i, ...] = feats_diff[:, l_idx : i + r_idx, ...].sum(dim=1)
+        else:
+            results = feats_diff.sum(dim=1, keepdim=True)
+
+        results = spatial_average_3d(results, keepdim=True)
 
         return results
 
 
 def spatial_average_3d(x: torch.Tensor, keepdim: bool = True) -> torch.Tensor:
     return x.mean([2, 3, 4], keepdim=keepdim)
```

## monai/networks/utils.py

```diff
@@ -982,14 +982,15 @@
                     )
                 ]
                 trt_model = torch_tensorrt.compile(
                     ir_model,
                     inputs=input_placeholder,
                     enabled_precisions=convert_precision,
                     device=target_device,
+                    ir="torchscript",
                     **kwargs,
                 )
 
     # verify the outputs between the TensorRT model and PyTorch model
     if verify:
         if inputs is None:
             raise ValueError("Missing input data for verification.")
```

## monai/networks/nets/__init__.py

```diff
@@ -55,14 +55,16 @@
 from .quicknat import Quicknat
 from .regressor import Regressor
 from .regunet import GlobalNet, LocalNet, RegUNet
 from .resnet import (
     ResNet,
     ResNetBlock,
     ResNetBottleneck,
+    ResNetEncoder,
+    ResNetFeatures,
     get_medicalnet_pretrained_resnet_args,
     get_pretrained_resnet_medicalnet,
     resnet10,
     resnet18,
     resnet34,
     resnet50,
     resnet101,
```

## monai/networks/nets/flexible_unet.py

```diff
@@ -20,14 +20,15 @@
 from torch import nn
 
 from monai.networks.blocks import BaseEncoder, UpSample
 from monai.networks.layers.factories import Conv
 from monai.networks.layers.utils import get_act_layer
 from monai.networks.nets import EfficientNetEncoder
 from monai.networks.nets.basic_unet import UpCat
+from monai.networks.nets.resnet import ResNetEncoder
 from monai.utils import InterpolateMode, optional_import
 
 __all__ = ["FlexibleUNet", "FlexUNet", "FLEXUNET_BACKBONE", "FlexUNetEncoderRegister"]
 
 
 class FlexUNetEncoderRegister:
     """
@@ -74,14 +75,15 @@
                 "parameter": parameter_list[cnt],
             }
             self.register_dict[name_string] = cur_dict
 
 
 FLEXUNET_BACKBONE = FlexUNetEncoderRegister()
 FLEXUNET_BACKBONE.register_class(EfficientNetEncoder)
+FLEXUNET_BACKBONE.register_class(ResNetEncoder)
 
 
 class UNetDecoder(nn.Module):
     """
     UNet Decoder.
     This class refers to `segmentation_models.pytorch
     <https://github.com/qubvel/segmentation_models.pytorch>`_.
@@ -234,28 +236,29 @@
         upsample: str = "nontrainable",
         pre_conv: str = "default",
         interp_mode: str = "nearest",
         is_pad: bool = True,
     ) -> None:
         """
         A flexible implement of UNet, in which the backbone/encoder can be replaced with
-        any efficient network. Currently the input must have a 2 or 3 spatial dimension
+        any efficient or residual network. Currently the input must have a 2 or 3 spatial dimension
         and the spatial size of each dimension must be a multiple of 32 if is_pad parameter
         is False.
         Please notice each output of backbone must be 2x downsample in spatial dimension
         of last output. For example, if given a 512x256 2D image and a backbone with 4 outputs.
         Spatial size of each encoder output should be 256x128, 128x64, 64x32 and 32x16.
 
         Args:
             in_channels: number of input channels.
             out_channels: number of output channels.
-            backbone: name of backbones to initialize, only support efficientnet right now,
-                can be from [efficientnet-b0,..., efficientnet-b8, efficientnet-l2].
-            pretrained: whether to initialize pretrained ImageNet weights, only available
-                for spatial_dims=2 and batch norm is used, default to False.
+            backbone: name of backbones to initialize, only support efficientnet and resnet right now,
+                can be from [efficientnet-b0, ..., efficientnet-b8, efficientnet-l2, resnet10, ..., resnet200].
+            pretrained: whether to initialize pretrained weights. ImageNet weights are available for efficient networks
+                if spatial_dims=2 and batch norm is used. MedicalNet weights are available for residual networks
+                if spatial_dims=3 and in_channels=1. Default to False.
             decoder_channels: number of output channels for all feature maps in decoder.
                 `len(decoder_channels)` should equal to `len(encoder_channels) - 1`,default
                 to (256, 128, 64, 32, 16).
             spatial_dims: number of spatial dimensions, default to 2.
             norm: normalization type and arguments, default to ("batch", {"eps": 1e-3,
                 "momentum": 0.1}).
             act: activation type and arguments, default to ("relu", {"inplace": True}).
```

## monai/networks/nets/resnet.py

```diff
@@ -17,14 +17,15 @@
 from functools import partial
 from pathlib import Path
 from typing import Any
 
 import torch
 import torch.nn as nn
 
+from monai.networks.blocks.encoder import BaseEncoder
 from monai.networks.layers.factories import Conv, Norm, Pool
 from monai.networks.layers.utils import get_pool_layer
 from monai.utils import ensure_tuple_rep
 from monai.utils.module import look_up_option, optional_import
 
 hf_hub_download, _ = optional_import("huggingface_hub", name="hf_hub_download")
 EntryNotFoundError, _ = optional_import("huggingface_hub.utils._errors", name="EntryNotFoundError")
@@ -41,14 +42,27 @@
     "resnet34",
     "resnet50",
     "resnet101",
     "resnet152",
     "resnet200",
 ]
 
+
+resnet_params = {
+    # model_name: (block, layers, shortcut_type, bias_downsample, datasets23)
+    "resnet10": ("basic", [1, 1, 1, 1], "B", False, True),
+    "resnet18": ("basic", [2, 2, 2, 2], "A", True, True),
+    "resnet34": ("basic", [3, 4, 6, 3], "A", True, True),
+    "resnet50": ("bottleneck", [3, 4, 6, 3], "B", False, True),
+    "resnet101": ("bottleneck", [3, 4, 23, 3], "B", False, False),
+    "resnet152": ("bottleneck", [3, 8, 36, 3], "B", False, False),
+    "resnet200": ("bottleneck", [3, 24, 36, 3], "B", False, False),
+}
+
+
 logger = logging.getLogger(__name__)
 
 
 def get_inplanes():
     return [64, 128, 256, 512]
 
 
@@ -331,14 +345,128 @@
         x = x.view(x.size(0), -1)
         if self.fc is not None:
             x = self.fc(x)
 
         return x
 
 
+class ResNetFeatures(ResNet):
+
+    def __init__(self, model_name: str, pretrained: bool = True, spatial_dims: int = 3, in_channels: int = 1) -> None:
+        """Initialize resnet18 to resnet200 models as a backbone, the backbone can be used as an encoder for
+        segmentation and objection models.
+
+        Compared with the class `ResNet`, the only different place is the forward function.
+
+        Args:
+            model_name: name of model to initialize, can be from [resnet10, ..., resnet200].
+            pretrained: whether to initialize pretrained MedicalNet weights,
+                only available for spatial_dims=3 and in_channels=1.
+            spatial_dims: number of spatial dimensions of the input image.
+            in_channels: number of input channels for first convolutional layer.
+        """
+        if model_name not in resnet_params:
+            model_name_string = ", ".join(resnet_params.keys())
+            raise ValueError(f"invalid model_name {model_name} found, must be one of {model_name_string} ")
+
+        block, layers, shortcut_type, bias_downsample, datasets23 = resnet_params[model_name]
+
+        super().__init__(
+            block=block,
+            layers=layers,
+            block_inplanes=get_inplanes(),
+            spatial_dims=spatial_dims,
+            n_input_channels=in_channels,
+            conv1_t_stride=2,
+            shortcut_type=shortcut_type,
+            feed_forward=False,
+            bias_downsample=bias_downsample,
+        )
+        if pretrained:
+            if spatial_dims == 3 and in_channels == 1:
+                _load_state_dict(self, model_name, datasets23=datasets23)
+            else:
+                raise ValueError("Pretrained resnet models are only available for in_channels=1 and spatial_dims=3.")
+
+    def forward(self, inputs: torch.Tensor):
+        """
+        Args:
+            inputs: input should have spatially N dimensions
+            ``(Batch, in_channels, dim_0[, dim_1, ..., dim_N])``, N is defined by `dimensions`.
+
+        Returns:
+            a list of torch Tensors.
+        """
+        x = self.conv1(inputs)
+        x = self.bn1(x)
+        x = self.relu(x)
+
+        features = []
+        features.append(x)
+
+        if not self.no_max_pool:
+            x = self.maxpool(x)
+
+        x = self.layer1(x)
+        features.append(x)
+
+        x = self.layer2(x)
+        features.append(x)
+
+        x = self.layer3(x)
+        features.append(x)
+
+        x = self.layer4(x)
+        features.append(x)
+
+        return features
+
+
+class ResNetEncoder(ResNetFeatures, BaseEncoder):
+    """Wrap the original resnet to an encoder for flexible-unet."""
+
+    backbone_names = ["resnet10", "resnet18", "resnet34", "resnet50", "resnet101", "resnet152", "resnet200"]
+
+    @classmethod
+    def get_encoder_parameters(cls) -> list[dict]:
+        """Get the initialization parameter for resnet backbones."""
+        parameter_list = []
+        for backbone_name in cls.backbone_names:
+            parameter_list.append(
+                {"model_name": backbone_name, "pretrained": True, "spatial_dims": 3, "in_channels": 1}
+            )
+        return parameter_list
+
+    @classmethod
+    def num_channels_per_output(cls) -> list[tuple[int, ...]]:
+        """Get number of resnet backbone output feature maps channel."""
+        return [
+            (64, 64, 128, 256, 512),
+            (64, 64, 128, 256, 512),
+            (64, 64, 128, 256, 512),
+            (64, 256, 512, 1024, 2048),
+            (64, 256, 512, 1024, 2048),
+            (64, 256, 512, 1024, 2048),
+            (64, 256, 512, 1024, 2048),
+        ]
+
+    @classmethod
+    def num_outputs(cls) -> list[int]:
+        """Get number of resnet backbone output feature maps.
+
+        Since every backbone contains the same 5 output feature maps, the number list should be `[5] * 7`.
+        """
+        return [5] * 7
+
+    @classmethod
+    def get_encoder_names(cls) -> list[str]:
+        """Get names of resnet backbones."""
+        return cls.backbone_names
+
+
 def _resnet(
     arch: str,
     block: type[ResNetBlock | ResNetBottleneck],
     layers: list[int],
     block_inplanes: list[int],
     pretrained: bool | str,
     progress: bool,
@@ -473,15 +601,15 @@
         progress (bool): If True, displays a progress bar of the download to stderr
     """
     return _resnet("resnet200", ResNetBottleneck, [3, 24, 36, 3], get_inplanes(), pretrained, progress, **kwargs)
 
 
 def get_pretrained_resnet_medicalnet(resnet_depth: int, device: str = "cpu", datasets23: bool = True):
     """
-    Donwlad resnet pretrained weights from https://huggingface.co/TencentMedicalNet
+    Download resnet pretrained weights from https://huggingface.co/TencentMedicalNet
 
     Args:
         resnet_depth: depth of the pretrained model. Supported values are 10, 18, 34, 50, 101, 152 and 200
         device: device on which the returned state dict will be loaded. "cpu" or "cuda" for example.
         datasets23: if True, get the weights trained on more datasets (23).
                     Not all depths are available. If not, standard weights are returned.
 
@@ -529,15 +657,28 @@
     logger.info(f"{filename} downloaded")
     return checkpoint.get("state_dict")
 
 
 def get_medicalnet_pretrained_resnet_args(resnet_depth: int):
     """
     Return correct shortcut_type and bias_downsample
-    for pretrained MedicalNet weights according to resnet depth
+    for pretrained MedicalNet weights according to resnet depth.
     """
     # After testing
     # False: 10, 50, 101, 152, 200
     # Any: 18, 34
     bias_downsample = -1 if resnet_depth in [18, 34] else 0  # 18, 10, 34
     shortcut_type = "A" if resnet_depth in [18, 34] else "B"
     return bias_downsample, shortcut_type
+
+
+def _load_state_dict(model: nn.Module, model_name: str, datasets23: bool = True) -> None:
+    search_res = re.search(r"resnet(\d+)", model_name)
+    if search_res:
+        resnet_depth = int(search_res.group(1))
+        datasets23 = model_name.endswith("_23datasets")
+    else:
+        raise ValueError("model_name argument should contain resnet depth. Example: resnet18 or resnet18_23datasets.")
+
+    model_state_dict = get_pretrained_resnet_medicalnet(resnet_depth, device="cpu", datasets23=datasets23)
+    model_state_dict = {key.replace("module.", ""): value for key, value in model_state_dict.items()}
+    model.load_state_dict(model_state_dict)
```

## monai/transforms/utils.py

```diff
@@ -2186,15 +2186,15 @@
     distances_original, indices_original = distances, indices
     distances, indices = None, None
     if use_cp:
         distances_, indices_ = None, None
         if return_distances:
             dtype = torch.float64 if float64_distances else torch.float32
             if distances is None:
-                distances = torch.zeros_like(img, dtype=dtype)  # type: ignore
+                distances = torch.zeros_like(img, memory_format=torch.contiguous_format, dtype=dtype)  # type: ignore
             else:
                 if not isinstance(distances, torch.Tensor) and distances.device != img.device:
                     raise TypeError("distances must be a torch.Tensor on the same device as img")
                 if not distances.dtype == dtype:
                     raise TypeError("distances must be a torch.Tensor of dtype float32 or float64")
             distances_ = convert_to_cupy(distances)
         if return_indices:
```

## monai/utils/misc.py

```diff
@@ -523,15 +523,15 @@
 
     @staticmethod
     def doc_images() -> str | None:
         return os.environ.get("MONAI_DOC_IMAGES")
 
     @staticmethod
     def algo_hash() -> str | None:
-        return os.environ.get("MONAI_ALGO_HASH", "def5f26")
+        return os.environ.get("MONAI_ALGO_HASH", "07acb39")
 
     @staticmethod
     def trace_transform() -> str | None:
         return os.environ.get("MONAI_TRACE_TRANSFORM", "1")
 
     @staticmethod
     def eval_expr() -> str | None:
```

## Comparing `monai-1.3.1rc5.dist-info/LICENSE` & `monai-1.3.1rc6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `monai-1.3.1rc5.dist-info/METADATA` & `monai-1.3.1rc6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai
-Version: 1.3.1rc5
+Version: 1.3.1rc6
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

## Comparing `monai-1.3.1rc5.dist-info/RECORD` & `monai-1.3.1rc6.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 monai/__init__.py,sha256=jkwqQsDlX2p6hEA7_htzcXj50xHmYyPXu5_wUSb6Nu0,2663
-monai/_version.py,sha256=nnkiQBTMF7VtCMsOwFNcd7B3HQBy0AE2UkLSseSQcBQ,500
+monai/_version.py,sha256=Ch8ZRYTLqUPCpmRZnGF7JyI8_eSY3A--UNDproiyLjE,500
 monai/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 monai/_extensions/__init__.py,sha256=NEBPreRhQ8H9gVvgrLr_y52_TmqB96u_u4VQmeNT93I,642
 monai/_extensions/loader.py,sha256=7SiKw36q-nOzH8CRbBurFrz7GM40GCu7rc93Tm8XpnI,3643
 monai/_extensions/gmm/gmm.cpp,sha256=GLC_KOEFUlEB8fUs6vjeuZBxIqzuatZBDc-ZoAtQ6Xg,2931
 monai/_extensions/gmm/gmm.h,sha256=c9n8RLa4r9jTbqpY4cCHFm3ldVER_FN8pG2hQx3Lb3c,1760
 monai/_extensions/gmm/gmm_cpu.cpp,sha256=cyKn-7DjtVCPb9bnGb0bWUfagb3KUFX9rD6mI5BEXrs,1118
 monai/_extensions/gmm/gmm_cuda.cu,sha256=egWZBIpNYfOfxn0TKX82y-S2M6jg9NCzWwRcTLNmmrU,15983
 monai/_extensions/gmm/gmm_cuda_linalg.cuh,sha256=Glqg2oAcUFUXg-DVfpROkiv-DdXvvVdM1nyiFm8qlHY,3520
 monai/apps/__init__.py,sha256=VDIc3HB_uFbqKL1TS-OeRvryEMDfzm22KJRzwpkXsGo,908
 monai/apps/datasets.py,sha256=msT58BoHlQFQpD4Tx-CThwAkkaUowoNZOgcH0THg0u0,35085
-monai/apps/utils.py,sha256=m4WicFL43ZwEeyUp0OfqzYcFPkuxxo9nU-WcuDQVE8w,14297
+monai/apps/utils.py,sha256=aMsYUlfAeRsdQL1YM4AA79GqPbMsQ1OQau9YNevoFQ4,14452
 monai/apps/auto3dseg/__init__.py,sha256=DhUB2Ol0-iNAk1ZNmD1RkTODUOhdiibv8h9MgcLuF6s,1016
 monai/apps/auto3dseg/__main__.py,sha256=fCDhD8uhmJQKkKBxLO6hMJhEvZJRIsjTc1Ad3bYmNIY,1411
 monai/apps/auto3dseg/auto_runner.py,sha256=-pJveBK3LhXwKfQPaxLG9jPOgMK8NGiNFNhOGmUHrsU,40110
 monai/apps/auto3dseg/bundle_gen.py,sha256=y_9lbw0xk1em0TsIn7mTJHmD3OQNcNZVsjgkhdYg0Lw,28994
 monai/apps/auto3dseg/data_analyzer.py,sha256=XJuQ-bSE3G_6r2i6S75jjo-klWTUGpy5aY3WqijSWqk,18628
 monai/apps/auto3dseg/ensemble_builder.py,sha256=GaLpeAIW5X9oC921cevE86coOsmXW2C136FHuo6UyMo,27277
 monai/apps/auto3dseg/hpo_gen.py,sha256=15u6SYIFfdwb-McQzb9Fcq3-jZjbi3idD8_XQX0veZU,16674
@@ -196,15 +196,15 @@
 monai/losses/dice.py,sha256=B0O56BeIqDBIQovqBoaKXdzyeyNbZXAZ1BuCWV0XYrE,51627
 monai/losses/ds_loss.py,sha256=iaR74lNAyWr6xi52cEIASMuFkeH9FiTpUcQLSEZfmWY,3854
 monai/losses/focal_loss.py,sha256=OhAtxzAwZ1CoNGH1S2dQbG7iDyowYUqv64KXi0GgMhk,11772
 monai/losses/giou_loss.py,sha256=Mogq6fR0tO__Xj0Ul388QMEx03XrSS-Ue96i9ahY-uo,2795
 monai/losses/hausdorff_loss.py,sha256=1TOUjDS9_1txlHw5DX71oshiXOzowLefg8Y-n-PsD5o,10697
 monai/losses/image_dissimilarity.py,sha256=fIIY1zyxfxl-hKi797xpyDDknUGkdLWGJDBwK3IvJ18,15460
 monai/losses/multi_scale.py,sha256=7hL4clBLa3f0tz9-74brq5XOFChrpyd_h9cHQKPnseQ,3636
-monai/losses/perceptual.py,sha256=onTKtb1bm1R6iTOD6AiNrkBAbaYEr4vsBUYvfcNxrgw,17586
+monai/losses/perceptual.py,sha256=_UQs6dUIsfff-sXx_Kvg3GcY6YN_2rhpSpt5b8idP58,19468
 monai/losses/spatial_mask.py,sha256=rPyW8fJPSdqHUS7YB7m30Sq4G-YYpobO_fvKsFSAFQ0,2955
 monai/losses/spectral_loss.py,sha256=PqmZdmJOAzaarW0bzBu8SeL9sOy3XQhul7pnLY4Ih-I,3368
 monai/losses/ssim_loss.py,sha256=v8LaVXtBzpTey80CBtsWTs5qWw7fiJwYAXqXcCgo5kA,5058
 monai/losses/sure_loss.py,sha256=PDDNNeZm8SLPRCDUPbc8o4--ribHnY4nbo8y55nRo0w,8179
 monai/losses/tversky.py,sha256=8idAtxrZW3SYI0vC8Hw2EDkOb4ybgCnJD3aNipWOEGc,6645
 monai/losses/unified_focal_loss.py,sha256=rCj8IpueYH_UMrOUXU0tjbXIN4Uix3bGnRZQtRvl7Sg,10224
 monai/metrics/__init__.py,sha256=DUjK3_qfGZbw0zCv6OJgMSL3AfiYN47aYqLsxn69-HU,2174
@@ -225,15 +225,15 @@
 monai/metrics/regression.py,sha256=JV7x8ibD04hZeWz83Ac26jjyufsCanvAmohD-eWKtbY,26218
 monai/metrics/rocauc.py,sha256=CJOAzDamB8TcFP1bEg-I1m5V1-Pq5RMaLFdM6MtNa_E,8038
 monai/metrics/surface_dice.py,sha256=aNERsTuJkPMfxatPaAzoW1KtvZvUAv4qe_7Kl_dOROI,15149
 monai/metrics/surface_distance.py,sha256=bKDTm7ulhjfiphHLrDJoA3OKI3npwQy2Z5wY-JkXtXg,9727
 monai/metrics/utils.py,sha256=0UYv-yYXCAa96rrBNvqYNxyoi8W_AIWNpDsoXep9j8M,46947
 monai/metrics/wrapper.py,sha256=c1zg-xcypQyZ840TEuhhLgr4sClYMWTxlv1OieJTtvE,11781
 monai/networks/__init__.py,sha256=X-z-kmVt9kwoNPgfYITGycnvG_9HC3_RSRKD2YC35Ag,1020
-monai/networks/utils.py,sha256=nWkN692j3_ympMPT9IiOTyOCsgHEpRVhmmfzjTMNw8U,49607
+monai/networks/utils.py,sha256=GRtep2gGG1xxiviaQx1BNXP0tT-Tu4tyMgfKp4kLdMc,49645
 monai/networks/blocks/__init__.py,sha256=umyJFI-rDAMuseC0gD1vwCE3EowQpWjVfuCLKGFoL1g,2134
 monai/networks/blocks/acti_norm.py,sha256=bVGXbTZ_ssRvmED5R7LOQ7jj4V6WbVFl8JMO-4iZ2Dk,4275
 monai/networks/blocks/activation.py,sha256=S5k3zcP2PsHBkeIxgWgNg8ppW80tTResVP2j9ZsvTFw,5839
 monai/networks/blocks/aspp.py,sha256=GGGE7NfWj77RkaWHbcLuUP4Aff-WeiDrtgtFuSoekQk,4380
 monai/networks/blocks/backbone_fpn_utils.py,sha256=mdXFwtnRgwuaisTlY-c7OkY1ZZBY3I82dAjpXFAZFbg,7488
 monai/networks/blocks/convolutions.py,sha256=gRmbYfy3IR4taiXuxeH5KGOFjP55FoVWfP4e1L6ai0s,11686
 monai/networks/blocks/crf.py,sha256=gHyRgBWD9DmmbCJnXwsMa6WN7N9fDLuT_SwH8MnHhXE,5009
@@ -265,37 +265,37 @@
 monai/networks/layers/factories.py,sha256=L4_JJSsdE02ovM2zgwN-JnUjQQCK2xPyf961O7n7SeU,15380
 monai/networks/layers/filtering.py,sha256=7ru9Yt3yOM-ko-UqzYp-2tMpb8VHt5d767F-KkzrqYY,17992
 monai/networks/layers/gmm.py,sha256=Aq-YCHgUalgOZQ0x5mwYKJe1G7aiCiJybdkPTiiT120,3325
 monai/networks/layers/simplelayers.py,sha256=MhJ0h-Tf4_ZXMMB1gGwc8Plheja6X5PToTJ0tMHjjuE,28472
 monai/networks/layers/spatial_transforms.py,sha256=fz2t7-ibijNLqTYpAn4ZgdXtzBSIyWlaF35mQtqWRY4,25581
 monai/networks/layers/utils.py,sha256=_387-Au76QG5wwGs7ESg0ocGTcBzw4DJz19H7vrPKjM,4296
 monai/networks/layers/weight_init.py,sha256=ehwI5F7jm_lmDkK4qVL7ocIzCEPx5UPgLaURcsfMNwk,2253
-monai/networks/nets/__init__.py,sha256=2CDne2u-evkHh8XrTRZaEc_S6kSdsZ9ps4R4Koez4to,3329
+monai/networks/nets/__init__.py,sha256=gAwfy-nj2hgClPBB3JdePgcBcLAvE3pfHR6Gp4opGwQ,3368
 monai/networks/nets/ahnet.py,sha256=RT-loCa5Z_3I2DWB8lmRkhxGXSsnMVBCEDpwo68-YB4,21570
 monai/networks/nets/attentionunet.py,sha256=jP0Y4miDOzK4Y6CzDFhDR3_Vzm8sYtctJ-lWd2vAzok,9206
 monai/networks/nets/autoencoder.py,sha256=QuLdDfDwhefIqA2n8XfmFyi5T8enP6O4PETdBKmFMKc,12586
 monai/networks/nets/basic_unet.py,sha256=K76Q-WXuCPGNf8X9qa1wwtiv1gzwlERrL6BKqKcpzlQ,10951
 monai/networks/nets/basic_unetplusplus.py,sha256=M2sSCgWvqgpiRq1tpR164udnbN1WkO1a81PmgCfV5lU,7961
 monai/networks/nets/classifier.py,sha256=U94OM91_pNT74wQV-_LOxAnbLvjuJvnorMK-xcE7HJE,6293
 monai/networks/nets/daf3d.py,sha256=wCAPZ4JngMHrAQ0u8kXho-JOD1tj17_k5wIbX80PgJU,23786
 monai/networks/nets/densenet.py,sha256=0LZqWU3HNfnEkNKBPwVg2GFoeIHQB5aBfP2_U54bv8g,15823
 monai/networks/nets/dints.py,sha256=GAL2cmWOk_mhsRaIdZ3pr-mMLqncWINdJCWj26IukL0,44775
 monai/networks/nets/dynunet.py,sha256=S2DX_tby7e5iCHL7q6X6f-vT6HwP6tbb2lRq9gHVJ24,18210
 monai/networks/nets/efficientnet.py,sha256=RcEM7ZTLCp9PzE06sCJDUbStzMZpItSiZjDlbRUaz-4,40671
-monai/networks/nets/flexible_unet.py,sha256=1FwOvDijaD-2V8nAaW2ibr5DYpl8Ule8LtPADH3TNb0,14147
+monai/networks/nets/flexible_unet.py,sha256=VN3cJQPMmY--TpZkuDwEWonPgJc4R3JKBwJCGsn7sgQ,14435
 monai/networks/nets/fullyconnectednet.py,sha256=j5uo68qnYSxgH_sEMRh7s3QGNKFaJAIxmx8OixEv2Ig,7212
 monai/networks/nets/generator.py,sha256=q20EAl9N7Q56t78JiZaUEkPhYWyD02oqO0yekJCd9x0,6581
 monai/networks/nets/highresnet.py,sha256=1Mx8lR5K4sRXGWjspDAHaKq0WrX9Q7qz8CcBCKZxIXk,8883
 monai/networks/nets/hovernet.py,sha256=E831rgNN8SP1lui8-ffV7IUscDWvyTr-YTqXcpof878,28684
 monai/networks/nets/milmodel.py,sha256=aUDgYJG0kS3p4nBW_dF7b4cWwuC31w3KIzmUzXA08HE,9813
 monai/networks/nets/netadapter.py,sha256=JtcME9pcg8ud4jHKZKM9fE-8leP2PQXgUIfKBdB0wcA,6102
 monai/networks/nets/quicknat.py,sha256=IisYwI-xtsf_Gfma_flkBQWc-o2m8wS0NaPWbbcYNko,20220
 monai/networks/nets/regressor.py,sha256=6Nz5yJuQDJJOr5R0rhot_mHu7_MDCA4ybV48wS1HS1M,6482
 monai/networks/nets/regunet.py,sha256=-A6ygR7lVyAflFyqWkVVOsY94uMXWol1f2xr_HmsU1c,18664
-monai/networks/nets/resnet.py,sha256=Yo0P-Ml3hRvVRuGSvUtGPQIxkbvyNZb-NZOOnAf0t5g,22089
+monai/networks/nets/resnet.py,sha256=PDSQCN6cwLP5ieLTXVVO4M5n8pE02L5s5BXTRwlzc5M,27339
 monai/networks/nets/segresnet.py,sha256=xNkSIvdk7kAyc3eVn-U_gGj8MoGVc5nklFKc_fkgOUs,13994
 monai/networks/nets/segresnet_ds.py,sha256=01R-t-cIvAoVEsqTRPC2sHVYGyiVfcvy8hng53X-6yQ,15703
 monai/networks/nets/senet.py,sha256=gulqPMYmSABbMbN39NElGzSU1TKGviJas7EPTBaZ60A,19289
 monai/networks/nets/swin_unetr.py,sha256=eDVGAGPaq5pL2E-dCyZTT4SmdUdRKU7iodunRnkWk1U,44811
 monai/networks/nets/torchvision_fc.py,sha256=3g5PD7C1MSkQ8xndhnVd0b3aN8zfshT8uiFS0OHyQaY,6309
 monai/networks/nets/transchex.py,sha256=uA_RfTDfPhwA1ecAPZ9EDnMyJKn2tUMLEWdyB_rU2v0,15726
 monai/networks/nets/unet.py,sha256=riKWB8iEEgO4CIiVTOo532726HWWBfuBcIHeoLvvN0w,13627
@@ -314,15 +314,15 @@
 monai/transforms/adaptors.py,sha256=jqh7cVvIj4h7-UndP7CNuwxgIUXWY_5kiMzjGC5jFBs,8950
 monai/transforms/compose.py,sha256=zQa_hf8gIater3Bo_XW1IVYgX7aFa_Co6-BZPwoeaQw,37663
 monai/transforms/inverse.py,sha256=Wg8UnMJru41G3eHGipUemAWziHGU-qdd-Flfi3eOpeo,18746
 monai/transforms/inverse_batch_transform.py,sha256=fMbukZq2P99BhqqMuWZFJ9uboZ5dN61MBvvicwf40V0,7055
 monai/transforms/nvtx.py,sha256=1EKEXZIhTUFKoIrJmd_fevwrHwo731dVFUFJQFiOk3w,3386
 monai/transforms/traits.py,sha256=F8kmhnekTyaAdo8wIFjO3-uqpVtmFym3mNxbYbyvkFI,3563
 monai/transforms/transform.py,sha256=XYunJKTgm99TPBAw4Ikams-wCpgGnKZYZTPN2042m7U,21532
-monai/transforms/utils.py,sha256=sIoXl3BPox4VIWa16BVOVY7lvIjAhk7O5xJUGZCR3lM,91619
+monai/transforms/utils.py,sha256=tkzZmaXPNU_YoV7cdnbLueQSCiqEteMllbw5UbvKP3A,91658
 monai/transforms/utils_create_transform_ims.py,sha256=20FdSIgkTqYY_yFX8MrrGznTTPCT6OtlmG-nL2vJCcI,31121
 monai/transforms/utils_pytorch_numpy_unification.py,sha256=9Exl8id6kPbFvdZLcgfpj0FCUSjrwIlB7qiSQ4OdTZM,18779
 monai/transforms/croppad/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/transforms/croppad/array.py,sha256=5W7ydnsaMxJ3vLSnfNyta6tHvJND1lmdqXEXasoSKBg,74745
 monai/transforms/croppad/batch.py,sha256=5ukcYk3VCDpk62AL5Q_jTqpXmSNTlw0UCUhDeAB4aV0,6138
 monai/transforms/croppad/dictionary.py,sha256=2pf_k3gvDi7ruzj6bx2gVNIae7SatiLEWLg7EKJZDbg,60722
 monai/transforms/croppad/functional.py,sha256=_agF3ustEVXVuKSF8qGNhXCrb3E6mc5Qypy37_MQU-8,12628
@@ -362,26 +362,26 @@
 monai/utils/aliases.py,sha256=uBxkLudRfy3Rts9RZo4NDPGoq4e3Ymcaihk6lT92GFo,4096
 monai/utils/component_store.py,sha256=VMF7CtPu5Wi_eX_qFtm9iWo5kvoWFuCUIxdRzk90zZo,4498
 monai/utils/decorators.py,sha256=YRK5iEMdbc2INrWnBNDSMTaHge_0ezRf2b9yJGL-opg,3129
 monai/utils/deprecate_utils.py,sha256=gKeEV4MsI51qeQ5gci2me_C-0e-tDwa3VZzd3XPQqLk,14759
 monai/utils/dist.py,sha256=mVaKlBTQJdWAG910sh5pGLEbb_KhRAXV5cPz7amH88Y,8639
 monai/utils/enums.py,sha256=Gdo9WBrFODIYz5zt6c00hGz0bqjUQbhCWsfGSgKlnAU,19674
 monai/utils/jupyter_utils.py,sha256=QqcKhJxzEf6YwM8Ik_HvfVDr7gNfrfzCXdzd2urEH8M,15651
-monai/utils/misc.py,sha256=e2R7jQlSj0qatN7UdT8KdG3ApONJDzgnXZz4zQ9C4f8,30908
+monai/utils/misc.py,sha256=azooCO5e8DLwYY-kX3WrAmHkM3dv8Zc6V-VLZ114cKc,30908
 monai/utils/module.py,sha256=fTy_Q1AhhLO0_xIh_hUaSxuCSmEP9aJaTyjwUlA7dLs,25008
 monai/utils/nvtx.py,sha256=i9JBxR1uhW1ZCgLPLlTx8b907QlXkFzJyTBLMlFjhtU,6876
 monai/utils/profiling.py,sha256=V2_cSHgrcmVF48_G3nUi2-O6fnXsS89nSlb8jj58YLo,15937
 monai/utils/state_cacher.py,sha256=ERBE-mnnf47MwKSq-pNbfu1D2C4ZqKH-mORyLaBa3EE,5955
 monai/utils/tf32.py,sha256=4bqpPxoTAMmQDNRbbrd4qHG27e1RrxeAmfDf3vP8tQc,3141
 monai/utils/type_conversion.py,sha256=CwmAfcFNgNOQdMaNdrDcIuj7_esJls4-BymtMD03ZuM,21520
 monai/visualize/__init__.py,sha256=p7dv9-hRa9vAhlpHyk86yap9HgeDeJRO3pXmFhDx8Mc,1038
 monai/visualize/class_activation_maps.py,sha256=jBej0DVDzXJlSpwGjHw4k84R-jFfux4Rvpdg-nuzzZ8,16158
 monai/visualize/gradient_based.py,sha256=oXqMxqIClVlrgloZwgdTUl4pWllsoS0ysbjuvAbu-Kg,6278
 monai/visualize/img2tensorboard.py,sha256=_p5olAefUs6t-y17z0TK32fKxNnUNXVkb0Op1SkfLMM,9200
 monai/visualize/occlusion_sensitivity.py,sha256=OQHEJLyIhB8zWqQsfKaX-1kvCjWFVYtLfS4dFC0nKFI,18160
 monai/visualize/utils.py,sha256=xJbG68R-W17aqm0cpmMrypbZaiVfUaG9GWMFtKV7VUo,9966
 monai/visualize/visualizer.py,sha256=qckyaMZCbezYUwE20k5yc-Pb7UozVavMDbrmyQwfYHY,1377
-monai-1.3.1rc5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-monai-1.3.1rc5.dist-info/METADATA,sha256=t886heeI7FA-Q8MbEa_hk9hIg_9Y78ms5xzWfoWQ6qw,10915
-monai-1.3.1rc5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-monai-1.3.1rc5.dist-info/top_level.txt,sha256=UaNwRzLGORdus41Ip446s3bBfViLkdkDsXDo34J2P44,6
-monai-1.3.1rc5.dist-info/RECORD,,
+monai-1.3.1rc6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+monai-1.3.1rc6.dist-info/METADATA,sha256=py05jdaCjgElfihwVOuQrIJA_2pI5fHTjVj0NfJVpbI,10915
+monai-1.3.1rc6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+monai-1.3.1rc6.dist-info/top_level.txt,sha256=UaNwRzLGORdus41Ip446s3bBfViLkdkDsXDo34J2P44,6
+monai-1.3.1rc6.dist-info/RECORD,,
```

