# Comparing `tmp/Hydro-Quebec-API-Wrapper-3.1.3.tar.gz` & `tmp/hydro_quebec_api_wrapper-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hydro-Quebec-API-Wrapper-3.1.3.tar", last modified: Fri Jan 19 15:28:47 2024, max compression
+gzip compressed data, was "hydro_quebec_api_wrapper-3.2.0.tar", last modified: Fri May 10 15:59:41 2024, max compression
```

## Comparing `Hydro-Quebec-API-Wrapper-3.1.3.tar` & `hydro_quebec_api_wrapper-3.2.0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.360538 Hydro-Quebec-API-Wrapper-3.1.3/
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/.coveragerc
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.352538 Hydro-Quebec-API-Wrapper-3.1.3/.devcontainer/
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/.devcontainer/devcontainer.json
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     2077 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    11749 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1223 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    19948 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/.pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.360538 Hydro-Quebec-API-Wrapper-3.1.3/Hydro_Quebec_API_Wrapper.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7925 2024-01-19 15:28:47.000000 Hydro-Quebec-API-Wrapper-3.1.3/Hydro_Quebec_API_Wrapper.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2593 2024-01-19 15:28:47.000000 Hydro-Quebec-API-Wrapper-3.1.3/Hydro_Quebec_API_Wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-19 15:28:47.000000 Hydro-Quebec-API-Wrapper-3.1.3/Hydro_Quebec_API_Wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-01-19 15:28:47.000000 Hydro-Quebec-API-Wrapper-3.1.3/Hydro_Quebec_API_Wrapper.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       86 2024-01-19 15:28:47.000000 Hydro-Quebec-API-Wrapper-3.1.3/Hydro_Quebec_API_Wrapper.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-01-19 15:28:47.000000 Hydro-Quebec-API-Wrapper-3.1.3/Hydro_Quebec_API_Wrapper.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7925 2024-01-19 15:28:47.360538 Hydro-Quebec-API-Wrapper-3.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7133 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1081 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/config.default.yaml
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/conflict_test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.352538 Hydro-Quebec-API-Wrapper-3.1.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)      770 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.352538 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.352538 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)      133 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/_static/custom.css
--rw-rw-rw-   0 root         (0) root         (0)     6049 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/_static/hydroqc-logo-128.png
--rw-rw-rw-   0 root         (0) root         (0)     8268 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/_static/hydroqc-logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     2304 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.352538 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/external/
--rw-rw-rw-   0 root         (0) root         (0)   348837 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/external/description-des-codes-interruption.pdf
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.356538 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/
--rw-rw-rw-   0 root         (0) root         (0)     1781 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/hydroqc.contract.rst
--rw-rw-rw-   0 root         (0) root         (0)      685 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/hydroqc.hydro_api.rst
--rw-rw-rw-   0 root         (0) root         (0)      665 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/hydroqc.peak.cpc.rst
--rw-rw-rw-   0 root         (0) root         (0)      665 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/hydroqc.peak.dpc.rst
--rw-rw-rw-   0 root         (0) root         (0)      255 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/hydroqc.peak.rst
--rw-rw-rw-   0 root         (0) root         (0)     1503 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/hydroqc.rst
--rw-rw-rw-   0 root         (0) root         (0)     1359 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/hydroqc.types.rst
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/modules.rst
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/docs/source/todo.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.356538 Hydro-Quebec-API-Wrapper-3.1.3/examples/
--rwxrwxrwx   0 root         (0) root         (0)     2305 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/examples/hydro.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.356538 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3363 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/account.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/consts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.356538 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/
--rw-rw-rw-   0 root         (0) root         (0)      547 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15445 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/common.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_d.py
--rw-rw-rw-   0 root         (0) root         (0)     1328 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_d_cpc.py
--rw-rw-rw-   0 root         (0) root         (0)     4952 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_dpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1629 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_dt.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_m.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_m_gdp.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_residential.py
--rw-rw-rw-   0 root         (0) root         (0)     3978 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/outage.py
--rw-rw-rw-   0 root         (0) root         (0)     6165 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/customer.py
--rw-rw-rw-   0 root         (0) root         (0)    15516 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/diagnostic.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.356538 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/hydro_api/
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/hydro_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/hydro_api/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    33955 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/hydro_api/client.py
--rw-rw-rw-   0 root         (0) root         (0)     4432 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/hydro_api/consts.py
--rw-rw-rw-   0 root         (0) root         (0)     1255 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.356538 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/
--rw-rw-rw-   0 root         (0) root         (0)       19 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.356538 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/cpc/
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/cpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/cpc/consts.py
--rw-rw-rw-   0 root         (0) root         (0)    15695 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/cpc/handler.py
--rw-rw-rw-   0 root         (0) root         (0)     6700 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/cpc/peak.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.356538 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/dpc/
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/dpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/dpc/consts.py
--rw-rw-rw-   0 root         (0) root         (0)     8860 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/dpc/handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/dpc/peak.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     1136 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/timerange.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.360538 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/
--rw-rw-rw-   0 root         (0) root         (0)     1333 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3695 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/account.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/common.py
--rw-rw-rw-   0 root         (0) root         (0)     5928 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/consump.py
--rw-rw-rw-   0 root         (0) root         (0)     1656 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/contract.py
--rw-rw-rw-   0 root         (0) root         (0)     2115 2024-01-19 15:28:40.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/cpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/dpc.py
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/dt.py
--rw-rw-rw-   0 root         (0) root         (0)     3931 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/outage.py
--rw-rw-rw-   0 root         (0) root         (0)      232 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4410 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/webuser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.360538 Hydro-Quebec-API-Wrapper-3.1.3/logo/
--rw-rw-rw-   0 root         (0) root         (0)     6049 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/logo/hydroqc-logo-128.png
--rw-rw-rw-   0 root         (0) root         (0)     8268 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/logo/hydroqc-logo.svg
--rw-rw-rw-   0 root         (0) root         (0)      976 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     3413 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/renovate.json5
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-01-19 15:28:47.360538 Hydro-Quebec-API-Wrapper-3.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 15:28:47.360538 Hydro-Quebec-API-Wrapper-3.1.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      315 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    18360 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_common.py
--rw-rw-rw-   0 root         (0) root         (0)     2591 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_contract_d.py
--rw-rw-rw-   0 root         (0) root         (0)     8496 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_contract_d_cpc.py
--rw-rw-rw-   0 root         (0) root         (0)     6651 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_contract_dpc.py
--rw-rw-rw-   0 root         (0) root         (0)     4019 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_contract_dt.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_contract_m.py
--rw-rw-rw-   0 root         (0) root         (0)     3247 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_contract_m_gdp.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/tests/test_basic.py
--rw-rw-rw-   0 root         (0) root         (0)     3647 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/tests/test_timerange.py
--rw-rw-rw-   0 root         (0) root         (0)     4062 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/tests/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2036 2024-01-19 15:28:41.000000 Hydro-Quebec-API-Wrapper-3.1.3/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.050068 hydro_quebec_api_wrapper-3.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/.coveragerc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.046068 hydro_quebec_api_wrapper-3.2.0/.devcontainer/
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/.devcontainer/devcontainer.json
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    11725 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    19957 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/.pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.050068 hydro_quebec_api_wrapper-3.2.0/Hydro_Quebec_API_Wrapper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7925 2024-05-10 15:59:41.000000 hydro_quebec_api_wrapper-3.2.0/Hydro_Quebec_API_Wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2593 2024-05-10 15:59:41.000000 hydro_quebec_api_wrapper-3.2.0/Hydro_Quebec_API_Wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 15:59:41.000000 hydro_quebec_api_wrapper-3.2.0/Hydro_Quebec_API_Wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-10 15:59:41.000000 hydro_quebec_api_wrapper-3.2.0/Hydro_Quebec_API_Wrapper.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2024-05-10 15:59:41.000000 hydro_quebec_api_wrapper-3.2.0/Hydro_Quebec_API_Wrapper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-10 15:59:41.000000 hydro_quebec_api_wrapper-3.2.0/Hydro_Quebec_API_Wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7925 2024-05-10 15:59:41.050068 hydro_quebec_api_wrapper-3.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7133 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/config.default.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/conflict_test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.046068 hydro_quebec_api_wrapper-3.2.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      770 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.046068 hydro_quebec_api_wrapper-3.2.0/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.046068 hydro_quebec_api_wrapper-3.2.0/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/_static/custom.css
+-rw-rw-rw-   0 root         (0) root         (0)     6049 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/_static/hydroqc-logo-128.png
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/_static/hydroqc-logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.046068 hydro_quebec_api_wrapper-3.2.0/docs/source/external/
+-rw-rw-rw-   0 root         (0) root         (0)   348837 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/external/description-des-codes-interruption.pdf
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.046068 hydro_quebec_api_wrapper-3.2.0/docs/source/reference/
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/reference/hydroqc.contract.rst
+-rw-rw-rw-   0 root         (0) root         (0)      685 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/reference/hydroqc.hydro_api.rst
+-rw-rw-rw-   0 root         (0) root         (0)      665 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/reference/hydroqc.peak.cpc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      665 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/reference/hydroqc.peak.dpc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      255 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/reference/hydroqc.peak.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/reference/hydroqc.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/reference/hydroqc.types.rst
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/reference/modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/docs/source/todo.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.046068 hydro_quebec_api_wrapper-3.2.0/examples/
+-rwxrwxrwx   0 root         (0) root         (0)     2319 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/examples/hydro.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.050068 hydro_quebec_api_wrapper-3.2.0/hydroqc/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3364 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/account.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/consts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.050068 hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/
+-rw-rw-rw-   0 root         (0) root         (0)      548 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15446 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_d.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_d_cpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4953 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_dpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_dt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_m.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_m_gdp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_residential.py
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/outage.py
+-rw-rw-rw-   0 root         (0) root         (0)     6166 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/customer.py
+-rw-rw-rw-   0 root         (0) root         (0)    15517 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/diagnostic.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.050068 hydro_quebec_api_wrapper-3.2.0/hydroqc/hydro_api/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/hydro_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/hydro_api/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    33956 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/hydro_api/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/hydro_api/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.050068 hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.050068 hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/cpc/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/cpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/cpc/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)    15696 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/cpc/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     6701 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/cpc/peak.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.050068 hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/dpc/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/dpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      555 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/dpc/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     8861 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/dpc/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/dpc/peak.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     1137 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/timerange.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.050068 hydro_quebec_api_wrapper-3.2.0/hydroqc/types/
+-rw-rw-rw-   0 root         (0) root         (0)     1334 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3696 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/types/account.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/types/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     5929 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/types/consump.py
+-rw-rw-rw-   0 root         (0) root         (0)     1657 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/types/contract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2116 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/types/cpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/types/dpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/types/dt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3932 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/types/outage.py
+-rw-rw-rw-   0 root         (0) root         (0)      232 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4411 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/hydroqc/webuser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.050068 hydro_quebec_api_wrapper-3.2.0/logo/
+-rw-rw-rw-   0 root         (0) root         (0)     6049 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/logo/hydroqc-logo-128.png
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/logo/hydroqc-logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     3463 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/renovate.json5
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-10 15:59:41.054069 hydro_quebec_api_wrapper-3.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:59:41.050068 hydro_quebec_api_wrapper-3.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      316 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    18361 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/tests/subtest_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     2592 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/tests/subtest_contract_d.py
+-rw-rw-rw-   0 root         (0) root         (0)     8497 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/tests/subtest_contract_d_cpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6652 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/tests/subtest_contract_dpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4020 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/tests/subtest_contract_dt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3468 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/tests/subtest_contract_m.py
+-rw-rw-rw-   0 root         (0) root         (0)     3248 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/tests/subtest_contract_m_gdp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1805 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/tests/test_basic.py
+-rw-rw-rw-   0 root         (0) root         (0)     3648 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/tests/test_timerange.py
+-rw-rw-rw-   0 root         (0) root         (0)     4063 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/tests/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2024-05-10 15:59:30.000000 hydro_quebec_api_wrapper-3.2.0/tox.ini
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/.gitignore` & `hydro_quebec_api_wrapper-3.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/.gitlab-ci.yml` & `hydro_quebec_api_wrapper-3.2.0/.gitlab-ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -26,18 +26,17 @@
         - renovate.json5
       when: on_success
     - when: never
 
 test:
   stage: test
   tags:
