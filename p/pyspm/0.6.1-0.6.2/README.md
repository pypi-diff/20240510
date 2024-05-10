# Comparing `tmp/pyspm-0.6.1.tar.gz` & `tmp/pyspm-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspm-0.6.1.tar", max compression
+gzip compressed data, was "pyspm-0.6.2.tar", max compression
```

## Comparing `pyspm-0.6.1.tar` & `pyspm-0.6.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11346 2023-04-12 14:13:51.314971 pyspm-0.6.1/LICENSE
--rw-r--r--   0        0        0     5352 2023-11-25 05:01:10.316913 pyspm-0.6.1/README.md
--rw-r--r--   0        0        0    35014 2024-01-13 06:29:03.381451 pyspm-0.6.1/pySPM/Block.py
--rw-r--r--   0        0        0    10264 2024-02-09 16:35:50.409746 pyspm-0.6.1/pySPM/Bruker.py
--rw-r--r--   0        0        0    43535 2024-01-13 06:12:18.927787 pyspm-0.6.1/pySPM/ITA.py
--rw-r--r--   0        0        0     4250 2024-01-12 04:14:01.892950 pyspm-0.6.1/pySPM/ITAX.py
--rw-r--r--   0        0        0     6884 2024-01-12 04:14:01.893239 pyspm-0.6.1/pySPM/ITAslicer.py
--rw-r--r--   0        0        0    63021 2024-01-13 06:29:03.386596 pyspm-0.6.1/pySPM/ITM.py
--rw-r--r--   0        0        0      778 2024-01-13 05:51:33.091690 pyspm-0.6.1/pySPM/ITS.py
--rw-r--r--   0        0        0     8488 2024-01-12 04:14:01.895167 pyspm-0.6.1/pySPM/PCA.py
--rw-r--r--   0        0        0    76965 2024-01-13 06:29:03.387025 pyspm-0.6.1/pySPM/SPM.py
--rw-r--r--   0        0        0     3159 2024-01-12 04:14:01.898191 pyspm-0.6.1/pySPM/SXM.py
--rw-r--r--   0        0        0     7676 2024-01-13 06:18:35.319790 pyspm-0.6.1/pySPM/ToF.py
--rw-r--r--   0        0        0      611 2024-01-13 05:50:23.500471 pyspm-0.6.1/pySPM/__init__.py
--rw-r--r--   0        0        0     1798 2024-01-12 04:14:01.892862 pyspm-0.6.1/pySPM/__main__.py
--rw-r--r--   0        0        0      162 2023-11-25 05:01:10.033528 pyspm-0.6.1/pySPM/_version.py
--rw-r--r--   0        0        0    10777 2024-01-12 04:14:01.902225 pyspm-0.6.1/pySPM/align.py
--rw-r--r--   0        0        0    10315 2024-01-13 05:54:34.680274 pyspm-0.6.1/pySPM/collection.py
--rw-r--r--   0        0        0   376832 2023-04-12 14:13:51.414468 pyspm-0.6.1/pySPM/data/elements.db
--rw-r--r--   0        0        0     1054 2024-01-11 19:57:38.305638 pyspm-0.6.1/pySPM/mplwidget.py
--rw-r--r--   0        0        0     9357 2024-01-13 05:55:11.783483 pyspm-0.6.1/pySPM/nanoscan.py
--rw-r--r--   0        0        0     5101 2024-01-13 06:23:04.007913 pyspm-0.6.1/pySPM/slicer.py
--rw-r--r--   0        0        0        0 2023-04-12 14:13:51.414758 pyspm-0.6.1/pySPM/tools/__init__.py
--rw-r--r--   0        0        0     1973 2024-01-11 19:04:18.499528 pyspm-0.6.1/pySPM/tools/emission_current_plotter.py
--rw-r--r--   0        0        0     3225 2024-01-13 05:57:27.180923 pyspm-0.6.1/pySPM/tools/fpanel.py
--rw-r--r--   0        0        0      996 2024-01-11 19:57:38.301793 pyspm-0.6.1/pySPM/tools/mplwidget.py
--rw-r--r--   0        0        0    12695 2024-01-12 04:14:01.907041 pyspm-0.6.1/pySPM/tools/spectra.py
--rw-r--r--   0        0        0     5637 2024-01-13 06:23:31.417040 pyspm-0.6.1/pySPM/tools/spectraviewer.py
--rw-r--r--   0        0        0     6760 2023-04-12 17:36:52.469324 pyspm-0.6.1/pySPM/tools/spectraviewer.ui
--rw-r--r--   0        0        0     2546 2024-01-12 04:14:01.902285 pyspm-0.6.1/pySPM/tools/stability.py
--rw-r--r--   0        0        0     1936 2024-01-11 18:53:31.936841 pyspm-0.6.1/pySPM/tools/timer_display.py
--rw-r--r--   0        0        0     1830 2023-04-12 17:36:52.470003 pyspm-0.6.1/pySPM/tools/timer_display.ui
--rw-r--r--   0        0        0     1802 2024-01-13 06:19:34.536702 pyspm-0.6.1/pySPM/tools/tof_timer.py
--rw-r--r--   0        0        0     1158 2024-01-13 06:13:44.343311 pyspm-0.6.1/pySPM/tools/values_display.py
--rw-r--r--   0        0        0     7289 2024-01-12 04:14:01.902660 pyspm-0.6.1/pySPM/tools/win32_helper.py
--rw-r--r--   0        0        0     7492 2024-01-13 06:08:41.013370 pyspm-0.6.1/pySPM/utils/__init__.py
--rw-r--r--   0        0        0      260 2023-04-12 17:36:52.470999 pyspm-0.6.1/pySPM/utils/colors.py
--rw-r--r--   0        0        0      341 2024-01-11 19:00:26.638706 pyspm-0.6.1/pySPM/utils/constants.py
--rw-r--r--   0        0        0    13622 2024-01-13 05:59:56.214863 pyspm-0.6.1/pySPM/utils/elts.py
--rw-r--r--   0        0        0    11688 2024-01-13 06:00:44.364361 pyspm-0.6.1/pySPM/utils/fit.py
--rw-r--r--   0        0        0     2913 2024-01-13 06:20:26.600725 pyspm-0.6.1/pySPM/utils/geometry.py
--rw-r--r--   0        0        0     1610 2024-01-12 04:14:01.889677 pyspm-0.6.1/pySPM/utils/haar.py
--rw-r--r--   0        0        0    10401 2024-01-13 06:20:33.981457 pyspm-0.6.1/pySPM/utils/math.py
--rw-r--r--   0        0        0     6043 2024-01-13 06:20:40.752996 pyspm-0.6.1/pySPM/utils/misc.py
--rw-r--r--   0        0        0    15967 2024-01-12 04:14:01.902523 pyspm-0.6.1/pySPM/utils/plot.py
--rw-r--r--   0        0        0      862 2024-01-11 19:04:18.405190 pyspm-0.6.1/pySPM/utils/progressbar.py
--rw-r--r--   0        0        0     6999 2024-01-13 06:02:19.022748 pyspm-0.6.1/pySPM/utils/restoration.py
--rw-r--r--   0        0        0     6194 2024-01-13 06:04:38.418802 pyspm-0.6.1/pySPM/utils/save.py
--rw-r--r--   0        0        0    17855 2024-01-13 06:29:03.384506 pyspm-0.6.1/pySPM/utils/spectra.py
--rw-r--r--   0        0        0     7124 2024-01-13 06:23:54.578711 pyspm-0.6.1/pySPM/utils/units.py
--rw-r--r--   0        0        0     1924 2024-02-09 16:42:11.514199 pyspm-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     6560 1970-01-01 00:00:00.000000 pyspm-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-04-12 14:13:51.314971 pyspm-0.6.2/LICENSE
+-rw-r--r--   0        0        0     5352 2023-11-25 05:01:10.316913 pyspm-0.6.2/README.md
+-rw-r--r--   0        0        0    35146 2024-03-02 13:00:18.372109 pyspm-0.6.2/pySPM/Block.py
+-rw-r--r--   0        0        0    10264 2024-02-09 16:35:50.409746 pyspm-0.6.2/pySPM/Bruker.py
+-rw-r--r--   0        0        0    43609 2024-03-02 13:00:26.737587 pyspm-0.6.2/pySPM/ITA.py
+-rw-r--r--   0        0        0     4250 2024-01-12 04:14:01.892950 pyspm-0.6.2/pySPM/ITAX.py
+-rw-r--r--   0        0        0     6884 2024-01-12 04:14:01.893239 pyspm-0.6.2/pySPM/ITAslicer.py
+-rw-r--r--   0        0        0    63092 2024-05-10 10:59:32.774581 pyspm-0.6.2/pySPM/ITM.py
+-rw-r--r--   0        0        0      778 2024-01-13 05:51:33.091690 pyspm-0.6.2/pySPM/ITS.py
+-rw-r--r--   0        0        0     8551 2024-03-02 13:00:18.370907 pyspm-0.6.2/pySPM/PCA.py
+-rw-r--r--   0        0        0    77354 2024-03-02 13:00:18.375740 pyspm-0.6.2/pySPM/SPM.py
+-rw-r--r--   0        0        0     3159 2024-01-12 04:14:01.898191 pyspm-0.6.2/pySPM/SXM.py
+-rw-r--r--   0        0        0     7674 2024-03-02 13:00:26.738178 pyspm-0.6.2/pySPM/ToF.py
+-rw-r--r--   0        0        0      611 2024-01-13 05:50:23.500471 pyspm-0.6.2/pySPM/__init__.py
+-rw-r--r--   0        0        0     1798 2024-01-12 04:14:01.892862 pyspm-0.6.2/pySPM/__main__.py
+-rw-r--r--   0        0        0      162 2023-11-25 05:01:10.033528 pyspm-0.6.2/pySPM/_version.py
+-rw-r--r--   0        0        0    10777 2024-01-12 04:14:01.902225 pyspm-0.6.2/pySPM/align.py
+-rw-r--r--   0        0        0    10315 2024-01-13 05:54:34.680274 pyspm-0.6.2/pySPM/collection.py
+-rw-r--r--   0        0        0   376832 2023-04-12 14:13:51.414468 pyspm-0.6.2/pySPM/data/elements.db
+-rw-r--r--   0        0        0     1054 2024-01-11 19:57:38.305638 pyspm-0.6.2/pySPM/mplwidget.py
+-rw-r--r--   0        0        0     9357 2024-01-13 05:55:11.783483 pyspm-0.6.2/pySPM/nanoscan.py
+-rw-r--r--   0        0        0     5101 2024-01-13 06:23:04.007913 pyspm-0.6.2/pySPM/slicer.py
+-rw-r--r--   0        0        0        0 2023-04-12 14:13:51.414758 pyspm-0.6.2/pySPM/tools/__init__.py
+-rw-r--r--   0        0        0     1973 2024-01-11 19:04:18.499528 pyspm-0.6.2/pySPM/tools/emission_current_plotter.py
+-rw-r--r--   0        0        0     3225 2024-01-13 05:57:27.180923 pyspm-0.6.2/pySPM/tools/fpanel.py
+-rw-r--r--   0        0        0      996 2024-01-11 19:57:38.301793 pyspm-0.6.2/pySPM/tools/mplwidget.py
+-rw-r--r--   0        0        0    12709 2024-03-02 12:54:27.445951 pyspm-0.6.2/pySPM/tools/spectra.py
+-rw-r--r--   0        0        0     5637 2024-01-13 06:23:31.417040 pyspm-0.6.2/pySPM/tools/spectraviewer.py
+-rw-r--r--   0        0        0     6760 2023-04-12 17:36:52.469324 pyspm-0.6.2/pySPM/tools/spectraviewer.ui
+-rw-r--r--   0        0        0     2546 2024-01-12 04:14:01.902285 pyspm-0.6.2/pySPM/tools/stability.py
+-rw-r--r--   0        0        0     1936 2024-01-11 18:53:31.936841 pyspm-0.6.2/pySPM/tools/timer_display.py
+-rw-r--r--   0        0        0     1830 2023-04-12 17:36:52.470003 pyspm-0.6.2/pySPM/tools/timer_display.ui
+-rw-r--r--   0        0        0     1802 2024-01-13 06:19:34.536702 pyspm-0.6.2/pySPM/tools/tof_timer.py
+-rw-r--r--   0        0        0     1158 2024-01-13 06:13:44.343311 pyspm-0.6.2/pySPM/tools/values_display.py
+-rw-r--r--   0        0        0     7289 2024-01-12 04:14:01.902660 pyspm-0.6.2/pySPM/tools/win32_helper.py
+-rw-r--r--   0        0        0     7508 2024-03-02 12:54:27.432208 pyspm-0.6.2/pySPM/utils/__init__.py
+-rw-r--r--   0        0        0      260 2023-04-12 17:36:52.470999 pyspm-0.6.2/pySPM/utils/colors.py
+-rw-r--r--   0        0        0      341 2024-01-11 19:00:26.638706 pyspm-0.6.2/pySPM/utils/constants.py
+-rw-r--r--   0        0        0    13658 2024-03-02 13:00:18.371463 pyspm-0.6.2/pySPM/utils/elts.py
+-rw-r--r--   0        0        0    11958 2024-03-02 13:00:18.370911 pyspm-0.6.2/pySPM/utils/fit.py
+-rw-r--r--   0        0        0     2912 2024-03-02 13:00:26.735740 pyspm-0.6.2/pySPM/utils/geometry.py
+-rw-r--r--   0        0        0     1610 2024-01-12 04:14:01.889677 pyspm-0.6.2/pySPM/utils/haar.py
+-rw-r--r--   0        0        0    10401 2024-01-13 06:20:33.981457 pyspm-0.6.2/pySPM/utils/math.py
+-rw-r--r--   0        0        0     6043 2024-01-13 06:20:40.752996 pyspm-0.6.2/pySPM/utils/misc.py
+-rw-r--r--   0        0        0    15981 2024-03-02 12:54:27.442673 pyspm-0.6.2/pySPM/utils/plot.py
+-rw-r--r--   0        0        0      862 2024-01-11 19:04:18.405190 pyspm-0.6.2/pySPM/utils/progressbar.py
+-rw-r--r--   0        0        0     6999 2024-01-13 06:02:19.022748 pyspm-0.6.2/pySPM/utils/restoration.py
+-rw-r--r--   0        0        0     6194 2024-01-13 06:04:38.418802 pyspm-0.6.2/pySPM/utils/save.py
+-rw-r--r--   0        0        0    17897 2024-03-02 12:54:27.439405 pyspm-0.6.2/pySPM/utils/spectra.py
+-rw-r--r--   0        0        0     7124 2024-01-13 06:23:54.578711 pyspm-0.6.2/pySPM/utils/units.py
+-rw-r--r--   0        0        0     1759 2024-05-10 11:06:06.020007 pyspm-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     6560 1970-01-01 00:00:00.000000 pyspm-0.6.2/PKG-INFO
```

### Comparing `pyspm-0.6.1/LICENSE` & `pyspm-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/README.md` & `pyspm-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/Block.py` & `pyspm-0.6.2/pySPM/Block.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
             )
         if len(self.Type) < 5:
             raise ValueError("EOF reached. Block cannot be read")
         self.head = dict(
             zip(
                 ["name_length", "ID", "N", "length1", "length2"],
                 struct.unpack("<5I", self.f.read(20)),
+                strict=False,
             )
         )
         self.name = self.f.read(self.head["name_length"]).decode("ascii")
         self.value = self.f.read(self.head["length1"])
         self.List = None
         self.iterP = 0
 
