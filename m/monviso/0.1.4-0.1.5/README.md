# Comparing `tmp/monviso-0.1.4.tar.gz` & `tmp/monviso-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/monviso-0.1.4.tar", last modified: Wed Apr 10 10:46:44 2024, max compression
+gzip compressed data, was "monviso-0.1.5.tar", last modified: Fri May 10 09:23:15 2024, max compression
```

## Comparing `monviso-0.1.4.tar` & `monviso-0.1.5.tar`

### file list

```diff
@@ -1,49 +1,53 @@
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-10 10:46:44.285040 monviso-0.1.4/
--rw-r--r--   0 albani     (502) staff       (20)     2173 2024-04-08 14:12:18.000000 monviso-0.1.4/Containerfile
--rw-r--r--   0 albani     (502) staff       (20)      648 2024-04-08 14:10:41.000000 monviso-0.1.4/HISTORY.md
--rw-r--r--   0 albani     (502) staff       (20)     1211 2024-02-28 10:12:03.000000 monviso-0.1.4/LICENSE
--rw-r--r--   0 albani     (502) staff       (20)       92 2024-02-28 10:12:03.000000 monviso-0.1.4/MANIFEST.in
--rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-10 10:46:44.278069 monviso-0.1.4/PKG-INFO
--rw-r--r--   0 albani     (502) staff       (20)     1302 2024-02-28 10:12:03.000000 monviso-0.1.4/README.md
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-10 10:46:44.213468 monviso-0.1.4/monviso.egg-info/
--rw-r--r--   0 albani     (502) staff       (20)     2260 2024-04-10 10:46:44.000000 monviso-0.1.4/monviso.egg-info/PKG-INFO
--rw-r--r--   0 albani     (502) staff       (20)     1433 2024-04-10 10:46:44.000000 monviso-0.1.4/monviso.egg-info/SOURCES.txt
--rw-r--r--   0 albani     (502) staff       (20)        1 2024-04-10 10:46:44.000000 monviso-0.1.4/monviso.egg-info/dependency_links.txt
--rw-r--r--   0 albani     (502) staff       (20)       69 2024-04-10 10:46:44.000000 monviso-0.1.4/monviso.egg-info/entry_points.txt
--rw-r--r--   0 albani     (502) staff       (20)      125 2024-04-10 10:46:44.000000 monviso-0.1.4/monviso.egg-info/requires.txt
--rw-r--r--   0 albani     (502) staff       (20)       17 2024-04-10 10:46:44.000000 monviso-0.1.4/monviso.egg-info/top_level.txt
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-10 10:46:44.232317 monviso-0.1.4/monviso_reloaded/
--rw-r--r--   0 albani     (502) staff       (20)     6906 2024-02-28 10:12:03.000000 monviso-0.1.4/monviso_reloaded/PDB_manager.py
--rw-r--r--   0 albani     (502) staff       (20)        6 2024-04-10 10:39:52.000000 monviso-0.1.4/monviso_reloaded/VERSION
--rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.4/monviso_reloaded/__init__.py
--rw-r--r--   0 albani     (502) staff       (20)      158 2024-02-28 10:12:03.000000 monviso-0.1.4/monviso_reloaded/__main__.py
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-10 10:46:44.264957 monviso-0.1.4/monviso_reloaded/__pycache__/
--rw-r--r--   0 albani     (502) staff       (20)     5885 2024-03-01 15:37:30.000000 monviso-0.1.4/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)      172 2024-03-01 15:27:07.000000 monviso-0.1.4/monviso_reloaded/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)      309 2024-03-01 15:27:07.000000 monviso-0.1.4/monviso_reloaded/__pycache__/__main__.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4774 2024-03-29 12:14:49.000000 monviso-0.1.4/monviso_reloaded/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)      873 2024-03-01 15:27:07.000000 monviso-0.1.4/monviso_reloaded/__pycache__/cli.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     1983 2024-03-01 15:37:30.000000 monviso-0.1.4/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:35:13.000000 monviso-0.1.4/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:31:42.000000 monviso-0.1.4/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     8605 2024-03-29 13:43:08.000000 monviso-0.1.4/monviso_reloaded/__pycache__/gene.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     6792 2024-03-01 15:46:41.000000 monviso-0.1.4/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)    16845 2024-03-29 09:02:50.000000 monviso-0.1.4/monviso_reloaded/__pycache__/isoform.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)    11396 2024-04-09 12:59:44.000000 monviso-0.1.4/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4678 2024-03-01 15:37:30.000000 monviso-0.1.4/monviso_reloaded/__pycache__/template.cpython-39.pyc
--rw-r--r--   0 albani     (502) staff       (20)     4378 2024-03-29 11:42:41.000000 monviso-0.1.4/monviso_reloaded/base.py
--rw-r--r--   0 albani     (502) staff       (20)      570 2024-02-28 10:12:03.000000 monviso-0.1.4/monviso_reloaded/cli.py
--rw-r--r--   0 albani     (502) staff       (20)     1739 2024-02-28 10:12:03.000000 monviso-0.1.4/monviso_reloaded/cobalt_wrapper.py
--rw-r--r--   0 albani     (502) staff       (20)     4013 2024-03-11 14:35:11.000000 monviso-0.1.4/monviso_reloaded/database_parser.py
--rw-r--r--   0 albani     (502) staff       (20)     4181 2024-03-11 14:31:34.000000 monviso-0.1.4/monviso_reloaded/file_handler.py
--rw-r--r--   0 albani     (502) staff       (20)    12827 2024-03-29 13:41:56.000000 monviso-0.1.4/monviso_reloaded/gene.py
--rw-r--r--   0 albani     (502) staff       (20)     8954 2024-03-01 15:46:37.000000 monviso-0.1.4/monviso_reloaded/input_parser.py
--rw-r--r--   0 albani     (502) staff       (20)    21299 2024-03-29 09:02:47.000000 monviso-0.1.4/monviso_reloaded/isoform.py
--rw-r--r--   0 albani     (502) staff       (20)    13278 2024-04-09 12:59:41.000000 monviso-0.1.4/monviso_reloaded/modeller_manager.py
--rw-r--r--   0 albani     (502) staff       (20)     5480 2024-02-28 10:12:03.000000 monviso-0.1.4/monviso_reloaded/template.py
--rw-r--r--   0 albani     (502) staff       (20)       38 2024-04-10 10:46:44.287119 monviso-0.1.4/setup.cfg
--rw-r--r--   0 albani     (502) staff       (20)     1567 2024-02-28 11:07:33.000000 monviso-0.1.4/setup.py
-drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-04-10 10:46:44.271430 monviso-0.1.4/tests/
--rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.4/tests/__init__.py
--rw-r--r--   0 albani     (502) staff       (20)      398 2024-02-28 10:12:03.000000 monviso-0.1.4/tests/conftest.py
--rw-r--r--   0 albani     (502) staff       (20)       96 2024-02-28 10:12:03.000000 monviso-0.1.4/tests/test_base.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-05-10 09:23:15.033574 monviso-0.1.5/
+-rw-r--r--   0 albani     (502) staff       (20)     2394 2024-05-10 09:20:41.000000 monviso-0.1.5/Containerfile
+-rw-r--r--   0 albani     (502) staff       (20)      995 2024-05-10 09:19:21.000000 monviso-0.1.5/HISTORY.md
+-rw-r--r--   0 albani     (502) staff       (20)     1211 2024-02-28 10:12:03.000000 monviso-0.1.5/LICENSE
+-rw-r--r--   0 albani     (502) staff       (20)       92 2024-02-28 10:12:03.000000 monviso-0.1.5/MANIFEST.in
+-rw-r--r--   0 albani     (502) staff       (20)     1887 2024-05-10 09:23:15.032968 monviso-0.1.5/PKG-INFO
+-rw-r--r--   0 albani     (502) staff       (20)     1323 2024-05-10 09:19:21.000000 monviso-0.1.5/README.md
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-05-10 09:23:14.982061 monviso-0.1.5/monviso.egg-info/
+-rw-r--r--   0 albani     (502) staff       (20)     1887 2024-05-10 09:23:14.000000 monviso-0.1.5/monviso.egg-info/PKG-INFO
+-rw-r--r--   0 albani     (502) staff       (20)     1628 2024-05-10 09:23:14.000000 monviso-0.1.5/monviso.egg-info/SOURCES.txt
+-rw-r--r--   0 albani     (502) staff       (20)        1 2024-05-10 09:23:14.000000 monviso-0.1.5/monviso.egg-info/dependency_links.txt
+-rw-r--r--   0 albani     (502) staff       (20)       60 2024-05-10 09:23:14.000000 monviso-0.1.5/monviso.egg-info/entry_points.txt
+-rw-r--r--   0 albani     (502) staff       (20)      208 2024-05-10 09:23:14.000000 monviso-0.1.5/monviso.egg-info/requires.txt
+-rw-r--r--   0 albani     (502) staff       (20)       17 2024-05-10 09:23:14.000000 monviso-0.1.5/monviso.egg-info/top_level.txt
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-05-10 09:23:14.999168 monviso-0.1.5/monviso_reloaded/
+-rw-r--r--   0 albani     (502) staff       (20)     7711 2024-05-10 09:19:21.000000 monviso-0.1.5/monviso_reloaded/PDB_manager.py
+-rw-r--r--   0 albani     (502) staff       (20)        6 2024-05-10 09:19:21.000000 monviso-0.1.5/monviso_reloaded/VERSION
+-rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.5/monviso_reloaded/__init__.py
+-rw-r--r--   0 albani     (502) staff       (20)      158 2024-02-28 10:12:03.000000 monviso-0.1.5/monviso_reloaded/__main__.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-05-10 09:23:15.028418 monviso-0.1.5/monviso_reloaded/__pycache__/
+-rw-r--r--   0 albani     (502) staff       (20)     5885 2024-03-01 15:37:30.000000 monviso-0.1.5/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      172 2024-03-01 15:27:07.000000 monviso-0.1.5/monviso_reloaded/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)      309 2024-03-01 15:27:07.000000 monviso-0.1.5/monviso_reloaded/__pycache__/__main__.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4434 2024-04-19 14:50:09.000000 monviso-0.1.5/monviso_reloaded/__pycache__/analyzer.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     5861 2024-04-19 14:50:08.000000 monviso-0.1.5/monviso_reloaded/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     1770 2024-05-08 15:27:11.000000 monviso-0.1.5/monviso_reloaded/__pycache__/cli.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     1983 2024-03-01 15:37:30.000000 monviso-0.1.5/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:35:13.000000 monviso-0.1.5/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4744 2024-03-11 14:31:42.000000 monviso-0.1.5/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     8605 2024-03-29 13:43:08.000000 monviso-0.1.5/monviso_reloaded/__pycache__/gene.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     7999 2024-04-16 15:01:10.000000 monviso-0.1.5/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     1830 2024-05-08 15:33:23.000000 monviso-0.1.5/monviso_reloaded/__pycache__/installer.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)    16845 2024-03-29 09:02:50.000000 monviso-0.1.5/monviso_reloaded/__pycache__/isoform.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)    11396 2024-04-09 12:59:44.000000 monviso-0.1.5/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     2658 2024-04-17 07:58:34.000000 monviso-0.1.5/monviso_reloaded/__pycache__/pesto_analyzer.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     4678 2024-03-01 15:37:30.000000 monviso-0.1.5/monviso_reloaded/__pycache__/template.cpython-39.pyc
+-rw-r--r--   0 albani     (502) staff       (20)     5220 2024-05-10 09:19:21.000000 monviso-0.1.5/monviso_reloaded/analyzer.py
+-rw-r--r--   0 albani     (502) staff       (20)     5177 2024-05-10 09:19:21.000000 monviso-0.1.5/monviso_reloaded/base.py
+-rw-r--r--   0 albani     (502) staff       (20)     1310 2024-05-10 09:19:21.000000 monviso-0.1.5/monviso_reloaded/cli.py
+-rw-r--r--   0 albani     (502) staff       (20)     1739 2024-02-28 10:12:03.000000 monviso-0.1.5/monviso_reloaded/cobalt_wrapper.py
+-rw-r--r--   0 albani     (502) staff       (20)     4013 2024-03-11 14:35:11.000000 monviso-0.1.5/monviso_reloaded/database_parser.py
+-rw-r--r--   0 albani     (502) staff       (20)     4181 2024-03-11 14:31:34.000000 monviso-0.1.5/monviso_reloaded/file_handler.py
+-rw-r--r--   0 albani     (502) staff       (20)    12946 2024-05-10 09:19:22.000000 monviso-0.1.5/monviso_reloaded/gene.py
+-rw-r--r--   0 albani     (502) staff       (20)    11364 2024-05-10 09:19:22.000000 monviso-0.1.5/monviso_reloaded/input_parser.py
+-rw-r--r--   0 albani     (502) staff       (20)    21313 2024-05-10 09:19:22.000000 monviso-0.1.5/monviso_reloaded/isoform.py
+-rw-r--r--   0 albani     (502) staff       (20)    13278 2024-04-09 12:59:41.000000 monviso-0.1.5/monviso_reloaded/modeller_manager.py
+-rw-r--r--   0 albani     (502) staff       (20)     5832 2024-05-10 09:19:22.000000 monviso-0.1.5/monviso_reloaded/template.py
+-rw-r--r--   0 albani     (502) staff       (20)       38 2024-05-10 09:23:15.033753 monviso-0.1.5/setup.cfg
+-rw-r--r--   0 albani     (502) staff       (20)     1561 2024-05-10 09:19:22.000000 monviso-0.1.5/setup.py
+drwxr-xr-x   0 albani     (502) staff       (20)        0 2024-05-10 09:23:15.031691 monviso-0.1.5/tests/
+-rw-r--r--   0 albani     (502) staff       (20)        0 2024-02-28 10:12:03.000000 monviso-0.1.5/tests/__init__.py
+-rw-r--r--   0 albani     (502) staff       (20)      398 2024-02-28 10:12:03.000000 monviso-0.1.5/tests/conftest.py
+-rw-r--r--   0 albani     (502) staff       (20)       96 2024-02-28 10:12:03.000000 monviso-0.1.5/tests/test_base.py
```

### Comparing `monviso-0.1.4/Containerfile` & `monviso-0.1.5/Containerfile`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Use Ubuntu as the base image
 FROM ubuntu:latest
 
 # Install necessary packages
-RUN apt-get update && apt-get install -y wget build-essential
+RUN apt-get update && apt-get install -y wget build-essential git
 RUN mkdir /Monviso
 
 # Download and install Miniconda
 RUN wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O miniconda.sh && \
     bash miniconda.sh -b -p /miniconda && \
     rm miniconda.sh
 
@@ -17,22 +17,20 @@
 RUN conda create -n myenv python=3.9 -y
 RUN echo "source activate myenv" > ~/.bashrc
 ENV PATH /miniconda/envs/myenv/bin:$PATH
 
 # Install Modeller
 RUN conda install -c salilab modeller -y
 
-# Define a build-time argument for the Modeller license
-ARG MODELLER_LICENSE=MODELIRANJE
-
+# Define a build argument for MODELLER_LICENSE
+ARG MODELLER_LICENSE
 
 # Replace the placeholder in the Modeller configuration file with the license key
 RUN sed -i "s/XXXX/${MODELLER_LICENSE}/" /miniconda/lib/modeller-*/modlib/modeller/config.py
 
-
 # Download and extract Cobalt
 RUN wget -r ftp://ftp.ncbi.nlm.nih.gov/pub/cobalt/executables/LATEST/*x64-linux.tar.gz && \
     mv ftp.ncbi.nlm.nih.gov/pub/cobalt/executables/LATEST/*x64-linux.tar.gz . && \
     rm -r ftp.ncbi.nlm.nih.gov && \
     tar -xzvf ncbi-cobalt-*-linux.tar.gz && \
     rm *.tar.gz
 RUN mv /ncbi-cobalt-3.0.0 /Monviso/cobalt/
@@ -45,18 +43,24 @@
     cd $hmmer_folder && \
     ./configure --prefix=/Monviso/hmmer/ && \
     make && \
     make install && \
     cd / && \
     rm -r $hmmer_folder
 
+# Clone the PeSTo repository from GitHub
+RUN git clone https://github.com/LBM-EPFL/PeSTo.git /Monviso/PeSTo
+RUN find /Monviso/PeSTo/ -name "*.pdb" -type f -delete
+RUN rm -r /Monviso/PeSTo/.git
+RUN rm -r /Monviso/PeSTo/masif-site_benchmark
+
 # Set the working directory
 WORKDIR /Monviso
 
 # Download and decompress the UniProt/SwissProt databases into /Monviso
 RUN wget https://ftp.uniprot.org/pub/databases/uniprot/current_release/knowledgebase/complete/uniprot_sprot.fasta.gz && \
     wget https://ftp.uniprot.org/pub/databases/uniprot/current_release/knowledgebase/complete/uniprot_sprot_varsplic.fasta.gz && \
     gzip -d uniprot_sprot.fasta.gz && \
     gzip -d uniprot_sprot_varsplic.fasta.gz
 
 # Install Monviso using pip in the myenv environment
-RUN /bin/bash -c "source activate myenv && pip install monviso==0.1.3"
+RUN /bin/bash -c "source activate myenv && pip install monviso==0.1.5"
```

