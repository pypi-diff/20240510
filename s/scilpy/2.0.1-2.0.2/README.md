# Comparing `tmp/scilpy-2.0.1.tar.gz` & `tmp/scilpy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scilpy-2.0.1.tar", last modified: Wed May  8 13:54:08 2024, max compression
+gzip compressed data, was "scilpy-2.0.2.tar", last modified: Fri May 10 13:59:07 2024, max compression
```

## Comparing `scilpy-2.0.1.tar` & `scilpy-2.0.2.tar`

### file list

```diff
@@ -1,667 +1,667 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.972408 scilpy-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 13:54:04.000000 scilpy-2.0.1/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-08 13:54:04.000000 scilpy-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-08 13:54:04.000000 scilpy-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-08 13:54:08.972408 scilpy-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-08 13:54:04.000000 scilpy-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.880409 scilpy-2.0.1/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.884409 scilpy-2.0.1/data/LUT/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-08 13:54:04.000000 scilpy-2.0.1/data/LUT/dk_aggregate_structures.json
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-08 13:54:04.000000 scilpy-2.0.1/data/LUT/freesurfer_desikan_killiany.json
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-08 13:54:04.000000 scilpy-2.0.1/data/LUT/freesurfer_subcortical.json
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 13:54:04.000000 scilpy-2.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.884409 scilpy-2.0.1/scilpy/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.884409 scilpy-2.0.1/scilpy/connectivity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/connectivity/connectivity_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.884409 scilpy-2.0.1/scilpy/denoise/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/denoise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/denoise/asym_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.884409 scilpy-2.0.1/scilpy/dwi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/dwi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13348 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/dwi/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.888409 scilpy-2.0.1/scilpy/dwi/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/dwi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/dwi/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/dwi/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/dwi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.888409 scilpy-2.0.1/scilpy/gpuparallel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/gpuparallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/gpuparallel/opencl_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.888409 scilpy-2.0.1/scilpy/gradients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/gradients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9265 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/gradients/bvec_bval_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/gradients/gen_gradient_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/gradients/optimize_gradient_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/gradients/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.888409 scilpy-2.0.1/scilpy/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11842 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/image/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/image/reslice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.888409 scilpy-2.0.1/scilpy/image/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/image/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/image/tests/test_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    19939 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/image/tests/test_volume_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/image/tests/test_volume_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/image/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/image/volume_b0_synthesis.py
--rw-r--r--   0 runner    (1001) docker     (127)    28583 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/image/volume_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/image/volume_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/image/volume_space_management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.892409 scilpy-2.0.1/scilpy/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/io/btensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/io/deprecator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/io/dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/io/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/io/gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/io/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/io/mti.py
--rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/io/streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/io/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    41807 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/io/varian_fdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.892409 scilpy-2.0.1/scilpy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/preprocessing/distortion_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.892409 scilpy-2.0.1/scilpy/reconst/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/reconst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/reconst/aodf.py
--rw-r--r--   0 runner    (1001) docker     (127)    15013 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/reconst/bingham.py
--rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/reconst/divide.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/reconst/fiber_coherence.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/reconst/fodf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/reconst/frf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12998 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/reconst/mti.py
--rw-r--r--   0 runner    (1001) docker     (127)    26961 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/reconst/sh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/reconst/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.892409 scilpy-2.0.1/scilpy/segment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/segment/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/segment/recobundlesx.py
--rw-r--r--   0 runner    (1001) docker     (127)    17573 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/segment/streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)    24047 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/segment/tractogram_from_roi.py
--rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/segment/voting_scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.892409 scilpy-2.0.1/scilpy/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/stats/matrix_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/stats/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    20428 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/stats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.896409 scilpy-2.0.1/scilpy/tracking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21531 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tracking/propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tracking/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)    25055 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tracking/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tracking/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.896409 scilpy-2.0.1/scilpy/tractanalysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/afd_along_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/bingham_metric_along_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)    12383 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/bundle_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/distance_to_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/grid_intersections.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/quick_tools.pyx
--rwxr-xr-x   0 runner    (1001) docker     (127)    24443 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/reproducibility_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/streamlines_metrics.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    14376 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/todi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/todi_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractanalysis/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.896409 scilpy-2.0.1/scilpy/tractograms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractograms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractograms/dps_and_dpp_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractograms/lazy_tractogram_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    16446 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractograms/streamline_and_mask_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    27844 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractograms/streamline_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.900409 scilpy-2.0.1/scilpy/tractograms/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractograms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractograms/tests/test_dps_and_dpp_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractograms/tests/test_streamline_and_mask_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    13641 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractograms/tests/test_streamline_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractograms/tests/test_tractogram_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    32727 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractograms/tractogram_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    15120 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/tractograms/uncompress.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.900409 scilpy-2.0.1/scilpy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/utils/filenames.py
--rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/utils/metrics_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/utils/spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.900409 scilpy-2.0.1/scilpy/viz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.900409 scilpy-2.0.1/scilpy/viz/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/viz/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/viz/backends/fury.py
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/viz/backends/pil.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/viz/backends/vtk.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/viz/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/viz/gradients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.900409 scilpy-2.0.1/scilpy/viz/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/viz/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/viz/legacy/chord_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/viz/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/viz/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-08 13:54:04.000000 scilpy-2.0.1/scilpy/viz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.972408 scilpy-2.0.1/scilpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-08 13:54:08.000000 scilpy-2.0.1/scilpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25180 2024-05-08 13:54:08.000000 scilpy-2.0.1/scilpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:54:08.000000 scilpy-2.0.1/scilpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25270 2024-05-08 13:54:08.000000 scilpy-2.0.1/scilpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-08 13:54:08.000000 scilpy-2.0.1/scilpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 13:54:08.000000 scilpy-2.0.1/scilpy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.928408 scilpy-2.0.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.948408 scilpy-2.0.1/scripts/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_add_tracking_mask_to_pft_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      446 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_analyse_lesions_load.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_apply_bias_field_on_dwi.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_apply_transform_to_bvecs.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_apply_transform_to_hdf5.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_apply_transform_to_image.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_apply_transform_to_surface.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      484 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_apply_transform_to_tractogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_assign_custom_color_to_tractogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_assign_uniform_color_to_tractograms.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_clean_qbx_clusters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      489 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_combine_labels.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      546 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compare_connectivity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compress_streamlines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_MT_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      417 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_NODDI.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_NODDI_priors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      432 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_asym_odf_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_bundle_mean_std.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_bundle_mean_std_per_point.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_bundle_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_bundle_volume_per_label.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      464 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_bundle_voxel_label_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_centroid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      540 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_connectivity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_divide.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_dti_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_endpoints_map.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_fodf_max_in_ventricles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_fodf_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      429 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_freewater.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_hdf5_average_density_map.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      427 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_ihMT_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      430 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_kurtosis_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      466 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_lobe_specific_fodf_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      434 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_local_tracking.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      464 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_local_tracking_dev.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      477 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_maps_for_particle_filter_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_mean_fixel_afd_from_bundles.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_mean_fixel_afd_from_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_mean_fixel_lobe_metric_from_bundles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_mean_frf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_memsmt_fodf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_memsmt_frf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      468 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_metrics_stats_in_ROI.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_msmt_fodf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_msmt_frf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      443 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_pca.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_pft.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_powder_average.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      431 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_qball_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_qbx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_rish_from_sh.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_seed_by_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_seed_density_map.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      418 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_sf_from_sh.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_sh_from_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_ssst_fodf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_ssst_frf.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_streamlines_density_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_streamlines_length_stats.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      440 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_compute_todi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      429 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_concatenate_dwi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_convert_fdf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      523 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_convert_gradients_fsl_to_mrtrix.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      523 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_convert_gradients_mrtrix_to_fsl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_convert_json_to_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_convert_rgb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_convert_sh_basis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_convert_surface.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_convert_tensors.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_convert_tractogram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      480 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_count_non_zero_voxels.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_count_streamlines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_crop_volume.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      451 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_cut_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_decompose_connectivity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      480 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_detect_dwi_volume_outliers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_detect_streamlines_loops.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      486 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_dilate_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_estimate_bundles_diameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_evaluate_bundles_binary_classification_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_evaluate_bundles_individual_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_evaluate_bundles_pairwise_agreement_measures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      570 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_evaluate_connectivity_graph_measures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      592 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_evaluate_connectivity_pairwise_agreement_measures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      506 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_execute_angle_aware_bilateral_filtering.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      506 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_execute_asymmetric_filtering.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_extract_b0.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      435 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_extract_dwi_shell.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_extract_ushape.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      519 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_filter_connectivity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      484 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_filter_streamlines_by_length.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      499 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_filter_streamlines_by_orientation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      449 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_filter_tractogram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      489 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_filter_tractogram_anatomically.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      433 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_fit_bingham_to_fodf.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_fix_dsi_studio_trk.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      484 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_flip_gradients.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      430 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_flip_streamlines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      438 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_flip_surface.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      417 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_flip_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_generate_gradient_sampling.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      536 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_generate_priors_from_bundle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      462 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_group_comparison.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      456 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_harmonize_json.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_image_math.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      456 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_merge_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_merge_sh.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      528 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_normalize_connectivity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      445 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_outlier_rejection.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_perform_majority_vote.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_plot_mean_std_per_point.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_prepare_eddy_command.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_prepare_topup_command.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      564 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_print_connectivity_filenames.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_print_header.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_project_streamlines_to_map.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      459 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_recognize_multi_bundles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_recognize_single_bundle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_register_tractogram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      479 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_remove_invalid_streamlines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      486 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_remove_labels.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      464 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_remove_outliers_ransac.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      532 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_reorder_connectivity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      441 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_reorder_dwi_philips.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      494 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_resample_bvals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_resample_streamlines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_resample_tractogram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_resample_volume.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_reshape_to_reference.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_run_commit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      429 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_run_nlmeans.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_save_connections_from_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_score_bundles.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_score_tractogram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_screenshot_bundle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      433 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_screenshot_dti.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_screenshot_volume.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      489 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_screenshot_volume_mosaic_overlap.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_set_response_function.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      439 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_shuffle_streamlines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_smooth_streamlines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      444 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_smooth_surface.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_snr_in_roi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      435 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_split_image.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      432 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_split_tractogram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      518 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_split_volume_by_ids.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      522 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_split_volume_by_labels.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      430 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_streamlines_math.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_swap_gradient_axis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      496 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_uniformize_streamlines_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_validate_and_correct_bvecs.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_validate_and_correct_eddy_gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_validate_bids.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_verify_space_attributes_compatibility.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      434 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_visualize_bingham_fit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_visualize_bundles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_visualize_bundles_mosaic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_visualize_connectivity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_visualize_fodf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_visualize_gradients.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_visualize_histogram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_visualize_scatterplot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      438 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_visualize_seeds.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/legacy/scil_visualize_seeds_3d.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7063 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_NODDI_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8298 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_NODDI_priors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8233 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_aodf_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18872 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bids_validate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5295 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bingham_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10051 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_btensor_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12336 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_clean_qbx_clusters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2013 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_compute_centroid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3939 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_compute_endpoints_map.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14156 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_diameter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5149 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_filter_by_occurence.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7046 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_generate_priors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12474 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_label_map.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3111 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_mean_fixel_afd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4885 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_mean_fixel_afd_from_hdf5.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3991 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_mean_fixel_bingham_metric.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6545 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_mean_std.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15129 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_pairwise_comparison.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3361 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_reject_outliers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9287 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_score_many_bundles_one_tractogram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9955 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_score_same_bundle_many_segmentations.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13443 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_shape_measures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2218 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_bundle_volume_per_label.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5771 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_connectivity_compare_populations.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20482 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_connectivity_compute_matrices.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13198 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_connectivity_compute_pca.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6076 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_connectivity_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5105 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_connectivity_graph_measures.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4076 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_connectivity_hdf5_average_density_map.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5213 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_connectivity_math.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6932 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_connectivity_normalize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3478 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_connectivity_pairwise_agreement.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2380 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_connectivity_print_filenames.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6188 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_connectivity_reorder_rois.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4407 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_denoising_nlmeans.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12102 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dki_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dti_convert_tensors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18355 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dti_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2435 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dwi_apply_bias_field.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7338 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dwi_compute_snr.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3471 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dwi_concatenate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2675 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dwi_convert_FDF.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2687 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dwi_detect_volume_outliers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4645 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dwi_extract_b0.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3773 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dwi_extract_shell.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4752 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dwi_powder_average.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9621 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dwi_prepare_eddy_command.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5651 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dwi_prepare_topup_command.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3695 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dwi_reorder_philips.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4005 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dwi_split_by_indices.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3604 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_dwi_to_sh.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4072 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_fodf_max_in_ventricles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11519 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_fodf_memsmt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9239 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_fodf_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9921 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_fodf_msmt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5301 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_fodf_ssst.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4290 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_fodf_to_bingham.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7082 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_freewater_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_freewater_priors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2044 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_frf_mean.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13178 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_frf_memsmt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10732 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_frf_msmt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2170 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_frf_set_diffusivities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5179 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_frf_ssst.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4128 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_get_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1719 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_gradients_apply_transform.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2243 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_gradients_convert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8202 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_gradients_generate_sampling.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4673 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_gradients_modify_axes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2421 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_gradients_round_bvals.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4838 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_gradients_validate_correct.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2226 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_gradients_validate_correct_eddy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2135 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_header_print_info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1262 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_header_validate_compatibility.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17341 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_json_convert_entries_to_xlsx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2713 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_json_harmonize_entries.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3567 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_json_merge_entries.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5194 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_labels_combine.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3812 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_labels_dilate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2002 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_labels_remove.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3435 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_labels_split_volume_by_ids.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3409 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_labels_split_volume_from_lut.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6747 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_lesions_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_mti_adjust_B1_header.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12294 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_mti_maps_MT.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14037 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_mti_maps_ihMT.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5740 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_plot_stats_per_point.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7952 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_qball_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2386 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_rgb_convert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6931 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_search_keywords.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2284 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_sh_convert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2339 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_sh_fusion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7934 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_sh_to_aodf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3337 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_sh_to_rish.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8271 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_sh_to_sf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10017 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_stats_group_comparison.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2609 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_surface_apply_transform.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2753 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_surface_convert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1878 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_surface_flip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2725 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_surface_smooth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11939 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tracking_local.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13166 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tracking_local_dev.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12588 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tracking_pft.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3629 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tracking_pft_maps.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tracking_pft_maps_edit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6970 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_apply_transform.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5760 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_apply_transform_to_hdf5.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10265 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_assign_custom_color.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5205 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_assign_uniform_color.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22039 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_commit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2178 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_compress.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6288 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_compute_TODI.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2691 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_compute_density_map.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1956 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_convert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5105 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_convert_hdf5_to_trk.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1674 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_count_streamlines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6984 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_cut_streamlines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4930 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_detect_loops.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9616 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_dpp_math.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3362 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_extract_ushape.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22160 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_filter_by_anatomy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2678 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_filter_by_length.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4885 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_filter_by_orientation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16674 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_filter_by_roi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10789 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_fix_trk.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1914 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_flip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7974 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     5197 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_pairwise_comparison.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2593 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_print_info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6369 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_project_map_to_streamlines.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9746 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_project_streamlines_to_map.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3359 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_qbx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3545 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_register.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3767 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_remove_invalid.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6921 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_resample.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2154 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_resample_nb_points.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4180 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_seed_density_map.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19762 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_segment_and_score.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5713 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_segment_bundles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19632 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_segment_bundles_for_connectivity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6467 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_segment_one_bundle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1598 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_shuffle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3995 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_smooth.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5101 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_split.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4698 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_tractogram_uniformize_endpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5076 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_bingham_fit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8780 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_bundle.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12686 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_bundle_screenshot_mni.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13215 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_bundle_screenshot_mosaic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14636 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_connectivity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8551 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_dti_screenshot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15553 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_fodf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6852 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_gradients_screenshot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2540 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_tractogram_seeds.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4150 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_tractogram_seeds_3d.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2918 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_volume_histogram.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10693 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_volume_scatterplot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8048 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_volume_screenshot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6474 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_viz_volume_screenshot_mosaic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2889 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_volume_apply_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_volume_b0_synthesis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3135 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_volume_count_non_zero_voxels.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3090 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_volume_crop.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1545 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_volume_flip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5323 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_volume_math.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2802 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_volume_remove_outliers_ransac.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3937 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_volume_resample.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2205 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_volume_reshape_to_reference.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5355 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_volume_stats_in_ROI.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2020 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/scil_volume_stats_in_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:08.972408 scilpy-2.0.1/scripts/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_NODDI_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_NODDI_priors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_aodf_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bids_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bingham_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_btensor_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_clean_qbx_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_compute_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_compute_endpoints_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_diameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_filter_by_occurence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_generate_priors.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_label_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_mean_fixel_afd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_mean_fixel_afd_from_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_mean_fixel_bingham_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_mean_std.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_pairwise_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_reject_outliers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_score_many_bundles_one_tractogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_score_same_bundle_many_segmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_shape_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_bundle_volume_per_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_connectivity_compare_populations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_connectivity_compute_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_connectivity_compute_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_connectivity_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_connectivity_graph_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_connectivity_hdf5_average_density_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_connectivity_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_connectivity_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_connectivity_pairwise_agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_connectivity_print_filenames.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_connectivity_reorder_rois.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_denoising_nlmeans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dki_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dti_convert_tensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dti_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dwi_apply_bias_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dwi_compute_snr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dwi_concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dwi_convert_FDF.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dwi_detect_volume_outliers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dwi_extract_b0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dwi_extract_shell.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dwi_powder_average.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dwi_prepare_eddy_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dwi_prepare_topup_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dwi_reorder_philips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dwi_split_by_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_dwi_to_sh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_fodf_max_in_ventricles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_fodf_memsmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_fodf_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_fodf_msmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_fodf_ssst.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_fodf_to_bingham.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_freewater_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_freewater_priors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_frf_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_frf_memsmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_frf_msmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_frf_set_diffusivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_frf_ssst.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1038 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_gradients_apply_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_gradients_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_gradients_generate_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_gradients_modify_axes.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_gradients_round_bvals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_gradients_validate_correct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_gradients_validate_correct_eddy.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_header_print_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_header_validate_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_json_convert_entries_to_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_json_harmonize_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_json_merge_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_labels_combine.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_labels_dilate.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_labels_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_labels_split_volume_by_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_labels_split_volume_from_lut.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_lesions_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_mti_adjust_B1_header.py
--rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_mti_maps_MT.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_mti_maps_ihMT.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_plot_stats_per_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_qball_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_rgb_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_search_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_sh_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_sh_fusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_sh_to_aodf.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_sh_to_rish.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2801 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_sh_to_sf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_stats_group_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_surface_apply_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_surface_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_surface_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_surface_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tracking_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tracking_local_dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tracking_pft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tracking_pft_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tracking_pft_maps_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_apply_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_apply_transform_to_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_assign_custom_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_assign_uniform_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_commit.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_compute_TODI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_compute_density_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_convert_hdf5_to_trk.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_count_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_cut_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_detect_loops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_dpp_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_extract_ushape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_filter_by_anatomy.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_filter_by_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_filter_by_orientation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_filter_by_roi.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_fix_trk.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_pairwise_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_print_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_project_map_to_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_project_streamlines_to_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_qbx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_remove_invalid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_resample_nb_points.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_seed_density_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_segment_and_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_segment_bundles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_segment_bundles_for_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_segment_one_bundles.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_tractogram_uniformize_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_bingham_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_bundle_screenshot_mni.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_bundle_screenshot_mosaic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_dti_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_fodf.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_gradients_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_tractogram_seeds.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_tractogram_seeds_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_volume_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_volume_scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_volume_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_viz_volume_screenshot_mosaic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_volume_apply_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_volume_b0_synthesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_volume_count_non_zero_voxels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_volume_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_volume_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_volume_math.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_volume_remove_outliers_ransac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_volume_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_volume_reshape_to_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_volume_stats_in_ROI.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-08 13:54:04.000000 scilpy-2.0.1/scripts/tests/test_volume_stats_in_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:54:08.972408 scilpy-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-08 13:54:04.000000 scilpy-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.950593 scilpy-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 13:59:02.000000 scilpy-2.0.2/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-10 13:59:02.000000 scilpy-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-10 13:59:02.000000 scilpy-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-10 13:59:07.950593 scilpy-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-10 13:59:02.000000 scilpy-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.858593 scilpy-2.0.2/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.862593 scilpy-2.0.2/data/LUT/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-10 13:59:02.000000 scilpy-2.0.2/data/LUT/dk_aggregate_structures.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-10 13:59:02.000000 scilpy-2.0.2/data/LUT/freesurfer_desikan_killiany.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-10 13:59:02.000000 scilpy-2.0.2/data/LUT/freesurfer_subcortical.json
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-10 13:59:02.000000 scilpy-2.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.862593 scilpy-2.0.2/scilpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.866593 scilpy-2.0.2/scilpy/connectivity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/connectivity/connectivity_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.866593 scilpy-2.0.2/scilpy/denoise/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/denoise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/denoise/asym_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.866593 scilpy-2.0.2/scilpy/dwi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/dwi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13348 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/dwi/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.866593 scilpy-2.0.2/scilpy/dwi/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/dwi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/dwi/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/dwi/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/dwi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.866593 scilpy-2.0.2/scilpy/gpuparallel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/gpuparallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/gpuparallel/opencl_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.866593 scilpy-2.0.2/scilpy/gradients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/gradients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9265 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/gradients/bvec_bval_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/gradients/gen_gradient_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/gradients/optimize_gradient_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/gradients/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.866593 scilpy-2.0.2/scilpy/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11842 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/image/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/image/reslice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.870593 scilpy-2.0.2/scilpy/image/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/image/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/image/tests/test_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19939 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/image/tests/test_volume_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/image/tests/test_volume_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/image/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/image/volume_b0_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28583 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/image/volume_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/image/volume_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/image/volume_space_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.870593 scilpy-2.0.2/scilpy/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/io/btensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/io/deprecator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/io/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/io/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/io/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/io/mti.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/io/streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/io/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41807 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/io/varian_fdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.870593 scilpy-2.0.2/scilpy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/preprocessing/distortion_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.870593 scilpy-2.0.2/scilpy/reconst/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/reconst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/reconst/aodf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15013 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/reconst/bingham.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/reconst/divide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/reconst/fiber_coherence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/reconst/fodf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/reconst/frf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12998 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/reconst/mti.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26961 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/reconst/sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/reconst/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.874593 scilpy-2.0.2/scilpy/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/segment/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/segment/recobundlesx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17573 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/segment/streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24047 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/segment/tractogram_from_roi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14126 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/segment/voting_scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.874593 scilpy-2.0.2/scilpy/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/stats/matrix_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/stats/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20428 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/stats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.874593 scilpy-2.0.2/scilpy/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21531 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tracking/propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tracking/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25055 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tracking/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18035 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tracking/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.874593 scilpy-2.0.2/scilpy/tractanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/afd_along_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/bingham_metric_along_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12383 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/bundle_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/distance_to_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/grid_intersections.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/quick_tools.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24443 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/reproducibility_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/streamlines_metrics.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    14376 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/todi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/todi_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractanalysis/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.878593 scilpy-2.0.2/scilpy/tractograms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractograms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractograms/dps_and_dpp_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractograms/lazy_tractogram_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16446 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractograms/streamline_and_mask_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27844 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractograms/streamline_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.878593 scilpy-2.0.2/scilpy/tractograms/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractograms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractograms/tests/test_dps_and_dpp_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractograms/tests/test_streamline_and_mask_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13641 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractograms/tests/test_streamline_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractograms/tests/test_tractogram_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32727 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractograms/tractogram_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15120 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/tractograms/uncompress.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.878593 scilpy-2.0.2/scilpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/utils/filenames.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13529 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/utils/metrics_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/utils/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.878593 scilpy-2.0.2/scilpy/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.878593 scilpy-2.0.2/scilpy/viz/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/viz/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/viz/backends/fury.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/viz/backends/pil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/viz/backends/vtk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/viz/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/viz/gradients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.878593 scilpy-2.0.2/scilpy/viz/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/viz/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/viz/legacy/chord_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/viz/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/viz/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-10 13:59:02.000000 scilpy-2.0.2/scilpy/viz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.950593 scilpy-2.0.2/scilpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-10 13:59:07.000000 scilpy-2.0.2/scilpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25172 2024-05-10 13:59:07.000000 scilpy-2.0.2/scilpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:59:07.000000 scilpy-2.0.2/scilpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25262 2024-05-10 13:59:07.000000 scilpy-2.0.2/scilpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-10 13:59:07.000000 scilpy-2.0.2/scilpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 13:59:07.000000 scilpy-2.0.2/scilpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.902593 scilpy-2.0.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.926593 scilpy-2.0.2/scripts/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_add_tracking_mask_to_pft_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      446 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_analyse_lesions_load.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_apply_bias_field_on_dwi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      458 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_apply_transform_to_bvecs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      472 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_apply_transform_to_hdf5.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      471 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_apply_transform_to_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_apply_transform_to_surface.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      484 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_apply_transform_to_tractogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      496 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_assign_custom_color_to_tractogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      499 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_assign_uniform_color_to_tractograms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_clean_qbx_clusters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      489 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_combine_labels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      546 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compare_connectivity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compress_streamlines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_MT_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      417 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_NODDI.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_NODDI_priors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      432 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_asym_odf_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_bundle_mean_std.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      530 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_bundle_mean_std_per_point.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      490 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_bundle_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      479 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_bundle_volume_per_label.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      464 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_bundle_voxel_label_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      446 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_centroid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      540 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_connectivity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_divide.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_dti_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      461 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_endpoints_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_fodf_max_in_ventricles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_fodf_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      429 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_freewater.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      508 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_hdf5_average_density_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      427 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_ihMT_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      430 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_kurtosis_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      466 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_lobe_specific_fodf_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      434 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_local_tracking.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      464 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_local_tracking_dev.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      477 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_maps_for_particle_filter_tracking.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      474 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_mean_fixel_afd_from_bundles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      481 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_mean_fixel_afd_from_hdf5.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      509 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_mean_fixel_lobe_metric_from_bundles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_mean_frf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_memsmt_fodf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_memsmt_frf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      468 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_metrics_stats_in_ROI.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_msmt_fodf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_msmt_frf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      443 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_pca.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_pft.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_powder_average.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      431 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_qball_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_qbx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_rish_from_sh.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      449 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_seed_by_labels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      462 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_seed_density_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      418 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_sf_from_sh.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_sh_from_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      419 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_ssst_fodf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_ssst_frf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      493 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_streamlines_density_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_streamlines_length_stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      440 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_compute_todi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      429 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_concatenate_dwi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      425 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_convert_fdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      523 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_convert_gradients_fsl_to_mrtrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      523 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_convert_gradients_mrtrix_to_fsl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_convert_json_to_xlsx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      501 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_convert_rgb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_convert_sh_basis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_convert_surface.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_convert_tensors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      509 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_convert_tractogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      480 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_count_non_zero_voxels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_count_streamlines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_crop_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      451 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_cut_streamlines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_decompose_connectivity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      480 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_detect_dwi_volume_outliers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_detect_streamlines_loops.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      486 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_dilate_labels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      457 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_estimate_bundles_diameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      541 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_evaluate_bundles_binary_classification_measures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      479 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_evaluate_bundles_individual_measures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      498 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_evaluate_bundles_pairwise_agreement_measures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      570 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_evaluate_connectivity_graph_measures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      592 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_evaluate_connectivity_pairwise_agreement_measures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      506 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_execute_angle_aware_bilateral_filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      506 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_execute_asymmetric_filtering.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_extract_b0.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      435 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_extract_dwi_shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_extract_ushape.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      519 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_filter_connectivity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      484 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_filter_streamlines_by_length.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      499 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_filter_streamlines_by_orientation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      449 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_filter_tractogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      489 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_filter_tractogram_anatomically.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      433 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_fit_bingham_to_fodf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      439 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_fix_dsi_studio_trk.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      484 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_flip_gradients.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      430 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_flip_streamlines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      438 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_flip_surface.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      417 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_flip_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      482 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_generate_gradient_sampling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      536 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_generate_priors_from_bundle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      462 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_group_comparison.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      456 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_harmonize_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_image_math.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      456 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_merge_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      410 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_merge_sh.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      528 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_normalize_connectivity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      445 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_outlier_rejection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      458 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_perform_majority_vote.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_plot_mean_std_per_point.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      452 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_prepare_eddy_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      455 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_prepare_topup_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      564 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_print_connectivity_filenames.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      430 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_print_header.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      502 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_project_streamlines_to_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      459 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_recognize_multi_bundles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      465 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_recognize_single_bundle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_register_tractogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      479 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_remove_invalid_streamlines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      486 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_remove_labels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      464 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_remove_outliers_ransac.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      532 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_reorder_connectivity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      441 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_reorder_dwi_philips.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      494 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_resample_bvals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_resample_streamlines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_resample_tractogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_resample_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_reshape_to_reference.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_run_commit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      429 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_run_nlmeans.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_save_connections_from_hdf5.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      483 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_score_bundles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      456 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_score_tractogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_screenshot_bundle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      433 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_screenshot_dti.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_screenshot_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      489 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_screenshot_volume_mosaic_overlap.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_set_response_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      439 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_shuffle_streamlines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_smooth_streamlines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      444 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_smooth_surface.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_snr_in_roi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      435 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_split_image.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      432 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_split_tractogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      518 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_split_volume_by_ids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      522 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_split_volume_by_labels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      430 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_streamlines_math.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_swap_gradient_axis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_uniformize_streamlines_endpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      480 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_validate_and_correct_bvecs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      499 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_validate_and_correct_eddy_gradients.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      441 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_validate_bids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      497 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_verify_space_attributes_compatibility.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      434 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_visualize_bingham_fit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_visualize_bundles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      463 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_visualize_bundles_mosaic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      437 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_visualize_connectivity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_visualize_fodf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_visualize_gradients.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      442 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_visualize_histogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_visualize_scatterplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      438 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_visualize_seeds.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      447 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/legacy/scil_visualize_seeds_3d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7063 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_NODDI_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8298 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_NODDI_priors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8233 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_aodf_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18872 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bids_validate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5295 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bingham_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10051 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_btensor_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12336 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_clean_qbx_clusters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2013 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_compute_centroid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3939 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_compute_endpoints_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14156 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_diameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5149 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_filter_by_occurence.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7046 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_generate_priors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12474 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_label_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3111 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_mean_fixel_afd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4885 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_mean_fixel_afd_from_hdf5.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3991 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_mean_fixel_bingham_metric.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6545 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_mean_std.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15129 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_pairwise_comparison.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3361 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_reject_outliers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9287 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_score_many_bundles_one_tractogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9955 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_score_same_bundle_many_segmentations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13443 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_shape_measures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4698 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_uniformize_endpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2218 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_bundle_volume_per_label.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5771 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_connectivity_compare_populations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20482 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_connectivity_compute_matrices.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13198 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_connectivity_compute_pca.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6076 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_connectivity_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5105 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_connectivity_graph_measures.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4076 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_connectivity_hdf5_average_density_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5213 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_connectivity_math.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6932 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_connectivity_normalize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3478 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_connectivity_pairwise_agreement.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2380 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_connectivity_print_filenames.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6188 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_connectivity_reorder_rois.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4407 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_denoising_nlmeans.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12102 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dki_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dti_convert_tensors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18355 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dti_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2447 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dwi_apply_bias_field.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7338 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dwi_compute_snr.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3471 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dwi_concatenate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2675 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dwi_convert_FDF.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2687 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dwi_detect_volume_outliers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4645 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dwi_extract_b0.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3773 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dwi_extract_shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4752 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dwi_powder_average.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9621 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dwi_prepare_eddy_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5651 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dwi_prepare_topup_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3695 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dwi_reorder_philips.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4005 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dwi_split_by_indices.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3604 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_dwi_to_sh.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4072 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_fodf_max_in_ventricles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11519 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_fodf_memsmt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9239 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_fodf_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9921 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_fodf_msmt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5301 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_fodf_ssst.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4290 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_fodf_to_bingham.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7082 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_freewater_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      233 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_freewater_priors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2044 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_frf_mean.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13178 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_frf_memsmt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10732 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_frf_msmt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2170 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_frf_set_diffusivities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5179 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_frf_ssst.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4128 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_get_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1719 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_gradients_apply_transform.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2243 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_gradients_convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8202 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_gradients_generate_sampling.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4673 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_gradients_modify_axes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2421 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_gradients_round_bvals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4838 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_gradients_validate_correct.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2226 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_gradients_validate_correct_eddy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2135 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_header_print_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1262 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_header_validate_compatibility.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17341 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_json_convert_entries_to_xlsx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2713 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_json_harmonize_entries.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3567 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_json_merge_entries.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5194 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_labels_combine.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3812 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_labels_dilate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2002 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_labels_remove.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3435 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_labels_split_volume_by_ids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3409 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_labels_split_volume_from_lut.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6747 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_lesions_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1657 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_mti_adjust_B1_header.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12294 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_mti_maps_MT.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14037 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_mti_maps_ihMT.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5740 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_plot_stats_per_point.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7952 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_qball_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2386 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_rgb_convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6931 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_search_keywords.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2284 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_sh_convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2339 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_sh_fusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7934 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_sh_to_aodf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3337 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_sh_to_rish.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8271 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_sh_to_sf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10017 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_stats_group_comparison.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2609 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_surface_apply_transform.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2752 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_surface_convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1878 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_surface_flip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2725 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_surface_smooth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11939 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tracking_local.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13166 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tracking_local_dev.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12588 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tracking_pft.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3629 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tracking_pft_maps.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tracking_pft_maps_edit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6970 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_apply_transform.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5760 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_apply_transform_to_hdf5.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10265 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_assign_custom_color.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5205 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_assign_uniform_color.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22039 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_commit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2178 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_compress.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6288 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_compute_TODI.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2691 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_compute_density_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1956 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5105 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_convert_hdf5_to_trk.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1674 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_count_streamlines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6984 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_cut_streamlines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4930 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_detect_loops.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9616 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_dpp_math.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3362 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_extract_ushape.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22160 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_filter_by_anatomy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2678 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_filter_by_length.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4885 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_filter_by_orientation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16674 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_filter_by_roi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10789 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_fix_trk.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1914 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_flip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7974 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_math.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5197 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_pairwise_comparison.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2593 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_print_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6369 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_project_map_to_streamlines.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9746 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_project_streamlines_to_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3359 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_qbx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3545 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_register.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3767 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_remove_invalid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6921 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_resample.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2154 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_resample_nb_points.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4180 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_seed_density_map.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19762 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_segment_and_score.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5713 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_segment_bundles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19632 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_segment_bundles_for_connectivity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6467 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_segment_one_bundle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1598 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_shuffle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3995 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_smooth.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5101 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_tractogram_split.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5076 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_bingham_fit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8780 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_bundle.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12686 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_bundle_screenshot_mni.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13215 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_bundle_screenshot_mosaic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14636 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_connectivity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8551 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_dti_screenshot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15553 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_fodf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6852 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_gradients_screenshot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2540 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_tractogram_seeds.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4150 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_tractogram_seeds_3d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2918 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_volume_histogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10693 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_volume_scatterplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8048 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_volume_screenshot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6474 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_viz_volume_screenshot_mosaic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2889 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_volume_apply_transform.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3404 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_volume_b0_synthesis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3135 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_volume_count_non_zero_voxels.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3090 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_volume_crop.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1545 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_volume_flip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5323 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_volume_math.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2802 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_volume_remove_outliers_ransac.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3937 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_volume_resample.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2205 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_volume_reshape_to_reference.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5355 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_volume_stats_in_ROI.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2020 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/scil_volume_stats_in_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:07.950593 scilpy-2.0.2/scripts/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_NODDI_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_NODDI_priors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_aodf_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14670 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bids_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bingham_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_btensor_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_clean_qbx_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_compute_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_compute_endpoints_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_diameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_filter_by_occurence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_generate_priors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_label_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_mean_fixel_afd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_mean_fixel_afd_from_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_mean_fixel_bingham_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_mean_std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_pairwise_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_reject_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_score_many_bundles_one_tractogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_score_same_bundle_many_segmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_shape_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_uniformize_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_bundle_volume_per_label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_connectivity_compare_populations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_connectivity_compute_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_connectivity_compute_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_connectivity_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_connectivity_graph_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_connectivity_hdf5_average_density_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_connectivity_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_connectivity_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_connectivity_pairwise_agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_connectivity_print_filenames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_connectivity_reorder_rois.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_denoising_nlmeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dki_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dti_convert_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dti_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dwi_apply_bias_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dwi_compute_snr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dwi_concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dwi_convert_FDF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dwi_detect_volume_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dwi_extract_b0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dwi_extract_shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dwi_powder_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dwi_prepare_eddy_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dwi_prepare_topup_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dwi_reorder_philips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dwi_split_by_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_dwi_to_sh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_fodf_max_in_ventricles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_fodf_memsmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_fodf_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_fodf_msmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_fodf_ssst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_fodf_to_bingham.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_freewater_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_freewater_priors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_frf_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_frf_memsmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_frf_msmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_frf_set_diffusivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_frf_ssst.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1038 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_gradients_apply_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_gradients_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_gradients_generate_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_gradients_modify_axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_gradients_round_bvals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_gradients_validate_correct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_gradients_validate_correct_eddy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_header_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_header_validate_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_json_convert_entries_to_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_json_harmonize_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_json_merge_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_labels_combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_labels_dilate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_labels_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_labels_split_volume_by_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_labels_split_volume_from_lut.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_lesions_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_mti_adjust_B1_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_mti_maps_MT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_mti_maps_ihMT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_plot_stats_per_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_qball_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_rgb_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_search_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_sh_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_sh_fusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_sh_to_aodf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_sh_to_rish.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2801 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_sh_to_sf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_stats_group_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_surface_apply_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_surface_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_surface_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_surface_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tracking_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tracking_local_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tracking_pft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tracking_pft_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tracking_pft_maps_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_apply_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_apply_transform_to_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_assign_custom_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_assign_uniform_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_compute_TODI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_compute_density_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_convert_hdf5_to_trk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_count_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_cut_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_detect_loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_dpp_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_extract_ushape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_filter_by_anatomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_filter_by_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_filter_by_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_filter_by_roi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_fix_trk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_pairwise_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_project_map_to_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_project_streamlines_to_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_qbx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_remove_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_resample_nb_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_seed_density_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_segment_and_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_segment_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_segment_bundles_for_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_segment_one_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_tractogram_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_bingham_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_bundle_screenshot_mni.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_bundle_screenshot_mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_dti_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_fodf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_gradients_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_tractogram_seeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_tractogram_seeds_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_volume_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_volume_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_volume_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_viz_volume_screenshot_mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_volume_apply_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_volume_b0_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_volume_count_non_zero_voxels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_volume_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_volume_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_volume_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_volume_remove_outliers_ransac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_volume_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_volume_reshape_to_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_volume_stats_in_ROI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-10 13:59:02.000000 scilpy-2.0.2/scripts/tests/test_volume_stats_in_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:59:07.950593 scilpy-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-10 13:59:02.000000 scilpy-2.0.2/setup.py
```

### Comparing `scilpy-2.0.1/LICENSE` & `scilpy-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/PKG-INFO` & `scilpy-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scilpy
-Version: 2.0.1
+Version: 2.0.2
 Summary: Scilpy: diffusion MRI tools and utilities
 Home-page: https://github.com/scilus/scilpy
 Download-URL: 
 Author: The SCIL developers
 Author-email: 
 Maintainer: Arnaud Boré
 Maintainer-email: arnaud.bore@gmail.com
