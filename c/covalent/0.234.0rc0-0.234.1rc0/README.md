# Comparing `tmp/covalent-0.234.0rc0.tar.gz` & `tmp/covalent-0.234.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-0.234.0rc0.tar", last modified: Wed Feb  7 13:40:18 2024, max compression
+gzip compressed data, was "covalent-0.234.1rc0.tar", last modified: Fri May 10 12:52:29 2024, max compression
```

## Comparing `covalent-0.234.0rc0.tar` & `covalent-0.234.1rc0.tar`

### file list

```diff
@@ -1,412 +1,412 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:18.028672 covalent-0.234.0rc0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-02-07 13:40:18.028672 covalent-0.234.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.964672 covalent-0.234.0rc0/covalent/
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.964672 covalent-0.234.0rc0/covalent/_api/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_api/apiclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.964672 covalent-0.234.0rc0/covalent/_dispatcher_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_dispatcher_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_dispatcher_plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21692 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_dispatcher_plugins/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.968673 covalent-0.234.0rc0/covalent/_file_transfer/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_file_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_file_transfer/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_file_transfer/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_file_transfer/file_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_file_transfer/folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.968673 covalent-0.234.0rc0/covalent/_file_transfer/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_file_transfer/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_file_transfer/strategies/blob_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_file_transfer/strategies/gcloud_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_file_transfer/strategies/http_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_file_transfer/strategies/rsync_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_file_transfer/strategies/s3_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_file_transfer/strategies/shutil_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_file_transfer/strategies/transfer_strategy_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.968673 covalent-0.234.0rc0/covalent/_programmatic/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_programmatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_programmatic/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.968673 covalent-0.234.0rc0/covalent/_results_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_results_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_results_manager/qresult.py
--rw-r--r--   0 runner    (1001) docker     (127)    18128 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_results_manager/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    18446 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_results_manager/results_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_results_manager/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_results_manager/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.968673 covalent-0.234.0rc0/covalent/_serialize/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_serialize/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_serialize/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_serialize/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_serialize/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_serialize/transport_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.972673 covalent-0.234.0rc0/covalent/_shared_files/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/pickling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/qelectron_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/qinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/qresult_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.972673 covalent-0.234.0rc0/covalent/_shared_files/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/schemas/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/schemas/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/schemas/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/schemas/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/schemas/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/schemas/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/schemas/transport_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/util_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_shared_files/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.976673 covalent-0.234.0rc0/covalent/_workflow/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/depsbash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/depscall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/depsmodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/depspip.py
--rw-r--r--   0 runner    (1001) docker     (127)    33822 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)    18557 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/lepton.py
--rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/qdevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/qelectron.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/qnode.py
--rw-r--r--   0 runner    (1001) docker     (127)    19920 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/_workflow/transportable_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.976673 covalent-0.234.0rc0/covalent/cloud_resource_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/cloud_resource_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/cloud_resource_manager/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.976673 covalent-0.234.0rc0/covalent/executor/
--rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29163 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.976673 covalent-0.234.0rc0/covalent/executor/executor_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/executor_plugins/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/executor_plugins/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/executor_plugins/remote_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/qbase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.960672 covalent-0.234.0rc0/covalent/executor/quantum_plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.976673 covalent-0.234.0rc0/covalent/executor/quantum_plugins/aws_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/quantum_plugins/aws_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/quantum_plugins/aws_plugin/aws_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.976673 covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/devices_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/local_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13221 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/runtime_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.976673 covalent-0.234.0rc0/covalent/executor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/utils/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    21178 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/executor/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.976673 covalent-0.234.0rc0/covalent/leptons/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/leptons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.976673 covalent-0.234.0rc0/covalent/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.980672 covalent-0.234.0rc0/covalent/quantum/qclient/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qclient/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qclient/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qclient/local_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.980672 covalent-0.234.0rc0/covalent/quantum/qcluster/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qcluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qcluster/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qcluster/clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qcluster/default_selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qcluster/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.980672 covalent-0.234.0rc0/covalent/quantum/qserver/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14831 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qserver/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qserver/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qserver/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.980672 covalent-0.234.0rc0/covalent/quantum/qserver/servers/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qserver/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qserver/servers/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/quantum/qserver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.980672 covalent-0.234.0rc0/covalent/triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/triggers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/triggers/database_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/triggers/dir_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/triggers/sqlite_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/triggers/time_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent/triggers/trigger_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.964672 covalent-0.234.0rc0/covalent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-02-07 13:40:17.000000 covalent-0.234.0rc0/covalent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-02-07 13:40:17.000000 covalent-0.234.0rc0/covalent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 13:40:17.000000 covalent-0.234.0rc0/covalent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-07 13:40:17.000000 covalent-0.234.0rc0/covalent.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 13:40:17.000000 covalent-0.234.0rc0/covalent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-07 13:40:17.000000 covalent-0.234.0rc0/covalent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-07 13:40:17.000000 covalent-0.234.0rc0/covalent.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.980672 covalent-0.234.0rc0/covalent_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.980672 covalent-0.234.0rc0/covalent_dispatcher/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.980672 covalent-0.234.0rc0/covalent_dispatcher/_cli/groups/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_cli/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_cli/groups/db_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_cli/groups/deploy_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_cli/groups/deploy_group_print_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    31291 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_cli/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.984672 covalent-0.234.0rc0/covalent_dispatcher/_core/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/data_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.984672 covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/asset_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/job_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/dispatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.984672 covalent-0.234.0rc0/covalent_dispatcher/_core/dispatcher_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/dispatcher_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/dispatcher_modules/caches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/dispatcher_modules/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.984672 covalent-0.234.0rc0/covalent_dispatcher/_core/runner_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/runner_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/runner_modules/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/runner_modules/executor_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/runner_modules/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/runner_modules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_core/runner_ng.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.988672 covalent-0.234.0rc0/covalent_dispatcher/_dal/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.988672 covalent-0.234.0rc0/covalent_dispatcher/_dal/db_interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/db_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/db_interfaces/edge_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/db_interfaces/electron_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/db_interfaces/lattice_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/db_interfaces/result_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/db_interfaces/tg_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/electron.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.988672 covalent-0.234.0rc0/covalent_dispatcher/_dal/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/exporters/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/exporters/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/exporters/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/exporters/tg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.988672 covalent-0.234.0rc0/covalent_dispatcher/_dal/importers/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/importers/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/importers/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/importers/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/importers/tg.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)    18552 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/tg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/tg_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.988672 covalent-0.234.0rc0/covalent_dispatcher/_dal/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/utils/file_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_dal/utils/uri_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.988672 covalent-0.234.0rc0/covalent_dispatcher/_db/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_db/datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_db/dispatchdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_db/jobdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_db/update.py
--rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_db/upsert.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_db/write_result_to_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.992673 covalent-0.234.0rc0/covalent_dispatcher/_object_store/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_object_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_object_store/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_object_store/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.992673 covalent-0.234.0rc0/covalent_dispatcher/_service/
--rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_service/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_service/app_dask.py
--rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_service/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_service/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_service/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_service/runnersvc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.992673 covalent-0.234.0rc0/covalent_dispatcher/_triggers_app/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_triggers_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/_triggers_app/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_dispatcher/entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.992673 covalent-0.234.0rc0/covalent_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.992673 covalent-0.234.0rc0/covalent_migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/versions/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/versions/1142d81b29b8_schema_updates_for_new_dal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/versions/26d71848a404_v12.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/versions/3727163f275c_consolidate_electron_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/versions/97202f5f47cb_v13.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/versions/9b9d58f02985_v11.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/versions/b60c5ecdf927_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/versions/de0a6c0a3e3d_add_qelectron_data_exists_flag_to_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_migrations/versions/f64ecaa040d5_add_jobs_db_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.992673 covalent-0.234.0rc0/covalent_ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.992673 covalent-0.234.0rc0/covalent_ui/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.992673 covalent-0.234.0rc0/covalent_ui/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.996672 covalent-0.234.0rc0/covalent_ui/api/v1/data_layer/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/data_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14035 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/data_layer/electron_dal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/data_layer/graph_dal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/data_layer/lattice_dal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/data_layer/logs_dal.py
--rw-r--r--   0 runner    (1001) docker     (127)    16365 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/data_layer/summary_dal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.996672 covalent-0.234.0rc0/covalent_ui/api/v1/database/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.996672 covalent-0.234.0rc0/covalent_ui/api/v1/database/config/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/database/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/database/config/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.996672 covalent-0.234.0rc0/covalent_ui/api/v1/database/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/database/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/database/schema/electron.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/database/schema/electron_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/database/schema/lattices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.996672 covalent-0.234.0rc0/covalent_ui/api/v1/models/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/models/dispatch_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/models/electrons_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/models/graph_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/models/lattices_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/models/logs_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/models/settings_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.996672 covalent-0.234.0rc0/covalent_ui/api/v1/routes/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.996672 covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/electron_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/graph_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/lattice_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/logs_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/settings_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/summary_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/routes/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:18.000672 covalent-0.234.0rc0/covalent_ui/api/v1/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/utils/file_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/utils/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/utils/models_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/api/v1/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/covalent_ui/result_webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.964672 covalent-0.234.0rc0/covalent_ui/webapp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:18.000672 covalent-0.234.0rc0/covalent_ui/webapp/build/
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-02-07 13:38:08.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-02-07 13:38:08.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/favicon64x64.ico
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-02-07 13:38:08.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/logo192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    29252 2024-02-07 13:38:08.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/logo512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-02-07 13:38:08.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/logo64x64.png
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-07 13:38:08.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-07 13:38:08.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:17.964672 covalent-0.234.0rc0/covalent_ui/webapp/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:18.000672 covalent-0.234.0rc0/covalent_ui/webapp/build/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:18.020672 covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)  2856333 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127) 10104263 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   307919 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   675742 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   374848 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   958942 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js
--rw-r--r--   0 runner    (1001) docker     (127)    15931 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 13:40:18.028672 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/SettingsIcon.29d14b34.svg
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/arg.71b4b335.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/atom.3f8fd5bf.svg
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/attribute.f1b86983.svg
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/back.c0aa0e78.svg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/checkmark.a5e834e4.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/circuit-large.a0c113f8.svg
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/close.2a867415.svg
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/codeview.eb72cac6.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/completing.e5f3aacb.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/connectionLost.d1c47690.svg
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/copy.4bbd1e1c.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/covalent-full-logo.0a6de0fd.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/covalent-logo-hover.87f421c8.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/covalent-logo.0a6de0fd.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/dashboard.4a7570e1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/delete.73fac4cf.svg
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/download.d767a1c5.svg
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/electron-dict.e471b060.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/electron-list.e5beabe1.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/error.6508a515.svg
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/exit.a2c5304b.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/failed.31c046fd.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/failedTopBar.e4182945.svg
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/filter.f9f7e173.svg
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/fit-view.a6228772.svg
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/fuction.f589c839.svg
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/generated.a2970d13.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/info.f99828bd.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/license.f61c24c7.svg
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/logs.551f3d28.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/parameter.11d0a2e0.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/parameter.a62e78f9.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/pending.1baceeef.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/post-process.8092f778.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/prettify.3bc46fc9.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/qelectron.ad89046a.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/queued.0af4b56e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/running.336c56e4.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/running.515f54a5.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/runningTopBar.bc8a86bd.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/screenshot.ebc53482.svg
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/stop.f09b4e72.svg
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/sublattice.f6ee1fb5.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/success.f693cbdc.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/successTopBar.f280e5c7.svg
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/terminal.1d8a1548.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/timeout.f67ccf19.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/tree.2780601c.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/view.f326778a.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/warning.6bae5b45.svg
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/zoom-in.f2603f36.svg
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-07 13:40:16.000000 covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/zoom-out.24dd0db1.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/requirements-client.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/requirements-qelectron.txt
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 13:40:18.028672 covalent-0.234.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-02-07 13:37:05.000000 covalent-0.234.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.798677 covalent-0.234.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-05-10 12:52:29.798677 covalent-0.234.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.730677 covalent-0.234.1rc0/covalent/
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.730677 covalent-0.234.1rc0/covalent/_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_api/apiclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.730677 covalent-0.234.1rc0/covalent/_dispatcher_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_dispatcher_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_dispatcher_plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21692 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_dispatcher_plugins/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.730677 covalent-0.234.1rc0/covalent/_file_transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/file_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.734677 covalent-0.234.1rc0/covalent/_file_transfer/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/blob_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/gcloud_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/http_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/rsync_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/s3_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/shutil_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_file_transfer/strategies/transfer_strategy_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.734677 covalent-0.234.1rc0/covalent/_programmatic/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_programmatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_programmatic/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.734677 covalent-0.234.1rc0/covalent/_results_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_results_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_results_manager/qresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18128 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_results_manager/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18446 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_results_manager/results_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_results_manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_results_manager/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.734677 covalent-0.234.1rc0/covalent/_serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_serialize/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_serialize/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_serialize/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_serialize/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_serialize/transport_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.738677 covalent-0.234.1rc0/covalent/_shared_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/context_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/pickling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/qelectron_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/qinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/qresult_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.738677 covalent-0.234.1rc0/covalent/_shared_files/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/schemas/transport_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/util_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_shared_files/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.738677 covalent-0.234.1rc0/covalent/_workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/depsbash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/depscall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/depsmodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/depspip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32980 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18557 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/lepton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/qdevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/qelectron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/qnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19920 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/_workflow/transportable_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.738677 covalent-0.234.1rc0/covalent/cloud_resource_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/cloud_resource_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/cloud_resource_manager/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/executor/
+-rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29163 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/executor/executor_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/executor_plugins/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9157 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/executor_plugins/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/executor_plugins/remote_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/qbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.722677 covalent-0.234.1rc0/covalent/executor/quantum_plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/executor/quantum_plugins/aws_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/aws_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/aws_plugin/aws_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/devices_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/local_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13221 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/runtime_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/executor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/utils/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21178 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/executor/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/leptons/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/leptons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.742677 covalent-0.234.1rc0/covalent/quantum/qclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qclient/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qclient/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qclient/local_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent/quantum/qcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qcluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qcluster/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qcluster/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qcluster/default_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qcluster/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent/quantum/qserver/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14831 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent/quantum/qserver/servers/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/servers/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/quantum/qserver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent/triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/database_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/dir_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/sqlite_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/time_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent/triggers/trigger_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.730677 covalent-0.234.1rc0/covalent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-10 12:52:29.000000 covalent-0.234.1rc0/covalent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent_dispatcher/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.746677 covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/db_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/deploy_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/deploy_group_print_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31291 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_cli/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.750676 covalent-0.234.1rc0/covalent_dispatcher/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.750676 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/asset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.750676 covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/caches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.750676 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/executor_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15331 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_core/runner_ng.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.754677 covalent-0.234.1rc0/covalent_dispatcher/_dal/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.754677 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/edge_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/electron_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/lattice_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/result_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/tg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/electron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.754677 covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/tg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.754677 covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/tg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18552 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/tg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/tg_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.754677 covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/file_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/uri_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.758677 covalent-0.234.1rc0/covalent_dispatcher/_db/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/dispatchdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/jobdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16350 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/upsert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_db/write_result_to_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.758677 covalent-0.234.1rc0/covalent_dispatcher/_object_store/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_object_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_object_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_object_store/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.758677 covalent-0.234.1rc0/covalent_dispatcher/_service/
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_service/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_service/app_dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17972 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_service/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_service/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_service/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_service/runnersvc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.758677 covalent-0.234.1rc0/covalent_dispatcher/_triggers_app/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_triggers_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/_triggers_app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_dispatcher/entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.758677 covalent-0.234.1rc0/covalent_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/1142d81b29b8_schema_updates_for_new_dal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/26d71848a404_v12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/3727163f275c_consolidate_electron_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/97202f5f47cb_v13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/9b9d58f02985_v11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/b60c5ecdf927_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/de0a6c0a3e3d_add_qelectron_data_exists_flag_to_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_migrations/versions/f64ecaa040d5_add_jobs_db_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14035 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/electron_dal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/graph_dal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/lattice_dal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/logs_dal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16365 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/summary_dal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/database/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/config/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/electron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/electron_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/lattices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/dispatch_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/electrons_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/graph_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/lattices_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/logs_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/models/settings_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.762677 covalent-0.234.1rc0/covalent_ui/api/v1/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.766677 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/electron_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/graph_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/lattice_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/logs_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/settings_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/summary_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/routes/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.766677 covalent-0.234.1rc0/covalent_ui/api/v1/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/utils/file_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/utils/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/utils/models_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/api/v1/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-10 12:49:21.000000 covalent-0.234.1rc0/covalent_ui/result_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.726677 covalent-0.234.1rc0/covalent_ui/webapp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.766677 covalent-0.234.1rc0/covalent_ui/webapp/build/
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/favicon64x64.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/logo192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29252 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/logo512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/logo64x64.png
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-10 12:50:20.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.726677 covalent-0.234.1rc0/covalent_ui/webapp/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.766677 covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.790677 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  2856333 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127) 10104263 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   307919 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   675742 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   374848 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   958942 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15931 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:52:29.798677 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/SettingsIcon.29d14b34.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/arg.71b4b335.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/atom.3f8fd5bf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/attribute.f1b86983.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/back.c0aa0e78.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/checkmark.a5e834e4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/circuit-large.a0c113f8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/close.2a867415.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/codeview.eb72cac6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/completing.e5f3aacb.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/connectionLost.d1c47690.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/copy.4bbd1e1c.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/covalent-full-logo.0a6de0fd.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/covalent-logo-hover.87f421c8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/covalent-logo.0a6de0fd.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/dashboard.4a7570e1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/delete.73fac4cf.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/download.d767a1c5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/electron-dict.e471b060.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/electron-list.e5beabe1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/error.6508a515.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/exit.a2c5304b.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/failed.31c046fd.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/failedTopBar.e4182945.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/filter.f9f7e173.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/fit-view.a6228772.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/fuction.f589c839.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/generated.a2970d13.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/info.f99828bd.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/license.f61c24c7.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/logs.551f3d28.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/parameter.11d0a2e0.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/parameter.a62e78f9.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/pending.1baceeef.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/post-process.8092f778.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/prettify.3bc46fc9.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/qelectron.ad89046a.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/queued.0af4b56e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/running.336c56e4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/running.515f54a5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/runningTopBar.bc8a86bd.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/screenshot.ebc53482.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/stop.f09b4e72.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/sublattice.f6ee1fb5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/success.f693cbdc.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/successTopBar.f280e5c7.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/terminal.1d8a1548.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/timeout.f67ccf19.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/tree.2780601c.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/view.f326778a.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/warning.6bae5b45.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/zoom-in.f2603f36.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-10 12:52:28.000000 covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/zoom-out.24dd0db1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-10 12:49:22.000000 covalent-0.234.1rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-10 12:49:22.000000 covalent-0.234.1rc0/requirements-client.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-10 12:49:22.000000 covalent-0.234.1rc0/requirements-qelectron.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-10 12:49:22.000000 covalent-0.234.1rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:52:29.798677 covalent-0.234.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-10 12:49:22.000000 covalent-0.234.1rc0/setup.py
```

### Comparing `covalent-0.234.0rc0/LICENSE` & `covalent-0.234.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/PKG-INFO` & `covalent-0.234.1rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent
-Version: 0.234.0rc0
+Version: 0.234.1rc0
 Summary: Covalent Workflow Tool
 Home-page: https://github.com/AgnostiqHQ/covalent
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: Apache License 2.0
-Download-URL: https://github.com/AgnostiqHQ/covalent/archive/v0.234.0-rc.0.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent/archive/v0.234.1-rc.0.tar.gz
 Description: <div align="center">
           <img src="./doc/source/_static/banner_executor.gif" alt="hero" />
         </div>
         </br>
         <div align="center">
         
         [![version](https://img.shields.io/github/v/tag/AgnostiqHQ/covalent?color=%235552FF&include_prereleases&label=version&sort=semver)](https://github.com/AgnostiqHQ/covalent/blob/develop/CHANGELOG.md)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: covalent Version: 0.234.0rc0 Summary: Covalent
+Metadata-Version: 2.1 Name: covalent Version: 0.234.1rc0 Summary: Covalent
 Workflow Tool Home-page: https://github.com/AgnostiqHQ/covalent Author:
 Agnostiq Author-email: support@agnostiq.ai Maintainer: Agnostiq License: Apache
 License 2.0 Download-URL: https://github.com/AgnostiqHQ/covalent/archive/
-v0.234.0-rc.0.tar.gz Description:
+v0.234.1-rc.0.tar.gz Description:
                                     [hero]
           [![version](https://img.shields.io/github/v/tag/AgnostiqHQ/
 covalent?color=%235552FF&include_prereleases&label=version&sort=semver)](https:
  //github.com/AgnostiqHQ/covalent/blob/develop/CHANGELOG.md) [![Static Badge]
   (https://img.shields.io/badge/python-3.8_%7C_3.9_%7C_3.10-%235552FF)](#) [!
           [Static Badge](https://img.shields.io/badge/tests-passing-
     %235552FF?logo=github)](https://github.com/AgnostiqHQ/covalent/actions/
```

### Comparing `covalent-0.234.0rc0/README.md` & `covalent-0.234.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/__init__.py` & `covalent-0.234.1rc0/covalent/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_api/__init__.py` & `covalent-0.234.1rc0/covalent/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_api/apiclient.py` & `covalent-0.234.1rc0/covalent/_api/apiclient.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_dispatcher_plugins/__init__.py` & `covalent-0.234.1rc0/covalent/_dispatcher_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_dispatcher_plugins/base.py` & `covalent-0.234.1rc0/covalent/_dispatcher_plugins/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_dispatcher_plugins/local.py` & `covalent-0.234.1rc0/covalent/_dispatcher_plugins/local.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_file_transfer/__init__.py` & `covalent-0.234.1rc0/covalent/_file_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_file_transfer/enums.py` & `covalent-0.234.1rc0/covalent/_file_transfer/enums.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_file_transfer/file.py` & `covalent-0.234.1rc0/covalent/_file_transfer/file.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_file_transfer/file_transfer.py` & `covalent-0.234.1rc0/covalent/_file_transfer/file_transfer.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_file_transfer/folder.py` & `covalent-0.234.1rc0/covalent/_file_transfer/folder.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_file_transfer/strategies/__init__.py` & `covalent-0.234.1rc0/covalent/_file_transfer/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_file_transfer/strategies/blob_strategy.py` & `covalent-0.234.1rc0/covalent/_file_transfer/strategies/blob_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_file_transfer/strategies/gcloud_strategy.py` & `covalent-0.234.1rc0/covalent/_file_transfer/strategies/gcloud_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_file_transfer/strategies/http_strategy.py` & `covalent-0.234.1rc0/covalent/_file_transfer/strategies/http_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_file_transfer/strategies/rsync_strategy.py` & `covalent-0.234.1rc0/covalent/_file_transfer/strategies/rsync_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_file_transfer/strategies/s3_strategy.py` & `covalent-0.234.1rc0/covalent/_file_transfer/strategies/s3_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_file_transfer/strategies/shutil_strategy.py` & `covalent-0.234.1rc0/covalent/_file_transfer/strategies/shutil_strategy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_file_transfer/strategies/transfer_strategy_base.py` & `covalent-0.234.1rc0/covalent/_file_transfer/strategies/transfer_strategy_base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_programmatic/__init__.py` & `covalent-0.234.1rc0/covalent/_programmatic/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_programmatic/commands.py` & `covalent-0.234.1rc0/covalent/_programmatic/commands.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_results_manager/__init__.py` & `covalent-0.234.1rc0/covalent/_results_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_results_manager/qresult.py` & `covalent-0.234.1rc0/covalent/_results_manager/qresult.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_results_manager/result.py` & `covalent-0.234.1rc0/covalent/_results_manager/result.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_results_manager/results_manager.py` & `covalent-0.234.1rc0/covalent/_results_manager/results_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_results_manager/utils.py` & `covalent-0.234.1rc0/covalent/_results_manager/utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_results_manager/wait.py` & `covalent-0.234.1rc0/covalent/_results_manager/wait.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_serialize/__init__.py` & `covalent-0.234.1rc0/covalent/_serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_serialize/common.py` & `covalent-0.234.1rc0/covalent/_serialize/common.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_serialize/electron.py` & `covalent-0.234.1rc0/covalent/_serialize/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_serialize/lattice.py` & `covalent-0.234.1rc0/covalent/_serialize/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_serialize/result.py` & `covalent-0.234.1rc0/covalent/_serialize/result.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_serialize/transport_graph.py` & `covalent-0.234.1rc0/covalent/_serialize/transport_graph.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/__init__.py` & `covalent-0.234.1rc0/covalent/_shared_files/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/config.py` & `covalent-0.234.1rc0/covalent/_shared_files/config.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/context_managers.py` & `covalent-0.234.1rc0/covalent/_shared_files/context_managers.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/defaults.py` & `covalent-0.234.1rc0/covalent/_shared_files/defaults.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/exceptions.py` & `covalent-0.234.1rc0/covalent/_shared_files/exceptions.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/logger.py` & `covalent-0.234.1rc0/covalent/_shared_files/logger.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/metrics.py` & `covalent-0.234.1rc0/covalent/_shared_files/metrics.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/pickling.py` & `covalent-0.234.1rc0/covalent/_shared_files/pickling.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/qelectron_utils.py` & `covalent-0.234.1rc0/covalent/_shared_files/qelectron_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/qinfo.py` & `covalent-0.234.1rc0/covalent/_shared_files/qinfo.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/qresult_utils.py` & `covalent-0.234.1rc0/covalent/_shared_files/qresult_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/schemas/__init__.py` & `covalent-0.234.1rc0/covalent/_shared_files/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/schemas/asset.py` & `covalent-0.234.1rc0/covalent/_shared_files/schemas/asset.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/schemas/common.py` & `covalent-0.234.1rc0/covalent/_shared_files/schemas/common.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/schemas/edge.py` & `covalent-0.234.1rc0/covalent/_shared_files/schemas/edge.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/schemas/electron.py` & `covalent-0.234.1rc0/covalent/_shared_files/schemas/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/schemas/lattice.py` & `covalent-0.234.1rc0/covalent/_shared_files/schemas/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/schemas/result.py` & `covalent-0.234.1rc0/covalent/_shared_files/schemas/result.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/schemas/transport_graph.py` & `covalent-0.234.1rc0/covalent/_shared_files/schemas/transport_graph.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/util_classes.py` & `covalent-0.234.1rc0/covalent/_shared_files/util_classes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_shared_files/utils.py` & `covalent-0.234.1rc0/covalent/_shared_files/utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/__init__.py` & `covalent-0.234.1rc0/covalent/_workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/deps.py` & `covalent-0.234.1rc0/covalent/_workflow/deps.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/depsbash.py` & `covalent-0.234.1rc0/covalent/_workflow/depsbash.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/depscall.py` & `covalent-0.234.1rc0/covalent/_workflow/depscall.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/depsmodule.py` & `covalent-0.234.1rc0/covalent/_workflow/depsmodule.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/depspip.py` & `covalent-0.234.1rc0/covalent/_workflow/depspip.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/electron.py` & `covalent-0.234.1rc0/covalent/_workflow/electron.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
         if metadata is None:
             metadata = {}
         self.function = function
         self.node_id = node_id
         self.metadata = metadata
         self.task_group_id = task_group_id
         self._packing_tasks = packing_tasks
+        self._function_string = get_serialized_function_str(function)
 
     @property
     def packing_tasks(self) -> bool:
         return self._packing_tasks
 
     def set_metadata(self, name: str, value: Any) -> None:
         """
@@ -438,15 +439,15 @@
 
             sub_electron = Electron(
                 function=_build_sublattice_graph,
                 metadata=e_meta,
             )
 
             name = sublattice_prefix + self.function.__name__
-            function_string = get_serialized_function_str(self.function)
+            function_string = self._function_string
             bound_electron = sub_electron(
                 self.function, json.dumps(parent_metadata), *args, **kwargs
             )
 
             active_lattice.transport_graph.set_node_value(bound_electron.node_id, "name", name)
             active_lattice.transport_graph.set_node_value(
                 bound_electron.node_id,
@@ -459,15 +460,15 @@
         # Add a node to the transport graph of the active lattice. Electrons bound to nodes will never be packed with the
         # 'master' Electron. # Add non-sublattice node to the transport graph of the active lattice.
 
         self.node_id = active_lattice.transport_graph.add_node(
             name=self.function.__name__,
             function=self.function,
             metadata=self.metadata.copy(),
-            function_string=get_serialized_function_str(self.function),
+            function_string=self._function_string,
             task_group_id=self.task_group_id if self.packing_tasks else None,
         )
         self.task_group_id = self.task_group_id if self.packing_tasks else self.node_id
 
         if self.function:
             named_args, named_kwargs = get_named_params(self.function, args, kwargs)
 
@@ -567,24 +568,24 @@
                 edge_name=param_name,
                 param_type=param_type,
                 arg_index=arg_index,
             )
 
         elif isinstance(param_value, dict):
 
-            def _auto_dict_node(*args, **kwargs):
-                return dict(kwargs)
+            def _auto_dict_node(keys, values):
+                return {keys[i]: values[i] for i in range(len(keys))}
 
             dict_electron = Electron(
                 function=_auto_dict_node,
                 metadata=collection_metadata,
                 task_group_id=self.task_group_id,
                 packing_tasks=True and active_lattice.task_packing,
             )  # Group the auto-generated node with the main node.
-            bound_electron = dict_electron(**param_value)
+            bound_electron = dict_electron(list(param_value.keys()), list(param_value.values()))
             transport_graph.set_node_value(bound_electron.node_id, "name", electron_dict_prefix)
             transport_graph.add_edge(
                 dict_electron.node_id,
                 node_id,
                 edge_name=param_name,
                 param_type=param_type,
                 arg_index=arg_index,
@@ -604,40 +605,14 @@
                 parameter_node,
                 node_id,
                 edge_name=param_name,
                 param_type=param_type,
                 arg_index=arg_index,
             )
 
-    def add_collection_node_to_graph(self, graph: "_TransportGraph", prefix: str) -> int:
-        """
-        Adds the node to lattice's transport graph in the case
-        where a collection of electrons is passed as an argument
-        to another electron.
-
-        Args:
-            graph: Transport graph of the lattice
-            prefix: Prefix of the node
-
-        Returns:
-            node_id: Node id of the added node
-        """
-
-        new_metadata = encode_metadata(DEFAULT_METADATA_VALUES.copy())
-        if "executor" in self.metadata:
-            new_metadata["executor"] = self.metadata["executor"]
-            new_metadata["executor_data"] = self.metadata["executor_data"]
-
-        node_id = graph.add_node(
-            name=prefix,
-            function=to_decoded_electron_collection,
-            metadata=new_metadata,
-            function_string=get_serialized_function_str(to_decoded_electron_collection),
-        )
-
         return node_id
 
     def wait_for(self, electrons: Union["Electron", Iterable["Electron"]]):
         """
         Waits for the given electrons to complete before executing this one.
         Adds the necessary edges between this and those electrons without explicitly
         connecting their inputs/outputs.
```

### Comparing `covalent-0.234.0rc0/covalent/_workflow/lattice.py` & `covalent-0.234.1rc0/covalent/_workflow/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/lepton.py` & `covalent-0.234.1rc0/covalent/_workflow/lepton.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/postprocessing.py` & `covalent-0.234.1rc0/covalent/_workflow/postprocessing.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/qdevice.py` & `covalent-0.234.1rc0/covalent/_workflow/qdevice.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/qelectron.py` & `covalent-0.234.1rc0/covalent/_workflow/qelectron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/qnode.py` & `covalent-0.234.1rc0/covalent/_workflow/qnode.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/transport.py` & `covalent-0.234.1rc0/covalent/_workflow/transport.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/_workflow/transportable_object.py` & `covalent-0.234.1rc0/covalent/_workflow/transportable_object.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/cloud_resource_manager/__init__.py` & `covalent-0.234.1rc0/covalent/cloud_resource_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/cloud_resource_manager/core.py` & `covalent-0.234.1rc0/covalent/cloud_resource_manager/core.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/__init__.py` & `covalent-0.234.1rc0/covalent/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/base.py` & `covalent-0.234.1rc0/covalent/executor/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/executor_plugins/dask.py` & `covalent-0.234.1rc0/covalent/executor/executor_plugins/dask.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/executor_plugins/local.py` & `covalent-0.234.1rc0/covalent/executor/executor_plugins/local.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/executor_plugins/remote_executor.py` & `covalent-0.234.1rc0/covalent/executor/executor_plugins/remote_executor.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/qbase.py` & `covalent-0.234.1rc0/covalent/executor/qbase.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/quantum_plugins/aws_plugin/__init__.py` & `covalent-0.234.1rc0/covalent/executor/quantum_plugins/aws_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/quantum_plugins/aws_plugin/aws_plugin.py` & `covalent-0.234.1rc0/covalent/executor/quantum_plugins/aws_plugin/aws_plugin.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/__init__.py` & `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/devices_base.py` & `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/devices_base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/local_sampler.py` & `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/local_sampler.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_plugin.py` & `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_plugin.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_utils.py` & `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/qiskit_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/runtime_sampler.py` & `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/runtime_sampler.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/quantum_plugins/qiskit_plugin/sessions.py` & `covalent-0.234.1rc0/covalent/executor/quantum_plugins/qiskit_plugin/sessions.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/schemas.py` & `covalent-0.234.1rc0/covalent/executor/schemas.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/utils/__init__.py` & `covalent-0.234.1rc0/covalent/executor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/utils/context.py` & `covalent-0.234.1rc0/covalent/executor/utils/context.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/utils/enums.py` & `covalent-0.234.1rc0/covalent/executor/utils/enums.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/utils/serialize.py` & `covalent-0.234.1rc0/covalent/executor/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/executor/utils/wrappers.py` & `covalent-0.234.1rc0/covalent/executor/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/leptons/__init__.py` & `covalent-0.234.1rc0/covalent/leptons/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/__init__.py` & `covalent-0.234.1rc0/covalent/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qclient/__init__.py` & `covalent-0.234.1rc0/covalent/quantum/qclient/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qclient/base_client.py` & `covalent-0.234.1rc0/covalent/quantum/qclient/base_client.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qclient/core.py` & `covalent-0.234.1rc0/covalent/quantum/qclient/core.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qclient/local_client.py` & `covalent-0.234.1rc0/covalent/quantum/qclient/local_client.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qcluster/__init__.py` & `covalent-0.234.1rc0/covalent/quantum/qcluster/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qcluster/base.py` & `covalent-0.234.1rc0/covalent/quantum/qcluster/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qcluster/clusters.py` & `covalent-0.234.1rc0/covalent/quantum/qcluster/clusters.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qcluster/default_selectors.py` & `covalent-0.234.1rc0/covalent/quantum/qcluster/default_selectors.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qcluster/simulator.py` & `covalent-0.234.1rc0/covalent/quantum/qcluster/simulator.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qserver/__init__.py` & `covalent-0.234.1rc0/covalent/quantum/qserver/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qserver/core.py` & `covalent-0.234.1rc0/covalent/quantum/qserver/core.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qserver/database.py` & `covalent-0.234.1rc0/covalent/quantum/qserver/database.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qserver/serialize.py` & `covalent-0.234.1rc0/covalent/quantum/qserver/serialize.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qserver/servers/__init__.py` & `covalent-0.234.1rc0/covalent/quantum/qserver/servers/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qserver/servers/local.py` & `covalent-0.234.1rc0/covalent/quantum/qserver/servers/local.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/quantum/qserver/utils.py` & `covalent-0.234.1rc0/covalent/quantum/qserver/utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/triggers/__init__.py` & `covalent-0.234.1rc0/covalent/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/triggers/base.py` & `covalent-0.234.1rc0/covalent/triggers/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/triggers/database_trigger.py` & `covalent-0.234.1rc0/covalent/triggers/database_trigger.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/triggers/dir_trigger.py` & `covalent-0.234.1rc0/covalent/triggers/dir_trigger.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/triggers/sqlite_trigger.py` & `covalent-0.234.1rc0/covalent/triggers/sqlite_trigger.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/triggers/time_trigger.py` & `covalent-0.234.1rc0/covalent/triggers/time_trigger.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent/triggers/trigger_loader.py` & `covalent-0.234.1rc0/covalent/triggers/trigger_loader.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent.egg-info/PKG-INFO` & `covalent-0.234.1rc0/covalent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: covalent
-Version: 0.234.0rc0
+Version: 0.234.1rc0
 Summary: Covalent Workflow Tool
 Home-page: https://github.com/AgnostiqHQ/covalent
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: Apache License 2.0
-Download-URL: https://github.com/AgnostiqHQ/covalent/archive/v0.234.0-rc.0.tar.gz
+Download-URL: https://github.com/AgnostiqHQ/covalent/archive/v0.234.1-rc.0.tar.gz
 Description: <div align="center">
           <img src="./doc/source/_static/banner_executor.gif" alt="hero" />
         </div>
         </br>
         <div align="center">
         
         [![version](https://img.shields.io/github/v/tag/AgnostiqHQ/covalent?color=%235552FF&include_prereleases&label=version&sort=semver)](https://github.com/AgnostiqHQ/covalent/blob/develop/CHANGELOG.md)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: covalent Version: 0.234.0rc0 Summary: Covalent
+Metadata-Version: 2.1 Name: covalent Version: 0.234.1rc0 Summary: Covalent
 Workflow Tool Home-page: https://github.com/AgnostiqHQ/covalent Author:
 Agnostiq Author-email: support@agnostiq.ai Maintainer: Agnostiq License: Apache
 License 2.0 Download-URL: https://github.com/AgnostiqHQ/covalent/archive/
-v0.234.0-rc.0.tar.gz Description:
+v0.234.1-rc.0.tar.gz Description:
                                     [hero]
           [![version](https://img.shields.io/github/v/tag/AgnostiqHQ/
 covalent?color=%235552FF&include_prereleases&label=version&sort=semver)](https:
  //github.com/AgnostiqHQ/covalent/blob/develop/CHANGELOG.md) [![Static Badge]
   (https://img.shields.io/badge/python-3.8_%7C_3.9_%7C_3.10-%235552FF)](#) [!
           [Static Badge](https://img.shields.io/badge/tests-passing-
     %235552FF?logo=github)](https://github.com/AgnostiqHQ/covalent/actions/
```

### Comparing `covalent-0.234.0rc0/covalent.egg-info/SOURCES.txt` & `covalent-0.234.1rc0/covalent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent.egg-info/requires.txt` & `covalent-0.234.1rc0/covalent.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_cli/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_cli/cli.py` & `covalent-0.234.1rc0/covalent_dispatcher/_cli/cli.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_cli/groups/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_cli/groups/db_group.py` & `covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/db_group.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_cli/groups/deploy_group.py` & `covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/deploy_group.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_cli/groups/deploy_group_print_callbacks.py` & `covalent-0.234.1rc0/covalent_dispatcher/_cli/groups/deploy_group_print_callbacks.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_cli/migrate.py` & `covalent-0.234.1rc0/covalent_dispatcher/_cli/migrate.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_cli/service.py` & `covalent-0.234.1rc0/covalent_dispatcher/_cli/service.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/data_manager.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/data_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/asset_manager.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/asset_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/dispatch.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/dispatch.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/electron.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/graph.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/graph.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/importer.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/importer.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/job_manager.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/job_manager.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/lattice.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/data_modules/utils.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/data_modules/utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/dispatcher.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,27 +179,30 @@
             "end_time": ts,
             "status": RESULT_STATUS.COMPLETED,
         }
         await datasvc.update_node_result(dispatch_id, node_result)
         app_log.debug("8A: Update node success (run_planned_workflow).")
 
     else:
+        # Nodes whose values have already been resolved
         known_nodes = []
 
         # Skip the group if all task outputs can be reused from a
         # previous dispatch (for redispatch).
         statuses = await datasvc.electron.get_bulk(dispatch_id, sorted_nodes, ["status"])
         incomplete = list(
             filter(lambda record: record["status"] != RESULT_STATUS.PENDING_REUSE, statuses)
         )
 
         if incomplete:
             # Gather inputs for each task and send the task spec sequence to the runner
             task_specs = []
 
+            sorted_nodes_set = set(sorted_nodes)
+
             for node_id in sorted_nodes:
                 app_log.debug(f"Gathering inputs for task {node_id} (run_planned_workflow).")
 
                 abs_task_input = await _get_abstract_task_inputs(dispatch_id, node_id, node_name)
 
                 executor_attrs = await datasvc.electron.get(
                     dispatch_id,
@@ -210,16 +213,24 @@
                 selected_executor_data = executor_attrs["executor_data"]
                 task_spec = {
                     "function_id": node_id,
                     "name": node_name,
                     "args_ids": abs_task_input["args"],
                     "kwargs_ids": abs_task_input["kwargs"],
                 }
-                known_nodes += abs_task_input["args"]
-                known_nodes += list(abs_task_input["kwargs"].values())
+                # Task inputs that don't belong to the task group have already beeen resolved
+                external_task_args = filter(
+                    lambda x: x not in sorted_nodes_set, abs_task_input["args"]
+                )
+                known_nodes.extend(external_task_args)
+                external_task_kwargs = filter(
+                    lambda x: x not in sorted_nodes_set, abs_task_input["kwargs"].values()
+                )
+                known_nodes.extend(external_task_kwargs)
+
                 task_specs.append(task_spec)
 
             app_log.debug(
                 f"Submitting task group {dispatch_id}:{task_group_id} ({len(sorted_nodes)} tasks) to runner"
             )
             app_log.debug(f"Using new runner for task group {task_group_id}")
```

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/dispatcher_modules/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/dispatcher_modules/caches.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/caches.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/dispatcher_modules/store.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/dispatcher_modules/store.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/execution.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/execution.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/runner.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/runner.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/runner_modules/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/runner_modules/cancel.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/cancel.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/runner_modules/executor_proxy.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/executor_proxy.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/runner_modules/jobs.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/jobs.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/runner_modules/utils.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/runner_modules/utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_core/runner_ng.py` & `covalent-0.234.1rc0/covalent_dispatcher/_core/runner_ng.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/asset.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/asset.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/base.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/controller.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/controller.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/db_interfaces/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/db_interfaces/edge_utils.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/edge_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/db_interfaces/electron_utils.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/electron_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/db_interfaces/lattice_utils.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/lattice_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/db_interfaces/result_utils.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/result_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/db_interfaces/tg_utils.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/db_interfaces/tg_utils.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/edge.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/edge.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/electron.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/exporters/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/exporters/electron.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/exporters/lattice.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/exporters/result.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/result.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/exporters/tg.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/exporters/tg.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/importers/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/importers/electron.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/importers/lattice.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/importers/result.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
         )
         if len(records) > 0:
             return _connect_result_to_electron(session, res, electron_id)
 
     # Main case: insert new lattice, electron, edge, and job records
 
     storage_path = os.path.join(base_path, dispatch_id)
-    os.makedirs(storage_path)
 
     lattice_record_kwargs = _get_result_meta(res, storage_path, electron_id)
     lattice_record_kwargs.update(_get_lattice_meta(res.lattice, storage_path))
 
     with Result.session() as session:
         st = datetime.now()
         lattice_row = ResultMeta.create(session, insert_kwargs=lattice_record_kwargs, flush=True)
@@ -139,14 +138,15 @@
         membership_filters={},
     )[0]
     parent_job_record = Job.get(
         session,
         fields={"id", "cancel_requested"},
         equality_filters={"id": parent_electron_record.job_id},
         membership_filters={},
+        for_update=True,
     )[0]
     cancel_requested = parent_job_record.cancel_requested
 
     sub_electron_records = ElectronMeta.get(
         session,
         fields={"id", "parent_lattice_id", "job_id"},
         equality_filters={"parent_lattice_id": sub_result._lattice_id},
```

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/importers/tg.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/importers/tg.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,17 @@
 ) -> TransportGraphSchema:
     electron_map = {}
     output_nodes = []
 
     # Propagate parent electron id's `cancel_requested` property to the sublattice electrons
     if electron_id is not None:
         parent_e_record = Electron.meta_type.get_by_primary_key(session, electron_id)
-        job_record = Job.get_by_primary_key(session=session, primary_key=parent_e_record.job_id)
+        job_record = Job.get_by_primary_key(
+            session=session, primary_key=parent_e_record.job_id, for_update=True
+        )
         cancel_requested = job_record.cancel_requested
     else:
         cancel_requested = False
 
     # Gather nodes into task groups
     task_groups = {i: [] for i in range(len(tg.nodes))}
     for node in tg.nodes:
```

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/job.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/job.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/lattice.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/lattice.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/result.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/result.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/tg.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/tg.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/tg_ops.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/tg_ops.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/utils/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/utils/file_transfer.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/file_transfer.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_dal/utils/uri_filters.py` & `covalent-0.234.1rc0/covalent_dispatcher/_dal/utils/uri_filters.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_db/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_db/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_db/datastore.py` & `covalent-0.234.1rc0/covalent_dispatcher/_db/datastore.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_db/dispatchdb.py` & `covalent-0.234.1rc0/covalent_dispatcher/_db/dispatchdb.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_db/jobdb.py` & `covalent-0.234.1rc0/covalent_dispatcher/_db/jobdb.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_db/models.py` & `covalent-0.234.1rc0/covalent_dispatcher/_db/models.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_db/update.py` & `covalent-0.234.1rc0/covalent_dispatcher/_db/update.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_db/upsert.py` & `covalent-0.234.1rc0/covalent_dispatcher/_db/upsert.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_db/write_result_to_db.py` & `covalent-0.234.1rc0/covalent_dispatcher/_db/write_result_to_db.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_object_store/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_object_store/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_object_store/base.py` & `covalent-0.234.1rc0/covalent_dispatcher/_object_store/base.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_object_store/local.py` & `covalent-0.234.1rc0/covalent_dispatcher/_object_store/local.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_service/app.py` & `covalent-0.234.1rc0/covalent_dispatcher/_service/app.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_service/app_dask.py` & `covalent-0.234.1rc0/covalent_dispatcher/_service/app_dask.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_service/assets.py` & `covalent-0.234.1rc0/covalent_dispatcher/_service/assets.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_service/heartbeat.py` & `covalent-0.234.1rc0/covalent_dispatcher/_service/heartbeat.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_service/models.py` & `covalent-0.234.1rc0/covalent_dispatcher/_service/models.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_service/runnersvc.py` & `covalent-0.234.1rc0/covalent_dispatcher/_service/runnersvc.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_triggers_app/__init__.py` & `covalent-0.234.1rc0/covalent_dispatcher/_triggers_app/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/_triggers_app/app.py` & `covalent-0.234.1rc0/covalent_dispatcher/_triggers_app/app.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_dispatcher/entry_point.py` & `covalent-0.234.1rc0/covalent_dispatcher/entry_point.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_migrations/README.md` & `covalent-0.234.1rc0/covalent_migrations/README.md`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_migrations/alembic.ini` & `covalent-0.234.1rc0/covalent_migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_migrations/env.py` & `covalent-0.234.1rc0/covalent_migrations/env.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_migrations/script.py.mako` & `covalent-0.234.1rc0/covalent_migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_migrations/versions/1142d81b29b8_schema_updates_for_new_dal.py` & `covalent-0.234.1rc0/covalent_migrations/versions/1142d81b29b8_schema_updates_for_new_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_migrations/versions/26d71848a404_v12.py` & `covalent-0.234.1rc0/covalent_migrations/versions/26d71848a404_v12.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_migrations/versions/3727163f275c_consolidate_electron_hooks.py` & `covalent-0.234.1rc0/covalent_migrations/versions/3727163f275c_consolidate_electron_hooks.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_migrations/versions/97202f5f47cb_v13.py` & `covalent-0.234.1rc0/covalent_migrations/versions/97202f5f47cb_v13.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_migrations/versions/9b9d58f02985_v11.py` & `covalent-0.234.1rc0/covalent_migrations/versions/9b9d58f02985_v11.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_migrations/versions/b60c5ecdf927_init.py` & `covalent-0.234.1rc0/covalent_migrations/versions/b60c5ecdf927_init.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_migrations/versions/de0a6c0a3e3d_add_qelectron_data_exists_flag_to_db.py` & `covalent-0.234.1rc0/covalent_migrations/versions/de0a6c0a3e3d_add_qelectron_data_exists_flag_to_db.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_migrations/versions/f64ecaa040d5_add_jobs_db_table.py` & `covalent-0.234.1rc0/covalent_migrations/versions/f64ecaa040d5_add_jobs_db_table.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/main.py` & `covalent-0.234.1rc0/covalent_ui/api/main.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/__init__.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/data_layer/__init__.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/data_layer/electron_dal.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/electron_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/data_layer/graph_dal.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/graph_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/data_layer/lattice_dal.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/lattice_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/data_layer/logs_dal.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/logs_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/data_layer/summary_dal.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/data_layer/summary_dal.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/database/__init__.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/database/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/database/config/__init__.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/database/config/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/database/config/db.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/database/config/db.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/database/schema/__init__.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/database/schema/electron.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/electron.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/database/schema/electron_dependency.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/electron_dependency.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/database/schema/lattices.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/database/schema/lattices.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/models/__init__.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/models/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/models/dispatch_model.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/models/dispatch_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/models/electrons_model.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/models/electrons_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/models/graph_model.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/models/graph_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/models/lattices_model.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/models/lattices_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/models/logs_model.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/models/logs_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/models/settings_model.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/models/settings_model.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/routes/__init__.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/electron_routes.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/electron_routes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/graph_route.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/graph_route.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/lattice_route.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/lattice_route.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/logs_route.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/logs_route.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/settings_routes.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/settings_routes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/routes/end_points/summary_routes.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/routes/end_points/summary_routes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/routes/routes.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/routes/routes.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/utils/__init__.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/utils/file_handle.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/utils/file_handle.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/utils/log_handler.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/utils/log_handler.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/utils/models_helper.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/utils/models_helper.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/api/v1/utils/status.py` & `covalent-0.234.1rc0/covalent_ui/api/v1/utils/status.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/app.py` & `covalent-0.234.1rc0/covalent_ui/app.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/result_webhook.py` & `covalent-0.234.1rc0/covalent_ui/result_webhook.py`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/asset-manifest.json` & `covalent-0.234.1rc0/covalent_ui/webapp/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/favicon.ico` & `covalent-0.234.1rc0/covalent_ui/webapp/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/favicon64x64.ico` & `covalent-0.234.1rc0/covalent_ui/webapp/build/favicon64x64.ico`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/index.html` & `covalent-0.234.1rc0/covalent_ui/webapp/build/index.html`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/logo192x192.png` & `covalent-0.234.1rc0/covalent_ui/webapp/build/logo192x192.png`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/logo512x512.png` & `covalent-0.234.1rc0/covalent_ui/webapp/build/logo512x512.png`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/logo64x64.png` & `covalent-0.234.1rc0/covalent_ui/webapp/build/logo64x64.png`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css.map` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/3.adb0c2e0.chunk.css.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css.map` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/css/main.0164e6d5.chunk.css.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.LICENSE.txt` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.map` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/2.07b8115b.chunk.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js.map` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/3.6e4b72b9.chunk.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js.map` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/4.2458d36c.chunk.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js.map` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/main.c54cebd5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js.map` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/js/runtime-main.561a5e8a.js.map`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/SettingsIcon.29d14b34.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/SettingsIcon.29d14b34.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/arg.71b4b335.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/arg.71b4b335.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/atom.3f8fd5bf.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/atom.3f8fd5bf.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/attribute.f1b86983.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/attribute.f1b86983.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/checkmark.a5e834e4.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/checkmark.a5e834e4.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/circuit-large.a0c113f8.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/circuit-large.a0c113f8.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/codeview.eb72cac6.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/codeview.eb72cac6.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/completing.e5f3aacb.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/completing.e5f3aacb.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/connectionLost.d1c47690.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/connectionLost.d1c47690.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/copy.4bbd1e1c.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/copy.4bbd1e1c.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/covalent-full-logo.0a6de0fd.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/covalent-full-logo.0a6de0fd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/covalent-logo-hover.87f421c8.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/covalent-logo-hover.87f421c8.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/covalent-logo.0a6de0fd.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/covalent-logo.0a6de0fd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/dashboard.4a7570e1.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/dashboard.4a7570e1.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/delete.73fac4cf.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/delete.73fac4cf.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/electron-dict.e471b060.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/electron-dict.e471b060.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/electron-list.e5beabe1.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/electron-list.e5beabe1.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/error.6508a515.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/error.6508a515.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/failed.31c046fd.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/failed.31c046fd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/failedTopBar.e4182945.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/failedTopBar.e4182945.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/filter.f9f7e173.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/filter.f9f7e173.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/fit-view.a6228772.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/fit-view.a6228772.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/fuction.f589c839.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/fuction.f589c839.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/generated.a2970d13.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/generated.a2970d13.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/info.f99828bd.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/info.f99828bd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/license.f61c24c7.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/license.f61c24c7.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/parameter.11d0a2e0.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/parameter.11d0a2e0.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/parameter.a62e78f9.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/parameter.a62e78f9.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/pending.1baceeef.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/pending.1baceeef.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/post-process.8092f778.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/post-process.8092f778.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/prettify.3bc46fc9.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/prettify.3bc46fc9.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/qelectron.ad89046a.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/qelectron.ad89046a.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/queued.0af4b56e.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/queued.0af4b56e.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/running.336c56e4.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/running.336c56e4.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/running.515f54a5.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/running.515f54a5.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/runningTopBar.bc8a86bd.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/runningTopBar.bc8a86bd.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/screenshot.ebc53482.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/screenshot.ebc53482.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/stop.f09b4e72.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/stop.f09b4e72.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/success.f693cbdc.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/success.f693cbdc.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/successTopBar.f280e5c7.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/successTopBar.f280e5c7.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/terminal.1d8a1548.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/terminal.1d8a1548.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/timeout.f67ccf19.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/timeout.f67ccf19.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/tree.2780601c.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/tree.2780601c.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/view.f326778a.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/view.f326778a.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/covalent_ui/webapp/build/static/media/warning.6bae5b45.svg` & `covalent-0.234.1rc0/covalent_ui/webapp/build/static/media/warning.6bae5b45.svg`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/pyproject.toml` & `covalent-0.234.1rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `covalent-0.234.0rc0/setup.py` & `covalent-0.234.1rc0/setup.py`

 * *Files identical despite different names*