### Comparing `monviso-0.1.4/LICENSE` & `monviso-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `monviso-0.1.4/PKG-INFO` & `monviso-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 Metadata-Version: 2.1
 Name: monviso
-Version: 0.1.4
+Version: 0.1.5
 Summary: MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins.
 Home-page: https://github.com/alisamalb/monviso_reloaded
-Author: Ciskio
+Author: S. Albani
 License: UNKNOWN
-Description: # Monviso reloaded
-        MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins. By leveraging data from the Uniprot database, MoNvIso facilitates a deeper understanding of protein function and variation.
-        
-        [Read the documentation here.](https://alisamalb.github.io/monviso_reloaded/)
-        
-        ## Quick start
-        
-         - Download uniprot_sprot.fasta and uniprot_sprot_varsplic.fasta from UniProt.
-        
-         - Write a mutation.txt file with the gene name and the mutations you are interested in (e.g.,):
-        ```
-        GRIN1
-        R       844     C
-        Ala     349     Thr
-        Pro     578     Arg
-        Ser     688     Tyr
-        Tyr     647     Ser
-        
-        GRIN2B
-        E413G
-        C436R
-        M1342R
-        L1424F
-        PRO1439ALA
-        ```
-        
-         - Write a parameters.dat with the calculation parameters:
-        
-        ```
-        DB_LOCATION=./
-        COBALT_HOME=./ncbi-cobalt-3.0.0/bin/
-        HMMER_HOME=/usr/local/bin/  
-        MODELLER_EXEC=mod10.5
-        RESOLUTION=4.50
-        SEQID=25
-        HMM_TO_IMPORT=100
-        MODEL_CUTOFF=5
-        PDB_TO_USE=10
-        NUM_OF_MOD_WT=1
-        NUM_OF_MOD_MUT=1
-        W_STRUCT=10
-        W_MUT=10
-        ```
-        
-        
-        ```bash
-        $ monviso_reloaded -i mutations.txt -o out/ -p parameters.dat
-        ```
-        
-        ## Development
-        
-        Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# Monviso reloaded
+MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins. By leveraging data from the Uniprot database, MoNvIso facilitates a deeper understanding of protein function and variation.
+
+[Read the documentation here.](https://alisamalb.github.io/monviso_reloaded/)
+
+## Quick start
+
+ - Download uniprot_sprot.fasta and uniprot_sprot_varsplic.fasta from UniProt.
+
+ - Write a mutation.txt file with the gene name and the mutations you are interested in (e.g.,):
+```
+GRIN1
+R       844     C
+Ala     349     Thr
+Pro     578     Arg
+Ser     688     Tyr
+Tyr     647     Ser
+
+GRIN2B
+E413G
+C436R
+M1342R
+L1424F
+PRO1439ALA
+```
+
+ - Write a parameters.dat with the calculation parameters:
+
+```
+DB_LOCATION=./
+COBALT_HOME=./ncbi-cobalt-3.0.0/bin/
+HMMER_HOME=/usr/local/bin/  
+PESTO_HOME=./PeSTO/
+MODELLER_EXEC=mod10.5
+RESOLUTION=4.50
+SEQID=25
+HMM_TO_IMPORT=100
+MODEL_CUTOFF=5
+PDB_TO_USE=10
+NUM_OF_MOD_WT=1
+NUM_OF_MOD_MUT=1
+W_STRUCT=10
+W_MUT=10
+```
+
+
+```bash
+$ monviso  isoform -i mutations.txt -o out/ -pf parameters.dat
+```
+
+## Development
+
+Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+
```

### Comparing `monviso-0.1.4/README.md` & `monviso-0.1.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -27,27 +27,28 @@
 
  - Write a parameters.dat with the calculation parameters:
 
 ```
 DB_LOCATION=./
 COBALT_HOME=./ncbi-cobalt-3.0.0/bin/
 HMMER_HOME=/usr/local/bin/  
+PESTO_HOME=./PeSTO/
 MODELLER_EXEC=mod10.5
 RESOLUTION=4.50
 SEQID=25
 HMM_TO_IMPORT=100
 MODEL_CUTOFF=5
 PDB_TO_USE=10
 NUM_OF_MOD_WT=1
 NUM_OF_MOD_MUT=1
 W_STRUCT=10
 W_MUT=10
 ```
 
 
 ```bash
-$ monviso_reloaded -i mutations.txt -o out/ -p parameters.dat
+$ monviso  isoform -i mutations.txt -o out/ -pf parameters.dat
 ```
 
 ## Development
 
 Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

### Comparing `monviso-0.1.4/monviso.egg-info/PKG-INFO` & `monviso-0.1.5/monviso.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 Metadata-Version: 2.1
 Name: monviso
-Version: 0.1.4
+Version: 0.1.5
 Summary: MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins.
 Home-page: https://github.com/alisamalb/monviso_reloaded
-Author: Ciskio
+Author: S. Albani
 License: UNKNOWN
-Description: # Monviso reloaded
-        MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins. By leveraging data from the Uniprot database, MoNvIso facilitates a deeper understanding of protein function and variation.
-        
-        [Read the documentation here.](https://alisamalb.github.io/monviso_reloaded/)
-        
-        ## Quick start
-        
-         - Download uniprot_sprot.fasta and uniprot_sprot_varsplic.fasta from UniProt.
-        
-         - Write a mutation.txt file with the gene name and the mutations you are interested in (e.g.,):
-        ```
-        GRIN1
-        R       844     C
-        Ala     349     Thr
-        Pro     578     Arg
-        Ser     688     Tyr
-        Tyr     647     Ser
-        
-        GRIN2B
-        E413G
-        C436R
-        M1342R
-        L1424F
-        PRO1439ALA
-        ```
-        
-         - Write a parameters.dat with the calculation parameters:
-        
-        ```
-        DB_LOCATION=./
-        COBALT_HOME=./ncbi-cobalt-3.0.0/bin/
-        HMMER_HOME=/usr/local/bin/  
-        MODELLER_EXEC=mod10.5
-        RESOLUTION=4.50
-        SEQID=25
-        HMM_TO_IMPORT=100
-        MODEL_CUTOFF=5
-        PDB_TO_USE=10
-        NUM_OF_MOD_WT=1
-        NUM_OF_MOD_MUT=1
-        W_STRUCT=10
-        W_MUT=10
-        ```
-        
-        
-        ```bash
-        $ monviso_reloaded -i mutations.txt -o out/ -p parameters.dat
-        ```
-        
-        ## Development
-        
-        Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# Monviso reloaded
+MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins. By leveraging data from the Uniprot database, MoNvIso facilitates a deeper understanding of protein function and variation.
+
+[Read the documentation here.](https://alisamalb.github.io/monviso_reloaded/)
+
+## Quick start
+
+ - Download uniprot_sprot.fasta and uniprot_sprot_varsplic.fasta from UniProt.
+
+ - Write a mutation.txt file with the gene name and the mutations you are interested in (e.g.,):
+```
+GRIN1
+R       844     C
+Ala     349     Thr
+Pro     578     Arg
+Ser     688     Tyr
+Tyr     647     Ser
+
+GRIN2B
+E413G
+C436R
+M1342R
+L1424F
+PRO1439ALA
+```
+
+ - Write a parameters.dat with the calculation parameters:
+
+```
+DB_LOCATION=./
+COBALT_HOME=./ncbi-cobalt-3.0.0/bin/
+HMMER_HOME=/usr/local/bin/  
+PESTO_HOME=./PeSTO/
+MODELLER_EXEC=mod10.5
+RESOLUTION=4.50
+SEQID=25
+HMM_TO_IMPORT=100
+MODEL_CUTOFF=5
+PDB_TO_USE=10
+NUM_OF_MOD_WT=1
+NUM_OF_MOD_MUT=1
+W_STRUCT=10
+W_MUT=10
+```
+
+
+```bash
+$ monviso  isoform -i mutations.txt -o out/ -pf parameters.dat
+```
+
+## Development
+
+Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+
```

### Comparing `monviso-0.1.4/monviso.egg-info/SOURCES.txt` & `monviso-0.1.5/monviso.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,33 +10,37 @@
 monviso.egg-info/entry_points.txt
 monviso.egg-info/requires.txt
 monviso.egg-info/top_level.txt
 monviso_reloaded/PDB_manager.py
 monviso_reloaded/VERSION
 monviso_reloaded/__init__.py
 monviso_reloaded/__main__.py
+monviso_reloaded/analyzer.py
 monviso_reloaded/base.py
 monviso_reloaded/cli.py
 monviso_reloaded/cobalt_wrapper.py
 monviso_reloaded/database_parser.py
 monviso_reloaded/file_handler.py
 monviso_reloaded/gene.py
 monviso_reloaded/input_parser.py
 monviso_reloaded/isoform.py
 monviso_reloaded/modeller_manager.py
 monviso_reloaded/template.py
 monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc
 monviso_reloaded/__pycache__/__init__.cpython-39.pyc
 monviso_reloaded/__pycache__/__main__.cpython-39.pyc
+monviso_reloaded/__pycache__/analyzer.cpython-39.pyc
 monviso_reloaded/__pycache__/base.cpython-39.pyc
 monviso_reloaded/__pycache__/cli.cpython-39.pyc
 monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc
 monviso_reloaded/__pycache__/database_parser.cpython-39.pyc
 monviso_reloaded/__pycache__/file_handler.cpython-39.pyc
 monviso_reloaded/__pycache__/gene.cpython-39.pyc
 monviso_reloaded/__pycache__/input_parser.cpython-39.pyc
+monviso_reloaded/__pycache__/installer.cpython-39.pyc
 monviso_reloaded/__pycache__/isoform.cpython-39.pyc
 monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc
+monviso_reloaded/__pycache__/pesto_analyzer.cpython-39.pyc
 monviso_reloaded/__pycache__/template.cpython-39.pyc
 tests/__init__.py
 tests/conftest.py
 tests/test_base.py
```

### Comparing `monviso-0.1.4/monviso_reloaded/PDB_manager.py` & `monviso-0.1.5/monviso_reloaded/PDB_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import Union
 
-from Bio.PDB import PDBIO, PDBList, PDBParser, Select, Selection
+from Bio.PDB import PDBIO, PDBList, PDBParser, Select, Selection, MMCIFParser
 from Bio.PDB.Polypeptide import index_to_one, three_to_index
 
 from .file_handler import FileHandler
 
 
 class ChainSelection(Select):
     def __init__(self, chain_letters, standard_atoms=True):
@@ -87,23 +87,40 @@
             else:
                 pdbl = PDBList()
                 filename = pdbl.retrieve_pdb_file(
                     pdb,
                     pdir=str(Path(out_path, download_dir)),
                     file_format="pdb",
                     overwrite=True,
+                    obsolete=False
                 )
 
                 if fh.check_existence(filename):
                     fh.move_file(
                         Path(out_path, download_dir, wrong_pdbname), filepath
                     )
                     return filepath
                 else:
-                    raise (FileNotFoundError(f"Could not download PDB {pdb}"))
+                    RuntimeWarning(f"Could not download PDB {pdb}. Now trying to find the mmCIF format...")
+                filepath = Path(out_path, download_dir, right_pdbname.replace("pdb","cif"))
+                filename = pdbl.retrieve_pdb_file(
+                    pdb,
+                    pdir=str(Path(out_path, download_dir)),
+                    overwrite=True,
+                    obsolete=False
+                )
+
+                if fh.check_existence(filename):
+                    fh.move_file(
+                        filename, filepath
+                    )
+                    return filepath
+                else:
+                    FileNotFoundError(f"Could not download mmCIF either. Structure {pdb} not found.")
+
 
     def extract_clean_chain(
         self,
         input_pdb_path: Union[Path, str],
         output_pdb_path: Union[Path, str],
         chain_letter: str,
         resolution_cutoff: float,
@@ -121,15 +138,18 @@
             output_pdb_path (Union[Path,str]): The path of the output PDB
             chain_letter (str): Letter of the chain to extract.
 
         Returns:
             resolution (float or None): The resolution of the
             X-Ray or CryoEM structure
         """
-        parser = PDBParser(QUIET=True)
+        if str(input_pdb_path).endswith("pdb"):
+            parser = PDBParser(QUIET=True)
+        else:
+            parser = MMCIFParser()
         structure = parser.get_structure("structure", str(input_pdb_path))
         if structure.header["resolution"]:
             if structure.header["resolution"] <= resolution_cutoff:
                 with FileHandler() as fh:
                     io = PDBIO()
                     io.set_structure(structure)
                     if not fh.check_existence(output_pdb_path):
```

### Comparing `monviso-0.1.4/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc` & `monviso-0.1.5/monviso_reloaded/__pycache__/PDB_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.4/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc` & `monviso-0.1.5/monviso_reloaded/__pycache__/cobalt_wrapper.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.4/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc` & `monviso-0.1.5/monviso_reloaded/__pycache__/database_parser.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.4/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc` & `monviso-0.1.5/monviso_reloaded/__pycache__/file_handler.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.4/monviso_reloaded/__pycache__/gene.cpython-39.pyc` & `monviso-0.1.5/monviso_reloaded/__pycache__/gene.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.4/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc` & `monviso-0.1.5/monviso_reloaded/__pycache__/input_parser.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Mar  1 15:46:37 2024 UTC, .py size: 8954 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,425 +1,500 @@
-00000000: 610d 0d0a 0000 0000 5df8 e165 fa22 0000  a.......]..e."..
+00000000: 610d 0d0a 0000 0000 b492 1e66 642c 0000  a..........fd,..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 6500 6a06  ..G.d.d...d.e.j.
 00000060: 8303 5a07 6401 5300 2906 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2901 da04 5061 7468 2902 da04 4469 6374  )...Path)...Dict
 00000080: da04 4c69 7374 6300 0000 0000 0000 0000  ..Listc.........
 00000090: 0000 0000 0000 0004 0000 0000 0000 0073  ...............s
-000000a0: 9a00 0000 6500 5a01 6400 5a02 8700 6601  ....e.Z.d.Z...f.
+000000a0: a200 0000 6500 5a01 6400 5a02 8700 6601  ....e.Z.d.Z...f.
 000000b0: 6401 6402 8408 5a03 6403 6404 9c01 8700  d.d...Z.d.d.....
 000000c0: 6601 6405 6406 840c 5a04 6505 6a06 6403  f.d.d...Z.e.j.d.
 000000d0: 6407 9c02 6408 6409 8404 5a07 6505 6a06  d...d.d...Z.e.j.
-000000e0: 6508 640a 9c02 640b 640c 8404 5a09 6418  e.d...d.d...Z.d.
+000000e0: 6508 640a 9c02 640b 640c 8404 5a09 641a  e.d...d.d...Z.d.
 000000f0: 6505 6a06 650a 640e 9c02 640f 6410 8405  e.j.e.d...d.d...
 00000100: 5a0b 6505 6a06 650a 6407 9c02 6411 6412  Z.e.j.e.d...d.d.
-00000110: 8404 5a0c 6505 6a06 650a 6403 6413 9c03  ..Z.e.j.e.d.d...
-00000120: 6414 6415 8404 5a0d 650e 6404 9c01 6416  d.d...Z.e.d...d.
-00000130: 6417 8404 5a0f 8700 0400 5a10 5300 2919  d...Z.....Z.S.).
-00000140: da0b 496e 7075 7450 6172 7365 7263 0100  ..InputParserc..
-00000150: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00000160: 0000 0f00 0000 731e 0000 0074 0083 006a  ......s....t...j
-00000170: 017c 0169 007c 02a4 018e 0101 007c 00a0  .|.i.|.......|..
-00000180: 02a1 0001 0064 0053 0029 014e 2903 da05  .....d.S.).N)...
-00000190: 7375 7065 72da 085f 5f69 6e69 745f 5fda  super..__init__.
-000001a0: 0d61 6464 5f61 7267 756d 656e 7473 2903  .add_arguments).
-000001b0: da04 7365 6c66 da04 6172 6773 da06 6b77  ..self..args..kw
-000001c0: 6172 6773 a901 da09 5f5f 636c 6173 735f  args....__class_
-000001d0: 5fa9 00fa 552f 5573 6572 732f 616c 6261  _...U/Users/alba
-000001e0: 6e69 2f57 6f72 6b2f 5072 6f6a 6563 7473  ni/Work/Projects
-000001f0: 2f4d 6f6e 7669 736f 2f6d 6f6e 7669 736f  /Monviso/monviso
-00000200: 5f72 656c 6f61 6465 642f 6d6f 6e76 6973  _reloaded/monvis
-00000210: 6f5f 7265 6c6f 6164 6564 2f69 6e70 7574  o_reloaded/input
-00000220: 5f70 6172 7365 722e 7079 7207 0000 0007  _parser.pyr.....
-00000230: 0000 0073 0400 0000 0001 1201 7a14 496e  ...s........z.In
-00000240: 7075 7450 6172 7365 722e 5f5f 696e 6974  putParser.__init
-00000250: 5f5f 4e29 01da 0672 6574 7572 6e63 0100  __N)...returnc..
-00000260: 0000 0000 0000 0000 0000 0200 0000 0800  ................
-00000270: 0000 0300 0000 735c 0100 0074 0083 006a  ......s\...t...j
-00000280: 0164 0164 0264 0374 0264 0464 058d 0501  .d.d.d.t.d.d....
-00000290: 0074 0083 006a 0164 0664 0764 0874 0264  .t...j.d.d.d.t.d
-000002a0: 0464 058d 0501 0074 0083 006a 0164 0964  .d.....t...j.d.d
-000002b0: 0a64 0b74 0264 0c64 058d 0501 0074 0083  .d.t.d.d.....t..
-000002c0: 006a 0164 0d64 0e64 0f74 0264 0c64 058d  .j.d.d.d.t.d.d..
-000002d0: 0501 0074 0083 006a 0164 1064 1164 1274  ...t...j.d.d.d.t
-000002e0: 0264 0c64 058d 0501 0074 0083 006a 0164  .d.d.....t...j.d
-000002f0: 1364 1464 1574 0264 0c64 058d 0501 0074  .d.d.t.d.d.....t
-00000300: 0083 00a0 0364 1664 17a1 027d 017c 016a  .....d.d...}.|.j
-00000310: 0164 1864 1964 1a74 0464 1b64 0c64 1c8d  .d.d.d.t.d.d.d..
-00000320: 0601 007c 016a 0164 1d64 1e64 1f74 0464  ...|.j.d.d.d.t.d
-00000330: 2064 0c64 1c8d 0601 007c 016a 0164 2164   d.d.....|.j.d!d
-00000340: 2264 2374 0564 2464 0c64 1c8d 0601 007c  "d#t.d$d.d.....|
-00000350: 016a 0164 2564 2664 2774 0564 2864 0c64  .j.d%d&d't.d(d.d
-00000360: 1c8d 0601 007c 016a 0164 2964 2a64 2b74  .....|.j.d)d*d+t
-00000370: 0564 2864 0c64 1c8d 0601 007c 016a 0164  .d(d.d.....|.j.d
-00000380: 2c64 2d64 2e74 0464 2f64 0c64 1c8d 0601  ,d-d.t.d/d.d....
-00000390: 007c 016a 0164 3064 3164 3274 0464 3364  .|.j.d0d1d2t.d3d
-000003a0: 0c64 1c8d 0601 007c 016a 0164 3464 3564  .d.....|.j.d4d5d
-000003b0: 3674 0464 3364 0c64 1c8d 0601 007c 016a  6t.d3d.d.....|.j
-000003c0: 0164 3764 3864 3974 0264 3a64 0c64 1c8d  .d7d8d9t.d:d.d..
-000003d0: 0601 0064 3b53 0029 3c7a 5841 6464 2061  ...d;S.)<zXAdd a
-000003e0: 206c 6973 7420 6f66 2065 7870 6563 7465   list of expecte
-000003f0: 6420 6172 6775 6d65 6e74 7320 746f 2074  d arguments to t
-00000400: 6865 2050 6172 7365 7220 696e 7374 616e  he Parser instan
-00000410: 6365 2e0a 0a20 2020 2020 2020 203a 7265  ce...        :re
-00000420: 7475 726e 3a20 4e6f 6e65 0a20 2020 2020  turn: None.     
-00000430: 2020 207a 022d 697a 0c2d 2d69 6e70 7574     z.-iz.--input
-00000440: 5f66 696c 657a 2450 6174 6820 746f 2074  _filez$Path to t
-00000450: 6865 2066 696c 6520 6765 6e65 7320 616e  he file genes an
-00000460: 6420 6d75 7461 7469 6f6e 7354 2903 da04  d mutationsT)...
-00000470: 6865 6c70 da04 7479 7065 da08 7265 7175  help..type..requ
-00000480: 6972 6564 7a02 2d6f 7a0a 2d2d 6f75 745f  iredz.-oz.--out_
-00000490: 7061 7468 7a19 5061 7468 2074 6f20 7468  pathz.Path to th
-000004a0: 6520 6f75 7470 7574 2066 6f6c 6465 727a  e output folderz
-000004b0: 032d 7066 7a0a 2d2d 7061 725f 6669 6c65  .-pfz.--par_file
-000004c0: 7a25 496e 7075 7420 7468 6520 7061 7468  z%Input the path
-000004d0: 2074 6f20 7468 6520 7061 7261 6d65 7465   to the paramete
-000004e0: 7273 2066 696c 6546 7a03 2d64 627a 092d  rs fileFz.-dbz.-
-000004f0: 2d64 625f 686f 6d65 7a4d 7061 7468 2074  -db_homezMpath t
-00000500: 6f20 7468 6520 4442 7320 636f 6e74 6169  o the DBs contai
-00000510: 6e69 6e67 2074 6865 2020 2020 2020 2020  ning the        
-00000520: 2020 2020 2020 2020 6361 6e6f 6e69 6361          canonica
-00000530: 6c20 616e 6420 6973 6f66 6f72 6d20 7365  l and isoform se
-00000540: 7175 656e 6365 737a 072d 636f 6261 6c74  quencesz.-cobalt
-00000550: 7a0d 2d2d 636f 6261 6c74 5f68 6f6d 657a  z.--cobalt_homez
-00000560: 1970 6174 6820 746f 2043 4f42 414c 5420  .path to COBALT 
-00000570: 6269 6e20 666f 6c64 6572 7a06 2d68 6d6d  bin folderz.-hmm
-00000580: 6572 7a0c 2d2d 686d 6d65 725f 686f 6d65  erz.--hmmer_home
-00000590: 7a18 7061 7468 2074 6f20 484d 4d45 5220  z.path to HMMER 
-000005a0: 6269 6e20 666f 6c64 6572 da05 696e 7075  bin folder..inpu
-000005b0: 747a 1c6d 616e 7561 6c6c 7920 7072 6f76  tz.manually prov
-000005c0: 6964 6573 2074 6865 2069 6e70 7574 737a  ides the inputsz
-000005d0: 042d 7265 737a 0c2d 2d72 6573 6f6c 7574  .-resz.--resolut
-000005e0: 696f 6e7a 1977 6f72 7374 2061 6363 6570  ionz.worst accep
-000005f0: 7465 6420 7265 736f 6c75 7469 6f6e 6700  ted resolutiong.
-00000600: 0000 0000 0012 4029 0472 1100 0000 7212  ......@).r....r.
-00000610: 0000 00da 0764 6566 6175 6c74 7213 0000  .....defaultr...
-00000620: 007a 062d 7365 7169 647a 132d 2d73 6571  .z.-seqidz.--seq
-00000630: 7565 6e63 655f 6964 656e 7469 7479 7a22  uence_identityz"
-00000640: 6d69 6e69 6d75 6d20 7365 7175 656e 6365  minimum sequence
-00000650: 2069 6465 6e74 6974 7920 6163 6365 7074   identity accept
-00000660: 6564 e919 0000 007a 082d 6d61 785f 7064  ed.....z.-max_pd
-00000670: 627a 132d 2d6d 6178 5f70 6462 5f74 656d  bz.--max_pdb_tem
-00000680: 706c 6174 6573 7a2a 6d61 7869 6d75 6d20  platesz*maximum 
-00000690: 6e75 6d62 6572 206f 6620 5044 4273 2074  number of PDBs t
-000006a0: 6f20 7573 6520 6173 2074 656d 706c 6174  o use as templat
-000006b0: 6573 e90a 0000 007a 072d 7774 5f6d 6f64  es.....z.-wt_mod
-000006c0: 7a0e 2d2d 6d61 785f 6d6f 6465 6c5f 7774  z.--max_model_wt
-000006d0: 7a2b 6d61 7869 6d75 6d20 6e75 6d62 6572  z+maximum number
-000006e0: 206f 6620 7769 6c64 2d74 7970 6520 6d6f   of wild-type mo
-000006f0: 6465 6c73 2074 6f20 6275 696c 64e9 0100  dels to build...
-00000700: 0000 7a08 2d6d 7574 5f6d 6f64 7a0f 2d2d  ..z.-mut_modz.--
-00000710: 6d61 785f 6d6f 6465 6c5f 6d75 747a 286d  max_model_mutz(m
-00000720: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
-00000730: 206d 7574 616e 7420 6d6f 6465 6c73 2074   mutant models t
-00000740: 6f20 6275 696c 647a 032d 7263 7a0c 2d2d  o buildz.-rcz.--
-00000750: 7265 735f 6375 746f 6666 7a59 6d61 7869  res_cutoffzYmaxi
-00000760: 6d75 6d20 6e75 6d62 6572 206f 6620 6e6f  mum number of no
-00000770: 7420 6372 7973 7461 6c69 7365 6420 7265  t crystalised re
-00000780: 7369 6475 6573 2020 2020 2020 2020 2020  sidues          
-00000790: 2020 2020 2020 6163 6365 7074 6564 2062        accepted b
-000007a0: 6566 6f72 6520 6375 7474 696e 6720 6120  efore cutting a 
-000007b0: 6d6f 6465 6c67 0000 0000 0000 1440 7a03  modelg.......@z.
-000007c0: 2d77 737a 0a2d 2d77 5f73 7472 7563 747a  -wsz.--w_structz
-000007d0: 2177 6569 6768 7420 6f66 2074 6865 2073  !weight of the s
-000007e0: 7472 7563 7475 7261 6c20 6675 6e63 7469  tructural functi
-000007f0: 6f6e 6700 0000 0000 0024 407a 032d 776d  ong......$@z.-wm
-00000800: 7a07 2d2d 775f 6d75 747a 1f77 6569 6768  z.--w_mutz.weigh
-00000810: 7420 6f66 2074 6865 206d 7574 6174 696f  t of the mutatio
-00000820: 6e20 6675 6e63 7469 6f6e 7a04 2d6d 6f64  n functionz.-mod
-00000830: 7a0f 2d2d 6d6f 6465 6c6c 6572 5f65 7865  z.--modeller_exe
-00000840: 637a 1f70 6174 6820 746f 2074 6865 206d  cz.path to the m
-00000850: 6f64 656c 6c65 7220 6578 6563 7574 6162  odeller executab
-00000860: 6c65 7a07 6d6f 6431 302e 344e 2906 7206  lez.mod10.4N).r.
-00000870: 0000 00da 0c61 6464 5f61 7267 756d 656e  .....add_argumen
-00000880: 74da 0373 7472 da12 6164 645f 6172 6775  t..str..add_argu
-00000890: 6d65 6e74 5f67 726f 7570 da05 666c 6f61  ment_group..floa
-000008a0: 74da 0369 6e74 2902 7209 0000 005a 1070  t..int).r....Z.p
-000008b0: 6172 616d 6574 6572 735f 6772 6f75 7072  arameters_groupr
-000008c0: 0c00 0000 720e 0000 0072 0f00 0000 7208  ....r....r....r.
-000008d0: 0000 000b 0000 0073 ea00 0000 0005 0601  .......s........
-000008e0: 0201 0201 0201 0201 02fb 0608 0601 0201  ................
-000008f0: 0201 0201 0201 02fb 0608 0601 0201 0201  ................
-00000900: 0201 0201 02fb 0607 0601 0201 0201 0202  ................
-00000910: 0201 02fa 0609 0601 0201 0201 0201 0201  ................
-00000920: 02fb 0608 0601 0201 0201 0201 0201 02fb  ................
-00000930: 0608 0601 04ff 0403 0401 0201 0201 0201  ................
-00000940: 0201 0201 02fa 0608 0401 0201 0201 0201  ................
-00000950: 0201 0201 02fa 0608 0401 0201 0201 0201  ................
-00000960: 0201 0201 02fa 0609 0401 0201 0201 0201  ................
-00000970: 0201 0201 02fa 0609 0401 0201 0201 0201  ................
-00000980: 0201 0201 02fa 0609 0401 0201 0201 0202  ................
-00000990: 0201 0201 02f9 060a 0401 0201 0201 0201  ................
-000009a0: 0201 0201 02fa 0609 0401 0201 0201 0201  ................
-000009b0: 0201 0201 02fa 0609 0401 0201 0201 0201  ................
-000009c0: 0201 0201 02fa 7a19 496e 7075 7450 6172  ......z.InputPar
-000009d0: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
-000009e0: 7329 0272 0a00 0000 7210 0000 0063 0200  s).r....r....c..
-000009f0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00000a00: 0000 4300 0000 7346 0000 007c 016a 0073  ..C...sF...|.j.s
-00000a10: 227c 016a 0172 187c 016a 0272 187c 016a  "|.j.r.|.j.r.|.j
-00000a20: 0373 2274 0464 0183 0182 016e 207c 016a  .s"t.d.....n |.j
-00000a30: 0072 427c 016a 0173 3a7c 016a 0273 3a7c  .rB|.j.s:|.j.s:|
-00000a40: 016a 0372 4274 0464 0283 0182 0164 0353  .j.rBt.d.....d.S
-00000a50: 0029 047a 6756 6572 6966 7920 7468 6174  .).zgVerify that
-00000a60: 2074 6865 206e 6563 6573 7361 7279 2070   the necessary p
-00000a70: 6172 616d 6574 6572 7320 6861 7665 2062  arameters have b
-00000a80: 6565 6e20 7072 6f76 6964 6564 0a0a 2020  een provided..  
-00000a90: 2020 2020 2020 3a70 6172 616d 2061 7267        :param arg
-00000aa0: 733a 2070 6173 7365 6420 6172 6775 6d65  s: passed argume
-00000ab0: 6e74 730a 2020 2020 2020 2020 7a66 5370  nts.        zfSp
-00000ac0: 6563 6966 7920 6120 7061 7261 6d65 7465  ecify a paramete
-00000ad0: 7273 2066 696c 6520 6f72 2069 6e73 6572  rs file or inser
-00000ae0: 7420 7468 6520 7061 7468 7320 2020 2020  t the paths     
-00000af0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00000b00: 6f20 7468 6520 4442 732c 2043 4f42 414c  o the DBs, COBAL
-00000b10: 5420 616e 6420 484d 4d45 5220 6d61 6e75  T and HMMER manu
-00000b20: 616c 6c79 7a51 4569 7468 6572 2073 7065  allyzQEither spe
-00000b30: 6369 6679 2061 2070 6172 616d 6574 6572  cify a parameter
-00000b40: 7320 6669 6c65 206f 7220 2020 2020 2020  s file or       
-00000b50: 2020 2020 2020 2020 2020 2020 2069 6e73               ins
-00000b60: 6572 7420 7061 7261 6d65 7465 7273 206d  ert parameters m
-00000b70: 616e 7561 6c6c 794e 2905 da08 7061 725f  anuallyN)...par_
-00000b80: 6669 6c65 da07 6462 5f68 6f6d 65da 0b63  file..db_home..c
-00000b90: 6f62 616c 745f 686f 6d65 da0a 686d 6d65  obalt_home..hmme
-00000ba0: 725f 686f 6d65 da09 5479 7065 4572 726f  r_home..TypeErro
-00000bb0: 72a9 0272 0900 0000 720a 0000 0072 0e00  r..r....r....r..
-00000bc0: 0000 720e 0000 0072 0f00 0000 da0f 6368  ..r....r......ch
-00000bd0: 6563 6b5f 6172 6775 6d65 6e74 7393 0000  eck_arguments...
-00000be0: 0073 2800 0000 0005 0601 04ff 0201 04ff  .s(.............
-00000bf0: 0201 04ff 0203 0201 02ff 0604 0601 04ff  ................
-00000c00: 0201 04ff 0201 04ff 0203 0201 02ff 7a1b  ..............z.
-00000c10: 496e 7075 7450 6172 7365 722e 6368 6563  InputParser.chec
-00000c20: 6b5f 6172 6775 6d65 6e74 7329 02da 126d  k_arguments)...m
-00000c30: 7574 6174 696f 6e5f 6669 6c65 5f70 6174  utation_file_pat
-00000c40: 6872 1000 0000 6302 0000 0000 0000 0000  hr....c.........
-00000c50: 0000 0005 0000 0008 0000 0043 0000 0073  ...........C...s
-00000c60: 7c00 0000 7400 7c01 8301 a001 a100 8f18  |...t.|.........
-00000c70: 7d02 7c02 a002 a100 7d03 5700 6401 0400  }.|.....}.W.d...
-00000c80: 0400 8303 0100 6e10 3100 732a 3000 0100  ......n.1.s*0...
-00000c90: 0100 0100 5900 0100 7c03 6402 1900 6403  ....Y...|.d...d.
-00000ca0: 6b02 724e 7c03 6401 6402 8502 1900 7d03  k.rN|.d.d.....}.
-00000cb0: 7134 6404 7c03 7600 7264 7c03 a003 6404  q4d.|.v.rd|...d.
-00000cc0: 6405 a102 7d03 714e 6406 6407 8400 7c03  d...}.qNd.d...|.
-00000cd0: a004 6405 a101 4400 8301 7d04 7c04 5300  ..d...D...}.|.S.
-00000ce0: 2908 7ade 5061 7273 6520 7468 6520 6c69  ).z.Parse the li
-00000cf0: 7374 206f 6620 6d75 7461 7469 6f6e 7320  st of mutations 
-00000d00: 616e 6420 6765 6e65 7320 6672 6f6d 2074  and genes from t
-00000d10: 6865 206d 7574 6174 696f 6e5f 6c69 7374  he mutation_list
-00000d20: 2066 696c 652e 0a0a 2020 2020 2020 2020   file...        
-00000d30: 3a70 6172 616d 206d 7574 6174 696f 6e5f  :param mutation_
-00000d40: 6c69 7374 3a20 7061 7468 2074 6f20 7468  list: path to th
-00000d50: 6520 6669 6c65 2063 6f6e 7461 696e 696e  e file containin
-00000d60: 6720 7468 6520 6c69 7374 0a20 2020 2020  g the list.     
-00000d70: 2020 206f 6620 6d75 7461 7469 6f6e 7320     of mutations 
-00000d80: 616e 6420 6765 6e65 730a 2020 2020 2020  and genes.      
-00000d90: 2020 3a72 6574 7572 6e3a 2054 6865 206c    :return: The l
-00000da0: 6973 7420 6f66 2067 656e 6520 616e 6420  ist of gene and 
-00000db0: 6d75 7461 7469 6f6e 730a 2020 2020 2020  mutations.      
-00000dc0: 2020 4ee9 ffff ffff da01 0a7a 030a 0a0a    N........z....
-00000dd0: 7a02 0a0a 6301 0000 0000 0000 0000 0000  z...c...........
-00000de0: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
-00000df0: 0000 6700 7c00 5d0c 7d01 7c01 a000 a100  ..g.|.].}.|.....
-00000e00: 9102 7104 5300 720e 0000 0029 01da 0a73  ..q.S.r....)...s
-00000e10: 706c 6974 6c69 6e65 7329 02da 022e 30da  plitlines)....0.
-00000e20: 0562 6c6f 636b 720e 0000 0072 0e00 0000  .blockr....r....
-00000e30: 720f 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
-00000e40: 3eb9 0000 00f3 0000 0000 7a2b 496e 7075  >.........z+Inpu
-00000e50: 7450 6172 7365 722e 7061 7273 655f 696e  tParser.parse_in
-00000e60: 7075 742e 3c6c 6f63 616c 733e 2e3c 6c69  put.<locals>.<li
-00000e70: 7374 636f 6d70 3e29 0572 0200 0000 da04  stcomp>).r......
-00000e80: 6f70 656e da04 7265 6164 da07 7265 706c  open..read..repl
-00000e90: 6163 65da 0573 706c 6974 2905 7209 0000  ace..split).r...
-00000ea0: 0072 2500 0000 da07 6d79 5f66 696c 65da  .r%.....my_file.
-00000eb0: 0763 6f6e 7465 6e74 da06 626c 6f63 6b73  .content..blocks
-00000ec0: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
-00000ed0: 0b70 6172 7365 5f69 6e70 7574 a700 0000  .parse_input....
-00000ee0: 7310 0000 0000 070e 0126 040c 010e 0208  s........&......
-00000ef0: 010e 0214 017a 1749 6e70 7574 5061 7273  .....z.InputPars
-00000f00: 6572 2e70 6172 7365 5f69 6e70 7574 fa0e  er.parse_input..
-00000f10: 7061 7261 6d65 7465 7273 2e64 6174 2902  parameters.dat).
-00000f20: da0f 7061 7261 6d65 7465 7273 5f70 6174  ..parameters_pat
-00000f30: 6872 1000 0000 6302 0000 0000 0000 0000  hr....c.........
-00000f40: 0000 000a 0000 000d 0000 0043 0000 0073  ...........C...s
-00000f50: bc00 0000 6401 6401 6401 6401 6401 6401  ....d.d.d.d.d.d.
-00000f60: 6401 6401 6401 6401 6401 6401 6402 9c0c  d.d.d.d.d.d.d...
-00000f70: 7d02 7400 7c02 8301 7d03 7401 7c01 8301  }.t.|...}.t.|...
-00000f80: a002 a100 7346 6403 7c01 9b00 6404 9d03  ....sFd.|...d...
-00000f90: 7d04 7403 7c04 8301 8201 7401 7c01 8301  }.t.|.....t.|...
-00000fa0: a004 a100 8f18 7d05 7c05 a005 a100 7d06  ......}.|.....}.
-00000fb0: 5700 6401 0400 0400 8303 0100 6e10 3100  W.d.........n.1.
-00000fc0: 7370 3000 0100 0100 0100 5900 0100 7c03  sp0.......Y...|.
-00000fd0: 4400 5d38 7d07 7c06 4400 5d2e 7d08 7c07  D.]8}.|.D.].}.|.
-00000fe0: 7c08 7600 7286 7c08 7c08 a006 6405 a101  |.v.r.|.|...d...
-00000ff0: 6406 1700 6401 8502 1900 a007 a100 7d09  d...d.........}.
-00001000: 7c09 7c02 7c07 3c00 7186 717e 7c02 5300  |.|.|.<.q.q~|.S.
-00001010: 2907 7aeb 436f 6c6c 6563 7420 7468 6520  ).z.Collect the 
-00001020: 7061 7261 6d65 7465 7273 2066 726f 6d20  parameters from 
-00001030: 7468 6520 7061 7261 6d65 7465 7273 2066  the parameters f
-00001040: 696c 6520 6966 2070 726f 7669 6465 642e  ile if provided.
-00001050: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00001060: 2070 6172 616d 6574 6572 735f 7061 7468   parameters_path
-00001070: 3a20 5061 7468 2074 6f20 7468 6520 7061  : Path to the pa
-00001080: 7261 6d65 7465 7273 2066 696c 652c 0a20  rameters file,. 
-00001090: 2020 2020 2020 2064 6566 6175 6c74 7320         defaults 
-000010a0: 746f 2022 7061 7261 6d65 7465 7273 2e64  to "parameters.d
-000010b0: 6174 222e 0a0a 2020 2020 2020 2020 3a72  at"...        :r
-000010c0: 6574 7572 6e3a 2044 6963 7420 6f66 206b  eturn: Dict of k
-000010d0: 6579 776f 7264 7320 7769 7468 2074 6865  eywords with the
-000010e0: 2061 7373 6f63 6961 7465 6420 7061 7261   associated para
-000010f0: 6d65 7465 7273 0a20 2020 2020 2020 204e  meters.        N
-00001100: a90c da0a 5245 534f 4c55 5449 4f4e da05  ....RESOLUTION..
-00001110: 5345 5149 44da 0a50 4442 5f54 4f5f 5553  SEQID..PDB_TO_US
-00001120: 45da 0b44 425f 4c4f 4341 5449 4f4e da0a  E..DB_LOCATION..
-00001130: 484d 4d45 525f 484f 4d45 da0b 434f 4241  HMMER_HOME..COBA
-00001140: 4c54 5f48 4f4d 45da 0c4d 4f44 454c 5f43  LT_HOME..MODEL_C
-00001150: 5554 4f46 46da 0d4e 554d 5f4f 465f 4d4f  UTOFF..NUM_OF_MO
-00001160: 445f 5754 da0e 4e55 4d5f 4f46 5f4d 4f44  D_WT..NUM_OF_MOD
-00001170: 5f4d 5554 da08 575f 5354 5255 4354 da05  _MUT..W_STRUCT..
-00001180: 575f 4d55 54da 0d4d 4f44 454c 4c45 525f  W_MUT..MODELLER_
-00001190: 4558 4543 7a1d 5061 7261 6d65 7465 7273  EXECz.Parameters
-000011a0: 2066 696c 6520 6e6f 7420 666f 756e 6420   file not found 
-000011b0: 696e 207a 302c 2020 2020 2020 2020 2020  in z0,          
-000011c0: 2020 2020 2020 706c 6561 7365 2063 6865        please che
-000011d0: 636b 2074 6865 2070 6174 6820 7072 6f76  ck the path prov
-000011e0: 6964 6564 2efa 013d 7218 0000 0029 08da  ided...=r....)..
-000011f0: 046c 6973 7472 0200 0000 da06 6578 6973  .listr......exis
-00001200: 7473 7222 0000 0072 2d00 0000 da09 7265  tsr"...r-.....re
-00001210: 6164 6c69 6e65 73da 0466 696e 64da 0573  adlines..find..s
-00001220: 7472 6970 290a 7209 0000 0072 3600 0000  trip).r....r6...
-00001230: da08 6b65 7977 6f72 6473 da04 6b65 7973  ..keywords..keys
-00001240: 5a0d 6572 726f 725f 6d65 7373 6167 6572  Z.error_messager
-00001250: 3100 0000 da05 6c69 6e65 73da 036b 6579  1.....lines..key
-00001260: da04 6c69 6e65 da05 7661 6c75 6572 0e00  ..line..valuer..
-00001270: 0000 720e 0000 0072 0f00 0000 da0e 6765  ..r....r......ge
-00001280: 745f 7061 7261 6d65 7465 7273 bc00 0000  t_parameters....
-00001290: 7332 0000 0000 0c02 0102 0102 0102 0102  s2..............
-000012a0: 0102 0102 0102 0102 0102 0102 0102 f406  ................
-000012b0: 0e08 010c 020c 0208 020e 0126 0208 0108  ...........&....
-000012c0: 0108 011a 010c 017a 1a49 6e70 7574 5061  .......z.InputPa
-000012d0: 7273 6572 2e67 6574 5f70 6172 616d 6574  rser.get_paramet
-000012e0: 6572 7363 0200 0000 0000 0000 0000 0000  ersc............
-000012f0: 0200 0000 0d00 0000 4300 0000 7336 0000  ........C...s6..
-00001300: 007c 016a 007c 016a 017c 016a 027c 016a  .|.j.|.j.|.j.|.j
-00001310: 037c 016a 047c 016a 057c 016a 067c 016a  .|.j.|.j.|.j.|.j
-00001320: 077c 016a 087c 016a 097c 016a 0a7c 016a  .|.j.|.j.|.j.|.j
-00001330: 0b64 019c 0c53 0029 027a 6e4d 616b 6520  .d...S.).znMake 
-00001340: 7468 6520 7061 7261 6d65 7465 7273 2064  the parameters d
-00001350: 6963 7469 6f6e 6172 7920 6966 2074 6865  ictionary if the
-00001360: 7920 6172 6520 7061 7373 6564 2061 7320  y are passed as 
-00001370: 6172 6775 6d65 6e74 730a 0a20 2020 2020  arguments..     
-00001380: 2020 203a 7061 7261 6d20 6172 6773 3a20     :param args: 
-00001390: 7061 7373 6564 2061 7267 756d 656e 7473  passed arguments
-000013a0: 0a20 2020 2020 2020 2072 3700 0000 290c  .        r7...).
-000013b0: da0a 7265 736f 6c75 7469 6f6e da11 7365  ..resolution..se
-000013c0: 7175 656e 6365 5f69 6465 6e74 6974 795a  quence_identityZ
-000013d0: 116d 6178 5f70 6462 5f74 656d 706c 6174  .max_pdb_templat
-000013e0: 6573 721f 0000 0072 2100 0000 7220 0000  esr....r!...r ..
-000013f0: 005a 0a72 6573 5f63 7574 6f66 665a 0c6d  .Z.res_cutoffZ.m
-00001400: 6178 5f6d 6f64 656c 5f77 745a 0d6d 6178  ax_model_wtZ.max
-00001410: 5f6d 6f64 656c 5f6d 7574 5a08 775f 7374  _model_mutZ.w_st
-00001420: 7275 6374 5a05 775f 6d75 74da 0d6d 6f64  ructZ.w_mut..mod
-00001430: 656c 6c65 725f 6578 6563 7223 0000 0072  eller_execr#...r
-00001440: 0e00 0000 720e 0000 0072 0f00 0000 da10  ....r....r......
-00001450: 6d65 7267 655f 7061 7261 6d65 7465 7273  merge_parameters
-00001460: e600 0000 731a 0000 0000 0604 0104 0104  ....s...........
-00001470: 0104 0104 0104 0104 0104 0104 0104 0104  ................
-00001480: 0104 f47a 1c49 6e70 7574 5061 7273 6572  ...z.InputParser
-00001490: 2e6d 6572 6765 5f70 6172 616d 6574 6572  .merge_parameter
-000014a0: 7329 0372 0a00 0000 da0a 7061 7261 6d65  s).r......parame
-000014b0: 7465 7273 7210 0000 0063 0300 0000 0000  tersr....c......
-000014c0: 0000 0000 0000 0400 0000 1d00 0000 4300  ..............C.
-000014d0: 0000 7398 0000 0064 017c 0264 0219 009b  ..s....d.|.d....
-000014e0: 0064 037c 0264 0419 009b 0064 057c 0264  .d.|.d.....d.|.d
-000014f0: 0619 009b 0064 077c 0264 0819 009b 0064  .....d.|.d.....d
-00001500: 097c 0264 0a19 009b 0064 0b7c 0264 0c19  .|.d.....d.|.d..
-00001510: 009b 0064 0d7c 016a 009b 0064 0e7c 016a  ...d.|.j...d.|.j
-00001520: 019b 0064 0f7c 0264 1019 009b 0064 117c  ...d.|.d.....d.|
-00001530: 0264 1219 009b 0064 137c 0264 1419 009b  .d.....d.|.d....
-00001540: 0064 157c 0264 1619 009b 0064 177c 0264  .d.|.d.....d.|.d
-00001550: 1819 009b 0064 197c 0264 1a19 009b 009d  .....d.|.d......
-00001560: 1c7d 0374 027c 0383 0101 0064 1b53 0029  .}.t.|.....d.S.)
-00001570: 1c7a 5650 7269 6e74 2074 6865 2070 6172  .zVPrint the par
-00001580: 616d 6574 6572 7320 7072 6f76 6964 6564  ameters provided
-00001590: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000015a0: 2070 6172 616d 6574 6572 733a 2050 726f   parameters: Pro
-000015b0: 7669 6465 6420 7061 7261 6d65 7465 7273  vided parameters
-000015c0: 0a20 2020 2020 2020 207a 0d0a 5265 736f  .        z..Reso
-000015d0: 6c75 7469 6f6e 3a20 7238 0000 007a 090a  lution: r8...z..
-000015e0: 5345 5120 4944 3a20 7239 0000 007a 170a  SEQ ID: r9...z..
-000015f0: 5754 204d 4f44 454c 5320 544f 2050 5245  WT MODELS TO PRE
-00001600: 5041 5245 3a20 723f 0000 007a 1b0a 4d55  PARE: r?...z..MU
-00001610: 5441 4e54 5320 4d4f 4445 4c20 544f 2050  TANTS MODEL TO P
-00001620: 5245 5041 5245 3a20 7240 0000 007a 180a  REPARE: r@...z..
-00001630: 4d41 5820 5044 4253 2041 5320 5445 4d50  MAX PDBS AS TEMP
-00001640: 4c41 5445 533a 2072 3a00 0000 7a12 0a52  LATES: r:...z..R
-00001650: 4553 4944 5545 5320 4355 544f 4646 3a20  ESIDUES CUTOFF: 
-00001660: 723e 0000 007a 0d0a 494e 5055 5420 4649  r>...z..INPUT FI
-00001670: 4c45 3a20 7a13 0a4f 5554 5055 5420 4449  LE: z..OUTPUT DI
-00001680: 5245 4354 4f52 593a 207a 160a 4441 5441  RECTORY: z..DATA
-00001690: 4241 5345 5320 4449 5245 4354 4f52 593a  BASES DIRECTORY:
-000016a0: 2072 3b00 0000 7a09 0a43 4f42 414c 543a   r;...z..COBALT:
-000016b0: 2072 3d00 0000 7a08 0a48 4d4d 4552 3a20   r=...z..HMMER: 
-000016c0: 723c 0000 007a 1a0a 5745 4947 4854 2053  r<...z..WEIGHT S
-000016d0: 5452 5543 5455 5241 4c20 5343 4f52 453a  TRUCTURAL SCORE:
-000016e0: 2072 4100 0000 7a18 0a57 4549 4748 5420   rA...z..WEIGHT 
-000016f0: 4d55 5441 5449 4f4e 2053 434f 5245 3a20  MUTATION SCORE: 
-00001700: 7242 0000 007a 160a 4d4f 4445 4c4c 4552  rB...z..MODELLER
-00001710: 2045 5845 4355 5441 424c 453a 2072 4300   EXECUTABLE: rC.
-00001720: 0000 4e29 03da 0a69 6e70 7574 5f66 696c  ..N)...input_fil
-00001730: 65da 086f 7574 5f70 6174 68da 0570 7269  e..out_path..pri
-00001740: 6e74 2904 7209 0000 0072 0a00 0000 7255  nt).r....r....rU
-00001750: 0000 00da 0570 6172 616d 720e 0000 0072  .....paramr....r
-00001760: 0e00 0000 720f 0000 00da 1070 7269 6e74  ....r......print
-00001770: 5f70 6172 616d 6574 6572 73fa 0000 0073  _parameters....s
-00001780: 3a00 0000 0008 0c01 06ff 0402 06fe 0403  :...............
-00001790: 06fd 0404 06fc 0405 06fb 0406 04fa 0407  ................
-000017a0: 04f9 0408 06f8 0409 06f7 040a 06f6 040b  ................
-000017b0: 06f5 040c 06f4 040d 06f3 04ff 0211 7a1c  ..............z.
-000017c0: 496e 7075 7450 6172 7365 722e 7072 696e  InputParser.prin
-000017d0: 745f 7061 7261 6d65 7465 7273 6302 0000  t_parametersc...
-000017e0: 0000 0000 0000 0000 0005 0000 0004 0000  ................
-000017f0: 0043 0000 0073 4a00 0000 7c00 a000 7c01  .C...sJ...|...|.
-00001800: a101 5c02 7d02 7d03 7c00 a001 7c02 a101  ..\.}.}.|...|...
-00001810: 0100 7c02 6a02 722c 7c00 a003 7c02 6a02  ..|.j.r,|...|.j.
-00001820: a101 7d04 6e0a 7c00 a004 7c02 a101 7d04  ..}.n.|...|...}.
-00001830: 7c00 a005 7c02 7c04 a102 0100 7c02 7c04  |...|.|.....|.|.
-00001840: 6602 5300 2901 7a70 4c6f 6164 2075 7365  f.S.).zpLoad use
-00001850: 7220 696e 7075 7420 6672 6f6d 2074 6865  r input from the
-00001860: 2063 6f6d 6d61 6e64 206c 696e 6520 616e   command line an
-00001870: 6420 7061 7261 6d65 7465 7273 2066 696c  d parameters fil
-00001880: 652e 0a0a 2020 2020 2020 2020 3a70 6172  e...        :par
-00001890: 616d 2061 7267 763a 2063 6f6d 6d61 6e64  am argv: command
-000018a0: 206c 696e 6520 6172 6775 6d65 6e74 730a   line arguments.
-000018b0: 2020 2020 2020 2020 2906 5a10 7061 7273          ).Z.pars
-000018c0: 655f 6b6e 6f77 6e5f 6172 6773 7224 0000  e_known_argsr$..
-000018d0: 0072 1e00 0000 7250 0000 0072 5400 0000  .r....rP...rT...
-000018e0: 725a 0000 0029 0572 0900 0000 da04 6172  rZ...).r......ar
-000018f0: 6776 720a 0000 005a 0875 6e70 6172 7365  gvr....Z.unparse
-00001900: 6472 5500 0000 720e 0000 0072 0e00 0000  drU...r....r....
-00001910: 720f 0000 00da 0a6c 6f61 645f 696e 7075  r......load_inpu
-00001920: 7414 0100 0073 0e00 0000 0005 0e01 0a01  t....s..........
-00001930: 0601 0e02 0a01 0c02 7a16 496e 7075 7450  ........z.InputP
-00001940: 6172 7365 722e 6c6f 6164 5f69 6e70 7574  arser.load_input
-00001950: 2901 7235 0000 0029 11da 085f 5f6e 616d  ).r5...)...__nam
-00001960: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00001970: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0700  .__qualname__r..
-00001980: 0000 7208 0000 00da 0861 7267 7061 7273  ..r......argpars
-00001990: 655a 094e 616d 6573 7061 6365 7224 0000  eZ.Namespacer$..
-000019a0: 0072 0400 0000 7234 0000 0072 0300 0000  .r....r4...r....
-000019b0: 7250 0000 0072 5400 0000 725a 0000 00da  rP...rT...rZ....
-000019c0: 0574 7570 6c65 725c 0000 00da 0d5f 5f63  .tupler\.....__c
-000019d0: 6c61 7373 6365 6c6c 5f5f 720e 0000 0072  lasscell__r....r
-000019e0: 0e00 0000 720c 0000 0072 0f00 0000 7205  ....r....r....r.
-000019f0: 0000 0006 0000 0073 1e00 0000 0801 0c04  .......s........
-00001a00: 127f 0009 1214 1217 00fe 0202 0401 02fd  ................
-00001a10: 0c2a 1215 0601 02fe 0c1a 7205 0000 0029  .*........r....)
-00001a20: 0872 6000 0000 da07 7061 7468 6c69 6272  .r`.....pathlibr
-00001a30: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
-00001a40: 0072 0400 0000 da0e 4172 6775 6d65 6e74  .r......Argument
-00001a50: 5061 7273 6572 7205 0000 0072 0e00 0000  Parserr....r....
-00001a60: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
-00001a70: 083c 6d6f 6475 6c65 3e01 0000 0073 0600  .<module>....s..
-00001a80: 0000 0801 0c01 1003                      ........
+00000110: 8404 5a0c 6413 6414 8400 5a0d 6505 6a06  ..Z.d.d...Z.e.j.
+00000120: 650a 6403 6415 9c03 6416 6417 8404 5a0e  e.d.d...d.d...Z.
+00000130: 650f 6404 9c01 6418 6419 8404 5a10 8700  e.d...d.d...Z...
+00000140: 0400 5a11 5300 291b da0b 496e 7075 7450  ..Z.S.)...InputP
+00000150: 6172 7365 7263 0100 0000 0000 0000 0000  arserc..........
+00000160: 0000 0300 0000 0400 0000 0f00 0000 731e  ..............s.
+00000170: 0000 0074 0083 006a 017c 0169 007c 02a4  ...t...j.|.i.|..
+00000180: 018e 0101 007c 00a0 02a1 0001 0064 0053  .....|.......d.S
+00000190: 0029 014e 2903 da05 7375 7065 72da 085f  .).N)...super.._
+000001a0: 5f69 6e69 745f 5fda 0d61 6464 5f61 7267  _init__..add_arg
+000001b0: 756d 656e 7473 2903 da04 7365 6c66 da04  uments)...self..
+000001c0: 6172 6773 da06 6b77 6172 6773 a901 da09  args..kwargs....
+000001d0: 5f5f 636c 6173 735f 5fa9 00fa 552f 5573  __class__...U/Us
+000001e0: 6572 732f 616c 6261 6e69 2f57 6f72 6b2f  ers/albani/Work/
+000001f0: 5072 6f6a 6563 7473 2f4d 6f6e 7669 736f  Projects/Monviso
+00000200: 2f6d 6f6e 7669 736f 5f72 656c 6f61 6465  /monviso_reloade
+00000210: 642f 6d6f 6e76 6973 6f5f 7265 6c6f 6164  d/monviso_reload
+00000220: 6564 2f69 6e70 7574 5f70 6172 7365 722e  ed/input_parser.
+00000230: 7079 7207 0000 0007 0000 0073 0400 0000  pyr........s....
+00000240: 0001 1201 7a14 496e 7075 7450 6172 7365  ....z.InputParse
+00000250: 722e 5f5f 696e 6974 5f5f 4e29 01da 0672  r.__init__N)...r
+00000260: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
+00000270: 0000 0200 0000 0800 0000 0300 0000 7372  ..............sr
+00000280: 0100 0074 0083 006a 0164 0164 0264 0374  ...t...j.d.d.d.t
+00000290: 0264 0464 058d 0501 0074 0083 006a 0164  .d.d.....t...j.d
+000002a0: 0664 0764 0874 0264 0464 058d 0501 0074  .d.d.t.d.d.....t
+000002b0: 0083 006a 0164 0964 0a64 0b74 0264 0c64  ...j.d.d.d.t.d.d
+000002c0: 058d 0501 0074 0083 006a 0164 0d64 0e64  .....t...j.d.d.d
+000002d0: 0f74 0264 0c64 058d 0501 0074 0083 006a  .t.d.d.....t...j
+000002e0: 0164 1064 1164 1274 0264 0c64 058d 0501  .d.d.d.t.d.d....
+000002f0: 0074 0083 006a 0164 1364 1464 1574 0264  .t...j.d.d.d.t.d
+00000300: 0c64 058d 0501 0074 0083 006a 0164 1664  .d.....t...j.d.d
+00000310: 1764 1874 0264 0c64 058d 0501 0074 0083  .d.t.d.d.....t..
+00000320: 00a0 0364 1964 1aa1 027d 017c 016a 0164  ...d.d...}.|.j.d
+00000330: 1b64 1c64 1d74 0464 1e64 0c64 1f8d 0601  .d.d.t.d.d.d....
+00000340: 007c 016a 0164 2064 2164 2274 0464 2364  .|.j.d d!d"t.d#d
+00000350: 0c64 1f8d 0601 007c 016a 0164 2464 2564  .d.....|.j.d$d%d
+00000360: 2674 0564 2764 0c64 1f8d 0601 007c 016a  &t.d'd.d.....|.j
+00000370: 0164 2864 2964 2a74 0564 2b64 0c64 1f8d  .d(d)d*t.d+d.d..
+00000380: 0601 007c 016a 0164 2c64 2d64 2e74 0564  ...|.j.d,d-d.t.d
+00000390: 2b64 0c64 1f8d 0601 007c 016a 0164 2f64  +d.d.....|.j.d/d
+000003a0: 3064 3174 0464 3264 0c64 1f8d 0601 007c  0d1t.d2d.d.....|
+000003b0: 016a 0164 3364 3464 3574 0464 3664 0c64  .j.d3d4d5t.d6d.d
+000003c0: 1f8d 0601 007c 016a 0164 3764 3864 3974  .....|.j.d7d8d9t
+000003d0: 0464 3664 0c64 1f8d 0601 007c 016a 0164  .d6d.d.....|.j.d
+000003e0: 3a64 3b64 3c74 0264 3d64 0c64 1f8d 0601  :d;d<t.d=d.d....
+000003f0: 0064 3e53 0029 3f7a 5841 6464 2061 206c  .d>S.)?zXAdd a l
+00000400: 6973 7420 6f66 2065 7870 6563 7465 6420  ist of expected 
+00000410: 6172 6775 6d65 6e74 7320 746f 2074 6865  arguments to the
+00000420: 2050 6172 7365 7220 696e 7374 616e 6365   Parser instance
+00000430: 2e0a 0a20 2020 2020 2020 203a 7265 7475  ...        :retu
+00000440: 726e 3a20 4e6f 6e65 0a20 2020 2020 2020  rn: None.       
+00000450: 207a 022d 697a 0c2d 2d69 6e70 7574 5f66   z.-iz.--input_f
+00000460: 696c 657a 2450 6174 6820 746f 2074 6865  ilez$Path to the
+00000470: 2066 696c 6520 6765 6e65 7320 616e 6420   file genes and 
+00000480: 6d75 7461 7469 6f6e 7354 2903 da04 6865  mutationsT)...he
+00000490: 6c70 da04 7479 7065 da08 7265 7175 6972  lp..type..requir
+000004a0: 6564 7a02 2d6f 7a0a 2d2d 6f75 745f 7061  edz.-oz.--out_pa
+000004b0: 7468 7a19 5061 7468 2074 6f20 7468 6520  thz.Path to the 
+000004c0: 6f75 7470 7574 2066 6f6c 6465 727a 032d  output folderz.-
+000004d0: 7066 7a0a 2d2d 7061 725f 6669 6c65 7a25  pfz.--par_filez%
+000004e0: 496e 7075 7420 7468 6520 7061 7468 2074  Input the path t
+000004f0: 6f20 7468 6520 7061 7261 6d65 7465 7273  o the parameters
+00000500: 2066 696c 6546 7a04 2d70 7374 7a0c 2d2d   fileFz.-pstz.--
+00000510: 7065 7374 6f5f 686f 6d65 7a55 7061 7468  pesto_homezUpath
+00000520: 2074 6f20 7468 6520 6469 7265 6374 6f72   to the director
+00000530: 7920 636f 6e74 6169 6e69 6e67 2074 6865  y containing the
+00000540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000550: 5065 5374 6f20 7265 706f 2064 6f77 6e6c  PeSto repo downl
+00000560: 6f61 6465 6420 6672 6f6d 2047 6974 4875  oaded from GitHu
+00000570: 627a 032d 6462 7a09 2d2d 6462 5f68 6f6d  bz.-dbz.--db_hom
+00000580: 657a 4d70 6174 6820 746f 2074 6865 2044  ezMpath to the D
+00000590: 4273 2063 6f6e 7461 696e 696e 6720 7468  Bs containing th
+000005a0: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+000005b0: 2063 616e 6f6e 6963 616c 2061 6e64 2069   canonical and i
+000005c0: 736f 666f 726d 2073 6571 7565 6e63 6573  soform sequences
+000005d0: 7a07 2d63 6f62 616c 747a 0d2d 2d63 6f62  z.-cobaltz.--cob
+000005e0: 616c 745f 686f 6d65 7a19 7061 7468 2074  alt_homez.path t
+000005f0: 6f20 434f 4241 4c54 2062 696e 2066 6f6c  o COBALT bin fol
+00000600: 6465 727a 062d 686d 6d65 727a 0c2d 2d68  derz.-hmmerz.--h
+00000610: 6d6d 6572 5f68 6f6d 657a 1870 6174 6820  mmer_homez.path 
+00000620: 746f 2048 4d4d 4552 2062 696e 2066 6f6c  to HMMER bin fol
+00000630: 6465 72da 0569 6e70 7574 7a1c 6d61 6e75  der..inputz.manu
+00000640: 616c 6c79 2070 726f 7669 6465 7320 7468  ally provides th
+00000650: 6520 696e 7075 7473 7a04 2d72 6573 7a0c  e inputsz.-resz.
+00000660: 2d2d 7265 736f 6c75 7469 6f6e 7a19 776f  --resolutionz.wo
+00000670: 7273 7420 6163 6365 7074 6564 2072 6573  rst accepted res
+00000680: 6f6c 7574 696f 6e67 0000 0000 0000 1240  olutiong.......@
+00000690: 2904 7211 0000 0072 1200 0000 da07 6465  ).r....r......de
+000006a0: 6661 756c 7472 1300 0000 7a06 2d73 6571  faultr....z.-seq
+000006b0: 6964 7a13 2d2d 7365 7175 656e 6365 5f69  idz.--sequence_i
+000006c0: 6465 6e74 6974 797a 226d 696e 696d 756d  dentityz"minimum
+000006d0: 2073 6571 7565 6e63 6520 6964 656e 7469   sequence identi
+000006e0: 7479 2061 6363 6570 7465 64e9 1900 0000  ty accepted.....
+000006f0: 7a08 2d6d 6178 5f70 6462 7a13 2d2d 6d61  z.-max_pdbz.--ma
+00000700: 785f 7064 625f 7465 6d70 6c61 7465 737a  x_pdb_templatesz
+00000710: 2a6d 6178 696d 756d 206e 756d 6265 7220  *maximum number 
+00000720: 6f66 2050 4442 7320 746f 2075 7365 2061  of PDBs to use a
+00000730: 7320 7465 6d70 6c61 7465 73e9 0a00 0000  s templates.....
+00000740: 7a07 2d77 745f 6d6f 647a 0e2d 2d6d 6178  z.-wt_modz.--max
+00000750: 5f6d 6f64 656c 5f77 747a 2b6d 6178 696d  _model_wtz+maxim
+00000760: 756d 206e 756d 6265 7220 6f66 2077 696c  um number of wil
+00000770: 642d 7479 7065 206d 6f64 656c 7320 746f  d-type models to
+00000780: 2062 7569 6c64 e901 0000 007a 082d 6d75   build.....z.-mu
+00000790: 745f 6d6f 647a 0f2d 2d6d 6178 5f6d 6f64  t_modz.--max_mod
+000007a0: 656c 5f6d 7574 7a28 6d61 7869 6d75 6d20  el_mutz(maximum 
+000007b0: 6e75 6d62 6572 206f 6620 6d75 7461 6e74  number of mutant
+000007c0: 206d 6f64 656c 7320 746f 2062 7569 6c64   models to build
+000007d0: 7a03 2d72 637a 0c2d 2d72 6573 5f63 7574  z.-rcz.--res_cut
+000007e0: 6f66 667a 596d 6178 696d 756d 206e 756d  offzYmaximum num
+000007f0: 6265 7220 6f66 206e 6f74 2063 7279 7374  ber of not cryst
+00000800: 616c 6973 6564 2072 6573 6964 7565 7320  alised residues 
+00000810: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00000820: 6363 6570 7465 6420 6265 666f 7265 2063  ccepted before c
+00000830: 7574 7469 6e67 2061 206d 6f64 656c 6700  utting a modelg.
+00000840: 0000 0000 0014 407a 032d 7773 7a0a 2d2d  ......@z.-wsz.--
+00000850: 775f 7374 7275 6374 7a21 7765 6967 6874  w_structz!weight
+00000860: 206f 6620 7468 6520 7374 7275 6374 7572   of the structur
+00000870: 616c 2066 756e 6374 696f 6e67 0000 0000  al functiong....
+00000880: 0000 2440 7a03 2d77 6d7a 072d 2d77 5f6d  ..$@z.-wmz.--w_m
+00000890: 7574 7a1f 7765 6967 6874 206f 6620 7468  utz.weight of th
+000008a0: 6520 6d75 7461 7469 6f6e 2066 756e 6374  e mutation funct
+000008b0: 696f 6e7a 042d 6d6f 647a 0f2d 2d6d 6f64  ionz.-modz.--mod
+000008c0: 656c 6c65 725f 6578 6563 7a1f 7061 7468  eller_execz.path
+000008d0: 2074 6f20 7468 6520 6d6f 6465 6c6c 6572   to the modeller
+000008e0: 2065 7865 6375 7461 626c 657a 076d 6f64   executablez.mod
+000008f0: 3130 2e34 4e29 0672 0600 0000 da0c 6164  10.4N).r......ad
+00000900: 645f 6172 6775 6d65 6e74 da03 7374 72da  d_argument..str.
+00000910: 1261 6464 5f61 7267 756d 656e 745f 6772  .add_argument_gr
+00000920: 6f75 70da 0566 6c6f 6174 da03 696e 7429  oup..float..int)
+00000930: 0272 0900 0000 5a10 7061 7261 6d65 7465  .r....Z.paramete
+00000940: 7273 5f67 726f 7570 720c 0000 0072 0e00  rs_groupr....r..
+00000950: 0000 720f 0000 0072 0800 0000 0b00 0000  ..r....r........
+00000960: 73f8 0000 0000 0506 0102 0102 0102 0102  s...............
+00000970: 0102 fb06 0806 0102 0102 0102 0102 0102  ................
+00000980: fb06 0806 0102 0102 0102 0102 0102 fb06  ................
+00000990: 0806 0102 0102 0102 0202 0102 fa06 0906  ................
+000009a0: 0102 0102 0102 0202 0102 fa06 0906 0102  ................
+000009b0: 0102 0102 0102 0102 fb06 0806 0102 0102  ................
+000009c0: 0102 0102 0102 fb06 0806 0104 ff04 0304  ................
+000009d0: 0102 0102 0102 0102 0102 0102 fa06 0804  ................
+000009e0: 0102 0102 0102 0102 0102 0102 fa06 0804  ................
+000009f0: 0102 0102 0102 0102 0102 0102 fa06 0904  ................
+00000a00: 0102 0102 0102 0102 0102 0102 fa06 0904  ................
+00000a10: 0102 0102 0102 0102 0102 0102 fa06 0904  ................
+00000a20: 0102 0102 0102 0202 0102 0102 f906 0a04  ................
+00000a30: 0102 0102 0102 0102 0102 0102 fa06 0904  ................
+00000a40: 0102 0102 0102 0102 0102 0102 fa06 0904  ................
+00000a50: 0102 0102 0102 0102 0102 0102 fa7a 1949  .............z.I
+00000a60: 6e70 7574 5061 7273 6572 2e61 6464 5f61  nputParser.add_a
+00000a70: 7267 756d 656e 7473 2902 720a 0000 0072  rguments).r....r
+00000a80: 1000 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00000a90: 0002 0000 0002 0000 0043 0000 0073 4c00  .........C...sL.
+00000aa0: 0000 7c01 6a00 7328 7c01 6a01 721e 7c01  ..|.j.s(|.j.r.|.
+00000ab0: 6a02 721e 7c01 6a03 721e 7c01 6a04 7328  j.r.|.j.r.|.j.s(
+00000ac0: 7405 6401 8301 8201 6e20 7c01 6a00 7248  t.d.....n |.j.rH
+00000ad0: 7c01 6a01 7340 7c01 6a02 7340 7c01 6a03  |.j.s@|.j.s@|.j.
+00000ae0: 7248 7405 6402 8301 8201 6403 5300 2904  rHt.d.....d.S.).
+00000af0: 7a67 5665 7269 6679 2074 6861 7420 7468  zgVerify that th
+00000b00: 6520 6e65 6365 7373 6172 7920 7061 7261  e necessary para
+00000b10: 6d65 7465 7273 2068 6176 6520 6265 656e  meters have been
+00000b20: 2070 726f 7669 6465 640a 0a20 2020 2020   provided..     
+00000b30: 2020 203a 7061 7261 6d20 6172 6773 3a20     :param args: 
+00000b40: 7061 7373 6564 2061 7267 756d 656e 7473  passed arguments
+00000b50: 0a20 2020 2020 2020 207a 6d53 7065 6369  .        zmSpeci
+00000b60: 6679 2061 2070 6172 616d 6574 6572 7320  fy a parameters 
+00000b70: 6669 6c65 206f 7220 696e 7365 7274 2074  file or insert t
+00000b80: 6865 2070 6174 6873 2020 2020 2020 2020  he paths        
+00000b90: 2020 2020 2020 2020 2020 2020 746f 2074              to t
+00000ba0: 6865 2044 4273 2c20 434f 4241 4c54 2c20  he DBs, COBALT, 
+00000bb0: 5045 5354 4f20 616e 6420 484d 4d45 5220  PESTO and HMMER 
+00000bc0: 6d61 6e75 616c 6c79 7a51 4569 7468 6572  manuallyzQEither
+00000bd0: 2073 7065 6369 6679 2061 2070 6172 616d   specify a param
+00000be0: 6574 6572 7320 6669 6c65 206f 7220 2020  eters file or   
+00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c00: 2069 6e73 6572 7420 7061 7261 6d65 7465   insert paramete
+00000c10: 7273 206d 616e 7561 6c6c 794e 2906 da08  rs manuallyN)...
+00000c20: 7061 725f 6669 6c65 da07 6462 5f68 6f6d  par_file..db_hom
+00000c30: 65da 0b63 6f62 616c 745f 686f 6d65 da0a  e..cobalt_home..
+00000c40: 686d 6d65 725f 686f 6d65 da0a 7065 7374  hmmer_home..pest
+00000c50: 6f5f 686f 6d65 da09 5479 7065 4572 726f  o_home..TypeErro
+00000c60: 72a9 0272 0900 0000 720a 0000 0072 0e00  r..r....r....r..
+00000c70: 0000 720e 0000 0072 0f00 0000 da0f 6368  ..r....r......ch
+00000c80: 6563 6b5f 6172 6775 6d65 6e74 739d 0000  eck_arguments...
+00000c90: 0073 2400 0000 0005 1201 04ff 0202 04fe  .s$.............
+00000ca0: 0203 0201 02ff 0604 0601 04ff 0201 04ff  ................
+00000cb0: 0201 04ff 0203 0201 02ff 7a1b 496e 7075  ..........z.Inpu
+00000cc0: 7450 6172 7365 722e 6368 6563 6b5f 6172  tParser.check_ar
+00000cd0: 6775 6d65 6e74 7329 02da 126d 7574 6174  guments)...mutat
+00000ce0: 696f 6e5f 6669 6c65 5f70 6174 6872 1000  ion_file_pathr..
+00000cf0: 0000 6302 0000 0000 0000 0000 0000 0005  ..c.............
+00000d00: 0000 0008 0000 0043 0000 0073 7c00 0000  .......C...s|...
+00000d10: 7400 7c01 8301 a001 a100 8f18 7d02 7c02  t.|.........}.|.
+00000d20: a002 a100 7d03 5700 6401 0400 0400 8303  ....}.W.d.......
+00000d30: 0100 6e10 3100 732a 3000 0100 0100 0100  ..n.1.s*0.......
+00000d40: 5900 0100 7c03 6402 1900 6403 6b02 724e  Y...|.d...d.k.rN
+00000d50: 7c03 6401 6402 8502 1900 7d03 7134 6404  |.d.d.....}.q4d.
+00000d60: 7c03 7600 7264 7c03 a003 6404 6405 a102  |.v.rd|...d.d...
+00000d70: 7d03 714e 6406 6407 8400 7c03 a004 6405  }.qNd.d...|...d.
+00000d80: a101 4400 8301 7d04 7c04 5300 2908 7ade  ..D...}.|.S.).z.
+00000d90: 5061 7273 6520 7468 6520 6c69 7374 206f  Parse the list o
+00000da0: 6620 6d75 7461 7469 6f6e 7320 616e 6420  f mutations and 
+00000db0: 6765 6e65 7320 6672 6f6d 2074 6865 206d  genes from the m
+00000dc0: 7574 6174 696f 6e5f 6c69 7374 2066 696c  utation_list fil
+00000dd0: 652e 0a0a 2020 2020 2020 2020 3a70 6172  e...        :par
+00000de0: 616d 206d 7574 6174 696f 6e5f 6c69 7374  am mutation_list
+00000df0: 3a20 7061 7468 2074 6f20 7468 6520 6669  : path to the fi
+00000e00: 6c65 2063 6f6e 7461 696e 696e 6720 7468  le containing th
+00000e10: 6520 6c69 7374 0a20 2020 2020 2020 206f  e list.        o
+00000e20: 6620 6d75 7461 7469 6f6e 7320 616e 6420  f mutations and 
+00000e30: 6765 6e65 730a 2020 2020 2020 2020 3a72  genes.        :r
+00000e40: 6574 7572 6e3a 2054 6865 206c 6973 7420  eturn: The list 
+00000e50: 6f66 2067 656e 6520 616e 6420 6d75 7461  of gene and muta
+00000e60: 7469 6f6e 730a 2020 2020 2020 2020 4ee9  tions.        N.
+00000e70: ffff ffff da01 0a7a 030a 0a0a 7a02 0a0a  .......z....z...
+00000e80: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000e90: 0004 0000 0053 0000 0073 1400 0000 6700  .....S...s....g.
+00000ea0: 7c00 5d0c 7d01 7c01 a000 a100 9102 7104  |.].}.|.......q.
+00000eb0: 5300 720e 0000 0029 01da 0a73 706c 6974  S.r....)...split
+00000ec0: 6c69 6e65 7329 02da 022e 30da 0562 6c6f  lines)....0..blo
+00000ed0: 636b 720e 0000 0072 0e00 0000 720f 0000  ckr....r....r...
+00000ee0: 00da 0a3c 6c69 7374 636f 6d70 3ec3 0000  ...<listcomp>...
+00000ef0: 00f3 0000 0000 7a2b 496e 7075 7450 6172  ......z+InputPar
+00000f00: 7365 722e 7061 7273 655f 696e 7075 742e  ser.parse_input.
+00000f10: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00000f20: 6d70 3e29 0572 0200 0000 da04 6f70 656e  mp>).r......open
+00000f30: da04 7265 6164 da07 7265 706c 6163 65da  ..read..replace.
+00000f40: 0573 706c 6974 2905 7209 0000 0072 2600  .split).r....r&.
+00000f50: 0000 da07 6d79 5f66 696c 65da 0763 6f6e  ....my_file..con
+00000f60: 7465 6e74 da06 626c 6f63 6b73 720e 0000  tent..blocksr...
+00000f70: 0072 0e00 0000 720f 0000 00da 0b70 6172  .r....r......par
+00000f80: 7365 5f69 6e70 7574 b100 0000 7310 0000  se_input....s...
+00000f90: 0000 070e 0126 040c 010e 0208 010e 0214  .....&..........
+00000fa0: 017a 1749 6e70 7574 5061 7273 6572 2e70  .z.InputParser.p
+00000fb0: 6172 7365 5f69 6e70 7574 fa0e 7061 7261  arse_input..para
+00000fc0: 6d65 7465 7273 2e64 6174 2902 da0f 7061  meters.dat)...pa
+00000fd0: 7261 6d65 7465 7273 5f70 6174 6872 1000  rameters_pathr..
+00000fe0: 0000 6302 0000 0000 0000 0000 0000 000a  ..c.............
+00000ff0: 0000 0010 0000 0043 0000 0073 c200 0000  .......C...s....
+00001000: 6401 6401 6401 6401 6401 6401 6401 6401  d.d.d.d.d.d.d.d.
+00001010: 6401 6401 6401 6401 6401 6401 6401 6402  d.d.d.d.d.d.d.d.
+00001020: 9c0f 7d02 7400 7c02 8301 7d03 7401 7c01  ..}.t.|...}.t.|.
+00001030: 8301 a002 a100 734c 6403 7c01 9b00 6404  ......sLd.|...d.
+00001040: 9d03 7d04 7403 7c04 8301 8201 7401 7c01  ..}.t.|.....t.|.
+00001050: 8301 a004 a100 8f18 7d05 7c05 a005 a100  ........}.|.....
+00001060: 7d06 5700 6401 0400 0400 8303 0100 6e10  }.W.d.........n.
+00001070: 3100 7376 3000 0100 0100 0100 5900 0100  1.sv0.......Y...
+00001080: 7c03 4400 5d38 7d07 7c06 4400 5d2e 7d08  |.D.]8}.|.D.].}.
+00001090: 7c07 7c08 7600 728c 7c08 7c08 a006 6405  |.|.v.r.|.|...d.
+000010a0: a101 6406 1700 6401 8502 1900 a007 a100  ..d...d.........
+000010b0: 7d09 7c09 7c02 7c07 3c00 718c 7184 7c02  }.|.|.|.<.q.q.|.
+000010c0: 5300 2907 7aeb 436f 6c6c 6563 7420 7468  S.).z.Collect th
+000010d0: 6520 7061 7261 6d65 7465 7273 2066 726f  e parameters fro
+000010e0: 6d20 7468 6520 7061 7261 6d65 7465 7273  m the parameters
+000010f0: 2066 696c 6520 6966 2070 726f 7669 6465   file if provide
+00001100: 642e 0a0a 2020 2020 2020 2020 3a70 6172  d...        :par
+00001110: 616d 2070 6172 616d 6574 6572 735f 7061  am parameters_pa
+00001120: 7468 3a20 5061 7468 2074 6f20 7468 6520  th: Path to the 
+00001130: 7061 7261 6d65 7465 7273 2066 696c 652c  parameters file,
+00001140: 0a20 2020 2020 2020 2064 6566 6175 6c74  .        default
+00001150: 7320 746f 2022 7061 7261 6d65 7465 7273  s to "parameters
+00001160: 2e64 6174 222e 0a0a 2020 2020 2020 2020  .dat"...        
+00001170: 3a72 6574 7572 6e3a 2044 6963 7420 6f66  :return: Dict of
+00001180: 206b 6579 776f 7264 7320 7769 7468 2074   keywords with t
+00001190: 6865 2061 7373 6f63 6961 7465 6420 7061  he associated pa
+000011a0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+000011b0: 204e a90f da0a 5245 534f 4c55 5449 4f4e   N....RESOLUTION
+000011c0: da05 5345 5149 44da 0a50 4442 5f54 4f5f  ..SEQID..PDB_TO_
+000011d0: 5553 45da 0a50 4553 544f 5f48 4f4d 45da  USE..PESTO_HOME.
+000011e0: 0a49 4e50 5554 5f46 494c 45da 0b4f 5554  .INPUT_FILE..OUT
+000011f0: 5055 545f 5041 5448 da0b 4442 5f4c 4f43  PUT_PATH..DB_LOC
+00001200: 4154 494f 4eda 0a48 4d4d 4552 5f48 4f4d  ATION..HMMER_HOM
+00001210: 45da 0b43 4f42 414c 545f 484f 4d45 da0c  E..COBALT_HOME..
+00001220: 4d4f 4445 4c5f 4355 544f 4646 da0d 4e55  MODEL_CUTOFF..NU
+00001230: 4d5f 4f46 5f4d 4f44 5f57 54da 0e4e 554d  M_OF_MOD_WT..NUM
+00001240: 5f4f 465f 4d4f 445f 4d55 54da 0857 5f53  _OF_MOD_MUT..W_S
+00001250: 5452 5543 54da 0557 5f4d 5554 da0d 4d4f  TRUCT..W_MUT..MO
+00001260: 4445 4c4c 4552 5f45 5845 437a 1d50 6172  DELLER_EXECz.Par
+00001270: 616d 6574 6572 7320 6669 6c65 206e 6f74  ameters file not
+00001280: 2066 6f75 6e64 2069 6e20 7a30 2c20 2020   found in z0,   
+00001290: 2020 2020 2020 2020 2020 2020 2070 6c65               ple
+000012a0: 6173 6520 6368 6563 6b20 7468 6520 7061  ase check the pa
+000012b0: 7468 2070 726f 7669 6465 642e fa01 3d72  th provided...=r
+000012c0: 1800 0000 2908 da04 6c69 7374 7202 0000  ....)...listr...
+000012d0: 00da 0665 7869 7374 7372 2300 0000 722e  ...existsr#...r.
+000012e0: 0000 00da 0972 6561 646c 696e 6573 da04  .....readlines..
+000012f0: 6669 6e64 da05 7374 7269 7029 0a72 0900  find..strip).r..
+00001300: 0000 7237 0000 00da 086b 6579 776f 7264  ..r7.....keyword
+00001310: 73da 046b 6579 735a 0d65 7272 6f72 5f6d  s..keysZ.error_m
+00001320: 6573 7361 6765 7232 0000 00da 056c 696e  essager2.....lin
+00001330: 6573 da03 6b65 79da 046c 696e 65da 0576  es..key..line..v
+00001340: 616c 7565 720e 0000 0072 0e00 0000 720f  aluer....r....r.
+00001350: 0000 00da 0e67 6574 5f70 6172 616d 6574  .....get_paramet
+00001360: 6572 73c6 0000 0073 3800 0000 000c 0201  ers....s8.......
+00001370: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00001380: 0201 0201 0201 0201 0201 02f1 0611 0801  ................
+00001390: 0c02 0c02 0802 0e01 2602 0801 0801 0801  ........&.......
+000013a0: 1a01 0c01 7a1a 496e 7075 7450 6172 7365  ....z.InputParse
+000013b0: 722e 6765 745f 7061 7261 6d65 7465 7273  r.get_parameters
+000013c0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+000013d0: 0010 0000 0043 0000 0073 4200 0000 7c01  .....C...sB...|.
+000013e0: 6a00 7c01 6a01 7c01 6a02 7c01 6a03 7c01  j.|.j.|.j.|.j.|.
+000013f0: 6a04 7c01 6a05 7c01 6a06 7c01 6a07 7c01  j.|.j.|.j.|.j.|.
+00001400: 6a08 7c01 6a09 7c01 6a0a 7c01 6a0b 7c01  j.|.j.|.j.|.j.|.
+00001410: 6a0c 7c01 6a0d 7c01 6a0e 6401 9c0f 5300  j.|.j.|.j.d...S.
+00001420: 2902 7a6e 4d61 6b65 2074 6865 2070 6172  ).znMake the par
+00001430: 616d 6574 6572 7320 6469 6374 696f 6e61  ameters dictiona
+00001440: 7279 2069 6620 7468 6579 2061 7265 2070  ry if they are p
+00001450: 6173 7365 6420 6173 2061 7267 756d 656e  assed as argumen
+00001460: 7473 0a0a 2020 2020 2020 2020 3a70 6172  ts..        :par
+00001470: 616d 2061 7267 733a 2070 6173 7365 6420  am args: passed 
+00001480: 6172 6775 6d65 6e74 730a 2020 2020 2020  arguments.      
+00001490: 2020 290f 7239 0000 0072 3a00 0000 723b    ).r9...r:...r;
+000014a0: 0000 0072 3c00 0000 723e 0000 0072 3d00  ...r<...r>...r=.
+000014b0: 0000 723f 0000 0072 4000 0000 7241 0000  ..r?...r@...rA..
+000014c0: 0072 4200 0000 7243 0000 0072 4400 0000  .rB...rC...rD...
+000014d0: 7245 0000 0072 4600 0000 7247 0000 0029  rE...rF...rG...)
+000014e0: 0fda 0a72 6573 6f6c 7574 696f 6eda 1173  ...resolution..s
+000014f0: 6571 7565 6e63 655f 6964 656e 7469 7479  equence_identity
+00001500: da11 6d61 785f 7064 625f 7465 6d70 6c61  ..max_pdb_templa
+00001510: 7465 7372 2200 0000 da08 6f75 745f 7061  tesr".....out_pa
+00001520: 7468 da0a 696e 7075 745f 6669 6c65 721f  th..input_filer.
+00001530: 0000 0072 2100 0000 7220 0000 00da 0a72  ...r!...r .....r
+00001540: 6573 5f63 7574 6f66 66da 0c6d 6178 5f6d  es_cutoff..max_m
+00001550: 6f64 656c 5f77 74da 0d6d 6178 5f6d 6f64  odel_wt..max_mod
+00001560: 656c 5f6d 7574 da08 775f 7374 7275 6374  el_mut..w_struct
+00001570: da05 775f 6d75 74da 0d6d 6f64 656c 6c65  ..w_mut..modelle
+00001580: 725f 6578 6563 7224 0000 0072 0e00 0000  r_execr$...r....
+00001590: 720e 0000 0072 0f00 0000 da17 636f 6e76  r....r......conv
+000015a0: 6572 7441 7267 7354 6f50 6172 616d 6574  ertArgsToParamet
+000015b0: 6572 73f3 0000 0073 2000 0000 0007 0401  ers....s .......
+000015c0: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+000015d0: 0401 0401 0401 0401 0401 04f1 7a23 496e  ............z#In
+000015e0: 7075 7450 6172 7365 722e 636f 6e76 6572  putParser.conver
+000015f0: 7441 7267 7354 6f50 6172 616d 6574 6572  tArgsToParameter
+00001600: 7363 0300 0000 0000 0000 0000 0000 0700  sc..............
+00001610: 0000 0f00 0000 4300 0000 739c 0000 007c  ......C...s....|
+00001620: 016a 007c 016a 017c 016a 027c 016a 037c  .j.|.j.|.j.|.j.|
+00001630: 016a 047c 016a 057c 016a 067c 016a 077c  .j.|.j.|.j.|.j.|
+00001640: 016a 087c 016a 097c 016a 0a7c 016a 0b7c  .j.|.j.|.j.|.j.|
+00001650: 016a 0c7c 016a 0d7c 016a 0e67 0f7d 0367  .j.|.j.|.j.g.}.g
+00001660: 0064 01a2 017d 0474 0f7c 0283 0144 005d  .d...}.t.|...D.]
+00001670: 465c 027d 057d 067c 027c 0619 0064 0275  F\.}.}.|.|...d.u
+00001680: 0072 507a 107c 037c 0519 007c 027c 063c  .rPz.|.|...|.|.<
+00001690: 0057 0071 5001 0001 0001 0074 1064 037c  .W.qP......t.d.|
+000016a0: 047c 0519 009b 0064 049d 0383 0182 0159  .|.....d.......Y
+000016b0: 0071 5030 0071 5064 0253 0029 057a ae4d  .qP0.qPd.S.).z.M
+000016c0: 6572 6765 7320 6172 6773 2061 6e64 2070  erges args and p
+000016d0: 6172 616d 6574 6572 732c 2077 6974 6820  arameters, with 
+000016e0: 6120 7072 6566 6572 656e 6365 2066 6f72  a preference for
+000016f0: 2070 6172 616d 6574 6572 732e 0a20 2020   parameters..   
+00001700: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
+00001710: 6520 7365 7474 696e 6773 2065 7870 7265  e settings expre
+00001720: 7373 6564 2069 6e20 7468 6520 636f 6d6d  ssed in the comm
+00001730: 616e 6420 6c69 6e65 2077 696c 6c20 6265  and line will be
+00001740: 2061 6464 6564 2074 6f20 7468 6520 7061   added to the pa
+00001750: 7261 6d65 7465 7273 2064 6963 7469 6f6e  rameters diction
+00001760: 6172 792e 0a20 2020 2020 2020 2072 3800  ary..        r8.
+00001770: 0000 4e7a 1154 6865 2061 7267 756d 656e  ..Nz.The argumen
+00001780: 7420 666f 7220 7a9a 2077 6173 2020 2020  t for z. was    
+00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017a0: 6e6f 7420 666f 756e 6420 696e 2074 6865  not found in the
+000017b0: 2070 6172 616d 6574 6572 2066 696c 652c   parameter file,
+000017c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017d0: 2020 2020 616e 6420 7468 6572 6520 7761      and there wa
+000017e0: 7320 6120 6572 726f 7220 696e 2072 6561  s a error in rea
+000017f0: 6469 6e67 2069 7420 6672 6f6d 2074 6865  ding it from the
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 2020 2020 636f 6d6d 616e 6420 6c69 6e65      command line
+00001820: 202e 2911 7255 0000 0072 5600 0000 7257   .).rU...rV...rW
+00001830: 0000 0072 2200 0000 7259 0000 0072 5800  ...r"...rY...rX.
+00001840: 0000 721f 0000 0072 2100 0000 7220 0000  ..r....r!...r ..
+00001850: 0072 5a00 0000 725b 0000 0072 5c00 0000  .rZ...r[...r\...
+00001860: 725d 0000 0072 5e00 0000 725f 0000 00da  r]...r^...r_....
+00001870: 0965 6e75 6d65 7261 7465 da0c 5275 6e74  .enumerate..Runt
+00001880: 696d 6545 7272 6f72 2907 7209 0000 0072  imeError).r....r
+00001890: 0a00 0000 da0a 7061 7261 6d65 7465 7273  ......parameters
+000018a0: 5a09 6172 6773 5f6e 616d 65da 0964 6963  Z.args_name..dic
+000018b0: 745f 6b65 7973 da01 6972 5100 0000 720e  t_keys..irQ...r.
+000018c0: 0000 0072 0e00 0000 720f 0000 00da 106d  ...r....r......m
+000018d0: 6572 6765 5f70 6172 616d 6574 6572 730b  erge_parameters.
+000018e0: 0100 0073 2e00 0000 0006 0401 0401 0401  ...s............
+000018f0: 0401 0401 0401 0401 0401 0401 0401 0401  ................
+00001900: 0401 0401 0401 04f2 0411 0811 1001 0c01  ................
+00001910: 0201 1001 0601 7a1c 496e 7075 7450 6172  ......z.InputPar
+00001920: 7365 722e 6d65 7267 655f 7061 7261 6d65  ser.merge_parame
+00001930: 7465 7273 2903 720a 0000 0072 6300 0000  ters).r....rc...
+00001940: 7210 0000 0063 0300 0000 0000 0000 0000  r....c..........
+00001950: 0000 0400 0000 1f00 0000 4300 0000 73a2  ..........C...s.
+00001960: 0000 0064 017c 0264 0219 009b 0064 037c  ...d.|.d.....d.|
+00001970: 0264 0419 009b 0064 057c 0264 0619 009b  .d.....d.|.d....
+00001980: 0064 077c 0264 0819 009b 0064 097c 0264  .d.|.d.....d.|.d
+00001990: 0a19 009b 0064 0b7c 0264 0c19 009b 0064  .....d.|.d.....d
+000019a0: 0d7c 016a 009b 0064 0e7c 016a 019b 0064  .|.j...d.|.j...d
+000019b0: 0f7c 0264 1019 009b 0064 117c 0264 1219  .|.d.....d.|.d..
+000019c0: 009b 0064 137c 0264 1419 009b 0064 157c  ...d.|.d.....d.|
+000019d0: 0264 1619 009b 0064 177c 0264 1819 009b  .d.....d.|.d....
+000019e0: 0064 197c 0264 1a19 009b 0064 1b7c 0264  .d.|.d.....d.|.d
+000019f0: 1c19 009b 009d 1e7d 0374 027c 0383 0101  .......}.t.|....
+00001a00: 0064 1d53 0029 1e7a 5650 7269 6e74 2074  .d.S.).zVPrint t
+00001a10: 6865 2070 6172 616d 6574 6572 7320 7072  he parameters pr
+00001a20: 6f76 6964 6564 0a0a 2020 2020 2020 2020  ovided..        
+00001a30: 3a70 6172 616d 2070 6172 616d 6574 6572  :param parameter
+00001a40: 733a 2050 726f 7669 6465 6420 7061 7261  s: Provided para
+00001a50: 6d65 7465 7273 0a20 2020 2020 2020 207a  meters.        z
+00001a60: 0d0a 5265 736f 6c75 7469 6f6e 3a20 7239  ..Resolution: r9
+00001a70: 0000 007a 090a 5345 5120 4944 3a20 723a  ...z..SEQ ID: r:
+00001a80: 0000 007a 170a 5754 204d 4f44 454c 5320  ...z..WT MODELS 
+00001a90: 544f 2050 5245 5041 5245 3a20 7243 0000  TO PREPARE: rC..
+00001aa0: 007a 1b0a 4d55 5441 4e54 5320 4d4f 4445  .z..MUTANTS MODE
+00001ab0: 4c20 544f 2050 5245 5041 5245 3a20 7244  L TO PREPARE: rD
+00001ac0: 0000 007a 180a 4d41 5820 5044 4253 2041  ...z..MAX PDBS A
+00001ad0: 5320 5445 4d50 4c41 5445 533a 2072 3b00  S TEMPLATES: r;.
+00001ae0: 0000 7a12 0a52 4553 4944 5545 5320 4355  ..z..RESIDUES CU
+00001af0: 544f 4646 3a20 7242 0000 007a 0d0a 494e  TOFF: rB...z..IN
+00001b00: 5055 5420 4649 4c45 3a20 7a13 0a4f 5554  PUT FILE: z..OUT
+00001b10: 5055 5420 4449 5245 4354 4f52 593a 207a  PUT DIRECTORY: z
+00001b20: 160a 4441 5441 4241 5345 5320 4449 5245  ..DATABASES DIRE
+00001b30: 4354 4f52 593a 2072 3f00 0000 7a09 0a43  CTORY: r?...z..C
+00001b40: 4f42 414c 543a 2072 4100 0000 7a08 0a50  OBALT: rA...z..P
+00001b50: 4553 544f 3a20 723c 0000 007a 080a 484d  ESTO: r<...z..HM
+00001b60: 4d45 523a 2072 4000 0000 7a1a 0a57 4549  MER: r@...z..WEI
+00001b70: 4748 5420 5354 5255 4354 5552 414c 2053  GHT STRUCTURAL S
+00001b80: 434f 5245 3a20 7245 0000 007a 180a 5745  CORE: rE...z..WE
+00001b90: 4947 4854 204d 5554 4154 494f 4e20 5343  IGHT MUTATION SC
+00001ba0: 4f52 453a 2072 4600 0000 7a16 0a4d 4f44  ORE: rF...z..MOD
+00001bb0: 454c 4c45 5220 4558 4543 5554 4142 4c45  ELLER EXECUTABLE
+00001bc0: 3a20 7247 0000 004e 2903 7259 0000 0072  : rG...N).rY...r
+00001bd0: 5800 0000 da05 7072 696e 7429 0472 0900  X.....print).r..
+00001be0: 0000 720a 0000 0072 6300 0000 da05 7061  ..r....rc.....pa
+00001bf0: 7261 6d72 0e00 0000 720e 0000 0072 0f00  ramr....r....r..
+00001c00: 0000 da10 7072 696e 745f 7061 7261 6d65  ....print_parame
+00001c10: 7465 7273 3d01 0000 733e 0000 0000 080c  ters=...s>......
+00001c20: 0106 ff04 0206 fe04 0306 fd04 0406 fc04  ................
+00001c30: 0506 fb04 0604 fa04 0704 f904 0806 f804  ................
+00001c40: 0906 f704 0a06 f604 0b06 f504 0c06 f404  ................
+00001c50: 0d06 f304 0e06 f204 ff02 127a 1c49 6e70  ...........z.Inp
+00001c60: 7574 5061 7273 6572 2e70 7269 6e74 5f70  utParser.print_p
+00001c70: 6172 616d 6574 6572 7363 0200 0000 0000  arametersc......
+00001c80: 0000 0000 0000 0500 0000 0400 0000 4300  ..............C.
+00001c90: 0000 7356 0000 007c 00a0 007c 01a1 015c  ..sV...|...|...\
+00001ca0: 027d 027d 037c 00a0 017c 02a1 0101 007c  .}.}.|...|.....|
+00001cb0: 026a 0272 2c7c 00a0 037c 026a 02a1 017d  .j.r,|...|.j...}
+00001cc0: 046e 0a7c 00a0 047c 02a1 017d 047c 00a0  .n.|...|...}.|..
+00001cd0: 057c 027c 04a1 0201 007c 00a0 067c 027c  .|.|.....|...|.|
+00001ce0: 04a1 0201 007c 027c 0466 0253 0029 017a  .....|.|.f.S.).z
+00001cf0: 704c 6f61 6420 7573 6572 2069 6e70 7574  pLoad user input
+00001d00: 2066 726f 6d20 7468 6520 636f 6d6d 616e   from the comman
+00001d10: 6420 6c69 6e65 2061 6e64 2070 6172 616d  d line and param
+00001d20: 6574 6572 7320 6669 6c65 2e0a 0a20 2020  eters file...   
+00001d30: 2020 2020 203a 7061 7261 6d20 6172 6776       :param argv
+00001d40: 3a20 636f 6d6d 616e 6420 6c69 6e65 2061  : command line a
+00001d50: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
+00001d60: 2029 075a 1070 6172 7365 5f6b 6e6f 776e   ).Z.parse_known
+00001d70: 5f61 7267 7372 2500 0000 721e 0000 0072  _argsr%...r....r
+00001d80: 5400 0000 7260 0000 0072 6600 0000 7269  T...r`...rf...ri
+00001d90: 0000 0029 0572 0900 0000 da04 6172 6776  ...).r......argv
+00001da0: 720a 0000 005a 0875 6e70 6172 7365 6472  r....Z.unparsedr
+00001db0: 6300 0000 720e 0000 0072 0e00 0000 720f  c...r....r....r.
+00001dc0: 0000 00da 0a6c 6f61 645f 696e 7075 7458  .....load_inputX
+00001dd0: 0100 0073 1000 0000 0005 0e01 0a01 0601  ...s............
+00001de0: 0e02 0a02 0c01 0c01 7a16 496e 7075 7450  ........z.InputP
+00001df0: 6172 7365 722e 6c6f 6164 5f69 6e70 7574  arser.load_input
+00001e00: 2901 7236 0000 0029 12da 085f 5f6e 616d  ).r6...)...__nam
+00001e10: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00001e20: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0700  .__qualname__r..
+00001e30: 0000 7208 0000 00da 0861 7267 7061 7273  ..r......argpars
+00001e40: 655a 094e 616d 6573 7061 6365 7225 0000  eZ.Namespacer%..
+00001e50: 0072 0400 0000 7235 0000 0072 0300 0000  .r....r5...r....
+00001e60: 7254 0000 0072 6000 0000 7266 0000 0072  rT...r`...rf...r
+00001e70: 6900 0000 da05 7475 706c 6572 6b00 0000  i.....tuplerk...
+00001e80: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
+00001e90: 0e00 0000 720e 0000 0072 0c00 0000 720f  ....r....r....r.
+00001ea0: 0000 0072 0500 0000 0600 0000 7320 0000  ...r........s ..
+00001eb0: 0008 010c 0412 7f00 1312 1412 1700 fe02  ................
+00001ec0: 0204 0102 fd0c 2d12 1808 3306 0102 fe0c  ......-...3.....
+00001ed0: 1b72 0500 0000 2908 726f 0000 00da 0770  .r....).ro.....p
+00001ee0: 6174 686c 6962 7202 0000 00da 0674 7970  athlibr......typ
+00001ef0: 696e 6772 0300 0000 7204 0000 00da 0e41  ingr....r......A
+00001f00: 7267 756d 656e 7450 6172 7365 7272 0500  rgumentParserr..
+00001f10: 0000 720e 0000 0072 0e00 0000 720e 0000  ..r....r....r...
+00001f20: 0072 0f00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001f30: 0100 0000 7306 0000 0008 010c 0110 03    ....s..........
```

### Comparing `monviso-0.1.4/monviso_reloaded/__pycache__/isoform.cpython-39.pyc` & `monviso-0.1.5/monviso_reloaded/__pycache__/isoform.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.4/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc` & `monviso-0.1.5/monviso_reloaded/__pycache__/modeller_manager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.4/monviso_reloaded/__pycache__/template.cpython-39.pyc` & `monviso-0.1.5/monviso_reloaded/__pycache__/template.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monviso-0.1.4/monviso_reloaded/base.py` & `monviso-0.1.5/monviso_reloaded/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,43 @@
 from .database_parser import DatabaseParser
 from .gene import Gene
 from .input_parser import InputParser
+from .analyzer import Analyzer
 
-
-class Run:
+class IsoformRun:
     def __init__(self):
-        self.args = []
         self.parameters = []
         self.mutation_list = []
         self.input_parser = InputParser()
         self.genes = []
 
     def load_input(self, argv) -> None:
         """Load user input from the command line and parameters file
          and save them as attributes.
 
         :param argv: command line arguments
         """
-        self.args, self.parameters = self.input_parser.load_input(argv)
+        _, self.parameters = self.input_parser.load_input(argv)
 
     def load_mutation_list(self) -> None:
         """Parse the list of mutations and genes from the mutation_list file
         and save it as attribute.
-
-        :param mutation_list: path to the file containing the list
-        of mutations and genes
         """
         self.mutation_list = self.input_parser.parse_input(
-            self.args.input_file
+            self.parameters["INPUT_FILE"]
         )
 
     def create_genes(self) -> None:
         """Take the list of mutations of the genes saved
         in self.mutation_list, and for each gene, create a Gene instance.
         All Gene instances are saved in the
         self.gene list.
-
-        :param mutation_list: A list of the blocks extracted
-        from the input file.
-        At index 0, the list contains the name of the gene.
         """
         for i, gene_mutation_block in enumerate(self.mutation_list):
-            self.genes.append(Gene(gene_mutation_block, self.args.out_path))
+            self.genes.append(Gene(gene_mutation_block, self.parameters["OUTPUT_PATH"]))
 
     def create_isoforms(self) -> None:
         """Loads isoforms for each gene in the 'genes' attribute from
         the Uniprot database.
         """
         with DatabaseParser(self.parameters["DB_LOCATION"]) as db_parser:
             for gene in self.genes:
@@ -112,8 +104,38 @@
                     int(self.parameters["NUM_OF_MOD_MUT"]),
                     self.parameters["COBALT_HOME"])
 
             
 
     def write_report(self):
         for gene in self.genes:
-            gene.write_report()
+            gene.write_report()
+            
+
+class AnalysisRun:
+    def __init__(self):
+        self.parameters = []
+        self.genes = []
+        self.input_parser = InputParser()
+        self.genes = []
+        
+    def load_input(self, argv) -> None:
+        """Load user input from the command line and parameters file
+         and save them as attributes.
+
+        :param argv: command line arguments
+        """
+        _, self.parameters = self.input_parser.load_input(argv)
+        self.pesto_home=self.parameters["PESTO_HOME"]
+        self.output_path=self.parameters["OUTPUT_PATH"]
+
+    def load_genes_from_mutation_list(self) -> None:
+        """Parse the list of mutations and genes from the mutation_list file
+        and save the genes as attribute.
+        """
+        self.genes = [m[0] for m in self.input_parser.parse_input(
+            self.parameters["INPUT_FILE"])]
+        
+    def analysis(self) -> None:
+        self.analyzer=Analyzer(self.pesto_home,self.output_path,
+                                    self.genes)
+
```

### Comparing `monviso-0.1.4/monviso_reloaded/cobalt_wrapper.py` & `monviso-0.1.5/monviso_reloaded/cobalt_wrapper.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.4/monviso_reloaded/database_parser.py` & `monviso-0.1.5/monviso_reloaded/database_parser.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.4/monviso_reloaded/file_handler.py` & `monviso-0.1.5/monviso_reloaded/file_handler.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.4/monviso_reloaded/gene.py` & `monviso-0.1.5/monviso_reloaded/gene.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,20 @@
             mutation (list): The mutation expressed as a list, with
             one-letter residue names (e.g., ['R','899','A'])
 
         Returns:
             can_be_mutated (bool): True if mutation can be applied
             without changing residue number.
         """
-        can_be_mutated = sequence[int(mutation[1]) - 1] == mutation[0]
+        residue_ID=int(mutation[1]) - 1
+
+        if len(sequence)<residue_ID+1: #if sequence too short
+            return False
+
+        can_be_mutated = sequence[residue_ID] == mutation[0]
         return can_be_mutated
 
     def _standardize_mutations(self, mutation_list) -> list:
         """Remove white spaces from mutations. Change residue names
         to one-letter format.
         Args:
             mutation_list (list): list of mutations as obtained
```

### Comparing `monviso-0.1.4/monviso_reloaded/isoform.py` & `monviso-0.1.5/monviso_reloaded/isoform.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         output_path = Path(self.out_path, self.isoform_name + ".hmm")
         aligned_path = Path(self.out_path, "aligned.fasta")
         with FileHandler() as fh:
             if fh.check_existence(output_path):
                 print("HMMsearch output file already present in folder.")
                 return output_path
             else:
-                command = f"{hmmer_home}hmmbuild {output_path} {aligned_path}"
+                command = f"{str(Path(hmmer_home,'hmmbuild'))} {output_path} {aligned_path}"
                 subprocess.run(
                     command, shell=True, universal_newlines=True, check=True
                 )
                 return output_path
         print("Done")
 
     def HMMsearch(self, hmmer_home: Union[str, Path]) -> None:
```

### Comparing `monviso-0.1.4/monviso_reloaded/modeller_manager.py` & `monviso-0.1.5/monviso_reloaded/modeller_manager.py`

 * *Files identical despite different names*

### Comparing `monviso-0.1.4/monviso_reloaded/template.py` & `monviso-0.1.5/monviso_reloaded/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,17 @@
         self.gene_name = gene_name
         self.out_path = Path(out_path)
         self.isoform_name = isoform_name
         self.templates_directory = Path(self.out_path, "templates")
         self.pdb_filename = Path(
             self.templates_directory, self.pdb_name + ".pdb"
         )
+        self.mmCIF_filename = Path(
+            self.templates_directory, self.pdb_name + ".cif"
+        )
         self.clean_pdb_filename = Path(
             self.templates_directory, pdb_name + "_clean.pdb"
         )
         self.clean_fasta_file = Path(
             self.templates_directory, pdb_name + ".fasta"
         )
         self.resolution_cutoff = resolution_cutoff
@@ -66,28 +69,33 @@
             templates_list (str): list of pdbs that could be used for modelling
         """
         with FileHandler() as fh:
             if not fh.check_existence(self.templates_directory):
                 fh.create_directory(self.templates_directory)
 
             with PDB_manager() as pm:
-                if not fh.check_existence(self.pdb_filename):
+                if (not fh.check_existence(self.pdb_filename)) and (not fh.check_existence(self.mmCIF_filename)):
                     file = pm.downloadPDB(
                         self.pdb_name, self.out_path.parent.parent
                     )
                     fh.copy_file(file, self.templates_directory)
 
     def get_clean_pdb_chain(self) -> None:
         """Take the original PDB file in the template directory,
         extract the standard atoms from the single chain of interest,
         save it as a new file.
         """
         with PDB_manager() as pm:
+            with FileHandler() as fh:
+                if fh.check_existence(self.pdb_filename):
+                    file=self.pdb_filename
+                else:
+                    file=self.mmCIF_filename
             self.resolution = pm.extract_clean_chain(
-                self.pdb_filename,
+                file,
                 self.clean_pdb_filename,
                 self.pdb_chain,
                 self.resolution_cutoff,
             )
             if self.resolution > self.resolution_cutoff:
                 self.usable = False
```

### Comparing `monviso-0.1.4/setup.py` & `monviso-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     name="monviso",
     python_requires='>=3.9',
     version=read("monviso_reloaded", "VERSION"),
     description="MoNvIso is a comprehensive software tool designed for the analysis and modeling of protein isoforms. It automates the process of identifying canonical and additional isoforms, assessing their modeling propensity, mapping mutations accurately, and building structural models of proteins.",
     url="https://github.com/alisamalb/monviso_reloaded",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
-    author="Ciskio",
+    author="S. Albani",
     packages=find_packages(exclude=["tests", ".github"]),
     install_requires=read_requirements("requirements.txt"),
     entry_points={
-        "console_scripts": ["monviso_reloaded = monviso_reloaded.__main__:main"]
+        "console_scripts": ["monviso = monviso_reloaded.__main__:main"]
     },
     extras_require={"test": read_requirements("requirements-test.txt")},
 )
```