```

### Comparing `scilpy-2.0.1/README.md` & `scilpy-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/data/LUT/dk_aggregate_structures.json` & `scilpy-2.0.2/data/LUT/dk_aggregate_structures.json`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/data/LUT/freesurfer_desikan_killiany.json` & `scilpy-2.0.2/data/LUT/freesurfer_desikan_killiany.json`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/data/LUT/freesurfer_subcortical.json` & `scilpy-2.0.2/data/LUT/freesurfer_subcortical.json`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/requirements.txt` & `scilpy-2.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/connectivity/connectivity_tools.py` & `scilpy-2.0.2/scilpy/connectivity/connectivity_tools.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/denoise/asym_filtering.py` & `scilpy-2.0.2/scilpy/denoise/asym_filtering.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/dwi/operations.py` & `scilpy-2.0.2/scilpy/dwi/operations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/dwi/tests/test_operations.py` & `scilpy-2.0.2/scilpy/dwi/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/dwi/tests/test_utils.py` & `scilpy-2.0.2/scilpy/dwi/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/dwi/utils.py` & `scilpy-2.0.2/scilpy/dwi/utils.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/gpuparallel/opencl_utils.py` & `scilpy-2.0.2/scilpy/gpuparallel/opencl_utils.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/gradients/bvec_bval_tools.py` & `scilpy-2.0.2/scilpy/gradients/bvec_bval_tools.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/gradients/gen_gradient_sampling.py` & `scilpy-2.0.2/scilpy/gradients/gen_gradient_sampling.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/gradients/optimize_gradient_sampling.py` & `scilpy-2.0.2/scilpy/gradients/optimize_gradient_sampling.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/gradients/utils.py` & `scilpy-2.0.2/scilpy/gradients/utils.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/image/labels.py` & `scilpy-2.0.2/scilpy/image/labels.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/image/reslice.py` & `scilpy-2.0.2/scilpy/image/reslice.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/image/tests/test_labels.py` & `scilpy-2.0.2/scilpy/image/tests/test_labels.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/image/tests/test_volume_math.py` & `scilpy-2.0.2/scilpy/image/tests/test_volume_math.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/image/tests/test_volume_operations.py` & `scilpy-2.0.2/scilpy/image/tests/test_volume_operations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/image/utils.py` & `scilpy-2.0.2/scilpy/image/utils.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/image/volume_b0_synthesis.py` & `scilpy-2.0.2/scilpy/image/volume_b0_synthesis.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/image/volume_math.py` & `scilpy-2.0.2/scilpy/image/volume_math.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/image/volume_operations.py` & `scilpy-2.0.2/scilpy/image/volume_operations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/image/volume_space_management.py` & `scilpy-2.0.2/scilpy/image/volume_space_management.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/io/btensor.py` & `scilpy-2.0.2/scilpy/io/btensor.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/io/deprecator.py` & `scilpy-2.0.2/scilpy/io/deprecator.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/io/dvc.py` & `scilpy-2.0.2/scilpy/io/dvc.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/io/fetcher.py` & `scilpy-2.0.2/scilpy/io/fetcher.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/io/gradients.py` & `scilpy-2.0.2/scilpy/io/gradients.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/io/hdf5.py` & `scilpy-2.0.2/scilpy/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/io/image.py` & `scilpy-2.0.2/scilpy/io/image.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/io/mti.py` & `scilpy-2.0.2/scilpy/io/mti.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/io/streamlines.py` & `scilpy-2.0.2/scilpy/io/streamlines.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/io/tensor.py` & `scilpy-2.0.2/scilpy/io/tensor.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/io/utils.py` & `scilpy-2.0.2/scilpy/io/utils.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/io/varian_fdf.py` & `scilpy-2.0.2/scilpy/io/varian_fdf.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/preprocessing/distortion_correction.py` & `scilpy-2.0.2/scilpy/preprocessing/distortion_correction.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/reconst/aodf.py` & `scilpy-2.0.2/scilpy/reconst/aodf.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/reconst/bingham.py` & `scilpy-2.0.2/scilpy/reconst/bingham.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/reconst/divide.py` & `scilpy-2.0.2/scilpy/reconst/divide.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/reconst/fiber_coherence.py` & `scilpy-2.0.2/scilpy/reconst/fiber_coherence.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/reconst/fodf.py` & `scilpy-2.0.2/scilpy/reconst/fodf.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/reconst/frf.py` & `scilpy-2.0.2/scilpy/reconst/frf.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/reconst/mti.py` & `scilpy-2.0.2/scilpy/reconst/mti.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/reconst/sh.py` & `scilpy-2.0.2/scilpy/reconst/sh.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/reconst/utils.py` & `scilpy-2.0.2/scilpy/reconst/utils.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/segment/models.py` & `scilpy-2.0.2/scilpy/segment/models.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/segment/recobundlesx.py` & `scilpy-2.0.2/scilpy/segment/recobundlesx.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/segment/streamlines.py` & `scilpy-2.0.2/scilpy/segment/streamlines.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/segment/tractogram_from_roi.py` & `scilpy-2.0.2/scilpy/segment/tractogram_from_roi.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/segment/voting_scheme.py` & `scilpy-2.0.2/scilpy/segment/voting_scheme.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/stats/matrix_stats.py` & `scilpy-2.0.2/scilpy/stats/matrix_stats.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/stats/stats.py` & `scilpy-2.0.2/scilpy/stats/stats.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/stats/utils.py` & `scilpy-2.0.2/scilpy/stats/utils.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tracking/propagator.py` & `scilpy-2.0.2/scilpy/tracking/propagator.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tracking/seed.py` & `scilpy-2.0.2/scilpy/tracking/seed.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tracking/tracker.py` & `scilpy-2.0.2/scilpy/tracking/tracker.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tracking/utils.py` & `scilpy-2.0.2/scilpy/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractanalysis/afd_along_streamlines.py` & `scilpy-2.0.2/scilpy/tractanalysis/afd_along_streamlines.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractanalysis/bingham_metric_along_streamlines.py` & `scilpy-2.0.2/scilpy/tractanalysis/bingham_metric_along_streamlines.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractanalysis/bundle_operations.py` & `scilpy-2.0.2/scilpy/tractanalysis/bundle_operations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractanalysis/distance_to_centroid.py` & `scilpy-2.0.2/scilpy/tractanalysis/distance_to_centroid.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractanalysis/grid_intersections.pyx` & `scilpy-2.0.2/scilpy/tractanalysis/grid_intersections.pyx`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractanalysis/json_utils.py` & `scilpy-2.0.2/scilpy/tractanalysis/json_utils.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractanalysis/quick_tools.pyx` & `scilpy-2.0.2/scilpy/tractanalysis/quick_tools.pyx`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractanalysis/reproducibility_measures.py` & `scilpy-2.0.2/scilpy/tractanalysis/reproducibility_measures.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractanalysis/scoring.py` & `scilpy-2.0.2/scilpy/tractanalysis/scoring.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractanalysis/streamlines_metrics.pyx` & `scilpy-2.0.2/scilpy/tractanalysis/streamlines_metrics.pyx`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractanalysis/todi.py` & `scilpy-2.0.2/scilpy/tractanalysis/todi.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractanalysis/todi_util.py` & `scilpy-2.0.2/scilpy/tractanalysis/todi_util.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractanalysis/tools.py` & `scilpy-2.0.2/scilpy/tractanalysis/tools.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractograms/dps_and_dpp_management.py` & `scilpy-2.0.2/scilpy/tractograms/dps_and_dpp_management.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractograms/lazy_tractogram_operations.py` & `scilpy-2.0.2/scilpy/tractograms/lazy_tractogram_operations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractograms/streamline_and_mask_operations.py` & `scilpy-2.0.2/scilpy/tractograms/streamline_and_mask_operations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractograms/streamline_operations.py` & `scilpy-2.0.2/scilpy/tractograms/streamline_operations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractograms/tests/test_dps_and_dpp_management.py` & `scilpy-2.0.2/scilpy/tractograms/tests/test_dps_and_dpp_management.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractograms/tests/test_streamline_and_mask_operations.py` & `scilpy-2.0.2/scilpy/tractograms/tests/test_streamline_and_mask_operations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractograms/tests/test_streamline_operations.py` & `scilpy-2.0.2/scilpy/tractograms/tests/test_streamline_operations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractograms/tests/test_tractogram_operations.py` & `scilpy-2.0.2/scilpy/tractograms/tests/test_tractogram_operations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractograms/tractogram_operations.py` & `scilpy-2.0.2/scilpy/tractograms/tractogram_operations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/tractograms/uncompress.pyx` & `scilpy-2.0.2/scilpy/tractograms/uncompress.pyx`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/utils/__init__.py` & `scilpy-2.0.2/scilpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/utils/filenames.py` & `scilpy-2.0.2/scilpy/utils/filenames.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/utils/metrics_tools.py` & `scilpy-2.0.2/scilpy/utils/metrics_tools.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/utils/spatial.py` & `scilpy-2.0.2/scilpy/utils/spatial.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/version.py` & `scilpy-2.0.2/scilpy/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import itertools
 import glob
 import os
 
 # Format expected by setup.py and doc/source/conf.py: string of form "X.Y.Z"
 _version_major = 2
 _version_minor = 0
-_version_micro = 1
+_version_micro = 2
 _version_extra = ''
 
 # Construct full version string from these.
 _ver = [_version_major, _version_minor, _version_micro]
 
 if _version_extra:
     _ver.append(_version_extra)
```