@@ -364,14 +365,15 @@
     def goto_next_block(self):
         offset = self.offset
         self.f.seek(offset)
         head = dict(
             zip(
                 ["name_length", "ID", "N", "length1", "length2"],
                 struct.unpack("<5x5I", self.f.read(25)),
+                strict=False,
             )
         )
         self.f.read(head["name_length"])
         length, nums, NextBlock = struct.unpack("<II25xQ", self.f.read(41))
         if NextBlock == 0:
             return None
         self.f.seek(NextBlock)
@@ -400,14 +402,15 @@
                         self.name, offset
                     )
                 )
             head = dict(
                 zip(
                     ["name_length", "ID", "N", "length1", "length2"],
                     struct.unpack("<5x5I", data),
+                    strict=False,
                 )
             )
             self.f.read(head["name_length"])
             data = self.f.tell()
             length, nums, next_block = struct.unpack("<II25xQ", self.f.read(41))
             N = head["N"]
             ## The following is commented as believed to be erroneous
@@ -415,14 +418,15 @@
             #    N = nums
             for i in range(N):
                 self.f.seek(data + 42 + 33 * i)
                 S = dict(
                     zip(
                         ["index", "slen", "id", "blen", "bidx"],
                         struct.unpack("<III4xQQ", self.f.read(32)),
+                        strict=False,
                     )
                 )
                 self.f.seek(data + S["index"])
                 S["name"] = self.f.read(S["slen"]).decode("ascii")
                 self.List.append(S)
             if next_block == 0:
                 break
