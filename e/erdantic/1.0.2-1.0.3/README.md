# Comparing `tmp/erdantic-1.0.2.tar.gz` & `tmp/erdantic-1.0.3.tar.gz`

## Comparing `erdantic-1.0.2.tar` & `erdantic-1.0.3.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 erdantic-1.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     9236 2020-02-02 00:00:00.000000 erdantic-1.0.2/HISTORY.md
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 erdantic-1.0.2/Makefile
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 erdantic-1.0.2/noxfile.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 erdantic-1.0.2/.github/codecov.yml
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 erdantic-1.0.2/.github/workflows/docs-main.yml
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 erdantic-1.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 erdantic-1.0.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/generate_images.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/generate_pydantic_with_default_column_diagram.py
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/hooks.py
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/mkdocs.yml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/changelog.md
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/cli.md
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/customizing.md
--rw-r--r--   0        0        0     7450 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/extending.md
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/forward-references.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/index.md
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/api-reference/convenience.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/api-reference/core.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/api-reference/exceptions.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/api-reference/typing_utils.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/api-reference/examples/attrs.md
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/api-reference/examples/dataclasses.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/api-reference/examples/pydantic.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/api-reference/examples/pydantic_v1.md
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/api-reference/plugins/attrs.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/api-reference/plugins/dataclasses.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/api-reference/plugins/index.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/api-reference/plugins/pydantic.md
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/assets/edge-many-unspecified.png
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/assets/edge-many-zero.png
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/assets/edge-one-one.png
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/assets/edge-one-zero.png
--rw-r--r--   0        0        0    93950 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/assets/erdantic_diagram.png
--rw-r--r--   0        0        0    21715 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/assets/erdantic_diagram.svg
--rw-r--r--   0        0        0    46733 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/assets/example_diagram.png
--rw-r--r--   0        0        0    13269 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/assets/example_diagram.svg
--rw-r--r--   0        0        0    46156 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/assets/pydantic_with_default_column_diagram.png
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/docs/css/mkdocs-jupyter-extra.css
--rw-r--r--   0        0        0   295642 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/notebooks/attrs.ipynb
--rw-r--r--   0        0        0   295870 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/notebooks/dataclasses.ipynb
--rw-r--r--   0        0        0   292514 2020-02-02 00:00:00.000000 erdantic-1.0.2/docs/notebooks/pydantic.ipynb
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/__main__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/_logging.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/_repr_utils.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/_version.py
--rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/cli.py
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/convenience.py
--rw-r--r--   0        0        0    28328 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/core.py
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/py.typed
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/typing_utils.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/examples/__init__.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/examples/attrs.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/examples/dataclasses.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/examples/pydantic.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/examples/pydantic_v1.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/plugins/__init__.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/plugins/attrs.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/plugins/dataclasses.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 erdantic-1.0.2/erdantic/plugins/pydantic.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 erdantic-1.0.2/requirements/dev.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 erdantic-1.0.2/requirements/docs.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 erdantic-1.0.2/requirements/lint.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 erdantic-1.0.2/requirements/tests.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 erdantic-1.0.2/requirements/typecheck.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/conftest.py
--rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/pydantic_with_default_column.py
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/test_against_assets.py
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/test_attrs.py
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/test_cli.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/test_convenience.py
--rw-r--r--   0        0        0    14682 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/test_core.py
--rw-r--r--   0        0        0     9867 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/test_dataclasses.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/test_plugins.py
--rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/test_pydantic.py
--rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/test_pydantic_v1.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/test_typing_utils.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/typechecks.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/utils.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/attrs.dot
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/attrs.json
--rw-r--r--   0        0        0    46807 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/attrs.png
--rw-r--r--   0        0        0    13191 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/attrs.svg
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/dataclasses.dot
--rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/dataclasses.json
--rw-r--r--   0        0        0    46807 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/dataclasses.png
--rw-r--r--   0        0        0    13335 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/dataclasses.svg
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/pydantic.dot
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/pydantic.json
--rw-r--r--   0        0        0    46807 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/pydantic.png
--rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/pydantic.svg
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/pydantic_v1.dot
--rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/pydantic_v1.json
--rw-r--r--   0        0        0    46807 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/pydantic_v1.png
--rw-r--r--   0        0        0    13335 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/pydantic_v1.svg
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/test_core-test_subclass/pydantic_with_default_column.dot
--rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/test_core-test_subclass/pydantic_with_default_column.json
--rw-r--r--   0        0        0    46347 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/test_core-test_subclass/pydantic_with_default_column.png
--rw-r--r--   0        0        0    15512 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/assets/test_core-test_subclass/pydantic_with_default_column.svg
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/scripts/generate_pydantic_with_defaults_assets.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 erdantic-1.0.2/tests/scripts/generate_static_assets.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 erdantic-1.0.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 erdantic-1.0.2/LICENSE
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 erdantic-1.0.2/README.md
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 erdantic-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 erdantic-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 erdantic-1.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     9466 2020-02-02 00:00:00.000000 erdantic-1.0.3/HISTORY.md
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 erdantic-1.0.3/Makefile
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 erdantic-1.0.3/noxfile.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 erdantic-1.0.3/.github/codecov.yml
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 erdantic-1.0.3/.github/workflows/docs-main.yml
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 erdantic-1.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 erdantic-1.0.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/generate_images.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/generate_pydantic_with_default_column_diagram.py
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/hooks.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/mkdocs.yml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/changelog.md
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/cli.md
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/customizing.md
+-rw-r--r--   0        0        0     7450 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/extending.md
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/forward-references.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/index.md
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/api-reference/convenience.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/api-reference/core.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/api-reference/exceptions.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/api-reference/typing_utils.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/api-reference/examples/attrs.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/api-reference/examples/dataclasses.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/api-reference/examples/pydantic.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/api-reference/examples/pydantic_v1.md
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/api-reference/plugins/attrs.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/api-reference/plugins/dataclasses.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/api-reference/plugins/index.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/api-reference/plugins/pydantic.md
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/assets/edge-many-unspecified.png
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/assets/edge-many-zero.png
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/assets/edge-one-one.png
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/assets/edge-one-zero.png
+-rw-r--r--   0        0        0    93950 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/assets/erdantic_diagram.png
+-rw-r--r--   0        0        0    21715 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/assets/erdantic_diagram.svg
+-rw-r--r--   0        0        0    46733 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/assets/example_diagram.png
+-rw-r--r--   0        0        0    13269 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/assets/example_diagram.svg
+-rw-r--r--   0        0        0    46156 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/assets/pydantic_with_default_column_diagram.png
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/docs/css/mkdocs-jupyter-extra.css
+-rw-r--r--   0        0        0   295642 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/notebooks/attrs.ipynb
+-rw-r--r--   0        0        0   295870 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/notebooks/dataclasses.ipynb
+-rw-r--r--   0        0        0   292514 2020-02-02 00:00:00.000000 erdantic-1.0.3/docs/notebooks/pydantic.ipynb
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/__main__.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/_logging.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/_repr_utils.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/_version.py
+-rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/cli.py
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/convenience.py
+-rw-r--r--   0        0        0    28446 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/core.py
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/py.typed
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/typing_utils.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/examples/__init__.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/examples/attrs.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/examples/dataclasses.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/examples/pydantic.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/examples/pydantic_v1.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/plugins/__init__.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/plugins/attrs.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/plugins/dataclasses.py
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 erdantic-1.0.3/erdantic/plugins/pydantic.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 erdantic-1.0.3/requirements/dev.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 erdantic-1.0.3/requirements/docs.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 erdantic-1.0.3/requirements/lint.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 erdantic-1.0.3/requirements/tests.txt
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 erdantic-1.0.3/requirements/typecheck.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/pydantic_with_default_column.py
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/test_against_assets.py
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/test_attrs.py
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/test_cli.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/test_convenience.py
+-rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/test_core.py
+-rw-r--r--   0        0        0     9867 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/test_dataclasses.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/test_plugins.py
+-rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/test_pydantic.py
+-rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/test_pydantic_v1.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/test_typing_utils.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/typechecks.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/utils.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/attrs.dot
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/attrs.json
+-rw-r--r--   0        0        0    46807 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/attrs.png
+-rw-r--r--   0        0        0    13191 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/attrs.svg
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/dataclasses.dot
+-rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/dataclasses.json
+-rw-r--r--   0        0        0    46807 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/dataclasses.png
+-rw-r--r--   0        0        0    13335 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/dataclasses.svg
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/pydantic.dot
+-rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/pydantic.json
+-rw-r--r--   0        0        0    46807 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/pydantic.png
+-rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/pydantic.svg
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/pydantic_v1.dot
+-rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/pydantic_v1.json
+-rw-r--r--   0        0        0    46807 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/pydantic_v1.png
+-rw-r--r--   0        0        0    13335 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/pydantic_v1.svg
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/test_core-test_subclass/pydantic_with_default_column.dot
+-rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/test_core-test_subclass/pydantic_with_default_column.json
+-rw-r--r--   0        0        0    46347 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/test_core-test_subclass/pydantic_with_default_column.png
+-rw-r--r--   0        0        0    15512 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/assets/test_core-test_subclass/pydantic_with_default_column.svg
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/scripts/generate_pydantic_with_defaults_assets.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 erdantic-1.0.3/tests/scripts/generate_static_assets.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 erdantic-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 erdantic-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 erdantic-1.0.3/README.md
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 erdantic-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 erdantic-1.0.3/PKG-INFO
```

### Comparing `erdantic-1.0.2/CONTRIBUTING.md` & `erdantic-1.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/HISTORY.md` & `erdantic-1.0.3/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # erdantic Changelog
 
