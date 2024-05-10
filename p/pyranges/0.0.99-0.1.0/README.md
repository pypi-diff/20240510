# Comparing `tmp/pyranges-0.0.99.tar.gz` & `tmp/pyranges-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyranges-0.0.99.tar", last modified: Mon Jun  7 14:59:43 2021, max compression
+gzip compressed data, was "pyranges-0.1.0.tar", last modified: Wed May  1 10:47:34 2024, max compression
```

## Comparing `pyranges-0.0.99.tar` & `pyranges-0.1.0.tar`

### file list

```diff
@@ -1,95 +1,168 @@
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-07 14:59:43.028482 pyranges-0.0.99/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      724 2021-06-07 14:59:43.028268 pyranges-0.0.99/PKG-INFO
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    14020 2021-05-20 16:47:07.000000 pyranges-0.0.99/README.md
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-07 14:59:43.010396 pyranges-0.0.99/pyranges/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    18620 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/__init__.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    23055 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/data.py
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-07 14:59:43.021256 pyranges-0.0.99/pyranges/example_data/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      327 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/aorta.bed
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      269 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/aorta2.bed
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    12966 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/bw.bw
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)   309369 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/chipseq.bed
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)   309045 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/chipseq_background.bed
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      426 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/chromsizes.bed
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    69054 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/control.bam
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)  1716400 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/control.bam.bai
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    28209 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/cpg.bed
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    36057 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/ensembl.gtf
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    35943 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/ensembl_human.gtf.gz
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    64417 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/exons.bed
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       69 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/f1.bed
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       30 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/f2.bed
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    81253 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/gencode_human.gtf.gz
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    55608 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/lamina.bed
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    62555 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/example_data/ucsc_human.bed.gz
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    31717 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/genomicfeatures.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     2447 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/get_fasta.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      813 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/helpers.py
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-07 14:59:43.025198 pyranges-0.0.99/pyranges/methods/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        0 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/__init__.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1808 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/attr.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1227 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/call.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1431 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/cluster.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1482 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/concat.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     2032 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/coverage.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     2132 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/drop.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      241 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/drop_duplicates.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1130 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/getitem.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     5712 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/init.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      992 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/insert.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     3447 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/intersection.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        0 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/itergrs.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     4253 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/join.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     5386 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/k_nearest.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     4970 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/k_nearest_old.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      317 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/max_disjoint.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     2555 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/merge.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     4757 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/nearest.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1452 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/new_position.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      576 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/sort.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      751 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/split.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1249 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/statistics.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1329 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/subtraction.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1312 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/summary.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      727 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/to_rle.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1173 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/methods/windows.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     6792 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/multioverlap.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    13033 2021-05-20 18:50:24.000000 pyranges-0.0.99/pyranges/multithreaded.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     7832 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/out.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)   233880 2021-06-07 14:36:27.000000 pyranges-0.0.99/pyranges/pyranges.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    19608 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/readers.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    28741 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/statistics.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       34 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/stats.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     3313 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/subset.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     9398 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/tostring.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     9597 2021-05-20 16:47:07.000000 pyranges-0.0.99/pyranges/tostring2.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       23 2021-06-07 14:33:40.000000 pyranges-0.0.99/pyranges/version.py
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-07 14:59:43.010994 pyranges-0.0.99/pyranges.egg-info/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      724 2021-06-07 14:59:42.000000 pyranges-0.0.99/pyranges.egg-info/PKG-INFO
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     2324 2021-06-07 14:59:42.000000 pyranges-0.0.99/pyranges.egg-info/SOURCES.txt
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        1 2021-06-07 14:59:42.000000 pyranges-0.0.99/pyranges.egg-info/dependency_links.txt
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       73 2021-06-07 14:59:42.000000 pyranges-0.0.99/pyranges.egg-info/requires.txt
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       15 2021-06-07 14:59:42.000000 pyranges-0.0.99/pyranges.egg-info/top_level.txt
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)       38 2021-06-07 14:59:43.028529 pyranges-0.0.99/setup.cfg
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1545 2021-05-20 16:47:07.000000 pyranges-0.0.99/setup.py
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-07 14:59:43.027850 pyranges-0.0.99/tests/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        0 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/__init__.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     2041 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/conftest.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1727 2021-06-03 13:40:31.000000 pyranges-0.0.99/tests/helpers.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     8661 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/hypothesis_helper.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     6044 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/k_nearest.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      229 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/statistics.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)    18840 2021-06-07 14:33:09.000000 pyranges-0.0.99/tests/test_binary.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      657 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/test_change_chromosome_custom.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      727 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/test_concat.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     3486 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/test_do_not_error.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     6150 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/test_genomicfeatures.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      430 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/test_getset_attr.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1459 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/test_guessers.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1009 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/test_io.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      157 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/test_pickle.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)      723 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/test_stranded.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     9365 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/test_unary.py
-drwxr-xr-x   0 endrebakkenstovner   (501) staff       (20)        0 2021-06-07 14:59:43.028057 pyranges-0.0.99/tests/windows/
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)        0 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/windows/__init__.py
--rw-r--r--   0 endrebakkenstovner   (501) staff       (20)     1143 2021-05-20 16:47:07.000000 pyranges-0.0.99/tests/windows/test_windows.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:34.830587 pyranges-0.1.0/
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:30.745858 pyranges-0.1.0/.github/
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:31.212871 pyranges-0.1.0/.github/workflows/
+-rw-r--r--   0 endbak01   (501) staff       (20)     1555 2024-05-01 07:23:12.000000 pyranges-0.1.0/.github/workflows/build-book.yml
+-rw-r--r--   0 endbak01   (501) staff       (20)      855 2024-05-01 07:23:12.000000 pyranges-0.1.0/.github/workflows/build_and_upload_wheels.yml
+-rw-r--r--   0 endbak01   (501) staff       (20)     1091 2024-05-01 07:23:12.000000 pyranges-0.1.0/.github/workflows/check.yml
+-rw-r--r--   0 endbak01   (501) staff       (20)      731 2024-05-01 07:23:12.000000 pyranges-0.1.0/.github/workflows/run_hypothesis_tests.yml
+-rw-r--r--   0 endbak01   (501) staff       (20)      270 2024-05-01 07:23:12.000000 pyranges-0.1.0/.gitignore
+-rw-r--r--   0 endbak01   (501) staff       (20)       54 2024-05-01 07:23:12.000000 pyranges-0.1.0/CHANGELOG.txt
+-rw-r--r--   0 endbak01   (501) staff       (20)     1063 2024-05-01 07:23:12.000000 pyranges-0.1.0/LICENSE
+-rw-r--r--   0 endbak01   (501) staff       (20)     4267 2024-05-01 10:47:34.829129 pyranges-0.1.0/PKG-INFO
+-rw-r--r--   0 endbak01   (501) staff       (20)     2342 2024-05-01 07:23:12.000000 pyranges-0.1.0/README.md
+-rwxr-xr-x   0 endbak01   (501) staff       (20)     2077 2024-05-01 07:23:12.000000 pyranges-0.1.0/check_typing_linting_and_formatting.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      718 2024-05-01 07:23:12.000000 pyranges-0.1.0/conftest.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:32.227520 pyranges-0.1.0/docs/
+-rw-r--r--   0 endbak01   (501) staff       (20)      634 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/Makefile
+-rw-r--r--   0 endbak01   (501) staff       (20)      557 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/api_reference.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)     2487 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/conf.py
+-rw-r--r--   0 endbak01   (501) staff       (20)    13159 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/developer_guide.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)      233 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/extension_orfs.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)      157 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/extension_seqs.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)      170 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/extension_stats.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)     8593 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/how_to_columns.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)    15830 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/how_to_create.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)    33827 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/how_to_genomic_ops.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)    11786 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/how_to_inspect.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)      246 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/how_to_pages.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)    21762 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/how_to_rows.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)     9979 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/how_to_sequences.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)     3737 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/how_to_write.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)     1633 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/index.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)      975 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/installation.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)      795 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/make.bat
+-rw-r--r--   0 endbak01   (501) staff       (20)      227 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/pyranges_extensions.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)     2979 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/pyranges_module.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)      209 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/pyranges_objects.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)      271 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/range_frame.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)       38 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/requirements.txt
+-rw-r--r--   0 endbak01   (501) staff       (20)     1191 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/todos.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)    46812 2024-05-01 07:23:12.000000 pyranges-0.1.0/docs/tutorial.rst
+-rw-r--r--   0 endbak01   (501) staff       (20)     2747 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyproject.toml
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:32.459536 pyranges-0.1.0/pyranges/
+-rw-r--r--   0 endbak01   (501) staff       (20)     1066 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/__init__.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:33.007920 pyranges-0.1.0/pyranges/core/
+-rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/__init__.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     1672 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/empty.py
+-rw-r--r--   0 endbak01   (501) staff       (20)    12623 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/example_data.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     5476 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/loci_getter.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     6200 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/multioverlap.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     5200 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/names.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     3424 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/options.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     9214 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/out.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     4957 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/parallelism.py
+-rw-r--r--   0 endbak01   (501) staff       (20)    10009 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/pyranges_groupby.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     7223 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/pyranges_helpers.py
+-rw-r--r--   0 endbak01   (501) staff       (20)   213034 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/pyranges_main.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     2845 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/random.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     7161 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/tostring.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     1315 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/core/version.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:33.744406 pyranges-0.1.0/pyranges/data/
+-rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/__init__.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      327 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/aorta.bed
+-rw-r--r--   0 endbak01   (501) staff       (20)      269 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/aorta2.bed
+-rw-r--r--   0 endbak01   (501) staff       (20)   309369 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/chipseq.bed
+-rw-r--r--   0 endbak01   (501) staff       (20)   309045 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/chipseq_background.bed
+-rw-r--r--   0 endbak01   (501) staff       (20)      426 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/chromsizes.bed
+-rw-r--r--   0 endbak01   (501) staff       (20)    28209 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/cpg.bed
+-rw-r--r--   0 endbak01   (501) staff       (20)     4845 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/ensembl.gtf
+-rw-r--r--   0 endbak01   (501) staff       (20)    35943 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/ensembl_human.gtf.gz
+-rw-r--r--   0 endbak01   (501) staff       (20)    64417 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/exons.bed
+-rw-r--r--   0 endbak01   (501) staff       (20)       69 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/f1.bed
+-rw-r--r--   0 endbak01   (501) staff       (20)       30 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/f2.bed
+-rw-r--r--   0 endbak01   (501) staff       (20)    81253 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/gencode_human.gtf.gz
+-rw-r--r--   0 endbak01   (501) staff       (20)    55608 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/lamina.bed
+-rw-r--r--   0 endbak01   (501) staff       (20)   387402 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/ncbi.fasta
+-rw-r--r--   0 endbak01   (501) staff       (20)      220 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/ncbi.fasta.fai
+-rw-r--r--   0 endbak01   (501) staff       (20)     3041 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/ncbi.gff.gz
+-rw-r--r--   0 endbak01   (501) staff       (20)     1366 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/smaller.bam
+-rw-r--r--   0 endbak01   (501) staff       (20)    62555 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/data/ucsc_human.bed.gz
+-rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/docs
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:33.765286 pyranges-0.1.0/pyranges/ext/
+-rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/ext/__init__.py
+-rw-r--r--   0 endbak01   (501) staff       (20)    30149 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/ext/orfs.py
+-rw-r--r--   0 endbak01   (501) staff       (20)    13762 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/ext/seqs.py
+-rw-r--r--   0 endbak01   (501) staff       (20)    27439 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/ext/stats.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:33.780238 pyranges-0.1.0/pyranges/methods/
+-rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/__init__.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     2197 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/boundaries.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      645 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/cluster.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      900 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/combine_positions.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     3407 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/concat.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     2114 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/coverage.py
+-rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/itergrs.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     2483 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/join.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      365 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/max_disjoint.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      857 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/merge.py
+-rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/merge_cluster.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     5349 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/nearest.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     3983 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/overlap.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      254 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/sort.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     3818 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/spliced_subsequence.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      952 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/split.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     1349 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/statistics.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     3500 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/subsequence.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     1229 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/subtraction.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     1612 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/summary.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     4056 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/tile_genome.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     1107 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/to_rle.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     2354 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/methods/windows.py
+-rw-r--r--   0 endbak01   (501) staff       (20)       73 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/orfs.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:33.788557 pyranges-0.1.0/pyranges/range_frame/
+-rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/range_frame/__init__.py
+-rw-r--r--   0 endbak01   (501) staff       (20)    12603 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/range_frame/range_frame.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     6741 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/range_frame/range_frame_validator.py
+-rw-r--r--   0 endbak01   (501) staff       (20)    21738 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/readers.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      138 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/seqs.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      338 2024-05-01 07:23:12.000000 pyranges-0.1.0/pyranges/stats.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:34.824736 pyranges-0.1.0/pyranges.egg-info/
+-rw-r--r--   0 endbak01   (501) staff       (20)     4267 2024-05-01 10:47:30.000000 pyranges-0.1.0/pyranges.egg-info/PKG-INFO
+-rw-r--r--   0 endbak01   (501) staff       (20)     3909 2024-05-01 10:47:30.000000 pyranges-0.1.0/pyranges.egg-info/SOURCES.txt
+-rw-r--r--   0 endbak01   (501) staff       (20)        1 2024-05-01 10:47:30.000000 pyranges-0.1.0/pyranges.egg-info/dependency_links.txt
+-rw-r--r--   0 endbak01   (501) staff       (20)      352 2024-05-01 10:47:30.000000 pyranges-0.1.0/pyranges.egg-info/requires.txt
+-rw-r--r--   0 endbak01   (501) staff       (20)       25 2024-05-01 10:47:30.000000 pyranges-0.1.0/pyranges.egg-info/top_level.txt
+-rw-r--r--   0 endbak01   (501) staff       (20)       38 2024-05-01 10:47:34.830782 pyranges-0.1.0/setup.cfg
+-rw-r--r--   0 endbak01   (501) staff       (20)      246 2024-05-01 07:23:12.000000 pyranges-0.1.0/setup.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:33.996915 pyranges-0.1.0/tests/
+-rw-r--r--   0 endbak01   (501) staff       (20)    11164 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/.fuse_hidden0000017200000002
+-rw-r--r--   0 endbak01   (501) staff       (20)     1820 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/helpers.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     1890 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/hi
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:34.249203 pyranges-0.1.0/tests/property_based/
+-rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/property_based/__init__.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     7906 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/property_based/hypothesis_helper.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     9254 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/property_based/new.py
+-rw-r--r--   0 endbak01   (501) staff       (20)    17767 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/property_based/test_binary.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     3413 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/property_based/test_do_not_error.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     9456 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/property_based/test_unary.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      312 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/run_doctest_tutorial_howto.py
+-rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/test_calculate_frame.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     1464 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/test_parallelism.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:34.581411 pyranges-0.1.0/tests/unit/
+-rw-r--r--   0 endbak01   (501) staff       (20)        1 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/__init__.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      534 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/chip_10.bed
+-rw-r--r--   0 endbak01   (501) staff       (20)     2354 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/conftest.py
+-rw-r--r--   0 endbak01   (501) staff       (20)       44 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/f1.bed
+-rw-r--r--   0 endbak01   (501) staff       (20)       29 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/f2.bed
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:34.582155 pyranges-0.1.0/tests/unit/getitem/
+-rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/getitem/test_getitem.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     1890 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/hi
+-rw-r--r--   0 endbak01   (501) staff       (20)     6096 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/k_nearest.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:34.660380 pyranges-0.1.0/tests/unit/new_position/
+-rw-r--r--   0 endbak01   (501) staff       (20)      456 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/new_position/test_new_position.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:34.673557 pyranges-0.1.0/tests/unit/out/
+-rw-r--r--   0 endbak01   (501) staff       (20)      827 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/out/test_out.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:34.684065 pyranges-0.1.0/tests/unit/spliced_subsequence/
+-rw-r--r--   0 endbak01   (501) staff       (20)     2293 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/spliced_subsequence/test_spliced_subsequence.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      282 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/statistics.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      784 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/test_concat.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     1542 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/test_count_overlaps.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:34.816026 pyranges-0.1.0/tests/unit/test_data/
+-rw-r--r--   0 endbak01   (501) staff       (20)     4399 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/test_data/ensembl.gtf
+-rw-r--r--   0 endbak01   (501) staff       (20)    71593 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/test_data/test_sorted.bam
+-rw-r--r--   0 endbak01   (501) staff       (20)  1706448 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/test_data/test_sorted.bam.bai
+-rw-r--r--   0 endbak01   (501) staff       (20)     1456 2024-05-01 07:23:12.000000 pyranges-0.1.0/tests/unit/test_guessers.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     2090 2024-05-01 07:23:13.000000 pyranges-0.1.0/tests/unit/test_join.py
+-rw-r--r--   0 endbak01   (501) staff       (20)     6641 2024-05-01 07:23:13.000000 pyranges-0.1.0/tests/unit/test_pandas_overrides.py
+-rw-r--r--   0 endbak01   (501) staff       (20)      395 2024-05-01 07:23:13.000000 pyranges-0.1.0/tests/unit/test_tostring.py
+drwxr-xr-x   0 endbak01   (501) staff       (20)        0 2024-05-01 10:47:34.823433 pyranges-0.1.0/tests/unit/unit/
+-rw-r--r--   0 endbak01   (501) staff       (20)        0 2024-05-01 07:23:13.000000 pyranges-0.1.0/tests/unit/unit/__init__.py
```

### Comparing `pyranges-0.0.99/pyranges/example_data/chipseq.bed` & `pyranges-0.1.0/pyranges/data/chipseq.bed`

 * *Files identical despite different names*

### Comparing `pyranges-0.0.99/pyranges/example_data/chipseq_background.bed` & `pyranges-0.1.0/pyranges/data/chipseq_background.bed`

 * *Files identical despite different names*

### Comparing `pyranges-0.0.99/pyranges/example_data/cpg.bed` & `pyranges-0.1.0/pyranges/data/cpg.bed`

 * *Files identical despite different names*

### Comparing `pyranges-0.0.99/pyranges/example_data/ensembl_human.gtf.gz` & `pyranges-0.1.0/pyranges/data/ensembl_human.gtf.gz`

 * *Files identical despite different names*

### Comparing `pyranges-0.0.99/pyranges/example_data/exons.bed` & `pyranges-0.1.0/pyranges/data/exons.bed`

 * *Files identical despite different names*

### Comparing `pyranges-0.0.99/pyranges/example_data/gencode_human.gtf.gz` & `pyranges-0.1.0/pyranges/data/gencode_human.gtf.gz`

 * *Files identical despite different names*

### Comparing `pyranges-0.0.99/pyranges/example_data/lamina.bed` & `pyranges-0.1.0/pyranges/data/lamina.bed`

 * *Files identical despite different names*

### Comparing `pyranges-0.0.99/pyranges/example_data/ucsc_human.bed.gz` & `pyranges-0.1.0/pyranges/data/ucsc_human.bed.gz`

 * *Files identical despite different names*

### Comparing `pyranges-0.0.99/pyranges/methods/coverage.py` & `pyranges-0.1.0/pyranges/methods/coverage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,72 @@
 import numpy as np
 import pandas as pd
-from ncls import NCLS
+from ncls import NCLS  # type: ignore[import]
 
 
-def _number_overlapping(scdf, ocdf, **kwargs):
-
+def _number_overlapping(df: pd.DataFrame, df2: pd.DataFrame, **kwargs) -> pd.DataFrame:
     keep_nonoverlapping = kwargs.get("keep_nonoverlapping", True)
     column_name = kwargs.get("overlap_col", True)
 
-    if scdf.empty:
-        return None
-    if ocdf.empty:
+    if df.empty:
+        return df
+    if df2.empty:
         if keep_nonoverlapping:
-            df = scdf.copy()
+            df = df.copy()
             df.insert(df.shape[1], column_name, 0)
             return df
-        else:
-            return None
+        return df2
 
-    oncls = NCLS(ocdf.Start.values, ocdf.End.values, ocdf.index.values)
+    oncls = NCLS(df2.Start.to_numpy(), df2.End.to_numpy(), df2.index.to_numpy())
 
-    starts = scdf.Start.values
-    ends = scdf.End.values
-    indexes = scdf.index.values
+    starts = df.Start.to_numpy()
+    ends = df.End.to_numpy()
+    indexes = df.index.to_numpy()
 
-    _self_indexes, _other_indexes = oncls.all_overlaps_both(
-        starts, ends, indexes)
+    _self_indexes, _other_indexes = oncls.all_overlaps_both(starts, ends, indexes)
 
     s = pd.Series(_self_indexes)
     counts_per_read = s.value_counts()[s.unique()].reset_index()
     counts_per_read.columns = ["Index", "Count"]
 
-    df = scdf.copy()
+    df = df.copy()
 
-    if keep_nonoverlapping:
-        _missing_indexes = np.setdiff1d(scdf.index, _self_indexes)
-        missing = pd.DataFrame(data={"Index": _missing_indexes, "Count": 0}, index=_missing_indexes)
-        counts_per_read = pd.concat([counts_per_read, missing])
-    else:
-        df = df.loc[_self_indexes]
+    _missing_indexes = np.setdiff1d(df.index, _self_indexes)
+    missing = pd.DataFrame(data={"Index": _missing_indexes, "Count": 0}, index=_missing_indexes)
+    counts_per_read = pd.concat([counts_per_read, missing])
 
-    counts_per_read = counts_per_read.set_index("Index")
+    counts_per_read = counts_per_read.set_index("Index").sort_index().squeeze()
 
     df.insert(df.shape[1], column_name, counts_per_read)
 
-    return df
-
-
+    if keep_nonoverlapping:
+        return df
+    return df[df[column_name] != 0]
 
-def _coverage(scdf, ocdf, **kwargs):
 
+def _coverage(df: pd.DataFrame, df2: pd.DataFrame, **kwargs) -> pd.DataFrame:
     fraction_col = kwargs["fraction_col"]
 
-    if scdf.empty:
-        return None
-    if ocdf.empty:
-        df = scdf.copy()
+    if df.empty:
+        return df
+    if df2.empty:
+        df = df.copy()
         df.insert(df.shape[1], fraction_col, 0.0)
         return df
 
-    oncls = NCLS(ocdf.Start.values, ocdf.End.values, ocdf.index.values)
+    oncls = NCLS(df2.Start.to_numpy(), df2.End.to_numpy(), df2.index.to_numpy())
 
-    starts = scdf.Start.values
-    ends = scdf.End.values
-    indexes = scdf.index.values
+    starts = df.Start.to_numpy()
+    ends = df.End.to_numpy()
+    indexes = df.index.to_numpy()
 
     _lengths = oncls.coverage(starts, ends, indexes)
-    _lengths = _lengths /  (ends - starts)
+    _lengths = _lengths / (ends - starts)
     _fractions = _lengths
     _fractions = _fractions.astype("float64")
     _fractions = np.nan_to_num(_fractions)
 
-    scdf = scdf.copy()
+    df = df.copy()
 
-    scdf.insert(scdf.shape[1], fraction_col, _fractions)
+    df.insert(df.shape[1], fraction_col, _fractions)
 
-    return scdf
+    return df
```

### Comparing `pyranges-0.0.99/pyranges/methods/nearest.py` & `pyranges-0.1.0/pyranges/methods/nearest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,150 +1,158 @@
-import pandas as pd
-
-
-from .join import _both_dfs
-from .sort import sort_one_by_one
-
-from sorted_nearest import (nearest_previous_nonoverlapping,
-                            nearest_next_nonoverlapping,
-                            nearest_nonoverlapping)
+from typing import TYPE_CHECKING
 
