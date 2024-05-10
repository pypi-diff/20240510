# Comparing `tmp/pheval-0.3.5.tar.gz` & `tmp/pheval-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheval-0.3.5.tar", max compression
+gzip compressed data, was "pheval-0.3.6.tar", max compression
```

## Comparing `pheval-0.3.5.tar` & `pheval-0.3.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0    11357 2024-04-25 15:18:28.184908 pheval-0.3.5/LICENSE
--rw-r--r--   0        0        0      751 2024-04-25 15:18:28.184908 pheval-0.3.5/README.md
--rw-r--r--   0        0        0     1529 2024-04-25 15:18:28.244908 pheval-0.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/__init__.py
--rw-r--r--   0        0        0     7743 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/analysis.py
--rw-r--r--   0        0        0     5943 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/benchmark_generator.py
--rw-r--r--   0        0        0      768 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/benchmarking_data.py
--rw-r--r--   0        0        0    12519 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/binary_classification_stats.py
--rw-r--r--   0        0        0    12649 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/disease_prioritisation_analysis.py
--rw-r--r--   0        0        0    12373 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/gene_prioritisation_analysis.py
--rw-r--r--   0        0        0    21350 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/generate_plots.py
--rw-r--r--   0        0        0     6591 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/generate_summary_outputs.py
--rw-r--r--   0        0        0     2384 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/parse_benchmark_summary.py
--rw-r--r--   0        0        0     1211 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/parse_pheval_result.py
--rw-r--r--   0        0        0     3223 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/prioritisation_rank_recorder.py
--rw-r--r--   0        0        0     1228 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/prioritisation_result_types.py
--rw-r--r--   0        0        0    15785 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/rank_stats.py
--rw-r--r--   0        0        0     1552 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/run_data_parser.py
--rw-r--r--   0        0        0    12384 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/analyse/variant_prioritisation_analysis.py
--rw-r--r--   0        0        0     1570 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/cli.py
--rw-r--r--   0        0        0     2424 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/cli_pheval.py
--rw-r--r--   0        0        0    20504 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/cli_pheval_utils.py
--rw-r--r--   0        0        0     1227 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/config_parser.py
--rw-r--r--   0        0        0      349 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/constants.py
--rw-r--r--   0        0        0     1228 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/implementations/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/infra/__init__.py
--rw-r--r--   0        0        0     5080 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/infra/exomiserdb.py
--rw-r--r--   0        0        0        0 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/post_processing/__init__.py
--rw-r--r--   0        0        0    16030 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/post_processing/post_processing.py
--rw-r--r--   0        0        0        0 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/prepare/__init__.py
--rw-r--r--   0        0        0    11236 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/prepare/create_noisy_phenopackets.py
--rw-r--r--   0        0        0    20235 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/prepare/create_spiked_vcf.py
--rw-r--r--   0        0        0     1719 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/prepare/custom_exceptions.py
--rw-r--r--   0        0        0     3456 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/prepare/prepare_corpus.py
--rw-r--r--   0        0        0     4770 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/prepare/update_phenopacket.py
--rw-r--r--   0        0        0      547 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/resources/alternate_ouputs/CADA_results.txt
--rw-r--r--   0        0        0     1508 2024-04-25 15:18:28.244908 pheval-0.3.5/src/pheval/resources/alternate_ouputs/DeepPVP_results.txt
--rw-r--r--   0        0        0     9845 2024-04-25 15:18:28.248908 pheval-0.3.5/src/pheval/resources/alternate_ouputs/OVA_results.txt
--rw-r--r--   0        0        0    14148 2024-04-25 15:18:28.248908 pheval-0.3.5/src/pheval/resources/alternate_ouputs/Phen2Gene_results.json
--rw-r--r--   0        0        0      594 2024-04-25 15:18:28.248908 pheval-0.3.5/src/pheval/resources/alternate_ouputs/Phenolyzer_results.txt
--rw-r--r--   0        0        0   431068 2024-04-25 15:18:28.248908 pheval-0.3.5/src/pheval/resources/alternate_ouputs/lirical_results.tsv
--rw-r--r--   0        0        0      714 2024-04-25 15:18:28.248908 pheval-0.3.5/src/pheval/resources/alternate_ouputs/svanna_results.tsv
--rw-r--r--   0        0        0 16462969 2024-04-25 15:18:28.312909 pheval-0.3.5/src/pheval/resources/hgnc_complete_set.txt
--rw-r--r--   0        0        0      919 2024-04-25 15:18:28.312909 pheval-0.3.5/src/pheval/run_metadata.py
--rw-r--r--   0        0        0        0 2024-04-25 15:18:28.312909 pheval-0.3.5/src/pheval/runners/__init__.py
--rw-r--r--   0        0        0     4451 2024-04-25 15:18:28.312909 pheval-0.3.5/src/pheval/runners/runner.py
--rw-r--r--   0        0        0        0 2024-04-25 15:18:28.312909 pheval-0.3.5/src/pheval/utils/__init__.py
--rw-r--r--   0        0        0     3193 2024-04-25 15:18:28.312909 pheval-0.3.5/src/pheval/utils/docs_gen.py
--rwxr-xr-x   0        0        0      477 2024-04-25 15:18:28.312909 pheval-0.3.5/src/pheval/utils/docs_gen.sh
--rw-r--r--   0        0        0      683 2024-04-25 15:18:28.312909 pheval-0.3.5/src/pheval/utils/exomiser.py
--rw-r--r--   0        0        0     4640 2024-04-25 15:18:28.312909 pheval-0.3.5/src/pheval/utils/file_utils.py
--rw-r--r--   0        0        0    26792 2024-04-25 15:18:28.312909 pheval-0.3.5/src/pheval/utils/phenopacket_utils.py
--rw-r--r--   0        0        0     6151 2024-04-25 15:18:28.312909 pheval-0.3.5/src/pheval/utils/semsim_utils.py
--rw-r--r--   0        0        0     2343 2024-04-25 15:18:28.312909 pheval-0.3.5/src/pheval/utils/utils.py
--rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 pheval-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 19:16:19.207976 pheval-0.3.6/LICENSE
+-rw-r--r--   0        0        0      751 2024-05-10 19:16:19.207976 pheval-0.3.6/README.md
+-rw-r--r--   0        0        0     1529 2024-05-10 19:16:19.267976 pheval-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/__init__.py
+-rw-r--r--   0        0        0     7743 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/analysis.py
+-rw-r--r--   0        0        0     5943 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/benchmark_generator.py
+-rw-r--r--   0        0        0      768 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/benchmarking_data.py
+-rw-r--r--   0        0        0    12519 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/binary_classification_stats.py
+-rw-r--r--   0        0        0    12649 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/disease_prioritisation_analysis.py
+-rw-r--r--   0        0        0    12373 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/gene_prioritisation_analysis.py
+-rw-r--r--   0        0        0    21350 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/generate_plots.py
+-rw-r--r--   0        0        0     6591 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/generate_summary_outputs.py
+-rw-r--r--   0        0        0     2384 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/parse_benchmark_summary.py
+-rw-r--r--   0        0        0     1211 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/parse_pheval_result.py
+-rw-r--r--   0        0        0     3223 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/prioritisation_rank_recorder.py
+-rw-r--r--   0        0        0     1228 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/prioritisation_result_types.py
+-rw-r--r--   0        0        0    15785 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/rank_stats.py
+-rw-r--r--   0        0        0     1552 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/run_data_parser.py
+-rw-r--r--   0        0        0    12384 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/analyse/variant_prioritisation_analysis.py
+-rw-r--r--   0        0        0     1570 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/cli.py
+-rw-r--r--   0        0        0     2424 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/cli_pheval.py
+-rw-r--r--   0        0        0    20504 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/cli_pheval_utils.py
+-rw-r--r--   0        0        0     1227 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/config_parser.py
+-rw-r--r--   0        0        0      349 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/constants.py
+-rw-r--r--   0        0        0     1228 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/infra/__init__.py
+-rw-r--r--   0        0        0     5080 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/infra/exomiserdb.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/post_processing/__init__.py
+-rw-r--r--   0        0        0    13368 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/post_processing/post_processing.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/prepare/__init__.py
+-rw-r--r--   0        0        0    11236 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/prepare/create_noisy_phenopackets.py
+-rw-r--r--   0        0        0    21111 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/prepare/create_spiked_vcf.py
+-rw-r--r--   0        0        0     1719 2024-05-10 19:16:19.267976 pheval-0.3.6/src/pheval/prepare/custom_exceptions.py
+-rw-r--r--   0        0        0     3692 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/prepare/prepare_corpus.py
+-rw-r--r--   0        0        0     4770 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/prepare/update_phenopacket.py
+-rw-r--r--   0        0        0      547 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/CADA_results.txt
+-rw-r--r--   0        0        0     1508 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/DeepPVP_results.txt
+-rw-r--r--   0        0        0     9845 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/OVA_results.txt
+-rw-r--r--   0        0        0    14148 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/Phen2Gene_results.json
+-rw-r--r--   0        0        0      594 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/Phenolyzer_results.txt
+-rw-r--r--   0        0        0   431068 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/lirical_results.tsv
+-rw-r--r--   0        0        0      714 2024-05-10 19:16:19.271976 pheval-0.3.6/src/pheval/resources/alternate_ouputs/svanna_results.tsv
+-rw-r--r--   0        0        0 16462969 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/resources/hgnc_complete_set.txt
+-rw-r--r--   0        0        0      919 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/run_metadata.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/runners/__init__.py
+-rw-r--r--   0        0        0     4451 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/runners/runner.py
+-rw-r--r--   0        0        0        0 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/__init__.py
+-rw-r--r--   0        0        0     3193 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/docs_gen.py
+-rwxr-xr-x   0        0        0      477 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/docs_gen.sh
+-rw-r--r--   0        0        0      683 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/exomiser.py
+-rw-r--r--   0        0        0     4640 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/file_utils.py
+-rw-r--r--   0        0        0    26792 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/phenopacket_utils.py
+-rw-r--r--   0        0        0     6151 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/semsim_utils.py
+-rw-r--r--   0        0        0     2343 2024-05-10 19:16:19.335976 pheval-0.3.6/src/pheval/utils/utils.py
+-rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 pheval-0.3.6/PKG-INFO
```

### Comparing `pheval-0.3.5/LICENSE` & `pheval-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/README.md` & `pheval-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/pyproject.toml` & `pheval-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pheval"
-version = "0.3.5"
+version = "0.3.6"
 description = ""
 authors = ["Yasemin Bridges <y.bridges@qmul.ac.uk>",
   "Julius Jacobsen <j.jacobsen@qmul.ac.uk>",
   "Nico Matentzoglu <nicolas.matentzoglu@gmail.com>",
   "Vinícius de Souza <souzadevinicius@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pheval", from = "src"}]
