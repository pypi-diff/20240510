# Comparing `tmp/mpl2nc-1.3.6.tar.gz` & `tmp/mpl2nc-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl2nc-1.3.6.tar", last modified: Sat Aug 19 18:31:32 2023, max compression
+gzip compressed data, was "mpl2nc-1.4.0.tar", last modified: Fri May 10 17:20:09 2024, max compression
```

## Comparing `mpl2nc-1.3.6.tar` & `mpl2nc-1.4.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-08-19 18:31:32.813910 mpl2nc-1.3.6/
--rw-r--r--   0 peter     (1000) peter     (1000)     1072 2023-08-19 18:27:16.000000 mpl2nc-1.3.6/LICENSE.md
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2023-08-19 18:27:16.000000 mpl2nc-1.3.6/MANIFEST.in
--rw-r--r--   0 peter     (1000) peter     (1000)      654 2023-08-19 18:31:32.813910 mpl2nc-1.3.6/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)    12749 2023-08-19 18:27:16.000000 mpl2nc-1.3.6/README.md
--rw-r--r--   0 peter     (1000) peter     (1000)     2622 2023-08-19 18:27:16.000000 mpl2nc-1.3.6/mpl2nc.1
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-08-19 18:31:32.813910 mpl2nc-1.3.6/mpl2nc.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)      654 2023-08-19 18:31:32.000000 mpl2nc-1.3.6/mpl2nc.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      252 2023-08-19 18:31:32.000000 mpl2nc-1.3.6/mpl2nc.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-08-19 18:31:32.000000 mpl2nc-1.3.6/mpl2nc.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       39 2023-08-19 18:31:32.000000 mpl2nc-1.3.6/mpl2nc.egg-info/entry_points.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       21 2023-08-19 18:31:32.000000 mpl2nc-1.3.6/mpl2nc.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        7 2023-08-19 18:31:32.000000 mpl2nc-1.3.6/mpl2nc.egg-info/top_level.txt
--rwxr-xr-x   0 peter     (1000) peter     (1000)    17386 2023-08-19 18:27:16.000000 mpl2nc-1.3.6/mpl2nc.py
--rw-r--r--   0 peter     (1000) peter     (1000)       79 2023-08-19 18:31:32.813910 mpl2nc-1.3.6/setup.cfg
--rw-r--r--   0 peter     (1000) peter     (1000)      968 2023-08-19 18:27:16.000000 mpl2nc-1.3.6/setup.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-10 17:20:09.760716 mpl2nc-1.4.0/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1072 2024-05-10 17:18:46.000000 mpl2nc-1.4.0/LICENSE.md
+-rw-r--r--   0 peter     (1000) peter     (1000)       74 2024-05-10 17:18:46.000000 mpl2nc-1.4.0/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)      654 2024-05-10 17:20:09.764716 mpl2nc-1.4.0/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)    15805 2024-05-10 17:18:46.000000 mpl2nc-1.4.0/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-10 17:20:09.760716 mpl2nc-1.4.0/dt-example/
+-rw-r--r--   0 peter     (1000) peter     (1000)      333 2024-05-10 17:18:46.000000 mpl2nc-1.4.0/dt-example/dt.csv
+-rw-r--r--   0 peter     (1000) peter     (1000)   285619 2024-05-10 17:18:46.000000 mpl2nc-1.4.0/dt-example/dt.png
+-rw-r--r--   0 peter     (1000) peter     (1000)     2619 2024-05-10 17:18:46.000000 mpl2nc-1.4.0/mpl2nc.1
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-05-10 17:20:09.760716 mpl2nc-1.4.0/mpl2nc.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)      654 2024-05-10 17:20:09.000000 mpl2nc-1.4.0/mpl2nc.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      288 2024-05-10 17:20:09.000000 mpl2nc-1.4.0/mpl2nc.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-05-10 17:20:09.000000 mpl2nc-1.4.0/mpl2nc.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       39 2024-05-10 17:20:09.000000 mpl2nc-1.4.0/mpl2nc.egg-info/entry_points.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-05-10 17:20:09.000000 mpl2nc-1.4.0/mpl2nc.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        7 2024-05-10 17:20:09.000000 mpl2nc-1.4.0/mpl2nc.egg-info/top_level.txt
+-rwxr-xr-x   0 peter     (1000) peter     (1000)    20148 2024-05-10 17:18:46.000000 mpl2nc-1.4.0/mpl2nc.py
+-rw-r--r--   0 peter     (1000) peter     (1000)       79 2024-05-10 17:20:09.764716 mpl2nc-1.4.0/setup.cfg
+-rw-r--r--   0 peter     (1000) peter     (1000)      996 2024-05-10 17:18:46.000000 mpl2nc-1.4.0/setup.py
```

### Comparing `mpl2nc-1.3.6/LICENSE.md` & `mpl2nc-1.4.0/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018-2020 Peter Kuma
+Copyright (c) 2018-2024 Peter Kuma
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mpl2nc-1.3.6/PKG-INFO` & `mpl2nc-1.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl2nc
-Version: 1.3.6
+Version: 1.4.0
 Summary: Convert Sigma Space Micro Pulse Lidar (MPL) data files to NetCDF
 Home-page: https://github.com/peterkuma/mpl2nc
 Author: Peter Kuma
 Author-email: peter@peterkuma.net
 License: MIT
 Keywords: sigmaspace,mpl,lidar,netcdf
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mpl2nc-1.3.6/README.md` & `mpl2nc-1.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -15,50 +15,53 @@
 correction files are supplied, the corrections are applied when calculating
 NRB.
 
 Note that the vendor-supplied dead time correction is known to be incorrect
 in some instances. The dead time bin files use 32-bit floating point values
 to store polynomial coefficients, which may be truncated due to the limited
 precision of the data type. Using such dead time correction with mpl2nc or
