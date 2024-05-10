# Comparing `tmp/torchinstaller-0.8.5.tar.gz` & `tmp/torchinstaller-0.8.6.tar.gz`

## Comparing `torchinstaller-0.8.5.tar` & `torchinstaller-0.8.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/.vscode/launch.json
--rw-r--r--   0        0        0    15956 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/assets/torchinstaller_icon.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/tests/__init__.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/tests/test_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/torchinstaller/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/torchinstaller/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/torchinstaller/__version__.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/torchinstaller/_parse.py
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/torchinstaller/_soup.py
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/torchinstaller/main.py
--rw-r--r--   0        0        0     8268 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/torchinstaller/utils.py
--rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/torchinstaller/config/commands.bak.toml
--rw-r--r--   0        0        0    17904 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/torchinstaller/config/commands.md
--rw-r--r--   0        0        0    34755 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/torchinstaller/config/commands.toml
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/LICENSE
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 torchinstaller-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/.vscode/launch.json
+-rw-r--r--   0        0        0    15956 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/assets/torchinstaller_icon.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/tests/__init__.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/tests/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/torchinstaller/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/torchinstaller/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/torchinstaller/__version__.py
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/torchinstaller/_parse.py
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/torchinstaller/_soup.py
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/torchinstaller/main.py
+-rw-r--r--   0        0        0     8268 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/torchinstaller/utils.py
+-rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/torchinstaller/config/commands.bak.toml
+-rw-r--r--   0        0        0    19784 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/torchinstaller/config/commands.md
+-rw-r--r--   0        0        0    38483 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/torchinstaller/config/commands.toml
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/LICENSE
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 torchinstaller-0.8.6/PKG-INFO
```

### Comparing `torchinstaller-0.8.5/.vscode/launch.json` & `torchinstaller-0.8.6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `torchinstaller-0.8.5/assets/torchinstaller_icon.png` & `torchinstaller-0.8.6/assets/torchinstaller_icon.png`

 * *Files identical despite different names*

### Comparing `torchinstaller-0.8.5/tests/test_config.py` & `torchinstaller-0.8.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `torchinstaller-0.8.5/torchinstaller/_parse.py` & `torchinstaller-0.8.6/torchinstaller/_parse.py`

 * *Files identical despite different names*

### Comparing `torchinstaller-0.8.5/torchinstaller/_soup.py` & `torchinstaller-0.8.6/torchinstaller/_soup.py`

 * *Files identical despite different names*

### Comparing `torchinstaller-0.8.5/torchinstaller/main.py` & `torchinstaller-0.8.6/torchinstaller/main.py`

 * *Files identical despite different names*

### Comparing `torchinstaller-0.8.5/torchinstaller/utils.py` & `torchinstaller-0.8.6/torchinstaller/utils.py`

 * *Files identical despite different names*

### Comparing `torchinstaller-0.8.5/torchinstaller/config/commands.bak.toml` & `torchinstaller-0.8.6/torchinstaller/config/commands.bak.toml`

 * *Files identical despite different names*

### Comparing `torchinstaller-0.8.5/torchinstaller/config/commands.md` & `torchinstaller-0.8.6/torchinstaller/config/commands.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,50 @@
 
-# latest (v2.2.1)
+# latest (v2.3.0)
 # macOS
 conda install pytorch::pytorch torchvision torchaudio -c pytorch
 # Linux
 conda install pytorch torchvision torchaudio pytorch-cuda=12.1 -c pytorch -c nvidia
 conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia
 conda install pytorch torchvision torchaudio cpuonly -c pytorch
 # macOS
 pip install torch torchvision torchaudio
 # Linux
 pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
 pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
 pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/rocm5.7
 pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cpu