```

### Comparing `pheval-0.3.5/src/pheval/analyse/analysis.py` & `pheval-0.3.6/src/pheval/analyse/analysis.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/benchmark_generator.py` & `pheval-0.3.6/src/pheval/analyse/benchmark_generator.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/benchmarking_data.py` & `pheval-0.3.6/src/pheval/analyse/benchmarking_data.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/binary_classification_stats.py` & `pheval-0.3.6/src/pheval/analyse/binary_classification_stats.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/disease_prioritisation_analysis.py` & `pheval-0.3.6/src/pheval/analyse/disease_prioritisation_analysis.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/gene_prioritisation_analysis.py` & `pheval-0.3.6/src/pheval/analyse/gene_prioritisation_analysis.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/generate_plots.py` & `pheval-0.3.6/src/pheval/analyse/generate_plots.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/generate_summary_outputs.py` & `pheval-0.3.6/src/pheval/analyse/generate_summary_outputs.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/parse_benchmark_summary.py` & `pheval-0.3.6/src/pheval/analyse/parse_benchmark_summary.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/parse_pheval_result.py` & `pheval-0.3.6/src/pheval/analyse/parse_pheval_result.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/prioritisation_rank_recorder.py` & `pheval-0.3.6/src/pheval/analyse/prioritisation_rank_recorder.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/prioritisation_result_types.py` & `pheval-0.3.6/src/pheval/analyse/prioritisation_result_types.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/rank_stats.py` & `pheval-0.3.6/src/pheval/analyse/rank_stats.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/run_data_parser.py` & `pheval-0.3.6/src/pheval/analyse/run_data_parser.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/analyse/variant_prioritisation_analysis.py` & `pheval-0.3.6/src/pheval/analyse/variant_prioritisation_analysis.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/cli.py` & `pheval-0.3.6/src/pheval/cli.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/cli_pheval.py` & `pheval-0.3.6/src/pheval/cli_pheval.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/cli_pheval_utils.py` & `pheval-0.3.6/src/pheval/cli_pheval_utils.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/config_parser.py` & `pheval-0.3.6/src/pheval/config_parser.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/implementations/__init__.py` & `pheval-0.3.6/src/pheval/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/infra/exomiserdb.py` & `pheval-0.3.6/src/pheval/infra/exomiserdb.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/post_processing/post_processing.py` & `pheval-0.3.6/src/pheval/post_processing/post_processing.py`

 * *Files 22% similar despite different names*

```diff
@@ -223,113 +223,34 @@
         return (
             self._sort_by_increasing_score()
             if self.sort_order == SortOrder.ASCENDING
             else self._sort_by_decreasing_score()
         )
 
 