```

### Comparing `pyspm-0.6.1/pySPM/Bruker.py` & `pyspm-0.6.2/pySPM/Bruker.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/ITA.py` & `pyspm-0.6.2/pySPM/ITA.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,24 +156,28 @@
             C_2H- (), mass: 24.98 - 25.04
             CN- (), mass: 25.97 - 26.04
             Cl- (), mass: 34.93 - 35.01
             C_2O- (), mass: 39.96 - 40.04
             CHNO- (), mass: 42.97 - 43.05
             CHO_2- (), mass: 44.95 - 45.04
             Cs- (), mass: 132.81 - 133.01
-        >>> ch = A.getChannelsByName("C[^a-z]") # Only carbon atoms (meaning that the char after C cannot be lowercase)
+        >>> ch = A.getChannelsByName(
+        ...     "C[^a-z]"
+        ... )  # Only carbon atoms (meaning that the char after C cannot be lowercase)
         >>> A.showChannels(ch)
                 CH- (), mass: 12.99 - 13.03
             C_2- (), mass: 23.97 - 24.03
             C_2H- (), mass: 24.98 - 25.04
             CN- (), mass: 25.97 - 26.04
             C_2O- (), mass: 39.96 - 40.04
             CHNO- (), mass: 42.97 - 43.05
             CHO_2- (), mass: 44.95 - 45.04
