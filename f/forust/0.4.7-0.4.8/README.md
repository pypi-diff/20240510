# Comparing `tmp/forust-0.4.7.tar.gz` & `tmp/forust-0.4.8.tar.gz`

## Comparing `forust-0.4.7.tar` & `forust-0.4.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0     1001      127      593 2024-04-12 16:25:13.000000 forust-0.4.7/Cargo.toml
--rw-r--r--   0     1001      127     6951 2024-04-12 16:24:35.000000 forust-0.4.7/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      964 2024-04-12 16:24:35.000000 forust-0.4.7/.github/workflows/cargo-build-publish.yml
--rw-r--r--   0     1001      127      733 2024-04-12 16:24:35.000000 forust-0.4.7/.github/workflows/docs.yml
--rw-r--r--   0     1001      127      268 2024-04-12 16:24:35.000000 forust-0.4.7/.gitignore
--rw-r--r--   0     1001      127      431 2024-04-12 16:24:35.000000 forust-0.4.7/.pre-commit-config.yaml
--rw-r--r--   0     1001      127     3533 2024-04-12 16:24:35.000000 forust-0.4.7/CONTRIBUTING.md
--rw-r--r--   0     1001      127    11341 2024-04-12 16:24:35.000000 forust-0.4.7/LICENSE
--rw-r--r--   0     1001      127     7350 2024-04-12 16:24:35.000000 forust-0.4.7/README.md
--rw-r--r--   0     1001      127     5468 2024-04-12 16:24:35.000000 forust-0.4.7/benches/forust_benchmarks.rs
--rw-r--r--   0     1001      127   566309 2024-04-12 16:26:38.000000 forust-0.4.7/dist/forust-0.4.7-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
--rw-r--r--   0     1001      127    16121 2024-04-12 16:24:35.000000 forust-0.4.7/resources/pdp_plot_age.png
--rw-r--r--   0     1001      127    10758 2024-04-12 16:24:35.000000 forust-0.4.7/resources/pdp_plot_age_mono.png
--rw-r--r--   0     1001      127    57018 2024-04-12 16:24:35.000000 forust-0.4.7/resources/titanic.csv
--rw-r--r--   0     1001      127   655700 2024-04-12 16:24:35.000000 forust-0.4.7/resources/tree-image-crop.png
--rw-r--r--   0     1001      127     2563 2024-04-12 16:24:35.000000 forust-0.4.7/rs-example.md
--rw-r--r--   0     1001      127     1271 2024-04-12 16:24:35.000000 forust-0.4.7/scripts/make_resources.py
--rw-r--r--   0     1001      127      370 2024-04-12 16:24:35.000000 forust-0.4.7/scripts/remove-optional-deps.py
--rw-r--r--   0     1001      127       53 2024-04-12 16:24:35.000000 forust-0.4.7/scripts/run-python-tests.ps1
--rw-r--r--   0     1001      127       53 2024-04-12 16:24:35.000000 forust-0.4.7/scripts/run-python-tests.sh
--rw-r--r--   0     1001      127     5647 2024-04-12 16:24:35.000000 forust-0.4.7/src/binning.rs
--rw-r--r--   0     1001      127      248 2024-04-12 16:24:35.000000 forust-0.4.7/src/constraints.rs
--rw-r--r--   0     1001      127    10051 2024-04-12 16:24:35.000000 forust-0.4.7/src/data.rs
--rw-r--r--   0     1001      127      945 2024-04-12 16:24:35.000000 forust-0.4.7/src/errors.rs
--rw-r--r--   0     1001      127    57204 2024-04-12 16:24:35.000000 forust-0.4.7/src/gradientbooster.rs
--rw-r--r--   0     1001      127      881 2024-04-12 16:24:35.000000 forust-0.4.7/src/grower.rs
--rw-r--r--   0     1001      127     9977 2024-04-12 16:24:35.000000 forust-0.4.7/src/histogram.rs
--rw-r--r--   0     1001      127      384 2024-04-12 16:24:35.000000 forust-0.4.7/src/lib.rs
--rw-r--r--   0     1001      127     8933 2024-04-12 16:24:35.000000 forust-0.4.7/src/metric.rs
--rw-r--r--   0     1001      127     6863 2024-04-12 16:24:35.000000 forust-0.4.7/src/node.rs
--rw-r--r--   0     1001      127     5956 2024-04-12 16:24:35.000000 forust-0.4.7/src/objective.rs
--rw-r--r--   0     1001      127     4195 2024-04-12 16:24:35.000000 forust-0.4.7/src/partial_dependence.rs
--rw-r--r--   0     1001      127     2923 2024-04-12 16:24:35.000000 forust-0.4.7/src/sampler.rs
--rw-r--r--   0     1001      127     8072 2024-04-12 16:24:35.000000 forust-0.4.7/src/shapley.rs
--rw-r--r--   0     1001      127    41163 2024-04-12 16:24:35.000000 forust-0.4.7/src/splitter.rs
--rw-r--r--   0     1001      127    33600 2024-04-12 16:24:35.000000 forust-0.4.7/src/tree.rs
--rw-r--r--   0     1001      127    35433 2024-04-12 16:24:35.000000 forust-0.4.7/src/utils.rs
--rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 forust-0.4.7/py-forust/Cargo.toml
--rw-r--r--   0     1001      127      685 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/.gitignore
--rw-r--r--   0     1001      127     7350 2024-04-12 16:25:13.000000 forust-0.4.7/py-forust/README.md
--rw-r--r--   0     1001      127     1634 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/docs/index.md
--rw-r--r--   0     1001      127    55983 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/forust/__init__.py
--rw-r--r--   0     1001      127     1870 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/forust/serialize.py
--rw-r--r--   0     1001      127     1192 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/mkdocs.yml
--rw-r--r--   0     1001      127    16405 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/src/lib.rs
--rw-r--r--   0     1001      127    55742 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/tests/test_booster.py
--rw-r--r--   0     1001      127     1318 2024-04-12 16:24:35.000000 forust-0.4.7/py-forust/tests/test_serailze.py
--rw-r--r--   0     1001      127    15147 2024-04-12 16:25:59.000000 forust-0.4.7/py-forust/Cargo.lock
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 forust-0.4.7/pyproject.toml
--rw-r--r--   0     1001      127    55983 2024-04-12 16:24:35.000000 forust-0.4.7/forust/__init__.py
--rw-r--r--   0     1001      127     1870 2024-04-12 16:24:35.000000 forust-0.4.7/forust/serialize.py
--rw-r--r--   0        0        0     8353 1970-01-01 00:00:00.000000 forust-0.4.7/PKG-INFO
+-rw-r--r--   0     1001      127      593 2024-05-09 23:38:55.000000 forust-0.4.8/Cargo.toml
+-rw-r--r--   0     1001      127     8869 2024-05-09 23:38:24.000000 forust-0.4.8/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      964 2024-05-09 23:38:24.000000 forust-0.4.8/.github/workflows/cargo-build-publish.yml
+-rw-r--r--   0     1001      127      733 2024-05-09 23:38:24.000000 forust-0.4.8/.github/workflows/docs.yml
+-rw-r--r--   0     1001      127      268 2024-05-09 23:38:24.000000 forust-0.4.8/.gitignore
+-rw-r--r--   0     1001      127      431 2024-05-09 23:38:24.000000 forust-0.4.8/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127     3533 2024-05-09 23:38:24.000000 forust-0.4.8/CONTRIBUTING.md
+-rw-r--r--   0     1001      127    11341 2024-05-09 23:38:24.000000 forust-0.4.8/LICENSE
+-rw-r--r--   0     1001      127     7350 2024-05-09 23:38:24.000000 forust-0.4.8/README.md
+-rw-r--r--   0     1001      127     5468 2024-05-09 23:38:24.000000 forust-0.4.8/benches/forust_benchmarks.rs
+-rw-r--r--   0     1001      127   574756 2024-05-09 23:40:19.000000 forust-0.4.8/dist/forust-0.4.8-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+-rw-r--r--   0     1001      127    16121 2024-05-09 23:38:24.000000 forust-0.4.8/resources/pdp_plot_age.png
+-rw-r--r--   0     1001      127    10758 2024-05-09 23:38:24.000000 forust-0.4.8/resources/pdp_plot_age_mono.png
+-rw-r--r--   0     1001      127    57018 2024-05-09 23:38:24.000000 forust-0.4.8/resources/titanic.csv
+-rw-r--r--   0     1001      127   655700 2024-05-09 23:38:24.000000 forust-0.4.8/resources/tree-image-crop.png
+-rw-r--r--   0     1001      127     2563 2024-05-09 23:38:24.000000 forust-0.4.8/rs-example.md
+-rw-r--r--   0     1001      127     1271 2024-05-09 23:38:24.000000 forust-0.4.8/scripts/make_resources.py
+-rw-r--r--   0     1001      127      370 2024-05-09 23:38:24.000000 forust-0.4.8/scripts/remove-optional-deps.py
+-rw-r--r--   0     1001      127       53 2024-05-09 23:38:24.000000 forust-0.4.8/scripts/run-python-tests.ps1
+-rw-r--r--   0     1001      127       53 2024-05-09 23:38:24.000000 forust-0.4.8/scripts/run-python-tests.sh
+-rw-r--r--   0     1001      127     5647 2024-05-09 23:38:24.000000 forust-0.4.8/src/binning.rs
+-rw-r--r--   0     1001      127      248 2024-05-09 23:38:24.000000 forust-0.4.8/src/constraints.rs
+-rw-r--r--   0     1001      127    10051 2024-05-09 23:38:24.000000 forust-0.4.8/src/data.rs
+-rw-r--r--   0     1001      127      945 2024-05-09 23:38:24.000000 forust-0.4.8/src/errors.rs
+-rw-r--r--   0     1001      127    57204 2024-05-09 23:38:24.000000 forust-0.4.8/src/gradientbooster.rs
+-rw-r--r--   0     1001      127      881 2024-05-09 23:38:24.000000 forust-0.4.8/src/grower.rs
+-rw-r--r--   0     1001      127     9977 2024-05-09 23:38:24.000000 forust-0.4.8/src/histogram.rs
+-rw-r--r--   0     1001      127      384 2024-05-09 23:38:24.000000 forust-0.4.8/src/lib.rs
+-rw-r--r--   0     1001      127     8933 2024-05-09 23:38:24.000000 forust-0.4.8/src/metric.rs
+-rw-r--r--   0     1001      127     6863 2024-05-09 23:38:24.000000 forust-0.4.8/src/node.rs
+-rw-r--r--   0     1001      127     5956 2024-05-09 23:38:24.000000 forust-0.4.8/src/objective.rs
+-rw-r--r--   0     1001      127     4195 2024-05-09 23:38:24.000000 forust-0.4.8/src/partial_dependence.rs
+-rw-r--r--   0     1001      127     2923 2024-05-09 23:38:24.000000 forust-0.4.8/src/sampler.rs
+-rw-r--r--   0     1001      127     8072 2024-05-09 23:38:24.000000 forust-0.4.8/src/shapley.rs
+-rw-r--r--   0     1001      127    41163 2024-05-09 23:38:24.000000 forust-0.4.8/src/splitter.rs
+-rw-r--r--   0     1001      127    33600 2024-05-09 23:38:24.000000 forust-0.4.8/src/tree.rs
+-rw-r--r--   0     1001      127    35433 2024-05-09 23:38:24.000000 forust-0.4.8/src/utils.rs
+-rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 forust-0.4.8/py-forust/Cargo.toml
+-rw-r--r--   0     1001      127      685 2024-05-09 23:38:24.000000 forust-0.4.8/py-forust/.gitignore
+-rw-r--r--   0     1001      127     7350 2024-05-09 23:38:55.000000 forust-0.4.8/py-forust/README.md
+-rw-r--r--   0     1001      127     1634 2024-05-09 23:38:24.000000 forust-0.4.8/py-forust/docs/index.md
+-rw-r--r--   0     1001      127    56274 2024-05-09 23:38:24.000000 forust-0.4.8/py-forust/forust/__init__.py
+-rw-r--r--   0     1001      127     1870 2024-05-09 23:38:24.000000 forust-0.4.8/py-forust/forust/serialize.py
+-rw-r--r--   0     1001      127     1192 2024-05-09 23:38:24.000000 forust-0.4.8/py-forust/mkdocs.yml
+-rw-r--r--   0     1001      127    16405 2024-05-09 23:38:24.000000 forust-0.4.8/py-forust/src/lib.rs
+-rw-r--r--   0     1001      127    56331 2024-05-09 23:38:24.000000 forust-0.4.8/py-forust/tests/test_booster.py
+-rw-r--r--   0     1001      127     1318 2024-05-09 23:38:24.000000 forust-0.4.8/py-forust/tests/test_serailze.py
+-rw-r--r--   0     1001      127    15378 2024-05-09 23:39:40.000000 forust-0.4.8/py-forust/Cargo.lock
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 forust-0.4.8/pyproject.toml
+-rw-r--r--   0     1001      127    56274 2024-05-09 23:38:24.000000 forust-0.4.8/forust/__init__.py
+-rw-r--r--   0     1001      127     1870 2024-05-09 23:38:24.000000 forust-0.4.8/forust/serialize.py
+-rw-r--r--   0        0        0     8353 1970-01-01 00:00:00.000000 forust-0.4.8/PKG-INFO
```

### Comparing `forust-0.4.7/Cargo.toml` & `forust-0.4.8/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "forust-ml"
-version = "0.4.7"
+version = "0.4.8"
 edition = "2021"
 authors = [ "James Inlow <james.d.inlow@gmail.com>",]
 homepage = "https://github.com/jinlow/forust"
 description = "A lightweight gradient boosting implementation in Rust."
 license-file = "LICENSE"
 readme = "README.md"
 repository = "https://github.com/jinlow/forust"
