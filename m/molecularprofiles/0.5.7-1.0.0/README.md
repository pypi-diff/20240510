# Comparing `tmp/molecularprofiles-0.5.7.tar.gz` & `tmp/molecularprofiles-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecularprofiles-0.5.7.tar", last modified: Fri May  3 15:14:01 2024, max compression
+gzip compressed data, was "molecularprofiles-1.0.0.tar", last modified: Fri May 10 15:04:34 2024, max compression
```

## Comparing `molecularprofiles-0.5.7.tar` & `molecularprofiles-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2024-05-03 15:14:01.289250 molecularprofiles-0.5.7/
--rw-r--r--   0 mdalchen   (501) staff       (20)     1474 2022-11-22 15:24:35.000000 molecularprofiles-0.5.7/LICENSE
--rw-r--r--   0 mdalchen   (501) staff       (20)     3269 2024-05-03 15:14:01.288790 molecularprofiles-0.5.7/PKG-INFO
--rw-r--r--   0 mdalchen   (501) staff       (20)      450 2023-02-01 16:41:16.000000 molecularprofiles-0.5.7/README.md
--rw-r--r--   0 mdalchen   (501) staff       (20)     1638 2023-07-21 08:41:06.000000 molecularprofiles-0.5.7/pyproject.toml
--rw-r--r--   0 mdalchen   (501) staff       (20)       38 2024-05-03 15:14:01.289323 molecularprofiles-0.5.7/setup.cfg
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2024-05-03 15:14:01.279369 molecularprofiles-0.5.7/src/
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2024-05-03 15:14:01.281453 molecularprofiles-0.5.7/src/molecularprofiles/
--rwxr-xr-x   0 mdalchen   (501) staff       (20)      195 2024-05-03 15:10:02.000000 molecularprofiles-0.5.7/src/molecularprofiles/__init__.py
--rwxr-xr-x   0 mdalchen   (501) staff       (20)    24137 2024-05-03 15:07:02.000000 molecularprofiles-0.5.7/src/molecularprofiles/molecularprofiles.py
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2024-05-03 15:14:01.286605 molecularprofiles-0.5.7/src/molecularprofiles/utils/
--rw-r--r--   0 mdalchen   (501) staff       (20)       27 2023-02-03 15:27:32.000000 molecularprofiles-0.5.7/src/molecularprofiles/utils/__init__.py
--rwxr-xr-x   0 mdalchen   (501) staff       (20)     2168 2024-05-03 15:07:02.000000 molecularprofiles-0.5.7/src/molecularprofiles/utils/constants.py
--rwxr-xr-x   0 mdalchen   (501) staff       (20)     8758 2024-05-03 15:09:25.000000 molecularprofiles-0.5.7/src/molecularprofiles/utils/grib_utils.py
--rwxr-xr-x   0 mdalchen   (501) staff       (20)    10490 2023-07-21 08:41:06.000000 molecularprofiles-0.5.7/src/molecularprofiles/utils/humidity.py
--rw-r--r--   0 mdalchen   (501) staff       (20)      327 2023-02-03 15:27:32.000000 molecularprofiles-0.5.7/src/molecularprofiles/utils/mdps_log.conf
--rw-r--r--   0 mdalchen   (501) staff       (20)    14694 2023-07-21 08:41:06.000000 molecularprofiles-0.5.7/src/molecularprofiles/utils/rayleigh.py
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2024-05-03 15:14:01.287265 molecularprofiles-0.5.7/src/molecularprofiles.egg-info/
--rw-r--r--   0 mdalchen   (501) staff       (20)     3269 2024-05-03 15:14:01.000000 molecularprofiles-0.5.7/src/molecularprofiles.egg-info/PKG-INFO
--rw-r--r--   0 mdalchen   (501) staff       (20)      578 2024-05-03 15:14:01.000000 molecularprofiles-0.5.7/src/molecularprofiles.egg-info/SOURCES.txt
--rw-r--r--   0 mdalchen   (501) staff       (20)        1 2024-05-03 15:14:01.000000 molecularprofiles-0.5.7/src/molecularprofiles.egg-info/dependency_links.txt
--rw-r--r--   0 mdalchen   (501) staff       (20)      193 2024-05-03 15:14:01.000000 molecularprofiles-0.5.7/src/molecularprofiles.egg-info/requires.txt
--rw-r--r--   0 mdalchen   (501) staff       (20)       18 2024-05-03 15:14:01.000000 molecularprofiles-0.5.7/src/molecularprofiles.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:04:34.793364 molecularprofiles-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3846 2024-05-10 15:04:34.793364 molecularprofiles-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      793 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 15:04:34.793364 molecularprofiles-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:04:34.785364 molecularprofiles-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:04:34.789364 molecularprofiles-1.0.0/src/molecularprofiles/
+-rwxrwxrwx   0 root         (0) root         (0)      195 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/src/molecularprofiles/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    24728 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/src/molecularprofiles/molecularprofiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:04:34.789364 molecularprofiles-1.0.0/src/molecularprofiles/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4436 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/src/molecularprofiles/tests/test_grib_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2911 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/src/molecularprofiles/tests/test_humidity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3521 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/src/molecularprofiles/tests/test_molecular_profiles.py
+-rw-rw-rw-   0 root         (0) root         (0)     3522 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/src/molecularprofiles/tests/test_rayleigh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:04:34.789364 molecularprofiles-1.0.0/src/molecularprofiles/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/src/molecularprofiles/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2198 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/src/molecularprofiles/utils/constants.py
+-rwxrwxrwx   0 root         (0) root         (0)     8093 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/src/molecularprofiles/utils/grib_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    10416 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/src/molecularprofiles/utils/humidity.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/src/molecularprofiles/utils/mdps_log.conf
+-rw-rw-rw-   0 root         (0) root         (0)    14517 2024-05-10 15:04:15.000000 molecularprofiles-1.0.0/src/molecularprofiles/utils/rayleigh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:04:34.789364 molecularprofiles-1.0.0/src/molecularprofiles.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3846 2024-05-10 15:04:34.000000 molecularprofiles-1.0.0/src/molecularprofiles.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      770 2024-05-10 15:04:34.000000 molecularprofiles-1.0.0/src/molecularprofiles.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 15:04:34.000000 molecularprofiles-1.0.0/src/molecularprofiles.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      243 2024-05-10 15:04:34.000000 molecularprofiles-1.0.0/src/molecularprofiles.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-10 15:04:34.000000 molecularprofiles-1.0.0/src/molecularprofiles.egg-info/top_level.txt
```

### Comparing `molecularprofiles-0.5.7/LICENSE` & `molecularprofiles-1.0.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
 THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
 IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
-ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `molecularprofiles-0.5.7/PKG-INFO` & `molecularprofiles-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularprofiles
-Version: 0.5.7
+Version: 1.0.0
 Summary: Meteorological data analysis suite
 Author-email: Pere Munar Adrover <pere.munar@uab.cat>, Markus Gaug <markus.gaug@uab.cat>, Scott Griffiths <sgriffiths@ifae.es>, Georgios Voutsinas <georgios.voutsinas@unige.ch>, Mykhailo Dalchenko <mykhailo.dalchenko@unige.ch>
 License: Copyright (c) 2020, Molecularprofiles Project
         
         Redistribution and use in source and binary forms, with or withoutmodification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -15,48 +15,61 @@
         
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
         THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
         IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
         (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
         HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
         ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
 Project-URL: Home, https://gitlab.cta-observatory.org/cta-array-elements/ccf/mdps
+Project-URL: Doc, http://cta-array-elements.gitlab-pages.cta-observatory.org/ccf/MDPs/
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: astropy
 Requires-Dist: pygrib
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pylint>=2.15; extra == "test"
 Requires-Dist: black>=22.5; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: coverage-badge; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: numpydoc; extra == "doc"
+Requires-Dist: pydata-sphinx-theme; extra == "doc"
+Requires-Dist: myst-parser<2.0.0; extra == "doc"
+Requires-Dist: sphinx-paramlinks; extra == "doc"
+Requires-Dist: sphinx-argparse; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
-Requires-Dist: sphinx_rtd_theme; extra == "doc"
-Requires-Dist: myst-parser; extra == "doc"
 Requires-Dist: linkify-it-py; extra == "doc"
-Requires-Dist: sphinx-argparse; extra == "doc"
-Requires-Dist: sphinx-paramlinks; extra == "doc"
+Requires-Dist: ipykernel; extra == "doc"
+Provides-Extra: dev
+Requires-Dist: setuptools_scm; extra == "dev"
 
 # molecularprofiles
 
-!! OBSOLETE !! 
-Will be updated upon availability of CI configuration
-
-See the documentation here: https://molecularprofiles.readthedocs.io/en/latest/
-
-functions to plot and work with meteorological data in grib2 format from ECMWF and GDAS. This work is used for the calibration of the CTA
-
-https://github.com/cambecc/grib2json
-
-In order to install it go to the directory containing the file setup.py and type:
+A collection of routines to read an analyze meteorological data in `grib2` format.
 
-pip install ./
+See [project documentation](http://cta-array-elements.gitlab-pages.cta-observatory.org/ccf/MDPs/) for API docs.
 
+## Development installation:
 
+- Clone the code with git:
+  ```shell
+  > git clone https://gitlab.cta-observatory.org/cta-array-elements/ccf/mdps.git
+  ```
+- Checkout an appropriate branch (currently, dev branch contains the most recent code):
+  ```shell
+  git checkout -b <branch_name>
+  ```
+- Use `mamba` to setup a clean environment
+  ```shell
+  > mamba create -n molecularprofiles -c conda-forge python==3.12
+  > mamba activate molecularprofiles
+  ```
+- Install molecularprofiles in editable mode with test dependencies:
+  ```shell
+  > pip install -e.[test,doc,dev]
+  ```
```