+import pandas as pd
+from ncls import NCLS  # type: ignore[import]
+from sorted_nearest import (  # type: ignore[import]
+    nearest_next_nonoverlapping,
+    nearest_nonoverlapping,
+    nearest_previous_nonoverlapping,
+)
+
+import pyranges.core.empty
+from pyranges import PyRanges
+from pyranges.core.names import END_COL, START_COL
+from pyranges.methods.sort import sort_one_by_one
+
+if TYPE_CHECKING:
+    from numpy.typing import ArrayLike, NDArray
+    from pandas import DataFrame
 
-def _insert_distance(ocdf, dist, suffix):
 
-    if "Distance" not in ocdf:
+def _insert_distance(df2: pd.DataFrame, dist: "NDArray | int", suffix: str) -> pd.DataFrame:
+    if "Distance" not in df2:
         distance_column_name = "Distance"
-    elif "Distance" + suffix not in ocdf:
+    elif "Distance" + suffix not in df2:
         distance_column_name = "Distance" + suffix
     else:
         i = 1
-        while "Distance" + str(i) in ocdf:
+        while "Distance" + str(i) in df2:
             i += 1
         distance_column_name = "Distance" + str(i)
 
-    ocdf.insert(ocdf.shape[1], distance_column_name,
-                pd.Series(dist, index=ocdf.index).fillna(-1).astype(int))
-
-    return ocdf
+    df2.insert(
+        df2.shape[1],
+        distance_column_name,
+        pd.Series(dist, index=df2.index).fillna(-1).astype(int),
+    )
 
+    return df2
 
-def _overlapping_for_nearest(scdf, ocdf, suffix):
 
+def _overlapping_for_nearest(df: pd.DataFrame, df2: pd.DataFrame, suffix: str) -> tuple[pd.DataFrame, pd.DataFrame]:
     nearest_df = pd.DataFrame(columns="Chromosome Start End Strand".split())
 
-    scdf2, ocdf2 = _both_dfs(scdf, ocdf, how="first")
+    it = NCLS(df2.Start.to_numpy(), df2.End.to_numpy(), df2.index.to_numpy())
 
-    if not ocdf2.empty:
-        original_idx = scdf.index
-
-        idxs = scdf2.index
-        original_idx = scdf.index.copy(deep=True)
+    idx_self, idx_other = it.first_overlap_both(
+        df[START_COL].to_numpy(),
+        df[END_COL].to_numpy(),
+        df.index.to_numpy(),
+    )
+    self, other = df.reindex(idx_self), df2.reindex(idx_other)
+
+    if not other.empty:
+        idxs = self.index
+        original_idx = df.index.copy(deep=True)
         missing_idxs = ~original_idx.isin(idxs)
-        missing_overlap = scdf.index[missing_idxs]
+        missing_overlap = df.index[missing_idxs]
 
-        df_to_find_nearest_in = scdf.reindex(missing_overlap)
+        df_to_find_nearest_in = df.reindex(missing_overlap)
 
-        odf = ocdf.reindex(ocdf2.index)
+        odf = df2.reindex(other.index)
         odf.index = idxs
-        sdf = scdf.reindex(idxs)
+        sdf = df.reindex(idxs)
 
         nearest_df = sdf.join(odf, rsuffix=suffix)
         nearest_df = _insert_distance(nearest_df, 0, suffix)
     else:
-        df_to_find_nearest_in = scdf
+        df_to_find_nearest_in = df
 
     return nearest_df, df_to_find_nearest_in
 
 
-def _next_nonoverlapping(left_ends, right_starts, right_indexes):
-
+def _next_nonoverlapping(
+    left_ends: pd.Series,
+    right_starts: pd.Series,
+    right_indexes: "ArrayLike",
+) -> tuple["NDArray", "NDArray"]:
     left_ends = left_ends.sort_values()
     right_starts = right_starts.sort_values()
-    r_idx, dist = nearest_next_nonoverlapping(
-        left_ends.values - 1, right_starts.values, right_indexes)
-    r_idx = pd.Series(r_idx, index=left_ends.index).sort_index().values
-    dist = pd.Series(dist, index=left_ends.index).sort_index().values
+    r_idx, dist = nearest_next_nonoverlapping(left_ends.to_numpy() - 1, right_starts.to_numpy(), right_indexes)
+    r_idx = pd.Series(r_idx, index=left_ends.index).sort_index().to_numpy()
+    dist = pd.Series(dist, index=left_ends.index).sort_index().to_numpy()
 
     return r_idx, dist
 
 
-def _previous_nonoverlapping(left_starts, right_ends):
-
+def _previous_nonoverlapping(left_starts: pd.Series, right_ends: pd.Series) -> tuple["NDArray", "NDArray"]:
     left_starts = left_starts.sort_values()
     right_ends = right_ends.sort_values()
     r_idx, dist = nearest_previous_nonoverlapping(
-        left_starts.values, right_ends.values - 1, right_ends.index.values)
+        left_starts.to_numpy(),
+        right_ends.to_numpy() - 1,
+        right_ends.index.to_numpy(),
+    )
 
-    r_idx = pd.Series(r_idx, index=left_starts.index).sort_index().values
-    dist = pd.Series(dist, index=left_starts.index).sort_index().values
+    r_idx = pd.Series(r_idx, index=left_starts.index).sort_index().to_numpy()
+    dist = pd.Series(dist, index=left_starts.index).sort_index().to_numpy()
 
     return r_idx, dist
 
 
-def _nearest(scdf, ocdf, **kwargs):
-
-    if scdf.empty or ocdf.empty:
-        return None
+def _nearest(df: "DataFrame", df2: "DataFrame", **kwargs) -> pd.DataFrame:
+    if df.empty or df2.empty:
+        return PyRanges()
 
     overlap = kwargs["overlap"]
     how = kwargs["how"]
     suffix = kwargs["suffix"]
 
     if how == "upstream":
-        strand = scdf.Strand.iloc[0]
+        strand = df.Strand.iloc[0]
         how = {"+": "previous", "-": "next"}[strand]
     elif how == "downstream":
-        strand = scdf.Strand.iloc[0]
+        strand = df.Strand.iloc[0]
         how = {"+": "next", "-": "previous"}[strand]
 
-    ocdf = ocdf.reset_index(drop=True)
+    df2 = df2.reset_index(drop=True)
 
     if overlap:
-        nearest_df, df_to_find_nearest_in = _overlapping_for_nearest(
-            scdf, ocdf, suffix)
+        nearest_df, df_to_find_nearest_in = _overlapping_for_nearest(df, df2, suffix)
     else:
-        df_to_find_nearest_in = scdf
+        df_to_find_nearest_in = df
+        nearest_df = pyranges.core.empty.empty()
 
+    df = pyranges.core.empty.empty_df()
     if not df_to_find_nearest_in.empty:
-        df_to_find_nearest_in = sort_one_by_one(df_to_find_nearest_in, "Start",
-                                                "End")
-        ocdf = sort_one_by_one(ocdf, "Start", "End")
-        df_to_find_nearest_in.index = pd.Index(
-            range(len(df_to_find_nearest_in)))
+        df_to_find_nearest_in = sort_one_by_one(df_to_find_nearest_in, "Start", "End")
+        df2 = sort_one_by_one(df2, "Start", "End")
+        df_to_find_nearest_in.index = pd.Index(range(len(df_to_find_nearest_in)))
 
         if how == "next":
-            r_idx, dist = _next_nonoverlapping(df_to_find_nearest_in.End,
-                                               ocdf.Start, ocdf.index.values)
+            r_idx, dist = _next_nonoverlapping(df_to_find_nearest_in.End, df2.Start, df2.index.to_numpy())
         elif how == "previous":
-            r_idx, dist = _previous_nonoverlapping(df_to_find_nearest_in.Start,
-                                                   ocdf.End)
+            r_idx, dist = _previous_nonoverlapping(df_to_find_nearest_in.Start, df2.End)
         else:
-            previous_r_idx, previous_dist = _previous_nonoverlapping(
-                df_to_find_nearest_in.Start, ocdf.End)
-
-            next_r_idx, next_dist = _next_nonoverlapping(
-                df_to_find_nearest_in.End, ocdf.Start, ocdf.index.values)
+            previous_r_idx, previous_dist = _previous_nonoverlapping(df_to_find_nearest_in.Start, df2.End)
 
-            r_idx, dist = nearest_nonoverlapping(previous_r_idx, previous_dist,
-                                                 next_r_idx, next_dist)
+            next_r_idx, next_dist = _next_nonoverlapping(df_to_find_nearest_in.End, df2.Start, df2.index.to_numpy())
 
+            r_idx, dist = nearest_nonoverlapping(previous_r_idx, previous_dist, next_r_idx, next_dist)
 
-        ocdf = ocdf.reindex(r_idx)
+        df2 = df2.reindex(r_idx)
 
-        ocdf.index = df_to_find_nearest_in.index
+        df2.index = df_to_find_nearest_in.index
 
-        ocdf = _insert_distance(ocdf, dist, suffix)
+        df2 = _insert_distance(df2, dist, suffix)
 
-        r_idx = pd.Series(r_idx, index=ocdf.index)
-        df_to_find_nearest_in = df_to_find_nearest_in.drop(
-            r_idx.loc[r_idx == -1].index)
+        _r_idx = pd.Series(r_idx, index=df2.index)
+        df_to_find_nearest_in = df_to_find_nearest_in.drop(_r_idx[_r_idx == -1].index)
 
-        df = df_to_find_nearest_in.join(ocdf, rsuffix=suffix)
+        df = df_to_find_nearest_in.join(df2, rsuffix=suffix)
 
     if overlap and "df" in locals() and not df.empty and not nearest_df.empty:
-
         df = pd.concat([nearest_df, df], sort=False)
     elif overlap and not nearest_df.empty:
         df = nearest_df
 
-    df = df.drop("Chromosome" + suffix, axis=1)
-    return df
+    return PyRanges(df.drop("Chromosome" + suffix, axis=1))
```

### Comparing `pyranges-0.0.99/pyranges/readers.py` & `pyranges-0.1.0/pyranges/readers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,535 +1,618 @@
-from __future__ import print_function
-
+import logging
 import sys
+from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pandas as pd
+from natsort import natsorted  # type: ignore[import]
+
+from pyranges.core.pyranges_helpers import mypy_ensure_pyranges
+
+if TYPE_CHECKING:
+    from pyranges.core.pyranges_main import PyRanges
 
-from pyranges.pyranges import PyRanges
+logging.basicConfig(level=logging.INFO)
+LOGGER = logging.getLogger(__name__)
+LOGGER.setLevel(logging.INFO)
 
-from io import StringIO
 
-import pyranges as pr
-from pyranges.version import __version__
+def from_string(s: str) -> "PyRanges":
+    """Create a PyRanges from multiline string.
 
+    Parameters
+    ----------
+    s : str
+        String with data.
 
-def read_bed(f, as_df=False, nrows=None):
+    Examples
+    --------
+    >>> import pyranges as pr
+    >>> s = '''Chromosome      Start        End Strand
+    ... chr1  246719402  246719502      +
+    ... chr5   15400908   15401008      +
+    ... chr9   68366534   68366634      +
+    ... chr14   79220091   79220191      +
+    ... chr14  103456471  103456571      -'''
+
+    >>> pr.from_string(s)
+      index  |    Chromosome        Start        End  Strand
+      int64  |    object            int64      int64  object
+    -------  ---  ------------  ---------  ---------  --------
+          0  |    chr1          246719402  246719502  +
+          1  |    chr5           15400908   15401008  +
+          2  |    chr9           68366534   68366634  +
+          3  |    chr14          79220091   79220191  +
+          4  |    chr14         103456471  103456571  -
+    PyRanges with 5 rows, 4 columns, and 1 index columns.
+    Contains 4 chromosomes and 2 strands.
+
+    """
+    from io import StringIO
 
+    df = pd.read_csv(StringIO(s), sep=r"\s+", index_col=None)
+
+    return mypy_ensure_pyranges(df)
+
+
+def read_bed(f: Path, /, nrows: int | None = None) -> "PyRanges":
     """Return bed file as PyRanges.
 
     This is a reader for files that follow the bed format. They can have from
     3-12 columns which will be named like so:
 
     Chromosome Start End Name Score Strand ThickStart ThickEnd ItemRGB
     BlockCount BlockSizes BlockStarts
 
     Parameters
     ----------
     f : str
-
         Path to bed file
 
-    as_df : bool, default False
-
-        Whether to return as pandas DataFrame instead of PyRanges.
-
-    nrows : int, default None
-
+    nrows : Optional int, default None
         Number of rows to return.
 
     Notes
     -----
-
     If you just want to create a PyRanges from a tab-delimited bed-like file,
     use `pr.PyRanges(pandas.read_table(f))` instead.
 
     Examples
     --------
-
-    >>> path = pr.get_example_path("aorta.bed")
+    >>> import pyranges as pr
+    >>> path = pr.example_data.files["aorta.bed"]
     >>> pr.read_bed(path, nrows=5)
-    +--------------+-----------+-----------+------------+-----------+--------------+
-    | Chromosome   |     Start |       End | Name       |     Score | Strand       |
-    | (category)   |   (int32) |   (int32) | (object)   |   (int64) | (category)   |
-    |--------------+-----------+-----------+------------+-----------+--------------|
-    | chr1         |      9939 |     10138 | H3K27me3   |         7 | +            |
-    | chr1         |      9953 |     10152 | H3K27me3   |         5 | +            |
-    | chr1         |      9916 |     10115 | H3K27me3   |         5 | -            |
-    | chr1         |      9951 |     10150 | H3K27me3   |         8 | -            |
-    | chr1         |      9978 |     10177 | H3K27me3   |         7 | -            |
-    +--------------+-----------+-----------+------------+-----------+--------------+
-    Stranded PyRanges object has 5 rows and 6 columns from 1 chromosomes.
-    For printing, the PyRanges was sorted on Chromosome and Strand.
-
-    >>> pr.read_bed(path, as_df=True, nrows=5)
-      Chromosome  Start    End      Name  Score Strand
-    0       chr1   9916  10115  H3K27me3      5      -
-    1       chr1   9939  10138  H3K27me3      7      +
-    2       chr1   9951  10150  H3K27me3      8      -
-    3       chr1   9953  10152  H3K27me3      5      +
-    4       chr1   9978  10177  H3K27me3      7      -
-    """
+      index  |    Chromosome      Start      End  Name        Score  Strand
+      int64  |    category        int64    int64  object      int64  category
+    -------  ---  ------------  -------  -------  --------  -------  ----------
+          0  |    chr1             9916    10115  H3K27me3        5  -
+          1  |    chr1             9939    10138  H3K27me3        7  +
+          2  |    chr1             9951    10150  H3K27me3        8  -
+          3  |    chr1             9953    10152  H3K27me3        5  +
+          4  |    chr1             9978    10177  H3K27me3        7  -
+    PyRanges with 5 rows, 6 columns, and 1 index columns.
+    Contains 1 chromosomes and 2 strands.
 
-    columns = "Chromosome Start End Name Score Strand ThickStart ThickEnd ItemRGB BlockCount BlockSizes BlockStarts".split(
+    """
+    columns = (
+        "Chromosome Start End Name Score Strand ThickStart ThickEnd ItemRGB BlockCount BlockSizes BlockStarts".split()
     )
-
-    if f.endswith(".gz"):
+    path = Path(f)
+    if path.name.endswith(".gz"):
         import gzip
-        first_start = gzip.open(f).readline().split()[1]
+
+        first_start = gzip.open(path).readline().decode().split()[1]
     else:
-        first_start = open(f).readline().split()[1]
+        first_start = path.open().readline().split()[1]
 
     header = None
 
     try:
         int(first_start)
     except ValueError:
         header = 0
 
+    ncols = pd.read_table(path, nrows=2).shape[1]
+
     df = pd.read_csv(
-        f,
-        dtype={
-            "Chromosome": "category",
-            "Strand": "category"
-        },
+        path,
+        dtype={"Chromosome": "category", "Strand": "category"},
         nrows=nrows,
         header=header,
-        sep="\t")
-
-    df.columns = columns[:df.shape[1]]
+        names=columns[:ncols] if header != 0 else None,
+        sep="\t",
+    )
 
-    if not as_df:
-        return PyRanges(df)
-    else:
-        return df
+    df.columns = pd.Index(columns[: df.shape[1]])
 
+    return mypy_ensure_pyranges(df)
 
-def read_bam(f, sparse=True, as_df=False, mapq=0, required_flag=0, filter_flag=1540):
 
+def read_bam(
+    f: str | Path,
+    /,
+    mapq: int = 0,
+    required_flag: int = 0,
+    filter_flag: int = 1540,
+    *,
+    sparse: bool = True,
+) -> "PyRanges":
     """Return bam file as PyRanges.
 
     Parameters
     ----------
     f : str
-
         Path to bam file
 
     sparse : bool, default True
-
-        Whether to return only.
-
-    as_df : bool, default False
-
-        Whether to return as pandas DataFrame instead of PyRanges.
+        Whether to return only the columns Chromosome, Start, End, Strand, Flag.
+        Set to False to return also columns
+        QueryStart, QueryEnd, QuerySequence, Name, Cigar, Quality (more time consuming).
 
     mapq : int, default 0
-
         Minimum mapping quality score.
 
     required_flag : int, default 0
-
         Flags which must be present for the interval to be read.
 
     filter_flag : int, default 1540
-
         Ignore reads with these flags. Default 1540, which means that either
         the read is unmapped, the read failed vendor or platfrom quality
         checks, or the read is a PCR or optical duplicate.
 
     Notes
     -----
-
     This functionality requires the library `bamread`. It can be installed with
     `pip install bamread` or `conda install -c bioconda bamread`.
 
     Examples
     --------
-
-    >>> path = pr.get_example_path("control.bam")
+    >>> import pyranges as pr
+    >>> path = pr.example_data.files["smaller.bam"]
     >>> pr.read_bam(path)
-    +--------------+-----------+-----------+--------------+------------+
-    | Chromosome   | Start     | End       | Strand       | Flag       |
-    | (category)   | (int32)   | (int32)   | (category)   | (uint16)   |
-    |--------------+-----------+-----------+--------------+------------|
-    | chr1         | 887771    | 887796    | +            | 16         |
-    | chr1         | 994660    | 994685    | +            | 16         |
-    | chr1         | 1770383   | 1770408   | +            | 16         |
-    | chr1         | 1995141   | 1995166   | +            | 16         |
-    | ...          | ...       | ...       | ...          | ...        |
-    | chrY         | 57402214  | 57402239  | +            | 16         |
-    | chrY         | 10643526  | 10643551  | -            | 0          |
-    | chrY         | 11776321  | 11776346  | -            | 0          |
-    | chrY         | 20557165  | 20557190  | -            | 0          |
-    +--------------+-----------+-----------+--------------+------------+
-    Stranded PyRanges object has 10,000 rows and 5 columns from 25 chromosomes.
-    For printing, the PyRanges was sorted on Chromosome and Strand.
-
-    >>> pr.read_bam(path, sparse=False, as_df=True)
-         Chromosome    Start      End Strand  Flag  QueryStart  QueryEnd Name Cigar Quality
-    0          chr1   887771   887796      +    16           0        25   U0   25M    None
-    1          chr1   994660   994685      +    16           0        25   U0   25M    None
-    2          chr1  1041102  1041127      -     0           0        25   U0   25M    None
-    3          chr1  1770383  1770408      +    16           0        25   U0   25M    None
-    4          chr1  1995141  1995166      +    16           0        25   U0   25M    None
-    ...         ...      ...      ...    ...   ...         ...       ...  ...   ...     ...
-    9995       chrM     3654     3679      -     0           0        25   U0   25M    None
-    9996       chrM     3900     3925      +    16           0        25   U0   25M    None
-    9997       chrM    13006    13031      +    16           0        25   U0   25M    None
-    9998       chrM    14257    14282      -     0           0        25   U0   25M    None
-    9999       chrM    14257    14282      -     0           0        25   U0   25M    None
-    <BLANKLINE>
-    [10000 rows x 10 columns]
-    """
+    index    |    Chromosome    Start     End       Strand      Flag
+    int64    |    category      int64     int64     category    uint16
+    -------  ---  ------------  --------  --------  ----------  --------
+    0        |    chr1          887771    887796    -           16
+    1        |    chr1          994660    994685    -           16
+    2        |    chr1          1041102   1041127   +           0
+    3        |    chr1          1770383   1770408   -           16
+    ...      |    ...           ...       ...       ...         ...
+    96       |    chr1          18800901  18800926  +           0
+    97       |    chr1          18800901  18800926  +           0
+    98       |    chr1          18855123  18855148  -           16
+    99       |    chr1          19373470  19373495  +           0
+    PyRanges with 100 rows, 5 columns, and 1 index columns.
+    Contains 1 chromosomes and 2 strands.
 
+    """
+    path = Path(f)
     try:
-        import bamread
-    except ModuleNotFoundError as e:
-        print("bamread must be installed to read bam. Use `conda install -c bioconda bamread` or `pip install bamread` to install it.")
+        import bamread  # type: ignore[import]
+    except ImportError:
+        LOGGER.exception(
+            "bamread must be installed to read bam. Use `conda install -c bioconda bamread` or `pip install bamread` to install it.",
+        )
         sys.exit(1)
 
-    if sparse:
-        df = bamread.read_bam(f, mapq, required_flag, filter_flag)
-    else:
-        try:
-            df = bamread.read_bam_full(f, mapq, required_flag, filter_flag)
-        except AttributeError:
-            print("bamread version 0.0.6 or higher is required to read bam non-sparsely.")
-
-    if as_df:
-        return df
-    else:
-        return PyRanges(df)
-
-    # return bamread.read_bam(f, mapq, required_flag, filter_flag)
+    if bamread.__version__ in {
+        "0.0.1",
+        "0.0.2",
+        "0.0.3",
+        "0.0.4",
+        "0.0.5",
+        "0.0.6",
+        "0.0.7",
+        "0.0.8",
+        "0.0.9",
+    }:
+        LOGGER.exception(
+            "bamread not recent enough. Must be 0.0.10 or higher. Use `conda install -c bioconda 'bamread>=0.0.10'` or `pip install bamread>=0.0.10` to install it.",
+        )
+        sys.exit(1)
 
+    if sparse:
+        return mypy_ensure_pyranges(bamread.read_bam(path, mapq, required_flag, filter_flag))
+    df = bamread.read_bam_full(path, mapq, required_flag, filter_flag)
+    return mypy_ensure_pyranges(df)
 
-def _fetch_gene_transcript_exon_id(attribute, annotation=None):
 
-    no_quotes = attribute.str.replace('"', '').str.replace("'", "")
+def _fetch_gene_transcript_exon_id(attribute: pd.Series, annotation: str | None = None) -> pd.DataFrame:
+    no_quotes = attribute.str.replace('"', "").str.replace("'", "")
 
     df = no_quotes.str.extract(
         "gene_id.?(.+?);(?:.*transcript_id.?(.+?);)?(?:.*exon_number.?(.+?);)?(?:.*exon_id.?(.+?);)?",
-        expand=True)  # .iloc[:, [1, 2, 3]]
+        expand=True,
+    )  # .iloc[:, [1, 2, 3]]
 