-class ScoreRanker:
-    """
-    Class for ranking scores based on a given sort order
-
-    Attributes:
-       rank (int): Represents the current rank, initialised with 0
-       current_score (float): Represents the current score, initialised with positive infinity (float("inf"))
-       count (int): Used for counting, initialised with 0
-    """
-
-    rank: int = 0
-    current_score: float = float("inf")
-    count: int = 0
-
-    def __init__(self, sort_order: SortOrder):
-        """
-        Initialise ScoreRanker
-
-        Args:
-            sort_order (SortOrder): Sorting order to be applied
-        """
-        self.sort_order = sort_order
-
-    def _check_rank_order(self, round_score: float) -> None:
-        """
-        Check if the results are correctly ordered
-
-        Args:
-            round_score (float): Score to be checked against the current score
-
-        Raises:
-            ValueError: If results are not correctly sorted.
-        """
-        if self.sort_order == SortOrder.ASCENDING and round_score < self.current_score != float(
-            "inf"
-        ):
-            raise ValueError("Results are not correctly sorted!")
-        elif self.sort_order == SortOrder.DESCENDING and round_score > self.current_score != float(
-            "inf"
-        ):
-            raise ValueError("Results are not correctly sorted!")
-
-    def rank_scores(self, round_score: float) -> int:
-        """
-        Add ranks to a result; equal scores are given the same rank, e.g., 1, 1, 3
-
-        Args:
-            round_score (float): Score to be ranked
-
-        Returns:
-            int: Rank assigned to the score
-        """
-        self._check_rank_order(round_score)
-        self.count += 1
-        if self.current_score == round_score:
-            return self.rank
-        self.current_score = round_score
-        self.rank = self.count
-        return self.rank
-
-
-def _rank_pheval_result(pheval_result: [PhEvalResult], sort_order: SortOrder) -> [PhEvalResult]:
+def _rank_pheval_result(pheval_result: [PhEvalResult], sort_order: SortOrder) -> pd.DataFrame:
     """
     Rank PhEval results post-processed from tool-specific output, managing tied scores (ex aequo)
 
     Args:
         pheval_result ([PhEvalResult]): PhEval results obtained from tool-specific output
         sort_order (SortOrder): Sorting order based on which ranking is performed
 
     Returns:
-        List[PhEvalResult]: Ranked PhEval results with tied scores managed
+        pd.DataFrame : Ranked PhEval results with tied scores managed
 
     Raises:
         ValueError: If an incompatible PhEval result type is encountered
     """