### Comparing `scilpy-2.0.1/scilpy/viz/backends/fury.py` & `scilpy-2.0.2/scilpy/viz/backends/fury.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/viz/backends/pil.py` & `scilpy-2.0.2/scilpy/viz/backends/pil.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/viz/backends/vtk.py` & `scilpy-2.0.2/scilpy/viz/backends/vtk.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/viz/color.py` & `scilpy-2.0.2/scilpy/viz/color.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/viz/gradients.py` & `scilpy-2.0.2/scilpy/viz/gradients.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/viz/legacy/__init__.py` & `scilpy-2.0.2/scilpy/viz/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/viz/legacy/chord_chart.py` & `scilpy-2.0.2/scilpy/viz/legacy/chord_chart.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/viz/screenshot.py` & `scilpy-2.0.2/scilpy/viz/screenshot.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/viz/slice.py` & `scilpy-2.0.2/scilpy/viz/slice.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy/viz/utils.py` & `scilpy-2.0.2/scilpy/viz/utils.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scilpy.egg-info/PKG-INFO` & `scilpy-2.0.2/scilpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scilpy
-Version: 2.0.1
+Version: 2.0.2
 Summary: Scilpy: diffusion MRI tools and utilities
 Home-page: https://github.com/scilus/scilpy
 Download-URL: 
 Author: The SCIL developers
 Author-email: 
 Maintainer: Arnaud Boré
 Maintainer-email: arnaud.bore@gmail.com