-    df.columns = "gene_id transcript_id exon_number exon_id".split()
+    df.columns = pd.Index("gene_id transcript_id exon_number exon_id".split())
 
     if annotation == "ensembl":
-        newdf = []
+        newdfs = []
         for c in "gene_id transcript_id exon_id".split():
-            r = df[c].astype(str).str.extract(r'(\d+)').astype(float)
-            newdf.append(r)
+            r = df[c].astype(str).str.extract(r"(\d+)").astype(float)
+            newdfs.append(r)
 
-        newdf = pd.concat(newdf, axis=1)
+        newdf = pd.concat(newdfs, axis=1)
         newdf.insert(2, "exon_number", df["exon_number"])
         df = newdf
 
     return df
 
 
-def skiprows(f):
-
+def find_first_data_line_index(file_path: Path) -> int:
+    """Find the first line that is not a comment."""
+    first_non_comment = 0
     try:
         import gzip
-        fh = gzip.open(f)
-        for i, l in enumerate(fh):
-            if l.decode()[0] != "#":
+
+        zh = gzip.open(file_path)
+        for i, zl in enumerate(zh):
+            if zl.decode()[0] != "#":
+                first_non_comment = i
                 break
+        zh.close()
     except (OSError, TypeError):  # not a gzipped file, or StringIO
-        fh = open(f)
-        for i, l in enumerate(fh):
-            if l[0] != "#":
+        fh = file_path.open()
+        for i, line in enumerate(fh):
+            if line[0] != "#":
+                first_non_comment = i
                 break
+        fh.close()
 
-    fh.close()
-
-    return i
-
+    return first_non_comment
 
-def read_gtf(f, full=True, as_df=False, nrows=None, duplicate_attr=False):
 
-    """Read files in the Gene Transfer Format.
+def read_gtf(
+    f: str | Path,
+    /,
+    nrows: bool | None = None,
+    *,
+    full: bool = True,
+    duplicate_attr: bool = False,
+    ignore_bad: bool = False,
+) -> "PyRanges":
+    r"""Read files in the Gene Transfer Format.
 
     Parameters
     ----------
     f : str
-
         Path to GTF file.
 
-    as_df : bool, default False
-
-        Whether to return as pandas DataFrame instead of PyRanges.
+    full : bool, default True
+        Whether to read and interpret the annotation column.
 
     nrows : int, default None
-
         Number of rows to read. Default None, i.e. all.
 
     duplicate_attr : bool, default False
-
         Whether to handle (potential) duplicate attributes or just keep last one.
 
+    ignore_bad : bool, default False
+        Whether to ignore bad lines or raise an error.
+
+    Note
+    ----
+
+    The GTF format encodes both Start and End as 1-based included.
+    PyRanges encodes intervals as 0-based, Start included and End excluded.
+
     See Also
     --------
-
     pyranges.read_gff3 : read files in the General Feature Format
 
     Examples
     --------
+    >>> import pyranges as pr
+    >>> from tempfile import NamedTemporaryFile
+    >>> contents = ['#!genome-build GRCh38.p10']
+    >>> contents.append('1\thavana\tgene\t11869\t14409\t.\t+\t.\tgene_id "ENSG00000223972"; gene_version "5"; gene_name "DDX11L1"; gene_source "havana"; gene_biotype "transcribed_unprocessed_pseudogene";')
+    >>> contents.append('1\thavana\ttranscript\t11869\t14409\t.\t+\t.\tgene_id "ENSG00000223972"; gene_version "5"; transcript_id "ENST00000456328"; transcript_version "2"; gene_name "DDX11L1"; gene_source "havana"; gene_biotype "transcribed_unprocessed_pseudogene"; transcript_name "DDX11L1-202"; transcript_source "havana"; transcript_biotype "processed_transcript"; tag "basic"; transcript_support_level "1";')
+    >>> f = NamedTemporaryFile("w")
+    >>> _bytes_written = f.write("\n".join(contents))
+    >>> f.flush()
+    >>> pr.read_gtf(f.name)
+      index  |      Chromosome  Source    Feature       Start      End  Score     Strand      Frame     gene_id          ...
+      int64  |        category  object    category      int64    int64  object    category    object    object           ...
+    -------  ---  ------------  --------  ----------  -------  -------  --------  ----------  --------  ---------------  -----
+          0  |               1  havana    gene          11868    14409  .         +           .         ENSG00000223972  ...
+          1  |               1  havana    transcript    11868    14409  .         +           .         ENSG00000223972  ...
+    PyRanges with 2 rows, 20 columns, and 1 index columns. (11 columns not shown: "gene_version", "gene_name", "gene_source", ...).
+    Contains 1 chromosomes and 1 strands.
 
-    >>> path = pr.get_example_path("ensembl.gtf")
-    >>> gr = pr.read_gtf(path)
-
-    >>> # +--------------+------------+--------------+-----------+-----------+------------+--------------+------------+-----------------+----------------+-------+
-    >>> # | Chromosome   | Source     | Feature      | Start     | End       | Score      | Strand       | Frame      | gene_id         | gene_version   | +18   |
-    >>> # | (category)   | (object)   | (category)   | (int32)   | (int32)   | (object)   | (category)   | (object)   | (object)        | (object)       | ...   |
-    >>> # |--------------+------------+--------------+-----------+-----------+------------+--------------+------------+-----------------+----------------+-------|
-    >>> # | 1            | havana     | gene         | 11868     | 14409     | .          | +            | .          | ENSG00000223972 | 5              | ...   |
-    >>> # | 1            | havana     | transcript   | 11868     | 14409     | .          | +            | .          | ENSG00000223972 | 5              | ...   |
-    >>> # | 1            | havana     | exon         | 11868     | 12227     | .          | +            | .          | ENSG00000223972 | 5              | ...   |
-    >>> # | 1            | havana     | exon         | 12612     | 12721     | .          | +            | .          | ENSG00000223972 | 5              | ...   |
-    >>> # | ...          | ...        | ...          | ...       | ...       | ...        | ...          | ...        | ...             | ...            | ...   |
-    >>> # | 1            | ensembl    | transcript   | 120724    | 133723    | .          | -            | .          | ENSG00000238009 | 6              | ...   |
-    >>> # | 1            | ensembl    | exon         | 133373    | 133723    | .          | -            | .          | ENSG00000238009 | 6              | ...   |
-    >>> # | 1            | ensembl    | exon         | 129054    | 129223    | .          | -            | .          | ENSG00000238009 | 6              | ...   |
-    >>> # | 1            | ensembl    | exon         | 120873    | 120932    | .          | -            | .          | ENSG00000238009 | 6              | ...   |
-    >>> # +--------------+------------+--------------+-----------+-----------+------------+--------------+------------+-----------------+----------------+-------+
-    >>> # Stranded PyRanges object has 95 rows and 28 columns from 1 chromosomes.
-    >>> # For printing, the PyRanges was sorted on Chromosome and Strand.
-    >>> # 18 hidden columns: gene_name, gene_source, gene_biotype, transcript_id, transcript_version, transcript_name, transcript_source, transcript_biotype, tag, transcript_support_level, ... (+ 8 more.)
     """
+    path = Path(f)
+    _skiprows = find_first_data_line_index(path)
 
-    _skiprows = skiprows(f)
-
-    gr = read_gtf_full(f, as_df, nrows, _skiprows, duplicate_attr)
+    if full:
+        gr = read_gtf_full(
+            path,
+            nrows=nrows,
+            skiprows=_skiprows,
+            duplicate_attr=duplicate_attr,
+            ignore_bad=ignore_bad,
+        )
+    else:
+        gr = read_gtf_restricted(path, _skiprows, nrows=None)
 
     return gr
 
 
-def read_gtf_full(f, as_df=False, nrows=None, skiprows=0, duplicate_attr=False):
+def read_gtf_full(
+    f: str | Path,
+    /,
+    nrows: int | None = None,
+    skiprows: int = 0,
+    chunksize: int = int(1e5),  # for unit-testing purposes
+    *,
+    duplicate_attr: bool = False,
+    ignore_bad: bool = False,
+) -> "PyRanges":
+    """Read files in the Gene Transfer Format.
 
-    dtypes = {
-        "Chromosome": "category",
-        "Feature": "category",
-        "Strand": "category"
-    }
+    Parameters
+    ----------
+    f : str
+        Path to GTF file.
 
-    names = "Chromosome Source Feature Start End Score Strand Frame Attribute".split(
-    )
+    nrows : int, default None
+        Number of rows to read. Default None, i.e. all.
+
+    skiprows : int, default 0
+        Number of rows to skip. Default 0.
+
+    chunksize : int, default 100000
+        Number of rows to read at a time. Default 100000.
+
+    duplicate_attr : bool, default False
+        Whether to handle (potential) duplicate attributes or just keep last one.
+
+    ignore_bad : bool, default False
+        Whether to ignore bad lines or raise an error.
+
+    """
+    dtypes = {"Chromosome": "category", "Feature": "category", "Strand": "category"}
+
+    names = "Chromosome Source Feature Start End Score Strand Frame Attribute".split()
+    path = Path(f)
 
     df_iter = pd.read_csv(
-        f,
+        path,
         sep="\t",
         header=None,
         names=names,
         dtype=dtypes,
-        chunksize=int(1e5),
+        chunksize=chunksize,
         skiprows=skiprows,
-        nrows=nrows)
+        nrows=nrows,
+    )
 
     _to_rows = to_rows_keep_duplicates if duplicate_attr else to_rows
 
     dfs = []
     for df in df_iter:
-        extra = _to_rows(df.Attribute)
-        df = df.drop("Attribute", axis=1)
-        ndf = pd.concat([df, extra], axis=1, sort=False)
+        extra = _to_rows(df.Attribute.astype(str), ignore_bad=ignore_bad)
+        _df = df.drop("Attribute", axis=1)
+        extra = extra.set_index(_df.index)
+        ndf = pd.concat([_df, extra], axis=1, sort=False)
         dfs.append(ndf)
 
     df = pd.concat(dfs, sort=False)
     df.loc[:, "Start"] = df.Start - 1
 
-    if not as_df:
-        return PyRanges(df)
-    else:
-        return df
+    return mypy_ensure_pyranges(df)
 
 
-def to_rows(anno):
-    rowdicts = []
+def parse_kv_fields(line: str) -> list[list[str]]:
+    """Parse GTF attribute column."""
+    return [kv.replace('""', '"NA"').replace('"', "").split(None, 1) for kv in line.rstrip("; ").split("; ")]
+
+
+def to_rows(anno: pd.Series, *, ignore_bad: bool = False) -> pd.DataFrame:
+    """Parse GTF attribute column into a dataframe of attribute columns."""
+    entry = ""
     try:
-        l = anno.head(1)
-        for l in l:
-            l.replace('"', '').replace(";", "").split()
+        row = anno.head(1)
+        for entry in row:
+            str(entry).replace('"', "").replace(";", "").split()
     except AttributeError:
-        raise Exception("Invalid attribute string: {l}. If the file is in GFF3 format, use pr.read_gff3 instead.".format(l=l))
+        msg = f"Invalid attribute string: {entry}. If the file is in GFF3 format, use pr.read_gff3 instead."
+        raise AttributeError(msg) from AttributeError
+
+    rowdicts = []
+    line = ""
+    try:
+        for line in anno:
+            rowdicts.append(dict(parse_kv_fields(line)))  # noqa: PERF401
+    except ValueError:
+        if not ignore_bad:
+            LOGGER.exception(
+                "The following line is not parseable as gtf:\n%s\n\nTo ignore bad lines use ignore_bad=True.",
+                line,
+            )
+            raise
 
-    for l in anno:
-        rowdicts.append({k: v
-                         for k, v in [kv.replace('"', '').split(None, 1)
-                                      # l[:-1] removes final ";" cheaply
-                                      for kv in l[:-1].split("; ")]})
+    return pd.DataFrame.from_records(rowdicts)
 
-    # for l in anno:
-    #     l = l.replace('"', '').replace(";", "").split()
-    #     rowdicts.append({k: v for k, v in zip(*([iter(l)] * 2))})
 
-    return pd.DataFrame.from_dict(rowdicts).set_index(anno.index)
+def to_rows_keep_duplicates(anno: pd.Series, *, ignore_bad: bool = False) -> pd.DataFrame:
+    """If an entry is found multiple times in the attribute string, keep all of them.
 
+    Examples
+    --------
+    >>> anno = pd.Series(["gene DDX11L1; gene sonic; unique hi"])
+    >>> result = to_rows_keep_duplicates(anno)
+    >>> result.to_dict(orient="records")
+    [{'gene': 'DDX11L1,sonic', 'unique': 'hi'}]
 
-def to_rows_keep_duplicates(anno):
+    """
     rowdicts = []
-    for l in anno:
-        rowdict = {}
+    line = ""
+    try:
+        for line in anno:
+            rowdict = {}
+
+            # rstrip: allows for GFF not having a last ";", or having final spaces
+            for k, v in tuple(parse_kv_fields(line)):
+                if k not in rowdict:
+                    rowdict[k] = [v]
+                else:
+                    rowdict[k].append(v)
+
+            rowdicts.append({k: ",".join(v) if isinstance(v, list) else v for k, v in rowdict.items()})
+    except ValueError:
+        if not ignore_bad:
+            LOGGER.exception(
+                "The following line is not parseable as gtf:\n\n%s\n\nTo ignore bad lines use ignore_bad=True.",
+                line,
+            )
+
+    return pd.DataFrame.from_records(rowdicts)
+
 
-        # l[:-1] removes final ";" cheaply
-        for k, v in (kv.replace('"', '').split(None, 1) for kv in l[:-1].split("; ")):
+def read_gtf_restricted(f: str | Path, skiprows: int | None, nrows: int | None = None) -> "PyRanges":
+    """Read certain columns from GTF file.
 
-            if k not in rowdict:
-                rowdict[k] = v
-            elif k in rowdict and isinstance(rowdict[k], list):
-                rowdict[k].append(v)
-            else:
-                rowdict[k] = [rowdict[k], v]
-
-        rowdicts.append({
-            k: ','.join(v) if isinstance(v, list) else v
-            for k, v in rowdict.items()
-        })
-
-    return pd.DataFrame.from_dict(rowdicts).set_index(anno.index)
-
-
-def read_gtf_restricted(f,
-                        as_df=False,
-                        skiprows=0,
-                        nrows=None):
-    """seqname - name of the chromosome or scaffold; chromosome names can be given with or without the 'chr' prefix. Important note: the seqname must be one used within Ensembl, i.e. a standard chromosome name or an Ensembl identifier such as a scaffold ID, without any additional content such as species or assembly. See the example GFF output below.
+    Seqname - name of the chromosome or scaffold; chromosome names can be given with or without the 'chr' prefix. Important note: the seqname must be one used within Ensembl, i.e. a standard chromosome name or an Ensembl identifier such as a scaffold ID, without any additional content such as species or assembly. See the example GFF output below.
     # source - name of the program that generated this feature, or the data source (database or project name)
     feature - feature type name, e.g. Gene, Variation, Similarity
     start - Start position of the feature, with sequence numbering starting at 1.
     end - End position of the feature, with sequence numbering starting at 1.
     score - A floating point value.
     strand - defined as + (forward) or - (reverse).
     # frame - One of '0', '1' or '2'. '0' indicates that the first base of the feature is the first base of a codon, '1' that the second base is the first base of a codon, and so on..
-    attribute - A semicolon-separated list of tag-value pairs, providing additional information about each feature."""
-    dtypes = {
-        "Chromosome": "category",
-        "Feature": "category",
-        "Strand": "category"
-    }
+    attribute - A semicolon-separated list of tag-value pairs, providing additional information about each feature.
+    """
+    dtypes = {"Chromosome": "category", "Feature": "category", "Strand": "category"}
+    path = Path(f)
 
     df_iter = pd.read_csv(
-        f,
+        path,
         sep="\t",
         comment="#",
         usecols=[0, 2, 3, 4, 5, 6, 8],
         header=None,
         names="Chromosome Feature Start End Score Strand Attribute".split(),
         dtype=dtypes,
         chunksize=int(1e5),
-        nrows=nrows)
+        skiprows=skiprows if skiprows is not None else False,
+        nrows=nrows,
+    )
 
     dfs = []
     for df in df_iter:
-        # Since Start is 1-indexed
-        df.Start -= 1
-
         if sum(df.Score == ".") == len(df):
             cols_to_concat = "Chromosome Start End Strand Feature".split()
         else:
-            cols_to_concat = "Chromosome Start End Strand Feature Score".split(
-            )
+            cols_to_concat = "Chromosome Start End Strand Feature Score".split()
 
         extract = _fetch_gene_transcript_exon_id(df.Attribute)
-        extract.columns = "gene_id transcript_id exon_number exon_id".split()
+        extract.columns = pd.Index("gene_id transcript_id exon_number exon_id".split())
 
         extract.exon_number = extract.exon_number.astype(float)
 
-        df = pd.concat([df[cols_to_concat], extract], axis=1, sort=False)
+        extract = extract.set_index(df.index)
+        _df = pd.concat([df[cols_to_concat], extract], axis=1, sort=False)
 
-        dfs.append(df)
+        dfs.append(_df)
 
     df = pd.concat(dfs, sort=False)
 
     df.loc[:, "Start"] = df.Start - 1
 
-    if not as_df:
-        return PyRanges(df)
-    else:
-        return df
+    return mypy_ensure_pyranges(df)
 
 
-def to_rows_gff3(anno):
-    rowdicts = []
+def to_rows_gff3(anno: pd.Series) -> pd.DataFrame:
+    """Parse GFF3 attribute column into a dataframe of attribute columns."""
+    rowdicts = [to_keys_and_values(line) for line in list(anno)]
 
-    for l in list(anno):
-        l = (it.split("=") for it in l.split(";"))
-        rowdicts.append({k: v for k, v in l})
+    return pd.DataFrame.from_records(rowdicts).set_index(anno.index)
 
-    return pd.DataFrame.from_dict(rowdicts).set_index(anno.index)
 
+def to_keys_and_values(line: str) -> dict[str, str]:
+    """Parse GFF3 attribute column."""
+    return dict(it.split("=") for it in line.rstrip("; ").split(";"))
 
-def read_gff3(f, annotation=None, as_df=False, nrows=None, skiprows=0):
 
+def read_gff3(
+    f: str | Path,
+    nrows: int | None = None,
+    *,
+    full: bool = True,
+) -> "PyRanges":
     """Read files in the General Feature Format.
 
     Parameters
     ----------
     f : str
-
         Path to GFF file.
 
-    as_df : bool, default False
-
-        Whether to return as pandas DataFrame instead of PyRanges.
+    full : bool, default True
+        Whether to read and interpret the annotation column.
 
     nrows : int, default None
-
         Number of rows to read. Default None, i.e. all.
 
+    Notes
+    -----
+    The gff3 format encodes both Start and End as 1-based included.
+    PyRanges (and also the DF returned by this function, if as_df=True), instead
+    encodes intervals as 0-based, Start included and End excluded.
+
     See Also
     --------
-
     pyranges.read_gtf : read files in the Gene Transfer Format
+
     """
+    path = Path(f)
+    _skiprows = find_first_data_line_index(path)
 
+    if not full:
+        return read_gtf_restricted(path, _skiprows, nrows=nrows)
 
-    dtypes = {
-        "Chromosome": "category",
-        "Feature": "category",
-        "Strand": "category"
-    }
+    dtypes = {"Chromosome": "category", "Feature": "category", "Strand": "category"}
 
-    names = "Chromosome Source Feature Start End Score Strand Frame Attribute".split(
-    )
+    names = "Chromosome Source Feature Start End Score Strand Frame Attribute".split()
 
     df_iter = pd.read_csv(
-        f,
+        path,
         comment="#",
         sep="\t",
         header=None,
         names=names,
         dtype=dtypes,
         chunksize=int(1e5),
-        skiprows=skiprows,
-        nrows=nrows)
+        skiprows=_skiprows,
+        nrows=nrows,
+    )
 
     dfs = []
     for df in df_iter:
         extra = to_rows_gff3(df.Attribute.astype(str))
-        df = df.drop("Attribute", axis=1)
-        ndf = pd.concat([df, extra], axis=1, sort=False)
+        _df = df.drop("Attribute", axis=1)
+        extra = extra.set_index(_df.index)
+        ndf = pd.concat([_df, extra], axis=1, sort=False)
         dfs.append(ndf)
 
     df = pd.concat(dfs, sort=False)
 
     df.loc[:, "Start"] = df.Start - 1
 
-    if not as_df:
-        return PyRanges(df)
-    else:
-        return df
-
+    return mypy_ensure_pyranges(df)
 
-def read_bigwig(f, as_df=False):
 
+def read_bigwig(f: str | Path) -> "PyRanges":
+    """Read bigwig files into a PyRanges."""
     try:
-        import pyBigWig
+        import pyBigWig  # type: ignore[import]
     except ModuleNotFoundError:
-        print("bwread must be installed to read bigwigs. Use `conda install -c bioconda bwread` or `pip install bwread` to install it.")
-        import sys
+        LOGGER.exception(
+            "bwread must be installed to read bigwigs. Use `conda install -c bioconda bwread` or `pip install bwread` to install it.",
+        )
         sys.exit(1)
 
     """Read bigwig files.
 
     Parameters
     ----------
     f : str
