# Comparing `tmp/tz-osemosys-0.0.1.tar.gz` & `tmp/tz_osemosys-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tz-osemosys-0.0.1.tar", last modified: Thu Mar 14 09:10:50 2024, max compression
+gzip compressed data, was "tz_osemosys-0.0.3.tar", last modified: Fri May 10 11:19:12 2024, max compression
```

## Comparing `tz-osemosys-0.0.1.tar` & `tz_osemosys-0.0.3.tar`

### file list

```diff
@@ -1,127 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.173738 tz-osemosys-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-03-14 09:10:50.173738 tz-osemosys-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.153738 tz-osemosys-0.0.1/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/bin/memory_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 09:10:50.173738 tz-osemosys-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.153738 tz-osemosys-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.157738 tz-osemosys-0.0.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/fixtures/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/fixtures/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.157738 tz-osemosys-0.0.1/tests/test_compatability/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_compatability/test_otoole_commodity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_compatability/test_otoole_impact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_compatability/test_otoole_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_compatability/test_otoole_roundtrip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_compatability/test_otoole_runspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_compatability/test_otoole_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_compatability/test_otoole_technology.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_compatability/test_otoole_timedef.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.157738 tz-osemosys-0.0.1/tests/test_composition/
--rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_composition/test_compose_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_composition/test_compose_runspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.157738 tz-osemosys-0.0.1/tests/test_construction/
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_construction/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_construction/test_commodity.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_construction/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_construction/test_impact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_construction/test_load_from_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_construction/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_construction/test_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_construction/test_runspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_construction/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_construction/test_technology.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_construction/test_timedefinition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.157738 tz-osemosys-0.0.1/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_integration/test_linopy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.161738 tz-osemosys-0.0.1/tests/test_solve/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_solve/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tests/test_solve/test_to_xr_ds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.153738 tz-osemosys-0.0.1/tz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.161738 tz-osemosys-0.0.1/tz/osemosys/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.161738 tz-osemosys-0.0.1/tz/osemosys/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/io/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    24598 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/io/simpleeval.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.161738 tz-osemosys-0.0.1/tz/osemosys/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.165738 tz-osemosys-0.0.1/tz/osemosys/model/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/accounting_technology.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/annual_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/capacity_adequacy_a.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/capacity_adequacy_b.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/capital_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/demand.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/energy_balance_a.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/energy_balance_b.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/new_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/operating_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/re_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/reserve_margin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/salvage_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/total_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/total_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/constraints/total_discounted_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/linear_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/objective.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.165738 tz-osemosys-0.0.1/tz/osemosys/model/variables/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/variables/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/variables/capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/variables/demand.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/variables/emissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/variables/other.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/model/variables/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.169738 tz-osemosys-0.0.1/tz/osemosys/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17417 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/commodity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.169738 tz-osemosys-0.0.1/tz/osemosys/schemas/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/compat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/compat/commodity.py
--rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/compat/impact.py
--rw-r--r--   0 runner    (1001) docker     (127)    19352 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/compat/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/compat/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/compat/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    19849 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/compat/technology.py
--rw-r--r--   0 runner    (1001) docker     (127)    12294 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/compat/time_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/impact.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/technology.py
--rw-r--r--   0 runner    (1001) docker     (127)    14385 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/time_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.169738 tz-osemosys-0.0.1/tz/osemosys/schemas/validation/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/validation/commodity_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/validation/impact_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/validation/model_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)    22164 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/validation/model_presolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/validation/region_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/validation/storage_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/validation/technology_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/validation/timedefinition_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/schemas/validation/validation_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.173738 tz-osemosys-0.0.1/tz/osemosys/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/utils/cfg_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-03-14 09:10:40.000000 tz-osemosys-0.0.1/tz/osemosys/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 09:10:50.173738 tz-osemosys-0.0.1/tz_osemosys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10412 2024-03-14 09:10:50.000000 tz-osemosys-0.0.1/tz_osemosys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-03-14 09:10:50.000000 tz-osemosys-0.0.1/tz_osemosys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 09:10:50.000000 tz-osemosys-0.0.1/tz_osemosys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-14 09:10:50.000000 tz-osemosys-0.0.1/tz_osemosys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-14 09:10:50.000000 tz-osemosys-0.0.1/tz_osemosys.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.438459 tz_osemosys-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-10 11:19:12.434459 tz_osemosys-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.418459 tz_osemosys-0.0.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/bin/memory_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:19:12.438459 tz_osemosys-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.418459 tz_osemosys-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.418459 tz_osemosys-0.0.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/fixtures/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/fixtures/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.418459 tz_osemosys-0.0.3/tests/test_compatability/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_commodity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_roundtrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_runspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_compatability/test_otoole_timedef.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.418459 tz_osemosys-0.0.3/tests/test_composition/
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_composition/test_compose_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_composition/test_compose_runspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.422459 tz_osemosys-0.0.3/tests/test_construction/
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_commodity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_load_from_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_runspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_construction/test_timedefinition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.422459 tz_osemosys-0.0.3/tests/test_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_integration/test_linopy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.422459 tz_osemosys-0.0.3/tests/test_solve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_solve/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tests/test_solve/test_to_xr_ds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.414459 tz_osemosys-0.0.3/tz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.422459 tz_osemosys-0.0.3/tz/osemosys/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.422459 tz_osemosys-0.0.3/tz/osemosys/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/io/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24600 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/io/simpleeval.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.422459 tz_osemosys-0.0.3/tz/osemosys/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.426459 tz_osemosys-0.0.3/tz/osemosys/model/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/accounting_technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/annual_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/capacity_adequacy_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/capacity_adequacy_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/capital_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/energy_balance_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/energy_balance_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/new_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/operating_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/re_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/reserve_margin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/salvage_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19117 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/total_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/total_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/constraints/total_discounted_costs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.426459 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/financials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/reserve_margin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/objective.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.430459 tz_osemosys-0.0.3/tz/osemosys/model/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/variables/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/variables/capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/variables/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/variables/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/model/variables/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.430459 tz_osemosys-0.0.3/tz/osemosys/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17417 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/commodity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.430459 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10554 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/commodity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21135 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10681 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19849 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/compat/time_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15116 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17046 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/time_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.434459 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/commodity_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/impact_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/model_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22164 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/model_presolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/region_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/storage_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/technology_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11627 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/timedefinition_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/schemas/validation/validation_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.434459 tz_osemosys-0.0.3/tz/osemosys/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/utils/cfg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-05-10 11:19:08.000000 tz_osemosys-0.0.3/tz/osemosys/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:19:12.434459 tz_osemosys-0.0.3/tz_osemosys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-10 11:19:12.000000 tz_osemosys-0.0.3/tz_osemosys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-10 11:19:12.000000 tz_osemosys-0.0.3/tz_osemosys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:19:12.000000 tz_osemosys-0.0.3/tz_osemosys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 11:19:12.000000 tz_osemosys-0.0.3/tz_osemosys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-10 11:19:12.000000 tz_osemosys-0.0.3/tz_osemosys.egg-info/top_level.txt
```

### Comparing `tz-osemosys-0.0.1/LICENSE` & `tz_osemosys-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/PKG-INFO` & `tz_osemosys-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tz-osemosys
-Version: 0.0.1
+Version: 0.0.3
 Summary: An OSeMOSYS implementation for the Future Energy Outlook by TransitionZero
 Author-email: Lucas Kruitwagen <lucas.kruitwagen@gmail.com>, Ed Gill <edwardxtg@gmail.com>, Abhishek Shivakumar <abhishek0208@gmail.com>
 Project-URL: Homepage, https://github.com/transitionzero/tz-osemosys
 Project-URL: Bug Reports, https://github.com/transitionzero/tz-osemosys/issues
 Project-URL: Funding, https://transitionzero.org
 Project-URL: Source, https://github.com/transitionzero/tz-osemosys
 Keywords: energy,milp,climate
@@ -18,25 +18,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>2
 Requires-Dist: pydantic-settings
 Requires-Dist: xarray
 Requires-Dist: orjson
 Requires-Dist: linopy
-Requires-Dist: highspy
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-order; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
+Requires-Dist: highspy; extra == "dev"
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/transition-zero/.github/raw/main/profile/img/logo-dark.png">
   <img alt="TransitionZero Logo" width="1000px" src="https://github.com/transition-zero/.github/raw/main/profile/img/logo-light.png">
   <a href="https://www.transitionzero.org/">
 </picture>
 
@@ -104,15 +104,15 @@
 
 HiGHS can be installed from source using `cmake` following the instructions [here](https://github.com/ERGO-Code/HiGHS?tab=readme-ov-file#installation). You'll need to install a cmake distribution for your relevant operating system.
 
 *common issue: make sure you have write-privileges to default directory for `cmake --install build`, or either run this command with administrator privileges (`sudo cmake --install build` on mac and linux) or specify a different build directory*
 
 ### Docker installation
 
-A docker container is provided that contains Python 3.11 and an installed version of HiGHS. You'll nedd to [install a docker distribution](https://docs.docker.com/engine/install/) relevant for your operating system.
+A docker container is provided that contains Python 3.11 and an installed version of HiGHS. You'll need to [install a docker distribution](https://docs.docker.com/engine/install/) relevant for your operating system.
 
 The docker container is used in testing, but can also be used for local development work. The following docker command will run and enter the docker container, mount the current working directory at the `/home` directory, and change directory within the container to this directory.
 
 ```console
 docker run -v $(pwd):/home -it  ghcr.io/transition-zero/tz-highs/highs-python:latest /bin/bash -c 'cd /home && /bin/bash'
 ```
 
@@ -136,15 +136,15 @@
     Impact,
     OperatingMode,
 )
 
 time_definition = TimeDefinition(id="years-only", years=range(2020, 2051))
 regions = [Region(id="single-region")]
 commodities = [Commodity(id="electricity", demand_annual=25 * 8760)]  # 25GW * 8760hr/yr
