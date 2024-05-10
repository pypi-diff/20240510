# Comparing `tmp/nanomotif-0.3.1.tar.gz` & `tmp/nanomotif-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomotif-0.3.1.tar", last modified: Mon May  6 09:14:25 2024, max compression
+gzip compressed data, was "nanomotif-0.4.0.tar", last modified: Fri May 10 11:39:11 2024, max compression
```

## Comparing `nanomotif-0.3.1.tar` & `nanomotif-0.4.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.588185 nanomotif-0.3.1/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1084 2023-09-06 10:54:37.000000 nanomotif-0.3.1/LICENSE
--rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7384 2024-05-06 09:14:25.584185 nanomotif-0.3.1/PKG-INFO
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6828 2024-05-06 09:04:24.000000 nanomotif-0.3.1/README.md
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.424185 nanomotif-0.3.1/nanomotif/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      278 2024-01-23 08:11:50.000000 nanomotif-0.3.1/nanomotif/__init__.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       22 2024-05-06 09:12:23.000000 nanomotif-0.3.1/nanomotif/_version.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    11018 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/argparser.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6016 2024-02-20 08:34:47.000000 nanomotif-0.3.1/nanomotif/bin_consensus.py
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.444185 nanomotif-0.3.1/nanomotif/binnary/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/binnary/__init__.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    13167 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/binnary/analysis.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    15629 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/binnary/data_processing.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3729 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/binnary/detect_contamination.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3014 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/binnary/include_contigs.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      890 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/binnary/logging.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     9127 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/binnary/scoring.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      522 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/binnary/utils.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    14165 2024-02-07 10:11:10.000000 nanomotif-0.3.1/nanomotif/candidate.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1078 2024-05-03 08:31:51.000000 nanomotif-0.3.1/nanomotif/constants.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1698 2023-11-17 10:28:11.000000 nanomotif-0.3.1/nanomotif/dataload.py
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.448185 nanomotif-0.3.1/nanomotif/datasets/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       27 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/datasets/geobacillus-contig-bin.tsv
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)   176247 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164) 26479844 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/datasets/geobacillus-plasmids.pileup.bed
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1106 2024-03-29 17:11:23.000000 nanomotif-0.3.1/nanomotif/datasets.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    28603 2024-05-03 08:31:52.000000 nanomotif-0.3.1/nanomotif/evaluate.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      539 2023-10-03 09:15:12.000000 nanomotif-0.3.1/nanomotif/feature.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      321 2023-11-19 13:30:13.000000 nanomotif-0.3.1/nanomotif/logger.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    19493 2024-05-06 09:04:24.000000 nanomotif-0.3.1/nanomotif/main.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1037 2024-02-19 12:26:57.000000 nanomotif-0.3.1/nanomotif/model.py
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.568185 nanomotif-0.3.1/nanomotif/mtase_linker/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       47 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/mtase_linker/__init__.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     5051 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/mtase_linker/command.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3615 2024-05-06 09:04:17.000000 nanomotif-0.3.1/nanomotif/mtase_linker/dependencies.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     5639 2023-10-16 10:50:49.000000 nanomotif-0.3.1/nanomotif/old_search_method.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      850 2024-01-23 09:46:13.000000 nanomotif-0.3.1/nanomotif/parallel.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6202 2024-02-07 10:11:10.000000 nanomotif-0.3.1/nanomotif/postprocess.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7193 2024-01-23 11:48:10.000000 nanomotif-0.3.1/nanomotif/scoremotifs.py
--rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      197 2024-01-23 07:18:32.000000 nanomotif-0.3.1/nanomotif/seed.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    20090 2024-02-19 12:26:57.000000 nanomotif-0.3.1/nanomotif/seq.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2677 2024-02-26 13:37:04.000000 nanomotif-0.3.1/nanomotif/utils.py
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.584185 nanomotif-0.3.1/nanomotif.egg-info/
--rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7384 2024-05-06 09:14:25.000000 nanomotif-0.3.1/nanomotif.egg-info/PKG-INFO
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1714 2024-05-06 09:14:25.000000 nanomotif-0.3.1/nanomotif.egg-info/SOURCES.txt
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        1 2024-05-06 09:14:25.000000 nanomotif-0.3.1/nanomotif.egg-info/dependency_links.txt
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       50 2024-05-06 09:14:25.000000 nanomotif-0.3.1/nanomotif.egg-info/entry_points.txt
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        1 2023-09-07 09:00:46.000000 nanomotif-0.3.1/nanomotif.egg-info/not-zip-safe
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      150 2024-05-06 09:14:25.000000 nanomotif-0.3.1/nanomotif.egg-info/requires.txt
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       16 2024-05-06 09:14:25.000000 nanomotif-0.3.1/nanomotif.egg-info/top_level.txt
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)       38 2024-05-06 09:14:25.588185 nanomotif-0.3.1/setup.cfg
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      947 2024-05-06 09:04:17.000000 nanomotif-0.3.1/setup.py
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.576185 nanomotif-0.3.1/tests/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2023-10-17 07:22:50.000000 nanomotif-0.3.1/tests/__init__.py
-drwxrwxr-x   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-06 09:14:25.584185 nanomotif-0.3.1/tests/binnary/
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/__init__.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2089 2024-05-06 09:04:17.000000 nanomotif-0.3.1/tests/binnary/conftest.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1019 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/test_arg_parser.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)    11132 2024-05-06 09:04:17.000000 nanomotif-0.3.1/tests/binnary/test_cli_commands.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     6352 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/test_data_processing_functions.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2585 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/test_detect_contamination.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1404 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/test_generate_output.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2132 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/test_include_contigs.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     3317 2024-05-06 09:04:17.000000 nanomotif-0.3.1/tests/binnary/test_scoring.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)      744 2024-03-29 17:11:23.000000 nanomotif-0.3.1/tests/binnary/test_utils.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     5405 2024-05-06 09:04:17.000000 nanomotif-0.3.1/tests/binnary/test_write_bins.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     7236 2023-11-17 09:23:51.000000 nanomotif-0.3.1/tests/test_candidate.py
--rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     1365 2024-01-23 08:24:14.000000 nanomotif-0.3.1/tests/test_dataload.py
--rw-r--r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)     2933 2024-01-23 09:52:43.000000 nanomotif-0.3.1/tests/test_motif_find.py
--rw-rw-r--   0 lx38ll@bio.aau.dk (232164) lx38ll@bio.aau.dk (232164)        0 2024-05-02 08:30:14.000000 nanomotif-0.3.1/tests/test_motif_score.py
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.674436 nanomotif-0.4.0/
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1084 2023-11-30 15:56:56.000000 nanomotif-0.4.0/LICENSE
+-rw-r--r--   0 shei      (1000) shei      (1000)     7424 2024-05-10 11:39:11.674436 nanomotif-0.4.0/PKG-INFO
+-rw-rw-r--   0 shei      (1000) shei      (1000)     6868 2024-05-10 11:37:33.000000 nanomotif-0.4.0/README.md
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.646436 nanomotif-0.4.0/nanomotif/
+-rw-rw-r--   0 shei      (1000) shei      (1000)      278 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/__init__.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)       22 2024-05-10 11:37:33.000000 nanomotif-0.4.0/nanomotif/_version.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    11266 2024-05-10 11:37:33.000000 nanomotif-0.4.0/nanomotif/argparser.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     6016 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/bin_consensus.py
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.650436 nanomotif-0.4.0/nanomotif/binnary/
+-rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/binnary/__init__.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    13167 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/binnary/analysis.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    15629 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/binnary/data_processing.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     3729 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/binnary/detect_contamination.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     3014 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/binnary/include_contigs.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      890 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/binnary/logging.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     9127 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/binnary/scoring.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      522 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/binnary/utils.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    14165 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/candidate.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1078 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/constants.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1698 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/dataload.py
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.650436 nanomotif-0.4.0/nanomotif/datasets/
+-rw-rw-r--   0 shei      (1000) shei      (1000)       27 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/datasets/geobacillus-contig-bin.tsv
+-rw-rw-r--   0 shei      (1000) shei      (1000)   176247 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/datasets/geobacillus-plasmids.assembly.fasta
+-rw-rw-r--   0 shei      (1000) shei      (1000) 26479844 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/datasets/geobacillus-plasmids.pileup.bed
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1106 2024-03-29 17:14:10.000000 nanomotif-0.4.0/nanomotif/datasets.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    28603 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/evaluate.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      539 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/feature.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      321 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/logger.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    19809 2024-05-10 11:37:33.000000 nanomotif-0.4.0/nanomotif/main.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1037 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/model.py
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.674436 nanomotif-0.4.0/nanomotif/mtase_linker/
+-rw-rw-r--   0 shei      (1000) shei      (1000)       47 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/mtase_linker/__init__.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     5051 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/mtase_linker/command.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     3615 2024-05-10 09:55:21.000000 nanomotif-0.4.0/nanomotif/mtase_linker/dependencies.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     5639 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/old_search_method.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      850 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/parallel.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     6202 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/postprocess.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     7193 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/scoremotifs.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      197 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/seed.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    20090 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/seq.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     2677 2024-03-29 12:58:11.000000 nanomotif-0.4.0/nanomotif/utils.py
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.674436 nanomotif-0.4.0/nanomotif.egg-info/
+-rw-r--r--   0 shei      (1000) shei      (1000)     7424 2024-05-10 11:39:11.000000 nanomotif-0.4.0/nanomotif.egg-info/PKG-INFO
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1714 2024-05-10 11:39:11.000000 nanomotif-0.4.0/nanomotif.egg-info/SOURCES.txt
+-rw-rw-r--   0 shei      (1000) shei      (1000)        1 2024-05-10 11:39:11.000000 nanomotif-0.4.0/nanomotif.egg-info/dependency_links.txt
+-rw-rw-r--   0 shei      (1000) shei      (1000)       50 2024-05-10 11:39:11.000000 nanomotif-0.4.0/nanomotif.egg-info/entry_points.txt
+-rw-rw-r--   0 shei      (1000) shei      (1000)        1 2023-11-30 15:56:57.000000 nanomotif-0.4.0/nanomotif.egg-info/not-zip-safe
+-rw-rw-r--   0 shei      (1000) shei      (1000)      150 2024-05-10 11:39:11.000000 nanomotif-0.4.0/nanomotif.egg-info/requires.txt
+-rw-rw-r--   0 shei      (1000) shei      (1000)       16 2024-05-10 11:39:11.000000 nanomotif-0.4.0/nanomotif.egg-info/top_level.txt
+-rw-rw-r--   0 shei      (1000) shei      (1000)       38 2024-05-10 11:39:11.678436 nanomotif-0.4.0/setup.cfg
+-rw-rw-r--   0 shei      (1000) shei      (1000)      947 2024-05-10 09:55:21.000000 nanomotif-0.4.0/setup.py
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.674436 nanomotif-0.4.0/tests/
+-rw-rw-r--   0 shei      (1000) shei      (1000)        0 2023-11-30 15:56:56.000000 nanomotif-0.4.0/tests/__init__.py
+drwxrwxr-x   0 shei      (1000) shei      (1000)        0 2024-05-10 11:39:11.674436 nanomotif-0.4.0/tests/binnary/
+-rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/__init__.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     2089 2024-05-10 09:55:21.000000 nanomotif-0.4.0/tests/binnary/conftest.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1019 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/test_arg_parser.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)    11132 2024-05-10 09:55:21.000000 nanomotif-0.4.0/tests/binnary/test_cli_commands.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     6352 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/test_data_processing_functions.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     2585 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/test_detect_contamination.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1404 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/test_generate_output.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     2132 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/test_include_contigs.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     3317 2024-05-10 09:55:21.000000 nanomotif-0.4.0/tests/binnary/test_scoring.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)      744 2024-03-29 17:14:10.000000 nanomotif-0.4.0/tests/binnary/test_utils.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     5405 2024-05-10 09:55:21.000000 nanomotif-0.4.0/tests/binnary/test_write_bins.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     7236 2023-11-30 15:56:57.000000 nanomotif-0.4.0/tests/test_candidate.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     1365 2024-03-29 11:56:23.000000 nanomotif-0.4.0/tests/test_dataload.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)     2933 2024-03-29 11:56:23.000000 nanomotif-0.4.0/tests/test_motif_find.py
+-rw-rw-r--   0 shei      (1000) shei      (1000)        0 2024-03-29 11:56:23.000000 nanomotif-0.4.0/tests/test_motif_score.py
```

### Comparing `nanomotif-0.3.1/LICENSE` & `nanomotif-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/PKG-INFO` & `nanomotif-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.3.1
+Version: 0.4.0
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
@@ -31,15 +31,15 @@
 
 ### Nanomotif offers
 - de novo methylated motif identification
 - metagenomic bin contamination detection
 - bin association of unbinned contigs (eg. plasmids)
 - association of MTases and RM-systems to motifs.
 <p align="center">