-    score_ranker = ScoreRanker(sort_order)
-    ranked_result = []
-    for result in pheval_result:
-        if type(result) == PhEvalGeneResult:
-            ranked_result.append(
-                RankedPhEvalGeneResult.from_gene_result(
-                    result, score_ranker.rank_scores(result.score)
-                )
-            )
-        elif type(result) == PhEvalVariantResult:
-            ranked_result.append(
-                RankedPhEvalVariantResult.from_variant_result(
-                    result, score_ranker.rank_scores(result.score)
-                )
-            )
-        elif type(result) == PhEvalDiseaseResult:
-            ranked_result.append(
-                RankedPhEvalDiseaseResult.from_disease_result(
-                    result, score_ranker.rank_scores(result.score)
-                )
-            )
-        else:
-            raise ValueError("Incompatible PhEval result type.")
-    return ranked_result
+    pheval_result_df = pd.DataFrame([data.__dict__ for data in pheval_result])
+    if sort_order == SortOrder.ASCENDING:
+        pheval_result_df["rank"] = pheval_result_df["score"].rank(method="max", ascending=True)
+    elif sort_order == SortOrder.DESCENDING:
+        pheval_result_df["rank"] = pheval_result_df["score"].rank(method="max", ascending=False)
+    return pheval_result_df
 
 
 def _return_sort_order(sort_order_str: str) -> SortOrder:
     """
     Convert a string derived from the config file into SortOrder Enum
 
     Args:
@@ -343,89 +264,88 @@
     """
     try:
         return SortOrder[sort_order_str.upper()]
     except KeyError:
         raise ValueError("Incompatible ordering method specified.")
 
 
