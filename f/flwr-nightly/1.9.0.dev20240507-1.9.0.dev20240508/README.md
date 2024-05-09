# Comparing `tmp/flwr_nightly-1.9.0.dev20240507.tar.gz` & `tmp/flwr_nightly-1.9.0.dev20240508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.9.0.dev20240507.tar", max compression
+gzip compressed data, was "flwr_nightly-1.9.0.dev20240508.tar", max compression
```

## Comparing `flwr_nightly-1.9.0.dev20240507.tar` & `flwr_nightly-1.9.0.dev20240508.tar`

### file list

```diff
@@ -1,222 +1,226 @@
--rw-r--r--   0        0        0    11358 2024-05-07 23:05:14.141739 flwr_nightly-1.9.0.dev20240507/LICENSE
--rw-r--r--   0        0        0    12915 2024-05-07 23:05:14.141739 flwr_nightly-1.9.0.dev20240507/README.md
--rw-r--r--   0        0        0     5812 2024-05-07 23:05:26.261728 flwr_nightly-1.9.0.dev20240507/pyproject.toml
--rw-r--r--   0        0        0      937 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1141 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     5106 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/build.py
--rw-r--r--   0        0        0     4899 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/config_utils.py
--rw-r--r--   0        0        0     2215 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0      789 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     6098 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0     3078 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/.gitignore.tpl
--rw-r--r--   0        0        0      668 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0     2113 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl
--rw-r--r--   0        0        0      521 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1172 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0     2801 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
--rw-r--r--   0        0        0     1280 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      272 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/server.mlx.py.tpl
--rw-r--r--   0        0        0      248 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      593 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0      341 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
--rw-r--r--   0        0        0      579 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     2598 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl
--rw-r--r--   0        0        0     3684 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0     1044 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl
--rw-r--r--   0        0        0      585 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl
--rw-r--r--   0        0        0      523 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      592 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      572 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
--rw-r--r--   0        0        0      571 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0      789 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2334 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     4119 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1268 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    22313 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8636 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8993 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     4903 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/grpc_rere_client/client_interceptor.py
--rw-r--r--   0        0        0     9597 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0     2404 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/heartbeat.py
--rw-r--r--   0        0        0      719 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5415 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2623 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     5012 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-05-07 23:05:14.557738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    11520 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0      865 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/supernode/__init__.py
--rw-r--r--   0        0        0     9052 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/supernode/app.py
--rw-r--r--   0        0        0     1006 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     2424 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2460 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     7107 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    13896 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4838 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     5056 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    13798 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    11707 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     4707 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7865 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3207 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     5016 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     5018 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     9161 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0    10605 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2811 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-07 23:05:14.561738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1785 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    28600 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     5287 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3468 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     5444 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      862 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     5090 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0    11832 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/driver/grpc_driver.py
--rw-r--r--   0        0        0     5121 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5972 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17664 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4402 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17502 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12949 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4796 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-05-07 23:05:14.565738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11932 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3387 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0     7691 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py
--rw-r--r--   0        0        0      731 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3622 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     7621 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6386 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    12455 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0    12750 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    28528 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     7989 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0     2207 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/state/utils.py
--rw-r--r--   0        0        0      913 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    12547 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29038 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1348 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    14380 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    19367 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    15956 2024-05-07 23:05:14.569738 flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15302 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240507/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-08 23:05:23.285217 flwr_nightly-1.9.0.dev20240508/LICENSE
+-rw-r--r--   0        0        0    12915 2024-05-08 23:05:23.285217 flwr_nightly-1.9.0.dev20240508/README.md
+-rw-r--r--   0        0        0     5812 2024-05-08 23:05:37.249258 flwr_nightly-1.9.0.dev20240508/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1141 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     5106 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/build.py
+-rw-r--r--   0        0        0     4899 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/config_utils.py
+-rw-r--r--   0        0        0     2215 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0      789 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     6168 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0     3078 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/.gitignore.tpl
+-rw-r--r--   0        0        0      668 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0     1450 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/client.hf.py.tpl
+-rw-r--r--   0        0        0     2113 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl
+-rw-r--r--   0        0        0      521 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1172 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0     2801 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
+-rw-r--r--   0        0        0     1280 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      338 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/server.hf.py.tpl
+-rw-r--r--   0        0        0      272 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/server.mlx.py.tpl
+-rw-r--r--   0        0        0      248 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      593 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0      341 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
+-rw-r--r--   0        0        0      579 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     2857 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/task.hf.py.tpl
+-rw-r--r--   0        0        0     2598 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl
+-rw-r--r--   0        0        0     3684 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0     1044 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl
+-rw-r--r--   0        0        0      676 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/pyproject.hf.toml.tpl
+-rw-r--r--   0        0        0      585 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl
+-rw-r--r--   0        0        0      523 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      592 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      572 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
+-rw-r--r--   0        0        0      571 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0      789 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2334 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     4119 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1268 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    22313 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8993 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     4903 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/grpc_rere_client/client_interceptor.py
+-rw-r--r--   0        0        0     9597 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2404 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-05-08 23:05:23.701218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5415 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2623 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     5012 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    11520 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0      865 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/supernode/__init__.py
+-rw-r--r--   0        0        0     9052 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/supernode/app.py
+-rw-r--r--   0        0        0     1006 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2460 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     7107 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    13896 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4838 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     5056 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    13798 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11707 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     4707 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7865 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3207 2024-05-08 23:05:23.705218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     5016 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5018 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     9161 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0    10605 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2811 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1716 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    28913 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     3421 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3468 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     5444 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      862 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     5090 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0    11832 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     5063 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5972 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17563 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17502 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12949 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-05-08 23:05:23.709218 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4796 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11932 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3387 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0     7691 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py
+-rw-r--r--   0        0        0      731 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3622 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     7621 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6550 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12455 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0    12750 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    28528 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     7989 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    12547 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1348 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    14380 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    16006 2024-05-08 23:05:23.713219 flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15302 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240508/PKG-INFO
```

### Comparing `flwr_nightly-1.9.0.dev20240507/LICENSE` & `flwr_nightly-1.9.0.dev20240508/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/README.md` & `flwr_nightly-1.9.0.dev20240508/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/pyproject.toml` & `flwr_nightly-1.9.0.dev20240508/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.9.0.dev20240507"
+version = "1.9.0.dev20240508"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
```

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/app.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/build.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/build.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/config_utils.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/example.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/new.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 class MlFramework(str, Enum):
     """Available frameworks."""
 
     NUMPY = "NumPy"
     PYTORCH = "PyTorch"
     TENSORFLOW = "TensorFlow"
+    HUGGINGFACE = "HF"
     MLX = "MLX"
     SKLEARN = "sklearn"
 
 
 class TemplateNotFound(Exception):
     """Raised when template does not exist."""
 
@@ -150,14 +151,15 @@
             "template": f"app/code/client.{framework_str}.py.tpl"
         },
     }
 
     # Depending on the framework, generate task.py file
     frameworks_with_tasks = [
         MlFramework.PYTORCH.value.lower(),
+        MlFramework.HUGGINGFACE.value.lower(),
         MlFramework.MLX.value.lower(),
         MlFramework.TENSORFLOW.value.lower(),
     ]
     if framework_str in frameworks_with_tasks:
         files[f"{import_name}/task.py"] = {
             "template": f"app/code/task.{framework_str}.py.tpl"
         }
```

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/.gitignore.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/.gitignore.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/run/run.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/cli/utils.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/cli/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/app.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/client.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/client_app.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/client_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/grpc_rere_client/client_interceptor.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/grpc_rere_client/client_interceptor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/heartbeat.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/heartbeat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/localdp_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/node_state.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/supernode/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/supernode/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/supernode/app.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/supernode/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/client/typing.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/address.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/constant.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/context.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/date.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/dp.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/grpc.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/logger.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/message.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/message.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/parameter.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/recordset.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/recordset_compat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/retry_invoker.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/serde.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/typing.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/common/version.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from .app import run_driver_api as run_driver_api
 from .app import run_fleet_api as run_fleet_api
 from .app import run_superlink as run_superlink
 from .app import start_server as start_server
 from .client_manager import ClientManager as ClientManager
 from .client_manager import SimpleClientManager as SimpleClientManager
 from .compat import LegacyContext as LegacyContext