### Comparing `molecularprofiles-0.5.7/src/molecularprofiles/molecularprofiles.py` & `molecularprofiles-1.0.0/src/molecularprofiles/molecularprofiles.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 This is a class that offers a set of functions to work with meteorological data
-in ecsv or grib(2) format.
+in ``ecsv`` or ``grib(2)`` format.
+
+Created by Pere Munar-Adrover (pere.munaradrover@gmail.com)
 
-Created by Pere Munar-Adrover
-email: pere.munaradrover@gmail.com
 Further developed and mainted by
-Mykhailo Dalchenko (mykhailo.dalchenko@unige.ch) and
-Georgios Voutsinas (georgios.voutsinas@unige.ch)
+
+* Mykhailo Dalchenko (mykhailo.dalchenko@unige.ch) and
+* Georgios Voutsinas (georgios.voutsinas@unige.ch)
 """
 
+from bisect import bisect_left
 import os
 import sys
 import logging
 
 import astropy.units as u
 from astropy.table import Table, QTable, vstack, Column
+from astropy.io.registry.base import IORegistryError
 import numpy as np
 from scipy.interpolate import interp1d
-from bisect import bisect_left
 
 from molecularprofiles.utils.grib_utils import get_grib_file_data, extend_grib_data
 from molecularprofiles.utils.constants import (
     DENSITY_SCALE_HEIGHT,
     N0_AIR,
     STD_GRAVITATIONAL_ACCELERATION,
     STD_AIR_DENSITY,
@@ -39,70 +41,97 @@
 
 ROOTDIR = os.path.dirname(os.path.abspath(__file__))
 log_config_file = f"{ROOTDIR}/utils/mdps_log.conf"
 logging.config.fileConfig(fname=log_config_file, disable_existing_loggers=False)
 logger = logging.getLogger(__name__)
 
 
+def _write(table_data, filename, _overwrite=True):
+    try:
+        table_data.write(filename, overwrite=_overwrite)
+    except (ValueError, TypeError, OSError, IORegistryError) as ex:
+        template = "An exception of type {0} occurred. Arguments:\n{1!r}"
+        message = template.format(type(ex).__name__, ex.args)
+        logger.error(message)
+        sys.exit(1)
+
+
 class MolecularProfile:
     """
-    This class provides a series of functions to analyze the quality of the data for both
-    CTA-North and CTA-South.
+    This class provides a series of functions to analyze the quality of the data
+    for both CTA-North and CTA-South.
 
     Methods within this class:
 
-    get_data:                   it retrieves the data from the input file. If the input file
-                                is a grib file and there is no file in the working directory
-                                with the same name but with .txt extension the program extracts
-                                the data from the grib file through the grib_utils program. If
-                                there is such a txt file, it reads it directly
-    write_atmospheric_profile:  prints the data into a txt file which format is compliant with the input card
-                                for the CORSIKA air shower simulation software
-    create_mdp:                 creates an altitude profile of the molecular number density
-    rayleigh_extinction:        creates a file, in format to be directly fed to simtel simulation, with the
-                                extinction per altitude bin for wavelengths from 200 to 1000 nm
+    get_data:                   retrieves the data from the input file.
+                                If the input filei is a ``grib`` file,
+                                the data is extracted using the grib_utils module.
+                                If the input file is an ``ecsv``,
+                                ``astropy.Table`` ``read`` method is used.
+    write_atmospheric_profile:  writes an ecsv file that contains the atmosphere-related
+                                information, required by Corsika simulations.
+    create_mdp:                 creates an altitude profile of the
+                                molecular number density.
+    rayleigh_extinction:        writes a table with the atmospheric absolute optical depth
+                                binned in wavelength and altitude into an ``ecsv`` file.
     """
 
     def __init__(self, data_file):
         """
         Constructor
 
         :param data_file: txt file containing the data (string)
         """
 
         self.data_file = data_file
+        self.data = None
+        self.stat_data = None
+        self.stat_description = None
+        self.stat_columns = [
+            "Pressure",
+            "Altitude",
+            "Density",
+            "Temperature",
+            "Wind Speed",
+            "Wind Direction",
+            "Relative humidity",
+            "Exponential Density",
+        ]
 
-    # =============================================================================================================
+    # ==================================================================================
     # Private functions
-    # =============================================================================================================
+    # ==================================================================================
+
     def _interpolate_cubic(self, x_param, y_param, new_x_param):
         func = interp1d(x_param, y_param, kind="cubic", bounds_error=False)
         return func(new_x_param)
 
     def _compute_mass_density(self, air="moist", co2_concentration=415):
         """
         Computes regular and exponential mass density of air.
 
         Adds to data the following columns:
-        - 'Xw': molar fraction of water vapor (0 if air is dry)
-        - 'Compressibility'
-        - 'Mass Density'
-        - 'Exponential Mass Density'
+        * 'Xw': molar fraction of water vapor (0 if air is dry)
+        * 'Compressibility'
+        * 'Mass Density'
+        * 'Exponential Mass Density'
 
         Parameters
         ----------
         air : str
             Type of air, can be 'moist' or 'dry'
         co2_concentration : float
             CO2 volume concentration in ppmv
         """
 
         if air == "moist":
             self.data["Xw"] = molar_fraction_water_vapor(
-                self.data["Pressure"], self.data["Temperature"], self.data["Relative humidity"]
+                self.data["Pressure"],
+                self.data["Temperature"],
+                self.data["Relative humidity"],
             )
         elif air == "dry":
             self.data["Xw"] = 0.0
         else:
             raise ValueError("Wrong air condition. It must be 'moist' or 'dry'.")
 
         self.data["Compressibility"] = compressibility(
@@ -113,67 +142,73 @@
             self.data["Temperature"],
             self.data["Compressibility"],
             self.data["Xw"],
             co2_concentration,
         )
         self.data["Exponential Mass Density"] = (
             self.data["Mass Density"] / STD_AIR_DENSITY
-        ).decompose() * np.exp((self.data["Altitude"] / DENSITY_SCALE_HEIGHT).decompose())
+        ).decompose() * np.exp(
+            (self.data["Altitude"] / DENSITY_SCALE_HEIGHT).decompose()
+        )
 
-    # =============================================================================================================
+    # ==================================================================================
     # Main get data function
-    # =============================================================================================================
+    # ==================================================================================
     def get_data(self):
         """
         Reads ECMWF or GDAS data in ecsv or grib(2) format
         and computes statistical description of the data
         """
+        if not os.path.isfile(self.data_file):
+            raise FileNotFoundError(f"The file '{self.data_file}' does not exist.")
         file_ext = os.path.splitext(self.data_file)[1]
-        if file_ext == ".grib" or file_ext == ".grib2":
+        if file_ext in (".grib", ".grib2"):
             self.data = get_grib_file_data(self.data_file)
             self.data = extend_grib_data(self.data)
         elif file_ext == ".ecsv":
             self.data = Table.read(self.data_file)
         else:
             raise NotImplementedError(
-                f"Only grib (1,2) and ecsv formats are supported at the moment. Requested format: {file_ext}"
+                "Only grib (1,2) and ecsv formats are supported at the moment. "
+                f"Requested format: {file_ext}"
             )
-        self.stat_columns = [
-            "Pressure",
-            "Altitude",
-            "Density",
-            "Temperature",
-            "Wind Speed",
-            "Wind Direction",
-            "Relative humidity",
-            "Exponential Density",
-        ]
         self.stat_data = self.data[self.stat_columns].group_by("Pressure")
         self.stat_description = {
             "avg": self.stat_data.groups.aggregate(np.mean),
             "std": self.stat_data.groups.aggregate(np.std),
-            "mad": self.stat_data.groups.aggregate(lambda x: np.mean(np.absolute(x - np.mean(x)))),
-            "p2p_max": self.stat_data.groups.aggregate(lambda x: np.max(x) - np.mean(x)),
-            "p2p_min": self.stat_data.groups.aggregate(lambda x: np.mean(x) - np.min(x)),
+            "mad": self.stat_data.groups.aggregate(
+                lambda x: np.mean(np.absolute(x - np.mean(x)))
+            ),
+            "p2p_max": self.stat_data.groups.aggregate(
+                lambda x: np.max(x) - np.mean(x)
+            ),
+            "p2p_min": self.stat_data.groups.aggregate(
+                lambda x: np.mean(x) - np.min(x)
+            ),
         }
 
-    def _refractive_index(self, P, T, RH, wavelength, C):
+    # pylint: disable=too-many-arguments
+    def _refractive_index(self, P, T, RH, wavelength, CO2):
         """Wrapper for Rayleigh.calculate_n()."""
-        rayleigh = Rayleigh(wavelength, C, P, T, RH)
+        rayleigh = Rayleigh(wavelength, CO2, P, T, RH)
         return rayleigh.refractive_index
 
+    # pylint: enable=too-many-arguments
+
     def _take_closest(self, my_list, my_number):
+        # pylint: disable=line-too-long
         """
         Returns closest value to my_number.
         If two numbers are equally close, return the smallest number.
         This function comes from the answer of user:
         https://stackoverflow.com/users/566644/lauritz-v-thaulow
         found in stack overflow post:
         https://stackoverflow.com/questions/12141150/from-list-of-integers-get-number-closest-to-a-given-value/12141511#12141511
         """
+        # pylint: enable=line-too-long
         pos = bisect_left(my_list, my_number)
         if pos == 0:
             return my_list[0]
         if pos == len(my_list):
             return my_list[-1]
         before = my_list[pos - 1]
         after = my_list[pos]
@@ -184,35 +219,38 @@
     def _get_data_altitude_range(self, altitude_profile):
         """
         Calculates the floor and ceiling of the available DAS data.
 
         Parameters:
         -----------
         altitude_profile : Quantity
-            Tuple with the altitudes that the atmospheric parameters will be calculated. Units of length.
+            Tuple with the altitudes that the atmospheric parameters will be calculated.
+            Units of length.
+
         Returns:
         --------
-            floor, ceiling : Quantities that define the highest and lowest altitude that DAS data are available.
+        m_floor, m_ceiling :
+            Highest and lowest altitudes, where DAS data is available.
         """
 
-        floor = self._take_closest(
+        m_floor = self._take_closest(
             altitude_profile,
             (
                 (self.stat_description["avg"]["Altitude"][-1])
                 * (self.stat_description["avg"]["Altitude"].unit)
             ).to(altitude_profile.unit),
         )
-        ceiling = self._take_closest(
+        m_ceiling = self._take_closest(
             altitude_profile,
             (
                 (self.stat_description["avg"]["Altitude"][0])
                 * (self.stat_description["avg"]["Altitude"].unit)
             ).to(altitude_profile.unit),
         )
-        return floor, ceiling
+        return m_floor, m_ceiling
 
     def _create_profile(self, interpolation_centers):
         """Interpolates atmospheric parameters in the requested interpolation centers"""
 
         temperature = (
             self._interpolate_cubic(
                 self.stat_description["avg"]["Altitude"].to(u.km),
@@ -244,108 +282,110 @@
                 interpolation_centers.to(u.km),
             )
             * self.stat_description["avg"]["Density"].unit
             / N0_AIR
         )
         return temperature, relative_humidity, pressure, density
 
-    def _pick_up_reference_atmosphere(self, ceiling, floor, reference_atmosphere):
+    def _pick_up_reference_atmosphere(self, m_ceiling, m_floor, reference_atmosphere):
         """
         Picks up the reference atmosphere corresponding to the season and
         the geographical location. It selects all rows above the given ceiling.
 
         Parameters:
         -----------
-        ceiling
+        m_ceiling
             Astropy quantity expressing the ceiling of the DAS data.
         reference_atmosphere
             ecsv file with the reference atmosphere profile.
 
         Returns:
         --------
         table
             Astropy table with the atmospheric profile above the given ceiling.
         """
         try:
             reference_atmosphere_table = Table.read(reference_atmosphere)
-        except Exception as ex:
-            template = "An exception of type {0} occurred. Arguments:\n{1!r}"
-            message = template.format(type(ex).__name__, ex.args)
-            logger.error(message)
-            sys.exit(1)
-        try:
-            mask = (
-                reference_atmosphere_table["altitude"]
-                >= ceiling.to(reference_atmosphere_table["altitude"].unit)
-            ) | (
-                reference_atmosphere_table["altitude"]
-                <= floor.to(reference_atmosphere_table["altitude"].unit)
-            )
-            return reference_atmosphere_table[mask]
-        except Exception as ex:
+        except (TypeError, ValueError, RuntimeError) as ex:
             template = "An exception of type {0} occurred. Arguments:\n{1!r}"
             message = template.format(type(ex).__name__, ex.args)
             logger.error(message)
             sys.exit(1)
+        mask = (
+            reference_atmosphere_table["altitude"]
+            >= m_ceiling.to(reference_atmosphere_table["altitude"].unit)
+        ) | (
+            reference_atmosphere_table["altitude"]
+            <= m_floor.to(reference_atmosphere_table["altitude"].unit)
+        )
+        return reference_atmosphere_table[mask]
 
-    # =======================================================================================================
+    # ==================================================================================
     # printing functions:
-    # =======================================================================================================
+    # ==================================================================================
 
+    # pylint: disable=too-many-locals
     def write_atmospheric_profile(
         self,
         outfile,
         co2_concentration,
-        floor=None,
         reference_atmosphere=None,
         altitude_list=STD_CORSIKA_ALTITUDE_PROFILE,
     ):
+        # pylint: disable=line-too-long
         """
-        Write an output file in the style of a CORSIKA atmospheric configuration file:
-        altitude (km)     density (g/cm^3)   thickness (g/cm^2)   refractive index -1   temperature (K)   pressure (hPA)   partial water pressure
+        Write an output file in the style of a CORSIKA atmospheric configuration file.
+
+        File format:
+        altitude (km)\tdensity (g/cm^3)\tthickness (g/cm^2)\trefractive index -1\ttemperature (K)\tpressure (hPA)\tpartial water pressure
 
         Parameters:
         -----------
         outfile : string
             Name of the returned file.
         co2_concentration : float
             12MACOBAC value
-        floor : Quantity
-            Lowest altitude level where the atmospheric parameters will be calculated. If none is provided, it gets the closer to the sea level altitude where data are available. Units of length.
         reference_atmosphere : path
             The path where the file with the reference atmosphere model is located.
         altitude_list : Quantity