-        >>> ch = A.getChannelsByName("CH", True) # Only CH channel and not CHNO and CHO_2
+        >>> ch = A.getChannelsByName(
+        ...     "CH", True
+        ... )  # Only CH channel and not CHNO and CHO_2
         >>> A.showChannels(ch)
                 CH- (), mass: 12.99 - 13.03
         """
         res = []
         if strict:
             if type(name) in [list, tuple]:
                 name = ["^" + n + "[+-]?$" for n in name]
@@ -513,15 +517,15 @@
                 ).value
             )
         except:
             return [(0, 0) for x in range(self.Nscan)]
         D = struct.unpack("<" + str(len(X) // 4) + "i", X)
         dx = D[::2]
         dy = D[1::2]
-        return list(zip(dx, dy))
+        return list(zip(dx, dy, strict=False))
 
     @alias("getShiftCorrectedImageByMass")
     def get_shift_corrected_image_by_mass(self, masses, **kargs):
         """
         Shortcut function for pySPM.ITA.get_sum_image_by_mass using the saved shift corrections.
         """
         return self.get_sum_image_by_mass(
@@ -534,15 +538,15 @@
         Similar to pySPM.ITA.getSumImageByName but instead of the names, the mass or list of mass is provided
         see pySPM.ITA.getSumImageByName for more details
         """
         if scans is None:
             scans = range(self.Nscan)
         if isinstance(scans, int):
             scans = [scans]
-        if isinstance(masses, (int, float)):
+        if isinstance(masses, int | float):
             masses = [masses]
         if prog:
             scans = PB(scans, leave=False)
         channels = [self.get_channel_by_mass(m, full=True) for m in masses]
         Z = self.__get_sum_image(scans, channels, **kargs)
         if raw:
             return Z, channels
@@ -573,15 +577,15 @@
         pySPM.SPM.SPM_image
             Image of the result
         list of dictionaries
             Only returned if raw is True
             List of all selected peaks used to compute the image.
             Note: Pass this list to pySPM.ITA.showChannels in order to print a human readable representation of it.
         """
-        if isinstance(masses, (int, float)):
+        if isinstance(masses, int | float):
             masses = [masses]
         Z = np.zeros((self.sy, self.sx))
         channels = []
         for m in masses:
             ch = self.get_channel_by_mass(m)
             m = self.get_masses()[ch]
             if m["assign"] != "":
@@ -1031,15 +1035,15 @@
     def __getitem__(self, key):
         """
         Retrieve the image of a given channel
 
         Example
         -------
         >>> A = pySPM.ITA_collection("myfile.ita")
-        >>> A['Au-']
+        >>> A["Au-"]
         <pySPM.SPM.SPM_image at 0x????????>
         """
         if key not in self.channels:
             return None
         return self.channels[key]
 
     @alias("runPCA")
```

### Comparing `pyspm-0.6.1/pySPM/ITAX.py` & `pyspm-0.6.2/pySPM/ITAX.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/ITAslicer.py` & `pyspm-0.6.2/pySPM/ITAslicer.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/ITM.py` & `pyspm-0.6.2/pySPM/ITM.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
             "UpperMass": Get("Measurement.UpperMass"),
             "LMIGDropouts": Get("Measurement.LMIGDropouts"),
             "ShotsPerPixel": Get("Registration.Raster.ShotsPerPixel"),
             "RasterMode": Get("Registration.Raster.Mode"),
         }
 
     def show_summary(self, fig=None, plot=True, **kargs):
-        from . import funit
+        from .utils import funit
 
         s = self.get_summary(numeric=False)
         print(
             """
         Analysis time: {AnalysisTime}
         Delayed extraction: {ExtractionDelay}
         Floodgun: {Floodgun}
@@ -375,16 +375,20 @@
         -------
         pySPM.SPM.SPM_image
             A SPM_image created with the data of a given array.
 
         Example
         -------
         >>> A = pySPM.ITA("myfile.ita")
