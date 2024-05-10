# Comparing `tmp/animaire-1.1.7.tar.gz` & `tmp/animaire-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animaire-1.1.7.tar", last modified: Mon May  6 21:56:01 2024, max compression
+gzip compressed data, was "animaire-1.1.8.tar", last modified: Fri May 10 12:26:14 2024, max compression
```

## Comparing `animaire-1.1.7.tar` & `animaire-1.1.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:56:01.457640 animaire-1.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:56:01.453640 animaire-1.1.7/AniMAIRE/
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/AniMAIRE.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:56:01.457640 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7011 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/AsymptoticDirectionProcessing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:56:01.457640 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4810 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2013.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     4217 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2020.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     3178 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response.csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     5409 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response_tabulated_2013.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5941 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/generalEngineInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/singleParticleEngineInstance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:56:01.457640 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1550 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/momentaDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleSpecies.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2906 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/pitchAngleDistribution.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4945 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/rigiditySpectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/dose_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-06 21:55:52.000000 animaire-1.1.7/AniMAIRE/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:56:01.457640 animaire-1.1.7/AniMAIRE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28365 2024-05-06 21:56:01.000000 animaire-1.1.7/AniMAIRE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-06 21:56:01.000000 animaire-1.1.7/AniMAIRE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:56:01.000000 animaire-1.1.7/AniMAIRE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-06 21:56:01.000000 animaire-1.1.7/AniMAIRE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 21:56:01.000000 animaire-1.1.7/AniMAIRE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-06 21:55:52.000000 animaire-1.1.7/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-06 21:55:52.000000 animaire-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28365 2024-05-06 21:56:01.457640 animaire-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27514 2024-05-06 21:55:52.000000 animaire-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:56:01.457640 animaire-1.1.7/pytests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 21:55:56.000000 animaire-1.1.7/pytests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-06 21:55:56.000000 animaire-1.1.7/pytests/test_anisotropic_MAIRE.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:56:01.461640 animaire-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-06 21:55:56.000000 animaire-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:26:14.717784 animaire-1.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:26:14.713784 animaire-1.1.8/AniMAIRE/
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/AniMAIRE.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:26:14.713784 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7011 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/AsymptoticDirectionProcessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:26:14.717784 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4810 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2013.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4217 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2020.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3178 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response.csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5409 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response_tabulated_2013.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5941 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/generalEngineInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/singleParticleEngineInstance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:26:14.717784 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1550 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/momentaDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleSpecies.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2906 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/pitchAngleDistribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4945 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/rigiditySpectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/dose_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-10 12:26:02.000000 animaire-1.1.8/AniMAIRE/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:26:14.717784 animaire-1.1.8/AniMAIRE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28740 2024-05-10 12:26:14.000000 animaire-1.1.8/AniMAIRE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-10 12:26:14.000000 animaire-1.1.8/AniMAIRE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:26:14.000000 animaire-1.1.8/AniMAIRE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-10 12:26:14.000000 animaire-1.1.8/AniMAIRE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 12:26:14.000000 animaire-1.1.8/AniMAIRE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-10 12:26:02.000000 animaire-1.1.8/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 12:26:02.000000 animaire-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28740 2024-05-10 12:26:14.717784 animaire-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27891 2024-05-10 12:26:02.000000 animaire-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:26:14.717784 animaire-1.1.8/pytests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:26:06.000000 animaire-1.1.8/pytests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-10 12:26:06.000000 animaire-1.1.8/pytests/test_anisotropic_MAIRE.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:26:14.717784 animaire-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-10 12:26:06.000000 animaire-1.1.8/setup.py
```

### Comparing `animaire-1.1.7/AniMAIRE/AniMAIRE.py` & `animaire-1.1.8/AniMAIRE/AniMAIRE.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/AsymptoticDirectionProcessing.py` & `animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/AsymptoticDirectionProcessing.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2013.csv` & `animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2013.csv`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2020.csv` & `animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_alpha_response_tabulated_2020.csv`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response.csv` & `animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response.csv`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response_tabulated_2013.csv` & `animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_proton_response_tabulated_2013.csv`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_responses.py` & `animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/data/NM64_responses.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/generalEngineInstance.py` & `animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/generalEngineInstance.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/singleParticleEngineInstance.py` & `animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/singleParticleEngineInstance.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/momentaDistribution.py` & `animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/momentaDistribution.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleDistribution.py` & `animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/particleDistribution.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/pitchAngleDistribution.py` & `animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/pitchAngleDistribution.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/rigiditySpectrum.py` & `animaire-1.1.8/AniMAIRE/anisotropic_MAIRE_engine/spectralCalculations/rigiditySpectrum.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/dose_plotting.py` & `animaire-1.1.8/AniMAIRE/dose_plotting.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE/utils.py` & `animaire-1.1.8/AniMAIRE/utils.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/AniMAIRE.egg-info/PKG-INFO` & `animaire-1.1.8/AniMAIRE.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AniMAIRE
-Version: 1.1.7
+Version: 1.1.8
 Summary: Python library for running the anisotropic version of MAIRE+
 Home-page: https://github.com/ssc-maire/AniMAIRE-public
 Author: Chris S. W. Davis
 Author-email: ChrisSWDavis@gmail.com
 License: GNU General Public License v3.0
 Keywords: anisotropic MAIRE+ atmospheric ionizing radiation dose rates cosmic rays ground level enhancements GLEs protons alpha particles neutrons effective ambient equivalent aircraft aviation Earth solar system sun space magnetic field
 Description-Content-Type: text/markdown