-            Tuple with the altitudes that the atmospheric parameters will be calculated. Units of length.
+            Tuple with the altitudes that the atmospheric parameters will be calculated.
+            Units of length.
 
         Returns:
         --------
             Ecsv file in the style of a CORSIKA atmospheric configuration file.
         """
+        # pylint: enable=line-too-long
 
-        floor, ceiling = self._get_data_altitude_range(
+        m_floor, m_ceiling = self._get_data_altitude_range(
             altitude_list.to(self.stat_description["avg"]["Altitude"].unit)
         )
         altitude = altitude_list[
-            (altitude_list.to_value() > floor.to_value(altitude_list.unit))
-            & (altitude_list.to_value() < ceiling.to_value(altitude_list.unit))
+            (altitude_list.to_value() > m_floor.to_value(altitude_list.unit))
+            & (altitude_list.to_value() < m_ceiling.to_value(altitude_list.unit))
         ]
         altitude = altitude.to(self.stat_description["avg"]["Altitude"].unit)
-        temperature, relative_humidity, pressure, density = self._create_profile(altitude)
+        temperature, relative_humidity, pressure, density = self._create_profile(
+            altitude
+        )
         thickness = pressure / STD_GRAVITATIONAL_ACCELERATION
         rel_water_vapor_pressure = (
             partial_pressure_water_vapor(temperature, relative_humidity) / pressure
         ).decompose()
         rel_refractive_index = (
             self._refractive_index(
-                pressure, temperature, relative_humidity, 350.0 * u.nm, co2_concentration
+                pressure,
+                temperature,
+                relative_humidity,
+                350.0 * u.nm,
+                co2_concentration,
             )
             - 1.0
         )
 
-        corsika_input_table = Table()
         tables = []
 
         for i in np.arange(len(altitude)):
             outdict = {
                 "altitude": altitude[i].to(u.km),
                 "atmospheric_density": density[i].to(u.g / u.cm**3),
                 "atmospheric_thickness": thickness[i].decompose().to(u.g / u.cm**2),
@@ -354,24 +394,28 @@
                 "pressure": pressure[i],
                 "partial_water_pressure": rel_water_vapor_pressure[i],
             }
             tables.append(outdict)
         # Merge ECMWF profile with upper atmospheric profile
         if reference_atmosphere:
             reference_atmosphere_table = self._pick_up_reference_atmosphere(
-                ceiling, floor, reference_atmosphere
+                m_ceiling, m_floor, reference_atmosphere
             )
             tables.append(reference_atmosphere_table)
         else:
-            logger.info(
-                "Since reference atmosphere was not provided, the resulting atmospheric model will be constrained to the extent of the provided meteorological data."
+            logger.warning(
+                "Since reference atmosphere was not provided, "
+                "the resulting atmospheric model will be constrained "
+                "to the extent of the provided meteorological data."
             )
         corsika_input_table = vstack(tables)
         corsika_input_table.sort("altitude")
-        corsika_input_table.write(outfile, overwrite=True)
+        _write(corsika_input_table, outfile)
+
+    # pylint: enable=too-many-locals
 
     def create_mdp(self, mdp_file):
         """
         Write an output file with the molecular number density per altitude
         """
 
         altitudes = np.arange(0.0, 20000.0, 1000) * u.m
@@ -381,37 +425,33 @@
                 self.stat_description["avg"]["Altitude"],
                 self.stat_description["avg"]["Density"],
                 altitudes,
             )
             * self.stat_description["avg"]["Density"].unit
         )
         t = Table([altitudes, number_density], names=["altitude", "number density"])
-        try:
-            t.write(mdp_file, overwrite=True)
-        except Exception as ex:
-            template = "An exception of type {0} occurred. Arguments:\n{1!r}"
-            message = template.format(type(ex).__name__, ex.args)
-            logger.error(message)
-            sys.exit(1)
+        _write(t, mdp_file)
 
+    # pylint: disable=too-many-arguments,too-many-locals
     def rayleigh_extinction(
         self,
         rayleigh_extinction_file,
         co2_concentration,
         wavelength_min=200 * u.nm,
         wavelength_max=700 * u.nm,
         reference_atmosphere=None,
         rayleigh_scattering_altitude_bins=RAYLEIGH_SCATTERING_ALTITUDE_BINS,
     ):
         """
         Calculates the absolute integral optical depth due to Rayleigh scattering
         per altitude bins as a function of wavelength.
+
         The optical depth (AOD) for an altitude h over the observatory will be given by
-        the integral of the monochromatic volume coefficient beta, with integration limits
-        h_obs up to h.
+        the integral of the monochromatic volume coefficient beta,
+        with integration limits h_obs up to h.
 
         Parameters:
         -----------
         rayleigh_extinction_file : string
             Name of the returned file with the extinction profile.
         co2_concentration : float
             12MACOBAC value
@@ -420,78 +460,87 @@
         reference_atmosphere : path
             The path where the file with the reference atmosphere model is located.
         rayleigh_scattering_altitude_bins : Quantity
             Tuple with the altitudes that the AOD will be calculated. Units of length.
 
         Returns:
         --------
-            Ecsv file with absolute optical depth per altitude bin per wavelength bin. The data model is the same with MODTRAN files.
+            Ecsv file with absolute optical depth per altitude bin per wavelength bin.
         """
 
-        floor, ceiling = self._get_data_altitude_range(rayleigh_scattering_altitude_bins)
+        m_floor, m_ceiling = self._get_data_altitude_range(
+            rayleigh_scattering_altitude_bins
+        )
         altitude = rayleigh_scattering_altitude_bins.to(u.km)
-        altitude = altitude[altitude < ceiling]
+        altitude = altitude[altitude < m_ceiling]
 
         interpolation_centers = (altitude[:-1] + altitude[1:]) / 2
         (
             temperature_lower,
             relative_humidity_lower,
             pressure_lower,
-            density_lower,
+            _,
         ) = self._create_profile(interpolation_centers)
 
         # Concatenate with reference atmosphere
         if reference_atmosphere:
             reference_atmosphere_table = self._pick_up_reference_atmosphere(
-                ceiling, floor, reference_atmosphere
+                m_ceiling, m_floor, reference_atmosphere
             )
             length_of_columns = len(reference_atmosphere_table)
             relative_humidity_upper = (
-                np.zeros(length_of_columns) * self.stat_description["avg"]["Relative humidity"].unit
+                np.zeros(length_of_columns)
+                * self.stat_description["avg"]["Relative humidity"].unit
+            )
+            relative_humidity = np.concatenate(
+                (relative_humidity_lower, relative_humidity_upper)
+            )
+            pressure = np.concatenate(
+                (pressure_lower, reference_atmosphere_table["pressure"])
+            )
+            temperature = np.concatenate(
+                (temperature_lower, reference_atmosphere_table["temperature"])
+            )
+            altitude = np.concatenate(
+                (altitude, reference_atmosphere_table["altitude"])
             )
-            try:
-                relative_humidity = np.concatenate(
-                    (relative_humidity_lower, relative_humidity_upper)
-                )
-                pressure = np.concatenate((pressure_lower, reference_atmosphere_table["pressure"]))
-                temperature = np.concatenate(
-                    (temperature_lower, reference_atmosphere_table["temperature"])
-                )
-                altitude = np.concatenate((altitude, reference_atmosphere_table["altitude"]))
-            except Exception as ex:
-                template = "An exception of type {0} occurred. Arguments:\n{1!r}"
-                message = template.format(type(ex).__name__, ex.args)
-                logger.error(message)
         else:
-            logger.info(
-                "Since the reference atmosphere was not provided, the resulting atmospheric model will be constrained to the extent of the provided meteorological data."
+            logger.warning(
+                "Since the reference atmosphere was not provided, "
+                "the resulting atmospheric model will be constrained "
+                "to the extent of the provided meteorological data."
             )
             temperature = temperature_lower
             pressure = pressure_lower
             relative_humidity = relative_humidity_lower
 
         t = QTable(
             [altitude[1:], pressure, temperature, relative_humidity],
             names=("altitude", "pressure", "temperature", "relative_humidity"),
         )
         t.sort("altitude")
         bin_widths = np.diff(np.sort(altitude))
         t["bin_widths"] = bin_widths
-        mask = t["altitude"] > floor
+        mask = t["altitude"] > m_floor
         wavelength_range = (
-            np.arange(wavelength_min.to_value(u.nm), wavelength_max.to_value(u.nm), 1) * u.nm
+            np.arange(wavelength_min.to_value(u.nm), wavelength_max.to_value(u.nm), 1)
+            * u.nm
         )
-        aod_units = len(wavelength_range) * [u.dimensionless_unscaled]
+        aod_units = len(wavelength_range) * [1 * u.dimensionless_unscaled]
         rayleigh_extinction_table = Table(names=wavelength_range, units=aod_units)
         col_alt_max = Column(name="altitude_max", unit=u.km)
         col_alt_min = Column(name="altitude_min", unit=u.km)
-        rayleigh_extinction_table.add_columns([col_alt_max, col_alt_min], indexes=[0, 0])
+        rayleigh_extinction_table.add_columns(
+            [col_alt_max, col_alt_min], indexes=[0, 0]
+        )
         aod_dict = {
             aod: 0
-            for aod in np.arange(wavelength_min.to_value(u.nm), wavelength_max.to_value(u.nm))
+            for aod in np.arange(
+                wavelength_min.to_value(u.nm), wavelength_max.to_value(u.nm)
+            )
         }
         for row in t[mask]:
             new_row = []
             new_row.append(row["altitude"])
             new_row.append(row["altitude"] - row["bin_widths"])
             for wavelength in wavelength_range:
                 rayleigh = Rayleigh(
@@ -502,64 +551,82 @@
                     row["relative_humidity"],
                 )
                 beta = rayleigh.beta
                 aod = row["bin_widths"] * beta
                 aod_dict[wavelength.to_value(u.nm)] += aod
                 new_row.append(aod_dict[wavelength.to_value(u.nm)])
             rayleigh_extinction_table.add_row(new_row)
-        rayleigh_extinction_table.write(rayleigh_extinction_file, overwrite=True)
+        _write(rayleigh_extinction_table, rayleigh_extinction_file)
         return rayleigh_extinction_file
 
-    def convert_to_simtel_compatible(self, input_ecsv_file, output_file, observation_altitude):
+    # pylint: enable=too-many-arguments,too-many-locals
+
+    def convert_to_simtel_compatible(
+        self, input_ecsv_file, output_file, observation_altitude
+    ):
         """
