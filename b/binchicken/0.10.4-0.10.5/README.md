# Comparing `tmp/binchicken-0.10.4.tar.gz` & `tmp/binchicken-0.10.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binchicken-0.10.4.tar", last modified: Mon Apr  8 04:48:46 2024, max compression
+gzip compressed data, was "binchicken-0.10.5.tar", last modified: Fri May 10 04:47:20 2024, max compression
```

## Comparing `binchicken-0.10.4.tar` & `binchicken-0.10.5.tar`

### file list

```diff
@@ -1,57 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.535195 binchicken-0.10.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 04:48:34.000000 binchicken-0.10.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 04:48:34.000000 binchicken-0.10.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42098 2024-04-08 04:48:46.535195 binchicken-0.10.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-08 04:48:34.000000 binchicken-0.10.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.523195 binchicken-0.10.4/binchicken/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    76901 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/binchicken.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.527195 binchicken-0.10.4/binchicken/config/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/config/template_coassemble.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/config/template_evaluate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.527195 binchicken-0.10.4/binchicken/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)    28468 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/coassemble.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.527195 binchicken-0.10.4/binchicken/workflow/env/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/aviary.yml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/coverm.yml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/fastp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/kingfisher.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/prodigal.yml
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/r.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/env/singlem.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/evaluate.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.531195 binchicken-0.10.4/binchicken/workflow/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4311 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/aviary_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/cluster_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3848 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/collect_reference_bins.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11697 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3492 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/is_interleaved.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1113 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/no_genomes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3724 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/query_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/summarise_coassemblies.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5390 2024-04-08 04:48:34.000000 binchicken-0.10.4/binchicken/workflow/scripts/target_elusive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.531195 binchicken-0.10.4/binchicken.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42098 2024-04-08 04:48:46.000000 binchicken-0.10.4/binchicken.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-08 04:48:46.000000 binchicken-0.10.4/binchicken.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 04:48:46.000000 binchicken-0.10.4/binchicken.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 04:48:46.000000 binchicken-0.10.4/binchicken.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 04:48:46.000000 binchicken-0.10.4/binchicken.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 04:48:46.000000 binchicken-0.10.4/binchicken.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-08 04:48:34.000000 binchicken-0.10.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 04:48:46.535195 binchicken-0.10.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 04:48:46.531195 binchicken-0.10.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_aviary_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)    32904 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_cluster_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    56811 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_coassemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_collect_reference_bins.py
--rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)    31280 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_evaluate_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_is_interleaved.py
--rw-r--r--   0 runner    (1001) docker     (127)    27959 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_iterate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_no_genomes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_query_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_summarise_coassemblies.py
--rw-r--r--   0 runner    (1001) docker     (127)    18764 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_target_elusive.py
--rw-r--r--   0 runner    (1001) docker     (127)    33155 2024-04-08 04:48:35.000000 binchicken-0.10.4/test/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:20.216127 binchicken-0.10.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-10 04:47:14.000000 binchicken-0.10.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 04:47:14.000000 binchicken-0.10.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42098 2024-05-10 04:47:20.216127 binchicken-0.10.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-10 04:47:14.000000 binchicken-0.10.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:20.212127 binchicken-0.10.5/binchicken/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 04:47:14.000000 binchicken-0.10.5/binchicken/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    77658 2024-05-10 04:47:14.000000 binchicken-0.10.5/binchicken/binchicken.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:20.212127 binchicken-0.10.5/binchicken/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-10 04:47:14.000000 binchicken-0.10.5/binchicken/config/template_coassemble.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-10 04:47:14.000000 binchicken-0.10.5/binchicken/config/template_evaluate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:20.212127 binchicken-0.10.5/binchicken/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)    28645 2024-05-10 04:47:14.000000 binchicken-0.10.5/binchicken/workflow/coassemble.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:20.216127 binchicken-0.10.5/binchicken/workflow/env/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 04:47:14.000000 binchicken-0.10.5/binchicken/workflow/env/aviary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-10 04:47:14.000000 binchicken-0.10.5/binchicken/workflow/env/coverm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 04:47:14.000000 binchicken-0.10.5/binchicken/workflow/env/fastp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-10 04:47:14.000000 binchicken-0.10.5/binchicken/workflow/env/kingfisher.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-10 04:47:14.000000 binchicken-0.10.5/binchicken/workflow/env/prodigal.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-10 04:47:14.000000 binchicken-0.10.5/binchicken/workflow/env/r.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-10 04:47:14.000000 binchicken-0.10.5/binchicken/workflow/env/singlem.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-10 04:47:14.000000 binchicken-0.10.5/binchicken/workflow/evaluate.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:20.216127 binchicken-0.10.5/binchicken.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42098 2024-05-10 04:47:20.000000 binchicken-0.10.5/binchicken.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-10 04:47:20.000000 binchicken-0.10.5/binchicken.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:47:20.000000 binchicken-0.10.5/binchicken.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 04:47:20.000000 binchicken-0.10.5/binchicken.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-10 04:47:20.000000 binchicken-0.10.5/binchicken.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 04:47:20.000000 binchicken-0.10.5/binchicken.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-10 04:47:14.000000 binchicken-0.10.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 04:47:20.216127 binchicken-0.10.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:47:20.216127 binchicken-0.10.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_aviary_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32940 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_cluster_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60127 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_coassemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_collect_reference_bins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31776 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_evaluate_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_is_interleaved.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27959 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_iterate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_no_genomes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_query_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_summarise_coassemblies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18764 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_target_elusive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33155 2024-05-10 04:47:14.000000 binchicken-0.10.5/test/test_update.py
```

### Comparing `binchicken-0.10.4/LICENSE` & `binchicken-0.10.5/LICENSE`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.4/PKG-INFO` & `binchicken-0.10.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binchicken
-Version: 0.10.4
+Version: 0.10.5
 Summary: Bin chicken - targeted recovery of low abundance metagenome assembled genomes through intelligent coassembly
 Author-email: Samuel Aroney <samuel.aroney@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `binchicken-0.10.4/README.md` & `binchicken-0.10.5/README.md`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.4/binchicken/binchicken.py` & `binchicken-0.10.5/binchicken/binchicken.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,14 +472,15 @@
         "run_qc": args.run_qc,
         "unmapping_min_appraised": args.unmapping_min_appraised,
         "unmapping_max_identity": args.unmapping_max_identity,
         "unmapping_max_alignment": args.unmapping_max_alignment,
         "aviary_speed": args.aviary_speed,
         "assembly_strategy": args.assembly_strategy,
         "run_aviary": args.run_aviary,
+        "cluster_submission": args.cluster_submission,
         "aviary_gtdbtk": args.aviary_gtdbtk_db,
         "aviary_checkm2": args.aviary_checkm2_db,
         "aviary_assemble_threads": args.aviary_assemble_cores,
         "aviary_assemble_memory": args.aviary_assemble_memory,
         "aviary_recover_threads": args.aviary_recover_cores,
         "aviary_recover_memory": args.aviary_recover_memory,
         "conda_prefix": args.conda_prefix,
@@ -923,14 +924,15 @@
 
     args.forward_list = None
     args.reverse_list = None
     args.genomes_list = None
     args.new_genomes_list = None
     args.coassembly_samples_list = None
     args.sample_read_size = None
+    args.cluster_submission = False
     args.aviary_gtdbtk_db = "."
     args.aviary_checkm2_db = "."
     args.aviary_assemble_cores = None
     args.aviary_recover_cores = None
     args.assemble_unmapped = True
     args.run_qc = True
     args.coassemblies = None
@@ -1107,15 +1109,15 @@
                                     help="Snakemake profile (see https://snakemake.readthedocs.io/en/v7.32.3/executing/cli.html#profiles).\n"
                                          "Can be used to submit rules as jobs to cluster engine (see https://snakemake.readthedocs.io/en/v7.32.3/executing/cluster.html).")
         local_cores_default = 1
         argument_group.add_argument("--local-cores", type=int, help=f"Maximum number of cores to use on localrules when running in cluster mode [default: {local_cores_default}]", default=local_cores_default)
         retries_default = 3
         argument_group.add_argument("--cluster-retries", help=f"Number of times to retry a failed job when using cluster submission (see `--snakemake-profile`) [default: {retries_default}].", default=retries_default)
         argument_group.add_argument("--snakemake-args", help="Additional commands to be supplied to snakemake in the form of a space-prefixed single string e.g. \" --quiet\"", default="")
-        argument_group.add_argument("--tmp-dir", help="Path to temporary directory. [default: Use path from TMPDIR env variable]")
+        argument_group.add_argument("--tmp-dir", help="Path to temporary directory. [default: no default]")
 
     def add_base_arguments(argument_group):
         argument_group.add_argument("--forward", "--reads", "--sequences", nargs='+', help="input forward/unpaired nucleotide read sequence(s)")
         argument_group.add_argument("--forward-list", "--reads-list", "--sequences-list", help="input forward/unpaired nucleotide read sequence(s) newline separated")
         argument_group.add_argument("--reverse", nargs='+', help="input reverse nucleotide read sequence(s)")
         argument_group.add_argument("--reverse-list", help="input reverse nucleotide read sequence(s) newline separated")
         argument_group.add_argument("--genomes", nargs='+', help="Reference genomes for read mapping")
@@ -1129,14 +1131,15 @@
         min_completeness_default = 70
         argument_group.add_argument("--min-completeness", type=int, help=f"Include bins with at least this minimum completeness [default: {min_completeness_default}]", default=min_completeness_default)
         max_contamination_default = 10
         argument_group.add_argument("--max-contamination", type=int, help=f"Include bins with at most this maximum contamination [default: {max_contamination_default}]", default=max_contamination_default)
 
     def add_aviary_options(argument_group):
         argument_group.add_argument("--run-aviary", action="store_true", help="Run Aviary commands for all identified coassemblies (unless specific coassemblies are chosen with --coassemblies) [default: do not]")
+        argument_group.add_argument("--cluster-submission", action="store_true", help="Flag that cluster submission will occur through `--snakemake-profile`. This sets the local threads of Aviary recover to 1, allowing parallel job submission [default: do not]")
         default_aviary_speed = FAST_AVIARY_MODE
         argument_group.add_argument("--aviary-speed", help=f"Run Aviary recover in 'fast' or 'comprehensive' mode. Fast mode skips slow binners and refinement steps. [default: {default_aviary_speed}]",
                                     default=default_aviary_speed, choices=[FAST_AVIARY_MODE, COMPREHENSIVE_AVIARY_MODE])
         default_assembly_strategy = DYNAMIC_ASSEMBLY_STRATEGY
         argument_group.add_argument("--assembly-strategy", help=f"Assembly strategy to use with Aviary. [default: {default_assembly_strategy}; attempts metaspades and if fails, switches to megahit]",
                                     default=default_assembly_strategy, choices=[DYNAMIC_ASSEMBLY_STRATEGY, METASPADES_ASSEMBLY, MEGAHIT_ASSEMBLY])
         argument_group.add_argument("--aviary-gtdbtk-db", help="Path to GTDB-Tk database directory for Aviary. [default: use path from GTDBTK_DATA_PATH env variable]")
@@ -1324,16 +1327,14 @@
             args.conda_prefix = load_variable("SNAKEMAKE_CONDA_PREFIX")
     if not hasattr(args, "singlem_metapackage") or not args.singlem_metapackage:
         args.singlem_metapackage = load_variable("SINGLEM_METAPACKAGE_PATH")
     if not hasattr(args, "aviary_gtdbtk_db") or not args.aviary_gtdbtk_db:
         args.aviary_gtdbtk_db = load_variable("GTDBTK_DATA_PATH")
     if not hasattr(args, "aviary_checkm2_db") or not args.aviary_checkm2_db:
         args.aviary_checkm2_db = load_variable("CHECKM2DB")
-    if not args.tmp_dir:
-        args.tmp_dir = load_variable("TMPDIR")
 
     if hasattr(args, "genomes"):
         if not (args.genomes or args.genomes_list):
             args.no_genomes = True
         else:
             args.no_genomes = False
 
@@ -1376,14 +1377,16 @@
             if args.max_coassembly_samples > args.max_recovery_samples:
                 raise Exception("Max recovery samples (--max-recovery-samples) must be greater than or equal to max coassembly samples (--max-coassembly-samples)")
         else:
             if args.num_coassembly_samples > args.max_recovery_samples:
                 raise Exception("Max recovery samples (--max-recovery-samples) must be greater than or equal to number of coassembly samples (--num-coassembly-samples)")
         if args.run_aviary and not (args.aviary_gtdbtk_db and args.aviary_checkm2_db):
             raise Exception("Run Aviary (--run-aviary) requires paths to GTDB-Tk and CheckM2 databases to be provided (--aviary-gtdbtk-db or GTDBTK_DATA_PATH and --aviary-checkm2-db or CHECKM2DB)")
+        if args.cluster_submission and not args.snakemake_profile:
+                logging.warning("The arg `--cluster-submission` is only a flag and cannot activate cluster submission alone. Please see `--snakemake-profile` for cluster submission.")
         if (args.sample_query or args.sample_query_list or args.sample_query_dir) and args.taxa_of_interest and args.assemble_unmapped:
             raise Exception("Unmapping is incompatible with the combination of sample query and taxa of interest")
 
     def coassemble_output_argument_verification(args, evaluate=False):
         summary_flag = args.coassemble_summary if evaluate else True
         if not args.coassemble_output and not (args.coassemble_unbinned and args.coassemble_binned and args.coassemble_targets and \
                                                args.coassemble_elusive_edges and args.coassemble_elusive_clusters and summary_flag):
@@ -1405,14 +1408,16 @@
             raise Exception("Name of coassembly run must be provided to evaluate binning")
         evaluate(args)
 
     elif args.subparser_name == "update":
         coassemble_output_argument_verification(args)
         if args.run_aviary and not (args.aviary_gtdbtk_db and args.aviary_checkm2_db):
             raise Exception("Run Aviary (--run-aviary) requires paths to GTDB-Tk and CheckM2 databases to be provided (--aviary-gtdbtk-db and --aviary-checkm2-db)")
+        if args.cluster_submission and not args.snakemake_profile:
+            logging.warning("The arg `--cluster-submission` is only a flag and cannot activate cluster submission alone. Please see `--snakemake-profile` for cluster submission.")
         update(args)
 
     elif args.subparser_name == "iterate":
         if args.sample_query or args.sample_query_list or args.sample_query_dir:
             raise Exception("Query arguments are incompatible with Bin chicken iterate")
         if args.sample_singlem_dir or args.sample_query_dir:
             raise Exception("Directory arguments are incompatible with Bin chicken iterate")
```