-impacts = [Impact(id="CO2", penalty=60)]  # 10 $mn/Mtonne
+impacts = [Impact(id="CO2", penalty=60)]  # 60 $mn/Mtonne
 technologies = [
     Technology(
         id="coal-gen",
         operating_life=40,  # years
         capex=800,  # mn$/GW
         # straight-line reduction to 2040
         residual_capacity={
@@ -199,17 +199,17 @@
 - model fields can also be populated from environment variables: `my_field: $ENV{MYVAR}`.
 - simple Python expressions are automatically evaluated, including list comprehensions, dictionary comprehensions, `min`, `max`, `sum`, and `range` functions.
 - for data keyed by an osemosys `set` (e.g. `YEARS`, `TIMESLICES`, `TECHNOLOGIES`), wildcards `"*"` can be used in place of explicitly listing all set members.
 - data field `set` dimensions and membership are also automatically inferred - a single value can be given which will be broadcast to all set member combinations.
 - single or multiple `.yaml` files can be composed together, allowing you to separate, e.g. `technologies.yaml`, from the rest of your model.
 
 ```python
-from tz.osemosys import load_model
+from tz.osemosys import Model
 
-my_model = load_model("path/to/yaml/directory")
+my_model = Model.from_yaml("path/to/yaml/directory")
 ```
 
 ### From Otoole outputs (legacy)
 
 TZ-OSeMOSYS is provided with backwards compatability with the [otoole](https://github.com/OSeMOSYS/otoole) osemosys tooling. Any legacy models can be loaded from the directory of otoole-formatted csvs.
 
 ```python
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: tz-osemosys Version: 0.0.1 Summary: An OSeMOSYS
+Metadata-Version: 2.1 Name: tz-osemosys Version: 0.0.3 Summary: An OSeMOSYS
 implementation for the Future Energy Outlook by TransitionZero Author-email:
 Lucas Kruitwagen
 gmail.com>, Ed Gill
 gmail.com>, Abhishek Shivakumar
 gmail.com> Project-URL: Homepage, https://github.com/transitionzero/tz-osemosys
 Project-URL: Bug Reports, https://github.com/transitionzero/tz-osemosys/issues
 Project-URL: Funding, https://transitionzero.org Project-URL: Source, https://
 github.com/transitionzero/tz-osemosys Keywords: energy,milp,climate Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Scientific/Engineering Classifier: License :: OSI
 Approved :: GNU Affero General Public License v3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
 Only Requires-Python: >=3.11 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: pydantic>2 Requires-Dist: pydantic-settings
-Requires-Dist: xarray Requires-Dist: orjson Requires-Dist: linopy Requires-
-Dist: highspy Provides-Extra: dev Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: black; extra == "dev" Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-order; extra == "dev" Requires-Dist: pytest-cov; extra ==
-"dev" Requires-Dist: pytest-asyncio; extra == "dev" Requires-Dist: mypy; extra
-== "dev" Requires-Dist: tox; extra == "dev" Requires-Dist: coverage; extra ==
-"dev" [TransitionZero Logo]_#_ _T_Z_-_O_S_E_M_O_S_Y_S_ _-_ _a_ _m_o_d_e_r_n_ _l_o_n_g_-_r_u_n_ _s_y_s_t_e_m_s_ _m_o_d_e_l_l_i_n_g
-_f_r_a_m_e_w_o_r_k_ _[_!_[_L_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_ _b_a_d_g_e_]_]_[_l_i_c_e_n_s_e_]_ _[_!_[_C_o_n_t_r_i_b_u_t_o_r_ _C_o_v_e_n_a_n_t_]
-_[_c_o_n_t_r_i_b_u_t_o_r_ _c_o_v_e_n_a_n_t_ _b_a_d_g_e_]_]_[_c_o_d_e_ _o_f_ _c_o_n_d_u_c_t_]_ _!_[_T_e_s_t_s_]_[_t_e_s_t_s_ _b_a_d_g_e_]_ _!
-_[_C_o_v_e_r_a_g_e_]_[_c_o_v_e_r_a_g_e_ _b_a_d_g_e_]_ _!_[_P_y_t_h_o_n_]_[_p_y_t_h_o_n_ _b_a_d_g_e_]_ _!_[_S_t_a_t_u_s_]_[_s_t_a_t_u_s_ _b_a_d_g_e_]_ 
-_[_l_i_c_e_n_s_e_ _b_a_d_g_e_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_a_d_-_a_u_r_e_s_/
+Requires-Dist: xarray Requires-Dist: orjson Requires-Dist: linopy Provides-
+Extra: dev Requires-Dist: pre-commit; extra == "dev" Requires-Dist: black;
+extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-
+order; extra == "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist:
+pytest-asyncio; extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-
+Dist: tox; extra == "dev" Requires-Dist: coverage; extra == "dev" Requires-
+Dist: highspy; extra == "dev" [TransitionZero Logo]_#_ _T_Z_-_O_S_E_M_O_S_Y_S_ _-_ _a_ _m_o_d_e_r_n
+_l_o_n_g_-_r_u_n_ _s_y_s_t_e_m_s_ _m_o_d_e_l_l_i_n_g_ _f_r_a_m_e_w_o_r_k_ _[_!_[_L_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_ _b_a_d_g_e_]_]_[_l_i_c_e_n_s_e_]_ _[_!
+_[_C_o_n_t_r_i_b_u_t_o_r_ _C_o_v_e_n_a_n_t_]_[_c_o_n_t_r_i_b_u_t_o_r_ _c_o_v_e_n_a_n_t_ _b_a_d_g_e_]_]_[_c_o_d_e_ _o_f_ _c_o_n_d_u_c_t_]_ _!_[_T_e_s_t_s_]
+_[_t_e_s_t_s_ _b_a_d_g_e_]_ _!_[_C_o_v_e_r_a_g_e_]_[_c_o_v_e_r_a_g_e_ _b_a_d_g_e_]_ _!_[_P_y_t_h_o_n_]_[_p_y_t_h_o_n_ _b_a_d_g_e_]_ _!_[_S_t_a_t_u_s_]
+_[_s_t_a_t_u_s_ _b_a_d_g_e_]_ _[_l_i_c_e_n_s_e_ _b_a_d_g_e_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_a_d_-_a_u_r_e_s_/
 _c_a_s_t_o_p_o_d_?_c_o_l_o_r_=_b_l_u_e_ _[_l_i_c_e_n_s_e_]_:_ _h_t_t_p_s_:_/_/_o_p_e_n_s_o_u_r_c_e_._o_r_g_/_l_i_c_e_n_s_e_/_a_g_p_l_-_v_3_ 
 _[_c_o_n_t_r_i_b_u_t_o_r_ _c_o_v_e_n_a_n_t_ _b_a_d_g_e_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
 _C_o_n_t_r_i_b_u_t_o_r_%_2_0_C_o_v_e_n_a_n_t_-_2_._1_-_4_b_a_a_a_a_._s_v_g_ _[_c_o_d_e_ _o_f_ _c_o_n_d_u_c_t_]_:_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
 _t_r_a_n_s_i_t_i_o_n_-_z_e_r_o_/_t_z_-_o_s_e_m_o_s_y_s_/_b_l_o_b_/_m_a_i_n_/_C_O_D_E_-_O_F_-_C_O_N_D_U_C_T_._m_d_ _[_t_e_s_t_s_ _b_a_d_g_e_]_:_ _h_t_t_p_s_:_/
 _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_e_n_d_p_o_i_n_t_?_u_r_l_=_h_t_t_p_s_:_/_/_g_i_s_t_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_L_k_r_u_i_t_w_a_g_e_n_/
 _f_e_f_f_b_3_8_d_4_6_c_7_5_0_c_a_d_5_4_0_2_d_c_a_5_d_d_5_4_b_f_9_/_r_a_w_/_t_e_s_t_s___p_a_s_s_i_n_g_._j_s_o_n_ _[_c_o_v_e_r_a_g_e_ _b_a_d_g_e_]_:
 _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_e_n_d_p_o_i_n_t_?_u_r_l_=_h_t_t_p_s_:_/_/_g_i_s_t_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/
@@ -66,15 +66,15 @@
 _(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_E_R_G_O_-_C_o_d_e_/_H_i_G_H_S_?_t_a_b_=_r_e_a_d_m_e_-_o_v_-_f_i_l_e_#_i_n_s_t_a_l_l_a_t_i_o_n_)_._ _Y_o_u_'_l_l
 _n_e_e_d_ _t_o_ _i_n_s_t_a_l_l_ _a_ _c_m_a_k_e_ _d_i_s_t_r_i_b_u_t_i_o_n_ _f_o_r_ _y_o_u_r_ _r_e_l_e_v_a_n_t_ _o_p_e_r_a_t_i_n_g_ _s_y_s_t_e_m_.
 _*_c_o_m_m_o_n_ _i_s_s_u_e_:_ _m_a_k_e_ _s_u_r_e_ _y_o_u_ _h_a_v_e_ _w_r_i_t_e_-_p_r_i_v_i_l_e_g_e_s_ _t_o_ _d_e_f_a_u_l_t_ _d_i_r_e_c_t_o_r_y_ _f_o_r
 _`_c_m_a_k_e_ _-_-_i_n_s_t_a_l_l_ _b_u_i_l_d_`_,_ _o_r_ _e_i_t_h_e_r_ _r_u_n_ _t_h_i_s_ _c_o_m_m_a_n_d_ _w_i_t_h_ _a_d_m_i_n_i_s_t_r_a_t_o_r
 _p_r_i_v_i_l_e_g_e_s_ _(_`_s_u_d_o_ _c_m_a_k_e_ _-_-_i_n_s_t_a_l_l_ _b_u_i_l_d_`_ _o_n_ _m_a_c_ _a_n_d_ _l_i_n_u_x_)_ _o_r_ _s_p_e_c_i_f_y_ _a
 _d_i_f_f_e_r_e_n_t_ _b_u_i_l_d_ _d_i_r_e_c_t_o_r_y_*_ _#_#_#_ _D_o_c_k_e_r_ _i_n_s_t_a_l_l_a_t_i_o_n_ _A_ _d_o_c_k_e_r_ _c_o_n_t_a_i_n_e_r_ _i_s
 _p_r_o_v_i_d_e_d_ _t_h_a_t_ _c_o_n_t_a_i_n_s_ _P_y_t_h_o_n_ _3_._1_1_ _a_n_d_ _a_n_ _i_n_s_t_a_l_l_e_d_ _v_e_r_s_i_o_n_ _o_f_ _H_i_G_H_S_._ _Y_o_u_'_l_l
-_n_e_d_d_ _t_o_ _[_i_n_s_t_a_l_l_ _a_ _d_o_c_k_e_r_ _d_i_s_t_r_i_b_u_t_i_o_n_]_(_h_t_t_p_s_:_/_/_d_o_c_s_._d_o_c_k_e_r_._c_o_m_/_e_n_g_i_n_e_/_i_n_s_t_a_l_l_/
+_n_e_e_d_ _t_o_ _[_i_n_s_t_a_l_l_ _a_ _d_o_c_k_e_r_ _d_i_s_t_r_i_b_u_t_i_o_n_]_(_h_t_t_p_s_:_/_/_d_o_c_s_._d_o_c_k_e_r_._c_o_m_/_e_n_g_i_n_e_/_i_n_s_t_a_l_l_/
 _)_ _r_e_l_e_v_a_n_t_ _f_o_r_ _y_o_u_r_ _o_p_e_r_a_t_i_n_g_ _s_y_s_t_e_m_._ _T_h_e_ _d_o_c_k_e_r_ _c_o_n_t_a_i_n_e_r_ _i_s_ _u_s_e_d_ _i_n_ _t_e_s_t_i_n_g_,
 _b_u_t_ _c_a_n_ _a_l_s_o_ _b_e_ _u_s_e_d_ _f_o_r_ _l_o_c_a_l_ _d_e_v_e_l_o_p_m_e_n_t_ _w_o_r_k_._ _T_h_e_ _f_o_l_l_o_w_i_n_g_ _d_o_c_k_e_r_ _c_o_m_m_a_n_d
 _w_i_l_l_ _r_u_n_ _a_n_d_ _e_n_t_e_r_ _t_h_e_ _d_o_c_k_e_r_ _c_o_n_t_a_i_n_e_r_,_ _m_o_u_n_t_ _t_h_e_ _c_u_r_r_e_n_t_ _w_o_r_k_i_n_g_ _d_i_r_e_c_t_o_r_y_ _a_t
 _t_h_e_ _`_/_h_o_m_e_`_ _d_i_r_e_c_t_o_r_y_,_ _a_n_d_ _c_h_a_n_g_e_ _d_i_r_e_c_t_o_r_y_ _w_i_t_h_i_n_ _t_h_e_ _c_o_n_t_a_i_n_e_r_ _t_o_ _t_h_i_s
 _d_i_r_e_c_t_o_r_y_._ _`_`_`_c_o_n_s_o_l_e_ _d_o_c_k_e_r_ _r_u_n_ _-_v_ _$_(_p_w_d_)_:_/_h_o_m_e_ _-_i_t_ _g_h_c_r_._i_o_/_t_r_a_n_s_i_t_i_o_n_-_z_e_r_o_/
 _t_z_-_h_i_g_h_s_/_h_i_g_h_s_-_p_y_t_h_o_n_:_l_a_t_e_s_t_ _/_b_i_n_/_b_a_s_h_ _-_c_ _'_c_d_ _/_h_o_m_e_ _&_&_ _/_b_i_n_/_b_a_s_h_'_ _`_`_`_ _*_n_o_t_e_!
 _A_n_y_ _f_i_l_e_s_ _c_h_a_n_g_e_d_ _w_i_t_h_i_n_ _t_h_i_s_ _m_o_u_n_t_e_d_ _d_i_r_e_c_t_o_r_y_ _w_i_l_l_ _p_e_r_s_i_s_t_,_ _b_u_t_ _a_n_y_ _c_h_a_n_g_e_s
@@ -86,15 +86,15 @@
 _b_e_t_w_e_e_n_ _t_h_e_ _o_b_j_e_c_t_ _t_y_p_e_s_._ _T_h_e_ _s_e_t_ _o_f_ _o_b_j_e_c_t_s_ _c_o_m_p_r_i_s_i_n_g_ _t_h_e_ _m_o_d_e_l_ _i_s_ _m_u_t_u_a_l_l_y
 _e_x_c_l_u_s_i_v_e_ _-_ _n_o_ _i_n_f_o_r_m_a_t_i_o_n_ _i_s_ _r_e_p_e_a_t_e_d_ _-_ _a_n_d_ _c_o_l_l_e_c_t_i_v_e_l_y_ _e_x_h_a_u_s_t_i_v_e_ _-_ _n_o
 _i_n_f_o_r_m_a_t_i_o_n_ _n_e_e_d_s_ _t_o_ _b_e_ _e_x_t_r_a_c_t_e_d_ _f_r_o_m_ _c_s_v_s_ _o_r_ _o_t_h_e_r_ _d_a_t_a_ _s_o_u_r_c_e_s_._ _`_`_`_p_y_t_h_o_n
 _f_r_o_m_ _t_z_._o_s_e_m_o_s_y_s_ _i_m_p_o_r_t_ _(_ _M_o_d_e_l_,_ _T_e_c_h_n_o_l_o_g_y_,_ _T_i_m_e_D_e_f_i_n_i_t_i_o_n_,_ _C_o_m_m_o_d_i_t_y_,_ _R_e_g_i_o_n_,
 _I_m_p_a_c_t_,_ _O_p_e_r_a_t_i_n_g_M_o_d_e_,_ _)_ _t_i_m_e___d_e_f_i_n_i_t_i_o_n_ _=_ _T_i_m_e_D_e_f_i_n_i_t_i_o_n_(_i_d_=_"_y_e_a_r_s_-_o_n_l_y_"_,
 _y_e_a_r_s_=_r_a_n_g_e_(_2_0_2_0_,_ _2_0_5_1_)_)_ _r_e_g_i_o_n_s_ _=_ _[_R_e_g_i_o_n_(_i_d_=_"_s_i_n_g_l_e_-_r_e_g_i_o_n_"_)_]_ _c_o_m_m_o_d_i_t_i_e_s_ _=_ 
 _[_C_o_m_m_o_d_i_t_y_(_i_d_=_"_e_l_e_c_t_r_i_c_i_t_y_"_,_ _d_e_m_a_n_d___a_n_n_u_a_l_=_2_5_ _*_ _8_7_6_0_)_]_ _#_ _2_5_G_W_ _*_ _8_7_6_0_h_r_/_y_r
-_i_m_p_a_c_t_s_ _=_ _[_I_m_p_a_c_t_(_i_d_=_"_C_O_2_"_,_ _p_e_n_a_l_t_y_=_6_0_)_]_ _#_ _1_0_ _$_m_n_/_M_t_o_n_n_e_ _t_e_c_h_n_o_l_o_g_i_e_s_ _=_ 
+_i_m_p_a_c_t_s_ _=_ _[_I_m_p_a_c_t_(_i_d_=_"_C_O_2_"_,_ _p_e_n_a_l_t_y_=_6_0_)_]_ _#_ _6_0_ _$_m_n_/_M_t_o_n_n_e_ _t_e_c_h_n_o_l_o_g_i_e_s_ _=_ 
 _[_ _T_e_c_h_n_o_l_o_g_y_(_ _i_d_=_"_c_o_a_l_-_g_e_n_"_,_ _o_p_e_r_a_t_i_n_g___l_i_f_e_=_4_0_,_ _#_ _y_e_a_r_s_ _c_a_p_e_x_=_8_0_0_,_ _#_ _m_n_$_/_G_W_ _#
 _s_t_r_a_i_g_h_t_-_l_i_n_e_ _r_e_d_u_c_t_i_o_n_ _t_o_ _2_0_4_0_ _r_e_s_i_d_u_a_l___c_a_p_a_c_i_t_y_=_{_ _y_r_:_ _2_5_ _*_ _m_a_x_(_(_1_ _-_ _(_y_r_ _-
 _2_0_2_0_)_ _/_ _(_2_0_4_0_ _-_ _2_0_2_0_)_,_ _0_)_)_ _f_o_r_ _y_r_ _i_n_ _r_a_n_g_e_(_2_0_2_0_,_ _2_0_5_1_)_ _}_,_ _o_p_e_r_a_t_i_n_g___m_o_d_e_s_=
 _[_ _O_p_e_r_a_t_i_n_g_M_o_d_e_(_ _i_d_=_"_g_e_n_e_r_a_t_i_o_n_"_,_ _#_ _$_m_n_2_0_/_M_t_._c_o_a_l_ _/_ _8_._1_4_ _T_W_h_/_M_t_ _c_o_a_l_ _*_ _8_7_6_0
 _G_W_h_/_G_W_ _/_ _0_._3_ _/_1_0_0_0_ _G_W_h_/_T_W_h_ _(_t_h_e_r_m_ _e_f_f_)_ _o_p_e_x___v_a_r_i_a_b_l_e_=_2_0_ _/_ _8_._1_4_ _*_ _8_7_6_0_ _/_ _0_._3_ _/
 _1_0_0_0_,_ _#_ _$_7_1_/_G_W_/_y_r_ _o_u_t_p_u_t___a_c_t_i_v_i_t_y___r_a_t_i_o_=_{_"_e_l_e_c_t_r_i_c_i_t_y_"_:_ _1_._0_ _*_ _8_7_6_0_}_,_ _#_ _G_W_h_/_y_r_/
 _G_W_ _e_m_i_s_s_i_o_n___a_c_t_i_v_i_t_y___r_a_t_i_o_=_{_ _"_C_O_2_"_:_ _0_._3_5_4_ _*_ _8_7_6_0_ _/_ _1_0_0_0_ _}_,_ _#_ _M_t_c_o_2_/_T_W_h_ _*
@@ -114,15 +114,15 @@
 _c_o_m_p_r_e_h_e_n_s_i_o_n_s_,_ _`_m_i_n_`_,_ _`_m_a_x_`_,_ _`_s_u_m_`_,_ _a_n_d_ _`_r_a_n_g_e_`_ _f_u_n_c_t_i_o_n_s_._ _-_ _f_o_r_ _d_a_t_a_ _k_e_y_e_d_ _b_y
 _a_n_ _o_s_e_m_o_s_y_s_ _`_s_e_t_`_ _(_e_._g_._ _`_Y_E_A_R_S_`_,_ _`_T_I_M_E_S_L_I_C_E_S_`_,_ _`_T_E_C_H_N_O_L_O_G_I_E_S_`_)_,_ _w_i_l_d_c_a_r_d_s_ _`_"_*_"_`
 _c_a_n_ _b_e_ _u_s_e_d_ _i_n_ _p_l_a_c_e_ _o_f_ _e_x_p_l_i_c_i_t_l_y_ _l_i_s_t_i_n_g_ _a_l_l_ _s_e_t_ _m_e_m_b_e_r_s_._ _-_ _d_a_t_a_ _f_i_e_l_d_ _`_s_e_t_`
 _d_i_m_e_n_s_i_o_n_s_ _a_n_d_ _m_e_m_b_e_r_s_h_i_p_ _a_r_e_ _a_l_s_o_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _i_n_f_e_r_r_e_d_ _-_ _a_ _s_i_n_g_l_e_ _v_a_l_u_e_ _c_a_n
 _b_e_ _g_i_v_e_n_ _w_h_i_c_h_ _w_i_l_l_ _b_e_ _b_r_o_a_d_c_a_s_t_ _t_o_ _a_l_l_ _s_e_t_ _m_e_m_b_e_r_ _c_o_m_b_i_n_a_t_i_o_n_s_._ _-_ _s_i_n_g_l_e_ _o_r
 _m_u_l_t_i_p_l_e_ _`_._y_a_m_l_`_ _f_i_l_e_s_ _c_a_n_ _b_e_ _c_o_m_p_o_s_e_d_ _t_o_g_e_t_h_e_r_,_ _a_l_l_o_w_i_n_g_ _y_o_u_ _t_o_ _s_e_p_a_r_a_t_e_,_ _e_._g_.
 _`_t_e_c_h_n_o_l_o_g_i_e_s_._y_a_m_l_`_,_ _f_r_o_m_ _t_h_e_ _r_e_s_t_ _o_f_ _y_o_u_r_ _m_o_d_e_l_._ _`_`_`_p_y_t_h_o_n_ _f_r_o_m_ _t_z_._o_s_e_m_o_s_y_s
-_i_m_p_o_r_t_ _l_o_a_d___m_o_d_e_l_ _m_y___m_o_d_e_l_ _=_ _l_o_a_d___m_o_d_e_l_(_"_p_a_t_h_/_t_o_/_y_a_m_l_/_d_i_r_e_c_t_o_r_y_"_)_ _`_`_`_ _#_#_#_ _F_r_o_m
+_i_m_p_o_r_t_ _M_o_d_e_l_ _m_y___m_o_d_e_l_ _=_ _M_o_d_e_l_._f_r_o_m___y_a_m_l_(_"_p_a_t_h_/_t_o_/_y_a_m_l_/_d_i_r_e_c_t_o_r_y_"_)_ _`_`_`_ _#_#_#_ _F_r_o_m
 _O_t_o_o_l_e_ _o_u_t_p_u_t_s_ _(_l_e_g_a_c_y_)_ _T_Z_-_O_S_e_M_O_S_Y_S_ _i_s_ _p_r_o_v_i_d_e_d_ _w_i_t_h_ _b_a_c_k_w_a_r_d_s_ _c_o_m_p_a_t_a_b_i_l_i_t_y
 _w_i_t_h_ _t_h_e_ _[_o_t_o_o_l_e_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_O_S_e_M_O_S_Y_S_/_o_t_o_o_l_e_)_ _o_s_e_m_o_s_y_s_ _t_o_o_l_i_n_g_._ _A_n_y
 _l_e_g_a_c_y_ _m_o_d_e_l_s_ _c_a_n_ _b_e_ _l_o_a_d_e_d_ _f_r_o_m_ _t_h_e_ _d_i_r_e_c_t_o_r_y_ _o_f_ _o_t_o_o_l_e_-_f_o_r_m_a_t_t_e_d_ _c_s_v_s_.
 _`_`_`_p_y_t_h_o_n_ _f_r_o_m_ _t_z_._o_s_e_m_o_s_y_s_ _i_m_p_o_r_t_ _M_o_d_e_l_ _m_y___m_o_d_e_l_ _=_ _M_o_d_e_l_._f_r_o_m___o_t_o_o_l_e___c_s_v_(_"_p_a_t_h_/
 _t_o_/_o_t_o_o_l_e_/_c_s_v_/_d_i_r_e_c_t_o_r_y_"_)_ _`_`_`_ _R_e_a_d_ _m_o_r_e_ _i_n_ _t_h_e_ _[_d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/
 _d_o_c_s_._f_e_o_._t_r_a_n_s_i_t_i_o_n_z_e_r_o_._o_r_g_/_)_ _#_#_#_ _D_e_v_e_l_o_p_m_e_n_t_ _a_n_d_ _C_o_n_t_r_i_b_u_t_i_n_g_ _W_e_ _w_e_l_c_o_m_e
 _c_o_n_t_r_i_b_u_t_i_o_n_s_!_ _T_o_ _g_e_t_ _s_t_a_r_t_e_d_ _a_s_ _a_ _c_o_n_t_r_i_b_u_t_o_r_ _o_r_ _a_s_ _a_ _d_e_v_e_l_o_p_e_r_,_ _p_l_e_a_s_e_ _r_e_a_d
```

### Comparing `tz-osemosys-0.0.1/README.md` & `tz_osemosys-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 HiGHS can be installed from source using `cmake` following the instructions [here](https://github.com/ERGO-Code/HiGHS?tab=readme-ov-file#installation). You'll need to install a cmake distribution for your relevant operating system.
 
 *common issue: make sure you have write-privileges to default directory for `cmake --install build`, or either run this command with administrator privileges (`sudo cmake --install build` on mac and linux) or specify a different build directory*
 
 ### Docker installation
 
-A docker container is provided that contains Python 3.11 and an installed version of HiGHS. You'll nedd to [install a docker distribution](https://docs.docker.com/engine/install/) relevant for your operating system.
+A docker container is provided that contains Python 3.11 and an installed version of HiGHS. You'll need to [install a docker distribution](https://docs.docker.com/engine/install/) relevant for your operating system.
 
 The docker container is used in testing, but can also be used for local development work. The following docker command will run and enter the docker container, mount the current working directory at the `/home` directory, and change directory within the container to this directory.
 
 ```console
 docker run -v $(pwd):/home -it  ghcr.io/transition-zero/tz-highs/highs-python:latest /bin/bash -c 'cd /home && /bin/bash'
 ```
 
@@ -100,15 +100,15 @@
     Impact,
     OperatingMode,
 )
 
 time_definition = TimeDefinition(id="years-only", years=range(2020, 2051))
 regions = [Region(id="single-region")]
 commodities = [Commodity(id="electricity", demand_annual=25 * 8760)]  # 25GW * 8760hr/yr
-impacts = [Impact(id="CO2", penalty=60)]  # 10 $mn/Mtonne
+impacts = [Impact(id="CO2", penalty=60)]  # 60 $mn/Mtonne
 technologies = [
     Technology(
         id="coal-gen",
         operating_life=40,  # years
         capex=800,  # mn$/GW
         # straight-line reduction to 2040
         residual_capacity={
@@ -163,17 +163,17 @@
 - model fields can also be populated from environment variables: `my_field: $ENV{MYVAR}`.
 - simple Python expressions are automatically evaluated, including list comprehensions, dictionary comprehensions, `min`, `max`, `sum`, and `range` functions.
 - for data keyed by an osemosys `set` (e.g. `YEARS`, `TIMESLICES`, `TECHNOLOGIES`), wildcards `"*"` can be used in place of explicitly listing all set members.
 - data field `set` dimensions and membership are also automatically inferred - a single value can be given which will be broadcast to all set member combinations.
 - single or multiple `.yaml` files can be composed together, allowing you to separate, e.g. `technologies.yaml`, from the rest of your model.
 
 ```python
-from tz.osemosys import load_model
+from tz.osemosys import Model
 
-my_model = load_model("path/to/yaml/directory")
+my_model = Model.from_yaml("path/to/yaml/directory")
 ```
 
 ### From Otoole outputs (legacy)
 
 TZ-OSeMOSYS is provided with backwards compatability with the [otoole](https://github.com/OSeMOSYS/otoole) osemosys tooling. Any legacy models can be loaded from the directory of otoole-formatted csvs.
 
 ```python
```

#### html2text {}

```diff
@@ -45,15 +45,15 @@
 _(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_E_R_G_O_-_C_o_d_e_/_H_i_G_H_S_?_t_a_b_=_r_e_a_d_m_e_-_o_v_-_f_i_l_e_#_i_n_s_t_a_l_l_a_t_i_o_n_)_._ _Y_o_u_'_l_l
 _n_e_e_d_ _t_o_ _i_n_s_t_a_l_l_ _a_ _c_m_a_k_e_ _d_i_s_t_r_i_b_u_t_i_o_n_ _f_o_r_ _y_o_u_r_ _r_e_l_e_v_a_n_t_ _o_p_e_r_a_t_i_n_g_ _s_y_s_t_e_m_.
 _*_c_o_m_m_o_n_ _i_s_s_u_e_:_ _m_a_k_e_ _s_u_r_e_ _y_o_u_ _h_a_v_e_ _w_r_i_t_e_-_p_r_i_v_i_l_e_g_e_s_ _t_o_ _d_e_f_a_u_l_t_ _d_i_r_e_c_t_o_r_y_ _f_o_r
 _`_c_m_a_k_e_ _-_-_i_n_s_t_a_l_l_ _b_u_i_l_d_`_,_ _o_r_ _e_i_t_h_e_r_ _r_u_n_ _t_h_i_s_ _c_o_m_m_a_n_d_ _w_i_t_h_ _a_d_m_i_n_i_s_t_r_a_t_o_r
 _p_r_i_v_i_l_e_g_e_s_ _(_`_s_u_d_o_ _c_m_a_k_e_ _-_-_i_n_s_t_a_l_l_ _b_u_i_l_d_`_ _o_n_ _m_a_c_ _a_n_d_ _l_i_n_u_x_)_ _o_r_ _s_p_e_c_i_f_y_ _a
 _d_i_f_f_e_r_e_n_t_ _b_u_i_l_d_ _d_i_r_e_c_t_o_r_y_*_ _#_#_#_ _D_o_c_k_e_r_ _i_n_s_t_a_l_l_a_t_i_o_n_ _A_ _d_o_c_k_e_r_ _c_o_n_t_a_i_n_e_r_ _i_s
 _p_r_o_v_i_d_e_d_ _t_h_a_t_ _c_o_n_t_a_i_n_s_ _P_y_t_h_o_n_ _3_._1_1_ _a_n_d_ _a_n_ _i_n_s_t_a_l_l_e_d_ _v_e_r_s_i_o_n_ _o_f_ _H_i_G_H_S_._ _Y_o_u_'_l_l
-_n_e_d_d_ _t_o_ _[_i_n_s_t_a_l_l_ _a_ _d_o_c_k_e_r_ _d_i_s_t_r_i_b_u_t_i_o_n_]_(_h_t_t_p_s_:_/_/_d_o_c_s_._d_o_c_k_e_r_._c_o_m_/_e_n_g_i_n_e_/_i_n_s_t_a_l_l_/
+_n_e_e_d_ _t_o_ _[_i_n_s_t_a_l_l_ _a_ _d_o_c_k_e_r_ _d_i_s_t_r_i_b_u_t_i_o_n_]_(_h_t_t_p_s_:_/_/_d_o_c_s_._d_o_c_k_e_r_._c_o_m_/_e_n_g_i_n_e_/_i_n_s_t_a_l_l_/
 _)_ _r_e_l_e_v_a_n_t_ _f_o_r_ _y_o_u_r_ _o_p_e_r_a_t_i_n_g_ _s_y_s_t_e_m_._ _T_h_e_ _d_o_c_k_e_r_ _c_o_n_t_a_i_n_e_r_ _i_s_ _u_s_e_d_ _i_n_ _t_e_s_t_i_n_g_,
 _b_u_t_ _c_a_n_ _a_l_s_o_ _b_e_ _u_s_e_d_ _f_o_r_ _l_o_c_a_l_ _d_e_v_e_l_o_p_m_e_n_t_ _w_o_r_k_._ _T_h_e_ _f_o_l_l_o_w_i_n_g_ _d_o_c_k_e_r_ _c_o_m_m_a_n_d
 _w_i_l_l_ _r_u_n_ _a_n_d_ _e_n_t_e_r_ _t_h_e_ _d_o_c_k_e_r_ _c_o_n_t_a_i_n_e_r_,_ _m_o_u_n_t_ _t_h_e_ _c_u_r_r_e_n_t_ _w_o_r_k_i_n_g_ _d_i_r_e_c_t_o_r_y_ _a_t
 _t_h_e_ _`_/_h_o_m_e_`_ _d_i_r_e_c_t_o_r_y_,_ _a_n_d_ _c_h_a_n_g_e_ _d_i_r_e_c_t_o_r_y_ _w_i_t_h_i_n_ _t_h_e_ _c_o_n_t_a_i_n_e_r_ _t_o_ _t_h_i_s
 _d_i_r_e_c_t_o_r_y_._ _`_`_`_c_o_n_s_o_l_e_ _d_o_c_k_e_r_ _r_u_n_ _-_v_ _$_(_p_w_d_)_:_/_h_o_m_e_ _-_i_t_ _g_h_c_r_._i_o_/_t_r_a_n_s_i_t_i_o_n_-_z_e_r_o_/
 _t_z_-_h_i_g_h_s_/_h_i_g_h_s_-_p_y_t_h_o_n_:_l_a_t_e_s_t_ _/_b_i_n_/_b_a_s_h_ _-_c_ _'_c_d_ _/_h_o_m_e_ _&_&_ _/_b_i_n_/_b_a_s_h_'_ _`_`_`_ _*_n_o_t_e_!
 _A_n_y_ _f_i_l_e_s_ _c_h_a_n_g_e_d_ _w_i_t_h_i_n_ _t_h_i_s_ _m_o_u_n_t_e_d_ _d_i_r_e_c_t_o_r_y_ _w_i_l_l_ _p_e_r_s_i_s_t_,_ _b_u_t_ _a_n_y_ _c_h_a_n_g_e_s
@@ -65,15 +65,15 @@
 _b_e_t_w_e_e_n_ _t_h_e_ _o_b_j_e_c_t_ _t_y_p_e_s_._ _T_h_e_ _s_e_t_ _o_f_ _o_b_j_e_c_t_s_ _c_o_m_p_r_i_s_i_n_g_ _t_h_e_ _m_o_d_e_l_ _i_s_ _m_u_t_u_a_l_l_y
 _e_x_c_l_u_s_i_v_e_ _-_ _n_o_ _i_n_f_o_r_m_a_t_i_o_n_ _i_s_ _r_e_p_e_a_t_e_d_ _-_ _a_n_d_ _c_o_l_l_e_c_t_i_v_e_l_y_ _e_x_h_a_u_s_t_i_v_e_ _-_ _n_o
 _i_n_f_o_r_m_a_t_i_o_n_ _n_e_e_d_s_ _t_o_ _b_e_ _e_x_t_r_a_c_t_e_d_ _f_r_o_m_ _c_s_v_s_ _o_r_ _o_t_h_e_r_ _d_a_t_a_ _s_o_u_r_c_e_s_._ _`_`_`_p_y_t_h_o_n
 _f_r_o_m_ _t_z_._o_s_e_m_o_s_y_s_ _i_m_p_o_r_t_ _(_ _M_o_d_e_l_,_ _T_e_c_h_n_o_l_o_g_y_,_ _T_i_m_e_D_e_f_i_n_i_t_i_o_n_,_ _C_o_m_m_o_d_i_t_y_,_ _R_e_g_i_o_n_,
 _I_m_p_a_c_t_,_ _O_p_e_r_a_t_i_n_g_M_o_d_e_,_ _)_ _t_i_m_e___d_e_f_i_n_i_t_i_o_n_ _=_ _T_i_m_e_D_e_f_i_n_i_t_i_o_n_(_i_d_=_"_y_e_a_r_s_-_o_n_l_y_"_,
 _y_e_a_r_s_=_r_a_n_g_e_(_2_0_2_0_,_ _2_0_5_1_)_)_ _r_e_g_i_o_n_s_ _=_ _[_R_e_g_i_o_n_(_i_d_=_"_s_i_n_g_l_e_-_r_e_g_i_o_n_"_)_]_ _c_o_m_m_o_d_i_t_i_e_s_ _=_ 
 _[_C_o_m_m_o_d_i_t_y_(_i_d_=_"_e_l_e_c_t_r_i_c_i_t_y_"_,_ _d_e_m_a_n_d___a_n_n_u_a_l_=_2_5_ _*_ _8_7_6_0_)_]_ _#_ _2_5_G_W_ _*_ _8_7_6_0_h_r_/_y_r
-_i_m_p_a_c_t_s_ _=_ _[_I_m_p_a_c_t_(_i_d_=_"_C_O_2_"_,_ _p_e_n_a_l_t_y_=_6_0_)_]_ _#_ _1_0_ _$_m_n_/_M_t_o_n_n_e_ _t_e_c_h_n_o_l_o_g_i_e_s_ _=_ 
+_i_m_p_a_c_t_s_ _=_ _[_I_m_p_a_c_t_(_i_d_=_"_C_O_2_"_,_ _p_e_n_a_l_t_y_=_6_0_)_]_ _#_ _6_0_ _$_m_n_/_M_t_o_n_n_e_ _t_e_c_h_n_o_l_o_g_i_e_s_ _=_ 
 _[_ _T_e_c_h_n_o_l_o_g_y_(_ _i_d_=_"_c_o_a_l_-_g_e_n_"_,_ _o_p_e_r_a_t_i_n_g___l_i_f_e_=_4_0_,_ _#_ _y_e_a_r_s_ _c_a_p_e_x_=_8_0_0_,_ _#_ _m_n_$_/_G_W_ _#
 _s_t_r_a_i_g_h_t_-_l_i_n_e_ _r_e_d_u_c_t_i_o_n_ _t_o_ _2_0_4_0_ _r_e_s_i_d_u_a_l___c_a_p_a_c_i_t_y_=_{_ _y_r_:_ _2_5_ _*_ _m_a_x_(_(_1_ _-_ _(_y_r_ _-
 _2_0_2_0_)_ _/_ _(_2_0_4_0_ _-_ _2_0_2_0_)_,_ _0_)_)_ _f_o_r_ _y_r_ _i_n_ _r_a_n_g_e_(_2_0_2_0_,_ _2_0_5_1_)_ _}_,_ _o_p_e_r_a_t_i_n_g___m_o_d_e_s_=
 _[_ _O_p_e_r_a_t_i_n_g_M_o_d_e_(_ _i_d_=_"_g_e_n_e_r_a_t_i_o_n_"_,_ _#_ _$_m_n_2_0_/_M_t_._c_o_a_l_ _/_ _8_._1_4_ _T_W_h_/_M_t_ _c_o_a_l_ _*_ _8_7_6_0
 _G_W_h_/_G_W_ _/_ _0_._3_ _/_1_0_0_0_ _G_W_h_/_T_W_h_ _(_t_h_e_r_m_ _e_f_f_)_ _o_p_e_x___v_a_r_i_a_b_l_e_=_2_0_ _/_ _8_._1_4_ _*_ _8_7_6_0_ _/_ _0_._3_ _/
 _1_0_0_0_,_ _#_ _$_7_1_/_G_W_/_y_r_ _o_u_t_p_u_t___a_c_t_i_v_i_t_y___r_a_t_i_o_=_{_"_e_l_e_c_t_r_i_c_i_t_y_"_:_ _1_._0_ _*_ _8_7_6_0_}_,_ _#_ _G_W_h_/_y_r_/
 _G_W_ _e_m_i_s_s_i_o_n___a_c_t_i_v_i_t_y___r_a_t_i_o_=_{_ _"_C_O_2_"_:_ _0_._3_5_4_ _*_ _8_7_6_0_ _/_ _1_0_0_0_ _}_,_ _#_ _M_t_c_o_2_/_T_W_h_ _*
@@ -93,15 +93,15 @@
 _c_o_m_p_r_e_h_e_n_s_i_o_n_s_,_ _`_m_i_n_`_,_ _`_m_a_x_`_,_ _`_s_u_m_`_,_ _a_n_d_ _`_r_a_n_g_e_`_ _f_u_n_c_t_i_o_n_s_._ _-_ _f_o_r_ _d_a_t_a_ _k_e_y_e_d_ _b_y
 _a_n_ _o_s_e_m_o_s_y_s_ _`_s_e_t_`_ _(_e_._g_._ _`_Y_E_A_R_S_`_,_ _`_T_I_M_E_S_L_I_C_E_S_`_,_ _`_T_E_C_H_N_O_L_O_G_I_E_S_`_)_,_ _w_i_l_d_c_a_r_d_s_ _`_"_*_"_`
 _c_a_n_ _b_e_ _u_s_e_d_ _i_n_ _p_l_a_c_e_ _o_f_ _e_x_p_l_i_c_i_t_l_y_ _l_i_s_t_i_n_g_ _a_l_l_ _s_e_t_ _m_e_m_b_e_r_s_._ _-_ _d_a_t_a_ _f_i_e_l_d_ _`_s_e_t_`
 _d_i_m_e_n_s_i_o_n_s_ _a_n_d_ _m_e_m_b_e_r_s_h_i_p_ _a_r_e_ _a_l_s_o_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _i_n_f_e_r_r_e_d_ _-_ _a_ _s_i_n_g_l_e_ _v_a_l_u_e_ _c_a_n
 _b_e_ _g_i_v_e_n_ _w_h_i_c_h_ _w_i_l_l_ _b_e_ _b_r_o_a_d_c_a_s_t_ _t_o_ _a_l_l_ _s_e_t_ _m_e_m_b_e_r_ _c_o_m_b_i_n_a_t_i_o_n_s_._ _-_ _s_i_n_g_l_e_ _o_r
 _m_u_l_t_i_p_l_e_ _`_._y_a_m_l_`_ _f_i_l_e_s_ _c_a_n_ _b_e_ _c_o_m_p_o_s_e_d_ _t_o_g_e_t_h_e_r_,_ _a_l_l_o_w_i_n_g_ _y_o_u_ _t_o_ _s_e_p_a_r_a_t_e_,_ _e_._g_.
 _`_t_e_c_h_n_o_l_o_g_i_e_s_._y_a_m_l_`_,_ _f_r_o_m_ _t_h_e_ _r_e_s_t_ _o_f_ _y_o_u_r_ _m_o_d_e_l_._ _`_`_`_p_y_t_h_o_n_ _f_r_o_m_ _t_z_._o_s_e_m_o_s_y_s
-_i_m_p_o_r_t_ _l_o_a_d___m_o_d_e_l_ _m_y___m_o_d_e_l_ _=_ _l_o_a_d___m_o_d_e_l_(_"_p_a_t_h_/_t_o_/_y_a_m_l_/_d_i_r_e_c_t_o_r_y_"_)_ _`_`_`_ _#_#_#_ _F_r_o_m
+_i_m_p_o_r_t_ _M_o_d_e_l_ _m_y___m_o_d_e_l_ _=_ _M_o_d_e_l_._f_r_o_m___y_a_m_l_(_"_p_a_t_h_/_t_o_/_y_a_m_l_/_d_i_r_e_c_t_o_r_y_"_)_ _`_`_`_ _#_#_#_ _F_r_o_m
 _O_t_o_o_l_e_ _o_u_t_p_u_t_s_ _(_l_e_g_a_c_y_)_ _T_Z_-_O_S_e_M_O_S_Y_S_ _i_s_ _p_r_o_v_i_d_e_d_ _w_i_t_h_ _b_a_c_k_w_a_r_d_s_ _c_o_m_p_a_t_a_b_i_l_i_t_y
 _w_i_t_h_ _t_h_e_ _[_o_t_o_o_l_e_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_O_S_e_M_O_S_Y_S_/_o_t_o_o_l_e_)_ _o_s_e_m_o_s_y_s_ _t_o_o_l_i_n_g_._ _A_n_y
 _l_e_g_a_c_y_ _m_o_d_e_l_s_ _c_a_n_ _b_e_ _l_o_a_d_e_d_ _f_r_o_m_ _t_h_e_ _d_i_r_e_c_t_o_r_y_ _o_f_ _o_t_o_o_l_e_-_f_o_r_m_a_t_t_e_d_ _c_s_v_s_.
 _`_`_`_p_y_t_h_o_n_ _f_r_o_m_ _t_z_._o_s_e_m_o_s_y_s_ _i_m_p_o_r_t_ _M_o_d_e_l_ _m_y___m_o_d_e_l_ _=_ _M_o_d_e_l_._f_r_o_m___o_t_o_o_l_e___c_s_v_(_"_p_a_t_h_/
 _t_o_/_o_t_o_o_l_e_/_c_s_v_/_d_i_r_e_c_t_o_r_y_"_)_ _`_`_`_ _R_e_a_d_ _m_o_r_e_ _i_n_ _t_h_e_ _[_d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/
 _d_o_c_s_._f_e_o_._t_r_a_n_s_i_t_i_o_n_z_e_r_o_._o_r_g_/_)_ _#_#_#_ _D_e_v_e_l_o_p_m_e_n_t_ _a_n_d_ _C_o_n_t_r_i_b_u_t_i_n_g_ _W_e_ _w_e_l_c_o_m_e
 _c_o_n_t_r_i_b_u_t_i_o_n_s_!_ _T_o_ _g_e_t_ _s_t_a_r_t_e_d_ _a_s_ _a_ _c_o_n_t_r_i_b_u_t_o_r_ _o_r_ _a_s_ _a_ _d_e_v_e_l_o_p_e_r_,_ _p_l_e_a_s_e_ _r_e_a_d
```

### Comparing `tz-osemosys-0.0.1/bin/memory_profile.py` & `tz_osemosys-0.0.3/bin/memory_profile.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/pyproject.toml` & `tz_osemosys-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tz-osemosys"  # Required
-version = "0.0.1"  # Required
+version = "0.0.3"  # Required
 description = "An OSeMOSYS implementation for the Future Energy Outlook by TransitionZero"  # Optional
 readme = "README.md" # Optional
 requires-python = ">=3.11"
 license = {file = "LICENSE.txt"}
 keywords = ["energy", "milp", "climate"]  # Optional
 authors = [
   {name = "Lucas Kruitwagen", email = "lucas.kruitwagen@gmail.com" },
@@ -32,30 +32,33 @@
 
 dependencies = [
   "pydantic>2",
   "pydantic-settings",
   "xarray",
   "orjson",
   "linopy",
-  "highspy",
+
 ]
 
 [project.optional-dependencies] # Optional
 dev = [
   "pre-commit",
   "black",
   "pytest",
   "pytest-order",
   "pytest-cov",
   "pytest-asyncio",
   "mypy",
   "tox",
   "coverage",
+  "highspy",
 ]
 
+
+
 [project.urls]  # Optional
 "Homepage" = "https://github.com/transitionzero/tz-osemosys"
 "Bug Reports" = "https://github.com/transitionzero/tz-osemosys/issues"
 "Funding" = "https://transitionzero.org"
 "Source" = "https://github.com/transitionzero/tz-osemosys"
 
 # The following would provide a command line executable called `sample`
```

### Comparing `tz-osemosys-0.0.1/tests/fixtures/misc.py` & `tz_osemosys-0.0.3/tests/fixtures/misc.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_compatability/test_otoole_commodity.py` & `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_commodity.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_compatability/test_otoole_impact.py` & `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_impact.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_compatability/test_otoole_region.py` & `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_region.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_compatability/test_otoole_roundtrip.py` & `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_roundtrip.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,30 +8,23 @@
 
 def test_files_equality():
     """
     Check CSVs are equivalent after creating a RunSpec object from CSVs and writing to CSVs
     """
 
     # to be implemented
+    # TODO
+
     EXCLUDE_STEMS = [
-        "OperationalLifeStorage",
+        "DiscountRateIdv",
         "DiscountRateStorage",
-        "CapitalCostStorage",
-        "TechnologyToStorage",
-        "TechnologyFromStorage",
-        "StorageLevelStart",
-        "STORAGE",
-        "StorageMaxChargeRate",
-        "StorageMaxDischargeRate",
-        "MinStorageCharge",
-        "ResidualStorageCapacity",
     ]
 
-    root_dir = "examples/otoole_compat/input_csv/otoole-full-electricity/"
-    output_directory = "tests/otoole_compare/otoole-full-electricity/"
+    root_dir = "examples/otoole_compat/input_csv/otoole-full-electricity-complete/"
+    output_directory = "tests/otoole_compare/otoole-full-electricity-complete/"
 
     create_output_directory(output_directory)
 
     # uses the class method on the base class to instantiate itself
     run_spec_object = RunSpec.from_otoole_csv(root_dir=root_dir)
 
     # Write output CSVs
```

### Comparing `tz-osemosys-0.0.1/tests/test_compatability/test_otoole_runspec.py` & `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_runspec.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_compatability/test_otoole_storage.py` & `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,15 @@
     for path in OTOOLE_SAMPLE_PATHS:
         comparison_model = Path(path).name
         output_directory = Path(comparison_root + comparison_model)
         output_directory.mkdir(parents=True, exist_ok=True)
 
         storage_technologies = Storage.from_otoole_csv(root_dir=path)
 
-        Storage.to_otoole_csv(
-            storage_technologies=storage_technologies, output_directory=output_directory
-        )
+        Storage.to_otoole_csv(storage=storage_technologies, output_directory=output_directory)
 
         if storage_technologies:
             for stem, params in storage_technologies[0].otoole_stems.items():
                 if stem not in storage_technologies[0].otoole_cfg.empty_dfs:
                     left = (
                         pd.read_csv(Path(path) / (stem + ".csv"))
                         .sort_values(params["columns"])
```

### Comparing `tz-osemosys-0.0.1/tests/test_compatability/test_otoole_technology.py` & `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_technology.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_compatability/test_otoole_timedef.py` & `tz_osemosys-0.0.3/tests/test_compatability/test_otoole_timedef.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_composition/test_compose_base.py` & `tz_osemosys-0.0.3/tests/test_composition/test_compose_base.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_composition/test_compose_runspec.py` & `tz_osemosys-0.0.3/tests/test_composition/test_compose_runspec.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,59 +9,79 @@
             timeslices=["A", "B", "C", "D"],
         ),
         regions=[dict(id="GB")],
         commodities=[dict(id="COAL")],
         impacts=[dict(id="CO2e")],
         technologies=[
             dict(
-                id="most_basic",
+                id="coal_powerplant",
                 operating_life=10,
                 capex=15,
                 opex_fixed=1.5,
                 operating_modes=[
                     dict(
                         id="mode_1",
                         opex_variable=1.5,
                         input_activity_ratio={"COAL": 1.0},
+                        emission_activity_ratio={"CO2e": 100},
                     )
                 ],
-            )
+            ),
+            dict(
+                id="coal_mine",
+                operating_life=10,
+                capex=15,
+                opex_fixed=1.5,
+                operating_modes=[
+                    dict(id="mode_1", opex_variable=1.5, output_activity_ratio={"COAL": 1.0})
+                ],
+            ),
         ],
     ),
     most_basic_with_storage=dict(
         time_definition=dict(
             id="yearpart-daypart",
             years=range(2020, 2051),
             timeslices=["A", "B", "C", "D"],
         ),
         regions=[dict(id="GB")],
         commodities=[dict(id="COAL")],
         impacts=[dict(id="CO2e")],
         technologies=[
             dict(
-                id="most_basic",
+                id="coal_powerplant",
                 operating_life=10,
                 capex=15,
                 opex_fixed=1.5,
                 operating_modes=[
                     dict(
                         id="mode_1",
                         opex_variable=1.5,
                         input_activity_ratio={"COAL": 1.0},
+                        emission_activity_ratio={"CO2e": 100},
                         to_storage={"*": {"STO": 1}},
                         from_storage={"*": {"STO": 1}},
                     )
                 ],
-            )
+            ),
+            dict(
+                id="coal_mine",
+                operating_life=10,
+                capex=15,
+                opex_fixed=1.5,
+                operating_modes=[
+                    dict(id="mode_1", opex_variable=1.5, output_activity_ratio={"COAL": 1.0})
+                ],
+            ),
         ],
         storage=[
             dict(
                 id="STO",
                 capex={"*": {"*": 100}},
-                operating_life={"*": {"*": 10}},
+                operating_life={"*": 10},
             )
         ],
     ),
 )
 
 
 def test_compose_runspec():
```

### Comparing `tz-osemosys-0.0.1/tests/test_construction/test_base.py` & `tz_osemosys-0.0.3/tests/test_construction/test_base.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_construction/test_commodity.py` & `tz_osemosys-0.0.3/tests/test_construction/test_commodity.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_construction/test_data.py` & `tz_osemosys-0.0.3/tests/test_construction/test_data.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_construction/test_impact.py` & `tz_osemosys-0.0.3/tests/test_construction/test_impact.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_construction/test_load_from_yaml.py` & `tz_osemosys-0.0.3/tests/test_construction/test_load_from_yaml.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         b: 2
     """
     data = yaml.load(blob, Loader=yaml.SafeLoader)
 
     sub_functions = substitute_factory(data)
 
     for f in sub_functions:
-        data = walk_dict(data, f)
+        walk_dict(data, f)
 
     assert data["myxref"] == 42
     assert data["xref2"][2]["a"] == 10.0
 
 
 def test_expression_parse():
     blob = """
@@ -45,15 +45,15 @@
     c: max([4,5,6])
     d: min([4,5,6])
     e: '{k:v for k,v in zip(["x","y","z"],[1,2,3])}'
     f: '{k:k+1 for k in range(3)}'
     """
     data = yaml.load(blob, Loader=yaml.SafeLoader)
 
-    data = walk_dict(data, maybe_eval_string)
+    walk_dict(data, maybe_eval_string)
     assert isinstance(data["a"], list)
     assert data["b"] == 3
     assert data["c"] == 6
     assert data["d"] == 4
     assert isinstance(data["e"], dict)
     assert data["e"]["x"] == 1
     assert data["f"][0] == 1
```

### Comparing `tz-osemosys-0.0.1/tests/test_construction/test_model.py` & `tz_osemosys-0.0.3/tests/test_construction/test_model.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_construction/test_region.py` & `tz_osemosys-0.0.3/tests/test_construction/test_region.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import pytest
 
 from tz.osemosys.schemas.region import Region
 
 PASSING_REGION_DEFINITIONS = dict(
     super_basic=dict(id="GB"),
-    with_neighbours=dict(
-        id="GB",
-        neighbours=["FR", "IE"],
-    ),
     with_trade_route=dict(
         id="GB",
         trade_routes={"FR": True, "IE": False},
     ),
 )
 
 FAILING_REGION_DEFINITIONS = dict()
```

### Comparing `tz-osemosys-0.0.1/tests/test_construction/test_storage.py` & `tz_osemosys-0.0.3/tests/test_construction/test_storage.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_construction/test_technology.py` & `tz_osemosys-0.0.3/tests/test_construction/test_technology.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_construction/test_timedefinition.py` & `tz_osemosys-0.0.3/tests/test_construction/test_timedefinition.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import pytest
 
 from tz.osemosys.schemas.time_definition import TimeDefinition
 
 PASSING_TIME_DEFINITIONS = dict(
     # nameplate params inherited from key
+    # Pathway 1
     years_only=dict(years=range(2020, 2051)),
+    # Pathway 3
     timeslices_simple=dict(  # just timeslices - no adjacency
         years=range(2020, 2051), timeslices=["A", "B", "C", "D"]
     ),
+    # Pathway 3
     timeslices_adjacency=dict(  # just timeslices - simple adjacency
         years=range(2020, 2051),
         timeslices=["A", "B", "C", "D"],
         adj={
             "years": dict(zip(range(2020, 2050), range(2021, 2051))),
             "timeslices": dict(zip(["A", "B", "C"], ["B", "C", "D"])),
         },
     ),
+    # Pathway 3
     timeslices_with_parts_for_adj=dict(  # infer adjacency from 'seasons' and 'day_types'
         years=range(2020, 2051),
         timeslices=["A", "B", "C", "D"],
         timeslice_in_season={
             "A": "winter",
             "B": "winter",
             "C": "summer",
@@ -30,28 +34,32 @@
             "B": "weekend",
             "C": "weekday",
             "D": "weekend",
         },
         seasons=["winter", "summer"],
         day_types=["weekday", "weekend"],
     ),
-    yearparts_dayparts_inferred=dict(  # infer timeslices from yearparts and time_brackets
+    # Pathway 2
+    yearparts_dayparts_inferred=dict(  # infer timeslices from yearparts and daily_time_brackets
         years=range(2020, 2051),
         seasons=["winter", "summer"],
-        time_brackets=["morning", "day", "evening", "night"],
+        daily_time_brackets=["morning", "day", "evening", "night"],
     ),
+    # Pathway 2
     yearparts_dayparts_list_of_int=dict(
-        years=range(2020, 2051), seasons=[1, 2], daily_timebrackets=[1, 2]
+        years=range(2020, 2051), seasons=[1, 2], daily_time_brackets=[1, 2]
     ),
+    # Pathway 2
     yearparts_dayparts_list_of_str=dict(
         years=range(2020, 2051),
         seasons=["winter", "spring", "summer", "autumn"],
         day_types=["weekday", "weekend"],
     ),
-    yearparts_dayparts_int=dict(years=range(2020, 2051), seasons=12, daily_time_brackets=6),
+    # # Pathway x
+    # yearparts_dayparts_int=dict(years=range(2020, 2051), seasons=12, daily_time_brackets=6),
 )
 
 FAILING_TIME_DEFINITIONS = dict(
     missing_season_adj=dict(  # some seasons provided - but there's no adjacency
         years=range(2020, 2051),
         timeslices=["A", "B", "C", "D"],
         timeslice_in_season={
```

### Comparing `tz-osemosys-0.0.1/tests/test_integration/test_linopy_model.py` & `tz_osemosys-0.0.3/tests/test_integration/test_linopy_model.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tests/test_solve/test_solve.py` & `tz_osemosys-0.0.3/tests/test_solve/test_solve.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     model = Model.from_yaml(EXAMPLE_YAML)
 
     model._build()
 
     model._m.solve()
 
     assert model._m.termination_condition == "optimal"
-    assert np.round(model._m.objective.value) == 10753472.0
+    assert np.round(model._m.objective.value) == 10746029.0
 
 
 def test_most_simple():
     model = Model(
         id="test-feasibility",
         time_definition=dict(id="years-only", years=range(2020, 2031)),
         regions=[dict(id="single-region")],
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/defaults.py` & `tz_osemosys-0.0.3/tz/osemosys/defaults.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     technology_capacity_activity_unit_ratio: float = Field(1.0)
     technology_capacity_factor: float = Field(1.0)
     technology_availability_factor: float = Field(1.0)
     technology_residual_capacity: float = Field(0.0)
     technology_storage_residual_capacity: float = Field(0.0)
     technology_storage_minimum_charge: float = Field(0.0)
     technology_storage_initial_level: float = Field(0.0)
-    technology_storage_residual_capacity: float = Field(0.0)
     technology_capex: float = Field(0.00001)
     technology_opex_variable_cost: float = Field(0.00001)
     technology_opex_fixed_cost: float = Field(0.0)
     technology_operating_life: int = Field(1)
     depreciation_method: str = "sinking-fund"
     discount_rate: float = Field(0.05)
     reserve_margin: float = Field(1.0)
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/io/load_model.py` & `tz_osemosys-0.0.3/tz/osemosys/io/load_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,18 +101,20 @@
     for f in spec_files:
         cfg.update(yaml.load(open(f), Loader=utils.EnvVarLoader))
 
     # substitute variables denoted by ${var.subvar}
     substitute_functions = utils.substitute_factory(cfg)
 
     for f in substitute_functions:
-        cfg = utils.walk_dict(cfg, f)
+        utils.walk_dict(cfg, f)
 
     # eval strings
-    cfg = utils.walk_dict(cfg, utils.maybe_eval_string)
+    changes_made = True
+    while changes_made:
+        changes_made = utils.walk_dict(cfg, utils.maybe_eval_string)
 
     return cfg
 
 
 def load_model(*spec_files):
     cfg = load_cfg(*spec_files)
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/io/simpleeval.py` & `tz_osemosys-0.0.3/tz/osemosys/io/simpleeval.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,17 +365,17 @@
         # py3k stuff:
         if hasattr(ast, "NameConstant"):
             self.nodes[ast.NameConstant] = self._eval_constant
 
         # py3.6, f-strings
         if hasattr(ast, "JoinedStr"):
             self.nodes[ast.JoinedStr] = self._eval_joinedstr  # f-string
-            self.nodes[
-                ast.FormattedValue
-            ] = self._eval_formattedvalue  # formatted value in f-string
+            self.nodes[ast.FormattedValue] = (
+                self._eval_formattedvalue
+            )  # formatted value in f-string
 
         # py3.8 uses ast.Constant instead of ast.Num, ast.Str, ast.NameConstant
         if hasattr(ast, "Constant"):
             self.nodes[ast.Constant] = self._eval_constant
 
         # Defaults:
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/constraints/__init__.py` & `tz_osemosys-0.0.3/tz/osemosys/model/constraints/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
+from typing import Dict
+
 import xarray as xr
-from linopy import Model
+from linopy import LinearExpression, Model
 
 from .accounting_technology import add_accounting_technology_constraints
 from .annual_activity import add_annual_activity_constraints
 from .capacity_adequacy_a import add_capacity_adequacy_a_constraints
 from .capacity_adequacy_b import add_capacity_adequacy_b_constraints
 from .capital_costs import add_capital_costs_constraints
-from .demand import add_demand_constraints
 from .emissions import add_emissions_constraints
 from .energy_balance_a import add_energy_balance_a_constraints
 from .energy_balance_b import add_energy_balance_b_constraints
 from .new_capacity import add_new_capacity_constraints
 from .operating_costs import add_operating_costs_constraints
 from .re_targets import add_re_targets_constraints
 from .reserve_margin import add_reserve_margin_constraints
 from .salvage_value import add_salvage_value_constraints
+from .storage import add_storage_constraints
 from .total_activity import add_total_activity_constraints
 from .total_capacity import add_total_capacity_constraints
 from .total_discounted_costs import add_total_discounted_costs_constraints
 
 
-def add_constraints(ds: xr.Dataset, m: Model) -> Model:
+def add_constraints(ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]) -> Model:
     """Add all constraints to the model
 
     Arguments
     ---------
     ds: xarray.Dataset
         The parameters dataset
     m: linopy.Model
@@ -32,27 +34,26 @@
 
     Returns
     -------
     linopy.Model
     """
 
     # restore one at a time
-    m = add_demand_constraints(ds, m)
-    m = add_capacity_adequacy_a_constraints(ds, m)
-    m = add_capacity_adequacy_b_constraints(ds, m)
-    m = add_energy_balance_a_constraints(ds, m)
-    m = add_energy_balance_b_constraints(ds, m)
-    m = add_capital_costs_constraints(ds, m)
-    m = add_emissions_constraints(ds, m)
-    m = add_annual_activity_constraints(ds, m)
-    m = add_accounting_technology_constraints(ds, m)
-    m = add_new_capacity_constraints(ds, m)
-    m = add_operating_costs_constraints(ds, m)
-    m = add_re_targets_constraints(ds, m)
-    m = add_reserve_margin_constraints(ds, m)
-    m = add_salvage_value_constraints(ds, m)
-    # m = add_storage_constraints(ds, m)
-    m = add_total_activity_constraints(ds, m)
-    m = add_total_capacity_constraints(ds, m)
-    m = add_total_discounted_costs_constraints(ds, m)
+    m = add_capacity_adequacy_a_constraints(ds, m, lex)
+    m = add_capacity_adequacy_b_constraints(ds, m, lex)
+    m = add_energy_balance_a_constraints(ds, m, lex)
+    m = add_energy_balance_b_constraints(ds, m, lex)
+    m = add_capital_costs_constraints(ds, m, lex)
+    m = add_emissions_constraints(ds, m, lex)
+    m = add_annual_activity_constraints(ds, m, lex)
+    m = add_accounting_technology_constraints(ds, m, lex)
+    m = add_new_capacity_constraints(ds, m, lex)
+    m = add_operating_costs_constraints(ds, m, lex)
+    m = add_re_targets_constraints(ds, m, lex)
+    m = add_reserve_margin_constraints(ds, m, lex)
+    m = add_salvage_value_constraints(ds, m, lex)
+    m = add_storage_constraints(ds, m, lex)
+    m = add_total_activity_constraints(ds, m, lex)
+    m = add_total_capacity_constraints(ds, m, lex)
+    m = add_total_discounted_costs_constraints(ds, m, lex)
 
     return m
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/constraints/accounting_technology.py` & `tz_osemosys-0.0.3/tz/osemosys/model/constraints/accounting_technology.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from typing import Dict
+
 import xarray as xr
-from linopy import Model
+from linopy import LinearExpression, Model
 
 
-def add_accounting_technology_constraints(ds: xr.Dataset, m: Model) -> Model:
+def add_accounting_technology_constraints(
+    ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]
+) -> Model:
     """Add accounting_technology constraints to the model.
     Creates intermediate results variables that are not strictly needed for the optimisation but
     are useful when analysing results. E.g. 'ProductionByTechnology' and 'UseByTechnology'.
 
     Arguments
     ---------
     ds: xarray.Dataset
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/constraints/capacity_adequacy_a.py` & `tz_osemosys-0.0.3/tz/osemosys/model/constraints/capacity_adequacy_a.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from typing import Dict
+
 import xarray as xr
-from linopy import Model
+from linopy import LinearExpression, Model
 
 
-def add_capacity_adequacy_a_constraints(ds: xr.Dataset, m: Model) -> Model:
+def add_capacity_adequacy_a_constraints(
+    ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]
+) -> Model:
     """Add Capacity Adequacy A constraints to the model
     Ensures that there is sufficient capacity of technologies to meet demand(s) in each timeslice.
 
     Arguments
     ---------
     ds: xarray.Dataset
         The parameters dataset
@@ -48,28 +52,26 @@
     s.t. CAa5_TotalNewCapacity{
         r in REGION, t in TECHNOLOGY, y in YEAR: CapacityOfOneTechnologyUnit[r,t,y]<>0}:
         CapacityOfOneTechnologyUnit[r,t,y] * NumberOfNewTechnologyUnits[r,t,y]
         =
         NewCapacity[r,t,y];
     ```
     """
-    new_cap = m["NewCapacity"].rename(YEAR="BUILDYEAR")
-    mask = (ds.YEAR - new_cap.data.BUILDYEAR >= 0) & (
-        ds.YEAR - new_cap.data.BUILDYEAR < ds.OperationalLife
+
+    mask = (ds.YEAR - lex["NewCapacity"].data.BUILDYEAR >= 0) & (
+        ds.YEAR - lex["NewCapacity"].data.BUILDYEAR < ds.OperationalLife
     )
-    con = m["AccumulatedNewCapacity"] - new_cap.where(mask).sum("BUILDYEAR") == 0
+    con = m["AccumulatedNewCapacity"] - lex["NewCapacity"].where(mask).sum("BUILDYEAR") == 0
     m.add_constraints(con, name="CAa1_TotalNewCapacity")
 
     con = m["TotalCapacityAnnual"] - m["AccumulatedNewCapacity"] == ds["ResidualCapacity"].fillna(0)
     m.add_constraints(con, name="CAa2_TotalAnnualCapacity")
 
-    RateOfTotalActivity = m["RateOfActivity"].sum(dims="MODE_OF_OPERATION")
-
     con = (
-        RateOfTotalActivity
+        lex["RateOfTotalActivity"]
         - (m["TotalCapacityAnnual"] * ds["CapacityFactor"] * ds["CapacityToActivityUnit"])
         <= 0
     )
     mask = ~ds["CapacityFactor"].isnull()
     m.add_constraints(con, name="CAa4_Constraint_Capacity", mask=mask)
 
     con = (
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/constraints/capacity_adequacy_b.py` & `tz_osemosys-0.0.3/tz/osemosys/model/constraints/capacity_adequacy_b.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from typing import Dict
+
 import xarray as xr
-from linopy import Model
+from linopy import LinearExpression, Model
 
 
-def add_capacity_adequacy_b_constraints(ds: xr.Dataset, m: Model) -> Model:
+def add_capacity_adequacy_b_constraints(
+    ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]
+) -> Model:
     """Add Capacity Adequacy B constraints to the model.
     Ensures that there is sufficient capacity of technologies to meet demand(s) in each year,
     taking planned maintainence into consideration.
 
     Arguments
     ---------
     ds: xarray.Dataset
@@ -26,18 +30,17 @@
         r in REGION, t in TECHNOLOGY, y in YEAR: AvailabilityFactor[r,t,y] < 1}:
         sum{l in TIMESLICE} RateOfTotalActivity[r,t,l,y] * YearSplit[l,y]
         <=
         sum{l in TIMESLICE} (TotalCapacityAnnual[r,t,y] * CapacityFactor[r,t,l,y] *
         YearSplit[l,y]) * AvailabilityFactor[r,t,y] * CapacityToActivityUnit[r,t];
     ```
     """
-    RateOfTotalActivity = m["RateOfActivity"].sum(dims="MODE_OF_OPERATION")
 
     mask = ds["AvailabilityFactor"] < 1
-    con = (RateOfTotalActivity * ds["YearSplit"]).sum(dims="TIMESLICE") - (
+    con = (lex["RateOfTotalActivity"] * ds["YearSplit"]).sum(dims="TIMESLICE") - (
         (m["TotalCapacityAnnual"] * ds["CapacityFactor"] * ds["YearSplit"]).sum(dims="TIMESLICE")
         * ds["AvailabilityFactor"]
         * ds["CapacityToActivityUnit"]
     ) <= 0
     m.add_constraints(con, name="CAb1_PlannedMaintenance", mask=mask)
 
     return m
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/constraints/emissions.py` & `tz_osemosys-0.0.3/tz/osemosys/model/constraints/emissions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,27 @@
-from typing import Any
+from typing import Dict
 
 import xarray as xr
 from linopy import LinearExpression, Model
-from linopy.common import as_dataarray
 
 
-def passthrough_mul(expr: LinearExpression, other: Any):
-    # Linopy has a hard check on the dimensions of the multiplier,
-    # and doesn't allow casting up dimensions
-    multiplier = as_dataarray(other, coords=expr.coords, dims=expr.coord_dims)
-    coeffs = expr.coeffs * multiplier
-    # assert set(coeffs.shape) == set(expr.coeffs.shape)
-    const = expr.const * multiplier
-    return expr.assign(coeffs=coeffs, const=const)
-
-
-def add_emissions_constraints(ds: xr.Dataset, m: Model) -> Model:
+def add_emissions_constraints(ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]) -> Model:
     """Add Emissions constraints to the model.
     Applies (1) user-defined emission limits annually and for the entire model period,
     (2) Emission penalities, and
     (3) Calculates emissions by technology and year
 
     Arguments
     ---------
     ds: xarray.Dataset
         The parameters dataset
     m: linopy.Model
         A linopy model
+    lex: Dict[str, LinearExpression]
+        A dictionary of linear expressions, persisted after solve
 
     Returns
     -------
     linopy.Model
 
 
     Notes
@@ -91,61 +82,28 @@
         r in REGION, e in EMISSION: ModelPeriodEmissionLimit[r, e] <> -1}:
         ModelPeriodEmissions[r,e]
         <=
         ModelPeriodEmissionLimit[r,e];
         ```
     """
 
-    discount_factor_mid = (1 + ds["DiscountRate"]) ** (
-        ds.coords["YEAR"] - min(ds.coords["YEAR"]) + 0.5
-    )
-
     if ds["EMISSION"].size > 0:
-        TotalAnnualTechnologyActivityByMode = (m["RateOfActivity"] * ds["YearSplit"]).sum(
-            "TIMESLICE"
-        )
-
-        # AnnualTechnologyEmissionByMode = (
-        #     ds["EmissionActivityRatio"] * TotalAnnualTechnologyActivityByMode
-        # ).where(ds["EmissionActivityRatio"].notnull())
-
-        AnnualTechnologyEmissionByMode = (
-            passthrough_mul(TotalAnnualTechnologyActivityByMode, ds["EmissionActivityRatio"])
-        ).where(ds["EmissionActivityRatio"].notnull())
-
-        AnnualTechnologyEmission = AnnualTechnologyEmissionByMode.sum(
-            dims="MODE_OF_OPERATION"
-        ).where(ds["EmissionActivityRatio"].sum("MODE_OF_OPERATION") != 0)
-        AnnualTechnologyEmissionPenaltyByEmission = (
-            AnnualTechnologyEmission * ds["EmissionsPenalty"]
-        ).where(
-            ds["EmissionsPenalty"].notnull()
-            & (ds["EmissionActivityRatio"].sum("MODE_OF_OPERATION") != 0)
-        )
-        AnnualTechnologyEmissionsPenalty = AnnualTechnologyEmissionPenaltyByEmission.sum(
-            dims="EMISSION"
-        )
-
-        AnnualEmissions = AnnualTechnologyEmission.sum(dims="TECHNOLOGY")
-        ModelPeriodEmissions = AnnualEmissions.sum(dims="YEAR") + ds[
-            "ModelPeriodExogenousEmission"
-        ].fillna(0)
 
         con = (
-            AnnualTechnologyEmissionsPenalty / discount_factor_mid
+            lex["AnnualTechnologyEmissionsPenalty"] / lex["DiscountFactorMid"]
             - m["DiscountedTechnologyEmissionsPenalty"]
             == 0
         )
         m.add_constraints(con, name="E5_DiscountedEmissionsPenaltyByTechnology")
 
-        con = AnnualEmissions.fillna(0) <= ds["AnnualEmissionLimit"] - ds[
+        con = lex["AnnualEmissions"].fillna(0) <= ds["AnnualEmissionLimit"] - ds[
             "AnnualExogenousEmission"
         ].fillna(0)
         mask = (ds["AnnualEmissionLimit"] != -1) & (ds["AnnualEmissionLimit"].notnull())
 
         m.add_constraints(con, name="E8_AnnualEmissionsLimit", mask=mask)
 
-        con = ModelPeriodEmissions.fillna(0) <= ds["ModelPeriodEmissionLimit"]
+        con = lex["ModelPeriodEmissions"].fillna(0) <= ds["ModelPeriodEmissionLimit"]
         mask = (ds["ModelPeriodEmissionLimit"] != -1) & (ds["ModelPeriodEmissionLimit"].notnull())
         m.add_constraints(con, name="E9_ModelPeriodEmissionsLimit", mask=mask)
 
     return m
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/constraints/energy_balance_a.py` & `tz_osemosys-0.0.3/tz/osemosys/model/constraints/energy_balance_a.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+from typing import Dict
+
 import xarray as xr
-from linopy import Model
+from linopy import LinearExpression, Model
 
 
-def add_energy_balance_a_constraints(ds: xr.Dataset, m: Model) -> Model:
+def add_energy_balance_a_constraints(
+    ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]
+) -> Model:
     """Add Energy Balance A constraints to the model.
     Ensures that energy balances of all commodities are maintained for each timeslice.
 
     Arguments
     ---------
     ds: xarray.Dataset
         The parameters dataset
     m: linopy.Model
         A linopy model
+    lex: Dict[str, LinearExpression]
+        A dictionary of linear expressions, persisted after solve
 
     Returns
     -------
     linopy.Model
 
 
     Notes
@@ -101,39 +107,16 @@
     """
     tr = ds["TradeRoute"]
     from_mask = tr.where(tr.REGION != tr._REGION).notnull()
     to_mask = tr.where(tr._REGION != tr.REGION).notnull()
     con = m["Trade"].where(from_mask) + m["Trade"].where(to_mask) == 0
     m.add_constraints(con, name="EBa10_EnergyBalanceEachTS4")
 
-    # Linear expressions
-
-    # Production
-    RateOfProductionByTechnologyByMode = m["RateOfActivity"] * ds["OutputActivityRatio"].where(
-        ds["OutputActivityRatio"].notnull()
-    )
-    RateOfProductionByTechnology = RateOfProductionByTechnologyByMode.where(
-        ds["OutputActivityRatio"].sum("MODE_OF_OPERATION") != 0
-    ).sum(dims="MODE_OF_OPERATION")
-    RateOfProduction = RateOfProductionByTechnology.sum(dims="TECHNOLOGY")
-    Production = RateOfProduction * ds["YearSplit"]
-
-    # Use
-    RateOfUseByTechnologyByMode = m["RateOfActivity"] * ds["InputActivityRatio"].where(
-        ds["InputActivityRatio"].notnull()
-    )
-    RateOfUseByTechnology = RateOfUseByTechnologyByMode.where(
-        ds["InputActivityRatio"].sum("MODE_OF_OPERATION") != 0
-    ).sum(dims="MODE_OF_OPERATION")
-    RateOfUse = RateOfUseByTechnology.sum(dims="TECHNOLOGY")
-    Use = RateOfUse * ds["YearSplit"]
-
-    # Demand
-    Demand = (m["RateOfDemand"] * ds["YearSplit"]).where(ds["SpecifiedAnnualDemand"].notnull())
-
     # Constraint
     con = (
-        Production - (Demand + Use + (m["Trade"] * ds["TradeRoute"].fillna(0)).sum(dims="_REGION"))
-        >= 0
-    )
+        lex["Production"]
+        - (ds["SpecifiedAnnualDemand"] * ds["SpecifiedDemandProfile"])
+        - lex["Use"]
+        - (m["Trade"] * ds["TradeRoute"].fillna(0)).sum(dims="_REGION")
+    ) >= 0
     m.add_constraints(con, name="EBa11_EnergyBalanceEachTS5_alt")
     return m
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/constraints/energy_balance_b.py` & `tz_osemosys-0.0.3/tz/osemosys/model/constraints/energy_balance_b.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+from typing import Dict
+
 import xarray as xr
-from linopy import Model
+from linopy import LinearExpression, Model
 
 
-def add_energy_balance_b_constraints(ds: xr.Dataset, m: Model) -> Model:
+def add_energy_balance_b_constraints(
+    ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]
+) -> Model:
     """Add Energy Balance B constraints to the model.
     Ensures that energy balances of all commodities are maintained for each year.
 
     Arguments
     ---------
     ds: xarray.Dataset
         The parameters dataset
     m: linopy.Model
         A linopy model
+    lex: Dict[str, LinearExpression]
+        A dictionary of linear expressions, persisted after solve
 
     Returns
     -------
     linopy.Model
 
 
     Notes
@@ -44,34 +50,13 @@
         ProductionAnnual[r,f,y]
         >=
         UseAnnual[r,f,y] +
         sum{rr in REGION} TradeAnnual[r,rr,f,y] * TradeRoute[r,rr,f,y] +
         AccumulatedAnnualDemand[r,f,y];
     ```
     """
-    # Production
-    RateOfProductionByTechnologyByMode = m["RateOfActivity"] * ds["OutputActivityRatio"].where(
-        ds["OutputActivityRatio"].notnull()
-    )
-    RateOfProductionByTechnology = RateOfProductionByTechnologyByMode.where(
-        ds["OutputActivityRatio"].sum("MODE_OF_OPERATION") != 0
-    ).sum(dims="MODE_OF_OPERATION")
-    RateOfProduction = RateOfProductionByTechnology.sum(dims="TECHNOLOGY")
-    Production = RateOfProduction * ds["YearSplit"]
-    ProductionAnnual = Production.sum(dims="TIMESLICE")
-
-    # Use
-    RateOfUseByTechnologyByMode = m["RateOfActivity"] * ds["InputActivityRatio"].where(
-        ds["InputActivityRatio"].notnull()
-    )
-    RateOfUseByTechnology = RateOfUseByTechnologyByMode.where(
-        ds["InputActivityRatio"].sum("MODE_OF_OPERATION") != 0
-    ).sum(dims="MODE_OF_OPERATION")
-    RateOfUse = RateOfUseByTechnology.sum(dims="TECHNOLOGY")
-    Use = RateOfUse * ds["YearSplit"]
-    UseAnnual = Use.sum(dims="TIMESLICE")
 
-    con = ProductionAnnual - UseAnnual - (
+    con = lex["ProductionAnnual"] - lex["UseAnnual"] - (
         (m["Trade"].sum(["TIMESLICE", "_REGION"])) * ds["TradeRoute"].sum("_REGION")
     ) >= ds["AccumulatedAnnualDemand"].fillna(0)
     m.add_constraints(con, name="EBb4_EnergyBalanceEachYear4")
     return m
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/constraints/new_capacity.py` & `tz_osemosys-0.0.3/tz/osemosys/model/constraints/new_capacity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+from typing import Dict
+
 import xarray as xr
-from linopy import Model
+from linopy import LinearExpression, Model
 
 
-def add_new_capacity_constraints(ds: xr.Dataset, m: Model) -> Model:
+def add_new_capacity_constraints(
+    ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]
+) -> Model:
     """Add New Capacity constraints to the model.
     Constrains new capacity of a technology for each year based on user-defined lower and upper
     limits.
 
     Arguments
     ---------
     ds: xarray.Dataset
         The parameters dataset
     m: linopy.Model
         A linopy model
+    lex: Dict[str, LinearExpression]
+        A dictionary of linear expressions, persisted after solve
 
     Returns
     -------
     linopy.Model
 
 
     Notes
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/constraints/operating_costs.py` & `tz_osemosys-0.0.3/tz/osemosys/model/constraints/operating_costs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+from typing import Dict
+
 import xarray as xr
-from linopy import Model
+from linopy import LinearExpression, Model
 
 
-def add_operating_costs_constraints(ds: xr.Dataset, m: Model) -> Model:
+def add_operating_costs_constraints(
+    ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]
+) -> Model:
     """Add Operating Costs constraint to the model.
     Calculates the total operating expenditure - both discounted and undiscounted - of total (new
     and existing) capacity.
 
     Arguments
     ---------
     ds: xarray.Dataset
         The parameters dataset
     m: linopy.Model
         A linopy model
+    lex: Dict[str, LinearExpression]
 
     Returns
     -------
     linopy.Model
 
 
     Notes
@@ -46,26 +51,10 @@
         r in REGION, t in TECHNOLOGY, y in YEAR}:
         OperatingCost[r,t,y] / DiscountFactorMid[r, y]
         =
         DiscountedOperatingCost[r,t,y];
     ```
     """
 
-    discount_factor_mid = (1 + ds["DiscountRate"]) ** (
-        ds.coords["YEAR"] - min(ds.coords["YEAR"]) + 0.5
-    )
-
-    TotalAnnualTechnologyActivityByMode = (m["RateOfActivity"] * ds["YearSplit"]).sum("TIMESLICE")
-    AnnualVariableOperatingCost = (
-        (TotalAnnualTechnologyActivityByMode * ds["VariableCost"].fillna(0))
-        .sum(dims="MODE_OF_OPERATION")
-        .where(
-            (ds["VariableCost"].sum(dim="MODE_OF_OPERATION") != 0)
-            & (~ds["VariableCost"].sum(dim="MODE_OF_OPERATION").isnull())
-        )
-    )
-    AnnualFixedOperatingCost = m["TotalCapacityAnnual"] * ds["FixedCost"].fillna(0)
-    OperatingCost = AnnualVariableOperatingCost + AnnualFixedOperatingCost
-
-    con = (OperatingCost / discount_factor_mid) - m["DiscountedOperatingCost"] == 0
+    con = (lex["OperatingCost"] / lex["DiscountFactorMid"]) - m["DiscountedOperatingCost"] == 0
     m.add_constraints(con, name="OC4_DiscountedOperatingCostsTotalAnnual")
     return m
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/constraints/re_targets.py` & `tz_osemosys-0.0.3/tz/osemosys/model/constraints/re_targets.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+from typing import Dict
+
 import xarray as xr
-from linopy import Model
+from linopy import LinearExpression, Model
 
 
-def add_re_targets_constraints(ds: xr.Dataset, m: Model) -> Model:
+def add_re_targets_constraints(ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]) -> Model:
     """Add Renewable Energy target constraints to the model.
     Sets user-defined renewable energy constraints for specific years and technologies.
 
     Arguments
     ---------
     ds: xarray.Dataset
         The parameters dataset
     m: linopy.Model
         A linopy model
+    lex: Dict[str, LinearExpression]
+        A dictionary of linear expressions, persisted after solve
 
     Returns
     -------
     linopy.Model
 
 
     Notes
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/constraints/reserve_margin.py` & `tz_osemosys-0.0.3/tz/osemosys/model/linear_expressions/reserve_margin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,59 @@
+from typing import Dict
+
 import xarray as xr
-from linopy import Model
+from linopy import LinearExpression, Model
 
 
-def add_reserve_margin_constraints(ds: xr.Dataset, m: Model) -> Model:
-    """Add Reserve Margin constraints to the model.
-    Ensures that adequate additional capacity, i.e. reserve margin, is available for relevant
-    technologies.
-
-    Arguments
-    ---------
-    ds: xarray.Dataset
-        The parameters dataset
-    m: linopy.Model
-        A linopy model
-
-    Returns
-    -------
-    linopy.Model
-
-
-    Notes
-    -----
-    ```ampl
-    s.t. RM1_ReserveMargin_TechnologiesIncluded_In_Activity_Units{
-        r in REGION, l in TIMESLICE, y in YEAR: ReserveMargin[r,y] > 0}:
-        sum {t in TECHNOLOGY}
-        TotalCapacityAnnual[r,t,y] * ReserveMarginTagTechnology[r,t,y] * CapacityToActivityUnit[r,t]
-        =
-        TotalCapacityInReserveMargin[r,y];
-
-    s.t. RM2_ReserveMargin_FuelsIncluded{
-        r in REGION, l in TIMESLICE, y in YEAR: ReserveMargin[r,y] > 0}:
-        sum {f in FUEL}
-        RateOfProduction[r,l,f,y] * ReserveMarginTagFuel[r,f,y]
-        =
-        DemandNeedingReserveMargin[r,l,y];
-
-    s.t. RM3_ReserveMargin_Constraint{
-        r in REGION, l in TIMESLICE, y in YEAR: ReserveMargin[r,y] > 0}:
-        DemandNeedingReserveMargin[r,l,y] * ReserveMargin[r,y]
-        <=
-        TotalCapacityInReserveMargin[r,y];
-    ```
-    """
+def add_lex_reserve_margin(ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]):
     TotalCapacityInReserveMargin = (
-        ds["ReserveMarginTagTechnology"] * ds["CapacityToActivityUnit"] * m["TotalCapacityAnnual"]
-    ).where((ds["ReserveMargin"] > 0) & (ds["ReserveMarginTagTechnology"] == 1))
-
-    # Production
-    RateOfProductionByTechnologyByMode = m["RateOfActivity"] * ds["OutputActivityRatio"].where(
+        (
+            ds["ReserveMarginTagTechnology"]
+            * ds["CapacityToActivityUnit"]
+            * m["TotalCapacityAnnual"]
+        ).where(
+            (ds["ReserveMargin"] > 0)
+            & (ds["ReserveMarginTagTechnology"] == 1)
+            & (ds["ReserveMarginTagTechnology"] * ds["CapacityToActivityUnit"]).notnull()
+        )
+    ).sum("TECHNOLOGY")
+
+    RateOfProductionByTechnologyByModeWithReserveMargin = m["RateOfActivity"] * ds[
+        "OutputActivityRatio"
+    ].where(
         (ds["OutputActivityRatio"].notnull())
         & (ds["ReserveMargin"] > 0)
         & (ds["ReserveMarginTagFuel"] == 1)
         & (ds["ReserveMarginTagTechnology"] == 1)
     )
-    RateOfProductionByTechnology = RateOfProductionByTechnologyByMode.where(
-        (ds["OutputActivityRatio"].notnull())
-        & (ds["ReserveMargin"] > 0)
-        & (ds["ReserveMarginTagFuel"] == 1)
-        & (ds["ReserveMarginTagTechnology"] == 1)
-    ).sum(dims="MODE_OF_OPERATION")
 
-    RateOfProduction = RateOfProductionByTechnology.where(
+    RateOfProductionByTechnologyWithReserveMargin = (
+        RateOfProductionByTechnologyByModeWithReserveMargin.where(
+            (ds["OutputActivityRatio"].notnull())
+            & (ds["ReserveMargin"] > 0)
+            & (ds["ReserveMarginTagFuel"] == 1)
+            & (ds["ReserveMarginTagTechnology"] == 1)
+        ).sum(dims="MODE_OF_OPERATION")
+    )
+
+    RateOfProductionWithReserveMargin = RateOfProductionByTechnologyWithReserveMargin.where(
         (ds["OutputActivityRatio"].notnull())
         & (ds["ReserveMargin"] > 0)
         & (ds["ReserveMarginTagFuel"] == 1)
         & (ds["ReserveMarginTagTechnology"] == 1)
     ).sum(dims="TECHNOLOGY")
 
-    DemandNeedingReserveMargin = (RateOfProduction * ds["ReserveMarginTagFuel"]).where(
-        (ds["ReserveMargin"] > 0) & (ds["ReserveMarginTagFuel"] == 1)
+    DemandNeedingReserveMargin = (
+        (lex["RateOfProduction"] * ds["ReserveMarginTagFuel"])
+        .where((ds["ReserveMargin"] > 0) & (ds["ReserveMarginTagFuel"] == 1))
+        .sum("FUEL")
     )
 
-    con = (ds["ReserveMargin"] * DemandNeedingReserveMargin - TotalCapacityInReserveMargin) <= 0
-    mask = (
-        (ds["ReserveMargin"] > 0)
-        & (ds["ReserveMarginTagFuel"] == 1)
-        & (ds["ReserveMarginTagTechnology"] == 1)
+    lex.update(
+        {
+            "TotalCapacityInReserveMargin": TotalCapacityInReserveMargin,
+            "RateOfProductionByTechnologyByModeWithReserveMargin": RateOfProductionByTechnologyByModeWithReserveMargin,  # noqa: E501
+            "RateOfProductionByTechnologyWithReserveMargin": RateOfProductionByTechnologyWithReserveMargin,  # noqa: E501
+            "RateOfProductionWithReserveMargin": RateOfProductionWithReserveMargin,
+            "DemandNeedingReserveMargin": DemandNeedingReserveMargin,
+        }
     )
-
-    m.add_constraints(con, name="RM3_ReserveMargin_Constraint", mask=mask)
-
-    return m
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/constraints/total_activity.py` & `tz_osemosys-0.0.3/tz/osemosys/model/constraints/annual_activity.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from typing import Dict
+
 import xarray as xr
-from linopy import Model
+from linopy import LinearExpression, Model
 
 
-def add_total_activity_constraints(ds: xr.Dataset, m: Model) -> Model:
-    """Add Total Activity constraints to the model.
-    Constrains model period activity of a technology based on user-defined lower and upper limits.
+def add_annual_activity_constraints(
+    ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]
+) -> Model:
+    """Add Annual Activity constraints to the model.
+    Constrains annual activity of a technology based on user-defined lower and upper limits.
 
     Arguments
     ---------
     ds: xarray.Dataset
         The parameters dataset
     m: linopy.Model
         A linopy model
@@ -17,38 +21,32 @@
     -------
     linopy.Model
 
 
     Notes
     -----
     ```ampl
-    s.t. TAC1_TotalModelHorizonTechnologyActivity{
-        r in REGION, t in TECHNOLOGY}:
-        sum{y in YEAR} TotalTechnologyAnnualActivity[r,t,y] =
-        TotalTechnologyModelPeriodActivity[r,t];
-
-    s.t. TAC2_TotalModelHorizonTechnologyActivityUpperLimit{
-        r in REGION, t in TECHNOLOGY:
-        TotalTechnologyModelPeriodActivityUpperLimit[r,t]<>-1}:
-        TotalTechnologyModelPeriodActivity[r,t] <=
-        TotalTechnologyModelPeriodActivityUpperLimit[r,t] ;
-
-    s.t. TAC3_TotalModelHorizenTechnologyActivityLowerLimit{
-        r in REGION, t in TECHNOLOGY:
-        TotalTechnologyModelPeriodActivityLowerLimit[r,t]>0}:
-        TotalTechnologyModelPeriodActivity[r,t] >=
-        TotalTechnologyModelPeriodActivityLowerLimit[r,t] ;
+    s.t. AAC1_TotalAnnualTechnologyActivity{
+        r in REGION, t in TECHNOLOGY, y in YEAR}:
+        sum{l in TIMESLICE} RateOfTotalActivity[r,t,l,y]*YearSplit[l,y] =
+        TotalTechnologyAnnualActivity[r,t,y];
+
+    s.t. AAC2_TotalAnnualTechnologyActivityUpperLimit{
+        r in REGION, t in TECHNOLOGY, y in YEAR:
+        TotalTechnologyAnnualActivityUpperLimit[r,t,y] <> -1}:
+        TotalTechnologyAnnualActivity[r,t,y] <= TotalTechnologyAnnualActivityUpperLimit[r,t,y] ;
+
+    s.t. AAC3_TotalAnnualTechnologyActivityLowerLimit{
+        r in REGION, t in TECHNOLOGY, y in YEAR:
+        TotalTechnologyAnnualActivityLowerLimit[r,t,y]>0}:
+        TotalTechnologyAnnualActivity[r,t,y] >= TotalTechnologyAnnualActivityLowerLimit[r,t,y] ;
     ```
     """
-    RateOfTotalActivity = m["RateOfActivity"].sum(dims="MODE_OF_OPERATION")
-    TotalTechnologyAnnualActivity = (RateOfTotalActivity * ds["YearSplit"]).sum("TIMESLICE")
-    TotalTechnologyModelPeriodActivity = TotalTechnologyAnnualActivity.sum(dims="YEAR")
-
-    con = TotalTechnologyModelPeriodActivity <= ds["TotalTechnologyModelPeriodActivityUpperLimit"]
-    mask = ds["TotalTechnologyModelPeriodActivityUpperLimit"] >= 0
-    m.add_constraints(con, name="TAC2_TotalModelHorizonTechnologyActivityUpperLimit", mask=mask)
-
-    con = TotalTechnologyModelPeriodActivity >= ds["TotalTechnologyModelPeriodActivityLowerLimit"]
-    mask = ds["TotalTechnologyModelPeriodActivityLowerLimit"] > 0
-    m.add_constraints(con, name="TAC3_TotalModelHorizenTechnologyActivityLowerLimit", mask=mask)
 
+    con = lex["TotalTechnologyAnnualActivity"] <= ds["TotalTechnologyAnnualActivityUpperLimit"]
+    mask = ds["TotalTechnologyAnnualActivityUpperLimit"] >= 0
+    m.add_constraints(con, name="AAC2_TotalAnnualTechnologyActivityUpperLimit", mask=mask)
+
+    con = lex["TotalTechnologyAnnualActivity"] >= ds["TotalTechnologyAnnualActivityLowerLimit"]
+    mask = ds["TotalTechnologyAnnualActivityLowerLimit"] > 0
+    m.add_constraints(con, name="AAC3_TotalAnnualTechnologyActivityLowerLimit", mask=mask)
     return m
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/constraints/total_discounted_costs.py` & `tz_osemosys-0.0.3/tz/osemosys/model/constraints/total_discounted_costs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+from typing import Dict
+
 import xarray as xr
-from linopy import Model
+from linopy import LinearExpression, Model
 
 
-def add_total_discounted_costs_constraints(ds: xr.Dataset, m: Model) -> Model:
+def add_total_discounted_costs_constraints(
+    ds: xr.Dataset, m: Model, lex: Dict[str, LinearExpression]
+) -> Model:
     """Add Total Discounted Costs constraints to the model.
     Calculates the total discounted costs of the entire system across the entire model period.
 
     Arguments
     ---------
     ds: xarray.Dataset
         The parameters dataset
     m: linopy.Model
         A linopy model
+    lex: Dict[str, LinearExpression]
+
 
     Returns
     -------
     linopy.Model
 
 
     Notes
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/variables/__init__.py` & `tz_osemosys-0.0.3/tz/osemosys/model/variables/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import xarray as xr
 from linopy import Model
 
 from .activity import add_activity_variables
 from .capacity import add_capacity_variables
-from .demand import add_demand_variables
 from .emissions import add_emission_variables
 from .other import add_cost_variables, add_margin_variables, add_re_variables
+from .storage import add_storage_variables
 
 
 def add_variables(ds: xr.Dataset, m: Model) -> Model:
     """Add all variables to the model
 
     Arguments
     ---------
@@ -19,16 +19,15 @@
         A linopy model
 
     Returns
     -------
     linopy.Model
     """
 
-    m = add_demand_variables(ds, m)
-    # m = add_storage_variables(ds, m)
+    m = add_storage_variables(ds, m)
     m = add_capacity_variables(ds, m)
     m = add_activity_variables(ds, m)
     m = add_cost_variables(ds, m)
     m = add_re_variables(ds, m)
     m = add_margin_variables(ds, m)
     m = add_emission_variables(ds, m)
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/variables/activity.py` & `tz_osemosys-0.0.3/tz/osemosys/model/variables/activity.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/variables/capacity.py` & `tz_osemosys-0.0.3/tz/osemosys/model/variables/capacity.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/variables/demand.py` & `tz_osemosys-0.0.3/tz/osemosys/model/variables/emissions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import xarray as xr
 from linopy import Model
 from numpy import inf
 
 
-def add_demand_variables(ds: xr.Dataset, m: Model) -> Model:
-    """Add demand variables to the model
+def add_emission_variables(ds: xr.Dataset, m: Model) -> Model:
+    """Add emisison variables to the model
 
     Arguments
     ---------
     ds: xarray.Dataset
         The parameters dataset
     m: linopy.Model
         A linopy model
 
     Returns
     -------
     linopy.Model
     """
-    RTiFY = [ds.coords["REGION"], ds.coords["TIMESLICE"], ds.coords["FUEL"], ds.coords["YEAR"]]
+    # Create the required indexes
+    RTeY = [ds.coords["REGION"], ds.coords["TECHNOLOGY"], ds.coords["YEAR"]]
+
+    m.add_variables(
+        lower=0, upper=inf, coords=RTeY, name="DiscountedTechnologyEmissionsPenalty", integer=False
+    )
 
-    # mask = ds['SpecifiedAnnualDemand'].expand_dims('TIMESLICE').notnull()
-    m.add_variables(lower=0, upper=inf, coords=RTiFY, name="RateOfDemand", integer=False)
-    m.add_variables(lower=0, upper=inf, coords=RTiFY, name="Demand", integer=False)
     return m
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/variables/other.py` & `tz_osemosys-0.0.3/tz/osemosys/model/variables/other.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/model/variables/storage.py` & `tz_osemosys-0.0.3/tz/osemosys/model/variables/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,31 +13,16 @@
     m: linopy.Model
         A linopy model
 
     Returns
     -------
     linopy.Model
     """
-    # Create the required index
-    RSSDDY = [
-        ds.coords["REGION"],
-        ds.coords["STORAGE"],
-        ds.coords["SEASON"],
-        ds.coords["DAYTYPE"],
-        ds.coords["DAILYTIMEBRACKET"],
-        ds.coords["YEAR"],
-    ]
     RSY = [ds.coords["REGION"], ds.coords["STORAGE"], ds.coords["YEAR"]]
 
-    m.add_variables(lower=-inf, upper=inf, coords=RSSDDY, name="RateOfStorageCharge", integer=False)
-    m.add_variables(
-        lower=-inf, upper=inf, coords=RSSDDY, name="RateOfStorageDischarge", integer=False
-    )
-    m.add_variables(lower=-inf, upper=inf, coords=RSSDDY, name="NetChargeWithinYear", integer=False)
-    m.add_variables(lower=-inf, upper=inf, coords=RSSDDY, name="NetChargeWithinDay", integer=False)
     m.add_variables(lower=0, upper=inf, coords=RSY, name="StorageLevelYearStart", integer=False)
     m.add_variables(lower=0, upper=inf, coords=RSY, name="StorageLevelYearFinish", integer=False)
     coords = [ds.coords["REGION"], ds.coords["STORAGE"], ds.coords["SEASON"], ds.coords["YEAR"]]
     m.add_variables(
         lower=0, upper=inf, coords=coords, name="StorageLevelSeasonStart", integer=False
     )
     coords = [
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/base.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/base.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/compat/base.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/base.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/compat/commodity.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/commodity.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/compat/impact.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/impact.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/compat/model.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from tz.osemosys.schemas.commodity import Commodity
 from tz.osemosys.schemas.compat.base import DefaultsOtoole, OtooleCfg
 from tz.osemosys.schemas.impact import Impact
 from tz.osemosys.schemas.region import Region
 from tz.osemosys.schemas.storage import Storage
 from tz.osemosys.schemas.technology import Technology
 from tz.osemosys.schemas.time_definition import TimeDefinition
+from tz.osemosys.schemas.validation.timedefinition_validation import time_adj_to_list
 from tz.osemosys.utils import flatten, group_to_json
 
 
 class RunSpecOtoole(BaseModel):
     """
     Class to contain methods for converting Runspec data to and from otoole style CSVs,
     and to xarray for use in linopy
@@ -59,17 +60,21 @@
             "columns": ["REGION", "VALUE"],
         },
         "DiscountRate": {
             "attribute": "discount_rate",
             "columns": ["REGION", "VALUE"],
         },
         "DiscountRateIdv": {
-            "attribute": "discount_rate",
+            "attribute": "cost_of_capital",
             "columns": ["REGION", "TECHNOLOGY", "VALUE"],
         },
+        "DiscountRateStorage": {
+            "attribute": "cost_of_capital_storage",
+            "columns": ["REGION", "STORAGE", "VALUE"],
+        },
     }
 
     def map_datatypes(self, df: pd.DataFrame):
         index_cols = df.index.names
         df = df.reset_index()
         for c in df.columns:
             if c == "YEAR":
@@ -120,14 +125,22 @@
         coords = {
             var_name: df["VALUE"].astype(str).tolist()
             for var_name, df in data_dfs.items()
             if var_name.isupper() and var_name != "YEAR"
         }
         coords["YEAR"] = data_dfs["YEAR"]["VALUE"].astype(int).tolist()
 
+        # Order seasons/day_types/time_brackets chronologically by adjacency if provided
+        if coords["SEASON"] and self.time_definition.adj.seasons:
+            coords["SEASON"] = time_adj_to_list(self.time_definition.adj.seasons)
+        if coords["DAYTYPE"] and self.time_definition.adj.day_types:
+            coords["DAYTYPE"] = time_adj_to_list(self.time_definition.adj.day_types)
+        if coords["DAILYTIMEBRACKET"] and self.time_definition.adj.time_brackets:
+            coords["DAILYTIMEBRACKET"] = time_adj_to_list(self.time_definition.adj.time_brackets)
+
         ds = xr.Dataset(data_vars=data_arrays, coords=coords)
 
         # # If runspec not generated using otoole config yaml, use linopy defaults
         # if self.defaults_otoole is None:
         #     default_values = defaults.otoole_name_defaults
         #     # If storage technologies present, use additional relevant default values
         #     if self.storage_technologies:
@@ -211,14 +224,23 @@
                 g=dfs["DiscountRateIdv"],
                 root_column=None,
                 data_columns=["REGION", "TECHNOLOGY"],
                 target_column="VALUE",
             )
         else:
             cost_of_capital = None
+        if "DiscountRateStorage" not in otoole_cfg.empty_dfs:
+            cost_of_capital_storage = group_to_json(
+                g=dfs["DiscountRateStorage"],
+                root_column=None,
+                data_columns=["REGION", "STORAGE"],
+                target_column="VALUE",
+            )
+        else:
+            cost_of_capital_storage = None
 
         # reserve margin and renewable production target
         reserve_margin = (
             group_to_json(
                 g=dfs["ReserveMargin"],
                 root_column=None,
                 data_columns=["REGION", "YEAR"],
@@ -300,14 +322,15 @@
                         reserve_margin_technology_data[technology.id]
                     )
 
         return cls(
             id=id if id else Path(root_dir).name,
             discount_rate=discount_rate or defaults.discount_rate,
             cost_of_capital=cost_of_capital,
+            cost_of_capital_storage=cost_of_capital_storage,
             depreciation_method=depreciation_method or defaults.depreciation_method,
             reserve_margin=reserve_margin or defaults.reserve_margin,
             renewable_production_target=renewable_production_target,
             impacts=impacts,
             regions=regions,
             technologies=technologies,
             storage=storage,
@@ -340,14 +363,21 @@
         if self.cost_of_capital:
             df = pd.json_normalize(self.cost_of_capital.data).T.rename(columns={0: "VALUE"})
             df[["REGION", "TECHNOLOGY"]] = pd.DataFrame(
                 df.index.str.split(".").to_list(), index=df.index
             )
             dfs["DiscountRateIdv"] = df
 
+        if self.cost_of_capital_storage:
+            df = pd.json_normalize(self.cost_of_capital_storage.data).T.rename(columns={0: "VALUE"})
+            df[["REGION", "STORAGE"]] = pd.DataFrame(
+                df.index.str.split(".").to_list(), index=df.index
+            )
+            dfs["DiscountRateStorage"] = df
+
         # reserve margins
         if self.reserve_margin:
             df = pd.json_normalize(self.reserve_margin.data).T.rename(columns={0: "VALUE"})
             df[["REGION", "YEAR"]] = pd.DataFrame(df.index.str.split(".").to_list(), index=df.index)
             dfs["ReserveMargin"] = df
 
             dfs_tag_technology = []
@@ -443,24 +473,28 @@
 
         # do subsidiary objects
         dfs.update(Technology.to_dataframes(technologies=self.technologies))
         dfs.update(Impact.to_dataframes(impacts=self.impacts))
         dfs.update(Commodity.to_dataframes(commodities=self.commodities))
         dfs.update(Region.to_dataframes(regions=self.regions))
         dfs.update(self.time_definition.to_dataframes())
+        if self.storage is not None:
+            dfs.update(Storage.to_dataframes(storage=self.storage))
 
         return dfs
 
     def to_otoole_csv(self, output_directory):
         dfs = self.to_model_dataframes()
 
         # do subsidiary objects
         Technology.to_otoole_csv(technologies=self.technologies, output_directory=output_directory)
         Impact.to_otoole_csv(impacts=self.impacts, output_directory=output_directory)
         Commodity.to_otoole_csv(commodities=self.commodities, output_directory=output_directory)
         Region.to_otoole_csv(regions=self.regions, output_directory=output_directory)
         self.time_definition.to_otoole_csv(output_directory=output_directory)
+        if self.storage is not None:
+            Storage.to_otoole_csv(storage=self.storage, output_directory=output_directory)
 
         # write dataframes
         for stem, _params in self.otoole_stems.items():
             if stem not in self.otoole_cfg.empty_dfs:
                 dfs[stem].to_csv(os.path.join(output_directory, f"{stem}.csv"), index=False)
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/compat/region.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/region.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,14 +94,23 @@
         # Convert TradeRoute binary linking value to bool
         dfs["TradeRoute"]["VALUE"] = dfs["TradeRoute"]["VALUE"].map({1: True, 0: False})
 
         ##########################
         # Define class instances #
         ##########################
 
+        # Identify regions with trade route defined
+        if "TradeRoute" not in otoole_cfg.empty_dfs:
+            regions_with_trade = []
+            for region in src_regions["VALUE"].values:
+                if not dfs["TradeRoute"].loc[dfs["TradeRoute"]["REGION"] == region].empty:
+                    regions_with_trade.append(region)
+        else:
+            regions_with_trade = []
+
         region_instances = []
         for _index, region in src_regions.iterrows():
             region_instances.append(
                 cls(
                     id=region["VALUE"],
                     otoole_cfg=otoole_cfg,
                     trade_routes=(
@@ -111,15 +120,15 @@
                                     dfs["TradeRoute"]["REGION"] == region["VALUE"]
                                 ],
                                 root_column="REGION",
                                 data_columns=["LINKED_REGION", "FUEL", "YEAR"],
                                 target_column="VALUE",
                             )
                         )
-                        if "TradeRoute" not in otoole_cfg.empty_dfs
+                        if region["VALUE"] in regions_with_trade
                         else None
                     ),
                 )
             )
 
         return region_instances
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/compat/technology.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/technology.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/compat/time_definition.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/compat/time_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,25 +204,21 @@
             timeslice_in_season=timeslice_in_season,
         )
 
     def _to_dataframe(self, stem: str) -> pd.DataFrame:
         if stem == "YEAR":
             return pd.DataFrame(data={"VALUE": sorted(self.years)})
         elif stem == "SEASON":
-            return pd.DataFrame(data={"VALUE": sorted(self.seasons or [])}, columns=["VALUE"])
+            return pd.DataFrame(data={"VALUE": self.seasons or []}, columns=["VALUE"])
         elif stem == "TIMESLICE":
             return pd.DataFrame(data={"VALUE": sorted(self.timeslices)}, columns=["VALUE"])
         elif stem == "DAILYTIMEBRACKET":
-            return pd.DataFrame(
-                data={"VALUE": sorted(self.daily_time_brackets or [])}, columns=["VALUE"]
-            )
+            return pd.DataFrame(data={"VALUE": self.daily_time_brackets or []}, columns=["VALUE"])
         elif stem == "DAYTYPE":
-            return pd.DataFrame(data={"VALUE": sorted(self.day_types or [])}, columns=["VALUE"])
-        elif stem == "DAILYTIMEBRACKET":
-            return pd.DataFrame(data={"VALUE": sorted(self.day_split or [])}, columns=["VALUE"])
+            return pd.DataFrame(data={"VALUE": self.day_types or []}, columns=["VALUE"])
         elif stem == "DaysInDayType":
             return (
                 pd.DataFrame.from_records(
                     [
                         {
                             "SEASON": season,
                             "DAYTYPE": daytype,
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/time_definition.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/time_definition.py`

 * *Files 22% similar despite different names*

```diff
@@ -142,23 +142,55 @@
       - build assume equal year, daytype, and day splitting where not specified
       - option: if adjacency is specified:
         - use specified adjacency, validating keys
         - else:
           - if ordered yearparts, daytypes, and dayparts given, assume adjacency
           - else: raise error for required parameter
     """
+
+    # Convert list of int to list of str
+    for key in values.keys():
+        if isinstance(values[key], list):
+            values[key] = [str(item) if isinstance(item, int) else item for item in values[key]]
+
     years = values.get("years")
     seasons = values.get("seasons")
     day_types = values.get("day_types")
     time_brackets = values.get("daily_time_brackets")
 
     # build timeslices from parts
     timeslices = build_timeslices_from_parts(seasons, day_types, time_brackets)
     values["timeslices"] = timeslices
 
+    # build time_brackets/seasons/day_types and link to timeslice if necessary
+    if time_brackets:
+        values["timeslice_in_timebracket"] = {
+            timeslice: [time_bracket for time_bracket in time_brackets if time_bracket in timeslice]
+            for timeslice in timeslices
+        }
+    else:
+        values["daily_time_brackets"] = [1]
+        values["timeslice_in_timebracket"] = {timeslice: [1] for timeslice in timeslices}
+    if seasons:
+        values["timeslice_in_season"] = {
+            timeslice: [season for season in seasons if season in timeslice]
+            for timeslice in timeslices
+        }
+    else:
+        values["seasons"] = [1]
+        values["timeslice_in_season"] = {timeslice: [1] for timeslice in timeslices}
+    if day_types:
+        values["timeslice_in_daytype"] = {
+            timeslice: [day_type for day_type in day_types if day_type in timeslice]
+            for timeslice in timeslices
+        }
+    else:
+        values["day_types"] = [1]
+        values["timeslice_in_daytype"] = {timeslice: [1] for timeslice in timeslices}
+
     # validate keys on splits, if any, or maybe get parts
     year_split, days_in_day_type, day_split = validate_parts_from_splits(
         timeslices, day_types, time_brackets, values
     )
     values["year_split"] = year_split
     values["day_split"] = day_split
     values["days_in_day_type"] = days_in_day_type
@@ -208,122 +240,157 @@
     if max > 10:
         return f"{val:02}"
     if max >= 100:
         return f"{val:03}"
     return f"{val}"
 
 
-def construction_from_yrparts_dayparts_int(values: Any):
-    """pathway 2: years plus yearparts and dayparts as integers
-    - build timeslices from yearparts and dayparts
-    - build adjacency from ordered years and timeslices
+class TimeDefinition(OSeMOSYSBase, OtooleTimeDefinition):
     """
-    years = values.get("years")
-    yearparts = values.get("seasons")
-    dayparts = values.get("daily_time_brackets")
-    yearparts = [("s" + format_by_max_length(ii, yearparts)) for ii in range(1, yearparts + 1)]
-    dayparts = [("h" + format_by_max_length(ii, dayparts)) for ii in range(1, dayparts + 1)]
-
-    for key in [
-        "timeslices",
-        "timeslice_in_timebracket",
-        "timeslice_in_daytype",
-        "timeslice_in_season",
-        "day_types",
-        "day_split",
-        "days_in_day_type",
-        "year_split",
-    ]:
-        if values.get(key) is not None:
-            raise ValueError(
-                """If specifying time_definition with a
-                             number of yearparts and dayparts, no other
-                             time_definition parameters can be specified."""
-            )
-
-    timeslices = build_timeslices_from_parts(yearparts, dayparts)
-    values["timeslices"] = timeslices
+    # TimeDefinition
 
-    values["timeslice_in_timebracket"] = {
-        timeslice: [time_bracket for time_bracket in dayparts if time_bracket in timeslice]
-        for timeslice in timeslices
+    The TimeDefinition class contains all temporal data needed for an OSeMOSYS model. There are
+    multiple pathways to creating a TimeDefinition object, where any missing information is
+    inferred from the data provided.
+
+    Only a single instance of TimeDefinition is needed to run a model and, as a minimum, only
+    `years` need to be provided to create a TimeDefinition object.
+
+    The other parameters corresponding to the OSeMOSYS time related sets (`seasons`, `timeslices`,
+    `day_types`, `daily_time_brackets`) can be provided as lists or ranges.
+
+    One parameter additional to those correponsding to OSeMOSYS parameters is used , `adj`,
+    which specified the adjency matrices for `years`, `seasons`, `day_types`,
+    `daily_time_brackets`, `timeslices`. If not providing values for `adj`, it is assumed that
+    the other variables are provided in order from first to last. If providing the values directly,
+    these can be provided as a dict, an example of which for years and timeslices is below:
+
+    ```python
+    adj = {
+        "years": dict(zip(range(2020, 2050), range(2021, 2051))),
+        "timeslices": {"A": "B", "B": "C", "C": "D"},
     }
-    values["timeslice_in_season"] = {
-        timeslice: [season for season in yearparts if season in timeslice]
-        for timeslice in timeslices
-    }
-    values["year_split"] = {yearpart: 1.0 / len(yearparts) for yearpart in yearparts}
-    values["day_split"] = {daypart: 1.0 / len(dayparts) for daypart in dayparts}
-    values["day_types"] = [1]
-    values["day_split"] = {1: 1.0}
-    values["days_in_day_type"] = {1: 1.0}
-    values["timeslice_in_daytype"] = {timeslice: [1] for timeslice in timeslices}
+    ```
+
+    ### Pathway 1 - Construction from years only
+
+    If only `years` are provided, the remaining necessary temporal parameters (`seasons`,
+    `day_types`, `daily_time_brackets`) are assumed to be singular.
+
+    ### Pathway 2 - Construction from parts
+
+    If no timeslice data is provided, but any of the below is, it is used to construct timeslices:
+        - seasons
+        - daily_time_brackets
+        - day_types
+        - year_split
+        - day_split
+        - days_in_day_type
+
+    ### Pathway 3 - Construction from timeslices
+
+    If timeslices are provided via any of the below parameters, this is used to construct the
+    TimeDefinition object:
+        - timeslices
+        - timeslice_in_timebracket
+        - timeslice_in_daytype
+        - timeslice_in_season
+
+
+    ## Parameters
+
+    `id` `(str)`: Any value may be provided for the single TimeDefintion instance.
+    Required parameter.
+
+    `years` `(List[int] | range(int)) | int`: OSeMOSYS YEARS. Required parameter.
+
+    `seasons` `(List[int | str]) | int`: OSeMOSYS SEASONS.
+    Optional, constructed if not provided.
+
+    `timeslices` `(List[int | str]) | int`: OSeMOSYS TIMESLICES.
+    Optional, constructed if not provided.
 
-    adj = TimeAdjacency(
-        years=dict(zip(sorted(years)[:-1], sorted(years)[1:])),
-        timeslices=dict(zip(timeslices[:-1], timeslices[1:])),
+    `day_types` `(List[int | str]) | int`: OSeMOSYS DAYTYPES.
+    Optional, constructed if not provided.
+
+    `daily_time_brackets` `(List[int | str])`: OSeMOSYS DAILYTIMEBRACKETS.
+    Optional, constructed if not provided.
+
+    `year_split` `({timeslice:{year:float}})`: OSeMOSYS YearSplit.
+    Optional, constructed if not provided.
+
+    `day_split` `({daily_time_bracket:{year:float}})`: OSeMOSYS DaySplit.
+    Optional, constructed if not provided.
+
+    `days_in_day_type` `({season:{day_type:{year:int}}})`: OSeMOSYS DaysInDayType.
+    Optional, constructed if not provided.
+
+    `timeslice_in_timebracket` `({timeslice:daily_time_bracket})`: OSeMOSYS Conversionlh.
+    Optional, constructed if not provided.
+
+    `timeslice_in_daytype` `({timeslice:day_type})`: OSeMOSYS Conversionld.
+    Optional, constructed if not provided.
+
+    `timeslice_in_season` `({timeslice:season})`: OSeMOSYS Conversionls.
+    Optional, constructed if not provided.
+
+    `adj` `({str:dict})`: Parameter to manually define adjanecy for `years`, `seasons`,
+    `day_types`, `daily_time_brackets`, and `timeslices`. Optional, if not providing values for
+    `adj`, it is assumed that the other variables are provided in order from first to last.
+
+    ## Examples
+
+    Examples are given below of how a TimeDefinition object might be created using the different
+    pathways.
+
+    ### Pathway 1 - Construction from years only
+
+    ```python
+    from tz.osemosys.schemas.time_definition import TimeDefinition
+
+    basic_time_definition = dict(
+        id="pathway_1",
+        years=[2021, 2022, 2023],
     )
-    values["adj"] = adj
-    values["adj_inv"] = adj.inv()
 
-    return values
+    TimeDefinition(**basic_time_definition)
+    ```
 
+    ### Pathway 2 - Construction from parts
 
-class TimeDefinition(OSeMOSYSBase, OtooleTimeDefinition):
-    """
-    Class to contain all temporal defition of the OSeMOSYS model.
+    ```python
+    from tz.osemosys.schemas.time_definition import TimeDefinition
+
+    basic_time_definition = dict(
+        id="pathway_2",
+        years=range(2020, 2051),
+        seasons=["winter", "summer"],
+        daily_time_brackets=["morning", "day", "evening", "night"],
+    )
+
+    TimeDefinition(**basic_time_definition)
+    ```
 
-    There are several pathways to constructing a TimeDefinition.
+    ### Pathway 3 - Construction from timeslices
 
-    pathway 1:
-    years only
+    ```python
+    from tz.osemosys.schemas.time_definition import TimeDefinition
 
-    pathway 2:
-    years plus yearparts and dayparts as integers
-
-    pathway 3:
-    years plus any of yearparts, daytypes, and dayparts, daysplit, yearsplit, days_in_daytype
-    with optional adjacency
-
-    pathway 4:
-    years plus any of timeslices, timeslice_in_timebracket, timeslice_in_daytype,
-    timeslice_in_season with optional year_split, day_split, days_in_day_type
-    and optional validation on yearparts, daytypes, and dayparts OR adjacency
-
-
-    Attributes:
-        years:
-            List[int]: a list of integer years for the capacity expansion study.
-                       Can also be a `range`.
-        seasons:
-            List[int | str]:
-        timeslices:
-            List[int | str]:
-        day_types:
-            List[int | str]:
-        daily_time_brackets:
-            List[int | str]:
-        year_split:
-            Mapping:
-        day_split:
-            Mapping:
-        days_in_day_type:
-            Mapping:
-        timeslice_in_timebracket:
-            Mapping:
-        timeslice_in_daytype:
-            Mapping:
-        timeslice_in_season:
-            Mapping:
-        adj:
-            TimeAdjacency:
-        adj_inv:
-            TimeAdjacency:
-        otoole_cfg:
-            OtooleCfg | None:
+    basic_time_definition = dict(
+        id="pathway_3",
+        years=range(2020, 2051),
+        timeslices=["A", "B", "C", "D"],
+        adj={
+            "years": dict(zip(range(2020, 2050), range(2021, 2051))),
+            "timeslices": dict(zip(["A", "B", "C"], ["B", "C", "D"])),
+        },
+    )
+
+    TimeDefinition(**basic_time_definition)
+    ```
 
     """
 
     # TODO: fix yearparts and dayparts then make extra params forbidden again
     # model_config = ConfigDict(extra="forbid")
 
     # always required
@@ -355,42 +422,45 @@
 
     @model_validator(mode="before")
     @classmethod
     def construction_validation(cls, values: Any, info: ValidationInfo) -> Any:
         # years is always required
         if values.get("years") is None:
             raise ValueError("'years' is a required parameter")
-        if isinstance(values.get("seasons"), int) and isinstance(
-            values.get("daily_time_brackets"), int
-        ):
-            values = construction_from_yrparts_dayparts_int(values)
-        elif any(
+
+        # # Pathway x
+        # if isinstance(values.get("seasons"), int) and isinstance(
+        #     values.get("daily_time_brackets"), int
+        # ):
+        #     values = construction_from_yrparts_dayparts_int(values)
+
+        # Pathway 3
+        if any(
             [
                 values.get("timeslices") is not None,
                 values.get("timeslice_in_timebracket") is not None,
                 values.get("timeslice_in_daytype") is not None,
                 values.get("timeslice_in_season") is not None,
             ]
         ):
-            # Validation if timeslice is provided
             values = construction_from_timeslices(values)
+        # Pathway 2
         elif any(
             [
-                values.get("yearparts") is not None,
+                values.get("seasons") is not None,
                 values.get("daily_time_brackets") is not None,
-                values.get("daytypes") is not None,
+                values.get("day_types") is not None,
                 values.get("year_split") is not None,
                 values.get("day_split") is not None,
                 values.get("days_in_day_type") is not None,
             ]
         ):
-            # Validation if parts or splits are provided
             values = construction_from_parts(values)
+        # Pathway 1
         else:
-            # just years provided
             values = construction_from_years_only(values)
 
         # maybe flip adj
         if values.get("adj_inv") is None:
             if isinstance(values.get("adj"), TimeAdjacency):
                 values["adj_inv"] = values["adj"].inv()
             elif isinstance(values.get("adj"), dict):
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/validation/impact_validation.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/impact_validation.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/validation/model_composition.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/model_composition.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 def check_tech_producing_commodity(values):
     """
     For each commodity, check there is a technology which produces it
     """
     for commodity in values.commodities:
         technology_missing = True
         for technology in values.technologies:
-            if technology_missing and technology.output_activity_ratio is not None:
-                for region in technology.output_activity_ratio.data.keys():
-                    if commodity.id in technology.output_activity_ratio.data[region].keys():
-                        technology_missing = False
+            for tech_mode in technology.operating_modes:
+                if technology_missing and tech_mode.output_activity_ratio is not None:
+                    for region in tech_mode.output_activity_ratio.data.keys():
+                        if commodity.id in tech_mode.output_activity_ratio.data[region].keys():
+                            technology_missing = False
         if technology_missing:
             raise ValueError(f"Commodity '{commodity.id}' is not an output of any technology")
 
     return values
 
 
 def check_tech_producing_impact(values):
     """
     For each impact, check there is a technology which produces it
     """
     for impact in values.impacts:
         technology_missing = True
         for technology in values.technologies:
-            if technology_missing and technology.emission_activity_ratio is not None:
-                for region in technology.emission_activity_ratio.data.keys():
-                    if impact.id in technology.emission_activity_ratio.data[region].keys():
-                        technology_missing = False
+            for tech_mode in technology.operating_modes:
+                if technology_missing and tech_mode.emission_activity_ratio is not None:
+                    for region in tech_mode.emission_activity_ratio.data.keys():
+                        if impact.id in tech_mode.emission_activity_ratio.data[region].keys():
+                            technology_missing = False
         if technology_missing:
             raise ValueError(f"Impact '{impact.id}' is not an output of any technology")
 
     return values
 
 
 def check_tech_consuming_commodity(values):
     """
     For each commodity which isn't a final demand, check it is the input of a technology
     """
     for commodity in values.commodities:
-        if commodity.demand_annual is None and commodity.accumulated_demand is None:
+        if commodity.demand_annual is None:
             technology_missing = True
             for technology in values.technologies:
-                if technology_missing and technology.input_activity_ratio is not None:
-                    for region in technology.input_activity_ratio.data.keys():
-                        if commodity.id in technology.input_activity_ratio.data[region].keys():
-                            technology_missing = False
+                for tech_mode in technology.operating_modes:
+                    if technology_missing and tech_mode.input_activity_ratio is not None:
+                        for region in tech_mode.input_activity_ratio.data.keys():
+                            if commodity.id in tech_mode.input_activity_ratio.data[region].keys():
+                                technology_missing = False
             if technology_missing:
                 raise ValueError(
                     f"Commodity '{commodity.id}' is neither a final demand nor "
                     f"an input of any technology"
                 )
 
     return values
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/validation/model_presolve.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/model_presolve.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/validation/region_validation.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/region_validation.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/validation/technology_validation.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/technology_validation.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/validation/timedefinition_validation.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/timedefinition_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,22 +254,45 @@
 
     else:
         ordered_timeslices = timeslices
 
     return dict(
         years=dict(zip(sorted(years)[:-1], sorted(years)[1:])),
         timeslices=dict(zip(sorted(ordered_timeslices)[:-1], sorted(ordered_timeslices)[1:])),
-        seasons=dict(zip(sorted(seasons)[:-1], sorted(seasons)[1:])) if seasons else None,
-        day_types=dict(zip(sorted(day_types)[:-1], sorted(day_types)[1:])) if day_types else None,
-        time_brackets=dict(zip(sorted(time_brackets)[:-1], sorted(time_brackets)[1:]))
-        if time_brackets
-        else None,
+        seasons=dict(zip(map(str, seasons[:-1]), map(str, seasons[1:]))) if seasons else None,
+        day_types=(
+            dict(zip(map(str, day_types[:-1]), map(str, day_types[1:]))) if day_types else None
+        ),
+        time_brackets=(
+            dict(zip(map(str, time_brackets[:-1]), map(str, time_brackets[1:])))
+            if time_brackets
+            else None
+        ),
     )
 
 
+def time_adj_to_list(adj_dict: dict):
+    """
+    Convert a time adjacency dict to a chronologically ordered list
+    """
+    chronological_list = []
+    # Add first item
+    chronological_list.append(
+        [item for item in adj_dict.keys() if item not in adj_dict.values()][0]
+    )
+    # iteratively add remaining items
+    add_to_list = True
+    while add_to_list:
+        chronological_list.append(adj_dict[chronological_list[-1]])
+        if chronological_list[-1] not in adj_dict.keys():
+            add_to_list = False
+
+    return chronological_list
+
+
 # ##########################################
 # Validation if timeslices are not defined #
 # ##########################################
 
 
 def build_timeslices_from_parts(seasons, day_types=None, time_brackets=None):
     """
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/schemas/validation/validation_utils.py` & `tz_osemosys-0.0.3/tz/osemosys/schemas/validation/validation_utils.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/utils/__init__.py` & `tz_osemosys-0.0.3/tz/osemosys/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz/osemosys/utils/cfg_parser.py` & `tz_osemosys-0.0.3/tz/osemosys/utils/cfg_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -106,12 +106,16 @@
 
     return [_inner(key, rgetattr(cfg, key.split("."))) for key in keys]
 
 
 def walk_dict(d, f, *args):
     list_of_keys = recursive_keys([], d)
 
+    changes_flag = False
+
     for sublist in list_of_keys:
-        val = rgetattr(d, sublist)
-        rsetattr(d, sublist, f(val, *args))
+        old_val = rgetattr(d, sublist)
+        new_val = f(old_val, *args)
+        rsetattr(d, sublist, new_val)
+        changes_flag = changes_flag or (old_val != new_val)
 
-    return d
+    return changes_flag
```

### Comparing `tz-osemosys-0.0.1/tz/osemosys/utils/utils.py` & `tz_osemosys-0.0.3/tz/osemosys/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tz-osemosys-0.0.1/tz_osemosys.egg-info/PKG-INFO` & `tz_osemosys-0.0.3/tz_osemosys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tz-osemosys
-Version: 0.0.1
+Version: 0.0.3
 Summary: An OSeMOSYS implementation for the Future Energy Outlook by TransitionZero
 Author-email: Lucas Kruitwagen <lucas.kruitwagen@gmail.com>, Ed Gill <edwardxtg@gmail.com>, Abhishek Shivakumar <abhishek0208@gmail.com>
 Project-URL: Homepage, https://github.com/transitionzero/tz-osemosys
 Project-URL: Bug Reports, https://github.com/transitionzero/tz-osemosys/issues
 Project-URL: Funding, https://transitionzero.org
 Project-URL: Source, https://github.com/transitionzero/tz-osemosys
 Keywords: energy,milp,climate
@@ -18,25 +18,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic>2
 Requires-Dist: pydantic-settings
 Requires-Dist: xarray
 Requires-Dist: orjson
 Requires-Dist: linopy
-Requires-Dist: highspy
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-order; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
+Requires-Dist: highspy; extra == "dev"
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://github.com/transition-zero/.github/raw/main/profile/img/logo-dark.png">
   <img alt="TransitionZero Logo" width="1000px" src="https://github.com/transition-zero/.github/raw/main/profile/img/logo-light.png">
   <a href="https://www.transitionzero.org/">
 </picture>
 
@@ -104,15 +104,15 @@
 
 HiGHS can be installed from source using `cmake` following the instructions [here](https://github.com/ERGO-Code/HiGHS?tab=readme-ov-file#installation). You'll need to install a cmake distribution for your relevant operating system.
 
 *common issue: make sure you have write-privileges to default directory for `cmake --install build`, or either run this command with administrator privileges (`sudo cmake --install build` on mac and linux) or specify a different build directory*
 
 ### Docker installation
 
-A docker container is provided that contains Python 3.11 and an installed version of HiGHS. You'll nedd to [install a docker distribution](https://docs.docker.com/engine/install/) relevant for your operating system.
+A docker container is provided that contains Python 3.11 and an installed version of HiGHS. You'll need to [install a docker distribution](https://docs.docker.com/engine/install/) relevant for your operating system.
 
 The docker container is used in testing, but can also be used for local development work. The following docker command will run and enter the docker container, mount the current working directory at the `/home` directory, and change directory within the container to this directory.
 
 ```console
 docker run -v $(pwd):/home -it  ghcr.io/transition-zero/tz-highs/highs-python:latest /bin/bash -c 'cd /home && /bin/bash'
 ```
 
@@ -136,15 +136,15 @@
     Impact,
     OperatingMode,
 )
 
 time_definition = TimeDefinition(id="years-only", years=range(2020, 2051))
 regions = [Region(id="single-region")]
 commodities = [Commodity(id="electricity", demand_annual=25 * 8760)]  # 25GW * 8760hr/yr
-impacts = [Impact(id="CO2", penalty=60)]  # 10 $mn/Mtonne
+impacts = [Impact(id="CO2", penalty=60)]  # 60 $mn/Mtonne
 technologies = [
     Technology(
         id="coal-gen",
         operating_life=40,  # years
         capex=800,  # mn$/GW
         # straight-line reduction to 2040
         residual_capacity={
@@ -199,17 +199,17 @@
 - model fields can also be populated from environment variables: `my_field: $ENV{MYVAR}`.
 - simple Python expressions are automatically evaluated, including list comprehensions, dictionary comprehensions, `min`, `max`, `sum`, and `range` functions.
 - for data keyed by an osemosys `set` (e.g. `YEARS`, `TIMESLICES`, `TECHNOLOGIES`), wildcards `"*"` can be used in place of explicitly listing all set members.
 - data field `set` dimensions and membership are also automatically inferred - a single value can be given which will be broadcast to all set member combinations.
 - single or multiple `.yaml` files can be composed together, allowing you to separate, e.g. `technologies.yaml`, from the rest of your model.
 
 ```python
-from tz.osemosys import load_model
+from tz.osemosys import Model
 
-my_model = load_model("path/to/yaml/directory")
+my_model = Model.from_yaml("path/to/yaml/directory")
 ```
 
 ### From Otoole outputs (legacy)
 
 TZ-OSeMOSYS is provided with backwards compatability with the [otoole](https://github.com/OSeMOSYS/otoole) osemosys tooling. Any legacy models can be loaded from the directory of otoole-formatted csvs.
 
 ```python
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: tz-osemosys Version: 0.0.1 Summary: An OSeMOSYS
+Metadata-Version: 2.1 Name: tz-osemosys Version: 0.0.3 Summary: An OSeMOSYS
 implementation for the Future Energy Outlook by TransitionZero Author-email:
 Lucas Kruitwagen
 gmail.com>, Ed Gill
 gmail.com>, Abhishek Shivakumar
 gmail.com> Project-URL: Homepage, https://github.com/transitionzero/tz-osemosys
 Project-URL: Bug Reports, https://github.com/transitionzero/tz-osemosys/issues
 Project-URL: Funding, https://transitionzero.org Project-URL: Source, https://
 github.com/transitionzero/tz-osemosys Keywords: energy,milp,climate Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Scientific/Engineering Classifier: License :: OSI
 Approved :: GNU Affero General Public License v3 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
 Only Requires-Python: >=3.11 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: pydantic>2 Requires-Dist: pydantic-settings
-Requires-Dist: xarray Requires-Dist: orjson Requires-Dist: linopy Requires-
-Dist: highspy Provides-Extra: dev Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: black; extra == "dev" Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-order; extra == "dev" Requires-Dist: pytest-cov; extra ==
-"dev" Requires-Dist: pytest-asyncio; extra == "dev" Requires-Dist: mypy; extra
-== "dev" Requires-Dist: tox; extra == "dev" Requires-Dist: coverage; extra ==
-"dev" [TransitionZero Logo]_#_ _T_Z_-_O_S_E_M_O_S_Y_S_ _-_ _a_ _m_o_d_e_r_n_ _l_o_n_g_-_r_u_n_ _s_y_s_t_e_m_s_ _m_o_d_e_l_l_i_n_g
-_f_r_a_m_e_w_o_r_k_ _[_!_[_L_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_ _b_a_d_g_e_]_]_[_l_i_c_e_n_s_e_]_ _[_!_[_C_o_n_t_r_i_b_u_t_o_r_ _C_o_v_e_n_a_n_t_]
-_[_c_o_n_t_r_i_b_u_t_o_r_ _c_o_v_e_n_a_n_t_ _b_a_d_g_e_]_]_[_c_o_d_e_ _o_f_ _c_o_n_d_u_c_t_]_ _!_[_T_e_s_t_s_]_[_t_e_s_t_s_ _b_a_d_g_e_]_ _!
-_[_C_o_v_e_r_a_g_e_]_[_c_o_v_e_r_a_g_e_ _b_a_d_g_e_]_ _!_[_P_y_t_h_o_n_]_[_p_y_t_h_o_n_ _b_a_d_g_e_]_ _!_[_S_t_a_t_u_s_]_[_s_t_a_t_u_s_ _b_a_d_g_e_]_ 
-_[_l_i_c_e_n_s_e_ _b_a_d_g_e_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_a_d_-_a_u_r_e_s_/
+Requires-Dist: xarray Requires-Dist: orjson Requires-Dist: linopy Provides-
+Extra: dev Requires-Dist: pre-commit; extra == "dev" Requires-Dist: black;
+extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-
+order; extra == "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist:
+pytest-asyncio; extra == "dev" Requires-Dist: mypy; extra == "dev" Requires-
+Dist: tox; extra == "dev" Requires-Dist: coverage; extra == "dev" Requires-
+Dist: highspy; extra == "dev" [TransitionZero Logo]_#_ _T_Z_-_O_S_E_M_O_S_Y_S_ _-_ _a_ _m_o_d_e_r_n
+_l_o_n_g_-_r_u_n_ _s_y_s_t_e_m_s_ _m_o_d_e_l_l_i_n_g_ _f_r_a_m_e_w_o_r_k_ _[_!_[_L_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_ _b_a_d_g_e_]_]_[_l_i_c_e_n_s_e_]_ _[_!
+_[_C_o_n_t_r_i_b_u_t_o_r_ _C_o_v_e_n_a_n_t_]_[_c_o_n_t_r_i_b_u_t_o_r_ _c_o_v_e_n_a_n_t_ _b_a_d_g_e_]_]_[_c_o_d_e_ _o_f_ _c_o_n_d_u_c_t_]_ _!_[_T_e_s_t_s_]
+_[_t_e_s_t_s_ _b_a_d_g_e_]_ _!_[_C_o_v_e_r_a_g_e_]_[_c_o_v_e_r_a_g_e_ _b_a_d_g_e_]_ _!_[_P_y_t_h_o_n_]_[_p_y_t_h_o_n_ _b_a_d_g_e_]_ _!_[_S_t_a_t_u_s_]
+_[_s_t_a_t_u_s_ _b_a_d_g_e_]_ _[_l_i_c_e_n_s_e_ _b_a_d_g_e_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_a_d_-_a_u_r_e_s_/
 _c_a_s_t_o_p_o_d_?_c_o_l_o_r_=_b_l_u_e_ _[_l_i_c_e_n_s_e_]_:_ _h_t_t_p_s_:_/_/_o_p_e_n_s_o_u_r_c_e_._o_r_g_/_l_i_c_e_n_s_e_/_a_g_p_l_-_v_3_ 
 _[_c_o_n_t_r_i_b_u_t_o_r_ _c_o_v_e_n_a_n_t_ _b_a_d_g_e_]_:_ _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
 _C_o_n_t_r_i_b_u_t_o_r_%_2_0_C_o_v_e_n_a_n_t_-_2_._1_-_4_b_a_a_a_a_._s_v_g_ _[_c_o_d_e_ _o_f_ _c_o_n_d_u_c_t_]_:_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
 _t_r_a_n_s_i_t_i_o_n_-_z_e_r_o_/_t_z_-_o_s_e_m_o_s_y_s_/_b_l_o_b_/_m_a_i_n_/_C_O_D_E_-_O_F_-_C_O_N_D_U_C_T_._m_d_ _[_t_e_s_t_s_ _b_a_d_g_e_]_:_ _h_t_t_p_s_:_/
 _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_e_n_d_p_o_i_n_t_?_u_r_l_=_h_t_t_p_s_:_/_/_g_i_s_t_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_L_k_r_u_i_t_w_a_g_e_n_/
 _f_e_f_f_b_3_8_d_4_6_c_7_5_0_c_a_d_5_4_0_2_d_c_a_5_d_d_5_4_b_f_9_/_r_a_w_/_t_e_s_t_s___p_a_s_s_i_n_g_._j_s_o_n_ _[_c_o_v_e_r_a_g_e_ _b_a_d_g_e_]_:
 _h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_e_n_d_p_o_i_n_t_?_u_r_l_=_h_t_t_p_s_:_/_/_g_i_s_t_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/
@@ -66,15 +66,15 @@
 _(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_E_R_G_O_-_C_o_d_e_/_H_i_G_H_S_?_t_a_b_=_r_e_a_d_m_e_-_o_v_-_f_i_l_e_#_i_n_s_t_a_l_l_a_t_i_o_n_)_._ _Y_o_u_'_l_l
 _n_e_e_d_ _t_o_ _i_n_s_t_a_l_l_ _a_ _c_m_a_k_e_ _d_i_s_t_r_i_b_u_t_i_o_n_ _f_o_r_ _y_o_u_r_ _r_e_l_e_v_a_n_t_ _o_p_e_r_a_t_i_n_g_ _s_y_s_t_e_m_.
 _*_c_o_m_m_o_n_ _i_s_s_u_e_:_ _m_a_k_e_ _s_u_r_e_ _y_o_u_ _h_a_v_e_ _w_r_i_t_e_-_p_r_i_v_i_l_e_g_e_s_ _t_o_ _d_e_f_a_u_l_t_ _d_i_r_e_c_t_o_r_y_ _f_o_r
 _`_c_m_a_k_e_ _-_-_i_n_s_t_a_l_l_ _b_u_i_l_d_`_,_ _o_r_ _e_i_t_h_e_r_ _r_u_n_ _t_h_i_s_ _c_o_m_m_a_n_d_ _w_i_t_h_ _a_d_m_i_n_i_s_t_r_a_t_o_r
 _p_r_i_v_i_l_e_g_e_s_ _(_`_s_u_d_o_ _c_m_a_k_e_ _-_-_i_n_s_t_a_l_l_ _b_u_i_l_d_`_ _o_n_ _m_a_c_ _a_n_d_ _l_i_n_u_x_)_ _o_r_ _s_p_e_c_i_f_y_ _a
 _d_i_f_f_e_r_e_n_t_ _b_u_i_l_d_ _d_i_r_e_c_t_o_r_y_*_ _#_#_#_ _D_o_c_k_e_r_ _i_n_s_t_a_l_l_a_t_i_o_n_ _A_ _d_o_c_k_e_r_ _c_o_n_t_a_i_n_e_r_ _i_s
 _p_r_o_v_i_d_e_d_ _t_h_a_t_ _c_o_n_t_a_i_n_s_ _P_y_t_h_o_n_ _3_._1_1_ _a_n_d_ _a_n_ _i_n_s_t_a_l_l_e_d_ _v_e_r_s_i_o_n_ _o_f_ _H_i_G_H_S_._ _Y_o_u_'_l_l
-_n_e_d_d_ _t_o_ _[_i_n_s_t_a_l_l_ _a_ _d_o_c_k_e_r_ _d_i_s_t_r_i_b_u_t_i_o_n_]_(_h_t_t_p_s_:_/_/_d_o_c_s_._d_o_c_k_e_r_._c_o_m_/_e_n_g_i_n_e_/_i_n_s_t_a_l_l_/
+_n_e_e_d_ _t_o_ _[_i_n_s_t_a_l_l_ _a_ _d_o_c_k_e_r_ _d_i_s_t_r_i_b_u_t_i_o_n_]_(_h_t_t_p_s_:_/_/_d_o_c_s_._d_o_c_k_e_r_._c_o_m_/_e_n_g_i_n_e_/_i_n_s_t_a_l_l_/
 _)_ _r_e_l_e_v_a_n_t_ _f_o_r_ _y_o_u_r_ _o_p_e_r_a_t_i_n_g_ _s_y_s_t_e_m_._ _T_h_e_ _d_o_c_k_e_r_ _c_o_n_t_a_i_n_e_r_ _i_s_ _u_s_e_d_ _i_n_ _t_e_s_t_i_n_g_,
 _b_u_t_ _c_a_n_ _a_l_s_o_ _b_e_ _u_s_e_d_ _f_o_r_ _l_o_c_a_l_ _d_e_v_e_l_o_p_m_e_n_t_ _w_o_r_k_._ _T_h_e_ _f_o_l_l_o_w_i_n_g_ _d_o_c_k_e_r_ _c_o_m_m_a_n_d
 _w_i_l_l_ _r_u_n_ _a_n_d_ _e_n_t_e_r_ _t_h_e_ _d_o_c_k_e_r_ _c_o_n_t_a_i_n_e_r_,_ _m_o_u_n_t_ _t_h_e_ _c_u_r_r_e_n_t_ _w_o_r_k_i_n_g_ _d_i_r_e_c_t_o_r_y_ _a_t
 _t_h_e_ _`_/_h_o_m_e_`_ _d_i_r_e_c_t_o_r_y_,_ _a_n_d_ _c_h_a_n_g_e_ _d_i_r_e_c_t_o_r_y_ _w_i_t_h_i_n_ _t_h_e_ _c_o_n_t_a_i_n_e_r_ _t_o_ _t_h_i_s
 _d_i_r_e_c_t_o_r_y_._ _`_`_`_c_o_n_s_o_l_e_ _d_o_c_k_e_r_ _r_u_n_ _-_v_ _$_(_p_w_d_)_:_/_h_o_m_e_ _-_i_t_ _g_h_c_r_._i_o_/_t_r_a_n_s_i_t_i_o_n_-_z_e_r_o_/
 _t_z_-_h_i_g_h_s_/_h_i_g_h_s_-_p_y_t_h_o_n_:_l_a_t_e_s_t_ _/_b_i_n_/_b_a_s_h_ _-_c_ _'_c_d_ _/_h_o_m_e_ _&_&_ _/_b_i_n_/_b_a_s_h_'_ _`_`_`_ _*_n_o_t_e_!
 _A_n_y_ _f_i_l_e_s_ _c_h_a_n_g_e_d_ _w_i_t_h_i_n_ _t_h_i_s_ _m_o_u_n_t_e_d_ _d_i_r_e_c_t_o_r_y_ _w_i_l_l_ _p_e_r_s_i_s_t_,_ _b_u_t_ _a_n_y_ _c_h_a_n_g_e_s
@@ -86,15 +86,15 @@
 _b_e_t_w_e_e_n_ _t_h_e_ _o_b_j_e_c_t_ _t_y_p_e_s_._ _T_h_e_ _s_e_t_ _o_f_ _o_b_j_e_c_t_s_ _c_o_m_p_r_i_s_i_n_g_ _t_h_e_ _m_o_d_e_l_ _i_s_ _m_u_t_u_a_l_l_y
 _e_x_c_l_u_s_i_v_e_ _-_ _n_o_ _i_n_f_o_r_m_a_t_i_o_n_ _i_s_ _r_e_p_e_a_t_e_d_ _-_ _a_n_d_ _c_o_l_l_e_c_t_i_v_e_l_y_ _e_x_h_a_u_s_t_i_v_e_ _-_ _n_o
 _i_n_f_o_r_m_a_t_i_o_n_ _n_e_e_d_s_ _t_o_ _b_e_ _e_x_t_r_a_c_t_e_d_ _f_r_o_m_ _c_s_v_s_ _o_r_ _o_t_h_e_r_ _d_a_t_a_ _s_o_u_r_c_e_s_._ _`_`_`_p_y_t_h_o_n
 _f_r_o_m_ _t_z_._o_s_e_m_o_s_y_s_ _i_m_p_o_r_t_ _(_ _M_o_d_e_l_,_ _T_e_c_h_n_o_l_o_g_y_,_ _T_i_m_e_D_e_f_i_n_i_t_i_o_n_,_ _C_o_m_m_o_d_i_t_y_,_ _R_e_g_i_o_n_,
 _I_m_p_a_c_t_,_ _O_p_e_r_a_t_i_n_g_M_o_d_e_,_ _)_ _t_i_m_e___d_e_f_i_n_i_t_i_o_n_ _=_ _T_i_m_e_D_e_f_i_n_i_t_i_o_n_(_i_d_=_"_y_e_a_r_s_-_o_n_l_y_"_,
 _y_e_a_r_s_=_r_a_n_g_e_(_2_0_2_0_,_ _2_0_5_1_)_)_ _r_e_g_i_o_n_s_ _=_ _[_R_e_g_i_o_n_(_i_d_=_"_s_i_n_g_l_e_-_r_e_g_i_o_n_"_)_]_ _c_o_m_m_o_d_i_t_i_e_s_ _=_ 
 _[_C_o_m_m_o_d_i_t_y_(_i_d_=_"_e_l_e_c_t_r_i_c_i_t_y_"_,_ _d_e_m_a_n_d___a_n_n_u_a_l_=_2_5_ _*_ _8_7_6_0_)_]_ _#_ _2_5_G_W_ _*_ _8_7_6_0_h_r_/_y_r
-_i_m_p_a_c_t_s_ _=_ _[_I_m_p_a_c_t_(_i_d_=_"_C_O_2_"_,_ _p_e_n_a_l_t_y_=_6_0_)_]_ _#_ _1_0_ _$_m_n_/_M_t_o_n_n_e_ _t_e_c_h_n_o_l_o_g_i_e_s_ _=_ 
+_i_m_p_a_c_t_s_ _=_ _[_I_m_p_a_c_t_(_i_d_=_"_C_O_2_"_,_ _p_e_n_a_l_t_y_=_6_0_)_]_ _#_ _6_0_ _$_m_n_/_M_t_o_n_n_e_ _t_e_c_h_n_o_l_o_g_i_e_s_ _=_ 
 _[_ _T_e_c_h_n_o_l_o_g_y_(_ _i_d_=_"_c_o_a_l_-_g_e_n_"_,_ _o_p_e_r_a_t_i_n_g___l_i_f_e_=_4_0_,_ _#_ _y_e_a_r_s_ _c_a_p_e_x_=_8_0_0_,_ _#_ _m_n_$_/_G_W_ _#
 _s_t_r_a_i_g_h_t_-_l_i_n_e_ _r_e_d_u_c_t_i_o_n_ _t_o_ _2_0_4_0_ _r_e_s_i_d_u_a_l___c_a_p_a_c_i_t_y_=_{_ _y_r_:_ _2_5_ _*_ _m_a_x_(_(_1_ _-_ _(_y_r_ _-
 _2_0_2_0_)_ _/_ _(_2_0_4_0_ _-_ _2_0_2_0_)_,_ _0_)_)_ _f_o_r_ _y_r_ _i_n_ _r_a_n_g_e_(_2_0_2_0_,_ _2_0_5_1_)_ _}_,_ _o_p_e_r_a_t_i_n_g___m_o_d_e_s_=
 _[_ _O_p_e_r_a_t_i_n_g_M_o_d_e_(_ _i_d_=_"_g_e_n_e_r_a_t_i_o_n_"_,_ _#_ _$_m_n_2_0_/_M_t_._c_o_a_l_ _/_ _8_._1_4_ _T_W_h_/_M_t_ _c_o_a_l_ _*_ _8_7_6_0
 _G_W_h_/_G_W_ _/_ _0_._3_ _/_1_0_0_0_ _G_W_h_/_T_W_h_ _(_t_h_e_r_m_ _e_f_f_)_ _o_p_e_x___v_a_r_i_a_b_l_e_=_2_0_ _/_ _8_._1_4_ _*_ _8_7_6_0_ _/_ _0_._3_ _/
 _1_0_0_0_,_ _#_ _$_7_1_/_G_W_/_y_r_ _o_u_t_p_u_t___a_c_t_i_v_i_t_y___r_a_t_i_o_=_{_"_e_l_e_c_t_r_i_c_i_t_y_"_:_ _1_._0_ _*_ _8_7_6_0_}_,_ _#_ _G_W_h_/_y_r_/
 _G_W_ _e_m_i_s_s_i_o_n___a_c_t_i_v_i_t_y___r_a_t_i_o_=_{_ _"_C_O_2_"_:_ _0_._3_5_4_ _*_ _8_7_6_0_ _/_ _1_0_0_0_ _}_,_ _#_ _M_t_c_o_2_/_T_W_h_ _*
@@ -114,15 +114,15 @@
 _c_o_m_p_r_e_h_e_n_s_i_o_n_s_,_ _`_m_i_n_`_,_ _`_m_a_x_`_,_ _`_s_u_m_`_,_ _a_n_d_ _`_r_a_n_g_e_`_ _f_u_n_c_t_i_o_n_s_._ _-_ _f_o_r_ _d_a_t_a_ _k_e_y_e_d_ _b_y
 _a_n_ _o_s_e_m_o_s_y_s_ _`_s_e_t_`_ _(_e_._g_._ _`_Y_E_A_R_S_`_,_ _`_T_I_M_E_S_L_I_C_E_S_`_,_ _`_T_E_C_H_N_O_L_O_G_I_E_S_`_)_,_ _w_i_l_d_c_a_r_d_s_ _`_"_*_"_`
 _c_a_n_ _b_e_ _u_s_e_d_ _i_n_ _p_l_a_c_e_ _o_f_ _e_x_p_l_i_c_i_t_l_y_ _l_i_s_t_i_n_g_ _a_l_l_ _s_e_t_ _m_e_m_b_e_r_s_._ _-_ _d_a_t_a_ _f_i_e_l_d_ _`_s_e_t_`
 _d_i_m_e_n_s_i_o_n_s_ _a_n_d_ _m_e_m_b_e_r_s_h_i_p_ _a_r_e_ _a_l_s_o_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _i_n_f_e_r_r_e_d_ _-_ _a_ _s_i_n_g_l_e_ _v_a_l_u_e_ _c_a_n
 _b_e_ _g_i_v_e_n_ _w_h_i_c_h_ _w_i_l_l_ _b_e_ _b_r_o_a_d_c_a_s_t_ _t_o_ _a_l_l_ _s_e_t_ _m_e_m_b_e_r_ _c_o_m_b_i_n_a_t_i_o_n_s_._ _-_ _s_i_n_g_l_e_ _o_r
 _m_u_l_t_i_p_l_e_ _`_._y_a_m_l_`_ _f_i_l_e_s_ _c_a_n_ _b_e_ _c_o_m_p_o_s_e_d_ _t_o_g_e_t_h_e_r_,_ _a_l_l_o_w_i_n_g_ _y_o_u_ _t_o_ _s_e_p_a_r_a_t_e_,_ _e_._g_.
 _`_t_e_c_h_n_o_l_o_g_i_e_s_._y_a_m_l_`_,_ _f_r_o_m_ _t_h_e_ _r_e_s_t_ _o_f_ _y_o_u_r_ _m_o_d_e_l_._ _`_`_`_p_y_t_h_o_n_ _f_r_o_m_ _t_z_._o_s_e_m_o_s_y_s
-_i_m_p_o_r_t_ _l_o_a_d___m_o_d_e_l_ _m_y___m_o_d_e_l_ _=_ _l_o_a_d___m_o_d_e_l_(_"_p_a_t_h_/_t_o_/_y_a_m_l_/_d_i_r_e_c_t_o_r_y_"_)_ _`_`_`_ _#_#_#_ _F_r_o_m
+_i_m_p_o_r_t_ _M_o_d_e_l_ _m_y___m_o_d_e_l_ _=_ _M_o_d_e_l_._f_r_o_m___y_a_m_l_(_"_p_a_t_h_/_t_o_/_y_a_m_l_/_d_i_r_e_c_t_o_r_y_"_)_ _`_`_`_ _#_#_#_ _F_r_o_m
 _O_t_o_o_l_e_ _o_u_t_p_u_t_s_ _(_l_e_g_a_c_y_)_ _T_Z_-_O_S_e_M_O_S_Y_S_ _i_s_ _p_r_o_v_i_d_e_d_ _w_i_t_h_ _b_a_c_k_w_a_r_d_s_ _c_o_m_p_a_t_a_b_i_l_i_t_y
 _w_i_t_h_ _t_h_e_ _[_o_t_o_o_l_e_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_O_S_e_M_O_S_Y_S_/_o_t_o_o_l_e_)_ _o_s_e_m_o_s_y_s_ _t_o_o_l_i_n_g_._ _A_n_y
 _l_e_g_a_c_y_ _m_o_d_e_l_s_ _c_a_n_ _b_e_ _l_o_a_d_e_d_ _f_r_o_m_ _t_h_e_ _d_i_r_e_c_t_o_r_y_ _o_f_ _o_t_o_o_l_e_-_f_o_r_m_a_t_t_e_d_ _c_s_v_s_.
 _`_`_`_p_y_t_h_o_n_ _f_r_o_m_ _t_z_._o_s_e_m_o_s_y_s_ _i_m_p_o_r_t_ _M_o_d_e_l_ _m_y___m_o_d_e_l_ _=_ _M_o_d_e_l_._f_r_o_m___o_t_o_o_l_e___c_s_v_(_"_p_a_t_h_/
 _t_o_/_o_t_o_o_l_e_/_c_s_v_/_d_i_r_e_c_t_o_r_y_"_)_ _`_`_`_ _R_e_a_d_ _m_o_r_e_ _i_n_ _t_h_e_ _[_d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/
 _d_o_c_s_._f_e_o_._t_r_a_n_s_i_t_i_o_n_z_e_r_o_._o_r_g_/_)_ _#_#_#_ _D_e_v_e_l_o_p_m_e_n_t_ _a_n_d_ _C_o_n_t_r_i_b_u_t_i_n_g_ _W_e_ _w_e_l_c_o_m_e
 _c_o_n_t_r_i_b_u_t_i_o_n_s_!_ _T_o_ _g_e_t_ _s_t_a_r_t_e_d_ _a_s_ _a_ _c_o_n_t_r_i_b_u_t_o_r_ _o_r_ _a_s_ _a_ _d_e_v_e_l_o_p_e_r_,_ _p_l_e_a_s_e_ _r_e_a_d
```

### Comparing `tz-osemosys-0.0.1/tz_osemosys.egg-info/SOURCES.txt` & `tz_osemosys-0.0.3/tz_osemosys.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -35,40 +35,45 @@
 tz/osemosys/defaults.py
 tz/osemosys/exceptions.py
 tz/osemosys/logger.py
 tz/osemosys/io/__init__.py
 tz/osemosys/io/load_model.py
 tz/osemosys/io/simpleeval.py
 tz/osemosys/model/__init__.py
-tz/osemosys/model/linear_expressions.py
 tz/osemosys/model/model.py
 tz/osemosys/model/objective.py
 tz/osemosys/model/constraints/__init__.py
 tz/osemosys/model/constraints/accounting_technology.py
 tz/osemosys/model/constraints/annual_activity.py
 tz/osemosys/model/constraints/capacity_adequacy_a.py
 tz/osemosys/model/constraints/capacity_adequacy_b.py
 tz/osemosys/model/constraints/capital_costs.py
-tz/osemosys/model/constraints/demand.py
 tz/osemosys/model/constraints/emissions.py
 tz/osemosys/model/constraints/energy_balance_a.py
 tz/osemosys/model/constraints/energy_balance_b.py
 tz/osemosys/model/constraints/new_capacity.py
 tz/osemosys/model/constraints/operating_costs.py
 tz/osemosys/model/constraints/re_targets.py
 tz/osemosys/model/constraints/reserve_margin.py
 tz/osemosys/model/constraints/salvage_value.py
 tz/osemosys/model/constraints/storage.py
 tz/osemosys/model/constraints/total_activity.py
 tz/osemosys/model/constraints/total_capacity.py
 tz/osemosys/model/constraints/total_discounted_costs.py
+tz/osemosys/model/linear_expressions/__init__.py
+tz/osemosys/model/linear_expressions/activity.py
+tz/osemosys/model/linear_expressions/capacity.py
+tz/osemosys/model/linear_expressions/emissions.py
+tz/osemosys/model/linear_expressions/financials.py
+tz/osemosys/model/linear_expressions/production.py
+tz/osemosys/model/linear_expressions/reserve_margin.py
+tz/osemosys/model/linear_expressions/storage.py
 tz/osemosys/model/variables/__init__.py
 tz/osemosys/model/variables/activity.py
 tz/osemosys/model/variables/capacity.py
-tz/osemosys/model/variables/demand.py
 tz/osemosys/model/variables/emissions.py
 tz/osemosys/model/variables/other.py
 tz/osemosys/model/variables/storage.py
 tz/osemosys/schemas/__init__.py
 tz/osemosys/schemas/base.py
 tz/osemosys/schemas/commodity.py
 tz/osemosys/schemas/impact.py
```

