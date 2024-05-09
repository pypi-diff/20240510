# Comparing `tmp/protein_design_tools-0.1.7.tar.gz` & `tmp/protein_design_tools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protein_design_tools-0.1.7.tar", last modified: Thu May  9 20:59:58 2024, max compression
+gzip compressed data, was "protein_design_tools-0.1.8.tar", last modified: Thu May  9 21:07:46 2024, max compression
```

## Comparing `protein_design_tools-0.1.7.tar` & `protein_design_tools-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 20:59:58.207535 protein_design_tools-0.1.7/
--rw-rw-r--   0 schaubaj (755442540) 1360859114     1069 2024-05-07 21:38:28.000000 protein_design_tools-0.1.7/LICENSE
--rw-r--r--   0 schaubaj (755442540) 1360859114     1304 2024-05-09 20:59:58.203051 protein_design_tools-0.1.7/PKG-INFO
--rw-rw-r--   0 schaubaj (755442540) 1360859114      695 2024-05-07 22:40:55.000000 protein_design_tools-0.1.7/README.md
-drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 20:59:58.190371 protein_design_tools-0.1.7/protein_design_tools/
--rw-rw-r--   0 schaubaj (755442540) 1360859114        0 2024-05-09 20:51:26.000000 protein_design_tools-0.1.7/protein_design_tools/__init__.py
--rw-r--r--   0 schaubaj (755442540) 1360859114     7078 2024-05-09 20:00:56.000000 protein_design_tools-0.1.7/protein_design_tools/protein_structure.py
--rw-r--r--   0 schaubaj (755442540) 1360859114    18862 2024-05-09 20:59:17.000000 protein_design_tools-0.1.7/protein_design_tools/protein_structure_utils.py
--rw-r--r--   0 schaubaj (755442540) 1360859114     1856 2024-05-07 22:03:29.000000 protein_design_tools-0.1.7/protein_design_tools/test.py
-drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 20:59:58.199602 protein_design_tools-0.1.7/protein_design_tools.egg-info/
--rw-r--r--   0 schaubaj (755442540) 1360859114     1304 2024-05-09 20:59:58.000000 protein_design_tools-0.1.7/protein_design_tools.egg-info/PKG-INFO
--rw-rw-r--   0 schaubaj (755442540) 1360859114      435 2024-05-09 20:59:58.000000 protein_design_tools-0.1.7/protein_design_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 schaubaj (755442540) 1360859114        1 2024-05-09 20:59:58.000000 protein_design_tools-0.1.7/protein_design_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 schaubaj (755442540) 1360859114        6 2024-05-09 20:59:58.000000 protein_design_tools-0.1.7/protein_design_tools.egg-info/requires.txt
--rw-rw-r--   0 schaubaj (755442540) 1360859114       21 2024-05-09 20:59:58.000000 protein_design_tools-0.1.7/protein_design_tools.egg-info/top_level.txt
--rw-rw-r--   0 schaubaj (755442540) 1360859114       38 2024-05-09 20:59:58.207675 protein_design_tools-0.1.7/setup.cfg
--rw-rw-r--   0 schaubaj (755442540) 1360859114      899 2024-05-09 20:59:35.000000 protein_design_tools-0.1.7/setup.py
-drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 20:59:58.196978 protein_design_tools-0.1.7/tests/
--rw-r--r--   0 schaubaj (755442540) 1360859114     1318 2024-05-07 19:58:11.000000 protein_design_tools-0.1.7/tests/test_protein_structure_utils.py
+drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 21:07:46.514261 protein_design_tools-0.1.8/
+-rw-rw-r--   0 schaubaj (755442540) 1360859114     1069 2024-05-07 21:38:28.000000 protein_design_tools-0.1.8/LICENSE
+-rw-r--r--   0 schaubaj (755442540) 1360859114     1304 2024-05-09 21:07:46.513208 protein_design_tools-0.1.8/PKG-INFO
+-rw-rw-r--   0 schaubaj (755442540) 1360859114      695 2024-05-07 22:40:55.000000 protein_design_tools-0.1.8/README.md
+drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 21:07:46.496703 protein_design_tools-0.1.8/protein_design_tools/
+-rw-rw-r--   0 schaubaj (755442540) 1360859114        0 2024-05-09 20:51:26.000000 protein_design_tools-0.1.8/protein_design_tools/__init__.py
+-rw-r--r--   0 schaubaj (755442540) 1360859114     7083 2024-05-09 21:07:08.000000 protein_design_tools-0.1.8/protein_design_tools/protein_structure.py
+-rw-r--r--   0 schaubaj (755442540) 1360859114    18866 2024-05-09 21:06:44.000000 protein_design_tools-0.1.8/protein_design_tools/protein_structure_utils.py
+-rw-r--r--   0 schaubaj (755442540) 1360859114     1856 2024-05-07 22:03:29.000000 protein_design_tools-0.1.8/protein_design_tools/test.py
+drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 21:07:46.512150 protein_design_tools-0.1.8/protein_design_tools.egg-info/
+-rw-r--r--   0 schaubaj (755442540) 1360859114     1304 2024-05-09 21:07:46.000000 protein_design_tools-0.1.8/protein_design_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 schaubaj (755442540) 1360859114      435 2024-05-09 21:07:46.000000 protein_design_tools-0.1.8/protein_design_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 schaubaj (755442540) 1360859114        1 2024-05-09 21:07:46.000000 protein_design_tools-0.1.8/protein_design_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 schaubaj (755442540) 1360859114        6 2024-05-09 21:07:46.000000 protein_design_tools-0.1.8/protein_design_tools.egg-info/requires.txt
+-rw-rw-r--   0 schaubaj (755442540) 1360859114       21 2024-05-09 21:07:46.000000 protein_design_tools-0.1.8/protein_design_tools.egg-info/top_level.txt
+-rw-rw-r--   0 schaubaj (755442540) 1360859114       38 2024-05-09 21:07:46.514327 protein_design_tools-0.1.8/setup.cfg
+-rw-rw-r--   0 schaubaj (755442540) 1360859114      899 2024-05-09 21:07:28.000000 protein_design_tools-0.1.8/setup.py
+drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 21:07:46.506117 protein_design_tools-0.1.8/tests/
+-rw-r--r--   0 schaubaj (755442540) 1360859114     1318 2024-05-07 19:58:11.000000 protein_design_tools-0.1.8/tests/test_protein_structure_utils.py
```

### Comparing `protein_design_tools-0.1.7/LICENSE` & `protein_design_tools-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `protein_design_tools-0.1.7/PKG-INFO` & `protein_design_tools-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-design-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library of tools for protein design.
 Home-page: https://github.com/drewschaub/protein-design-tools
 Author: Andrew Schaub
 Author-email: andrew.schaub@protonmail.com
 License:  MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `protein_design_tools-0.1.7/README.md` & `protein_design_tools-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `protein_design_tools-0.1.7/protein_design_tools/protein_structure.py` & `protein_design_tools-0.1.8/protein_design_tools/protein_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                         charge = line[78:80].strip()
                         atom = next((a for a in residue.atoms if a.atom_id == atom_id), None)
                         if atom is None:
                             # Create an Atom object and append it to self.atoms
                             atom = self.Chain.Residue.Atom(atom_id, atom_name, alt_loc, x, y, z, occupancy, temp_factor, segment_id, element, charge)
                             residue.atoms.append(atom)
 
-    def get_sequence(self):
+    def get_sequence_dict(self):
         """
         Return the sequence of the protein structure as a dictionary of chains and sequences.
 
         Returns:
         dict: A dictionary of chains and sequences. The keys are the chain names and the values are the sequences.
 
         """
```