```

### Comparing `scilpy-2.0.1/scilpy.egg-info/SOURCES.txt` & `scilpy-2.0.2/scilpy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -145,14 +145,15 @@
 scripts/scil_bundle_mean_fixel_bingham_metric.py
 scripts/scil_bundle_mean_std.py
 scripts/scil_bundle_pairwise_comparison.py
 scripts/scil_bundle_reject_outliers.py
 scripts/scil_bundle_score_many_bundles_one_tractogram.py
 scripts/scil_bundle_score_same_bundle_many_segmentations.py
 scripts/scil_bundle_shape_measures.py
+scripts/scil_bundle_uniformize_endpoints.py
 scripts/scil_bundle_volume_per_label.py
 scripts/scil_connectivity_compare_populations.py
 scripts/scil_connectivity_compute_matrices.py
 scripts/scil_connectivity_compute_pca.py
 scripts/scil_connectivity_filter.py
 scripts/scil_connectivity_graph_measures.py
 scripts/scil_connectivity_hdf5_average_density_map.py
@@ -267,15 +268,14 @@
 scripts/scil_tractogram_segment_and_score.py
 scripts/scil_tractogram_segment_bundles.py
 scripts/scil_tractogram_segment_bundles_for_connectivity.py
 scripts/scil_tractogram_segment_one_bundle.py
 scripts/scil_tractogram_shuffle.py
 scripts/scil_tractogram_smooth.py
 scripts/scil_tractogram_split.py
