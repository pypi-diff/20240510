# Comparing `tmp/nima-0.9.0.tar.gz` & `tmp/nima-0.9.1.tar.gz`

## Comparing `nima-0.9.0.tar` & `nima-0.9.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 nima-0.9.0/.codespellrc
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nima-0.9.0/.darglint
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 nima-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nima-0.9.0/.readthedocs.yml
--rw-r--r--   0        0        0    22775 2020-02-02 00:00:00.000000 nima-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 nima-0.9.0/bandit.yml
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nima-0.9.0/.github/dependabot.yml
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 nima-0.9.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nima-0.9.0/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 nima-0.9.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nima-0.9.0/docs/Makefile
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 nima-0.9.0/docs/click.rst
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 nima-0.9.0/docs/conf.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 nima-0.9.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 nima-0.9.0/docs/make.bat
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 nima-0.9.0/docs/_static/.gitignore
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nima-0.9.0/docs/_static/custom.css
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nima-0.9.0/docs/api/api.rst
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nima-0.9.0/docs/api/generat.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 nima-0.9.0/docs/api/nima.rst
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 nima-0.9.0/docs/references/contributing.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nima-0.9.0/docs/references/description.rst
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 nima-0.9.0/docs/references/development.rst
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 nima-0.9.0/docs/references/nima.rst
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nima-0.9.0/docs/references/references.rst
--rw-r--r--   0        0        0    25513 2020-02-02 00:00:00.000000 nima-0.9.0/docs/tutorials/dev_xr_hvplot_holoviews.ipynb
--rw-r--r--   0        0        0    31723 2020-02-02 00:00:00.000000 nima-0.9.0/docs/tutorials/flat_bg_dask.ipynb
--rw-r--r--   0        0        0    15423 2020-02-02 00:00:00.000000 nima-0.9.0/docs/tutorials/ratioing.ipynb
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nima-0.9.0/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 nima-0.9.0/docs/tutorials/usage.ipynb
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nima-0.9.0/src/nima/__init__.py
--rw-r--r--   0        0        0    18282 2020-02-02 00:00:00.000000 nima-0.9.0/src/nima/__main__.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 nima-0.9.0/src/nima/generat.py
--rw-r--r--   0        0        0    33966 2020-02-02 00:00:00.000000 nima-0.9.0/src/nima/nima.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nima-0.9.0/src/nima/py.typed
--rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 nima-0.9.0/src/nima/utils.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nima-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nima-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 nima-0.9.0/tests/test_cli.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 nima-0.9.0/tests/test_generat.py
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 nima-0.9.0/tests/test_nima.py
--rw-r--r--   0        0        0  6538791 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/1b_c16_15.tif
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/test_flat0.tif
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/test_flat1.tif
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/test_flat2.tif
--rw-r--r--   0        0        0   746328 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15_dim.png
--rw-r--r--   0        0        0   101490 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15_meas.png
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/test_flat.tif
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/test_flat_gaussnorm.tif
--rw-r--r--   0        0        0   616620 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15/bg-C-li_adaptive.pdf
--rw-r--r--   0        0        0   469663 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15/bg-G-li_adaptive.pdf
--rw-r--r--   0        0        0   626676 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15/bg-R-li_adaptive.pdf
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15/bg.csv
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15/label1.csv
--rw-r--r--   0        0        0   179299 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15/label1_rcl.tif
--rw-r--r--   0        0        0   186357 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15/label1_rpH.tif
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15/label2.csv
--rw-r--r--   0        0        0    96791 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15/label2_rcl.tif
--rw-r--r--   0        0        0   114272 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15/label2_rpH.tif
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15/label3.csv
--rw-r--r--   0        0        0    54510 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15/label3_rcl.tif
--rw-r--r--   0        0        0    50655 2020-02-02 00:00:00.000000 nima-0.9.0/tests/data/output/1b_c16_15/label3_rpH.tif
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 nima-0.9.0/.gitignore
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 nima-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 nima-0.9.0/README.md
--rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 nima-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 nima-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 nima-0.9.1/.codespellrc
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nima-0.9.1/.darglint
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 nima-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nima-0.9.1/.readthedocs.yml
+-rw-r--r--   0        0        0    22927 2020-02-02 00:00:00.000000 nima-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 nima-0.9.1/bandit.yml
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nima-0.9.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 nima-0.9.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nima-0.9.1/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 nima-0.9.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nima-0.9.1/docs/Makefile
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 nima-0.9.1/docs/click.rst
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 nima-0.9.1/docs/conf.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 nima-0.9.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 nima-0.9.1/docs/make.bat
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 nima-0.9.1/docs/_static/.gitignore
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nima-0.9.1/docs/_static/custom.css
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nima-0.9.1/docs/api/api.rst
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nima-0.9.1/docs/api/generat.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 nima-0.9.1/docs/api/nima.rst
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 nima-0.9.1/docs/references/contributing.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 nima-0.9.1/docs/references/description.rst
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 nima-0.9.1/docs/references/development.rst
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 nima-0.9.1/docs/references/nima.rst
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nima-0.9.1/docs/references/references.rst
+-rw-r--r--   0        0        0    25513 2020-02-02 00:00:00.000000 nima-0.9.1/docs/tutorials/dev_xr_hvplot_holoviews.ipynb
+-rw-r--r--   0        0        0    31723 2020-02-02 00:00:00.000000 nima-0.9.1/docs/tutorials/flat_bg_dask.ipynb
+-rw-r--r--   0        0        0    15423 2020-02-02 00:00:00.000000 nima-0.9.1/docs/tutorials/ratioing.ipynb
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nima-0.9.1/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0    17153 2020-02-02 00:00:00.000000 nima-0.9.1/docs/tutorials/usage.ipynb
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 nima-0.9.1/src/nima/__init__.py
+-rw-r--r--   0        0        0    18282 2020-02-02 00:00:00.000000 nima-0.9.1/src/nima/__main__.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 nima-0.9.1/src/nima/generat.py
+-rw-r--r--   0        0        0    33966 2020-02-02 00:00:00.000000 nima-0.9.1/src/nima/nima.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nima-0.9.1/src/nima/py.typed
+-rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 nima-0.9.1/src/nima/utils.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nima-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 nima-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 nima-0.9.1/tests/test_cli.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 nima-0.9.1/tests/test_generat.py
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 nima-0.9.1/tests/test_nima.py
+-rw-r--r--   0        0        0  6538791 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/1b_c16_15.tif
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/test_flat0.tif
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/test_flat1.tif
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/test_flat2.tif
+-rw-r--r--   0        0        0   746328 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15_dim.png
+-rw-r--r--   0        0        0   101490 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15_meas.png
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/test_flat.tif
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/test_flat_gaussnorm.tif
+-rw-r--r--   0        0        0   616620 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15/bg-C-li_adaptive.pdf
+-rw-r--r--   0        0        0   469663 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15/bg-G-li_adaptive.pdf
+-rw-r--r--   0        0        0   626676 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15/bg-R-li_adaptive.pdf
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15/bg.csv
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15/label1.csv
+-rw-r--r--   0        0        0   179299 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15/label1_rcl.tif
+-rw-r--r--   0        0        0   186357 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15/label1_rpH.tif
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15/label2.csv
+-rw-r--r--   0        0        0    96791 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15/label2_rcl.tif
+-rw-r--r--   0        0        0   114272 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15/label2_rpH.tif
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15/label3.csv
+-rw-r--r--   0        0        0    54510 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15/label3_rcl.tif
+-rw-r--r--   0        0        0    50655 2020-02-02 00:00:00.000000 nima-0.9.1/tests/data/output/1b_c16_15/label3_rpH.tif
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 nima-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 nima-0.9.1/LICENSE.txt
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 nima-0.9.1/README.md
+-rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 nima-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 nima-0.9.1/PKG-INFO
```

### Comparing `nima-0.9.0/.pre-commit-config.yaml` & `nima-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/CHANGELOG.md` & `nima-0.9.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## v0.9.1 (2024-03-28)
+
+### Fix
+
+- **ci**: Add codecov token
+
+### Build
+
+- **deps-dev**: update ipykernel requirement from <=6.29.3 to <=6.29.4 (#512)
+
 ## v0.9.0 (2024-03-28)
 
 ### Feat
 
 - Add utils and more temporary tutorials
 
 ### Fix
```

### Comparing `nima-0.9.0/.github/workflows/ci.yml` & `nima-0.9.1/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,16 @@
         run: |
           coverage run -p -m pytest
           coverage combine
           coverage report
           coverage xml
       - name: Upload coverage report
         uses: codecov/codecov-action@v4.1.1
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
 
   testpypi:
     needs: [pre-commit, checks, typeguard, tests]
     runs-on: ubuntu-latest
     if: "startsWith(github.event.head_commit.message, 'bump:')"
     outputs:
       version: ${{ steps.version.outputs.ver }}
```

### Comparing `nima-0.9.0/.github/workflows/docs.yml` & `nima-0.9.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/docs/Makefile` & `nima-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/docs/conf.py` & `nima-0.9.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 sys.path.insert(0, str(Path("../..").resolve()))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "nima"
-release = "0.9.0"
+release = "0.9.1"
 author = "Daniele Arosio"
 copyright = f"2023, {author}"  # noqa A001
 html_static_path = ["_static"]
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `nima-0.9.0/docs/index.rst` & `nima-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/docs/make.bat` & `nima-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/docs/references/contributing.rst` & `nima-0.9.1/docs/references/contributing.rst`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/docs/references/development.rst` & `nima-0.9.1/docs/references/development.rst`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/docs/tutorials/dev_xr_hvplot_holoviews.ipynb` & `nima-0.9.1/docs/tutorials/dev_xr_hvplot_holoviews.ipynb`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/docs/tutorials/flat_bg_dask.ipynb` & `nima-0.9.1/docs/tutorials/flat_bg_dask.ipynb`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/docs/tutorials/ratioing.ipynb` & `nima-0.9.1/docs/tutorials/ratioing.ipynb`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/docs/tutorials/usage.ipynb` & `nima-0.9.1/docs/tutorials/usage.ipynb`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/src/nima/__main__.py` & `nima-0.9.1/src/nima/__main__.py`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/src/nima/generat.py` & `nima-0.9.1/src/nima/generat.py`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/src/nima/nima.py` & `nima-0.9.1/src/nima/nima.py`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/src/nima/utils.py` & `nima-0.9.1/src/nima/utils.py`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/test_cli.py` & `nima-0.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/test_generat.py` & `nima-0.9.1/tests/test_generat.py`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/test_nima.py` & `nima-0.9.1/tests/test_nima.py`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/1b_c16_15.tif` & `nima-0.9.1/tests/data/1b_c16_15.tif`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/output/1b_c16_15_dim.png` & `nima-0.9.1/tests/data/output/1b_c16_15_dim.png`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/output/1b_c16_15_meas.png` & `nima-0.9.1/tests/data/output/1b_c16_15_meas.png`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/output/1b_c16_15/bg-C-li_adaptive.pdf` & `nima-0.9.1/tests/data/output/1b_c16_15/bg-C-li_adaptive.pdf`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/output/1b_c16_15/bg-G-li_adaptive.pdf` & `nima-0.9.1/tests/data/output/1b_c16_15/bg-G-li_adaptive.pdf`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/output/1b_c16_15/bg-R-li_adaptive.pdf` & `nima-0.9.1/tests/data/output/1b_c16_15/bg-R-li_adaptive.pdf`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/output/1b_c16_15/label1.csv` & `nima-0.9.1/tests/data/output/1b_c16_15/label1.csv`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/output/1b_c16_15/label1_rcl.tif` & `nima-0.9.1/tests/data/output/1b_c16_15/label1_rcl.tif`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/output/1b_c16_15/label1_rpH.tif` & `nima-0.9.1/tests/data/output/1b_c16_15/label1_rpH.tif`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/output/1b_c16_15/label2.csv` & `nima-0.9.1/tests/data/output/1b_c16_15/label2.csv`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/output/1b_c16_15/label2_rcl.tif` & `nima-0.9.1/tests/data/output/1b_c16_15/label2_rcl.tif`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/output/1b_c16_15/label2_rpH.tif` & `nima-0.9.1/tests/data/output/1b_c16_15/label2_rpH.tif`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/output/1b_c16_15/label3_rcl.tif` & `nima-0.9.1/tests/data/output/1b_c16_15/label3_rcl.tif`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/tests/data/output/1b_c16_15/label3_rpH.tif` & `nima-0.9.1/tests/data/output/1b_c16_15/label3_rpH.tif`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/.gitignore` & `nima-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/LICENSE.txt` & `nima-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nima-0.9.0/README.md` & `nima-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![CI](https://github.com/darosio/nima/actions/workflows/ci.yml/badge.svg)](https://github.com/darosio/nima/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/darosio/nima/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/nima)
 [![RtD](https://readthedocs.org/projects/nima/badge/)](https://nima.readthedocs.io/)
 
 A library and a command-line interface (CLI) designed to assist with image
 analysis tasks using scipy.ndimage and scikit-image.
 
-- Version: “0.9.0”
+- Version: “0.9.1”
 
 ## Features
 
 - Bias and Flat Correction
 - Automatic Cell Segmentation
 - Multi-Ratio Ratiometric Imaging, enabling users to analyze multiple ratios
   with ease.
```

### Comparing `nima-0.9.0/pyproject.toml` & `nima-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -33,21 +33,21 @@
 description = "Numerical IMage Analyses."
 keywords = ["ClopHensor", "ratio imaging", "image analysis", "chloride", "pH"]
 license = "BSD-3-Clause"
 license-files = {paths = ["LICENSE.txt"]}
 name = "nima"
 readme = "README.md"
 requires-python = ">=3.10,<3.12"
-version = "0.9.0"
+version = "0.9.1"
 
 [project.optional-dependencies]
 dev = [
   "commitizen <= 3.20.0",
   "pre-commit <= 3.7.0",
-  "ipykernel <=6.29.3",
+  "ipykernel <=6.29.4",
   "ruff <= 0.3.4",
   "pylsp-mypy",
   "jupyter",
   "jupyterlab",
   "python-lsp-ruff"
 ]
 docs = [
@@ -106,15 +106,15 @@
 '''
 line-length = 88
 skip-string-normalization = false
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.9.0"
+version = "0.9.1"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
   "README.md:Version"
 ]
 
 [tool.commitizen.customize]
```

### Comparing `nima-0.9.0/PKG-INFO` & `nima-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nima
-Version: 0.9.0
+Version: 0.9.1
 Summary: Numerical IMage Analyses.
 Project-URL: homepage, https://github.com/darosio/nima/
 Project-URL: repository, https://github.com/darosio/nima/
 Author-email: daniele arosio <daniele.arosio@cnr.it>
 License-Expression: BSD-3-Clause
 License-File: LICENSE.txt
 Keywords: ClopHensor,chloride,image analysis,pH,ratio imaging
@@ -27,15 +27,15 @@
 Requires-Dist: scikit-image<=0.22.0
 Requires-Dist: scipy<=1.12.0
 Requires-Dist: sigfig<=1.3.3
 Requires-Dist: tifffile<=2024.2.12
 Requires-Dist: zarr<=2.17.1
 Provides-Extra: dev
 Requires-Dist: commitizen<=3.20.0; extra == 'dev'
-Requires-Dist: ipykernel<=6.29.3; extra == 'dev'
+Requires-Dist: ipykernel<=6.29.4; extra == 'dev'
 Requires-Dist: jupyter; extra == 'dev'
 Requires-Dist: jupyterlab; extra == 'dev'
 Requires-Dist: pre-commit<=3.7.0; extra == 'dev'
 Requires-Dist: pylsp-mypy; extra == 'dev'
 Requires-Dist: python-lsp-ruff; extra == 'dev'
 Requires-Dist: ruff<=0.3.4; extra == 'dev'
 Provides-Extra: docs
@@ -74,15 +74,15 @@
 [![CI](https://github.com/darosio/nima/actions/workflows/ci.yml/badge.svg)](https://github.com/darosio/nima/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/darosio/nima/branch/main/graph/badge.svg?token=OU6F9VFUQ6)](https://codecov.io/gh/darosio/nima)
 [![RtD](https://readthedocs.org/projects/nima/badge/)](https://nima.readthedocs.io/)
 
 A library and a command-line interface (CLI) designed to assist with image
 analysis tasks using scipy.ndimage and scikit-image.
 
-- Version: “0.9.0”
+- Version: “0.9.1”
 
 ## Features
 
 - Bias and Flat Correction
 - Automatic Cell Segmentation
 - Multi-Ratio Ratiometric Imaging, enabling users to analyze multiple ratios
   with ease.
```