-    - hydroqc
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.11@sha256:e6ef50dbb2f351fbd4e20c39512885bdcd62d202f05c8558a4d40ac2d9836763
+   - hydroqc
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.12@sha256:b66812346075aabc0ee6cf452d734c28589bbe97a82c179b0a95d3a95c04ad41
   script:
-    - pip install tox
     - tox -e pylint,flake8,pydocstyle,typing,black,deps-conflict --parallel auto
     - cat mypy-txt-report/index.txt
   artifacts:
     reports:
       junit: mypy-junit.xml
     paths:
       - mypy-txt-report/
@@ -64,19 +63,19 @@
     # Make it manual for external MR
     - if: "$CI_MERGE_REQUEST_IID && $CI_MERGE_REQUEST_PROJECT_PATH != $CI_MERGE_REQUEST_SOURCE_PROJECT_PATH"
       when: manual
     - when: never
 
 .private_test_script: &private_test_script
   stage: private_tests
-  tags:
-    - hydroqc
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.11@sha256:e6ef50dbb2f351fbd4e20c39512885bdcd62d202f05c8558a4d40ac2d9836763
+  # Run on shared runners to lighten the load on the private runners
+  # tags:
+  # - hydroqc
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.12@sha256:b66812346075aabc0ee6cf452d734c28589bbe97a82c179b0a95d3a95c04ad41
   script:
