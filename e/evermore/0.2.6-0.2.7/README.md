# Comparing `tmp/evermore-0.2.6.tar.gz` & `tmp/evermore-0.2.7.tar.gz`

## Comparing `evermore-0.2.6.tar` & `evermore-0.2.7.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 evermore-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 evermore-0.2.6/.readthedocs.yaml
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 evermore-0.2.6/CONTRIBUTING.md
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 evermore-0.2.6/pixi.toml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 evermore-0.2.6/.github/dependabot.yml
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 evermore-0.2.6/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 evermore-0.2.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0    14463 2020-02-02 00:00:00.000000 evermore-0.2.6/assets/favicon.png
--rw-r--r--   0        0        0    19246 2020-02-02 00:00:00.000000 evermore-0.2.6/assets/logo.png
--rw-r--r--   0        0        0    85492 2020-02-02 00:00:00.000000 evermore-0.2.6/assets/logo_vertical.png
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/Makefile
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/binned_likelihood.md
--rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/building_blocks.md
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/conf.py
--rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/evermore_for_ATLAS.md
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/evermore_for_CMS.md
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/index.md
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/tips_and_tricks.md
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/_static/styles_sphinx_book_theme.css
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/effect.md
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/index.md
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/loss.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/modifier.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/parameter.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/pdf.md
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/util.md
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/bin_by_bin_uncs.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/dnn_weights_constraint.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/grad_nll.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/model.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/nll_fit.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/nll_profiling.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/serialize_model.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/toy_generation.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/unbinned_model.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/__init__.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/custom_types.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/effect.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/loss.py
--rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/modifier.py
--rw-r--r--   0        0        0     9861 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/parameter.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/pdf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/py.typed
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/staterror.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/util.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 evermore-0.2.6/tests/test_effect.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 evermore-0.2.6/tests/test_loss.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 evermore-0.2.6/tests/test_modifier.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 evermore-0.2.6/tests/test_parameter.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 evermore-0.2.6/tests/test_pdf.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 evermore-0.2.6/tests/test_util.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 evermore-0.2.6/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 evermore-0.2.6/LICENSE
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 evermore-0.2.6/README.md
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 evermore-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 evermore-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 evermore-0.2.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 evermore-0.2.7/.readthedocs.yaml
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 evermore-0.2.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 evermore-0.2.7/pixi.toml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 evermore-0.2.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 evermore-0.2.7/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 evermore-0.2.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    14463 2020-02-02 00:00:00.000000 evermore-0.2.7/assets/favicon.png
+-rw-r--r--   0        0        0    19246 2020-02-02 00:00:00.000000 evermore-0.2.7/assets/logo.png
+-rw-r--r--   0        0        0    85492 2020-02-02 00:00:00.000000 evermore-0.2.7/assets/logo_vertical.png
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/Makefile
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/binned_likelihood.md
+-rw-r--r--   0        0        0     9788 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/building_blocks.md
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/conf.py
+-rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/evermore_for_ATLAS.md
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/evermore_for_CMS.md
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/index.md
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/tips_and_tricks.md
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/_static/styles_sphinx_book_theme.css
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/api/effect.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/api/index.md
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/api/loss.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/api/modifier.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/api/parameter.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/api/pdf.md
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 evermore-0.2.7/docs/api/util.md
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 evermore-0.2.7/examples/bin_by_bin_uncs.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 evermore-0.2.7/examples/dnn_weights_constraint.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 evermore-0.2.7/examples/grad_nll.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 evermore-0.2.7/examples/model.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 evermore-0.2.7/examples/nll_fit.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 evermore-0.2.7/examples/nll_profiling.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 evermore-0.2.7/examples/serialize_model.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 evermore-0.2.7/examples/toy_generation.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 evermore-0.2.7/examples/unbinned_model.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 evermore-0.2.7/src/evermore/__init__.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 evermore-0.2.7/src/evermore/custom_types.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 evermore-0.2.7/src/evermore/effect.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 evermore-0.2.7/src/evermore/loss.py
+-rw-r--r--   0        0        0    12840 2020-02-02 00:00:00.000000 evermore-0.2.7/src/evermore/modifier.py
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 evermore-0.2.7/src/evermore/parameter.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 evermore-0.2.7/src/evermore/pdf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 evermore-0.2.7/src/evermore/py.typed
+-rw-r--r--   0        0        0     5724 2020-02-02 00:00:00.000000 evermore-0.2.7/src/evermore/staterror.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 evermore-0.2.7/src/evermore/util.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 evermore-0.2.7/src/evermore/visualization.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 evermore-0.2.7/tests/test_effect.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 evermore-0.2.7/tests/test_loss.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 evermore-0.2.7/tests/test_modifier.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 evermore-0.2.7/tests/test_parameter.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 evermore-0.2.7/tests/test_pdf.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 evermore-0.2.7/tests/test_util.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 evermore-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 evermore-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 evermore-0.2.7/README.md
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 evermore-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 evermore-0.2.7/PKG-INFO
```

### Comparing `evermore-0.2.6/.pre-commit-config.yaml` & `evermore-0.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/.readthedocs.yaml` & `evermore-0.2.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/CONTRIBUTING.md` & `evermore-0.2.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/pixi.toml` & `evermore-0.2.7/pixi.toml`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 [host-dependencies]
 pip = "*"
 sphinx = "*"
 sphinx-copybutton = "*"
 sphinx-book-theme = "*"
 sphinx-design = "*"
 sphinx-togglebutton = "*"
+myst-nb = "*"
+
+[pypi-dependencies]
+penzai = "*"
 
 [tasks]
 postinstall = "pip install -e '.[dev]' && pip install pre-commit && pre-commit install"
 test = "pytest"
 lint = "ruff check . --fix --show-fixes"
 checkall = "pre-commit run --all-files"
-builddocs = "sphinx-build -M html ./docs ./build -W --keep-going"
+builddocs = "rm -rf build/ && sphinx-build -M html ./docs ./build -W --keep-going"
```

