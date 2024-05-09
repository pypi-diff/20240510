# Comparing `tmp/alabamaEncoder-0.2.tar.gz` & `tmp/alabamaEncoder-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alabamaEncoder-0.2.tar", last modified: Tue Mar  5 20:07:16 2024, max compression
+gzip compressed data, was "alabamaEncoder-0.3.tar", last modified: Tue Mar  5 20:19:58 2024, max compression
```

## Comparing `alabamaEncoder-0.2.tar` & `alabamaEncoder-0.3.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.761457 alabamaEncoder-0.2/
--rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      197 2024-03-05 20:07:16.761457 alabamaEncoder-0.2/PKG-INFO
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.729455 alabamaEncoder-0.2/alabamaEncode/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2021-04-17 09:55:33.000000 alabamaEncoder-0.2/alabamaEncode/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.729455 alabamaEncoder-0.2/alabamaEncode/ai_vmaf/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 08:49:47.000000 alabamaEncoder-0.2/alabamaEncode/ai_vmaf/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1554 2023-12-13 17:07:22.000000 alabamaEncoder-0.2/alabamaEncode/ai_vmaf/aom_firstpass.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1026 2023-12-18 07:05:43.000000 alabamaEncoder-0.2/alabamaEncode/ai_vmaf/perdict.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.729455 alabamaEncoder-0.2/alabamaEncode/ai_vmaf/train/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 10:35:40.000000 alabamaEncoder-0.2/alabamaEncode/ai_vmaf/train/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12402 2023-12-14 22:03:21.000000 alabamaEncoder-0.2/alabamaEncode/ai_vmaf/train/train.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.733456 alabamaEncoder-0.2/alabamaEncode/conent_analysis/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:25:35.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.733456 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:35.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.733456 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-17 00:34:57.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      671 2024-01-17 00:37:48.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1064 2024-01-17 00:37:48.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3356 2024-02-04 12:12:23.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4061 2024-02-04 12:03:51.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10662 2024-01-17 00:37:48.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      597 2024-01-17 00:37:48.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      606 2024-01-17 00:37:48.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5750 2024-02-13 01:32:21.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      448 2023-12-10 19:05:23.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/chunk_analyse_step.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      623 2023-12-05 14:54:46.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_step.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.737456 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-05 14:55:01.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      684 2024-01-17 00:37:48.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1584 2024-01-17 00:37:48.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10491 2024-02-10 20:59:51.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6476 2024-02-04 12:12:23.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2247 2024-01-20 21:54:56.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      859 2024-02-02 15:57:21.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6701 2024-02-04 12:09:55.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/weirdX264.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2122 2024-02-28 15:17:20.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/opinionated_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6184 2024-01-25 02:24:33.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/pipelines.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      133 2024-01-15 01:49:31.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/refine_step.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.737456 alabamaEncoder-0.2/alabamaEncode/conent_analysis/refine_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-14 19:17:26.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/refine_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4949 2024-01-21 06:06:00.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/refine_steps/multires_package.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7817 2024-01-20 18:40:41.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.741456 alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:49.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1498 2024-02-12 21:25:13.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/args_tune.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4691 2024-01-25 02:38:15.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/autocrop.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      552 2024-01-25 02:38:21.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/denoise_filtering.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2356 2024-01-25 02:38:27.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/encoding_tiles.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9823 2024-02-04 12:39:56.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/ideal_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7511 2024-02-12 05:33:32.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5994 2024-02-04 12:07:28.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/sequence_autograin.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3119 2024-02-02 18:54:38.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6920 2024-02-04 12:09:55.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2777 2024-02-04 12:09:55.000000 alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/x264_tune.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.745456 alabamaEncoder-0.2/alabamaEncode/core/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-19 23:19:38.000000 alabamaEncoder-0.2/alabamaEncode/core/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10246 2024-02-04 12:09:55.000000 alabamaEncoder-0.2/alabamaEncode/core/alabama.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1813 2024-01-28 06:16:28.000000 alabamaEncoder-0.2/alabamaEncode/core/alamaba_kv.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2879 2024-02-21 15:17:46.000000 alabamaEncoder-0.2/alabamaEncode/core/bin_utils.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3695 2024-02-12 05:31:26.000000 alabamaEncoder-0.2/alabamaEncode/core/chunk_job.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4947 2024-01-31 09:31:42.000000 alabamaEncoder-0.2/alabamaEncode/core/cli_executor.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13646 2024-01-20 23:26:34.000000 alabamaEncoder-0.2/alabamaEncode/core/ffmpeg.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6016 2024-03-01 18:23:51.000000 alabamaEncoder-0.2/alabamaEncode/core/final_touches.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    18882 2024-02-12 05:35:07.000000 alabamaEncoder-0.2/alabamaEncode/core/job.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      813 2023-11-25 00:35:54.000000 alabamaEncoder-0.2/alabamaEncode/core/path.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      556 2023-11-12 21:29:16.000000 alabamaEncoder-0.2/alabamaEncode/core/timer.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1776 2023-12-24 03:53:49.000000 alabamaEncoder-0.2/alabamaEncode/core/ws_update.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.745456 alabamaEncoder-0.2/alabamaEncode/encoder/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-09-27 12:09:43.000000 alabamaEncoder-0.2/alabamaEncode/encoder/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      748 2024-01-17 00:16:49.000000 alabamaEncoder-0.2/alabamaEncode/encoder/codec.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11408 2024-02-12 22:35:38.000000 alabamaEncoder-0.2/alabamaEncode/encoder/encoder.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1536 2024-02-12 05:37:04.000000 alabamaEncoder-0.2/alabamaEncode/encoder/encoder_factory.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.749456 alabamaEncoder-0.2/alabamaEncode/encoder/impl/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4369 2024-02-12 05:35:10.000000 alabamaEncoder-0.2/alabamaEncode/encoder/impl/Aomenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2087 2024-02-12 05:35:10.000000 alabamaEncoder-0.2/alabamaEncode/encoder/impl/Nvenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1586 2024-01-28 06:23:47.000000 alabamaEncoder-0.2/alabamaEncode/encoder/impl/SvtAvif.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7581 2024-02-12 21:28:16.000000 alabamaEncoder-0.2/alabamaEncode/encoder/impl/Svtenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2172 2024-02-12 05:35:10.000000 alabamaEncoder-0.2/alabamaEncode/encoder/impl/VaapiH264.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2113 2024-02-12 05:35:10.000000 alabamaEncoder-0.2/alabamaEncode/encoder/impl/VaapiH265.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7238 2024-02-12 05:35:10.000000 alabamaEncoder-0.2/alabamaEncode/encoder/impl/X264.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4097 2024-02-12 05:35:10.000000 alabamaEncoder-0.2/alabamaEncode/encoder/impl/X265.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2022-12-05 03:43:14.000000 alabamaEncoder-0.2/alabamaEncode/encoder/impl/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2033 2024-02-12 05:35:10.000000 alabamaEncoder-0.2/alabamaEncode/encoder/impl/rav1e.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3557 2024-02-12 05:35:10.000000 alabamaEncoder-0.2/alabamaEncode/encoder/impl/vp9.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      269 2024-01-17 00:14:46.000000 alabamaEncoder-0.2/alabamaEncode/encoder/rate_dist.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2494 2024-02-04 12:07:28.000000 alabamaEncoder-0.2/alabamaEncode/encoder/stats.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.753456 alabamaEncoder-0.2/alabamaEncode/experiments/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3713 2023-12-11 23:14:15.000000 alabamaEncoder-0.2/alabamaEncode/experiments/Aq.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4337 2023-12-11 23:14:15.000000 alabamaEncoder-0.2/alabamaEncode/experiments/Overlays.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2950 2024-02-02 15:19:02.000000 alabamaEncoder-0.2/alabamaEncode/experiments/Svtav1Speed.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5719 2023-12-11 23:14:15.000000 alabamaEncoder-0.2/alabamaEncode/experiments/Svtav1Tunes.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3749 2023-12-11 23:14:15.000000 alabamaEncoder-0.2/alabamaEncode/experiments/TemporalFiltering.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-06 18:23:30.000000 alabamaEncoder-0.2/alabamaEncode/experiments/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2496 2023-12-02 16:35:17.000000 alabamaEncoder-0.2/alabamaEncode/experiments/ai_feature_extract.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      319 2023-12-10 22:37:13.000000 alabamaEncoder-0.2/alabamaEncode/experiments/aom_extract.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5812 2024-02-04 12:09:55.000000 alabamaEncoder-0.2/alabamaEncode/experiments/convexhull.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    16885 2024-02-04 12:09:55.000000 alabamaEncoder-0.2/alabamaEncode/experiments/crf_vmaf_relation.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4941 2024-02-04 12:09:55.000000 alabamaEncoder-0.2/alabamaEncode/experiments/denoise.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2210 2024-02-04 12:09:55.000000 alabamaEncoder-0.2/alabamaEncode/experiments/sequence_convex.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      254 2023-12-20 04:58:54.000000 alabamaEncoder-0.2/alabamaEncode/experiments/serialise_context.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      793 2023-12-31 13:08:11.000000 alabamaEncoder-0.2/alabamaEncode/experiments/streaming_output.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6592 2023-12-11 23:14:15.000000 alabamaEncoder-0.2/alabamaEncode/experiments/superres.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4106 2023-11-15 20:26:48.000000 alabamaEncoder-0.2/alabamaEncode/experiments/target_vmaf.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.753456 alabamaEncoder-0.2/alabamaEncode/experiments/util/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11478 2024-02-04 12:09:55.000000 alabamaEncoder-0.2/alabamaEncode/experiments/util/ExperimentUtil.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-10-17 18:48:28.000000 alabamaEncoder-0.2/alabamaEncode/experiments/util/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.753456 alabamaEncoder-0.2/alabamaEncode/metrics/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-17 22:15:46.000000 alabamaEncoder-0.2/alabamaEncode/metrics/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5237 2024-02-04 12:44:56.000000 alabamaEncoder-0.2/alabamaEncode/metrics/calculate.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      911 2023-11-22 22:07:47.000000 alabamaEncoder-0.2/alabamaEncode/metrics/comparison_display.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      384 2024-01-26 03:01:39.000000 alabamaEncoder-0.2/alabamaEncode/metrics/exception.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3033 2023-11-19 23:24:09.000000 alabamaEncoder-0.2/alabamaEncode/metrics/image.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.753456 alabamaEncoder-0.2/alabamaEncode/metrics/impl/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-02-04 12:02:29.000000 alabamaEncoder-0.2/alabamaEncode/metrics/impl/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      924 2023-11-19 23:28:00.000000 alabamaEncoder-0.2/alabamaEncode/metrics/impl/psnr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1432 2023-11-25 03:14:34.000000 alabamaEncoder-0.2/alabamaEncode/metrics/impl/ssim.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3093 2024-02-05 00:20:43.000000 alabamaEncoder-0.2/alabamaEncode/metrics/impl/ssimu2.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9052 2024-02-05 00:40:43.000000 alabamaEncoder-0.2/alabamaEncode/metrics/impl/vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      117 2024-02-04 12:09:55.000000 alabamaEncoder-0.2/alabamaEncode/metrics/metric.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      373 2024-02-04 12:36:30.000000 alabamaEncoder-0.2/alabamaEncode/metrics/options.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      308 2024-02-02 14:53:33.000000 alabamaEncoder-0.2/alabamaEncode/metrics/result.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.757457 alabamaEncoder-0.2/alabamaEncode/parallelEncoding/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2357 2024-01-07 02:35:39.000000 alabamaEncoder-0.2/alabamaEncode/parallelEncoding/CeleryApp.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3848 2023-11-19 23:24:09.000000 alabamaEncoder-0.2/alabamaEncode/parallelEncoding/CeleryAutoscaler.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-16 16:38:33.000000 alabamaEncoder-0.2/alabamaEncode/parallelEncoding/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      148 2023-11-05 09:04:10.000000 alabamaEncoder-0.2/alabamaEncode/parallelEncoding/command.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     8001 2024-02-05 23:23:24.000000 alabamaEncoder-0.2/alabamaEncode/parallelEncoding/execute_commands.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      581 2024-01-07 00:27:19.000000 alabamaEncoder-0.2/alabamaEncode/parallelEncoding/worker.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.757457 alabamaEncoder-0.2/alabamaEncode/scene/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-15 20:18:27.000000 alabamaEncoder-0.2/alabamaEncode/scene/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     8712 2024-01-28 07:34:00.000000 alabamaEncoder-0.2/alabamaEncode/scene/chunk.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10414 2024-01-29 15:55:32.000000 alabamaEncoder-0.2/alabamaEncode/scene/concat.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4874 2024-01-28 07:36:56.000000 alabamaEncoder-0.2/alabamaEncode/scene/sequence.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11307 2024-01-28 07:36:58.000000 alabamaEncoder-0.2/alabamaEncode/scene/split.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.757457 alabamaEncoder-0.2/alabamaEncode_frontends/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:32:46.000000 alabamaEncoder-0.2/alabamaEncode_frontends/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.757457 alabamaEncoder-0.2/alabamaEncode_frontends/cli/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:52:09.000000 alabamaEncoder-0.2/alabamaEncode_frontends/cli/__init__.py
--rwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)     4369 2023-12-28 09:15:33.000000 alabamaEncoder-0.2/alabamaEncode_frontends/cli/__main__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.761457 alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 18:44:18.000000 alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4148 2023-12-27 17:17:40.000000 alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/autopaths.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    19854 2024-02-12 05:32:29.000000 alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/cli_args.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      973 2023-12-10 22:17:58.000000 alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/paths.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1088 2024-01-23 00:24:16.000000 alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/ratecontrol.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1130 2023-12-10 18:44:44.000000 alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/res_preset.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      321 2023-12-28 09:17:41.000000 alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/validate_codecs.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1144 2024-01-15 02:14:38.000000 alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/video_filters.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.761457 alabamaEncoder-0.2/alabamaEncode_frontends/demon/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:38:55.000000 alabamaEncoder-0.2/alabamaEncode_frontends/demon/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2277 2023-12-24 15:12:07.000000 alabamaEncoder-0.2/alabamaEncode_frontends/demon/demon.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:07:16.761457 alabamaEncoder-0.2/alabamaEncoder.egg-info/
--rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      197 2024-03-05 20:07:16.000000 alabamaEncoder-0.2/alabamaEncoder.egg-info/PKG-INFO
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6013 2024-03-05 20:07:16.000000 alabamaEncoder-0.2/alabamaEncoder.egg-info/SOURCES.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        1 2024-03-05 20:07:16.000000 alabamaEncoder-0.2/alabamaEncoder.egg-info/dependency_links.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       77 2024-03-05 20:07:16.000000 alabamaEncoder-0.2/alabamaEncoder.egg-info/entry_points.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       51 2024-03-05 20:07:16.000000 alabamaEncoder-0.2/alabamaEncoder.egg-info/requires.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-03-05 20:07:16.000000 alabamaEncoder-0.2/alabamaEncoder.egg-info/top_level.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-03-05 20:07:16.761457 alabamaEncoder-0.2/setup.cfg
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      396 2024-03-05 20:05:45.000000 alabamaEncoder-0.2/setup.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.894717 alabamaEncoder-0.3/
+-rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      221 2024-03-05 20:19:58.894717 alabamaEncoder-0.3/PKG-INFO
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.882716 alabamaEncoder-0.3/alabamaEncode/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2021-04-17 09:55:33.000000 alabamaEncoder-0.3/alabamaEncode/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.882716 alabamaEncoder-0.3/alabamaEncode/ai_vmaf/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 08:49:47.000000 alabamaEncoder-0.3/alabamaEncode/ai_vmaf/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1554 2023-12-13 17:07:22.000000 alabamaEncoder-0.3/alabamaEncode/ai_vmaf/aom_firstpass.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1026 2023-12-18 07:05:43.000000 alabamaEncoder-0.3/alabamaEncode/ai_vmaf/perdict.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.882716 alabamaEncoder-0.3/alabamaEncode/ai_vmaf/train/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 10:35:40.000000 alabamaEncoder-0.3/alabamaEncode/ai_vmaf/train/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12402 2023-12-14 22:03:21.000000 alabamaEncoder-0.3/alabamaEncode/ai_vmaf/train/train.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.882716 alabamaEncoder-0.3/alabamaEncode/conent_analysis/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:25:35.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.882716 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:35.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.882716 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-17 00:34:57.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      671 2024-01-17 00:37:48.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1064 2024-01-17 00:37:48.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3356 2024-02-04 12:12:23.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4061 2024-02-04 12:03:51.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10662 2024-01-17 00:37:48.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      597 2024-01-17 00:37:48.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      606 2024-01-17 00:37:48.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5750 2024-02-13 01:32:21.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      448 2023-12-10 19:05:23.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/chunk_analyse_step.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      623 2023-12-05 14:54:46.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_step.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.886716 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-05 14:55:01.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      684 2024-01-17 00:37:48.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1584 2024-01-17 00:37:48.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10491 2024-02-10 20:59:51.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6476 2024-02-04 12:12:23.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2247 2024-01-20 21:54:56.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      859 2024-02-02 15:57:21.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6701 2024-02-04 12:09:55.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/weirdX264.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2122 2024-02-28 15:17:20.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/opinionated_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6184 2024-01-25 02:24:33.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/pipelines.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      133 2024-01-15 01:49:31.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/refine_step.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.886716 alabamaEncoder-0.3/alabamaEncode/conent_analysis/refine_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-14 19:17:26.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/refine_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4949 2024-01-21 06:06:00.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/refine_steps/multires_package.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7817 2024-01-20 18:40:41.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.886716 alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:49.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1498 2024-02-12 21:25:13.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/args_tune.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4691 2024-01-25 02:38:15.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/autocrop.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      552 2024-01-25 02:38:21.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/denoise_filtering.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2356 2024-01-25 02:38:27.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/encoding_tiles.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9823 2024-02-04 12:39:56.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/ideal_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7511 2024-02-12 05:33:32.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5994 2024-02-04 12:07:28.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/sequence_autograin.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3119 2024-02-02 18:54:38.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6920 2024-02-04 12:09:55.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2777 2024-02-04 12:09:55.000000 alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/x264_tune.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.886716 alabamaEncoder-0.3/alabamaEncode/core/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-19 23:19:38.000000 alabamaEncoder-0.3/alabamaEncode/core/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10246 2024-02-04 12:09:55.000000 alabamaEncoder-0.3/alabamaEncode/core/alabama.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1813 2024-01-28 06:16:28.000000 alabamaEncoder-0.3/alabamaEncode/core/alamaba_kv.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2879 2024-02-21 15:17:46.000000 alabamaEncoder-0.3/alabamaEncode/core/bin_utils.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3695 2024-02-12 05:31:26.000000 alabamaEncoder-0.3/alabamaEncode/core/chunk_job.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4947 2024-01-31 09:31:42.000000 alabamaEncoder-0.3/alabamaEncode/core/cli_executor.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13646 2024-01-20 23:26:34.000000 alabamaEncoder-0.3/alabamaEncode/core/ffmpeg.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6016 2024-03-01 18:23:51.000000 alabamaEncoder-0.3/alabamaEncode/core/final_touches.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    18882 2024-02-12 05:35:07.000000 alabamaEncoder-0.3/alabamaEncode/core/job.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      813 2023-11-25 00:35:54.000000 alabamaEncoder-0.3/alabamaEncode/core/path.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      556 2023-11-12 21:29:16.000000 alabamaEncoder-0.3/alabamaEncode/core/timer.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1776 2023-12-24 03:53:49.000000 alabamaEncoder-0.3/alabamaEncode/core/ws_update.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.886716 alabamaEncoder-0.3/alabamaEncode/encoder/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-09-27 12:09:43.000000 alabamaEncoder-0.3/alabamaEncode/encoder/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      748 2024-01-17 00:16:49.000000 alabamaEncoder-0.3/alabamaEncode/encoder/codec.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11408 2024-02-12 22:35:38.000000 alabamaEncoder-0.3/alabamaEncode/encoder/encoder.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1536 2024-02-12 05:37:04.000000 alabamaEncoder-0.3/alabamaEncode/encoder/encoder_factory.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.890716 alabamaEncoder-0.3/alabamaEncode/encoder/impl/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4369 2024-02-12 05:35:10.000000 alabamaEncoder-0.3/alabamaEncode/encoder/impl/Aomenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2087 2024-02-12 05:35:10.000000 alabamaEncoder-0.3/alabamaEncode/encoder/impl/Nvenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1586 2024-01-28 06:23:47.000000 alabamaEncoder-0.3/alabamaEncode/encoder/impl/SvtAvif.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7581 2024-02-12 21:28:16.000000 alabamaEncoder-0.3/alabamaEncode/encoder/impl/Svtenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2172 2024-02-12 05:35:10.000000 alabamaEncoder-0.3/alabamaEncode/encoder/impl/VaapiH264.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2113 2024-02-12 05:35:10.000000 alabamaEncoder-0.3/alabamaEncode/encoder/impl/VaapiH265.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7238 2024-02-12 05:35:10.000000 alabamaEncoder-0.3/alabamaEncode/encoder/impl/X264.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4097 2024-02-12 05:35:10.000000 alabamaEncoder-0.3/alabamaEncode/encoder/impl/X265.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2022-12-05 03:43:14.000000 alabamaEncoder-0.3/alabamaEncode/encoder/impl/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2033 2024-02-12 05:35:10.000000 alabamaEncoder-0.3/alabamaEncode/encoder/impl/rav1e.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3557 2024-02-12 05:35:10.000000 alabamaEncoder-0.3/alabamaEncode/encoder/impl/vp9.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      269 2024-01-17 00:14:46.000000 alabamaEncoder-0.3/alabamaEncode/encoder/rate_dist.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2494 2024-02-04 12:07:28.000000 alabamaEncoder-0.3/alabamaEncode/encoder/stats.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.890716 alabamaEncoder-0.3/alabamaEncode/experiments/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3713 2023-12-11 23:14:15.000000 alabamaEncoder-0.3/alabamaEncode/experiments/Aq.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4337 2023-12-11 23:14:15.000000 alabamaEncoder-0.3/alabamaEncode/experiments/Overlays.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2950 2024-02-02 15:19:02.000000 alabamaEncoder-0.3/alabamaEncode/experiments/Svtav1Speed.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5719 2023-12-11 23:14:15.000000 alabamaEncoder-0.3/alabamaEncode/experiments/Svtav1Tunes.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3749 2023-12-11 23:14:15.000000 alabamaEncoder-0.3/alabamaEncode/experiments/TemporalFiltering.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-06 18:23:30.000000 alabamaEncoder-0.3/alabamaEncode/experiments/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2496 2023-12-02 16:35:17.000000 alabamaEncoder-0.3/alabamaEncode/experiments/ai_feature_extract.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      319 2023-12-10 22:37:13.000000 alabamaEncoder-0.3/alabamaEncode/experiments/aom_extract.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5812 2024-02-04 12:09:55.000000 alabamaEncoder-0.3/alabamaEncode/experiments/convexhull.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    16885 2024-02-04 12:09:55.000000 alabamaEncoder-0.3/alabamaEncode/experiments/crf_vmaf_relation.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4941 2024-02-04 12:09:55.000000 alabamaEncoder-0.3/alabamaEncode/experiments/denoise.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2210 2024-02-04 12:09:55.000000 alabamaEncoder-0.3/alabamaEncode/experiments/sequence_convex.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      254 2023-12-20 04:58:54.000000 alabamaEncoder-0.3/alabamaEncode/experiments/serialise_context.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      793 2023-12-31 13:08:11.000000 alabamaEncoder-0.3/alabamaEncode/experiments/streaming_output.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6592 2023-12-11 23:14:15.000000 alabamaEncoder-0.3/alabamaEncode/experiments/superres.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4106 2023-11-15 20:26:48.000000 alabamaEncoder-0.3/alabamaEncode/experiments/target_vmaf.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.890716 alabamaEncoder-0.3/alabamaEncode/experiments/util/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11478 2024-02-04 12:09:55.000000 alabamaEncoder-0.3/alabamaEncode/experiments/util/ExperimentUtil.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-10-17 18:48:28.000000 alabamaEncoder-0.3/alabamaEncode/experiments/util/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.890716 alabamaEncoder-0.3/alabamaEncode/metrics/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-17 22:15:46.000000 alabamaEncoder-0.3/alabamaEncode/metrics/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5237 2024-02-04 12:44:56.000000 alabamaEncoder-0.3/alabamaEncode/metrics/calculate.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      911 2023-11-22 22:07:47.000000 alabamaEncoder-0.3/alabamaEncode/metrics/comparison_display.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      384 2024-01-26 03:01:39.000000 alabamaEncoder-0.3/alabamaEncode/metrics/exception.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3033 2023-11-19 23:24:09.000000 alabamaEncoder-0.3/alabamaEncode/metrics/image.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.890716 alabamaEncoder-0.3/alabamaEncode/metrics/impl/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-02-04 12:02:29.000000 alabamaEncoder-0.3/alabamaEncode/metrics/impl/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      924 2023-11-19 23:28:00.000000 alabamaEncoder-0.3/alabamaEncode/metrics/impl/psnr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1432 2023-11-25 03:14:34.000000 alabamaEncoder-0.3/alabamaEncode/metrics/impl/ssim.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3093 2024-02-05 00:20:43.000000 alabamaEncoder-0.3/alabamaEncode/metrics/impl/ssimu2.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9052 2024-02-05 00:40:43.000000 alabamaEncoder-0.3/alabamaEncode/metrics/impl/vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      117 2024-02-04 12:09:55.000000 alabamaEncoder-0.3/alabamaEncode/metrics/metric.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      373 2024-02-04 12:36:30.000000 alabamaEncoder-0.3/alabamaEncode/metrics/options.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      308 2024-02-02 14:53:33.000000 alabamaEncoder-0.3/alabamaEncode/metrics/result.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.894717 alabamaEncoder-0.3/alabamaEncode/parallelEncoding/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2357 2024-01-07 02:35:39.000000 alabamaEncoder-0.3/alabamaEncode/parallelEncoding/CeleryApp.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3848 2023-11-19 23:24:09.000000 alabamaEncoder-0.3/alabamaEncode/parallelEncoding/CeleryAutoscaler.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-16 16:38:33.000000 alabamaEncoder-0.3/alabamaEncode/parallelEncoding/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      148 2023-11-05 09:04:10.000000 alabamaEncoder-0.3/alabamaEncode/parallelEncoding/command.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     8001 2024-02-05 23:23:24.000000 alabamaEncoder-0.3/alabamaEncode/parallelEncoding/execute_commands.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      581 2024-01-07 00:27:19.000000 alabamaEncoder-0.3/alabamaEncode/parallelEncoding/worker.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.894717 alabamaEncoder-0.3/alabamaEncode/scene/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-15 20:18:27.000000 alabamaEncoder-0.3/alabamaEncode/scene/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     8712 2024-01-28 07:34:00.000000 alabamaEncoder-0.3/alabamaEncode/scene/chunk.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10414 2024-01-29 15:55:32.000000 alabamaEncoder-0.3/alabamaEncode/scene/concat.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4874 2024-01-28 07:36:56.000000 alabamaEncoder-0.3/alabamaEncode/scene/sequence.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11307 2024-01-28 07:36:58.000000 alabamaEncoder-0.3/alabamaEncode/scene/split.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.894717 alabamaEncoder-0.3/alabamaEncode_frontends/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:32:46.000000 alabamaEncoder-0.3/alabamaEncode_frontends/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.894717 alabamaEncoder-0.3/alabamaEncode_frontends/cli/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:52:09.000000 alabamaEncoder-0.3/alabamaEncode_frontends/cli/__init__.py
+-rwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)     4369 2023-12-28 09:15:33.000000 alabamaEncoder-0.3/alabamaEncode_frontends/cli/__main__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.894717 alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 18:44:18.000000 alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4148 2023-12-27 17:17:40.000000 alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/autopaths.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    19854 2024-02-12 05:32:29.000000 alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/cli_args.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      973 2023-12-10 22:17:58.000000 alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/paths.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1088 2024-01-23 00:24:16.000000 alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/ratecontrol.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1130 2023-12-10 18:44:44.000000 alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/res_preset.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      321 2023-12-28 09:17:41.000000 alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/validate_codecs.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1144 2024-01-15 02:14:38.000000 alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/video_filters.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.894717 alabamaEncoder-0.3/alabamaEncode_frontends/demon/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:38:55.000000 alabamaEncoder-0.3/alabamaEncode_frontends/demon/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2277 2023-12-24 15:12:07.000000 alabamaEncoder-0.3/alabamaEncode_frontends/demon/demon.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-03-05 20:19:58.894717 alabamaEncoder-0.3/alabamaEncoder.egg-info/
+-rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      221 2024-03-05 20:19:58.000000 alabamaEncoder-0.3/alabamaEncoder.egg-info/PKG-INFO
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6013 2024-03-05 20:19:58.000000 alabamaEncoder-0.3/alabamaEncoder.egg-info/SOURCES.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        1 2024-03-05 20:19:58.000000 alabamaEncoder-0.3/alabamaEncoder.egg-info/dependency_links.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       77 2024-03-05 20:19:58.000000 alabamaEncoder-0.3/alabamaEncoder.egg-info/entry_points.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       60 2024-03-05 20:19:58.000000 alabamaEncoder-0.3/alabamaEncoder.egg-info/requires.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-03-05 20:19:58.000000 alabamaEncoder-0.3/alabamaEncoder.egg-info/top_level.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-03-05 20:19:58.894717 alabamaEncoder-0.3/setup.cfg
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      416 2024-03-05 20:18:11.000000 alabamaEncoder-0.3/setup.py
```

### Comparing `alabamaEncoder-0.2/alabamaEncode/ai_vmaf/aom_firstpass.py` & `alabamaEncoder-0.3/alabamaEncode/ai_vmaf/aom_firstpass.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/ai_vmaf/perdict.py` & `alabamaEncoder-0.3/alabamaEncode/ai_vmaf/perdict.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/ai_vmaf/train/train.py` & `alabamaEncoder-0.3/alabamaEncode/ai_vmaf/train/train.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_step.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_step.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/weirdX264.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/weirdX264.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/opinionated_vmaf.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/opinionated_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/pipelines.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/pipelines.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/refine_steps/multires_package.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/refine_steps/multires_package.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/args_tune.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/args_tune.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/autocrop.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/autocrop.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/denoise_filtering.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/denoise_filtering.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/encoding_tiles.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/encoding_tiles.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/ideal_crf.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/ideal_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/sequence_autograin.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/sequence_autograin.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/conent_analysis/sequence/x264_tune.py` & `alabamaEncoder-0.3/alabamaEncode/conent_analysis/sequence/x264_tune.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/core/alabama.py` & `alabamaEncoder-0.3/alabamaEncode/core/alabama.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/core/alamaba_kv.py` & `alabamaEncoder-0.3/alabamaEncode/core/alamaba_kv.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/core/bin_utils.py` & `alabamaEncoder-0.3/alabamaEncode/core/bin_utils.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/core/chunk_job.py` & `alabamaEncoder-0.3/alabamaEncode/core/chunk_job.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/core/cli_executor.py` & `alabamaEncoder-0.3/alabamaEncode/core/cli_executor.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/core/ffmpeg.py` & `alabamaEncoder-0.3/alabamaEncode/core/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/core/final_touches.py` & `alabamaEncoder-0.3/alabamaEncode/core/final_touches.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/core/job.py` & `alabamaEncoder-0.3/alabamaEncode/core/job.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/core/path.py` & `alabamaEncoder-0.3/alabamaEncode/core/path.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/core/timer.py` & `alabamaEncoder-0.3/alabamaEncode/core/timer.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/core/ws_update.py` & `alabamaEncoder-0.3/alabamaEncode/core/ws_update.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/codec.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/codec.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/encoder.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/encoder_factory.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/encoder_factory.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/impl/Aomenc.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/impl/Aomenc.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/impl/Nvenc.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/impl/Nvenc.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/impl/SvtAvif.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/impl/SvtAvif.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/impl/Svtenc.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/impl/Svtenc.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/impl/VaapiH264.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/impl/VaapiH264.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/impl/VaapiH265.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/impl/VaapiH265.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/impl/X264.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/impl/X264.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/impl/X265.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/impl/X265.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/impl/rav1e.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/impl/rav1e.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/impl/vp9.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/impl/vp9.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/encoder/stats.py` & `alabamaEncoder-0.3/alabamaEncode/encoder/stats.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/Aq.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/Aq.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/Overlays.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/Overlays.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/Svtav1Speed.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/Svtav1Speed.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/Svtav1Tunes.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/Svtav1Tunes.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/TemporalFiltering.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/TemporalFiltering.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/ai_feature_extract.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/ai_feature_extract.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/convexhull.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/convexhull.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/crf_vmaf_relation.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/crf_vmaf_relation.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/denoise.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/denoise.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/sequence_convex.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/sequence_convex.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/streaming_output.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/streaming_output.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/superres.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/superres.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/target_vmaf.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/target_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/experiments/util/ExperimentUtil.py` & `alabamaEncoder-0.3/alabamaEncode/experiments/util/ExperimentUtil.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/metrics/calculate.py` & `alabamaEncoder-0.3/alabamaEncode/metrics/calculate.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/metrics/comparison_display.py` & `alabamaEncoder-0.3/alabamaEncode/metrics/comparison_display.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/metrics/image.py` & `alabamaEncoder-0.3/alabamaEncode/metrics/image.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/metrics/impl/psnr.py` & `alabamaEncoder-0.3/alabamaEncode/metrics/impl/psnr.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/metrics/impl/ssim.py` & `alabamaEncoder-0.3/alabamaEncode/metrics/impl/ssim.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/metrics/impl/ssimu2.py` & `alabamaEncoder-0.3/alabamaEncode/metrics/impl/ssimu2.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/metrics/impl/vmaf.py` & `alabamaEncoder-0.3/alabamaEncode/metrics/impl/vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/parallelEncoding/CeleryApp.py` & `alabamaEncoder-0.3/alabamaEncode/parallelEncoding/CeleryApp.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/parallelEncoding/CeleryAutoscaler.py` & `alabamaEncoder-0.3/alabamaEncode/parallelEncoding/CeleryAutoscaler.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/parallelEncoding/execute_commands.py` & `alabamaEncoder-0.3/alabamaEncode/parallelEncoding/execute_commands.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/parallelEncoding/worker.py` & `alabamaEncoder-0.3/alabamaEncode/parallelEncoding/worker.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/scene/chunk.py` & `alabamaEncoder-0.3/alabamaEncode/scene/chunk.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/scene/concat.py` & `alabamaEncoder-0.3/alabamaEncode/scene/concat.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/scene/sequence.py` & `alabamaEncoder-0.3/alabamaEncode/scene/sequence.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode/scene/split.py` & `alabamaEncoder-0.3/alabamaEncode/scene/split.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode_frontends/cli/__main__.py` & `alabamaEncoder-0.3/alabamaEncode_frontends/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/autopaths.py` & `alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/autopaths.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/cli_args.py` & `alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/cli_args.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/paths.py` & `alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/paths.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/ratecontrol.py` & `alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/ratecontrol.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/res_preset.py` & `alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/res_preset.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode_frontends/cli/cli_setup/video_filters.py` & `alabamaEncoder-0.3/alabamaEncode_frontends/cli/cli_setup/video_filters.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncode_frontends/demon/demon.py` & `alabamaEncoder-0.3/alabamaEncode_frontends/demon/demon.py`

 * *Files identical despite different names*

### Comparing `alabamaEncoder-0.2/alabamaEncoder.egg-info/SOURCES.txt` & `alabamaEncoder-0.3/alabamaEncoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

