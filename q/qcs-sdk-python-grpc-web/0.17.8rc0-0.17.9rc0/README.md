# Comparing `tmp/qcs_sdk_python_grpc_web-0.17.8rc0.tar.gz` & `tmp/qcs_sdk_python_grpc_web-0.17.9rc0.tar.gz`

## Comparing `qcs_sdk_python_grpc_web-0.17.8rc0.tar` & `qcs_sdk_python_grpc_web-0.17.9rc0.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0     1001      127     2496 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/Cargo.toml
--rw-r--r--   0     1001      127    44997 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/CHANGELOG.md
--rw-r--r--   0     1001      127      752 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/Makefile.toml
--rw-r--r--   0     1001      127     2186 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/README.md
--rw-r--r--   0     1001      127       95 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/build.rs
--rw-r--r--   0     1001      127      931 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/delayed_job_retrieval.rs
--rw-r--r--   0     1001      127     1770 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/execute.rs
--rw-r--r--   0     1001      127      674 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/libquil.rs
--rw-r--r--   0     1001      127      767 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/local.rs
--rw-r--r--   0     1001      127     2154 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/parametric_compilation.rs
--rw-r--r--   0     1001      127     1277 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/quil_t.rs
--rw-r--r--   0     1001      127      126 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/bin/diagnostics.rs
--rw-r--r--   0     1001      127     5479 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/client.rs
--rw-r--r--   0     1001      127     8277 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/edge.rs
--rw-r--r--   0     1001      127     6791 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/mod.rs
--rw-r--r--   0     1001      127     8320 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/operator.rs
--rw-r--r--   0     1001      127    13686 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/qubit.rs
--rw-r--r--   0     1001      127    11548 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/libquil.rs
--rw-r--r--   0     1001      127      198 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/mod.rs
--rw-r--r--   0     1001      127    16466 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/quilc.rs
--rw-r--r--   0     1001      127    11529 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/rpcq.rs
--rw-r--r--   0     1001      127     8271 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/diagnostics.rs
--rw-r--r--   0     1001      127    36127 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/executable.rs
--rw-r--r--   0     1001      127    23212 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/execution_data.rs
--rw-r--r--   0     1001      127     1984 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/lib.rs
--rw-r--r--   0     1001      127    25522 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/api.rs
--rw-r--r--   0     1001      127    12027 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/execution.rs
--rw-r--r--   0     1001      127     3187 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/mod.rs
--rw-r--r--   0     1001      127     6058 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/result_data.rs
--rw-r--r--   0     1001      127    17418 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/rewrite_arithmetic.rs
--rw-r--r--   0     1001      127      137 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_allocates_for_multiple_expressions-2.snap
--rw-r--r--   0     1001      127      131 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_allocates_for_multiple_expressions.snap
--rw-r--r--   0     1001      127      112 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_frequency_expressions-2.snap
--rw-r--r--   0     1001      127      119 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_frequency_expressions.snap
--rw-r--r--   0     1001      127      127 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_phases.snap
--rw-r--r--   0     1001      127      111 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_set_scale_units.snap
--rw-r--r--   0     1001      127      134 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_substitutes_and_reuses_gate_expressions.snap
--rw-r--r--   0     1001      127      127 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_substitutes_gate_parameters.snap
--rw-r--r--   0     1001      127     9322 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/translation.rs
--rw-r--r--   0     1001      127     4292 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/execution.rs
--rw-r--r--   0     1001      127    13970 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/http.rs
--rw-r--r--   0     1001      127     6966 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/libquil.rs
--rw-r--r--   0     1001      127    11138 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/mod.rs
--rw-r--r--   0     1001      127      154 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/snapshots/qcs__qvm__test__apply_valid_parameters_to_program.snap
--rw-r--r--   0     1001      127     1938 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/register_data.rs
--rw-r--r--   0     1001      127   104426 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/aspen_9_isa.json
--rw-r--r--   0     1001      127     1921 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/basic_qvm.rs
--rw-r--r--   0     1001      127      558 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/bell_state_response_data.hex
--rw-r--r--   0     1001      127    81629 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/compiler-isa-Aspen-8.json
--rw-r--r--   0     1001      127    14144 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/mocked_qpu.rs
--rw-r--r--   0     1001      127     2071 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/parametric_compilation.rs
--rw-r--r--   0     1001      127    71490 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/qcs-isa-Aspen-8.json
--rw-r--r--   0     1001      127     3933 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/qvm_api.rs
--rw-r--r--   0     1001      127     2275 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/qvm_isa.json
--rw-r--r--   0     1001      127      148 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/secrets.toml
--rw-r--r--   0     1001      127      298 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/settings.toml
--rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/Cargo.toml
--rw-r--r--   0     1001      127      203 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/.flake8
--rw-r--r--   0     1001      127       64 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/.stubtest-allowlist
--rw-r--r--   0     1001      127    46591 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/CHANGELOG.md
--rw-r--r--   0     1001      127     1332 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/Makefile.toml
--rw-r--r--   0     1001      127     3674 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/README.md
--rw-r--r--   0     1001      127       71 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/build.rs
--rw-r--r--   0     1001      127    34757 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/poetry.lock
--rw-r--r--   0     1001      127      257 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/__init__.py
--rw-r--r--   0     1001      127    17080 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/__init__.pyi
--rw-r--r--   0     1001      127       29 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/client.py
--rw-r--r--   0     1001      127     4116 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/client.pyi
--rw-r--r--   0     1001      127      100 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/compiler/__init__.py
--rw-r--r--   0     1001      127      299 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/compiler/__init__.pyi
--rw-r--r--   0     1001      127    11882 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/compiler/quilc.pyi
--rw-r--r--   0     1001      127      736 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/diagnostics.py
--rw-r--r--   0     1001      127        0 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/py.typed
--rw-r--r--   0     1001      127       85 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/__init__.py
--rw-r--r--   0     1001      127     7954 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/__init__.pyi
--rw-r--r--   0     1001      127    21174 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/api.pyi
--rw-r--r--   0     1001      127    12322 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/isa.pyi
--rw-r--r--   0     1001      127     1884 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/rewrite_arithmetic.pyi
--rw-r--r--   0     1001      127     5935 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/translation.pyi
--rw-r--r--   0     1001      127       85 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qvm/__init__.py
--rw-r--r--   0     1001      127     5671 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qvm/__init__.pyi
--rw-r--r--   0     1001      127     9537 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qvm/api.pyi
--rw-r--r--   0     1001      127     1113 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/scripts/patch_grpc_web.py
--rw-r--r--   0     1001      127     6001 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/client.rs
--rw-r--r--   0     1001      127      149 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/compiler/mod.rs
--rw-r--r--   0     1001      127    12242 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/compiler/quilc.rs
--rw-r--r--   0     1001      127    10280 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/executable.rs
--rw-r--r--   0     1001      127    10202 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/execution_data.rs
--rw-r--r--   0     1001      127      637 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/from_py.rs
--rw-r--r--   0     1001      127       16 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/grpc/mod.rs
--rw-r--r--   0     1001      127     1988 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/grpc/models/controller.rs
--rw-r--r--   0     1001      127       20 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/grpc/models/mod.rs
--rw-r--r--   0     1001      127     2064 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/lib.rs
--rw-r--r--   0     1001      127     4303 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/py_sync.rs
--rw-r--r--   0     1001      127    17827 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/api.rs
--rw-r--r--   0     1001      127     4501 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/isa.rs
--rw-r--r--   0     1001      127     1762 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/mod.rs
--rw-r--r--   0     1001      127     4554 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/result_data.rs
--rw-r--r--   0     1001      127     4560 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/rewrite_arithmetic.rs
--rw-r--r--   0     1001      127     6203 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/translation.rs
--rw-r--r--   0     1001      127     8832 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qvm/api.rs
--rw-r--r--   0     1001      127     8478 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qvm/mod.rs
--rw-r--r--   0     1001      127     1248 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/register_data.rs
--rw-r--r--   0     1001      127   410675 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_fixtures/aspen-m-3.json
--rw-r--r--   0     1001      127     7302 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_fixtures/device-2q.json
--rw-r--r--   0     1001      127      190 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_qcs_config/secrets.toml
--rw-r--r--   0     1001      127      605 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_qcs_config/settings.toml
--rw-r--r--   0     1001      127     1212 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/compiler/__snapshots__/test_quilc.ambr
--rw-r--r--   0     1001      127     4818 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/compiler/test_quilc.py
--rw-r--r--   0     1001      127     3233 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/conftest.py
--rw-r--r--   0     1001      127     5219 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/execution_data/test_execution_data.py
--rw-r--r--   0     1001      127     1384 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_api.py
--rw-r--r--   0     1001      127     1096 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_isa.py
--rw-r--r--   0     1001      127     2124 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_qpu.py
--rw-r--r--   0     1001      127      823 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_rewrite_arithmetic.py
--rw-r--r--   0     1001      127     1704 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_translation.py
--rw-r--r--   0     1001      127      301 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qvm/test_qvm.py
--rw-r--r--   0     1001      127     2410 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/test_client.py
--rw-r--r--   0     1001      127      154 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/test_diagnostics.py
--rw-r--r--   0     1001      127     1637 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/test_executable.py
--rw-r--r--   0     1001      127      162 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/test_logging.py
--rw-r--r--   0     1001      127   100372 2024-04-24 19:33:43.000000 qcs_sdk_python_grpc_web-0.17.8rc0/Cargo.lock
--rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.8rc0/Cargo.toml
--rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.8rc0/pyproject.toml
--rw-r--r--   0     1001      127       85 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qvm/__init__.py
--rw-r--r--   0     1001      127     9537 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qvm/api.pyi
--rw-r--r--   0     1001      127     5671 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qvm/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/py.typed
--rw-r--r--   0     1001      127      736 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/diagnostics.py
--rw-r--r--   0     1001      127       29 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/client.py
--rw-r--r--   0     1001      127      100 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/compiler/__init__.py
--rw-r--r--   0     1001      127      299 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/compiler/__init__.pyi
--rw-r--r--   0     1001      127    11882 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/compiler/quilc.pyi
--rw-r--r--   0     1001      127      257 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/__init__.py
--rw-r--r--   0     1001      127     5935 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/translation.pyi
--rw-r--r--   0     1001      127    12322 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/isa.pyi
--rw-r--r--   0     1001      127       85 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/__init__.py
--rw-r--r--   0     1001      127    21174 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/api.pyi
--rw-r--r--   0     1001      127     7954 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/__init__.pyi
--rw-r--r--   0     1001      127     1884 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/rewrite_arithmetic.pyi
--rw-r--r--   0     1001      127    17080 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/__init__.pyi
--rw-r--r--   0     1001      127     4116 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/client.pyi
--rw-r--r--   0     1001      127     3674 2024-04-24 19:33:31.000000 qcs_sdk_python_grpc_web-0.17.8rc0/README.md
--rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.8rc0/PKG-INFO
+-rw-r--r--   0     1001      127     2496 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/Cargo.toml
+-rw-r--r--   0     1001      127    45140 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/CHANGELOG.md
+-rw-r--r--   0     1001      127      752 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/Makefile.toml
+-rw-r--r--   0     1001      127     2186 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/README.md
+-rw-r--r--   0     1001      127       95 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/build.rs
+-rw-r--r--   0     1001      127      931 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/examples/delayed_job_retrieval.rs
+-rw-r--r--   0     1001      127     1770 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/examples/execute.rs
+-rw-r--r--   0     1001      127      674 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/examples/libquil.rs
+-rw-r--r--   0     1001      127      767 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/examples/local.rs
+-rw-r--r--   0     1001      127     2154 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/examples/parametric_compilation.rs
+-rw-r--r--   0     1001      127     1277 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/examples/quil_t.rs
+-rw-r--r--   0     1001      127      126 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/bin/diagnostics.rs
+-rw-r--r--   0     1001      127     5479 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/client.rs
+-rw-r--r--   0     1001      127     8277 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/isa/edge.rs
+-rw-r--r--   0     1001      127     6791 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/isa/mod.rs
+-rw-r--r--   0     1001      127     8320 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/isa/operator.rs
+-rw-r--r--   0     1001      127    13686 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/isa/qubit.rs
+-rw-r--r--   0     1001      127    11548 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/libquil.rs
+-rw-r--r--   0     1001      127      198 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/mod.rs
+-rw-r--r--   0     1001      127    16449 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/quilc.rs
+-rw-r--r--   0     1001      127    11529 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/rpcq.rs
+-rw-r--r--   0     1001      127     8271 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/diagnostics.rs
+-rw-r--r--   0     1001      127    36127 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/executable.rs
+-rw-r--r--   0     1001      127    23212 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/execution_data.rs
+-rw-r--r--   0     1001      127     1984 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/lib.rs
+-rw-r--r--   0     1001      127    25525 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/api.rs
+-rw-r--r--   0     1001      127    12027 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/execution.rs
+-rw-r--r--   0     1001      127     3187 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/mod.rs
+-rw-r--r--   0     1001      127     6058 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/result_data.rs
+-rw-r--r--   0     1001      127    17418 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/rewrite_arithmetic.rs
+-rw-r--r--   0     1001      127      137 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_allocates_for_multiple_expressions-2.snap
+-rw-r--r--   0     1001      127      131 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_allocates_for_multiple_expressions.snap
+-rw-r--r--   0     1001      127      112 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_frequency_expressions-2.snap
+-rw-r--r--   0     1001      127      119 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_frequency_expressions.snap
+-rw-r--r--   0     1001      127      127 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_phases.snap
+-rw-r--r--   0     1001      127      111 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_converts_set_scale_units.snap
+-rw-r--r--   0     1001      127      134 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_substitutes_and_reuses_gate_expressions.snap
+-rw-r--r--   0     1001      127      127 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/snapshots/qcs__qpu__rewrite_arithmetic__describe_rewrite_arithmetic__it_substitutes_gate_parameters.snap
+-rw-r--r--   0     1001      127     9322 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/translation.rs
+-rw-r--r--   0     1001      127     4292 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qvm/execution.rs
+-rw-r--r--   0     1001      127    13970 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qvm/http.rs
+-rw-r--r--   0     1001      127     6966 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qvm/libquil.rs
+-rw-r--r--   0     1001      127    11138 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qvm/mod.rs
+-rw-r--r--   0     1001      127      154 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qvm/snapshots/qcs__qvm__test__apply_valid_parameters_to_program.snap
+-rw-r--r--   0     1001      127     1938 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/register_data.rs
+-rw-r--r--   0     1001      127   104426 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/aspen_9_isa.json
+-rw-r--r--   0     1001      127     1921 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/basic_qvm.rs
+-rw-r--r--   0     1001      127      558 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/bell_state_response_data.hex
+-rw-r--r--   0     1001      127    81629 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/compiler-isa-Aspen-8.json
+-rw-r--r--   0     1001      127    14144 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/mocked_qpu.rs
+-rw-r--r--   0     1001      127     2071 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/parametric_compilation.rs
+-rw-r--r--   0     1001      127    71490 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/qcs-isa-Aspen-8.json
+-rw-r--r--   0     1001      127     3933 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/qvm_api.rs
+-rw-r--r--   0     1001      127     2275 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/qvm_isa.json
+-rw-r--r--   0     1001      127      148 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/secrets.toml
+-rw-r--r--   0     1001      127      298 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/settings.toml
+-rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/Cargo.toml
+-rw-r--r--   0     1001      127      203 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/.flake8
+-rw-r--r--   0     1001      127       64 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/.stubtest-allowlist
+-rw-r--r--   0     1001      127    46734 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/CHANGELOG.md
+-rw-r--r--   0     1001      127     1332 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/Makefile.toml
+-rw-r--r--   0     1001      127     3674 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/README.md
+-rw-r--r--   0     1001      127       71 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/build.rs
+-rw-r--r--   0     1001      127    34757 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/poetry.lock
+-rw-r--r--   0     1001      127      257 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/__init__.py
+-rw-r--r--   0     1001      127    17080 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/__init__.pyi
+-rw-r--r--   0     1001      127       29 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/client.py
+-rw-r--r--   0     1001      127     4116 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/client.pyi
+-rw-r--r--   0     1001      127      100 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/compiler/__init__.py
+-rw-r--r--   0     1001      127      299 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/compiler/__init__.pyi
+-rw-r--r--   0     1001      127    11882 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/compiler/quilc.pyi
+-rw-r--r--   0     1001      127      736 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/diagnostics.py
+-rw-r--r--   0     1001      127        0 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/py.typed
+-rw-r--r--   0     1001      127       85 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qpu/__init__.py
+-rw-r--r--   0     1001      127     7954 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qpu/__init__.pyi
+-rw-r--r--   0     1001      127    21174 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qpu/api.pyi
+-rw-r--r--   0     1001      127    12322 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qpu/isa.pyi
+-rw-r--r--   0     1001      127     1884 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qpu/rewrite_arithmetic.pyi
+-rw-r--r--   0     1001      127     5935 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qpu/translation.pyi
+-rw-r--r--   0     1001      127       85 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qvm/__init__.py
+-rw-r--r--   0     1001      127     5671 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qvm/__init__.pyi
+-rw-r--r--   0     1001      127     9537 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qvm/api.pyi
+-rw-r--r--   0     1001      127     1113 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/scripts/patch_grpc_web.py
+-rw-r--r--   0     1001      127     6001 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/client.rs
+-rw-r--r--   0     1001      127      149 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/compiler/mod.rs
+-rw-r--r--   0     1001      127    12242 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/compiler/quilc.rs
+-rw-r--r--   0     1001      127    10280 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/executable.rs
+-rw-r--r--   0     1001      127    10202 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/execution_data.rs
+-rw-r--r--   0     1001      127      637 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/from_py.rs
+-rw-r--r--   0     1001      127       16 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     1988 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/grpc/models/controller.rs
+-rw-r--r--   0     1001      127       20 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/grpc/models/mod.rs
+-rw-r--r--   0     1001      127     2064 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/lib.rs
+-rw-r--r--   0     1001      127     4303 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/py_sync.rs
+-rw-r--r--   0     1001      127    17827 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qpu/api.rs
+-rw-r--r--   0     1001      127     4501 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qpu/isa.rs
+-rw-r--r--   0     1001      127     1762 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qpu/mod.rs
+-rw-r--r--   0     1001      127     4554 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qpu/result_data.rs
+-rw-r--r--   0     1001      127     4560 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qpu/rewrite_arithmetic.rs
+-rw-r--r--   0     1001      127     6203 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qpu/translation.rs
+-rw-r--r--   0     1001      127     8832 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qvm/api.rs
+-rw-r--r--   0     1001      127     8478 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qvm/mod.rs
+-rw-r--r--   0     1001      127     1248 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/register_data.rs
+-rw-r--r--   0     1001      127   410675 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/_fixtures/aspen-m-3.json
+-rw-r--r--   0     1001      127     7302 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/_fixtures/device-2q.json
+-rw-r--r--   0     1001      127      190 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/_qcs_config/secrets.toml
+-rw-r--r--   0     1001      127      605 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/_qcs_config/settings.toml
+-rw-r--r--   0     1001      127     1212 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/compiler/__snapshots__/test_quilc.ambr
+-rw-r--r--   0     1001      127     4818 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/compiler/test_quilc.py
+-rw-r--r--   0     1001      127     3233 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/conftest.py
+-rw-r--r--   0     1001      127     5219 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/execution_data/test_execution_data.py
+-rw-r--r--   0     1001      127     1384 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/qpu/test_api.py
+-rw-r--r--   0     1001      127     1096 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/qpu/test_isa.py
+-rw-r--r--   0     1001      127     2124 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/qpu/test_qpu.py
+-rw-r--r--   0     1001      127      823 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/qpu/test_rewrite_arithmetic.py
+-rw-r--r--   0     1001      127     1704 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/qpu/test_translation.py
+-rw-r--r--   0     1001      127      301 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/qvm/test_qvm.py
+-rw-r--r--   0     1001      127     2410 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/test_client.py
+-rw-r--r--   0     1001      127      154 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/test_diagnostics.py
+-rw-r--r--   0     1001      127     1637 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/test_executable.py
+-rw-r--r--   0     1001      127      162 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/test_logging.py
+-rw-r--r--   0     1001      127   101369 2024-05-09 23:53:05.000000 qcs_sdk_python_grpc_web-0.17.9rc0/Cargo.lock
+-rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.9rc0/Cargo.toml
+-rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.9rc0/pyproject.toml
+-rw-r--r--   0     1001      127       85 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qvm/__init__.py
+-rw-r--r--   0     1001      127     9537 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qvm/api.pyi
+-rw-r--r--   0     1001      127     5671 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qvm/__init__.pyi
+-rw-r--r--   0     1001      127        0 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/py.typed
+-rw-r--r--   0     1001      127      736 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/diagnostics.py
+-rw-r--r--   0     1001      127       29 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/client.py
+-rw-r--r--   0     1001      127      100 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/compiler/__init__.py
+-rw-r--r--   0     1001      127      299 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/compiler/__init__.pyi
+-rw-r--r--   0     1001      127    11882 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/compiler/quilc.pyi
+-rw-r--r--   0     1001      127      257 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/__init__.py
+-rw-r--r--   0     1001      127     5935 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qpu/translation.pyi
+-rw-r--r--   0     1001      127    12322 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qpu/isa.pyi
+-rw-r--r--   0     1001      127       85 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qpu/__init__.py
+-rw-r--r--   0     1001      127    21174 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qpu/api.pyi
+-rw-r--r--   0     1001      127     7954 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qpu/__init__.pyi
+-rw-r--r--   0     1001      127     1884 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qpu/rewrite_arithmetic.pyi
+-rw-r--r--   0     1001      127    17080 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/__init__.pyi
+-rw-r--r--   0     1001      127     4116 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/client.pyi
+-rw-r--r--   0     1001      127     3674 2024-05-09 23:52:45.000000 qcs_sdk_python_grpc_web-0.17.9rc0/README.md
+-rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 qcs_sdk_python_grpc_web-0.17.9rc0/PKG-INFO
```

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/Cargo.toml` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "qcs"
 description = "High level interface for running Quil on a QPU"
