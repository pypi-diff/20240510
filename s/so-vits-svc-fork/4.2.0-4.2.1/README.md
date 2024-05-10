# Comparing `tmp/so_vits_svc_fork-4.2.0.tar.gz` & `tmp/so_vits_svc_fork-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-4.2.0.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-4.2.1.tar", max compression
```

## Comparing `so_vits_svc_fork-4.2.0.tar` & `so_vits_svc_fork-4.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    12463 2024-04-11 03:10:27.152538 so_vits_svc_fork-4.2.0/LICENSE
--rw-r--r--   0        0        0    33321 2024-04-11 03:10:27.152538 so_vits_svc_fork-4.2.0/README.md
--rw-r--r--   0        0        0     3121 2024-04-11 03:10:27.952539 so_vits_svc_fork-4.2.0/pyproject.toml
--rw-r--r--   0        0        0       70 2024-04-11 03:10:27.916539 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    24947 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1393 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     4914 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2875 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2599 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    30617 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      872 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2024-04-11 03:10:27.156538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    24749 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     9418 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1169 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     4620 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1463 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4733 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     2051 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1705 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1862 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2975 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
--rw-r--r--   0        0        0     2710 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4667 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4447 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     3004 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     2206 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    21359 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    15617 2024-04-11 03:10:27.160538 so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    35235 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0    12463 2024-05-10 11:29:36.365282 so_vits_svc_fork-4.2.1/LICENSE
+-rw-r--r--   0        0        0    33321 2024-05-10 11:29:36.365282 so_vits_svc_fork-4.2.1/README.md
+-rw-r--r--   0        0        0     3171 2024-05-10 11:29:37.177288 so_vits_svc_fork-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-05-10 11:29:37.137287 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    24947 2024-05-10 11:29:36.365282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1393 2024-05-10 11:29:36.365282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     4914 2024-05-10 11:29:36.365282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2875 2024-05-10 11:29:36.365282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2599 2024-05-10 11:29:36.365282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    30617 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      872 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24749 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     9418 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1169 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     4620 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1463 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4733 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2051 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1705 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1862 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2975 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
+-rw-r--r--   0        0        0     2710 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4667 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4447 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     3004 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     2206 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    21359 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    15617 2024-05-10 11:29:36.369282 so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    35298 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.2.1/PKG-INFO
```

### Comparing `so_vits_svc_fork-4.2.0/LICENSE` & `so_vits_svc_fork-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/README.md` & `so_vits_svc_fork-4.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -79,41 +79,41 @@
 python -m pip install --user pipx
 python -m pipx ensurepath
 ```
 
 #### 2. Installing so-vits-svc-fork
 
 ```shell
-pipx install so-vits-svc-fork --python=3.10
+pipx install so-vits-svc-fork --python=3.11
 pipx inject so-vits-svc-fork torch torchaudio --pip-args="--upgrade" --index-url=https://download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
 ```
 
 ### Option 3. Manual installation
 
 <details>
   <summary>Creating a virtual environment</summary>
 
 Windows:
 
 ```shell
-py -3.10 -m venv venv
+py -3.11 -m venv venv
 venv\Scripts\activate
 ```
 
 Linux/MacOS:
 
 ```shell
-python3.10 -m venv venv
+python3.11 -m venv venv
 source venv/bin/activate
 ```
 
 Anaconda:
 
 ```shell
-conda create -n so-vits-svc-fork python=3.10 pip
+conda create -n so-vits-svc-fork python=3.11 pip
 conda activate so-vits-svc-fork
 ```
 
 Installing without creating a virtual environment may cause a `PermissionError` if Python is installed in Program Files, etc.
 
 </details>
```

#### html2text {}

