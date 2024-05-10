# Comparing `tmp/TorchKAN-0.1.0.tar.gz` & `tmp/TorchKAN-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchKAN-0.1.0.tar", last modified: Fri May 10 01:39:44 2024, max compression
+gzip compressed data, was "TorchKAN-0.1.1.tar", last modified: Fri May 10 05:33:03 2024, max compression
```

## Comparing `TorchKAN-0.1.0.tar` & `TorchKAN-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 u7143478 (7143478) users      (100)        0 2024-05-10 01:39:44.970453 TorchKAN-0.1.0/
--rw-r--r--   0 u7143478 (7143478) users      (100)     1083 2024-05-10 01:03:46.000000 TorchKAN-0.1.0/LICENSE.md
--rw-r--r--   0 u7143478 (7143478) users      (100)     3330 2024-05-10 01:39:44.970453 TorchKAN-0.1.0/PKG-INFO
--rw-r--r--   0 u7143478 (7143478) users      (100)     2418 2024-05-10 01:31:12.000000 TorchKAN-0.1.0/README.md
-drwxr-xr-x   0 u7143478 (7143478) users      (100)        0 2024-05-10 01:39:44.970453 TorchKAN-0.1.0/TorchKAN.egg-info/
--rw-r--r--   0 u7143478 (7143478) users      (100)     3330 2024-05-10 01:39:44.000000 TorchKAN-0.1.0/TorchKAN.egg-info/PKG-INFO
--rw-r--r--   0 u7143478 (7143478) users      (100)      188 2024-05-10 01:39:44.000000 TorchKAN-0.1.0/TorchKAN.egg-info/SOURCES.txt
--rw-r--r--   0 u7143478 (7143478) users      (100)        1 2024-05-10 01:39:44.000000 TorchKAN-0.1.0/TorchKAN.egg-info/dependency_links.txt
--rw-r--r--   0 u7143478 (7143478) users      (100)       90 2024-05-10 01:39:44.000000 TorchKAN-0.1.0/TorchKAN.egg-info/requires.txt
--rw-r--r--   0 u7143478 (7143478) users      (100)        1 2024-05-10 01:39:44.000000 TorchKAN-0.1.0/TorchKAN.egg-info/top_level.txt
--rw-r--r--   0 u7143478 (7143478) users      (100)       38 2024-05-10 01:39:44.970453 TorchKAN-0.1.0/setup.cfg
--rw-r--r--   0 u7143478 (7143478) users      (100)     1133 2024-05-10 01:39:15.000000 TorchKAN-0.1.0/setup.py
+drwxr-xr-x   0 u7143478 (7143478) users      (100)        0 2024-05-10 05:33:03.472648 TorchKAN-0.1.1/
+-rw-r--r--   0 u7143478 (7143478) users      (100)     1083 2024-05-10 01:03:46.000000 TorchKAN-0.1.1/LICENSE.md
+-rw-r--r--   0 u7143478 (7143478) users      (100)     3828 2024-05-10 05:33:03.472648 TorchKAN-0.1.1/PKG-INFO
+-rw-r--r--   0 u7143478 (7143478) users      (100)     3022 2024-05-10 05:25:58.000000 TorchKAN-0.1.1/README.md
+drwxr-xr-x   0 u7143478 (7143478) users      (100)        0 2024-05-10 05:33:03.472648 TorchKAN-0.1.1/TorchKAN.egg-info/
+-rw-r--r--   0 u7143478 (7143478) users      (100)     3828 2024-05-10 05:33:03.000000 TorchKAN-0.1.1/TorchKAN.egg-info/PKG-INFO
+-rw-r--r--   0 u7143478 (7143478) users      (100)      188 2024-05-10 05:33:03.000000 TorchKAN-0.1.1/TorchKAN.egg-info/SOURCES.txt
+-rw-r--r--   0 u7143478 (7143478) users      (100)        1 2024-05-10 05:33:03.000000 TorchKAN-0.1.1/TorchKAN.egg-info/dependency_links.txt
+-rw-r--r--   0 u7143478 (7143478) users      (100)       29 2024-05-10 05:33:03.000000 TorchKAN-0.1.1/TorchKAN.egg-info/requires.txt
+-rw-r--r--   0 u7143478 (7143478) users      (100)        1 2024-05-10 05:33:03.000000 TorchKAN-0.1.1/TorchKAN.egg-info/top_level.txt
+-rw-r--r--   0 u7143478 (7143478) users      (100)       38 2024-05-10 05:33:03.472648 TorchKAN-0.1.1/setup.cfg
+-rw-r--r--   0 u7143478 (7143478) users      (100)     1039 2024-05-10 05:32:59.000000 TorchKAN-0.1.1/setup.py
```

### Comparing `TorchKAN-0.1.0/LICENSE.md` & `TorchKAN-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `TorchKAN-0.1.0/PKG-INFO` & `TorchKAN-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: TorchKAN
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy-to-use PyTorch implementation of the Kolmogorov Arnold Network
 Home-page: https://github.com/1ssb/torchkan
 Author: Subhransu Bhattacharjee
 Author-email: Subhransu.Bhattacharjee@anu.edu.au
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: torch==1.8.1+cu101
-Requires-Dist: torchvision==0.9.1+cu101
-Requires-Dist: torchaudio==0.8.1
+Requires-Dist: torch
+Requires-Dist: torchvision
 Requires-Dist: wandb
 Requires-Dist: tqdm
-Requires-Dist: numpy
-Requires-Dist: matplotlib
 
-# TorchKAN: Simplified KAN Model Evaluation
+# TorchKAN: A Simplified KAN Model (Version: 0)
+[![PyPI version](https://badge.fury.io/py/TorchKAN.svg)](https://pypi.org/project/TorchKAN/)
 
-This project demonstrates the training, validation, and quantization of the KAN model using PyTorch with CUDA acceleration. The `torchkan` model evaluates performance on the MNIST dataset, providing insights into the capabilities of Generalized Additive Models (GAMs).
+This project demonstrates the training, validation, and quantization of the KAN model using PyTorch with CUDA acceleration. The `torchkan` model evaluates performance on the MNIST dataset.
 
 ## Project Status: Under Development
 
-The KAN model has shown promising results amidst various GAMs since the 1980s. This implementation, inspired by various sources, achieves over 97% accuracy on the MNIST dataset. As this model is still under study, further exploration into its full capabilities is ongoing.
+The KAN model has shown promising results amidst various GAMs since the 1980s. This implementation, inspired by various sources, achieves over 97% accuracy with an eval time of 0.6 seconds and the quantised model achieves under 0.55 seconds on the MNIST dataset in 8 epochs on a Ubuntu 22.04 OS with a single Nvidia RTX4090. 
+
+As this model is still under study, further exploration into its full capabilities is ongoing.
 
 ## Prerequisites
 
 Ensure you have the following installed on your system:
 
 - Python (version 3.9 or higher)
 - CUDA Toolkit (corresponding to your PyTorch installation's CUDA version)
@@ -49,14 +49,20 @@
 
 ```bash
 git clone https://github.com/1ssb/torchkan.git
 cd torchkan
 pip install -r requirements.txt
 ```
 
+Alternately PyPi install as:
+
+```bash
+pip install torchKAN
+```
+
 ### 2. Configure CUDA environment variables if they are not already set:
 
 ```bash
 export PATH=/usr/local/cuda/bin:$PATH
 export LD_LIBRARY_PATH=/usr/local/cuda/lib64:$LD_LIBRARY_PATH
 ```
 
@@ -83,14 +89,29 @@
 
 This script will train the model, validate it, and log performance metrics using wandb.
 
 ## Contact
 
 For any inquiries or support, contact: Subhransu.Bhattacharjee@anu.edu.au
 
+## Cite this Project
+
+If you use this project in your research or wish to refer to the baseline results, please use the following BibTeX entry.
+
+```bibtex
+@misc{torchkan,
+  author = {Subhransu S. Bhattacharjee},
+  title = {TorchKAN},
+  year = {2024},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/1ssb/torchkan/}}
+}
+```
+
 ## Contributions
 
 Contributions are welcome. Please raise issues as necessary after commit "Fin.", scheduled end-June, 2024. The code is licensed under the MIT License.
 
 ## References
 
 - [0] Ziming Liu et al., "KAN: Kolmogorov-Arnold Networks", 2024, arXiv. https://arxiv.org/abs/2404.19756
```