-def _create_pheval_result(pheval_result: [PhEvalResult], sort_order_str: str) -> [PhEvalResult]:
+def _create_pheval_result(pheval_result: [PhEvalResult], sort_order_str: str) -> pd.DataFrame:
     """
     Create PhEval results with corresponding ranks based on the specified sorting order.
 
     Args:
         pheval_result ([PhEvalResult]): List of PhEvalResult instances to be processed.
         sort_order_str (str): String representation of the desired sorting order.
 
     Returns:
-        List[PhEvalResult]: PhEval results with ranks assigned.
+       pd.DataFrame: PhEval results with ranks assigned.
     """
     sort_order = _return_sort_order(sort_order_str)
     sorted_pheval_result = ResultSorter(pheval_result, sort_order).sort_pheval_results()
     return _rank_pheval_result(sorted_pheval_result, sort_order)
 
 
 def _write_pheval_gene_result(
-    ranked_pheval_result: [PhEvalResult], output_dir: Path, tool_result_path: Path
+    ranked_pheval_result: pd.DataFrame, output_dir: Path, tool_result_path: Path
 ) -> None:
     """
     Write ranked PhEval gene results to a TSV file
 
     Args:
         ranked_pheval_result ([PhEvalResult]): List of ranked PhEval gene results
         output_dir (Path): Path to the output directory
         tool_result_path (Path): Path to the tool-specific result file
     """
-    ranked_result = pd.DataFrame([data.__dict__ for data in ranked_pheval_result])
-    pheval_gene_output = ranked_result.loc[:, ["rank", "score", "gene_symbol", "gene_identifier"]]
+    pheval_gene_output = ranked_pheval_result.loc[
+        :, ["rank", "score", "gene_symbol", "gene_identifier"]
+    ]
     pheval_gene_output.to_csv(
         output_dir.joinpath(
             "pheval_gene_results/" + tool_result_path.stem + "-pheval_gene_result.tsv"
         ),
         sep="\t",
         index=False,
     )
 
 
 def _write_pheval_variant_result(
-    ranked_pheval_result: [PhEvalResult], output_dir: Path, tool_result_path: Path
+    ranked_pheval_result: pd.DataFrame, output_dir: Path, tool_result_path: Path
 ) -> None:
     """
     Write ranked PhEval variant results to a TSV file
 
     Args:
         ranked_pheval_result ([PhEvalResult]): List of ranked PhEval gene results
         output_dir (Path): Path to the output directory
         tool_result_path (Path): Path to the tool-specific result file
     """
