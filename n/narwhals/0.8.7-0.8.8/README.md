# Comparing `tmp/narwhals-0.8.7.tar.gz` & `tmp/narwhals-0.8.8.tar.gz`

## Comparing `narwhals-0.8.7.tar` & `narwhals-0.8.8.tar`

### file list

```diff
@@ -1,122 +1,122 @@
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.7/mkdocs.yml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.7/requirements-dev.txt
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.7/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.7/.github/workflows/extremes.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.7/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.7/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.7/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/extending.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/generate_members.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/installation.md
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/quick_start.md
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/related.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/requirements-docs.txt
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/roadmap.md
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/why.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/dataframe.md
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/dependencies.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/dtypes.md
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/expressions.md
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/expressions_dt.md
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/expressions_str.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/index.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/lazyframe.md
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/narwhals.md
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/series.md
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/series_dt.md
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/api-reference/series_str.md
--rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/assets/image.png
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/basics/column.md
--rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/basics/complete_example.md
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/basics/dataframe.md
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.7/docs/other/pandas_index.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/__init__.py
--rw-r--r--   0        0        0    93496 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/dataframe.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/dependencies.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/dtypes.py
--rw-r--r--   0        0        0    37580 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/expression.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/functions.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/group_by.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/py.typed
--rw-r--r--   0        0        0    13814 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/series.py
--rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/translate.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/typing.py
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/__init__.py
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/dataframe.py
--rw-r--r--   0        0        0    10392 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/expr.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/group_by.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/namespace.py
--rw-r--r--   0        0        0    16348 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/series.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/typing.py
--rw-r--r--   0        0        0    14015 2020-02-02 00:00:00.000000 narwhals-0.8.7/narwhals/_pandas_like/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/group_by_test.py
--rw-r--r--   0        0        0    22286 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_common.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_dt.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_group_by.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_invalid.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_pandas.py
--rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_series.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/test_str.py
--rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/tpch_q1_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/utils.py
--rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/customer.parquet
--rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/lineitem.parquet
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/nation.parquet
--rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/orders.parquet
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/part.parquet
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/partsupp.parquet
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/region.parquet
--rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/data/supplier.parquet
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/cum_sum_test.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/diff_test.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/fill_null_test.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/over_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/test_over.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/str/__init__.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/str/head_test.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/expr/str/to_datetime_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/frame/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/frame/pipe_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/hypothesis/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/hypothesis/test_basic_arithmetic.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/hypothesis/test_concat.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.7/tests/hypothesis/test_join.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/__init__.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/q1.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/q2.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/q3.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/q4.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/q5.py
--rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/gpu/execute.ipynb
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/gpu/kernel-metadata.json
--rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q1/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q1/kernel-metadata.json
--rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q2/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q2/kernel-metadata.json
--rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q3/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q3/kernel-metadata.json
--rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q4/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q4/kernel-metadata.json
--rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q5/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q5/kernel-metadata.json
--rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q6/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q6/kernel-metadata.json
--rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q7/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q7/kernel-metadata.json
--rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q8/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.7/tpch/notebooks/q8/kernel-metadata.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.7/utils/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.7/utils/bump_version.py
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.7/utils/check_api_reference.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.7/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.7/LICENSE.md
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.7/README.md
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.7/pyproject.toml
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 narwhals-0.8.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 narwhals-0.8.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 narwhals-0.8.8/mkdocs.yml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 narwhals-0.8.8/requirements-dev.txt
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.8.8/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 narwhals-0.8.8/.github/workflows/extremes.yml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.8.8/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.8.8/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 narwhals-0.8.8/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/extending.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/generate_members.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/installation.md
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/quick_start.md
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/related.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/requirements-docs.txt
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/roadmap.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/why.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/dataframe.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/dependencies.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/dtypes.md
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/expressions.md
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/expressions_dt.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/expressions_str.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/index.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/lazyframe.md
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/narwhals.md
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/series.md
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/series_dt.md
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/api-reference/series_str.md
+-rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/assets/image.png
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/basics/column.md
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/basics/complete_example.md
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/basics/dataframe.md
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 narwhals-0.8.8/docs/other/pandas_index.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/__init__.py
+-rw-r--r--   0        0        0    93496 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/dataframe.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/dependencies.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/dtypes.py
+-rw-r--r--   0        0        0    38122 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/expression.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/functions.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/group_by.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/py.typed
+-rw-r--r--   0        0        0    15333 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/series.py
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/translate.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/typing.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/__init__.py
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/dataframe.py
+-rw-r--r--   0        0        0    10392 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/expr.py
+-rw-r--r--   0        0        0     5801 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/group_by.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/namespace.py
+-rw-r--r--   0        0        0    16348 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/series.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/typing.py
+-rw-r--r--   0        0        0    14015 2020-02-02 00:00:00.000000 narwhals-0.8.8/narwhals/_pandas_like/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/__init__.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/conftest.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/group_by_test.py
+-rw-r--r--   0        0        0    22286 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_common.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_dt.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_group_by.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_invalid.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_pandas.py
+-rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_series.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/test_str.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/tpch_q1_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/utils.py
+-rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/customer.parquet
+-rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/lineitem.parquet
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/nation.parquet
+-rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/orders.parquet
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/part.parquet
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/partsupp.parquet
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/region.parquet
+-rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/data/supplier.parquet
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/cum_sum_test.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/diff_test.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/fill_null_test.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/over_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/test_over.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/str/__init__.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/str/head_test.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/expr/str/to_datetime_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/frame/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/frame/pipe_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/hypothesis/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/hypothesis/test_basic_arithmetic.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/hypothesis/test_concat.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 narwhals-0.8.8/tests/hypothesis/test_join.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/q1.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/q2.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/q3.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/q4.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/q5.py
+-rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/gpu/execute.ipynb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/gpu/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17860 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q1/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q1/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18811 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q2/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q2/kernel-metadata.json
+-rwxr-xr-x   0        0        0    17692 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q3/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q3/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16689 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q4/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q4/kernel-metadata.json
+-rwxr-xr-x   0        0        0    18235 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q5/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q5/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16156 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q6/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q6/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27860 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q7/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q7/kernel-metadata.json
+-rwxr-xr-x   0        0        0    27709 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q8/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.8.8/tpch/notebooks/q8/kernel-metadata.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.8.8/utils/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.8.8/utils/bump_version.py
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 narwhals-0.8.8/utils/check_api_reference.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.8.8/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.8.8/LICENSE.md
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 narwhals-0.8.8/README.md
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 narwhals-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 narwhals-0.8.8/PKG-INFO
```