-    #- apt update && apt install -y jq unzip curl
     - >
       OUTPUT=$(curl
       --globoff
       --header "Content-Type: application/json"
       --header "PRIVATE-TOKEN: ${HYDROQC_SA_TOKEN}"
       "https://gitlab.com/api/v4/projects/${PROJECT_ID}")
     - PROJECT_PATH=$(echo ${OUTPUT} | jq -r .path_with_namespace)
@@ -254,19 +253,18 @@
       when: never
     - !reference [.private_test_script, rules]
 
 private_tests_done:
   stage: private_tests_done
   tags:
     - hydroqc
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.11@sha256:e6ef50dbb2f351fbd4e20c39512885bdcd62d202f05c8558a4d40ac2d9836763
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.12@sha256:b66812346075aabc0ee6cf452d734c28589bbe97a82c179b0a95d3a95c04ad41
   script:
     #- apt-get update && apt-get install --no-install-recommends -y python3.10 python3-venv python3-pip --no-install-recommends git
     - echo "Private Tests done"
-    - pip install tox
     - find .
     - mv -v hydroqc/.coverage* .
     - mv -v hydroqc/*.xml .
     - tox -e cov-combine,cov-report
     - ls -al
   coverage: '/TOTAL.*\s+(\d+%)$/'
   artifacts:
@@ -297,15 +295,15 @@
       when: manual
     - when: never
 
 package:
   stage: test
   tags:
     - hydroqc
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.11@sha256:e6ef50dbb2f351fbd4e20c39512885bdcd62d202f05c8558a4d40ac2d9836763
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.12@sha256:b66812346075aabc0ee6cf452d734c28589bbe97a82c179b0a95d3a95c04ad41
   script:
     # Build a package with a version based on the commmit short sha
     - pip install --upgrade pip
     - pip install --upgrade build setuptools wheel twine setuptools_scm
     - python3 -m build -o dist
     - python3 -m twine check --strict dist/*
     - TWINE_PASSWORD=${CI_JOB_TOKEN} TWINE_USERNAME=gitlab-ci-token python3 -m twine upload --verbose --repository-url ${CI_API_V4_URL}/projects/${CI_PROJECT_ID}/packages/pypi dist/*
@@ -327,15 +325,15 @@
       when: manual
     - when: never
 
 promote2pypi:
   stage: pypi
   tags:
     - hydroqc
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.11@sha256:e6ef50dbb2f351fbd4e20c39512885bdcd62d202f05c8558a4d40ac2d9836763
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.12@sha256:b66812346075aabc0ee6cf452d734c28589bbe97a82c179b0a95d3a95c04ad41
   script:
     # TODO: try to pull the good package from gitlab pypi repo
     #       then change the version (promote)
     #       then push it to pypi
     #- rm -rf dist
     #- mkdir -p dist
     #- cd dist
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/.pylintrc` & `hydro_quebec_api_wrapper-3.2.0/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -272,11 +272,11 @@
 int-import-graph=
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
 
 max-nested-blocks=7
 max-bool-expr=10
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/Hydro_Quebec_API_Wrapper.egg-info/PKG-INFO` & `hydro_quebec_api_wrapper-3.2.0/Hydro_Quebec_API_Wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: Hydro-Quebec-API-Wrapper
-Version: 3.1.3
+Version: 3.2.0
 Summary: A wrapper library to access hydro quebec API and more
 Home-page: https://hydroqc.ca
 Author-email: Hydroqc Team <info@hydroqc.ca>
 License: LGPL-3.0-or-later
 Project-URL: Source Code, https://gitlab.com/hydroqc/hydroqc
 Project-URL: Bug Reports, https://gitlab.com/hydroqc/hydroqc/-/issues
 Project-URL: Home-page, https://hydroqc.ca
 Keywords: hydroquebec,lib
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp==3.9.1
-Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: pytz==2023.3.post1
+Requires-Dist: aiohttp==3.9.5
+Requires-Dist: python-dateutil==2.9.0.post0
+Requires-Dist: pytz==2024.1
 Requires-Dist: aiocache==0.12.2
 Requires-Dist: pkce==1.0.3
 
 # HydroQC - Hydro Quebec API wrapper
 
 
 [![coverage report](https://gitlab.com/hydroqc/hydroqc/badges/main/coverage.svg)](https://gitlab.com/hydroqc/hydroqc/-/commits/main)
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/Hydro_Quebec_API_Wrapper.egg-info/SOURCES.txt` & `hydro_quebec_api_wrapper-3.2.0/Hydro_Quebec_API_Wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/LICENSE` & `hydro_quebec_api_wrapper-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/PKG-INFO` & `hydro_quebec_api_wrapper-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: Hydro-Quebec-API-Wrapper
-Version: 3.1.3
+Version: 3.2.0
 Summary: A wrapper library to access hydro quebec API and more
 Home-page: https://hydroqc.ca
 Author-email: Hydroqc Team <info@hydroqc.ca>
 License: LGPL-3.0-or-later
 Project-URL: Source Code, https://gitlab.com/hydroqc/hydroqc
 Project-URL: Bug Reports, https://gitlab.com/hydroqc/hydroqc/-/issues
 Project-URL: Home-page, https://hydroqc.ca
 Keywords: hydroquebec,lib
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: aiohttp==3.9.1
-Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: pytz==2023.3.post1
+Requires-Dist: aiohttp==3.9.5
+Requires-Dist: python-dateutil==2.9.0.post0
+Requires-Dist: pytz==2024.1
 Requires-Dist: aiocache==0.12.2
 Requires-Dist: pkce==1.0.3
 
 # HydroQC - Hydro Quebec API wrapper
 
 
 [![coverage report](https://gitlab.com/hydroqc/hydroqc/badges/main/coverage.svg)](https://gitlab.com/hydroqc/hydroqc/-/commits/main)
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/README.md` & `hydro_quebec_api_wrapper-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/config.default.yaml` & `hydro_quebec_api_wrapper-3.2.0/config.default.yaml`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/docs/Makefile` & `hydro_quebec_api_wrapper-3.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/docs/make.bat` & `hydro_quebec_api_wrapper-3.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/docs/source/_static/hydroqc-logo-128.png` & `hydro_quebec_api_wrapper-3.2.0/docs/source/_static/hydroqc-logo-128.png`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/docs/source/_static/hydroqc-logo.svg` & `hydro_quebec_api_wrapper-3.2.0/docs/source/_static/hydroqc-logo.svg`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/docs/source/conf.py` & `hydro_quebec_api_wrapper-3.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/docs/source/external/description-des-codes-interruption.pdf` & `hydro_quebec_api_wrapper-3.2.0/docs/source/external/description-des-codes-interruption.pdf`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/hydroqc.contract.rst` & `hydro_quebec_api_wrapper-3.2.0/docs/source/reference/hydroqc.contract.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/hydroqc.hydro_api.rst` & `hydro_quebec_api_wrapper-3.2.0/docs/source/reference/hydroqc.hydro_api.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/hydroqc.peak.cpc.rst` & `hydro_quebec_api_wrapper-3.2.0/docs/source/reference/hydroqc.peak.cpc.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/hydroqc.peak.dpc.rst` & `hydro_quebec_api_wrapper-3.2.0/docs/source/reference/hydroqc.peak.dpc.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/hydroqc.rst` & `hydro_quebec_api_wrapper-3.2.0/docs/source/reference/hydroqc.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/docs/source/reference/hydroqc.types.rst` & `hydro_quebec_api_wrapper-3.2.0/docs/source/reference/hydroqc.types.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/examples/hydro.py` & `hydro_quebec_api_wrapper-3.2.0/examples/hydro.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,17 @@
     print(data)
     data = await contract.get_today_daily_consumption()
     print(data)
     data = await contract.get_monthly_consumption()
     print(data)
     data = await contract.get_annual_consumption()
     print(data)
-    data = await contract.get_daily_consumption(date.fromisoformat("2022-01-10"), date.fromisoformat("2022-01-20"))
+    data = await contract.get_daily_consumption(
+        date.fromisoformat("2022-01-10"), date.fromisoformat("2022-01-20")
+    )
     print(data)
 
 
 loop = asyncio.get_event_loop()
 
 
 # Fetch data
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/account.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroquebec Account Module."""
+
 from hydroqc.contract.common import Contract
 from hydroqc.error import HydroQcError
 from hydroqc.hydro_api.client import HydroClient
 from hydroqc.logger import get_logger
 from hydroqc.types import ContractTyping, ListAccountsContractsTyping
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/__init__.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contracts module."""
+
 from hydroqc.contract.common import ContractFallBack
 from hydroqc.contract.contract_d import ContractD
 from hydroqc.contract.contract_d_cpc import ContractDCPC
 from hydroqc.contract.contract_dpc import ContractDPC
 from hydroqc.contract.contract_dt import ContractDT
 from hydroqc.contract.contract_m import ContractM
 from hydroqc.contract.contract_m_gdp import ContractMGDP
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/common.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroquebec contract module."""
+
 import functools
 import logging
 from abc import ABC
 from collections.abc import Callable, Iterator
 from datetime import date, datetime, timedelta
 from io import StringIO
 from typing import ParamSpec, TypeVar, cast
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_d.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroquebec contract module."""
+
 from hydroqc.contract.contract_residential import ContractResidential
 from hydroqc.hydro_api.client import HydroClient
 
 
 class ContractD(ContractResidential):
     """Hydroquebec contract.
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_d_cpc.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_d_cpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroquebec contract module."""
+
 from hydroqc.contract.contract_d import ContractD
 from hydroqc.hydro_api.client import HydroClient
 from hydroqc.peak.cpc.handler import CPCPeakHandler
 
 
 class ContractDCPC(ContractD):
     """Hydroquebec contract.
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_dpc.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_dpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroquebec contract module."""
+
 from collections.abc import Callable
 from datetime import date
 
 from hydroqc.contract.common import check_period_data_present
 from hydroqc.contract.contract_residential import ContractResidential
 from hydroqc.hydro_api.client import HydroClient
 from hydroqc.peak.dpc.handler import DPCPeakHandler
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_dt.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_dt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroquebec contract module."""
+
 from hydroqc.contract.common import check_annual_data_present, check_period_data_present
 from hydroqc.contract.contract_residential import ContractResidential
 from hydroqc.hydro_api.client import HydroClient
 
 
 class ContractDT(ContractResidential):
     """Hydroquebec contract.
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_m.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_m.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroquebec contract module."""
+
 from collections.abc import Iterator
 from datetime import date
 from io import StringIO
 
 from hydroqc.contract.common import Contract
 from hydroqc.hydro_api.client import HydroClient
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_m_gdp.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_m_gdp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroquebec contract module."""
+
 from hydroqc.contract.contract_m import ContractM
 from hydroqc.hydro_api.client import HydroClient
 
 
 class ContractMGDP(ContractM):
     """Hydroquebec contract.
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/contract_residential.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/contract_residential.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroquebec contract module."""
+
 from collections.abc import Iterator
 from datetime import date
 from io import StringIO
 
 from hydroqc.contract.common import Contract
 from hydroqc.hydro_api.client import HydroClient
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/contract/outage.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/contract/outage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """HydroQC planned and not planned Outage module.
 
 See:
     * https://www.hydroquebec.com/documents-donnees/donnees-ouvertes/pannes-interruptions.html
     * https://infopannes.solutions.hydroquebec.com/statut-adresse/
     * https://www.hydroquebec.com/data/loi-sur-acces/pdf/description-des-codes-interruption.pdf
 """
+
 import datetime
 import logging
 
 from hydroqc import utils
 from hydroqc.types import OutageCause, OutageCode, OutageStatus, OutageTyping
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/customer.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/customer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroquebec customer module."""
+
 import logging
 
 from hydroqc import contract as contractModule
 from hydroqc.account import Account
 from hydroqc.error import HydroQcError
 from hydroqc.hydro_api.client import HydroClient
 from hydroqc.logger import get_logger
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/diagnostic.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/diagnostic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Diagnostic module to help users to send debug to devs."""
+
 import argparse
 import asyncio
 import copy
 import datetime
 import io
 import logging
 import os
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/error.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/error.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/hydro_api/cache.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/hydro_api/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custon cache module."""
+
 import functools
 from collections.abc import Callable
 from typing import ParamSpec, TypeVar, cast
 
 from aiocache import Cache, cached  # type: ignore
 
 T = TypeVar("T")
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/hydro_api/client.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/hydro_api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """HydroQc Client Module."""
+
 import base64
 import csv
 import json
 import logging
 import os
 import platform
 import re
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/hydro_api/consts.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/hydro_api/consts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Hydroqc API Consts.
 
 .. todo::
 
     avoid all the /portail/ URLs
 """
+
 # Always get the time using HydroQuebec Local Time
 REQUESTS_TIMEOUT = 30
 REQUESTS_TTL = 1
 
 HOST_LOGIN = "https://connexion.solutions.hydroquebec.com"
 HOST_SESSION = "https://session.hydroquebec.com"
-HOST_SERVICES = "https://cl-services.solutions.hydroquebec.com"
-HOST_SPRING = "https://cl-ec-lsw.solutions.hydroquebec.com"
+HOST_SERVICES = "https://services-cl.solutions.hydroquebec.com"
+# HOST_SPRING = "https://cl-ec-lsw.solutions.hydroquebec.com"
 HOST_RB_SOL = "https://rb.solutions.hydroquebec.com"
 HOST_OUTAGES = "https://services-bs.solutions.hydroquebec.com"
 
 # Azure B2C
 AZB2C_TENANT_ID = "32bf9b91-0a36-4385-b231-d9a8fa3b05ab"
 AZB2C_POLICY = "B2C_1A_PRD_signup_signin"
 AZB2C_CLIENT_ID_WEB = "09b0ae72-6db8-4ecc-a1be-041b67afc1cd"
@@ -40,86 +41,86 @@
 TOKEN_URL = f"{HOST_LOGIN}/{AZB2C_TENANT_ID}/{AZB2C_POLICY.lower()}/oauth2/v2.0/token"
 
 CHECK_SESSION_URL = f"{HOST_LOGIN}/hqam/oauth2/connect/checkSession"
 
 
 SECURITY_URL = f"{HOST_SESSION}/config/security.json"
 SESSION_REFRESH_URL = f"{HOST_SESSION}/oauth2/callback/silent-refresh"
-LOGIN_URL_6 = f"{HOST_SERVICES}/web/prive/api/v3_0/conversion/codeAcces"
+LOGIN_URL_6 = f"{HOST_SERVICES}/wsapi/web/prive/api/v3_0/conversion/codeAcces"
 
 # Initialization uri
-RELATION_URL = f"{HOST_SERVICES}/web/prive/api/v1_0/relations"
+RELATION_URL = f"{HOST_SERVICES}/wsapi/web/prive/api/v1_0/relations"
 
 FLEXD_DATA_URL = (
-    f"{HOST_SPRING}/portail/fr/group/clientele/portrait-de-consommation/"
+    f"{HOST_SERVICES}/lsw/portail/fr/group/clientele/portrait-de-consommation/"
     "resourceObtenirDonneesMoisHiverFlex"
 )
-FLEXD_PEAK_URL = f"{HOST_RB_SOL}/portraitweb/api/v3_0/conso"
+FLEXD_PEAK_URL = f"{HOST_SERVICES}/conso/portraitweb/api/v3_0/conso"
 CONSO_CSV_URL = (
-    f"{HOST_SPRING}/portail/fr/group/clientele/portrait-de-consommation/"
+    f"{HOST_SERVICES}/lsw/portail/fr/group/clientele/portrait-de-consommation/"
     "resourceTelechargerDonneesConsommation"
 )
 CONSO_OVERVIEW_CSV_URL = (
-    f"{HOST_SPRING}/portail/en/group/clientele/portrait-de-consommation/"
+    f"{HOST_SERVICES}/lsw/portail/en/group/clientele/portrait-de-consommation/"
     "resourceTelechargerPeriodesFacturation"
 )
 
 # TODO avoid all the /portail/ URLs
-SESSION_URL = f"{HOST_SPRING}/portail/prive/maj-session/"
+SESSION_URL = f"{HOST_SERVICES}/lsw/portail/prive/maj-session/"
 # TODO avoid all the /portail/ URLs
-CONTRACT_HTML_URL = f"{HOST_SPRING}/portail/fr/group/clientele/gerer-mon-compte"
+CONTRACT_HTML_URL = f"{HOST_SERVICES}/lsw/portail/fr/group/clientele/gerer-mon-compte"
 #
-INFOBASE_URL = f"{HOST_SERVICES}/web/prive/api/v3_0/partenaires/infoBase"
+INFOBASE_URL = f"{HOST_SERVICES}/wsapi/web/prive/api/v3_0/partenaires/infoBase"
 CONTRACT_SUMMARY_URL = (
-    f"{HOST_SERVICES}/web/prive/api/v3_0/partenaires/"
+    f"{HOST_SERVICES}/wsapi/web/prive/api/v3_0/partenaires/"
     "calculerSommaireContractuel?indMAJNombres=true"
 )
-CONTRACT_LIST_URL = f"{HOST_SERVICES}/web/prive/api/v3_0/partenaires/contrats"
-# CONTRACT_URL_4 = (f"{HOST_SERVICES}/web/prive/api/v3_0/partenaires/"
-#                  "calculerSommaireContractuel")
+CONTRACT_LIST_URL = f"{HOST_SERVICES}/wsapi/web/prive/api/v3_0/partenaires/contrats"
 
-CUSTOMER_INFO_URL = f"{HOST_SERVICES}/web/prive/api/v3_0/partenaires/infoCompte"
+CUSTOMER_INFO_URL = f"{HOST_SERVICES}/wsapi/web/prive/api/v3_0/partenaires/infoCompte"
 
 # TODO avoid all the /portail/ URLs
-PORTRAIT_URL = f"{HOST_SPRING}/portail/fr/group/clientele/portrait-de-consommation"
+PORTRAIT_URL = (
+    f"{HOST_SERVICES}/lsw/portail/fr/group/clientele/portrait-de-consommation"
+)
 # TODO avoid all the /portail/ URLs
 PERIOD_DATA_URL = (
-    f"{HOST_SPRING}/portail/fr/group/clientele/portrait-de-consommation/"
+    f"{HOST_SERVICES}/lsw/portail/fr/group/clientele/portrait-de-consommation/"
     "resourceObtenirDonneesPeriodesConsommation"
 )
 
 # TODO avoid all the /portail/ URLs
 ANNUAL_DATA_URL = (
-    f"{HOST_SPRING}/portail/fr/group/clientele/portrait-de-consommation/"
+    f"{HOST_SERVICES}/lsw/portail/fr/group/clientele/portrait-de-consommation/"
     "resourceObtenirDonneesConsommationAnnuelles"
 )
 
 # TODO avoid all the /portail/ URLs
 MONTHLY_DATA_URL = (
-    f"{HOST_SPRING}/portail/fr/group/clientele/portrait-de-consommation/"
+    f"{HOST_SERVICES}/lsw/portail/fr/group/clientele/portrait-de-consommation/"
     "resourceObtenirDonneesConsommationMensuelles"
 )
 
 # TODO avoid all the /portail/ URLs
 DAILY_CONSUMPTION_API_URL = (
-    f"{HOST_SPRING}/portail/fr/group/clientele/portrait-de-consommation/"
+    f"{HOST_SERVICES}/lsw/portail/fr/group/clientele/portrait-de-consommation/"
     "resourceObtenirDonneesQuotidiennesConsommation"
 )
 
 # TODO avoid all the /portail/ URLs
 HOURLY_CONSUMPTION_API_URL = (
-    f"{HOST_SPRING}/portail/fr/group/clientele/portrait-de-consommation/"
+    f"{HOST_SERVICES}/lsw/portail/fr/group/clientele/portrait-de-consommation/"
     "resourceObtenirDonneesConsommationHoraires"
 )
 # TODO avoid all the /portail/ URLs
 HOURLY_DATA_URL_2 = (
-    f"{HOST_SPRING}/portail/fr/group/clientele/portrait-de-consommation/"
+    f"{HOST_SERVICES}/lsw/portail/fr/group/clientele/portrait-de-consommation/"
     "resourceObtenirDonneesMeteoHoraires"  # not used
 )
 
 # CPC
 GET_CPC_API_URL = (
-    f"{HOST_SERVICES}/web/prive/api/v3_0/tarificationDynamique/creditPointeCritique"
+    f"{HOST_SERVICES}/wsapi/web/prive/api/v3_0/tarificationDynamique/"
+    "creditPointeCritique"
 )
-
 # IS PORTAL RUNNING
 IS_HYDRO_PORTAL_UP_URL = f"{HOST_SESSION}/portail/fr/group/clientele/gerer-mon-compte"
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/logger.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Logging module."""
+
 import logging
 
 from hydroqc.consts import LOGGING_LEVELS
 from hydroqc.error import HydroQcError
 
 
 def get_logger(
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/cpc/consts.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/cpc/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Constants module for CPC."""
+
 # from typing import Literal
 import datetime
 
 DEFAULT_ANCHOR_START_OFFSET = 5
 DEFAULT_ANCHOR_DURATION = 3
 DEFAULT_EVENT_REFRESH_SECONDS = 300
 DEFAULT_PRE_HEAT_DURATION = 180
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/cpc/handler.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/cpc/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CPC processing."""
+
 import datetime
 import logging
 
 from hydroqc import utils
 from hydroqc.error import HydroQcCPCPeakError
 from hydroqc.hydro_api.client import HydroClient
 from hydroqc.peak.cpc.consts import (
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/cpc/peak.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/cpc/peak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class describing a period."""
+
 import datetime
 
 from hydroqc.error import HydroQcCPCPeakError
 from hydroqc.peak.cpc.consts import (
     DEFAULT_ANCHOR_DURATION,
     DEFAULT_ANCHOR_START_OFFSET,
     DEFAULT_EVENING_PEAK_END,
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/dpc/consts.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/dpc/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Constants module for winter credits."""
+
 # from typing import Literal
 import datetime
 
 DEFAULT_ANCHOR_START_OFFSET = 5
 DEFAULT_ANCHOR_DURATION = 3
 DEFAULT_EVENT_REFRESH_SECONDS = 300
 DEFAULT_PRE_HEAT_DURATION = 180
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/dpc/handler.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/dpc/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """DPC processing."""
+
 import datetime
 import logging
 
 from hydroqc import utils
 from hydroqc.error import HydroQcDPCPeakError
 from hydroqc.hydro_api.client import HydroClient
 from hydroqc.peak.dpc.consts import DEFAULT_PRE_HEAT_DURATION
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/peak/dpc/peak.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/peak/dpc/peak.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class describing a period."""
+
 import datetime
 
 from hydroqc.peak.dpc.consts import DEFAULT_PRE_HEAT_DURATION
 from hydroqc.timerange import TimeRange
 from hydroqc.utils import EST_TIMEZONE
 
 __all__ = ["PreHeat", "Peak"]
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/timerange.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/timerange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class describing an interval of time."""
+
 import datetime
 
 
 class TimeRange:
     """This class describe an interval of time."""
 
     def __init__(
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/__init__.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroqc custom types."""
+
 from hydroqc.types.account import (
     AccountContractSummaryTyping,
     AccountTyping,
     InfoAccountTyping,
     ListAccountsContractsTyping,
 )
 from hydroqc.types.common import IDTokenTyping, Rates
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/account.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/types/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Info account json output formats."""
+
 # pylint: disable=invalid-name
 from typing import Any, TypedDict
 
 from hydroqc.types.contract import ContractTyping
 
 
 # https://cl-services.idp.hydroquebec.com/cl/prive/api/v1_0/relations
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/common.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/types/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common types."""
+
 # pylint: disable=invalid-name
 from enum import Enum
 from typing import TypedDict
 
 
 class IDTokenTyping(TypedDict, total=True):
     """ID token output format."""
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/consump.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/types/consump.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroqc custom types."""
+
 # pylint: disable=invalid-name
 from typing import TypedDict
 
 
 # API URL: https://cl-ec-spring.hydroquebec.com/portail/fr/group/clientele/
 # portrait-de-consommation/resourceObtenirDonneesConsommationHoraires
 class ConsumpHourlyResultTyping(TypedDict, total=True):
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/contract.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/types/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contract json output formats."""
+
 # pylint: disable=invalid-name
 from typing import TypedDict
 
 
 class ContractTyping(TypedDict, total=True):
     """Contract json output formats."""
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/cpc.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/types/cpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroqc custom types."""
+
 from typing import TypedDict
 
 
 class PeriodDataTyping(TypedDict, total=True):
     """CPC Period json output format."""
 
     nbJourLecturePeriode: int
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/dpc.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/types/dpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroqc DPC types."""
+
 # pylint: disable=invalid-name
 from typing import TypedDict
 
 
 class DPCDataResultsTyping(TypedDict, total=True):
     """FlexD data json sub output format."""
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/types/outage.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/types/outage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Outage output formats."""
+
 # pylint: disable=invalid-name
 from enum import Enum, IntEnum
 from typing import TypedDict
 
 # Outages
 
 # Outage example
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/hydroqc/webuser.py` & `hydro_quebec_api_wrapper-3.2.0/hydroqc/webuser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hydroquebec webuser module."""
+
 import logging
 
 from hydroqc.customer import Customer
 from hydroqc.error import HydroQcError
 from hydroqc.hydro_api.client import HydroClient
 from hydroqc.logger import get_logger
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/logo/hydroqc-logo-128.png` & `hydro_quebec_api_wrapper-3.2.0/logo/hydroqc-logo-128.png`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/logo/hydroqc-logo.svg` & `hydro_quebec_api_wrapper-3.2.0/logo/hydroqc-logo.svg`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/pyproject.toml` & `hydro_quebec_api_wrapper-3.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
-    "setuptools==69.0.3",
-    "setuptools_scm[toml]==8.0.4",
-    "wheel==0.42.0",
+    "setuptools==69.5.1",
+    "setuptools_scm[toml]==8.1.0",
+    "wheel==0.43.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Hydro-Quebec-API-Wrapper"
 dynamic = ["version", "dependencies"]
 description = "A wrapper library to access hydro quebec API and more"
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/renovate.json5` & `hydro_quebec_api_wrapper-3.2.0/renovate.json5`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7336309523809523%*

 * *Differences: {"'extends'": "{insert: [(2, ':disableRateLimiting')]}",*

 * * "'packageRules'": "{6: {'automergeType': 'branch'}}",*

 * * "'platformAutomerge'": 'True',*

 * * 'delete': "['platform']"}*

```diff
@@ -14,14 +14,15 @@
             ],
             "versioningTemplate": "pep440"
         }
     ],
     "extends": [
         "config:recommended",
         ":dependencyDashboard",
+        ":disableRateLimiting",
         ":gitSignOff"
     ],
     "packageRules": [
         {
             "automerge": true,
             "groupName": "Python devDependencies - non-major",
             "groupSlug": "python-devdeps-nonmajor",
@@ -146,23 +147,23 @@
             ],
             "matchUpdateTypes": [
                 "major"
             ]
         },
         {
             "automerge": true,
-            "automergeType": "pr",
+            "automergeType": "branch",
             "description": "Auto merge container digests",
             "ignoreTests": false,
             "matchDatasources": [
                 "docker"
             ],
             "matchUpdateTypes": [
                 "digest"
             ]
         }
     ],
-    "platform": "gitlab",
+    "platformAutomerge": true,
     "pre-commit": {
         "enabled": true
     }
 }
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_common.py` & `hydro_quebec_api_wrapper-3.2.0/tests/subtest_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Basics tests for hydroqc."""
+
 import asyncio
 import datetime
 import typing
 
 import pytest
 
 from hydroqc.account import Account
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_contract_d.py` & `hydro_quebec_api_wrapper-3.2.0/tests/subtest_contract_d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contract D tests module."""
+
 import pytest
 
 from hydroqc.contract import ContractD
 
 from .tools import SkipIfBadRate, today, yesterday
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_contract_d_cpc.py` & `hydro_quebec_api_wrapper-3.2.0/tests/subtest_contract_d_cpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contract D CPC tests module."""
+
 import datetime
 
 import pytest
 
 from hydroqc.account import Account
 from hydroqc.contract import ContractDCPC
 from hydroqc.peak.cpc.consts import (
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_contract_dpc.py` & `hydro_quebec_api_wrapper-3.2.0/tests/subtest_contract_dpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contract DPC tests module."""
+
 import datetime
 
 import pytest
 
 from hydroqc.contract import ContractDPC
 
 from .tools import SkipIfBadRate, today, yesterday
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_contract_dt.py` & `hydro_quebec_api_wrapper-3.2.0/tests/subtest_contract_dt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contract DT tests module."""
+
 from types import NoneType
 
 import pytest
 
 from hydroqc.contract import ContractDT
 
 from .tools import SkipIfBadRate, today, yesterday
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_contract_m.py` & `hydro_quebec_api_wrapper-3.2.0/tests/subtest_contract_m.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contract M tests module."""
+
 import pytest
 
 from hydroqc.contract import ContractM
 
 from .tools import SkipIfBadRate, today, yesterday
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/tests/subtest_contract_m_gdp.py` & `hydro_quebec_api_wrapper-3.2.0/tests/subtest_contract_m_gdp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contract M GDP tests module."""
+
 import pytest
 
 from hydroqc.contract import ContractMGDP
 
 from .tools import SkipIfBadRate, today, yesterday
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/tests/test_basic.py` & `hydro_quebec_api_wrapper-3.2.0/tests/test_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Basics tests for hydroqc."""
+
 import parameterized  # type: ignore
 
 from .subtest_common import SubTestCommon
 from .subtest_contract_d import SubTestContractD
 from .subtest_contract_d_cpc import SubTestContractDCPC
 from .subtest_contract_dpc import SubTestContractDPC
 from .subtest_contract_dt import SubTestContractDT
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/tests/test_timerange.py` & `hydro_quebec_api_wrapper-3.2.0/tests/test_timerange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """TimeRange tests for hydroqc."""
+
 import datetime
 
 import pytest
 
 from hydroqc.error import HydroQcCPCPeakError
 from hydroqc.peak.cpc.peak import Anchor, Peak, PreHeat
 from hydroqc.peak.dpc.peak import Peak as DPCPeak
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/tests/tools.py` & `hydro_quebec_api_wrapper-3.2.0/tests/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test tools."""
+
 import datetime
 import functools
 import os
 from collections.abc import Callable
 from typing import ParamSpec, TypeVar, cast
 
 import pytest
```

### Comparing `Hydro-Quebec-API-Wrapper-3.1.3/tox.ini` & `hydro_quebec_api_wrapper-3.2.0/tox.ini`

 * *Files identical despite different names*