```

### Comparing `forust-0.4.7/.github/workflows/CI.yml` & `forust-0.4.8/.github/workflows/CI.yml`

 * *Files 8% similar despite different names*

```diff
@@ -51,19 +51,19 @@
           path: dist
       - if: "startsWith(github.ref, 'refs/tags/')"
         name: Publish Wheels
         uses: PyO3/maturin-action@v1
         with:
           command: publish
           args: --username __token__ --password ${{ secrets.PYPI_TOKEN }} --interpreter python --skip-existing --manifest-path py-forust/Cargo.toml
-
+# "3.8", "3.9", "3.10",
   macos-build-test:
     strategy:
       matrix:
-        pyversion: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+        pyversion: ["3.11", "3.12"]
     runs-on: "macos-latest"
     steps:
       - uses: actions/checkout@v3
       - name: Install latests stable Rust
         uses: dtolnay/rust-toolchain@stable
         with:
           toolchain: stable
@@ -85,14 +85,69 @@
       - name: Build Wheels with maturin
         uses: PyO3/maturin-action@v1
         with:
           target: x86_64
           command: build
           args: --release --strip --interpreter python --manifest-path py-forust/Cargo.toml --out dist
       - name: Install wheel
+        run: cd py-forust; pip install --no-deps --force-reinstall -e .; cd ..
+      - name: Run Package Tests
+        run: |
+          pip install pytest pytest-cov 'black>=24.0.0,<25.0.0' ruff setuptools --upgrade
+          cd py-forust
+          ruff check .
+          black --check .
+          pytest --cov-fail-under=90 tests
+          cd ..
+      - name: Save Artifacts
+        uses: actions/upload-artifact@v3
+        with:
+          name: wheels
+          path: dist
+      - if: "startsWith(github.ref, 'refs/tags/')"
+        name: Publish Wheels
+        uses: PyO3/maturin-action@v1
+        with:
+          command: publish
+          target: x86_64
+          args: --username __token__ --password ${{ secrets.PYPI_TOKEN }} --interpreter python --skip-existing --manifest-path py-forust/Cargo.toml
+
+  macos-13-build-test:
+    strategy:
+      matrix:
+        pyversion: ["3.8", "3.9", "3.10"]
+    runs-on: "macos-13"
+    steps:
+      - uses: actions/checkout@v3
+      - name: Install latests stable Rust
+        uses: dtolnay/rust-toolchain@stable
+        with:
+          toolchain: stable
+      - uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.pyversion }}
+          architecture: x64
+      - name: Install deps
+        run: pip install numpy pandas seaborn xgboost=='1.6.1' scikit-learn toml
+      - run: |
+          cp README.md py-forust/README.md
+          cp LICENSE py-forust/LICENSE
+      - name: Update TOML
+        run: python scripts/remove-optional-deps.py
+      - name: Build test data
+        run: python scripts/make_resources.py
+      - name: Run tests
+        run: cargo test --verbose
+      - name: Build Wheels with maturin
+        uses: PyO3/maturin-action@v1
+        with:
+          target: x86_64
+          command: build
+          args: --release --strip --interpreter python --manifest-path py-forust/Cargo.toml --out dist
+      - name: Install wheel
         run: pip install forust --no-index --find-links dist --no-deps --force-reinstall
       - name: Run Package Tests
         run: |
           pip install pytest pytest-cov 'black>=24.0.0,<25.0.0' ruff setuptools --upgrade
           cd py-forust
           ruff check .
           black --check .