-    ranked_result = pd.DataFrame([data.__dict__ for data in ranked_pheval_result])
-    pheval_variant_output = ranked_result.loc[
+    pheval_variant_output = ranked_pheval_result.loc[
         :, ["rank", "score", "chromosome", "start", "end", "ref", "alt"]
     ]
     pheval_variant_output.to_csv(
         output_dir.joinpath(
             "pheval_variant_results/" + tool_result_path.stem + "-pheval_variant_result.tsv"
         ),
         sep="\t",
         index=False,
     )
 
 
 def _write_pheval_disease_result(
-    ranked_pheval_result: [RankedPhEvalDiseaseResult], output_dir: Path, tool_result_path: Path
+    ranked_pheval_result: pd.DataFrame, output_dir: Path, tool_result_path: Path
 ) -> None:
     """
     Write ranked PhEval disease results to a TSV file
 
     Args:
         ranked_pheval_result ([PhEvalResult]): List of ranked PhEval gene results
         output_dir (Path): Path to the output directory
         tool_result_path (Path): Path to the tool-specific result file
     """
-    ranked_result = pd.DataFrame([data.__dict__ for data in ranked_pheval_result])
-    pheval_disease_output = ranked_result.loc[
+    pheval_disease_output = ranked_pheval_result.loc[
         :, ["rank", "score", "disease_name", "disease_identifier"]
     ]
     pheval_disease_output.to_csv(
         output_dir.joinpath(
             "pheval_disease_results/" + tool_result_path.stem + "-pheval_disease_result.tsv"
         ),
         sep="\t",
```

### Comparing `pheval-0.3.5/src/pheval/prepare/create_noisy_phenopackets.py` & `pheval-0.3.6/src/pheval/prepare/create_noisy_phenopackets.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/prepare/create_spiked_vcf.py` & `pheval-0.3.6/src/pheval/prepare/create_spiked_vcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,59 +324,78 @@
             "100",
             "PASS",
             proband_variant_data.info if proband_variant_data.info else ".",
             "GT",
             genotype_codes[proband_variant_data.genotype.lower()] + "\n",
         ]
 
-    def construct_vcf_records(self) -> List[str]:
+    def construct_vcf_records(self, template_vcf_name: str) -> List[str]:
         """
         Construct updated VCF records by inserting spiked variants into the correct positions within the VCF.
 
+        Args:
+            template_vcf_name (str): Name of the template VCF file.
+
         Returns:
             List[str]: Updated VCF records containing the spiked variants.
         """
         updated_vcf_records = copy(self.vcf_contents)
         for variant in self.proband_causative_variants:
-            variant = self.construct_variant_entry(variant)
-            variant_entry_position = [
+            variant_entry = self.construct_variant_entry(variant)
+            matching_indices = [
                 i
                 for i, val in enumerate(updated_vcf_records)
-                if val.split("\t")[0] == variant[0] and int(val.split("\t")[1]) < int(variant[1])
-            ][-1] + 1
-            updated_vcf_records.insert(variant_entry_position, "\t".join(variant))
+                if val.split("\t")[0] == variant_entry[0]
+                and int(val.split("\t")[1]) < int(variant_entry[1])
+            ]
+            if matching_indices:
+                variant_entry_position = matching_indices[-1] + 1
+            else:
+                info_log.warning(
+                    f"Could not find entry position for {variant.variant.chrom}-{variant.variant.pos}-"
+                    f"{variant.variant.ref}-{variant.variant.alt} in {template_vcf_name}, "
+                    "inserting at end of VCF contents."
+                )
+                variant_entry_position = len(updated_vcf_records)
+            updated_vcf_records.insert(variant_entry_position, "\t".join(variant_entry))
         return updated_vcf_records
 
     def construct_header(self, updated_vcf_records: List[str]) -> List[str]:
         """
         Construct the header of the VCF.
 
         Args:
             updated_vcf_records (List[str]): Updated VCF records.
 
         Returns:
             List[str]: Constructed header as a list of strings.
         """
         updated_vcf_file = []
         for line in updated_vcf_records:
-            text = line.replace(
-                self.vcf_header.sample_id,
-                self.proband_causative_variants[0].proband_id,
-            )
+            if line.startswith("#"):
+                text = line.replace(
+                    self.vcf_header.sample_id,
+                    self.proband_causative_variants[0].proband_id,
+                )
+            else:
+                text = line
             updated_vcf_file.append(text)
         return updated_vcf_file
 
-    def construct_vcf(self) -> List[str]:
+    def construct_vcf(self, template_vcf_name: str) -> List[str]:
         """
         Construct the entire spiked VCF file by incorporating the spiked variants into the VCF.
 
+        Args:
+            template_vcf_name (str): Name of the template VCF file.
+
         Returns:
             List[str]: The complete spiked VCF file content as a list of strings.
         """
-        return self.construct_header(self.construct_vcf_records())
+        return self.construct_header(self.construct_vcf_records(template_vcf_name))
 
 
 class VcfWriter:
     """Class for writing VCF file."""
 
     def __init__(
         self,
@@ -450,15 +469,15 @@
     )
     return (
         chosen_template_vcf.vcf_header.assembly,
         VcfSpiker(
             chosen_template_vcf.vcf_contents,
             phenopacket_causative_variants,
             chosen_template_vcf.vcf_header,
-        ).construct_vcf(),
+        ).construct_vcf(chosen_template_vcf.vcf_file_name),
     )
 
 
 def generate_spiked_vcf_file(
     output_dir: Path,
     phenopacket: Union[Phenopacket, Family],
     phenopacket_path: Path,
```

### Comparing `pheval-0.3.5/src/pheval/prepare/custom_exceptions.py` & `pheval-0.3.6/src/pheval/prepare/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/prepare/prepare_corpus.py` & `pheval-0.3.6/src/pheval/prepare/prepare_corpus.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,19 @@
         hg38_template_vcf (Path): Path to the hg38 template VCF file (optional), to spike variants into
         VCFs for variant-based analysis at least one of hg19_template_vcf or hg38_template_vcf is required.
         output_dir (Path): The directory to save the prepared Phenopackets and, optionally, VCF files.
     """
     output_dir.joinpath("phenopackets").mkdir(exist_ok=True, parents=True)
     for phenopacket_path in all_files(phenopacket_dir):
         phenopacket_util = PhenopacketUtil(phenopacket_reader(phenopacket_path))
+        if not phenopacket_util.observed_phenotypic_features():
+            info_log.warning(
+                f"Removed {phenopacket_path.name} from the corpus due to no observed phenotypic features."
+            )
+            continue
         if variant_analysis:
             if phenopacket_util.check_incomplete_variant_record():
                 info_log.warning(
                     f"Removed {phenopacket_path.name} from the corpus due to missing variant fields."
                 )
                 continue
         if gene_analysis:
```

### Comparing `pheval-0.3.5/src/pheval/prepare/update_phenopacket.py` & `pheval-0.3.6/src/pheval/prepare/update_phenopacket.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/resources/alternate_ouputs/CADA_results.txt` & `pheval-0.3.6/src/pheval/resources/alternate_ouputs/CADA_results.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/resources/alternate_ouputs/DeepPVP_results.txt` & `pheval-0.3.6/src/pheval/resources/alternate_ouputs/DeepPVP_results.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/resources/alternate_ouputs/OVA_results.txt` & `pheval-0.3.6/src/pheval/resources/alternate_ouputs/OVA_results.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/resources/alternate_ouputs/Phen2Gene_results.json` & `pheval-0.3.6/src/pheval/resources/alternate_ouputs/Phen2Gene_results.json`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/resources/alternate_ouputs/Phenolyzer_results.txt` & `pheval-0.3.6/src/pheval/resources/alternate_ouputs/Phenolyzer_results.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/resources/alternate_ouputs/lirical_results.tsv` & `pheval-0.3.6/src/pheval/resources/alternate_ouputs/lirical_results.tsv`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/resources/alternate_ouputs/svanna_results.tsv` & `pheval-0.3.6/src/pheval/resources/alternate_ouputs/svanna_results.tsv`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/resources/hgnc_complete_set.txt` & `pheval-0.3.6/src/pheval/resources/hgnc_complete_set.txt`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/run_metadata.py` & `pheval-0.3.6/src/pheval/run_metadata.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/runners/runner.py` & `pheval-0.3.6/src/pheval/runners/runner.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/utils/docs_gen.py` & `pheval-0.3.6/src/pheval/utils/docs_gen.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/utils/exomiser.py` & `pheval-0.3.6/src/pheval/utils/exomiser.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/utils/file_utils.py` & `pheval-0.3.6/src/pheval/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/utils/phenopacket_utils.py` & `pheval-0.3.6/src/pheval/utils/phenopacket_utils.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/utils/semsim_utils.py` & `pheval-0.3.6/src/pheval/utils/semsim_utils.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/src/pheval/utils/utils.py` & `pheval-0.3.6/src/pheval/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pheval-0.3.5/PKG-INFO` & `pheval-0.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheval
-Version: 0.3.5
+Version: 0.3.6
 Summary: 
 Author: Yasemin Bridges
 Author-email: y.bridges@qmul.ac.uk
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

