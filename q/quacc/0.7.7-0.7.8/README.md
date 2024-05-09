# Comparing `tmp/quacc-0.7.7.tar.gz` & `tmp/quacc-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quacc-0.7.7.tar", last modified: Tue Apr 23 21:38:43 2024, max compression
+gzip compressed data, was "quacc-0.7.8.tar", last modified: Thu May  9 23:37:59 2024, max compression
```

## Comparing `quacc-0.7.7.tar` & `quacc-0.7.8.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.560052 quacc-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-23 21:36:44.000000 quacc-0.7.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 21:36:44.000000 quacc-0.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-23 21:38:43.560052 quacc-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-23 21:36:44.000000 quacc-0.7.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-04-23 21:36:44.000000 quacc-0.7.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 21:38:43.560052 quacc-0.7.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.524052 quacc-0.7.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.528052 quacc-0.7.7/src/quacc/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.528052 quacc-0.7.7/src/quacc/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/_cli/quacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.532052 quacc-0.7.7/src/quacc/atoms/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/atoms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/atoms/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/atoms/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/atoms/deformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/atoms/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/atoms/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.532052 quacc-0.7.7/src/quacc/calculators/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.532052 quacc-0.7.7/src/quacc/calculators/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17619 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/espresso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.532052 quacc-0.7.7/src/quacc/calculators/espresso/presets/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/metal_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.536052 quacc-0.7.7/src/quacc/calculators/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/qchem/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/qchem/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/qchem/qchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/qchem/qchem_custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.536052 quacc-0.7.7/src/quacc/calculators/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.536052 quacc-0.7.7/src/quacc/calculators/vasp/presets/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/BulkSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/QMOFSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/SlabSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/magmoms_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/setups_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/vasp_custodian.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.536052 quacc-0.7.7/src/quacc/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.540052 quacc-0.7.7/src/quacc/recipes/common/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/common/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/common/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/common/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/common/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.540052 quacc-0.7.7/src/quacc/recipes/dftb/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/dftb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/dftb/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/dftb/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.540052 quacc-0.7.7/src/quacc/recipes/emt/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/emt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/emt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/emt/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/emt/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/emt/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/emt/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.540052 quacc-0.7.7/src/quacc/recipes/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/espresso/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/espresso/bands.py
--rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/espresso/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/espresso/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    24396 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/espresso/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.540052 quacc-0.7.7/src/quacc/recipes/gaussian/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/gaussian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/gaussian/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/gaussian/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/gulp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/gulp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/gulp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/gulp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/lj/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/lj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/lj/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/mlp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/mlp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/mlp/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/newtonnet/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/newtonnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/newtonnet/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/newtonnet/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/onetep/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/onetep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/onetep/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/onetep/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/orca/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/orca/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/orca/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/psi4/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/psi4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/psi4/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/psi4/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.548052 quacc-0.7.7/src/quacc/recipes/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/qchem/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/qchem/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/qchem/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.548052 quacc-0.7.7/src/quacc/recipes/tblite/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/tblite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/tblite/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/tblite/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.548052 quacc-0.7.7/src/quacc/recipes/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/vasp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/vasp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/vasp/mp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/vasp/qmof.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/vasp/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.548052 quacc-0.7.7/src/quacc/runners/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/runners/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/runners/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/runners/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/runners/thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.552052 quacc-0.7.7/src/quacc/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.552052 quacc-0.7.7/src/quacc/schemas/_aliases/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/emmet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    16656 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.552052 quacc-0.7.7/src/quacc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/utils/kpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/utils/lists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.552052 quacc-0.7.7/src/quacc/wflow_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/wflow_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/wflow_tools/customizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/wflow_tools/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/wflow_tools/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.552052 quacc-0.7.7/src/quacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-23 21:38:43.000000 quacc-0.7.7/src/quacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-23 21:38:43.000000 quacc-0.7.7/src/quacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:38:43.000000 quacc-0.7.7/src/quacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 21:38:43.000000 quacc-0.7.7/src/quacc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-23 21:38:43.000000 quacc-0.7.7/src/quacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 21:38:43.000000 quacc-0.7.7/src/quacc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:59.001201 quacc-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-09 23:36:36.000000 quacc-0.7.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 23:36:36.000000 quacc-0.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-05-09 23:37:59.001201 quacc-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-09 23:36:36.000000 quacc-0.7.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-09 23:36:36.000000 quacc-0.7.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 23:37:59.001201 quacc-0.7.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.969201 quacc-0.7.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.973201 quacc-0.7.8/src/quacc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.973201 quacc-0.7.8/src/quacc/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/_cli/quacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.973201 quacc-0.7.8/src/quacc/atoms/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/atoms/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/atoms/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/atoms/deformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/atoms/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/atoms/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.973201 quacc-0.7.8/src/quacc/calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.977201 quacc-0.7.8/src/quacc/calculators/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/espresso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.977201 quacc-0.7.8/src/quacc/calculators/espresso/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/metal_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/espresso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.977201 quacc-0.7.8/src/quacc/calculators/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/qchem/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/qchem/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/qchem/qchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/qchem/qchem_custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.981201 quacc-0.7.8/src/quacc/calculators/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.981201 quacc-0.7.8/src/quacc/calculators/vasp/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/BulkSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/QMOFSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/SlabSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/magmoms_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/presets/setups_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/calculators/vasp/vasp_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.981201 quacc-0.7.8/src/quacc/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.981201 quacc-0.7.8/src/quacc/recipes/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/common/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/common/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/common/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/common/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.981201 quacc-0.7.8/src/quacc/recipes/dftb/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/dftb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/dftb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/dftb/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.985201 quacc-0.7.8/src/quacc/recipes/emt/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/emt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/emt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/emt/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/emt/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/emt/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/emt/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.985201 quacc-0.7.8/src/quacc/recipes/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/espresso/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/espresso/bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/espresso/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/espresso/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24396 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/espresso/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.985201 quacc-0.7.8/src/quacc/recipes/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/gaussian/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/gaussian/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.985201 quacc-0.7.8/src/quacc/recipes/gulp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/gulp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/gulp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/gulp/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.985201 quacc-0.7.8/src/quacc/recipes/lj/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/lj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/lj/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.989201 quacc-0.7.8/src/quacc/recipes/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/mlp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/mlp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/mlp/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.989201 quacc-0.7.8/src/quacc/recipes/newtonnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/newtonnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/newtonnet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/newtonnet/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.989201 quacc-0.7.8/src/quacc/recipes/onetep/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/onetep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/onetep/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/onetep/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.989201 quacc-0.7.8/src/quacc/recipes/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/orca/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/orca/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.989201 quacc-0.7.8/src/quacc/recipes/psi4/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/psi4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/psi4/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/psi4/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.989201 quacc-0.7.8/src/quacc/recipes/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/qchem/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/qchem/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/qchem/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.993201 quacc-0.7.8/src/quacc/recipes/tblite/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/tblite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/tblite/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/tblite/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.993201 quacc-0.7.8/src/quacc/recipes/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/vasp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/vasp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/vasp/mp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/vasp/qmof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/recipes/vasp/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.993201 quacc-0.7.8/src/quacc/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/runners/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/runners/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/runners/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/runners/thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.993201 quacc-0.7.8/src/quacc/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.997201 quacc-0.7.8/src/quacc/schemas/_aliases/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/emmet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/_aliases/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/schemas/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16656 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.997201 quacc-0.7.8/src/quacc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/utils/kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/utils/lists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.997201 quacc-0.7.8/src/quacc/wflow_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/wflow_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/wflow_tools/customizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/wflow_tools/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13248 2024-05-09 23:36:36.000000 quacc-0.7.8/src/quacc/wflow_tools/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:37:58.997201 quacc-0.7.8/src/quacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-05-09 23:37:58.000000 quacc-0.7.8/src/quacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-09 23:37:58.000000 quacc-0.7.8/src/quacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 23:37:58.000000 quacc-0.7.8/src/quacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 23:37:58.000000 quacc-0.7.8/src/quacc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-09 23:37:58.000000 quacc-0.7.8/src/quacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 23:37:58.000000 quacc-0.7.8/src/quacc.egg-info/top_level.txt
```

### Comparing `quacc-0.7.7/LICENSE.md` & `quacc-0.7.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/PKG-INFO` & `quacc-0.7.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.7
+Version: 0.7.8
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
@@ -34,51 +34,49 @@
 Requires-Dist: psutil
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-settings>=2.2.0
 Requires-Dist: pymatgen>=2024.4.13
 Requires-Dist: ruamel.yaml>=0.17.40
 Requires-Dist: typer>=0.12.1
 Provides-Extra: covalent
-Requires-Dist: covalent>=0.234.0rc0; extra == "covalent"
-Requires-Dist: covalent-cloud>=0.39.0; extra == "covalent"
+Requires-Dist: covalent>=0.234.0rc0; platform_system != "Windows" and extra == "covalent"
+Requires-Dist: covalent-cloud>=0.39.0; platform_system != "Windows" and extra == "covalent"
 Provides-Extra: dask
 Requires-Dist: dask[distributed]>=2023.12.1; extra == "dask"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "dask"
 Provides-Extra: defects
 Requires-Dist: pymatgen-analysis-defects>=2023.8.22; extra == "defects"
 Requires-Dist: shakenbreak>=3.2.0; extra == "defects"
 Provides-Extra: jobflow
-Requires-Dist: jobflow>=0.1.14; extra == "jobflow"
+Requires-Dist: jobflow[fireworks]>=0.1.14; extra == "jobflow"
 Requires-Dist: jobflow-remote>=0.1.0; extra == "jobflow"
-Requires-Dist: fireworks>=2.0.3; extra == "jobflow"
 Provides-Extra: mlp
 Requires-Dist: matgl>=1.0.0; extra == "mlp"
 Requires-Dist: chgnet>=0.3.3; extra == "mlp"
 Requires-Dist: mace-torch>=0.3.3; extra == "mlp"
 Requires-Dist: torch-dftd>=0.4.0; extra == "mlp"