### Comparing `binchicken-0.10.4/binchicken/config/template_coassemble.yaml` & `binchicken-0.10.5/binchicken/config/template_coassemble.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 max_recovery_samples: 1
 unmapping_min_appraised: 1
 unmapping_max_identity: 1
 unmapping_max_alignment: 1
 aviary_speed: "fast"
 assembly_strategy: "dynamic"
 run_aviary: false
+cluster_submission: false
 aviary_gtdbtk: ""
 aviary_checkm2: ""
 aviary_assemble_memory: 1
 aviary_assemble_threads: 1
 aviary_recover_memory: 1
 aviary_recover_threads: 1
 test: false
 mock_sra: false
 aviary_dryrun: false
 conda_prefix: false
-tmpdir: "/tmp"
+tmpdir: false
 build: false
```

### Comparing `binchicken-0.10.4/binchicken/workflow/coassemble.smk` & `binchicken-0.10.5/binchicken/workflow/coassemble.smk`

 * *Files 1% similar despite different names*

```diff
@@ -469,15 +469,15 @@
         json = output_dir + "/qc/{read}.json",
         html = output_dir + "/qc/{read}.html",
     group: "unmapping"
     params:
         quality_cutoff = 15,
         unqualified_percent_limit = 40,
         min_length = 80,