### Comparing `TorchKAN-0.1.0/README.md` & `TorchKAN-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-# TorchKAN: Simplified KAN Model Evaluation
+# TorchKAN: A Simplified KAN Model (Version: 0)
+[![PyPI version](https://badge.fury.io/py/TorchKAN.svg)](https://pypi.org/project/TorchKAN/)
 
-This project demonstrates the training, validation, and quantization of the KAN model using PyTorch with CUDA acceleration. The `torchkan` model evaluates performance on the MNIST dataset, providing insights into the capabilities of Generalized Additive Models (GAMs).
+This project demonstrates the training, validation, and quantization of the KAN model using PyTorch with CUDA acceleration. The `torchkan` model evaluates performance on the MNIST dataset.
 
 ## Project Status: Under Development
 
-The KAN model has shown promising results amidst various GAMs since the 1980s. This implementation, inspired by various sources, achieves over 97% accuracy on the MNIST dataset. As this model is still under study, further exploration into its full capabilities is ongoing.
+The KAN model has shown promising results amidst various GAMs since the 1980s. This implementation, inspired by various sources, achieves over 97% accuracy with an eval time of 0.6 seconds and the quantised model achieves under 0.55 seconds on the MNIST dataset in 8 epochs on a Ubuntu 22.04 OS with a single Nvidia RTX4090. 
+
+As this model is still under study, further exploration into its full capabilities is ongoing.
 
 ## Prerequisites
 
 Ensure you have the following installed on your system:
 
 - Python (version 3.9 or higher)
 - CUDA Toolkit (corresponding to your PyTorch installation's CUDA version)
@@ -24,14 +27,20 @@
 
 ```bash
 git clone https://github.com/1ssb/torchkan.git
 cd torchkan
 pip install -r requirements.txt
 ```
 
+Alternately PyPi install as:
+
+```bash
+pip install torchKAN
+```
+
 ### 2. Configure CUDA environment variables if they are not already set:
 
 ```bash
 export PATH=/usr/local/cuda/bin:$PATH
 export LD_LIBRARY_PATH=/usr/local/cuda/lib64:$LD_LIBRARY_PATH
 ```
 
@@ -58,14 +67,29 @@
 
 This script will train the model, validate it, and log performance metrics using wandb.
 
 ## Contact
 
 For any inquiries or support, contact: Subhransu.Bhattacharjee@anu.edu.au
 
+## Cite this Project
+
+If you use this project in your research or wish to refer to the baseline results, please use the following BibTeX entry.
+
+```bibtex
+@misc{torchkan,
+  author = {Subhransu S. Bhattacharjee},
+  title = {TorchKAN},
+  year = {2024},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/1ssb/torchkan/}}
+}
+```
+
 ## Contributions
 
 Contributions are welcome. Please raise issues as necessary after commit "Fin.", scheduled end-June, 2024. The code is licensed under the MIT License.
 
 ## References
 
 - [0] Ziming Liu et al., "KAN: Kolmogorov-Arnold Networks", 2024, arXiv. https://arxiv.org/abs/2404.19756
```

### Comparing `TorchKAN-0.1.0/TorchKAN.egg-info/PKG-INFO` & `TorchKAN-0.1.1/TorchKAN.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: TorchKAN
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy-to-use PyTorch implementation of the Kolmogorov Arnold Network
 Home-page: https://github.com/1ssb/torchkan
 Author: Subhransu Bhattacharjee
 Author-email: Subhransu.Bhattacharjee@anu.edu.au
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: torch==1.8.1+cu101
-Requires-Dist: torchvision==0.9.1+cu101
-Requires-Dist: torchaudio==0.8.1
+Requires-Dist: torch
+Requires-Dist: torchvision
 Requires-Dist: wandb
 Requires-Dist: tqdm
-Requires-Dist: numpy
-Requires-Dist: matplotlib
 
-# TorchKAN: Simplified KAN Model Evaluation
+# TorchKAN: A Simplified KAN Model (Version: 0)
+[![PyPI version](https://badge.fury.io/py/TorchKAN.svg)](https://pypi.org/project/TorchKAN/)
 
-This project demonstrates the training, validation, and quantization of the KAN model using PyTorch with CUDA acceleration. The `torchkan` model evaluates performance on the MNIST dataset, providing insights into the capabilities of Generalized Additive Models (GAMs).
+This project demonstrates the training, validation, and quantization of the KAN model using PyTorch with CUDA acceleration. The `torchkan` model evaluates performance on the MNIST dataset.
 
 ## Project Status: Under Development
 
-The KAN model has shown promising results amidst various GAMs since the 1980s. This implementation, inspired by various sources, achieves over 97% accuracy on the MNIST dataset. As this model is still under study, further exploration into its full capabilities is ongoing.
+The KAN model has shown promising results amidst various GAMs since the 1980s. This implementation, inspired by various sources, achieves over 97% accuracy with an eval time of 0.6 seconds and the quantised model achieves under 0.55 seconds on the MNIST dataset in 8 epochs on a Ubuntu 22.04 OS with a single Nvidia RTX4090. 
+
+As this model is still under study, further exploration into its full capabilities is ongoing.
 
 ## Prerequisites
 
 Ensure you have the following installed on your system:
 
 - Python (version 3.9 or higher)
 - CUDA Toolkit (corresponding to your PyTorch installation's CUDA version)
@@ -49,14 +49,20 @@
 
 ```bash
 git clone https://github.com/1ssb/torchkan.git
 cd torchkan
 pip install -r requirements.txt
 ```
 
+Alternately PyPi install as:
+
+```bash
+pip install torchKAN
+```
+
 ### 2. Configure CUDA environment variables if they are not already set:
 
 ```bash
 export PATH=/usr/local/cuda/bin:$PATH
 export LD_LIBRARY_PATH=/usr/local/cuda/lib64:$LD_LIBRARY_PATH
 ```
 
@@ -83,14 +89,29 @@
 
 This script will train the model, validate it, and log performance metrics using wandb.
 
 ## Contact
 
 For any inquiries or support, contact: Subhransu.Bhattacharjee@anu.edu.au
 
+## Cite this Project
+
+If you use this project in your research or wish to refer to the baseline results, please use the following BibTeX entry.
+
+```bibtex
+@misc{torchkan,
+  author = {Subhransu S. Bhattacharjee},
+  title = {TorchKAN},
+  year = {2024},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/1ssb/torchkan/}}
+}
+```
+
 ## Contributions
 
 Contributions are welcome. Please raise issues as necessary after commit "Fin.", scheduled end-June, 2024. The code is licensed under the MIT License.
 
 ## References
 
 - [0] Ziming Liu et al., "KAN: Kolmogorov-Arnold Networks", 2024, arXiv. https://arxiv.org/abs/2404.19756
```

### Comparing `TorchKAN-0.1.0/setup.py` & `TorchKAN-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='TorchKAN',  # Replace with your package name
-    version='0.1.0',  # Version 0 indicating early development
+    version='0.1.1',  # Version 0 indicating early development
     packages=find_packages(),
     description='An easy-to-use PyTorch implementation of the Kolmogorov Arnold Network',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Subhransu Bhattacharjee',
     author_email='Subhransu.Bhattacharjee@anu.edu.au',
     url='https://github.com/1ssb/torchkan',
     install_requires=[
-        'torch==1.8.1+cu101',
-        'torchvision==0.9.1+cu101',
-        'torchaudio==0.8.1',
+        'torch',
+        'torchvision',
         'wandb',
-        'tqdm',
-        'numpy',
-        'matplotlib'
+        'tqdm'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
```

