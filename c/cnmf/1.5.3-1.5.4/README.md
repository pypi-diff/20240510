# Comparing `tmp/cnmf-1.5.3.tar.gz` & `tmp/cnmf-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmf-1.5.3.tar", last modified: Wed May  8 03:56:07 2024, max compression
+gzip compressed data, was "cnmf-1.5.4.tar", last modified: Fri May 10 00:22:29 2024, max compression
```

## Comparing `cnmf-1.5.3.tar` & `cnmf-1.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 03:56:07.235247 cnmf-1.5.3/
--rw-r--r--   0 dkotliar   (503) staff       (20)     1070 2024-05-08 02:54:21.000000 cnmf-1.5.3/LICENSE
--rw-r--r--   0 dkotliar   (503) staff       (20)     9537 2024-05-08 03:56:07.234568 cnmf-1.5.3/PKG-INFO
--rw-r--r--   0 dkotliar   (503) staff       (20)     8831 2024-05-08 03:45:02.000000 cnmf-1.5.3/README.md
--rw-r--r--   0 dkotliar   (503) staff       (20)      103 2024-05-08 02:54:21.000000 cnmf-1.5.3/pyproject.toml
--rw-r--r--   0 dkotliar   (503) staff       (20)       38 2024-05-08 03:56:07.235472 cnmf-1.5.3/setup.cfg
--rw-r--r--   0 dkotliar   (503) staff       (20)     1333 2024-05-08 02:54:21.000000 cnmf-1.5.3/setup.py
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 03:56:07.226005 cnmf-1.5.3/src/
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 03:56:07.230565 cnmf-1.5.3/src/cnmf/
--rw-r--r--   0 dkotliar   (503) staff       (20)      131 2024-05-08 02:54:21.000000 cnmf-1.5.3/src/cnmf/__init__.py
--rwxr-xr-x   0 dkotliar   (503) staff       (20)    53213 2024-05-08 03:52:51.000000 cnmf-1.5.3/src/cnmf/cnmf.py
--rw-r--r--   0 dkotliar   (503) staff       (20)    20172 2024-05-08 02:54:21.000000 cnmf-1.5.3/src/cnmf/preprocess.py
--rw-r--r--   0 dkotliar   (503) staff       (20)       22 2024-05-08 03:55:26.000000 cnmf-1.5.3/src/cnmf/version.py
-drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-08 03:56:07.233890 cnmf-1.5.3/src/cnmf.egg-info/
--rw-r--r--   0 dkotliar   (503) staff       (20)     9537 2024-05-08 03:56:07.000000 cnmf-1.5.3/src/cnmf.egg-info/PKG-INFO
--rw-r--r--   0 dkotliar   (503) staff       (20)      316 2024-05-08 03:56:07.000000 cnmf-1.5.3/src/cnmf.egg-info/SOURCES.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)        1 2024-05-08 03:56:07.000000 cnmf-1.5.3/src/cnmf.egg-info/dependency_links.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)       35 2024-05-08 03:56:07.000000 cnmf-1.5.3/src/cnmf.egg-info/entry_points.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)       98 2024-05-08 03:56:07.000000 cnmf-1.5.3/src/cnmf.egg-info/requires.txt
--rw-r--r--   0 dkotliar   (503) staff       (20)        5 2024-05-08 03:56:07.000000 cnmf-1.5.3/src/cnmf.egg-info/top_level.txt
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-10 00:22:29.189706 cnmf-1.5.4/
+-rw-r--r--   0 dkotliar   (503) staff       (20)     1070 2024-05-10 00:18:00.000000 cnmf-1.5.4/LICENSE
+-rw-r--r--   0 dkotliar   (503) staff       (20)     9707 2024-05-10 00:22:29.189024 cnmf-1.5.4/PKG-INFO
+-rw-r--r--   0 dkotliar   (503) staff       (20)     9001 2024-05-10 00:18:00.000000 cnmf-1.5.4/README.md
+-rw-r--r--   0 dkotliar   (503) staff       (20)      103 2024-05-10 00:18:00.000000 cnmf-1.5.4/pyproject.toml
+-rw-r--r--   0 dkotliar   (503) staff       (20)       38 2024-05-10 00:22:29.189842 cnmf-1.5.4/setup.cfg
+-rw-r--r--   0 dkotliar   (503) staff       (20)     1333 2024-05-10 00:18:00.000000 cnmf-1.5.4/setup.py
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-10 00:22:29.178619 cnmf-1.5.4/src/
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-10 00:22:29.184475 cnmf-1.5.4/src/cnmf/
+-rw-r--r--   0 dkotliar   (503) staff       (20)      131 2024-05-10 00:18:00.000000 cnmf-1.5.4/src/cnmf/__init__.py
+-rwxr-xr-x   0 dkotliar   (503) staff       (20)    53213 2024-05-10 00:18:00.000000 cnmf-1.5.4/src/cnmf/cnmf.py
+-rw-r--r--   0 dkotliar   (503) staff       (20)    20207 2024-05-10 00:19:11.000000 cnmf-1.5.4/src/cnmf/preprocess.py
+-rw-r--r--   0 dkotliar   (503) staff       (20)       22 2024-05-10 00:21:20.000000 cnmf-1.5.4/src/cnmf/version.py
+drwxr-xr-x   0 dkotliar   (503) staff       (20)        0 2024-05-10 00:22:29.187997 cnmf-1.5.4/src/cnmf.egg-info/
+-rw-r--r--   0 dkotliar   (503) staff       (20)     9707 2024-05-10 00:22:29.000000 cnmf-1.5.4/src/cnmf.egg-info/PKG-INFO
+-rw-r--r--   0 dkotliar   (503) staff       (20)      316 2024-05-10 00:22:29.000000 cnmf-1.5.4/src/cnmf.egg-info/SOURCES.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)        1 2024-05-10 00:22:29.000000 cnmf-1.5.4/src/cnmf.egg-info/dependency_links.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)       35 2024-05-10 00:22:29.000000 cnmf-1.5.4/src/cnmf.egg-info/entry_points.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)       98 2024-05-10 00:22:29.000000 cnmf-1.5.4/src/cnmf.egg-info/requires.txt
+-rw-r--r--   0 dkotliar   (503) staff       (20)        5 2024-05-10 00:22:29.000000 cnmf-1.5.4/src/cnmf.egg-info/top_level.txt
```

### Comparing `cnmf-1.5.3/LICENSE` & `cnmf-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmf-1.5.3/PKG-INFO` & `cnmf-1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmf
-Version: 1.5.3
+Version: 1.5.4
 Summary: Consensus NMF for scRNA-Seq data
 Home-page: https://github.com/dylkot/cNMF
 Author: Dylan Kotliar
 Author-email: dylkot@gmail.com
 Project-URL: Bug Tracker, https://github.com/dylkot/cNMF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,16 @@
 
 # Consensus NMF (cNMF)
 
 <img src="https://storage.googleapis.com/sabeti-public/dkotliar/elife-cNMF-fig1.jpg" style="height: 800px;" />
 
 cNMF is a pipeline for inferring gene expression programs from scRNA-Seq. It takes a count matrix (N cells X G genes) as input and produces a (K x G) matrix of gene expression programs (GEPs) and a (N x K) matrix specifying the usage of each program for each cell in the data. Read more about the method in the [publication](https://elifesciences.org/articles/43803) and check out examples on [simulated data](Tutorials/analyze_simulated_example_data.ipynb) and [PBMCs](Tutorials/analyze_pbmc_example_data.ipynb).
 
+We have also created a tutorial for running cNMF from R. See the [Rmd notebook](Tutorials/R_vignette.Rmd) or the [compiled html](Tutorials/R_vignette.nb.html) for this.
+
 # Installation
 cNMF has been tested with Python 3.7 and 3.10 and requires scikit-learn>=1.0, scanpy>=1.8, and AnnData>=0.9
 
 You can install with [pip](https://pypi.org/):
 
 ```bash
 pip install cnmf
```

### Comparing `cnmf-1.5.3/README.md` & `cnmf-1.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Consensus NMF (cNMF)
 
 <img src="https://storage.googleapis.com/sabeti-public/dkotliar/elife-cNMF-fig1.jpg" style="height: 800px;" />
 
 cNMF is a pipeline for inferring gene expression programs from scRNA-Seq. It takes a count matrix (N cells X G genes) as input and produces a (K x G) matrix of gene expression programs (GEPs) and a (N x K) matrix specifying the usage of each program for each cell in the data. Read more about the method in the [publication](https://elifesciences.org/articles/43803) and check out examples on [simulated data](Tutorials/analyze_simulated_example_data.ipynb) and [PBMCs](Tutorials/analyze_pbmc_example_data.ipynb).
 
+We have also created a tutorial for running cNMF from R. See the [Rmd notebook](Tutorials/R_vignette.Rmd) or the [compiled html](Tutorials/R_vignette.nb.html) for this.
+
 # Installation
 cNMF has been tested with Python 3.7 and 3.10 and requires scikit-learn>=1.0, scanpy>=1.8, and AnnData>=0.9
 
 You can install with [pip](https://pypi.org/):
 
 ```bash
 pip install cnmf
```

### Comparing `cnmf-1.5.3/setup.py` & `cnmf-1.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `cnmf-1.5.3/src/cnmf/cnmf.py` & `cnmf-1.5.4/src/cnmf/cnmf.py`

 * *Files identical despite different names*

### Comparing `cnmf-1.5.3/src/cnmf/preprocess.py` & `cnmf-1.5.4/src/cnmf/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 
         tp10k = sc.pp.normalize_per_cell(adata_RNA, counts_per_cell_after=librarysize_targetsum, copy=True)
         adata_RNA, hvgs = self.normalize_batchcorrect(adata_RNA, harmony_vars=harmony_vars,
                                                 n_top_genes = n_top_rna_genes, 
                                                 librarysize_targetsum= librarysize_targetsum,
                                                 max_scaled_thresh = max_scaled_thresh,
                                                 quantile_thresh = quantile_thresh, theta=theta,
-                                                makeplots=makeplots)
+                                                makeplots=makeplots, max_iter_harmony=max_iter_harmony)
         
         if adata_ADT is not None:            
             adata_ADT = adata_ADT[adata_RNA.obs.index, :]
             sc.pp.normalize_per_cell(adata_ADT, counts_per_cell_after=librarysize_targetsum)
             
             merge_var = pd.concat([tp10k.var, adata_ADT.var], axis=0)            
             tp10k = sc.AnnData(hstack((tp10k.X, adata_ADT.X)), obs=tp10k.obs, var=merge_var)
```

### Comparing `cnmf-1.5.3/src/cnmf.egg-info/PKG-INFO` & `cnmf-1.5.4/src/cnmf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmf
-Version: 1.5.3
+Version: 1.5.4
 Summary: Consensus NMF for scRNA-Seq data
 Home-page: https://github.com/dylkot/cNMF
 Author: Dylan Kotliar
 Author-email: dylkot@gmail.com
 Project-URL: Bug Tracker, https://github.com/dylkot/cNMF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,16 @@
 
 # Consensus NMF (cNMF)
 
 <img src="https://storage.googleapis.com/sabeti-public/dkotliar/elife-cNMF-fig1.jpg" style="height: 800px;" />
 
 cNMF is a pipeline for inferring gene expression programs from scRNA-Seq. It takes a count matrix (N cells X G genes) as input and produces a (K x G) matrix of gene expression programs (GEPs) and a (N x K) matrix specifying the usage of each program for each cell in the data. Read more about the method in the [publication](https://elifesciences.org/articles/43803) and check out examples on [simulated data](Tutorials/analyze_simulated_example_data.ipynb) and [PBMCs](Tutorials/analyze_pbmc_example_data.ipynb).
 
+We have also created a tutorial for running cNMF from R. See the [Rmd notebook](Tutorials/R_vignette.Rmd) or the [compiled html](Tutorials/R_vignette.nb.html) for this.
+
 # Installation
 cNMF has been tested with Python 3.7 and 3.10 and requires scikit-learn>=1.0, scanpy>=1.8, and AnnData>=0.9
 
 You can install with [pip](https://pypi.org/):
 
 ```bash
 pip install cnmf
```

