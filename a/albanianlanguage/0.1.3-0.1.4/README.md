# Comparing `tmp/albanianlanguage-0.1.3.tar.gz` & `tmp/albanianlanguage-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albanianlanguage-0.1.3.tar", last modified: Mon Apr 29 21:09:08 2024, max compression
+gzip compressed data, was "albanianlanguage-0.1.4.tar", last modified: Fri May 10 14:40:01 2024, max compression
```

## Comparing `albanianlanguage-0.1.3.tar` & `albanianlanguage-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 21:09:08.665553 albanianlanguage-0.1.3/
--rw-r--r--   0 flori      (501) staff       (20)     1075 2024-04-29 20:36:09.000000 albanianlanguage-0.1.3/LICENSE.md
--rw-r--r--   0 flori      (501) staff       (20)     2423 2024-04-29 21:09:08.664939 albanianlanguage-0.1.3/PKG-INFO
--rw-r--r--   0 flori      (501) staff       (20)     2009 2024-04-29 20:37:10.000000 albanianlanguage-0.1.3/README.md
-drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 21:09:08.660784 albanianlanguage-0.1.3/albanianlanguage/
--rw-r--r--   0 flori      (501) staff       (20)       33 2024-04-29 19:58:25.000000 albanianlanguage-0.1.3/albanianlanguage/__init__.py
--rw-r--r--   0 flori      (501) staff       (20) 12203635 2024-04-29 20:10:19.000000 albanianlanguage-0.1.3/albanianlanguage/words.csv
--rw-r--r--   0 flori      (501) staff       (20)     1894 2024-04-29 21:08:34.000000 albanianlanguage-0.1.3/albanianlanguage/words.py
-drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-04-29 21:09:08.664226 albanianlanguage-0.1.3/albanianlanguage.egg-info/
--rw-r--r--   0 flori      (501) staff       (20)     2423 2024-04-29 21:09:08.000000 albanianlanguage-0.1.3/albanianlanguage.egg-info/PKG-INFO
--rw-r--r--   0 flori      (501) staff       (20)      271 2024-04-29 21:09:08.000000 albanianlanguage-0.1.3/albanianlanguage.egg-info/SOURCES.txt
--rw-r--r--   0 flori      (501) staff       (20)        1 2024-04-29 21:09:08.000000 albanianlanguage-0.1.3/albanianlanguage.egg-info/dependency_links.txt
--rw-r--r--   0 flori      (501) staff       (20)       17 2024-04-29 21:09:08.000000 albanianlanguage-0.1.3/albanianlanguage.egg-info/top_level.txt
--rw-r--r--   0 flori      (501) staff       (20)       38 2024-04-29 21:09:08.665616 albanianlanguage-0.1.3/setup.cfg
--rw-r--r--   0 flori      (501) staff       (20)      671 2024-04-29 21:08:41.000000 albanianlanguage-0.1.3/setup.py
+drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-05-10 14:40:01.445077 albanianlanguage-0.1.4/
+-rw-r--r--   0 flori      (501) staff       (20)     3268 2024-05-10 14:40:01.444786 albanianlanguage-0.1.4/PKG-INFO
+-rw-r--r--   0 flori      (501) staff       (20)     2291 2024-04-29 21:23:34.000000 albanianlanguage-0.1.4/README.md
+drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-05-10 14:40:01.439192 albanianlanguage-0.1.4/albanianlanguage/
+-rw-r--r--   0 flori      (501) staff       (20)       32 2024-04-29 21:23:46.000000 albanianlanguage-0.1.4/albanianlanguage/__init__.py
+-rw-r--r--   0 flori      (501) staff       (20) 12203635 2024-04-29 20:10:19.000000 albanianlanguage-0.1.4/albanianlanguage/words.csv
+-rw-r--r--   0 flori      (501) staff       (20)     2057 2024-05-10 14:27:01.000000 albanianlanguage-0.1.4/albanianlanguage/words.py
+drwxr-xr-x   0 flori      (501) staff       (20)        0 2024-05-10 14:40:01.444349 albanianlanguage-0.1.4/albanianlanguage.egg-info/
+-rw-r--r--   0 flori      (501) staff       (20)     3268 2024-05-10 14:40:00.000000 albanianlanguage-0.1.4/albanianlanguage.egg-info/PKG-INFO
+-rw-r--r--   0 flori      (501) staff       (20)      260 2024-05-10 14:40:00.000000 albanianlanguage-0.1.4/albanianlanguage.egg-info/SOURCES.txt
+-rw-r--r--   0 flori      (501) staff       (20)        1 2024-05-10 14:40:00.000000 albanianlanguage-0.1.4/albanianlanguage.egg-info/dependency_links.txt
+-rw-r--r--   0 flori      (501) staff       (20)       17 2024-05-10 14:40:00.000000 albanianlanguage-0.1.4/albanianlanguage.egg-info/top_level.txt
+-rw-r--r--   0 flori      (501) staff       (20)       38 2024-05-10 14:40:01.445214 albanianlanguage-0.1.4/setup.cfg
+-rw-r--r--   0 flori      (501) staff       (20)      675 2024-05-10 14:37:10.000000 albanianlanguage-0.1.4/setup.py
```

### Comparing `albanianlanguage-0.1.3/PKG-INFO` & `albanianlanguage-0.1.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: albanianlanguage
-Version: 0.1.3
-Summary: A package with a few functionalities for albanian language.
-Home-page: http://github.com/florijanqosja/albanianlanguage
-Author: Florijan Qosja
-Author-email: florijanqosja@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # AlbanianLanguage Package
 
 The `AlbanianLanguage` package is a comprehensive toolkit designed for handling various linguistic tasks associated with the Albanian language. It offers functionalities to read words from a CSV file, apply filters based on specific criteria, and optionally include additional details such as word types and definitions.
 
 ## Installation
 
 Install `AlbanianLanguage` directly from PyPI:
@@ -54,14 +42,26 @@
 
 Efficiently read and filter words from a CSV file.
 Optionally retrieve additional linguistic details such as type and definition.
 Designed specifically for applications related to the Albanian language.
 Requirements
 This package requires Python 3.x. No additional libraries are needed for the basic functionality, but make sure to handle dependencies if you expand the package.
 
+## **Pushing to PYPI**
+
+```python
+!pip install setuptools wheel twine # Install the necessary tools:
+
+!python setup.py sdist bdist_wheel # Generate distribution archives:
+
+!rm -rf dist # if there are any previous builds
+
+!twine upload dist/* # Upload the distribution to PyPI:
+```
+
 ## Contributing
 
 Contributions to AlbanianLanguage are warmly welcomed. Please fork the repository, make your changes, and submit a pull request for review.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE.md](LICENSE) file for details.
```

### Comparing `albanianlanguage-0.1.3/README.md` & `albanianlanguage-0.1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,80 @@
-# AlbanianLanguage Package
-
-The `AlbanianLanguage` package is a comprehensive toolkit designed for handling various linguistic tasks associated with the Albanian language. It offers functionalities to read words from a CSV file, apply filters based on specific criteria, and optionally include additional details such as word types and definitions.
-
-## Installation
-
-Install `AlbanianLanguage` directly from PyPI:
-
-```bash
-pip install albanianlanguage
-```
-
-## Usage
-
-To use the AlbanianLanguage package, import and call its main functions:
-
-```
-from albanianlanguage import get_all_words
-
-# Get all words from the specified CSV
-words = get_all_words()
-
-# Get words that start with "ka"
-ex_words = get_all_words(starts_with="ka")
-
-# Get words that include "pse"
-ample_words = get_all_words(includes="pse")
-
-# Get words along with their types and definitions
-detailed_words = get_all_words(return_type=True, return_definition=True)
-```
-
-## Parameters
-
-- filename (str): Path to the CSV file. Defaults to 'albanianlanguage/ff.csv'.
-- starts_with (str, optional): Filter words that start with this substring.
-- includes (str, optional): Filter words that include this substring.
-- return_type (bool, optional): If true, includes the word's type in the output.
-- return_definition (bool, optional): If true, includes the word's definition in the output.
-
-## Features
-
-Efficiently read and filter words from a CSV file.
-Optionally retrieve additional linguistic details such as type and definition.
-Designed specifically for applications related to the Albanian language.
-Requirements
-This package requires Python 3.x. No additional libraries are needed for the basic functionality, but make sure to handle dependencies if you expand the package.
-
-## Contributing
-
-Contributions to AlbanianLanguage are warmly welcomed. Please fork the repository, make your changes, and submit a pull request for review.
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE.md](LICENSE) file for details.
+Metadata-Version: 2.1
+Name: albanianlanguage
+Version: 0.1.4
+Summary: A package with a few functionalities for the albanian language.
+Home-page: http://github.com/florijanqosja/albanianlanguage
+Author: Florijan Qosja
+Author-email: florijanqosja@gmail.com
+License: UNKNOWN
+Description: # AlbanianLanguage Package
+        
+        The `AlbanianLanguage` package is a comprehensive toolkit designed for handling various linguistic tasks associated with the Albanian language. It offers functionalities to read words from a CSV file, apply filters based on specific criteria, and optionally include additional details such as word types and definitions.
+        
+        ## Installation
+        
+        Install `AlbanianLanguage` directly from PyPI:
+        
+        ```bash
+        pip install albanianlanguage
+        ```
+        
+        ## Usage
+        
+        To use the AlbanianLanguage package, import and call its main functions:
+        
+        ```
+        from albanianlanguage import get_all_words
+        
+        # Get all words from the specified CSV
+        words = get_all_words()
+        
+        # Get words that start with "ka"
+        ex_words = get_all_words(starts_with="ka")
+        
+        # Get words that include "pse"
+        ample_words = get_all_words(includes="pse")
+        
+        # Get words along with their types and definitions
+        detailed_words = get_all_words(return_type=True, return_definition=True)
+        ```
+        
+        ## Parameters
+        
+        - filename (str): Path to the CSV file. Defaults to 'albanianlanguage/ff.csv'.
+        - starts_with (str, optional): Filter words that start with this substring.
+        - includes (str, optional): Filter words that include this substring.
+        - return_type (bool, optional): If true, includes the word's type in the output.
+        - return_definition (bool, optional): If true, includes the word's definition in the output.
+        
+        ## Features
+        
+        Efficiently read and filter words from a CSV file.
+        Optionally retrieve additional linguistic details such as type and definition.
+        Designed specifically for applications related to the Albanian language.
+        Requirements
+        This package requires Python 3.x. No additional libraries are needed for the basic functionality, but make sure to handle dependencies if you expand the package.
+        
+        ## **Pushing to PYPI**
+        
+        ```python
+        !pip install setuptools wheel twine # Install the necessary tools:
+        
+        !python setup.py sdist bdist_wheel # Generate distribution archives:
+        
+        !rm -rf dist # if there are any previous builds
+        
+        !twine upload dist/* # Upload the distribution to PyPI:
+        ```
+        
+        ## Contributing
+        
+        Contributions to AlbanianLanguage are warmly welcomed. Please fork the repository, make your changes, and submit a pull request for review.
+        
+        ## License
+        
+        This project is licensed under the MIT License - see the [LICENSE.md](LICENSE) file for details.
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
```

### Comparing `albanianlanguage-0.1.3/albanianlanguage/words.csv` & `albanianlanguage-0.1.4/albanianlanguage/words.csv`

 * *Files identical despite different names*

### Comparing `albanianlanguage-0.1.3/albanianlanguage/words.py` & `albanianlanguage-0.1.4/albanianlanguage/words.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import csv
 import ast
 import pkg_resources
 