-    threads: 16
+    threads: 32
     resources:
         mem_mb=get_mem_mb,
         runtime = lambda wildcards, attempt: 4*60*attempt,
     log:
         logs_dir + "/mapping/{read}_qc.log"
     benchmark:
         benchmarks_dir + "/mapping/{read}_qc.tsv"
@@ -516,15 +516,15 @@
     input:
         reads_1 = lambda wildcards: config["reads_1"][wildcards.read] if not config["run_qc"] else output_dir + "/qc/{read}_1.fastq.gz",
         reads_2 = lambda wildcards: config["reads_2"][wildcards.read] if not config["run_qc"] else output_dir + "/qc/{read}_2.fastq.gz",
         genomes = output_dir + "/mapping/{read}_reference.fna",
     output:
         dir = temp(directory(output_dir + "/mapping/{read}_coverm")),
     group: "unmapping"
-    threads: 16
+    threads: 32
     resources:
         mem_mb=get_mem_mb,
         runtime = lambda wildcards, attempt: 12*60*attempt,
     log:
         logs_dir + "/mapping/{read}_coverm.log",
     benchmark:
         benchmarks_dir + "/mapping/{read}_coverm.tsv"
@@ -543,18 +543,18 @@
     input:
         output_dir + "/mapping/{read}_coverm",
     output:
         temp(output_dir + "/mapping/{read}_unmapped.bam"),
     group: "unmapping"
     params:
         genomes = "{read}_reference.fna",
-        reads_1 = lambda wildcards: os.path.basename(config["reads_1"][wildcards.read]),
+        reads_1 = lambda wildcards: os.path.basename(config["reads_1"][wildcards.read]) if not config["run_qc"] else wildcards.read + "_1.fastq.gz",
         sequence_identity = config["unmapping_max_identity"],
         alignment_percent = config["unmapping_max_alignment"],
-    threads: 16
+    threads: 32
     resources:
         mem_mb=get_mem_mb,
         runtime = lambda wildcards, attempt: 4*60*attempt,
     log:
         logs_dir + "/mapping/{read}_filter.log",
     benchmark:
         benchmarks_dir + "/mapping/{read}_filter.tsv"
@@ -573,15 +573,15 @@
 rule bam_to_fastq:
     input:
         output_dir + "/mapping/{read}_unmapped.bam",
     output:
         reads_1 = output_dir + "/mapping/{read}_unmapped.1.fq.gz",
         reads_2 = output_dir + "/mapping/{read}_unmapped.2.fq.gz",
     group: "unmapping"
-    threads: 16
+    threads: 32
     resources:
         mem_mb=get_mem_mb,
         runtime = lambda wildcards, attempt: 4*60*attempt,
     log:
         logs_dir + "/mapping/{read}_fastq.log",
     conda:
         "env/coverm.yml"
@@ -691,15 +691,15 @@
     params:
         reads_1 = lambda wildcards: get_reads_coassembly(wildcards),
         reads_2 = lambda wildcards: get_reads_coassembly(wildcards, forward=False),
         dryrun = "--build" if config["build"] else "--dryrun" if config["aviary_dryrun"] else "",
         drymkdir = "&& mkdir -p "+output_dir+"/coassemble/{coassembly}/assemble/assembly" if config["aviary_dryrun"] else "",
         drytouch = "&& touch "+output_dir+"/coassemble/{coassembly}/assemble/assembly/final_contigs.fasta" if config["aviary_dryrun"] else "",
         conda_prefix = config["conda_prefix"] if config["conda_prefix"] else ".",
