# Comparing `tmp/mimllearning-0.3.7.tar.gz` & `tmp/mimllearning-0.3.8.tar.gz`

## Comparing `mimllearning-0.3.7.tar` & `mimllearning-0.3.8.tar`

### file list

```diff
@@ -1,46 +1,45 @@
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.7/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.3.7/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/data/__init__.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/data/arff_to_csv.py
--rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/data/bag.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/data/instance.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/data/load_datasets.py
--rw-r--r--   0        0        0    15879 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/datasets/toy.csv
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/report/__init__.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/report/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/tutorial/demo.ipynb
--rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/tutorial/miml_data.ipynb
--rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/tutorial/miml_transformations.ipynb
--rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/tutorial/mimltoml_classifiers.ipynb
--rw-r--r--   0        0        0    16340 2020-02-02 00:00:00.000000 mimllearning-0.3.7/src/miml/tutorial/new_demo.ipynb
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.3.7/.gitignore
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.7/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.8/readme.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.3.8/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/data/arff_to_csv.py
+-rw-r--r--   0        0        0     9571 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/data/instance.py
+-rw-r--r--   0        0        0    18252 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/datasets/__init__.py
+-rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/datasets/dataset_utils.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     7750 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/report/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0    16340 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/tutorial/demo.ipynb
+-rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/tutorial/miml_data.ipynb
+-rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/tutorial/miml_transformations.ipynb
+-rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.3.8/src/miml/tutorial/mimltoml_classifiers.ipynb
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.3.8/.gitignore
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.8/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.3.8/PKG-INFO
```

### Comparing `mimllearning-0.3.7/readme.md` & `mimllearning-0.3.8/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.3.8/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/classifier/miml_classifier.py` & `mimllearning-0.3.8/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.3.8/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/classifier/mi/apr_classifier.py` & `mimllearning-0.3.8/src/miml/classifier/mi/apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.3.8/src/miml/classifier/mi/miles_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.3.8/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.3.8/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.3.8/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/data/bag.py` & `mimllearning-0.3.8/src/miml/data/bag.py`

 * *Files 6% similar despite different names*

```diff
@@ -285,18 +285,32 @@
         Parameters
         ----------
         dataset : MIMLDataset
             Dataset for the bag
         """
         self.dataset = dataset
 
-    def show_bag(self) -> None:
+    def show_bag(self, mode="table") -> None:
         """
         Show bag info in table format
+
+        Parameters
+        ----------
+        mode : str
+            Mode to show the bag. Modes available are "table" and "compact" (csv format)
         """
-        if self.dataset is None:
-            table = [[self.key] + [""] * self.get_number_attributes()]
+        header = [self.key] + [""] * self.get_number_attributes()
+        if self.dataset is not None:
+            header = [self.key] + self.get_features_name() + self.get_labels_name()
+        if mode == "table":
+            table = [header]
+            for index_instance in range(self.get_number_instances()):
+                table.append([index_instance] + list(self.get_instance(index_instance).get_attributes()))
+            print(tabulate(table, headers='firstrow', tablefmt="grid", numalign="center"))
+
+        elif mode == "compact":
+            print(", ".join(header))
+            for index_instance in range(self.get_number_instances()):
+                print(", ".join([self.key] + list(self.get_instance(index_instance).get_attributes())))
+
         else:
-            table = [[self.key] + self.get_features_name() + self.get_labels_name()]
-        for index_instance in range(self.get_number_instances()):
-            table.append([index_instance] + list(self.get_instance(index_instance).get_attributes()))
-        print(tabulate(table, headers='firstrow', tablefmt="grid", numalign="center"))
+            raise Exception("Mode not available. Mode options are \"table\" and \"compact\"")
```

### Comparing `mimllearning-0.3.7/src/miml/data/instance.py` & `mimllearning-0.3.8/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/data/miml_dataset.py` & `mimllearning-0.3.8/src/miml/data/miml_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import random
+
 import numpy as np
 
 from .bag import Bag
 from .instance import Instance
 
 
 class MIMLDataset:
