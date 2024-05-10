# Comparing `tmp/clipzyme-0.0.5.tar.gz` & `tmp/clipzyme-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipzyme-0.0.5.tar", max compression
+gzip compressed data, was "clipzyme-0.0.6.tar", max compression
```

## Comparing `clipzyme-0.0.5.tar` & `clipzyme-0.0.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    11358 2024-03-28 18:26:04.343837 clipzyme-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     7694 2024-04-08 16:54:12.469585 clipzyme-0.0.5/README.md
--rw-r--r--   0        0        0     1788 2024-03-29 19:24:34.636971 clipzyme-0.0.5/clipzyme/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.578850 clipzyme-0.0.5/clipzyme/callbacks/__init__.py
--rw-r--r--   0        0        0      948 2024-03-28 15:53:13.579321 clipzyme-0.0.5/clipzyme/callbacks/basic.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.579397 clipzyme-0.0.5/clipzyme/datasets/__init__.py
--rw-r--r--   0        0        0     8552 2024-03-28 15:53:13.579934 clipzyme-0.0.5/clipzyme/datasets/abstract.py
--rw-r--r--   0        0        0    12769 2024-03-28 15:53:13.580656 clipzyme-0.0.5/clipzyme/datasets/enzyme_screening.py
--rw-r--r--   0        0        0    43705 2024-04-08 16:54:12.470132 clipzyme-0.0.5/clipzyme/datasets/enzymemap.py
--rw-r--r--   0        0        0    11816 2024-04-08 02:52:05.338533 clipzyme-0.0.5/clipzyme/datasets/reaction.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.581466 clipzyme-0.0.5/clipzyme/learning/losses/__init__.py
--rw-r--r--   0        0        0    10857 2024-03-28 15:53:13.581946 clipzyme-0.0.5/clipzyme/learning/losses/basic.py
--rw-r--r--   0        0        0    17891 2024-03-28 18:04:43.398133 clipzyme-0.0.5/clipzyme/learning/losses/contrastive.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.582586 clipzyme-0.0.5/clipzyme/learning/metrics/__init__.py
--rw-r--r--   0        0        0    20086 2024-03-28 15:53:13.582961 clipzyme-0.0.5/clipzyme/learning/metrics/basic.py
--rw-r--r--   0        0        0     6590 2024-03-28 15:53:13.583284 clipzyme-0.0.5/clipzyme/learning/metrics/representation.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.583361 clipzyme-0.0.5/clipzyme/learning/optimizers/__init__.py
--rw-r--r--   0        0        0     2406 2024-03-28 15:53:13.583673 clipzyme-0.0.5/clipzyme/learning/optimizers/basic.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.583744 clipzyme-0.0.5/clipzyme/learning/schedulers/__init__.py
--rw-r--r--   0        0        0     1855 2024-03-28 15:53:13.583927 clipzyme-0.0.5/clipzyme/learning/schedulers/basic.py
--rw-r--r--   0        0        0     6835 2024-03-28 18:04:43.397866 clipzyme-0.0.5/clipzyme/learning/schedulers/warmup.py
--rw-r--r--   0        0        0      122 2024-03-28 15:53:13.584578 clipzyme-0.0.5/clipzyme/learning/utils.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.584651 clipzyme-0.0.5/clipzyme/lightning/__init__.py
--rw-r--r--   0        0        0    21181 2024-03-28 15:53:13.584896 clipzyme-0.0.5/clipzyme/lightning/base.py
--rw-r--r--   0        0        0    12584 2024-04-08 17:02:34.466944 clipzyme-0.0.5/clipzyme/lightning/clipzyme.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.585018 clipzyme-0.0.5/clipzyme/loggers/__init__.py
--rw-r--r--   0        0        0      637 2024-03-28 15:53:13.585360 clipzyme-0.0.5/clipzyme/loggers/tensorboard.py
--rw-r--r--   0        0        0     2254 2024-03-28 15:53:13.585569 clipzyme-0.0.5/clipzyme/loggers/wandb.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.585646 clipzyme-0.0.5/clipzyme/models/__init__.py
--rw-r--r--   0        0        0      300 2024-03-28 15:53:13.585810 clipzyme-0.0.5/clipzyme/models/abstract.py
--rw-r--r--   0        0        0     7144 2024-03-28 15:53:13.585987 clipzyme-0.0.5/clipzyme/models/chemprop.py
--rw-r--r--   0        0        0     7285 2024-03-28 15:53:13.586155 clipzyme-0.0.5/clipzyme/models/classifier.py
--rw-r--r--   0        0        0    29102 2024-03-28 15:53:13.586482 clipzyme-0.0.5/clipzyme/models/egnn.py
--rw-r--r--   0        0        0     6917 2024-03-28 15:53:13.586943 clipzyme-0.0.5/clipzyme/models/fair_esm.py
--rw-r--r--   0        0        0    10220 2024-03-28 15:53:13.587252 clipzyme-0.0.5/clipzyme/models/gat.py
--rw-r--r--   0        0        0    28859 2024-03-29 19:38:31.847201 clipzyme-0.0.5/clipzyme/models/protmol.py
--rw-r--r--   0        0        0     5331 2024-03-28 15:53:13.588426 clipzyme-0.0.5/clipzyme/models/seq2seq.py
--rw-r--r--   0        0        0    24182 2024-03-28 15:53:13.588821 clipzyme-0.0.5/clipzyme/models/wln.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.588932 clipzyme-0.0.5/clipzyme/utils/__init__.py
--rw-r--r--   0        0        0     1891 2024-03-28 15:53:13.589041 clipzyme-0.0.5/clipzyme/utils/amino_acids.py
--rw-r--r--   0        0        0     1679 2024-03-28 15:53:13.589238 clipzyme-0.0.5/clipzyme/utils/callbacks.py
--rw-r--r--   0        0        0     3669 2024-03-28 15:53:13.589424 clipzyme-0.0.5/clipzyme/utils/classes.py
--rw-r--r--   0        0        0     8793 2024-03-28 18:04:43.397858 clipzyme-0.0.5/clipzyme/utils/colabfold_msa.py
--rw-r--r--   0        0        0    11554 2024-03-28 15:53:13.589737 clipzyme-0.0.5/clipzyme/utils/loading.py
--rw-r--r--   0        0        0      154 2024-03-28 15:53:13.589922 clipzyme-0.0.5/clipzyme/utils/messages.py
--rw-r--r--   0        0        0    22189 2024-03-28 15:53:13.590443 clipzyme-0.0.5/clipzyme/utils/parsing.py
--rw-r--r--   0        0        0    13604 2024-04-08 17:00:53.080799 clipzyme-0.0.5/clipzyme/utils/protein_utils.py
--rw-r--r--   0        0        0    15629 2024-03-28 18:04:43.398175 clipzyme-0.0.5/clipzyme/utils/proteins.py
--rw-r--r--   0        0        0    13289 2024-03-28 15:53:13.591225 clipzyme-0.0.5/clipzyme/utils/pyg.py
--rw-r--r--   0        0        0    17957 2024-03-28 18:04:43.399109 clipzyme-0.0.5/clipzyme/utils/reactions.py
--rw-r--r--   0        0        0     1187 2024-03-28 15:53:13.591465 clipzyme-0.0.5/clipzyme/utils/registry.py
--rw-r--r--   0        0        0     4638 2024-03-28 15:53:13.591739 clipzyme-0.0.5/clipzyme/utils/sampler.py
--rw-r--r--   0        0        0     4897 2024-04-08 16:56:54.314023 clipzyme-0.0.5/clipzyme/utils/screening.py
--rw-r--r--   0        0        0    22325 2024-03-28 15:53:13.591875 clipzyme-0.0.5/clipzyme/utils/smiles.py
--rw-r--r--   0        0        0    48101 2024-03-28 18:04:43.399645 clipzyme-0.0.5/clipzyme/utils/wln_processing.py
--rw-r--r--   0        0        0      623 2024-04-08 17:03:00.807007 clipzyme-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8219 1970-01-01 00:00:00.000000 clipzyme-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-28 18:26:04.343837 clipzyme-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     7976 2024-05-10 20:57:34.422852 clipzyme-0.0.6/README.md
+-rw-r--r--   0        0        0     1788 2024-03-29 19:24:34.636971 clipzyme-0.0.6/clipzyme/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.578850 clipzyme-0.0.6/clipzyme/callbacks/__init__.py
+-rw-r--r--   0        0        0      948 2024-03-28 15:53:13.579321 clipzyme-0.0.6/clipzyme/callbacks/basic.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.579397 clipzyme-0.0.6/clipzyme/datasets/__init__.py
+-rw-r--r--   0        0        0     8552 2024-03-28 15:53:13.579934 clipzyme-0.0.6/clipzyme/datasets/abstract.py
+-rw-r--r--   0        0        0    12769 2024-03-28 15:53:13.580656 clipzyme-0.0.6/clipzyme/datasets/enzyme_screening.py
+-rw-r--r--   0        0        0    43705 2024-04-08 16:54:12.470132 clipzyme-0.0.6/clipzyme/datasets/enzymemap.py
+-rw-r--r--   0        0        0    11816 2024-04-08 02:52:05.338533 clipzyme-0.0.6/clipzyme/datasets/reaction.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.581466 clipzyme-0.0.6/clipzyme/learning/losses/__init__.py
+-rw-r--r--   0        0        0    10857 2024-03-28 15:53:13.581946 clipzyme-0.0.6/clipzyme/learning/losses/basic.py
+-rw-r--r--   0        0        0    17891 2024-03-28 18:04:43.398133 clipzyme-0.0.6/clipzyme/learning/losses/contrastive.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.582586 clipzyme-0.0.6/clipzyme/learning/metrics/__init__.py
+-rw-r--r--   0        0        0    20086 2024-03-28 15:53:13.582961 clipzyme-0.0.6/clipzyme/learning/metrics/basic.py
+-rw-r--r--   0        0        0     6590 2024-03-28 15:53:13.583284 clipzyme-0.0.6/clipzyme/learning/metrics/representation.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.583361 clipzyme-0.0.6/clipzyme/learning/optimizers/__init__.py
+-rw-r--r--   0        0        0     2406 2024-03-28 15:53:13.583673 clipzyme-0.0.6/clipzyme/learning/optimizers/basic.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.583744 clipzyme-0.0.6/clipzyme/learning/schedulers/__init__.py
+-rw-r--r--   0        0        0     1855 2024-03-28 15:53:13.583927 clipzyme-0.0.6/clipzyme/learning/schedulers/basic.py
+-rw-r--r--   0        0        0     6835 2024-03-28 18:04:43.397866 clipzyme-0.0.6/clipzyme/learning/schedulers/warmup.py
+-rw-r--r--   0        0        0      122 2024-03-28 15:53:13.584578 clipzyme-0.0.6/clipzyme/learning/utils.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.584651 clipzyme-0.0.6/clipzyme/lightning/__init__.py
+-rw-r--r--   0        0        0    21181 2024-03-28 15:53:13.584896 clipzyme-0.0.6/clipzyme/lightning/base.py
+-rw-r--r--   0        0        0    12789 2024-05-10 20:56:23.614929 clipzyme-0.0.6/clipzyme/lightning/clipzyme.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.585018 clipzyme-0.0.6/clipzyme/loggers/__init__.py
+-rw-r--r--   0        0        0      637 2024-03-28 15:53:13.585360 clipzyme-0.0.6/clipzyme/loggers/tensorboard.py
+-rw-r--r--   0        0        0     2254 2024-03-28 15:53:13.585569 clipzyme-0.0.6/clipzyme/loggers/wandb.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.585646 clipzyme-0.0.6/clipzyme/models/__init__.py
+-rw-r--r--   0        0        0      300 2024-03-28 15:53:13.585810 clipzyme-0.0.6/clipzyme/models/abstract.py
+-rw-r--r--   0        0        0     7144 2024-03-28 15:53:13.585987 clipzyme-0.0.6/clipzyme/models/chemprop.py
+-rw-r--r--   0        0        0     7285 2024-03-28 15:53:13.586155 clipzyme-0.0.6/clipzyme/models/classifier.py
+-rw-r--r--   0        0        0    29102 2024-03-28 15:53:13.586482 clipzyme-0.0.6/clipzyme/models/egnn.py
+-rw-r--r--   0        0        0     6917 2024-03-28 15:53:13.586943 clipzyme-0.0.6/clipzyme/models/fair_esm.py
+-rw-r--r--   0        0        0    10220 2024-03-28 15:53:13.587252 clipzyme-0.0.6/clipzyme/models/gat.py
+-rw-r--r--   0        0        0    28859 2024-03-29 19:38:31.847201 clipzyme-0.0.6/clipzyme/models/protmol.py
+-rw-r--r--   0        0        0     5331 2024-03-28 15:53:13.588426 clipzyme-0.0.6/clipzyme/models/seq2seq.py
+-rw-r--r--   0        0        0    24182 2024-03-28 15:53:13.588821 clipzyme-0.0.6/clipzyme/models/wln.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.588932 clipzyme-0.0.6/clipzyme/utils/__init__.py
+-rw-r--r--   0        0        0     1891 2024-03-28 15:53:13.589041 clipzyme-0.0.6/clipzyme/utils/amino_acids.py
+-rw-r--r--   0        0        0     1679 2024-03-28 15:53:13.589238 clipzyme-0.0.6/clipzyme/utils/callbacks.py
+-rw-r--r--   0        0        0     3669 2024-03-28 15:53:13.589424 clipzyme-0.0.6/clipzyme/utils/classes.py
+-rw-r--r--   0        0        0     8793 2024-03-28 18:04:43.397858 clipzyme-0.0.6/clipzyme/utils/colabfold_msa.py
+-rw-r--r--   0        0        0    11554 2024-03-28 15:53:13.589737 clipzyme-0.0.6/clipzyme/utils/loading.py
+-rw-r--r--   0        0        0      154 2024-03-28 15:53:13.589922 clipzyme-0.0.6/clipzyme/utils/messages.py
+-rw-r--r--   0        0        0    22189 2024-03-28 15:53:13.590443 clipzyme-0.0.6/clipzyme/utils/parsing.py
+-rw-r--r--   0        0        0    13604 2024-04-08 17:00:53.080799 clipzyme-0.0.6/clipzyme/utils/protein_utils.py
+-rw-r--r--   0        0        0    15629 2024-03-28 18:04:43.398175 clipzyme-0.0.6/clipzyme/utils/proteins.py
+-rw-r--r--   0        0        0    13289 2024-03-28 15:53:13.591225 clipzyme-0.0.6/clipzyme/utils/pyg.py
+-rw-r--r--   0        0        0    17957 2024-03-28 18:04:43.399109 clipzyme-0.0.6/clipzyme/utils/reactions.py
+-rw-r--r--   0        0        0     1187 2024-03-28 15:53:13.591465 clipzyme-0.0.6/clipzyme/utils/registry.py
+-rw-r--r--   0        0        0     4638 2024-03-28 15:53:13.591739 clipzyme-0.0.6/clipzyme/utils/sampler.py
+-rw-r--r--   0        0        0     4897 2024-04-08 16:56:54.314023 clipzyme-0.0.6/clipzyme/utils/screening.py
+-rw-r--r--   0        0        0    22325 2024-03-28 15:53:13.591875 clipzyme-0.0.6/clipzyme/utils/smiles.py
+-rw-r--r--   0        0        0    48101 2024-03-28 18:04:43.399645 clipzyme-0.0.6/clipzyme/utils/wln_processing.py
+-rw-r--r--   0        0        0      623 2024-05-10 20:58:54.523385 clipzyme-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8501 1970-01-01 00:00:00.000000 clipzyme-0.0.6/PKG-INFO
```

### Comparing `clipzyme-0.0.5/LICENSE.txt` & `clipzyme-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/README.md` & `clipzyme-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: clipzyme
+Version: 0.0.6
+Summary: Reaction-Conditioned Virtual Screening of Enzymes
+Home-page: https://github.com/pgmikhael/clipzyme
+License: Apache 2.0
+Author: Peter G Mikhael
+Author-email: pgmikhael@csail.mit.edu
+Requires-Python: >=3.10,<3.11
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Project-URL: Repository, https://github.com/pgmikhael/clipzyme
+Description-Content-Type: text/markdown
+
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/pgmikhael/CLIPZyme/blob/main/LICENSE.txt) 
 [![arXiv](https://img.shields.io/badge/arXiv-1234.56789-b31b1b.svg)](https://arxiv.org/abs/2402.06748)
 <!-- ![version](https://img.shields.io/badge/version-1.0.2-success) -->
 
 # CLIPZyme
 
 Implementation of the paper [**CLIPZyme: Reaction-Conditioned Virtual Screening of Enzymes**](https://github.com/pgmikhael/CLIPZyme/blob/main/LICENSE.txt)
@@ -9,14 +24,15 @@
 
 
 Table of contents
 =================
 
 <!--ts-->
    * [Installation](#installation)
+   * [Checkpoints and Data Files](#checkpoints-and-data-files)
    * [Screening with CLIPZyme](#screening-with-clipzyme)
         * [Using CLIPZyme's screening set](#using-clipzyme's-screening-set)
         * [Using your own screening set](#using-your-own-screening-set)
             * [Interactive (slow)](#interactive-slow)
             * [Batched (fast)](#batched-fast)
    * [Reproducing published results](#reproducing-published-results)
         * [Data processing](#data-processing)
@@ -34,26 +50,36 @@
 2. Install the dependencies:
 ```bash
 conda create env -f environment.yml
 pip install clipzyme
 ```
 
 3. Download ESM-2 checkpoint `esm2_t33_650M_UR50D`. The `esm_dir` argument should point to this directory.
-# Screening with CLIPZyme
 
-## Using CLIPZyme's screening set
+# Checkpoints and Data Files:
 
-1. Download the screening set and extract the files into `files/`.
+The model checkpoint and data are available on Zenodo [here](https://zenodo.org/records/10950376):
 
-```bash
+- [clipzyme_data.zip](https://zenodo.org/records/10950376/files/clipzyme_data.zip?download=1):
+  - `enzymemap.json`: contains the EnzymeMap dataset.
+  - `cached_enzymemap.p`: contains the processed EnzymeMap dataset.
+  - `clipzyme_screening_set.p`: contains the screening set as dict of UniProt IDs and precomputed protein embeddings.
+  - `uniprot2sequence.p`: contains the mapping form sequence ID to amino acids.
 
-wget https://github.com/pgmikhael/clipzyme/releases/download/v1.0.0/clipzyme_screening_set.zip
+- [clipzyme_model.zip](https://zenodo.org/records/10950376/files/clipzyme_model.zip?download=1):
+  - `clipzyme_model.ckpt`: the trained model checkpoint.
+
+
+
+# Screening with CLIPZyme
+
+## Using CLIPZyme's screening set
+
+First, download the screening set and extract the files into `files/`.
 
-unzip clipzyme_screening_set.zip -d files/
-```
 
 ```python
 import pickle
 from clipzyme import CLIPZyme
 
 ## Load the screening set
 ##-----------------------
@@ -164,19 +190,15 @@
 
 ## Data processing
 
 We obtain the data from the following sources:
 - [EnzymeMap:](`https://doi.org/10.5281/zenodo.7841780`) Heid et al. Enzymemap: Curation, validation and data-driven prediction of enzymatic reactions. 2023.
 - [Terpene Synthases:](`https://zenodo.org/records/10567437`) Samusevich et al. Discovery and characterization of terpene synthases powered by machine learning. 2024. 
 
-Our processed data is available at [here](`https://doi.org/10.5281/zenodo.5555555`). It consists of the following files:
-- `enzymemap.json`: contains the EnzymeMap dataset.
-- `terpene_synthases.json`: contains the Terpene Synthases dataset.
-- `clipzyme_screening_set.p`: contains the screening set as dict of UniProt IDs and precomputed protein embeddings.
-- `uniprot2sequence.p`: contains the mapping form sequence ID to amino acids.
+Our processed data is can be downloaded from [here](https://zenodo.org/records/10950376). 
 
 
 ## Training and evaluation
 1. To train the models presented in the tables below, run the following command:
     ```
     python scripts/dispatcher.py -c {config_path} -l {log_path}
     ```
@@ -192,15 +214,16 @@
     python scripts/dispatcher.py -c configs/eval/clip_egnn.json -l ./logs/
     ```
 3. We perform all analysis in the jupyter notebook included [Results.ipynb](analysis/Results.ipynb). We first calculate the hidden representations of the screening using the eval configs above and collect them into one matrix (saved as a pickle file). These are loaded into the jupyter notebook as well as the test set. All tables are then generated in the notebook.
 
 
 ## Citation
 
-```
+```bibtex
 @article{mikhael2024clipzyme,
   title={CLIPZyme: Reaction-Conditioned Virtual Screening of Enzymes},
   author={Mikhael, Peter G and Chinn, Itamar and Barzilay, Regina},
   journal={arXiv preprint arXiv:2402.06748},
   year={2024}
 }
 ```
+
```

### Comparing `clipzyme-0.0.5/clipzyme/__init__.py` & `clipzyme-0.0.6/clipzyme/__init__.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/callbacks/basic.py` & `clipzyme-0.0.6/clipzyme/callbacks/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/datasets/abstract.py` & `clipzyme-0.0.6/clipzyme/datasets/abstract.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/datasets/enzyme_screening.py` & `clipzyme-0.0.6/clipzyme/datasets/enzyme_screening.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/datasets/enzymemap.py` & `clipzyme-0.0.6/clipzyme/datasets/enzymemap.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/datasets/reaction.py` & `clipzyme-0.0.6/clipzyme/datasets/reaction.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/learning/losses/basic.py` & `clipzyme-0.0.6/clipzyme/learning/losses/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/learning/losses/contrastive.py` & `clipzyme-0.0.6/clipzyme/learning/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/learning/metrics/basic.py` & `clipzyme-0.0.6/clipzyme/learning/metrics/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/learning/metrics/representation.py` & `clipzyme-0.0.6/clipzyme/learning/metrics/representation.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/learning/optimizers/basic.py` & `clipzyme-0.0.6/clipzyme/learning/optimizers/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/learning/schedulers/basic.py` & `clipzyme-0.0.6/clipzyme/learning/schedulers/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/learning/schedulers/warmup.py` & `clipzyme-0.0.6/clipzyme/learning/schedulers/warmup.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/lightning/base.py` & `clipzyme-0.0.6/clipzyme/lightning/base.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/lightning/clipzyme.py` & `clipzyme-0.0.6/clipzyme/lightning/clipzyme.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 from typing import Optional, List, NamedTuple, Union
-from io import BytesIO
+import wget
 import shutil
-from zipfile import ZipFile
-from urllib.request import urlopen
 from pathlib import Path
 import os
+import subprocess
 import torch
 from rich import print
 import pytorch_lightning as pl
 import argparse
 from clipzyme.models.protmol import EnzymeReactionCLIP
 from clipzyme.utils.screening import process_mapped_reaction
 from clipzyme.utils.protein_utils import create_protein_graph
 from clipzyme.utils.loading import default_collate
 
-CHECKPOINT_URL = "https://github.com/pgmikhael/clipzyme/releases/download/v0.0.5/clipzyme_files.zip"  # TODO: Update this
+CHECKPOINT_URL = "https://zenodo.org/records/10950376/files/clipzyme_model.zip"
 
 
-def download_and_extract(remote_model_url: str, local_model_dir) -> List[str]:
-    resp = urlopen(remote_model_url)
-    os.makedirs(local_model_dir, exist_ok=True)
-    with ZipFile(BytesIO(resp.read())) as zip_file:
-        all_files_and_dirs = zip_file.namelist()
-        zip_file.extractall(local_model_dir)
-    assert len(all_files_and_dirs) == 1, "Expected only one file in the zip"
+def download_and_extract(remote_model_url: str, local_model_dir: str) -> str:
+    """
+    Download and extract model.
+
+    Parameters
+    ----------
+    remote_model_url : str
+        link to model file
+    local_model_dir : str
+        local directory to save model
+
+    Returns
+    -------
+    str
+        name of model file
+    """
+    zipfile = wget.download(remote_model_url, out=local_model_dir)
+    # unzip
+    subprocess.call(f"unzip {zipfile} -d {local_model_dir}", shell=True)
+    # remove zip
+    os.remove(zipfile)
+    # get all files and dirs
+    all_files_and_dirs = os.listdir(local_model_dir)
+    assert len(all_files_and_dirs) == 1, "More than one file in model directory"
     return all_files_and_dirs[0]
 
 
 def download_model(checkpoint_path) -> str:
     """
     Download trained clipzyme model.
```

### Comparing `clipzyme-0.0.5/clipzyme/loggers/tensorboard.py` & `clipzyme-0.0.6/clipzyme/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/loggers/wandb.py` & `clipzyme-0.0.6/clipzyme/loggers/wandb.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/models/chemprop.py` & `clipzyme-0.0.6/clipzyme/models/chemprop.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/models/classifier.py` & `clipzyme-0.0.6/clipzyme/models/classifier.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/models/egnn.py` & `clipzyme-0.0.6/clipzyme/models/egnn.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/models/fair_esm.py` & `clipzyme-0.0.6/clipzyme/models/fair_esm.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/models/gat.py` & `clipzyme-0.0.6/clipzyme/models/gat.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/models/protmol.py` & `clipzyme-0.0.6/clipzyme/models/protmol.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/models/seq2seq.py` & `clipzyme-0.0.6/clipzyme/models/seq2seq.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/models/wln.py` & `clipzyme-0.0.6/clipzyme/models/wln.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/amino_acids.py` & `clipzyme-0.0.6/clipzyme/utils/amino_acids.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/callbacks.py` & `clipzyme-0.0.6/clipzyme/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/classes.py` & `clipzyme-0.0.6/clipzyme/utils/classes.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/colabfold_msa.py` & `clipzyme-0.0.6/clipzyme/utils/colabfold_msa.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/loading.py` & `clipzyme-0.0.6/clipzyme/utils/loading.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/parsing.py` & `clipzyme-0.0.6/clipzyme/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/protein_utils.py` & `clipzyme-0.0.6/clipzyme/utils/protein_utils.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/proteins.py` & `clipzyme-0.0.6/clipzyme/utils/proteins.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/pyg.py` & `clipzyme-0.0.6/clipzyme/utils/pyg.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/reactions.py` & `clipzyme-0.0.6/clipzyme/utils/reactions.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/registry.py` & `clipzyme-0.0.6/clipzyme/utils/registry.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/sampler.py` & `clipzyme-0.0.6/clipzyme/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/screening.py` & `clipzyme-0.0.6/clipzyme/utils/screening.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/smiles.py` & `clipzyme-0.0.6/clipzyme/utils/smiles.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/clipzyme/utils/wln_processing.py` & `clipzyme-0.0.6/clipzyme/utils/wln_processing.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.5/pyproject.toml` & `clipzyme-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clipzyme"
-version = "0.0.5"
+version = "0.0.6"
 description = "Reaction-Conditioned Virtual Screening of Enzymes"
 authors = ["Peter G Mikhael <pgmikhael@csail.mit.edu>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/pgmikhael/clipzyme"
```

### Comparing `clipzyme-0.0.5/PKG-INFO` & `clipzyme-0.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: clipzyme
-Version: 0.0.5
-Summary: Reaction-Conditioned Virtual Screening of Enzymes
-Home-page: https://github.com/pgmikhael/clipzyme
-License: Apache 2.0
-Author: Peter G Mikhael
-Author-email: pgmikhael@csail.mit.edu
-Requires-Python: >=3.10,<3.11
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Project-URL: Repository, https://github.com/pgmikhael/clipzyme
-Description-Content-Type: text/markdown
-
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/pgmikhael/CLIPZyme/blob/main/LICENSE.txt) 
 [![arXiv](https://img.shields.io/badge/arXiv-1234.56789-b31b1b.svg)](https://arxiv.org/abs/2402.06748)
 <!-- ![version](https://img.shields.io/badge/version-1.0.2-success) -->
 
 # CLIPZyme
 
 Implementation of the paper [**CLIPZyme: Reaction-Conditioned Virtual Screening of Enzymes**](https://github.com/pgmikhael/CLIPZyme/blob/main/LICENSE.txt)
@@ -24,14 +9,15 @@
 
 
 Table of contents
 =================
 
 <!--ts-->
    * [Installation](#installation)
+   * [Checkpoints and Data Files](#checkpoints-and-data-files)
    * [Screening with CLIPZyme](#screening-with-clipzyme)
         * [Using CLIPZyme's screening set](#using-clipzyme's-screening-set)
         * [Using your own screening set](#using-your-own-screening-set)
             * [Interactive (slow)](#interactive-slow)
             * [Batched (fast)](#batched-fast)
    * [Reproducing published results](#reproducing-published-results)
         * [Data processing](#data-processing)
@@ -49,26 +35,36 @@
 2. Install the dependencies:
 ```bash
 conda create env -f environment.yml
 pip install clipzyme
 ```
 
 3. Download ESM-2 checkpoint `esm2_t33_650M_UR50D`. The `esm_dir` argument should point to this directory.
-# Screening with CLIPZyme
 
-## Using CLIPZyme's screening set
+# Checkpoints and Data Files:
 
-1. Download the screening set and extract the files into `files/`.
+The model checkpoint and data are available on Zenodo [here](https://zenodo.org/records/10950376):
 
-```bash
+- [clipzyme_data.zip](https://zenodo.org/records/10950376/files/clipzyme_data.zip?download=1):
+  - `enzymemap.json`: contains the EnzymeMap dataset.
+  - `cached_enzymemap.p`: contains the processed EnzymeMap dataset.
+  - `clipzyme_screening_set.p`: contains the screening set as dict of UniProt IDs and precomputed protein embeddings.
+  - `uniprot2sequence.p`: contains the mapping form sequence ID to amino acids.
 
-wget https://github.com/pgmikhael/clipzyme/releases/download/v1.0.0/clipzyme_screening_set.zip
+- [clipzyme_model.zip](https://zenodo.org/records/10950376/files/clipzyme_model.zip?download=1):
+  - `clipzyme_model.ckpt`: the trained model checkpoint.
+
+
+
+# Screening with CLIPZyme
+
+## Using CLIPZyme's screening set
+
+First, download the screening set and extract the files into `files/`.
 
-unzip clipzyme_screening_set.zip -d files/
-```
 
 ```python
 import pickle
 from clipzyme import CLIPZyme
 
 ## Load the screening set
 ##-----------------------
@@ -179,19 +175,15 @@
 
 ## Data processing
 
 We obtain the data from the following sources:
 - [EnzymeMap:](`https://doi.org/10.5281/zenodo.7841780`) Heid et al. Enzymemap: Curation, validation and data-driven prediction of enzymatic reactions. 2023.
 - [Terpene Synthases:](`https://zenodo.org/records/10567437`) Samusevich et al. Discovery and characterization of terpene synthases powered by machine learning. 2024. 
 
-Our processed data is available at [here](`https://doi.org/10.5281/zenodo.5555555`). It consists of the following files:
-- `enzymemap.json`: contains the EnzymeMap dataset.
-- `terpene_synthases.json`: contains the Terpene Synthases dataset.
-- `clipzyme_screening_set.p`: contains the screening set as dict of UniProt IDs and precomputed protein embeddings.
-- `uniprot2sequence.p`: contains the mapping form sequence ID to amino acids.
+Our processed data is can be downloaded from [here](https://zenodo.org/records/10950376). 
 
 
 ## Training and evaluation
 1. To train the models presented in the tables below, run the following command:
     ```
     python scripts/dispatcher.py -c {config_path} -l {log_path}
     ```
@@ -207,16 +199,15 @@
     python scripts/dispatcher.py -c configs/eval/clip_egnn.json -l ./logs/
     ```
 3. We perform all analysis in the jupyter notebook included [Results.ipynb](analysis/Results.ipynb). We first calculate the hidden representations of the screening using the eval configs above and collect them into one matrix (saved as a pickle file). These are loaded into the jupyter notebook as well as the test set. All tables are then generated in the notebook.
 
 
 ## Citation
 
-```
+```bibtex
 @article{mikhael2024clipzyme,
   title={CLIPZyme: Reaction-Conditioned Virtual Screening of Enzymes},
   author={Mikhael, Peter G and Chinn, Itamar and Barzilay, Regina},
   journal={arXiv preprint arXiv:2402.06748},
   year={2024}
 }
 ```
-
```