-        tmpdir = config["tmpdir"],
+        tmpdir = f"TMPDIR={config['tmpdir']}" if config["tmpdir"] else "",
     threads: lambda wildcards, attempt: get_assemble_threads(wildcards, attempt)
     resources:
         mem_mb = lambda wildcards, attempt: get_assemble_memory(wildcards, attempt, unit="MB"),
         mem_gb = get_assemble_memory,
         runtime = lambda wildcards, attempt: 96*60*attempt,
         assembler = get_assemble_assembler,
     log:
@@ -708,15 +708,15 @@
         "env/aviary.yml"
     shell:
         "GTDBTK_DATA_PATH=. "
         "CHECKM2DB=. "
         "EGGNOG_DATA_DIR=. "
         "CONDA_ENV_PATH={params.conda_prefix} "
         "SINGLEM_METAPACKAGE_PATH=. "
-        "TMPDIR={params.tmpdir} "
+        "{params.tmpdir} "
         "aviary assemble "
         "--coassemble "
         "-1 {params.reads_1} "
         "-2 {params.reads_2} "
         "--output {output.dir} "
         "-n {threads} "
         "-t {threads} "
@@ -739,44 +739,45 @@
         reads_1 = lambda wildcards: get_reads_coassembly(wildcards, recover=True),
         reads_2 = lambda wildcards: get_reads_coassembly(wildcards, forward=False, recover=True),
         dryrun = "--build" if config["build"] else "--dryrun" if config["aviary_dryrun"] else "",
         gtdbtk = config["aviary_gtdbtk"],
         checkm2 = config["aviary_checkm2"],
         conda_prefix = config["conda_prefix"] if config["conda_prefix"] else ".",
         singlem_metapackage = config["singlem_metapackage"],
-        fast = "--workflow recover_mags_no_singlem --skip-binners maxbin concoct rosella --skip-abundances --refinery-max-iterations 0" if config["aviary_speed"] == FAST_AVIARY_MODE else "",
+        fast = "--skip-singlem --skip-abundances --refinery-max-iterations 0" if config["aviary_speed"] == FAST_AVIARY_MODE else "",
         snakemake_profile = f"--snakemake-profile {config['snakemake_profile']}" if config["snakemake_profile"] else "",
         cluster_retries = f"--cluster-retries {config['cluster_retries']}" if config["cluster_retries"] else "",
-        tmpdir = config["tmpdir"],
+        tmpdir = f"TMPDIR={config['tmpdir']}" if config["tmpdir"] else "",
+        threads = int(config["aviary_recover_threads"])
     localrule: True
     threads:
-        int(config["aviary_recover_threads"])
+        1 if config["cluster_submission"] else int(config["aviary_recover_threads"])
     resources:
         mem_mb = int(config["aviary_recover_memory"])*1000,
         mem_gb = int(config["aviary_recover_memory"]),
         runtime = "168h",
     log:
         logs_dir + "/aviary/{coassembly}_recover.log"
     conda:
         "env/aviary.yml"
     shell:
         "GTDBTK_DATA_PATH={params.gtdbtk} "
         "CHECKM2DB={params.checkm2} "
         "EGGNOG_DATA_DIR=. "
         "CONDA_ENV_PATH={params.conda_prefix} "
         "SINGLEM_METAPACKAGE_PATH={params.singlem_metapackage} "
-        "TMPDIR={params.tmpdir} "
+        "{params.tmpdir} "
         "aviary recover "
         "--assembly {input.assembly} "
         "-1 {params.reads_1} "
         "-2 {params.reads_2} "
         "--output {params.output} "
         "{params.fast} "
-        "-n {threads} "
-        "-t {threads} "
+        "-n {params.threads} "
+        "-t {params.threads} "
         "-m {resources.mem_gb} "
         "--skip-qc "
         "{params.snakemake_profile} "
         "{params.cluster_retries} "
         "{params.dryrun} "
         "&> {log} "
         "&& touch {output} "
```

### Comparing `binchicken-0.10.4/binchicken/workflow/evaluate.smk` & `binchicken-0.10.5/binchicken/workflow/evaluate.smk`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.4/binchicken.egg-info/PKG-INFO` & `binchicken-0.10.5/binchicken.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binchicken
-Version: 0.10.4
+Version: 0.10.5
 Summary: Bin chicken - targeted recovery of low abundance metagenome assembled genomes through intelligent coassembly
 Author-email: Samuel Aroney <samuel.aroney@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `binchicken-0.10.4/binchicken.egg-info/SOURCES.txt` & `binchicken-0.10.5/binchicken.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,23 +17,14 @@
 binchicken/workflow/env/aviary.yml
 binchicken/workflow/env/coverm.yml
 binchicken/workflow/env/fastp.yml
 binchicken/workflow/env/kingfisher.yml
 binchicken/workflow/env/prodigal.yml
 binchicken/workflow/env/r.yml
 binchicken/workflow/env/singlem.yml
-binchicken/workflow/scripts/aviary_commands.py
-binchicken/workflow/scripts/cluster_graph.py
-binchicken/workflow/scripts/collect_reference_bins.py
-binchicken/workflow/scripts/evaluate.py
-binchicken/workflow/scripts/is_interleaved.py
-binchicken/workflow/scripts/no_genomes.py
-binchicken/workflow/scripts/query_processing.py
-binchicken/workflow/scripts/summarise_coassemblies.py
-binchicken/workflow/scripts/target_elusive.py
 test/test_aviary_commands.py
 test/test_build.py
 test/test_cluster_graph.py
 test/test_coassemble.py
 test/test_collect_reference_bins.py
 test/test_evaluate.py
 test/test_evaluate_script.py
```

### Comparing `binchicken-0.10.4/pyproject.toml` & `binchicken-0.10.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -28,9 +28,12 @@
 "Homepage" = "https://github.com/AroneyS/binchicken"
 "Bug Tracker" = "https://github.com/AroneyS/binchicken/issues"
 
 [project.scripts]
 binchicken = "binchicken.binchicken:main"
 ibis = "binchicken.binchicken:main"
 
+[tool.setuptools]
+packages = ["binchicken"]
+
 [tool.setuptools.dynamic]
 version = {attr = "binchicken.__version__"}