@@ -207,29 +209,33 @@
         Returns
         ----------
         numbers of labels: int
             Numbers of labels of the dataset
         """
         return len(self.get_labels_name())
 
-    def get_bag(self, key_bag: str) -> Bag:
+    def get_bag(self, bag) -> Bag:
         """
         Get data of a bag of the dataset
 
         Parameters
         ----------
-        key_bag: str
-            Key of the bag to be obtained
+        bag: int/str
+            Index or key of the bag to be obtained
 
         Returns
         ----------
         bag: Bag
             Instance of Bag class
         """
-        return self.data[key_bag]
+        if isinstance(bag, int):
+            return list(self.data.values())[bag]
+        elif isinstance(bag, str):
+            return self.data[bag]
+        raise Exception("The bag can be obtained using an index (int) or his key (str)")
 
     def get_number_bags(self) -> int:
         """
         Get numbers of bags of the dataset
 
         Returns
         ----------
@@ -290,42 +296,46 @@
         Returns
         ----------
         numbers of instances: int
             Numbers of instances of the dataset
         """
         return sum(self.data[bag].get_number_instances() for bag in self.data.keys())
 
-    def add_instance(self, key: str, instance: Instance) -> None:
+    def add_instance(self, bag, instance: Instance) -> None:
         """
         Add an Instance to a Bag of the dataset
 
         Parameters
         ----------
-        key : str
-            Key of the bag where the instance will be added
+        bag : str
+            Index or key of the bag where the instance will be added
 
         instance : Instance
             Instance of Instance class to be added
         """
         #TODO: Test if it works
-        self.get_bag(key).add_instance(instance)
+        bag = self.get_bag(bag)
+        bag.add_instance(instance)
+        self.data[bag] = bag
 
-    def delete_instance(self, key_bag: str, index_instance: int) -> None:
+    def delete_instance(self, bag, index_instance: int) -> None:
         """
         Delete an instance of a bag of the dataset
 
         Parameters
         ----------
-        key_bag : str
-            Key of the bag which contains the instance to be deleted
+        bag : int/str
+            Index or key of the bag which contains the instance to be deleted
 
         index_instance : int
             Index of the instance to be deleted
         """
-        self.get_bag(key_bag).delete_instance(index_instance)
+        bag = self.get_bag(bag)
+        bag.delete_instance(index_instance)
+        self.data[bag] = bag
 
     def get_attribute(self, bag, instance, attribute) -> float:
         """
         Get value of an attribute of the bag
 
         Parameters
         ----------
@@ -341,47 +351,49 @@
         Returns
         -------
         value : float
             Value of the attribute
         """
         return self.get_instance(bag, instance).get_attribute(attribute)
 
-    def set_attribute(self, key_bag: str, index_instance: int, attribute, value: float) -> None:
+    def set_attribute(self, bag, index_instance: int, attribute, value: float) -> None:
         """
         Update value from attributes
 
-            Parameters
-            ----------
-            key_bag : str
-                Bag key of the dataset
-
-            index_instance : int
-                Index of the instance
-
-            attribute: int/str
-                Attribute of the dataset
-
-            value: float
-                New value for the update
-            """
-        self.get_instance(key_bag, index_instance).set_attribute(attribute, value)
+        Parameters
+        ----------
+        bag : int/str
+            Index or key of the bag of the dataset
+
+        index_instance : int
+            Index of the instance
+
+        attribute: int/str
+            Attribute of the dataset
+
+        value: float
+            New value for the update
+        """
+        bag = self.get_bag(bag)
+        bag.set_attribute(index_instance, attribute, value)
+        self.data[bag] = bag
 
     def add_attribute(self, position: int, values=None) -> None:
         """
         Add attribute to the dataset
 
         Parameters
         ----------
         position : int
             Index for the new attribute
 
         values:  ndarray of shape(n_instances)
             Values for the new attribute
         """