+## v1.0.3 (2024-05-10)
+
+- Fixed `StopIteration` error when rendering a model that has no fields. ([Issue #120](https://github.com/drivendataorg/erdantic/issues/120), [PR #121](https://github.com/drivendataorg/erdantic/pull/121))
+
 ## v1.0.2 (2024-04-11)
 
 - Fixed `AttributeError` when adding a model that has a field annotated with certain typing special forms like `Any`, `Literal`, or `TypeVar` instances. ([Issue #114](https://github.com/drivendataorg/erdantic/issues/114), [PR #115](https://github.com/drivendataorg/erdantic/pull/115))
 
 ## v1.0.1 (2024-04-10)
 
 - Fixed `ModuleNotFoundError` when importing from `erdantic.examples` without attrs installed.
```

### Comparing `erdantic-1.0.2/Makefile` & `erdantic-1.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/noxfile.py` & `erdantic-1.0.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/.github/codecov.yml` & `erdantic-1.0.3/.github/codecov.yml`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/.github/workflows/docs-main.yml` & `erdantic-1.0.3/.github/workflows/docs-main.yml`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/.github/workflows/release.yml` & `erdantic-1.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/.github/workflows/tests.yml` & `erdantic-1.0.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/generate_images.py` & `erdantic-1.0.3/docs/generate_images.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/hooks.py` & `erdantic-1.0.3/docs/hooks.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/mkdocs.yml` & `erdantic-1.0.3/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/docs/customizing.md` & `erdantic-1.0.3/docs/docs/customizing.md`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/docs/extending.md` & `erdantic-1.0.3/docs/docs/extending.md`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/docs/forward-references.md` & `erdantic-1.0.3/docs/docs/forward-references.md`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/docs/assets/edge-many-unspecified.png` & `erdantic-1.0.3/docs/docs/assets/edge-many-unspecified.png`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/docs/assets/edge-many-zero.png` & `erdantic-1.0.3/docs/docs/assets/edge-many-zero.png`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/docs/assets/edge-one-one.png` & `erdantic-1.0.3/docs/docs/assets/edge-one-one.png`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/docs/assets/edge-one-zero.png` & `erdantic-1.0.3/docs/docs/assets/edge-one-zero.png`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/docs/assets/erdantic_diagram.png` & `erdantic-1.0.3/docs/docs/assets/erdantic_diagram.png`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/docs/assets/erdantic_diagram.svg` & `erdantic-1.0.3/docs/docs/assets/erdantic_diagram.svg`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/docs/assets/example_diagram.png` & `erdantic-1.0.3/docs/docs/assets/example_diagram.png`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/docs/assets/example_diagram.svg` & `erdantic-1.0.3/docs/docs/assets/example_diagram.svg`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/docs/assets/pydantic_with_default_column_diagram.png` & `erdantic-1.0.3/docs/docs/assets/pydantic_with_default_column_diagram.png`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/notebooks/attrs.ipynb` & `erdantic-1.0.3/docs/notebooks/attrs.ipynb`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/notebooks/dataclasses.ipynb` & `erdantic-1.0.3/docs/notebooks/dataclasses.ipynb`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/docs/notebooks/pydantic.ipynb` & `erdantic-1.0.3/docs/notebooks/pydantic.ipynb`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/erdantic/_repr_utils.py` & `erdantic-1.0.3/erdantic/_repr_utils.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/erdantic/cli.py` & `erdantic-1.0.3/erdantic/cli.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/erdantic/convenience.py` & `erdantic-1.0.3/erdantic/convenience.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/erdantic/core.py` & `erdantic-1.0.3/erdantic/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,19 @@
         model. It is used as the `label` attribute of data model's node in the graph's DOT
         representation.
 
         Returns:
             str: DOT language for table
         """
         # Get number of columns dynamically from first row
-        num_cols = next(iter(self.fields.values())).to_dot_row().count("<td")
+        try:
+            num_cols = next(iter(self.fields.values())).to_dot_row().count("<td")
+        except StopIteration:
+            # No fields, so just use 1 column
+            num_cols = 1
         # Concatenate DOT of all rows together
         rows = "\n".join(field_info.to_dot_row() for field_info in self.fields.values()) + "\n"
         return self._dot_table_template.format(
             name=self.name, num_cols=num_cols, rows=rows
         ).replace("\n", "")
```

### Comparing `erdantic-1.0.2/erdantic/exceptions.py` & `erdantic-1.0.3/erdantic/exceptions.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/erdantic/typing_utils.py` & `erdantic-1.0.3/erdantic/typing_utils.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/erdantic/examples/attrs.py` & `erdantic-1.0.3/erdantic/examples/attrs.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/erdantic/examples/dataclasses.py` & `erdantic-1.0.3/erdantic/examples/dataclasses.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/erdantic/examples/pydantic.py` & `erdantic-1.0.3/erdantic/examples/pydantic.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/erdantic/examples/pydantic_v1.py` & `erdantic-1.0.3/erdantic/examples/pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/erdantic/plugins/__init__.py` & `erdantic-1.0.3/erdantic/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/erdantic/plugins/attrs.py` & `erdantic-1.0.3/erdantic/plugins/attrs.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/erdantic/plugins/dataclasses.py` & `erdantic-1.0.3/erdantic/plugins/dataclasses.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/erdantic/plugins/pydantic.py` & `erdantic-1.0.3/erdantic/plugins/pydantic.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/conftest.py` & `erdantic-1.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/pydantic_with_default_column.py` & `erdantic-1.0.3/tests/pydantic_with_default_column.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/test_against_assets.py` & `erdantic-1.0.3/tests/test_against_assets.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/test_attrs.py` & `erdantic-1.0.3/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/test_cli.py` & `erdantic-1.0.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/test_convenience.py` & `erdantic-1.0.3/tests/test_convenience.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/test_core.py` & `erdantic-1.0.3/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,25 @@
         type_var_field: T
         anystr_field: AnyStr
 
     diagram = EntityRelationshipDiagram()
     diagram.add_model(MyModel)
 
 
+def test_model_with_no_fields():
+    """Model with no fields should not error."""
+
+    class EmptyModel(pydantic.BaseModel):
+        pass
+
+    diagram = EntityRelationshipDiagram()
+    diagram.add_model(EmptyModel)
+    diagram.to_dot()
+
+
 def test_unsupported_forward_ref_resolution(monkeypatch):
     """Plugin implementation does not do anything to resolve forward references."""
 
     def get_fields_from_dataclass_no_get_type_hints(model: DataclassType) -> List[FieldInfo]:
         """Version of get_fields_from_dataclass that doesn't use get_type_hints and doesn't do
         anything to resolve forward references."""
         return [
```

### Comparing `erdantic-1.0.2/tests/test_dataclasses.py` & `erdantic-1.0.3/tests/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/test_plugins.py` & `erdantic-1.0.3/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/test_pydantic.py` & `erdantic-1.0.3/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/test_pydantic_v1.py` & `erdantic-1.0.3/tests/test_pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/test_typing_utils.py` & `erdantic-1.0.3/tests/test_typing_utils.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/typechecks.py` & `erdantic-1.0.3/tests/typechecks.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/attrs.dot` & `erdantic-1.0.3/tests/assets/attrs.dot`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/attrs.json` & `erdantic-1.0.3/tests/assets/attrs.json`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/attrs.png` & `erdantic-1.0.3/tests/assets/attrs.png`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/attrs.svg` & `erdantic-1.0.3/tests/assets/attrs.svg`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/dataclasses.dot` & `erdantic-1.0.3/tests/assets/dataclasses.dot`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/dataclasses.json` & `erdantic-1.0.3/tests/assets/dataclasses.json`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/dataclasses.png` & `erdantic-1.0.3/tests/assets/dataclasses.png`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/dataclasses.svg` & `erdantic-1.0.3/tests/assets/dataclasses.svg`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/pydantic.dot` & `erdantic-1.0.3/tests/assets/pydantic.dot`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/pydantic.json` & `erdantic-1.0.3/tests/assets/pydantic.json`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/pydantic.png` & `erdantic-1.0.3/tests/assets/pydantic.png`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/pydantic.svg` & `erdantic-1.0.3/tests/assets/pydantic.svg`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/pydantic_v1.dot` & `erdantic-1.0.3/tests/assets/pydantic_v1.dot`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/pydantic_v1.json` & `erdantic-1.0.3/tests/assets/pydantic_v1.json`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/pydantic_v1.png` & `erdantic-1.0.3/tests/assets/pydantic_v1.png`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/pydantic_v1.svg` & `erdantic-1.0.3/tests/assets/pydantic_v1.svg`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/test_core-test_subclass/pydantic_with_default_column.dot` & `erdantic-1.0.3/tests/assets/test_core-test_subclass/pydantic_with_default_column.dot`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/test_core-test_subclass/pydantic_with_default_column.json` & `erdantic-1.0.3/tests/assets/test_core-test_subclass/pydantic_with_default_column.json`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/test_core-test_subclass/pydantic_with_default_column.png` & `erdantic-1.0.3/tests/assets/test_core-test_subclass/pydantic_with_default_column.png`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/assets/test_core-test_subclass/pydantic_with_default_column.svg` & `erdantic-1.0.3/tests/assets/test_core-test_subclass/pydantic_with_default_column.svg`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/scripts/generate_pydantic_with_defaults_assets.py` & `erdantic-1.0.3/tests/scripts/generate_pydantic_with_defaults_assets.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/tests/scripts/generate_static_assets.py` & `erdantic-1.0.3/tests/scripts/generate_static_assets.py`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/.gitignore` & `erdantic-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/LICENSE` & `erdantic-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/README.md` & `erdantic-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `erdantic-1.0.2/pyproject.toml` & `erdantic-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "erdantic"
-version = "1.0.2"
+version = "1.0.3"
 description = "Entity relationship diagrams for Python data model classes like Pydantic."
 readme = "README.md"
 authors = [{ name = "DrivenData", email = "info@drivendata.org" }, { name = "Jay Qi" }]
 license = { text = "MIT License" }
 keywords = ["erd", "entity relationship diagram", "dataclasses", "pydantic", "attrs"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `erdantic-1.0.2/PKG-INFO` & `erdantic-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: erdantic
-Version: 1.0.2
+Version: 1.0.3
 Summary: Entity relationship diagrams for Python data model classes like Pydantic.
 Project-URL: Repository, https://github.com/drivendataorg/erdantic
 Project-URL: Documentation, https://erdantic.drivendata.org/
 Project-URL: Bug Tracker, https://github.com/drivendataorg/erdantic/issues
 Project-URL: Changelog, https://erdantic.drivendata.org/stable/changelog/
 Author: Jay Qi
 Author-email: DrivenData <info@drivendata.org>
```