```

### Comparing `binchicken-0.10.4/test/test_aviary_commands.py` & `binchicken-0.10.5/test/test_aviary_commands.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.4/test/test_build.py` & `binchicken-0.10.5/test/test_build.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.4/test/test_cluster_graph.py` & `binchicken-0.10.5/test/test_cluster_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,72 +398,72 @@
             MIN_COASSEMBLY_SAMPLES=3,
             MAX_COASSEMBLY_SAMPLES=3,
             MAX_SAMPLES_COMBINATIONS=5,
             )
         self.assertDataFrameEqual(expected, observed)
 
     def test_cluster_four_samples(self):
-        # 1:   2 3 4
-        # 2: 1   3 4
-        # 3: 1 2   4
-        # 4: 1 2 3 4
+        # 1: 0   2 3 4
+        # 2: 0 1   3 4
+        # 3: 0 1 2   4
+        # 4: 0 1 2 3 4
 
-        # 5: 1         6 7 8 9 10
-        # 6:         5   7 8
-        # 7:         5 6   8
-        # 8:               8 9 10
+        # 5:   1         6 7 8 9 10
+        # 6:           5   7 8
+        # 7:           5 6   8
+        # 8:                 8 9 10
 
         elusive_edges = pl.DataFrame([
             # pairs of 1,2,3,4
-            ["match", 2, "1,2", "3,4"],
-            ["match", 2, "1,3", "2,4"],
-            ["match", 2, "1,4", "2,3,4"],
-            ["match", 2, "2,3", "1,4"],
-            ["match", 2, "2,4", "1,3,4"],
-            ["match", 2, "3,4", "1,2,4"],
+            ["match", 2, "1,2", "0,3,4"],
+            ["match", 2, "1,3", "0,2,4"],
+            ["match", 2, "1,4", "0,2,3,4"],
+            ["match", 2, "2,3", "0,1,4"],
+            ["match", 2, "2,4", "0,1,3,4"],
+            ["match", 2, "3,4", "0,1,2,4"],
             # pairs of 5,6,7,8
             ["match", 2, "5,6", "7,8"],
             ["match", 2, "5,7", "6,8"],
             ["match", 2, "5,8", "8,9,10"],
             ["match", 2, "6,7", "5,8"],
             ["match", 2, "6,8", "8"],
             ["match", 2, "7,8", "8"],
             # joint pairs
             ["match", 2, "2,5", "1"],
             ["match", 2, "3,5", "1"],
             ["match", 2, "4,5", "1"],
             # triplets
             ["pool", 3, "2,3,4,5", "1"],
-            ["pool", 3, "1,3,4", "2"],
-            ["pool", 3, "1,2,4", "3"],
-            ["pool", 3, "1,2,3,4", "4"],
+            ["pool", 3, "1,3,4", "0,2"],
+            ["pool", 3, "1,2,4", "0,3"],
+            ["pool", 3, "1,2,3,4", "0,4"],
             ["pool", 3, "5,6,7,8", "8"],
             # quads
             ["pool", 4, "2,3,4,5", "1"],
-            ["pool", 4, "1,2,3,4", "4"],
+            ["pool", 4, "1,2,3,4", "0,4"],
             ["pool", 4, "5,6,7,8", "8"],
         ], schema = ELUSIVE_EDGES_COLUMNS)
         read_size = pl.DataFrame([
             ["1", 1000],
             ["2", 2000],
             ["3", 3000],
             ["4", 4000],
             ["5", 5000],
             ["6", 6000],
             ["7", 7000],
             ["8", 8000],
         ], schema=READ_SIZE_COLUMNS)
 
         expected = pl.DataFrame([
-            ["1,4", 2, 3, 5000, "1,2,3,4", "coassembly_0"],
-            ["5,8", 2, 3, 13000, "5,6,7,8", "coassembly_1"],
-            ["2,3", 2, 2, 5000, "2,3,4,5", "coassembly_2"],
-            ["1,2,4", 3, 2, 7000, "1,2,3,4", "coassembly_3"],
-            ["6,7", 2, 2, 13000, "5,6,7,8", "coassembly_4"],
-            ["1,2,3,4", 4, 1, 10000, "1,2,3,4", "coassembly_5"],
+            ["1,4", 2, 4, 5000, "1,2,3,4", "coassembly_0"],
+            ["2,3", 2, 3, 5000, "1,2,3,4", "coassembly_1"],
+            ["1,2,4", 3, 3, 7000, "1,2,3,4", "coassembly_2"],
+            ["5,8", 2, 3, 13000, "5,6,7,8", "coassembly_3"],
+            ["1,2,3,4", 4, 2, 10000, "1,2,3,4", "coassembly_4"],
+            ["6,7", 2, 2, 13000, "5,6,7,8", "coassembly_5"],
             ["5,6,7", 3, 1, 18000, "5,6,7,8", "coassembly_6"],
             ["5,6,7,8", 4, 1, 26000, "5,6,7,8", "coassembly_7"],
         ], schema=ELUSIVE_CLUSTERS_COLUMNS)
         observed = pipeline(
             elusive_edges,
             read_size,
             MAX_RECOVERY_SAMPLES=4,
```

### Comparing `binchicken-0.10.4/test/test_coassemble.py` & `binchicken-0.10.5/test/test_coassemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,14 +341,75 @@
                     ]),
                     ""
                 ]
             )
             with open(recover_path) as f:
                 self.assertEqual(expected, f.read())
 
