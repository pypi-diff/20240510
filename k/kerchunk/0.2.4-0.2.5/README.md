# Comparing `tmp/kerchunk-0.2.4.tar.gz` & `tmp/kerchunk-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerchunk-0.2.4.tar", last modified: Tue Mar  5 14:16:51 2024, max compression
+gzip compressed data, was "kerchunk-0.2.5.tar", last modified: Fri May 10 20:08:56 2024, max compression
```

## Comparing `kerchunk-0.2.4.tar` & `kerchunk-0.2.5.tar`

### file list

```diff
@@ -1,98 +1,75 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-05 14:16:51.128221 kerchunk-0.2.4/
--rw-r--r--   0 mdurant    (502) staff       (20)      219 2022-10-31 16:19:59.000000 kerchunk-0.2.4/.coveragerc
--rw-r--r--   0 mdurant    (502) staff       (20)       34 2022-09-18 01:28:32.000000 kerchunk-0.2.4/.gitattributes
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-05 14:16:51.072878 kerchunk-0.2.4/.github/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-05 14:16:51.078813 kerchunk-0.2.4/.github/workflows/
--rw-r--r--   0 mdurant    (502) staff       (20)     1040 2023-12-14 16:32:14.000000 kerchunk-0.2.4/.github/workflows/default.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      320 2023-10-21 00:47:02.000000 kerchunk-0.2.4/.github/workflows/pre-commit.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      334 2023-12-14 16:32:14.000000 kerchunk-0.2.4/.github/workflows/pull_request.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      657 2024-02-05 15:54:00.000000 kerchunk-0.2.4/.github/workflows/tests.yml
--rw-r--r--   0 mdurant    (502) staff       (20)     1768 2023-05-12 18:30:53.000000 kerchunk-0.2.4/.gitignore
--rw-r--r--   0 mdurant    (502) staff       (20)      416 2022-09-18 01:28:32.000000 kerchunk-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0 mdurant    (502) staff       (20)     1063 2022-09-18 01:28:32.000000 kerchunk-0.2.4/LICENSE
--rw-r--r--   0 mdurant    (502) staff       (20)       91 2023-10-21 00:47:02.000000 kerchunk-0.2.4/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     4251 2024-03-05 14:16:51.127835 kerchunk-0.2.4/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     2433 2022-09-23 18:01:10.000000 kerchunk-0.2.4/README.md
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-05 14:16:51.079257 kerchunk-0.2.4/binder/
--rw-r--r--   0 mdurant    (502) staff       (20)      193 2022-09-18 01:28:32.000000 kerchunk-0.2.4/binder/environment.yml
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-05 14:16:51.086248 kerchunk-0.2.4/ci/
--rw-r--r--   0 mdurant    (502) staff       (20)      439 2023-12-14 16:32:20.000000 kerchunk-0.2.4/ci/environment-docs.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      466 2024-02-05 15:54:00.000000 kerchunk-0.2.4/ci/environment-py310.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      463 2024-02-05 15:54:00.000000 kerchunk-0.2.4/ci/environment-py311.yml
--rw-r--r--   0 mdurant    (502) staff       (20)      462 2024-02-05 15:54:00.000000 kerchunk-0.2.4/ci/environment-py39.yml
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-05 14:16:51.087291 kerchunk-0.2.4/docs/
--rw-r--r--   0 mdurant    (502) staff       (20)      661 2022-09-18 01:28:32.000000 kerchunk-0.2.4/docs/Makefile
--rw-r--r--   0 mdurant    (502) staff       (20)      209 2022-09-18 01:28:32.000000 kerchunk-0.2.4/docs/README.md
--rw-r--r--   0 mdurant    (502) staff       (20)      795 2022-09-18 01:28:32.000000 kerchunk-0.2.4/docs/make.bat
--rw-r--r--   0 mdurant    (502) staff       (20)      118 2023-12-14 16:32:14.000000 kerchunk-0.2.4/docs/requirements.txt
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-05 14:16:51.095528 kerchunk-0.2.4/docs/source/
--rw-r--r--   0 mdurant    (502) staff       (20)     7845 2024-02-05 15:54:00.000000 kerchunk-0.2.4/docs/source/advanced.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     1118 2023-08-31 17:50:54.000000 kerchunk-0.2.4/docs/source/beyond.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     2681 2023-08-31 17:50:54.000000 kerchunk-0.2.4/docs/source/cases.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     1996 2022-12-09 18:27:45.000000 kerchunk-0.2.4/docs/source/conf.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7553 2023-08-31 17:50:54.000000 kerchunk-0.2.4/docs/source/contributing.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     3973 2023-08-31 17:50:54.000000 kerchunk-0.2.4/docs/source/detail.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-05 14:16:51.098395 kerchunk-0.2.4/docs/source/images/
--rw-r--r--   0 mdurant    (502) staff       (20)   394242 2022-09-18 01:28:32.000000 kerchunk-0.2.4/docs/source/images/binary_buffer.png
--rw-r--r--   0 mdurant    (502) staff       (20)   126383 2022-09-18 01:28:32.000000 kerchunk-0.2.4/docs/source/images/multi_refs.png
--rw-r--r--   0 mdurant    (502) staff       (20)     3704 2023-08-31 17:50:54.000000 kerchunk-0.2.4/docs/source/index.rst
--rw-r--r--   0 mdurant    (502) staff       (20)    15075 2022-09-18 01:28:32.000000 kerchunk-0.2.4/docs/source/kerchunk.png
--rw-r--r--   0 mdurant    (502) staff       (20)     3003 2023-08-31 17:50:54.000000 kerchunk-0.2.4/docs/source/nonzarr.rst
--rw-r--r--   0 mdurant    (502) staff       (20)    65655 2022-10-31 16:19:59.000000 kerchunk-0.2.4/docs/source/output_62_2.png
--rw-r--r--   0 mdurant    (502) staff       (20)    28361 2022-10-31 16:19:59.000000 kerchunk-0.2.4/docs/source/output_63_2.png
--rw-r--r--   0 mdurant    (502) staff       (20)     2433 2024-01-29 19:49:20.000000 kerchunk-0.2.4/docs/source/reference.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     7704 2024-02-16 19:53:29.000000 kerchunk-0.2.4/docs/source/spec.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     4092 2023-08-31 17:50:54.000000 kerchunk-0.2.4/docs/source/test_example.rst
--rw-r--r--   0 mdurant    (502) staff       (20)    25323 2024-02-16 19:53:29.000000 kerchunk-0.2.4/docs/source/tutorial.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-05 14:16:51.103986 kerchunk-0.2.4/kerchunk/
--rw-r--r--   0 mdurant    (502) staff       (20)      756 2024-01-29 19:49:20.000000 kerchunk-0.2.4/kerchunk/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7000 2023-10-21 00:47:02.000000 kerchunk-0.2.4/kerchunk/codecs.py
--rw-r--r--   0 mdurant    (502) staff       (20)    33189 2024-02-05 15:54:00.000000 kerchunk-0.2.4/kerchunk/combine.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4628 2023-11-17 17:47:22.000000 kerchunk-0.2.4/kerchunk/df.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9397 2023-11-09 18:05:32.000000 kerchunk-0.2.4/kerchunk/fits.py
--rw-r--r--   0 mdurant    (502) staff       (20)    21477 2024-02-16 19:53:29.000000 kerchunk-0.2.4/kerchunk/grib2.py
--rw-r--r--   0 mdurant    (502) staff       (20)    25559 2024-02-29 21:00:13.000000 kerchunk-0.2.4/kerchunk/hdf.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2483 2023-11-07 18:51:08.000000 kerchunk-0.2.4/kerchunk/mzML.py
--rw-r--r--   0 mdurant    (502) staff       (20)    11482 2023-11-09 18:05:32.000000 kerchunk-0.2.4/kerchunk/netCDF3.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-05 14:16:51.125379 kerchunk-0.2.4/kerchunk/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)    96479 2022-09-18 01:28:32.000000 kerchunk-0.2.4/kerchunk/tests/CMC_reg_DEPR_ISBL_10_ps10km_2022072000_P000.grib2
--rw-r--r--   0 mdurant    (502) staff       (20)  2999392 2023-08-15 13:44:50.000000 kerchunk-0.2.4/kerchunk/tests/NEONDSTowerTemperatureData.hdf5
--rw-r--r--   0 mdurant    (502) staff       (20)       30 2022-10-31 16:19:59.000000 kerchunk-0.2.4/kerchunk/tests/conftest.py
--rw-r--r--   0 mdurant    (502) staff       (20)      469 2023-08-31 17:50:56.000000 kerchunk-0.2.4/kerchunk/tests/gen_hdf5.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3591 2023-08-31 17:50:56.000000 kerchunk-0.2.4/kerchunk/tests/hdf5_compression_bitshuffle.h5
--rw-r--r--   0 mdurant    (502) staff       (20)     3931 2023-08-31 17:50:56.000000 kerchunk-0.2.4/kerchunk/tests/hdf5_compression_blosc_lz4_bitshuffle.h5
--rw-r--r--   0 mdurant    (502) staff       (20)     3917 2023-08-31 17:50:56.000000 kerchunk-0.2.4/kerchunk/tests/hdf5_compression_lz4.h5
--rw-r--r--   0 mdurant    (502) staff       (20)     3643 2023-08-31 17:50:56.000000 kerchunk-0.2.4/kerchunk/tests/hdf5_compression_zstd.h5
--rw-r--r--   0 mdurant    (502) staff       (20)    80896 2023-12-07 16:17:36.000000 kerchunk-0.2.4/kerchunk/tests/hrrr.wrfsfcf.subset.json
--rw-r--r--   0 mdurant    (502) staff       (20)   714485 2023-10-21 00:47:02.000000 kerchunk-0.2.4/kerchunk/tests/hrrr.wrfsubhf.sample.grib2
--rw-r--r--   0 mdurant    (502) staff       (20)    66248 2023-12-07 16:17:36.000000 kerchunk-0.2.4/kerchunk/tests/hrrr.wrfsubhf.subset.json
--rw-r--r--   0 mdurant    (502) staff       (20)   370414 2022-09-18 01:28:32.000000 kerchunk-0.2.4/kerchunk/tests/lcmap_tiny_cog_2019.tif
--rw-r--r--   0 mdurant    (502) staff       (20)   364458 2022-09-18 01:28:32.000000 kerchunk-0.2.4/kerchunk/tests/lcmap_tiny_cog_2020.tif
--rw-r--r--   0 mdurant    (502) staff       (20)    24244 2024-02-05 15:54:00.000000 kerchunk-0.2.4/kerchunk/tests/test_combine.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4026 2023-05-31 01:26:55.000000 kerchunk-0.2.4/kerchunk/tests/test_combine_concat.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1307 2023-05-12 18:30:53.000000 kerchunk-0.2.4/kerchunk/tests/test_combine_dask.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1975 2023-05-31 01:26:55.000000 kerchunk-0.2.4/kerchunk/tests/test_df.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2570 2022-10-31 16:19:59.000000 kerchunk-0.2.4/kerchunk/tests/test_fits.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9669 2023-12-07 16:17:36.000000 kerchunk-0.2.4/kerchunk/tests/test_grib.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10400 2023-08-31 17:50:56.000000 kerchunk-0.2.4/kerchunk/tests/test_hdf.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4126 2023-10-21 00:47:02.000000 kerchunk-0.2.4/kerchunk/tests/test_netcdf.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1072 2022-10-31 17:15:23.000000 kerchunk-0.2.4/kerchunk/tests/test_tiff.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5187 2023-08-31 17:50:54.000000 kerchunk-0.2.4/kerchunk/tests/test_utils.py
--rw-r--r--   0 mdurant    (502) staff       (20)      634 2023-10-21 00:47:02.000000 kerchunk-0.2.4/kerchunk/tests/test_xarray_backend.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2416 2024-01-29 19:49:20.000000 kerchunk-0.2.4/kerchunk/tests/test_zarr.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7744 2022-09-18 01:28:32.000000 kerchunk-0.2.4/kerchunk/tests/vlen.h5
--rw-r--r--   0 mdurant    (502) staff       (20)     8544 2022-09-18 01:28:32.000000 kerchunk-0.2.4/kerchunk/tests/vlen2.h5
--rw-r--r--   0 mdurant    (502) staff       (20)     3589 2023-03-13 14:06:07.000000 kerchunk-0.2.4/kerchunk/tiff.py
--rw-r--r--   0 mdurant    (502) staff       (20)    13850 2023-12-14 16:32:14.000000 kerchunk-0.2.4/kerchunk/utils.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1382 2024-02-05 15:54:00.000000 kerchunk-0.2.4/kerchunk/xarray_backend.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1642 2023-12-14 16:32:14.000000 kerchunk-0.2.4/kerchunk/zarr.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-03-05 14:16:51.126051 kerchunk-0.2.4/kerchunk.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     4251 2024-03-05 14:16:50.000000 kerchunk-0.2.4/kerchunk.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     2280 2024-03-05 14:16:51.000000 kerchunk-0.2.4/kerchunk.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-03-05 14:16:50.000000 kerchunk-0.2.4/kerchunk.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      314 2024-03-05 14:16:50.000000 kerchunk-0.2.4/kerchunk.egg-info/entry_points.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      231 2024-03-05 14:16:50.000000 kerchunk-0.2.4/kerchunk.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        9 2024-03-05 14:16:50.000000 kerchunk-0.2.4/kerchunk.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)    15075 2022-09-18 01:28:32.000000 kerchunk-0.2.4/kerchunk.png
--rw-r--r--   0 mdurant    (502) staff       (20)     1833 2024-02-29 21:00:13.000000 kerchunk-0.2.4/pyproject.toml
--rw-r--r--   0 mdurant    (502) staff       (20)      476 2024-03-05 14:16:51.128658 kerchunk-0.2.4/setup.cfg
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-10 20:08:56.339878 kerchunk-0.2.5/
+-rw-r--r--   0 mdurant    (502) staff       (20)      219 2022-10-31 16:19:59.000000 kerchunk-0.2.5/.coveragerc
+-rw-r--r--   0 mdurant    (502) staff       (20)       34 2022-09-18 01:28:32.000000 kerchunk-0.2.5/.gitattributes
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-10 20:08:56.313714 kerchunk-0.2.5/.github/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-10 20:08:56.319366 kerchunk-0.2.5/.github/workflows/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1040 2023-12-14 16:32:14.000000 kerchunk-0.2.5/.github/workflows/default.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      320 2023-10-21 00:47:02.000000 kerchunk-0.2.5/.github/workflows/pre-commit.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      334 2023-12-14 16:32:14.000000 kerchunk-0.2.5/.github/workflows/pull_request.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      560 2024-05-03 18:35:33.000000 kerchunk-0.2.5/.github/workflows/tests.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)     1796 2024-05-03 18:35:33.000000 kerchunk-0.2.5/.gitignore
+-rw-r--r--   0 mdurant    (502) staff       (20)      416 2022-09-18 01:28:32.000000 kerchunk-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 mdurant    (502) staff       (20)     1063 2022-09-18 01:28:32.000000 kerchunk-0.2.5/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)      161 2024-05-03 18:35:33.000000 kerchunk-0.2.5/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     4251 2024-05-10 20:08:56.339741 kerchunk-0.2.5/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     2433 2022-09-23 18:01:10.000000 kerchunk-0.2.5/README.md
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-10 20:08:56.319710 kerchunk-0.2.5/binder/
+-rw-r--r--   0 mdurant    (502) staff       (20)      193 2022-09-18 01:28:32.000000 kerchunk-0.2.5/binder/environment.yml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-10 20:08:56.320715 kerchunk-0.2.5/ci/
+-rw-r--r--   0 mdurant    (502) staff       (20)      435 2024-05-03 18:35:33.000000 kerchunk-0.2.5/ci/environment-docs.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      462 2024-05-03 18:35:33.000000 kerchunk-0.2.5/ci/environment-py310.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      459 2024-05-03 18:35:33.000000 kerchunk-0.2.5/ci/environment-py311.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      459 2024-05-03 18:35:33.000000 kerchunk-0.2.5/ci/environment-py312.yml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-10 20:08:56.321864 kerchunk-0.2.5/docs/
+-rw-r--r--   0 mdurant    (502) staff       (20)      661 2022-09-18 01:28:32.000000 kerchunk-0.2.5/docs/Makefile
+-rw-r--r--   0 mdurant    (502) staff       (20)      209 2022-09-18 01:28:32.000000 kerchunk-0.2.5/docs/README.md
+-rw-r--r--   0 mdurant    (502) staff       (20)      795 2022-09-18 01:28:32.000000 kerchunk-0.2.5/docs/make.bat
+-rw-r--r--   0 mdurant    (502) staff       (20)      118 2023-12-14 16:32:14.000000 kerchunk-0.2.5/docs/requirements.txt
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-10 20:08:56.329611 kerchunk-0.2.5/docs/source/
+-rw-r--r--   0 mdurant    (502) staff       (20)     7845 2024-02-05 15:54:00.000000 kerchunk-0.2.5/docs/source/advanced.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     1118 2023-08-31 17:50:54.000000 kerchunk-0.2.5/docs/source/beyond.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     2681 2023-08-31 17:50:54.000000 kerchunk-0.2.5/docs/source/cases.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     1996 2022-12-09 18:27:45.000000 kerchunk-0.2.5/docs/source/conf.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7553 2023-08-31 17:50:54.000000 kerchunk-0.2.5/docs/source/contributing.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     3973 2023-08-31 17:50:54.000000 kerchunk-0.2.5/docs/source/detail.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-10 20:08:56.330890 kerchunk-0.2.5/docs/source/images/
+-rw-r--r--   0 mdurant    (502) staff       (20)   394242 2022-09-18 01:28:32.000000 kerchunk-0.2.5/docs/source/images/binary_buffer.png
+-rw-r--r--   0 mdurant    (502) staff       (20)   126383 2022-09-18 01:28:32.000000 kerchunk-0.2.5/docs/source/images/multi_refs.png
+-rw-r--r--   0 mdurant    (502) staff       (20)     3704 2023-08-31 17:50:54.000000 kerchunk-0.2.5/docs/source/index.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)    15075 2022-09-18 01:28:32.000000 kerchunk-0.2.5/docs/source/kerchunk.png
+-rw-r--r--   0 mdurant    (502) staff       (20)     3003 2023-08-31 17:50:54.000000 kerchunk-0.2.5/docs/source/nonzarr.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)    65655 2022-10-31 16:19:59.000000 kerchunk-0.2.5/docs/source/output_62_2.png
+-rw-r--r--   0 mdurant    (502) staff       (20)    28361 2022-10-31 16:19:59.000000 kerchunk-0.2.5/docs/source/output_63_2.png
+-rw-r--r--   0 mdurant    (502) staff       (20)     2433 2024-01-29 19:49:20.000000 kerchunk-0.2.5/docs/source/reference.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     7704 2024-02-16 19:53:29.000000 kerchunk-0.2.5/docs/source/spec.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     4092 2023-08-31 17:50:54.000000 kerchunk-0.2.5/docs/source/test_example.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)    25323 2024-02-16 19:53:29.000000 kerchunk-0.2.5/docs/source/tutorial.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-10 20:08:56.335383 kerchunk-0.2.5/kerchunk/
+-rw-r--r--   0 mdurant    (502) staff       (20)      756 2024-01-29 19:49:20.000000 kerchunk-0.2.5/kerchunk/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7000 2023-10-21 00:47:02.000000 kerchunk-0.2.5/kerchunk/codecs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    33190 2024-05-03 18:35:33.000000 kerchunk-0.2.5/kerchunk/combine.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4628 2023-11-17 17:47:22.000000 kerchunk-0.2.5/kerchunk/df.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9397 2023-11-09 18:05:32.000000 kerchunk-0.2.5/kerchunk/fits.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    21489 2024-05-03 18:35:33.000000 kerchunk-0.2.5/kerchunk/grib2.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    25691 2024-03-05 18:30:04.000000 kerchunk-0.2.5/kerchunk/hdf.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2483 2023-11-07 18:51:08.000000 kerchunk-0.2.5/kerchunk/mzML.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    11482 2023-11-09 18:05:32.000000 kerchunk-0.2.5/kerchunk/netCDF3.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-10 20:08:56.337529 kerchunk-0.2.5/kerchunk/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)    75779 2024-05-10 20:08:05.000000 kerchunk-0.2.5/kerchunk/tests/air.nc
+-rw-r--r--   0 mdurant    (502) staff       (20)       30 2022-10-31 16:19:59.000000 kerchunk-0.2.5/kerchunk/tests/conftest.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      469 2023-08-31 17:50:56.000000 kerchunk-0.2.5/kerchunk/tests/gen_hdf5.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      179 2024-05-03 18:35:33.000000 kerchunk-0.2.5/kerchunk/tests/tinygrib.grb2
+-rw-r--r--   0 mdurant    (502) staff       (20)     3589 2023-03-13 14:06:07.000000 kerchunk-0.2.5/kerchunk/tiff.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    13850 2023-12-14 16:32:14.000000 kerchunk-0.2.5/kerchunk/utils.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1382 2024-02-05 15:54:00.000000 kerchunk-0.2.5/kerchunk/xarray_backend.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1828 2024-05-03 18:35:33.000000 kerchunk-0.2.5/kerchunk/zarr.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2024-05-10 20:08:56.338189 kerchunk-0.2.5/kerchunk.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     4251 2024-05-10 20:08:56.000000 kerchunk-0.2.5/kerchunk.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     1424 2024-05-10 20:08:56.000000 kerchunk-0.2.5/kerchunk.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2024-05-10 20:08:56.000000 kerchunk-0.2.5/kerchunk.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      314 2024-05-10 20:08:56.000000 kerchunk-0.2.5/kerchunk.egg-info/entry_points.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      231 2024-05-10 20:08:56.000000 kerchunk-0.2.5/kerchunk.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        9 2024-05-10 20:08:56.000000 kerchunk-0.2.5/kerchunk.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)    15075 2022-09-18 01:28:32.000000 kerchunk-0.2.5/kerchunk.png
+-rw-r--r--   0 mdurant    (502) staff       (20)     1833 2024-02-29 21:00:13.000000 kerchunk-0.2.5/pyproject.toml
+-rw-r--r--   0 mdurant    (502) staff       (20)      476 2024-05-10 20:08:56.340241 kerchunk-0.2.5/setup.cfg
```

### Comparing `kerchunk-0.2.4/.github/workflows/default.yml` & `kerchunk-0.2.5/.github/workflows/default.yml`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/.github/workflows/tests.yml` & `kerchunk-0.2.5/.github/workflows/tests.yml`

 * *Files 16% similar despite different names*

