# Comparing `tmp/BlueDesc_pywrapper-0.0.4.tar.gz` & `tmp/bluedesc_pywrapper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlueDesc_pywrapper-0.0.4.tar", last modified: Wed Aug  9 06:56:39 2023, max compression
+gzip compressed data, was "bluedesc_pywrapper-0.0.5.tar", last modified: Fri May 10 17:09:54 2024, max compression
```

## Comparing `BlueDesc_pywrapper-0.0.4.tar` & `bluedesc_pywrapper-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-09 06:56:39.417555 BlueDesc_pywrapper-0.0.4/
--rw-rw-rw-   0        0        0     1100 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3151 2023-08-09 06:56:39.417555 BlueDesc_pywrapper-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2218 2023-07-14 13:15:51.000000 BlueDesc_pywrapper-0.0.4/README.md
--rw-rw-rw-   0        0        0     1361 2023-08-09 06:56:39.419558 BlueDesc_pywrapper-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-09 06:56:39.360324 BlueDesc_pywrapper-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-08-09 06:56:39.396525 BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper/
--rw-rw-rw-   0        0        0      142 2023-08-09 06:55:48.000000 BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper/__init__.py
--rw-rw-rw-   0        0        0     9636 2023-08-09 06:55:16.000000 BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper/bluedesc_pywrapper.py
--rw-rw-rw-   0        0        0    36313 2023-07-14 12:26:42.000000 BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper/descs.json
--rw-rw-rw-   0        0        0     3450 2023-06-27 13:36:16.000000 BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper/dtypes.json
--rw-rw-rw-   0        0        0     3040 2023-06-27 11:18:36.000000 BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-09 06:56:39.410045 BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper.egg-info/
--rw-rw-rw-   0        0        0     3151 2023-08-09 06:56:39.000000 BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-08-09 06:56:39.000000 BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-09 06:56:39.000000 BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      172 2023-08-09 06:56:39.000000 BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-08-09 06:56:39.000000 BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-09 06:56:39.415046 BlueDesc_pywrapper-0.0.4/tests/
--rw-rw-rw-   0        0        0     2021 2023-07-14 13:08:16.000000 BlueDesc_pywrapper-0.0.4/tests/test_descriptors.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:09:54.275822 bluedesc_pywrapper-0.0.5/
+-rw-rw-rw-   0        0        0     1100 2023-06-27 11:18:36.000000 bluedesc_pywrapper-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3566 2024-05-10 17:09:54.275822 bluedesc_pywrapper-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2217 2023-08-11 12:16:36.000000 bluedesc_pywrapper-0.0.5/README.md
+-rw-rw-rw-   0        0        0     1361 2024-05-10 17:09:54.275822 bluedesc_pywrapper-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-06-27 11:18:36.000000 bluedesc_pywrapper-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:09:54.244195 bluedesc_pywrapper-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 17:09:54.244195 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/
+-rw-rw-rw-   0        0        0      142 2024-05-10 17:09:07.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/__init__.py
+-rw-rw-rw-   0        0        0    10509 2024-05-09 19:50:00.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/bluedesc_pywrapper.py
+-rw-rw-rw-   0        0        0    36313 2023-07-14 12:26:42.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/descs.json
+-rw-rw-rw-   0        0        0     3450 2023-06-27 13:36:16.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/dtypes.json
+-rw-rw-rw-   0        0        0     3040 2023-06-27 11:18:36.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 17:09:54.266806 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper.egg-info/
+-rw-rw-rw-   0        0        0     3566 2024-05-10 17:09:54.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2024-05-10 17:09:54.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 17:09:54.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      172 2024-05-10 17:09:54.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-10 17:09:54.000000 bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 17:09:54.266806 bluedesc_pywrapper-0.0.5/tests/
+-rw-rw-rw-   0        0        0     2021 2023-07-14 13:08:16.000000 bluedesc_pywrapper-0.0.5/tests/test_descriptors.py
```

### Comparing `BlueDesc_pywrapper-0.0.4/LICENSE` & `bluedesc_pywrapper-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.4/PKG-INFO` & `bluedesc_pywrapper-0.0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: BlueDesc_pywrapper
-Version: 0.0.4
-Summary: Python wrapper for BlueDesc molecular descriptors
-Home-page: https://github.com/OlivierBeq/bluedesc_pywrapper
-Author: Olivier J. M. Béquignon
-Author-email: "olivier.bequignon.maintainer@gmail.com"
-Maintainer: Olivier J. M. Béquignon
-Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
-Keywords: BlueDesc,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: testing
-License-File: LICENSE
-
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 # Python wrapper for BlueDesc molecular descriptors
 
 ## Installation
 
 From source:
@@ -79,15 +57,15 @@
 
 ## Documentation
 
 ```python
 def calculate(mols, show_banner=True, njobs=1, chunksize=1000):
 ```
 