-        >>> Au,_ = A.getAddedImageByName("Au") # retrieve the gold channel (total counts)
-        >>> Au_tofcorr = A.image(-np.log(1-np.fmin(.999, Au.pixels(A.Nscan))), "Au", zscale="yield") # Create a new image with the tof-corrected data
+        >>> Au, _ = A.getAddedImageByName(
+        ...     "Au"
+        ... )  # retrieve the gold channel (total counts)
+        >>> Au_tofcorr = A.image(
+        ...     -np.log(1 - np.fmin(0.999, Au.pixels(A.Nscan))), "Au", zscale="yield"
+        ... )  # Create a new image with the tof-corrected data
         """
         from .SPM import SPM_image
 
         return SPM_image(
             I, real=self.size["real"], _type="TOF", zscale=zscale, channel=channel
         )
```

### Comparing `pyspm-0.6.1/pySPM/ITS.py` & `pyspm-0.6.2/pySPM/ITS.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/PCA.py` & `pyspm-0.6.2/pySPM/PCA.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         columns = pd.MultiIndex.from_tuples(
             [
                 ("sdev", "Standard deviation"),
                 ("varprop", "Proportion of Variance"),
                 ("cumprop", "Cumulative Proportion"),
             ]
         )
-        Z = zip(a, b, c)
+        Z = zip(a, b, c, strict=False)
         summary = pd.DataFrame(list(Z), index=names, columns=columns)
         return summary
 
     def screeplot(self, ax=None, num=None):
         if self.pca is None:
             self.run_pca()
         ax = ax if ax is not None else plt.gca()
@@ -179,23 +179,24 @@
 
         foo = self.get_pca_transf()
         if classifs is None:
             if light:
                 plt.scatter(foo[:, 0], foo[:, 1])
             else:
                 bar = pd.DataFrame(
-                    list(zip(foo[:, 0], foo[:, 1])), columns=["PC1", "PC2"]
+                    list(zip(foo[:, 0], foo[:, 1], strict=False)),
+                    columns=["PC1", "PC2"],
                 )
                 sns.lmplot("PC1", "PC2", bar, fit_reg=False)
         else:
             if light:
                 plt.scatter(foo[:, 0], foo[:, 1], color=cm.Scalar)
             else:
                 bar = pd.DataFrame(
-                    list(zip(foo[:, 0], foo[:, 1], classifs)),
+                    list(zip(foo[:, 0], foo[:, 1], classifs, strict=False)),
                     columns=["PC1", "PC2", "Class"],
                 )
                 sns.lmplot("PC1", "PC2", bar, hue="Class", fit_reg=False)
 
 
 class ITA_PCA(PCA):
     def __init__(self, c, channels=None):
```

### Comparing `pyspm-0.6.1/pySPM/SPM.py` & `pyspm-0.6.2/pySPM/SPM.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,20 +184,20 @@
         fontsize : float
             The fontsize used to display the text
 
         Example
         -------
         >>> img = pySPM.SPM_image()
         >>> img.show()
-        >>> img.add_scale(50e-6, pixels=False);
+        >>> img.add_scale(50e-6, pixels=False)
         Add a scale of 50 μm on an image displayed with real units
 
         >>> img = pySPM.SPM_image()
         >>> img.show(pixels=True)
-        >>> img.add_scale(50e-6);
+        >>> img.add_scale(50e-6)
         Add a scale of 50 μm on an image displayed in pixels
         """
 
         import matplotlib.patches
         import matplotlib.patheffects
 
         fL = length / self.size["real"]["x"]
@@ -293,24 +293,24 @@
             axPixels: set to True if you axis "ax" have the data plotted in pixel instead of real distance
 
         Example
         -------
         Exampel if the data are plotted in pixels:
         >>> topo = pySPM.SPM_image(...)
         >>> fig, ax = plt.subplots(1, 2, figsize=(10, 5))
-        >>> topoC = topo.offset([[150, 0, 220, 255]], inline=False,axPixels=True)
+        >>> topoC = topo.offset([[150, 0, 220, 255]], inline=False, axPixels=True)
         >>> topo.show(pixels=True, ax=ax[0])
-        >>> topoC.show(ax=ax[1]);
+        >>> topoC.show(ax=ax[1])
 
         Example if the data are plotted with real units
         >>> topo = pySPM.SPM_image(...)
         >>> fig, ax = plt.subplots(1, 2, figsize=(10, 5))
         >>> topoC = topo.offset([[150, 0, 220, 255]], inline=False)
         >>> topo.show(ax=ax[0])
-        >>> topoC.show(ax=ax[1]);
+        >>> topoC.show(ax=ax[1])
         """
         offset = np.zeros(self.pixels.shape[0])
         counts = np.zeros(self.pixels.shape[0])
         for i, p in enumerate(profiles):
             if kargs.get("labels", False):
                 y, D = self.get_row_profile(
                     *p, width=width, ax=ax, col=col, label=str(i), **kargs
@@ -668,20 +668,31 @@
         matplotlib.image.AxesImage
             matplolib axis instance returned by imshow
 
         Examples
         --------
         >>> topo = pySPM.SPM_image(...)
         >>> fig, (ax, ax2) = plt.subplots(2, 3, figsize=(15, 10))
-        >>> topo.show(ax=ax[0], cmap='gray', title="color map=\"gray\"")
+        >>> topo.show(ax=ax[0], cmap="gray", title='color map="gray"')
         >>> topo.show(ax=ax[1], sig=2, title="standard deviation=2")
         >>> topo.show(ax=ax[2], adaptive=True, title="Adaptive colormap")
-        >>> topo.show(ax=ax2[0], dmin=4e-8, cmap='gray', title="raise the lowest value for the colormap of +40nm")
-        >>> topo.show(ax=ax2[1], dmin=3e-8, dmax=-3e-8, cmap='gray',title="raise lower of +30nm and highest of -30nm")
-        >>> topo.show(ax=ax2[2], pixels=True, title="Set axis value in pixels");
+        >>> topo.show(
+        ...     ax=ax2[0],
+        ...     dmin=4e-8,
+        ...     cmap="gray",
+        ...     title="raise the lowest value for the colormap of +40nm",
+        ... )
+        >>> topo.show(
+        ...     ax=ax2[1],
+        ...     dmin=3e-8,
+        ...     dmax=-3e-8,
+        ...     cmap="gray",
+        ...     title="raise lower of +30nm and highest of -30nm",
+        ... )
+        >>> topo.show(ax=ax2[2], pixels=True, title="Set axis value in pixels")
         """
         mpl.rc("axes", grid=False)
 
         if ax is None:
             ax = plt.gca()
         ax.src = self
         if title is None:
@@ -1179,16 +1190,25 @@
         -------
         dictionary : {'plot': matplotlib_plot_instance, 'l': profile_xaxis, 'z': profile_yaxis}
 
         Examples
         --------
         >>> topo = pySPM.SPM_image(...)
         >>> fig, ax = plt.subplots(1, 2, figsize=(10, 5))