-Requires-Dist: torch<=2.2.1; extra == "mlp"
 Provides-Extra: mp
 Requires-Dist: pymatgen-io-validation>=0.0.1; extra == "mp"
 Provides-Extra: newtonnet
 Requires-Dist: newtonnet>=1.1; extra == "newtonnet"
 Provides-Extra: parsl
-Requires-Dist: parsl[monitoring]>=2023.10.23; extra == "parsl"
+Requires-Dist: parsl[monitoring]>=2023.10.23; platform_system != "Windows" and extra == "parsl"
 Provides-Extra: phonons
 Requires-Dist: phonopy>=2.20.0; extra == "phonons"
 Requires-Dist: seekpath>=2.1.0; extra == "phonons"
 Provides-Extra: prefect
 Requires-Dist: prefect>=2.14.14; extra == "prefect"
 Requires-Dist: prefect-dask>=0.2.6; extra == "prefect"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "prefect"
 Provides-Extra: redun
 Requires-Dist: redun>=0.16.2; extra == "redun"
 Provides-Extra: sella
 Requires-Dist: sella>=2.3.3; extra == "sella"
 Provides-Extra: tblite
-Requires-Dist: tblite[ase]>=0.3.0; platform_system == "Linux" and extra == "tblite"
+Requires-Dist: tblite>=0.3.0; platform_system == "Linux" and extra == "tblite"
 Provides-Extra: dev
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: ruff>=0.0.285; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: blacken-docs>=1.16.0; extra == "docs"
 Requires-Dist: mkdocs-material>=9.5.16; extra == "docs"
@@ -109,15 +107,15 @@
 
 ## Documentation 📖
 
 <p align="center">
      <a href="https://quantum-accelerators.github.io/quacc/"><b><i>Learn More Here!</i></b></a>
 </p>
 