@@ -544,17 +627,16 @@
     --------
 
     >>> f = pr.get_example_path("bw.bw")
     >>> gr = pr.read_bigwig(f)
     >>> gr
     """
 
-    from natsort import natsorted
-
-    bw = pyBigWig.open(f)
+    path = Path(f)
+    bw = pyBigWig.open(path)
 
     size = int(1e5)
     chromosomes = bw.chroms()
 
     dfs = {}
 
     for chromosome in natsorted(chromosomes):
@@ -563,21 +645,28 @@
         outvalues = []
 
         length = chromosomes[chromosome]
 
         starts = list(range(0, length, size))
         ends = list(range(size, length + size, size))
         ends[-1] = length
-        for start, end in zip(starts, ends):
+        for start, end in zip(starts, ends, strict=True):
             intervals = bw.intervals(chromosome, start, end)
             if intervals is not None:
                 for s, e, v in intervals:
                     outstarts.append(s)
                     outends.append(e)
                     outvalues.append(v)
 
         outstarts = pd.Series(outstarts)
         outends = pd.Series(outends)
         outvalues = pd.Series(outvalues)
-        dfs[chromosome] = pd.DataFrame({"Chromosome": chromosome, "Start": outstarts, "End": outends, "Value": outvalues})
+        dfs[chromosome] = pd.DataFrame(
+            {
+                "Chromosome": chromosome,
+                "Start": outstarts,
+                "End": outends,
+                "Value": outvalues,
+            },
+        )
 
-    return pr.PyRanges(dfs)
+    return mypy_ensure_pyranges(pd.concat(dfs))
```

### Comparing `pyranges-0.0.99/pyranges/statistics.py` & `pyranges-0.1.0/pyranges/ext/stats.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,476 +1,539 @@
 """Statistics useful for genomics."""
 
-import pandas as pd
+import logging
+import sys
+from collections import defaultdict
+from collections.abc import Iterable
+from itertools import combinations_with_replacement
+from math import sqrt
+from typing import TYPE_CHECKING, Any
+
 import numpy as np
+import pandas as pd
+from numpy import ndarray
+from pandas import DataFrame, Series
 
 import pyranges as pr
-from pyranges.multithreaded import pyrange_apply
-
+from pyranges.core.names import (
+    CHROM_COL,
+    END_COL,
+    GENOME_LOC_COLS,
+    STRAND_BEHAVIOR_IGNORE,
+    STRAND_BEHAVIOR_SAME,
+    VALID_STRAND_BEHAVIOR_TYPE,
+)
+from pyranges.core.pyranges_helpers import (
+    mypy_ensure_pyranges,
+    strand_behavior_from_validated_use_strand,
+    use_strand_from_validated_strand_behavior,
+    validate_and_convert_strand_behavior,
+)
 from pyranges.methods.statistics import _relative_distance
 
-from collections import defaultdict
+if TYPE_CHECKING:
+    from numpy.typing import NDArray
+
+    from pyranges import PyRanges
+
+logging.basicConfig(level=logging.INFO)
+LOGGER = logging.getLogger(__name__)
+LOGGER.setLevel(logging.INFO)
+
+
+####################################################################################################
+# methods and objects that are not exported
+GenomeType = dict[str, int] | pd.DataFrame | None
+LabelsType = list[str] | list[int]
+
+
+def _chromsizes_as_int(chromsizes: "PyRanges | DataFrame | dict[Any, int]") -> int:
+    if isinstance(chromsizes, dict):
+        _chromsizes = sum(chromsizes.values())
+    elif isinstance(chromsizes, pd.DataFrame | pr.PyRanges):
+        _chromsizes = chromsizes.End.sum()
+    else:
+        msg = f"chromsizes must be dict, DataFrame or PyRanges, was {type(chromsizes)}"
+        raise TypeError(msg)
+
+    return _chromsizes
+
+
+def _mcc(tp: int, fp: int, tn: int, fn: int) -> float:
+    # https://stackoverflow.com/a/56875660/992687
+    x = (tp + fp) * (tp + fn) * (tn + fp) * (tn + fn)
+    return ((tp * tn) - (fp * fn)) / sqrt(x)
+
+
+def _process_genome_data(grs: list[Any], genome: GenomeType, labels: LabelsType) -> tuple[pd.DataFrame, int, Iterable]:
+    _genome = _find_chromosome_max_end_positions(grs) if genome is None else _ensure_genome_dataframe(genome)
+
+    genome_length = _compute_genome_length(_genome)
+
+    _labels = (
+        _generate_labels(labels, grs) if labels is not None else combinations_with_replacement(np.arange(len(grs)), r=2)
+    )
+
+    return _genome, genome_length, _labels
+
+
+def _ensure_genome_dataframe(genome: GenomeType) -> pd.DataFrame:
+    if isinstance(genome, dict):
+        return _create_genome_dataframe(genome)
+
+    if isinstance(genome, pd.DataFrame):
+        return genome
+
+    msg = f"genome must be dict or DataFrame, was {type(genome)}"
+    raise TypeError(msg)
+
+
+def _find_chromosome_max_end_positions(grs: list["PyRanges"]) -> pd.DataFrame:
+    """Find the largest end position in each chromosome.
+
+    Examples
+    --------
+    >>> f1, f2 = pr.example_data.f1, pr.example_data.f2  # both only have chr1
+    >>> f1["End"].max()
+    9
+    >>> f2["End"].max()
+    7
+
+    """
+    genome: dict[str, int] = defaultdict(int)
+    for gr in grs:
+        for chrom, chrom_df in gr.groupby(CHROM_COL):
+            genome[chrom] = max(chrom_df[END_COL].max(), genome[chrom])
+    return _create_genome_dataframe(dict(genome))
+
+
+def _create_genome_dataframe(genome: dict[str, int]) -> pd.DataFrame:
+    return pd.DataFrame({"Chromosome": list(genome.keys()), "Start": 0, "End": list(genome.values())})
+
 
-__all__ = ["simes", "fisher_exact", "StatisticsMethods", "fdr", "rowbased_rankdata", "rowbased_pearson", "rowbased_spearman", "mcc"]
+def _compute_genome_length(genome: pd.DataFrame) -> int:
+    return int(genome[END_COL].sum())
 
-def fdr(p_vals):
 
+def _generate_labels(labels: LabelsType, grs: list[Any]) -> Iterable:
+    if len(labels) != len(grs):
+        msg = "Labels length must match the length of grs"
+        raise ValueError(msg)
+    return combinations_with_replacement(labels, r=2)
+
+
+def fdr(p_vals: Series) -> Series:
     """Adjust p-values with Benjamini-Hochberg.
 
     Parameters
     ----------
-    data : array-like
-
+    p_vals : array-like
+           P-values to adjust.
 
     Returns
     -------
     Pandas.DataFrame
 
         DataFrame where values are order of data.
 
     Examples
     --------
+    >>> import pyranges as pr
+    >>> d = {'Chromosome': ['chr3', 'chr6', 'chr13'], 'Start': [146419383, 39800100, 24537618], 'End': [146419483, 39800200, 24537718], 'Strand': ['-', '+', '-'], 'PValue': [0.0039591368855297175, 0.0037600512992788937, 0.0075061166500909205]}
+    >>> gr = pr.PyRanges(d)
+    >>> gr
+      index  |    Chromosome        Start        End  Strand        PValue
+      int64  |    object            int64      int64  object       float64
+    -------  ---  ------------  ---------  ---------  --------  ----------
+          0  |    chr3          146419383  146419483  -         0.00395914
+          1  |    chr6           39800100   39800200  +         0.00376005
+          2  |    chr13          24537618   24537718  -         0.00750612
+    PyRanges with 3 rows, 5 columns, and 1 index columns.
+    Contains 3 chromosomes and 2 strands.
 
-    >>> np.random.seed(0)
-    >>> x = np.random.random(10) / 100
-
-    >>> gr = pr.random(10)
-    >>> gr.PValue = x
+    >>> gr["FDR"] = pr.stats.fdr(gr.PValue)
     >>> gr
-    +--------------+-----------+-----------+--------------+----------------------+
-    | Chromosome   | Start     | End       | Strand       | PValue               |
-    | (category)   | (int32)   | (int32)   | (category)   | (float64)            |
-    |--------------+-----------+-----------+--------------+----------------------|
-    | chr1         | 176601938 | 176602038 | +            | 0.005488135039273248 |
-    | chr1         | 155082851 | 155082951 | -            | 0.007151893663724195 |
-    | chr2         | 211134424 | 211134524 | -            | 0.006027633760716439 |
-    | chr9         | 78826761  | 78826861  | -            | 0.005448831829968969 |
-    | ...          | ...       | ...       | ...          | ...                  |
-    | chr16        | 52216522  | 52216622  | +            | 0.004375872112626925 |
-    | chr17        | 8085927   | 8086027   | -            | 0.008917730007820798 |
-    | chr19        | 17333425  | 17333525  | +            | 0.009636627605010294 |
-    | chr22        | 16728001  | 16728101  | +            | 0.003834415188257777 |
-    +--------------+-----------+-----------+--------------+----------------------+
-    Stranded PyRanges object has 10 rows and 5 columns from 9 chromosomes.
-    For printing, the PyRanges was sorted on Chromosome and Strand.
-
-    >>> gr.FDR = pr.stats.fdr(gr.PValue)
-    >>> gr.print(formatting={"PValue": "{:.4f}", "FDR": "{:.4}"})
-    +--------------+-----------+-----------+--------------+-------------+-------------+
-    | Chromosome   | Start     | End       | Strand       | PValue      | FDR         |
-    | (category)   | (int32)   | (int32)   | (category)   | (float64)   | (float64)   |
-    |--------------+-----------+-----------+--------------+-------------+-------------|
-    | chr1         | 176601938 | 176602038 | +            | 0.0055      | 0.01098     |
-    | chr1         | 155082851 | 155082951 | -            | 0.0072      | 0.00894     |
-    | chr2         | 211134424 | 211134524 | -            | 0.0060      | 0.01005     |
-    | chr9         | 78826761  | 78826861  | -            | 0.0054      | 0.01362     |
-    | ...          | ...       | ...       | ...          | ...         | ...         |
-    | chr16        | 52216522  | 52216622  | +            | 0.0044      | 0.01459     |
-    | chr17        | 8085927   | 8086027   | -            | 0.0089      | 0.009909    |
-    | chr19        | 17333425  | 17333525  | +            | 0.0096      | 0.009637    |
-    | chr22        | 16728001  | 16728101  | +            | 0.0038      | 0.03834     |
-    +--------------+-----------+-----------+--------------+-------------+-------------+
-    Stranded PyRanges object has 10 rows and 6 columns from 9 chromosomes.
-    For printing, the PyRanges was sorted on Chromosome and Strand.
+      index  |    Chromosome        Start        End  Strand        PValue         FDR
+      int64  |    object            int64      int64  object       float64     float64
+    -------  ---  ------------  ---------  ---------  --------  ----------  ----------
+          0  |    chr3          146419383  146419483  -         0.00395914  0.00593871
+          1  |    chr6           39800100   39800200  +         0.00376005  0.0112802
+          2  |    chr13          24537618   24537718  -         0.00750612  0.00750612
+    PyRanges with 3 rows, 6 columns, and 1 index columns.
+    Contains 3 chromosomes and 2 strands.
+
     """
+    from scipy.stats import rankdata  # type: ignore[import]
 
-    from scipy.stats import rankdata
     ranked_p_values = rankdata(p_vals)
     fdr = p_vals * len(p_vals) / ranked_p_values
     fdr[fdr > 1] = 1
 
     return fdr
 
 
-def fisher_exact(tp, fp, fn, tn, pseudocount=0):
-
+def fisher_exact(tp: Series, fp: Series, fn: Series, tn: Series, pseudocount: int = 0) -> DataFrame:
     """Fisher's exact for contingency tables.
 
     Computes the hypotheses two-sided, less and greater at the same time.
 
     The odds-ratio is
 
     Parameters
     ----------
     tp : array-like of int
-
         Top left square of contingency table (true positives).
 
     fp : array-like of int
-
         Top right square of contingency table (false positives).
 
     fn : array-like of int
-
         Bottom left square of contingency table (false negatives).
 
     tn : array-like of int
-
         Bottom right square of contingency table (true negatives).
 
     pseudocount : float, default 0
-
         Values > 0 allow Odds Ratio to always be a finite number.
 
     Notes
     -----
-
     The odds-ratio is computed thusly:
 
     ``((tp + pseudocount) / (fp + pseudocount)) / ((fn + pseudocount) / (tn + pseudocount))``
 
     Returns
     -------
     pandas.DataFrame
 
-        DataFrame with columns OR and P, PLeft and PRight.
+        DataFrame with columns odds_ratio and P, PLeft and PRight.
 
     See Also
     --------
-
     pr.stats.fdr : correct for multiple testing
 
     Examples
     --------
-
     >>> d = {"TP": [12, 0], "FP": [5, 12], "TN": [29, 10], "FN": [2, 2]}
     >>> df = pd.DataFrame(d)
     >>> df
        TP  FP  TN  FN
     0  12   5  29   2
     1   0  12  10   2
 
     >>> pr.stats.fisher_exact(df.TP, df.FP, df.TN, df.FN)
-             OR         P     PLeft    PRight
-    0  0.165517  0.080269  0.044555  0.994525
-    1  0.000000  0.000067  0.000034  1.000000
-    """
-
+       odds_ratio         P     PLeft    PRight
+    0    0.165517  0.080269  0.044555  0.994525
+    1    0.000000  0.000067  0.000034  1.000000
 
+    """
     try:
-        from fisher import pvalue_npy
-    except:
-        import sys
-        print("fisher needs to be installed to use fisher exact. pip install fisher or conda install -c bioconda fisher.")
+        from fisher import pvalue_npy  # type: ignore[import]
+    except ImportError:
+        LOGGER.exception(
+            "fisher needs to be installed to use fisher exact. pip install fisher or conda install -c bioconda fisher.",
+        )
         sys.exit(-1)
 
-    tp = np.array(tp, dtype=np.uint)
-    fp = np.array(fp, dtype=np.uint)
-    fn = np.array(fn, dtype=np.uint)
-    tn = np.array(tn, dtype=np.uint)
-
-    left, right, twosided = pvalue_npy(tp, fp, fn, tn)
+    _tp = np.array(tp, dtype=np.uint)
+    _fp = np.array(fp, dtype=np.uint)
+    _fn = np.array(fn, dtype=np.uint)
+    _tn = np.array(tn, dtype=np.uint)
 
-    OR = ((tp + pseudocount) / (fp + pseudocount)) / ((fn + pseudocount) / (tn + pseudocount))
+    left, right, twosided = pvalue_npy(_tp, _fp, _fn, _tn)
 
-    df = pd.DataFrame({"OR": OR, "P": twosided, "PLeft": left, "PRight": right})
+    odds_ratio = ((_tp + pseudocount) / (_fp + pseudocount)) / ((_fn + pseudocount) / (_tn + pseudocount))
 
-    return df
+    return pd.DataFrame({"odds_ratio": odds_ratio, "P": twosided, "PLeft": left, "PRight": right})
 
 
-def mcc(grs, genome=None, labels=None, strand=False, verbose=False):
-
+def mcc(
+    grs: list["PyRanges"],
+    *,
+    labels: list[str],
+    genome: "PyRanges | pd.DataFrame | dict[str, int] | None" = None,
+    use_strand: bool = False,
+) -> DataFrame:
     """Compute Matthew's correlation coefficient for PyRanges overlaps.
 
     Parameters
     ----------
     grs : list of PyRanges
-
         PyRanges to compare.
 
     genome : DataFrame or dict, default None
-
         Should contain chromosome sizes. By default, end position of the
         rightmost intervals are used as proxies for the chromosome size, but
         it is recommended to use a genome.
 
     labels : list of str, default None
-
         Names to give the PyRanges in the output.
 
-    strand : bool, default False
-
+    use_strand : bool, default False
         Whether to compute correlations per strand.
 
-    verbose : bool, default False
-
-        Warn if some chromosomes are in the genome, but not in the PyRanges.
-
     Examples
     --------
-    >>> np.random.seed(0)
-    >>> chromsizes = {"chrM": 16000}
-    >>> grs = [pr.random(chromsizes=chromsizes) for _ in range(3)]
-    >>> labels = ["a", "b", "c"]
-    >>> mcc = pr.stats.mcc(grs, labels=labels, genome=chromsizes)
+    >>> grs = [pr.example_data.aorta, pr.example_data.aorta, pr.example_data.aorta2]
+    >>> mcc = pr.stats.mcc(grs, labels="abc", genome={"chr1": 2100000})
     >>> mcc
-       T  F     TP  FP  TN  FN       MCC
-    0  a  a  15920   0  80   0  1.000000
-    1  a  b  15875  65  15  45  0.213109
-    3  a  c  15896  72   8  24  0.155496
-    2  b  a  15875  45  15  65  0.213109
-    5  b  b  15940   0  60   0  1.000000
-    6  b  c  15916  52   8  24  0.180354
-    4  c  a  15896  24   8  72  0.155496
-    7  c  b  15916  24   8  52  0.180354
-    8  c  c  15968   0  32   0  1.000000
+       T  F   TP   FP       TN   FN      MCC
+    0  a  a  728    0  2099272    0  1.00000
+    1  a  b  728    0  2099272    0  1.00000
+    3  a  c  457  485  2098787  271  0.55168
+    2  b  a  728    0  2099272    0  1.00000
+    5  b  b  728    0  2099272    0  1.00000
+    6  b  c  457  485  2098787  271  0.55168
+    4  c  a  457  271  2098787  485  0.55168
+    7  c  b  457  271  2098787  485  0.55168
+    8  c  c  942    0  2099058    0  1.00000
 
     To create a symmetric matrix (useful for heatmaps of correlations):
 
-    >>> mcc.set_index(["T", "F"]).MCC.unstack()
-    F         a         b         c
-    T
-    a  1.000000  0.213109  0.155496
-    b  0.213109  1.000000  0.180354
-    c  0.155496  0.180354  1.000000"""
-
-    import sys
-    from itertools import combinations_with_replacement, chain
-
-    if labels is None:
-        _labels = list(range(len(grs)))
-        _labels = combinations_with_replacement(_labels, r=2)
-    else:
-        assert len(labels) == len(grs)
-        _labels = combinations_with_replacement(labels, r=2)
-
-    # remove all non-loc columns before computation
-    grs = [gr.merge(strand=strand) for gr in grs]
+    >>> mcc.set_index(["T", "F"]).MCC.unstack().rename_axis(None, axis=0)
+    F        a        b        c
+    a  1.00000  1.00000  0.55168
+    b  1.00000  1.00000  0.55168
+    c  0.55168  0.55168  1.00000
 
-    if genome is not None:
-        if isinstance(genome, (pd.DataFrame, pr.PyRanges)):
-            genome_length = int(genome.End.sum())
-        else:
-            genome_length = sum(genome.values())
-
-        if verbose:
-            # check that genome definition does not have many more
-            # chromosomes than datafiles
-            gr_cs = set(chain(*[gr.chromosomes for gr in grs]))
-
-            g_cs = set(genome.chromosomes)
-            surplus = g_cs - gr_cs
-            if len(surplus):
-                print("The following chromosomes are in the genome, but not the PyRanges:", ", ".join(surplus), file=sys.stderr)
-
-        if strand:
-            def make_stranded(df):
-                df = df.copy()
-                df2 = df.copy()
-                df.insert(df.shape[1], "Strand", "+")
-                df2.insert(df2.shape[1], "Strand", "-")
-                return pd.concat([df, df2])
-
-            genome = genome.apply(make_stranded)
+    """
+    _genome, genome_length, _labels = _process_genome_data(grs, labels=labels, genome=genome)
 
-    else:
-        d = defaultdict(int)
-        for gr in grs:
-            for k, v in gr:
-                d[k] = max(d[k], v.End.max())
+    if use_strand and not all(gr.strand_valid for gr in grs):
+        msg = "use_strand=True but one or more PyRanges have invalid strand information."
+        raise AssertionError(msg)
 
-        genome_length = sum(d.values())
+    # remove all non-loc columns before computation
+    grs = [gr.merge_overlaps(use_strand=use_strand) for gr in grs]
 
-    strandedness = "same" if strand else None
+    strand_behavior_same = all(
+        strand_behavior_from_validated_use_strand(gr, use_strand) == STRAND_BEHAVIOR_SAME for gr in grs
+    )
+    strand_behavior: VALID_STRAND_BEHAVIOR_TYPE = (
+        STRAND_BEHAVIOR_SAME if strand_behavior_same else STRAND_BEHAVIOR_IGNORE
+    )
 
     rowdicts = []
-    for (lt, lf), (t, f) in zip(_labels, combinations_with_replacement(grs, r=2)):
-        if verbose:
-            print(lt, lf, file=sys.stderr)
-
+    for (lt, lf), (t, f) in zip(_labels, combinations_with_replacement(grs, r=2), strict=True):
         if lt == lf:
-
-            if not strand:
+            if not use_strand:
                 tp = t.length
                 fn = 0
                 tn = genome_length - tp
                 fp = 0
                 rowdicts.append({"T": lt, "F": lf, "TP": tp, "FP": fp, "TN": tn, "FN": fn, "MCC": 1})
             else:
-                for strand in "+ -".split():
-                    tp = t[strand].length
+                for _strand in "+ -".split():
+                    tp = t[use_strand].length
                     fn = 0
                     tn = genome_length - tp
                     fp = 0
-                    rowdicts.append({"T": lt, "F": lf, "Strand": strand, "TP": tp, "FP": fp, "TN": tn, "FN": fn, "MCC": 1})
+                    rowdicts.append(
+                        {
+                            "T": lt,
+                            "F": lf,
+                            "Strand": _strand,
+                            "TP": tp,
+                            "FP": fp,
+                            "TN": tn,
+                            "FN": fn,
+                            "MCC": 1,
+                        },
+                    )
             continue
 
-        else:
-            j = t.join(f, strandedness=strandedness)
-            tp_gr = j.new_position("intersection").merge(strand=strand)
-            if strand:
-                for strand in "+ -".split():
-                    tp = tp_gr[strand].length
-                    fp = f[strand].length - tp
-                    fn = t[strand].length - tp
+        else:  # noqa: RET507
+            j = t.join_ranges(f, strand_behavior=strand_behavior)
+            tp_gr = j.combine_interval_columns().merge_overlaps(use_strand=use_strand)
+            if use_strand:
+                for _strand in "+ -".split():
+                    tp = tp_gr[_strand].length
+                    fp = f[_strand].length - tp
+                    fn = t[_strand].length - tp
                     tn = genome_length - (tp + fp + fn)
                     mcc = _mcc(tp, fp, tn, fn)
-                    rowdicts.append({"T": lt, "F": lf, "Strand": strand, "TP": tp, "FP": fp, "TN": tn, "FN": fn, "MCC": mcc})
-                    rowdicts.append({"T": lf, "F": lt, "Strand": strand, "TP": tp, "FP": fn, "TN": tn, "FN": fp, "MCC": mcc})
+                    rowdicts.extend(
+                        [
+                            {
+                                "T": lt,
+                                "F": lf,
+                                "Strand": _strand,
+                                "TP": tp,
+                                "FP": fp,
+                                "TN": tn,
+                                "FN": fn,
+                                "MCC": mcc,
+                            },
+                            {
+                                "T": lf,
+                                "F": lt,
+                                "Strand": _strand,
+                                "TP": tp,
+                                "FP": fn,
+                                "TN": tn,
+                                "FN": fp,
+                                "MCC": mcc,
+                            },
+                        ],
+                    )
             else:
                 tp = tp_gr.length
                 fp = f.length - tp
                 fn = t.length - tp
                 tn = genome_length - (tp + fp + fn)
                 mcc = _mcc(tp, fp, tn, fn)
 
-                rowdicts.append({"T": lt, "F": lf, "TP": tp, "FP": fp, "TN": tn, "FN": fn, "MCC": mcc})
-                rowdicts.append({"T": lf, "F": lt, "TP": tp, "FP": fn, "TN": tn, "FN": fp, "MCC": mcc})
-
-    df = pd.DataFrame.from_dict(rowdicts).sort_values(["T", "F"])
+                rowdicts.extend(
+                    [
+                        {
+                            "T": lt,
+                            "F": lf,
+                            "TP": tp,
+                            "FP": fp,
+                            "TN": tn,
+                            "FN": fn,
+                            "MCC": mcc,
+                        },
+                        {
+                            "T": lf,
+                            "F": lt,
+                            "TP": tp,
+                            "FP": fn,
+                            "TN": tn,
+                            "FN": fp,
+                            "MCC": mcc,
+                        },
+                    ],
+                )
 
-    return df
+    return pd.DataFrame.from_records(rowdicts).sort_values(["T", "F"])
 
 
-def rowbased_spearman(x, y):
-
+def rowbased_spearman(x: ndarray, y: ndarray) -> ndarray:
     """Fast row-based Spearman's correlation.
 
     Parameters
     ----------
     x : matrix-like
-
         2D numerical matrix. Same size as y.
 
     y : matrix-like
-
         2D numerical matrix. Same size as x.
 
     Returns
     -------
     numpy.array
 
         Array with same length as input, where values are P-values.
 
     See Also
     --------
-
-    pyranges.statistics.rowbased_pearson : fast row-based Pearson's correlation.
-    pr.stats.fdr : correct for multiple testing
+    pyranges.stats.rowbased_pearson : fast row-based Pearson's correlation.
+    pyranges.stats.fdr : correct for multiple testing
 
     Examples
     --------