-
 def get_all_words(starts_with=None, includes=None, return_type=False, return_definition=False):
     """
     Reads words and their details from a CSV file and optionally filters them based on provided criteria. 
     Can also format the output to include word types and definitions.
     
     Parameters:
     filename (str): The path to the CSV file containing the words. Default is 'wordtype/ff.csv'.
@@ -15,27 +14,33 @@
     return_type (bool, optional): If True, includes the word type in the return data.
     return_definition (bool, optional): If True, includes the word definition in the return data.
     
     Returns:
     list: Depending on the parameters, returns either a list of words or a list of dictionaries with word details.
     """
     words = []
+    seen_words = set()
     filename = pkg_resources.resource_filename('albanianlanguage', 'words.csv')
 
     with open(filename, newline='') as csvfile:
         reader = csv.DictReader(csvfile)
         for row in reader:
             word = row['word']
-            # Check if the word meets the 'starts_with' or 'includes' condition
             if (starts_with and not word.startswith(starts_with)) or (includes and includes not in word):
                 continue
             
             if return_type or return_definition:
-                word_details = {'word': word}
-                if return_type and 'type' in row:
-                    word_details['type'] = row['type']
-                if return_definition and 'definition' in row:
-                    word_details['definition'] = ast.literal_eval(row['definition'])
-                words.append(word_details)
+                if word not in seen_words:
+                    word_details = {'word': word}
+                    if return_type and 'type' in row:
+                        
+                        word_details['type'] = row['type']
+                    if return_definition and 'definition' in row:
+                        word_details['definition'] = ast.literal_eval(row['definition'])
+                    words.append(word_details)
+                    seen_words.add(word)
             else:
-                words.append(word)
-    return words
+                if word not in seen_words:
+                    words.append(word)
+                    seen_words.add(word)
+
+    return words
```

### Comparing `albanianlanguage-0.1.3/setup.py` & `albanianlanguage-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='albanianlanguage',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         # none so fas
     ],
     author='Florijan Qosja',
     package_data={'albanianlanguage': ['words.csv']},
     author_email='florijanqosja@gmail.com',
-    description='A package with a few functionalities for albanian language.',
+    description='A package with a few functionalities for the albanian language.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='http://github.com/florijanqosja/albanianlanguage',
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
     ],
```