-        >>> topo.plot_profile(70, 100, 170, 200, ax=ax[1], img=ax[0], ztransf=lambda x:x*1e9, zunit='nm');
-        >>> topo.show(ax=ax[0], pixels=True);
+        >>> topo.plot_profile(
+        ...     70,
+        ...     100,
+        ...     170,
+        ...     200,
+        ...     ax=ax[1],
+        ...     img=ax[0],
+        ...     ztransf=lambda x: x * 1e9,
+        ...     zunit="nm",
+        ... )
+        >>> topo.show(ax=ax[0], pixels=True)
         """
         col = kargs.get("color", kargs.get("col", "C0"))
         W = self.size["real"]["x"]
         fact = int(np.floor(np.log(W) / np.log(10) / 3)) * 3
         if ax is None:
             ax = plt.gca()
         xvalues, p = self.get_profile(
@@ -1642,15 +1662,19 @@
         self if inplace, clipped SPM_image otherwises2 = pySPM.Nanoscan("%s/CyI5b_PCB_ns.xml"%(Path))
         """
         if "inplace" in kargs:
             inline = kargs["inplace"]
         if kargs.get("debug", False):
             print("cut) Input coordinates:", c)
         if not pixels:
-            c = [z for s in zip(*self.real2pixels(c[0::2], c[1::2])) for z in s]
+            c = [
+                z
+                for s in zip(*self.real2pixels(c[0::2], c[1::2]), strict=False)
+                for z in s
+            ]
             if kargs.get("debug", False):
                 print("cut) pixel coordinates:", c)
         if not inline:
             new = copy.deepcopy(self)
             new.pixels = cut(self.pixels, c, **kargs)
             new._resize_infos()
             return new
```

### Comparing `pyspm-0.6.1/pySPM/SXM.py` & `pyspm-0.6.2/pySPM/SXM.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/ToF.py` & `pyspm-0.6.2/pySPM/ToF.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         assert ID >= 0 and self.header[1] >= ID
         self.f.seek(32 + ID * (4 * self.N + 16))
         return np.array(
             struct.unpack(str(self.N) + "I", self.f.read(4 * self.N))
         ).reshape(self.size)
 
     def getImgMass(self, masses, raw=False):
-        if isinstance(masses, (float, int)):
+        if isinstance(masses, float | int):
             masses = [masses]
         SUM = None
         for i, x in enumerate(self.cat):
             for m in masses:
                 if m >= x[0] - 0.5 and m <= x[1] + 0.5:
                     if SUM is None:
                         SUM = self.getImgID(i)
@@ -175,15 +175,15 @@
     def getIDs(self, channels):
         assert type(channels) in [str, int, list, tuple]
         if isinstance(channels, int):
             return channels
         if isinstance(channels, str):
             assert channels in self.RPeaks
             return self.RPeaks[channels]
-        if isinstance(channels, (list, tuple)):
+        if isinstance(channels, list | tuple):
             ID = []
             for x in channels:
                 ID.append(self.getIDs(x))
             return ID
 
     def getChannel(self, channel):
         k = self.getIDs(channel)
```

### Comparing `pyspm-0.6.1/pySPM/__init__.py` & `pyspm-0.6.2/pySPM/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/__main__.py` & `pyspm-0.6.2/pySPM/__main__.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/align.py` & `pyspm-0.6.2/pySPM/align.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/collection.py` & `pyspm-0.6.2/pySPM/collection.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/data/elements.db` & `pyspm-0.6.2/pySPM/data/elements.db`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/mplwidget.py` & `pyspm-0.6.2/pySPM/mplwidget.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/nanoscan.py` & `pyspm-0.6.2/pySPM/nanoscan.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/slicer.py` & `pyspm-0.6.2/pySPM/slicer.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/tools/emission_current_plotter.py` & `pyspm-0.6.2/pySPM/tools/emission_current_plotter.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/tools/fpanel.py` & `pyspm-0.6.2/pySPM/tools/fpanel.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/tools/mplwidget.py` & `pyspm-0.6.2/pySPM/tools/mplwidget.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/tools/spectra.py` & `pyspm-0.6.2/pySPM/tools/spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         if colors is None:
             colors = ["r", "g", "b"]
         r = self.ax.get_xlim()
         E = []
         for nm in range(int(np.round(r[0], 0)), int(np.round(r[1], 0)) + 1):
             E += pySPM.utils.get_peaklist(nm, self.ita.polarity == "Negative")
         m0s = [pySPM.utils.get_mass(x) for x in E]
-        P = list(zip(m0s, E))
+        P = list(zip(m0s, E, strict=False))
         P.sort(key=lambda x: x[0])
         y = self.ax.get_ylim()[1]
         for i, (mi, Ei) in enumerate(P):
             dmi = (
                 2
                 * np.sqrt(mi)
                 * np.sqrt(
```

### Comparing `pyspm-0.6.1/pySPM/tools/spectraviewer.py` & `pyspm-0.6.2/pySPM/tools/spectraviewer.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/tools/spectraviewer.ui` & `pyspm-0.6.2/pySPM/tools/spectraviewer.ui`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/tools/stability.py` & `pyspm-0.6.2/pySPM/tools/stability.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/tools/timer_display.py` & `pyspm-0.6.2/pySPM/tools/timer_display.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/tools/timer_display.ui` & `pyspm-0.6.2/pySPM/tools/timer_display.ui`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/tools/tof_timer.py` & `pyspm-0.6.2/pySPM/tools/tof_timer.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/tools/values_display.py` & `pyspm-0.6.2/pySPM/tools/values_display.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/tools/win32_helper.py` & `pyspm-0.6.2/pySPM/tools/win32_helper.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/utils/__init__.py` & `pyspm-0.6.2/pySPM/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     Returns
     -------
     dictionary with formated 'value' and 'unit'.
     The value will be: ≥1 and <1000
 
     Examples
     --------
-    >>> funit(0.01,'m')
+    >>> funit(0.01, "m")
     {'value': 10.0, 'unit': 'mm'}
-    >>> funit(1, 'cm')
+    >>> funit(1, "cm")
     {'value': 1.0, 'unit': 'cm'}