### Comparing `narwhals-0.8.7/.pre-commit-config.yaml` & `narwhals-0.8.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/CONTRIBUTING.md` & `narwhals-0.8.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/mkdocs.yml` & `narwhals-0.8.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/.github/CODE_OF_CONDUCT.md` & `narwhals-0.8.8/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/.github/workflows/extremes.yml` & `narwhals-0.8.8/.github/workflows/extremes.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/.github/workflows/mkdocs.yml` & `narwhals-0.8.8/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/.github/workflows/publish_to_pypi.yml` & `narwhals-0.8.8/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/.github/workflows/pytest.yml` & `narwhals-0.8.8/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/docs/extending.md` & `narwhals-0.8.8/docs/extending.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/docs/generate_members.py` & `narwhals-0.8.8/docs/generate_members.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/docs/index.md` & `narwhals-0.8.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/docs/quick_start.md` & `narwhals-0.8.8/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/docs/related.md` & `narwhals-0.8.8/docs/related.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/docs/why.md` & `narwhals-0.8.8/docs/why.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/docs/api-reference/index.md` & `narwhals-0.8.8/docs/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/docs/api-reference/series.md` & `narwhals-0.8.8/docs/api-reference/series.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/docs/assets/image.png` & `narwhals-0.8.8/docs/assets/image.png`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/docs/basics/column.md` & `narwhals-0.8.8/docs/basics/column.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/docs/basics/complete_example.md` & `narwhals-0.8.8/docs/basics/complete_example.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/docs/basics/dataframe.md` & `narwhals-0.8.8/docs/basics/dataframe.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/docs/other/pandas_index.md` & `narwhals-0.8.8/docs/other/pandas_index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/narwhals/__init__.py` & `narwhals-0.8.8/narwhals/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from narwhals.expression import sum
 from narwhals.expression import sum_horizontal
 from narwhals.functions import concat
 from narwhals.series import Series
 from narwhals.translate import from_native
 from narwhals.translate import to_native
 