-from .compat import start_driver as start_driver
 from .driver import Driver as Driver
 from .history import History as History
 from .run_serverapp import run_server_app as run_server_app
 from .server import Server as Server
 from .server_app import ServerApp as ServerApp
 from .server_config import ServerConfig as ServerConfig
 
@@ -41,12 +40,11 @@
     "run_fleet_api",
     "run_server_app",
     "run_superlink",
     "Server",
     "ServerApp",
     "ServerConfig",
     "SimpleClientManager",
-    "start_driver",
     "start_server",
     "strategy",
     "workflow",
 ]
```

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/app.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from flwr.common.constant import (
     MISSING_EXTRA_REST,
     TRANSPORT_TYPE_GRPC_RERE,
     TRANSPORT_TYPE_REST,
     TRANSPORT_TYPE_VCE,
 )
 from flwr.common.exit_handlers import register_exit_handlers
-from flwr.common.logger import log
+from flwr.common.logger import log, warn_deprecated_feature
 from flwr.common.secure_aggregation.crypto.symmetric_encryption import (
     private_key_to_bytes,
     public_key_to_bytes,
     ssh_types_to_elliptic_curve,
 )
 from flwr.proto.fleet_pb2_grpc import (  # pylint: disable=E0611
     add_FleetServicer_to_server,
@@ -192,14 +192,17 @@
 
     return hist
 
 
 def run_driver_api() -> None:
     """Run Flower server (Driver API)."""
     log(INFO, "Starting Flower server (Driver API)")
+    # Running `flower-driver-api` is deprecated
+    warn_deprecated_feature("flower-driver-api")
+    log(WARN, "Use `flower-superlink` instead")
     event(EventType.RUN_DRIVER_API_ENTER)
     args = _parse_args_run_driver_api().parse_args()
 
     # Parse IP address
     parsed_address = parse_address(args.driver_api_address)
     if not parsed_address:
         sys.exit(f"Driver IP address ({args.driver_api_address}) cannot be parsed.")
@@ -229,14 +232,17 @@
     # Block
     grpc_server.wait_for_termination()
 
 
 def run_fleet_api() -> None:
     """Run Flower server (Fleet API)."""
     log(INFO, "Starting Flower server (Fleet API)")
+    # Running `flower-fleet-api` is deprecated
+    warn_deprecated_feature("flower-fleet-api")
+    log(WARN, "Use `flower-superlink` instead")
     event(EventType.RUN_FLEET_API_ENTER)
     args = _parse_args_run_fleet_api().parse_args()
 
     # Obtain certificates
     certificates = _try_obtain_certificates(args)
 
     # Initialize StateFactory
```

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/compat/app_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/criterion.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/driver/grpc_driver.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/driver/grpc_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/history.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/history.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,39 +87,39 @@
         Returns
         -------
         representation : str
             The string representation of the history object.
         """
         rep = ""
         if self.losses_distributed:
-            rep += "History (loss, distributed):\n" + pprint.pformat(
-                reduce(
-                    lambda a, b: a + b,
-                    [
-                        f"\tround {server_round}: {loss}\n"
-                        for server_round, loss in self.losses_distributed
-                    ],
-                )
+            rep += "History (loss, distributed):\n" + reduce(
+                lambda a, b: a + b,
+                [
+                    f"\tround {server_round}: {loss}\n"
+                    for server_round, loss in self.losses_distributed
+                ],
             )
         if self.losses_centralized:
-            rep += "History (loss, centralized):\n" + pprint.pformat(
-                reduce(
-                    lambda a, b: a + b,
-                    [
-                        f"\tround {server_round}: {loss}\n"
-                        for server_round, loss in self.losses_centralized
-                    ],
-                )
+            rep += "History (loss, centralized):\n" + reduce(
+                lambda a, b: a + b,
+                [
+                    f"\tround {server_round}: {loss}\n"
+                    for server_round, loss in self.losses_centralized
+                ],
             )
         if self.metrics_distributed_fit:
-            rep += "History (metrics, distributed, fit):\n" + pprint.pformat(
-                self.metrics_distributed_fit
+            rep += (
+                "History (metrics, distributed, fit):\n"
+                + pprint.pformat(self.metrics_distributed_fit)
+                + "\n"
             )
         if self.metrics_distributed:
-            rep += "History (metrics, distributed, evaluate):\n" + pprint.pformat(
-                self.metrics_distributed
+            rep += (
+                "History (metrics, distributed, evaluate):\n"
+                + pprint.pformat(self.metrics_distributed)
+                + "\n"
             )
         if self.metrics_centralized:
             rep += "History (metrics, centralized):\n" + pprint.pformat(
                 self.metrics_centralized
             )
         return rep
```

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/run_serverapp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/server.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -483,18 +483,15 @@
     hist, elapsed_time = server.fit(
         num_rounds=config.num_rounds, timeout=config.round_timeout
     )
 
     log(INFO, "")
     log(INFO, "[SUMMARY]")
     log(INFO, "Run finished %s rounds in %.2fs", config.num_rounds, elapsed_time)
-    for idx, line in enumerate(io.StringIO(str(hist))):
-        if idx == 0:
-            log(INFO, "%s", line.strip("\n"))
-        else:
-            log(INFO, "\t%s", line.strip("\n"))
+    for line in io.StringIO(str(hist)):
+        log(INFO, "\t%s", line.strip("\n"))
     log(INFO, "")
 
     # Graceful shutdown
     server.disconnect_all_clients(timeout=config.round_timeout)
 
     return hist
```

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/server_app.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/server_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/server_config.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Ray backend for the Fleet API using the Simulation Engine."""
 
 import pathlib