```diff
@@ -4,25 +4,22 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [39, 310, 311]
+        python-version: [310, 311, 312]
 
     steps:
       - uses: actions/checkout@v4
       - name: Setup conda
-        uses: mamba-org/setup-micromamba@v1
+        uses: conda-incubator/setup-miniconda@v3
         with:
           environment-file: ci/environment-py${{matrix.python-version}}.yml
-          cache-downloads: false
-          cache-environment: true
-          generate-run-shell: false
       - name: Install kerchunk
         shell: bash -l {0}
         run: |
           pip install -e .
       - name: Test with pytest
         shell: bash -l {0}
         run: |
```

### Comparing `kerchunk-0.2.4/.gitignore` & `kerchunk-0.2.5/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -120,7 +120,10 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# VSCode settings
+.vscode/
```

### Comparing `kerchunk-0.2.4/LICENSE` & `kerchunk-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/PKG-INFO` & `kerchunk-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerchunk
-Version: 0.2.4
+Version: 0.2.5
 Summary: Functions to make reference descriptions for ReferenceFileSystem
 Author-email: Martin Durant <martin.durant@alumni.utoronto.ca>
 License: MIT
 Project-URL: Documentation, https://fsspec.github.io/kerchunk
 Project-URL: issue-tracker, https://github.com/fsspec/kerchunk/issues
 Project-URL: source-code, https://github.com/fsspec/kerchunk
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kerchunk-0.2.4/README.md` & `kerchunk-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/Makefile` & `kerchunk-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/make.bat` & `kerchunk-0.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/advanced.rst` & `kerchunk-0.2.5/docs/source/advanced.rst`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/beyond.rst` & `kerchunk-0.2.5/docs/source/beyond.rst`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/cases.rst` & `kerchunk-0.2.5/docs/source/cases.rst`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/conf.py` & `kerchunk-0.2.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/contributing.rst` & `kerchunk-0.2.5/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/detail.rst` & `kerchunk-0.2.5/docs/source/detail.rst`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/images/binary_buffer.png` & `kerchunk-0.2.5/docs/source/images/binary_buffer.png`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/images/multi_refs.png` & `kerchunk-0.2.5/docs/source/images/multi_refs.png`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/index.rst` & `kerchunk-0.2.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/kerchunk.png` & `kerchunk-0.2.5/docs/source/kerchunk.png`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/nonzarr.rst` & `kerchunk-0.2.5/docs/source/nonzarr.rst`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/output_62_2.png` & `kerchunk-0.2.5/docs/source/output_62_2.png`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/output_63_2.png` & `kerchunk-0.2.5/docs/source/output_63_2.png`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/reference.rst` & `kerchunk-0.2.5/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/spec.rst` & `kerchunk-0.2.5/docs/source/spec.rst`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/test_example.rst` & `kerchunk-0.2.5/docs/source/test_example.rst`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/docs/source/tutorial.rst` & `kerchunk-0.2.5/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/kerchunk/__init__.py` & `kerchunk-0.2.5/kerchunk/__init__.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/kerchunk/codecs.py` & `kerchunk-0.2.5/kerchunk/codecs.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/kerchunk/combine.py` & `kerchunk-0.2.5/kerchunk/combine.py`

 * *Files 0% similar despite different names*

```diff
@@ -752,15 +752,15 @@
     out[f"{path}.zarray"] = ujson.dumps(result_zarray)
 
     return consolidate(out)
 
 
 def auto_dask(
     urls: List[str],
-    single_driver: str,
+    single_driver: type,
     single_kwargs: dict,
     mzz_kwargs: dict,
     n_batches: int,
     remote_protocol=None,
     remote_options=None,
     filename=None,
     output_options=None,
```

### Comparing `kerchunk-0.2.4/kerchunk/df.py` & `kerchunk-0.2.5/kerchunk/df.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/kerchunk/fits.py` & `kerchunk-0.2.5/kerchunk/fits.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/kerchunk/grib2.py` & `kerchunk-0.2.5/kerchunk/grib2.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,21 +45,19 @@
         size = f.seek(0, 2)
         f.seek(0)
     part = 0
 
     while f.tell() < size:
         logger.debug(f"extract part {part + 1}")
         head = f.read(1024)
-        if len(head) < 1024:
-            break  # EOF
         if b"GRIB" not in head:
             f.seek(-4, 1)
             continue
         ind = head.index(b"GRIB")
-        start = f.tell() - 1024 + ind
+        start = f.tell() - len(head) + ind
         part_size = int.from_bytes(head[ind + 12 : ind + 16], "big")
         f.seek(start)
         yield start, part_size, f.read(part_size)
         part += 1
         if skip and part >= skip:
             break
 
@@ -248,17 +246,19 @@
                 ["y", "x"]
                 if m["gridType"] in cfgrib.dataset.GRID_TYPES_2D_NON_DIMENSION_COORDS
                 else ["latitude", "longitude"]
             )
             z[varName].attrs["_ARRAY_DIMENSIONS"] = dims
 
             for coord in cfgrib.dataset.COORD_ATTRS:
-                coord2 = {"latitude": "latitudes", "longitude": "longitudes"}.get(
-                    coord, coord
-                )
+                coord2 = {
+                    "latitude": "latitudes",
+                    "longitude": "longitudes",
+                    "step": "step:int",
+                }.get(coord, coord)
                 try:
                     x = m.get(coord2)
                 except eccodes.WrongStepUnitError as e:
                     logger.warning(
                         "Ignoring coordinate '%s' for varname '%s', raises: eccodes.WrongStepUnitError(%s)",
                         coord2,
                         varName,
```

### Comparing `kerchunk-0.2.4/kerchunk/hdf.py` & `kerchunk-0.2.5/kerchunk/hdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,23 +454,27 @@
 
                 # Store chunk location metadata...
                 if cinfo:
                     for k, v in cinfo.items():
                         if h5obj.fletcher32:
                             logging.info("Discarding fletcher32 checksum")
                             v["size"] -= 4
-                        if self.inline and isinstance(v, list) and v[2] < self.inline:
+                        if (
+                            self.inline
+                            and isinstance(v, dict)
+                            and v["size"] < self.inline
+                        ):
                             self.input_file.seek(v["offset"])
                             data = self.input_file.read(v["size"])
                             try:
                                 # easiest way to test if data is ascii
                                 data.decode("ascii")
                             except UnicodeDecodeError:
                                 data = b"base64:" + base64.b64encode(data)
-                            self.store[k] = data
+                            self.store[za._chunk_key(k)] = data
                         else:
                             self.store[za._chunk_key(k)] = [
                                 self._uri,
                                 v["offset"],
                                 v["size"],
                             ]
```

### Comparing `kerchunk-0.2.4/kerchunk/mzML.py` & `kerchunk-0.2.5/kerchunk/mzML.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/kerchunk/netCDF3.py` & `kerchunk-0.2.5/kerchunk/netCDF3.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/kerchunk/tiff.py` & `kerchunk-0.2.5/kerchunk/tiff.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/kerchunk/utils.py` & `kerchunk-0.2.5/kerchunk/utils.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/kerchunk/xarray_backend.py` & `kerchunk-0.2.5/kerchunk/xarray_backend.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/kerchunk/zarr.py` & `kerchunk-0.2.5/kerchunk/zarr.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import fsspec
 from fsspec.implementations.reference import LazyReferenceMapper
 
-from kerchunk.utils import class_factory
+import kerchunk.utils
 
 
 def single_zarr(
-    uri_or_store, storage_options=None, inline_threshold=100, inline=None, out=None
+    uri_or_store,
+    storage_options=None,
+    inline_threshold=100,
+    inline=None,
+    out=None,
 ):
     """kerchunk-style view on zarr mapper
 
     This is a similar process to zarr's consolidate_metadata, but does not
     need to be held in the original file tree. You do not need zarr itself
     to do this.
 
@@ -29,25 +33,28 @@
     -------
     reference dict like
     """
     if isinstance(uri_or_store, str):
         mapper = fsspec.get_mapper(uri_or_store, **(storage_options or {}))
     else:
         mapper = uri_or_store
+        if isinstance(mapper, fsspec.FSMap) and storage_options is None:
+            storage_options = mapper.fs.storage_options
 
     refs = out or {}
     for k in mapper:
         if k.startswith("."):
             refs[k] = mapper[k]
         else:
             refs[k] = [fsspec.utils._unstrip_protocol(mapper._key_to_str(k), mapper.fs)]
     from kerchunk.utils import do_inline
 
     inline_threshold = inline or inline_threshold
     if inline_threshold:
         refs = do_inline(refs, inline_threshold, remote_options=storage_options)
     if isinstance(refs, LazyReferenceMapper):
         refs.flush()
+    refs = kerchunk.utils.consolidate(refs)
     return refs
 
 
-ZarrToZarr = class_factory(single_zarr)
+ZarrToZarr = kerchunk.utils.class_factory(single_zarr)
```

### Comparing `kerchunk-0.2.4/kerchunk.egg-info/PKG-INFO` & `kerchunk-0.2.5/kerchunk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerchunk
-Version: 0.2.4
+Version: 0.2.5
 Summary: Functions to make reference descriptions for ReferenceFileSystem
 Author-email: Martin Durant <martin.durant@alumni.utoronto.ca>
 License: MIT
 Project-URL: Documentation, https://fsspec.github.io/kerchunk
 Project-URL: issue-tracker, https://github.com/fsspec/kerchunk/issues
 Project-URL: source-code, https://github.com/fsspec/kerchunk
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kerchunk-0.2.4/kerchunk.png` & `kerchunk-0.2.5/kerchunk.png`

 * *Files identical despite different names*

### Comparing `kerchunk-0.2.4/pyproject.toml` & `kerchunk-0.2.5/pyproject.toml`

 * *Files identical despite different names*