+    def test_coassemble_unmap_runqc(self):
+        with in_tempdir():
+            cmd = (
+                f"binchicken coassemble "
+                f"--assemble-unmapped "
+                f"--run-qc "
+                f"--forward {SAMPLE_READS_FORWARD} "
+                f"--reverse {SAMPLE_READS_REVERSE} "
+                f"--genomes {GENOMES} "
+                f"--genome-transcripts {GENOME_TRANSCRIPTS} "
+                f"--sample-singlem {SAMPLE_SINGLEM} "
+                f"--sample-read-size {SAMPLE_READ_SIZE} "
+                f"--genome-singlem {GENOME_SINGLEM} "
+                f"--singlem-metapackage {METAPACKAGE} "
+                f"--output test "
+                f"--conda-prefix {path_to_conda} "
+            )
+            extern.run(cmd)
+
+            config_path = os.path.join("test", "config.yaml")
+            self.assertTrue(os.path.exists(config_path))
+
+            edges_path = os.path.join("test", "coassemble", "target", "targets.tsv")
+            self.assertTrue(os.path.exists(edges_path))
+
+            edges_path = os.path.join("test", "coassemble", "target", "elusive_edges.tsv")
+            self.assertTrue(os.path.exists(edges_path))
+
+            cluster_path = os.path.join("test", "coassemble", "target", "elusive_clusters.tsv")
+            self.assertTrue(os.path.exists(cluster_path))
+
+            qc_sample_1F_path = os.path.join("test", "coassemble", "qc", "sample_1_1.fastq.gz")
+            self.assertTrue(os.path.exists(qc_sample_1F_path))
+            qc_sample_1R_path = os.path.join("test", "coassemble", "qc", "sample_1_2.fastq.gz")
+            self.assertTrue(os.path.exists(qc_sample_1R_path))
+
+            qc_sample_2F_path = os.path.join("test", "coassemble", "qc", "sample_2_1.fastq.gz")
+            self.assertTrue(os.path.exists(qc_sample_2F_path))
+            qc_sample_2R_path = os.path.join("test", "coassemble", "qc", "sample_2_2.fastq.gz")
+            self.assertTrue(os.path.exists(qc_sample_2R_path))
+
+            qc_sample_3F_path = os.path.join("test", "coassemble", "qc", "sample_3_1.fastq.gz")
+            self.assertTrue(os.path.exists(qc_sample_3F_path))
+            qc_sample_3R_path = os.path.join("test", "coassemble", "qc", "sample_3_2.fastq.gz")
+            self.assertTrue(os.path.exists(qc_sample_3R_path))
+
+            map_sample_1F_path = os.path.join("test", "coassemble", "mapping", "sample_1_unmapped.1.fq.gz")
+            self.assertTrue(os.path.exists(map_sample_1F_path))
+            map_sample_1R_path = os.path.join("test", "coassemble", "mapping", "sample_1_unmapped.2.fq.gz")
+            self.assertTrue(os.path.exists(map_sample_1R_path))
+
+            map_sample_2F_path = os.path.join("test", "coassemble", "mapping", "sample_2_unmapped.1.fq.gz")
+            self.assertTrue(os.path.exists(map_sample_2F_path))
+            map_sample_2R_path = os.path.join("test", "coassemble", "mapping", "sample_2_unmapped.2.fq.gz")
+            self.assertTrue(os.path.exists(map_sample_2R_path))
+
+            map_sample_3F_path = os.path.join("test", "coassemble", "mapping", "sample_3_unmapped.1.fq.gz")
+            self.assertTrue(os.path.exists(map_sample_3F_path))
+            map_sample_3R_path = os.path.join("test", "coassemble", "mapping", "sample_3_unmapped.2.fq.gz")
+            self.assertTrue(os.path.exists(map_sample_3R_path))
+
     def test_coassemble_query_input(self):
         with in_tempdir():
             cmd = (
                 f"binchicken coassemble "
                 f"--forward {SAMPLE_READS_FORWARD} "
                 f"--reverse {SAMPLE_READS_REVERSE} "
                 f"--genomes {GENOMES} "
```

### Comparing `binchicken-0.10.4/test/test_collect_reference_bins.py` & `binchicken-0.10.5/test/test_collect_reference_bins.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.4/test/test_evaluate.py` & `binchicken-0.10.5/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.4/test/test_evaluate_script.py` & `binchicken-0.10.5/test/test_evaluate_script.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     "coassembly": str,
     "gene": str,
     "sequence": str,
     "genome": str,
     "target": str,
     "found_in": str,
     "source_samples": str,
+    "source_num_hits": int,
+    "source_coverage": float,
     "taxonomy": str,
     }
 SUMMARY_COLUMNS = {
     "coassembly": str,
     "statistic": str,
     "within": str,
     "match": int,
@@ -63,21 +65,21 @@
         ], schema=SINGLEM_COLUMNS)
         recovered_bins = {
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
-            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1", "Root"],
-            ["coassembly_0", "S3.1", "CCC", "genome_1_transcripts", None, None, "sample_1,sample_2", "Root"],
-            ["coassembly_0", "S3.1", "DDD", "genome_1_transcripts", None, None, "sample_1", "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", 10, 20.0, "Root"],
+            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1", 5, 10.0, "Root"],
+            ["coassembly_0", "S3.1", "CCC", "genome_1_transcripts", None, None, "sample_1,sample_2", 2, 4.0, "Root"],
+            ["coassembly_0", "S3.1", "DDD", "genome_1_transcripts", None, None, "sample_1", 1, 2.0, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 1, 0, 1, 100],
             ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
             ["coassembly_0", "nontarget_bin_sequences", "recovery", 1, 4, 5, 20.00],
             ["coassembly_0", "nontarget_unbin_sequences", "recovery", 2, 3, 5, 40.00],
             ["coassembly_0", "novel_sequences", "recovery", 1, 4, 5, 20.00],
@@ -108,15 +110,15 @@
         ], schema=SINGLEM_COLUMNS)
         recovered_bins = {
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", 10, 20.0, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 1, 0, 1, 100],
             ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
             ["coassembly_0", "nontarget_bin_sequences", "recovery", 0, 1, 1, 0],
@@ -149,18 +151,18 @@
         ], schema=SINGLEM_COLUMNS)
         recovered_bins = {
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", None, "10", None, "sample_1,sample_2", "Root; old"],
+            ["coassembly_0", "S3.1", "AAA", None, "10", None, "sample_1,sample_2", 10, 20.0, "Root; old"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 0, 1, 1, 0],
             ["coassembly_0", "taxonomy", "targets", 0, 1, 1, 0],
             ["coassembly_0", "nontarget_bin_sequences", "recovery", 0, 1, 1, 0],
             ["coassembly_0", "nontarget_unbin_sequences", "recovery", 0, 1, 1, 0],
             ["coassembly_0", "novel_sequences", "recovery", 1, 0, 1, 100],
@@ -226,19 +228,19 @@
         ], schema=SINGLEM_COLUMNS)
         recovered_bins = {
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", 10, 20.0, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
-            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, None, None, "Root"],
+            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, None, None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 1, 0, 1, 100],
             ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
             ["coassembly_0", "nontarget_bin_sequences", "recovery", 0, 3, 3, 0],
             ["coassembly_0", "nontarget_unbin_sequences", "recovery", 0, 3, 3, 0],
             ["coassembly_0", "novel_sequences", "recovery", 2, 1, 3, 66.67],