-scripts/scil_tractogram_uniformize_endpoints.py
 scripts/scil_viz_bingham_fit.py
 scripts/scil_viz_bundle.py
 scripts/scil_viz_bundle_screenshot_mni.py
 scripts/scil_viz_bundle_screenshot_mosaic.py
 scripts/scil_viz_connectivity.py
 scripts/scil_viz_dti_screenshot.py
 scripts/scil_viz_fodf.py
@@ -483,14 +483,15 @@
 scripts/tests/test_bundle_mean_fixel_bingham_metric.py
 scripts/tests/test_bundle_mean_std.py
 scripts/tests/test_bundle_pairwise_comparison.py
 scripts/tests/test_bundle_reject_outliers.py
 scripts/tests/test_bundle_score_many_bundles_one_tractogram.py
 scripts/tests/test_bundle_score_same_bundle_many_segmentations.py
 scripts/tests/test_bundle_shape_measures.py
+scripts/tests/test_bundle_uniformize_endpoints.py
 scripts/tests/test_bundle_volume_per_label.py
 scripts/tests/test_connectivity_compare_populations.py
 scripts/tests/test_connectivity_compute_matrices.py
 scripts/tests/test_connectivity_compute_pca.py
 scripts/tests/test_connectivity_filter.py
 scripts/tests/test_connectivity_graph_measures.py
 scripts/tests/test_connectivity_hdf5_average_density_map.py
@@ -604,15 +605,14 @@
 scripts/tests/test_tractogram_segment_and_score.py
 scripts/tests/test_tractogram_segment_bundles.py
 scripts/tests/test_tractogram_segment_bundles_for_connectivity.py
 scripts/tests/test_tractogram_segment_one_bundles.py
 scripts/tests/test_tractogram_shuffle.py
 scripts/tests/test_tractogram_smooth.py
 scripts/tests/test_tractogram_split.py
-scripts/tests/test_tractogram_uniformize_endpoints.py
 scripts/tests/test_viz_bingham_fit.py
 scripts/tests/test_viz_bundle.py
 scripts/tests/test_viz_bundle_screenshot_mni.py
 scripts/tests/test_viz_bundle_screenshot_mosaic.py
 scripts/tests/test_viz_connectivity.py
 scripts/tests/test_viz_dti_screenshot.py
 scripts/tests/test_viz_fodf.py
```

### Comparing `scilpy-2.0.1/scilpy.egg-info/entry_points.txt` & `scilpy-2.0.2/scilpy.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 scil_bundle_mean_fixel_bingham_metric.py = scripts.scil_bundle_mean_fixel_bingham_metric:main
 scil_bundle_mean_std.py = scripts.scil_bundle_mean_std:main
 scil_bundle_pairwise_comparison.py = scripts.scil_bundle_pairwise_comparison:main
 scil_bundle_reject_outliers.py = scripts.scil_bundle_reject_outliers:main
 scil_bundle_score_many_bundles_one_tractogram.py = scripts.scil_bundle_score_many_bundles_one_tractogram:main
 scil_bundle_score_same_bundle_many_segmentations.py = scripts.scil_bundle_score_same_bundle_many_segmentations:main
 scil_bundle_shape_measures.py = scripts.scil_bundle_shape_measures:main
+scil_bundle_uniformize_endpoints.py = scripts.scil_bundle_uniformize_endpoints:main
 scil_bundle_volume_per_label.py = scripts.scil_bundle_volume_per_label:main
 scil_clean_qbx_clusters.py = scripts.legacy.scil_clean_qbx_clusters:main
 scil_combine_labels.py = scripts.legacy.scil_combine_labels:main
 scil_compare_connectivity.py = scripts.legacy.scil_compare_connectivity:main
 scil_compress_streamlines.py = scripts.legacy.scil_compress_streamlines:main
 scil_compute_MT_maps.py = scripts.legacy.scil_compute_MT_maps:main
 scil_compute_NODDI.py = scripts.legacy.scil_compute_NODDI:main
@@ -290,15 +291,14 @@
 scil_tractogram_segment_and_score.py = scripts.scil_tractogram_segment_and_score:main
 scil_tractogram_segment_bundles.py = scripts.scil_tractogram_segment_bundles:main
 scil_tractogram_segment_bundles_for_connectivity.py = scripts.scil_tractogram_segment_bundles_for_connectivity:main
 scil_tractogram_segment_one_bundle.py = scripts.scil_tractogram_segment_one_bundle:main
 scil_tractogram_shuffle.py = scripts.scil_tractogram_shuffle:main
 scil_tractogram_smooth.py = scripts.scil_tractogram_smooth:main
 scil_tractogram_split.py = scripts.scil_tractogram_split:main
-scil_tractogram_uniformize_endpoints.py = scripts.scil_tractogram_uniformize_endpoints:main
 scil_uniformize_streamlines_endpoints.py = scripts.legacy.scil_uniformize_streamlines_endpoints:main
 scil_validate_and_correct_bvecs.py = scripts.legacy.scil_validate_and_correct_bvecs:main
 scil_validate_and_correct_eddy_gradients.py = scripts.legacy.scil_validate_and_correct_eddy_gradients:main
 scil_validate_bids.py = scripts.legacy.scil_validate_bids:main
 scil_verify_space_attributes_compatibility.py = scripts.legacy.scil_verify_space_attributes_compatibility:main
 scil_visualize_bingham_fit.py = scripts.legacy.scil_visualize_bingham_fit:main
 scil_visualize_bundles.py = scripts.legacy.scil_visualize_bundles:main