-    >>> funit({'value':2340, 'unit': 'um'})
+    >>> funit({"value": 2340, "unit": "um"})
     {'value': 2.34, 'unit': 'mm'}
     """
     if unit is None:
         unit = value["unit"]
         value = value["value"]
     import math
 
@@ -270,15 +270,15 @@
 
 
 def getToFsimg(I, N=None, prog=False):
     if N is None:
         N = [10, 50, 100, 300, 500]
     Ns = np.insert(np.diff(N), 0, N[0])
     T = [getToFimg(I, n) for n in Ns]
-    return dict(zip(N, np.cumsum(T, axis=0)))
+    return dict(zip(N, np.cumsum(T, axis=0), strict=False))
 
 
 def centered_meshgrid(A):
     w = A.shape[1]
     h = A.shape[0]
     Y, X = np.mgrid[-h // 2 : h // 2, -w // 2 : w // 2]
     return Y, X
```

### Comparing `pyspm-0.6.1/pySPM/utils/elts.py` & `pyspm-0.6.2/pySPM/utils/elts.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,15 +394,17 @@
 
     r = [({}, 0)]
     res = []
     if isinstance(elts, str):
         elts = re.compile(r"((?:^[0-9]+)?[A-Z][a-z]?(?:_[0-9]+)?)").findall(elts)
     me = [get_mass(x) for x in elts]
     while r:
-        rnew = _elts_add(r, list(zip([_formula2dict(x) for x in elts], me)))
+        rnew = _elts_add(
+            r, list(zip([_formula2dict(x) for x in elts], me, strict=False))
+        )
         r = [x for x in rnew if x[1] < NM + 0.5]
         res += [
             _dict2formula(x[0])
             for x in r
             if x[1] > NM - 0.5
             if _dict2formula(x[0]) not in res
         ]
```

### Comparing `pyspm-0.6.1/pySPM/utils/fit.py` & `pyspm-0.6.2/pySPM/utils/fit.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,19 @@
         xi: position
         si: sigma of CDF
                      _
     ex: step edge: _| |_ between 0.2 and 0.7 in y and -1 and 1 in x with sigma=5
         CDF(x, 0.2, 0.5, -1, 5, -0.5, 1, 5)
     """
     if "A" in kargs and "x0" in kargs and "sig" in kargs:
