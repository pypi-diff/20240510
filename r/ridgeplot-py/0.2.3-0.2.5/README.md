# Comparing `tmp/ridgeplot_py-0.2.3.tar.gz` & `tmp/ridgeplot_py-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ridgeplot_py-0.2.3.tar", max compression
+gzip compressed data, was "ridgeplot_py-0.2.5.tar", max compression
```

## Comparing `ridgeplot_py-0.2.3.tar` & `ridgeplot_py-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-01-08 04:59:43.283531 ridgeplot_py-0.2.3/LICENSE
--rw-r--r--   0        0        0     2960 2024-01-08 04:59:43.283531 ridgeplot_py-0.2.3/README.md
--rw-r--r--   0        0        0     1367 2024-01-08 05:00:03.775368 ridgeplot_py-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       73 2024-01-08 04:59:43.283531 ridgeplot_py-0.2.3/ridgeplot/__init__.py
--rw-r--r--   0        0        0     8283 2024-01-08 04:59:43.283531 ridgeplot_py-0.2.3/ridgeplot/colors.py
--rw-r--r--   0        0        0     3287 2024-01-08 04:59:43.283531 ridgeplot_py-0.2.3/ridgeplot/ridge_plot.py
--rw-r--r--   0        0        0      687 2024-01-08 04:59:43.283531 ridgeplot_py-0.2.3/ridgeplot/stats.py
--rw-r--r--   0        0        0     3753 1970-01-01 00:00:00.000000 ridgeplot_py-0.2.3/setup.py
--rw-r--r--   0        0        0     3686 1970-01-01 00:00:00.000000 ridgeplot_py-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2960 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/README.md
+-rw-r--r--   0        0        0     1465 2024-05-10 05:09:40.904313 ridgeplot_py-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/ridgeplot/__init__.py
+-rw-r--r--   0        0        0     8754 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/ridgeplot/colors.py
+-rw-r--r--   0        0        0     2174 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/ridgeplot/dotted_heatmap.py
+-rw-r--r--   0        0        0     3299 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/ridgeplot/ridge_plot.py
+-rw-r--r--   0        0        0      687 2024-05-10 05:09:27.876379 ridgeplot_py-0.2.5/ridgeplot/stats.py
+-rw-r--r--   0        0        0     3741 1970-01-01 00:00:00.000000 ridgeplot_py-0.2.5/PKG-INFO
```

### Comparing `ridgeplot_py-0.2.3/LICENSE` & `ridgeplot_py-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.3/README.md` & `ridgeplot_py-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.3/pyproject.toml` & `ridgeplot_py-0.2.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 [tool.poetry]
 name = "ridgeplot-py"
-version = "0.2.3" # managed by poetry-dynamic-versioning
+version = "0.2.5"                                   # managed by poetry-dynamic-versioning
 description = "Plotting ridgeplots with matplotlib"
 authors = ["Douglas Wu <wckdouglas@gmail.com>"]
 license = "MIT"
-packages = [
-    {"include" = "ridgeplot"}
-]
+packages = [{ "include" = "ridgeplot" }]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 scipy = "^1.8.0"
-matplotlib = "^3.1.3"
+matplotlib = "^3.8"
 more-itertools = "^8.9.0"
 numpy = "^1.21.1"