+# v2.2.2
+## macOS
+conda install pytorch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 -c pytorch
+## Linux
+conda install pytorch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 pytorch-cuda=11.8 -c pytorch -c nvidia
+conda install pytorch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 pytorch-cuda=12.1 -c pytorch -c nvidia
+conda install pytorch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 cpuonly -c pytorch
+## macOS
+pip install torch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2
+## Linux
+pip install torch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 --index-url https://download.pytorch.org/whl/rocm5.7
+pip install torch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 --index-url https://download.pytorch.org/whl/cu118
+pip install torch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 --index-url https://download.pytorch.org/whl/cu121
+pip install torch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 --index-url https://download.pytorch.org/whl/cpu
+# v2.2.1
+## macOS
+conda install pytorch==2.2.1 torchvision==0.17.1 torchaudio==2.2.1 -c pytorch
+## Linux
+conda install pytorch==2.2.1 torchvision==0.17.1 torchaudio==2.2.1 pytorch-cuda=11.8 -c pytorch -c nvidia
+conda install pytorch==2.2.1 torchvision==0.17.1 torchaudio==2.2.1 pytorch-cuda=12.1 -c pytorch -c nvidia
+conda install pytorch==2.2.1 torchvision==0.17.1 torchaudio==2.2.1 cpuonly -c pytorch
+## macOS
+pip install torch==2.2.1 torchvision==0.17.1 torchaudio==2.2.1
+## Linux
+pip install torch==2.2.1 torchvision==0.17.1 torchaudio==2.2.1 --index-url https://download.pytorch.org/whl/rocm5.7
+pip install torch==2.2.1 torchvision==0.17.1 torchaudio==2.2.1 --index-url https://download.pytorch.org/whl/cu118
+pip install torch==2.2.1 torchvision==0.17.1 torchaudio==2.2.1 --index-url https://download.pytorch.org/whl/cu121
+pip install torch==2.2.1 torchvision==0.17.1 torchaudio==2.2.1 --index-url https://download.pytorch.org/whl/cpu
 # v2.2.0
 ## macOS
 conda install pytorch==2.2.0 torchvision==0.17.0 torchaudio==2.2.0 -c pytorch
 ## Linux
 conda install pytorch==2.2.0 torchvision==0.17.0 torchaudio==2.2.0 pytorch-cuda=11.8 -c pytorch -c nvidia
 conda install pytorch==2.2.0 torchvision==0.17.0 torchaudio==2.2.0 pytorch-cuda=12.1 -c pytorch -c nvidia
 conda install pytorch==2.2.0 torchvision==0.17.0 torchaudio==2.2.0 cpuonly -c pytorch
```

### Comparing `torchinstaller-0.8.5/torchinstaller/config/commands.toml` & `torchinstaller-0.8.6/torchinstaller/config/commands.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,36 @@
 version = "latest"
 
 [cpu.conda.packages]
 
 [[cpu.conda]]
 installer = "conda"
 flags = ["cpuonly", "-c", "pytorch"]
+version = "2.2.2"
+platform = "cpu"
+
+[cpu.conda.packages]
+pytorch = "2.2.2"
+torchvision = "0.17.2"
+torchaudio = "2.2.2"
+
+[[cpu.conda]]
+installer = "conda"
+flags = ["cpuonly", "-c", "pytorch"]
+version = "2.2.1"
+platform = "cpu"
+
+[cpu.conda.packages]
+pytorch = "2.2.1"
+torchvision = "0.17.1"
+torchaudio = "2.2.1"
+
+[[cpu.conda]]
+installer = "conda"
+flags = ["cpuonly", "-c", "pytorch"]
 version = "2.2.0"
 platform = "cpu"
 
 [cpu.conda.packages]
 pytorch = "2.2.0"
 torchvision = "0.17.0"
 torchaudio = "2.2.0"
@@ -187,14 +209,36 @@
 version = "latest"
 
 [cpu.pip.packages]
 
 [[cpu.pip]]
 installer = "pip"
 flags = ["--index-url", "https://download.pytorch.org/whl/cpu"]
+version = "2.2.2"
+platform = "cpu"
+
+[cpu.pip.packages]
+torch = "2.2.2"
+torchvision = "0.17.2"
+torchaudio = "2.2.2"
+
+[[cpu.pip]]
+installer = "pip"
+flags = ["--index-url", "https://download.pytorch.org/whl/cpu"]
+version = "2.2.1"
+platform = "cpu"
+
+[cpu.pip.packages]
+torch = "2.2.1"
+torchvision = "0.17.1"
+torchaudio = "2.2.1"
+
+[[cpu.pip]]
+installer = "pip"
+flags = ["--index-url", "https://download.pytorch.org/whl/cpu"]
 version = "2.2.0"
 platform = "cpu"
 
 [cpu.pip.packages]
 torch = "2.2.0"
 torchvision = "0.17.0"
 torchaudio = "2.2.0"
@@ -933,14 +977,38 @@
 
 [cu118.conda.packages]
 pytorch-cuda = "11.8"
 
 [[cu118.conda]]
 installer = "conda"
 flags = ["-c", "pytorch", "-c", "nvidia"]