-
-    >>> np.random.seed(0)
-    >>> x = np.random.randint(10, size=(10, 10))
-    >>> y = np.random.randint(10, size=(10, 10))
+    >>> x = np.array([[7, 2, 9], [3, 6, 0], [0, 6, 3]])
+    >>> y = np.array([[5, 3, 2], [9, 6, 0], [7, 3, 5]])
 
     Perform Spearman's correlation pairwise on each row in 10x10 matrixes:
 
     >>> pr.stats.rowbased_spearman(x, y)
-    array([ 0.07523548, -0.24838724,  0.03703774,  0.24194052,  0.04778621,
-           -0.23913505,  0.12923138,  0.26840486,  0.13292204, -0.29846295])
-    """
+    array([-0.5,  0.5, -1. ])
 
+    """
     x = np.asarray(x)
     y = np.asarray(y)
 
     rx = rowbased_rankdata(x)
     ry = rowbased_rankdata(y)
 
     return rowbased_pearson(rx, ry)
 
 
-def rowbased_pearson(x, y):
-
+def rowbased_pearson(x: ndarray | DataFrame, y: ndarray | DataFrame) -> ndarray:
     """Fast row-based Pearson's correlation.
 
     Parameters
     ----------
     x : matrix-like
-
         2D numerical matrix. Same size as y.
 
     y : matrix-like
-
         2D numerical matrix. Same size as x.
 
     Returns
     -------
     numpy.array
 
         Array with same length as input, where values are P-values.
 
     See Also
     --------
-
-    pyranges.statistics.rowbased_spearman : fast row-based Spearman's correlation.
-    pr.stats.fdr : correct for multiple testing
+    pyranges.stats.rowbased_spearman : fast row-based Spearman's correlation.
+    pyranges.stats.fdr : correct for multiple testing
 
     Examples
     --------
-
-    >>> np.random.seed(0)
-    >>> x = np.random.randint(10, size=(10, 10))
-    >>> y = np.random.randint(10, size=(10, 10))
+    >>> x = np.array([[7, 2, 9], [3, 6, 0], [0, 6, 3]])
+    >>> y = np.array([[5, 3, 2], [9, 6, 0], [7, 3, 5]])
 
     Perform Pearson's correlation pairwise on each row in 10x10 matrixes:
 
     >>> pr.stats.rowbased_pearson(x, y)
-    array([ 0.20349603, -0.01667236, -0.01448763, -0.00442322,  0.06527234,
-           -0.36710862,  0.14978726,  0.32360286,  0.17209191, -0.08902829])
-    """
+    array([-0.09078413,  0.65465367, -1.        ])
 
+    """
     # Thanks to https://github.com/dengemann
 
-    def ss(a, axis):
+    def ss(a: "NDArray[np.float64]", axis: int) -> "NDArray[np.float64]":
         return np.sum(a * a, axis=axis)
 
     x = np.asarray(x)
     y = np.asarray(y)
 
     mx = x.mean(axis=-1)
     my = y.mean(axis=-1)
 
     xm, ym = x - mx[..., None], y - my[..., None]
 
     r_num = np.add.reduce(xm * ym, axis=-1)
     r_den = np.sqrt(ss(xm, axis=-1) * ss(ym, axis=-1))
 
-    with np.errstate(divide='ignore', invalid="ignore"):
-
-        r = r_num / r_den
+    with np.errstate(divide="ignore", invalid="ignore"):
+        return r_num / r_den
 
-    return r
-
-
-def rowbased_rankdata(data):
 
+def rowbased_rankdata(data: ndarray) -> DataFrame:
     """Rank order of entries in each row.
 
     Same as SciPy rankdata with method=mean.
 
     Parameters
     ----------
     data : matrix-like
-
         The data to find order of.
 
     Returns
     -------
     Pandas.DataFrame
 
         DataFrame where values are order of data.
 
     Examples
     --------
-
-    >>> np.random.seed(0)
-    >>> x = np.random.randint(10, size=(3, 10))
-    >>> x
-    array([[5, 0, 3, 3, 7, 9, 3, 5, 2, 4],
-           [7, 6, 8, 8, 1, 6, 7, 7, 8, 1],
-           [5, 9, 8, 9, 4, 3, 0, 3, 5, 0]])
+    >>> x = np.random.randint(10, size=(3, 4))
+    >>> x = np.array([[3, 7, 6, 0], [1, 3, 8, 9], [5, 9, 3, 5]])
     >>> pr.stats.rowbased_rankdata(x)
-         0    1    2    3    4     5    6    7    8    9
-    0  7.5  1.0  4.0  4.0  9.0  10.0  4.0  7.5  2.0  6.0
-    1  6.0  3.5  9.0  9.0  1.5   3.5  6.0  6.0  9.0  1.5
-    2  6.5  9.5  8.0  9.5  5.0   3.5  1.5  3.5  6.5  1.5
-    """
+         0    1    2    3
+    0  2.0  4.0  3.0  1.0
+    1  1.0  2.0  3.0  4.0
+    2  2.5  4.0  1.0  2.5
 
+    """
     dc = np.asarray(data).copy()
     sorter = np.apply_along_axis(np.argsort, 1, data)
 
     inv = np.empty(data.shape, np.intp)
 
     ranks = np.tile(np.arange(data.shape[1]), (len(data), 1))
 
@@ -478,450 +541,325 @@
 
     dc = np.take_along_axis(dc, sorter, 1)
 
     res = np.apply_along_axis(lambda r: r[1:] != r[:-1], 1, dc)
 
     obs = np.column_stack([np.ones(len(res), dtype=bool), res])
 
-    dense = np.take_along_axis(np.apply_along_axis(np.cumsum, 1, obs), inv, 1)
+    dense = pd.DataFrame(np.take_along_axis(np.apply_along_axis(np.cumsum, 1, obs), inv, 1))
 
     len_r = obs.shape[1]
 
     nonzero = np.count_nonzero(obs, axis=1)
-    obs = pd.DataFrame(obs)
-    nonzero = pd.Series(nonzero)
-    dense = pd.DataFrame(dense)
-
-    ranks = []
-    for _nonzero, nzdf in obs.groupby(nonzero, sort=False):
 
+    _ranks = []
+    for _nonzero, nzdf in pd.DataFrame(obs).groupby(pd.Series(nonzero), sort=False):
         nz = np.apply_along_axis(lambda r: np.nonzero(r)[0], 1, nzdf)
 
         _count = np.column_stack([nz, np.ones(len(nz)) * len_r])
-        _dense = dense.reindex(nzdf.index).values
+        _dense = dense.reindex(nzdf.index).to_numpy()
 
         _result = 0.5 * (np.take_along_axis(_count, _dense, 1) + np.take_along_axis(_count, _dense - 1, 1) + 1)
 
         result = pd.DataFrame(_result, index=nzdf.index)
-        ranks.append(result)
-
-    final = pd.concat(ranks).sort_index(kind="mergesort")
-
-    return final
+        _ranks.append(result)
 
+    return pd.concat(_ranks).sort_index(kind="mergesort")
 
-def simes(df, groupby, pcol, keep_position=False):
 
+def simes(
+    df: "pr.PyRanges",
+    by: str | list[str],
+    pcol: str,
+    *,
+    keep_position: bool = False,
+) -> "pr.PyRanges | DataFrame":
     """Apply Simes method for giving dependent events a p-value.
 
     Parameters
     ----------
     df : pandas.DataFrame
-
         Data to analyse with Simes.
 
-    groupby : str or list of str
-
+    by : str or list of str
         Features equal in these columns will be merged with Simes.
 
     pcol : str
-
         Name of column with p-values.
 
     keep_position : bool, default False
-
         Keep columns "Chromosome", "Start", "End" and "Strand" if they exist.
 
     See Also
     --------
-
     pr.stats.fdr : correct for multiple testing
 
     Examples
     --------
-
     >>> s = '''Chromosome Start End Strand Gene PValue
     ... 1 10 20 + P53 0.0001
-    ... 1 20 20 + P53 0.0002
-    ... 1 30 20 + P53 0.0003
+    ... 1 20 35 + P53 0.0002
+    ... 1 30 40 + P53 0.0003
     ... 2 60 65 - FOX 0.05
     ... 2 70 75 - FOX 0.0000001
     ... 2 80 90 - FOX 0.0000021'''
 
     >>> gr = pr.from_string(s)
     >>> gr
-    +--------------+-----------+-----------+--------------+------------+-------------+
-    |   Chromosome |     Start |       End | Strand       | Gene       |      PValue |
-    |   (category) |   (int32) |   (int32) | (category)   | (object)   |   (float64) |
-    |--------------+-----------+-----------+--------------+------------+-------------|
-    |            1 |        10 |        20 | +            | P53        |     0.0001  |
-    |            1 |        20 |        20 | +            | P53        |     0.0002  |
-    |            1 |        30 |        20 | +            | P53        |     0.0003  |
-    |            2 |        60 |        65 | -            | FOX        |     0.05    |
-    |            2 |        70 |        75 | -            | FOX        |     1e-07   |
-    |            2 |        80 |        90 | -            | FOX        |     2.1e-06 |
-    +--------------+-----------+-----------+--------------+------------+-------------+
-    Stranded PyRanges object has 6 rows and 6 columns from 2 chromosomes.
-    For printing, the PyRanges was sorted on Chromosome and Strand.
+      index  |      Chromosome    Start      End  Strand    Gene         PValue
+      int64  |           int64    int64    int64  object    object      float64
+    -------  ---  ------------  -------  -------  --------  --------  ---------
+          0  |               1       10       20  +         P53         0.0001
+          1  |               1       20       35  +         P53         0.0002
+          2  |               1       30       40  +         P53         0.0003
+          3  |               2       60       65  -         FOX         0.05
+          4  |               2       70       75  -         FOX         1e-07
+          5  |               2       80       90  -         FOX         2.1e-06
+    PyRanges with 6 rows, 6 columns, and 1 index columns.
+    Contains 2 chromosomes and 2 strands.
 
-    >>> simes = pr.stats.simes(gr.df, "Gene", "PValue")
+    >>> simes = pr.stats.simes(gr, "Gene", "PValue")
     >>> simes
       Gene         Simes
     0  FOX  3.000000e-07
     1  P53  3.000000e-04
 
-    >>> gr.apply(lambda df:
-    ... pr.stats.simes(df, "Gene", "PValue", keep_position=True))
-    +--------------+-----------+-----------+-------------+------------+------------+
-    |   Chromosome |     Start |       End |       Simes | Strand     | Gene       |
-    |     (object) |   (int32) |   (int32) |   (float64) | (object)   | (object)   |
-    |--------------+-----------+-----------+-------------+------------+------------|
-    |            1 |        10 |        20 |      0.0001 | +          | P53        |
-    |            2 |        60 |        90 |      1e-07  | -          | FOX        |
-    +--------------+-----------+-----------+-------------+------------+------------+
-    Stranded PyRanges object has 2 rows and 6 columns from 2 chromosomes.
-    For printing, the PyRanges was sorted on Chromosome and Strand.
-    """
+    >>> pr.stats.simes(gr, "Gene", "PValue", keep_position=True)
+      index  |      Chromosome    Start      End      Simes  Strand    Gene
+      int64  |           int64    int64    int64    float64  object    object
+    -------  ---  ------------  -------  -------  ---------  --------  --------
+          0  |               2       60       90     1e-07   -         FOX
+          1  |               1       10       40     0.0001  +         P53
+    PyRanges with 2 rows, 6 columns, and 1 index columns.
+    Contains 2 chromosomes and 2 strands.
 
-    if isinstance(groupby, str):
-        groupby = [groupby]
+    """
+    if isinstance(by, str):
+        by = [by]
 
     positions = []
-    if "Strand" in df:
-        stranded = True
 
     if keep_position:
-        positions += ["Chromosome", "Start", "End"]
-        if stranded:
+        positions += GENOME_LOC_COLS
+        if df.has_strand:
             positions += ["Strand"]
 
-    sorter = groupby + [pcol]
+    sorter = [*by, pcol]
 
     sdf = df[positions + sorter].sort_values(sorter)
-    g = sdf.groupby(positions + groupby)
+    g = sdf.groupby(positions + by)
 
-    ranks = g.cumcount().values + 1
-    size = g.size().values
+    ranks = g.cumcount().to_numpy() + 1
+    size = g.size().to_numpy()
     size = np.repeat(size, size)
-    multiplied = (sdf[pcol].values * size)
+    multiplied = sdf[pcol].to_numpy() * size
 
     simes = multiplied / ranks
 
     sdf.insert(sdf.shape[1], "Simes", simes)
 
     if keep_position:
+        grpby_dict = {
+            "Chromosome": "first",
+            "Start": "min",
+            "End": "max",
+            "Simes": "min",
+        }
 
-        grpby_dict = {"Chromosome": "first", "Start": "min", "End": "max", "Simes": "min"}
-
-        if stranded:
+        if sdf.has_strand:
             grpby_dict["Strand"] = "first"
 
-        simes = sdf.groupby(groupby).agg(grpby_dict).reset_index()
+        simes = sdf.groupby(by).agg(grpby_dict).reset_index()
         columns = list(simes.columns)
         columns.append(columns[0])
         del columns[0]
-        simes = simes[columns]
+        _simes: "PyRanges | DataFrame"
+        _simes = mypy_ensure_pyranges(simes[columns])
     else:
-        simes = sdf.groupby(groupby).Simes.min().reset_index()
-
-    return simes
-
-
-
-def chromsizes_as_int(chromsizes):
-        if isinstance(chromsizes, int):
-            pass
-        elif isinstance(chromsizes, dict):
-            chromsizes = sum(chromsizes.values())
-        elif isinstance(chromsizes, (pd.DataFrame, pr.PyRanges)):
-            chromsizes = chromsizes.End.sum()
-
-        return chromsizes
+        _simes = sdf.groupby(by).Simes.min().reset_index()
 
+    return _simes
 
-class StatisticsMethods():
 
-    """Namespace for statistical comparsion-operations.
+####################################################################################################
+# methods available at pr.stats and at pr.PyRanges.stats: (see usages of StatsManager for how to)
 
-    Accessed with gr.stats."""
 
-    pr = None
+def forbes(
+    p: "PyRanges",
+    other: "PyRanges",
+    chromsizes: "PyRanges | DataFrame | dict[Any, int]",
+    strand_behavior: VALID_STRAND_BEHAVIOR_TYPE = "auto",
+) -> float:
+    """Compute Forbes coefficient.
 
-    def __init__(self, pr):
+    Ratio which represents observed versus expected co-occurence.
 
-        self.pr = pr
+    Described in ``Forbes SA (1907): On the local distribution of certain Illinois fishes: an essay in statistical ecology.``
 
+    Parameters
+    ----------
+    p : PyRanges
+        Intervals to compare.
 
-    def forbes(self, other, chromsizes, strandedness=None):
-
-        """Compute Forbes coefficient.
-
-        Ratio which represents observed versus expected co-occurence.
-
-        Described in ``Forbes SA (1907): On the local distribution of certain Illinois fishes: an essay in statistical ecology.``
-
-        Parameters
-        ----------
-        other : PyRanges
+    other : PyRanges
+        Intervals to compare with.
 
-            Intervals to compare with.
+    chromsizes : int, dict, DataFrame or PyRanges
+        Integer representing genome length or mapping from chromosomes
+        to its length.
+
+    strand_behavior : {"auto", "same", "opposite", "ignore"}, default "auto"
+        Whether to consider overlaps of intervals on the same strand, the opposite or ignore strand
+        information. The default, "auto", means use "same" if both PyRanges are stranded (see .strand_valid)
+        otherwise ignore the strand information.
 
-        chromsizes : int, dict, DataFrame or PyRanges
+    Returns
+    -------
+    float
 
-            Integer representing genome length or mapping from chromosomes
-            to its length.
+        Ratio of observed versus expected co-occurence.
 
-        strandedness : {None, "same", "opposite", False}, default None, i.e. "auto"
+    See Also
+    --------
+    pyranges.stats.jaccard : compute the jaccard coefficient
 
-            Whether to compute without regards to strand or on same or opposite.
+    Examples
+    --------
+    >>> gr, gr2 = pr.example_data.f1, pr.example_data.f2
+    >>> pr.stats.forbes(gr, gr2, chromsizes={"chr1": 10})
+    0.8333333333333334
 
-        Returns
-        -------
-        float
+    """
+    _chromsizes = _chromsizes_as_int(chromsizes)
 
-            Ratio of observed versus expected co-occurence.
+    strand_behavior = validate_and_convert_strand_behavior(p, other, strand_behavior)
+    use_strand = use_strand_from_validated_strand_behavior(p, other, strand_behavior)
 
-        See Also
-        --------
+    reference_length = p.merge_overlaps(use_strand=use_strand).length
+    query_length = other.merge_overlaps(use_strand=use_strand).length
 
-        pyranges.statistics.jaccard : compute the jaccard coefficient
+    intersection_sum = p.set_intersect(other, strand_behavior=strand_behavior).lengths().sum()
+    return _chromsizes * intersection_sum / (reference_length * query_length)
 
-        Examples
-        --------
 
-        >>> gr, gr2 = pr.data.chipseq(), pr.data.chipseq_background()
-        >>> chromsizes = pr.data.chromsizes()
-        >>> gr.stats.forbes(gr2, chromsizes=chromsizes)
-        1.7168314674978278"""
+def jaccard(
+    p: "PyRanges",
+    other: "PyRanges",
+    strand_behavior: VALID_STRAND_BEHAVIOR_TYPE = "auto",
+) -> float:
+    """Compute Jaccards coefficient.
 
-        chromsizes = chromsizes_as_int(chromsizes)
+    Ratio of the intersection and union of two sets.
 
-        self = self.pr
+    Parameters
+    ----------
+    p : PyRanges
+        Intervals to compare.
 
-        kwargs = {}
-        kwargs["sparse"] = {"self": True, "other": True}
-        kwargs = pr.pyranges.fill_kwargs(kwargs)
-        strand = True if kwargs.get("strandedness") else False
+    other : PyRanges
+        Intervals to compare with.
 
-        reference_length = self.merge(strand=strand).length
-        query_length = other.merge(strand=strand).length
+    strand_behavior : {"auto", "same", "opposite", "ignore"}, default "auto"
+        Whether to consider overlaps of intervals on the same strand, the opposite or ignore strand
+        information. The default, "auto", means use "same" if both PyRanges are stranded (see .strand_valid)
+        otherwise ignore the strand information.
 
-        intersection_sum = sum(
-            v.sum()
-            for v in self.set_intersect(
-                    other, strandedness=strandedness).lengths(as_dict=True).values())
+    Returns
+    -------
+    float
 
-        forbes = chromsizes * intersection_sum / (reference_length * query_length)
+        Ratio of the intersection and union of two sets.
 
-        return forbes
+    See Also
+    --------
+    pyranges.stats.forbes : compute the forbes coefficient
 
+    Examples
+    --------
+    >>> gr, gr2 = pr.example_data.f1, pr.example_data.f2
+    >>> chromsizes = pr.example_data.chromsizes
+    >>> pr.stats.jaccard(gr, gr2)
+    0.14285714285714285
 
-    def jaccard(self, other, **kwargs):
+    """
+    strand_behavior = validate_and_convert_strand_behavior(p, other, strand_behavior)
+    use_strand = use_strand_from_validated_strand_behavior(p, other, strand_behavior)
 
-        """Compute Jaccards coefficient.
+    intersection_sum = p.set_intersect(other).lengths().sum()
 
-        Ratio of the intersection and union of two sets.
+    union_sum = 0
+    for gr in [p, other]:
+        union_sum += gr.merge_overlaps(use_strand=use_strand).lengths().sum()
 
-        Parameters
-        ----------
-        other : PyRanges
-
-            Intervals to compare with.
-
-        chromsizes : int, dict, DataFrame or PyRanges
-
-            Integer representing genome length or mapping from chromosomes
-            to its length.
-
-        strandedness : {None, "same", "opposite", False}, default None, i.e. "auto"
-
-            Whether to compute without regards to strand or on same or opposite.
-
-        Returns
-        -------
-        float
-
-            Ratio of the intersection and union of two sets.
-
-        See Also
-        --------
-
-        pyranges.statistics.forbes : compute the forbes coefficient
-
-        Examples
-        --------
-
-        >>> gr, gr2 = pr.data.chipseq(), pr.data.chipseq_background()
-        >>> chromsizes = pr.data.chromsizes()
-        >>> gr.stats.jaccard(gr2, chromsizes=chromsizes)
-        6.657941988519211e-05"""
-
-        self = self.pr
-
-        kwargs["sparse"] = {"self": True, "other": True}
-        kwargs = pr.pyranges.fill_kwargs(kwargs)
-        strand = True if kwargs.get("strandedness") else False
-
-        intersection_sum = sum(
-            v.sum()
-            for v in self.set_intersect(other).lengths(as_dict=True).values())
-
-        union_sum = 0
-        for gr in [self, other]:
-            union_sum += sum(
-                v.sum() for v in gr.merge(strand=strand).lengths(as_dict=True).values())
-
-        denominator = (union_sum - intersection_sum)
-        if denominator == 0:
-            return 1
-        else:
-            jc = intersection_sum / denominator
-
-        return jc
-
-    def relative_distance(self, other):
-
-        """Compute spatial correllation between two sets.
-
-        Metric which describes relative distance between each interval in one
-        set and two closest intervals in another.
-
-        Parameters
-        ----------
-        other : PyRanges
-
-            Intervals to compare with.
-
-        chromsizes : int, dict, DataFrame or PyRanges
-
-            Integer representing genome length or mapping from chromosomes
-            to its length.
-
-        strandedness : {None, "same", "opposite", False}, default None, i.e. "auto"
-
-            Whether to compute without regards to strand or on same or opposite.
-
-        Returns
-        -------
-        pandas.DataFrame
-
-            DataFrame containing the frequency of each relative distance.
-
-        See Also
-        --------
-
-        pyranges.statistics.jaccard : compute the jaccard coefficient
-        pyranges.statistics.forbes : compute the forbes coefficient
-
-        Examples
-        --------
-
-        >>> gr, gr2 = pr.data.chipseq(), pr.data.chipseq_background()
-        >>> chromsizes = pr.data.chromsizes()
-        >>> gr.stats.relative_distance(gr2)
-            reldist  count  total  fraction
-        0      0.00    264   9956  0.026517
-        1      0.01    226   9956  0.022700
-        2      0.02    206   9956  0.020691
-        3      0.03    235   9956  0.023604
-        4      0.04    194   9956  0.019486
-        5      0.05    241   9956  0.024207
-        6      0.06    201   9956  0.020189
-        7      0.07    191   9956  0.019184
-        8      0.08    192   9956  0.019285
-        9      0.09    191   9956  0.019184
-        10     0.10    186   9956  0.018682
-        11     0.11    203   9956  0.020390
-        12     0.12    218   9956  0.021896
-        13     0.13    209   9956  0.020992
-        14     0.14    201   9956  0.020189
-        15     0.15    178   9956  0.017879
-        16     0.16    202   9956  0.020289
-        17     0.17    197   9956  0.019787
-        18     0.18    208   9956  0.020892
-        19     0.19    202   9956  0.020289
-        20     0.20    191   9956  0.019184
-        21     0.21    188   9956  0.018883
-        22     0.22    213   9956  0.021394
-        23     0.23    192   9956  0.019285
-        24     0.24    199   9956  0.019988
-        25     0.25    181   9956  0.018180
-        26     0.26    172   9956  0.017276
-        27     0.27    191   9956  0.019184
-        28     0.28    190   9956  0.019084
-        29     0.29    192   9956  0.019285
-        30     0.30    201   9956  0.020189
-        31     0.31    212   9956  0.021294
-        32     0.32    213   9956  0.021394
-        33     0.33    177   9956  0.017778
-        34     0.34    197   9956  0.019787
-        35     0.35    163   9956  0.016372
-        36     0.36    191   9956  0.019184
-        37     0.37    198   9956  0.019888
-        38     0.38    160   9956  0.016071
-        39     0.39    188   9956  0.018883
-        40     0.40    200   9956  0.020088
-        41     0.41    188   9956  0.018883
-        42     0.42    230   9956  0.023102
-        43     0.43    197   9956  0.019787
-        44     0.44    224   9956  0.022499
-        45     0.45    184   9956  0.018481
-        46     0.46    198   9956  0.019888
-        47     0.47    187   9956  0.018783
-        48     0.48    200   9956  0.020088
-        49     0.49    194   9956  0.019486
-        """
-
-        self = self.pr
-
-        kwargs = {}
-        kwargs["sparse"] = {"self": True, "other": True}
-        kwargs = pr.pyranges.fill_kwargs(kwargs)
-
-        result = pyrange_apply(_relative_distance, self, other, **kwargs)  # pylint: disable=E1132
-
-        result = pd.Series(np.concatenate(list(result.values())))
-
-        not_nan = ~np.isnan(result)
-        result.loc[not_nan] = np.floor(result[not_nan] * 100) / 100
-        vc = result.value_counts(dropna=False).to_frame().reset_index()
-        vc.columns = "reldist count".split()
-        vc.insert(vc.shape[1], "total", len(result))
-        vc.insert(vc.shape[1], "fraction", vc["count"] / len(result))
-        vc = vc.sort_values("reldist", ascending=True)
-        vc = vc.reset_index(drop=True)
+    denominator = union_sum - intersection_sum
+    if denominator == 0:
+        return 1.0
+    return intersection_sum / denominator
 
-        return vc
 
-from math import sqrt
-def _mcc(tp, fp, tn, fn):
+def relative_distance(p: "PyRanges", other: "PyRanges", **_) -> DataFrame:
+    """Compute spatial correlation between two sets.
 