-the SigmaMPL software will result in wrong calibration.
+the SigmaMPL software will result in wrong calibration. In such case please
+use a CSV file with dead time correction polynomial curve values as specified in
+the instrument's documentation ([see below](#dead-time-correction)).
 
 ## Usage
 
-mpl2nc is supposed to be run from the command line. Linux is recommended,
-but it may be possible to run mpl2nc under
-[Anaconda](https://www.anaconda.com/distribution/)
-on other operating systems.
+mpl2nc is a command line program to be run a terminal (Linux and macOS) or the
+Command Prompt (Windows).
 
-Usage:
+Synopsis:
 
-```sh
-mpl2nc [-a <afterpulse>] [-d <dead_time>] [-h] [-o <overlap>] [-q] [-v] [<input>] <output>
-```
+`mpl2nc` [`-a` *afterpulse*] [`-d` *dead_time*] [`-o` *overlap*] [`-q`] [`-v`] [*input*] *output* \
+`mpl2nc` `-h`|`--help`
 
 Optional arguments:
 
-- `-a <afterpulse>`: Afterpulse correction file (`.bin`).
-- `-d <dead_time>`: Dead time correction file (`.bin`).
-- `-h`: Show help message and exit.
-- `-o <overlap>`: Overlap correction file (`.bin`).
+- `-a` *afterpulse*: Afterpulse correction file (`.bin`).
+- `-d` *dead_time*: Dead time correction file (`.bin` or `.csv`).
+- `-h`, `--help`: Show help message and exit.
+- `-o` *overlap*: Overlap correction file (`.bin`).
 - `-q`: Run quietly (suppress output).
 - `-v`: Show program's version number and exit.
 
 Positional arguments:
 
-- `input`: Input `.mpl` file or a directory containing `.mpl` files.
-- `output`: Output `.nc` file or a directory where the resulting `.nc` files are written.
+- *input*: Input `.mpl` file or a directory containing `.mpl` files.
+- *output*: Output `.nc` file or a directory where the resulting `.nc` files are written.
+
+If *input* is not specified, only the correction files are converted and
+written to *output*.
 
-If `input` is not specified, only the correction files are converted
-and written to `output`.
+Currently only afterpulse correction file version 3 (SigmaMPL2013R1.0 and
+later) is supported.
 
-Currently only afterpulse correction file version 3 (SigmaMPL2013R1.0 and later)
-is supported.
+The dead time correction file can come either from the vendor-supplied `.bin` file
+or from a CSV file created manually from a polynomial curve specified in the
+instrument's documentation ([see below](#dead-time-correction)).
 
-See also the man page for information about usage:
+On Linux and macOS, see also the man page for information about usage:
 
 ```
 man mpl2nc
 ```
 
 ## Examples
 
@@ -78,33 +81,95 @@
 mpl2nc -a MMPL5054_Afterpulse_201903220500.bin -o MMPL5054_Overlap_201903270700.bin -d MMPL5054_SPCM34184_Deadtime7.bin calibration.nc
 ```
 
 Convert afterpulse, overlap and dead time correction files to the NetCDF file `calibration.nc`.
 
 ## Installation
 
-Install the required software:
+It is recommended to run mpl2nc on Linux.
+
+### Linux
+
+On Debian-derived distributions (Ubuntu, Devuan, ...), install the required
+system packages with:
+
+```sh
+sudo apt install python3 python3-pip pipx
+```
+
+On Fedora, install the required system packages with:
 
-- Python 3 or [Anaconda](https://www.anaconda.com/distribution/)
-- pipx (on Linux)
+```sh
+sudo yum install python3 pipx
+```
 
-To install mpl2nc with pipx on Python 3 on Linux:
+Install mpl2nc:
 
 ```sh
 pipx install mpl2nc
+mkdir -p ~/.local/share/man/man1
+ln -s ~/.local/pipx/venvs/mpl2nc/share/man/man1/mpl2nc.1 ~/.local/share/man/man1/
+```
+
+Make sure that `$HOME/.local/bin` is included in the `PATH` environment
+variable if not already. This can be done with `pipx ensurepath`.
+
+You should now be able to run `mpl2nc` and see the manual page with `man mpl2nc`.
+
+To uninstall:
+
+```sh
+pipx uninstall mpl2nc
+rm ~/.local/share/man/man1/mpl2nc.1
+```
+
+### macOS
+
+Open the Terminal. Install mpl2nc with:
+
+```sh
+python3 -m pip install mpl2nc
 ```
 
-To install in Anaconda:
+Make sure that `/Users/<user>/Library/Python/<version>/bin` is included in the
+`PATH` environment variable if not already, where `<user>` is your system
+user name and `<version>` is the Python version. This path should be printed
+by the above command. This can be done by adding this line to the file
+`.zprofile` in your home directory and restart the Terminal:
+
+```sh
+PATH="$PATH:/Users/<user>/Library/Python/<version>/bin"
+```
+
+You should now be able to run `mpl2nc` and see the manual page with `man mpl2nc`.
+
+To uninstall:
+
+```sh
+python3 -m pip uninstall mpl2nc
+```
+
+### Windows
+
+Install [Python 3](https://www.python.org). In the installer, tick `Add
+python.exe to PATH`.
+
+Open Command Prompt from the Start menu. Install mpl2nc with:
 
 ```sh
 pip install mpl2nc
 ```
 
-Make sure that `$HOME/.local/bin` is included in the `PATH` environment
-variable.
+You should now be able to run `mpl2nc`.
+
+To uninstall:
+
+```sh
+pip uninstall mpl2nc
+```
 
 ## NetCDF output description
 
 ### Dimensions
 
 - profile – backscatter profile
 - range – backscatter range
@@ -236,24 +301,77 @@
                range**2/(ol_overlap*energy_monitor*1e-3)
 ```
 
 where `range` is range in m and dtcf is a function which calculates the dead
 time correction factor for given photon counts. The correction fields
 are interpolated on the data range.
 
+### Dead time correction
+
+A CSV file with dead time correction values can be supplied with the `-d` option.
+This can be created from a dead time correction polynomial curve table supplied
+with the instrument. For example:
+
+![](dt-example/dt.png)
+
+The CSV file should contain two columns: `count` (in Kc/s) and `factor`
+(unitless). The values should be as specified in the table for your particular
+instrument. For the above example, the content of the
+[CSV file](dt-example/dt.csv) should be:
+
+```csv
+count,factor
+13.6,1.00
+33.9,1.01
+87.1,0.98
+220.3,0.98
+542.4,1.00
+1332.2,1.02
+2071.1,1.04
+3101.2,1.10
+4550.5,1.19
+6630.3,1.29
+9281.0,1.46
+10855.9,1.58
+12618.1,1.71
+14570.7,1.86
+16570.5,2.06
+18778.5,2.29
+20667.1,2.62
+23145.1,2.94
+25075.1,3.42
+27049.1,3.99
+28816.7,4.71
+30462.6,5.61
+31942.1,6.74
+33147.1,8.18
+33964.4,10.05
+34434.4,12.47
+```
+
+The resulting curve is linearly interpolated between the specified points
+in the `count`–*log*(`factor`) space. For count values below the smallest value,
+a factor of 1 is used. For count values above the largest values, a factor
+of infinity (in the floating-point data type) is used and a warning is issued.
+
 ## License
 
-This software can be used, modified and distributed freely under
-the terms of an MIT license
-(see [LICENSE.md](LICENSE.md) in the source distribution).
+This software can be used, modified and distributed freely under the terms of
+an MIT license (see [LICENSE.md](LICENSE.md) in the source distribution).
 
 ## Release notes
 
 Version numbering follows [Semantic Versioning](https://semver.org/).
 
+### 1.4.0 (2024-05-10)
+
+- Support for dead time correction supplied as a CSV file.
+- Better error reporting.
+- Improvements in the documentation.
+
 ### 1.3.6 (2023-08-19)
 
 - Installation with pipx.
 - Improved list of dependencies in setup.py.
 - Dropped support for Python 2.7.
 
 ### 1.3.5 (2020-07-18)
```

### Comparing `mpl2nc-1.3.6/mpl2nc.1` & `mpl2nc-1.4.0/mpl2nc.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH mpl2nc 1 01/02/2020
+.TH mpl2nc 1 08/21/2023
 
 .SH NAME
 mpl2nc \- convert Sigma Space Micro Pulse Lidar (MPL) data files and afterpulse, overlap and dead time correction files to NetCDF
 
 .SH SYNOPSIS
 .B mpl2nc
 .RI "[-a " afterpulse ]
@@ -38,15 +38,15 @@
 .I .nc
 file or a directory where the resulting
 .I .nc
 files are written.
 If
 .I input
 is not specified, only the correction files are converted and written to the
-.I output 
+.I output
 .I .nc
 file.
 
 .SH OPTIONS
 
 .TP
 .RI "-a " afterpulse
@@ -68,29 +68,29 @@
 Show version number and exit.
 
 .SH EXAMPLES
 
 .B mpl2nc 201803040300.mpl 201803040300.nc
 
 Convert
-.I 201803040300.mpl 
+.I 201803040300.mpl
 to
 .IR 201803040300.nc .
 
 .B mpl2nc in out
 
 Convert MPL files in the directory
 .I in
 to NetCDF files in the directory
 .IR out .
 
 .B mpl2nc -a MMPL5054_Afterpulse_201903220500.bin -o MMPL5054_Overlap_201903270700.bin -d MMPL5054_SPCM34184_Deadtime7.bin 201803040300.mpl 201803040300.nc
 
 Convert
-.I 201803040300.mpl 
+.I 201803040300.mpl
 to
 .I 201803040300.nc
 using correction files for afterpulse, overlap and dead time.
 
 .B mpl2nc -a MMPL5054_Afterpulse_201903220500.bin -o MMPL5054_Overlap_201903270700.bin -d MMPL5054_SPCM34184_Deadtime7.bin in out
 
 Convert MPL files in the directory
@@ -102,15 +102,15 @@
 .B mpl2nc -a MMPL5054_Afterpulse_201903220500.bin -o MMPL5054_Overlap_201903270700.bin -d MMPL5054_SPCM34184_Deadtime7.bin calibration.nc
 
 Convert afterpulse, overlap and dead time correction files to the NetCDF file
 .IR calibration.nc .
 
 .SH COPYRIGHT
 
-Copyright (C) 2018-2020 Peter Kuma.
+Copyright (C) 2018-2023 Peter Kuma.
 .PP
 This program is available under the terms of an MIT license (see LICENSE.md in the distribution).
 
 .SH SEE ALSO
 
 See <https://github.com/peterkuma/mpl2nc>
 for more information about
```

### Comparing `mpl2nc-1.3.6/mpl2nc.egg-info/PKG-INFO` & `mpl2nc-1.4.0/mpl2nc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl2nc
-Version: 1.3.6
+Version: 1.4.0
 Summary: Convert Sigma Space Micro Pulse Lidar (MPL) data files to NetCDF
 Home-page: https://github.com/peterkuma/mpl2nc
 Author: Peter Kuma
 Author-email: peter@peterkuma.net
 License: MIT
 Keywords: sigmaspace,mpl,lidar,netcdf
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mpl2nc-1.3.6/mpl2nc.py` & `mpl2nc-1.4.0/mpl2nc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
+
+import signal
+signal.signal(signal.SIGINT, signal.SIG_DFL)
 
 import sys
 import os
 import argparse
-import logging
+import warnings
 import struct
 import datetime as dt
 
 import numpy as np
 from netCDF4 import Dataset
+import ds_format as ds
 
-__version__ = '1.3.6'
+__version__ = '1.4.0'
 
 C = 299792458 # m.s-1
 
 TYPES = {
     'float32': 'f',
     'float64': 'd',
     'int16': 'h',
@@ -153,14 +157,16 @@
     ['channel_2', 'float32', 'channel #2 data', 'Used only with POL-FS option. The co-polarized return signal array is stored here.', 'count us-1', ['profile', 'range']],
     ['ol_number_bins', 'uint32', 'overlap number of bins', None, 'count'],
     ['dt_number_coeff', 'uint32', 'dead time number of coefficients', None, 'count'],
     ['ol_overlap', 'float64', 'overlap values', None, None, ['ol_range']],
     ['ol_range', 'float64', 'overlap range', None, 'km', ['ol_range']],
     ['dt_coeff', 'float32', 'dead time coefficient', 'N coefficients of polynomial degree N-1 in decreasing order', None, ['dt_coeff_degree']],
     ['dt_coeff_degree', 'uint32', 'dead time coefficient degree', None, 'count', ['dt_coeff_degree']],
+    ['dt_count', 'float64', 'dead time count', None, 'count', ['dt_count']],
+    ['dt_factor', 'float64', 'dead time factor', None, '1', ['dt_count']],
     ['nrb_copol', 'float64', 'copol normalized relative backscatter', 'Experimental.', 'count us-1 uJ-1 km2', ['profile', 'range']],
     ['nrb_crosspol', 'float64', 'crosspol normalized relative backscatter', 'Experimental.', 'count us-1 uJ-1 km2', ['profile', 'range']],
     ['time', 'uint64', 'time', 'Record collection time.', 'seconds since 1970-01-01 00:00:00', ['profile']],
     ['time_utc', 'S19', 'UTC time', 'Record collection time (UTC).', 'ISO 8601', ['profile']],
 ]
 
 NC_HEADER = {x[0]: {
@@ -178,62 +184,73 @@
     fmt = '<' + ''.join([TYPES[x[1]] for x in header_dsc])
     size = struct.calcsize(fmt)
     fields = [x[0] for x in header_dsc]
     buf = f.read(size)
     if len(buf) == 0:
         return None
     if len(buf) < size:
-        raise IOError('Incomplete header')
+        raise IOError('incomplete header')
     res = struct.unpack_from(fmt, buf)
     return {k: np.array(v, dtype=t) for k, v, t in zip(fields, res, types)}
 
 def read_afterpulse(f):
     d = read_header(f, HEADER_AFTERPULSE)
     if d['ap_header'] != 0xAAEEEEAA:
-        raise IOError('Invalid afterpulse header')
+        raise IOError('invalid afterpulse header')
     n = int(d['ap_number_bins'])
     for x in ['ap_range', 'ap_copol', 'ap_crosspol']:
         buf = f.read(8*n)
         if len(buf) < 8*n:
-            raise IOError('Incomplete %s data' % x)
+            raise IOError('incomplete %s data' % x)
         a = struct.unpack_from('<' + 'd'*n, buf)
         d[x] = np.array(a, np.float64)
     return d
 
 def read_overlap(f):
     buf = f.read()
     n = len(buf)//16
     f.seek(0)
     d = {'ol_number_bins': np.array(n, np.uint32)}
     for x in ['ol_range', 'ol_overlap']:
         buf = f.read(8*n)
         if len(buf) < 8*n:
-            raise IOError('Incomplete %s data' % x)
+            raise IOError('incomplete %s data' % x)
         a = struct.unpack_from('<' + 'd'*n, buf)
         d[x] = np.array(a, np.float64)
     return d
 
-def read_dead_time(f):
+def read_dt(f):
     buf = f.read()
     n = len(buf)//4
-    d = {'dt_number_coeff': np.array(n, np.uint32)}
     a = struct.unpack_from('<' + 'f'*n, buf)
-    d['dt_coeff'] = np.array(a, np.float32)
-    d['dt_coeff_degree'] = np.arange(n - 1, -1, -1, dtype=np.uint32)
-    return d
+    return {
+        'dt_number_coeff': np.array(n, np.uint32),
+        'dt_coeff': np.array(a),
+        'dt_coeff_degree': np.arange(n - 1, -1, -1, dtype=np.uint32),
+    }
+
+def read_dt_csv(filename):
+    d = ds.read(filename)
+    if 'count' not in d or 'factor' not in d or \
+        d['count'].dtype != np.float64 or d['factor'].dtype != np.float64:
+        raise IOError('invalid dead time correction file: the file must contain two numerical columns "count" and "factor"')
+    return {
+        'dt_factor': d['factor'],
+        'dt_count': d['count']*1e3,
+    }
 
 def read_mpl_profile(f):
     d = read_header(f, HEADER_MPL)
     if d is None:
         return None
     n = int(d['number_bins'])
     for x in ['channel_1', 'channel_2']:
         buf = f.read(4*n)
         if len(buf) < 4*n:
-            raise IOError('Incomplete %s data' % x)
+            raise IOError('incomplete %s data' % x)
         a = struct.unpack_from('<' + 'f'*n, buf)
         d[x] = np.array(a, dtype=np.float32)
     return d
 
 def time_utc(d):
     return '%04d-%02d-%02dT%02d:%02d:%02d' % (
         d['year'],
@@ -246,41 +263,73 @@
 
 def time(d):
     t = dt.datetime(d['year'], d['month'], d['day'], d['hours'], d['minutes'],
         d['seconds'])
     t0 = dt.datetime(1970, 1, 1)
     return (t - t0).total_seconds()
 
-def calc_dtcf(x, coeff):
+def calc_dtcf_from_coeff(x, coeff):
     n = len(coeff)
-    return np.sum([(x*1e3)**(n-i-1)*coeff[i] for i in range(n)], axis=0)
+    with warnings.catch_warnings():
+        warnings.filterwarnings('error')
+        try:
+            return np.sum([(x*1e3)**(n-i-1)*coeff[i] for i in range(n)], axis=0)
+        except RuntimeWarning as e:
+            raise ValueError('overflow encountered in dead time correction calculation - please supply dead time correction polynomial curve from the instrument\'s documentation as a CSV file (see README for instructions)')
+
+def calc_dtcf_from_count_factor(x, count, factor, plot=False):
+    logcount = np.log(count)
+    logfactor = np.log(factor)
+    if type(x) is not np.ndarray or x.ndim == 0:
+        x = np.array([x])
+    dtcf = np.ones(len(x), np.float64)
+    mask = x*1e3 <= count[-1]
+    if not np.all(mask):
+        warnings.warn('input data contain values outside of the supplied dead time correction polynomial curve')
+    dtcf[mask] = np.exp(np.interp(x[mask]*1e3, count, logfactor, left=0, right=np.inf))
+    if plot:
+        import matplotlib.pyplot as plt
+        u = np.linspace(0, 35000e3, 100)
+        v = np.exp(np.interp(u, count, logfactor, left=0, right=np.inf))
+        plt.plot(u*1e-3, v)
+        plt.savefig('plot.pdf')
+    return dtcf
 
 def calc_nrb(d, channel, name, name2):
     raw = d[channel]
     n, m = raw.shape
     background = d['background_average' + name2]
     ap = d.get('ap' + name, np.zeros(m, np.float64))
     energy = d['energy_monitor']*1e-3
     ap_energy = d.get('ap_energy', 1.)
     ap_background = d.get('ap_background_average' + name, 0.)
     ol_range = d.get('ol_range')
     ap_range = d.get('ap_range')
     overlap = d.get('ol_overlap', np.ones(m, np.float64))
-    dt_coeff = d.get('dt_coeff', np.array([1.]))
 
     nrb = np.full((n, m), np.nan, np.float64)
 
+    if 'dt_coeff' in d:
+        calc_dtcf = lambda x: calc_dtcf_from_coeff(x, d['dt_coeff'])
+    elif 'dt_count' in d and 'dt_factor' in d:
+        calc_dtcf = lambda x: \
+            calc_dtcf_from_count_factor(x, d['dt_count'], d['dt_factor'])
+    else:
+        calc_dtcf = lambda x: 1
+
+    calc_dtcf_from_count_factor(0, d['dt_count'], d['dt_factor'], plot=True)
+
     for i in range(n):
         range_ = 0.5*d['bin_time'][i]*C*(np.arange(m) + 0.5)*1e-3
         ap2 = np.interp(range_, ap_range, ap) if ap_range is not None else ap
         overlap2 = np.interp(range_, ol_range, overlap) if ol_range is not None else overlap
-        nrb[i] = (raw[i,:]*calc_dtcf(raw[i,:], dt_coeff) - \
-            background[i]*calc_dtcf(background[i], dt_coeff) - \
-            ap2*calc_dtcf(ap2, dt_coeff)*energy[i]/ap_energy + \
-            ap_background*calc_dtcf(ap_background, dt_coeff)*energy[i]/ap_energy)* \
+        nrb[i] = (raw[i,:]*calc_dtcf(raw[i,:]) - \
+            background[i]*calc_dtcf(background[i]) - \
+            ap2*calc_dtcf(ap2)*energy[i]/ap_energy + \
+            ap_background*calc_dtcf(ap_background)*energy[i]/ap_energy)* \
             range_**2/(overlap2*energy[i])
 
     return nrb
 
 def process_mpl(dd):
     dx = {}
     for k in FIELDS:
@@ -313,46 +362,32 @@
 
 def write(d, filename):
     f = Dataset(filename, 'w')
     f.createDimension('profile', None)
     f.createDimension('range', None)
     f.createDimension('ap_range', None)
     f.createDimension('ol_range', None)
-    f.createDimension('dt_coeff_degree', None)
+    if 'dt_coeff' in d:
+        f.createDimension('dt_coeff_degree', None)
+    if 'dt_count' in d:
+        f.createDimension('dt_count', None)
     for k, v in d.items():
         h = NC_HEADER[k]
         var = f.createVariable(k, NC_TYPE[h['dtype']], h['dims'],
             fill_value=FILL_VALUE[h['dtype']])
         var[::] = v
         if h['units'] is not None: var.units = h['units']
         if h['long_name'] is not None: var.long_name = h['long_name']
         if h['comment'] is not None: var.comment = h['comment']
     f.created = dt.datetime.utcnow().strftime('%Y-%m-%dT:%H:%M:%SZ')
     f.software = 'mpl2nc (https://github.com/peterkuma/mpl2nc)'
     f.version = __version__
     f.close()
 
-def main():
-    p = argparse.ArgumentParser(prog='mpl2nc',
-        description='Convert Sigma Space Micro Pulse Lidar (MPL) data files to NetCDF.'
-    )
-    p.add_argument('-a', nargs=1, dest='afterpulse',
-        help='afterpulse (bin)')
-    p.add_argument('-d', nargs=1, dest='dead_time',
-        help='dead time correction (bin)')
-    p.add_argument('-o', nargs=1, dest='overlap',
-        help='overlap correction (bin)')
-    p.add_argument('-q', dest='quiet', action='store_true',
-        help='run quietly (suppress output)')
-    p.add_argument('-v', action='version', version=__version__)
-    p.add_argument('input', help='input file or directory (mpl)', nargs='?')
-    p.add_argument('output', help='output file or directory (NetCDF)')
-
-    args = p.parse_args()
-
+def main2(args):
     if args.input is None and \
         args.afterpulse is None and \
         args.overlap is None and \
         args.dead_time is None:
         sys.stderr.write('mpl2nc: at least one correction file or input have to be specified\n')
         sys.exit(1)
 
@@ -365,16 +400,19 @@
             afterpulse = read_afterpulse(f)
 
     if args.overlap is not None:
         with open(args.overlap[0], 'rb') as f:
             overlap = read_overlap(f)
 
     if args.dead_time is not None:
-        with open(args.dead_time[0], 'rb') as f:
-            dead_time = read_dead_time(f)
+        if args.dead_time[0].endswith('.csv'):
+            dead_time = read_dt_csv(args.dead_time[0])
+        else:
+            with open(args.dead_time[0], 'rb') as f:
+                dead_time = read_dt(f)
 
     d = {}
     if afterpulse is not None:
         d.update(afterpulse)
     if overlap is not None:
         d.update(overlap)
     if dead_time is not None:
@@ -398,9 +436,42 @@
                 write(mpl, output_filename)
         else:
             mpl = read_mpl(args.input)
             mpl.update(d)
             process_nrb(mpl)
             write(mpl, args.output)
 
+def main():
+    p = argparse.ArgumentParser(prog='mpl2nc',
+        description='Convert Sigma Space Micro Pulse Lidar (MPL) data files to NetCDF.'
+    )
+    p.add_argument('-a', nargs=1, dest='afterpulse',
+        help='afterpulse correction file (".bin")')
+    p.add_argument('-d', nargs=1, dest='dead_time',
+        help='dead time correction file (".bin" or ".csv")')
+    p.add_argument('-o', nargs=1, dest='overlap',
+        help='overlap correction file (".bin")')
+    p.add_argument('-q', dest='quiet', action='store_true',
+        help='run quietly (suppress output)')
+    p.add_argument('-v', action='version', version=__version__)
+    p.add_argument('--debug', dest='debug', action='store_true',
+        help='print debugging information'
+    )
+    p.add_argument('input', help='input file or directory (".mpl")', nargs='?')
+    p.add_argument('output', help='output file or directory (NetCDF)')
+
+    args = p.parse_args()
+
+    if not args.debug:
+        warnings.formatwarning = lambda msg, *args, **kwargs: \
+            'Warning: %s. Use --debug for more information.\n' % str(msg)
+
+    try:
+        main2(args)
+    except Exception as e:
+        if args.debug:
+            raise e
+        else:
+            print('Error: %s. Use --debug for more information.' % str(e), file=sys.stderr)
+
 if __name__ == '__main__':
     main()
```

### Comparing `mpl2nc-1.3.6/setup.py` & `mpl2nc-1.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(
     name='mpl2nc',
-    version='1.3.6',
+    version='1.4.0',
     description='Convert Sigma Space Micro Pulse Lidar (MPL) data files to NetCDF',
     author='Peter Kuma',
     author_email='peter@peterkuma.net',
     license='MIT',
     py_modules=['mpl2nc'],
     entry_points={
         'console_scripts': ['mpl2nc=mpl2nc:main'],
     },
     data_files=[('share/man/man1', ['mpl2nc.1'])],
     install_requires=[
         'numpy',
         'netCDF4>=1.2.9',
+        'ds-format>=4.1.0',
 	],
     keywords=['sigmaspace', 'mpl', 'lidar', 'netcdf'],
     url='https://github.com/peterkuma/mpl2nc',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
```