-        Converts an ecsv file of an extinction profile to a format digestible by sim_telarray.
+        Converts extinction profile from ``ecsv`` to ``sim_telarray``-compatible format.
+
         Parameters:
         -----------
         input_ecsv_file : string
             Name of the input extinction profile file in ecsv format.
         output_file : string
-            Name of the output extinction profile file in simtel digestible format.
+            Name of the output extinction profile file in simtel-compatible format.
         observation_altitude : quantity
             Starting altitude measured from sea level.
         """
         extinction_table = QTable.read(input_ecsv_file)
-        with open(output_file, "w") as f:
+        with open(output_file, "w", encoding="utf-8") as f:
             H2 = observation_altitude.to_value(u.km)
             H1 = extinction_table["altitude_max"].to_value(u.km)
             list_of_altitude_bins = f"# H2= {H2:.3f}, H1= "
             for height in H1:
                 list_of_altitude_bins += f"{height:.3f}\t"
             list_of_altitude_bins += "\n"
             f.writelines(list_of_altitude_bins)
             for wl in extinction_table.columns:
                 if wl not in ("altitude_max", "altitude_min"):
-                    file_line = [str(wl).split(" ")[0], "\t"]
+                    file_line = [str(wl).split(" ", maxsplit=1)[0], "\t"]
                     for aod in extinction_table[wl]:
                         file_line += [f"{aod:.6f}", "\t"]
                     file_line += ["\n"]
                     f.writelines(file_line)
 
-    def timeseries_analysis(self, outfile, altitude_list=STD_CORSIKA_ALTITUDE_PROFILE):
+    # pylint: disable=too-many-locals
+    def timeseries_analysis(
+        self,
+        outfile,
+        altitude_list=STD_CORSIKA_ALTITUDE_PROFILE,
+        m_floor=1 * u.km,
+        m_ceiling=20 * u.km,
+    ):
         """
         Analyses timeseries of meteorological data.
-        It produces an astropy table with the scaled exponential density at 15km a.s.l. as a function of the MJD.
+        It produces an astropy table with the scaled exponential density at 15km a.s.l.
+        as a function of the MJD.
         This timeseries is used for the identification of seasons.
+
+        Parameters
+        ----------
         outfile : string
             Name of the produced file where the table is stored.
         altitude_list : Quantity
-            Tuple with the altitudes that the atmospheric parameters will be calculated. Units of length.
+            Tuple with the altitudes that the atmospheric parameters will be calculated.
+            Units of length.
+        m_floor: Quantity
+            Lowest altitude considered in calculations.
+        m_ceiling: Quantity
+            Highest altitude considered in calculations.
         """
 
-        output_table = QTable()
         tables = []
-        floor = 1 * u.km
-        ceiling = 20 * u.km
         altitude = altitude_list[
-            (altitude_list.to_value() >= floor.to_value(altitude_list.unit))
-            & (altitude_list.to_value() < ceiling.to_value(altitude_list.unit))
+            (altitude_list.to_value() >= m_floor.to_value(altitude_list.unit))
+            & (altitude_list.to_value() < m_ceiling.to_value(altitude_list.unit))
         ]
 
         self.data["MJD"] = self.data["Timestamp"].mjd
         test_table = self.data.group_by("MJD")
         indices = test_table.groups.indices
         for first, second in zip(indices, indices[1:]):
             t = test_table[first:second]
@@ -572,8 +639,11 @@
                 * u.dimensionless_unscaled
             )
             current_table = QTable([n_exp, altitude], names=("n_exp", "altitude"))
             current_table["mjd"] = t["MJD"][1]
             mask = current_table["altitude"] == 15000 * u.m
             tables.append(current_table[mask])
         output_table = vstack(tables)
-        output_table.write(outfile, overwrite=True)
+        _write(output_table, outfile)
+        del tables
+
+    # pylint: enable=too-many-locals
```

### Comparing `molecularprofiles-0.5.7/src/molecularprofiles/utils/constants.py` & `molecularprofiles-1.0.0/src/molecularprofiles/utils/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Constants definitions."""
+
 import astropy.units as u
 from astropy.constants import N_A
 
 # standard atmosphere thermodynamic values
 STD_NUMBER_DENSITY = (
     2.546899e19 / u.cm**3
 )  # [cm^-3] molecular number density for standard air conditions
```

### Comparing `molecularprofiles-0.5.7/src/molecularprofiles/utils/grib_utils.py` & `molecularprofiles-1.0.0/src/molecularprofiles/utils/grib_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     astropy.units.Quantity [u.m]
         Real altitude as fGeoidOffset.
     """
 
     lat = (np.asarray(latitude) * latitude.unit).to_value(u.rad)
     return (
         (1.0 + 0.002644 * np.cos(2 * lat)) * (geopotential_height)
-        + (1 + 0.0089 * np.cos(2 * lat)) * ((geopotential_height) ** 2 / STD_EARTH_RADIUS.to(u.m))
+        + (1 + 0.0089 * np.cos(2 * lat))
+        * ((geopotential_height) ** 2 / STD_EARTH_RADIUS.to(u.m))
     ).to(u.m)
 
 
 def get_gribfile_variables(filename):
     """
     Returns all the different variable names in a grib file.
 