-    # https://stackoverflow.com/a/56875660/992687
-    x = (tp + fp) * (tp + fn) * (tn + fp) * (tn + fn)
-    return ((tp * tn) - (fp * fn)) / sqrt(x)
+    Metric which describes relative distance between each interval in one
+    set and two closest intervals in another.
 
+    Parameters
+    ----------
+    p : PyRanges
+        Intervals to compare.
 
+    other : PyRanges
+        Intervals to compare with.
 
-# def __tetrachoric(self, other, chromsizes, **kwargs):
+    chromsizes : int, dict, DataFrame or PyRanges
 
-#     self = self.pr
+        Integer representing genome length or mapping from chromosomes
+        to its length.
 
-#     chromsizes = chromsizes_as_int(chromsizes)
+    strandedness : {None, "same", "opposite", False}, default None, i.e. "auto"
 
-#     kwargs["new_pos"] = "intersection"
-#     strand = True if kwargs.get("strandedness") else False
+        Whether to compute without regards to strand or on same or opposite.
 
-#     ss = self.merge(strand=strand)
-#     so = other.merge(strand=strand)
-#     a = ss.intersect(so, **kwargs).length
-#     b = ss.subtract(so, **kwargs).length
-#     c = so.subtract(ss, **kwargs).length
+    Returns
+    -------
+    pandas.DataFrame
 
-#     m = pr.concat([ss, so]).merge(strand=strand).length
+        DataFrame containing the frequency of each relative distance.
 
-#     d = chromsizes - m
+    See Also
+    --------
+    pyranges.stats.jaccard : compute the jaccard coefficient
+    pyranges.stats.forbes : compute the forbes coefficient
 
-#     from math import cos, sqrt
+    Examples
+    --------
+    >>> gr1, gr2 = pr.example_data.chipseq, pr.example_data.chipseq_background
+    >>> gr = pd.concat([gr1, gr1.head(4), gr2.tail(4)])
+    >>> chromsizes = pr.example_data.chromsizes
+    >>> pr.stats.relative_distance(gr, gr2)
+        reldist  count  total  fraction
+    0      0.00      4     18  0.222222
+    1      0.03      1     18  0.055556
+    2      0.04      1     18  0.055556
+    3      0.10      1     18  0.055556
+    4      0.12      1     18  0.055556
+    5      0.13      1     18  0.055556
+    6      0.19      1     18  0.055556
+    7      0.23      1     18  0.055556
+    8      0.24      1     18  0.055556
+    9      0.38      1     18  0.055556
+    10     0.41      2     18  0.111111
+    11     0.42      1     18  0.055556
+    12     0.43      2     18  0.111111
 