```diff
@@ -22,21 +22,21 @@
 Installation ### Option 1. One click easy installation _[_D_o_w_n_l_o_a_d_ _._b_a_t_]This BAT
 file will automatically perform the steps described below. ### Option 2. Manual
 installation (using pipx, experimental) #### 1. Installing pipx Windows
 (development version required due to [pypa/pipx#940](https://github.com/pypa/
 pipx/issues/940)): ```shell py -3 -m pip install --user git+https://github.com/
 pypa/pipx.git py -3 -m pipx ensurepath ``` Linux/MacOS: ```shell python -m pip
 install --user pipx python -m pipx ensurepath ``` #### 2. Installing so-vits-
-svc-fork ```shell pipx install so-vits-svc-fork --python=3.10 pipx inject so-
+svc-fork ```shell pipx install so-vits-svc-fork --python=3.11 pipx inject so-
 vits-svc-fork torch torchaudio --pip-args="--upgrade" --index-url=https://
 download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
 ``` ### Option 3. Manual installation Creating a virtual environment Windows:
-```shell py -3.10 -m venv venv venv\Scripts\activate ``` Linux/MacOS: ```shell
-python3.10 -m venv venv source venv/bin/activate ``` Anaconda: ```shell conda
-create -n so-vits-svc-fork python=3.10 pip conda activate so-vits-svc-fork ```
+```shell py -3.11 -m venv venv venv\Scripts\activate ``` Linux/MacOS: ```shell
+python3.11 -m venv venv source venv/bin/activate ``` Anaconda: ```shell conda
+create -n so-vits-svc-fork python=3.11 pip conda activate so-vits-svc-fork ```
 Installing without creating a virtual environment may cause a `PermissionError`
 if Python is installed in Program Files, etc. Install this via pip (or your
 favourite package manager that uses pip): ```shell python -m pip install -U pip
 setuptools wheel pip install -U torch torchaudio --index-url https://
 download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
 pip install -U so-vits-svc-fork ``` Notes - If no GPU is available or using
 MacOS, simply remove `pip install -U torch torchaudio --index-url https://
```

### Comparing `so_vits_svc_fork-4.2.0/pyproject.toml` & `so_vits_svc_fork-4.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "4.2.0"
+version = "4.2.1"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
@@ -27,45 +27,47 @@
 svcf-gui = "so_vits_svc_fork.gui:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/34j/so-vits-svc-fork/issues"
 "Changelog" = "https://github.com/34j/so-vits-svc-fork/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.13"
+python = ">=3.9,<3.13"
 librosa = "*"
-numpy = "^1.23"
+numpy = "^1.26.4"
 pyworld = "*"
 requests = "*"
 scipy = "*"
 sounddevice = "*"
 SoundFile = "*"
 tqdm = "*"
 praat-parselmouth = "*"
 onnx = "*"
 onnxsim = "*"
 onnxoptimizer = "*"
-torch = "*"
+torch = "^2"
 torchaudio = "*"
 tensorboard = "*"
 rich = "*"
-tqdm-joblib = "*"
+tqdm-joblib = "^0.0.3"
 tensorboardx = "*"
 cm-time = ">=0.1.2"
 pysimplegui = ">=4.6,<5" # never update this, advertising popup window will be shown
 pebble = ">=5.0"
 torchcrepe = ">=0.0.17"
 lightning = "^2.0.1"
 fastapi = "==0.110.1"
 transformers = "^4.28.1"
 matplotlib = "^3.7.1"
+click = "^8.1.7"
+setuptools = "^69.5.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=3"
-pytest = "^7.0"
+pytest = "^8.0.0"
 pytest-cov = "^4.0.0"
 pipdeptree = "^2.7.0"
 pip-licenses = "^4.3.1"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_classify.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/preprocess_classify.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/train.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-4.2.1/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.0/PKG-INFO` & `so_vits_svc_fork-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 4.2.0