@@ -107,14 +162,15 @@
         name: Publish Wheels
         uses: PyO3/maturin-action@v1
         with:
           command: publish
           target: x86_64
           args: --username __token__ --password ${{ secrets.PYPI_TOKEN }} --interpreter python --skip-existing --manifest-path py-forust/Cargo.toml
 
+
   linux-build-test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         pyversion: ["3.8", "3.9", "3.10", "3.11", "3.12"]
         # target: [x86_64, i686]
     steps:
```

### Comparing `forust-0.4.7/.github/workflows/cargo-build-publish.yml` & `forust-0.4.8/.github/workflows/cargo-build-publish.yml`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/.github/workflows/docs.yml` & `forust-0.4.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/CONTRIBUTING.md` & `forust-0.4.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/LICENSE` & `forust-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/README.md` & `forust-0.4.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.4.7"
+forust-ml = "0.4.8"
 ```
 
 ## Usage
 
 For details on all of the methods and their respective parameters, see the [python api documentation](https://jinlow.github.io/forust/).
 
 The [`GradientBooster`](https://jinlow.github.io/forust/#forust.GradientBooster) class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
```

#### html2text {}

```diff
@@ -15,15 +15,15 @@
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Documentation
 Documentation for the python API can be found [here](https://jinlow.github.io/
 forust/). ## Installation The package can be installed directly from [pypi]
 (https://pypi.org/project/forust/). ```shell pip install forust ``` To use in a
 rust project add the following to your Cargo.toml file. ```toml forust-ml =
-"0.4.7" ``` ## Usage For details on all of the methods and their respective
+"0.4.8" ``` ## Usage For details on all of the methods and their respective
 parameters, see the [python api documentation](https://jinlow.github.io/forust/
 ). The [`GradientBooster`](https://jinlow.github.io/forust/
 #forust.GradientBooster) class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. ### Training and Predicting Once, the booster has
 been initialized, it can be fit on a provided dataset, and performance field.
 After fitting, the model can be used to predict on a dataset. In the case of
```

### Comparing `forust-0.4.7/benches/forust_benchmarks.rs` & `forust-0.4.8/benches/forust_benchmarks.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/resources/pdp_plot_age.png` & `forust-0.4.8/resources/pdp_plot_age.png`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/resources/pdp_plot_age_mono.png` & `forust-0.4.8/resources/pdp_plot_age_mono.png`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/resources/titanic.csv` & `forust-0.4.8/resources/titanic.csv`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/resources/tree-image-crop.png` & `forust-0.4.8/resources/tree-image-crop.png`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/rs-example.md` & `forust-0.4.8/rs-example.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## A Complete Rust Example
 
 To run this example, add the following code to your `Cargo.toml` file.
 ```toml
 [dependencies]
-forust-ml = "0.4.7"
+forust-ml = "0.4.8"
 polars = "0.28"
 reqwest = { version = "0.11", features = ["blocking"] }
 ```
 
 The following is a runable example using `polars` for data processing. The actual data manipulation can be performed with any tool, the only vital part, is the data be in column major format.
 ```rust
 use forust_ml::{GradientBooster, Matrix};
```

### Comparing `forust-0.4.7/scripts/make_resources.py` & `forust-0.4.8/scripts/make_resources.py`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/binning.rs` & `forust-0.4.8/src/binning.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/data.rs` & `forust-0.4.8/src/data.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/errors.rs` & `forust-0.4.8/src/errors.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/gradientbooster.rs` & `forust-0.4.8/src/gradientbooster.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/grower.rs` & `forust-0.4.8/src/grower.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/histogram.rs` & `forust-0.4.8/src/histogram.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/metric.rs` & `forust-0.4.8/src/metric.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/node.rs` & `forust-0.4.8/src/node.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/objective.rs` & `forust-0.4.8/src/objective.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/partial_dependence.rs` & `forust-0.4.8/src/partial_dependence.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/sampler.rs` & `forust-0.4.8/src/sampler.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/shapley.rs` & `forust-0.4.8/src/shapley.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/splitter.rs` & `forust-0.4.8/src/splitter.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/tree.rs` & `forust-0.4.8/src/tree.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/src/utils.rs` & `forust-0.4.8/src/utils.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/py-forust/.gitignore` & `forust-0.4.8/py-forust/.gitignore`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/py-forust/README.md` & `forust-0.4.8/py-forust/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.4.7"
+forust-ml = "0.4.8"
 ```
 
 ## Usage
 
 For details on all of the methods and their respective parameters, see the [python api documentation](https://jinlow.github.io/forust/).
 
 The [`GradientBooster`](https://jinlow.github.io/forust/#forust.GradientBooster) class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
```

#### html2text {}

```diff
@@ -15,15 +15,15 @@
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Documentation
 Documentation for the python API can be found [here](https://jinlow.github.io/
 forust/). ## Installation The package can be installed directly from [pypi]
 (https://pypi.org/project/forust/). ```shell pip install forust ``` To use in a
 rust project add the following to your Cargo.toml file. ```toml forust-ml =
-"0.4.7" ``` ## Usage For details on all of the methods and their respective
+"0.4.8" ``` ## Usage For details on all of the methods and their respective
 parameters, see the [python api documentation](https://jinlow.github.io/forust/
 ). The [`GradientBooster`](https://jinlow.github.io/forust/
 #forust.GradientBooster) class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. ### Training and Predicting Once, the booster has
 been initialized, it can be fit on a provided dataset, and performance field.
 After fitting, the model can be used to predict on a dataset. In the case of
```

### Comparing `forust-0.4.7/py-forust/docs/index.md` & `forust-0.4.8/py-forust/docs/index.md`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/py-forust/forust/__init__.py` & `forust-0.4.8/py-forust/forust/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,18 @@
         node_list.append(
             dataclasses.asdict(
                 Node._from_xgboost_node(xgb_node, feature_map=feature_map)
             )
         )
         if "leaf" not in xgb_node:
             buffer.extend(xgb_node["children"])
+    # We can't depend on the children to be in the "depth-wise" order, sometimes they
+    # will be built with lossguide, in which case the order will differ. Because of this,
+    # We need do tresort the list, by the node number...
+    node_list = sorted(node_list, key=lambda n: n["num"])
     # Ensure the nodeids all align with the nodes index
     for idx, node in enumerate(node_list):
         if idx != node["num"]:
             raise ValueError(
                 f"Nodes are unaligned for node {node['num']} at index {idx}"
             )
     return node_list
```

### Comparing `forust-0.4.7/py-forust/forust/serialize.py` & `forust-0.4.8/py-forust/forust/serialize.py`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/py-forust/mkdocs.yml` & `forust-0.4.8/py-forust/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/py-forust/src/lib.rs` & `forust-0.4.8/py-forust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/py-forust/tests/test_booster.py` & `forust-0.4.8/py-forust/tests/test_booster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1153,14 +1153,36 @@
     xmod_contribs_shapley = xmod.get_booster().predict(
         xgb.DMatrix(X), approx_contribs=False, pred_contribs=True
     )
     assert np.allclose(contribs_shapley, xmod_contribs_shapley, atol=0.00001)
     assert np.allclose(fmod_preds, xmod.predict(X, output_margin=True), atol=0.00001)
 
 
+@pytest.mark.parametrize("growth_policy", ["depthwise", "lossguide"])
+def test_from_xgboost(X_y, growth_policy):
+    X, y = X_y
+    X = X.astype(np.float32)
+    xmod = XGBClassifier(
+        n_estimators=200,
+        learning_rate=0.03,
+        max_depth=10,
+        objective="binary:logitraw",
+        eval_metric="auc",
+        tree_method="hist",
+        base_score=0.5,
+        growth_policy=growth_policy,
+    )
+    xmod.fit(X, y)
+
+    fmod = forust._from_xgboost_model(xmod)
+    assert np.allclose(
+        xmod.predict(X, output_margin=True), fmod.predict(X), atol=0.00001
+    )
+
+
 def test_missing_branch_with_contributions(X_y):
     X, y = X_y
     X = X
     fmod_miss_leaf = GradientBooster(
         iterations=100,
         learning_rate=0.3,
         max_depth=5,
```

### Comparing `forust-0.4.7/py-forust/tests/test_serailze.py` & `forust-0.4.8/py-forust/tests/test_serailze.py`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/py-forust/Cargo.lock` & `forust-0.4.8/py-forust/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 name = "arc-swap"
 version = "1.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "69f7f8c3906b62b754cd5326047894316021dcfe5a194c8ea52bdd94934a3457"
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -49,35 +49,35 @@
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "forust-ml"
-version = "0.4.7"
+version = "0.4.8"
 dependencies = [
  "log",
  "rand",
  "rayon",
  "serde",
  "serde_json",
  "thiserror",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -96,23 +96,23 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -150,17 +150,17 @@
  "num-integer",
  "num-traits",
  "rawpointer",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.46"
@@ -168,17 +168,17 @@
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "numpy"
 version = "0.20.0"
@@ -198,27 +198,27 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
@@ -233,24 +233,24 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-forust"
-version = "0.4.7"
+version = "0.4.8"
 dependencies = [
  "forust-ml",
  "ndarray",
  "numpy",
  "pyo3",
  "pyo3-log",
  "serde",
@@ -394,64 +394,64 @@
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -467,43 +467,43 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -522,61 +522,68 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "windows-targets"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `forust-0.4.7/pyproject.toml` & `forust-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/forust/__init__.py` & `forust-0.4.8/forust/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,18 @@
         node_list.append(
             dataclasses.asdict(
                 Node._from_xgboost_node(xgb_node, feature_map=feature_map)
             )
         )
         if "leaf" not in xgb_node:
             buffer.extend(xgb_node["children"])
+    # We can't depend on the children to be in the "depth-wise" order, sometimes they
+    # will be built with lossguide, in which case the order will differ. Because of this,
+    # We need do tresort the list, by the node number...
+    node_list = sorted(node_list, key=lambda n: n["num"])
     # Ensure the nodeids all align with the nodes index
     for idx, node in enumerate(node_list):
         if idx != node["num"]:
             raise ValueError(
                 f"Nodes are unaligned for node {node['num']} at index {idx}"
             )
     return node_list
```

### Comparing `forust-0.4.7/forust/serialize.py` & `forust-0.4.8/forust/serialize.py`

 * *Files identical despite different names*

### Comparing `forust-0.4.7/PKG-INFO` & `forust-0.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: forust
-Version: 0.4.7
+Version: 0.4.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy >=1.21
 Requires-Dist: pandas >=1.3
 Requires-Dist: maturin ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
@@ -50,15 +50,15 @@
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.4.7"
+forust-ml = "0.4.8"
 ```
 
 ## Usage
 
 For details on all of the methods and their respective parameters, see the [python api documentation](https://jinlow.github.io/forust/).
 
 The [`GradientBooster`](https://jinlow.github.io/forust/#forust.GradientBooster) class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: forust Version: 0.4.7 Classifier: Programming
+Metadata-Version: 2.3 Name: forust Version: 0.4.8 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy >=1.21 Requires-Dist: pandas >=1.3 Requires-Dist: maturin
 ; extra == 'dev' Requires-Dist: pytest ; extra == 'dev' Requires-Dist: seaborn
 ; extra == 'dev' Requires-Dist: xgboost ==1.6.1 ; extra == 'dev' Requires-Dist:
 scikit-learn ; extra == 'dev' Requires-Dist: mkdocs-material ==9.* ; extra ==
 'dev' Requires-Dist: mkdocstrings[python] ==0.22.0 ; extra == 'dev' Requires-
@@ -28,15 +28,15 @@
 to the algorithm in a smaller simpler codebase. All of the rust code for the
 package can be found in the [src](src/) directory, while all of the python
 wrapper code is in the [py-forust](py-forust/) directory. ## Documentation
 Documentation for the python API can be found [here](https://jinlow.github.io/
 forust/). ## Installation The package can be installed directly from [pypi]
 (https://pypi.org/project/forust/). ```shell pip install forust ``` To use in a
 rust project add the following to your Cargo.toml file. ```toml forust-ml =
-"0.4.7" ``` ## Usage For details on all of the methods and their respective
+"0.4.8" ``` ## Usage For details on all of the methods and their respective
 parameters, see the [python api documentation](https://jinlow.github.io/forust/
 ). The [`GradientBooster`](https://jinlow.github.io/forust/
 #forust.GradientBooster) class is currently the only public facing class in the
 package, and can be used to train gradient boosted decision tree ensembles with
 multiple objective functions. ### Training and Predicting Once, the booster has
 been initialized, it can be fit on a provided dataset, and performance field.
 After fitting, the model can be used to predict on a dataset. In the case of
```