-__version__ = "0.8.7"
+__version__ = "0.8.8"
 
 __all__ = [
     "concat",
     "to_native",
     "from_native",
     "all",
     "col",
```

### Comparing `narwhals-0.8.7/narwhals/dataframe.py` & `narwhals-0.8.8/narwhals/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/narwhals/dependencies.py` & `narwhals-0.8.8/narwhals/dependencies.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/narwhals/dtypes.py` & `narwhals-0.8.8/narwhals/dtypes.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/narwhals/expression.py` & `narwhals-0.8.8/narwhals/expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1025,33 +1025,33 @@
             >>> df_pd = pd.DataFrame(data)
             >>> df_pl = pl.DataFrame(data)
 
             We define a dataframe-agnostic function:
 
             >>> def func(df_any):
             ...     df = nw.from_native(df_any)
-            ...     df = df.select(nw.col('a').dt.ordinal_day())
+            ...     df = df.with_columns(a_ordinal_day=nw.col('a').dt.ordinal_day())
             ...     return nw.to_native(df)
 
             We can then pass either pandas or Polars to `func`:
 
             >>> func(df_pd)
-                 a
-            0    1
-            1  216
+                       a  a_ordinal_day
+            0 2020-01-01              1
+            1 2020-08-03            216
             >>> func(df_pl)
-            shape: (2, 1)
-            ┌─────┐
-            │ a   │
-            │ --- │
-            │ i16 │
-            ╞═════╡
-            │ 1   │
-            │ 216 │
-            └─────┘
+            shape: (2, 2)
+            ┌─────────────────────┬───────────────┐
+            │ a                   ┆ a_ordinal_day │
+            │ ---                 ┆ ---           │
+            │ datetime[μs]        ┆ i16           │
+            ╞═════════════════════╪═══════════════╡
+            │ 2020-01-01 00:00:00 ┆ 1             │
+            │ 2020-08-03 00:00:00 ┆ 216           │
+            └─────────────────────┴───────────────┘
         """
         return self._expr.__class__(lambda plx: self._expr._call(plx).dt.ordinal_day())
 
 
 def col(*names: str | Iterable[str]) -> Expr:
     """
     Instantiate an expression, similar to `polars.col`.
```

### Comparing `narwhals-0.8.7/narwhals/functions.py` & `narwhals-0.8.8/narwhals/functions.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/narwhals/group_by.py` & `narwhals-0.8.8/narwhals/group_by.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,52 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
+from typing import Any
 from typing import Iterable
+from typing import Iterator
+
+from narwhals.utils import flatten
+from narwhals.utils import tupleify
 
 if TYPE_CHECKING:
     from narwhals.dataframe import DataFrame
     from narwhals.dataframe import LazyFrame
     from narwhals.typing import IntoExpr
 
 
 class GroupBy:
     def __init__(self, df: DataFrame, *keys: str | Iterable[str]) -> None:
         self._df = df
-        self._keys = keys
+        self._keys = flatten(keys)
+        self._grouped = self._df._dataframe.group_by(self._keys)
 
     def agg(
         self, *aggs: IntoExpr | Iterable[IntoExpr], **named_aggs: IntoExpr
     ) -> DataFrame:
         aggs, named_aggs = self._df._flatten_and_extract(*aggs, **named_aggs)
         return self._df.__class__(
-            self._df._dataframe.group_by(*self._keys).agg(*aggs, **named_aggs),
+            self._grouped.agg(*aggs, **named_aggs),
+        )
+
+    def __iter__(self) -> Iterator[tuple[Any, DataFrame]]:
+        import narwhals as nw
+
+        yield from (
+            (tupleify(key), nw.from_native(df, eager_only=True))
+            for (key, df) in self._grouped.__iter__()
         )
 
 
 class LazyGroupBy:
     def __init__(self, df: LazyFrame, *keys: str | Iterable[str]) -> None:
         self._df = df
         self._keys = keys
+        self._grouped = self._df._dataframe.group_by(*self._keys)
 
     def agg(
         self, *aggs: IntoExpr | Iterable[IntoExpr], **named_aggs: IntoExpr
     ) -> LazyFrame:
         aggs, named_aggs = self._df._flatten_and_extract(*aggs, **named_aggs)
         return self._df.__class__(
-            self._df._dataframe.group_by(*self._keys).agg(*aggs, **named_aggs),
+            self._grouped.agg(*aggs, **named_aggs),
         )
```

### Comparing `narwhals-0.8.7/narwhals/series.py` & `narwhals-0.8.8/narwhals/series.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,14 +134,38 @@
             3
             >>> func(s_pl)
             3
         """
         return self._series.max()
 
     def sum(self) -> Any:
+        """
+        Reduce this Series to the sum value.
+
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> import narwhals as nw
+            >>> s = [1, 2, 3]
+            >>> s_pd = pd.Series(s)
+            >>> s_pl = pl.Series(s)
+
+            We define a library agnostic function:
+
+            >>> def func(s_any):
+            ...     s = nw.from_native(s_any, series_only=True)
+            ...     return s.sum()
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(s_pd)
+            6
+            >>> func(s_pl)
+            6
+        """
         return self._series.sum()
 
     def std(self, *, ddof: int = 1) -> Any:
         return self._series.std(ddof=ddof)
 
     def is_in(self, other: Any) -> Self:
         return self._from_series(self._series.is_in(self._extract_native(other)))
@@ -226,14 +250,48 @@
                6
                9
             ]
         """
         return self._from_series(self._series.cum_sum())
 
     def unique(self) -> Self:
+        """
+        Returns unique values
+
+        Examples:
+            >>> import pandas as pd
+            >>> import polars as pl
+            >>> import narwhals as nw
+            >>> s = [2, 4, 4, 6]
+            >>> s_pd = pd.Series(s)
+            >>> s_pl = pl.Series(s)
+
+            Let's define a dataframe-agnostic function:
+
+            >>> def func(s_any):
+            ...    s = nw.from_native(s_any, series_only=True)
+            ...    s = s.unique()
+            ...    return nw.to_native(s)
+
+            We can then pass either pandas or Polars to `func`:
+
+            >>> func(s_pd)
+            0    2
+            1    4
+            2    6
+            dtype: int64
+            >>> func(s_pl)  # doctest: +NORMALIZE_WHITESPACE
+            shape: (3,)
+            Series: '' [i64]
+            [
+               2
+               4
+               6
+            ]
+        """
         return self._from_series(self._series.unique())
 
     def diff(self) -> Self:
         """
         Calculate the difference with the previous element, for each element.
 
         Notes:
```

### Comparing `narwhals-0.8.7/narwhals/translate.py` & `narwhals-0.8.8/narwhals/translate.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/narwhals/typing.py` & `narwhals-0.8.8/narwhals/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/narwhals/utils.py` & `narwhals-0.8.8/narwhals/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
 import re
 from typing import Any
 from typing import Iterable
 from typing import Sequence
+from typing import TypeVar
 
 from narwhals.dependencies import get_pandas
 from narwhals.dependencies import get_polars
 
+T = TypeVar("T")
+
 
 def remove_prefix(text: str, prefix: str) -> str:
     if text.startswith(prefix):
         return text[len(prefix) :]
     return text  # pragma: no cover
 
 
@@ -25,14 +28,20 @@
     if not args:
         return []
     if len(args) == 1 and _is_iterable(args[0]):
         return args[0]  # type: ignore[no-any-return]
     return args  # type: ignore[no-any-return]
 
 
+def tupleify(arg: Any) -> Any:
+    if not isinstance(arg, (list, tuple)):  # pragma: no cover
+        return (arg,)
+    return arg
+
+
 def _is_iterable(arg: Any | Iterable[Any]) -> bool:
     from narwhals.series import Series
 
     if (pd := get_pandas()) is not None and isinstance(arg, (pd.Series, pd.DataFrame)):
         msg = f"Expected Narwhals class or scalar, got: {type(arg)}. Perhaps you forgot a `nw.from_native` somewhere?"
         raise TypeError(msg)
     if (pl := get_polars()) is not None and isinstance(
```

### Comparing `narwhals-0.8.7/narwhals/_pandas_like/dataframe.py` & `narwhals-0.8.8/narwhals/_pandas_like/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/narwhals/_pandas_like/expr.py` & `narwhals-0.8.8/narwhals/_pandas_like/expr.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/narwhals/_pandas_like/group_by.py` & `narwhals-0.8.8/narwhals/_pandas_like/group_by.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import collections
 import warnings
 from copy import copy
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
 from typing import Iterable
+from typing import Iterator
 
 from narwhals._pandas_like.utils import is_simple_aggregation
 from narwhals._pandas_like.utils import item
 from narwhals._pandas_like.utils import parse_into_exprs
 from narwhals.utils import parse_version
 from narwhals.utils import remove_prefix
 
@@ -20,45 +21,44 @@
     from narwhals._pandas_like.typing import IntoPandasExpr
 
 
 class PandasGroupBy:
     def __init__(self, df: PandasDataFrame, keys: list[str]) -> None:
         self._df = df
         self._keys = list(keys)
+        self._grouped = self._df._dataframe.groupby(
+            list(self._keys),
+            sort=False,
+            as_index=True,
+        )
 
     def agg(
         self,
         *aggs: IntoPandasExpr | Iterable[IntoPandasExpr],
         **named_aggs: IntoPandasExpr,
     ) -> PandasDataFrame:
-        df = self._df._dataframe
         exprs = parse_into_exprs(
             self._df._implementation,
             *aggs,
             **named_aggs,
         )
-        grouped = df.groupby(
-            list(self._keys),
-            sort=False,
-            as_index=True,
-        )
         implementation: str = self._df._implementation
         output_names: list[str] = copy(self._keys)
         for expr in exprs:
             if expr._output_names is None:
                 msg = (
                     "Anonymous expressions are not supported in group_by.agg.\n"
                     "Instead of `nw.all()`, try using a named expression, such as "
                     "`nw.col('a', 'b')`\n"
                 )
                 raise ValueError(msg)
             output_names.extend(expr._output_names)
 
         return agg_pandas(
-            grouped,
+            self._grouped,
             exprs,
             self._keys,
             output_names,
             self._from_dataframe,
             implementation,
         )
 
@@ -66,14 +66,17 @@
         from narwhals._pandas_like.dataframe import PandasDataFrame
 
         return PandasDataFrame(
             df,
             implementation=self._df._implementation,
         )
 
+    def __iter__(self) -> Iterator[tuple[Any, PandasDataFrame]]:
+        return self._grouped.__iter__()  # type: ignore[no-any-return]
+
 
 def agg_pandas(  # noqa: PLR0913
     grouped: Any,
     exprs: list[PandasExpr],
     keys: list[str],
     output_names: list[str],
     from_dataframe: Callable[[Any], PandasDataFrame],
```

### Comparing `narwhals-0.8.7/narwhals/_pandas_like/namespace.py` & `narwhals-0.8.8/narwhals/_pandas_like/namespace.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/narwhals/_pandas_like/series.py` & `narwhals-0.8.8/narwhals/_pandas_like/series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/narwhals/_pandas_like/typing.py` & `narwhals-0.8.8/narwhals/_pandas_like/typing.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/narwhals/_pandas_like/utils.py` & `narwhals-0.8.8/narwhals/_pandas_like/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/conftest.py` & `narwhals-0.8.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/test_common.py` & `narwhals-0.8.8/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/test_dt.py` & `narwhals-0.8.8/tests/test_dt.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/test_group_by.py` & `narwhals-0.8.8/tests/test_group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/test_series.py` & `narwhals-0.8.8/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/test_str.py` & `narwhals-0.8.8/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/tpch_q1_test.py` & `narwhals-0.8.8/tests/tpch_q1_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/utils.py` & `narwhals-0.8.8/tests/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/data/customer.parquet` & `narwhals-0.8.8/tests/data/customer.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/data/lineitem.parquet` & `narwhals-0.8.8/tests/data/lineitem.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/data/nation.parquet` & `narwhals-0.8.8/tests/data/nation.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/data/orders.parquet` & `narwhals-0.8.8/tests/data/orders.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/data/part.parquet` & `narwhals-0.8.8/tests/data/part.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/data/partsupp.parquet` & `narwhals-0.8.8/tests/data/partsupp.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/data/region.parquet` & `narwhals-0.8.8/tests/data/region.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/data/supplier.parquet` & `narwhals-0.8.8/tests/data/supplier.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/expr/cum_sum_test.py` & `narwhals-0.8.8/tests/expr/cum_sum_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/expr/diff_test.py` & `narwhals-0.8.8/tests/expr/diff_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/expr/fill_null_test.py` & `narwhals-0.8.8/tests/expr/fill_null_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/expr/over_test.py` & `narwhals-0.8.8/tests/expr/over_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/expr/str/head_test.py` & `narwhals-0.8.8/tests/expr/str/head_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/expr/str/to_datetime_test.py` & `narwhals-0.8.8/tests/expr/str/to_datetime_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/frame/pipe_test.py` & `narwhals-0.8.8/tests/frame/pipe_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/hypothesis/test_basic_arithmetic.py` & `narwhals-0.8.8/tests/hypothesis/test_basic_arithmetic.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/hypothesis/test_concat.py` & `narwhals-0.8.8/tests/hypothesis/test_concat.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tests/hypothesis/test_join.py` & `narwhals-0.8.8/tests/hypothesis/test_join.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/q1.py` & `narwhals-0.8.8/tpch/q1.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/q2.py` & `narwhals-0.8.8/tpch/q2.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/q3.py` & `narwhals-0.8.8/tpch/q3.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/q4.py` & `narwhals-0.8.8/tpch/q4.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/q5.py` & `narwhals-0.8.8/tpch/q5.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/notebooks/gpu/execute.ipynb` & `narwhals-0.8.8/tpch/notebooks/gpu/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/notebooks/q1/execute.ipynb` & `narwhals-0.8.8/tpch/notebooks/q1/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/notebooks/q2/execute.ipynb` & `narwhals-0.8.8/tpch/notebooks/q2/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/notebooks/q3/execute.ipynb` & `narwhals-0.8.8/tpch/notebooks/q3/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/notebooks/q4/execute.ipynb` & `narwhals-0.8.8/tpch/notebooks/q4/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/notebooks/q5/execute.ipynb` & `narwhals-0.8.8/tpch/notebooks/q5/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/notebooks/q6/execute.ipynb` & `narwhals-0.8.8/tpch/notebooks/q6/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/notebooks/q7/execute.ipynb` & `narwhals-0.8.8/tpch/notebooks/q7/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/tpch/notebooks/q8/execute.ipynb` & `narwhals-0.8.8/tpch/notebooks/q8/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/utils/bump_version.py` & `narwhals-0.8.8/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/utils/check_api_reference.py` & `narwhals-0.8.8/utils/check_api_reference.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/LICENSE.md` & `narwhals-0.8.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/README.md` & `narwhals-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.8.7/pyproject.toml` & `narwhals-0.8.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "narwhals"
-version = "0.8.7"
+version = "0.8.8"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `narwhals-0.8.7/PKG-INFO` & `narwhals-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: narwhals
-Version: 0.8.7
+Version: 0.8.8
 Summary: Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin
 Project-URL: Homepage, https://github.com/MarcoGorelli/narwhals
 Project-URL: Bug Tracker, https://github.com/MarcoGorelli/narwhals
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

