# Comparing `tmp/mwtoolbox-0.0.7.tar.gz` & `tmp/mwtoolbox-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwtoolbox-0.0.7.tar", last modified: Wed Apr 17 09:11:33 2024, max compression
+gzip compressed data, was "mwtoolbox-0.0.8.tar", last modified: Fri May 10 09:03:50 2024, max compression
```

## Comparing `mwtoolbox-0.0.7.tar` & `mwtoolbox-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 09:11:33.403808 mwtoolbox-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-05-09 08:27:16.000000 mwtoolbox-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1076 2024-04-17 09:11:33.402764 mwtoolbox-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      465 2024-04-17 09:11:27.000000 mwtoolbox-0.0.7/README.md
--rw-rw-rw-   0        0        0     3341 2024-04-17 09:11:27.000000 mwtoolbox-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 09:11:33.403808 mwtoolbox-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 09:11:33.365697 mwtoolbox-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 09:11:33.389719 mwtoolbox-0.0.7/src/mwtoolbox/
--rw-rw-rw-   0        0        0      138 2024-04-17 09:11:27.000000 mwtoolbox-0.0.7/src/mwtoolbox/__init__.py
--rw-rw-rw-   0        0        0    76586 2023-06-14 12:48:56.000000 mwtoolbox-0.0.7/src/mwtoolbox/components.py
--rw-rw-rw-   0        0        0    15140 2023-05-23 13:47:25.000000 mwtoolbox-0.0.7/src/mwtoolbox/filters.py
--rw-rw-rw-   0        0        0    19885 2023-09-08 15:41:32.000000 mwtoolbox-0.0.7/src/mwtoolbox/genel.py
--rw-rw-rw-   0        0        0      414 2022-07-19 09:02:27.000000 mwtoolbox-0.0.7/src/mwtoolbox/myconstants.py
--rw-rw-rw-   0        0        0    16284 2023-10-13 07:56:27.000000 mwtoolbox-0.0.7/src/mwtoolbox/network.py
--rw-rw-rw-   0        0        0    15327 2023-10-11 06:16:46.000000 mwtoolbox-0.0.7/src/mwtoolbox/networksym.py
--rw-rw-rw-   0        0        0   159951 2024-04-10 06:14:55.000000 mwtoolbox-0.0.7/src/mwtoolbox/rfnetwork.py
--rw-rw-rw-   0        0        0   142167 2023-07-02 15:36:38.000000 mwtoolbox-0.0.7/src/mwtoolbox/transmission_lines.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:11:33.401719 mwtoolbox-0.0.7/src/mwtoolbox.egg-info/
--rw-rw-rw-   0        0        0     1076 2024-04-17 09:11:33.000000 mwtoolbox-0.0.7/src/mwtoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2024-04-17 09:11:33.000000 mwtoolbox-0.0.7/src/mwtoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 09:11:33.000000 mwtoolbox-0.0.7/src/mwtoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-17 09:11:33.000000 mwtoolbox-0.0.7/src/mwtoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-17 09:11:33.000000 mwtoolbox-0.0.7/src/mwtoolbox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 09:11:33.400719 mwtoolbox-0.0.7/tests/
--rw-rw-rw-   0        0        0      796 2023-05-09 20:25:20.000000 mwtoolbox-0.0.7/tests/test1.py
--rw-rw-rw-   0        0        0      473 2023-05-09 20:25:16.000000 mwtoolbox-0.0.7/tests/test2.py
--rw-rw-rw-   0        0        0      320 2023-07-02 15:34:38.000000 mwtoolbox-0.0.7/tests/test_embedded_microstrip.py
--rw-rw-rw-   0        0        0      315 2023-06-14 12:08:25.000000 mwtoolbox-0.0.7/tests/test_microstrip_synthesis.py
--rw-rw-rw-   0        0        0      812 2023-05-09 20:25:00.000000 mwtoolbox-0.0.7/tests/tests.py
--rw-rw-rw-   0        0        0      962 2023-05-09 20:24:48.000000 mwtoolbox-0.0.7/tests/tests4.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:03:50.821296 mwtoolbox-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-05-09 08:27:16.000000 mwtoolbox-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1076 2024-05-10 09:03:50.819284 mwtoolbox-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2024-04-17 09:11:27.000000 mwtoolbox-0.0.8/README.md
+-rw-rw-rw-   0        0        0     3341 2024-05-10 09:03:44.000000 mwtoolbox-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 09:03:50.821296 mwtoolbox-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 09:03:50.773149 mwtoolbox-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 09:03:50.795075 mwtoolbox-0.0.8/src/mwtoolbox/
+-rw-rw-rw-   0        0        0      138 2024-05-10 09:03:44.000000 mwtoolbox-0.0.8/src/mwtoolbox/__init__.py
+-rw-rw-rw-   0        0        0    76586 2023-06-14 12:48:56.000000 mwtoolbox-0.0.8/src/mwtoolbox/components.py
+-rw-rw-rw-   0        0        0    15140 2023-05-23 13:47:25.000000 mwtoolbox-0.0.8/src/mwtoolbox/filters.py
+-rw-rw-rw-   0        0        0    19885 2023-09-08 15:41:32.000000 mwtoolbox-0.0.8/src/mwtoolbox/genel.py
+-rw-rw-rw-   0        0        0      414 2022-07-19 09:02:27.000000 mwtoolbox-0.0.8/src/mwtoolbox/myconstants.py
+-rw-rw-rw-   0        0        0    16284 2023-10-13 07:56:27.000000 mwtoolbox-0.0.8/src/mwtoolbox/network.py
+-rw-rw-rw-   0        0        0    15327 2023-10-11 06:16:46.000000 mwtoolbox-0.0.8/src/mwtoolbox/networksym.py
+-rw-rw-rw-   0        0        0   166715 2024-05-01 17:13:06.000000 mwtoolbox-0.0.8/src/mwtoolbox/rfnetwork.py
+-rw-rw-rw-   0        0        0   142167 2023-07-02 15:36:38.000000 mwtoolbox-0.0.8/src/mwtoolbox/transmission_lines.py
+drwxrwxrwx   0        0        0        0 2024-05-10 09:03:50.817282 mwtoolbox-0.0.8/src/mwtoolbox.egg-info/
+-rw-rw-rw-   0        0        0     1076 2024-05-10 09:03:50.000000 mwtoolbox-0.0.8/src/mwtoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2024-05-10 09:03:50.000000 mwtoolbox-0.0.8/src/mwtoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 09:03:50.000000 mwtoolbox-0.0.8/src/mwtoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-10 09:03:50.000000 mwtoolbox-0.0.8/src/mwtoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-10 09:03:50.000000 mwtoolbox-0.0.8/src/mwtoolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 09:03:50.814213 mwtoolbox-0.0.8/tests/
+-rw-rw-rw-   0        0        0      796 2023-05-09 20:25:20.000000 mwtoolbox-0.0.8/tests/test1.py
+-rw-rw-rw-   0        0        0      473 2023-05-09 20:25:16.000000 mwtoolbox-0.0.8/tests/test2.py
+-rw-rw-rw-   0        0        0      320 2023-07-02 15:34:38.000000 mwtoolbox-0.0.8/tests/test_embedded_microstrip.py
+-rw-rw-rw-   0        0        0      315 2023-06-14 12:08:25.000000 mwtoolbox-0.0.8/tests/test_microstrip_synthesis.py
+-rw-rw-rw-   0        0        0      812 2023-05-09 20:25:00.000000 mwtoolbox-0.0.8/tests/tests.py
+-rw-rw-rw-   0        0        0      962 2023-05-09 20:24:48.000000 mwtoolbox-0.0.8/tests/tests4.py
```

### Comparing `mwtoolbox-0.0.7/LICENSE` & `mwtoolbox-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.7/PKG-INFO` & `mwtoolbox-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwtoolbox
-Version: 0.0.7
+Version: 0.0.8
 Summary: Microwave Toolbox
 Author-email: Tuncay Erdöl <terdol@hotmail.com>
 License: MIT
 Keywords: microwave,rf,s-parameters
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mwtoolbox-0.0.7/pyproject.toml` & `mwtoolbox-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 6275 696c 642d 6261 636b 656e 6420 3d20  build-backend = 
 00000020: 2773 6574 7570 746f 6f6c 732e 6275 696c  'setuptools.buil
 00000030: 645f 6d65 7461 270d 0a72 6571 7569 7265  d_meta'..require
 00000040: 7320 3d20 5b27 7365 7475 7074 6f6f 6c73  s = ['setuptools
 00000050: 272c 2027 7768 6565 6c27 5d0d 0a0d 0a5b  ', 'wheel']....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6d77 746f 6f6c 626f 7822 0d0a 7665   "mwtoolbox"..ve
-00000080: 7273 696f 6e20 3d20 2230 2e30 2e37 220d  rsion = "0.0.7".
+00000080: 7273 696f 6e20 3d20 2230 2e30 2e38 220d  rsion = "0.0.8".
 00000090: 0a64 6570 656e 6465 6e63 6965 7320 3d20  .dependencies = 
 000000a0: 5b22 7175 616e 7469 7469 6573 222c 0d0a  ["quantities",..
 000000b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000000c0: 226e 756d 7079 3c32 222c 0d0a 2020 2020  "numpy<2",..    
 000000d0: 2020 2020 2020 2020 2020 2020 2273 6369              "sci
 000000e0: 7079 222c 0d0a 2020 2020 2020 2020 2020  py",..          
 000000f0: 2020 2020 2020 2273 796d 7079 222c 0d0a        "sympy",..
@@ -165,15 +165,15 @@
 00000a40: 6f63 756d 656e 7473 2f54 656b 6e69 6b2f  ocuments/Teknik/
 00000a50: 5079 7468 6f6e 2f74 7970 696e 6773 5f66  Python/typings_f
 00000a60: 6f72 5f70 7972 6967 6874 220d 0a74 7970  or_pyright"..typ
 00000a70: 6543 6865 636b 696e 674d 6f64 6520 3d20  eCheckingMode = 
 00000a80: 2262 6173 6963 220d 0a0d 0a5b 746f 6f6c  "basic"....[tool
 00000a90: 2e62 756d 7076 6572 5d0d 0a63 7572 7265  .bumpver]..curre
 00000aa0: 6e74 5f76 6572 7369 6f6e 203d 2022 302e  nt_version = "0.
-00000ab0: 302e 3722 0d0a 7665 7273 696f 6e5f 7061  0.7"..version_pa
+00000ab0: 302e 3822 0d0a 7665 7273 696f 6e5f 7061  0.8"..version_pa
 00000ac0: 7474 6572 6e20 3d20 224d 414a 4f52 2e4d  ttern = "MAJOR.M
 00000ad0: 494e 4f52 2e50 4154 4348 220d 0a63 6f6d  INOR.PATCH"..com
 00000ae0: 6d69 745f 6d65 7373 6167 6520 3d20 2262  mit_message = "b
 00000af0: 756d 7020 7665 7273 696f 6e20 7b6f 6c64  ump version {old
 00000b00: 5f76 6572 7369 6f6e 7d20 2d3e 207b 6e65  _version} -> {ne
 00000b10: 775f 7665 7273 696f 6e7d 220d 0a63 6f6d  w_version}"..com
 00000b20: 6d69 7420 3d20 7472 7565 0d0a 7461 6720  mit = true..tag
```

### Comparing `mwtoolbox-0.0.7/src/mwtoolbox/components.py` & `mwtoolbox-0.0.8/src/mwtoolbox/components.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.7/src/mwtoolbox/filters.py` & `mwtoolbox-0.0.8/src/mwtoolbox/filters.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.7/src/mwtoolbox/genel.py` & `mwtoolbox-0.0.8/src/mwtoolbox/genel.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.7/src/mwtoolbox/network.py` & `mwtoolbox-0.0.8/src/mwtoolbox/network.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.7/src/mwtoolbox/networksym.py` & `mwtoolbox-0.0.8/src/mwtoolbox/networksym.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.7/src/mwtoolbox/rfnetwork.py` & `mwtoolbox-0.0.8/src/mwtoolbox/rfnetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -617,14 +617,116 @@
     # Tlauncherout.sdata[:,2]=-Tlauncherout.sdata[:,2]
     # if np.abs(Tlauncherin.S(2,1,"phase"))[0]>90:
     # Tlauncherin.sdata[:,1]=-Tlauncherin.sdata[:,1]
     # Tlauncherin.sdata[:,2]=-Tlauncherin.sdata[:,2]
     Tlauncherout.snp2smp([2, 1], 1)
     return Tlauncherin, Tlauncherout, np.array(faz)
 
+def merge_spfiles(spfilelist):
+    """This method merges multiple SPFILEs to a single one. The aim if to merge multiple SPFILEs defined for the same network at different frequency values. All SPFILEs are assumed to represent the same network except the frequencies. Port names are taken from the first SPFILE.
+
+    Args:
+        spfilelist(list): List of SPFILE objects.
+
+    Returns:
+        SPFILE object.
+    """
+    spout = deepcopy(spfilelist[0])
+    n_ports = spfilelist[0].n_ports
+    freqs = np.concatenate(tuple(a.freqs for a in spfilelist))
+    
+    refimpedance = [None]*n_ports
+    for cc, sps in enumerate(spfilelist):
+        n_freqs = len(sps.freqs)
+        if not hasattr(sps.refimpedance,"__iter__"):
+            for j in range(n_ports):
+                if cc==0:
+                    refimpedance[j] = [sps.refimpedance]*n_freqs
+                else:
+                    refimpedance[j].extend([sps.refimpedance]*n_freqs)
+        else:
+            for i in range(n_ports):
+                if not hasattr(sps.refimpedance[i],"__iter__"):                    
+                    if cc==0:
+                        refimpedance[i] = [sps.refimpedance[i]]*n_freqs
+                    else:
+                        refimpedance[i].extend([sps.refimpedance[i]]*n_freqs)
+                else:
+                    if cc==0:
+                        refimpedance[i] = sps.refimpedance[i][:]
+                    else:
+                        refimpedance[i].extend(sps.refimpedance[i])
+
+    gammas = [None]*n_ports
+    for cc, sps in enumerate(spfilelist):
+        n_freqs = len(sps.freqs)
+        if not hasattr(sps.gammas,"__iter__"):
+            for j in range(n_ports):
+                if cc==0:
+                    gammas[j] = [sps.gammas]*n_freqs
+                else:
+                    gammas[j].extend([sps.gammas]*n_freqs)
+        else:
+            for i in range(n_ports):
+                if not hasattr(sps.gammas[i],"__iter__"):                    
+                    if cc==0:
+                        gammas[i] = [sps.gammas[i]]*n_freqs
+                    else:
+                        gammas[i].extend([sps.gammas[i]]*n_freqs)
+                else:
+                    if cc==0:
+                        gammas[i] = list(sps.gammas[i][:])
+                    else:
+                        gammas[i].extend(sps.gammas[i])
+
+    roworder = freqs.argsort()
+    spout.freqs = freqs[roworder]
+    try:
+        spout.refimpedance = [[refimpedance[p][k] for k in roworder] for p in range(n_ports)]
+        spout.gammas = [[gammas[p][k] for k in roworder] for p in range(n_ports)]
+    except Exception as e:
+        print(repr(e))
+
+    try:
+        sdata = np.concatenate(tuple(a.sdata for a in spfilelist))
+        spout.sdata = sdata[roworder,:]
+    except Exception as e:
+        spout.sdata = None
+    try:
+        ydata = np.concatenate(tuple(a.ydata for a in spfilelist))
+        spout.ydata = ydata[roworder,:]
+    except Exception as e:
+        spout.ydata = None
+    try:
+        zdata = np.concatenate(tuple(a.zdata for a in spfilelist))
+        spout.zdata = zdata[roworder,:]
+    except Exception as e:
+        spout.zdata = None
+    try:
+        abcddata = np.concatenate(tuple(a.abcddata for a in spfilelist))
+        spout.abcddata = abcddata[roworder,:]
+    except Exception as e:
+        spout.abcddata = None
+    try:
+        tdata = np.concatenate(tuple(a.tdata for a in spfilelist))
+        spout.tdata = tdata[roworder,:]
+    except Exception as e:
+        spout.tdata = None
+    try:
+        hdata = np.concatenate(tuple(a.hdata for a in spfilelist))
+        spout.hdata = hdata[roworder,:]
+    except Exception as e:
+        spout.hdata = None
+    try:
+        gdata = np.concatenate(tuple(a.gdata for a in spfilelist))
+        spout.gdata = gdata[roworder,:]
+    except Exception as e:
+        spout.gdata = None
+
+    return spout
 
 class spfile:
     """Class that represents an RF network. It can be used to read/write Touchstone files and process RF networks.
 
     Attributes:
         file_data_format(str): Format of the data in the file if the data is read from a Touchstone file. Possible values are "DB", "MA", "RI".
         file_freq_unit(str):
@@ -664,14 +766,16 @@
                  only_port_number=False):
         self.file_data_format = "DB"
         self.file_freq_unit = "HZ"
         self.refimpedance = []
         self.sdata = None
         self.ydata = None
         self.zdata = None
+        self.hdata = None
+        self.gdata = None
         self.abcddata = None
         self.tdata = None
         self.port_names = []
         self.gammas = []  #np.array with shape (n_ports, frequencypoints)
         self.inplace = 1
         self.z_ok = False
         self.y_ok = False
@@ -998,20 +1102,69 @@
         for i in range(newps):
             for j in range(newps):
                 n = (i) * newps + (j)
                 m = (ports[i] - 1) * ps + (ports[j] - 1)
                 new_sdata[:, n] = sdata[:, m]
         obj.sdata = new_sdata
         obj.n_ports = newps
-        obj.refimpedance = [obj.refimpedance[x - 1] for x in ports]
+        try:
+            obj.refimpedance = [obj.refimpedance[x - 1] for x in ports]
+        except TypeError:
+            pass
+        try:
+            obj.gammas = [obj.gammas[x - 1] for x in ports]
+        except Exception as e:
+            print(repr(e))
         names = obj.port_names
         obj.port_names = [names[ports[i] - 1] for i in range(obj.n_ports)]
         obj.z_ok, obj.y_ok, obj.abcd_ok, obj.t_ok = False, False, False, False
         return obj
 
+    def remove_duplicate_freqs(self, abstol=None, reltol=None, inplace=-1):
+        """This function removes duplicate frequency points. Latter frequency point is retained.
+        Args:
+            abstol(float, optional): If given, used as absolute minimum difference between the frequencies to be compared. Default is None.        
+            reltol(float, optional): If given, used as relative minimum difference between the frequencies to be compared. Default is None.        
+        Returns:
+            SPFILE object
+        """
+        if inplace == -1: inplace = self.inplace
+        if inplace == 0:
+            obj = deepcopy(self)
+            obj.inplace = 1
+        else:
+            obj = self
+        points_to_be_deleted = []
+        for i in range(len(obj.freqs)-1):
+            abscriteria = False
+            if abstol:
+                abscriteria = obj.freqs[i] > (obj.freqs[i+1] - abstol)
+            relcriteria = False
+            if reltol:
+                relcriteria = obj.freqs[i] > (obj.freqs[i+1] * (1-reltol))
+            if (abscriteria and relcriteria):
+                points_to_be_deleted.append(i+1)
+        # print(f"{points_to_be_deleted=}")
+        obj.freqs = np.delete(obj.freqs, points_to_be_deleted)
+        # print(obj.refimpedance)
+        try:
+            obj.refimpedance = [[obj.refimpedance[p][k] for k in range(len(obj.refimpedance[p])) if k not in points_to_be_deleted] for p in range(obj.n_ports)]
+            obj.gammas = [[obj.gammas[p][k] for k in range(len(obj.gammas[p])) if k not in points_to_be_deleted] for p in range(obj.n_ports)]
+        except Exception as e:
+            print(repr(e))
+        if obj.sdata is not None: obj.sdata = np.delete(obj.sdata, points_to_be_deleted, axis=0)
+        if obj.ydata is not None: obj.ydata = np.delete(obj.ydata, points_to_be_deleted, axis=0)
+        if obj.zdata is not None: obj.zdata = np.delete(obj.zdata, points_to_be_deleted, axis=0)
+        if obj.abcddata is not None: obj.abcddata = np.delete(obj.abcddata, points_to_be_deleted, axis=0)
+        if obj.tdata is not None: obj.tdata = np.delete(obj.tdata, points_to_be_deleted, axis=0)
+        if obj.gdata is not None: obj.gdata = np.delete(obj.gdata, points_to_be_deleted, axis=0)
+        if obj.hdata is not None: obj.hdata = np.delete(obj.hdata, points_to_be_deleted, axis=0)
+
+        return obj
+
     def scaledata(self, scale=1.0, dataindices=None):
         """
         Multiply all elements in S-Parameter matrices by *scale*.
         """
         if not dataindices:
             for i in range(self.n_ports**2):
                 self.sdata[:, i] = self.sdata[:, i] * scale
@@ -1047,15 +1200,15 @@
             else:
                 print("Wrong file extension!")
                 return 0
 
         try:
             with open(file_name, 'r') as f:
                 linesread = f.readlines()[skiplines:]
-        except:
+        except Exception as e:
             print("Error opening the file: " + file_name + "\n")
             sys.exit(0)
         self.header = [
             l for l in linesread if (l.startswith("! ") and not (
                 l.startswith("! Port Impedance") or l.startswith("! Gamma")))
         ]
         lines = []
@@ -1189,20 +1342,20 @@
 
         # frequencies should increase monotonically.
         # this step is to omit noise and other data after s-parameters data.
         c = [1 + cmp(datalar[i, 0], datalar[i + 1, 0]) for i in range(nop - 1)]
 
         try:
             nop = c.index(1)
-        except:
+        except Exception as e:
             pass
 
         try:
             nop = min(nop, c.index(2))
-        except:
+        except Exception as e:
             pass
 
         self.freqs = datalar[:, 0] * fcoef[self.file_freq_unit]
         data = np.zeros((nop, ps**2), dtype=np.complex128)
 
         if self.file_data_format == "RI":
             for i in range(ps**2):
@@ -1404,27 +1557,27 @@
                 Sm = np.matrix(sdata[i, :]).reshape(ps, ps)
                 try:
                     if self.smatrix_type == 1:
                         Ym = F.I * (Sm * G + G.conj()).I * (I0 - Sm) * F
                     else:
                         Ym = F.I * (Sm * G + G).I * (I0 - Sm) * F
                     self.ydata[i, :] = Ym.reshape(ps**2)
-                except:
+                except Exception as e:
                     print(f"Y-Matrix is undefined at frequency: {self.freqs[i]: f}\n")
                     self.undefinedYindices.add(i)
                     break
                 try:
                     if self.smatrix_type == 1:
                         Zm = F.I * (I0 - Sm).I * (Sm * G + G.conj()) * F
                         # Zm=(G+G.conj()).I*F.I*(G*Sm+G.conj())*(I0-Sm).I*F*(G+G.conj())
                         # gives the same result
                     else:
                         Zm = F.I * (I0 - Sm).I * (Sm * G + G) * F
                     self.zdata[i, :] = Zm.reshape(ps**2)
-                except:
+                except Exception as e:
                     print(f"Z-Matrix is undefined at frequency: {self.freqs[i]: f}\n")
                     self.undefinedZindices.add(i)
                     break
 
         elif input == "Z":
             zdata = self.zdata
             if self.ydata is None or self.ydata.shape != (ns, ps**2):
@@ -1434,15 +1587,15 @@
             for i in indices:
                 G = np.matrix(np.diag(impT[:][i]))
                 F = self.Ffunc(impT[:][i])
                 Zm = np.matrix(zdata[i, :]).reshape(ps, ps)
                 try:
                     Ym = Zm.I
                     self.ydata[i, :] = Ym.reshape(ps**2)
-                except:
+                except Exception as e:
                     print(f"Y-Matrix is undefined at frequency: {self.freqs[i]: f}\n")
                     self.undefinedYindices.add(i)
                 if self.smatrix_type == 1:
                     Sm = F * (Zm - G.conj()) * (Zm + G).I * F.I
                 else:
                     Sm = F * (Zm - G) * (Zm + G).I * F.I
                 self.sdata[i, :] = Sm.reshape(ps**2)
@@ -1456,15 +1609,15 @@
             for i in indices:
                 G = np.matrix(np.diag(impT[:][i]))
                 F = self.Ffunc(impT[:][i])
                 Ym = np.matrix(ydata[i, :]).reshape(ps, ps)
                 try:
                     Zm = Ym.I
                     self.zdata[i, :] = Zm.reshape(ps**2)
-                except:
+                except Exception as e:
                     print(f"Z-Matrix is undefined at frequency: {self.freqs[i]: f}\n")
                     self.undefinedZindices.add(i)
                 if self.smatrix_type == 1:
                     Sm = F * (I0 - G.H * Ym) * (I0 + G * Ym).I * F.I
                 else:
                     Sm = F * (I0 - G * Ym) * (I0 + G * Ym).I * F.I
                 self.sdata[i, :] = Sm.reshape(ps**2)
@@ -2531,15 +2684,15 @@
                     try:
                         import nlopt
                         opt = nlopt.opt(nlopt.GN_ESCH, len(2 * t))
                         opt.add_inequality_constraint(constraint1)
                         # opt.set_maxeval(1000)
                         # opt.set_maxtime(5)
                         x = opt.optimize(xvar)
-                    except:
+                    except Exception as e:
                         print("Error at root finding with NLOPT")
 
                 for y in range(t):
                     perturbation[(y / ps),
                                  y % ps] = x[2 * y] + x[2 * y + 1] * 1.0j
                 smatrix = smatrix + perturbation
                 #tempmatrix=np.matrix(np.eye(ps).astype(complex))-smatrix.H*smatrix
@@ -3445,15 +3598,15 @@
             obj.inplace = 1
         else:
             obj = self
         if not fstart:
             fstart = obj.freqs[0] * 0.999999
         if not fstop:
             fstop = obj.freqs[-1] * 1.000001
-        temp = [x > fstart and x < fstop for x in obj.freqs]
+        temp = [x > fstart * 0.99999 and x < fstop * 1.00001 for x in obj.freqs]
         index_begin = temp.index(True)
         try:
             index_end = temp.index(False, index_begin)
         except ValueError:
             index_end = -1
         obj.freqs = obj.freqs[index_begin:index_end]
         if isinstance(obj.refimpedance, (list, np.ndarray)):
```

### Comparing `mwtoolbox-0.0.7/src/mwtoolbox/transmission_lines.py` & `mwtoolbox-0.0.8/src/mwtoolbox/transmission_lines.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.7/src/mwtoolbox.egg-info/PKG-INFO` & `mwtoolbox-0.0.8/src/mwtoolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwtoolbox
-Version: 0.0.7
+Version: 0.0.8
 Summary: Microwave Toolbox
 Author-email: Tuncay Erdöl <terdol@hotmail.com>
 License: MIT
 Keywords: microwave,rf,s-parameters
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mwtoolbox-0.0.7/src/mwtoolbox.egg-info/SOURCES.txt` & `mwtoolbox-0.0.8/src/mwtoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.7/tests/test1.py` & `mwtoolbox-0.0.8/tests/test1.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.7/tests/tests.py` & `mwtoolbox-0.0.8/tests/tests.py`

 * *Files identical despite different names*

### Comparing `mwtoolbox-0.0.7/tests/tests4.py` & `mwtoolbox-0.0.8/tests/tests4.py`

 * *Files identical despite different names*