-        args = [x for y in zip(kargs["A"], kargs["x0"], kargs["sig"]) for x in y]
+        args = [
+            x
+            for y in zip(kargs["A"], kargs["x0"], kargs["sig"], strict=False)
+            for x in y
+        ]
 
     r = bg * np.ones(x.shape)
     if len(args) % 3 != 0:
         raise Exception("Invalid number of arguments. see help.")
         return
 
     for i in range(len(args) // 3):
@@ -71,15 +75,19 @@
         si: sigma of CDF
                      _
     ex: step edge: _| |_ between 0.2 and 0.7 in y and -1 and 1 in x with sigma=5
         lgCDF(x, lg, 0.2, 0.5, -1, 5, -0.5, 1, 5)
     """
 
     if "A" in kargs and "x0" in kargs and "sig" in kargs:
-        args = [x for y in zip(kargs["A"], kargs["x0"], kargs["sig"]) for x in y]
+        args = [
+            x
+            for y in zip(kargs["A"], kargs["x0"], kargs["sig"], strict=False)
+            for x in y
+        ]
 
     r = bg * np.ones(x.shape)
     if len(args) % 3 != 0:
         raise Exception("Invalid number of arguments. see help.")
         return
 
     for i in range(len(args) // 3):
@@ -192,15 +200,17 @@
             pout.append(pfit[0][j])
             dpout.append(np.sqrt(pfit[1][j, j]))
             j += 1
     pout = pout[:2] + [ratio * pout[2]] + pout[2:]
     dpout = dpout[:2] + [ratio * dpout[2]] + dpout[2:]
     if dic:
         params2 = params[:2] + ["sig_x"] + params[2:]
-        return dict(zip(params2, pout)), dict(zip(params2, dpout))
+        return dict(zip(params2, pout, strict=False)), dict(
+            zip(params2, dpout, strict=False)
+        )
     return pout, dpout
 
 
 def LG2D(A, Rweight=None, sigma=None, dic=False, **kargs):
     """
     Perform a 2D Lorentz-Gauss fitting on a 2D array A
     dic: if True return the solution as a dictionary
@@ -285,15 +295,17 @@
             dpout.append(0)
         else:
             pout.append(pfit[0][j])
             dpout.append(np.sqrt(pfit[1][j, j]))
             j += 1
 
     if dic:
-        return dict(zip(params, pout)), dict(zip(params, dpout))
+        return dict(zip(params, pout, strict=False)), dict(
+            zip(params, dpout, strict=False)
+        )
     return pout, dpout
 
 
 def LG2Da(A, Rweight=None, sigma=None, dic=False, **kargs):
     """
     Perform a 2D Lorentz-Gauss fitting on a 2D array A
     dic: if True return the solution as a dictionary
@@ -383,9 +395,11 @@
             dpout.append(0)
         else:
             pout.append(pfit[0][j])
             dpout.append(np.sqrt(pfit[1][j, j]))
             j += 1
 
     if dic:
-        return dict(zip(params, pout)), dict(zip(params, dpout))
+        return dict(zip(params, pout, strict=False)), dict(
+            zip(params, dpout, strict=False)
+        )
     return pout, dpout
```

### Comparing `pyspm-0.6.1/pySPM/utils/geometry.py` & `pyspm-0.6.2/pySPM/utils/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         elif len(args) == 1:
             assert isinstance(args[0], dict)
             self.left = args[0]["left"]
             self.right = args[0]["right"]
             self.top = args[0]["top"]
             self.bottom = args[0]["bottom"]
         elif len(args) == 3:
-            assert isinstance(args[0], (list, tuple))
+            assert isinstance(args[0], list | tuple)
             self.left = args[0][0]
             self.bottom = args[0][1]
             self.right = self.left + args[1]
             self.top = self.bottom + args[2]
         else:
             assert len(args) == 4
             self.left = args[0]
```

### Comparing `pyspm-0.6.1/pySPM/utils/haar.py` & `pyspm-0.6.2/pySPM/utils/haar.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/utils/math.py` & `pyspm-0.6.2/pySPM/utils/math.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/utils/misc.py` & `pyspm-0.6.2/pySPM/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/utils/plot.py` & `pyspm-0.6.2/pySPM/utils/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,15 @@
 
 
 def put_Xlabels(
     ax, pos, labels, colors="rgb", debug=False, save=False, bbox=False, **kargs
 ):
     fig = ax.get_figure()
     renderer = fig.canvas.get_renderer()
-    P = list(zip(pos, labels))
+    P = list(zip(pos, labels, strict=False))
     P.sort(key=lambda x: x[0])  # sort labels by ascending x
     labs = []
     ax.draw(renderer)  # make sure to draw the new object
     ylim = ax.get_ylim()
     objs = [o for o in ax.get_children() if type(o) not in [mpl.patches.Rectangle]]
     coli = [None, None]
     for i, (x, lab) in enumerate(P):
```

### Comparing `pyspm-0.6.1/pySPM/utils/progressbar.py` & `pyspm-0.6.2/pySPM/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/utils/restoration.py` & `pyspm-0.6.2/pySPM/utils/restoration.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/utils/save.py` & `pyspm-0.6.2/pySPM/utils/save.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pySPM/utils/spectra.py` & `pyspm-0.6.2/pySPM/utils/spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     else:
         E = []
     if negative:
         E = [x + ["-", ""]["-" in x] for x in E]
     if do_debug(debug):
         print("Selected Elements: " + ", ".join(E))
     m0s = [get_mass(x) for x in E]
-    E = [x for x, y in zip(E, m0s) if y >= lower_mass and y <= upper_mass]
+    E = [x for x, y in zip(E, m0s, strict=False) if y >= lower_mass and y <= upper_mass]
     m0s = [get_mass(x) for x in E]
     E_labels = [formulafy(x) for x in E] if formula else E
     if do_debug(debug):
         print("Displayed elements:", ", ".join(E))
 
     Dt = np.copy(D[mask])
     mt = m[mask]
@@ -386,24 +386,24 @@
         elif pretty:
             put_Xlabels(
                 ax, m0s, E_labels, color=colors, debug=dec_debug(debug), **kargs
             )
 
         if "dsf" in kargs and "dk0" in kargs and "sf" in kargs and "k0" in kargs:
             sf, dsf, k0, dk0 = (kargs[x] for x in "sf,dsf,k0,dk0".split(","))
-            P = list(zip(m0s, E))
+            P = list(zip(m0s, E, strict=False))
             P.sort(key=lambda x: x[0])
             for i, (mi, Ei) in enumerate(P):
                 col = colors[i % len(colors)]
                 dmi = get_dm(mi, sf, k0, dsf, dk0)
                 ax.axvline(mi - dmi, color=col, alpha=0.5, linestyle=":")
                 ax.axvline(mi + dmi, color=col, alpha=0.5, linestyle=":")
 
         if not pretty:
-            P = list(zip(m0s, E_labels))
+            P = list(zip(m0s, E_labels, strict=False))
             P.sort(key=lambda x: x[0])
             y = ax.get_ylim()[1]
             for i, (mi, Ei) in enumerate(P):
                 col = colors[i % len(colors)]
                 ax.axvline(mi, color=col, alpha=0.5)
                 ax.annotate(
                     Ei,
```

### Comparing `pyspm-0.6.1/pySPM/utils/units.py` & `pyspm-0.6.2/pySPM/utils/units.py`

 * *Files identical despite different names*

### Comparing `pyspm-0.6.1/pyproject.toml` & `pyspm-0.6.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyspm"
-version = "0.6.1"
+version = "0.6.2"
 description = "Library to handle SPM and ToF-SIMS data"
 authors = ["Olivier Scholder <o.scholder@gmail.com>"]
 maintainers = ["Dinesh Pinto <annual.fallout_0z@icloud.com>"]
 homepage = "https://github.com/scholi/pySPM"
 repository = "https://github.com/scholi/pySPM"
 license = "Apache-2.0"
 readme = "README.md"
@@ -37,36 +37,33 @@
 ruff-lsp = "^0.0.49"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
+target-version = "py310"
+
+[tool.ruff.lint]
 extend-select = [
+    "E", # pycodestyle-error
+    "W", # pycodestyle-warning
+    "F", # pyflakes
+    "N", # pep8-naming
     "B", # flake8-bugbear
+    "I", # isort
+    "ASYNC", # flake8-async
+    "BLE", # flake8-blind-except
+    "A", # flake8-builtins
     "C4", # flake8-comprehensions
     "ERA", # flake8-eradicate/eradicate
-    "I", # isort
-    "N", # pep8-naming
     "PIE", # flake8-pie
     "PGH", # pygrep
     "RUF", # ruff checks
     "SIM", # flake8-simplify
     "TCH", # flake8-type-checking
     "TID", # flake8-tidy-imports
     "UP", # pyupgrade
 ]
-ignore = [
-    "N806", # variable in function should be lowercase
-    "N802", # function name should be lowercase
-    "N801", # class name should use CapWords convention
-    "ERA001", # eradicate: Found commented out code
-    "N803", # argument name should be lowercase
-    "E741", # ambiguous variable name
-    "E722", # do not use bare except
-    "RUF001",
-    "RUF003",
-    "N999",
-    "F405",
-    "F403",
-    "SIM115",
-]
+
+[tool.ruff.format]
+docstring-code-format = true
```

### Comparing `pyspm-0.6.1/PKG-INFO` & `pyspm-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspm
-Version: 0.6.1
+Version: 0.6.2
 Summary: Library to handle SPM and ToF-SIMS data
 Home-page: https://github.com/scholi/pySPM
 License: Apache-2.0
 Keywords: ToF,SIMS,ION-ToF,SPM,SFM,SXM,AFM,KPFM,PCA,ITA,imaging,ITM,Bruker,Nanonis
 Author: Olivier Scholder
 Author-email: o.scholder@gmail.com
 Maintainer: Dinesh Pinto
```