-        # TODO: Test
+        # TODO: Arreglar
         for bag_index, bag in enumerate(self.data.keys()):
             add_values = values[bag_index]
             if values is None:
                 add_values = np.zeros(self.data[bag].get_number_instances())
             self.data[bag].add_attribute(position, add_values)
 
     def delete_attribute(self, position: int) -> None:
@@ -392,16 +404,17 @@
         Parameters
         ----------
         position : int
             Index of the attribute to be deleted
         """
         for bag in self.data.keys():
             self.data[bag].data = np.delete(self.data[bag].data, position, axis=1)
+        self.attributes.pop(list(self.attributes)[position])
 
-    def show_dataset(self, head: int = None, attributes=None, labels=None, info=True) -> None:
+    def show_dataset(self, mode: str="table", head: int = None, attributes=None, labels=None, info=True) -> None:
         """
         Function to show information about the dataset
 
         Parameters
         ----------
             head : int
                 Number of the nth firsts bag to show
@@ -418,26 +431,74 @@
         # TODO: Hacer algo como head y tail de pandas, ponerlo como parametro quizas, tambien lista atributos y labels
         #  a mostrar opcionales
         if info:
             print("Name: ", self.get_name())
             print("Features: ", self.get_features_name())
             print("Labels: ", self.get_labels_name())
             print("Bags:")