-from logging import DEBUG, ERROR, INFO
+from logging import DEBUG, ERROR, INFO, WARNING
 from typing import Callable, Dict, List, Tuple, Union
 
 import ray
 
 from flwr.client.client_app import ClientApp
 from flwr.common.context import Context
 from flwr.common.logger import log
@@ -51,15 +51,18 @@
         if not pathlib.Path(work_dir).exists():
             raise ValueError(f"Specified work_dir {work_dir} does not exist.")
 
         # Init ray and append working dir if needed
         runtime_env = (
             self._configure_runtime_env(work_dir=work_dir) if work_dir else None
         )
-        init_ray(runtime_env=runtime_env)
+        if backend_config.get("silent", False):
+            init_ray(logging_level=WARNING, log_to_driver=True, runtime_env=runtime_env)
+        else:
+            init_ray(runtime_env=runtime_env)
 
         # Validate client resources
         self.client_resources_key = "client_resources"
 
         # Create actor pool
         use_tf = backend_config.get("tensorflow", False)
         actor_kwargs = {"on_actor_init_fn": enable_tf_gpu_growth} if use_tf else {}
```

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/superlink/state/utils.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/superlink/state/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/typing.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/workflow/default_workflows.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/app.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240507/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.9.0.dev20240508/src/py/flwr/simulation/run_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,21 +313,23 @@
         all GPU memory. Read mor about how `tf.config.experimental.set_memory_growth()`
         works in the TensorFlow documentation: https://www.tensorflow.org/api/stable.
 
     verbose_logging : bool (default: False)
         When diabled, only INFO, WARNING and ERROR log messages will be shown. If
         enabled, DEBUG-level logs will be displayed.
     """
+    if backend_config is None:
+        backend_config = {}
+
     # Set logging level
     logger = logging.getLogger("flwr")
     if verbose_logging:
         update_console_handler(level=DEBUG, timestamps=True, colored=True)
-
-    if backend_config is None:
-        backend_config = {}
+    else:
+        backend_config["silent"] = True
 
     if enable_tf_gpu_growth:
         # Check that Backend config has also enabled using GPU growth
         use_tf = backend_config.get("tensorflow", False)
         if not use_tf:
             log(WARNING, "Enabling GPU growth for your backend.")
             backend_config["tensorflow"] = True
```

### Comparing `flwr_nightly-1.9.0.dev20240507/PKG-INFO` & `flwr_nightly-1.9.0.dev20240508/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.9.0.dev20240507
+Version: 1.9.0.dev20240508
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.ai
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.ai
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240507 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240508 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

