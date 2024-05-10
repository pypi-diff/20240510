# Comparing `tmp/EMAtools-0.1.0.tar.gz` & `tmp/EMAtools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EMAtools-0.1.0.tar", last modified: Thu Mar 14 19:52:00 2024, max compression
+gzip compressed data, was "EMAtools-0.2.0.tar", last modified: Fri May 10 00:19:46 2024, max compression
```

## Comparing `EMAtools-0.1.0.tar` & `EMAtools-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 19:52:00.153513 EMAtools-0.1.0/
--rw-rw-rw-   0        0        0     1090 2024-02-07 18:45:22.000000 EMAtools-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      590 2024-03-14 19:52:00.152541 EMAtools-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    26038 2024-03-04 16:59:29.000000 EMAtools-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-14 19:52:00.153513 EMAtools-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1162 2024-03-14 19:30:06.000000 EMAtools-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:52:00.130888 EMAtools-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-14 19:52:00.151514 EMAtools-0.1.0/src/EMAtools.egg-info/
--rw-rw-rw-   0        0        0      590 2024-03-14 19:52:00.000000 EMAtools-0.1.0/src/EMAtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2024-03-14 19:52:00.000000 EMAtools-0.1.0/src/EMAtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 19:52:00.000000 EMAtools-0.1.0/src/EMAtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-14 19:52:00.000000 EMAtools-0.1.0/src/EMAtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-03-14 19:52:00.000000 EMAtools-0.1.0/src/EMAtools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 19:52:00.146363 EMAtools-0.1.0/src/ema/
-drwxrwxrwx   0        0        0        0 2024-03-14 19:52:00.150532 EMAtools-0.1.0/src/ema/Veelo/
--rw-rw-rw-   0        0        0       18 2024-02-08 14:56:33.000000 EMAtools-0.1.0/src/ema/Veelo/__init__.py
--rw-rw-rw-   0        0        0      869 2024-02-08 14:56:33.000000 EMAtools-0.1.0/src/ema/Veelo/modify_current.py
--rw-rw-rw-   0        0        0     3585 2024-02-08 14:56:33.000000 EMAtools-0.1.0/src/ema/Veelo/preprocess.py
--rw-rw-rw-   0        0        0    25322 2024-02-08 14:56:33.000000 EMAtools-0.1.0/src/ema/Veelo/util.py
--rw-rw-rw-   0        0        0      158 2024-03-03 00:49:08.000000 EMAtools-0.1.0/src/ema/__init__.py
--rw-rw-rw-   0        0        0      314 2024-02-27 23:57:38.000000 EMAtools-0.1.0/src/ema/cin.py
--rw-rw-rw-   0        0        0     4261 2024-03-04 16:59:29.000000 EMAtools-0.1.0/src/ema/emc.py
--rw-rw-rw-   0        0        0     5741 2024-02-29 22:34:30.000000 EMAtools-0.1.0/src/ema/emin.py
--rw-rw-rw-   0        0        0    13142 2024-03-04 21:55:53.000000 EMAtools-0.1.0/src/ema/file.py
--rw-rw-rw-   0        0        0     4487 2024-03-01 19:43:00.000000 EMAtools-0.1.0/src/ema/inp.py
--rw-rw-rw-   0        0        0     6953 2024-03-04 21:55:53.000000 EMAtools-0.1.0/src/ema/probes.py
--rw-rw-rw-   0        0        0     7648 2024-03-03 00:49:08.000000 EMAtools-0.1.0/src/ema/signal.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:19:46.323864 EMAtools-0.2.0/
+-rw-rw-rw-   0        0        0     1090 2024-02-07 18:45:22.000000 EMAtools-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      579 2024-05-10 00:19:46.319851 EMAtools-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    32622 2024-05-10 00:15:50.000000 EMAtools-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-10 00:19:46.323864 EMAtools-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1151 2024-05-09 16:17:34.000000 EMAtools-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:19:46.175153 EMAtools-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 00:19:46.316859 EMAtools-0.2.0/src/EMAtools.egg-info/
+-rw-rw-rw-   0        0        0      579 2024-05-10 00:19:46.000000 EMAtools-0.2.0/src/EMAtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2024-05-10 00:19:46.000000 EMAtools-0.2.0/src/EMAtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 00:19:46.000000 EMAtools-0.2.0/src/EMAtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-10 00:19:46.000000 EMAtools-0.2.0/src/EMAtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-10 00:19:46.000000 EMAtools-0.2.0/src/EMAtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 00:19:46.300862 EMAtools-0.2.0/src/ema/
+drwxrwxrwx   0        0        0        0 2024-05-10 00:19:46.313845 EMAtools-0.2.0/src/ema/Veelo/
+-rw-rw-rw-   0        0        0       18 2024-02-08 14:56:33.000000 EMAtools-0.2.0/src/ema/Veelo/__init__.py
+-rw-rw-rw-   0        0        0      869 2024-02-08 14:56:33.000000 EMAtools-0.2.0/src/ema/Veelo/modify_current.py
+-rw-rw-rw-   0        0        0     3585 2024-02-08 14:56:33.000000 EMAtools-0.2.0/src/ema/Veelo/preprocess.py
+-rw-rw-rw-   0        0        0    25322 2024-02-08 14:56:33.000000 EMAtools-0.2.0/src/ema/Veelo/util.py
+-rw-rw-rw-   0        0        0      268 2024-05-02 23:29:09.000000 EMAtools-0.2.0/src/ema/__init__.py
+-rw-rw-rw-   0        0        0      314 2024-03-25 20:09:49.000000 EMAtools-0.2.0/src/ema/cin.py
+-rw-rw-rw-   0        0        0     3342 2024-05-09 16:02:07.000000 EMAtools-0.2.0/src/ema/coupled.py
+-rw-rw-rw-   0        0        0     4262 2024-03-25 20:46:45.000000 EMAtools-0.2.0/src/ema/emc.py
+-rw-rw-rw-   0        0        0     5741 2024-02-29 22:34:30.000000 EMAtools-0.2.0/src/ema/emin.py
+-rw-rw-rw-   0        0        0     1692 2024-05-03 21:27:54.000000 EMAtools-0.2.0/src/ema/endpoint_probes.py
+-rw-rw-rw-   0        0        0    14966 2024-05-09 23:21:42.000000 EMAtools-0.2.0/src/ema/file.py
+-rw-rw-rw-   0        0        0     5037 2024-05-03 19:41:13.000000 EMAtools-0.2.0/src/ema/inp.py
+-rw-rw-rw-   0        0        0    12916 2024-05-09 16:01:34.000000 EMAtools-0.2.0/src/ema/midpoint_probes.py
+-rw-rw-rw-   0        0        0     8475 2024-03-28 18:20:10.000000 EMAtools-0.2.0/src/ema/results.py
+-rw-rw-rw-   0        0        0     7648 2024-05-02 23:22:25.000000 EMAtools-0.2.0/src/ema/signal.py
```

### Comparing `EMAtools-0.1.0/LICENSE.txt` & `EMAtools-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EMAtools-0.1.0/PKG-INFO` & `EMAtools-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: EMAtools
-Version: 0.1.0
-Summary: An assortment of computational tools to make life easier at EMA.
+Version: 0.2.0
+Summary: Python library for users of EMC Plus and Charge Plus.
 Home-page: https://github.com/GriffinKowash/EMAtools
 Author: Griffin Kowash
 Author-email: griffin.kowash@ema3d.com
 Project-URL: Usage guide, https://github.com/GriffinKowash/EMAtools/blob/main/README.md
 Project-URL: GitHub, https://github.com/GriffinKowash/EMAtools
 Project-URL: Changelog, https://github.com/GriffinKowash/EMAtools/blob/main/CHANGELOG.md
 Requires-Python: >=3.7, <4