```

### Comparing `scilpy-2.0.1/scilpy.egg-info/requires.txt` & `scilpy-2.0.2/scilpy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_compare_connectivity.py` & `scilpy-2.0.2/scripts/legacy/scil_compare_connectivity.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_compute_bundle_mean_std_per_point.py` & `scilpy-2.0.2/scripts/legacy/scil_compute_bundle_mean_std_per_point.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_compute_connectivity.py` & `scilpy-2.0.2/scripts/legacy/scil_compute_connectivity.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_convert_gradients_fsl_to_mrtrix.py` & `scilpy-2.0.2/scripts/legacy/scil_convert_gradients_fsl_to_mrtrix.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_convert_gradients_mrtrix_to_fsl.py` & `scilpy-2.0.2/scripts/legacy/scil_convert_gradients_mrtrix_to_fsl.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_evaluate_bundles_binary_classification_measures.py` & `scilpy-2.0.2/scripts/legacy/scil_evaluate_bundles_binary_classification_measures.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_evaluate_connectivity_graph_measures.py` & `scilpy-2.0.2/scripts/legacy/scil_evaluate_connectivity_graph_measures.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_evaluate_connectivity_pairwise_agreement_measures.py` & `scilpy-2.0.2/scripts/legacy/scil_evaluate_connectivity_pairwise_agreement_measures.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_filter_connectivity.py` & `scilpy-2.0.2/scripts/legacy/scil_filter_connectivity.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_generate_priors_from_bundle.py` & `scilpy-2.0.2/scripts/legacy/scil_generate_priors_from_bundle.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_normalize_connectivity.py` & `scilpy-2.0.2/scripts/legacy/scil_normalize_connectivity.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_print_connectivity_filenames.py` & `scilpy-2.0.2/scripts/legacy/scil_print_connectivity_filenames.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_reorder_connectivity.py` & `scilpy-2.0.2/scripts/legacy/scil_reorder_connectivity.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_split_volume_by_ids.py` & `scilpy-2.0.2/scripts/legacy/scil_split_volume_by_ids.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/legacy/scil_split_volume_by_labels.py` & `scilpy-2.0.2/scripts/legacy/scil_split_volume_by_labels.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_NODDI_maps.py` & `scilpy-2.0.2/scripts/scil_NODDI_maps.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_NODDI_priors.py` & `scilpy-2.0.2/scripts/scil_NODDI_priors.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_aodf_metrics.py` & `scilpy-2.0.2/scripts/scil_aodf_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bids_validate.py` & `scilpy-2.0.2/scripts/scil_bids_validate.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bingham_metrics.py` & `scilpy-2.0.2/scripts/scil_bingham_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_btensor_metrics.py` & `scilpy-2.0.2/scripts/scil_btensor_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_clean_qbx_clusters.py` & `scilpy-2.0.2/scripts/scil_bundle_clean_qbx_clusters.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_compute_centroid.py` & `scilpy-2.0.2/scripts/scil_bundle_compute_centroid.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_compute_endpoints_map.py` & `scilpy-2.0.2/scripts/scil_bundle_compute_endpoints_map.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_diameter.py` & `scilpy-2.0.2/scripts/scil_bundle_diameter.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_filter_by_occurence.py` & `scilpy-2.0.2/scripts/scil_bundle_filter_by_occurence.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_generate_priors.py` & `scilpy-2.0.2/scripts/scil_bundle_generate_priors.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_label_map.py` & `scilpy-2.0.2/scripts/scil_bundle_label_map.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_mean_fixel_afd.py` & `scilpy-2.0.2/scripts/scil_bundle_mean_fixel_afd.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_mean_fixel_afd_from_hdf5.py` & `scilpy-2.0.2/scripts/scil_bundle_mean_fixel_afd_from_hdf5.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_mean_fixel_bingham_metric.py` & `scilpy-2.0.2/scripts/scil_bundle_mean_fixel_bingham_metric.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_mean_std.py` & `scilpy-2.0.2/scripts/scil_bundle_mean_std.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_pairwise_comparison.py` & `scilpy-2.0.2/scripts/scil_bundle_pairwise_comparison.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_reject_outliers.py` & `scilpy-2.0.2/scripts/scil_bundle_reject_outliers.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_score_many_bundles_one_tractogram.py` & `scilpy-2.0.2/scripts/scil_bundle_score_many_bundles_one_tractogram.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_score_same_bundle_many_segmentations.py` & `scilpy-2.0.2/scripts/scil_bundle_score_same_bundle_many_segmentations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_shape_measures.py` & `scilpy-2.0.2/scripts/scil_bundle_shape_measures.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_bundle_volume_per_label.py` & `scilpy-2.0.2/scripts/scil_bundle_volume_per_label.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_connectivity_compare_populations.py` & `scilpy-2.0.2/scripts/scil_connectivity_compare_populations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_connectivity_compute_matrices.py` & `scilpy-2.0.2/scripts/scil_connectivity_compute_matrices.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_connectivity_compute_pca.py` & `scilpy-2.0.2/scripts/scil_connectivity_compute_pca.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_connectivity_filter.py` & `scilpy-2.0.2/scripts/scil_connectivity_filter.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_connectivity_graph_measures.py` & `scilpy-2.0.2/scripts/scil_connectivity_graph_measures.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_connectivity_hdf5_average_density_map.py` & `scilpy-2.0.2/scripts/scil_connectivity_hdf5_average_density_map.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_connectivity_math.py` & `scilpy-2.0.2/scripts/scil_connectivity_math.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_connectivity_normalize.py` & `scilpy-2.0.2/scripts/scil_connectivity_normalize.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_connectivity_pairwise_agreement.py` & `scilpy-2.0.2/scripts/scil_connectivity_pairwise_agreement.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_connectivity_print_filenames.py` & `scilpy-2.0.2/scripts/scil_connectivity_print_filenames.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_connectivity_reorder_rois.py` & `scilpy-2.0.2/scripts/scil_connectivity_reorder_rois.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_denoising_nlmeans.py` & `scilpy-2.0.2/scripts/scil_denoising_nlmeans.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dki_metrics.py` & `scilpy-2.0.2/scripts/scil_dki_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dti_convert_tensors.py` & `scilpy-2.0.2/scripts/scil_dti_convert_tensors.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dti_metrics.py` & `scilpy-2.0.2/scripts/scil_dti_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dwi_apply_bias_field.py` & `scilpy-2.0.2/scripts/scil_dwi_apply_bias_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     dwi_img = nib.load(args.in_dwi)
     dwi_data = dwi_img.get_fdata(dtype=np.float32)
 
     bias_field_img = nib.load(args.in_bias_field)
     bias_field_data = bias_field_img.get_fdata(dtype=np.float32)
 
     if args.mask:
-        mask_data = get_data_as_mask(nib.load(args.mask))
+        mask_data = get_data_as_mask(nib.load(args.mask), dtype=bool)
     else:
         mask_data = np.average(dwi_data, axis=-1) != 0
 
     dwi_data = apply_bias_field(dwi_data, bias_field_data, mask_data)
 
     nib.save(nib.Nifti1Image(dwi_data, dwi_img.affine, dwi_img.header),
              args.out_name)
```

### Comparing `scilpy-2.0.1/scripts/scil_dwi_compute_snr.py` & `scilpy-2.0.2/scripts/scil_dwi_compute_snr.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dwi_concatenate.py` & `scilpy-2.0.2/scripts/scil_dwi_concatenate.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dwi_convert_FDF.py` & `scilpy-2.0.2/scripts/scil_dwi_convert_FDF.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dwi_detect_volume_outliers.py` & `scilpy-2.0.2/scripts/scil_dwi_detect_volume_outliers.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dwi_extract_b0.py` & `scilpy-2.0.2/scripts/scil_dwi_extract_b0.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dwi_extract_shell.py` & `scilpy-2.0.2/scripts/scil_dwi_extract_shell.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dwi_powder_average.py` & `scilpy-2.0.2/scripts/scil_dwi_powder_average.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dwi_prepare_eddy_command.py` & `scilpy-2.0.2/scripts/scil_dwi_prepare_eddy_command.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dwi_prepare_topup_command.py` & `scilpy-2.0.2/scripts/scil_dwi_prepare_topup_command.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dwi_reorder_philips.py` & `scilpy-2.0.2/scripts/scil_dwi_reorder_philips.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dwi_split_by_indices.py` & `scilpy-2.0.2/scripts/scil_dwi_split_by_indices.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_dwi_to_sh.py` & `scilpy-2.0.2/scripts/scil_dwi_to_sh.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_fodf_max_in_ventricles.py` & `scilpy-2.0.2/scripts/scil_fodf_max_in_ventricles.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_fodf_memsmt.py` & `scilpy-2.0.2/scripts/scil_fodf_memsmt.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_fodf_metrics.py` & `scilpy-2.0.2/scripts/scil_fodf_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_fodf_msmt.py` & `scilpy-2.0.2/scripts/scil_fodf_msmt.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_fodf_ssst.py` & `scilpy-2.0.2/scripts/scil_fodf_ssst.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_fodf_to_bingham.py` & `scilpy-2.0.2/scripts/scil_fodf_to_bingham.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_freewater_maps.py` & `scilpy-2.0.2/scripts/scil_freewater_maps.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_frf_mean.py` & `scilpy-2.0.2/scripts/scil_frf_mean.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_frf_memsmt.py` & `scilpy-2.0.2/scripts/scil_frf_memsmt.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_frf_msmt.py` & `scilpy-2.0.2/scripts/scil_frf_msmt.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_frf_set_diffusivities.py` & `scilpy-2.0.2/scripts/scil_frf_set_diffusivities.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_frf_ssst.py` & `scilpy-2.0.2/scripts/scil_frf_ssst.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_get_version.py` & `scilpy-2.0.2/scripts/scil_get_version.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_gradients_apply_transform.py` & `scilpy-2.0.2/scripts/scil_gradients_apply_transform.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_gradients_convert.py` & `scilpy-2.0.2/scripts/scil_gradients_convert.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_gradients_generate_sampling.py` & `scilpy-2.0.2/scripts/scil_gradients_generate_sampling.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_gradients_modify_axes.py` & `scilpy-2.0.2/scripts/scil_gradients_modify_axes.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_gradients_round_bvals.py` & `scilpy-2.0.2/scripts/scil_gradients_round_bvals.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_gradients_validate_correct.py` & `scilpy-2.0.2/scripts/scil_gradients_validate_correct.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_gradients_validate_correct_eddy.py` & `scilpy-2.0.2/scripts/scil_gradients_validate_correct_eddy.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_header_print_info.py` & `scilpy-2.0.2/scripts/scil_header_print_info.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_header_validate_compatibility.py` & `scilpy-2.0.2/scripts/scil_header_validate_compatibility.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_json_convert_entries_to_xlsx.py` & `scilpy-2.0.2/scripts/scil_json_convert_entries_to_xlsx.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_json_harmonize_entries.py` & `scilpy-2.0.2/scripts/scil_json_harmonize_entries.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_json_merge_entries.py` & `scilpy-2.0.2/scripts/scil_json_merge_entries.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_labels_combine.py` & `scilpy-2.0.2/scripts/scil_labels_combine.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_labels_dilate.py` & `scilpy-2.0.2/scripts/scil_labels_dilate.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_labels_remove.py` & `scilpy-2.0.2/scripts/scil_labels_remove.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_labels_split_volume_by_ids.py` & `scilpy-2.0.2/scripts/scil_labels_split_volume_by_ids.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_labels_split_volume_from_lut.py` & `scilpy-2.0.2/scripts/scil_labels_split_volume_from_lut.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_lesions_info.py` & `scilpy-2.0.2/scripts/scil_lesions_info.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_mti_adjust_B1_header.py` & `scilpy-2.0.2/scripts/scil_mti_adjust_B1_header.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_mti_maps_MT.py` & `scilpy-2.0.2/scripts/scil_mti_maps_MT.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_mti_maps_ihMT.py` & `scilpy-2.0.2/scripts/scil_mti_maps_ihMT.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_plot_stats_per_point.py` & `scilpy-2.0.2/scripts/scil_plot_stats_per_point.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_qball_metrics.py` & `scilpy-2.0.2/scripts/scil_qball_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_rgb_convert.py` & `scilpy-2.0.2/scripts/scil_rgb_convert.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_search_keywords.py` & `scilpy-2.0.2/scripts/scil_search_keywords.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_sh_convert.py` & `scilpy-2.0.2/scripts/scil_sh_convert.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_sh_fusion.py` & `scilpy-2.0.2/scripts/scil_sh_fusion.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_sh_to_aodf.py` & `scilpy-2.0.2/scripts/scil_sh_to_aodf.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_sh_to_rish.py` & `scilpy-2.0.2/scripts/scil_sh_to_rish.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_sh_to_sf.py` & `scilpy-2.0.2/scripts/scil_sh_to_sf.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_stats_group_comparison.py` & `scilpy-2.0.2/scripts/scil_stats_group_comparison.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_surface_apply_transform.py` & `scilpy-2.0.2/scripts/scil_surface_apply_transform.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_surface_convert.py` & `scilpy-2.0.2/scripts/scil_surface_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         xform_translation = [0, 0, 0]
 
     if not ((os.path.splitext(args.in_surface)[1])
             in ['.vtk', '.vtp', '.fib', '.ply', '.stl', '.xml', '.obj']):
         polydata = convert_freesurfer_into_polydata(args.in_surface,
                                                     xform_translation)
     else:
-        polydata = load_polydata(args.out_surface)
+        polydata = load_polydata(args.in_surface)
 
     if args.to_lps:
         polydata = flip_LPS(polydata)
 
     save_polydata(polydata, args.out_surface, legacy_vtk_format=True)