-#     _tetrachoric = cos(180/(1 + sqrt((b * c) / (a * d))))
+    """
+    result = pd.Series(_relative_distance(p, other))
 
-#     return _tetrachoric
+    not_nan = ~np.isnan(result)
+    result.loc[not_nan] = np.floor(result[not_nan] * 100) / 100
+    vc = result.value_counts(dropna=False).to_frame().reset_index()
+    vc.columns = pd.Index(["reldist", "count"])
+    vc.insert(vc.shape[1], "total", len(result))
+    vc.insert(vc.shape[1], "fraction", vc["count"] / len(result))
+    vc = vc.sort_values("reldist", ascending=True)
+    return vc.reset_index(drop=True)
```

### Comparing `pyranges-0.0.99/tests/helpers.py` & `pyranges-0.1.0/tests/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import pandas as pd
 
 
-def assert_df_equal(df1, df2):
+def assert_df_equal(df1, df2) -> None:
+    print("-" * 100)
+    print("df1")
+    print(df1)
+    print("df2")
+    print(df2)
 
     # df1.loc[:, "Start"] = df1.Start.astype(np.int64)
     # df2.loc[:, "Start"] = df1.Start.astype(np.int64)
     # df1.loc[:, "End"] = df1.End.astype(np.int64)
     # df2.loc[:, "End"] = df1.End.astype(np.int64)
 
     pd.options.mode.chained_assignment = None
```

### Comparing `pyranges-0.0.99/tests/hypothesis_helper.py` & `pyranges-0.1.0/tests/property_based/hypothesis_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,155 +1,134 @@
-from hypothesis.extra.pandas import data_frames, column, indexes
 import hypothesis.strategies as st
+import numpy as np
+import pandas as pd
+from hypothesis.extra.pandas import column, data_frames, indexes
 
 import pyranges as pr
 from pyranges import PyRanges
 
-import pandas as pd
-import numpy as np
-
-from os import environ
-from sys import platform
-
-if environ.get("TRAVIS") or platform == "darwin":
-    max_examples = 100
-    slow_max_examples = 10
-    deadline = None
-else:
-    max_examples = 1000
-    slow_max_examples = 100
-    deadline = None
+max_examples = 15
+slow_max_examples = 5
+deadline = None
 
 lengths = st.integers(min_value=1, max_value=int(1e7))
 small_lengths = st.integers(min_value=1, max_value=int(1e4))
 
 strands = st.sampled_from("+ -".split())
 single_strand = st.sampled_from(["+"])
 names = st.text("abcdefghijklmnopqrstuvxyz", min_size=1)
 scores = st.integers(min_value=0, max_value=256)
 
 datatype = st.sampled_from([pd.Series, np.array, list])
 
 feature_data = st.sampled_from(["ensembl_gtf", "gencode_gtf", "ucsc_bed"])
 
-chromosomes = st.sampled_from(
-    ["chr{}".format(str(e)) for e in list(range(1, 23)) + "X Y M".split()])
+chromosomes = st.sampled_from([f"chr{e!s}" for e in list(range(1, 23)) + "X Y M".split()])
 chromosomes_small = st.sampled_from(["chr1"])
 cs = st.one_of(chromosomes, chromosomes_small)
 
 runlengths = data_frames(
     index=indexes(dtype=np.int64, min_size=1, unique=True),
     columns=[
         column("Runs", st.integers(min_value=1, max_value=int(1e7))),
         # must have a min/max on floats because R S4vectors translates too big ones into inf.
         # which is unequal to eg -1.79769e+308 so the tests fail
-        column("Values", st.integers(min_value=-int(1e7), max_value=int(1e7)))
-    ])
+        column("Values", st.integers(min_value=-int(1e7), max_value=int(1e7))),
+    ],
+)
 
 better_dfs_no_min = data_frames(
     index=indexes(dtype=np.int64, min_size=0, unique=True, elements=lengths),
     columns=[
         column("Chromosome", cs),
         column("Start", elements=lengths),
         column("End", elements=small_lengths),
         # column("Name", elements=names),
         # column("Score", elements=scores),
-        column("Strand", strands)
-    ])
+        column("Strand", strands),
+    ],
+)
 
 better_dfs_min = data_frames(
     index=indexes(dtype=np.int64, min_size=1, unique=True, elements=lengths),
     columns=[
         column("Chromosome", cs),
         column("Start", elements=lengths),
         column("End", elements=small_lengths),
         # column("Name", elements=names),
         # column("Score", elements=scores),
-        column("Strand", strands)
-    ])
+        column("Strand", strands),
+    ],
+)
 
 better_dfs_min_2 = data_frames(
     index=indexes(dtype=np.int64, min_size=2, unique=True, elements=lengths),
     columns=[
         column("Chromosome", chromosomes_small),
         column("Start", elements=lengths),
         column("End", elements=small_lengths),
         # column("Name", elements=names),
         # column("Score", elements=scores),
-        column("Strand", single_strand)
-    ])
+        column("Strand", single_strand),
+    ],
+)
 
 better_dfs_min_single_chromosome = data_frames(
     index=indexes(dtype=np.int64, min_size=1, unique=True, elements=lengths),
     columns=[
         column("Chromosome", chromosomes_small),
         column("Start", elements=lengths),
         column("End", elements=small_lengths),
         # column("Name", elements=names),
         # column("Score", elements=scores),
-        column("Strand", strands)
-    ])
+        column("Strand", strands),
+    ],
+)
 
 runlengths_same_length_integers = data_frames(
     index=indexes(dtype=np.int64, min_size=1, unique=True),
     columns=[
         column("Runs", st.integers(min_value=1, max_value=int(1e4))),
         column("Values", st.integers(min_value=1, max_value=int(1e4))),
-        column("Values2", st.integers(min_value=1, max_value=int(1e4)))
-    ])
+        column("Values2", st.integers(min_value=1, max_value=int(1e4))),
+    ],
+)
 
 
 @st.composite
 def dfs_min2(draw):  # nosec
     df = draw(better_dfs_min_2)
     # strand = draw(use_strand)
     df.loc[:, "End"] += df.Start
 
     df.insert(3, "Name", "a")
     df.insert(4, "Score", 0)
 
     # if not strand:
     #     df = df.drop("Strand", axis=1)
 
-    gr = PyRanges(df, int64=True)
+    return PyRanges(df)
     # gr = PyRanges(df)
 
     # do not sort like this, use pyranges sort
     # np.random.seed(draw(st.integers(min_value=0, max_value=int(1e6))))
     # gr.df = df.reindex(np.random.permutation(df.index.values))
 
-    return gr
-
 
 @st.composite
-def dfs_min(draw):  # nosec
+def dfs_min(draw):
     df = draw(better_dfs_min)
     # strand = draw(use_strand)
     df.loc[:, "End"] += df.Start
 
     df.insert(3, "Name", "a")
     df.insert(4, "Score", 0)
 
-    # df.Start = df.Start.astype(np.int32)
-    # df.End = df.End.astype(np.int32)
-    # print(df.dtypes)
-    # stranded = draw(st.booleans())
-    # if not strand:
-    #     df = df.drop("Strand", axis=1)
-
-    gr = PyRanges(df, int64=True)
-    # print(gr)
-    # raise
-    # gr = PyRanges(df)
-
-    # do not sort like this, use pyranges sort
-    # np.random.seed(draw(st.integers(min_value=0, max_value=int(1e6))))
-    # gr.df = df.reindex(np.random.permutation(df.index.values))
-
-    return gr
+    print(df)
+    return PyRanges(df)
 
 
 @st.composite
 def dfs_no_min(draw):  # nosec
     df = draw(better_dfs_no_min)
     # strand = draw(use_strand)
     df.loc[:, "End"] += df.Start
@@ -157,23 +136,21 @@
     df.insert(3, "Name", "a")
     df.insert(4, "Score", 0)
 
     # stranded = draw(st.booleans())
     # if not strand:
     #     df = df.drop("Strand", axis=1)
 
-    gr = PyRanges(df, int64=True)
+    return PyRanges(df)
     # gr = PyRanges(df)
 
     # do not sort like this, use pyranges sort
     # np.random.seed(draw(st.integers(min_value=0, max_value=int(1e6))))
     # gr.df = df.reindex(np.random.permutation(df.index.values))
 
-    return gr
-
 
 @st.composite
 def dfs_min_with_id(draw):  # nosec
     df = draw(better_dfs_min)
     ids = df.Start
     # strand = draw(use_strand)
     df.loc[:, "End"] += df.Start
@@ -185,25 +162,23 @@
     # df.Start = df.Start.astype(np.int32)
     # df.End = df.End.astype(np.int32)
     # print(df.dtypes)
     # stranded = draw(st.booleans())
     # if not strand:
     #     df = df.drop("Strand", axis=1)
 
-    gr = PyRanges(df)
+    return PyRanges(df)
     # print(gr)
     # raise
     # gr = PyRanges(df)
 
     # do not sort like this, use pyranges sort
     # np.random.seed(draw(st.integers(min_value=0, max_value=int(1e6))))
     # gr.df = df.reindex(np.random.permutation(df.index.values))
 
-    return gr
-
 
 @st.composite
 def dfs_min_with_gene_id(draw):  # nosec
     df = draw(better_dfs_min)
     ids = df.Start
     # strand = draw(use_strand)
     df.loc[:, "End"] += df.Start
@@ -216,29 +191,26 @@
     # df.Start = df.Start.astype(np.int32)
     # df.End = df.End.astype(np.int32)
     # print(df.dtypes)
     # stranded = draw(st.booleans())
     # if not strand:
     #     df = df.drop("Strand", axis=1)
 
-    gr = PyRanges(df)
+    return PyRanges(df)
     # print(gr)
     # raise
     # gr = PyRanges(df)
 
     # do not sort like this, use pyranges sort
     # np.random.seed(draw(st.integers(min_value=0, max_value=int(1e6))))
     # gr.df = df.reindex(np.random.permutation(df.index.values))
 
-    return gr
-
 
 @st.composite
 def df_data(draw):
-
     df = draw(better_dfs_min)
     df.loc[:, "End"] += df.Start
 
     chromosome_type = draw(datatype)
     start_type = draw(datatype)
     end_type = draw(datatype)
     strand_type = draw(datatype)
@@ -259,32 +231,27 @@
     df.insert(4, "Score", 0)
 
     return df
 
 
 @st.composite
 def genomicfeature(draw):
-
     dataset_name = draw(feature_data)
     print("dataset name " * 5, dataset_name)
-    dataset = getattr(pr.data, dataset_name)()
+    dataset = getattr(pr.example_data, dataset_name)()
     dataset = dataset[dataset.Feature.isin(["gene", "transcript", "exon"])]
 
     # subsetter = draw(arrays(np.bool, shape=len(dataset)))
     gene_ids = list(dataset.gene_id.drop_duplicates())
-    genes = draw(
-        st.lists(st.sampled_from(gene_ids), unique="True", min_size=1))
-    dataset = dataset[dataset.gene_id.isin(genes)]
-
-    return dataset
+    genes = draw(st.lists(st.sampled_from(gene_ids), unique="True", min_size=1))
+    return dataset[dataset.gene_id.isin(genes)]
 
 
 @st.composite
 def selector(draw):
-
     df = draw(better_dfs_min)
     h = df.head(1)
     chromosome = h["Chromosome"].iloc[0]
     start = h["Start"].iloc[0]
     end = h["End"].iloc[0]
     strand = h["Strand"].iloc[0]
 
@@ -293,15 +260,15 @@
     start_bool = draw(st.booleans())
     end_bool = draw(st.booleans())
 
     _slice = {
         (True, True): slice(start, end),
         (True, False): slice(start, None),
         (False, True): slice(None, end),
-        (False, False): slice(None, None)
+        (False, False): slice(None, None),
     }[start_bool, end_bool]
 
     to_return = []
     if chromosome_bool:
         to_return.append(chromosome)
     if strand_bool:
         to_return.append(strand)
```

### Comparing `pyranges-0.0.99/tests/k_nearest.py` & `pyranges-0.1.0/tests/unit/k_nearest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,76 @@
-import pytest 
-
-import pyranges as pr
+from io import StringIO
 
 import numpy as np
 import pandas as pd
+import pytest
 
-from io import StringIO
+import pyranges as pr
 
-def string_to_df(c):
 
-    return pd.read_csv(StringIO(c), sep=r"\s+", dtype={"Chromosome": "category", "Start": np.int32, "End": np.int32, "Start_b": np.int32, "End_b": np.int32})
+def string_to_df(c):
+    return pd.read_csv(
+        StringIO(c),
+        sep=r"\s+",
+        dtype={
+            "Chromosome": "category",
+            "Start": np.int32,
+            "End": np.int32,
+            "Start_b": np.int32,
+            "End_b": np.int32,
+        },
+    )
 
 
-@pytest.fixture
+@pytest.fixture()
 def gr():
-
     return pr.PyRanges(chromosomes="chr1", starts=[1, 15, 200], ends=[10, 20, 2000])
 
 
-@pytest.fixture
+@pytest.fixture()
 def gr2():
-
     return pr.PyRanges(chromosomes="chr1", starts=[11, 11, 20, 20, 50], ends=[16, 20, 21, 22, 100])
 
-@pytest.fixture
-def result_k_nearest_different():
 
+@pytest.fixture()
+def result_k_nearest_different():
     c = """Chromosome  Start   End  Start_b  End_b  Distance
 chr1      1    10       11     16         2
 chr1      1    10       11     20         2
 chr1      1    10       20     21        11
 chr1      1    10       20     22        11
 chr1      1    10       50    100        41
 chr1     15    20       11     20         0
 chr1     15    20       11     16         0
 chr1     15    20       20     21         1
 chr1     15    20       20     22         1
 chr1    200  2000       50    100      -101"""
 
-    df = string_to_df(c)
+    return string_to_df(c)
 
-    return df
 
-@pytest.fixture
+@pytest.fixture()
 def result_k_nearest_different2():
-
     c = """Chromosome  Start  End  Start_b  End_b  Distance
 0        chr1     11   16       15     20         0
 1        chr1     11   20       15     20         0
 2        chr1     11   20        1     10        -2
 3        chr1     20   21       15     20         1
 4        chr1     20   21        1     10       -11
 5        chr1     20   21      200   2000       180
 6        chr1     20   22       15     20         1
 7        chr1     20   22        1     10       -11
 8        chr1     20   22      200   2000       179
 9        chr1     50  100       15     20       -31
 10       chr1     50  100        1     10       -41"""
 
-    df = string_to_df(c)
-
-    return df
+    return string_to_df(c)
 
 
-def test_k_nearest_different(result_k_nearest_different, result_k_nearest_different2, gr, gr2):
-
+def test_k_nearest_different(result_k_nearest_different, result_k_nearest_different2, gr, gr2) -> None:
     k = [3, 2, 1]
     r = gr.k_nearest(gr2, ties="different", k=k).df
 
     print(r)
     print(result_k_nearest_different)
 
     pd.testing.assert_frame_equal(r, result_k_nearest_different)
@@ -84,53 +86,47 @@
     print(r2)
     print("expected")
     print(result_k_nearest_different2)
 
     pd.testing.assert_frame_equal(r2, result_k_nearest_different2)
 
 
-@pytest.fixture
+@pytest.fixture()
 def result_k_nearest_first():
-
     c = """Chromosome  Start   End  Start_b  End_b  Distance
 0       chr1      1    10       11     16         2
 1       chr1      1    10       20     21        11
 2       chr1      1    10       50    100        41
 3       chr1     15    20       11     20         0
 4       chr1     15    20       20     21         1
 5       chr1    200  2000       50    100      -101"""
 
-    df = string_to_df(c)
+    return string_to_df(c)
 
-    return df
 
-@pytest.fixture
+@pytest.fixture()
 def result_k_nearest_first2():
-
     c = """Chromosome  Start  End  Start_b  End_b  Distance
 0        chr1     11   16       15     20         0
 1        chr1     11   20       15     20         0
 2        chr1     11   20        1     10        -2
 3        chr1     20   21       15     20         1
 4        chr1     20   21        1     10       -11
 5        chr1     20   21      200   2000       180
 6        chr1     20   22       15     20         1
 7        chr1     20   22        1     10       -11
 8        chr1     20   22      200   2000       179
 9        chr1     50  100       15     20       -31
 10       chr1     50  100        1     10       -41
 11       chr1     50  100      200   2000       101"""
 
-    df = string_to_df(c)
+    return string_to_df(c)
 
-    return df
-
-
-def test_k_nearest_first(result_k_nearest_first, result_k_nearest_first2, gr, gr2): # result_k_nearest_first, 
 
+def test_k_nearest_first(result_k_nearest_first, result_k_nearest_first2, gr, gr2) -> None:  # result_k_nearest_first,
     print(gr)
     print(gr2)
     k = [3, 2, 1]
     r = gr.k_nearest(gr2, ties="first", k=k).df
 
     # print(r)
     # print(result_k_nearest_first)
@@ -143,54 +139,47 @@
     # print(r2)
     # print(result_k_nearest_first2)
     # raise
 
     pd.testing.assert_frame_equal(r2, result_k_nearest_first2)
 
 
-@pytest.fixture
+@pytest.fixture()
 def result_k_nearest_last():
-
     c = """Chromosome  Start   End  Start_b  End_b  Distance
 0       chr1      1    10       11     20         2
 1       chr1      1    10       20     22        11
 2       chr1      1    10       50    100        41
 3       chr1     15    20       11     20         0
 4       chr1     15    20       20     22         1
 5       chr1    200  2000       50    100      -101"""
 
-    df = string_to_df(c)
+    return string_to_df(c)
 
-    return df
 
-@pytest.fixture
+@pytest.fixture()
 def result_k_nearest_last2():
-
     c = """Chromosome  Start  End  Start_b  End_b  Distance
 0        chr1     11   16       15     20         0
 1        chr1     11   20       15     20         0
 2        chr1     11   20        1     10        -2
 3        chr1     20   21       15     20         1
 4        chr1     20   21        1     10       -11
 5        chr1     20   21      200   2000       180
 6        chr1     20   22       15     20         1
 7        chr1     20   22        1     10       -11
 8        chr1     20   22      200   2000       179
 9        chr1     50  100       15     20       -31
 10       chr1     50  100        1     10       -41
 11       chr1     50  100      200   2000       101"""
 
-    df = string_to_df(c)
-
-    return df
-
+    return string_to_df(c)
 
 
-def test_k_nearest_last(result_k_nearest_last, result_k_nearest_last2, gr, gr2): # result_k_nearest_last, 
-
+def test_k_nearest_last(result_k_nearest_last, result_k_nearest_last2, gr, gr2) -> None:  # result_k_nearest_last,
     # print(gr)
     # print(gr2)
     k = [3, 2, 1]
     r = gr.k_nearest(gr2, ties="last", k=k).df
 
     print(gr)
     print(gr2)
@@ -205,9 +194,7 @@
     print(gr2)
     print(gr)
     print(r2)
     print(result_k_nearest_last2)
 
     pd.testing.assert_frame_equal(r2, result_k_nearest_last2)
     # assert 0
-
-
```

### Comparing `pyranges-0.0.99/tests/test_binary.py` & `pyranges-0.1.0/tests/property_based/test_binary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,71 +1,63 @@
-import pytest
-
-from hypothesis import given, settings, HealthCheck
-from hypothesis import reproduce_failure  # pylint: disable=unused-import
-
-from itertools import product
-import tempfile
 import subprocess  # nosec
+import tempfile
 from io import StringIO
+from itertools import product
 
-import pandas as pd
 import numpy as np
+import pandas as pd
+import pytest
+from hypothesis import (
+    HealthCheck,
+    given,
+    reproduce_failure,  # noqa: F401
+    settings,
+)
 
 from tests.helpers import assert_df_equal
-from tests.hypothesis_helper import dfs_min2, dfs_min
-from tests.hypothesis_helper import max_examples, deadline
+from tests.property_based.hypothesis_helper import (
+    deadline,
+    dfs_min,
+    dfs_min2,
+    max_examples,
+)
 
 strandedness = [False, "same", "opposite"]
 no_opposite = [False, "same"]
 
 
-def run_bedtools(command,
-                 gr,
-                 gr2,
-                 strandedness,
-                 nearest_overlap=False,
-                 nearest_how=None,
-                 ties=""):
-
+def run_bedtools(command, gr, gr2, strandedness, nearest_overlap=False, nearest_how=None, ties=""):
     bedtools_strand = {False: "", "same": "-s", "opposite": "-S"}[strandedness]
     bedtools_overlap = {True: "", False: "-io"}[nearest_overlap]
-    bedtools_how = {
-        "upstream": "-id",
-        "downstream": "-iu",
-        None: ""
-    }[nearest_how] + " -D a"
+    bedtools_how = {"upstream": "-id", "downstream": "-iu", None: ""}[nearest_how] + " -D a"
     # print("bedtools how:", bedtools_how)
     ties = "-t " + ties if ties else ""
 
     with tempfile.TemporaryDirectory() as temp_dir:
-        f1 = "{}/f1.bed".format(temp_dir)
-        f2 = "{}/f2.bed".format(temp_dir)
+        f1 = f"{temp_dir}/f1.bed"
+        f2 = f"{temp_dir}/f2.bed"
         gr.df.to_csv(f1, sep="\t", header=False, index=False)
         gr2.df.to_csv(f2, sep="\t", header=False, index=False)
 
         cmd = command.format(
             f1=f1,
             f2=f2,
             strand=bedtools_strand,
             overlap=bedtools_overlap,
             bedtools_how=bedtools_how,
-            ties=ties)
+            ties=ties,
+        )
         print("cmd " * 5)
         print(cmd)
         # ignoring the below line in bandit as only strings created by
         # the test suite is run here; no user input ever sought
-        result = subprocess.check_output(  # nosec
-            cmd, shell=True, executable="/bin/bash").decode()  #nosec
-
-    return result
+        return subprocess.check_output(cmd, shell=True, executable="/bin/bash").decode()  # nosec  # nosec
 
 
 def read_bedtools_result_set_op(bedtools_result, strandedness):
-
     if strandedness:
         usecols = [0, 1, 2, 5]
         names = "Chromosome Start End Strand".split()
     else:
         usecols = [0, 1, 2]
         names = "Chromosome Start End".split()
 
@@ -74,178 +66,150 @@
         header=None,
         usecols=usecols,
         names=names,
         # dtype={
         #     "Start": np.int32,
         #     "End": np.int32
         # },
-        sep="\t")
-
+        sep="\t",
+    )
 
-def compare_results(bedtools_df, result):
 
+def compare_results(bedtools_df, result) -> None:
     # from pydbg import dbg
     # dbg(bedtools_df.dtypes)
     # dbg(result.df.dtypes)
 
     if not bedtools_df.empty:
         assert_df_equal(result.df, bedtools_df)
     else:
         assert bedtools_df.empty == result.df.empty
 
 
-def compare_results_nearest(bedtools_df, result):
-
+def compare_results_nearest(bedtools_df, result) -> None:
     if not bedtools_df.empty:
         bedtools_df = bedtools_df[bedtools_df.Distance != -1]
 
     result = result.df
 
-    if not len(result) == 0:
+    if len(result) != 0:
         bedtools_df = bedtools_df.sort_values("Start End Distance".split())
         result = result.sort_values("Start End Distance".split())
         result_df = result["Chromosome Start End Strand Distance".split()]
         assert_df_equal(result_df, bedtools_df)
     else:
         assert bedtools_df.empty
 
 
-@pytest.mark.bedtools
+@pytest.mark.bedtools()
 @pytest.mark.parametrize("strandedness", no_opposite)
 @settings(
     max_examples=max_examples,
     deadline=deadline,
     print_blob=True,
-    suppress_health_check=HealthCheck.all())
+)
 @given(gr=dfs_min(), gr2=dfs_min())  # pylint: disable=no-value-for-parameter
-def test_set_intersect(gr, gr2, strandedness):
-
+def test_set_intersect(gr, gr2, strandedness) -> None:
     set_intersect_command = "bedtools intersect {strand} -a <(sort -k1,1 -k2,2n {f1} | bedtools merge {strand} -c 4,5,6 -o first -i -) -b <(sort -k1,1 -k2,2n {f2} | bedtools merge {strand} -c 4,5,6 -o first -i -)"
-    bedtools_result = run_bedtools(set_intersect_command, gr, gr2,
-                                   strandedness)
+    bedtools_result = run_bedtools(set_intersect_command, gr, gr2, strandedness)
 
     bedtools_df = read_bedtools_result_set_op(bedtools_result, strandedness)
 
     result = gr.set_intersect(gr2, strandedness=strandedness)
 
     compare_results(bedtools_df, result)
 
 
-@pytest.mark.bedtools
+@pytest.mark.bedtools()
 @pytest.mark.parametrize("strandedness", no_opposite)
 @settings(
     max_examples=max_examples,
     deadline=deadline,
     print_blob=True,
-    suppress_health_check=HealthCheck.all())
+)
 @given(gr=dfs_min(), gr2=dfs_min())  # pylint: disable=no-value-for-parameter
 # @reproduce_failure('4.15.0', b'AXicY2RAA4zoAgAAVQAD')
-def test_set_union(gr, gr2, strandedness):
-
+def test_set_union(gr, gr2, strandedness) -> None:
     set_union_command = "cat {f1} {f2} | bedtools sort | bedtools merge {strand} -c 4,5,6 -o first -i -"  # set_union_command = "bedtools merge {strand} -c 4,5,6 -o first -i {f1}"
     bedtools_result = run_bedtools(set_union_command, gr, gr2, strandedness)
 
     bedtools_df = read_bedtools_result_set_op(bedtools_result, strandedness)
 
     result = gr.set_union(gr2, strandedness=strandedness)
 
     compare_results(bedtools_df, result)
 
 
-@pytest.mark.bedtools
+@pytest.mark.bedtools()
 @pytest.mark.parametrize("strandedness", strandedness)
 @settings(
     max_examples=max_examples,
     deadline=deadline,
     print_blob=True,
-    suppress_health_check=HealthCheck.all())
+)
 @given(gr=dfs_min(), gr2=dfs_min())  # pylint: disable=no-value-for-parameter
 # @reproduce_failure('4.32.2', b'AXicY2RAA4wQzIgiCAAAgAAF')
 # @reproduce_failure('5.5.4', b'AXicY2RABYyMEAqKGRgAAHMABg==')
-def test_overlap(gr, gr2, strandedness):
-
+def test_overlap(gr, gr2, strandedness) -> None:
     overlap_command = "bedtools intersect -u {strand} -a {f1} -b {f2}"
 
     bedtools_result = run_bedtools(overlap_command, gr, gr2, strandedness)
 
     bedtools_df = pd.read_csv(
         StringIO(bedtools_result),
         header=None,
         names="Chromosome Start End Name Score Strand".split(),
-        sep="\t")
+        sep="\t",
+    )
 
     result = gr.overlap(gr2, strandedness=strandedness)
 
     compare_results(bedtools_df, result)
 
 
-@pytest.mark.bedtools
-@pytest.mark.parametrize("strandedness", strandedness)
-@settings(
-    max_examples=max_examples,
-    deadline=deadline,
-    print_blob=True,
-    suppress_health_check=HealthCheck.all())
-@given(gr=dfs_min(), gr2=dfs_min())  # pylint: disable=no-value-for-parameter
-def test_intersect(gr, gr2, strandedness):
-
-    intersect_command = "bedtools intersect {strand} -a {f1} -b {f2}"
-
-    bedtools_result = run_bedtools(intersect_command, gr, gr2, strandedness)
-
-    bedtools_df = pd.read_csv(
-        StringIO(bedtools_result),
-        header=None,
-        names="Chromosome Start End Name Score Strand".split(),
-        sep="\t")
-
-    result = gr.intersect(gr2, strandedness=strandedness)
-
-    compare_results(bedtools_df, result)
-
-
-@pytest.mark.bedtools
+@pytest.mark.bedtools()
 @pytest.mark.parametrize("strandedness", strandedness)
 @settings(
     max_examples=max_examples,
     print_blob=True,
     deadline=deadline,
-    suppress_health_check=HealthCheck.all())
+)
 @given(gr=dfs_min(), gr2=dfs_min())  # pylint: disable=no-value-for-parameter
 # @reproduce_failure('4.15.0', b'AXicY2RABoxghAoAAGkABA==')
 # @reproduce_failure('4.15.0', b'AXicY2RABoxgxAAjQQAAAG8ABQ==')
 # @reproduce_failure('4.15.0', b'AXicY2RABqwMDIwMaAAAALkACA==')
 # @reproduce_failure('4.15.0', b'AXicY2RAA4xIJAgAAABcAAQ=')
 # reproduce_failure('4.15.0', b'AXicY2RAAEYGhv9AkhHGgQIAFHQBBQ==')
 # @reproduce_failure('4.15.0', b'AXicY2QAAUYGGGCEYIQAVAgAALUACA==')
-def test_coverage(gr, gr2, strandedness):
-
+def test_coverage(gr, gr2, strandedness) -> None:
     print(gr.df)
     print(gr2.df)
     coverage_command = "bedtools coverage {strand} -a {f1} -b {f2}"
 
     bedtools_result = run_bedtools(coverage_command, gr, gr2, strandedness)
 
     bedtools_df = pd.read_csv(
         StringIO(bedtools_result),
         header=None,
         usecols=[0, 1, 2, 3, 4, 5, 6, 9],
-        names=
-        "Chromosome Start End Name Score Strand NumberOverlaps FractionOverlaps"
-        .split(),
-        dtype={"FractionOverlap": np.float},
-        sep="\t")
+        names="Chromosome Start End Name Score Strand NumberOverlaps FractionOverlaps".split(),
+        dtype={"FractionOverlap": np.float_},
+        sep="\t",
+    )
 
     result = gr.coverage(gr2, strandedness=strandedness)
 
+    print("pyranges")
+    print(result.df)
+    print("bedtools")
+    print(bedtools_df)
+
     # assert len(result) > 0
-    assert np.all(
-        bedtools_df.NumberOverlaps.values == result.NumberOverlaps.values)
-    np.testing.assert_allclose(
-        bedtools_df.FractionOverlaps, result.FractionOverlaps, atol=1e-5)
+    assert np.all(bedtools_df.NumberOverlaps.values == result.NumberOverlaps.values)
+    np.testing.assert_allclose(bedtools_df.FractionOverlaps, result.FractionOverlaps, atol=1e-5)
     # compare_results(bedtools_df, result)
 
 
 # @pytest.mark.bedtools
 # @pytest.mark.parametrize("strandedness", strandedness)
 # @settings(
 #     max_examples=max_examples,
@@ -273,156 +237,146 @@
 #     dbg(bedtools_df)
 
 #     # result2 = gr.intersect(gr2, strandedness)
 
 #     compare_results(bedtools_df, result)
 
 
-@pytest.mark.bedtools
+@pytest.mark.bedtools()
 @pytest.mark.parametrize("strandedness", ["same", "opposite", False])  #
 @settings(
     max_examples=max_examples,
     deadline=deadline,
     print_blob=True,
-    suppress_health_check=HealthCheck.all())
+)
 @given(gr=dfs_min(), gr2=dfs_min())  # pylint: disable=no-value-for-parameter
 # @reproduce_failure('4.5.7', b'AXicLYaJCQAACIS0/YfuuQRRAbVG94Dk5LHSBgJ3ABU=')
 # @reproduce_failure('4.15.0', b'AXicY2QAAUYGGAVlIQAAAIIABQ==')
-def test_subtraction(gr, gr2, strandedness):
-
+def test_subtraction(gr, gr2, strandedness) -> None:
     subtract_command = "bedtools subtract {strand} -a {f1} -b {f2}"
 
     bedtools_result = run_bedtools(subtract_command, gr, gr2, strandedness)
 
     bedtools_df = pd.read_csv(
         StringIO(bedtools_result),
         header=None,
         names="Chromosome Start End Name Score Strand".split(),
-        sep="\t")
+        sep="\t",
+    )
 
-    result = gr.subtract(gr2, strandedness=strandedness)
+    print("subtracting" * 50)
+    result = gr.range_subtract(gr2, strandedness=strandedness)
 
+    print("bedtools_result")
     print(bedtools_df)
+    print("PyRanges result:")
     print(result)
 
     compare_results(bedtools_df, result)
 
 
 nearest_hows = [None, "upstream", "downstream"]
 overlaps = [True, False]
 
 
-@pytest.mark.bedtools
-@pytest.mark.parametrize("nearest_how,overlap,strandedness",
-                         product(nearest_hows, overlaps, strandedness))
+@pytest.mark.bedtools()
+@pytest.mark.parametrize(("nearest_how", "overlap", "strandedness"), product(nearest_hows, overlaps, strandedness))
 @settings(
     max_examples=max_examples,
     deadline=deadline,
     print_blob=True,
-    suppress_health_check=HealthCheck.all())
+)
 @given(gr=dfs_min(), gr2=dfs_min())  # pylint: disable=no-value-for-parameter
-# @reproduce_failure('4.32.2', b'AXicY2RkAAEQWf///38IByYGoYEAAFjhA4Q=')
-def test_nearest(gr, gr2, nearest_how, overlap, strandedness):
-
+def test_nearest(gr, gr2, nearest_how, overlap, strandedness) -> None:
     nearest_command = "bedtools closest {bedtools_how} {strand} {overlap} -t first -d -a <(sort -k1,1 -k2,2n {f1}) -b <(sort -k1,1 -k2,2n {f2})"
 
-    bedtools_result = run_bedtools(nearest_command, gr, gr2, strandedness,
-                                   overlap, nearest_how)
+    bedtools_result = run_bedtools(nearest_command, gr, gr2, strandedness, overlap, nearest_how)
 
     bedtools_df = pd.read_csv(
         StringIO(bedtools_result),
         header=None,
         names="Chromosome Start End Strand Chromosome2 Distance".split(),
         usecols=[0, 1, 2, 5, 6, 12],
-        sep="\t")
+        sep="\t",
+    )
 
     bedtools_df.Distance = bedtools_df.Distance.abs()
 
     bedtools_df = bedtools_df[bedtools_df.Chromosome2 != "."]
-    bedtools_df = bedtools_df.drop("Chromosome2", 1)
+    bedtools_df = bedtools_df.drop("Chromosome2", axis=1)
 
-    result = gr.nearest(
-        gr2, strandedness=strandedness, overlap=overlap, how=nearest_how)
+    result = gr.nearest(gr2, strandedness=strandedness, overlap=overlap, how=nearest_how)
 
     print("bedtools " * 5)
     print(bedtools_df)
     print("result " * 5)
     print(result)
 
     compare_results_nearest(bedtools_df, result)
 
 
-@pytest.mark.bedtools
+@pytest.mark.bedtools()
 @pytest.mark.parametrize("strandedness", no_opposite)
 @settings(
     max_examples=max_examples,
     deadline=deadline,
     print_blob=True,
-    suppress_health_check=HealthCheck.all())
+    suppress_health_check=list(HealthCheck),
+)
 @given(gr=dfs_min(), gr2=dfs_min())  # pylint: disable=no-value-for-parameter
-def test_jaccard(gr, gr2, strandedness):
-
-    """Bedtools segfaults"""
-
-    jaccard_command = "bedtools jaccard {strand}  -a <(sort -k1,1 -k2,2n {f1}) -b <(sort -k1,1 -k2,2n {f2})"
+def test_jaccard(gr, gr2, strandedness) -> None:
+    """Bedtools segfaults."""
+    jaccard_command = (  # noqa: F841
+        "bedtools jaccard {strand}  -a <(sort -k1,1 -k2,2n {f1}) -b <(sort -k1,1 -k2,2n {f2})"
+    )
 
     #     # https://github.com/arq5x/bedtools2/issues/645
     #     # will make tests proper when bedtools is fixed
     result = gr.stats.jaccard(gr2, strandedness=strandedness)
 
-
     assert 0 <= result <= 1
 
 
-
-
-@pytest.mark.bedtools
+@pytest.mark.bedtools()
 @pytest.mark.parametrize("strandedness", strandedness)
 @settings(
     max_examples=max_examples,
     deadline=deadline,
     print_blob=True,
-    suppress_health_check=HealthCheck.all())
+)
 @given(gr=dfs_min(), gr2=dfs_min())  # pylint: disable=no-value-for-parameter
-def test_join(gr, gr2, strandedness):
-
+def test_join(gr, gr2, strandedness) -> None:
     join_command = "bedtools intersect {strand} -wo -a {f1} -b {f2}"
 
     bedtools_result = run_bedtools(join_command, gr, gr2, strandedness)
 
     bedtools_df = pd.read_csv(
         StringIO(bedtools_result),
         header=None,
         sep="\t",
-        names=
-        "Chromosome Start End Name Score Strand Chromosome_b Start_b End_b Name_b Score_b Strand_b Overlap"
-        .split(),
-        dtype={
-            "Chromosome": "category",
-            "Strand": "category"
-        }).drop(
-            "Chromosome_b Overlap".split(), axis=1)
+        names="Chromosome Start End Name Score Strand Chromosome_b Start_b End_b Name_b Score_b Strand_b Overlap".split(),
+        dtype={"Chromosome": "category", "Strand": "category"},
+    ).drop("Chromosome_b Overlap".split(), axis=1)
 
-    result = gr.join(gr2, strandedness=strandedness)
+    result = gr.join_ranges(gr2, strandedness=strandedness)
 
     if result.df.empty:
         assert bedtools_df.empty
     else:
         assert_df_equal(result.df, bedtools_df)
 
 
-@pytest.mark.bedtools
+@pytest.mark.bedtools()
 @settings(
     max_examples=max_examples,
     deadline=deadline,
     print_blob=True,
-    suppress_health_check=HealthCheck.all())
+)
 @given(gr=dfs_min2(), gr2=dfs_min2())  # pylint: disable=no-value-for-parameter
-def test_reldist(gr, gr2):
-
+def test_reldist(gr, gr2) -> None:
     reldist_command = "bedtools reldist -a <(sort -k1,1 -k2,2n {f1}) -b <(sort -k1,1 -k2,2n {f2})"
 
     bedtools_result = run_bedtools(reldist_command, gr, gr2, False)
     bedtools_result = pd.read_csv(StringIO(bedtools_result), sep="\t")
 
     print("bedtools_result")
     print(bedtools_result.reldist)
@@ -494,65 +448,69 @@
 
 k_nearest_ties = ["first", "last", None]
 # k_nearest_ties = ["first", None]
 k_nearest_ties = ["last"]
 
 k_nearest_params = reversed(list(product(nearest_hows, [True, False], strandedness, k_nearest_ties)))
 
-@pytest.mark.bedtools
-@pytest.mark.explore
-@pytest.mark.parametrize("nearest_how,overlap,strandedness,ties", k_nearest_params) #
-@settings(
-    max_examples=max_examples,
-    deadline=deadline,
-    print_blob=True,
-    suppress_health_check=HealthCheck.all())
-@given(gr=dfs_min(), gr2=dfs_min())  # pylint: disable=no-value-for-parameter
-# @reproduce_failure('4.43.5', b'AXicY2RAA4zoTAAAWwAE')
-def test_k_nearest(gr, gr2, nearest_how, overlap, strandedness, ties):
-
-    print("-----" * 20)
-
-    # gr = gr.apply(lambda df: df.astype({"Start": np.int32, "End": np.int32}))
-    # gr2 = gr2.apply(lambda df: df.astype({"Start": np.int32, "End": np.int32}))
-
-    # print(gr)
-    # print(gr2)
-
-    nearest_command = "bedtools closest -k 2 {bedtools_how} {strand} {overlap} {ties} -a <(sort -k1,1 -k2,2n {f1}) -b <(sort -k1,1 -k2,2n {f2})"
-
-    bedtools_result = run_bedtools(nearest_command, gr, gr2, strandedness,
-                                   overlap, nearest_how, ties)
-
-    bedtools_df = pd.read_csv(
-        StringIO(bedtools_result),
-        header=None,
-        names="Chromosome Start End Strand Chromosome2 Distance".split(),
-        usecols=[0, 1, 2, 5, 6, 12],
-        sep="\t")
-
-    bedtools_df.Distance = bedtools_df.Distance.abs()
-
-    bedtools_df = bedtools_df[bedtools_df.Chromosome2 != "."]
-    bedtools_df = bedtools_df.drop("Chromosome2", 1)
-
-    # cannot test with k > 1 because bedtools algo has different syntax
-    # cannot test keep_duplicates "all" or None/False properly, as the semantics is different for bedtools
-    result = gr.k_nearest(
-        gr2, k=2, strandedness=strandedness, overlap=overlap, how=nearest_how, ties=ties)
-
-    # result = result.apply(lambda df: df.astype({"Start": np.int64, "End": np.int64, "Distance": np.int64}))
-    if len(result):
-        result.Distance = result.Distance.abs()
-    print("bedtools " * 5)
-    print(bedtools_df)
-    print("result " * 5)
-    print(result)
 
-    compare_results_nearest(bedtools_df, result)
+# @pytest.mark.bedtools
+# @pytest.mark.explore
+# @pytest.mark.parametrize("nearest_how,overlap,strandedness,ties", k_nearest_params)  #
+# @settings(
+#     max_examples=max_examples,
+#     deadline=deadline,
+#     print_blob=True,
+#     suppress_health_check=HealthCheck.all(),
+# )
+# @given(gr=dfs_min(), gr2=dfs_min())  # pylint: disable=no-value-for-parameter
+# # @reproduce_failure('4.43.5', b'AXicY2RAA4zoTAAAWwAE')
+# def test_k_nearest(gr, gr2, nearest_how, overlap, strandedness, ties):
+#     print("-----" * 20)
+#
+#     # gr = gr.apply(lambda df: df.astype({"Start": np.int32, "End": np.int32}))
+#     # gr2 = gr2.apply(lambda df: df.astype({"Start": np.int32, "End": np.int32}))
+#
+#     # print(gr)
+#     # print(gr2)
+#
+#     nearest_command = "bedtools closest -k 2 {bedtools_how} {strand} {overlap} {ties} -a <(sort -k1,1 -k2,2n {f1}) -b <(sort -k1,1 -k2,2n {f2})"
+#
+#     bedtools_result = run_bedtools(
+#         nearest_command, gr, gr2, strandedness, overlap, nearest_how, ties
+#     )
+#
+#     bedtools_df = pd.read_csv(
+#         StringIO(bedtools_result),
+#         header=None,
+#         names="Chromosome Start End Strand Chromosome2 Distance".split(),
+#         usecols=[0, 1, 2, 5, 6, 12],
+#         sep="\t",
+#     )
+#
+#     bedtools_df.Distance = bedtools_df.Distance.abs()
+#
+#     bedtools_df = bedtools_df[bedtools_df.Chromosome2 != "."]
+#     bedtools_df = bedtools_df.drop("Chromosome2", axis=1)
+#
+#     # cannot test with k > 1 because bedtools algo has different syntax
+#     # cannot test keep_duplicates "all" or None/False properly, as the semantics is different for bedtools
+#     result = gr.k_nearest(
+#         gr2, k=2, strandedness=strandedness, overlap=overlap, how=nearest_how, ties=ties
+#     )
+#
+#     # result = result.apply(lambda df: df.astype({"Start": np.int64, "End": np.int64, "Distance": np.int64}))
+#     if len(result):
+#         result.Distance = result.Distance.abs()
+#     print("bedtools " * 5)
+#     print(bedtools_df)
+#     print("result " * 5)
+#     print(result)
+#
+#     compare_results_nearest(bedtools_df, result)
 
 
 # @settings(
 #     max_examples=max_examples,
 #     deadline=deadline,
 #     print_blob=True,
 #     suppress_health_check=HealthCheck.all())
@@ -560,25 +518,26 @@
 # def test_k_nearest_nearest_self_same_size(gr):
 
 #     result = gr.k_nearest(
 #         gr, k=1, strandedness=None, overlap=True, how=None, ties="first")
 
 #     assert len(result) == len(gr)
 
-@settings(
-    max_examples=max_examples,
-    deadline=deadline,
-    print_blob=True,
-    suppress_health_check=HealthCheck.all())
-@given(gr=dfs_min(), gr2=dfs_min())  # pylint: disable=no-value-for-parameter
-def test_k_nearest_1_vs_nearest(gr, gr2):
-
-    result_k = gr.k_nearest(gr2, k=1, strandedness=None, overlap=True, how=None)
-    if len(result_k) > 0:
-        result_k.Distance = result_k.Distance.abs()
-
-    result_n = gr.nearest(gr2, strandedness=None, overlap=True, how=None)
 
-    if len(result_k) == 0 and len(result_n) == 0:
-        pass
-    else:
-        assert (result_k.sort().Distance.abs() == result_n.sort().Distance).all()
+# @settings(
+#     max_examples=max_examples,
+#     deadline=deadline,
+#     print_blob=True,
+#     suppress_health_check=HealthCheck.all(),
+# )
+# @given(gr=dfs_min(), gr2=dfs_min())  # pylint: disable=no-value-for-parameter
+# def test_k_nearest_1_vs_nearest(gr, gr2):
+#     result_k = gr.k_nearest(gr2, k=1, strandedness=None, overlap=True, how=None)
+#     if len(result_k) > 0:
+#         result_k.Distance = result_k.Distance.abs()
+#
+#     result_n = gr.nearest(gr2, strandedness=None, overlap=True, how=None)
+#
+#     if len(result_k) == 0 and len(result_n) == 0:
+#         pass
+#     else:
+#         assert (result_k.sort().Distance.abs() == result_n.sort().Distance).all()
```

### Comparing `pyranges-0.0.99/tests/test_do_not_error.py` & `pyranges-0.1.0/tests/property_based/test_do_not_error.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,93 @@
-import pytest
-
-from hypothesis import given, settings, HealthCheck
-from hypothesis import reproduce_failure  # pylint: disable=unused-import
-
 from itertools import product
 
 import numpy as np
+import pytest
+from hypothesis import HealthCheck, given, settings
 
-from tests.hypothesis_helper import dfs_min2, dfs_no_min
-
-from os import environ
-
-if environ.get("TRAVIS"):
-    max_examples = 10
-    deadline = None
-else:
-    max_examples = 100
-    deadline = None
+from tests.property_based.hypothesis_helper import deadline, dfs_no_min, max_examples
 
 strandedness = [False, "same", "opposite"]
 
 binary_methods = [
-    "set_union", "set_intersect", "overlap", "nearest", "intersect",
-    "subtract", "join"
+    "set_union",
+    "set_intersect",
+    "overlap",
+    "nearest",
+    "intersect",
+    "subtract",
+    "join",
 ]
 
 unary_methods = [
-    "merge", "sort", "cluster", "pc", "mpc", "spc", "drop_duplicate_positions",
-    "drop"
+    "merge",
+    "sort",
+    "cluster",
+    "pc",
+    "mpc",
+    "spc",
+    "drop_duplicate_positions",
+    "drop",
 ]
 
 method_chain = product(binary_methods, binary_methods)
 # cannot start with an operation that makes pyrange unstranded and then try a stranded op
-strandedness_chain = list(product(["same", "opposite"], strandedness)) + list(
-    product(strandedness, [None]))
+strandedness_chain = list(product(["same", "opposite"], strandedness)) + list(product(strandedness, [None]))
 
 
-@pytest.mark.bedtools
-@pytest.mark.parametrize("strandedness_chain,method_chain",
-                         product(strandedness_chain, method_chain))
+@pytest.mark.bedtools()
+@pytest.mark.parametrize(("strandedness_chain", "method_chain"), product(strandedness_chain, method_chain))
 @settings(
     max_examples=max_examples,
     deadline=deadline,
     print_blob=True,
-    suppress_health_check=HealthCheck.all())
+    suppress_health_check=HealthCheck.all(),
+)
 @given(gr=dfs_no_min(), gr2=dfs_no_min(), gr3=dfs_no_min())  # pylint: disable=no-value-for-parameter
 # @reproduce_failure('5.5.4', b'AXicY2RAA4xIJCoLygcAALIABg==') # test_three_in_a_row[strandedness_chain122-method_chain122]
 # @reproduce_failure('5.5.4', b'AXicY2QAAUYGKGBkxM9nAAABEAAJ') # test_three_in_a_row[strandedness_chain45-method_chain45]
 # @reproduce_failure('5.5.4', b'AXicY2RAA4xIJDY+AAC2AAY=') # test_three_in_a_row[strandedness_chain24-method_chain24]
-def test_three_in_a_row(gr, gr2, gr3, strandedness_chain, method_chain):
+def test_three_in_a_row(gr, gr2, gr3, strandedness_chain, method_chain) -> None:
+    print(method_chain)
 
     s1, s2 = strandedness_chain
     f1, f2 = method_chain
 
     suffix_methods = ["nearest", "join"]
 
     if f1 in suffix_methods and f2 in suffix_methods:
-
         m1 = getattr(gr, f1)
         gr2 = m1(gr2, strandedness=s1)
         if len(gr2) > 0:
             assert gr2.Start.dtype == np.int64
-            assert (gr2.Start >= 0).all() and (gr2.End >= 0).all()
+            assert (gr2.Start >= 0).all()
+            assert (gr2.End >= 0).all()
         m2 = getattr(gr2, f2)
         gr3 = m2(gr3, strandedness=s2, suffix="_c")
         print(gr3)
         if len(gr3) > 0:
             assert gr3.Start.dtype == np.int64
-            assert (gr3.Start >= 0).all() and (gr3.End >= 0).all()
+            assert (gr3.Start >= 0).all()
+            assert (gr3.End >= 0).all()
 
     else:
-
         m1 = getattr(gr, f1)
         gr2 = m1(gr2, strandedness=s1)
         if len(gr2) > 0:
             assert gr2.Start.dtype == np.int64
-            assert (gr2.Start >= 0).all() and (gr2.End >= 0).all()
+            assert (gr2.Start >= 0).all()
+            assert (gr2.End >= 0).all()
         m2 = getattr(gr2, f2)
         gr3 = m2(gr3, strandedness=s2)
         print(gr3)
         if len(gr3) > 0:
             assert gr3.Start.dtype == np.int64
-            assert (gr3.Start >= 0).all() and (gr3.End >= 0).all()
+            assert (gr3.Start >= 0).all()
+            assert (gr3.End >= 0).all()
+
 
 # @pytest.mark.bedtools
 # @pytest.mark.parametrize("strandedness_chain,method_chain",
 #                          product(strandedness_chain, method_chain))
 # @settings(
 #     max_examples=max_examples,
 #     deadline=deadline,
```

### Comparing `pyranges-0.0.99/tests/test_guessers.py` & `pyranges-0.1.0/tests/unit/test_guessers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # import pytest
 
 # from io import StringIO
 
 # import pyranges as pr
 
 # from pyranges.guessers import (parse_file, guess_columns, guess_chromosome, guess_strand, guess_start_end, guess_delim)
@@ -34,16 +33,14 @@
 
 # def test_guess_delim(gtf_file):
 
 #     delim = guess_delim(gtf_file).encode()
 #     assert delim == " ".encode() # this is the wrong guess
 
 
-
-
 # def test_guess_strand(bed_df, number_unique):
 
 #     result = guess_strand(bed_df, number_unique, "Start", "End")
 
 #     assert result == "Strand"
```

### Comparing `pyranges-0.0.99/tests/test_unary.py` & `pyranges-0.1.0/tests/property_based/test_unary.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,189 +1,193 @@
-import pytest
-from natsort import natsorted
-
-from hypothesis import given, settings, HealthCheck  #, assume
-from hypothesis import reproduce_failure  # pylint: disable=unused-import
-
-import tempfile
 import subprocess  # nosec
+import tempfile
 from io import StringIO
 
 import numpy as np
-
 import pandas as pd
-
-from tests.helpers import assert_df_equal
-from tests.hypothesis_helper import dfs_min, df_data, selector, dfs_min_with_id, max_examples, deadline
+import pytest
+from hypothesis import (
+    HealthCheck,
+    given,
+    reproduce_failure,  # noqa: F401
+    settings,
+)
+from natsort import natsorted  # type: ignore
 
 import pyranges as pr
+from tests.helpers import assert_df_equal
+from tests.property_based.hypothesis_helper import (
+    deadline,
+    df_data,
+    dfs_min,
+    dfs_min_with_id,
+    max_examples,
+    selector,
+)
 
 # if environ.get("TRAVIS"):
 #     max_examples = 100
 #     deadline = None
 # else:
 #     max_examples = 1000
 #     deadline = None
 
 merge_command = "bedtools merge -o first,count -c 6,1 {} -i <(sort -k1,1 -k2,2n {})"
 
 
-@pytest.mark.bedtools
+@pytest.mark.bedtools()
 @pytest.mark.parametrize("strand", [True, False])
 @settings(
     max_examples=max_examples,
     deadline=deadline,
-    suppress_health_check=HealthCheck.all())
+    suppress_health_check=HealthCheck.all(),
+)
 @given(gr=dfs_min())  # pylint: disable=no-value-for-parameter
-def test_merge(gr, strand):
-
+def test_merge(gr, strand) -> None:
     bedtools_strand = {True: "-s", False: ""}[strand]
 
     print(gr)
 
     with tempfile.TemporaryDirectory() as temp_dir:
-        f1 = "{}/f1.bed".format(temp_dir)
+        f1 = f"{temp_dir}/f1.bed"
         gr.df.to_csv(f1, sep="\t", header=False, index=False)
 
         cmd = merge_command.format(bedtools_strand, f1)
         print(cmd)
 
         # ignoring bandit security warning. All strings created by test suite
-        result = subprocess.check_output(  # nosec
-            cmd, shell=True, executable="/bin/bash").decode()  # nosec
+        result = subprocess.check_output(cmd, shell=True, executable="/bin/bash").decode()  # nosec  # nosec
 
         print("result" * 10)
         print(result)
 
         if not strand:
             print("if not " * 10)
             bedtools_df = pd.read_csv(
                 StringIO(result),
                 sep="\t",
                 header=None,
                 usecols=[0, 1, 2, 4],
                 names="Chromosome Start End Count".split(),
-                dtype={"Chromosome": "category"})
+                dtype={"Chromosome": "category"},
+            )
         else:
             bedtools_df = pd.read_csv(
                 StringIO(result),
                 sep="\t",
                 header=None,
                 names="Chromosome Start End Strand Count".split(),
-                dtype={"Chromosome": "category"})
+                dtype={"Chromosome": "category"},
+            )
 
     print("bedtools_df\n", bedtools_df)
-    result = gr.merge(strand=strand, count=True)
+    result = gr.merge_overlaps(use_strand=strand)
     print("result\n", result.df)
 
     if not bedtools_df.empty:
         # need to sort because bedtools sometimes gives the result in non-natsorted chromosome order!
-        if result.stranded:
+        if result.strand_valid:
             assert_df_equal(
                 result.df.sort_values("Chromosome Start Strand".split()),
-                bedtools_df.sort_values("Chromosome Start Strand".split()))
+                bedtools_df.sort_values("Chromosome Start Strand".split()),
+            )
         else:
             assert_df_equal(
                 result.df.sort_values("Chromosome Start".split()),
-                bedtools_df.sort_values("Chromosome Start".split()))
+                bedtools_df.sort_values("Chromosome Start".split()),
+            )
     else:
         assert bedtools_df.empty == result.df.empty
 
 
 cluster_command = "bedtools cluster {} -i <(sort -k1,1 -k2,2n {})"
 
 
-@pytest.mark.bedtools
+@pytest.mark.bedtools()
 @pytest.mark.parametrize("strand", [True, False])
 @settings(
     max_examples=max_examples,
     deadline=deadline,
-    suppress_health_check=HealthCheck.all())
+    suppress_health_check=HealthCheck.all(),
+)
 @given(gr=dfs_min())  # pylint: disable=no-value-for-parameter
-def test_cluster(gr, strand):
-
+def test_cluster(gr, strand) -> None:
     bedtools_strand = {True: "-s", False: ""}[strand]
 
     print(gr)
 
     with tempfile.TemporaryDirectory() as temp_dir:
-        f1 = "{}/f1.bed".format(temp_dir)
+        f1 = f"{temp_dir}/f1.bed"
         gr.df.to_csv(f1, sep="\t", header=False, index=False)
 
         cmd = cluster_command.format(bedtools_strand, f1)
         print(cmd)
 
         # ignoring bandit security warning. All strings created by test suite
-        result = subprocess.check_output(  # nosec
-            cmd, shell=True, executable="/bin/bash").decode()  # nosec
+        result = subprocess.check_output(cmd, shell=True, executable="/bin/bash").decode()  # nosec  # nosec
 
         bedtools_df = pd.read_csv(
             StringIO(result),
             sep="\t",
             header=None,
-            squeeze=True,
             names="Chromosome Start End Name Score Strand Cluster".split(),
-            dtype={"Chromosome": "category"})
+            dtype={"Chromosome": "category"},
+        )
 
     print("bedtools_df\n", bedtools_df)
 
-    # from pydbg import dbg
-    # dbg(gr.cluster(strand=strand))
-
     print("gr\n", gr)
-    result = gr.cluster(strand=strand)
+    result = gr.cluster(use_strand=strand)
     print("result\n", result[["Cluster"]])
     print("result\n", result.df)
 
     if not bedtools_df.empty:
         # need to sort because bedtools sometimes gives the result in non-natsorted chromosome order!
-        if result.stranded:
-            sort_values = "Chromosome Start Strand".split()
-        else:
-            sort_values = "Chromosome Start".split()
+        sort_values = "Chromosome Start Strand".split() if result.strand_valid else "Chromosome Start".split()
 
         result_df = result.df.sort_values(sort_values)
+        print(bedtools_df)
         bedtools_df = bedtools_df.sort_values(sort_values)
 
-        cluster_ids = {
-            k: v
-            for k, v in zip(result_df.Cluster.drop_duplicates(),
-                            bedtools_df.Cluster.drop_duplicates())
-        }
+        cluster_ids = dict(
+            zip(
+                result_df.Cluster.drop_duplicates(),
+                bedtools_df.Cluster.drop_duplicates(),
+            ),
+        )
 
         # bedtools gives different cluster ids than pyranges
-        result_df.Cluster.replace(cluster_ids, inplace=True)
-        assert_df_equal(result_df, bedtools_df)
+        result_df.Cluster = result_df.Cluster.replace(cluster_ids)
+
+        bedtools_df.Cluster = bedtools_df.Cluster.astype("int32")
+        assert_df_equal(result_df.drop("Cluster", axis=1), bedtools_df.drop("Cluster", axis=1))
     else:
         assert bedtools_df.empty == result.df.empty
 
 
 @pytest.mark.parametrize("strand", [True, False])
 @settings(
     max_examples=max_examples,
     deadline=deadline,
-    suppress_health_check=HealthCheck.all())
+    suppress_health_check=HealthCheck.all(),
+)
 @given(gr=dfs_min_with_id())  # pylint: disable=no-value-for-parameter
-def test_cluster_by(gr, strand):
-
-    result = gr.cluster(by="ID", strand=strand).df
+def test_cluster_by(gr, strand) -> None:
+    result = gr.cluster(use_strand=strand, by="ID").df
     print(result)
     df = gr.df
 
-    if strand:
-        groupby = ["Chromosome", "Strand", "ID"]
-    else:
-        groupby = ["Chromosome", "ID"]
+    groupby = ["Chromosome", "Strand", "ID"] if strand else ["Chromosome", "ID"]
 
     grs = []
 
     for _, gdf in natsorted(df.groupby(groupby)):
         grs.append(pr.PyRanges(gdf))
 
-    clusters = [gr.cluster(strand=strand) for gr in grs]
+    clusters = [gr.cluster(use_strand=strand) for gr in grs]
     i = 1
     new_clusters = []
     for c in clusters:
         print("c")
         print(c)
         c.Cluster = i
         i += 1
@@ -192,133 +196,132 @@
     expected = pr.concat(new_clusters).df
     expected.loc[:, "Cluster"] = expected.Cluster.astype(np.int32)
     # expected = expected.drop_duplicates()
 
     print(expected)
     print(result)
 
-    assert_df_equal(result, expected)
+    assert_df_equal(result.drop("Cluster", axis=1), expected.drop("Cluster", axis=1))
 
 
 @pytest.mark.parametrize("strand", [True, False])
 @settings(
     max_examples=max_examples,
     deadline=deadline,
-    suppress_health_check=HealthCheck.all())
+    suppress_health_check=HealthCheck.all(),
+)
 @given(gr=dfs_min_with_id())  # pylint: disable=no-value-for-parameter
-def test_merge_by(gr, strand):
-
+def test_merge_by(gr, strand) -> None:
     print(gr)
-    result = gr.merge(by="ID").df.drop("ID", axis=1)
+    result = gr.merge_overlaps(by="ID").df.drop("ID", axis=1)
 
     df = gr.df
 
     grs = []
     for _, gdf in df.groupby("ID"):
         grs.append(pr.PyRanges(gdf))
 
-    expected = pr.concat([gr.merge() for gr in grs]).df
+    expected = pr.concat([gr.merge_overlaps() for gr in grs]).df
 
     print(expected)
     print(result)
 
     assert_df_equal(result, expected)
 
 
 makewindows_command = "bedtools makewindows -w 10 -b <(sort -k1,1 -k2,2n {})"
 
 
-@pytest.mark.bedtools
+@pytest.mark.bedtools()
 @settings(
     max_examples=max_examples,
     print_blob=True,
     deadline=deadline,
-    suppress_health_check=HealthCheck.all())
+    suppress_health_check=HealthCheck.all(),
+)
 @given(gr=dfs_min())  # pylint: disable=no-value-for-parameter
 # @reproduce_failure('5.5.4', b'AXicY2RgYGAEIzgAsRkBAFsABg==')
-def test_windows(gr):
-
+def test_windows(gr) -> None:
     with tempfile.TemporaryDirectory() as temp_dir:
-        f1 = "{}/f1.bed".format(temp_dir)
+        f1 = f"{temp_dir}/f1.bed"
         gr.df.to_csv(f1, sep="\t", header=False, index=False)
 
         cmd = makewindows_command.format(f1)
         print(cmd)
 
         # ignoring bandit security warning. All strings created by test suite
-        result = subprocess.check_output(  # nosec
-            cmd, shell=True, executable="/bin/bash").decode()  # nosec
+        result = subprocess.check_output(cmd, shell=True, executable="/bin/bash").decode()  # nosec  # nosec
 
         bedtools_df = pd.read_csv(
             StringIO(result),
             sep="\t",
             header=None,
-            squeeze=True,
             names="Chromosome Start End".split(),
-            dtype={"Chromosome": "category"})
+            dtype={"Chromosome": "category"},
+        )
 
     print("bedtools_df\n", bedtools_df)
 
-    result = gr.window(10)["Chromosome Start End".split()].unstrand()
+    result = gr.window(10)["Chromosome Start End".split()].remove_strand()
     print("result\n", result.df)
 
     if not bedtools_df.empty:
         assert_df_equal(result.df, bedtools_df)
     else:
         assert bedtools_df.empty == result.df.empty
 
 
 @pytest.mark.parametrize("strand", [True, False])
 @settings(
     max_examples=max_examples,
     deadline=deadline,
-    suppress_health_check=HealthCheck.all())
+    suppress_health_check=HealthCheck.all(),
+)
 @given(gr=df_data())  # pylint: disable=no-value-for-parameter
-def test_init(gr, strand):
-
+def test_init(gr, strand) -> None:
     c, s, e, strands = gr
 
     if strand:
         pr.PyRanges(chromosomes=c, starts=s, ends=e, strands=strands)
     else:
         pr.PyRanges(chromosomes=c, starts=s, ends=e)
 
 
-chipseq = pr.data.chipseq()
+chipseq = pr.example_data.chipseq()
 
 
 @settings(
     max_examples=max_examples,
     deadline=deadline,
-    suppress_health_check=HealthCheck.all())
+    suppress_health_check=HealthCheck.all(),
+)
 @given(selector=selector())  # pylint: disable=no-value-for-parameter
-def test_getitem(selector):
-
-    # have these weird returns to avoid being flagged as unused code
+def test_getitem(selector) -> None:
     if len(selector) == 3:
         a, b, c = selector
-        return chipseq[a, b, c]
+        chipseq[a, b, c]
     elif len(selector) == 2:
         a, b = selector
-        return chipseq[a, b]
+        chipseq[a, b]
     elif len(selector) == 1:
         a = selector[0]
-        return chipseq[a]
+        chipseq[a]
     elif len(selector) == 0:
         pass
     else:
-        raise Exception("Should never happen")
+        msg = "Should never happen"
+        raise Exception(msg)
 
 
-@pytest.mark.bedtools
+@pytest.mark.bedtools()
 @settings(
     max_examples=max_examples,
     deadline=deadline,
     print_blob=True,
-    suppress_health_check=HealthCheck.all())
+    suppress_health_check=HealthCheck.all(),
+)
 @given(gr=dfs_min())  # pylint: disable=no-value-for-parameter
-def test_summary(gr):
-
+def test_summary(gr) -> None:
     print(gr.to_example())
     # merely testing that it does not error
     # contents are just (pandas) dataframe.describe()
     gr.summary()
```