+version = "2.2.2"
+platform = "cu118"
+
+[cu118.conda.packages]
+pytorch = "2.2.2"
+torchvision = "0.17.2"
+torchaudio = "2.2.2"
+pytorch-cuda = "11.8"
+
+[[cu118.conda]]
+installer = "conda"
+flags = ["-c", "pytorch", "-c", "nvidia"]
+version = "2.2.1"
+platform = "cu118"
+
+[cu118.conda.packages]
+pytorch = "2.2.1"
+torchvision = "0.17.1"
+torchaudio = "2.2.1"
+pytorch-cuda = "11.8"
+
+[[cu118.conda]]
+installer = "conda"
+flags = ["-c", "pytorch", "-c", "nvidia"]
 version = "2.2.0"
 platform = "cu118"
 
 [cu118.conda.packages]
 pytorch = "2.2.0"
 torchvision = "0.17.0"
 torchaudio = "2.2.0"
@@ -1013,14 +1081,36 @@
 version = "latest"
 
 [cu118.pip.packages]
 
 [[cu118.pip]]
 installer = "pip"
 flags = ["--index-url", "https://download.pytorch.org/whl/cu118"]
+version = "2.2.2"
+platform = "cu118"
+
+[cu118.pip.packages]
+torch = "2.2.2"
+torchvision = "0.17.2"
+torchaudio = "2.2.2"
+
+[[cu118.pip]]
+installer = "pip"
+flags = ["--index-url", "https://download.pytorch.org/whl/cu118"]
+version = "2.2.1"
+platform = "cu118"
+
+[cu118.pip.packages]
+torch = "2.2.1"
+torchvision = "0.17.1"
+torchaudio = "2.2.1"
+
+[[cu118.pip]]
+installer = "pip"
+flags = ["--index-url", "https://download.pytorch.org/whl/cu118"]
 version = "2.2.0"
 platform = "cu118"
 
 [cu118.pip.packages]
 torch = "2.2.0"
 torchvision = "0.17.0"
 torchaudio = "2.2.0"
@@ -1089,14 +1179,38 @@
 
 [cu121.conda.packages]
 pytorch-cuda = "12.1"
 
 [[cu121.conda]]
 installer = "conda"
 flags = ["-c", "pytorch", "-c", "nvidia"]
+version = "2.2.2"
+platform = "cu121"
+
+[cu121.conda.packages]
+pytorch = "2.2.2"
+torchvision = "0.17.2"
+torchaudio = "2.2.2"
+pytorch-cuda = "12.1"
+
+[[cu121.conda]]
+installer = "conda"
+flags = ["-c", "pytorch", "-c", "nvidia"]
+version = "2.2.1"
+platform = "cu121"
+
+[cu121.conda.packages]
+pytorch = "2.2.1"
+torchvision = "0.17.1"
+torchaudio = "2.2.1"
+pytorch-cuda = "12.1"
+
+[[cu121.conda]]
+installer = "conda"
+flags = ["-c", "pytorch", "-c", "nvidia"]
 version = "2.2.0"
 platform = "cu121"
 
 [cu121.conda.packages]
 pytorch = "2.2.0"
 torchvision = "0.17.0"
 torchaudio = "2.2.0"
@@ -1145,14 +1259,36 @@
 version = "latest"
 
 [cu121.pip.packages]
 
 [[cu121.pip]]
 installer = "pip"
 flags = ["--index-url", "https://download.pytorch.org/whl/cu121"]
+version = "2.2.2"
+platform = "cu121"
+
+[cu121.pip.packages]
+torch = "2.2.2"
+torchvision = "0.17.2"
+torchaudio = "2.2.2"
+
+[[cu121.pip]]
+installer = "pip"
+flags = ["--index-url", "https://download.pytorch.org/whl/cu121"]
+version = "2.2.1"
+platform = "cu121"
+
+[cu121.pip.packages]
+torch = "2.2.1"
+torchvision = "0.17.1"
+torchaudio = "2.2.1"
+
+[[cu121.pip]]
+installer = "pip"
+flags = ["--index-url", "https://download.pytorch.org/whl/cu121"]
 version = "2.2.0"
 platform = "cu121"
 
 [cu121.pip.packages]
 torch = "2.2.0"
 torchvision = "0.17.0"
 torchaudio = "2.2.0"
@@ -1198,14 +1334,36 @@
 version = "latest"
 
 [macos.conda.packages]
 
 [[macos.conda]]
 installer = "conda"
 flags = ["-c", "pytorch"]