### Comparing `evermore-0.2.6/.github/workflows/cd.yml` & `evermore-0.2.7/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/.github/workflows/ci.yml` & `evermore-0.2.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/assets/favicon.png` & `evermore-0.2.7/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/assets/logo.png` & `evermore-0.2.7/assets/logo.png`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/assets/logo_vertical.png` & `evermore-0.2.7/assets/logo_vertical.png`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/docs/Makefile` & `evermore-0.2.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/docs/binned_likelihood.md` & `evermore-0.2.7/docs/binned_likelihood.md`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/docs/building_blocks.md` & `evermore-0.2.7/docs/building_blocks.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+---
+jupytext:
+  formats: md:myst
+  text_representation:
+    extension: .md
+    format_name: myst
+kernelspec:
+  display_name: Python 3
+  language: python
+  name: python3
+---
+
 (building-blocks)=
 # Building Blocks
 
 ## Parameter
 
 A parameter {math}`\phi` (see Eq.{eq}`likelihood`) is defined in evermore by `evm.Parameter`.
 It holds a `value` which holds a single value or an array of values that can be optimized during a fit.
@@ -113,34 +125,20 @@
 :::{admonition} Inspect `evm.Parameters` with `penzai`
 :class: tip dropdown
 
 Inspect a (PyTree of) `evm.Parameters` with [`penzai`'s treescope](https://penzai.readthedocs.io/en/stable/notebooks/treescope_prettyprinting.html) visualization in IPython or Colab notebooks.
 You can even add custom visualizers, such as:
 
 ```{code-block} python
-from penzai import pz
 import evermore as evm
-import plotly.express as px
 
 
 tree = {"a": evm.NormalParameter(), "b": evm.NormalParameter()}
 
-# custom plotly visualization of prior PDF
-def plot_prior_pdf(value, path):
-    if isinstance(value, evm.Parameter) and isinstance(value.prior, evm.custom_types.PDFLike):
-        x = jnp.arange(-3, 3, 0.1)
-        return pz.ts.IPythonVisualization(
-            px.bar(
-                x=x, y=jnp.exp(value.prior.log_prob(x)),
-                width=400, height=200
-            ).update_layout(margin=dict(l=20, r=20, t=20, b=20))
-        )
-
-with pz.ts.active_autovisualizer.set_scoped(plot_prior_pdf):
-    pz.ts.display(tree)
+evm.visualization.display(tree)
 ```
 :::
 
 ## Effect
 
 Effects describe how data ({math}`d`), i.e., histogram bins, are varied as a function of `evm.Parameters` ({math}`\phi`).
 They return multiplicative ({math}`\alpha`) and additive ({math}`\Delta`) variations that are applied to the data as follows:
@@ -267,25 +265,30 @@
     # apply the modifier
     modify(jnp.array([10, 20, 30]))
     # -> Array([10.336512, 20.6, 30.936512], dtype=float32)
     ```
 
 Multiple modifiers should be combined using `evm.modifier.Compose` or the `@` operator:
 
-```{code-block} python
+```{code-cell} ipython3
+import jax
 import jax.numpy as jnp
 import evermore as evm
 
 
+jax.config.update("jax_enable_x64", True)
+
 param = evm.NormalParameter(value=0.1)
 
 modifier1 = param.morphing(
     up_template=[12, 23, 35],
     down_template=[9, 17, 26],
 )
 
 modifier2 = param.scale_log(up=1.1, down=0.9)
 
 # apply the composed modifier
-(modifier1 @ modifier2)(jnp.array([10, 20, 30])
+(modifier1 @ modifier2)(jnp.array([10, 20, 30]))
 # -> Array([10.259877, 20.500944, 30.760822], dtype=float32)
+
+evm.visualization.display(modifier1 @ modifier2)
 ```
```

### Comparing `evermore-0.2.6/docs/conf.py` & `evermore-0.2.7/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     "use_edit_page_button": True,
 }
 html_context = {"default_mode": "light"}
 html_logo = "../assets/favicon.png"
 html_favicon = "../assets/favicon.png"
 
 extensions = [
-    "myst_parser",
+    "myst_nb",
+    # "myst_parser",
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
     "sphinx.ext.autosectionlabel",
     "sphinx_copybutton",
```

### Comparing `evermore-0.2.6/docs/evermore_for_ATLAS.md` & `evermore-0.2.7/docs/evermore_for_ATLAS.md`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/docs/evermore_for_CMS.md` & `evermore-0.2.7/docs/evermore_for_CMS.md`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/docs/index.md` & `evermore-0.2.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/docs/tips_and_tricks.md` & `evermore-0.2.7/docs/tips_and_tricks.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,63 @@
+---
+jupytext:
+  formats: md:myst
+  text_representation:
+    extension: .md
+    format_name: myst
+kernelspec:
+  display_name: Python 3
+  language: python
+  name: python3
+---
+
+
 # Tips and Tricks
 
 Here are some advanced tips and tricks.
 
 
+## penzai Visualization
+
+Use `penzai` to visualize evermore components!
+
+```{code-cell} ipython3
+import jax
+import jax.numpy as jnp
+import evermore as evm
+import equinox as eqx
+
+jax.config.update("jax_enable_x64", True)
+
+
+mu = evm.Parameter(value=1.1)
+sigma1 = evm.NormalParameter(value=0.1)
+sigma2 = evm.NormalParameter(value=0.2)
+
+hist = jnp.array([10, 20, 30])
+
+
+mu_mod = mu.scale(offset=0, slope=1)
+sigma1_mod = sigma1.scale_log(up=1.1, down=0.9)
+sigma2_mod = sigma2.scale_log(up=1.05, down=0.95)
+composition = evm.modifier.Compose(
+    mu_mod,
+    sigma1_mod,
+    evm.modifier.Where(hist < 15, sigma2_mod, sigma1_mod),
+)
+composition = evm.modifier.Compose(
+    composition,
+    evm.Modifier(parameter=sigma1, effect=evm.effect.AsymmetricExponential(up=1.2, down=0.8)),
+)
+
+evm.visualization.display(composition)
+```
+
+
+
 ## Parameter Partitioning
 
 For optimization it is necessary to differentiate only against meaningful leaves of the PyTree of `evm.Parameters`.
 By default JAX would differentiate w.r.t. every non-static leaf of a `evm.Parameter`, including the prior PDF and its bounds.
 Gradients are typically only wanted w.r.t. the `.value` attribute of the `evm.Parameters`. This is solved by splitting
 the PyTree of `evm.Parameters` into a differentiable and a non-differentiable part, and then defining the loss function
 w.r.t. both parts. Gradient calculation is performed only w.r.t. the differentiable arguement, see:
@@ -43,43 +94,27 @@
 
 
 ## JAX Transformations
 
 Evert component of evermore is compatible with JAX transformations. That means you can `jax.jit`, `jax.vmap`, ... _everything_.
 You can e.g. sample the parameter values multiple times vectorized from its prior PDF:
 
-```{code-block} python
+```{code-cell} ipython3
 import jax
 import evermore as evm
 
 
 params = {"a": evm.NormalParameter(), "b": evm.NormalParameter()}
 
 rng_key = jax.random.key(0)
 rng_keys = jax.random.split(rng_key, 100)
 
 vec_sample = jax.vmap(evm.parameter.sample, in_axes=(None, 0))
 
-print(vec_sample(params, rng_keys))
-# {'a': NormalParameter(
-#   value=f32[100,1],
-#   name=None,
-#   lower=f32[100,1],
-#   upper=f32[100,1],
-#   prior=Normal(mean=f32[100,1], width=f32[100,1]),
-#   frozen=False,
-# ),
-#  'b': NormalParameter(
-#   value=f32[100,1],
-#   name=None,
-#   lower=f32[100,1],
-#   upper=f32[100,1],
-#   prior=Normal(mean=f32[100,1], width=f32[100,1]),
-#   frozen=False,
-# )}
+evm.visualization.display(vec_sample(params, rng_keys))
 ```
 
 Many minimizers from the JAX ecosystem are e.g. batchable (`optax`, `optimistix`), which allows you vectorize _full fits_, e.g., for embarrassingly parallel likleihood profiles.
 
 ## Visualize the Computational Graph
 
 You can visualize the computational graph of a JAX computation by:
```

### Comparing `evermore-0.2.6/examples/bin_by_bin_uncs.py` & `evermore-0.2.7/examples/bin_by_bin_uncs.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,23 +34,24 @@
         expectations["bkg2"] = bkg2_mcstat_mod(hists["bkg2"])
 
         # return the modified expectations
         return expectations
 
 
 hists = {
-    "signal": jnp.array([3]),
-    "bkg1": jnp.array([10]),
-    "bkg2": jnp.array([20]),
+    "signal": jnp.array([3.0]),
+    "bkg1": jnp.array([10.0]),
+    "bkg2": jnp.array([20.0]),
 }
 histsw2 = {
-    "signal": jnp.array([5]),
-    "bkg1": jnp.array([11]),
-    "bkg2": jnp.array([25]),
+    "signal": jnp.array([5.0]),
+    "bkg1": jnp.array([11.0]),
+    "bkg2": jnp.array([25.0]),
 }
+observation = jnp.array([34.0])
 
 model = SPlusBModel(hists, histsw2)
 
 # test the model
 expectations = model(hists)
```

### Comparing `evermore-0.2.6/examples/dnn_weights_constraint.py` & `evermore-0.2.7/examples/dnn_weights_constraint.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/examples/grad_nll.py` & `evermore-0.2.7/examples/grad_nll.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/examples/model.py` & `evermore-0.2.7/examples/model.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/examples/nll_fit.py` & `evermore-0.2.7/examples/nll_fit.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/examples/nll_profiling.py` & `evermore-0.2.7/examples/nll_profiling.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/examples/toy_generation.py` & `evermore-0.2.7/examples/toy_generation.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/examples/unbinned_model.py` & `evermore-0.2.7/examples/unbinned_model.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/src/evermore/__init__.py` & `evermore-0.2.7/src/evermore/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 __author__ = "Peter Fackeldey"
 __email__ = "peter.fackeldey@rwth-aachen.de"
 __copyright__ = "Copyright 2023, Peter Fackeldey"
 __credits__ = ["Peter Fackeldey"]
 __contact__ = "https://github.com/pfackeldey/evermore"
 __license__ = "BSD-3-Clause"
 __status__ = "Development"
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 
 
 # expose public API
 
 __all__ = [
     "__version__",
     "effect",
     "loss",
     "parameter",
     "pdf",
     "util",
     "modifier",
     "staterror",
+    "visualization",
     # explicitely expose some classes
     "Parameter",
     "NormalParameter",
     "Modifier",
 ]
 
 
@@ -40,13 +41,14 @@
     effect,
     loss,
     modifier,
     parameter,
     pdf,
     staterror,
     util,
+    visualization,
 )
 from evermore.modifier import Modifier  # noqa: E402
 from evermore.parameter import (  # noqa: E402,
     NormalParameter,
     Parameter,
 )