@@ -69,109 +70,83 @@
     list
         varshortname (str): variable short names.
     """
     logger.debug("Opening %s grib file", filename)
     with pg.open(filename) as grib_file:
         varshortname = []
         varname = []
-        grib_file.read(10)[0]
+        grib_file.read(10)[0]  # pylint: disable=expression-not-assigned
         while True:
             v = grib_file.read(1)[0]
             variable_name = v.name.replace(" ", "")
             variable_short_name = v.shortName
             if variable_name not in varname:
                 varname.append(variable_name)
                 varshortname.append(variable_short_name)
             else:
                 break
     return varname, varshortname
 
 
-def get_plevels(atmo_parameter):
-    """
-    The measurements of atmospheres parameters are taking place in various pressure levels.
-    This functions returns the indices of these levels where we have measurements
-    for the given atmospheric parameter.
-    E.g. for GDAS data that should be a range of values [1, 23].
-
-    Parameters
-    ----------
-    atmo_parameter : str FIXME: this description doesn't
-        Atmospheric parameter from grib file.
-
-    Returns
-    -------
-    list
-        List (int) with the indices of the pressure levels
-    """
-
-    plevels = []
-    index = []
-    for i in range(len(atmo_parameter)):
-        pressure_level = atmo_parameter[i].level
-        if pressure_level not in plevels:
-            plevels.append(pressure_level)
-            index.append(i + 1)
-        else:
-            break
-    return index
-
-
 def create_table(grib_var):
     """
     Create astropy.table.Table from grib record
 
     Parameters
     ----------
     grib_var :
         Grib data record
 
      Returns
      -------
      astropy.table.Table
          Table with the different measurables together with their dimensions
     """
-    res = Table()
+    tables = []
     for v in grib_var:
         unit = u.Unit(v.units)
         timestamp = Time(
-            {"year": v.year, "month": v.month, "day": v.day, "hour": v.hour}, scale="utc"
+            {"year": v.year, "month": v.month, "day": v.day, "hour": v.hour},
+            scale="utc",
         )
         pressure_level = v.level * u.hPa
         latitudes = Latitude(v.latlons()[0].ravel() * u.deg)
         longitudes = Longitude(v.latlons()[1].ravel() * u.deg, wrap_angle=180 * u.deg)
         if isinstance(v.values, float):
             vals = np.array([v.values]) * unit
         else:
             vals = v.values.ravel() * unit
         t = Table([latitudes, longitudes], names=["Latitude", "Longitude"])
         t["Timestamp"] = timestamp
         t["Pressure"] = pressure_level
         t[v.name] = vals
-        res = vstack([res, t])
+        tables.append(t)
+    res = Table(vstack(tables), masked=True)
+    del tables
     return res
 
 
 def get_grib_file_data(filename):
     """
     This function opens a grib file, selects the parameters
     (all available: Temperature, Geopotential, RH, ...),
     and creates an astropy.table.Table with them.
+
     Parameters
     ----------
     filename : str
         Path to the grib file.
 
     Returns
     -------
     astropy.table.Table
         Table with grib file data gridded in isobaric levels
     """
 
-    variable_names, variable_short_names = get_gribfile_variables(filename)
+    _, variable_short_names = get_gribfile_variables(filename)
     grib_file = pg.open(filename)
     gpm = u.def_unit("gpm", u.m)
     u.add_enabled_units([gpm])
     data = Table()
     for short_name in variable_short_names:
         if short_name == "unknown":
             continue
@@ -186,24 +161,28 @@
         else:
             data = join(data, t, join_type="outer")
     return data
 
 
 def extend_grib_data(data):
     """
-    Extends grib data table by filling the gaps in data and calculating additional quantities:
-        - altitude
-        - density
-        - exponential density
-        - wind direction
+    Extends grib data table.
+
+    Extends grib data table by filling the gaps in data
+    and calculating additional quantities:
+    - altitude
+    - density
+    - exponential density
+    - wind direction
 
     Parameters
     ----------
     astropy.table.Table
         Table with grib data
+
     Returns
     -------
     astropy.table.Table
         Extended table with grib data and additional quantities
     """
 
     logger.debug("Check for gaps in relative humidity and fill them if neccessary")
@@ -211,36 +190,41 @@
     logger.debug("Compute altitude from geopotential")
     if "Geopotential height" in data.keys():
         data["Altitude"] = get_altitude_from_geopotential_height(
             data["Geopotential height"], data["Latitude"]
         )
     else:
         data["Altitude"] = get_altitude_from_geopotential_height(
-            data["Geopotential"].quantity / STD_GRAVITATIONAL_ACCELERATION, data["Latitude"]
+            data["Geopotential"].quantity / STD_GRAVITATIONAL_ACCELERATION,
+            data["Latitude"],
         )
     logger.debug("Compute density")
     data["Density"] = (
         STD_NUMBER_DENSITY
         * data["Pressure"]
         / STD_AIR_PRESSURE
         * STD_AIR_TEMPERATURE
         / data["Temperature"]
     )
     logger.debug("Compute exponential density")
     data["Exponential Density"] = (
-        data["Density"] / STD_NUMBER_DENSITY * np.exp(data["Altitude"] / DENSITY_SCALE_HEIGHT)
+        data["Density"]
+        / STD_NUMBER_DENSITY
+        * np.exp(data["Altitude"] / DENSITY_SCALE_HEIGHT)
     )
     logger.debug("Compute wind speed")
     data["Wind Speed"] = np.sqrt(
         data["U component of wind"] ** 2 + data["V component of wind"] ** 2
     )
     logger.debug("Compute wind direction")
     data["Wind Direction"] = Angle(
         np.array(
-            np.arctan2(-data["V component of wind"].value, -data["U component of wind"].value)
+            np.arctan2(
+                -data["V component of wind"].value, -data["U component of wind"].value
+            )
         ),
         unit=u.rad,
     ).wrap_at(360 * u.deg)
     return data
 
 
 def save_grib_table(data, filename, fmt="ecsv"):
```

### Comparing `molecularprofiles-0.5.7/src/molecularprofiles/utils/humidity.py` & `molecularprofiles-1.0.0/src/molecularprofiles/utils/humidity.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     Notes
     -----
     Implemented according to Eq. 5 of [1]_. Notation and constants according to
     Eq. 16 of [2]_.
 
     References
     ----------
-    .. [1] R.S. Davis, "Equation for the determination of the density of moist air" Metrologia, 29 (1992) 67-70
+    .. [1] R.S. Davis, "Equation for the determination of the density of moist air"
+       Metrologia, 29 (1992) 67-70
     .. [2] C. Tomasi, V. Vitale, B. Petkov, A. Lupi, A. Cacciari "Improved algorithm
        for calculations of Rayleigh-scattering optical depth in standard atmospheres",
        Applied Optics 44 Nr. 16 (2005) 3320
     """
     p = pressure.to(u.Pa)
     T = temperature.to(u.K, equivalencies=u.temperature())
     a_0 = 1.58123e-6 * u.K / u.Pa
@@ -96,19 +97,19 @@
     ----------
     .. [1] C. Tomasi, V. Vitale, B. Petkov, A. Lupi, A. Cacciari "Improved algorithm
        for calculations of Rayleigh-scattering optical depth in standard atmospheres",
        Applied Optics 44 Nr. 16 (2005) 3320
     """
     p = pressure.to(u.Pa)
     T = temperature.to(u.K, equivalencies=u.temperature())
-    return (1.00062 + 3.14e-8 * p / u.Pa + 5.6e-7 * (T - 273.15 * u.K) ** 2 / u.K**2).to_value()
+    return (
+        1.00062 + 3.14e-8 * p / u.Pa + 5.6e-7 * (T - 273.15 * u.K) ** 2 / u.K**2
+    ).to_value()
 
 
-# TODO: This function needs a simple unit test to check which function is called
-# TODO: Goff-Gratch doesn't seem to be as good as Buck, or maybe Wexler
 def saturation_vapor_pressure(temperature):
     """
     Calculates the vapor pressure at saturation.
 
     Parameters
     ----------
     temperature : astropy.units.Quantity
@@ -122,15 +123,16 @@
     Notes
     -----
     In case temperatures above 0 deg C it follows [1]_, see also Eq. 15 in [2]_.
     Otherwise, Goff-Gratch equation (Eq. 1 in [3]_) is used.
 
     References
     ----------
-    .. [1] R.S. Davis, "Equation for the determination of the density of moist air" Metrologia, 29 (1992) 67-70
+    .. [1] R.S. Davis, "Equation for the determination of the density of moist air"
+       Metrologia, 29 (1992) 67-70
     .. [2] C. Tomasi, V. Vitale, B. Petkov, A. Lupi, A. Cacciari "Improved algorithm
        for calculations of Rayleigh-scattering optical depth in standard atmospheres",
        Applied Optics 44 Nr. 16 (2005) 3320
     .. [3] http://cires.colorado.edu/~voemel/vp.html
     """
     T = temperature.to(u.K, equivalencies=u.temperature())
     mask = T > 273.15 * u.K
@@ -142,15 +144,17 @@
             + 33.93711047
             - 6343.1645 * u.K / T[mask]
         )
         / 100.0
         # * u.Pa
     )
 
-    theta = (373.16 * u.K / T[~mask]).to_value()  # ratio of steam point (100 deg C) to temperature
+    theta = (
+        373.16 * u.K / T[~mask]
+    ).to_value()  # ratio of steam point (100 deg C) to temperature
     res[~mask] = (
         np.power(
             10,
             (
                 -7.90298 * (theta - 1)
                 + 5.02808 * np.log10(theta)
                 - 1.3816e-7 * (np.power(10, 11.344 * (1 - 1 / theta)) - 1)
@@ -160,15 +164,15 @@
         )
         # * u.hPa
     )
 
     return res * u.hPa
 
 
-# TODO: Check this function and write unit test
+# pylint: disable=too-many-locals
 def saturation_vapor_pressure_over_water(temperature):
     """
     Calculates the vapor pressure at saturation over water.
 
     Parameters
     ----------
     temperature : astropy.units.Quantity