@@ -31,15 +31,17 @@
 
 ![The AniMAIRE logo](https://raw.githubusercontent.com/ssc-maire/AniMAIRE-public/main/AniMAIRE_logo.svg)
 
 A Python toolkit for calculating dose rates and aircraft electronics upset rates in Earth's atmosphere based on any incoming proton or alpha particle spectra, with any pitch angle distribution. 
 
 **N.B. Currently this tool only runs on Linux-based machines (not on Windows) and requires a copy of [MAGNETOCOSMICS](http://cosray.unibe.ch/~laurent/magnetocosmics/) to be installed.**
 
-If you use this software for scientific research, please reference AniMAIRE as **C. S. W. Davis, F. Lei, F. Baird, K. Ryden and C. Dyer (2023). AniMAIRE version {version number}. https://github.com/ssc-maire/AniMAIRE-public , https://pypi.org/project/AniMAIRE/ . Surrey Space Center, University of Surrey.**. A scientific paper about this software is currently in production.
+If you use this software for scientific research, please reference AniMAIRE as **C. S. W. Davis, F. Lei, F. Baird, K. Ryden and C. Dyer (2023). AniMAIRE version {version number}. https://github.com/ssc-maire/AniMAIRE-public , https://pypi.org/project/AniMAIRE/ . Surrey Space Center, University of Surrey.**. 
+
+A scientific paper about this software is currently in production, and we recently published a preprint, [which can be found here](https://www.researchgate.net/publication/380403797_AniMAIRE_-_A_New_Openly_Available_Tool_for_Calculating_Atmospheric_Ionising_Radiation_Dose_Rates_and_Single_Event_Effects_During_Anisotropic_Conditions), about AniMAIRE and some interesting scientific findings we've made using our work with AniMAIRE so far.
 
 You can use AniMAIRE to produce dose rate data and maps throughout large space weather events and plot them like this:
 
 <img src="https://raw.githubusercontent.com/ssc-maire/AniMAIRE-public/main/Ani_GLE_only_timestamp1_with_legend.svg" width="350"/> <img src="https://raw.githubusercontent.com/ssc-maire/AniMAIRE-public/main/Ani_GLE_only_timestamp5_with_legend.svg" width="350"/> 
 
 Feel free to contribute to this package through forks and pull requests; the package is intended for usage and potential modification by the community. If you have any questions about this software, please contact myself, https://github.com/ChrisSWDavis, the primary author of this package.
```

### Comparing `animaire-1.1.7/AniMAIRE.egg-info/SOURCES.txt` & `animaire-1.1.8/AniMAIRE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/LICENCE` & `animaire-1.1.8/LICENCE`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/PKG-INFO` & `animaire-1.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AniMAIRE
-Version: 1.1.7
+Version: 1.1.8
 Summary: Python library for running the anisotropic version of MAIRE+
 Home-page: https://github.com/ssc-maire/AniMAIRE-public
 Author: Chris S. W. Davis
 Author-email: ChrisSWDavis@gmail.com
 License: GNU General Public License v3.0
 Keywords: anisotropic MAIRE+ atmospheric ionizing radiation dose rates cosmic rays ground level enhancements GLEs protons alpha particles neutrons effective ambient equivalent aircraft aviation Earth solar system sun space magnetic field
 Description-Content-Type: text/markdown
@@ -31,15 +31,17 @@
 
 ![The AniMAIRE logo](https://raw.githubusercontent.com/ssc-maire/AniMAIRE-public/main/AniMAIRE_logo.svg)
 
 A Python toolkit for calculating dose rates and aircraft electronics upset rates in Earth's atmosphere based on any incoming proton or alpha particle spectra, with any pitch angle distribution. 
 
 **N.B. Currently this tool only runs on Linux-based machines (not on Windows) and requires a copy of [MAGNETOCOSMICS](http://cosray.unibe.ch/~laurent/magnetocosmics/) to be installed.**
 
-If you use this software for scientific research, please reference AniMAIRE as **C. S. W. Davis, F. Lei, F. Baird, K. Ryden and C. Dyer (2023). AniMAIRE version {version number}. https://github.com/ssc-maire/AniMAIRE-public , https://pypi.org/project/AniMAIRE/ . Surrey Space Center, University of Surrey.**. A scientific paper about this software is currently in production.
+If you use this software for scientific research, please reference AniMAIRE as **C. S. W. Davis, F. Lei, F. Baird, K. Ryden and C. Dyer (2023). AniMAIRE version {version number}. https://github.com/ssc-maire/AniMAIRE-public , https://pypi.org/project/AniMAIRE/ . Surrey Space Center, University of Surrey.**. 
+
+A scientific paper about this software is currently in production, and we recently published a preprint, [which can be found here](https://www.researchgate.net/publication/380403797_AniMAIRE_-_A_New_Openly_Available_Tool_for_Calculating_Atmospheric_Ionising_Radiation_Dose_Rates_and_Single_Event_Effects_During_Anisotropic_Conditions), about AniMAIRE and some interesting scientific findings we've made using our work with AniMAIRE so far.
 
 You can use AniMAIRE to produce dose rate data and maps throughout large space weather events and plot them like this:
 
 <img src="https://raw.githubusercontent.com/ssc-maire/AniMAIRE-public/main/Ani_GLE_only_timestamp1_with_legend.svg" width="350"/> <img src="https://raw.githubusercontent.com/ssc-maire/AniMAIRE-public/main/Ani_GLE_only_timestamp5_with_legend.svg" width="350"/> 
 
 Feel free to contribute to this package through forks and pull requests; the package is intended for usage and potential modification by the community. If you have any questions about this software, please contact myself, https://github.com/ChrisSWDavis, the primary author of this package.
```

### Comparing `animaire-1.1.7/README.md` & `animaire-1.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 ![The AniMAIRE logo](https://raw.githubusercontent.com/ssc-maire/AniMAIRE-public/main/AniMAIRE_logo.svg)
 
 A Python toolkit for calculating dose rates and aircraft electronics upset rates in Earth's atmosphere based on any incoming proton or alpha particle spectra, with any pitch angle distribution. 
 
 **N.B. Currently this tool only runs on Linux-based machines (not on Windows) and requires a copy of [MAGNETOCOSMICS](http://cosray.unibe.ch/~laurent/magnetocosmics/) to be installed.**
 
-If you use this software for scientific research, please reference AniMAIRE as **C. S. W. Davis, F. Lei, F. Baird, K. Ryden and C. Dyer (2023). AniMAIRE version {version number}. https://github.com/ssc-maire/AniMAIRE-public , https://pypi.org/project/AniMAIRE/ . Surrey Space Center, University of Surrey.**. A scientific paper about this software is currently in production.
+If you use this software for scientific research, please reference AniMAIRE as **C. S. W. Davis, F. Lei, F. Baird, K. Ryden and C. Dyer (2023). AniMAIRE version {version number}. https://github.com/ssc-maire/AniMAIRE-public , https://pypi.org/project/AniMAIRE/ . Surrey Space Center, University of Surrey.**. 
+
+A scientific paper about this software is currently in production, and we recently published a preprint, [which can be found here](https://www.researchgate.net/publication/380403797_AniMAIRE_-_A_New_Openly_Available_Tool_for_Calculating_Atmospheric_Ionising_Radiation_Dose_Rates_and_Single_Event_Effects_During_Anisotropic_Conditions), about AniMAIRE and some interesting scientific findings we've made using our work with AniMAIRE so far.
 
 You can use AniMAIRE to produce dose rate data and maps throughout large space weather events and plot them like this:
 
 <img src="https://raw.githubusercontent.com/ssc-maire/AniMAIRE-public/main/Ani_GLE_only_timestamp1_with_legend.svg" width="350"/> <img src="https://raw.githubusercontent.com/ssc-maire/AniMAIRE-public/main/Ani_GLE_only_timestamp5_with_legend.svg" width="350"/> 
 
 Feel free to contribute to this package through forks and pull requests; the package is intended for usage and potential modification by the community. If you have any questions about this software, please contact myself, https://github.com/ChrisSWDavis, the primary author of this package.
```

### Comparing `animaire-1.1.7/pytests/test_anisotropic_MAIRE.py` & `animaire-1.1.8/pytests/test_anisotropic_MAIRE.py`

 * *Files identical despite different names*

### Comparing `animaire-1.1.7/setup.py` & `animaire-1.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 setup(
     name='AniMAIRE',
     packages=find_packages(exclude='pytests'),
     package_data={"AniMAIRE":[
                                 "anisotropic_MAIRE_engine/data/*.csv"
                                          ]},
-    version='1.1.7',
+    version='1.1.8',
     description='Python library for running the anisotropic version of MAIRE+',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Chris S. W. Davis',
     author_email='ChrisSWDavis@gmail.com',
     license='GNU General Public License v3.0',
     url='https://github.com/ssc-maire/AniMAIRE-public',
```