@@ -272,19 +274,19 @@
         ], schema=SINGLEM_COLUMNS)
         recovered_bins = {
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
-            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1,sample_2", "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", 10, 20.0, "Root"],
+            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1,sample_2", 10, 20.0, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 1, 0, 1, 100],
             ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
             ["coassembly_0", "nontarget_bin_sequences", "recovery", 1, 2, 3, 33.33],
             ["coassembly_0", "nontarget_unbin_sequences", "recovery", 0, 3, 3, 0],
             ["coassembly_0", "novel_sequences", "recovery", 1, 2, 3, 33.33],
@@ -330,23 +332,23 @@
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             "coassembly_1-genome_0": "genome_0.fna",
             "coassembly_1-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
-            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1", "Root"],
-            ["coassembly_1", "S3.1", "CCC", "genome_1_transcripts", "11", None, "sample_1,sample_3", "Root"],
-            ["coassembly_1", "S3.1", "DDD", "genome_1_transcripts", None, "oldgenome_2", "sample_3", "Root"],
-            ["coassembly_1", "S3.1", "EEE", "genome_1_transcripts", None, None, "sample_1,sample_3", "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", 10, 20.0, "Root"],
+            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1", 5, 10.0, "Root"],
+            ["coassembly_1", "S3.1", "CCC", "genome_1_transcripts", "11", None, "sample_1,sample_3", 10, 20.0, "Root"],
+            ["coassembly_1", "S3.1", "DDD", "genome_1_transcripts", None, "oldgenome_2", "sample_3", 5, 10.0, "Root"],
+            ["coassembly_1", "S3.1", "EEE", "genome_1_transcripts", None, None, "sample_1,sample_3", 2, 4.0, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
-            ["coassembly_1", "S3.1", "CCD", "genome_1_transcripts", None, None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, None, None, "Root"],
+            ["coassembly_1", "S3.1", "CCD", "genome_1_transcripts", None, None, None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 1, 0, 1, 100],
             ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
             ["coassembly_0", "nontarget_bin_sequences", "recovery", 1, 2, 3, 33.33],
             ["coassembly_0", "nontarget_unbin_sequences", "recovery", 0, 3, 3, 0],
             ["coassembly_0", "novel_sequences", "recovery", 1, 2, 3, 33.33],
@@ -398,25 +400,25 @@
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             "coassembly_1-genome_0": "genome_0.fna",
             "coassembly_1-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
-            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1", "Root"],
-            ["coassembly_0", "S3.1", "CCC", "genome_1_transcripts", "11", None, "sample_1,sample_3", "Root"],
-            ["coassembly_0", "S3.1", "DDD", "genome_1_transcripts", None, "oldgenome_2", "sample_3", "Root"],
-            ["coassembly_1", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
-            ["coassembly_1", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1", "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", 10, 20.0, "Root"],
+            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1", 5, 10.0, "Root"],
+            ["coassembly_0", "S3.1", "CCC", "genome_1_transcripts", "11", None, "sample_1,sample_3", 10, 20.0, "Root"],
+            ["coassembly_0", "S3.1", "DDD", "genome_1_transcripts", None, "oldgenome_2", "sample_3", 5, 10.0, "Root"],
+            ["coassembly_1", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", 10, 20.0, "Root"],
+            ["coassembly_1", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_1", 5, 10.0, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
-            ["coassembly_0", "S3.1", "CCD", "genome_1_transcripts", None, None, None, "Root"],
-            ["coassembly_1", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, None, None, "Root"],
+            ["coassembly_0", "S3.1", "CCD", "genome_1_transcripts", None, None, None, None, None, "Root"],
+            ["coassembly_1", "S3.1", "AAB", "genome_1_transcripts", None, None, None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 2, 0, 2, 100],
             ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
             ["coassembly_0", "nontarget_bin_sequences", "recovery", 2, 4, 6, 33.33],
             ["coassembly_0", "nontarget_unbin_sequences", "recovery", 0, 6, 6, 0],
             ["coassembly_0", "novel_sequences", "recovery", 2, 4, 6, 33.33],
@@ -472,27 +474,27 @@
             "coassembly_0-genome_1": "genome_1.fna",
             "coassembly_1-genome_0": "genome_0.fna",
             "coassembly_1-genome_1": "genome_1.fna",
             "coassembly_1-genome_2": "genome_2.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_0_transcripts", "10", None, "sample_1,sample_3", "Root"],
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_3", "Root"],
-            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_3", "Root"],
-            ["coassembly_0", "S3.1", "CCC", None, "11", None, "sample_1,sample_2", "Root; old"],
-            ["coassembly_0", "S3.1", "YYY", None, "98", None, "sample_1,sample_2", "Root; old"],
-            ["coassembly_0", "S3.1", "ZZZ", None, "99", None, "sample_2,sample_3", "Root; old"],
-            ["coassembly_1", "S3.1", "CCC", "genome_1_transcripts", "11", None, "sample_1,sample_2", "Root"],
-            ["coassembly_1", "S3.1", "DDD", "genome_1_transcripts", None, "oldgenome_2", "sample_1", "Root"],
-            ["coassembly_1", "S3.1", "YYY", None, "98", None, "sample_1,sample_2", "Root; old"],
+            ["coassembly_0", "S3.1", "AAA", "genome_0_transcripts", "10", None, "sample_1,sample_3", 10, 20.0, "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_3", 10, 20.0, "Root"],
+            ["coassembly_0", "S3.1", "BBB", "genome_1_transcripts", None, "oldgenome_1", "sample_3", 5, 10.0, "Root"],
+            ["coassembly_0", "S3.1", "CCC", None, "11", None, "sample_1,sample_2", 10, 20.0, "Root; old"],
+            ["coassembly_0", "S3.1", "YYY", None, "98", None, "sample_1,sample_2", 10, 20.0, "Root; old"],
+            ["coassembly_0", "S3.1", "ZZZ", None, "99", None, "sample_2,sample_3", 10, 20.0, "Root; old"],
+            ["coassembly_1", "S3.1", "CCC", "genome_1_transcripts", "11", None, "sample_1,sample_2", 10, 20.0, "Root"],
+            ["coassembly_1", "S3.1", "DDD", "genome_1_transcripts", None, "oldgenome_2", "sample_1", 5, 10.0, "Root"],
+            ["coassembly_1", "S3.1", "YYY", None, "98", None, "sample_1,sample_2", 10, 20.0, "Root; old"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, "Root"],
-            ["coassembly_1", "S3.1", "CCD", "genome_1_transcripts", None, None, None, "Root"],
+            ["coassembly_0", "S3.1", "AAB", "genome_1_transcripts", None, None, None, None, None, "Root"],
+            ["coassembly_1", "S3.1", "CCD", "genome_1_transcripts", None, None, None, None, None, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 1, 3, 4, 25],
             ["coassembly_0", "taxonomy", "targets", 1, 1, 2, 50],
             ["coassembly_0", "nontarget_bin_sequences", "recovery", 1, 3, 4, 25],
             ["coassembly_0", "nontarget_unbin_sequences", "recovery", 0, 4, 4, 0],
             ["coassembly_0", "novel_sequences", "recovery", 1, 3, 4, 25],
@@ -532,16 +534,16 @@
         ], schema=SINGLEM_COLUMNS)
         recovered_bins = {
             "coassembly_0-genome_0": "genome_0.fna",
             "coassembly_0-genome_1": "genome_1.fna",
             }
 
         expected_matches = pl.DataFrame([
-            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", "Root"],
-            ["coassembly_0", "S3.1", "CCC", "genome_1_transcripts", None, None, "sample_1", "Root"],
+            ["coassembly_0", "S3.1", "AAA", "genome_1_transcripts", "10", None, "sample_1,sample_2", 10, 20.0, "Root"],
+            ["coassembly_0", "S3.1", "CCC", "genome_1_transcripts", None, None, "sample_1", 1, 2.0, "Root"],
         ], schema=OUTPUT_COLUMNS)
         expected_unmatched = pl.DataFrame([
         ], schema=OUTPUT_COLUMNS)
         expected_summary = pl.DataFrame([
             ["coassembly_0", "sequences", "targets", 1, 0, 1, 100],
             ["coassembly_0", "taxonomy", "targets", 1, 0, 1, 100],
             ["coassembly_0", "nontarget_bin_sequences", "recovery", 0, 2, 2, 0],
```

### Comparing `binchicken-0.10.4/test/test_is_interleaved.py` & `binchicken-0.10.5/test/test_is_interleaved.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.4/test/test_iterate.py` & `binchicken-0.10.5/test/test_iterate.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.4/test/test_manual.py` & `binchicken-0.10.5/test/test_manual.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ])
 GENOMES = " ".join([os.path.join(path_to_data, "GB_GCA_013286235.1.fna")])
 TWO_GENOMES = " ".join([
     os.path.join(path_to_data, "GB_GCA_013286235.1.fna"),
     os.path.join(path_to_data, "GB_GCA_013286235.2.fna"),
     ])
 
-MOCK_COASSEMBLE = os.path.join(path_to_data, "mock_coassemble")
+MOCK_COASSEMBLE = os.path.join(path_to_data, "mock_coassemble", "coassemble")
 APPRAISE_BINNED = os.path.join(MOCK_COASSEMBLE, "coassemble", "appraise", "binned.otu_table.tsv")
 APPRAISE_UNBINNED = os.path.join(MOCK_COASSEMBLE, "coassemble", "appraise", "unbinned.otu_table.tsv")
 ELUSIVE_CLUSTERS = os.path.join(MOCK_COASSEMBLE, "coassemble", "target", "elusive_clusters.tsv")
 ELUSIVE_CLUSTERS_TWO = os.path.join(MOCK_COASSEMBLE, "coassemble", 'target', 'elusive_clusters_two.tsv')
 
 
 class Tests(unittest.TestCase):
@@ -98,14 +98,15 @@
             f"--coassemble-elusive-clusters {os.path.join(MOCK_COASSEMBLE, 'target', 'elusive_clusters_sra.tsv')} "
             f"--coassemble-summary {os.path.join(MOCK_COASSEMBLE, 'summary.tsv')} "
             f"--output {output_dir} "
             f"--conda-prefix {path_to_conda} "
             f"--snakemake-profile mqsub "
             f"--local-cores 5 "
             f"--cluster-retries 1 "
+            f"--cluster-submission "
         )
         subprocess.run(cmd, shell=True, check=True)
 
         config_path = os.path.join(output_dir, "config.yaml")
         self.assertTrue(os.path.exists(config_path))
 
         self.assertTrue(os.path.exists(os.path.join(output_dir, "coassemble", "sra", "SRR8334323_1.fastq.gz")))
@@ -135,15 +136,18 @@
             f"--coassemble-binned {os.path.join(MOCK_COASSEMBLE, 'appraise', 'binned_sra.otu_table.tsv')} "
             f"--coassemble-targets {os.path.join(MOCK_COASSEMBLE, 'target', 'targets.tsv')} "
             f"--coassemble-elusive-edges {os.path.join(MOCK_COASSEMBLE, 'target', 'elusive_edges.tsv')} "
             f"--coassemble-elusive-clusters {os.path.join(MOCK_COASSEMBLE, 'target', 'elusive_clusters_sra_large.tsv')} "
             f"--coassemble-summary {os.path.join(MOCK_COASSEMBLE, 'summary.tsv')} "
             f"--output {output_dir} "
             f"--conda-prefix {path_to_conda} "
-            f"--snakemake-args '--profile mqsub --retries 1' "
+            f"--snakemake-profile mqsub "
+            f"--local-cores 5 "
+            f"--cluster-retries 1 "
+            f"--cluster-submission "
         )
         subprocess.run(cmd, shell=True, check=True)
 
 
         config_path = os.path.join(output_dir, "config.yaml")
         self.assertTrue(os.path.exists(config_path))
```

### Comparing `binchicken-0.10.4/test/test_no_genomes.py` & `binchicken-0.10.5/test/test_no_genomes.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.4/test/test_query_processing.py` & `binchicken-0.10.5/test/test_query_processing.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.4/test/test_summarise_coassemblies.py` & `binchicken-0.10.5/test/test_summarise_coassemblies.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "total_targets": int,
     "total_size": int,
     "unmapped_size": int,
     }
 
 class Tests(unittest.TestCase):
     def assertDataFrameEqual(self, a, b):
-        assert_frame_equal(a, b, check_dtype=False)
+        assert_frame_equal(a, b, check_dtype=False, check_row_order=False)
 
     def test_summarise_coassemblies(self):
         elusive_clusters = pl.DataFrame([
             ["coassembly_1", "sample_1,sample_2", 2, 200, 1000],
             ["coassembly_2", "sample_1,sample_3", 2, 100, 2000],
         ], schema=ELUSIVE_CLUSTERS_COLUMNS)
```

### Comparing `binchicken-0.10.4/test/test_target_elusive.py` & `binchicken-0.10.5/test/test_target_elusive.py`

 * *Files identical despite different names*

### Comparing `binchicken-0.10.4/test/test_update.py` & `binchicken-0.10.5/test/test_update.py`

 * *Files identical despite different names*