@@ -210,15 +214,17 @@
     a = omega**2 + k_1 * omega + k_2
     b = k_3 * omega**2 + k_4 * omega + k_5
     c = k_6 * omega**2 + k_7 * omega + k_8
     x = -b + np.sqrt(b**2 - 4 * a * c)
     return 1e6 * np.power(2 * c / x, 4) * u.Pa
 
 
-# TODO: Check this function and write unit test
+# pylint: enable=too-many-locals
+
+
 def saturation_vapor_pressure_over_ice(temperature):
     """
     Calculates the vapor pressure at saturation over ice.
 
     Parameters
     ----------
     temperature: astropy.units.Quantity
@@ -240,15 +246,17 @@
        range -100 deg. C to 100 deg. C for use with the 1997 NIST/ASME steam tables"
        Papers and abstracts from the third international symposium on humidity and
        moisture, Vol. 1, p. 69-76, National Physical Laboratory, Teddington,
        Middlesex, UK, April 1998.
     .. [2] http://cires.colorado.edu/~voemel/vp.html
     .. [3] https://emtoolbox.nist.gov/wavelength/documentation.asp#AppendixA
     """
-    theta = temperature.to(u.K, equivalencies=u.temperature()) / 273.16 * u.K
+    theta = (
+        temperature.to(u.K, equivalencies=u.temperature()) / 273.16 * u.K
+    ).to_value()
     a_1 = -13.928169
     a_2 = 34.7078238
     y = a_1 * (1 - np.power(theta, -1.5)) + a_2 * (1 - np.power(theta, -1.25))
     return 611.657 * np.exp(y) * u.Pa
 
 
 def molar_fraction_water_vapor(pressure, temperature, relative_humidity):
@@ -278,15 +286,17 @@
     .. [1] C. Tomasi, V. Vitale, B. Petkov, A. Lupi, A. Cacciari
        "Improved algorithm for calculations of Rayleigh-scattering optical depth
        in standard atmospheres", Applied Optics 44 Nr. 16 (2005) 3320
     """
     factor = enhancement_factor(pressure, temperature)
     psv = saturation_vapor_pressure(temperature)
     return (
-        factor * relative_humidity.to(u.dimensionless_unscaled) * (psv / pressure).decompose()
+        factor
+        * relative_humidity.to(u.dimensionless_unscaled)
+        * (psv / pressure).decompose()
     ).to_value()
 
 
 def density_moist_air(pressure, temperature, moist_air_compressibility, x_w, co2_bkg):
     """
     Density equation of moist air, according to Eq. 1 of [1]_.
 
@@ -317,20 +327,23 @@
     m_w = MOLAR_MASS_WATER_VAPOR
     m_a = (
         1e-3 * (28.9635 + 12.011e-6 * (co2_bkg - 400)) * u.kg / u.mol
     )  # molar mass of dry air [kg/mol]
     return (
         pressure.to(u.Pa)
         * m_a
-        / (moist_air_compressibility * R * temperature.to(u.K, equivalencies=u.temperature()))
+        / (
+            moist_air_compressibility
+            * R
+            * temperature.to(u.K, equivalencies=u.temperature())
+        )
         * (1 - x_w * (1 - m_w / m_a))
     ).decompose()  # Tomasi eq. 12
 
 
-# TODO: This function has no unit test
 def partial_pressure_water_vapor(temperature, relative_humidity):
     """
     Calculates the partial pressure of water vapor in the air.
 
     Parameters
     ----------
     temperature : astropy.units.Quantity
@@ -339,8 +352,10 @@
         Relative humidity
 
     Returns
     -------
     astropy.units.Quantity
         Water vapor partial pressure
     """
-    return relative_humidity.to(u.dimensionless_unscaled) * saturation_vapor_pressure(temperature)
+    return relative_humidity.to(u.dimensionless_unscaled) * saturation_vapor_pressure(
+        temperature
+    )
```

### Comparing `molecularprofiles-0.5.7/src/molecularprofiles/utils/rayleigh.py` & `molecularprofiles-1.0.0/src/molecularprofiles/utils/rayleigh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+Calculates properties related to Rayleigh scattering.
+
+Adapted from MRayleigh, written by Markus Gaug <markus.gaug@uab.cat>, 04/2013
+.. moduleauthor:: Scott Griffiths <sgriffiths@ifae.es>
+"""
+
 import functools
 import numpy as np
 import astropy.units as u
 from molecularprofiles.utils import humidity
 from molecularprofiles.utils.constants import (
     STD_NUMBER_DENSITY,
     STD_AIR_PRESSURE,
@@ -11,16 +18,19 @@
     OXYGEN_RATIO,
     ARGON_RATIO,
     GAS_CONSTANT,
 )
 
 
 class Rayleigh:
+    # pylint: disable=line-too-long
     """
-    A small Rayleigh-scattering program based on:
+    A small Rayleigh-scattering program.
+
+    Computations are based on:
     C. Tomasi, V. Vitale, B. Petkov, A. Lupi, A. Cacciari
     "Improved algorithm for calculations of Rayleigh-scattering optical
     depth in standard atmospheres"
     Applied Optics 44 Nr. 16 (2005) 3320
 
     The calculation of refractive index is based on:
     P.E. Ciddor, "Refractive index of air: new equations for hte visible and near infrared",
@@ -37,19 +47,18 @@
     J. Atmosph. Osceanic Technol. 16 (1999) 1854
 
     The calculation of the Chandrasekhar phase function is based on:
     S. Chandrasekhar, Radiative Transfer, Dover Publications, 1960.
 
     E.J. McCartney, "Optics of the Atmosphere. Scattering by Molecules and Particles"
     Wiley & Sons, New York, 1977.
-
-    Adapted from MRayleigh, written by Markus Gaug <markus.gaug@uab.cat>, 04/2013
-    .. moduleauthor:: Scott Griffiths <sgriffiths@ifae.es>
     """
+    # pylint: enable=line-too-long
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         wavelength,
         co2_bkg,
         pressure=STD_AIR_PRESSURE,
         temperature=STD_AIR_TEMPERATURE,
         relative_humidity=STD_RELATIVE_HUMIDITY,
@@ -68,34 +77,34 @@
         temperature : astropy.units.Quantity
             Air temperature
         relative_humidity : astropy.units.Quantity
             Relative humidity [%]
         """
         # check inputs for bad values
         if np.any(wavelength < 200 * u.nm) or np.any(wavelength > 4000 * u.nm):
-            raise ValueError("Wavelength range only from 200 nm - 4 micrometer allowed.")
+            raise ValueError(
+                "Wavelength range only from 200 nm - 4 micrometer allowed."
+            )
         if np.any(pressure < 0 * u.hPa) or np.any(pressure > 1400 * u.hPa):
             raise ValueError("Pressure only in range 0 - 1400 hPa allowed.")
         if np.any(temperature < 150 * u.K) or np.any(temperature > 400 * u.K):
             raise ValueError("Temperatures only in range 150 - 400 K allowed.")
-        # if np.any(relative_humidity < 0) or np.any(relative_humidity > 100 * u.percent):
-        #    raise ValueError("Relative humity must lie between 0 - 100.")
-        # FIXME: Relative humidity can exceed 100%, in case of supersaturated air.
-        # The maximum limit should be thought better. However relative humidity cannot go negative.
-        # If we receive negative values it is most probably due to interpolation problems.
-        # Till we fix these issues it is better to comment out the minimum limit.
         if co2_bkg < 200 or co2_bkg > 1000:
-            raise ValueError("CO2 concentrations only in range 200 - 1000 ppmv allowed.")
+            raise ValueError(
+                "CO2 concentrations only in range 200 - 1000 ppmv allowed."
+            )
 
         self.wavelength = wavelength.to(u.nm)
         self.pressure = pressure.to(u.hPa)
         self.temperature = temperature.to(u.K, equivalencies=u.temperature())
         self.relative_humidity = relative_humidity.to(u.percent)
         self.co2_bkg = co2_bkg  # [ppmv]  CO2 concentration of air
 