+Version: 4.2.1
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
-Requires-Python: >=3.8,<3.13
+Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: SoundFile
+Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cm-time (>=0.1.2)
 Requires-Dist: fastapi (==0.110.1)
 Requires-Dist: librosa
 Requires-Dist: lightning (>=2.0.1,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (>=1.23,<2.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: onnx
 Requires-Dist: onnxoptimizer
 Requires-Dist: onnxsim
 Requires-Dist: pebble (>=5.0)
 Requires-Dist: praat-parselmouth
 Requires-Dist: pysimplegui (>=4.6,<5)
 Requires-Dist: pyworld
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: scipy
+Requires-Dist: setuptools (>=69.5.1,<70.0.0)
 Requires-Dist: sounddevice
 Requires-Dist: tensorboard
 Requires-Dist: tensorboardx
-Requires-Dist: torch
+Requires-Dist: torch (>=2,<3)
 Requires-Dist: torchaudio
 Requires-Dist: torchcrepe (>=0.0.17)
 Requires-Dist: tqdm
-Requires-Dist: tqdm-joblib
+Requires-Dist: tqdm-joblib (>=0.0.3,<0.0.4)
 Requires-Dist: transformers (>=4.28.1,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/34j/so-vits-svc-fork/issues
 Project-URL: Changelog, https://github.com/34j/so-vits-svc-fork/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://so-vits-svc-fork.readthedocs.io
 Project-URL: Repository, https://github.com/34j/so-vits-svc-fork
 Description-Content-Type: text/markdown
 
@@ -132,41 +133,41 @@
 python -m pip install --user pipx
 python -m pipx ensurepath
 ```
 
 #### 2. Installing so-vits-svc-fork
 
 ```shell
-pipx install so-vits-svc-fork --python=3.10
+pipx install so-vits-svc-fork --python=3.11
 pipx inject so-vits-svc-fork torch torchaudio --pip-args="--upgrade" --index-url=https://download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
 ```
 
 ### Option 3. Manual installation
 
 <details>
   <summary>Creating a virtual environment</summary>
 
 Windows:
 
 ```shell
-py -3.10 -m venv venv
+py -3.11 -m venv venv
 venv\Scripts\activate
 ```
 
 Linux/MacOS:
 
 ```shell
-python3.10 -m venv venv
+python3.11 -m venv venv
 source venv/bin/activate
 ```
 
 Anaconda:
 
 ```shell
-conda create -n so-vits-svc-fork python=3.10 pip
+conda create -n so-vits-svc-fork python=3.11 pip
 conda activate so-vits-svc-fork
 ```
 
 Installing without creating a virtual environment may cause a `PermissionError` if Python is installed in Program Files, etc.
 
 </details>
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.2.0 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.2.1 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
->=3.8,<3.13 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
+>=3.9,<3.13 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Topic :: Software Development :: Libraries Requires-
-Dist: SoundFile Requires-Dist: cm-time (>=0.1.2) Requires-Dist: fastapi
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Topic :: Software
+Development :: Libraries Requires-Dist: SoundFile Requires-Dist: click
+(>=8.1.7,<9.0.0) Requires-Dist: cm-time (>=0.1.2) Requires-Dist: fastapi
 (==0.110.1) Requires-Dist: librosa Requires-Dist: lightning (>=2.0.1,<3.0.0)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist: numpy (>=1.23,<2.0)
-Requires-Dist: onnx Requires-Dist: onnxoptimizer Requires-Dist: onnxsim
-Requires-Dist: pebble (>=5.0) Requires-Dist: praat-parselmouth Requires-Dist:
-pysimplegui (>=4.6,<5) Requires-Dist: pyworld Requires-Dist: requests Requires-
-Dist: rich Requires-Dist: scipy Requires-Dist: sounddevice Requires-Dist:
-tensorboard Requires-Dist: tensorboardx Requires-Dist: torch Requires-Dist:
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist: numpy
+(>=1.26.4,<2.0.0) Requires-Dist: onnx Requires-Dist: onnxoptimizer Requires-
+Dist: onnxsim Requires-Dist: pebble (>=5.0) Requires-Dist: praat-parselmouth
+Requires-Dist: pysimplegui (>=4.6,<5) Requires-Dist: pyworld Requires-Dist:
+requests Requires-Dist: rich Requires-Dist: scipy Requires-Dist: setuptools
+(>=69.5.1,<70.0.0) Requires-Dist: sounddevice Requires-Dist: tensorboard
+Requires-Dist: tensorboardx Requires-Dist: torch (>=2,<3) Requires-Dist:
 torchaudio Requires-Dist: torchcrepe (>=0.0.17) Requires-Dist: tqdm Requires-
-Dist: tqdm-joblib Requires-Dist: transformers (>=4.28.1,<5.0.0) Project-URL:
-Bug Tracker, https://github.com/34j/so-vits-svc-fork/issues Project-URL:
-Changelog, https://github.com/34j/so-vits-svc-fork/blob/main/CHANGELOG.md
-Project-URL: Documentation, https://so-vits-svc-fork.readthedocs.io Project-
-URL: Repository, https://github.com/34j/so-vits-svc-fork Description-Content-
-Type: text/markdown # SoftVC VITS Singing Voice Conversion Fork [ç®ä½ä¸­æ]
-(README_zh_CN.md)
+Dist: tqdm-joblib (>=0.0.3,<0.0.4) Requires-Dist: transformers
+(>=4.28.1,<5.0.0) Project-URL: Bug Tracker, https://github.com/34j/so-vits-svc-
+fork/issues Project-URL: Changelog, https://github.com/34j/so-vits-svc-fork/
+blob/main/CHANGELOG.md Project-URL: Documentation, https://so-vits-svc-
+fork.readthedocs.io Project-URL: Repository, https://github.com/34j/so-vits-
+svc-fork Description-Content-Type: text/markdown # SoftVC VITS Singing Voice
+Conversion Fork [ç®ä½ä¸­æ](README_zh_CN.md)
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 A fork of [`so-vits-svc`](https://github.com/svc-develop-team/so-vits-svc) with
 **realtime support** and **greatly improved interface**. Based on branch `4.0`
 (v1) (or `4.1`) and the models are compatible. > Updates to this repository
 have been limited to maintenance since Spring 2023. > It is difficult to narrow
@@ -48,21 +49,21 @@
 Installation ### Option 1. One click easy installation _[_D_o_w_n_l_o_a_d_ _._b_a_t_]This BAT
 file will automatically perform the steps described below. ### Option 2. Manual
 installation (using pipx, experimental) #### 1. Installing pipx Windows
 (development version required due to [pypa/pipx#940](https://github.com/pypa/
 pipx/issues/940)): ```shell py -3 -m pip install --user git+https://github.com/
 pypa/pipx.git py -3 -m pipx ensurepath ``` Linux/MacOS: ```shell python -m pip
 install --user pipx python -m pipx ensurepath ``` #### 2. Installing so-vits-
-svc-fork ```shell pipx install so-vits-svc-fork --python=3.10 pipx inject so-
+svc-fork ```shell pipx install so-vits-svc-fork --python=3.11 pipx inject so-
 vits-svc-fork torch torchaudio --pip-args="--upgrade" --index-url=https://
 download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
 ``` ### Option 3. Manual installation Creating a virtual environment Windows:
-```shell py -3.10 -m venv venv venv\Scripts\activate ``` Linux/MacOS: ```shell
-python3.10 -m venv venv source venv/bin/activate ``` Anaconda: ```shell conda
-create -n so-vits-svc-fork python=3.10 pip conda activate so-vits-svc-fork ```
+```shell py -3.11 -m venv venv venv\Scripts\activate ``` Linux/MacOS: ```shell
+python3.11 -m venv venv source venv/bin/activate ``` Anaconda: ```shell conda
+create -n so-vits-svc-fork python=3.11 pip conda activate so-vits-svc-fork ```
 Installing without creating a virtual environment may cause a `PermissionError`
 if Python is installed in Program Files, etc. Install this via pip (or your
 favourite package manager that uses pip): ```shell python -m pip install -U pip
 setuptools wheel pip install -U torch torchaudio --index-url https://
 download.pytorch.org/whl/cu121 # https://download.pytorch.org/whl/nightly/cu121
 pip install -U so-vits-svc-fork ``` Notes - If no GPU is available or using
 MacOS, simply remove `pip install -U torch torchaudio --index-url https://
```

