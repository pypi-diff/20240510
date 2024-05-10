# Comparing `tmp/zynapse-0.1.0.tar.gz` & `tmp/zynapse-0.1.1.tar.gz`

## Comparing `zynapse-0.1.0.tar` & `zynapse-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,20 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 zynapse-0.1.0/.python-version
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 zynapse-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 zynapse-0.1.0/requirements.lock
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zynapse-0.1.0/src/zynapse/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 zynapse-0.1.0/.gitignore
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 zynapse-0.1.0/README.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 zynapse-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 zynapse-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 zynapse-0.1.1/.python-version
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 zynapse-0.1.1/ARCHITECTURE.md
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zynapse-0.1.1/LEARNINGS.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zynapse-0.1.1/.github/workflows/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zynapse-0.1.1/docs/.gitkeep
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 zynapse-0.1.1/src/sdk/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zynapse-0.1.1/src/sdk/gpu/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 zynapse-0.1.1/src/sdk/gpu/connection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zynapse-0.1.1/src/sdk/model/__init__.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 zynapse-0.1.1/src/sdk/model/llm.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 zynapse-0.1.1/src/sdk/model/ml.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zynapse-0.1.1/src/sdk/privacy/__init__.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 zynapse-0.1.1/src/sdk/privacy/zk_proof.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zynapse-0.1.1/src/sdk/tracker/__init__.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 zynapse-0.1.1/src/sdk/tracker/contribution.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 zynapse-0.1.1/src/sdk/tracker/usage.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 zynapse-0.1.1/.gitignore
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 zynapse-0.1.1/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 zynapse-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 zynapse-0.1.1/PKG-INFO
```