```

### Comparing `evermore-0.2.6/src/evermore/custom_types.py` & `evermore-0.2.7/src/evermore/custom_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         shape = jnp.broadcast_shapes(self.offset.shape, self.scale.shape)
         return type(self)(
             offset=jnp.broadcast_to(self.offset, shape),
             scale=jnp.broadcast_to(self.scale, shape),
         )
 
 
+@runtime_checkable
 class ModifierLike(Protocol):
     def offset_and_scale(self, hist: Array) -> OffsetAndScale: ...
     def __call__(self, hist: Array) -> Array: ...
     def __matmul__(self, other: ModifierLike) -> Compose: ...
 
 
 @runtime_checkable
```

### Comparing `evermore-0.2.6/src/evermore/effect.py` & `evermore-0.2.7/src/evermore/effect.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/src/evermore/loss.py` & `evermore-0.2.7/src/evermore/loss.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/src/evermore/modifier.py` & `evermore-0.2.7/src/evermore/modifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -347,38 +347,39 @@
         eqx.filter_jit(composition)(hist)
     """
 
     modifiers: list[ModifierLike]
 
     def __init__(self, *modifiers: ModifierLike) -> None:
         self.modifiers = list(modifiers)
-        # unroll nested compositions
+
+    def unroll_modifiers(self) -> list[ModifierLike]:
         _modifiers = []
         for mod in self.modifiers:
             if isinstance(mod, Compose):
                 _modifiers.extend(mod.modifiers)
             else:
-                assert isinstance(mod, ModifierBase)
+                assert isinstance(mod, ModifierLike)
                 _modifiers.append(mod)
         # by now all are modifiers
-        self.modifiers = _modifiers
+        return _modifiers
 
     def __len__(self) -> int:
-        return len(self.modifiers)
+        return len(self.unroll_modifiers())
 
     def offset_and_scale(self, hist: Array) -> OffsetAndScale:
         from collections import defaultdict
 
         # initial scale and offset
         scale = jnp.ones_like(hist)
         offset = jnp.zeros_like(hist)
 
         groups = defaultdict(list)
         # first group modifiers into same tree structures
-        for mod in self.modifiers:
+        for mod in self.unroll_modifiers():
             groups[hash(jtu.tree_structure(mod))].append(mod)
         # then do the `jax.lax.scan` loops
         for _, group_mods in groups.items():
             # skip empty groups
             if not group_mods:
                 continue
             # Essentially we are turning an array of modifiers into a single modifier of stacked leaves.
```

### Comparing `evermore-0.2.6/src/evermore/parameter.py` & `evermore-0.2.7/src/evermore/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
     # 2. set the filter_spec to True for each parameter value
     def _replace_value(leaf: Any) -> Any:
         if isinstance(leaf, Parameter):
             leaf = eqx.tree_at(lambda p: p.value, leaf, not leaf.frozen)
         return leaf
 
-    return params_map(_replace_value, filter_spec)
+    return jtu.tree_map(_replace_value, filter_spec, is_leaf=is_parameter)
 
 
 def partition(tree: PyTree) -> tuple[PyTree, PyTree]:
     """
     Short hand for:
 
     .. code-block:: python