```

### Comparing `scilpy-2.0.1/scripts/scil_surface_flip.py` & `scilpy-2.0.2/scripts/scil_surface_flip.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_surface_smooth.py` & `scilpy-2.0.2/scripts/scil_surface_smooth.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tracking_local.py` & `scilpy-2.0.2/scripts/scil_tracking_local.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tracking_local_dev.py` & `scilpy-2.0.2/scripts/scil_tracking_local_dev.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tracking_pft.py` & `scilpy-2.0.2/scripts/scil_tracking_pft.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tracking_pft_maps.py` & `scilpy-2.0.2/scripts/scil_tracking_pft_maps.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tracking_pft_maps_edit.py` & `scilpy-2.0.2/scripts/scil_tracking_pft_maps_edit.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_apply_transform.py` & `scilpy-2.0.2/scripts/scil_tractogram_apply_transform.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_apply_transform_to_hdf5.py` & `scilpy-2.0.2/scripts/scil_tractogram_apply_transform_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_assign_custom_color.py` & `scilpy-2.0.2/scripts/scil_tractogram_assign_custom_color.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_assign_uniform_color.py` & `scilpy-2.0.2/scripts/scil_tractogram_assign_uniform_color.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_commit.py` & `scilpy-2.0.2/scripts/scil_tractogram_commit.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_compress.py` & `scilpy-2.0.2/scripts/scil_tractogram_compress.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_compute_TODI.py` & `scilpy-2.0.2/scripts/scil_tractogram_compute_TODI.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_compute_density_map.py` & `scilpy-2.0.2/scripts/scil_tractogram_compute_density_map.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_convert.py` & `scilpy-2.0.2/scripts/scil_tractogram_convert.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_convert_hdf5_to_trk.py` & `scilpy-2.0.2/scripts/scil_tractogram_convert_hdf5_to_trk.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_count_streamlines.py` & `scilpy-2.0.2/scripts/scil_tractogram_count_streamlines.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_cut_streamlines.py` & `scilpy-2.0.2/scripts/scil_tractogram_cut_streamlines.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_detect_loops.py` & `scilpy-2.0.2/scripts/scil_tractogram_detect_loops.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_dpp_math.py` & `scilpy-2.0.2/scripts/scil_tractogram_dpp_math.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_extract_ushape.py` & `scilpy-2.0.2/scripts/scil_tractogram_extract_ushape.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_filter_by_anatomy.py` & `scilpy-2.0.2/scripts/scil_tractogram_filter_by_anatomy.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_filter_by_length.py` & `scilpy-2.0.2/scripts/scil_tractogram_filter_by_length.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_filter_by_orientation.py` & `scilpy-2.0.2/scripts/scil_tractogram_filter_by_orientation.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_filter_by_roi.py` & `scilpy-2.0.2/scripts/scil_tractogram_filter_by_roi.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_fix_trk.py` & `scilpy-2.0.2/scripts/scil_tractogram_fix_trk.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_flip.py` & `scilpy-2.0.2/scripts/scil_tractogram_flip.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_math.py` & `scilpy-2.0.2/scripts/scil_tractogram_math.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_pairwise_comparison.py` & `scilpy-2.0.2/scripts/scil_tractogram_pairwise_comparison.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_print_info.py` & `scilpy-2.0.2/scripts/scil_tractogram_print_info.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_project_map_to_streamlines.py` & `scilpy-2.0.2/scripts/scil_tractogram_project_map_to_streamlines.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_project_streamlines_to_map.py` & `scilpy-2.0.2/scripts/scil_tractogram_project_streamlines_to_map.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_qbx.py` & `scilpy-2.0.2/scripts/scil_tractogram_qbx.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_register.py` & `scilpy-2.0.2/scripts/scil_tractogram_register.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_remove_invalid.py` & `scilpy-2.0.2/scripts/scil_tractogram_remove_invalid.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_resample.py` & `scilpy-2.0.2/scripts/scil_tractogram_resample.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_resample_nb_points.py` & `scilpy-2.0.2/scripts/scil_tractogram_resample_nb_points.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_seed_density_map.py` & `scilpy-2.0.2/scripts/scil_tractogram_seed_density_map.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_segment_and_score.py` & `scilpy-2.0.2/scripts/scil_tractogram_segment_and_score.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_segment_bundles.py` & `scilpy-2.0.2/scripts/scil_tractogram_segment_bundles.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_segment_bundles_for_connectivity.py` & `scilpy-2.0.2/scripts/scil_tractogram_segment_bundles_for_connectivity.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_segment_one_bundle.py` & `scilpy-2.0.2/scripts/scil_tractogram_segment_one_bundle.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_shuffle.py` & `scilpy-2.0.2/scripts/scil_tractogram_shuffle.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_smooth.py` & `scilpy-2.0.2/scripts/scil_tractogram_smooth.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_split.py` & `scilpy-2.0.2/scripts/scil_tractogram_split.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_tractogram_uniformize_endpoints.py` & `scilpy-2.0.2/scripts/scil_bundle_uniformize_endpoints.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_bingham_fit.py` & `scilpy-2.0.2/scripts/scil_viz_bingham_fit.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_bundle.py` & `scilpy-2.0.2/scripts/scil_viz_bundle.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_bundle_screenshot_mni.py` & `scilpy-2.0.2/scripts/scil_viz_bundle_screenshot_mni.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_bundle_screenshot_mosaic.py` & `scilpy-2.0.2/scripts/scil_viz_bundle_screenshot_mosaic.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_connectivity.py` & `scilpy-2.0.2/scripts/scil_viz_connectivity.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_dti_screenshot.py` & `scilpy-2.0.2/scripts/scil_viz_dti_screenshot.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_fodf.py` & `scilpy-2.0.2/scripts/scil_viz_fodf.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_gradients_screenshot.py` & `scilpy-2.0.2/scripts/scil_viz_gradients_screenshot.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_tractogram_seeds.py` & `scilpy-2.0.2/scripts/scil_viz_tractogram_seeds.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_tractogram_seeds_3d.py` & `scilpy-2.0.2/scripts/scil_viz_tractogram_seeds_3d.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_volume_histogram.py` & `scilpy-2.0.2/scripts/scil_viz_volume_histogram.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_volume_scatterplot.py` & `scilpy-2.0.2/scripts/scil_viz_volume_scatterplot.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_volume_screenshot.py` & `scilpy-2.0.2/scripts/scil_viz_volume_screenshot.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_viz_volume_screenshot_mosaic.py` & `scilpy-2.0.2/scripts/scil_viz_volume_screenshot_mosaic.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_volume_apply_transform.py` & `scilpy-2.0.2/scripts/scil_volume_apply_transform.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_volume_b0_synthesis.py` & `scilpy-2.0.2/scripts/scil_volume_b0_synthesis.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_volume_count_non_zero_voxels.py` & `scilpy-2.0.2/scripts/scil_volume_count_non_zero_voxels.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_volume_crop.py` & `scilpy-2.0.2/scripts/scil_volume_crop.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_volume_flip.py` & `scilpy-2.0.2/scripts/scil_volume_flip.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_volume_math.py` & `scilpy-2.0.2/scripts/scil_volume_math.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_volume_remove_outliers_ransac.py` & `scilpy-2.0.2/scripts/scil_volume_remove_outliers_ransac.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_volume_resample.py` & `scilpy-2.0.2/scripts/scil_volume_resample.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_volume_reshape_to_reference.py` & `scilpy-2.0.2/scripts/scil_volume_reshape_to_reference.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_volume_stats_in_ROI.py` & `scilpy-2.0.2/scripts/scil_volume_stats_in_ROI.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/scil_volume_stats_in_labels.py` & `scilpy-2.0.2/scripts/scil_volume_stats_in_labels.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_NODDI_maps.py` & `scilpy-2.0.2/scripts/tests/test_NODDI_maps.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_NODDI_priors.py` & `scilpy-2.0.2/scripts/tests/test_NODDI_priors.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_aodf_metrics.py` & `scilpy-2.0.2/scripts/tests/test_aodf_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bids_validate.py` & `scilpy-2.0.2/scripts/tests/test_bids_validate.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bingham_metrics.py` & `scilpy-2.0.2/scripts/tests/test_bingham_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_btensor_metrics.py` & `scilpy-2.0.2/scripts/tests/test_btensor_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_compute_centroid.py` & `scilpy-2.0.2/scripts/tests/test_bundle_compute_centroid.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_compute_endpoints_map.py` & `scilpy-2.0.2/scripts/tests/test_bundle_compute_endpoints_map.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_diameter.py` & `scilpy-2.0.2/scripts/tests/test_bundle_diameter.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_filter_by_occurence.py` & `scilpy-2.0.2/scripts/tests/test_bundle_filter_by_occurence.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_generate_priors.py` & `scilpy-2.0.2/scripts/tests/test_bundle_generate_priors.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_label_map.py` & `scilpy-2.0.2/scripts/tests/test_bundle_label_map.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_mean_fixel_afd.py` & `scilpy-2.0.2/scripts/tests/test_bundle_mean_fixel_afd.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_mean_fixel_afd_from_hdf5.py` & `scilpy-2.0.2/scripts/tests/test_bundle_mean_fixel_afd_from_hdf5.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_mean_fixel_bingham_metric.py` & `scilpy-2.0.2/scripts/tests/test_bundle_mean_fixel_bingham_metric.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_mean_std.py` & `scilpy-2.0.2/scripts/tests/test_bundle_mean_std.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_pairwise_comparison.py` & `scilpy-2.0.2/scripts/tests/test_bundle_pairwise_comparison.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_reject_outliers.py` & `scilpy-2.0.2/scripts/tests/test_bundle_reject_outliers.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_score_many_bundles_one_tractogram.py` & `scilpy-2.0.2/scripts/tests/test_bundle_score_many_bundles_one_tractogram.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_score_same_bundle_many_segmentations.py` & `scilpy-2.0.2/scripts/tests/test_bundle_score_same_bundle_many_segmentations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_shape_measures.py` & `scilpy-2.0.2/scripts/tests/test_bundle_shape_measures.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_bundle_volume_per_label.py` & `scilpy-2.0.2/scripts/tests/test_bundle_volume_per_label.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_connectivity_compare_populations.py` & `scilpy-2.0.2/scripts/tests/test_connectivity_compare_populations.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_connectivity_compute_matrices.py` & `scilpy-2.0.2/scripts/tests/test_connectivity_compute_matrices.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_connectivity_compute_pca.py` & `scilpy-2.0.2/scripts/tests/test_connectivity_compute_pca.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_connectivity_filter.py` & `scilpy-2.0.2/scripts/tests/test_connectivity_filter.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_connectivity_graph_measures.py` & `scilpy-2.0.2/scripts/tests/test_connectivity_graph_measures.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_connectivity_hdf5_average_density_map.py` & `scilpy-2.0.2/scripts/tests/test_connectivity_hdf5_average_density_map.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_connectivity_math.py` & `scilpy-2.0.2/scripts/tests/test_connectivity_math.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_connectivity_normalize.py` & `scilpy-2.0.2/scripts/tests/test_connectivity_normalize.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_connectivity_pairwise_agreement.py` & `scilpy-2.0.2/scripts/tests/test_connectivity_pairwise_agreement.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_connectivity_print_filenames.py` & `scilpy-2.0.2/scripts/tests/test_connectivity_print_filenames.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_connectivity_reorder_rois.py` & `scilpy-2.0.2/scripts/tests/test_connectivity_reorder_rois.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_denoising_nlmeans.py` & `scilpy-2.0.2/scripts/tests/test_denoising_nlmeans.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_dki_metrics.py` & `scilpy-2.0.2/scripts/tests/test_dki_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_dti_convert_tensors.py` & `scilpy-2.0.2/scripts/tests/test_dti_convert_tensors.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_dti_metrics.py` & `scilpy-2.0.2/scripts/tests/test_dti_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_dwi_apply_bias_field.py` & `scilpy-2.0.2/scripts/tests/test_dwi_apply_bias_field.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_dwi_compute_snr.py` & `scilpy-2.0.2/scripts/tests/test_dwi_compute_snr.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_dwi_concatenate.py` & `scilpy-2.0.2/scripts/tests/test_dwi_concatenate.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_dwi_detect_volume_outliers.py` & `scilpy-2.0.2/scripts/tests/test_dwi_detect_volume_outliers.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_dwi_extract_b0.py` & `scilpy-2.0.2/scripts/tests/test_dwi_extract_b0.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_dwi_extract_shell.py` & `scilpy-2.0.2/scripts/tests/test_dwi_extract_shell.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_dwi_powder_average.py` & `scilpy-2.0.2/scripts/tests/test_dwi_powder_average.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_dwi_reorder_philips.py` & `scilpy-2.0.2/scripts/tests/test_dwi_reorder_philips.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_dwi_split_by_indices.py` & `scilpy-2.0.2/scripts/tests/test_dwi_split_by_indices.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_dwi_to_sh.py` & `scilpy-2.0.2/scripts/tests/test_dwi_to_sh.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_fodf_max_in_ventricles.py` & `scilpy-2.0.2/scripts/tests/test_fodf_max_in_ventricles.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_fodf_memsmt.py` & `scilpy-2.0.2/scripts/tests/test_fodf_memsmt.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_fodf_metrics.py` & `scilpy-2.0.2/scripts/tests/test_fodf_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_fodf_msmt.py` & `scilpy-2.0.2/scripts/tests/test_fodf_msmt.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_fodf_ssst.py` & `scilpy-2.0.2/scripts/tests/test_fodf_ssst.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_fodf_to_bingham.py` & `scilpy-2.0.2/scripts/tests/test_fodf_to_bingham.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_freewater_maps.py` & `scilpy-2.0.2/scripts/tests/test_freewater_maps.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_frf_mean.py` & `scilpy-2.0.2/scripts/tests/test_frf_mean.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_frf_memsmt.py` & `scilpy-2.0.2/scripts/tests/test_frf_memsmt.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_frf_msmt.py` & `scilpy-2.0.2/scripts/tests/test_frf_msmt.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_frf_set_diffusivities.py` & `scilpy-2.0.2/scripts/tests/test_frf_set_diffusivities.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_frf_ssst.py` & `scilpy-2.0.2/scripts/tests/test_frf_ssst.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_gradients_apply_transform.py` & `scilpy-2.0.2/scripts/tests/test_gradients_apply_transform.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_gradients_convert.py` & `scilpy-2.0.2/scripts/tests/test_gradients_convert.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_gradients_generate_sampling.py` & `scilpy-2.0.2/scripts/tests/test_gradients_generate_sampling.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_gradients_modify_axes.py` & `scilpy-2.0.2/scripts/tests/test_gradients_modify_axes.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_gradients_round_bvals.py` & `scilpy-2.0.2/scripts/tests/test_gradients_round_bvals.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_gradients_validate_correct.py` & `scilpy-2.0.2/scripts/tests/test_gradients_validate_correct.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_gradients_validate_correct_eddy.py` & `scilpy-2.0.2/scripts/tests/test_gradients_validate_correct_eddy.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_header_print_info.py` & `scilpy-2.0.2/scripts/tests/test_header_print_info.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_header_validate_compatibility.py` & `scilpy-2.0.2/scripts/tests/test_header_validate_compatibility.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_json_convert_entries_to_xlsx.py` & `scilpy-2.0.2/scripts/tests/test_json_convert_entries_to_xlsx.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_json_merge_entries.py` & `scilpy-2.0.2/scripts/tests/test_json_merge_entries.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_labels_combine.py` & `scilpy-2.0.2/scripts/tests/test_labels_combine.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_labels_dilate.py` & `scilpy-2.0.2/scripts/tests/test_labels_dilate.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_labels_remove.py` & `scilpy-2.0.2/scripts/tests/test_labels_remove.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_labels_split_volume_by_ids.py` & `scilpy-2.0.2/scripts/tests/test_labels_split_volume_by_ids.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_labels_split_volume_from_lut.py` & `scilpy-2.0.2/scripts/tests/test_labels_split_volume_from_lut.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_mti_adjust_B1_header.py` & `scilpy-2.0.2/scripts/tests/test_mti_adjust_B1_header.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_mti_maps_MT.py` & `scilpy-2.0.2/scripts/tests/test_mti_maps_MT.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_mti_maps_ihMT.py` & `scilpy-2.0.2/scripts/tests/test_mti_maps_ihMT.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_plot_stats_per_point.py` & `scilpy-2.0.2/scripts/tests/test_plot_stats_per_point.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_qball_metrics.py` & `scilpy-2.0.2/scripts/tests/test_qball_metrics.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_rgb_convert.py` & `scilpy-2.0.2/scripts/tests/test_rgb_convert.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_search_keywords.py` & `scilpy-2.0.2/scripts/tests/test_search_keywords.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_sh_convert.py` & `scilpy-2.0.2/scripts/tests/test_sh_convert.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_sh_fusion.py` & `scilpy-2.0.2/scripts/tests/test_sh_fusion.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_sh_to_aodf.py` & `scilpy-2.0.2/scripts/tests/test_sh_to_aodf.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_sh_to_rish.py` & `scilpy-2.0.2/scripts/tests/test_sh_to_rish.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_sh_to_sf.py` & `scilpy-2.0.2/scripts/tests/test_sh_to_sf.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_stats_group_comparison.py` & `scilpy-2.0.2/scripts/tests/test_stats_group_comparison.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_surface_apply_transform.py` & `scilpy-2.0.2/scripts/tests/test_surface_apply_transform.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_surface_convert.py` & `scilpy-2.0.2/scripts/tests/test_surface_convert.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_surface_flip.py` & `scilpy-2.0.2/scripts/tests/test_surface_flip.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_surface_smooth.py` & `scilpy-2.0.2/scripts/tests/test_surface_smooth.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tracking_local.py` & `scilpy-2.0.2/scripts/tests/test_tracking_local.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tracking_local_dev.py` & `scilpy-2.0.2/scripts/tests/test_tracking_local_dev.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tracking_pft.py` & `scilpy-2.0.2/scripts/tests/test_tracking_pft.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tracking_pft_maps.py` & `scilpy-2.0.2/scripts/tests/test_tracking_pft_maps.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tracking_pft_maps_edit.py` & `scilpy-2.0.2/scripts/tests/test_tracking_pft_maps_edit.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_apply_transform.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_apply_transform.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_apply_transform_to_hdf5.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_apply_transform_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_assign_custom_color.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_assign_custom_color.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_assign_uniform_color.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_assign_uniform_color.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_commit.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_commit.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_compress.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_compress.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_compute_TODI.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_compute_TODI.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_compute_density_map.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_compute_density_map.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_convert.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_convert.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_convert_hdf5_to_trk.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_convert_hdf5_to_trk.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_count_streamlines.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_count_streamlines.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_cut_streamlines.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_cut_streamlines.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_detect_loops.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_detect_loops.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_dpp_math.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_dpp_math.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_extract_ushape.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_extract_ushape.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_filter_by_anatomy.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_filter_by_anatomy.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_filter_by_length.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_filter_by_length.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_filter_by_orientation.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_filter_by_orientation.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_filter_by_roi.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_filter_by_roi.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_flip.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_flip.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_math.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_math.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_pairwise_comparison.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_pairwise_comparison.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_print_info.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_print_info.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_project_map_to_streamlines.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_project_map_to_streamlines.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_project_streamlines_to_map.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_project_streamlines_to_map.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_qbx.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_qbx.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_register.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_register.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_remove_invalid.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_remove_invalid.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_resample.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_resample.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_resample_nb_points.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_resample_nb_points.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_seed_density_map.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_seed_density_map.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_segment_and_score.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_segment_and_score.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_segment_bundles.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_segment_bundles.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_segment_bundles_for_connectivity.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_segment_bundles_for_connectivity.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_segment_one_bundles.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_segment_one_bundles.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_shuffle.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_shuffle.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_smooth.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_smooth.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_split.py` & `scilpy-2.0.2/scripts/tests/test_tractogram_split.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_tractogram_uniformize_endpoints.py` & `scilpy-2.0.2/scripts/tests/test_bundle_uniformize_endpoints.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 # If they already exist, this only takes 5 seconds (check md5sum)
 fetch_data(get_testing_files_dict(), keys=['tractometry.zip'])
 tmp_dir = tempfile.TemporaryDirectory()
 
 
 def test_help_option(script_runner):