```

### Comparing `EMAtools-0.1.0/README.md` & `EMAtools-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 - Complex preprocessing operations
 
 
 # Table of Contents
 
 - **[Installation](#installation)**
 - **[Usage](#usage)**
-	- **[Probes module](#probes-module)**
+	- **[Results module](#results-module)**
 		- **[Loading point probe results](#loading-point-probe-results)**
 		- **[Loading box/distributed probe results](#loading-boxdistributed-probe-results)**
+		- **[Loading Charge results](#loading-charge-results)**
 	- **[Signal module](#signal-module)**
 		- **[FFT](#fft)**
 		- **[Trimming](#trimming)**
 		- **[Padding](#padding)**
 		- **[Resampling](#resampling)**
 		- **[Statistics](#statistics)**
 	- **[EMC module](#emc_module)**
@@ -37,14 +38,18 @@
 	- **[Emin class](#emin-class)**
 		- **[Instantiating an Emin object](#instantiating-an-emin-object)**
 		- **[Modifying isotropic materials](#modify-isotropic-material)**
 		- **[Restricting surface currents](#restrict-surface-current)**
 	- **[Inp class](#inp-class)**
 		- **[Instantiating an Inp object](#instantiating-an-inp-object)**
 		- **[Probing voltage/current](#probing-voltagecurrent)**
+	- **[CoupledSim class](#coupledsim-class)**
+		- **[Instantiating a CoupledSim object](#instantiating-a-coupledsim-object)**
+		- **[Probing current at midpoints](#probing-currents-at-midpoints)**
+		- **[Probing voltage at terminations](#probing-voltage-at-terminations)**
 
 
 # Installation
 
 EMAtools can be installed using the Pip package manager:
 
 ```
@@ -59,19 +64,20 @@
 
 Import EMAtools in a Python script or shell:
 
 ```
 import ema
 ```
 
+
 # Usage
 
 When in doubt, refer to in-code documention for the feature in question at https://github.com/GriffinKowash/EMAtools/tree/main/src/ema. Please notify Griffin at griffin.kowash@ema3d.com if any conflicts between documentation and true behavior are observed.
 
-## Probes module
+## Results module
 
 ### Loading point probe results
 
 Any probe results that are formatted with a single timestep per line can be loaded using the `load_probe` function:
 
 ```
 results = ema.load_probe('path/to/file.dat')
@@ -109,14 +115,25 @@
 
 The physical location of each sample point can be determined by reference to the Emin file, where they are listed in the same order along with their mesh indices.
   
   Note that probe results generated by older versions of EMA3D may fail to load due to a difference in file format. The oldest version currently known to be supported is 2023R2.
   
   Precision can be specified in the same way as for the `load_probe` function.
  
+ 
+### Loading Charge results
+
+Any Charge Plus output file ending in `_results.dat` can be loaded using the `load_charge_results` function. For example:
+
+```
+t, data = load_charge_results('path/to/picCHARGE_results.dat')
+```
+ 
+The function returns a tuple of the time steps and field data, with the field data arranged in the shape [field, node, time].
+
 
 
 ## Signal module
   
 ### FFT
 
 A fast Fourier transform (FFT) can be applied to real-valued time series data `t, x` as follows:
@@ -363,29 +380,41 @@
 
 ```
 1 	| * File Name: test.emin
 14 	| !MPIBLOCKS
 25 	| !EMRESULTS
 ```
 
-The `File.print` method performs the same function but accepts indices instead of line numbers. For the examples above, `file.print(9, 14)` and `file.print([0, 13, 24])` would produce identical results.
+The `File.print` method performs the same function but accepts indices (0-indexed) instead of line numbers (1-indexed). For the examples above, `file.print(9, 14)` and `file.print([0, 13, 24])` would produce identical results.
 
 The `File.head` method is a wrapper for `File.printlines` that displays the first `n` lines, where `n` is an integer provided as an argument. For example, running `file.head(5)` will display the following:
 
 ```
 1 	| * File Name: test.emin
 2 	| * Created  : Tue, 05 Sep 08:39:11 GMT-06:00  
 3 	| * DO NOT MODIFY >>>       
 4 	| * <Cached>test_.sav</Cached>
 5 	| * <CachedId>28120648-340b-4e3a-8138-63381f05d812</CachedId>
 ```
 
+By default, the result is printed with line numbers and indentation for readability. To suppress this behavior, set the optional argument `numbered` to `False` in any of the print methods described above. For example, executing `file.head(5, numbered=False)` outputs the following:
+
+```
+* File Name: test.emin
+* Created  : Tue, 05 Sep 08:39:11 GMT-06:00  
+* DO NOT MODIFY >>>       
+* <Cached>test_.sav</Cached>
+* <CachedId>28120648-340b-4e3a-8138-63381f05d812</CachedId>
+```
+
 
 ### Searching
 
+#### Find all
+
 Any change to a simulation file typically begins with locating a particular string of text. The base function for this task is `File.find_all`, which returns a list of all indices at which the provided search string is present in the file. For example, to search for every instance of `!NEW PROBE FILE NAME`:
 
 ```
 probe_indices = file.find_all('!NEW PROBE FILE NAME')
 ```
 
 Printing the result using `file.print(probe_indices)` reveals that several probes have been identified in the file:
@@ -400,46 +429,63 @@
 ```
 
 Several optional keyword arguments can be set to refine the search parameters. 
 
 - `start` specifies an index at which to begin searching, with all previous lines being omitted from the search. (Default 0)
 
 - `exact` is a boolean that determines whether a line must exactly match or simply contain the search string. (Default False)
+
+- `separator` is an optional string that modifies the behavior of `exact` mode; [see explanation below](#separator-keyword).
   
 - `case` is a boolean that determines whether the comparison against the search string should be case-sensitive. (Default True)
   
 - `n_max` is an integer that interrupts the search operation after `n_max` number of instances have been found, which can reduce search time when working with large files. (Default None)
 
 As an example, the following command will locate case-insensitive exact matches to the string "* geometry: line", beginning at index 150 and exiting after five matches have been found:
   
   ```
   indices = file.find_all('* geometry: line', start=150, exact=True, case=False, n_max=5)
   ```
   
-`File.find` is a wrapper method for `File.find_all` that finds a single match to the search string rather than returning a list of all matches. To find the first instance of "!NEW PROBE FILE NAME":
+#### Find
+  
+ `File.find` is a wrapper method for `File.find_all` that finds a single match to the search string rather than returning a list of all matches. To find the first instance of "!NEW PROBE FILE NAME":
 
 ```
 file.find('!NEW PROBE FILE NAME')
 ```
 
 The positional argument `n` can be used to locate the nth instance of the search string. For example, to find the index of the fifth probe defined in the file:
 
 ```
 file.find('!NEW PROBE FILE NAME', 5)
 ```
 
 The same keyword arguments used by `File.find_all` can also be provided to `File.find`, apart from `n_max`, which is automatically set to `n`.
 
+#### Find next
+
   Finally, the `File.find_next` method provides a convenient syntax for finding the next occurrence of a text string after a specified index. For example, after finding the starting index of a current source definition, a user may wish to locate the next blank line in the file:
   
 ```
 source_index = file.find('SOURCE NAME: Current Source')
 next_blank = file.find_next(source_index, '')
 ```
 
+#### Separator keyword
+
+The `separator` argument is only used with `exact=True` and allows a non-endline separator to be specified when searching for an exact match. During the search process, each line is split into separate strings at instances of the separator, and the search text is compared against each resulting string rather than against the line as a whole.
+
+ Setting the separator to an empty string will split each line by whitespace. Instead of a string, multiple separators can be specified in a list or tuple; for example, providing `separator=['(', ')']` will split each line by open and closed parentheses. Any standard regular expression may also be used. This option is supported for all of the search methods described above.
+
+ For a practical use case, consider that segment names in MHARNESS files have topology information encoded using underscores; for example, "SEG5___S0___C0" indicates a conductor nested in a shield along segment SEG5. If the user wishes to find occurrences of SEG5 that do *not* contain topology information, executing `file.find('SEG5')` will yield false positives, since "SEG5" is a partial match for "SEG5___S0___C0". On the other hand, `file.find('SEG5', exact=True)` will likely yield no results, since an "exact" search only identifies exact matches to entire lines, and additional information will typically be present in the same line.
+
+ The desired result can be achieved by executing `file.find('SEG5', exact=True, separator='')`, with an empty string as the separator. This will only flag occurrences of "SEG5" that are surrounded by whitespace, which excludes instances with topology information, and it will not overlook lines where additional, whitespace-delimited information is present.
+
+
 
 ### Inserting
 
 The `File.insert` method allows the user to insert one or more lines at a given index. For example, utilizing `File.find` from the previous section, a comment can be inserted at the index of the line "!SUMMARY":
 
 ```
 index = file.find('!SUMMARY', exact=True)
@@ -669,8 +715,94 @@
 126 	| !PROBE
 127 	| !!CABLE VOLTAGE
 128 	| voltage_SEG_C1_12.dat  
 129 	| 0.0000000000E+00    9.9999812000E-07    8.3600000000E-12   
 130 	| SEG      C1      12  
 ```
 
-Note that `Inp.probe_voltage` and `Inp.probe_current` do not verify whether the segment and conductor names provided by the user actually exist in the harness.
+Note that `Inp.probe_voltage` and `Inp.probe_current` do not verify whether the segment and conductor names provided by the user actually exist in the harness.
+
+
+## CoupledSim class
+
+The CoupledSim class provides functionality specific to coupled EMA3D/MHARNESS simulations.
+
+### Instantiating a CoupledSim object
+
+To instantiate a `CoupledSim` object, first import the `Emin`, `Inp`, and `CoupledSim` classes:
+
+```
+from ema import Emin, Inp, CoupledSim
+```
+
+Next, load the simulation input files as `Emin` and `Inp` objects, as described in the previous sections:
+
+```
+emin = Emin('path/to/file.emin')
+inp = Inp('path/to/file.inp')
+```
+
+Finally, pass the `Emin` and `Inp` objects as arguments to the `CoupledSim` constructor:
+```
+coupled = CoupledSim(emin, inp)
+```
+
+
+### Probing currents at midpoints
+
+Manually placing current probes on a harness can be extremely time intensive when working with large models. The `probe_midpoint_currents` method automates this procedure by detecting points of interest in the harness and adding probe definitions to the input file.
+
+ Probes are placed at the midpoint of each unbranching chain of MHARNESS segments comprising a given conductor. This ensures that all unique currents in the conductor are captured without requiring a probe to be placed on every segment.
+
+ The image below shows the probe placement generated for an example conductor. Since the conductor is not routed into `SEG1` (top right), segments `SEG` and `SEG2` are treated as a single, continuous current path. The `probe_midpoint_currents` method therefore places a single probe at their combined midpoint rather than placing one on `SEG` and another on `SEG2`.
+
+ <p align="center"><img src="resources/readme_midpoint_probes.png" /></p>
+ <p align="center">Figure 1: Placement of current probes by CoupledSim.probe_midpoint_currents</p>
+ <br>
+
+ After creating a `CoupledSim` object as described above, simply call the `probe_midpoint_currents` method:
+
+```
+coupled.probe_midpoint_currents()
+```
+
+By default, this method places current probes on every conductor in the harness. To probe a single conductor, pass the conductor name as a positional argument:
+
+```
+coupled.probe_midpoint_currents('Conductor_1')
+```
+
+To probe several conductors, provide a list of names:
+
+```
+coupled.probe_midpoint_currents(['Conductor_1', 'Conductor_2'])
+```
+
+If additional information from the algorithm is desired for debugging purposes, set the `verbose` keyword argument to `True`:
+
+```
+coupled.probe_midpoint_currents('Conductor_1', verbose=True)
+```
+
+
+### Probing voltage at terminations
+
+The `CoupledSim` class also supports automatic probing of conductor terminations. After creating a `CoupledSim` object as described above, call the  `probe_termination_voltages` method:
+
+```
+coupled.probe_termination_voltages()
+```
+
+As with `CoupledSim.probe_midpoint_currents`, a conductor or list of conductors can optionally be provided:
+
+```
+coupled.probe_termination_voltages('Conductor_1')
+coupled.probe_termination_voltages(['Conductor_3, 'Conductor_4'])
+```
+
+By default, this method places probes on all conductor terminations; however, for open-circuit voltage analysis, it is generally only necessary to probe high-resistance terminations. To exclude terminations below a minimum resistance, specify a cutoff using the `threshold` keyword argument:
+
+```
+coupled.probe_termination_voltages(threshold=1e6)
+```
+
+Note that any conductor endpoints without defined terminations will be ignored by this method.
```

### Comparing `EMAtools-0.1.0/setup.py` & `EMAtools-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 #long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="EMAtools",  # Required
-    version="0.1.0",  # Required
-    description="An assortment of computational tools to make life easier at EMA.",  # Optional
+    version="0.2.0",  # Required
+    description="Python library for users of EMC Plus and Charge Plus.",  # Optional
     #long_description=long_description,  # Optional
     #long_description_content_type="text/markdown",  # Optional (see note above)
     url="https://github.com/GriffinKowash/EMAtools",  # Optional
     author="Griffin Kowash",  # Optional
     author_email="griffin.kowash@ema3d.com",  # Optional
     package_dir={"": "src"},  # Optional
     packages=find_packages(where="src"),  # Required
```

### Comparing `EMAtools-0.1.0/src/EMAtools.egg-info/PKG-INFO` & `EMAtools-0.2.0/src/EMAtools.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: EMAtools
-Version: 0.1.0
-Summary: An assortment of computational tools to make life easier at EMA.
+Version: 0.2.0
+Summary: Python library for users of EMC Plus and Charge Plus.
 Home-page: https://github.com/GriffinKowash/EMAtools
 Author: Griffin Kowash
 Author-email: griffin.kowash@ema3d.com
 Project-URL: Usage guide, https://github.com/GriffinKowash/EMAtools/blob/main/README.md
 Project-URL: GitHub, https://github.com/GriffinKowash/EMAtools
 Project-URL: Changelog, https://github.com/GriffinKowash/EMAtools/blob/main/CHANGELOG.md
 Requires-Python: >=3.7, <4
```

### Comparing `EMAtools-0.1.0/src/ema/Veelo/modify_current.py` & `EMAtools-0.2.0/src/ema/Veelo/modify_current.py`

 * *Files identical despite different names*

### Comparing `EMAtools-0.1.0/src/ema/Veelo/preprocess.py` & `EMAtools-0.2.0/src/ema/Veelo/preprocess.py`

 * *Files identical despite different names*

### Comparing `EMAtools-0.1.0/src/ema/Veelo/util.py` & `EMAtools-0.2.0/src/ema/Veelo/util.py`

 * *Files identical despite different names*

### Comparing `EMAtools-0.1.0/src/ema/emc.py` & `EMAtools-0.2.0/src/ema/emc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import warnings
 import os
 import numpy as np
 
 from .signal import rfft
-from .probes import load_probe
+from .results import load_probe
 
 
 def shielding(xf, xf_ref, axis=-1):
     """Calculates shielding effectiveness in decibels from frequency domain data.
     
     Default settings require x to have time along the first axis.
     Multiple data sets can be processed simultaneously by stacking along additional axes.
```

### Comparing `EMAtools-0.1.0/src/ema/emin.py` & `EMAtools-0.2.0/src/ema/emin.py`

 * *Files identical despite different names*

### Comparing `EMAtools-0.1.0/src/ema/file.py` & `EMAtools-0.2.0/src/ema/file.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import warnings
 import os
 import time
+import re
 
 import numpy as np
 
 
 class File:
     """Parent class for handling .emin, .inp, and .cin files."""
     
@@ -108,57 +109,91 @@
                 i = np.array(args)
             else:
                 i = args[0]
         
         return i + 1
         
         
-    def find_all(self, text, start=0, exact=False, case=True, n_max=None):
+    def find_all(self, text, start=0, end=None, exact=False, separator=None, case=True, n_max=None, verbose=True):
         """Finds indices of all occurrences of a text string in self.lines.
 
         Parameters
         ----------
         text : str
             Text string for which to search file.
         start : int (optional)
             Index at which to begin search; defaults to start of file.
+        end : int (optional)
+            Index at which to stop search; defaults to end of file.
         exact : bool (optional)
             Whether line must exactly match or simply contain text string.
+        separator : str | None (optional)
+            Used with "exact" to split each line by the separator before comparison.
         case : bool (optional)
             Whether to require case matching.
         n_max : int (optional)
             Interrupts search after n_max occurrences have been found.
+        verbose : bool (optional)
+            Prints a message when the specified string is not found.
             
         Returns
         -------
         list
             Indices of text string in self.lines; empty list if not present.
         """
         
         # Make text lowercase if not case sensitive
         if not case:
             text = text.lower()
+
+        # Format separators into regex pattern if needed
+        if exact and separator is not None:
+            if isinstance(separator, (list, str)):
+                pattern = '|'.join(separator)
+
+        # Create subset of self.lines bounded by start and end arguments
+        if end is not None:
+            lines = self.lines[start:end]
+        else:
+            lines = self.lines[start:]
         
         # Search for occurrences of text up to n_max
         n_found = 0
         indices = []
         
-        for i, line in enumerate(self.lines[start:]):
+        for i, line in enumerate(lines):
+            match = False
+
             if not case:
                 line = line.lower()
                 
             if (exact and text == line) or (not exact and text in line):
+                match = True
+
+            elif exact and separator is not None:
+                if separator == '': #general whitespace separator
+                    if text in line.split():
+                        match = True
+                else:
+                    try:
+                        if text in re.split(pattern, line):
+                            match = True
+                    except ValueError as exc:
+                        print(f'Separator(s) not valid: {separator}')
+                        print(exc)
+
+            if match:
                 indices.append(start + i)
                 n_found += 1
                 
                 if n_found == n_max:
                     break
-            
-        if n_found == 0:
-            print(f'Text string "{text}" not found in file.')
+
+        if n_found == 0 and verbose:
+            print(f'Text string "{text}" not found.')
 
         return np.array(indices)
         
         
     def find(self, text, n=1, **kwargs):
         """Finds index of nth occurrence (default first) of text string in self.lines.
 
@@ -386,27 +421,29 @@
         
         elif l1 is not None:
             i0, i1 = File.ltoi(l0, l1)
         
         return self.get(i0, i1)
 
     
-    def printlines(self, l0, l1=None):
+    def printlines(self, l0, l1=None, numbered=True):
         """
         Prints out lines l0 to l1 (1-based indexing) formatted with line numbers.
         
         Alternatively, if l0 is an iterable object, it will be treated as an array
         of lines to print out. Values passed for l1 will be ignored in this case.
 
         Parameters
         ----------
         l0 : int | array-like
             First line to print, or array of lines to print.
         l1 : int
             Last line to print.
+        numbered : bool
+            Whether to print line numbers alongside the text.
 
         Returns
         -------
         None
         """
         
         # Handle warnings
@@ -416,54 +453,63 @@
                 l0 = 1
             
         elif np.iterable(l0) and l1 is not None:
             warnings.warn('Argument l0 is iterable; l1 will be ignored.')
                     
         # Print lines
         lines = self.getlines(l0, l1)
+        if l1 is None:
+            lines = [lines]
 
         for i, line in enumerate(lines):
             if np.iterable(l0):
                 n = l0[i]
             else:
                 n = l0 + i
             
-            print(n, '\t|', line)
+            if numbered:
+                print(n, '\t|', line)
+            else:
+                print(line)
 
 
-    def print(self, i0, i1=None):
+    def print(self, i0, i1=None, numbered=True):
         """
         Prints out indices i0 to i1 (0-based indexing); wrapper for File.printlines.
 
         Parameters
         ----------
         i0 : int | array-like
             First index to print, or array of indices to print.
         i1 : int
             Last index to print.
+        numbered : bool
+            Whether to print line numbers alongside the text.
 
         Returns
         -------
         None
         """
 
-        self.printlines(self.itol(i0), self.itol(i1))
+        self.printlines(self.itol(i0), self.itol(i1), numbered)
             
                 
-    def head(self, n=10):
+    def head(self, n=10, numbered=True):
         """Wrapper for File.printlines; prints first n lines of file contents.
 
         Parameters
         ----------
         n : int
             Number of lines to print.
+        numbered : bool
+            Whether to print line numbers alongside the text.
 
         Returns
         -------
         None
         """
         
-        self.printlines(1, n)
+        self.printlines(1, n, numbered)
 
 
     ### Aliases for backward compatibility ###
     find_occurrences = find_all
```

### Comparing `EMAtools-0.1.0/src/ema/inp.py` & `EMAtools-0.2.0/src/ema/inp.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         # Replace whitespace with underscores
         segment = segment.replace(' ', '_')
         conductor = conductor.replace(' ', '_')
 
         # Default name if not provided
         if name is None:
-            name = '{}_{}_{}_{}'.format(probe_type, segment, conductor, index)
+            name = '{}_{}_{}_{}'.format(probe_type, conductor, segment, index)
 
         # Pull start, end, and step from domain settings if not provided
         if start is None:
             start = 0
 
         if end is None:
             end = self.endtime
@@ -144,8 +144,28 @@
         **kwargs : see Inp.probe
 
         Returns
         -------
         None
         """
 
-        self.probe('current', segment, conductor, index, **kwargs)
+        self.probe('current', segment, conductor, index, **kwargs)
+
+
+    def print_probes(self, numbered=True):
+        """Prints lines containing probe definitions to the console.
+
+        Parameters
+        ----------
+        numbered : bool (optional)
+            Whether to print with line numbers and indents (set False if planning to copy-paste output)
+
+        Returns
+        -------
+        None
+        """
+
+        i0 = self.find('OUTPUT / PROBES') - 1
+        i1 = self.find('END THE INPUT FILE')
+
+        if i0 is not None and i1 is not None:
+            self.print(i0, i1, numbered)
```

### Comparing `EMAtools-0.1.0/src/ema/probes.py` & `EMAtools-0.2.0/src/ema/results.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import warnings
 import time
 import os
 import glob
 
 import numpy as np
 
+from .file import File
+
 
 def load_data(path_and_name, precision='single'):
     """Loads a generic data file with a consistent number of entries per row.
 
     Parameters
     ----------
     path_and_name : str
@@ -206,12 +208,67 @@
         save_path_and_name = path_and_name[:-4] + '_' + str(time.time()) + '.dat'
     else:
         save_path_and_name = '\\'.join(path_and_name.split('\\')[-1] + [fname])
         
     fmt = '%.7E' if precision == 'single' else '%.15E'
     np.savetxt(save_path_and_name, combined, fmt=fmt)
 
+
+def load_charge_results(path_and_name, fields=False):
+    """Loads FEM results file (femCHARGE_results.dat, picCHARGE_results.dat, etc.)
+
+    Parameters
+    ----------
+    path_and_name : str
+        Path to probe file (with .dat suffix)
+    fields : bool
+        If True, returns dict of field names and indices
+
+    Returns
+    -------
+    tuple
+        A tuple of time steps and probe results, and optionally a dict of column names
+    """
+
+    # Use file class for convenience
+    file = File(path_and_name)
+
+    # Find all time step flags
+    indices = file.find_all('Current time')
+
+    # Find number of mesh nodes
+    i0 = file.find('Node ')
+    i1 = file.find_next(i0, '', exact=True)
+    n = i1 - i0 - 1
+
+    # Unpack data
+    t, data = [], []
+    file.insert(len(file.lines), '') #helps with isolating time steps
+
+    for i in indices:
+        t.append(float(file.get(i).split()[-1]))
+
+        i0 = i + 4
+        i1 = i0 + n - 1
     
+        lines = file.get(i0, i1)
+        d = np.array([line.split() for line in lines], dtype=float)
+        data.append(d)
+
+    # Restructure to shape (fields, nodes, timesteps)
+    data = np.swapaxes(np.array(data), 0, -1)
+    t = np.array(t)
+
+    # Optionally return dict of column name/index mappings
+    if fields:
+        names = file.get(file.find('Node ')).split()
+        field_dict = {name:index for index, name in enumerate(names)}
+
+        return t, data, field_dict
+
+    return t, data
+
+
 ### Create aliases for box probes ###
 load_box_probe = load_distributed_probe
 load_box_probes = load_distributed_probes
 convert_box_probe = convert_distributed_probe
```

### Comparing `EMAtools-0.1.0/src/ema/signal.py` & `EMAtools-0.2.0/src/ema/signal.py`

 * *Files identical despite different names*