```

### Comparing `evermore-0.2.6/src/evermore/pdf.py` & `evermore-0.2.7/src/evermore/pdf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
+from jax.scipy.special import gammaln, xlogy
 from jaxtyping import Array, PRNGKeyArray
 
 __all__ = [
     "PDF",
     "Normal",
     "Poisson",
 ]
@@ -42,14 +43,17 @@
         return self.mean + self.width * jax.random.normal(key)
 
 
 class Poisson(PDF):
     lamb: Array = eqx.field(converter=jnp.atleast_1d)
 
     def log_prob(self, x: Array) -> Array:
-        logpdf_max = jax.scipy.stats.poisson.logpmf(self.lamb, mu=self.lamb)
-        unnormalized = jax.scipy.stats.poisson.logpmf((x + 1) * self.lamb, mu=self.lamb)
+        def _continous_poisson_log_prob(x, lamb):
+            return xlogy(x, lamb) - lamb - gammaln(x + 1)
+
+        logpdf_max = _continous_poisson_log_prob(self.lamb, self.lamb)
+        unnormalized = _continous_poisson_log_prob((x + 1) * self.lamb, self.lamb)
         return unnormalized - logpdf_max
 
     def sample(self, key: PRNGKeyArray) -> Array:
         # this samples only integers, do we want that?
         return jax.random.poisson(key, self.lamb)