+    # pylint: enable=too-many-arguments
+
     @functools.cached_property
     def molecular_number_density(self):
         """
         Returns
         -------
         astropy.units.Quantity
             Molecular number density [cm^-3]
@@ -175,15 +184,17 @@
         References
         ----------
         .. [1] C. Tomasi, V. Vitale, B. Petkov, A. Lupi, A. Cacciari
            "Improved algorithm for calculations of Rayleigh-scattering optical depth
            in standard atmospheres", Applied Optics 44 Nr. 16 (2005) 3320
         """
         return (
-            (self.molecular_number_density * self.scattering_cross_section).decompose().to(1 / u.km)
+            (self.molecular_number_density * self.scattering_cross_section)
+            .decompose()
+            .to(1 / u.km)
         )
 
     @functools.cached_property
     def refractive_index(self):
         """
         Ciddor formula for calculation of refractive index in moist air.
         The obtained refractive index is precise to 1e-7.
@@ -241,18 +252,23 @@
         )  # compressibility of pure water vapor
         compressibility_moist_air = humidity.compressibility(
             self.pressure, self.temperature, molar_fraction_water_vapour
         )  # compressibility of moist air
 
         # density of dry air at standard p and T
         dry_air_density_stdpt = humidity.density_moist_air(
-            STD_AIR_PRESSURE, STD_AIR_TEMPERATURE, compressibility_dry_air, 0, self.co2_bkg
+            STD_AIR_PRESSURE,
+            STD_AIR_TEMPERATURE,
+            compressibility_dry_air,
+            0,
+            self.co2_bkg,
         )
 
-        # density of pure water vapor at at standard T and e (T* = 293.15 K = 20 C, and e* = 1333 Pa)
+        # density of pure water vapor at at standard T and e
+        # (T* = 293.15 K = 20 C, and e* = 1333 Pa)
         water_vapour_density_stdpt = humidity.density_moist_air(
             1333 * u.Pa, 293.15 * u.K, compressibility_water_vapour, 1, self.co2_bkg
         )
 
         # density of the dry component of moist air
         density_dry_comp_moist_air = (
             self.pressure
@@ -310,15 +326,17 @@
             + 1.448e-4 / self.wavelength.to_value(u.micron) ** 4
         )  # partial King factor for O2 molecules
         king_factor_ar = 1.00  # partial King factor for Ar molecules
         king_factor_co2 = 1.15  # partial King factor for CO2 molecules
         king_factor_wv = 1.001  # partial King factor for water vapor
 
         co2_ratio = 1e-6 * self.co2_bkg  # CO2
-        water_vapour_ratio = (water_vapour_partial_pressure / self.pressure).decompose().to_value()
+        water_vapour_ratio = (
+            (water_vapour_partial_pressure / self.pressure).decompose().to_value()
+        )
 
         return (
             NITROGEN_RATIO * king_factor_n2
             + OXYGEN_RATIO * king_factor_o2
             + ARGON_RATIO * king_factor_ar
             + co2_ratio * king_factor_co2
             + water_vapour_ratio * king_factor_wv
@@ -363,15 +381,14 @@
         rho = self.depolarization
 
         # need to solve Chandrasekhar eq. 254 for gamma as a function of rho
         f_1 = (2 + 2 * rho) / (2 + rho)
         f_2 = (1 - rho) / (1 + rho)
         return 0.75 * f_1 * (1 + f_2 * np.cos(angle) ** 2)  # Chandrasekhar eq. 255
 
-    # TODO: where does this come from? Needs unit test
     def back_scattering_coefficient(self, angle):
         """
         Back-scattering coefficient for a given scattering angle.
 
         Parameters
         ----------
         angle : astropy.units.Quantity
```

### Comparing `molecularprofiles-0.5.7/src/molecularprofiles.egg-info/PKG-INFO` & `molecularprofiles-1.0.0/src/molecularprofiles.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularprofiles
-Version: 0.5.7
+Version: 1.0.0
 Summary: Meteorological data analysis suite
 Author-email: Pere Munar Adrover <pere.munar@uab.cat>, Markus Gaug <markus.gaug@uab.cat>, Scott Griffiths <sgriffiths@ifae.es>, Georgios Voutsinas <georgios.voutsinas@unige.ch>, Mykhailo Dalchenko <mykhailo.dalchenko@unige.ch>
 License: Copyright (c) 2020, Molecularprofiles Project
         
         Redistribution and use in source and binary forms, with or withoutmodification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -15,48 +15,61 @@
         
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
         THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
         IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
         (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
         HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
         ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
 Project-URL: Home, https://gitlab.cta-observatory.org/cta-array-elements/ccf/mdps
+Project-URL: Doc, http://cta-array-elements.gitlab-pages.cta-observatory.org/ccf/MDPs/
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: astropy
 Requires-Dist: pygrib
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pylint>=2.15; extra == "test"
 Requires-Dist: black>=22.5; extra == "test"
-Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: coverage-badge; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: numpydoc; extra == "doc"
+Requires-Dist: pydata-sphinx-theme; extra == "doc"
+Requires-Dist: myst-parser<2.0.0; extra == "doc"
+Requires-Dist: sphinx-paramlinks; extra == "doc"
+Requires-Dist: sphinx-argparse; extra == "doc"
 Requires-Dist: nbsphinx; extra == "doc"
-Requires-Dist: sphinx_rtd_theme; extra == "doc"
-Requires-Dist: myst-parser; extra == "doc"
 Requires-Dist: linkify-it-py; extra == "doc"
-Requires-Dist: sphinx-argparse; extra == "doc"
-Requires-Dist: sphinx-paramlinks; extra == "doc"
+Requires-Dist: ipykernel; extra == "doc"
+Provides-Extra: dev
+Requires-Dist: setuptools_scm; extra == "dev"
 
 # molecularprofiles
 
-!! OBSOLETE !! 
-Will be updated upon availability of CI configuration
-
-See the documentation here: https://molecularprofiles.readthedocs.io/en/latest/
-
-functions to plot and work with meteorological data in grib2 format from ECMWF and GDAS. This work is used for the calibration of the CTA
-
-https://github.com/cambecc/grib2json
-
-In order to install it go to the directory containing the file setup.py and type:
+A collection of routines to read an analyze meteorological data in `grib2` format.
 
-pip install ./
+See [project documentation](http://cta-array-elements.gitlab-pages.cta-observatory.org/ccf/MDPs/) for API docs.
 
+## Development installation:
 
+- Clone the code with git:
+  ```shell
+  > git clone https://gitlab.cta-observatory.org/cta-array-elements/ccf/mdps.git
+  ```
+- Checkout an appropriate branch (currently, dev branch contains the most recent code):
+  ```shell
+  git checkout -b <branch_name>
+  ```
+- Use `mamba` to setup a clean environment
+  ```shell
+  > mamba create -n molecularprofiles -c conda-forge python==3.12
+  > mamba activate molecularprofiles
+  ```
+- Install molecularprofiles in editable mode with test dependencies:
+  ```shell
+  > pip install -e.[test,doc,dev]
+  ```
```

### Comparing `molecularprofiles-0.5.7/src/molecularprofiles.egg-info/SOURCES.txt` & `molecularprofiles-1.0.0/src/molecularprofiles.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,13 +4,17 @@
 src/molecularprofiles/__init__.py
 src/molecularprofiles/molecularprofiles.py
 src/molecularprofiles.egg-info/PKG-INFO
 src/molecularprofiles.egg-info/SOURCES.txt
 src/molecularprofiles.egg-info/dependency_links.txt
 src/molecularprofiles.egg-info/requires.txt
 src/molecularprofiles.egg-info/top_level.txt
+src/molecularprofiles/tests/test_grib_utils.py
+src/molecularprofiles/tests/test_humidity.py
+src/molecularprofiles/tests/test_molecular_profiles.py
+src/molecularprofiles/tests/test_rayleigh.py
 src/molecularprofiles/utils/__init__.py
 src/molecularprofiles/utils/constants.py
 src/molecularprofiles/utils/grib_utils.py
 src/molecularprofiles/utils/humidity.py
 src/molecularprofiles/utils/mdps_log.conf
 src/molecularprofiles/utils/rayleigh.py
```