-... or skip straight to one of the following sections:
+... or skip to one of the following sections:
 
 - 🔧 [Installation Guide](https://quantum-accelerators.github.io/quacc/install/install.html)
 - 🧠 [User Guide](https://quantum-accelerators.github.io/quacc/user/recipes/recipes_intro.html)
 - 🤝 [Developer Guide](https://quantum-accelerators.github.io/quacc/dev/contributing.html)
 
 ## Visual Example ✨
```

### Comparing `quacc-0.7.7/README.md` & `quacc-0.7.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 ## Documentation 📖
 
 <p align="center">
      <a href="https://quantum-accelerators.github.io/quacc/"><b><i>Learn More Here!</i></b></a>
 </p>
 
-... or skip straight to one of the following sections:
+... or skip to one of the following sections:
 
 - 🔧 [Installation Guide](https://quantum-accelerators.github.io/quacc/install/install.html)
 - 🧠 [User Guide](https://quantum-accelerators.github.io/quacc/user/recipes/recipes_intro.html)
 - 🤝 [Developer Guide](https://quantum-accelerators.github.io/quacc/dev/contributing.html)
 
 ## Visual Example ✨
```

#### html2text {}

```diff
@@ -18,17 +18,17 @@
 interface to several [workflow management solutions](https://quantum-
 accelerators.github.io/quacc/user/basics/wflow_overview.html), you can use what
 best suits your unique computing needs. - `quacc` leverages community resources
 so we don't reinvent the wheel. It is built around the Atomic Simulation
 Environment and much of the software infrastructure powering the Materials
 Project. ## Documentation ð
                                _LL_ee_aa_rr_nn_ _MM_oo_rr_ee_ _HH_ee_rr_ee_!!
-... or skip straight to one of the following sections: - ð§ [Installation
-Guide](https://quantum-accelerators.github.io/quacc/install/install.html) -
-ð§  [User Guide](https://quantum-accelerators.github.io/quacc/user/recipes/
+... or skip to one of the following sections: - ð§ [Installation Guide]
+(https://quantum-accelerators.github.io/quacc/install/install.html) - ð§ 
+[User Guide](https://quantum-accelerators.github.io/quacc/user/recipes/
 recipes_intro.html) - ð¤ [Developer Guide](https://quantum-
 accelerators.github.io/quacc/dev/contributing.html) ## Visual Example â¨ ð
 Representative `quacc` workflow using [Covalent](https://github.com/AgnostiqHQ/
 covalent) as one of the several supported workflow managers. ![](https://
 github.com/Quantum-Accelerators/quacc/blob/main/docs/images/start/start.gif) ##
 Citation ð If you use `quacc` in your work, please cite it as follows: -
 quacc â The Quantum Accelerator, https://doi.org/10.5281/zenodo.7720998. ##
```

### Comparing `quacc-0.7.7/pyproject.toml` & `quacc-0.7.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quacc"
 description="A platform to enable high-throughput, database-driven quantum chemistry and computational materials science"
-version = "0.7.7"
+version = "0.7.8"
 readme = "README.md"
 license = { text = "BSD-3" }
 authors = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 maintainers = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 keywords = ["high-throughput", "automated", "workflow", "dft"]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -39,27 +39,27 @@
     "pydantic-settings>=2.2.0", # for settings management
     "pymatgen>=2024.4.13", # for structure manipulation
     "ruamel.yaml>=0.17.40", # for YAML
     "typer>=0.12.1", # for the CLI
 ]
 
 [project.optional-dependencies]
-covalent = ["covalent>=0.234.0rc0", "covalent-cloud>=0.39.0"]
+covalent = ["covalent>=0.234.0rc0; platform_system!='Windows'", "covalent-cloud>=0.39.0; platform_system!='Windows'"]
 dask = ["dask[distributed]>=2023.12.1", "dask-jobqueue>=0.8.2"]
 defects = ["pymatgen-analysis-defects>=2023.8.22", "shakenbreak>=3.2.0"]
-jobflow = ["jobflow>=0.1.14", "jobflow-remote>=0.1.0", "fireworks>=2.0.3"]
-mlp = ["matgl>=1.0.0", "chgnet>=0.3.3", "mace-torch>=0.3.3", "torch-dftd>=0.4.0", "torch<=2.2.1"]
+jobflow = ["jobflow[fireworks]>=0.1.14", "jobflow-remote>=0.1.0"]
+mlp = ["matgl>=1.0.0", "chgnet>=0.3.3", "mace-torch>=0.3.3", "torch-dftd>=0.4.0"]
 mp = ["pymatgen-io-validation>=0.0.1"]
 newtonnet = ["newtonnet>=1.1"]
-parsl = ["parsl[monitoring]>=2023.10.23"]
+parsl = ["parsl[monitoring]>=2023.10.23; platform_system!='Windows'"]
 phonons = ["phonopy>=2.20.0", "seekpath>=2.1.0"]
 prefect = ["prefect>=2.14.14", "prefect-dask>=0.2.6", "dask-jobqueue>=0.8.2"]
 redun = ["redun>=0.16.2"]
 sella = ["sella>=2.3.3"]
-tblite = ["tblite[ase]>=0.3.0; platform_system=='Linux'"]
+tblite = ["tblite>=0.3.0; platform_system=='Linux'"]
 dev = ["pytest>=7.4.0", "pytest-cov>=3.0.0", "ruff>=0.0.285"]
 docs = [
     "blacken-docs>=1.16.0",
     "mkdocs-material>=9.5.16",
     "mkdocstrings[python]>=0.22.0",
     "mkdocs-gen-files>=0.5.0",
     "mkdocs-literate-nav>=0.6.0",
```

### Comparing `quacc-0.7.7/src/quacc/__init__.py` & `quacc-0.7.8/src/quacc/__init__.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/_cli/quacc.py` & `quacc-0.7.8/src/quacc/_cli/quacc.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/atoms/core.py` & `quacc-0.7.8/src/quacc/atoms/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/atoms/defects.py` & `quacc-0.7.8/src/quacc/atoms/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/atoms/deformation.py` & `quacc-0.7.8/src/quacc/atoms/deformation.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/atoms/phonons.py` & `quacc-0.7.8/src/quacc/atoms/phonons.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,30 +7,27 @@
 
 import numpy as np
 from monty.dev import requires
 from pymatgen.io.ase import AseAtomsAdaptor
 from pymatgen.io.phonopy import get_phonopy_structure, get_pmg_structure
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
-try:
-    import phonopy
+has_phonopy = find_spec("phonopy")
 
-    has_deps = find_spec("seekpath") is not None
-except ImportError:
-    has_deps = False
+if has_phonopy:
+    from phonopy import Phonopy
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
 
-    if phonopy:
-        from phonopy import Phonopy
+    if has_phonopy:
         from phonopy.structure.atoms import PhonopyAtoms
 
 
-@requires(has_deps, "Phonopy or seekpath is not installed.")
+@requires(has_phonopy, "Phonopy not installed.")
 def get_phonopy(
     atoms: Atoms,
     min_lengths: float | tuple[float, float, float] | None = None,
     supercell_matrix: (
         tuple[tuple[int, int, int], tuple[int, int, int], tuple[int, int, int]] | None
     ) = None,
     symprec: float = 1e-5,
@@ -59,26 +56,25 @@
     Returns
     -------
     Phonopy
         Phonopy object
     """
     phonopy_kwargs = phonopy_kwargs or {}
 
-    structure = AseAtomsAdaptor().get_structure(atoms)
-    structure = SpacegroupAnalyzer(
-        structure, symprec=symprec
+    symmetrized_structure = SpacegroupAnalyzer(
+        AseAtomsAdaptor().get_structure(atoms), symprec=symprec
     ).get_symmetrized_structure()
 
     if supercell_matrix is None and min_lengths is not None:
-        n_supercells = np.round(np.ceil(min_lengths / atoms.cell.lengths()))
-        supercell_matrix = np.diag([n_supercells, n_supercells, n_supercells])
+        supercell_matrix = np.diag(
+            np.round(np.ceil(min_lengths / np.array(symmetrized_structure.lattice.abc)))
+        )
 
-    phonopy_atoms = get_phonopy_structure(structure)
-    phonon = phonopy.Phonopy(
-        phonopy_atoms,
+    phonon = Phonopy(
+        get_phonopy_structure(symmetrized_structure),
         symprec=symprec,
         supercell_matrix=supercell_matrix,
         **phonopy_kwargs,
     )
     phonon.generate_displacements(distance=displacement)
     return phonon
```

### Comparing `quacc-0.7.7/src/quacc/atoms/slabs.py` & `quacc-0.7.8/src/quacc/atoms/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/espresso/espresso.py` & `quacc-0.7.8/src/quacc/calculators/espresso/espresso.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import os
 import re
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import numpy as np
 from ase.atoms import Atoms
-from ase.calculators.espresso import Espresso as Espresso_
 from ase.calculators.espresso import EspressoProfile
 from ase.calculators.espresso import EspressoTemplate as EspressoTemplate_
+from ase.calculators.genericfileio import GenericFileIOCalculator
 from ase.io import read, write
 from ase.io.espresso import (
     Namelist,
     read_espresso_ph,
     write_espresso_ph,
     write_fortran_namelist,
 )
@@ -348,28 +348,27 @@
 
             parameters["input_data"]["inputph"] = input_ph
             parameters["qpts"] = qpts
 
         return remove_dict_entries(parameters, remove_trigger=Remove)
 
 
-class Espresso(Espresso_):
+class Espresso(GenericFileIOCalculator):
     """
     A wrapper around the ASE Espresso calculator that adjusts input_data
     parameters and allows for the use of presets.
     Templates are used to set the binary and input/output file names.
     """
 
     def __init__(
         self,
         input_atoms: Atoms | None = None,
         preset: str | None = None,
         parallel_info: dict[str, Any] | None = None,
         template: EspressoTemplate | None = None,
-        profile: EspressoProfile | None = None,
         **kwargs,
     ) -> None:
         """
         Initialize the Espresso calculator.
 
         Parameters
         ----------
@@ -385,18 +384,14 @@
             parallel_info is a dictionary passed to the ASE Espresso calculator
             profile. It is used to specify prefixes for the command line arguments.
             See the ASE documentation for more details.
         template
             ASE calculator templace which can be used to specify which espresso
             binary will be used in the calculation. This is taken care of by recipe
             in most cases.
-        profile
-            ASE calculator profile which can be used to specify the location of
-            the espresso binary and pseudopotential files. This is taken care of
-            internally using quacc settings.
         **kwargs
             Additional arguments to be passed to the Espresso calculator. Takes all valid
             ASE calculator arguments, such as `input_data` and `kpts`. Refer to
             [ase.calculators.espresso.Espresso][] for details. Note that the full input
             must be described; use `{"system":{"ecutwfc": 60}}` and not the `{"ecutwfc": 60}`
             short-hand.
 
@@ -430,28 +425,26 @@
             self.user_calc_params = self.kwargs
 
         self._pseudo_path = (
             self.user_calc_params.get("input_data", {})
             .get("control", {})
             .get("pseudo_dir", str(SETTINGS.ESPRESSO_PSEUDO))
         )
-        self.profile = profile or EspressoProfile(
-            binary=self._bin_path,
-            parallel_info=parallel_info,
-            pseudo_dir=self._pseudo_path,
+
+        profile = EspressoProfile(
+            self._bin_path, self._pseudo_path, parallel_info=parallel_info
         )
 
         super().__init__(
-            profile=self.profile,
-            parallel_info=self.parallel_info,
-            **self.user_calc_params,
+            template=template,
+            profile=profile,
+            directory=".",
+            parameters=self.user_calc_params,
         )
 
-        self.template = template
-
     def _cleanup_params(self) -> None:
         """
         Function that handles the kwargs. It will merge the user-supplied kwargs with
         the preset values, using the former as priority.
 
         Parameters
         ----------
```

### Comparing `quacc-0.7.7/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml` & `quacc-0.7.8/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml` & `quacc-0.7.8/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml` & `quacc-0.7.8/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/espresso/utils.py` & `quacc-0.7.8/src/quacc/calculators/espresso/utils.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/qchem/io.py` & `quacc-0.7.8/src/quacc/calculators/qchem/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/qchem/params.py` & `quacc-0.7.8/src/quacc/calculators/qchem/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/qchem/qchem.py` & `quacc-0.7.8/src/quacc/calculators/qchem/qchem.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/qchem/qchem_custodian.py` & `quacc-0.7.8/src/quacc/calculators/qchem/qchem_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/vasp/io.py` & `quacc-0.7.8/src/quacc/calculators/vasp/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/vasp/params.py` & `quacc-0.7.8/src/quacc/calculators/vasp/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml` & `quacc-0.7.8/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/vasp/presets/setups_pbe54.yaml` & `quacc-0.7.8/src/quacc/calculators/vasp/presets/setups_pbe54.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/vasp/presets/setups_qmof.yaml` & `quacc-0.7.8/src/quacc/calculators/vasp/presets/setups_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/calculators/vasp/vasp.py` & `quacc-0.7.8/src/quacc/calculators/vasp/vasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,18 +182,14 @@
         # Set the VASP pseudopotential directory
         if SETTINGS.VASP_PP_PATH:
             os.environ["VASP_PP_PATH"] = str(SETTINGS.VASP_PP_PATH)
 
         # Set the ASE_VASP_VDW environmentvariable
         if SETTINGS.VASP_VDW:
             os.environ["ASE_VASP_VDW"] = str(SETTINGS.VASP_VDW)
-        if self.user_calc_params.get("luse_vdw") and "ASE_VASP_VDW" not in os.environ:
-            raise OSError(
-                "VASP_VDW setting was not provided, yet you requested a vdW functional."
-            )
 
         # Return vanilla ASE command
         vasp_cmd = (
             SETTINGS.VASP_GAMMA_CMD
             if (
                 np.prod(self.user_calc_params.get("kpts", [1, 1, 1])) == 1
                 and not self.user_calc_params.get("kspacing", None)
```

### Comparing `quacc-0.7.7/src/quacc/calculators/vasp/vasp_custodian.py` & `quacc-0.7.8/src/quacc/calculators/vasp/vasp_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/common/defects.py` & `quacc-0.7.8/src/quacc/recipes/common/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/common/elastic.py` & `quacc-0.7.8/src/quacc/recipes/common/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/common/phonons.py` & `quacc-0.7.8/src/quacc/recipes/common/phonons.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,23 +18,25 @@
     from typing import Any
 
     from ase.atoms import Atoms
 
     from quacc import Job
     from quacc.schemas._aliases.phonons import PhononSchema
 
+    if has_deps:
+        from phonopy import Phonopy
+
 
 @subflow
 @requires(
     has_deps, "Phonopy and seekpath must be installed. Run `pip install quacc[phonons]`"
 )
 def phonon_subflow(
     atoms: Atoms,
     force_job: Job,
-    relax_job: Job | None = None,
     symprec: float = 1e-4,
     min_lengths: float | tuple[float, float, float] | None = 20.0,
     supercell_matrix: (
         tuple[tuple[int, int, int], tuple[int, int, int], tuple[int, int, int]] | None
     ) = None,
     displacement: float = 0.01,
     t_step: float = 10,
@@ -48,16 +50,14 @@
 
     Parameters
     ----------
     atoms
         Atoms object with calculator attached.
     force_job
         The static job to calculate the forces.
-    relax_job
-        The job used to relax the structure before calculating the forces.
     symprec
         Precision for symmetry detection.
     min_lengths
         Minimum length of each lattice dimension (A).
     supercell_matrix
         The supercell matrix to use. If specified, it will override any
         value specified by `min_lengths`.
@@ -68,62 +68,60 @@
     t_min
         Min temperature (K).
     t_max
         Max temperature (K).
     phonopy_kwargs
         Additional kwargs to pass to the Phonopy class.
     additional_fields
-        Additional fields to store in the database.
+        Additional fields to add to the output schema.
 
     Returns
     -------
     PhononSchema
         Dictionary of results from [quacc.schemas.phonons.summarize_phonopy][]
     """
 
-    phonon = get_phonopy(
-        atoms,
-        min_lengths=min_lengths,
-        supercell_matrix=supercell_matrix,
-        symprec=symprec,
-        displacement=displacement,
-        phonopy_kwargs=phonopy_kwargs,
-    )
-    supercells = [
-        phonopy_atoms_to_ase_atoms(s) for s in phonon.supercells_with_displacements
-    ]
-
     @subflow
     def _get_forces_subflow(supercells: list[Atoms]) -> list[dict]:
         return [
             force_job(supercell) for supercell in supercells if supercell is not None
         ]
 
     @job
-    def _thermo_job(atoms: Atoms, force_job_results: list[dict]) -> PhononSchema:
-        phonon = get_phonopy(
-            atoms,
-            min_lengths=min_lengths,
-            supercell_matrix=supercell_matrix,
-            symprec=symprec,
-            displacement=displacement,
-            phonopy_kwargs=phonopy_kwargs,
-        )
+    def _thermo_job(
+        atoms: Atoms,
+        phonopy: Phonopy,
+        force_job_results: list[dict],
+        t_step: float,
+        t_min: float,
+        t_max: float,
+        additional_fields: dict[str, Any] | None,
+    ) -> PhononSchema:
         parameters = force_job_results[-1].get("parameters")
         forces = [output["results"]["forces"] for output in force_job_results]
-        phonon_results = run_phonopy(
-            phonon, forces, t_step=t_step, t_min=t_min, t_max=t_max
+        phonopy_results = run_phonopy(
+            phonopy, forces, t_step=t_step, t_min=t_min, t_max=t_max
         )
 
         return summarize_phonopy(
-            phonon,
+            phonopy,
             atoms,
-            phonon_results.directory,
+            phonopy_results.directory,
             parameters=parameters,
             additional_fields=additional_fields,
         )
 
-    if relax_job is not None:
-        atoms = relax_job(atoms)["atoms"]
-
+    phonopy = get_phonopy(
+        atoms,
+        min_lengths=min_lengths,
+        supercell_matrix=supercell_matrix,
+        symprec=symprec,
+        displacement=displacement,
+        phonopy_kwargs=phonopy_kwargs,
+    )
+    supercells = [
+        phonopy_atoms_to_ase_atoms(s) for s in phonopy.supercells_with_displacements
+    ]
     force_job_results = _get_forces_subflow(supercells)
-    return _thermo_job(atoms, force_job_results)
+    return _thermo_job(
+        atoms, phonopy, force_job_results, t_step, t_min, t_max, additional_fields
+    )
```

### Comparing `quacc-0.7.7/src/quacc/recipes/common/slabs.py` & `quacc-0.7.8/src/quacc/recipes/common/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/dftb/_base.py` & `quacc-0.7.8/src/quacc/recipes/dftb/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/dftb/core.py` & `quacc-0.7.8/src/quacc/recipes/dftb/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/emt/core.py` & `quacc-0.7.8/src/quacc/recipes/emt/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 from ase.calculators.emt import EMT
 
 from quacc import job
 from quacc.runners.ase import run_calc, run_opt
 from quacc.schemas.ase import summarize_opt_run, summarize_run
 
 if TYPE_CHECKING:
-    from typing import Any
-
     from ase.atoms import Atoms
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.ase import OptSchema, RunSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 @job
 def static_job(
     atoms: Atoms,
@@ -55,15 +54,15 @@
     return summarize_run(final_atoms, atoms, additional_fields={"name": "EMT Static"})
 
 
 @job
 def relax_job(
     atoms: Atoms,
     relax_cell: bool = False,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> OptSchema:
     """
     Carry out a geometry optimization.
 
     Parameters
```

### Comparing `quacc-0.7.7/src/quacc/recipes/emt/defects.py` & `quacc-0.7.8/src/quacc/recipes/emt/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/emt/elastic.py` & `quacc-0.7.8/src/quacc/recipes/emt/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/emt/phonons.py` & `quacc-0.7.8/src/quacc/recipes/emt/phonons.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,19 +88,20 @@
 
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
         parameters=job_params,
         decorators=job_decorators,
     )
+    if run_relax:
+        atoms = relax_job_(atoms)["atoms"]
 
     return phonon_subflow(
         atoms,
         static_job_,
-        relax_job=relax_job_ if run_relax else None,
         symprec=symprec,
         min_lengths=min_lengths,
         supercell_matrix=supercell_matrix,
         displacement=displacement,
         t_step=t_step,
         t_min=t_min,
         t_max=t_max,
```

### Comparing `quacc-0.7.7/src/quacc/recipes/emt/slabs.py` & `quacc-0.7.8/src/quacc/recipes/emt/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/espresso/_base.py` & `quacc-0.7.8/src/quacc/recipes/espresso/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from quacc.runners.ase import run_calc, run_opt
 from quacc.schemas.ase import summarize_opt_run, summarize_run
 from quacc.utils.dicts import recursive_dict_merge
 
 if TYPE_CHECKING:
     from typing import Any
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.ase import RunSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 def run_and_summarize(
     atoms: Atoms | None = None,
     preset: str | None = None,
@@ -105,15 +106,15 @@
     atoms: Atoms | None = None,
     preset: str | None = None,
     template: EspressoTemplate | None = None,
     profile: EspressoProfile | None = None,
     calc_defaults: dict[str, Any] | None = None,
     calc_swaps: dict[str, Any] | None = None,
     opt_defaults: dict[str, Any] | None = None,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     parallel_info: dict[str, Any] | None = None,
     additional_fields: dict[str, Any] | None = None,
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
```

### Comparing `quacc-0.7.7/src/quacc/recipes/espresso/bands.py` & `quacc-0.7.8/src/quacc/recipes/espresso/bands.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/espresso/core.py` & `quacc-0.7.8/src/quacc/recipes/espresso/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 
 from quacc import job
 from quacc.atoms.core import check_is_metal
 from quacc.calculators.espresso.espresso import EspressoTemplate
 from quacc.recipes.espresso._base import run_and_summarize, run_and_summarize_opt
 
 if TYPE_CHECKING:
-    from typing import Any
-
     from ase.atoms import Atoms
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.ase import RunSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 BASE_SET_METAL = {
     "input_data": {
         "system": {"occupations": "smearing", "smearing": "cold", "degauss": 0.01},
         "electrons": {"conv_thr": 1e-8, "mixing_mode": "local-TF", "mixing_beta": 0.35},
@@ -184,15 +183,15 @@
 @job
 def ase_relax_job(
     atoms: Atoms,
     preset: str | None = "sssp_1.3.0_pbe_efficiency",
     autorestart: bool = True,
     relax_cell: bool = False,
     parallel_info: dict[str] | None = None,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
     prev_outdir: SourceDirectory | None = None,
```

### Comparing `quacc-0.7.7/src/quacc/recipes/espresso/dos.py` & `quacc-0.7.8/src/quacc/recipes/espresso/dos.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/espresso/phonons.py` & `quacc-0.7.8/src/quacc/recipes/espresso/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/gaussian/_base.py` & `quacc-0.7.8/src/quacc/recipes/gaussian/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/gaussian/core.py` & `quacc-0.7.8/src/quacc/recipes/gaussian/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/gulp/_base.py` & `quacc-0.7.8/src/quacc/recipes/gulp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/gulp/core.py` & `quacc-0.7.8/src/quacc/recipes/gulp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/lj/core.py` & `quacc-0.7.8/src/quacc/recipes/lj/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,17 @@
 
 from quacc import job
 from quacc.runners.ase import run_calc, run_opt, run_vib
 from quacc.runners.thermo import run_ideal_gas
 from quacc.schemas.ase import summarize_opt_run, summarize_run, summarize_vib_and_thermo
 
 if TYPE_CHECKING:
-    from typing import Any
-
     from ase.atoms import Atoms
 
-    from quacc.runners.ase import VibKwargs
+    from quacc.runners.ase import OptParams, VibKwargs
     from quacc.schemas._aliases.ase import OptSchema, RunSchema, VibThermoSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 @job
 def static_job(
     atoms: Atoms,
@@ -56,15 +54,15 @@
 
     return summarize_run(final_atoms, atoms, additional_fields={"name": "LJ Static"})
 
 
 @job
 def relax_job(
     atoms: Atoms,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> OptSchema:
     """
     Function to carry out a geometry optimization.
 
     Parameters
```

### Comparing `quacc-0.7.7/src/quacc/recipes/mlp/_base.py` & `quacc-0.7.8/src/quacc/recipes/mlp/_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 """Base functions for universal machine-learned interatomic potentials."""
 
 from __future__ import annotations
 
 import logging
 from functools import lru_cache
 from typing import TYPE_CHECKING
+from warnings import warn
 
 if TYPE_CHECKING:
     from typing import Literal
 
-    from ase.calculator.calculator import Calculator
+    from ase.calculators.calculator import Calculator
 
 logger = logging.getLogger(__name__)
 
 
 @lru_cache
 def pick_calculator(
-    method: Literal["mace", "m3gnet", "chgnet"], **kwargs
+    method: Literal["mace-mp-0", "m3gnet", "chgnet"], **kwargs
 ) -> Calculator:
     """
     Adapted from `matcalc.util.get_universal_calculator`.
 
+    .. deprecated:: 0.7.6
+            method `mace` will be removed in a later version, it is replaced by 'mace-mp-0'
+            which more accurately reflects the nature of the model and allows for versioning
+            in the future.
+
     Parameters
     ----------
     method
         Name of the calculator to use
     **kwargs
         Custom kwargs for the underlying calculator. Set a value to
         `quacc.Remove` to remove a pre-existing key entirely. For a list of available
@@ -52,18 +58,25 @@
 
     elif method.lower() == "chgnet":
         from chgnet import __version__
         from chgnet.model.dynamics import CHGNetCalculator
 
         calc = CHGNetCalculator(**kwargs)
 
-    elif method.lower() == "mace":
+    elif method.lower() in ["mace-mp-0", "mace"]:
         from mace import __version__
         from mace.calculators import mace_mp
 
+        if method.lower() == "mace":
+            warn(
+                "'mace' is deprecated and support will be removed. Use 'mace-mp-0' instead!",
+                DeprecationWarning,
+                stacklevel=3,
+            )
+
         if "default_dtype" not in kwargs:
             kwargs["default_dtype"] = "float64"
         calc = mace_mp(**kwargs)
 
     else:
         raise ValueError(f"Unrecognized {method=}.")
```

### Comparing `quacc-0.7.7/src/quacc/recipes/mlp/core.py` & `quacc-0.7.8/src/quacc/recipes/mlp/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 from quacc import job
 from quacc.recipes.mlp._base import pick_calculator
 from quacc.runners.ase import run_calc, run_opt
 from quacc.schemas.ase import summarize_opt_run, summarize_run
 from quacc.utils.dicts import recursive_dict_merge
 
 if TYPE_CHECKING:
-    from typing import Any, Literal
+    from typing import Literal
 
     from ase.atoms import Atoms
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.ase import OptSchema, RunSchema
 
 
 @job
 def static_job(
-    atoms: Atoms, method: Literal["mace", "m3gnet", "chgnet"], **calc_kwargs
+    atoms: Atoms, method: Literal["mace-mp-0", "m3gnet", "chgnet"], **calc_kwargs
 ) -> RunSchema:
     """
     Carry out a single-point calculation.
 
     Parameters
     ----------
     atoms
@@ -49,17 +50,17 @@
         final_atoms, atoms, additional_fields={"name": f"{method} Static"}
     )
 
 
 @job
 def relax_job(
     atoms: Atoms,
-    method: Literal["mace", "m3gnet", "chgnet"],
+    method: Literal["mace-mp-0", "m3gnet", "chgnet"],
     relax_cell: bool = False,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     **calc_kwargs,
 ) -> OptSchema:
     """
     Relax a structure.
 
     Parameters
     ----------
```

### Comparing `quacc-0.7.7/src/quacc/recipes/mlp/phonons.py` & `quacc-0.7.8/src/quacc/recipes/mlp/phonons.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 @flow
 @requires(
     has_deps,
     message="Phonopy and seekpath must be installed. Run `pip install quacc[phonons]`",
 )
 def phonon_flow(
     atoms: Atoms,
-    method: Literal["mace", "m3gnet", "chgnet"],
+    method: Literal["mace-mp-0", "m3gnet", "chgnet"],
     symprec: float = 1e-4,
     min_lengths: float | tuple[float, float, float] | None = 20.0,
     supercell_matrix: (
         tuple[tuple[int, int, int], tuple[int, int, int], tuple[int, int, int]] | None
     ) = None,
     displacement: float = 0.01,
     t_step: float = 10,
@@ -101,19 +101,20 @@
 
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
         parameters=job_params,
         decorators=job_decorators,
     )
+    if run_relax:
+        atoms = relax_job_(atoms)["atoms"]
 
     return phonon_subflow(
         atoms,
         static_job_,
-        relax_job=relax_job_ if run_relax else None,
         symprec=symprec,
         min_lengths=min_lengths,
         supercell_matrix=supercell_matrix,
         displacement=displacement,
         t_step=t_step,
         t_min=t_min,
         t_max=t_max,
```

### Comparing `quacc-0.7.7/src/quacc/recipes/newtonnet/core.py` & `quacc-0.7.8/src/quacc/recipes/newtonnet/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     NewtonNet = None
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.ase import OptSchema, RunSchema, VibThermoSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 @job
 @requires(NewtonNet, "NewtonNet must be installed. Refer to the quacc documentation.")
 def static_job(
@@ -73,15 +74,15 @@
     )
 
 
 @job
 @requires(NewtonNet, "NewtonNet must be installed. Refer to the quacc documentation.")
 def relax_job(
     atoms: Atoms,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> OptSchema:
     """
     Relax a structure.
 
     Parameters
```

### Comparing `quacc-0.7.7/src/quacc/recipes/newtonnet/ts.py` & `quacc-0.7.8/src/quacc/recipes/newtonnet/ts.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 if TYPE_CHECKING:
     from typing import Any, Literal
 
     from ase.atoms import Atoms
     from numpy.typing import NDArray
 
     from quacc.recipes.newtonnet.core import FreqSchema
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.ase import OptSchema
 
     class TSSchema(OptSchema):
         freq_job: FreqSchema | None
 
     class IRCSchema(OptSchema):
         freq_job: FreqSchema | None
@@ -46,15 +47,15 @@
 @requires(NewtonNet, "NewtonNet must be installed. Refer to the quacc documentation.")
 @requires(Sella, "Sella must be installed. Refer to the quacc documentation.")
 def ts_job(
     atoms: Atoms,
     use_custom_hessian: bool = False,
     run_freq: bool = True,
     freq_job_kwargs: dict[str, Any] | None = None,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     **calc_kwargs,
 ) -> TSSchema:
     """
     Perform a transition state (TS) job using the given atoms object.
 
     Parameters
     ----------
@@ -125,15 +126,15 @@
 @requires(NewtonNet, "NewtonNet must be installed. Refer to the quacc documentation.")
 @requires(Sella, "Sella must be installed. Refer to the quacc documentation.")
 def irc_job(
     atoms: Atoms,
     direction: Literal["forward", "reverse"] = "forward",
     run_freq: bool = True,
     freq_job_kwargs: dict[str, Any] | None = None,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     **calc_kwargs,
 ) -> IRCSchema:
     """
     Perform an intrinsic reaction coordinate (IRC) job using the given atoms object.
 
     Parameters
     ----------
```

### Comparing `quacc-0.7.7/src/quacc/recipes/onetep/_base.py` & `quacc-0.7.8/src/quacc/recipes/onetep/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from quacc.utils.dicts import recursive_dict_merge
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.ase import RunSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 def run_and_summarize(
     atoms: Atoms,
     calc_defaults: dict[str, Any] | None = None,
@@ -57,15 +58,15 @@
 
 
 def run_and_summarize_opt(
     atoms: Atoms,
     calc_defaults: dict[str, Any] | None = None,
     calc_swaps: dict[str, Any] | None = None,
     opt_defaults: dict[str, Any] | None = None,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     additional_fields: dict[str, Any] | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
 ) -> RunSchema:
     """
     Base function to carry out Onetep recipes with ASE optimizers.
 
     Parameters
```

### Comparing `quacc-0.7.7/src/quacc/recipes/onetep/core.py` & `quacc-0.7.8/src/quacc/recipes/onetep/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 from ase.optimize import LBFGS
 
 from quacc import job
 from quacc.recipes.onetep._base import run_and_summarize, run_and_summarize_opt
 from quacc.utils.dicts import recursive_dict_merge
 
 if TYPE_CHECKING:
-    from typing import Any
-
     from ase.atoms import Atoms
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.ase import RunSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 BASE_SET = {
     "keywords": {
         "output_detail": "verbose",
         "do_properties": True,
@@ -65,15 +64,15 @@
     )
 
 
 @job
 def ase_relax_job(
     atoms: Atoms,
     relax_cell: bool = False,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> RunSchema:
     """
     Function to carry out a structure relaxation with ONETEP using ASE
     external optimizers.
```

### Comparing `quacc-0.7.7/src/quacc/recipes/orca/_base.py` & `quacc-0.7.8/src/quacc/recipes/orca/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from quacc.utils.lists import merge_list_params
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.cclib import cclibASEOptSchema, cclibSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 _LABEL = OrcaTemplate()._label  # skipcq: PYL-W0212
 LOG_FILE = f"{_LABEL}.out"
 GEOM_FILE = f"{_LABEL}.xyz"
 
@@ -90,15 +91,15 @@
     charge: int = 0,
     spin_multiplicity: int = 1,
     default_inputs: list[str] | None = None,
     default_blocks: list[str] | None = None,
     input_swaps: list[str] | None = None,
     block_swaps: list[str] | None = None,
     opt_defaults: dict[str, Any] | None = None,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     additional_fields: dict[str, Any] | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> cclibASEOptSchema:
     """
     Base job function for ORCA recipes with ASE optimizer.
```

### Comparing `quacc-0.7.7/src/quacc/recipes/orca/core.py` & `quacc-0.7.8/src/quacc/recipes/orca/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 import psutil
 
 from quacc import job
 from quacc.atoms.core import perturb
 from quacc.recipes.orca._base import run_and_summarize, run_and_summarize_opt
 
 if TYPE_CHECKING:
-    from typing import Any, Literal
+    from typing import Literal
 
     from ase.atoms import Atoms
     from numpy.typing import NDArray
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.cclib import cclibASEOptSchema, cclibSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 @job
 def static_job(
     atoms: Atoms,
@@ -80,43 +81,43 @@
         block_swaps=orcablocks,
         additional_fields={"name": "ORCA Static"},
         copy_files=copy_files,
     )
 
 
 @job
-def freq_job(
+def relax_job(
     atoms: Atoms,
     charge: int = 0,
     spin_multiplicity: int = 1,
     xc: str = "wb97x-d3bj",
     basis: str = "def2-tzvp",
-    numerical: bool = False,
+    run_freq: bool = False,
     orcasimpleinput: list[str] | None = None,
     orcablocks: list[str] | None = None,
     nprocs: int | Literal["max"] = "max",
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
 ) -> cclibSchema:
     """
-    Carry out a vibrational frequency analysis calculation.
+    Carry out a geometry optimization.
 
     Parameters
     ----------
     atoms
         Atoms object
     charge
         Charge of the system.
     spin_multiplicity
         Multiplicity of the system.
     xc
         Exchange-correlation functional
     basis
         Basis set
-    numerical
-        If True (default False), a numeric frequency calculation will be requested
+    run_freq
+        If a frequency calculation should be carried out.
     orcasimpleinput
         List of `orcasimpleinput` swaps for the calculator. To remove entries
         from the defaults, put a `#` in front of the name. Refer to the
         [ase.calculators.orca.ORCA][] calculator for details on `orcasimpleinput`.
     orcablocks
         List of `orcablocks` swaps for the calculator. To remove entries
         from the defaults, put a `#` in front of the name. Refer to the
@@ -130,61 +131,63 @@
     -------
     cclibSchema
         Dictionary of results from [quacc.schemas.cclib.cclib_summarize_run][].
         See the type-hint for the data structure.
     """
     nprocs = psutil.cpu_count(logical=False) if nprocs == "max" else nprocs
 
-    default_inputs = [xc, basis, "normalprint", "numfreq" if numerical else "freq"]
+    default_inputs = [xc, basis, "normalprint", "opt"]
+    if run_freq:
+        default_inputs.append("freq")
 
     default_blocks = [f"%pal nprocs {nprocs} end"]
 
     return run_and_summarize(
         atoms,
-        charge,
-        spin_multiplicity,
+        charge=charge,
+        spin_multiplicity=spin_multiplicity,
         default_inputs=default_inputs,
         default_blocks=default_blocks,
         input_swaps=orcasimpleinput,
         block_swaps=orcablocks,
-        additional_fields={"name": "ORCA vibrational frequency analysis"},
+        additional_fields={"name": "ORCA Relax"},
         copy_files=copy_files,
     )
 
 
 @job
-def relax_job(
+def freq_job(
     atoms: Atoms,
     charge: int = 0,
     spin_multiplicity: int = 1,
     xc: str = "wb97x-d3bj",
     basis: str = "def2-tzvp",
-    run_freq: bool = False,
+    numerical: bool = False,
     orcasimpleinput: list[str] | None = None,
     orcablocks: list[str] | None = None,
     nprocs: int | Literal["max"] = "max",
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
 ) -> cclibSchema:
     """
-    Carry out a geometry optimization.
+    Carry out a vibrational frequency analysis calculation.
 
     Parameters
     ----------
     atoms
         Atoms object
     charge
         Charge of the system.
     spin_multiplicity
         Multiplicity of the system.
     xc
         Exchange-correlation functional
     basis
         Basis set
-    run_freq
-        If a frequency calculation should be carried out.
+    numerical
+        If True (default False), a numeric frequency calculation will be requested
     orcasimpleinput
         List of `orcasimpleinput` swaps for the calculator. To remove entries
         from the defaults, put a `#` in front of the name. Refer to the
         [ase.calculators.orca.ORCA][] calculator for details on `orcasimpleinput`.
     orcablocks
         List of `orcablocks` swaps for the calculator. To remove entries
         from the defaults, put a `#` in front of the name. Refer to the
@@ -198,43 +201,41 @@
     -------
     cclibSchema
         Dictionary of results from [quacc.schemas.cclib.cclib_summarize_run][].
         See the type-hint for the data structure.
     """
     nprocs = psutil.cpu_count(logical=False) if nprocs == "max" else nprocs
 
-    default_inputs = [xc, basis, "normalprint", "opt"]
-    if run_freq:
-        default_inputs.append("freq")
+    default_inputs = [xc, basis, "normalprint", "numfreq" if numerical else "freq"]
 
     default_blocks = [f"%pal nprocs {nprocs} end"]
 
     return run_and_summarize(
         atoms,
-        charge=charge,
-        spin_multiplicity=spin_multiplicity,
+        charge,
+        spin_multiplicity,
         default_inputs=default_inputs,
         default_blocks=default_blocks,
         input_swaps=orcasimpleinput,
         block_swaps=orcablocks,
-        additional_fields={"name": "ORCA Relax"},
+        additional_fields={"name": "ORCA vibrational frequency analysis"},
         copy_files=copy_files,
     )
 
 
 @job
 def ase_relax_job(
     atoms: Atoms,
     charge: int = 0,
     spin_multiplicity: int = 1,
     xc: str = "wb97x-d3bj",
     basis: str = "def2-tzvp",
     orcasimpleinput: list[str] | None = None,
     orcablocks: list[str] | None = None,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     nprocs: int | Literal["max"] = "max",
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
 ) -> cclibASEOptSchema:
     """
     Carry out a geometry optimization.
 
     Parameters
@@ -287,23 +288,23 @@
     )
 
 
 @job
 def ase_quasi_irc_perturb_job(
     atoms: Atoms,
     mode: list[list[float]] | NDArray,
-    charge: int = 0,
-    spin_multiplicity: int = 1,
     perturb_magnitude: float = 0.6,
     direction: Literal["forward", "reverse"] = "forward",
+    charge: int = 0,
+    spin_multiplicity: int = 1,
     xc: str = "wb97x-d3bj",
     basis: str = "def2-tzvp",
     orcasimpleinput: list[str] | None = None,
     orcablocks: list[str] | None = None,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     nprocs: int | Literal["max"] = "max",
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
 ) -> cclibASEOptSchema:
     """
     Quasi-IRC to optimize a reaction endpoint from a transition-state with known vibrational frequency modes.
     Perturbs the structure of `atoms` by a finite amount (0.6 * the normalized mode magnitude) along the specified
     vibrational frequency mode (assumed to be the transition mode), and then performs a `relax_job` on the perturbed
@@ -311,23 +312,23 @@
 
     Parameters
     ----------
     atoms
         Atoms object
     mode
         Transition mode. This should be an Nx3 matrix, where N is the number of atoms in `atoms`.
-    charge
-        Charge of the system.
-    spin_multiplicity
-        Multiplicity of the system.
     perturb_magnitude
         Factor to multiply the transition mode. Default is 0.6. In some cases, it may be advisable to increase this
         factor, perhaps to 1.0 or 1.1. Lowering it is not generally found to be helpful.
     direction
         Direction of the (Quasi)IRC. Should be "forward" or "reverse".
+    charge
+        Charge of the system.
+    spin_multiplicity
+        Multiplicity of the system.
     xc
         Exchange-correlation functional
     basis
         Basis set.
     orcasimpleinput
         List of `orcasimpleinput` swaps for the calculator. To remove entries
         from the defaults, put a `#` in front of the name. Refer to the
```

### Comparing `quacc-0.7.7/src/quacc/recipes/psi4/_base.py` & `quacc-0.7.8/src/quacc/recipes/psi4/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/psi4/core.py` & `quacc-0.7.8/src/quacc/recipes/psi4/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/qchem/_base.py` & `quacc-0.7.8/src/quacc/recipes/qchem/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from quacc.utils.dicts import recursive_dict_merge
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.ase import OptSchema, RunSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 def run_and_summarize(
     atoms: Atoms,
     charge: int = 0,
@@ -72,15 +73,15 @@
 def run_and_summarize_opt(
     atoms: Atoms,
     charge: int = 0,
     spin_multiplicity: int = 1,
     calc_defaults: dict[str, Any] | None = None,
     calc_swaps: dict[str, Any] | None = None,
     opt_defaults: dict[str, Any] | None = None,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     additional_fields: dict[str, Any] | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
 ) -> OptSchema:
     """
     Base function for Q-Chem recipes that involve ASE optimizers.
 
     Parameters
```

### Comparing `quacc-0.7.7/src/quacc/recipes/qchem/core.py` & `quacc-0.7.8/src/quacc/recipes/qchem/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,17 @@
     from sella import Sella
 
     has_sella = True
 except ImportError:
     has_sella = False
 
 if TYPE_CHECKING:
-    from typing import Any
-
     from ase.atoms import Atoms
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.ase import OptSchema, RunSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 _BASE_SET = {
     "rem": {
         "gen_scfman": True,
         "xc_grid": 3,
@@ -94,15 +93,15 @@
 @job
 def relax_job(
     atoms: Atoms,
     charge: int = 0,
     spin_multiplicity: int = 1,
     method: str = "wb97mv",
     basis: str = "def2-svpd",
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> OptSchema:
     """
     Optimize aka "relax" a molecular structure with an ASE optimizer.
 
     Parameters
```

### Comparing `quacc-0.7.7/src/quacc/recipes/qchem/ts.py` & `quacc-0.7.8/src/quacc/recipes/qchem/ts.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,28 @@
 
 if TYPE_CHECKING:
     from typing import Any, Literal
 
     from ase.atoms import Atoms
     from numpy.typing import NDArray
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.ase import OptSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 @job
 @requires(has_sella, "Sella must be installed. Refer to the quacc documentation.")
 def ts_job(
     atoms: Atoms,
     charge: int = 0,
     spin_multiplicity: int = 1,
     method: str = "wb97mv",
     basis: str = "def2-svpd",
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> OptSchema:
     """
     TS optimize a molecular structure.
 
     Parameters
@@ -100,15 +101,15 @@
 def irc_job(
     atoms: Atoms,
     charge: int = 0,
     spin_multiplicity: int = 1,
     direction: Literal["forward", "reverse"] = "forward",
     method: str = "wb97mv",
     basis: str = "def2-svpd",
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> OptSchema:
     """
     IRC optimize a molecular structure.
 
     Parameters
@@ -236,21 +237,21 @@
 
 
 @job
 @requires(has_sella, "Sella must be installed. Refer to the quacc documentation.")
 def quasi_irc_perturb_job(
     atoms: Atoms,
     mode: list[list[float]] | NDArray,
-    charge: int = 0,
-    spin_multiplicity: int = 1,
     perturb_magnitude: float = 0.6,
     direction: Literal["forward", "reverse"] = "forward",
+    charge: int = 0,
+    spin_multiplicity: int = 1,
     method: str = "wb97mv",
     basis: str = "def2-svpd",
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> OptSchema:
     """
     Quasi-IRC to optimize a reaction endpoint from a transition-state with known vibrational frequency modes.
     Perturbs the structure of `atoms` by a finite amount (0.6 * the normalized mode magnitude) along the specified
     vibrational frequency mode (assumed to be the transition mode), and then performs a `relax_job` on the perturbed
@@ -258,23 +259,23 @@
 
     Parameters
     ----------
     atoms
         Atoms object.
     mode
         Transition mode. This should be an Nx3 matrix, where N is the number of atoms in `atoms`.
-    charge
-        Charge of the system.
-    spin_multiplicity
-        Multiplicity of the system.
     perturb_magnitude
         Factor to multiply the transition mode. Default is 0.6. In some cases, it may be advisable to increase this
         factor, perhaps to 1.0 or 1.1. Lowering it is not generally found to be helpful.
     direction
         Direction of the (Quasi)IRC. Should be "forward" or "reverse".
+    charge
+        Charge of the system.
+    spin_multiplicity
+        Multiplicity of the system.
     method
         DFT exchange-correlation functional or other electronic structure
         method.
     basis
         Basis set.
     opt_params
         Dictionary of custom kwargs for the optimization process. For a list
```

### Comparing `quacc-0.7.7/src/quacc/recipes/tblite/core.py` & `quacc-0.7.8/src/quacc/recipes/tblite/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 try:
     from tblite.ase import TBLite
 except ImportError:
     TBLite = None
 
 if TYPE_CHECKING:
-    from typing import Any, Literal
+    from typing import Literal
 
     from ase.atoms import Atoms
 
-    from quacc.runners.ase import VibKwargs
+    from quacc.runners.ase import OptParams, VibKwargs
     from quacc.schemas._aliases.ase import OptSchema, RunSchema, VibThermoSchema
 
 
 @job
 @requires(TBLite, "tblite must be installed. Refer to the quacc documentation.")
 def static_job(
     atoms: Atoms,
@@ -65,15 +65,15 @@
 
 @job
 @requires(TBLite, "tblite must be installed. Refer to the quacc documentation.")
 def relax_job(
     atoms: Atoms,
     method: Literal["GFN1-xTB", "GFN2-xTB", "IPEA1-xTB"] = "GFN2-xTB",
     relax_cell: bool = False,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     **calc_kwargs,
 ) -> OptSchema:
     """
     Relax a structure.
 
     Parameters
     ----------
```

### Comparing `quacc-0.7.7/src/quacc/recipes/tblite/phonons.py` & `quacc-0.7.8/src/quacc/recipes/tblite/phonons.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,19 +101,20 @@
 
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
         parameters=job_params,
         decorators=job_decorators,
     )
+    if run_relax:
+        atoms = relax_job_(atoms)["atoms"]
 
     return phonon_subflow(
         atoms,
         static_job_,
-        relax_job=relax_job_ if run_relax else None,
         symprec=symprec,
         min_lengths=min_lengths,
         supercell_matrix=supercell_matrix,
         displacement=displacement,
         t_step=t_step,
         t_min=t_min,
         t_max=t_max,
```

### Comparing `quacc-0.7.7/src/quacc/recipes/vasp/_base.py` & `quacc-0.7.8/src/quacc/recipes/vasp/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from quacc.utils.dicts import recursive_dict_merge
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.vasp import VaspASEOptSchema, VaspSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 def run_and_summarize(
     atoms: Atoms,
     preset: str | None = None,
@@ -68,15 +69,15 @@
 
 def run_and_summarize_opt(
     atoms: Atoms,
     preset: str | None = None,
     calc_defaults: dict[str, Any] | None = None,
     calc_swaps: dict[str, Any] | None = None,
     opt_defaults: dict[str, Any] | None = None,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     report_mp_corrections: bool = False,
     additional_fields: dict[str, Any] | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
 ) -> VaspASEOptSchema:
     """
     Base job function for VASP recipes with ASE optimizers.
```

### Comparing `quacc-0.7.7/src/quacc/recipes/vasp/core.py` & `quacc-0.7.8/src/quacc/recipes/vasp/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from quacc.recipes.vasp._base import run_and_summarize, run_and_summarize_opt
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
 
+    from quacc.runners.ase import OptParams
     from quacc.schemas._aliases.vasp import VaspASEOptSchema, VaspSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 @job
 def static_job(
     atoms: Atoms,
@@ -179,15 +180,15 @@
 
 
 @job
 def ase_relax_job(
     atoms: Atoms,
     preset: str | None = "BulkSet",
     relax_cell: bool = True,
-    opt_params: dict[str, Any] | None = None,
+    opt_params: OptParams | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> VaspASEOptSchema:
     """
     Relax a structure.
 
     Parameters
```

### Comparing `quacc-0.7.7/src/quacc/recipes/vasp/mp.py` & `quacc-0.7.8/src/quacc/recipes/vasp/mp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/vasp/qmof.py` & `quacc-0.7.8/src/quacc/recipes/vasp/qmof.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/recipes/vasp/slabs.py` & `quacc-0.7.8/src/quacc/recipes/vasp/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/runners/ase.py` & `quacc-0.7.8/src/quacc/runners/ase.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utility functions for running ASE calculators with ASE-based methods."""
 
 from __future__ import annotations
 
 import sys
 from shutil import copy, copytree
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Callable
 
 import numpy as np
 from ase.filters import FrechetCellFilter
 from ase.io import Trajectory, read
 from ase.optimize import BFGS
 from ase.vibrations import Vibrations
 from monty.dev import requires
@@ -30,14 +30,27 @@
     from typing import Any, TypedDict
 
     from ase.atoms import Atoms
     from ase.optimize.optimize import Optimizer
 
     from quacc.utils.files import Filenames, SourceDirectory
 
+    class OptParams(TypedDict, total=False):
+        """
+        Type hint for `opt_params` used throughout quacc.
+        """
+
+        fmax: float
+        max_steps: int
+        optimizer: Optimizer = BFGS
+        optimizer_kwargs: OptimizerKwargs | None
+        store_intermediate_results: bool
+        fn_hook: Callable | None
+        run_kwargs: dict[str, Any] | None
+
     class OptimizerKwargs(TypedDict, total=False):
         """
         Type hint for `optimizer_kwargs` in [quacc.runners.ase.run_opt][].
         """
 
         restart: Path | str | None  # default = None
         append_trajectory: bool  # default = False
@@ -131,14 +144,15 @@
     atoms: Atoms,
     relax_cell: bool = False,
     fmax: float = 0.01,
     max_steps: int = 1000,
     optimizer: Optimizer = BFGS,
     optimizer_kwargs: OptimizerKwargs | None = None,
     store_intermediate_results: bool = False,
+    fn_hook: Callable | None = None,
     run_kwargs: dict[str, Any] | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
 ) -> Optimizer:
     """
     Run an ASE-based optimization in a scratch directory and copy the results back to
     the original directory. This can be useful if file I/O is slow in the working
     directory, so long as file transfer speeds are reasonable.
@@ -162,14 +176,18 @@
         Dictionary of kwargs for the optimizer. Takes all valid kwargs for ASE
         Optimizer classes. Refer to `_set_sella_kwargs` for Sella-related
         kwargs and how they are set.
     store_intermediate_results
         Whether to store the files generated at each intermediate step in the
         optimization. If enabled, they will be stored in a directory named
         `stepN` where `N` is the step number, starting at 0.
+    fn_hook
+        A custom function to call after each step of the optimization.
+        The function must take the instantiated dynamics class as
+        its only argument.
     run_kwargs
         Dictionary of kwargs for the run() method of the optimizer.
     copy_files
         Files to copy (and decompress) from source to the runtime directory.
 
     Returns
     -------
@@ -212,28 +230,31 @@
 
     # Set volume relaxation constraints, if relevant
     if relax_cell and atoms.pbc.any():
         atoms = FrechetCellFilter(atoms)
 
     # Run optimization
     with traj, optimizer(atoms, **optimizer_kwargs) as dyn:
-        if store_intermediate_results:
-            opt = dyn.irun(fmax=fmax, steps=max_steps, **run_kwargs)
-            for i, _ in enumerate(opt):
-                _copy_intermediate_files(
-                    tmpdir,
-                    i,
-                    files_to_ignore=[
-                        traj_file,
-                        optimizer_kwargs["restart"],
-                        optimizer_kwargs["logfile"],
-                    ],
-                )
-        else:
+        if optimizer.__name__.startswith("SciPy"):
+            # https://gitlab.com/ase/ase/-/issues/1475
             dyn.run(fmax=fmax, steps=max_steps, **run_kwargs)
+        else:
+            for i, _ in enumerate(dyn.irun(fmax=fmax, steps=max_steps, **run_kwargs)):
+                if store_intermediate_results:
+                    _copy_intermediate_files(
+                        tmpdir,
+                        i,
+                        files_to_ignore=[
+                            traj_file,
+                            optimizer_kwargs["restart"],
+                            optimizer_kwargs["logfile"],
+                        ],
+                    )
+                if fn_hook:
+                    fn_hook(dyn)
 
     # Store the trajectory atoms
     dyn.traj_atoms = read(traj_file, index=":")
 
     # Perform cleanup operations
     calc_cleanup(get_final_atoms_from_dynamics(dyn), tmpdir, job_results_dir)
```

### Comparing `quacc-0.7.7/src/quacc/runners/phonons.py` & `quacc-0.7.8/src/quacc/runners/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/runners/prep.py` & `quacc-0.7.8/src/quacc/runners/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/runners/thermo.py` & `quacc-0.7.8/src/quacc/runners/thermo.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/schemas/_aliases/ase.py` & `quacc-0.7.8/src/quacc/schemas/_aliases/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/schemas/_aliases/atoms.py` & `quacc-0.7.8/src/quacc/schemas/_aliases/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/schemas/_aliases/cclib.py` & `quacc-0.7.8/src/quacc/schemas/_aliases/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/schemas/_aliases/emmet.py` & `quacc-0.7.8/src/quacc/schemas/_aliases/emmet.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/schemas/_aliases/phonons.py` & `quacc-0.7.8/src/quacc/schemas/_aliases/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/schemas/_aliases/vasp.py` & `quacc-0.7.8/src/quacc/schemas/_aliases/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/schemas/ase.py` & `quacc-0.7.8/src/quacc/schemas/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/schemas/atoms.py` & `quacc-0.7.8/src/quacc/schemas/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/schemas/cclib.py` & `quacc-0.7.8/src/quacc/schemas/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/schemas/phonons.py` & `quacc-0.7.8/src/quacc/schemas/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/schemas/prep.py` & `quacc-0.7.8/src/quacc/schemas/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/schemas/vasp.py` & `quacc-0.7.8/src/quacc/schemas/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/settings.py` & `quacc-0.7.8/src/quacc/settings.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/utils/dicts.py` & `quacc-0.7.8/src/quacc/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/utils/files.py` & `quacc-0.7.8/src/quacc/utils/files.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/utils/kpts.py` & `quacc-0.7.8/src/quacc/utils/kpts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/utils/lists.py` & `quacc-0.7.8/src/quacc/utils/lists.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/wflow_tools/customizers.py` & `quacc-0.7.8/src/quacc/wflow_tools/customizers.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/wflow_tools/db.py` & `quacc-0.7.8/src/quacc/wflow_tools/db.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc/wflow_tools/decorators.py` & `quacc-0.7.8/src/quacc/wflow_tools/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import TYPE_CHECKING, TypeVar
 
 Job = TypeVar("Job")
 Flow = TypeVar("Flow")
 Subflow = TypeVar("Subflow")
 
 if TYPE_CHECKING:
-    from typing import Callable
+    from typing import Any, Callable
 
 
 def job(_func: Callable | None = None, **kwargs) -> Job:
     """
     Decorator for individual compute jobs. This is a `#!Python @job` decorator. Think of
     each `#!Python @job`-decorated function as an individual SLURM job, if that helps.
 
@@ -158,15 +158,17 @@
     elif SETTINGS.WORKFLOW_ENGINE == "jobflow":
         from jobflow import job as jf_job
 
         return jf_job(_func, **kwargs)
     elif SETTINGS.WORKFLOW_ENGINE == "parsl":
         from parsl import python_app
 
-        return python_app(_func, **kwargs)
+        wrapped_fn = _get_parsl_wrapped_func(_func, kwargs)
+
+        return python_app(wrapped_fn, **kwargs)
     elif SETTINGS.WORKFLOW_ENGINE == "redun":
         from redun import task
 
         return task(_func, namespace=_func.__module__, **kwargs)
     elif SETTINGS.WORKFLOW_ENGINE == "prefect":
         from prefect import task
 
@@ -561,27 +563,67 @@
                 futures = client.compute(_func(*f_args, **f_kwargs))
                 return client.gather(futures)
 
         return delayed(wrapper, **kwargs)
     elif SETTINGS.WORKFLOW_ENGINE == "parsl":
         from parsl import join_app
 
-        return join_app(_func, **kwargs)
+        wrapped_fn = _get_parsl_wrapped_func(_func, kwargs)
+
+        return join_app(wrapped_fn, **kwargs)
     elif SETTINGS.WORKFLOW_ENGINE == "prefect":
         from prefect import flow as prefect_flow
 
         return prefect_flow(_func, validate_parameters=False, **kwargs)
     elif SETTINGS.WORKFLOW_ENGINE == "redun":
         from redun import task
 
         return task(_func, namespace=_func.__module__, **kwargs)
     else:
         return _func
 
 
+def _get_parsl_wrapped_func(
+    func: Callable, decorator_kwargs: dict[str, Any]
+) -> Callable:
+    """
+    Wrap a function to handle special Parsl arguments.
+
+    Parameters
+    ----------
+    func
+        The function to wrap.
+    decorator_kwargs
+        Decorator keyword arguments, including Parsl-specific ones that
+        are meant to be passed to the underlying function. The `walltime`
+        and `parsl_resource_specification` arguments will be injected
+        into the function call and removed from the decorator arguments.
+
+    Returns
+    -------
+    callable
+        The wrapped function.
+    """
+    walltime = decorator_kwargs.pop("walltime", None)
+    parsl_resource_specification = decorator_kwargs.pop(
+        "parsl_resource_specification", {}
+    )
+
+    def wrapper(
+        *f_args,
+        walltime=walltime,  # noqa: ARG001
+        parsl_resource_specification=parsl_resource_specification,  # noqa: ARG001
+        **f_kwargs,
+    ):
+        return func(*f_args, **f_kwargs)
+
+    wrapper.__name__ = func.__name__
+    return wrapper
+
+
 class Delayed_:
     """A small Dask-compatible, serializable object to wrap delayed functions that we
     don't want to execute.
     """
 
     __slots__ = ("func",)
```

### Comparing `quacc-0.7.7/src/quacc.egg-info/PKG-INFO` & `quacc-0.7.8/src/quacc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.7
+Version: 0.7.8
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
@@ -34,51 +34,49 @@
 Requires-Dist: psutil
 Requires-Dist: pydantic>=2.0.1
 Requires-Dist: pydantic-settings>=2.2.0
 Requires-Dist: pymatgen>=2024.4.13
 Requires-Dist: ruamel.yaml>=0.17.40
 Requires-Dist: typer>=0.12.1
 Provides-Extra: covalent
-Requires-Dist: covalent>=0.234.0rc0; extra == "covalent"
-Requires-Dist: covalent-cloud>=0.39.0; extra == "covalent"
+Requires-Dist: covalent>=0.234.0rc0; platform_system != "Windows" and extra == "covalent"
+Requires-Dist: covalent-cloud>=0.39.0; platform_system != "Windows" and extra == "covalent"
 Provides-Extra: dask
 Requires-Dist: dask[distributed]>=2023.12.1; extra == "dask"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "dask"
 Provides-Extra: defects
 Requires-Dist: pymatgen-analysis-defects>=2023.8.22; extra == "defects"
 Requires-Dist: shakenbreak>=3.2.0; extra == "defects"
 Provides-Extra: jobflow
-Requires-Dist: jobflow>=0.1.14; extra == "jobflow"
+Requires-Dist: jobflow[fireworks]>=0.1.14; extra == "jobflow"
 Requires-Dist: jobflow-remote>=0.1.0; extra == "jobflow"
-Requires-Dist: fireworks>=2.0.3; extra == "jobflow"
 Provides-Extra: mlp
 Requires-Dist: matgl>=1.0.0; extra == "mlp"
 Requires-Dist: chgnet>=0.3.3; extra == "mlp"
 Requires-Dist: mace-torch>=0.3.3; extra == "mlp"
 Requires-Dist: torch-dftd>=0.4.0; extra == "mlp"
-Requires-Dist: torch<=2.2.1; extra == "mlp"
 Provides-Extra: mp
 Requires-Dist: pymatgen-io-validation>=0.0.1; extra == "mp"
 Provides-Extra: newtonnet
 Requires-Dist: newtonnet>=1.1; extra == "newtonnet"
 Provides-Extra: parsl
-Requires-Dist: parsl[monitoring]>=2023.10.23; extra == "parsl"
+Requires-Dist: parsl[monitoring]>=2023.10.23; platform_system != "Windows" and extra == "parsl"
 Provides-Extra: phonons
 Requires-Dist: phonopy>=2.20.0; extra == "phonons"
 Requires-Dist: seekpath>=2.1.0; extra == "phonons"
 Provides-Extra: prefect
 Requires-Dist: prefect>=2.14.14; extra == "prefect"
 Requires-Dist: prefect-dask>=0.2.6; extra == "prefect"
 Requires-Dist: dask-jobqueue>=0.8.2; extra == "prefect"
 Provides-Extra: redun
 Requires-Dist: redun>=0.16.2; extra == "redun"
 Provides-Extra: sella
 Requires-Dist: sella>=2.3.3; extra == "sella"
 Provides-Extra: tblite
-Requires-Dist: tblite[ase]>=0.3.0; platform_system == "Linux" and extra == "tblite"
+Requires-Dist: tblite>=0.3.0; platform_system == "Linux" and extra == "tblite"
 Provides-Extra: dev
 Requires-Dist: pytest>=7.4.0; extra == "dev"
 Requires-Dist: pytest-cov>=3.0.0; extra == "dev"
 Requires-Dist: ruff>=0.0.285; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: blacken-docs>=1.16.0; extra == "docs"
 Requires-Dist: mkdocs-material>=9.5.16; extra == "docs"
@@ -109,15 +107,15 @@
 
 ## Documentation 📖
 
 <p align="center">
      <a href="https://quantum-accelerators.github.io/quacc/"><b><i>Learn More Here!</i></b></a>
 </p>
 
-... or skip straight to one of the following sections:
+... or skip to one of the following sections:
 
 - 🔧 [Installation Guide](https://quantum-accelerators.github.io/quacc/install/install.html)
 - 🧠 [User Guide](https://quantum-accelerators.github.io/quacc/user/recipes/recipes_intro.html)
 - 🤝 [Developer Guide](https://quantum-accelerators.github.io/quacc/dev/contributing.html)
 
 ## Visual Example ✨
```

### Comparing `quacc-0.7.7/src/quacc.egg-info/SOURCES.txt` & `quacc-0.7.8/src/quacc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quacc-0.7.7/src/quacc.egg-info/requires.txt` & `quacc-0.7.8/src/quacc.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 pydantic>=2.0.1
 pydantic-settings>=2.2.0
 pymatgen>=2024.4.13
 ruamel.yaml>=0.17.40
 typer>=0.12.1
 
 [covalent]
+
+[covalent:platform_system != "Windows"]
 covalent>=0.234.0rc0
 covalent-cloud>=0.39.0
 
 [dask]
 dask[distributed]>=2023.12.1
 dask-jobqueue>=0.8.2
 
@@ -35,32 +37,32 @@
 mkdocstrings[python]>=0.22.0
 mkdocs-gen-files>=0.5.0
 mkdocs-literate-nav>=0.6.0
 pillow>=10.0.0
 cairosvg>=2.7.1
 
 [jobflow]
-jobflow>=0.1.14
+jobflow[fireworks]>=0.1.14
 jobflow-remote>=0.1.0
-fireworks>=2.0.3
 
 [mlp]
 matgl>=1.0.0
 chgnet>=0.3.3
 mace-torch>=0.3.3
 torch-dftd>=0.4.0
-torch<=2.2.1
 
 [mp]
 pymatgen-io-validation>=0.0.1
 
 [newtonnet]
 newtonnet>=1.1
 
 [parsl]
+
+[parsl:platform_system != "Windows"]
 parsl[monitoring]>=2023.10.23
 
 [phonons]
 phonopy>=2.20.0
 seekpath>=2.1.0
 
 [prefect]
@@ -73,8 +75,8 @@
 
 [sella]
 sella>=2.3.3
 
 [tblite]
 
 [tblite:platform_system == "Linux"]
-tblite[ase]>=0.3.0
+tblite>=0.3.0
```