```

### Comparing `evermore-0.2.6/src/evermore/staterror.py` & `evermore-0.2.7/src/evermore/staterror.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,36 +70,46 @@
         ), "The PyTree structure of hists and histsw2 must be the same!"
         self.hists = hists
         self.histsw2 = histsw2
         self.threshold = threshold
 
         self.ntot = sum_over_leaves(self.hists)
         self.etot = jnp.sqrt(sum_over_leaves(self.histsw2))
-        ntot_eff = jnp.round(self.ntot**2 / self.etot**2, decimals=0)
+        ntot_eff = self.ntot**2 / self.etot**2
         self.mask = ntot_eff > self.threshold
 
         # setup params
         self.gaussians_global = NormalParameter(value=jnp.zeros_like(self.ntot))
         self.gaussians_per_process = jtu.tree_map(
             lambda hist: NormalParameter(value=jnp.zeros_like(hist)), self.hists
         )
         self.poissons_per_process = jtu.tree_map(
-            lambda hist: Parameter(
-                value=jnp.zeros_like(hist),
-                prior=Poisson(lamb=cast(Array, jnp.where(hist > 0.0, hist, 1.0))),
+            lambda w, w2: Parameter(
+                value=jnp.zeros_like(w),
+                prior=Poisson(
+                    lamb=cast(
+                        Array,
+                        jnp.where(
+                            (w**2 / jnp.sqrt(w2**2)) > 0.0,
+                            (w**2 / jnp.sqrt(w2**2)),
+                            1.0,
+                        ),
+                    )
+                ),
             ),
             self.hists,
+            self.histsw2,
         )
 
     def modifier(self, getter: Callable) -> ModifierLike:
         # see: https://github.com/cms-analysis/HiggsAnalysis-CombinedLimit/pull/929
         # and: https://cms-analysis.github.io/HiggsAnalysis-CombinedLimit/latest/part2/bin-wise-stats/#usage-instructions
 
         # poisson case per process
-        # if w > 0.0, then poisson, else noop (no effect)
+        # if w > 0.0, then poisson, else Identity (no effect)
         # since w <= 0 leads to NaNs in derivatives, we need to mask them
         w = getter(self.hists)
         poisson_params = getter(self.poissons_per_process)
         poisson_identity_mod = Modifier(parameter=poisson_params, effect=Identity())
         poisson_mod = Where(
             w > 0.0, poisson_params.scale(slope=1.0, offset=1.0), poisson_identity_mod
         )
@@ -137,15 +147,15 @@
         #
         # if n_tot_eff > threshold:
         #   apply global gaussian(width=e_tot/n_tot)
         # else:
         #   if n_i_eff > threshold or e_i > n_i or n_i <= 0.0:
         #       apply per process gaussian(width=e_i/n_i)
         #   else:
-        #       apply per process poisson(lamb=n_i)
+        #       apply per process poisson(lamb=n_i_eff)
         per_process_mask = (
             ((w**2 / w2**2) > self.threshold) | (jnp.sqrt(w2) > w) | (w <= 0)
         )
         return Where(
             self.mask,
             gauss_global_mod,
             Where(per_process_mask, gauss_mod, poisson_mod),
```

### Comparing `evermore-0.2.6/src/evermore/util.py` & `evermore-0.2.7/src/evermore/util.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/tests/test_effect.py` & `evermore-0.2.7/tests/test_effect.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/tests/test_loss.py` & `evermore-0.2.7/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/tests/test_modifier.py` & `evermore-0.2.7/tests/test_modifier.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/tests/test_parameter.py` & `evermore-0.2.7/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/.gitignore` & `evermore-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/LICENSE` & `evermore-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/README.md` & `evermore-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `evermore-0.2.6/pyproject.toml` & `evermore-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,23 @@
     "equinox>=0.10.6", # eqx.field
 ]
 
 [project.optional-dependencies]
 test = ["pytest >=6", "pytest-cov >=3"]
 dev = ["pytest >=6", "pytest-cov >=3", "optax", "jaxopt >=0.6"]
 docs = [
-    "sphinx>=7.0",
-    "myst_parser>=0.13",
+    "sphinx",
+    "myst-parser",
+    "myst-nb",
     "sphinx_copybutton",
     "sphinx_autodoc_typehints",
     "sphinx-book-theme",
     "sphinx-design",
     "sphinx-togglebutton",
+    "penzai",
 ]
 
 [project.urls]
 Homepage = "https://github.com/pfackeldey/evermore"
 "Bug Tracker" = "https://github.com/pfackeldey/evermore/issues"
 Discussions = "https://github.com/pfackeldey/evermore/discussions"
 Changelog = "https://github.com/pfackeldey/evermore/releases"
```

### Comparing `evermore-0.2.6/PKG-INFO` & `evermore-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: evermore
-Version: 0.2.6
+Version: 0.2.7
 Summary: Differentiable (binned) likelihoods in JAX.
 Project-URL: Homepage, https://github.com/pfackeldey/evermore
 Project-URL: Bug Tracker, https://github.com/pfackeldey/evermore/issues
 Project-URL: Discussions, https://github.com/pfackeldey/evermore/discussions
 Project-URL: Changelog, https://github.com/pfackeldey/evermore/releases
 Author-email: Peter Fackeldey <peter.fackeldey@rwth-aachen.de>
 License-File: LICENSE
@@ -28,21 +28,23 @@
 Requires-Dist: jaxtyping
 Provides-Extra: dev
 Requires-Dist: jaxopt>=0.6; extra == 'dev'
 Requires-Dist: optax; extra == 'dev'
 Requires-Dist: pytest-cov>=3; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: myst-parser>=0.13; extra == 'docs'
+Requires-Dist: myst-nb; extra == 'docs'
+Requires-Dist: myst-parser; extra == 'docs'
+Requires-Dist: penzai; extra == 'docs'
+Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-book-theme; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx-design; extra == 'docs'
 Requires-Dist: sphinx-togglebutton; extra == 'docs'
-Requires-Dist: sphinx>=7.0; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest-cov>=3; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
 
 <div align="center" style="height:250px;width:250px">
 <img src="https://raw.githubusercontent.com/pfackeldey/evermore/main/assets/logo.png" alt="logo"></img>
```