+pandas = "^2.2.2"
+poetry = "^1.8.3"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev]
+optional = true
+
+[tool.poetry.group.dev.dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^2.12.1"
-mypy = "^0.910"
-black = "22.3.0"
+mypy = "^0.990"
 ruff = "^0.0.290"
+pre-commit = "^3.7.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
-metadata= false
+metadata = false
 bump = true
 style = "pep440"
-pattern  = "^(?P<base>\\d+\\.\\d+\\.\\d+)(-?((?P<stage>[a-zA-Z]+)\\.?(?P<revision>\\d+)?))?"
+pattern = "^(?P<base>\\d+\\.\\d+\\.\\d+)(-?((?P<stage>[a-zA-Z]+)\\.?(?P<revision>\\d+)?))?"
 format-jinja = """
     {%- set ns = namespace(version=base) -%}
     {%- for i in range(distance) -%}
         {%- set ns.version = bump_version(ns.version) -%}
     {%- endfor -%}
     {{- ns.version -}}
 """
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
-[tool.poetry.extras]
-dev = ["pytest", "pytest-cov", "mypy", "ruff", "black"]
-
 [tool.mypy]
 plugins = "numpy.typing.mypy_plugin"
+ignore_missing_imports = true
+strict_optional = true
+check_untyped_defs = true
 
 [[tool.mypy.overrides]]
-module = [
-    "matplotlib.*",
-    "scipy.*"
-]
-ignore_missing_imports = true
+module = ["matplotlib.*", "scipy.*"]
+ignore_errors = true
+
 
 [tool.ruff]
 line-length = 120
 select = ['E', 'F', 'W', 'I']
-
```

### Comparing `ridgeplot_py-0.2.3/ridgeplot/colors.py` & `ridgeplot_py-0.2.5/ridgeplot/colors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """This module collects functions for manipulating color legends
 for matplotlib plots and a collections of color palettes.
 """
 
 from collections import OrderedDict
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Tuple
 
 import matplotlib.axes
 import matplotlib.patches as mpatches
 from matplotlib import legend
+from matplotlib.cm import get_cmap
+from matplotlib.colors import to_hex
 
 ColorPalette: Dict[str, List[str]] = dict(
     # 1. maximum
     # modified from:
     # https://sashat.me/2017/01/11/list-of-20-simple-distinct-colors/
     maximum=[
         "#f58231",
@@ -244,15 +246,20 @@
             colors: list of colors to be assigned to the categories
         Returns:
             list of colors corresponding to the input
         """
         self.fit(categories, colors=colors)
         return self.transform(categories)
 
-    def show_legend(self, ax: matplotlib.axes, sort: bool = False, **kwargs: Dict[str, Any]) -> legend.Legend:
+    def show_legend(
+        self,
+        ax: matplotlib.axes._axes.Axes,
+        sort: bool = False,
+        **kwargs: Dict[str, Any],
+    ) -> legend.Legend:
         """
         Adding matplotlib legend describing the color encoder to a matplotlib ax object
 
         Args:
             ax: matplotlib ax object
             sort: sort the legend by the category
             **kwargs: keyword arguments for matplotlib.pyplot.legend
@@ -262,7 +269,18 @@
         """
 
         if sort:
             self.encoder = OrderedDict(sorted(self.encoder.items(), key=lambda item: item[0]))
         pat = [mpatches.Patch(color=col, label=lab) for lab, col in self.encoder.items()]
         lgd = ax.legend(handles=pat, **kwargs)
         return lgd
+
+
+def get_cmap_color_values(cmap_name: str) -> Tuple[str, str]:
+    """
+    Get color values for the min and max color in a color map
+
+    :param str cmap_name: color map name (e.g. viridis)
+    :return Tuple[str, str]: hex code for the min and max color
+    """
+    cmap = get_cmap(cmap_name)
+    return to_hex(cmap(0.0)), to_hex(cmap(1.0))
```

### Comparing `ridgeplot_py-0.2.3/ridgeplot/ridge_plot.py` & `ridgeplot_py-0.2.5/ridgeplot/ridge_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module contains the main function to plot
 [ridgeplots](https://clauswilke.com/blog/2017/09/15/goodbye-joyplots/).
 """
+
 from __future__ import annotations
 
 from typing import Optional
 
 import matplotlib.axes
 import numpy as np
 from more_itertools import first
@@ -14,15 +15,15 @@
 
 
 class RidgePlotError(Exception):
     pass
 
 
 def ridgeplot(
-    ax: matplotlib.axes,
+    ax: matplotlib.axes._axes.Axes,
     data: dict[str, list[float]],
     xlim: Optional[tuple[float, float]] = None,
     fill_colors: Optional[list[str]] = None,
     line_colors: Optional[list[str]] = None,
     label_size: float = 10.0,
     fill_alpha: float = 0.5,
 ) -> None:
```

### Comparing `ridgeplot_py-0.2.3/ridgeplot/stats.py` & `ridgeplot_py-0.2.5/ridgeplot/stats.py`

 * *Files identical despite different names*

### Comparing `ridgeplot_py-0.2.3/setup.py` & `ridgeplot_py-0.2.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,100 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ridgeplot-py
+Version: 0.2.5
+Summary: Plotting ridgeplots with matplotlib
+License: MIT
+Author: Douglas Wu
+Author-email: wckdouglas@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: matplotlib (>=3.8,<4.0)
+Requires-Dist: more-itertools (>=8.9.0,<9.0.0)
+Requires-Dist: numpy (>=1.21.1,<2.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: poetry (>=1.8.3,<2.0.0)
+Requires-Dist: scipy (>=1.8.0,<2.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['ridgeplot']
+# ridgeplot-py #
 
-package_data = \
-{'': ['*']}
+[![CI](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml/badge.svg)](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/wckdouglas/ridgeplot-py/branch/main/graph/badge.svg?token=2owCGZa1K4)](https://codecov.io/gh/wckdouglas/ridgeplot-py) [![PyPI version](https://badge.fury.io/py/ridgeplot-py.svg)](https://badge.fury.io/py/ridgeplot-py) [![conda-forge](https://anaconda.org/conda-forge/ridgeplot-py/badges/version.svg)](https://anaconda.org/conda-forge/ridgeplot-py)
 
-install_requires = \
-['matplotlib>=3.1.3,<4.0.0',
- 'more-itertools>=8.9.0,<9.0.0',
- 'numpy>=1.21.1,<2.0.0',
- 'scipy>=1.8.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'ridgeplot-py',
-    'version': '0.2.3',
-    'description': 'Plotting ridgeplots with matplotlib',
-    'long_description': '# ridgeplot-py #\n\n[![CI](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml/badge.svg)](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/wckdouglas/ridgeplot-py/branch/main/graph/badge.svg?token=2owCGZa1K4)](https://codecov.io/gh/wckdouglas/ridgeplot-py) [![PyPI version](https://badge.fury.io/py/ridgeplot-py.svg)](https://badge.fury.io/py/ridgeplot-py) [![conda-forge](https://anaconda.org/conda-forge/ridgeplot-py/badges/version.svg)](https://anaconda.org/conda-forge/ridgeplot-py)\n\n\nThis is a simple module for plotting [ridgeplot](https://clauswilke.com/blog/2017/09/15/goodbye-joyplots/) with the [scipy ecosystem](https://www.scipy.org/about.html).\n\nRidgeplot is a great data visualization technique to compare distributions from multiple groups at the same time, and was first introduced in 2017 as joy plot:\n\n<blockquote class="twitter-tweet"><p lang="en" dir="ltr">I hereby propose that we call these &quot;joy plots&quot; <a href="https://twitter.com/hashtag/rstats?src=hash&amp;ref_src=twsrc%5Etfw">#rstats</a> <a href="https://t.co/uuLGpQLAwY">https://t.co/uuLGpQLAwY</a></p>&mdash; Jenny Bryan (@JennyBryan) <a href="https://twitter.com/JennyBryan/status/856674638981550080?ref_src=twsrc%5Etfw">April 25, 2017</a></blockquote> \n\n[ridgeplot-py](https://pypi.org/project/ridgeplot-py/) provides a simple API to produce matplotlib-compatible ridgeplots, as well as a handy [ColorEncoder](https://github.com/wckdouglas/ridgeplot-py/blob/0198628ce0622e2e7f4f4e9284165d5d09324ca9/ridgeplot/colors.py#L117) class with scikit-learn syntax for manipulating color annotations in a consistent way [through out manuscripts or presentations].\n\n## Install ##\n\n```bash\ngit clone git@github.com:wckdouglas/ridgeplot-py.git\ncd ridgeplot-py\npython setup.py install \n```\n\nor via conda:\n\n```bash\nconda install -c conda-forge ridgeplot-py\n```\n\nor via pypi:\n\n```bash\npip install ridgeplot-py\n```\n\n## Usage ##\n\n```python\nfrom ridgeplot import ridgeplot\nfrom ridgeplot.colors import ColorEncoder, ColorPalette\nimport numpy as np\nimport matplotlib.pyplot as plt\n\n# mocking some data\n# the input data should be a dict of\n# - keys: group names for the distributions\n# - values: list of values \ndata = {}\nfor i in range(8):\n    data[\'data_{}\'.format(i)] = np.random.randn(100) * (i+1)\n\n# make the plot\nfig = plt.figure()\nax = fig.add_subplot(111)\nridgeplot(\n    ax, \n    data, \n    xlim=(-20,20), \n    label_size=15\n)\n```\n\n![img](https://raw.githubusercontent.com/wckdouglas/ridgeplot-py/main/img/ridgeplot.png)\n\n\n## Example ##\n\nA [notebook](https://github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick howto is included in this repo!\n\n\n## Build on Apple silicon ##\n\nscipy may cause error and may be able to solved by the [this stackoverflow answer](https://stackoverflow.com/a/71764028):\n\n```\nbrew install openblas\nexport OPENBLAS="$(brew --prefix openblas)" \npoetry install\n```\n',
-    'author': 'Douglas Wu',
-    'author_email': 'wckdouglas@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
 
+This is a simple module for plotting [ridgeplot](https://clauswilke.com/blog/2017/09/15/goodbye-joyplots/) with the [scipy ecosystem](https://www.scipy.org/about.html).
+
+Ridgeplot is a great data visualization technique to compare distributions from multiple groups at the same time, and was first introduced in 2017 as joy plot:
+
+<blockquote class="twitter-tweet"><p lang="en" dir="ltr">I hereby propose that we call these &quot;joy plots&quot; <a href="https://twitter.com/hashtag/rstats?src=hash&amp;ref_src=twsrc%5Etfw">#rstats</a> <a href="https://t.co/uuLGpQLAwY">https://t.co/uuLGpQLAwY</a></p>&mdash; Jenny Bryan (@JennyBryan) <a href="https://twitter.com/JennyBryan/status/856674638981550080?ref_src=twsrc%5Etfw">April 25, 2017</a></blockquote> 
+
+[ridgeplot-py](https://pypi.org/project/ridgeplot-py/) provides a simple API to produce matplotlib-compatible ridgeplots, as well as a handy [ColorEncoder](https://github.com/wckdouglas/ridgeplot-py/blob/0198628ce0622e2e7f4f4e9284165d5d09324ca9/ridgeplot/colors.py#L117) class with scikit-learn syntax for manipulating color annotations in a consistent way [through out manuscripts or presentations].
+
+## Install ##
+
+```bash
+git clone git@github.com:wckdouglas/ridgeplot-py.git
+cd ridgeplot-py
+python setup.py install 
+```
+
+or via conda:
+
+```bash
+conda install -c conda-forge ridgeplot-py
+```
+
+or via pypi:
+
+```bash
+pip install ridgeplot-py
+```
+
+## Usage ##
+
+```python
+from ridgeplot import ridgeplot
+from ridgeplot.colors import ColorEncoder, ColorPalette
+import numpy as np
+import matplotlib.pyplot as plt
+
+# mocking some data
+# the input data should be a dict of
+# - keys: group names for the distributions
+# - values: list of values 
+data = {}
+for i in range(8):
+    data['data_{}'.format(i)] = np.random.randn(100) * (i+1)
+
+# make the plot
+fig = plt.figure()
+ax = fig.add_subplot(111)
+ridgeplot(
+    ax, 
+    data, 
+    xlim=(-20,20), 
+    label_size=15
+)
+```
+
+![img](https://raw.githubusercontent.com/wckdouglas/ridgeplot-py/main/img/ridgeplot.png)
+
+
+## Example ##
+
+A [notebook](https://github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick howto is included in this repo!
+
+
+## Build on Apple silicon ##
+
+scipy may cause error and may be able to solved by the [this stackoverflow answer](https://stackoverflow.com/a/71764028):
+
+```
+brew install openblas
+export OPENBLAS="$(brew --prefix openblas)" 
+poetry install
+```
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,47 +1,48 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['ridgeplot']
-package_data = \ {'': ['*']} install_requires = \ ['matplotlib>=3.1.3,<4.0.0',
-'more-itertools>=8.9.0,<9.0.0', 'numpy>=1.21.1,<2.0.0', 'scipy>=1.8.0,<2.0.0']
-setup_kwargs = { 'name': 'ridgeplot-py', 'version': '0.2.3', 'description':
-'Plotting ridgeplots with matplotlib', 'long_description': '# ridgeplot-py
-#\n\n[![CI](https://github.com/wckdouglas/ridgeplot-py/actions/workflows/
-ci.yaml/badge.svg)](https://github.com/wckdouglas/ridgeplot-py/actions/
-workflows/ci.yaml) [![codecov](https://codecov.io/gh/wckdouglas/ridgeplot-py/
-branch/main/graph/badge.svg?token=2owCGZa1K4)](https://codecov.io/gh/
-wckdouglas/ridgeplot-py) [![PyPI version](https://badge.fury.io/py/ridgeplot-
-py.svg)](https://badge.fury.io/py/ridgeplot-py) [![conda-forge](https://
-anaconda.org/conda-forge/ridgeplot-py/badges/version.svg)](https://
-anaconda.org/conda-forge/ridgeplot-py)\n\n\nThis is a simple module for
-plotting [ridgeplot](https://clauswilke.com/blog/2017/09/15/goodbye-joyplots/
-) with the [scipy ecosystem](https://www.scipy.org/about.html).\n\nRidgeplot is
-a great data visualization technique to compare distributions from multiple
-groups at the same time, and was first introduced in 2017 as joy plot:\n\n
+Metadata-Version: 2.1 Name: ridgeplot-py Version: 0.2.5 Summary: Plotting
+ridgeplots with matplotlib License: MIT Author: Douglas Wu Author-email:
+wckdouglas@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Requires-Dist: matplotlib
+(>=3.8,<4.0) Requires-Dist: more-itertools (>=8.9.0,<9.0.0) Requires-Dist:
+numpy (>=1.21.1,<2.0.0) Requires-Dist: pandas (>=2.2.2,<3.0.0) Requires-Dist:
+poetry (>=1.8.3,<2.0.0) Requires-Dist: scipy (>=1.8.0,<2.0.0) Description-
+Content-Type: text/markdown # ridgeplot-py # [![CI](https://github.com/
+wckdouglas/ridgeplot-py/actions/workflows/ci.yaml/badge.svg)](https://
+github.com/wckdouglas/ridgeplot-py/actions/workflows/ci.yaml) [![codecov]
+(https://codecov.io/gh/wckdouglas/ridgeplot-py/branch/main/graph/
+badge.svg?token=2owCGZa1K4)](https://codecov.io/gh/wckdouglas/ridgeplot-py) [!
+[PyPI version](https://badge.fury.io/py/ridgeplot-py.svg)](https://
+badge.fury.io/py/ridgeplot-py) [![conda-forge](https://anaconda.org/conda-
+forge/ridgeplot-py/badges/version.svg)](https://anaconda.org/conda-forge/
+ridgeplot-py) This is a simple module for plotting [ridgeplot](https://
+clauswilke.com/blog/2017/09/15/goodbye-joyplots/) with the [scipy ecosystem]
+(https://www.scipy.org/about.html). Ridgeplot is a great data visualization
+technique to compare distributions from multiple groups at the same time, and
+was first introduced in 2017 as joy plot:
      I hereby propose that we call these "joy plots" _#_r_s_t_a_t_s _h_t_t_p_s_:_/_/_t_._c_o_/
      _u_u_L_G_p_Q_L_A_w_Y
      — Jenny Bryan (@JennyBryan) _A_p_r_i_l_ _2_5_,_ _2_0_1_7
-\n\n[ridgeplot-py](https://pypi.org/project/ridgeplot-py/) provides a simple
-API to produce matplotlib-compatible ridgeplots, as well as a handy
-[ColorEncoder](https://github.com/wckdouglas/ridgeplot-py/blob/
+[ridgeplot-py](https://pypi.org/project/ridgeplot-py/) provides a simple API to
+produce matplotlib-compatible ridgeplots, as well as a handy [ColorEncoder]
+(https://github.com/wckdouglas/ridgeplot-py/blob/
 0198628ce0622e2e7f4f4e9284165d5d09324ca9/ridgeplot/colors.py#L117) class with
 scikit-learn syntax for manipulating color annotations in a consistent way
-[through out manuscripts or presentations].\n\n## Install ##\n\n```bash\ngit
-clone git@github.com:wckdouglas/ridgeplot-py.git\ncd ridgeplot-py\npython
-setup.py install \n```\n\nor via conda:\n\n```bash\nconda install -c conda-
-forge ridgeplot-py\n```\n\nor via pypi:\n\n```bash\npip install ridgeplot-
-py\n```\n\n## Usage ##\n\n```python\nfrom ridgeplot import ridgeplot\nfrom
-ridgeplot.colors import ColorEncoder, ColorPalette\nimport numpy as np\nimport
-matplotlib.pyplot as plt\n\n# mocking some data\n# the input data should be a
-dict of\n# - keys: group names for the distributions\n# - values: list of
-values \ndata = {}\nfor i in range(8):\n data[\'data_{}\'.format(i)] =
-np.random.randn(100) * (i+1)\n\n# make the plot\nfig = plt.figure()\nax =
-fig.add_subplot(111)\nridgeplot(\n ax, \n data, \n xlim=(-20,20), \n
-label_size=15\n)\n```\n\n![img](https://raw.githubusercontent.com/wckdouglas/
-ridgeplot-py/main/img/ridgeplot.png)\n\n\n## Example ##\n\nA [notebook](https:/
-/github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick
-howto is included in this repo!\n\n\n## Build on Apple silicon ##\n\nscipy may
-cause error and may be able to solved by the [this stackoverflow answer](https:
-//stackoverflow.com/a/71764028):\n\n```\nbrew install openblas\nexport
-OPENBLAS="$(brew --prefix openblas)" \npoetry install\n```\n', 'author':
-'Douglas Wu', 'author_email': 'wckdouglas@gmail.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'None', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+[through out manuscripts or presentations]. ## Install ## ```bash git clone
+git@github.com:wckdouglas/ridgeplot-py.git cd ridgeplot-py python setup.py
+install ``` or via conda: ```bash conda install -c conda-forge ridgeplot-py ```
+or via pypi: ```bash pip install ridgeplot-py ``` ## Usage ## ```python from
+ridgeplot import ridgeplot from ridgeplot.colors import ColorEncoder,
+ColorPalette import numpy as np import matplotlib.pyplot as plt # mocking some
+data # the input data should be a dict of # - keys: group names for the
+distributions # - values: list of values data = {} for i in range(8): data
+['data_{}'.format(i)] = np.random.randn(100) * (i+1) # make the plot fig =
+plt.figure() ax = fig.add_subplot(111) ridgeplot( ax, data, xlim=(-20,20),
+label_size=15 ) ``` ![img](https://raw.githubusercontent.com/wckdouglas/
+ridgeplot-py/main/img/ridgeplot.png) ## Example ## A [notebook](https://
+github.com/wckdouglas/ridgeplot-py/blob/main/Example.ipynb) showing quick howto
+is included in this repo! ## Build on Apple silicon ## scipy may cause error
+and may be able to solved by the [this stackoverflow answer](https://
+stackoverflow.com/a/71764028): ``` brew install openblas export OPENBLAS="$
+(brew --prefix openblas)" poetry install ```
```