-  <img src="docs/figures/nanomotif_method.png" width="400"/>
+  <img src="docs/figures/nanomotif_method.png" width="400" style="background-color:white;"/>
 </p>
 
 
 
 ## Documentation
 Please see the [documentation](https://nanomotif.readthedocs.io) for detailed installation and usage instructions, descriptions of required files, and analysis examples.
 
@@ -54,15 +54,15 @@
 conda activate nanomotif
 conda install -c bioconda nanomotif
 ```
 
 #### Check installation
 Once installed, the installation can be checked by running:
 ```shell
-nanomotif check-installation
+nanomotif check_installation
 ```
 This runs a test run on a small dataset, ensuring everything works.
 
 For further details, check out the [installation guidelines]().
 
 
 ### Usage
@@ -74,18 +74,18 @@
 - tab-separated file describing `contig-bin` relationship.
 
 For further details, check out the [required files]() documentation.
 
 
 #### Motif discovery
 
-Whether you are interested in finding methylated motifs in monoculture samples or metagenomic samples, we recomment just running `find_motifs`
+Whether you are interested in finding methylated motifs in monoculture samples or metagenomic samples, we recomment just running `motif_discovery`
 
 ```
-nanomotif find_motifs ASSEMBLY.fasta PILEUP.bed CONTIG_BIN.tsv -t THREADS --out OUT
+nanomotif motif_discovery ASSEMBLY.fasta PILEUP.bed CONTIG_BIN.tsv -t THREADS --out OUT
 ```
 
 This will create three files: `motifs.tsv`,`motif-scored.tsv`, and `bin-motifs.tsv`. Highly methylated motifs are found in `bin-motifs.tsv`.
 
 See [usage]() and [output]() for detailed usage and output information.
 
 #### Bin contamination
```

### Comparing `nanomotif-0.3.1/README.md` & `nanomotif-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ### Nanomotif offers
 - de novo methylated motif identification
 - metagenomic bin contamination detection
 - bin association of unbinned contigs (eg. plasmids)
 - association of MTases and RM-systems to motifs.
 <p align="center">
-  <img src="docs/figures/nanomotif_method.png" width="400"/>
+  <img src="docs/figures/nanomotif_method.png" width="400" style="background-color:white;"/>
 </p>
 
 
 
 ## Documentation
 Please see the [documentation](https://nanomotif.readthedocs.io) for detailed installation and usage instructions, descriptions of required files, and analysis examples.
 
@@ -33,15 +33,15 @@
 conda activate nanomotif
 conda install -c bioconda nanomotif
 ```
 
 #### Check installation
 Once installed, the installation can be checked by running:
 ```shell
-nanomotif check-installation
+nanomotif check_installation
 ```
 This runs a test run on a small dataset, ensuring everything works.
 
 For further details, check out the [installation guidelines]().
 
 
 ### Usage
@@ -53,18 +53,18 @@
 - tab-separated file describing `contig-bin` relationship.
 
 For further details, check out the [required files]() documentation.
 
 
 #### Motif discovery
 
-Whether you are interested in finding methylated motifs in monoculture samples or metagenomic samples, we recomment just running `find_motifs`
+Whether you are interested in finding methylated motifs in monoculture samples or metagenomic samples, we recomment just running `motif_discovery`
 
 ```
-nanomotif find_motifs ASSEMBLY.fasta PILEUP.bed CONTIG_BIN.tsv -t THREADS --out OUT
+nanomotif motif_discovery ASSEMBLY.fasta PILEUP.bed CONTIG_BIN.tsv -t THREADS --out OUT
 ```
 
 This will create three files: `motifs.tsv`,`motif-scored.tsv`, and `bin-motifs.tsv`. Highly methylated motifs are found in `bin-motifs.tsv`.
 
 See [usage]() and [output]() for detailed usage and output information.
 
 #### Bin contamination
```

### Comparing `nanomotif-0.3.1/nanomotif/argparser.py` & `nanomotif-0.4.0/nanomotif/argparser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import argparse
 from nanomotif._version import __version__
 import os
 
 
 def  create_parser():
-    parser = argparse.ArgumentParser(description="Motif identification and utilisation commands")
+    formatter = lambda prog: argparse.HelpFormatter(prog,max_help_position=28)
+    parser = argparse.ArgumentParser(description="Motif identification and utilisation commands", formatter_class=formatter)
     parser.add_argument("--version", action="version", version="%(prog)s {}".format(__version__))
-    subparsers = parser.add_subparsers(help="Command descriptions", dest="command")
+    subparsers = parser.add_subparsers(help="-- Command descriptions --", dest="command")
 
     ###########################################################################
     # Shared sub-command arguments
     parser_positional = argparse.ArgumentParser(add_help=False)
     parser_positional.add_argument("assembly", type=str, help="path to the assembly file.")
     parser_positional.add_argument("pileup", type=str, help="path to the modkit pileup file.")
 
@@ -24,50 +25,46 @@
     ###########################################################################
     # Find Motifs
     parser_shared_find_motifs = argparse.ArgumentParser(add_help=False)
     parser_shared_find_motifs.add_argument("--search_frame_size", type=int, default=40, help="length of the sequnces sampled around confident methylatyion sites. Default: %(default)s")
     parser_shared_find_motifs.add_argument("--threshold_methylation_confident", type=float, default=0.80, help="minimum fraction of reads that must be methylated at a position for the position to be considered confiently methylated. These position are used to search for candidate motifs. Default: %(default)s")
     parser_shared_find_motifs.add_argument("--threshold_valid_coverage", type=int, default=5, help="minimum valid base coverage for a position to be considered. Default: %(default)s")
     parser_shared_find_motifs.add_argument("--minimum_kl_divergence", type=float, default=0.05, help="minimum KL-divergence for a position to considered for expansion in  motif search. Higher value means less exhaustive, but faster search. Default: %(default)s")
-    #parser_find_motifs = subparsers.add_parser(
-    #    'find-motifs', 
-    #    parents=[parser_positional, parser_optional, parser_shared_find_motifs], 
-    #    help="identifies motifs in contigs"
-    #)
+    parser_find_motifs = subparsers.add_parser(
+        'find_motifs', 
+        parents=[parser_positional, parser_optional, parser_shared_find_motifs], 
+        help="Finds motifs directly on contig level in provided assembly"
+    )
 
     ###########################################################################
     # Score motifs
-    #parser_score_motifs = subparsers.add_parser(
-    #    'score-motifs', 
-    #    parents=[parser_positional, parser_optional],
-    #    help="generate feature complete output"
-    #)
-    #parser_score_motifs.add_argument("motifs", type=str, help="path to the motifs file.")
+    parser_score_motifs = subparsers.add_parser(
+        'score_motifs', 
+        parents=[parser_positional, parser_optional],
+        help="Find motifs indirectly in contigs by scoring with motifs found in other contigs"
+    )
+    parser_score_motifs.add_argument("motifs", type=str, help="path to the motifs file.")
     
     ###########################################################################
     # Bin consensus
     parser_shared_bin_consensus = argparse.ArgumentParser(add_help=False, conflict_handler="resolve")
     parser_shared_bin_consensus.add_argument("bins", type=str, help="tsv file specifying which bin contigs belong.")
-    #parser_bin_consensus = subparsers.add_parser(
-    #    'bin-consensus', 
-    #    parents=[parser_positional, parser_optional, parser_shared_bin_consensus],
-    #    help="generate consensus set of motif for each bin"
-    #)
-    #parser_bin_consensus.add_argument("motifs", type=str, help="path to the motifs file.")
-    #parser_bin_consensus.add_argument("motifs_scored", metavar="motifs-scored", type=str, help="path to the motif-scored file.")
+    parser_bin_consensus = subparsers.add_parser(
+        'bin_consensus', 
+        parents=[parser_positional, parser_optional, parser_shared_bin_consensus],
+        help="Indentifies highly methylated motifs in bins"
+    )
+    parser_bin_consensus.add_argument("motifs", type=str, help="path to the motifs file.")
+    parser_bin_consensus.add_argument("motifs_scored", metavar="motifs-scored", type=str, help="path to the motif-scored file.")
 
     ###########################################################################
     # Complete workflow
-    parser_complete_workflow = subparsers.add_parser('find_motifs', help='Identify methylated motifs on and contig and bin level', parents=[parser_positional, parser_optional, parser_shared_find_motifs, parser_shared_bin_consensus], conflict_handler="resolve")
+    parser_complete_workflow = subparsers.add_parser('motif_discovery', help='Runs find_motifs, score_motifs and bin_consensus', parents=[parser_positional, parser_optional, parser_shared_find_motifs, parser_shared_bin_consensus], conflict_handler="resolve")
+
 
-    ###########################################################################
-    # Check installation
-    parser_check_installation = subparsers.add_parser('check-installation', parents=[parser_optional, parser_shared_find_motifs], add_help=False)
-    
-    
     ###########################################################################
     # Bin contamination and inclusion
     parser_binnary_shared = argparse.ArgumentParser(description="Contamination DNA Methylation Pattern", add_help=False)
     """Function to add common arguments to a subparser."""
     parser_binnary_shared.add_argument(
         "--motifs_scored", type=str, help="Path to motifs-scored.tsv from nanomotif", required=True
     )
@@ -186,9 +183,16 @@
 
     parser_mtase_linker_install = mtase_linker_subparsers.add_parser(
         'install', 
         help="Install additional dependencies for MTase-linker"
     )
     parser_mtase_linker_install.add_argument("-d", "--dependency_dir", type=str, default=os.getcwd(), help="Path to the directory, where dependencies should be installed. A folder named ML_dependencies will be generated. Default is cwd.")
     
+
+
+    ###########################################################################
+    # Check installation
+    parser_check_installation = subparsers.add_parser('check_installation', parents=[parser_optional, parser_shared_find_motifs], add_help=False, help="Performs small test run to verify that the installation is correct.")
+    
+    
     return parser
```

### Comparing `nanomotif-0.3.1/nanomotif/bin_consensus.py` & `nanomotif-0.4.0/nanomotif/bin_consensus.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/binnary/analysis.py` & `nanomotif-0.4.0/nanomotif/binnary/analysis.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/binnary/data_processing.py` & `nanomotif-0.4.0/nanomotif/binnary/data_processing.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/binnary/detect_contamination.py` & `nanomotif-0.4.0/nanomotif/binnary/detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/binnary/include_contigs.py` & `nanomotif-0.4.0/nanomotif/binnary/include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/binnary/logging.py` & `nanomotif-0.4.0/nanomotif/binnary/logging.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/binnary/scoring.py` & `nanomotif-0.4.0/nanomotif/binnary/scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/binnary/utils.py` & `nanomotif-0.4.0/nanomotif/binnary/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/candidate.py` & `nanomotif-0.4.0/nanomotif/candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/constants.py` & `nanomotif-0.4.0/nanomotif/constants.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/dataload.py` & `nanomotif-0.4.0/nanomotif/dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/datasets/geobacillus-plasmids.assembly.fasta` & `nanomotif-0.4.0/nanomotif/datasets/geobacillus-plasmids.assembly.fasta`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/datasets/geobacillus-plasmids.pileup.bed` & `nanomotif-0.4.0/nanomotif/datasets/geobacillus-plasmids.pileup.bed`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/datasets.py` & `nanomotif-0.4.0/nanomotif/datasets.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/evaluate.py` & `nanomotif-0.4.0/nanomotif/evaluate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/feature.py` & `nanomotif-0.4.0/nanomotif/feature.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/main.py` & `nanomotif-0.4.0/nanomotif/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,21 +130,21 @@
     if len(motifs) == 0:
         log.info("No motifs found")
         return
     
     motifs_file_name = motifs_file_name + "-score"
     save_motif_df(motifs, motifs_file_name)
 
-    #log.info(" - Removing sub motifs")
-    #motifs = nm.postprocess.remove_sub_motifs(motifs)
-    #if len(motifs) == 0:
-    #    log.info("No motifs found")
-    #    return
-    #motifs_file_name = motifs_file_name +   "-sub"
-    #save_motif_df(motifs, motifs_file_name)
+    log.info(" - Removing sub motifs")
+    motifs = nm.postprocess.remove_sub_motifs(motifs)
+    if len(motifs) == 0:
+        log.info("No motifs found")
+        return
+    motifs_file_name = motifs_file_name +   "-sub"
+    save_motif_df(motifs, motifs_file_name)
 
     log.info(" - Removing noisy motifs")
     motifs = nm.postprocess.remove_noisy_motifs(motifs)
     if len(motifs) == 0:
         log.info("No motifs found")
         return
     motifs_file_name = motifs_file_name +   "-noise"
@@ -317,15 +317,15 @@
     log.info("Scoring motifs")
     scored_all = score_motifs(args, pileup=pileup, assembly=assembly, motifs=motifs)
 
     # Bin consensus
     log.info("Finding bin consensus motifs")
     args.bins = nm.datasets.geobacillus_plasmids_bin_path()
     bin_consensus(args, pileup=pileup, assembly=assembly, motifs=motifs, motifs_scored=scored_all)
-
+    
     log.info("Done")
     shutil.rmtree(args.out)
 
 
 ####################################################################################################
 # Binnary - contamination and inclusion
 from nanomotif.binnary import data_processing, detect_contamination, include_contigs
@@ -483,26 +483,35 @@
     
     if args.command in ["detect_contamination", "include_contigs", "MTase-linker"]:
         args.verbose = False
         args.seed = 1
     
     if args.command == "find_motifs":
         shared_setup(args, args.out)
-        motif_discovery(args)
-    elif args.command == "check-installation":
-        args.out = "nanomotif_install_check"
+        find_motifs(args)
+    elif args.command == "score_motifs":
         shared_setup(args, args.out)
-        check_install(args)
+        score_motifs(args)
+    elif args.command == "bin_consensus":
+        shared_setup(args, args.out)
+        bin_consensus(args)
+    elif args.command == "motif_discovery":
+        shared_setup(args, args.out)
+        motif_discovery(args)
 
     elif args.command in ["detect_contamination", "include_contigs"]:
         shared_setup(args, args.out)
         binnary(args)
 
     elif args.command == "MTase-linker":
         mtase_linker(args)
 
+    elif args.command == "check_installation":
+        args.out = "nanomotif_install_check"
+        shared_setup(args, args.out)
+        check_install(args)
 
     else:
         parser.print_help()
         exit()
 if __name__ == "__main__":
     main()
```

### Comparing `nanomotif-0.3.1/nanomotif/model.py` & `nanomotif-0.4.0/nanomotif/model.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/mtase_linker/command.py` & `nanomotif-0.4.0/nanomotif/mtase_linker/command.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/mtase_linker/dependencies.py` & `nanomotif-0.4.0/nanomotif/mtase_linker/dependencies.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/old_search_method.py` & `nanomotif-0.4.0/nanomotif/old_search_method.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/parallel.py` & `nanomotif-0.4.0/nanomotif/parallel.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/postprocess.py` & `nanomotif-0.4.0/nanomotif/postprocess.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/scoremotifs.py` & `nanomotif-0.4.0/nanomotif/scoremotifs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/seq.py` & `nanomotif-0.4.0/nanomotif/seq.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif/utils.py` & `nanomotif-0.4.0/nanomotif/utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/nanomotif.egg-info/PKG-INFO` & `nanomotif-0.4.0/nanomotif.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomotif
-Version: 0.3.1
+Version: 0.4.0
 Summary: Identifying methlyation motifs in nanopore data
 Author: AAU_DarkScience
 Author-email: shei@bio.aau.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
@@ -31,15 +31,15 @@
 
 ### Nanomotif offers
 - de novo methylated motif identification
 - metagenomic bin contamination detection
 - bin association of unbinned contigs (eg. plasmids)
 - association of MTases and RM-systems to motifs.
 <p align="center">
-  <img src="docs/figures/nanomotif_method.png" width="400"/>
+  <img src="docs/figures/nanomotif_method.png" width="400" style="background-color:white;"/>
 </p>
 
 
 
 ## Documentation
 Please see the [documentation](https://nanomotif.readthedocs.io) for detailed installation and usage instructions, descriptions of required files, and analysis examples.
 
@@ -54,15 +54,15 @@
 conda activate nanomotif
 conda install -c bioconda nanomotif
 ```
 
 #### Check installation
 Once installed, the installation can be checked by running:
 ```shell
-nanomotif check-installation
+nanomotif check_installation
 ```
 This runs a test run on a small dataset, ensuring everything works.
 
 For further details, check out the [installation guidelines]().
 
 
 ### Usage
@@ -74,18 +74,18 @@
 - tab-separated file describing `contig-bin` relationship.
 
 For further details, check out the [required files]() documentation.
 
 
 #### Motif discovery
 
-Whether you are interested in finding methylated motifs in monoculture samples or metagenomic samples, we recomment just running `find_motifs`
+Whether you are interested in finding methylated motifs in monoculture samples or metagenomic samples, we recomment just running `motif_discovery`
 
 ```
-nanomotif find_motifs ASSEMBLY.fasta PILEUP.bed CONTIG_BIN.tsv -t THREADS --out OUT
+nanomotif motif_discovery ASSEMBLY.fasta PILEUP.bed CONTIG_BIN.tsv -t THREADS --out OUT
 ```
 
 This will create three files: `motifs.tsv`,`motif-scored.tsv`, and `bin-motifs.tsv`. Highly methylated motifs are found in `bin-motifs.tsv`.
 
 See [usage]() and [output]() for detailed usage and output information.
 
 #### Bin contamination
```

### Comparing `nanomotif-0.3.1/nanomotif.egg-info/SOURCES.txt` & `nanomotif-0.4.0/nanomotif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/setup.py` & `nanomotif-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/tests/binnary/conftest.py` & `nanomotif-0.4.0/tests/binnary/conftest.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/tests/binnary/test_arg_parser.py` & `nanomotif-0.4.0/tests/binnary/test_arg_parser.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/tests/binnary/test_cli_commands.py` & `nanomotif-0.4.0/tests/binnary/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/tests/binnary/test_data_processing_functions.py` & `nanomotif-0.4.0/tests/binnary/test_data_processing_functions.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/tests/binnary/test_detect_contamination.py` & `nanomotif-0.4.0/tests/binnary/test_detect_contamination.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/tests/binnary/test_generate_output.py` & `nanomotif-0.4.0/tests/binnary/test_generate_output.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/tests/binnary/test_include_contigs.py` & `nanomotif-0.4.0/tests/binnary/test_include_contigs.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/tests/binnary/test_scoring.py` & `nanomotif-0.4.0/tests/binnary/test_scoring.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/tests/binnary/test_utils.py` & `nanomotif-0.4.0/tests/binnary/test_utils.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/tests/binnary/test_write_bins.py` & `nanomotif-0.4.0/tests/binnary/test_write_bins.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/tests/test_candidate.py` & `nanomotif-0.4.0/tests/test_candidate.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/tests/test_dataload.py` & `nanomotif-0.4.0/tests/test_dataload.py`

 * *Files identical despite different names*

### Comparing `nanomotif-0.3.1/tests/test_motif_find.py` & `nanomotif-0.4.0/tests/test_motif_find.py`

 * *Files identical despite different names*