-version = "0.21.8-rc.0"
+version = "0.21.9-rc.0"
 edition = "2018"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/qcs-sdk-rust"
 keywords = ["pyquil", "SDK", "Rigetti", "Quil", "Quantum"]
 categories = ["api-bindings", "compilers", "science", "emulators"]
 readme = "./README.md"
```

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/CHANGELOG.md` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## 0.21.9-rc.0
+
+### Fixes
+
+- Refresh JWT only when expired, not before every request (#470)
+
+## 0.21.8
+
+### Features
+
+- Update quil-rs (#464)
+
 ## 0.21.8-rc.0
 
 ### Features
 
 - Update quil-rs (#464)
 
 ## 0.21.7
```

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/Makefile.toml` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/Makefile.toml`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/README.md` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/README.md`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/delayed_job_retrieval.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/examples/delayed_job_retrieval.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/execute.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/examples/execute.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/libquil.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/examples/libquil.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/local.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/examples/local.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/parametric_compilation.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/examples/parametric_compilation.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/examples/quil_t.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/examples/quil_t.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/client.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/client.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/edge.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/isa/edge.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/mod.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/isa/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/operator.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/isa/operator.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/isa/qubit.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/isa/qubit.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/libquil.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/libquil.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/quilc.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/quilc.rs`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
 pub enum CompilationError {
     #[cfg(feature = "libquil")]
     /// Errors during compilation when using libquil
     #[error("compilation error from libquil: {0}")]
     Libquil(crate::compiler::libquil::Error),
     /// Errors during compilation when using RPCQ
     #[error("compilation error from RPCQ: {0}")]
-    Rpcq(crate::compiler::rpcq::Error),
+    Rpcq(rpcq::Error),
 }
 
 /// The response from quilc for a `quil_to_native_quil` request.
 #[derive(Clone, Deserialize, Debug, PartialEq, PartialOrd)]
 pub(crate) struct QuilToNativeQuilResponse {
     /// The compiled program
     pub(crate) quil: String,
```

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/compiler/rpcq.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/compiler/rpcq.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/diagnostics.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/diagnostics.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/executable.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/executable.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/execution_data.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/execution_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/lib.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/api.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/api.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 //! Rigetti QPUs using the QCS API.
 
 use std::{fmt, time::Duration};
 
 use cached::proc_macro::cached;
 use derive_builder::Builder;
 use qcs_api_client_common::configuration::RefreshError;
-pub use qcs_api_client_grpc::channel::Error as GrpcError;
 #[cfg(feature = "grpc-web")]
 use qcs_api_client_grpc::channel::wrap_channel_with_grpc_web;
+pub use qcs_api_client_grpc::channel::Error as GrpcError;
 use qcs_api_client_grpc::{
     channel::{parse_uri, wrap_channel_with, wrap_channel_with_retry},
     get_channel_with_timeout,
     models::controller::{
         controller_job_execution_result, data_value::Value, ControllerJobExecutionResult,
         DataValue, EncryptedControllerJob, JobExecutionConfiguration, RealDataValue,
     },
@@ -594,15 +594,15 @@
             })
             .min_by_key(|acc| acc.rank.unwrap_or(i64::MAX));
 
         min = std::cmp::min_by_key(min, accessor, |acc| {
             acc.as_ref().and_then(|acc| acc.rank).unwrap_or(i64::MAX)
         });
 
-        next_page_token = accessors.next_page_token.clone();
+        next_page_token.clone_from(&accessors.next_page_token);
         if next_page_token.is_none() {
             break;
         }
     }
     min.map(|accessor| accessor.url)
         .ok_or_else(|| QpuApiError::GatewayNotFound(quantum_processor_id.to_string()))
 }
```

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/execution.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/execution.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/mod.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/result_data.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/result_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/rewrite_arithmetic.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/rewrite_arithmetic.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qpu/translation.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qpu/translation.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/execution.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qvm/execution.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/http.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qvm/http.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/libquil.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qvm/libquil.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/qvm/mod.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/qvm/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/src/register_data.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/src/register_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/aspen_9_isa.json` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/aspen_9_isa.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/basic_qvm.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/basic_qvm.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/bell_state_response_data.hex` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/bell_state_response_data.hex`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/compiler-isa-Aspen-8.json` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/compiler-isa-Aspen-8.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/mocked_qpu.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/mocked_qpu.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/parametric_compilation.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/parametric_compilation.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/qcs-isa-Aspen-8.json` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/qcs-isa-Aspen-8.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/qvm_api.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/qvm_api.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/lib/tests/qvm_isa.json` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/lib/tests/qvm_isa.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/Cargo.toml` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "qcs-sdk-python-grpc-web"
 description = "Python bindings to qcs-sdk-rust"
-version = "0.17.8-rc.0"
+version = "0.17.9-rc.0"
 edition = "2021"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/qcs-sdk-rust"
 keywords = [ "pyquil", "SDK", "Rigetti", "Quil", "Quantum",]
 categories = [ "api-bindings", "compilers", "science", "emulators",]
 readme = "./README.md"
```

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/CHANGELOG.md` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## 0.17.9-rc.0
+
+### Fixes
+
+- Refresh JWT only when expired, not before every request (#470)
+
+## 0.17.8
+
+### Features
+
+- Update quil-rs (#464)
+
 ## 0.17.8-rc.0
 
 ### Features
 
 - Update quil-rs (#464)
 
 ## 0.17.7
```

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/Makefile.toml` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/Makefile.toml`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/README.md` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/README.md`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/poetry.lock` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/poetry.lock`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/__init__.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/client.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/client.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/compiler/quilc.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/compiler/quilc.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/diagnostics.py` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/diagnostics.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/__init__.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qpu/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/api.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qpu/api.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/isa.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qpu/isa.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/rewrite_arithmetic.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qpu/rewrite_arithmetic.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qpu/translation.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qpu/translation.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qvm/__init__.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/qcs_sdk/qvm/api.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/qcs_sdk/qvm/api.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/scripts/patch_grpc_web.py` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/scripts/patch_grpc_web.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/client.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/client.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/compiler/quilc.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/compiler/quilc.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/executable.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/executable.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/execution_data.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/execution_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/from_py.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/grpc/models/controller.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/grpc/models/controller.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/lib.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/py_sync.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/py_sync.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/api.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qpu/api.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/isa.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qpu/isa.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/mod.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qpu/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/result_data.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qpu/result_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/rewrite_arithmetic.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qpu/rewrite_arithmetic.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qpu/translation.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qpu/translation.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qvm/api.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qvm/api.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/qvm/mod.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/qvm/mod.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/src/register_data.rs` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/src/register_data.rs`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_fixtures/aspen-m-3.json` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/_fixtures/aspen-m-3.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_fixtures/device-2q.json` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/_fixtures/device-2q.json`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/_qcs_config/settings.toml` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/_qcs_config/settings.toml`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/compiler/__snapshots__/test_quilc.ambr` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/compiler/__snapshots__/test_quilc.ambr`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/compiler/test_quilc.py` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/compiler/test_quilc.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/conftest.py` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/execution_data/test_execution_data.py` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/execution_data/test_execution_data.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_api.py` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/qpu/test_api.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_isa.py` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/qpu/test_isa.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_qpu.py` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/qpu/test_qpu.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_rewrite_arithmetic.py` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/qpu/test_rewrite_arithmetic.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/qpu/test_translation.py` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/qpu/test_translation.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/test_client.py` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/crates/python/tests/test_executable.py` & `qcs_sdk_python_grpc_web-0.17.9rc0/crates/python/tests/test_executable.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/Cargo.lock` & `qcs_sdk_python_grpc_web-0.17.9rc0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,20 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
+version = "0.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
+
+[[package]]
+name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "bindgen"
 version = "0.53.3"
@@ -924,15 +930,15 @@
 
 [[package]]
 name = "headers"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06683b93020a07e3dbcf5f8c0f6d40080d725bea7936fc01ad345c01b97dc270"
 dependencies = [
- "base64",
+ "base64 0.21.7",
  "bytes",
  "headers-core",
  "http",
  "httpdate",
  "mime",
  "sha1",
 ]
@@ -1248,22 +1254,21 @@
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "jsonwebtoken"
-version = "9.2.0"
+version = "8.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c7ea04a7c5c055c175f189b6dc6ba036fd62306b58c66c9f6389036c503a3f4"
+checksum = "6971da4d9c3aa03c3d8f3ff0f4155b534aad021292003895a469716b2a230378"
 dependencies = [
- "base64",
- "js-sys",
+ "base64 0.21.7",
  "pem",
- "ring",
+ "ring 0.16.20",
  "serde",
  "serde_json",
  "simple_asn1",
 ]
 
 [[package]]
 name = "jwalk"
@@ -1806,15 +1811,15 @@
 
 [[package]]
 name = "pbjson"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1030c719b0ec2a2d25a5df729d6cff1acf3cc230bf766f4f97833591f7577b90"
 dependencies = [
- "base64",
+ "base64 0.21.7",
  "serde",
 ]
 
 [[package]]
 name = "pbjson-build"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1845,20 +1850,19 @@
 name = "peeking_take_while"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
 
 [[package]]
 name = "pem"
-version = "3.0.3"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b8fcc794035347fb64beda2d3b462595dd2753e3f268d89c5aae77e8cf2c310"
+checksum = "a8835c273a76a90455d7344889b0964598e3316e2a79ede8e36f16bdcf2228b8"
 dependencies = [
- "base64",
- "serde",
+ "base64 0.13.1",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
@@ -2089,15 +2093,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.53",
 ]
 
 [[package]]
 name = "qcs"
-version = "0.21.8-rc.0"
+version = "0.21.9-rc.0"
 dependencies = [
  "assert2",
  "async-trait",
  "built",
  "cached",
  "derive_builder",
  "enum-as-inner",
@@ -2149,17 +2153,17 @@
  "serde_derive",
  "serde_json",
  "url",
 ]
 
 [[package]]
 name = "qcs-api-client-common"
-version = "0.7.12"
+version = "0.7.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e96a94ca1f4ac3e094d51d90deb5d158dddfd0723cca1b50d302acfd2e4e78ef"
+checksum = "53c56fa367070074f32143b4adef924af1441faa86e835f45371e14801884d14"
 dependencies = [
  "async-trait",
  "backoff",
  "futures",
  "home",
  "http",
  "jsonwebtoken",
@@ -2172,17 +2176,17 @@
  "tracing",
  "url",
  "urlpattern",
 ]
 
 [[package]]
 name = "qcs-api-client-grpc"
-version = "0.7.14"
+version = "0.7.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b82196be0676c8dc24749a830e886ffda6e34b3130c6a7078354c24dec07933a"
+checksum = "01247ae1b0523e058007edb0132cd40915452b8b4dc669d68156e187740ead70"
 dependencies = [
  "backoff",
  "http",
  "http-body",
  "hyper",
  "hyper-proxy",
  "hyper-socks2",
@@ -2205,17 +2209,17 @@
  "tracing",
  "url",
  "urlpattern",
 ]
 
 [[package]]
 name = "qcs-api-client-openapi"
-version = "0.8.13"
+version = "0.8.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0e318c4bffb689688d4f95afb2b5a52a70e12a191da402e0dded093102fcb1e9"
+checksum = "04d7172e79b083a85c911917c03be58eda083b36ea7575db685d21aa2fa99b41"
 dependencies = [
  "anyhow",
  "qcs-api-client-common",
  "reqwest",
  "reqwest-middleware",
  "reqwest-tracing",
  "serde",
@@ -2225,15 +2229,15 @@
  "tracing",
  "url",
  "urlpattern",
 ]
 
 [[package]]
 name = "qcs-sdk-python-grpc-web"
-version = "0.17.8-rc.0"
+version = "0.17.9-rc.0"
 dependencies = [
  "async-trait",
  "numpy",
  "once_cell",
  "paste",
  "pyo3",
  "pyo3-asyncio",
@@ -2383,15 +2387,15 @@
 
 [[package]]
 name = "reqwest"
 version = "0.11.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
 dependencies = [
- "base64",
+ "base64 0.21.7",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
@@ -2468,24 +2472,39 @@
  "num-traits",
  "paste",
  "pyo3",
 ]
 
 [[package]]
 name = "ring"
+version = "0.16.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
+dependencies = [
+ "cc",
+ "libc",
+ "once_cell",
+ "spin 0.5.2",
+ "untrusted 0.7.1",
+ "web-sys",
+ "winapi",
+]
+
+[[package]]
+name = "ring"
 version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
 dependencies = [
  "cc",
  "cfg-if 1.0.0",
  "getrandom",
  "libc",
- "spin",
- "untrusted",
+ "spin 0.9.8",
+ "untrusted 0.9.0",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rmp"
 version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2570,27 +2589,27 @@
 [[package]]
 name = "rustls"
 version = "0.21.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fecbfb7b1444f477b345853b1fce097a2c6fb637b2bfb87e6bc5db0f043fae4"
 dependencies = [
  "log",
- "ring",
+ "ring 0.17.8",
  "rustls-webpki 0.101.7",
  "sct",
 ]
 
 [[package]]
 name = "rustls"
 version = "0.22.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
 dependencies = [
  "log",
- "ring",
+ "ring 0.17.8",
  "rustls-pki-types",
  "rustls-webpki 0.102.2",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
@@ -2620,24 +2639,24 @@
 
 [[package]]
 name = "rustls-pemfile"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
 dependencies = [
- "base64",
+ "base64 0.21.7",
 ]
 
 [[package]]
 name = "rustls-pemfile"
 version = "2.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f48172685e6ff52a556baa527774f61fcaa884f59daf3375c62a3f1cd2549dab"
 dependencies = [
- "base64",
+ "base64 0.21.7",
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2645,27 +2664,27 @@
 
 [[package]]
 name = "rustls-webpki"
 version = "0.101.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
 dependencies = [
- "ring",
- "untrusted",
+ "ring 0.17.8",
+ "untrusted 0.9.0",
 ]
 
 [[package]]
 name = "rustls-webpki"
 version = "0.102.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
 dependencies = [
- "ring",
+ "ring 0.17.8",
  "rustls-pki-types",
- "untrusted",
+ "untrusted 0.9.0",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
@@ -2708,16 +2727,16 @@
 
 [[package]]
 name = "sct"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da046153aa2352493d6cb7da4b6e5c0c057d8a1d0a9aa8560baffdd945acd414"
 dependencies = [
- "ring",
- "untrusted",
+ "ring 0.17.8",
+ "untrusted 0.9.0",
 ]
 
 [[package]]
 name = "security-framework"
 version = "2.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
@@ -2877,14 +2896,20 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
+
+[[package]]
+name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
@@ -3308,15 +3333,15 @@
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "76c4eb7a4e9ef9d4763600161f12f5070b92a578e1b634db88a6887844c91a13"
 dependencies = [
  "async-stream",
  "async-trait",
  "axum",
- "base64",
+ "base64 0.21.7",
  "bytes",
  "h2",
  "http",
  "http-body",
  "hyper",
  "hyper-timeout",
  "percent-encoding",
@@ -3349,15 +3374,15 @@
 
 [[package]]
 name = "tonic-web"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc3b0e1cedbf19fdfb78ef3d672cb9928e0a91a9cb4629cc0c916e8cff8aaaa1"
 dependencies = [
- "base64",
+ "base64 0.21.7",
  "bytes",
  "http",
  "http-body",
  "hyper",
  "pin-project",
  "tokio-stream",
  "tonic",
@@ -3593,14 +3618,20 @@
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "untrusted"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
+
+[[package]]
+name = "untrusted"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
 [[package]]
 name = "url"
 version = "2.5.0"
@@ -3796,16 +3827,16 @@
 
 [[package]]
 name = "webpki"
 version = "0.22.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed63aea5ce73d0ff405984102c42de94fc55a6b75765d621c65262469b3c9b53"
 dependencies = [
- "ring",
- "untrusted",
+ "ring 0.17.8",
+ "untrusted 0.9.0",
 ]
 
 [[package]]
 name = "webpki-roots"
 version = "0.25.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5f20c57d8d7db6d3b86154206ae5d8fba62dd39573114de97c2cb0578251f8e1"
```

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/Cargo.toml` & `qcs_sdk_python_grpc_web-0.17.9rc0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [workspace]
 members = ["crates/*"]
 resolver = "2"
 
 [workspace.dependencies]
 qcs-api = "0.2.1"
-qcs-api-client-common = "0.7.12"
-qcs-api-client-grpc = "0.7.14"
-qcs-api-client-openapi = "0.8.13"
+qcs-api-client-common = "0.7.14"
+qcs-api-client-grpc = "0.7.16"
+qcs-api-client-openapi = "0.8.15"
 serde_json = "1.0.86"
 thiserror = "1.0.57"
 tokio = "1.36.0"
 numpy = "0.20.0"
 pyo3-build-config = "0.20.0"
 
 [profile.release]
```

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/pyproject.toml` & `qcs_sdk_python_grpc_web-0.17.9rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qcs-sdk-python-grpc-web"
-version = "0.17.8-rc.0"
+version = "0.17.9-rc.0"
 description = "Python interface for the QCS Rust SDK"
 readme = "README.md"
 classifiers = [ "Development Status :: 3 - Alpha", "License :: OSI Approved :: Apache Software License", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3.10", "Programming Language :: Python :: 3.11", "Operating System :: OS Independent",]
 dependencies = [ "quil==0.10.0",]
 [[project.authors]]
 name = "Rigetti Computing"
 email = "softapps@rigetti.com"
@@ -26,15 +26,15 @@
 build-backend = "maturin"
 
 [project.license]
 text = "Apache-2.0"
 
 [tool.poetry]
 name = "qcs-sdk-python"
-version = "0.17.8-rc.0"
+version = "0.17.9-rc.0"
 description = "Python interface for the QCS Rust SDK"
 readme = "README.md"
 authors = [ "Rigetti Computing <softapps@rigetti.com>", "Mark Skilbeck <mark.skilbeck@rigetti.com>", "Marquess Valdez <mvaldez@rigetti.com>", "Randall Fulton <rfulton@rigetti.com>",]
 
 [tool.maturin]
 features = [ "pyo3/extension-module",]
 bindings = "pyo3"
```

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qvm/api.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qvm/api.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qvm/__init__.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/diagnostics.py` & `qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/diagnostics.py`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/compiler/quilc.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/compiler/quilc.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/translation.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qpu/translation.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/isa.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qpu/isa.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/api.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qpu/api.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/__init__.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qpu/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/qpu/rewrite_arithmetic.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/qpu/rewrite_arithmetic.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/__init__.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/qcs_sdk/client.pyi` & `qcs_sdk_python_grpc_web-0.17.9rc0/qcs_sdk/client.pyi`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/README.md` & `qcs_sdk_python_grpc_web-0.17.9rc0/README.md`

 * *Files identical despite different names*

### Comparing `qcs_sdk_python_grpc_web-0.17.8rc0/PKG-INFO` & `qcs_sdk_python_grpc_web-0.17.9rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qcs-sdk-python-grpc-web
-Version: 0.17.8rc0
+Version: 0.17.9rc0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
```