### Comparing `protein_design_tools-0.1.7/protein_design_tools/protein_structure_utils.py` & `protein_design_tools-0.1.8/protein_design_tools/protein_structure_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,14 @@
 
 def get_radgy_ratio(structure, atom_type="backbone", chains=None, residue_numbers=None, residue_indices=None, residue_ids=None):
 
     # Get the radius of gyration
     structure_radius_of_gyration = get_radgy(structure, atom_type=atom_type, chains=chains, residue_numbers=residue_numbers, residue_indices=residue_indices, residue_ids=residue_ids)
 
     # Get the radius of gyration of an ideal alanine helix of the same length. structure.get_sequences will return the sequendes of each chain of the protein, so these need to be summed
-    structure_seq_len = sum([len(sequence) for sequence in structure.get_sequences()])
+    structure_seq_len = sum([len(sequence) for sequence in structure.get_sequence_dict()])
     alanine_radius_of_gyration = get_radgy_alanine_helix(structure_seq_len, atom_type=atom_type)
 
     # Calculate the radius of gyration ratio
     radius_of_gyration_ratio = structure_radius_of_gyration / alanine_radius_of_gyration
 
     return radius_of_gyration_ratio
```

### Comparing `protein_design_tools-0.1.7/protein_design_tools/test.py` & `protein_design_tools-0.1.8/protein_design_tools/test.py`

 * *Files identical despite different names*

### Comparing `protein_design_tools-0.1.7/protein_design_tools.egg-info/PKG-INFO` & `protein_design_tools-0.1.8/protein_design_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-design-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library of tools for protein design.
 Home-page: https://github.com/drewschaub/protein-design-tools
 Author: Andrew Schaub
 Author-email: andrew.schaub@protonmail.com
 License:  MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `protein_design_tools-0.1.7/setup.py` & `protein_design_tools-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='protein-design-tools',
-    version='0.1.7',
+    version='0.1.8',
     author='Andrew Schaub',
     author_email='andrew.schaub@protonmail.com',
     description='A library of tools for protein design.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/drewschaub/protein-design-tools',
     license=' MIT License',
```

### Comparing `protein_design_tools-0.1.7/tests/test_protein_structure_utils.py` & `protein_design_tools-0.1.8/tests/test_protein_structure_utils.py`

 * *Files identical despite different names*