-        count = 0
-        for key in self.data:
-            # print("\n")
-            bag = self.get_bag(key)
-            # print("Key: ", key_bag)
-            # print("Attributes: ", bag[0])
-            # print("Labels: ", bag[1])
-            bag.show_bag()
-            count += 1
-            if head is not None:
-                if count >= head:
-                    break
+
+        if mode == "table":
+            for bag_index in range(self.get_number_bags()):
+                bag = self.get_bag(bag_index)
+                bag.show_bag()
+                if head is not None:
+                    if bag_index+1 >= head:
+                        break
+
+        elif mode == "compact":
+            header = [self.name] + self.get_features_name() + self.get_labels_name()
+            print(", ".join(header))
+            for bag_index in range(self.get_number_bags()):
+                bag = self.get_bag(bag_index)
+                for index_instance in range(bag.get_number_instances()):
+                    print(", ".join([bag.key] + list(bag.get_instance(index_instance).get_attributes())))
+
+                if head is not None:
+                    if bag_index+1 >= head:
+                        break
+
+        else:
+            raise Exception("Mode not available. Mode options are \"table\" and \"compact\"")
+
+    def split_dataset(self, train_percentage: float=0.8, seed=0):
+        for count_label in np.sum(self.get_features_by_bag(), 1):
+            print(count_label)
+            if count_label == 0:
+                raise Exception("Dataset contain a label with no positive instance for a label")
+
+        random.seed(seed)
+        labels_train = [range(self.get_number_labels())]
+        bags_not_used = [range(self.get_number_bags())]
+
+        dataset_train = MIMLDataset()
+        dataset_train.set_name(self.get_name()+"_train")
+        dataset_train.set_features_name(self.get_features_name())
+        dataset_train.set_labels_name(self.get_labels_name())
+
+        dataset_test = MIMLDataset()
+        dataset_test.set_name(self.get_name() + "_test")
+        dataset_test.set_features_name(self.get_features_name())
+        dataset_test.set_labels_name(self.get_labels_name())
+
+        while bags_not_used and labels_train:
+            bag_index = random.randint(0, len(bags_not_used)-1)
+            bag = self.get_bag(bags_not_used[bag_index])
+            used = False
+
+            for label_index in range(len(bag.get_labels())):
+                if bag.get_labels()[label_index] == 1 and label_index in labels_train:
+                    used = True
+                    del labels_train[label_index]
+            if used:
+                del bags_not_used[bag_index]
+
+
+
+
+
 
     # TODO: Ver si separar esto
     def cardinality(self):
         """
         Computes the Cardinality as the average number of labels per pattern.
 
         Returns
@@ -511,23 +572,22 @@
 
     def describe(self):
         """
         Print statistics about the dataset
         """
 
         print("-----MULTILABEL-----")
-        print("Cardinalidad: ", self.cardinality())
-        print("Densidad: ", self.density())
+        print("Cardinality: ", self.cardinality())
+        print("Density: ", self.density())
         print("Distinct: ", self.distinct())
         print("")
         n_instances, min_instances, max_instances, distribution = self.get_statistics()
         print("-----MULTIINSTANCE-----")
         print("Nº of bags: ", self.get_number_bags())
         print("Total instances: ", n_instances)
         print("Average Instances per bag: ", n_instances / self.get_number_bags())
         print("Min Instances per bag: ", min_instances)
         print("Max Instances per bag: ", max_instances)
         print("Attributes per bag: ", self.get_number_attributes())
-        # TODO: Implementarlo
         print("\nDistribution of bags:")
-        for number_instances_in_bag, occurrences in distribution.items():
+        for number_instances_in_bag, occurrences in sorted(distribution.items()):
             print("\tBags with ", number_instances_in_bag, " instances: ", occurrences)
```

### Comparing `mimllearning-0.3.7/src/miml/datasets/miml_birds.arff` & `mimllearning-0.3.8/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/datasets/miml_birds.csv` & `mimllearning-0.3.8/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.3.8/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.3.8/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/report/report.py` & `mimllearning-0.3.8/src/miml/report/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+import numpy as np
 from sklearn.metrics import hamming_loss, accuracy_score, fbeta_score, jaccard_score, log_loss, \
     roc_auc_score, f1_score, precision_score, recall_score, average_precision_score
 from ..classifier import MIMLClassifier
 from ..data import MIMLDataset
 
 
 class Report:
@@ -16,21 +17,21 @@
         self.dataset = dataset_test
         self.y_true = dataset_test.get_labels_by_bag()
         self.y_pred = classifier.evaluate(dataset_test)
         self.probs = classifier.predict_proba(dataset_test)
 
         all_metrics = ["precision-score-macro", "precision-score-micro", "average-precision-score-macro",
                        "average-precision-score-micro", "recall-score-macro", "recall-score-micro", "f1-score-macro",
-                       "f1-score-micro", "fbeta-score-macro", "fbeta-score-micro", "accuracy-score", "hamming-loss",
-                       "jaccard-score-macro", "jaccard-score-micro", "log-loss"]
+                       "f1-score-micro", "fbeta-score-macro", "fbeta-score-micro", "subset-accuracy-score",
+                       "hamming-loss", "jaccard-score-macro", "jaccard-score-micro", "log-loss"]
         if per_label:
             per_label_metrics = ["precision-score", "recall-score", "f1-score", "fbeta-score", "jaccard-score"]
             for metric in per_label_metrics:
                 for label in dataset_test.get_labels_name():
-                    all_metrics.append(metric+"-"+label)
+                    all_metrics.append(metric + "-" + label)
 
         if metrics is None:
             metrics = all_metrics
         else:
             for metric in metrics:
                 if metric not in all_metrics:
                     raise Exception("Metric ", metric, "is not valid\n", "Metrics availables: ", all_metrics)
@@ -61,15 +62,16 @@
         self.metrics_value["fbeta-score-macro"] = fbeta_score(self.y_true, self.y_pred, beta=0.5, average="macro",
                                                               zero_division=0)
         self.metrics_value["fbeta-score-micro"] = fbeta_score(self.y_true, self.y_pred, beta=0.5, average="micro",
                                                               zero_division=0)
         # TODO: ValueError: Only one class present in y_true. ROC AUC score is not defined in that case.
         # self.metrics_value["roc-auc-score-macro"] = roc_auc_score(self.y_true, self.probs, average="macro")
         # self.metrics_value["roc-auc-score-micro"] = roc_auc_score(self.y_true, self.probs, average="micro")
-        self.metrics_value["accuracy-score"] = accuracy_score(self.y_true, self.y_pred)
+        self.metrics_value["subset-accuracy-score"] = accuracy_score(self.y_true, self.y_pred)
+        # self.metrics_value["hamming-score"] = hamming_score(self.y_true, self.y_pred)
         self.metrics_value["hamming-loss"] = hamming_loss(self.y_true, self.y_pred)
         self.metrics_value["jaccard-score-macro"] = jaccard_score(self.y_true, self.y_pred, average="macro",
                                                                   zero_division=0)
         self.metrics_value["jaccard-score-micro"] = jaccard_score(self.y_true, self.y_pred, average="micro",
                                                                   zero_division=0)
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
@@ -78,23 +80,23 @@
             self.metrics_value["log-loss"] = log_loss(self.y_true, self.probs)
 
         if self.per_label:
             precision_score_per_label = list(precision_score(self.y_true, self.y_pred, average=None, zero_division=0))
             recall_score_per_label = list(recall_score(self.y_true, self.y_pred, average=None, zero_division=0))
             f1_score_per_label = list(f1_score(self.y_true, self.y_pred, average=None, zero_division=0))
             fbeta_score_per_label = list(fbeta_score(self.y_true, self.y_pred, beta=0.5, average=None, zero_division=0))
-            #roc_auc_score_per_label = list(roc_auc_score(self.y_true, self.probs, average="None"))
+            # roc_auc_score_per_label = list(roc_auc_score(self.y_true, self.probs, average="None"))
             jaccard_score_per_label = list(jaccard_score(self.y_true, self.y_pred, average=None, zero_division=0))
             for i, label in enumerate(self.dataset.get_labels_name()):
-                self.metrics_value["precision-score-"+label] = precision_score_per_label[i]
-                self.metrics_value["recall-score-"+label] = recall_score_per_label[i]
-                self.metrics_value["f1-score-"+label] = f1_score_per_label[i]
-                self.metrics_value["fbeta-score-"+label] = fbeta_score_per_label[i]
+                self.metrics_value["precision-score-" + label] = precision_score_per_label[i]
+                self.metrics_value["recall-score-" + label] = recall_score_per_label[i]
+                self.metrics_value["f1-score-" + label] = f1_score_per_label[i]
+                self.metrics_value["fbeta-score-" + label] = fbeta_score_per_label[i]
                 # self.metrics_value["roc-auc-score-"+label] = roc_auc_score_per_label[i]
-                self.metrics_value["jaccard-score-"+label] = jaccard_score_per_label[i]
+                self.metrics_value["jaccard-score-" + label] = jaccard_score_per_label[i]
 
     def to_csv(self, path=None):
         self.calculate_metrics()
         header = ""
         if self.header:
             header = ",".join(str(metric) for metric in self.metrics_name)
         values = ",".join(str(self.metrics_value[metric]) for metric in self.metrics_name)
@@ -106,7 +108,15 @@
                 f.write(header)
                 f.write(values)
 
     def to_string(self):
         self.calculate_metrics()
         for metric in self.metrics_name:
             print(metric, ": ", self.metrics_value[metric])
+
+
+def hamming_score(y_true: np.ndarray, y_pred: np.ndarray):
+    numerator = (y_true & y_pred).sum(axis=1)
+    denominator = (y_true | y_pred).sum(axis=1)
+
+    return np.divide(numerator, denominator, out=np.ones_like(numerator, dtype=np.float_),
+                     where=denominator != 0).mean()
```

### Comparing `mimllearning-0.3.7/src/miml/test/data_test.py` & `mimllearning-0.3.8/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.3.8/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.3.8/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.3.8/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.3.8/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/tutorial/miml_data.ipynb` & `mimllearning-0.3.8/src/miml/tutorial/miml_data.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9577083333333334%*

 * *Differences: {"'cells'": "{0: {'execution_count': 3, 'metadata': {'outputId': "*

 * *            "'b1c17b05-cebb-4b53-a0bb-e7500adb3922'}}, 1: {'metadata': {'outputId': "*

 * *            "'78cf00b9-a0d6-48ad-beab-b752e4fc4b9a'}, 'execution_count': 4}, 2: {'metadata': "*

 * *            "{'outputId': '12da0fae-5b6c-4b95-a166-6bb5bf6fc193'}, 'execution_count': 5, "*

 * *            "'outputs': {0: {'text': {insert: [(12, '\\n'), (13, 'Distribution of bags:\\n'), (14, "*

 * *            "'\\tBags with  3  instances:  2\\n')]}}}}, delete: [0]}"}*

```diff
@@ -1,27 +1,18 @@
 {
     "cells": [
         {
-            "cell_type": "markdown",
-            "metadata": {
-                "id": "UwOvUSvR-8Sm"
-            },
-            "source": [
-                "#Installation and requirements of library\n"
-            ]
-        },
-        {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 3,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "L-_qkpnOxj_V",
-                "outputId": "62b3e76d-0212-4bea-ad99-e349b5e09154"
+                "outputId": "b1c17b05-cebb-4b53-a0bb-e7500adb3922"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Number of bags: 2\n",
@@ -43,21 +34,21 @@
                 "print(\"Number of Features:\", dataset.get_number_features())\n",
                 "print(\"Number of Labels:\", dataset.get_number_labels())\n",
                 "print(\"Number of Attributes:\", dataset.get_number_attributes())\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 4,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "c1OvYWW9Eyhw",
-                "outputId": "0d1812a2-baac-41c0-fee6-7ff7e1d2db72"
+                "outputId": "78cf00b9-a0d6-48ad-beab-b752e4fc4b9a"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Bag: bag1\n",
@@ -141,21 +132,21 @@
                 "        for k in range(instance.get_number_attributes()):\n",
                 "            print(\"\\t\\t\\tAttribute\", k, \":\", instance.get_attribute(k))\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 5,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "_bVd_RyLgqlG",
-                "outputId": "73667c1a-ebbf-4f49-9486-fdf82195f857"
+                "outputId": "12da0fae-5b6c-4b95-a166-6bb5bf6fc193"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "-----MULTILABEL-----\n",
@@ -165,15 +156,18 @@
                         "\n",
                         "-----MULTIINSTANCE-----\n",
                         "N\u00ba of bags:  2\n",
                         "Total instances:  6\n",
                         "Average Instances per bag:  3.0\n",
                         "Min Instances per bag:  3\n",
                         "Max Instances per bag:  3\n",
-                        "Attributes per bag:  7\n"
+                        "Attributes per bag:  7\n",
+                        "\n",
+                        "Distribution of bags:\n",
+                        "\tBags with  3  instances:  2\n"
                     ]
                 }
             ],
             "source": [
                 "# Shows dataset metrics\n",
                 "dataset.describe()"
             ]
```

### Comparing `mimllearning-0.3.7/src/miml/tutorial/miml_transformations.ipynb` & `mimllearning-0.3.8/src/miml/tutorial/miml_transformations.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/tutorial/mimltoml_classifiers.ipynb` & `mimllearning-0.3.8/src/miml/tutorial/mimltoml_classifiers.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/src/miml/tutorial/new_demo.ipynb` & `mimllearning-0.3.8/src/miml/tutorial/demo.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/README.md` & `mimllearning-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.7/pyproject.toml` & `mimllearning-0.3.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.3.7"
+version = "0.3.8"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.3.7"
+version = "0.3.8"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.3.7/PKG-INFO` & `mimllearning-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.3.7
+Version: 0.3.8
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