-    ret = script_runner.run('scil_tractogram_uniformize_endpoints.py',
+    ret = script_runner.run('scil_bundle_uniformize_endpoints.py',
                             '--help')
     assert ret.success
 
 
 def test_execution_auto(script_runner, monkeypatch):
     monkeypatch.chdir(os.path.expanduser(tmp_dir.name))
     in_bundle = os.path.join(SCILPY_HOME, 'tractometry', 'IFGWM.trk')
-    ret = script_runner.run('scil_tractogram_uniformize_endpoints.py',
+    ret = script_runner.run('scil_bundle_uniformize_endpoints.py',
                             in_bundle, 'IFGWM_uni.trk', '--auto')
     assert ret.success
 
 
 def test_execution_target_atlas(script_runner, monkeypatch):
     monkeypatch.chdir(os.path.expanduser(tmp_dir.name))
     in_bundle = os.path.join(SCILPY_HOME, 'tractometry', 'IFGWM.trk')
     label = os.path.join(SCILPY_HOME, 'tractometry', 'IFGWM_labels_map.nii.gz')
-    ret = script_runner.run('scil_tractogram_uniformize_endpoints.py',
+    ret = script_runner.run('scil_bundle_uniformize_endpoints.py',
                             in_bundle, 'IFGWM_uni2.trk', '--target_roi', label,
                             '3', '10')
     assert ret.success
```

### Comparing `scilpy-2.0.1/scripts/tests/test_viz_bingham_fit.py` & `scilpy-2.0.2/scripts/tests/test_viz_bingham_fit.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_viz_bundle.py` & `scilpy-2.0.2/scripts/tests/test_viz_bundle.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_viz_connectivity.py` & `scilpy-2.0.2/scripts/tests/test_viz_connectivity.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_viz_fodf.py` & `scilpy-2.0.2/scripts/tests/test_viz_fodf.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_viz_volume_histogram.py` & `scilpy-2.0.2/scripts/tests/test_viz_volume_histogram.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_viz_volume_scatterplot.py` & `scilpy-2.0.2/scripts/tests/test_viz_volume_scatterplot.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_viz_volume_screenshot.py` & `scilpy-2.0.2/scripts/tests/test_viz_volume_screenshot.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_volume_apply_transform.py` & `scilpy-2.0.2/scripts/tests/test_volume_apply_transform.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_volume_b0_synthesis.py` & `scilpy-2.0.2/scripts/tests/test_volume_b0_synthesis.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_volume_count_non_zero_voxels.py` & `scilpy-2.0.2/scripts/tests/test_volume_count_non_zero_voxels.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_volume_crop.py` & `scilpy-2.0.2/scripts/tests/test_volume_crop.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_volume_flip.py` & `scilpy-2.0.2/scripts/tests/test_volume_flip.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_volume_math.py` & `scilpy-2.0.2/scripts/tests/test_volume_math.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_volume_remove_outliers_ransac.py` & `scilpy-2.0.2/scripts/tests/test_volume_remove_outliers_ransac.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_volume_resample.py` & `scilpy-2.0.2/scripts/tests/test_volume_resample.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_volume_reshape_to_reference.py` & `scilpy-2.0.2/scripts/tests/test_volume_reshape_to_reference.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_volume_stats_in_ROI.py` & `scilpy-2.0.2/scripts/tests/test_volume_stats_in_ROI.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/scripts/tests/test_volume_stats_in_labels.py` & `scilpy-2.0.2/scripts/tests/test_volume_stats_in_labels.py`

 * *Files identical despite different names*

### Comparing `scilpy-2.0.1/setup.py` & `scilpy-2.0.2/setup.py`

 * *Files identical despite different names*