-Default method to calculate BlueDesc fingerprints.
+Default method to calculate BlueDesc descriptors.
 
 Parameters:
 
 - ***mols  : Iterable[Chem.Mol]***  
   RDKit molecule objects for which to obtain BlueDesc descriptors.
 - ***show_banner  : bool***  
   Displays default notice about BlueDesc.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `BlueDesc_pywrapper-0.0.4/setup.cfg` & `bluedesc_pywrapper-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper/bluedesc_pywrapper.py` & `bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/bluedesc_pywrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -115,56 +115,70 @@
                     if needsHs(mol):
                         warnings.warn('Molecule lacks hydrogen atoms: this might affect the value of calculated descriptors')
                     # Are molecules 3D
                     if self.include_3D:
                         confs = list(mol.GetConformers())
                         if not (len(confs) > 0 and confs[-1].Is3D()):
                             raise ValueError('Cannot calculate the 3D descriptors of a conformer-less molecule')
+                    mol.SetProp('index', str(i))
                     writer.write(mol)
                 else:
                     self._skipped.append(i)
                 self.n += 1
             writer.close()
             del block
         except ValueError as e:
             # Free resources and raise error
             writer.close()
             del block
             os.remove(self._tmp_sd)
             raise e from None
         # 3) Create command
         java_path = install_java()
-        command = f"{java_path} -jar {self._jarfile} -f {self._tmp_sd} -l \'?\'"
+        command = f"{java_path} -jar {self._jarfile} -f {self._tmp_sd} -l ?"
         return command
 
     def _cleanup(self) -> None:
         """Cleanup resources used for calculation."""
         # Remove temporary files
         os.remove(self._tmp_sd)
         os.remove(self._out)
         os.remove(f'{self._tmp_sd}.lp.oddescriptors.att')
 
     def _run_command(self, command: str) -> pd.DataFrame:
         """Run the BlueDesc command.
 
         :param command: The command to be run.
         """
-        process = subprocess.run(command.split(), stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+        process = subprocess.run(command.split(), capture_output=True, text=True)
         if process.returncode == 0:
             self._out = f'{self._tmp_sd}.oddescriptors.arff'
             try:
                 values = arff.loadarff(self._out)
                 values = (pd.DataFrame(values[0])
-                          .drop("'?'", axis=1)
+                          .drop("?", axis=1)
                           .rename(columns=lambda x: x.replace('joelib2.feature.types.count.', ''))
                           .rename(columns=lambda x: x.replace('joelib2.feature.types.', ''))
                           )
-                if values.shape[0] != self.n:
-                    warnings.warn('Some molecules were skipped by BlueDesc')
-            except:
+                if values.shape[0] != (self.n - self._skipped):
+                    # Create an empty array
+                    values_ = pd.DataFrame(np.zeros(((self.n - self._skipped), values.shape[1])),
+                                           columns=values.columns)
+                    # Identify skipped molecules
+                    start = process.stdout.find('Sequence of skipped instances:')
+                    skipped = pd.Series(process.stdout[start + 30:].split()).astype(int) - 1
+                    for i in range((self.n - self._skipped)):
+                        if i in skipped.tolist():
+                            values_.iloc[i, :] = np.NaN
+                        else:
+                            values_.iloc[i, :] = values.iloc[0, :]
+                            values = values.iloc[1:, :]
+                    values = values_
+            except Exception as e:
+                raise e
                 details = self.get_details()
                 values = np.zeros((self.n, details.shape[0]))
                 with open(os.path.abspath(os.path.join(__file__, os.pardir, 'dtypes.json'))) as fh:
                     dtypes = json.load(fh)
                 values = pd.DataFrame(values, columns=details.Name.tolist()).astype(dtypes)
             # If only 2D, remove 3D descriptors
             if not self.include_3D:
@@ -192,16 +206,16 @@
         # Insert lines of skipped molecules
         if len(self._skipped):
             results = (pd.DataFrame(np.insert(results.values, self._skipped,
                                               values=[np.NaN] * len(results.columns),
                                               axis=0),
                                     columns=results.columns)
                        )
-        results = (results.apply(pd.to_numeric, errors='coerce', axis=1)
-                          .convert_dtypes()
+        results = (results.apply(pd.to_numeric, errors='ignore', downcast='integer', axis=0)
+                          .apply(pd.to_numeric, errors='ignore', downcast='float', axis=0)
                    )
         return results
 
     def _multiproc_calculate(self, mols: List[Chem.Mol], nbits: int = 1024) -> pd.DataFrame:
         """Calculate BlueDesc descriptors in thread-safe manner.
 
         :param mols: RDKit molecules for which BlueDesc fingerprints should be calculated
```

### Comparing `BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper/descs.json` & `bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/descs.json`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper/dtypes.json` & `bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/dtypes.json`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper/utils.py` & `bluedesc_pywrapper-0.0.5/src/BlueDesc_pywrapper/utils.py`

 * *Files identical despite different names*

### Comparing `BlueDesc_pywrapper-0.0.4/src/BlueDesc_pywrapper.egg-info/PKG-INFO` & `bluedesc_pywrapper-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: BlueDesc-pywrapper
-Version: 0.0.4
+Name: BlueDesc_pywrapper
+Version: 0.0.5
 Summary: Python wrapper for BlueDesc molecular descriptors
 Home-page: https://github.com/OlivierBeq/bluedesc_pywrapper
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: BlueDesc,molecular descriptors,cheminformatics,toxicoinformatics,QSAR
@@ -12,17 +12,29 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: more-itertools
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: rdkit
+Requires-Dist: install-jdk==0.3.0
+Requires-Dist: bounded-pool-executor==0.0.3
+Requires-Dist: BlueDesc
 Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Provides-Extra: testing
-License-File: LICENSE
+Requires-Dist: pytest; extra == "testing"
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 # Python wrapper for BlueDesc molecular descriptors
 
 ## Installation
 
@@ -79,15 +91,15 @@
 
 ## Documentation
 
 ```python
 def calculate(mols, show_banner=True, njobs=1, chunksize=1000):
 ```
 
-Default method to calculate BlueDesc fingerprints.
+Default method to calculate BlueDesc descriptors.
 
 Parameters:
 
 - ***mols  : Iterable[Chem.Mol]***  
   RDKit molecule objects for which to obtain BlueDesc descriptors.
 - ***show_banner  : bool***  
   Displays default notice about BlueDesc.
```

### Comparing `BlueDesc_pywrapper-0.0.4/tests/test_descriptors.py` & `bluedesc_pywrapper-0.0.5/tests/test_descriptors.py`

 * *Files identical despite different names*