+version = "2.2.2"
+platform = "macos"
+
+[macos.conda.packages]
+pytorch = "2.2.2"
+torchvision = "0.17.2"
+torchaudio = "2.2.2"
+
+[[macos.conda]]
+installer = "conda"
+flags = ["-c", "pytorch"]
+version = "2.2.1"
+platform = "macos"
+
+[macos.conda.packages]
+pytorch = "2.2.1"
+torchvision = "0.17.1"
+torchaudio = "2.2.1"
+
+[[macos.conda]]
+installer = "conda"
+flags = ["-c", "pytorch"]
 version = "2.2.0"
 platform = "macos"
 
 [macos.conda.packages]
 pytorch = "2.2.0"
 torchvision = "0.17.0"
 torchaudio = "2.2.0"
@@ -1371,14 +1529,36 @@
 version = "latest"
 
 [macos.pip.packages]
 
 [[macos.pip]]
 installer = "pip"
 flags = []
+version = "2.2.2"
+platform = "macos"
+
+[macos.pip.packages]
+torch = "2.2.2"
+torchvision = "0.17.2"
+torchaudio = "2.2.2"
+
+[[macos.pip]]
+installer = "pip"
+flags = []
+version = "2.2.1"
+platform = "macos"
+
+[macos.pip.packages]
+torch = "2.2.1"
+torchvision = "0.17.1"
+torchaudio = "2.2.1"
+
+[[macos.pip]]
+installer = "pip"
+flags = []
 version = "2.2.0"
 platform = "macos"
 
 [macos.pip.packages]
 torch = "2.2.0"
 torchvision = "0.17.0"
 torchaudio = "2.2.0"
@@ -1793,7 +1973,29 @@
 [["rocm5.7".pip]]
 installer = "pip"
 flags = ["torch", "torchvision", "torchaudio", "--index-url", "https://download.pytorch.org/whl/rocm5.7"]
 platform = "rocm5.7"
 version = "latest"
 
 ["rocm5.7".pip.packages]
+
+[["rocm5.7".pip]]
+installer = "pip"
+flags = ["--index-url", "https://download.pytorch.org/whl/rocm5.7"]
+version = "2.2.2"
+platform = "rocm5.7"
+
+["rocm5.7".pip.packages]
+torch = "2.2.2"
+torchvision = "0.17.2"
+torchaudio = "2.2.2"
+
+[["rocm5.7".pip]]
+installer = "pip"
+flags = ["--index-url", "https://download.pytorch.org/whl/rocm5.7"]
+version = "2.2.1"
+platform = "rocm5.7"
+
+["rocm5.7".pip.packages]
+torch = "2.2.1"
+torchvision = "0.17.1"
+torchaudio = "2.2.1"
```

### Comparing `torchinstaller-0.8.5/.gitignore` & `torchinstaller-0.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `torchinstaller-0.8.5/LICENSE` & `torchinstaller-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `torchinstaller-0.8.5/README.md` & `torchinstaller-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `torchinstaller-0.8.5/pyproject.toml` & `torchinstaller-0.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchinstaller-0.8.5/PKG-INFO` & `torchinstaller-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: torchinstaller
-Version: 0.8.5
+Version: 0.8.6
 Summary: Simple utility to install pytorch, pytorch-geometric and pytorch-lightning. Detects CUDA version automatically.
 Project-URL: github, https://github.com/dk0d/torchinstaller.git
 Author-email: Daniel Capecci <7775585+dk0d@users.noreply.github.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: <4.0,>=3.10
 Requires-Dist: rich<14.0.0,>=13.3.3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchinstaller Version: 0.8.5 Summary: Simple
+Metadata-Version: 2.3 Name: torchinstaller Version: 0.8.6 Summary: Simple
 utility to install pytorch, pytorch-geometric and pytorch-lightning. Detects
 CUDA version automatically. Project-URL: github, https://github.com/dk0d/
 torchinstaller.git Author-email: Daniel Capecci
 <7775585+dk0d@users.noreply.github.com> License: MIT License-File: LICENSE
 Requires-Python: <4.0,>=3.10 Requires-Dist: rich<14.0.0,>=13.3.3 Requires-Dist:
 tomlkit<1.0.0,>=0.11.7 Provides-Extra: soup Requires-Dist: beautifulsoup4;
 extra == 'soup' Requires-Dist: requests; extra == 'soup' Requires-Dist:
```

