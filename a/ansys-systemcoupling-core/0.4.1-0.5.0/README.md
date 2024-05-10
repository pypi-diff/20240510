# Comparing `tmp/ansys_systemcoupling_core-0.4.1.tar.gz` & `tmp/ansys_systemcoupling_core-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_systemcoupling_core-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_systemcoupling_core-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_systemcoupling_core-0.4.1.tar` & `ansys_systemcoupling_core-0.5.0.tar`

### file list

```diff
@@ -1,328 +1,439 @@
--rw-r--r--   0        0        0     1090 2024-03-04 12:57:29.290001 ansys_systemcoupling_core-0.4.1/LICENSE
--rw-r--r--   0        0        0     8081 2024-03-04 12:57:29.290001 ansys_systemcoupling_core-0.4.1/README.rst
--rw-r--r--   0        0        0     2853 2024-03-04 12:57:29.306002 ansys_systemcoupling_core-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7031 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/__init__.py
--rw-r--r--   0        0        0     1579 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/_version.py
--rw-r--r--   0        0        0     1198 2024-03-04 12:58:18.758014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/_add_participant.py
--rw-r--r--   0        0        0      204 2024-03-04 12:58:18.962014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/_solve.py
--rw-r--r--   0        0        0      858 2024-03-04 12:58:19.022014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/abort.py
--rw-r--r--   0        0        0     1421 2024-03-04 12:58:17.494014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/activate_hidden.py
--rw-r--r--   0        0        0     8249 2024-03-04 12:58:18.690014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_data_transfer.py
--rw-r--r--   0        0        0     8052 2024-03-04 12:58:18.714014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_data_transfer_by_display_names.py
--rw-r--r--   0        0        0     2044 2024-03-04 12:58:18.802014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_expression_function.py
--rw-r--r--   0        0        0     2163 2024-03-04 12:58:18.658014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_interface.py
--rw-r--r--   0        0        0     2212 2024-03-04 12:58:18.670014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_interface_by_display_names.py
--rw-r--r--   0        0        0     1150 2024-03-04 12:58:18.790014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_named_expression.py
--rw-r--r--   0        0        0     5511 2024-03-04 12:58:18.826014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_participant.py
--rw-r--r--   0        0        0     1170 2024-03-04 12:58:18.726014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_reference_frame.py
--rw-r--r--   0        0        0     3347 2024-03-04 12:58:18.738014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_transformation.py
--rw-r--r--   0        0        0     9171 2024-03-04 12:58:18.254014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/analysis_control.py
--rw-r--r--   0        0        0      839 2024-03-04 12:58:18.082014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/apip.py
--rw-r--r--   0        0        0     1015 2024-03-04 12:58:18.606014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/ascii_output.py
--rw-r--r--   0        0        0      403 2024-03-04 12:58:17.690014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/attribute.py
--rw-r--r--   0        0        0     1456 2024-03-04 12:58:17.686014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/attribute_child.py
--rw-r--r--   0        0        0     1200 2024-03-04 12:58:18.502014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/available_ports.py
--rw-r--r--   0        0        0      980 2024-03-04 12:58:18.098014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/avoid_data_reconstruction.py
--rw-r--r--   0        0        0     1385 2024-03-04 12:58:18.942014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/case_root.py
--rw-r--r--   0        0        0      380 2024-03-04 12:58:18.886014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/clear_state.py
--rw-r--r--   0        0        0      471 2024-03-04 12:58:18.490014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_interface.py
--rw-r--r--   0        0        0     1089 2024-03-04 12:58:18.486014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_interface_child.py
--rw-r--r--   0        0        0      579 2024-03-04 12:58:18.026014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_participant.py
--rw-r--r--   0        0        0     5540 2024-03-04 12:58:18.022014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_participant_child.py
--rw-r--r--   0        0        0     1118 2024-03-04 12:58:18.998014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/create_restart_point.py
--rw-r--r--   0        0        0      450 2024-03-04 12:58:18.398014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/data_transfer.py
--rw-r--r--   0        0        0     6375 2024-03-04 12:58:18.394014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/data_transfer_child.py
--rw-r--r--   0        0        0      509 2024-03-04 12:58:18.922014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/delete_snapshot.py
--rw-r--r--   0        0        0     1069 2024-03-04 12:58:18.746014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/delete_transformation.py
--rw-r--r--   0        0        0     2822 2024-03-04 12:58:17.666014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/dimensionality.py
--rw-r--r--   0        0        0     6688 2024-03-04 12:58:17.958014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/execution_control.py
--rw-r--r--   0        0        0      447 2024-03-04 12:58:17.510014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/expression.py
--rw-r--r--   0        0        0     1039 2024-03-04 12:58:17.506014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_child.py
--rw-r--r--   0        0        0      510 2024-03-04 12:58:17.542014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_function.py
--rw-r--r--   0        0        0     1265 2024-03-04 12:58:17.538014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_function_child.py
--rw-r--r--   0        0        0      595 2024-03-04 12:58:17.966014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/external_data_file.py
--rw-r--r--   0        0        0     1879 2024-03-04 12:58:17.894014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/fluent_input.py
--rw-r--r--   0        0        0      454 2024-03-04 12:58:17.858014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/fmu_parameter.py
--rw-r--r--   0        0        0     3845 2024-03-04 12:58:17.850014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/fmu_parameter_child.py
--rw-r--r--   0        0        0     1030 2024-03-04 12:58:18.778014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/generate_input_file.py
--rw-r--r--   0        0        0      660 2024-03-04 12:58:18.770014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/get_execution_command.py
--rw-r--r--   0        0        0      227 2024-03-04 12:58:19.006014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/get_machines.py
--rw-r--r--   0        0        0      730 2024-03-04 12:58:18.718014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/get_region_names_for_participant.py
--rw-r--r--   0        0        0      772 2024-03-04 12:58:18.830014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/get_setup_summary.py
--rw-r--r--   0        0        0      277 2024-03-04 12:58:18.926014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/get_snapshots.py
--rw-r--r--   0        0        0     2222 2024-03-04 12:58:18.838014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/get_status_messages.py
--rw-r--r--   0        0        0     4506 2024-03-04 12:58:18.070014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/global_stabilization.py
--rw-r--r--   0        0        0      903 2024-03-04 12:58:18.810014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/has_input_file_changed.py
--rw-r--r--   0        0        0      993 2024-03-04 12:58:18.782014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/import_system_coupling_input_file.py
--rw-r--r--   0        0        0     1025 2024-03-04 12:58:18.954014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/initialize.py
--rw-r--r--   0        0        0      507 2024-03-04 12:58:17.622014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/instancing.py
--rw-r--r--   0        0        0     2231 2024-03-04 12:58:17.614014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/instancing_child.py
--rw-r--r--   0        0        0      906 2024-03-04 12:58:19.018014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/interrupt.py
--rw-r--r--   0        0        0      932 2024-03-04 12:58:17.630014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/library.py
--rw-r--r--   0        0        0     8521 2024-03-04 12:58:18.470014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/mapping_control.py
--rw-r--r--   0        0        0     4810 2024-03-04 12:58:18.898014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/open.py
--rw-r--r--   0        0        0     1063 2024-03-04 12:58:18.986014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/open_results_in_ensight.py
--rw-r--r--   0        0        0     1153 2024-03-04 12:58:18.918014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/open_snapshot.py
--rw-r--r--   0        0        0     4386 2024-03-04 12:58:18.646014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/output_control.py
--rw-r--r--   0        0        0     6261 2024-03-04 12:58:18.982014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/partition_participants.py
--rw-r--r--   0        0        0      476 2024-03-04 12:58:17.598014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/reference_frame.py
--rw-r--r--   0        0        0     2421 2024-03-04 12:58:17.590014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/reference_frame_child.py
--rw-r--r--   0        0        0      393 2024-03-04 12:58:17.790014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/region.py
--rw-r--r--   0        0        0     2238 2024-03-04 12:58:17.786014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/region_child.py
--rw-r--r--   0        0        0      357 2024-03-04 12:58:18.806014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/reload_expression_function_modules.py
--rw-r--r--   0        0        0     2658 2024-03-04 12:58:18.594014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/results.py
--rw-r--r--   0        0        0     1684 2024-03-04 12:58:18.902014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/save.py
--rw-r--r--   0        0        0     1950 2024-03-04 12:58:18.910014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/save_snapshot.py
--rw-r--r--   0        0        0     6426 2024-03-04 12:58:18.882014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/setup_root.py
--rw-r--r--   0        0        0      808 2024-03-04 12:58:18.958014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/shutdown.py
--rw-r--r--   0        0        0      372 2024-03-04 12:58:18.282014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/side.py
--rw-r--r--   0        0        0     1721 2024-03-04 12:58:18.274014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/side_child.py
--rw-r--r--   0        0        0     2845 2024-03-04 12:58:18.534014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/solution_control.py
--rw-r--r--   0        0        0     2730 2024-03-04 12:58:19.050014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/solution_root.py
--rw-r--r--   0        0        0     1057 2024-03-04 12:58:19.010014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/solve.py
--rw-r--r--   0        0        0     5536 2024-03-04 12:58:18.334014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/stabilization.py
--rw-r--r--   0        0        0     1769 2024-03-04 12:58:18.950014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/start_participants.py
--rw-r--r--   0        0        0     1986 2024-03-04 12:58:18.970014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/step.py
--rw-r--r--   0        0        0      509 2024-03-04 12:58:17.570014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/transformation.py
--rw-r--r--   0        0        0     1837 2024-03-04 12:58:17.562014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/transformation_child.py
--rw-r--r--   0        0        0      879 2024-03-04 12:58:18.574014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/type.py
--rw-r--r--   0        0        0     5626 2024-03-04 12:58:18.154014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/unmapped_value_options.py
--rw-r--r--   0        0        0     1086 2024-03-04 12:58:17.806014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/update_control.py
--rw-r--r--   0        0        0     2211 2024-03-04 12:58:18.766014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/update_participant.py
--rw-r--r--   0        0        0      411 2024-03-04 12:58:17.762014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/variable.py
--rw-r--r--   0        0        0     6137 2024-03-04 12:58:17.754014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/variable_child.py
--rw-r--r--   0        0        0      656 2024-03-04 12:58:19.002014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/write_csv_chart_files.py
--rw-r--r--   0        0        0     1278 2024-03-04 12:58:18.994014 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/write_ensight.py
--rw-r--r--   0        0        0     1198 2024-03-04 12:58:58.633895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/_add_participant.py
--rw-r--r--   0        0        0      204 2024-03-04 12:58:58.873894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/_solve.py
--rw-r--r--   0        0        0      858 2024-03-04 12:58:58.945894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/abort.py
--rw-r--r--   0        0        0     1421 2024-03-04 12:58:57.281896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/activate_hidden.py
--rw-r--r--   0        0        0     8249 2024-03-04 12:58:58.565894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_data_transfer.py
--rw-r--r--   0        0        0     8052 2024-03-04 12:58:58.585894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_data_transfer_by_display_names.py
--rw-r--r--   0        0        0     2044 2024-03-04 12:58:58.677894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_expression_function.py
--rw-r--r--   0        0        0     2163 2024-03-04 12:58:58.529894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_interface.py
--rw-r--r--   0        0        0     2212 2024-03-04 12:58:58.541895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_interface_by_display_names.py
--rw-r--r--   0        0        0     1150 2024-03-04 12:58:58.665894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_named_expression.py
--rw-r--r--   0        0        0     5511 2024-03-04 12:58:58.701894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_participant.py
--rw-r--r--   0        0        0     1170 2024-03-04 12:58:58.597895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_reference_frame.py
--rw-r--r--   0        0        0     3347 2024-03-04 12:58:58.613895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_transformation.py
--rw-r--r--   0        0        0     9461 2024-03-04 12:58:58.101895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/analysis_control.py
--rw-r--r--   0        0        0      839 2024-03-04 12:58:57.901895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/apip.py
--rw-r--r--   0        0        0     1015 2024-03-04 12:58:58.453895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/ascii_output.py
--rw-r--r--   0        0        0      403 2024-03-04 12:58:57.485895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/attribute.py
--rw-r--r--   0        0        0     1456 2024-03-04 12:58:57.477896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/attribute_child.py
--rw-r--r--   0        0        0     1428 2024-03-04 12:58:57.997895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/automatic_alignment_options.py
--rw-r--r--   0        0        0     1200 2024-03-04 12:58:58.381895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/available_ports.py
--rw-r--r--   0        0        0     1353 2024-03-04 12:58:57.921895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/avoid_data_reconstruction.py
--rw-r--r--   0        0        0     1385 2024-03-04 12:58:58.853894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/case_root.py
--rw-r--r--   0        0        0      380 2024-03-04 12:58:58.797894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/clear_state.py
--rw-r--r--   0        0        0      471 2024-03-04 12:58:58.369895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_interface.py
--rw-r--r--   0        0        0     1089 2024-03-04 12:58:58.333895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_interface_child.py
--rw-r--r--   0        0        0      579 2024-03-04 12:58:57.845895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_participant.py
--rw-r--r--   0        0        0     5540 2024-03-04 12:58:57.841895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_participant_child.py
--rw-r--r--   0        0        0     1118 2024-03-04 12:58:58.913894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/create_restart_point.py
--rw-r--r--   0        0        0      450 2024-03-04 12:58:58.245895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/data_transfer.py
--rw-r--r--   0        0        0     6375 2024-03-04 12:58:58.241895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/data_transfer_child.py
--rw-r--r--   0        0        0      509 2024-03-04 12:58:58.833894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/delete_snapshot.py
--rw-r--r--   0        0        0     1069 2024-03-04 12:58:58.617895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/delete_transformation.py
--rw-r--r--   0        0        0     2822 2024-03-04 12:58:57.461896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/dimensionality.py
--rw-r--r--   0        0        0     6688 2024-03-04 12:58:57.777895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/execution_control.py
--rw-r--r--   0        0        0      447 2024-03-04 12:58:57.301896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/expression.py
--rw-r--r--   0        0        0     1039 2024-03-04 12:58:57.293896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_child.py
--rw-r--r--   0        0        0      510 2024-03-04 12:58:57.333896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_function.py
--rw-r--r--   0        0        0     1265 2024-03-04 12:58:57.325896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_function_child.py
--rw-r--r--   0        0        0      595 2024-03-04 12:58:57.785895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/external_data_file.py
--rw-r--r--   0        0        0     1879 2024-03-04 12:58:57.713895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/fluent_input.py
--rw-r--r--   0        0        0      454 2024-03-04 12:58:57.693895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/fmu_parameter.py
--rw-r--r--   0        0        0     4880 2024-03-04 12:58:57.685895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/fmu_parameter_child.py
--rw-r--r--   0        0        0     1030 2024-03-04 12:58:58.653895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/generate_input_file.py
--rw-r--r--   0        0        0      660 2024-03-04 12:58:58.645894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/get_execution_command.py
--rw-r--r--   0        0        0      227 2024-03-04 12:58:58.929894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/get_machines.py
--rw-r--r--   0        0        0      730 2024-03-04 12:58:58.593895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/get_region_names_for_participant.py
--rw-r--r--   0        0        0      772 2024-03-04 12:58:58.705894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/get_setup_summary.py
--rw-r--r--   0        0        0      277 2024-03-04 12:58:58.837894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/get_snapshots.py
--rw-r--r--   0        0        0     2222 2024-03-04 12:58:58.713894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/get_status_messages.py
--rw-r--r--   0        0        0      999 2024-03-04 12:58:58.921894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/get_transformation.py
--rw-r--r--   0        0        0     4506 2024-03-04 12:58:57.889895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/global_stabilization.py
--rw-r--r--   0        0        0      903 2024-03-04 12:58:58.685894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/has_input_file_changed.py
--rw-r--r--   0        0        0      993 2024-03-04 12:58:58.661894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/import_system_coupling_input_file.py
--rw-r--r--   0        0        0     1025 2024-03-04 12:58:58.865894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/initialize.py
--rw-r--r--   0        0        0      507 2024-03-04 12:58:57.413896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/instancing.py
--rw-r--r--   0        0        0     2231 2024-03-04 12:58:57.405896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/instancing_child.py
--rw-r--r--   0        0        0      906 2024-03-04 12:58:58.937894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/interrupt.py
--rw-r--r--   0        0        0      932 2024-03-04 12:58:57.421896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/library.py
--rw-r--r--   0        0        0      486 2024-03-04 12:58:58.477895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/live_visualization.py
--rw-r--r--   0        0        0     2250 2024-03-04 12:58:58.473895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/live_visualization_child.py
--rw-r--r--   0        0        0     8521 2024-03-04 12:58:58.321895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/mapping_control.py
--rw-r--r--   0        0        0     4810 2024-03-04 12:58:58.805894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/open.py
--rw-r--r--   0        0        0     1903 2024-03-04 12:58:58.901894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/open_results_in_en_sight.py
--rw-r--r--   0        0        0     1153 2024-03-04 12:58:58.825894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/open_snapshot.py
--rw-r--r--   0        0        0     4587 2024-03-04 12:58:58.517895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/output_control.py
--rw-r--r--   0        0        0     6261 2024-03-04 12:58:58.893894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/partition_participants.py
--rw-r--r--   0        0        0      476 2024-03-04 12:58:57.389896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/reference_frame.py
--rw-r--r--   0        0        0     2421 2024-03-04 12:58:57.381896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/reference_frame_child.py
--rw-r--r--   0        0        0      393 2024-03-04 12:58:57.601895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/region.py
--rw-r--r--   0        0        0     2238 2024-03-04 12:58:57.593896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/region_child.py
--rw-r--r--   0        0        0      357 2024-03-04 12:58:58.681894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/reload_expression_function_modules.py
--rw-r--r--   0        0        0     2658 2024-03-04 12:58:58.441895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/results.py
--rw-r--r--   0        0        0     1684 2024-03-04 12:58:58.813894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/save.py
--rw-r--r--   0        0        0     1950 2024-03-04 12:58:58.821894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/save_snapshot.py
--rw-r--r--   0        0        0     6426 2024-03-04 12:58:58.789894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/setup_root.py
--rw-r--r--   0        0        0      808 2024-03-04 12:58:58.869894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/shutdown.py
--rw-r--r--   0        0        0      372 2024-03-04 12:58:58.125895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/side.py
--rw-r--r--   0        0        0     1721 2024-03-04 12:58:58.121895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/side_child.py
--rw-r--r--   0        0        0     2845 2024-03-04 12:58:58.409895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/solution_control.py
--rw-r--r--   0        0        0     2947 2024-03-04 12:58:58.973894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/solution_root.py
--rw-r--r--   0        0        0     1057 2024-03-04 12:58:58.933894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/solve.py
--rw-r--r--   0        0        0     5536 2024-03-04 12:58:58.181895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/stabilization.py
--rw-r--r--   0        0        0     1769 2024-03-04 12:58:58.861894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/start_participants.py
--rw-r--r--   0        0        0     1986 2024-03-04 12:58:58.881894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/step.py
--rw-r--r--   0        0        0      509 2024-03-04 12:58:57.357896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/transformation.py
--rw-r--r--   0        0        0     1837 2024-03-04 12:58:57.353896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/transformation_child.py
--rw-r--r--   0        0        0      879 2024-03-04 12:58:58.425895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/type.py
--rw-r--r--   0        0        0     5626 2024-03-04 12:58:57.981895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/unmapped_value_options.py
--rw-r--r--   0        0        0     1086 2024-03-04 12:58:57.613896 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/update_control.py
--rw-r--r--   0        0        0     2211 2024-03-04 12:58:58.637894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/update_participant.py
--rw-r--r--   0        0        0      411 2024-03-04 12:58:57.569895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/variable.py
--rw-r--r--   0        0        0     7249 2024-03-04 12:58:57.565895 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/variable_child.py
--rw-r--r--   0        0        0      656 2024-03-04 12:58:58.925894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/write_csv_chart_files.py
--rw-r--r--   0        0        0     1278 2024-03-04 12:58:58.909894 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/write_ensight.py
--rw-r--r--   0        0        0     1198 2024-03-04 12:59:38.949762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/_add_participant.py
--rw-r--r--   0        0        0      204 2024-03-04 12:59:39.181761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/_solve.py
--rw-r--r--   0        0        0      858 2024-03-04 12:59:39.253761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/abort.py
--rw-r--r--   0        0        0     1421 2024-03-04 12:59:37.409766 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/activate_hidden.py
--rw-r--r--   0        0        0     1113 2024-03-04 12:59:38.929762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_aerodamping_data_transfers.py
--rw-r--r--   0        0        0     8249 2024-03-04 12:59:38.809762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_data_transfer.py
--rw-r--r--   0        0        0     8168 2024-03-04 12:59:38.833762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_data_transfer_by_display_names.py
--rw-r--r--   0        0        0     2044 2024-03-04 12:59:38.993762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_expression_function.py
--rw-r--r--   0        0        0      694 2024-03-04 12:59:38.873762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_fsi_data_transfers.py
--rw-r--r--   0        0        0     2574 2024-03-04 12:59:38.777762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_interface.py
--rw-r--r--   0        0        0     2324 2024-03-04 12:59:38.789762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_interface_by_display_names.py
--rw-r--r--   0        0        0     1150 2024-03-04 12:59:38.981762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_named_expression.py
--rw-r--r--   0        0        0      735 2024-03-04 12:59:38.937762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_ordered_data_transfers.py
--rw-r--r--   0        0        0     5361 2024-03-04 12:59:39.037762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_participant.py
--rw-r--r--   0        0        0     1170 2024-03-04 12:59:38.845762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_reference_frame.py
--rw-r--r--   0        0        0     1105 2024-03-04 12:59:38.881762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_thermal_data_transfers.py
--rw-r--r--   0        0        0     3347 2024-03-04 12:59:38.857762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_transformation.py
--rw-r--r--   0        0        0    10857 2024-03-04 12:59:38.321764 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/analysis_control.py
--rw-r--r--   0        0        0      839 2024-03-04 12:59:38.105764 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/apip.py
--rw-r--r--   0        0        0     1015 2024-03-04 12:59:38.697762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/ascii_output.py
--rw-r--r--   0        0        0      403 2024-03-04 12:59:37.609765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/attribute.py
--rw-r--r--   0        0        0     1456 2024-03-04 12:59:37.601765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/attribute_child.py
--rw-r--r--   0        0        0     1428 2024-03-04 12:59:38.225764 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/automatic_alignment_options.py
--rw-r--r--   0        0        0     1200 2024-03-04 12:59:38.613763 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/available_ports.py
--rw-r--r--   0        0        0     1353 2024-03-04 12:59:38.125764 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/avoid_data_reconstruction.py
--rw-r--r--   0        0        0     1214 2024-03-04 12:59:39.157761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/case_root.py
--rw-r--r--   0        0        0      380 2024-03-04 12:59:39.109761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/clear_state.py
--rw-r--r--   0        0        0      471 2024-03-04 12:59:38.601763 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_interface.py
--rw-r--r--   0        0        0     1089 2024-03-04 12:59:38.597763 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_interface_child.py
--rw-r--r--   0        0        0      579 2024-03-04 12:59:38.049764 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_participant.py
--rw-r--r--   0        0        0     8720 2024-03-04 12:59:38.041764 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_participant_child.py
--rw-r--r--   0        0        0     1118 2024-03-04 12:59:39.217761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/create_restart_point.py
--rw-r--r--   0        0        0      450 2024-03-04 12:59:38.469763 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/data_transfer.py
--rw-r--r--   0        0        0     6375 2024-03-04 12:59:38.461763 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/data_transfer_child.py
--rw-r--r--   0        0        0      509 2024-03-04 12:59:39.145761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/delete_snapshot.py
--rw-r--r--   0        0        0     1069 2024-03-04 12:59:38.865762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/delete_transformation.py
--rw-r--r--   0        0        0     2822 2024-03-04 12:59:37.585765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/dimensionality.py
--rw-r--r--   0        0        0     7049 2024-03-04 12:59:37.933765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/execution_control.py
--rw-r--r--   0        0        0      447 2024-03-04 12:59:37.429766 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/expression.py
--rw-r--r--   0        0        0     1039 2024-03-04 12:59:37.421766 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/expression_child.py
--rw-r--r--   0        0        0      510 2024-03-04 12:59:37.461766 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/expression_function.py
--rw-r--r--   0        0        0     1265 2024-03-04 12:59:37.453766 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/expression_function_child.py
--rw-r--r--   0        0        0      595 2024-03-04 12:59:37.941764 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/external_data_file.py
--rw-r--r--   0        0        0     1879 2024-03-04 12:59:37.861765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/fluent_input.py
--rw-r--r--   0        0        0      454 2024-03-04 12:59:37.841765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/fmu_parameter.py
--rw-r--r--   0        0        0     4880 2024-03-04 12:59:37.833765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/fmu_parameter_child.py
--rw-r--r--   0        0        0     1030 2024-03-04 12:59:38.969762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/generate_input_file.py
--rw-r--r--   0        0        0      617 2024-03-04 12:59:39.001762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_add_data_transfer_group_commands.py
--rw-r--r--   0        0        0      660 2024-03-04 12:59:38.961762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_execution_command.py
--rw-r--r--   0        0        0      227 2024-03-04 12:59:39.233761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_machines.py
--rw-r--r--   0        0        0      604 2024-03-04 12:59:39.013762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_mode_shape_variables.py
--rw-r--r--   0        0        0      730 2024-03-04 12:59:38.837762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_region_names_for_participant.py
--rw-r--r--   0        0        0      772 2024-03-04 12:59:39.041761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_setup_summary.py
--rw-r--r--   0        0        0     2222 2024-03-04 12:59:39.045761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_status_messages.py
--rw-r--r--   0        0        0      829 2024-03-04 12:59:39.009762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_thermal_data_transfer_options.py
--rw-r--r--   0        0        0      999 2024-03-04 12:59:39.225761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_transformation.py
--rw-r--r--   0        0        0     4506 2024-03-04 12:59:38.093764 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/global_stabilization.py
--rw-r--r--   0        0        0      909 2024-03-04 12:59:39.021762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/has_input_file_changed.py
--rw-r--r--   0        0        0      993 2024-03-04 12:59:38.977762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/import_system_coupling_input_file.py
--rw-r--r--   0        0        0     1025 2024-03-04 12:59:39.173761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/initialize.py
--rw-r--r--   0        0        0      507 2024-03-04 12:59:37.537766 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/instancing.py
--rw-r--r--   0        0        0     2231 2024-03-04 12:59:37.533766 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/instancing_child.py
--rw-r--r--   0        0        0      906 2024-03-04 12:59:39.245761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/interrupt.py
--rw-r--r--   0        0        0      932 2024-03-04 12:59:37.549766 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/library.py
--rw-r--r--   0        0        0      486 2024-03-04 12:59:38.721762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/live_visualization.py
--rw-r--r--   0        0        0     2250 2024-03-04 12:59:38.717762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/live_visualization_child.py
--rw-r--r--   0        0        0     8900 2024-03-04 12:59:38.581763 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/mapping_control.py
--rw-r--r--   0        0        0     4810 2024-03-04 12:59:39.117761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/open.py
--rw-r--r--   0        0        0     1902 2024-03-04 12:59:39.205761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/open_results_in_ensight.py
--rw-r--r--   0        0        0     1153 2024-03-04 12:59:39.137761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/open_snapshot.py
--rw-r--r--   0        0        0     4587 2024-03-04 12:59:38.765762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/output_control.py
--rw-r--r--   0        0        0      420 2024-03-04 12:59:37.717765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/parameter.py
--rw-r--r--   0        0        0     1686 2024-03-04 12:59:37.713765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/parameter_child.py
--rw-r--r--   0        0        0     6261 2024-03-04 12:59:39.197761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/partition_participants.py
--rw-r--r--   0        0        0     1091 2024-03-04 12:59:37.957764 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/record_interactions.py
--rw-r--r--   0        0        0      476 2024-03-04 12:59:37.517766 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/reference_frame.py
--rw-r--r--   0        0        0     2421 2024-03-04 12:59:37.509766 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/reference_frame_child.py
--rw-r--r--   0        0        0      393 2024-03-04 12:59:37.749765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/region.py
--rw-r--r--   0        0        0     2252 2024-03-04 12:59:37.741765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/region_child.py
--rw-r--r--   0        0        0      357 2024-03-04 12:59:38.997762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/reload_expression_function_modules.py
--rw-r--r--   0        0        0     2658 2024-03-04 12:59:38.685763 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/results.py
--rw-r--r--   0        0        0     1684 2024-03-04 12:59:39.125761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/save.py
--rw-r--r--   0        0        0     1950 2024-03-04 12:59:39.133761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/save_snapshot.py
--rw-r--r--   0        0        0     8420 2024-03-04 12:59:39.101761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/setup_root.py
--rw-r--r--   0        0        0      808 2024-03-04 12:59:39.177761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/shutdown.py
--rw-r--r--   0        0        0      372 2024-03-04 12:59:38.349763 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/side.py
--rw-r--r--   0        0        0     1721 2024-03-04 12:59:38.341763 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/side_child.py
--rw-r--r--   0        0        0     4048 2024-03-04 12:59:38.653763 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/solution_control.py
--rw-r--r--   0        0        0     2940 2024-03-04 12:59:39.281761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/solution_root.py
--rw-r--r--   0        0        0     1057 2024-03-04 12:59:39.241761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/solve.py
--rw-r--r--   0        0        0     5536 2024-03-04 12:59:38.401763 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/stabilization.py
--rw-r--r--   0        0        0     1764 2024-03-04 12:59:39.169761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/start_participants.py
--rw-r--r--   0        0        0     1986 2024-03-04 12:59:39.185761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/step.py
--rw-r--r--   0        0        0      509 2024-03-04 12:59:37.485766 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/transformation.py
--rw-r--r--   0        0        0     1837 2024-03-04 12:59:37.481766 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/transformation_child.py
--rw-r--r--   0        0        0      879 2024-03-04 12:59:38.665763 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/type.py
--rw-r--r--   0        0        0     5626 2024-03-04 12:59:38.209764 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/unmapped_value_options.py
--rw-r--r--   0        0        0     1086 2024-03-04 12:59:37.761765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/update_control.py
--rw-r--r--   0        0        0     2341 2024-03-04 12:59:38.957762 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/update_participant.py
--rw-r--r--   0        0        0      411 2024-03-04 12:59:37.689765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/variable.py
--rw-r--r--   0        0        0     7234 2024-03-04 12:59:37.685765 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/variable_child.py
--rw-r--r--   0        0        0      656 2024-03-04 12:59:39.229761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/write_csv_chart_files.py
--rw-r--r--   0        0        0     1278 2024-03-04 12:59:39.213761 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/write_ensight.py
--rw-r--r--   0        0        0     4210 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/get_status_messages.py
--rw-r--r--   0        0        0     2489 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/get_syc_version.py
--rw-r--r--   0        0        0    12247 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/injected_commands.py
--rw-r--r--   0        0        0    12828 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/root_source.py
--rw-r--r--   0        0        0    14927 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/static_info.py
--rw-r--r--   0        0        0     4784 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy.py
--rw-r--r--   0        0        0     2281 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy_interface.py
--rw-r--r--   0        0        0    25130 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/types.py
--rw-r--r--   0        0        0    14735 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/grpc_client.py
--rw-r--r--   0        0        0     2256 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/services/command_query.py
--rw-r--r--   0        0        0     2148 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/services/output_stream.py
--rw-r--r--   0        0        0     1683 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/services/process.py
--rw-r--r--   0        0        0     2518 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/services/solution.py
--rw-r--r--   0        0        0     2752 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/syc_container.py
--rw-r--r--   0        0        0     5635 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/syc_process.py
--rw-r--r--   0        0        0     3064 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/variant.py
--rw-r--r--   0        0        0     1223 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/examples/__init__.py
--rw-r--r--   0        0        0     4101 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/examples/downloads.py
--rw-r--r--   0        0        0     1188 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/native_api/__init__.py
--rw-r--r--   0        0        0     1734 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/native_api/command_metadata.py
--rw-r--r--   0        0        0     4836 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/native_api/datamodel_metadata.py
--rw-r--r--   0        0        0     1462 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/native_api/meta_wrapper.py
--rw-r--r--   0        0        0     7116 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/native_api/native_api.py
--rw-r--r--   0        0        0     4153 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/native_api/object_path.py
--rw-r--r--   0        0        0     8839 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/participant/manager.py
--rw-r--r--   0        0        0    11166 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/participant/mapdl.py
--rw-r--r--   0        0        0     2427 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/participant/protocol.py
--rw-r--r--   0        0        0    10219 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/session.py
--rw-r--r--   0        0        0     3783 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/syc_version.py
--rw-r--r--   0        0        0     5186 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/util/file_transfer.py
--rw-r--r--   0        0        0     5040 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/util/logging.py
--rw-r--r--   0        0        0     1470 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/util/name_util.py
--rw-r--r--   0        0        0     1941 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/util/pathstr.py
--rw-r--r--   0        0        0     4545 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/util/state_keys.py
--rw-r--r--   0        0        0     2982 2024-03-04 12:57:29.310001 ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/util/yaml_helper.py
--rw-r--r--   0        0        0    10946 1970-01-01 00:00:00.000000 ansys_systemcoupling_core-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-05-10 14:02:43.484587 ansys_systemcoupling_core-0.5.0/LICENSE
+-rw-r--r--   0        0        0     8081 2024-05-10 14:02:43.484587 ansys_systemcoupling_core-0.5.0/README.rst
+-rw-r--r--   0        0        0     2855 2024-05-10 14:02:43.500587 ansys_systemcoupling_core-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7031 2024-05-10 14:02:43.500587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/__init__.py
+-rw-r--r--   0        0        0     1579 2024-05-10 14:02:43.500587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/_version.py
+-rw-r--r--   0        0        0     1198 2024-05-10 14:03:30.092980 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/_add_participant.py
+-rw-r--r--   0        0        0      215 2024-05-10 14:03:30.236981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/_clear_state.py
+-rw-r--r--   0        0        0      204 2024-05-10 14:03:30.324981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/_solve.py
+-rw-r--r--   0        0        0      858 2024-05-10 14:03:30.388982 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/abort.py
+-rw-r--r--   0        0        0     1421 2024-05-10 14:03:28.664968 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/activate_hidden.py
+-rw-r--r--   0        0        0     8249 2024-05-10 14:03:30.020979 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_data_transfer.py
+-rw-r--r--   0        0        0     8052 2024-05-10 14:03:30.044979 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_data_transfer_by_display_names.py
+-rw-r--r--   0        0        0     2044 2024-05-10 14:03:30.140980 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_expression_function.py
+-rw-r--r--   0        0        0     2163 2024-05-10 14:03:29.988979 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_interface.py
+-rw-r--r--   0        0        0     2212 2024-05-10 14:03:30.000979 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_interface_by_display_names.py
+-rw-r--r--   0        0        0     1150 2024-05-10 14:03:30.132980 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_named_expression.py
+-rw-r--r--   0        0        0     5511 2024-05-10 14:03:30.172980 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_participant.py
+-rw-r--r--   0        0        0     1170 2024-05-10 14:03:30.056979 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_reference_frame.py
+-rw-r--r--   0        0        0     3347 2024-05-10 14:03:30.072979 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_transformation.py
+-rw-r--r--   0        0        0     9171 2024-05-10 14:03:29.520975 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/analysis_control.py
+-rw-r--r--   0        0        0      839 2024-05-10 14:03:29.312973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/apip.py
+-rw-r--r--   0        0        0     1015 2024-05-10 14:03:29.932978 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/ascii_output.py
+-rw-r--r--   0        0        0      403 2024-05-10 14:03:28.876970 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/attribute.py
+-rw-r--r--   0        0        0     1456 2024-05-10 14:03:28.872970 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/attribute_child.py
+-rw-r--r--   0        0        0     1200 2024-05-10 14:03:29.788977 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/available_ports.py
+-rw-r--r--   0        0        0      980 2024-05-10 14:03:29.324973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/avoid_data_reconstruction.py
+-rw-r--r--   0        0        0     1549 2024-05-10 14:03:30.300981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/case_root.py
+-rw-r--r--   0        0        0      419 2024-05-10 14:03:30.284981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/clear_state.py
+-rw-r--r--   0        0        0      471 2024-05-10 14:03:29.776977 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_interface.py
+-rw-r--r--   0        0        0     1089 2024-05-10 14:03:29.768977 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_interface_child.py
+-rw-r--r--   0        0        0      579 2024-05-10 14:03:29.248973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_participant.py
+-rw-r--r--   0        0        0     5540 2024-05-10 14:03:29.244973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_participant_child.py
+-rw-r--r--   0        0        0     1118 2024-05-10 14:03:30.364982 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/create_restart_point.py
+-rw-r--r--   0        0        0      450 2024-05-10 14:03:29.672976 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/data_transfer.py
+-rw-r--r--   0        0        0     6375 2024-05-10 14:03:29.668976 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/data_transfer_child.py
+-rw-r--r--   0        0        0      509 2024-05-10 14:03:30.272981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/delete_snapshot.py
+-rw-r--r--   0        0        0     1069 2024-05-10 14:03:30.080979 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/delete_transformation.py
+-rw-r--r--   0        0        0     2822 2024-05-10 14:03:28.852970 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/dimensionality.py
+-rw-r--r--   0        0        0     6688 2024-05-10 14:03:29.176972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/execution_control.py
+-rw-r--r--   0        0        0      447 2024-05-10 14:03:28.680969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/expression.py
+-rw-r--r--   0        0        0     1039 2024-05-10 14:03:28.676968 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_child.py
+-rw-r--r--   0        0        0      510 2024-05-10 14:03:28.716969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_function.py
+-rw-r--r--   0        0        0     1265 2024-05-10 14:03:28.712969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_function_child.py
+-rw-r--r--   0        0        0      595 2024-05-10 14:03:29.184972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/external_data_file.py
+-rw-r--r--   0        0        0     1879 2024-05-10 14:03:29.104972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/fluent_input.py
+-rw-r--r--   0        0        0      454 2024-05-10 14:03:29.056971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/fmu_parameter.py
+-rw-r--r--   0        0        0     3845 2024-05-10 14:03:29.052971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/fmu_parameter_child.py
+-rw-r--r--   0        0        0     1030 2024-05-10 14:03:30.116980 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/generate_input_file.py
+-rw-r--r--   0        0        0      660 2024-05-10 14:03:30.108980 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/get_execution_command.py
+-rw-r--r--   0        0        0      227 2024-05-10 14:03:30.372982 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/get_machines.py
+-rw-r--r--   0        0        0      730 2024-05-10 14:03:30.052979 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/get_region_names_for_participant.py
+-rw-r--r--   0        0        0      772 2024-05-10 14:03:30.176980 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/get_setup_summary.py
+-rw-r--r--   0        0        0      277 2024-05-10 14:03:30.280981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/get_snapshots.py
+-rw-r--r--   0        0        0     2222 2024-05-10 14:03:30.180980 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/get_status_messages.py
+-rw-r--r--   0        0        0     4506 2024-05-10 14:03:29.296973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/global_stabilization.py
+-rw-r--r--   0        0        0      903 2024-05-10 14:03:30.152980 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/has_input_file_changed.py
+-rw-r--r--   0        0        0      993 2024-05-10 14:03:30.124980 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/import_system_coupling_input_file.py
+-rw-r--r--   0        0        0     1025 2024-05-10 14:03:30.316981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/initialize.py
+-rw-r--r--   0        0        0      507 2024-05-10 14:03:28.800969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/instancing.py
+-rw-r--r--   0        0        0     2231 2024-05-10 14:03:28.796970 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/instancing_child.py
+-rw-r--r--   0        0        0      906 2024-05-10 14:03:30.384982 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/interrupt.py
+-rw-r--r--   0        0        0      932 2024-05-10 14:03:28.812970 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/library.py
+-rw-r--r--   0        0        0     8521 2024-05-10 14:03:29.756977 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/mapping_control.py
+-rw-r--r--   0        0        0     4810 2024-05-10 14:03:30.244981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/open.py
+-rw-r--r--   0        0        0     1063 2024-05-10 14:03:30.348981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/open_results_in_ensight.py
+-rw-r--r--   0        0        0     1153 2024-05-10 14:03:30.268981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/open_snapshot.py
+-rw-r--r--   0        0        0     4386 2024-05-10 14:03:29.976979 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/output_control.py
+-rw-r--r--   0        0        0     6261 2024-05-10 14:03:30.344981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/partition_participants.py
+-rw-r--r--   0        0        0      476 2024-05-10 14:03:28.776969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/reference_frame.py
+-rw-r--r--   0        0        0     2421 2024-05-10 14:03:28.772969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/reference_frame_child.py
+-rw-r--r--   0        0        0      393 2024-05-10 14:03:28.988971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/region.py
+-rw-r--r--   0        0        0     2238 2024-05-10 14:03:28.980971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/region_child.py
+-rw-r--r--   0        0        0      357 2024-05-10 14:03:30.144980 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/reload_expression_function_modules.py
+-rw-r--r--   0        0        0     2658 2024-05-10 14:03:29.920978 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/results.py
+-rw-r--r--   0        0        0     1684 2024-05-10 14:03:30.252981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/save.py
+-rw-r--r--   0        0        0     1950 2024-05-10 14:03:30.260981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/save_snapshot.py
+-rw-r--r--   0        0        0     6426 2024-05-10 14:03:30.228980 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/setup_root.py
+-rw-r--r--   0        0        0      808 2024-05-10 14:03:30.320981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/shutdown.py
+-rw-r--r--   0        0        0      372 2024-05-10 14:03:29.548975 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/side.py
+-rw-r--r--   0        0        0     1721 2024-05-10 14:03:29.540975 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/side_child.py
+-rw-r--r--   0        0        0     2845 2024-05-10 14:03:29.884978 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/solution_control.py
+-rw-r--r--   0        0        0     2730 2024-05-10 14:03:30.416982 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/solution_root.py
+-rw-r--r--   0        0        0     1057 2024-05-10 14:03:30.376982 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/solve.py
+-rw-r--r--   0        0        0     5536 2024-05-10 14:03:29.604976 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/stabilization.py
+-rw-r--r--   0        0        0     1769 2024-05-10 14:03:30.312981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/start_participants.py
+-rw-r--r--   0        0        0     1986 2024-05-10 14:03:30.332981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/step.py
+-rw-r--r--   0        0        0      509 2024-05-10 14:03:28.744969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/transformation.py
+-rw-r--r--   0        0        0     1837 2024-05-10 14:03:28.740969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/transformation_child.py
+-rw-r--r--   0        0        0      879 2024-05-10 14:03:29.896978 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/type.py
+-rw-r--r--   0        0        0     5626 2024-05-10 14:03:29.392974 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/unmapped_value_options.py
+-rw-r--r--   0        0        0     1086 2024-05-10 14:03:29.000971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/update_control.py
+-rw-r--r--   0        0        0     2211 2024-05-10 14:03:30.100979 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/update_participant.py
+-rw-r--r--   0        0        0      411 2024-05-10 14:03:28.952971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/variable.py
+-rw-r--r--   0        0        0     6137 2024-05-10 14:03:28.948971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/variable_child.py
+-rw-r--r--   0        0        0      656 2024-05-10 14:03:30.368981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/write_csv_chart_files.py
+-rw-r--r--   0        0        0     1278 2024-05-10 14:03:30.356981 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/write_ensight.py
+-rw-r--r--   0        0        0     1198 2024-05-10 14:04:11.121295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/_add_participant.py
+-rw-r--r--   0        0        0      215 2024-05-10 14:04:11.305297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/_clear_state.py
+-rw-r--r--   0        0        0      204 2024-05-10 14:04:11.393297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/_solve.py
+-rw-r--r--   0        0        0      858 2024-05-10 14:04:11.473298 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/abort.py
+-rw-r--r--   0        0        0     1421 2024-05-10 14:04:09.605284 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/activate_hidden.py
+-rw-r--r--   0        0        0     8249 2024-05-10 14:04:11.053295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_data_transfer.py
+-rw-r--r--   0        0        0     8052 2024-05-10 14:04:11.073295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_data_transfer_by_display_names.py
+-rw-r--r--   0        0        0     2044 2024-05-10 14:04:11.169295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_expression_function.py
+-rw-r--r--   0        0        0     2163 2024-05-10 14:04:11.017294 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_interface.py
+-rw-r--r--   0        0        0     2212 2024-05-10 14:04:11.029294 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_interface_by_display_names.py
+-rw-r--r--   0        0        0     1150 2024-05-10 14:04:11.157295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_named_expression.py
+-rw-r--r--   0        0        0     5511 2024-05-10 14:04:11.197296 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_participant.py
+-rw-r--r--   0        0        0     1170 2024-05-10 14:04:11.085295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_reference_frame.py
+-rw-r--r--   0        0        0     3347 2024-05-10 14:04:11.101295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_transformation.py
+-rw-r--r--   0        0        0     9461 2024-05-10 14:04:10.525291 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/analysis_control.py
+-rw-r--r--   0        0        0      839 2024-05-10 14:04:10.297289 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/apip.py
+-rw-r--r--   0        0        0     1015 2024-05-10 14:04:10.937294 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/ascii_output.py
+-rw-r--r--   0        0        0      403 2024-05-10 14:04:09.821285 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/attribute.py
+-rw-r--r--   0        0        0     1456 2024-05-10 14:04:09.817285 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/attribute_child.py
+-rw-r--r--   0        0        0     1428 2024-05-10 14:04:10.437290 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/automatic_alignment_options.py
+-rw-r--r--   0        0        0     1200 2024-05-10 14:04:10.857293 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/available_ports.py
+-rw-r--r--   0        0        0     1353 2024-05-10 14:04:10.317289 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/avoid_data_reconstruction.py
+-rw-r--r--   0        0        0     1549 2024-05-10 14:04:11.369297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/case_root.py
+-rw-r--r--   0        0        0      419 2024-05-10 14:04:11.353297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/clear_state.py
+-rw-r--r--   0        0        0      471 2024-05-10 14:04:10.841293 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_interface.py
+-rw-r--r--   0        0        0     1089 2024-05-10 14:04:10.837293 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_interface_child.py
+-rw-r--r--   0        0        0      579 2024-05-10 14:04:10.237288 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_participant.py
+-rw-r--r--   0        0        0     5540 2024-05-10 14:04:10.229288 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_participant_child.py
+-rw-r--r--   0        0        0     1118 2024-05-10 14:04:11.437297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/create_restart_point.py
+-rw-r--r--   0        0        0      450 2024-05-10 14:04:10.681292 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/data_transfer.py
+-rw-r--r--   0        0        0     6375 2024-05-10 14:04:10.673292 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/data_transfer_child.py
+-rw-r--r--   0        0        0      509 2024-05-10 14:04:11.341297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/delete_snapshot.py
+-rw-r--r--   0        0        0     1069 2024-05-10 14:04:11.109295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/delete_transformation.py
+-rw-r--r--   0        0        0     2822 2024-05-10 14:04:09.797285 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/dimensionality.py
+-rw-r--r--   0        0        0     6688 2024-05-10 14:04:10.161288 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/execution_control.py
+-rw-r--r--   0        0        0      447 2024-05-10 14:04:09.625284 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/expression.py
+-rw-r--r--   0        0        0     1039 2024-05-10 14:04:09.617284 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_child.py
+-rw-r--r--   0        0        0      510 2024-05-10 14:04:09.661284 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_function.py
+-rw-r--r--   0        0        0     1265 2024-05-10 14:04:09.653284 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_function_child.py
+-rw-r--r--   0        0        0      595 2024-05-10 14:04:10.169288 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/external_data_file.py
+-rw-r--r--   0        0        0     1879 2024-05-10 14:04:10.089287 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/fluent_input.py
+-rw-r--r--   0        0        0      454 2024-05-10 14:04:10.065287 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/fmu_parameter.py
+-rw-r--r--   0        0        0     4880 2024-05-10 14:04:10.057287 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/fmu_parameter_child.py
+-rw-r--r--   0        0        0     1030 2024-05-10 14:04:11.145295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/generate_input_file.py
+-rw-r--r--   0        0        0      660 2024-05-10 14:04:11.137295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_execution_command.py
+-rw-r--r--   0        0        0      227 2024-05-10 14:04:11.453297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_machines.py
+-rw-r--r--   0        0        0      730 2024-05-10 14:04:11.081295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_region_names_for_participant.py
+-rw-r--r--   0        0        0      772 2024-05-10 14:04:11.201296 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_setup_summary.py
+-rw-r--r--   0        0        0      277 2024-05-10 14:04:11.345297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_snapshots.py
+-rw-r--r--   0        0        0     2222 2024-05-10 14:04:11.205296 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_status_messages.py
+-rw-r--r--   0        0        0      999 2024-05-10 14:04:11.445298 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_transformation.py
+-rw-r--r--   0        0        0     4506 2024-05-10 14:04:10.285289 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/global_stabilization.py
+-rw-r--r--   0        0        0      903 2024-05-10 14:04:11.177296 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/has_input_file_changed.py
+-rw-r--r--   0        0        0      993 2024-05-10 14:04:11.149295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/import_system_coupling_input_file.py
+-rw-r--r--   0        0        0     1025 2024-05-10 14:04:11.385297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/initialize.py
+-rw-r--r--   0        0        0      507 2024-05-10 14:04:09.745285 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/instancing.py
+-rw-r--r--   0        0        0     2231 2024-05-10 14:04:09.741285 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/instancing_child.py
+-rw-r--r--   0        0        0      906 2024-05-10 14:04:11.465298 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/interrupt.py
+-rw-r--r--   0        0        0      932 2024-05-10 14:04:09.757285 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/library.py
+-rw-r--r--   0        0        0      486 2024-05-10 14:04:10.961294 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/live_visualization.py
+-rw-r--r--   0        0        0     2250 2024-05-10 14:04:10.953294 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/live_visualization_child.py
+-rw-r--r--   0        0        0     8521 2024-05-10 14:04:10.761292 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/mapping_control.py
+-rw-r--r--   0        0        0     4810 2024-05-10 14:04:11.317297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/open.py
+-rw-r--r--   0        0        0     1903 2024-05-10 14:04:11.421297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/open_results_in_en_sight.py
+-rw-r--r--   0        0        0     1153 2024-05-10 14:04:11.337297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/open_snapshot.py
+-rw-r--r--   0        0        0     4587 2024-05-10 14:04:11.005294 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/output_control.py
+-rw-r--r--   0        0        0     6261 2024-05-10 14:04:11.413297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/partition_participants.py
+-rw-r--r--   0        0        0      476 2024-05-10 14:04:09.721284 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/reference_frame.py
+-rw-r--r--   0        0        0     2421 2024-05-10 14:04:09.713284 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/reference_frame_child.py
+-rw-r--r--   0        0        0      393 2024-05-10 14:04:09.945286 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/region.py
+-rw-r--r--   0        0        0     2238 2024-05-10 14:04:09.941286 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/region_child.py
+-rw-r--r--   0        0        0      357 2024-05-10 14:04:11.173295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/reload_expression_function_modules.py
+-rw-r--r--   0        0        0     2658 2024-05-10 14:04:10.921294 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/results.py
+-rw-r--r--   0        0        0     1684 2024-05-10 14:04:11.321297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/save.py
+-rw-r--r--   0        0        0     1950 2024-05-10 14:04:11.329297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/save_snapshot.py
+-rw-r--r--   0        0        0     6426 2024-05-10 14:04:11.297296 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/setup_root.py
+-rw-r--r--   0        0        0      808 2024-05-10 14:04:11.389297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/shutdown.py
+-rw-r--r--   0        0        0      372 2024-05-10 14:04:10.553291 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/side.py
+-rw-r--r--   0        0        0     1721 2024-05-10 14:04:10.545291 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/side_child.py
+-rw-r--r--   0        0        0     2845 2024-05-10 14:04:10.889293 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/solution_control.py
+-rw-r--r--   0        0        0     2947 2024-05-10 14:04:11.497298 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/solution_root.py
+-rw-r--r--   0        0        0     1057 2024-05-10 14:04:11.457298 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/solve.py
+-rw-r--r--   0        0        0     5536 2024-05-10 14:04:10.609291 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/stabilization.py
+-rw-r--r--   0        0        0     1769 2024-05-10 14:04:11.381297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/start_participants.py
+-rw-r--r--   0        0        0     1986 2024-05-10 14:04:11.401297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/step.py
+-rw-r--r--   0        0        0      509 2024-05-10 14:04:09.689284 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/transformation.py
+-rw-r--r--   0        0        0     1837 2024-05-10 14:04:09.685284 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/transformation_child.py
+-rw-r--r--   0        0        0      879 2024-05-10 14:04:10.901293 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/type.py
+-rw-r--r--   0        0        0     5626 2024-05-10 14:04:10.377289 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/unmapped_value_options.py
+-rw-r--r--   0        0        0     1086 2024-05-10 14:04:09.961286 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/update_control.py
+-rw-r--r--   0        0        0     2211 2024-05-10 14:04:11.129295 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/update_participant.py
+-rw-r--r--   0        0        0      411 2024-05-10 14:04:09.913286 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/variable.py
+-rw-r--r--   0        0        0     7249 2024-05-10 14:04:09.905286 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/variable_child.py
+-rw-r--r--   0        0        0      656 2024-05-10 14:04:11.449298 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/write_csv_chart_files.py
+-rw-r--r--   0        0        0     1278 2024-05-10 14:04:11.433297 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/write_ensight.py
+-rw-r--r--   0        0        0     1198 2024-05-10 14:04:52.433595 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/_add_participant.py
+-rw-r--r--   0        0        0      215 2024-05-10 14:04:52.617596 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/_clear_state.py
+-rw-r--r--   0        0        0      204 2024-05-10 14:04:52.701597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/_solve.py
+-rw-r--r--   0        0        0      858 2024-05-10 14:04:52.773597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/abort.py
+-rw-r--r--   0        0        0     1421 2024-05-10 14:04:50.797583 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/activate_hidden.py
+-rw-r--r--   0        0        0     1113 2024-05-10 14:04:52.413595 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_aerodamping_data_transfers.py
+-rw-r--r--   0        0        0     8249 2024-05-10 14:04:52.277594 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_data_transfer.py
+-rw-r--r--   0        0        0     8168 2024-05-10 14:04:52.301594 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_data_transfer_by_display_names.py
+-rw-r--r--   0        0        0     2044 2024-05-10 14:04:52.481595 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_expression_function.py
+-rw-r--r--   0        0        0      694 2024-05-10 14:04:52.341594 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_fsi_data_transfers.py
+-rw-r--r--   0        0        0     2574 2024-05-10 14:04:52.237594 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_interface.py
+-rw-r--r--   0        0        0     2324 2024-05-10 14:04:52.249594 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_interface_by_display_names.py
+-rw-r--r--   0        0        0     1150 2024-05-10 14:04:52.469595 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_named_expression.py
+-rw-r--r--   0        0        0      735 2024-05-10 14:04:52.421595 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_ordered_data_transfers.py
+-rw-r--r--   0        0        0     5361 2024-05-10 14:04:52.533596 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_participant.py
+-rw-r--r--   0        0        0     1170 2024-05-10 14:04:52.313594 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_reference_frame.py
+-rw-r--r--   0        0        0     1105 2024-05-10 14:04:52.349594 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_thermal_data_transfers.py
+-rw-r--r--   0        0        0     3347 2024-05-10 14:04:52.325594 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_transformation.py
+-rw-r--r--   0        0        0    10857 2024-05-10 14:04:51.765590 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/analysis_control.py
+-rw-r--r--   0        0        0      839 2024-05-10 14:04:51.537589 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/apip.py
+-rw-r--r--   0        0        0     1015 2024-05-10 14:04:52.157593 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/ascii_output.py
+-rw-r--r--   0        0        0      403 2024-05-10 14:04:51.009585 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/attribute.py
+-rw-r--r--   0        0        0     1456 2024-05-10 14:04:51.005585 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/attribute_child.py
+-rw-r--r--   0        0        0     1428 2024-05-10 14:04:51.665590 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/automatic_alignment_options.py
+-rw-r--r--   0        0        0     1200 2024-05-10 14:04:52.069593 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/available_ports.py
+-rw-r--r--   0        0        0     1353 2024-05-10 14:04:51.557589 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/avoid_data_reconstruction.py
+-rw-r--r--   0        0        0     1378 2024-05-10 14:04:52.677597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/case_root.py
+-rw-r--r--   0        0        0      419 2024-05-10 14:04:52.661597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/clear_state.py
+-rw-r--r--   0        0        0      471 2024-05-10 14:04:52.053592 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_interface.py
+-rw-r--r--   0        0        0     1089 2024-05-10 14:04:52.049592 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_interface_child.py
+-rw-r--r--   0        0        0      579 2024-05-10 14:04:51.477588 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_participant.py
+-rw-r--r--   0        0        0     8720 2024-05-10 14:04:51.469588 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_participant_child.py
+-rw-r--r--   0        0        0     1118 2024-05-10 14:04:52.741597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/create_restart_point.py
+-rw-r--r--   0        0        0      450 2024-05-10 14:04:51.917591 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/data_transfer.py
+-rw-r--r--   0        0        0     6375 2024-05-10 14:04:51.909591 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/data_transfer_child.py
+-rw-r--r--   0        0        0      509 2024-05-10 14:04:52.653596 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/delete_snapshot.py
+-rw-r--r--   0        0        0     1069 2024-05-10 14:04:52.333594 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/delete_transformation.py
+-rw-r--r--   0        0        0     2822 2024-05-10 14:04:50.985585 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/dimensionality.py
+-rw-r--r--   0        0        0     7049 2024-05-10 14:04:51.357587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/execution_control.py
+-rw-r--r--   0        0        0      447 2024-05-10 14:04:50.817584 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/expression.py
+-rw-r--r--   0        0        0     1039 2024-05-10 14:04:50.809584 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/expression_child.py
+-rw-r--r--   0        0        0      510 2024-05-10 14:04:50.849584 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/expression_function.py
+-rw-r--r--   0        0        0     1265 2024-05-10 14:04:50.845584 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/expression_function_child.py
+-rw-r--r--   0        0        0      595 2024-05-10 14:04:51.365588 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/external_data_file.py
+-rw-r--r--   0        0        0     1879 2024-05-10 14:04:51.281587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/fluent_input.py
+-rw-r--r--   0        0        0      454 2024-05-10 14:04:51.261587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/fmu_parameter.py
+-rw-r--r--   0        0        0     4880 2024-05-10 14:04:51.253587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/fmu_parameter_child.py
+-rw-r--r--   0        0        0     1030 2024-05-10 14:04:52.457595 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/generate_input_file.py
+-rw-r--r--   0        0        0      617 2024-05-10 14:04:52.489596 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_add_data_transfer_group_commands.py
+-rw-r--r--   0        0        0      660 2024-05-10 14:04:52.449595 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_execution_command.py
+-rw-r--r--   0        0        0      227 2024-05-10 14:04:52.757597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_machines.py
+-rw-r--r--   0        0        0      604 2024-05-10 14:04:52.505596 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_mode_shape_variables.py
+-rw-r--r--   0        0        0      730 2024-05-10 14:04:52.309594 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_region_names_for_participant.py
+-rw-r--r--   0        0        0      772 2024-05-10 14:04:52.541596 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_setup_summary.py
+-rw-r--r--   0        0        0     2222 2024-05-10 14:04:52.545596 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_status_messages.py
+-rw-r--r--   0        0        0      829 2024-05-10 14:04:52.497595 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_thermal_data_transfer_options.py
+-rw-r--r--   0        0        0      999 2024-05-10 14:04:52.749597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_transformation.py
+-rw-r--r--   0        0        0     4506 2024-05-10 14:04:51.525589 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/global_stabilization.py
+-rw-r--r--   0        0        0      909 2024-05-10 14:04:52.513596 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/has_input_file_changed.py
+-rw-r--r--   0        0        0      993 2024-05-10 14:04:52.461595 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/import_system_coupling_input_file.py
+-rw-r--r--   0        0        0     1025 2024-05-10 14:04:52.689597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/initialize.py
+-rw-r--r--   0        0        0      507 2024-05-10 14:04:50.933584 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/instancing.py
+-rw-r--r--   0        0        0     2231 2024-05-10 14:04:50.929584 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/instancing_child.py
+-rw-r--r--   0        0        0      906 2024-05-10 14:04:52.769597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/interrupt.py
+-rw-r--r--   0        0        0      932 2024-05-10 14:04:50.945584 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/library.py
+-rw-r--r--   0        0        0      486 2024-05-10 14:04:52.181593 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/live_visualization.py
+-rw-r--r--   0        0        0     2250 2024-05-10 14:04:52.177593 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/live_visualization_child.py
+-rw-r--r--   0        0        0     8900 2024-05-10 14:04:52.033592 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/mapping_control.py
+-rw-r--r--   0        0        0     4810 2024-05-10 14:04:52.625596 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/open.py
+-rw-r--r--   0        0        0     1902 2024-05-10 14:04:52.729597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/open_results_in_ensight.py
+-rw-r--r--   0        0        0     1153 2024-05-10 14:04:52.649597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/open_snapshot.py
+-rw-r--r--   0        0        0     4587 2024-05-10 14:04:52.225594 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/output_control.py
+-rw-r--r--   0        0        0      420 2024-05-10 14:04:51.125586 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/parameter.py
+-rw-r--r--   0        0        0     1686 2024-05-10 14:04:51.121586 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/parameter_child.py
+-rw-r--r--   0        0        0     6261 2024-05-10 14:04:52.721597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/partition_participants.py
+-rw-r--r--   0        0        0     1091 2024-05-10 14:04:51.381588 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/record_interactions.py
+-rw-r--r--   0        0        0      476 2024-05-10 14:04:50.909584 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/reference_frame.py
+-rw-r--r--   0        0        0     2421 2024-05-10 14:04:50.905584 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/reference_frame_child.py
+-rw-r--r--   0        0        0      393 2024-05-10 14:04:51.161586 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/region.py
+-rw-r--r--   0        0        0     2252 2024-05-10 14:04:51.153586 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/region_child.py
+-rw-r--r--   0        0        0      357 2024-05-10 14:04:52.485595 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/reload_expression_function_modules.py
+-rw-r--r--   0        0        0     2658 2024-05-10 14:04:52.145593 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/results.py
+-rw-r--r--   0        0        0     1684 2024-05-10 14:04:52.633597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/save.py
+-rw-r--r--   0        0        0     1950 2024-05-10 14:04:52.641596 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/save_snapshot.py
+-rw-r--r--   0        0        0     8420 2024-05-10 14:04:52.609596 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/setup_root.py
+-rw-r--r--   0        0        0      808 2024-05-10 14:04:52.693597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/shutdown.py
+-rw-r--r--   0        0        0      372 2024-05-10 14:04:51.793590 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/side.py
+-rw-r--r--   0        0        0     1721 2024-05-10 14:04:51.789590 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/side_child.py
+-rw-r--r--   0        0        0     4048 2024-05-10 14:04:52.109593 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/solution_control.py
+-rw-r--r--   0        0        0     2940 2024-05-10 14:04:52.801598 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/solution_root.py
+-rw-r--r--   0        0        0     1057 2024-05-10 14:04:52.761597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/solve.py
+-rw-r--r--   0        0        0     5536 2024-05-10 14:04:51.849591 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/stabilization.py
+-rw-r--r--   0        0        0     1764 2024-05-10 14:04:52.685597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/start_participants.py
+-rw-r--r--   0        0        0     1986 2024-05-10 14:04:52.705597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/step.py
+-rw-r--r--   0        0        0      509 2024-05-10 14:04:50.877584 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/transformation.py
+-rw-r--r--   0        0        0     1837 2024-05-10 14:04:50.873584 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/transformation_child.py
+-rw-r--r--   0        0        0      879 2024-05-10 14:04:52.125593 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/type.py
+-rw-r--r--   0        0        0     5626 2024-05-10 14:04:51.649589 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/unmapped_value_options.py
+-rw-r--r--   0        0        0     1086 2024-05-10 14:04:51.173586 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/update_control.py
+-rw-r--r--   0        0        0     2341 2024-05-10 14:04:52.441595 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/update_participant.py
+-rw-r--r--   0        0        0      411 2024-05-10 14:04:51.097586 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/variable.py
+-rw-r--r--   0        0        0     7234 2024-05-10 14:04:51.093586 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/variable_child.py
+-rw-r--r--   0        0        0      656 2024-05-10 14:04:52.753597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/write_csv_chart_files.py
+-rw-r--r--   0        0        0     1278 2024-05-10 14:04:52.737597 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/write_ensight.py
+-rw-r--r--   0        0        0     1374 2024-05-10 14:05:45.541971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/_add_participant.py
+-rw-r--r--   0        0        0      215 2024-05-10 14:05:45.717972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/_clear_state.py
+-rw-r--r--   0        0        0      204 2024-05-10 14:05:45.797973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/_solve.py
+-rw-r--r--   0        0        0      858 2024-05-10 14:05:45.881974 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/abort.py
+-rw-r--r--   0        0        0     1421 2024-05-10 14:05:43.805958 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/activate_hidden.py
+-rw-r--r--   0        0        0     1113 2024-05-10 14:05:45.521971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/add_aerodamping_data_transfers.py
+-rw-r--r--   0        0        0     8251 2024-05-10 14:05:45.433970 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/add_data_transfer.py
+-rw-r--r--   0        0        0     8168 2024-05-10 14:05:45.457970 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/add_data_transfer_by_display_names.py
+-rw-r--r--   0        0        0     2044 2024-05-10 14:05:45.589971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/add_expression_function.py
+-rw-r--r--   0        0        0     1079 2024-05-10 14:05:45.505971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/add_fsi_data_transfers.py
+-rw-r--r--   0        0        0     2574 2024-05-10 14:05:45.329970 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/add_interface.py
+-rw-r--r--   0        0        0     2324 2024-05-10 14:05:45.413970 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/add_interface_by_display_names.py
+-rw-r--r--   0        0        0     1150 2024-05-10 14:05:45.577971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/add_named_expression.py
+-rw-r--r--   0        0        0      735 2024-05-10 14:05:45.525971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/add_ordered_data_transfers.py
+-rw-r--r--   0        0        0     6389 2024-05-10 14:05:45.641972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/add_participant.py
+-rw-r--r--   0        0        0     1170 2024-05-10 14:05:45.469971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/add_reference_frame.py
+-rw-r--r--   0        0        0     1105 2024-05-10 14:05:45.513971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/add_thermal_data_transfers.py
+-rw-r--r--   0        0        0     3347 2024-05-10 14:05:45.485971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/add_transformation.py
+-rw-r--r--   0        0        0    10857 2024-05-10 14:05:44.825966 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/analysis_control.py
+-rw-r--r--   0        0        0      839 2024-05-10 14:05:44.621964 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/apip.py
+-rw-r--r--   0        0        0     1015 2024-05-10 14:05:45.229969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/ascii_output.py
+-rw-r--r--   0        0        0      403 2024-05-10 14:05:44.017960 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/attribute.py
+-rw-r--r--   0        0        0     1456 2024-05-10 14:05:44.013960 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/attribute_child.py
+-rw-r--r--   0        0        0     1428 2024-05-10 14:05:44.721965 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/automatic_alignment_options.py
+-rw-r--r--   0        0        0     1200 2024-05-10 14:05:45.141968 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/available_ports.py
+-rw-r--r--   0        0        0     1353 2024-05-10 14:05:44.641964 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/avoid_data_reconstruction.py
+-rw-r--r--   0        0        0     1378 2024-05-10 14:05:45.777973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/case_root.py
+-rw-r--r--   0        0        0      419 2024-05-10 14:05:45.761973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/clear_state.py
+-rw-r--r--   0        0        0     1180 2024-05-10 14:05:45.813973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/connect_ensight_dvs.py
+-rw-r--r--   0        0        0      471 2024-05-10 14:05:45.129968 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/coupling_interface.py
+-rw-r--r--   0        0        0     1089 2024-05-10 14:05:45.121968 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/coupling_interface_child.py
+-rw-r--r--   0        0        0      579 2024-05-10 14:05:44.525963 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/coupling_participant.py
+-rw-r--r--   0        0        0     8961 2024-05-10 14:05:44.521963 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/coupling_participant_child.py
+-rw-r--r--   0        0        0     1118 2024-05-10 14:05:45.849973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/create_restart_point.py
+-rw-r--r--   0        0        0      450 2024-05-10 14:05:45.025967 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/data_transfer.py
+-rw-r--r--   0        0        0     6375 2024-05-10 14:05:45.017967 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/data_transfer_child.py
+-rw-r--r--   0        0        0      509 2024-05-10 14:05:45.757973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/delete_snapshot.py
+-rw-r--r--   0        0        0     1069 2024-05-10 14:05:45.493971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/delete_transformation.py
+-rw-r--r--   0        0        0     2822 2024-05-10 14:05:43.993960 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/dimensionality.py
+-rw-r--r--   0        0        0     9047 2024-05-10 14:05:44.401963 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/execution_control.py
+-rw-r--r--   0        0        0      556 2024-05-10 14:05:45.241969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/execution_control_1.py
+-rw-r--r--   0        0        0      447 2024-05-10 14:05:43.825958 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/expression.py
+-rw-r--r--   0        0        0     1039 2024-05-10 14:05:43.817958 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/expression_child.py
+-rw-r--r--   0        0        0      510 2024-05-10 14:05:43.861959 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/expression_function.py
+-rw-r--r--   0        0        0     1265 2024-05-10 14:05:43.857958 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/expression_function_child.py
+-rw-r--r--   0        0        0      595 2024-05-10 14:05:44.413963 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/external_data_file.py
+-rw-r--r--   0        0        0     2290 2024-05-10 14:05:44.305962 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/fluent_input.py
+-rw-r--r--   0        0        0      454 2024-05-10 14:05:44.281962 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/fmu_parameter.py
+-rw-r--r--   0        0        0     4880 2024-05-10 14:05:44.273962 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/fmu_parameter_child.py
+-rw-r--r--   0        0        0     1030 2024-05-10 14:05:45.565971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/generate_input_file.py
+-rw-r--r--   0        0        0      617 2024-05-10 14:05:45.597972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/get_add_data_transfer_group_commands.py
+-rw-r--r--   0        0        0      660 2024-05-10 14:05:45.557971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/get_execution_command.py
+-rw-r--r--   0        0        0      227 2024-05-10 14:05:45.865973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/get_machines.py
+-rw-r--r--   0        0        0      604 2024-05-10 14:05:45.613972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/get_mode_shape_variables.py
+-rw-r--r--   0        0        0      730 2024-05-10 14:05:45.465970 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/get_region_names_for_participant.py
+-rw-r--r--   0        0        0      772 2024-05-10 14:05:45.645972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/get_setup_summary.py
+-rw-r--r--   0        0        0     2222 2024-05-10 14:05:45.649972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/get_status_messages.py
+-rw-r--r--   0        0        0      304 2024-05-10 14:05:45.617972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/get_supported_participant_types.py
+-rw-r--r--   0        0        0      829 2024-05-10 14:05:45.605971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/get_thermal_data_transfer_options.py
+-rw-r--r--   0        0        0     1000 2024-05-10 14:05:45.857973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/get_transformation.py
+-rw-r--r--   0        0        0     4506 2024-05-10 14:05:44.609964 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/global_stabilization.py
+-rw-r--r--   0        0        0      909 2024-05-10 14:05:45.621972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/has_input_file_changed.py
+-rw-r--r--   0        0        0      993 2024-05-10 14:05:45.569971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/import_system_coupling_input_file.py
+-rw-r--r--   0        0        0     1025 2024-05-10 14:05:45.789973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/initialize.py
+-rw-r--r--   0        0        0      507 2024-05-10 14:05:43.945959 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/instancing.py
+-rw-r--r--   0        0        0     2231 2024-05-10 14:05:43.937959 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/instancing_child.py
+-rw-r--r--   0        0        0      906 2024-05-10 14:05:45.877973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/interrupt.py
+-rw-r--r--   0        0        0      932 2024-05-10 14:05:43.953959 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/library.py
+-rw-r--r--   0        0        0      486 2024-05-10 14:05:45.273969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/live_visualization.py
+-rw-r--r--   0        0        0     3258 2024-05-10 14:05:45.269969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/live_visualization_child.py
+-rw-r--r--   0        0        0     8900 2024-05-10 14:05:45.109968 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/mapping_control.py
+-rw-r--r--   0        0        0     4810 2024-05-10 14:05:45.729972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/open.py
+-rw-r--r--   0        0        0     1902 2024-05-10 14:05:45.837973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/open_results_in_ensight.py
+-rw-r--r--   0        0        0     1153 2024-05-10 14:05:45.749973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/open_snapshot.py
+-rw-r--r--   0        0        0     4587 2024-05-10 14:05:45.317969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/output_control.py
+-rw-r--r--   0        0        0      420 2024-05-10 14:05:44.133961 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/parameter.py
+-rw-r--r--   0        0        0     1686 2024-05-10 14:05:44.129960 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/parameter_child.py
+-rw-r--r--   0        0        0     6261 2024-05-10 14:05:45.829973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/partition_participants.py
+-rw-r--r--   0        0        0     1036 2024-05-10 14:05:44.181961 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/properties.py
+-rw-r--r--   0        0        0     1469 2024-05-10 14:05:44.429963 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/record_interactions.py
+-rw-r--r--   0        0        0      476 2024-05-10 14:05:43.921959 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/reference_frame.py
+-rw-r--r--   0        0        0     2421 2024-05-10 14:05:43.913959 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/reference_frame_child.py
+-rw-r--r--   0        0        0      393 2024-05-10 14:05:44.165961 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/region.py
+-rw-r--r--   0        0        0     2204 2024-05-10 14:05:44.161961 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/region_child.py
+-rw-r--r--   0        0        0      357 2024-05-10 14:05:45.593971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/reload_expression_function_modules.py
+-rw-r--r--   0        0        0     2658 2024-05-10 14:05:45.217969 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/results.py
+-rw-r--r--   0        0        0     1684 2024-05-10 14:05:45.733972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/save.py
+-rw-r--r--   0        0        0     1950 2024-05-10 14:05:45.745972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/save_snapshot.py
+-rw-r--r--   0        0        0     8734 2024-05-10 14:05:45.709972 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/setup_root.py
+-rw-r--r--   0        0        0      808 2024-05-10 14:05:45.793973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/shutdown.py
+-rw-r--r--   0        0        0      372 2024-05-10 14:05:44.853966 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/side.py
+-rw-r--r--   0        0        0     1721 2024-05-10 14:05:44.849966 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/side_child.py
+-rw-r--r--   0        0        0     4048 2024-05-10 14:05:45.181968 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/solution_control.py
+-rw-r--r--   0        0        0     3157 2024-05-10 14:05:45.909974 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/solution_root.py
+-rw-r--r--   0        0        0     1057 2024-05-10 14:05:45.869974 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/solve.py
+-rw-r--r--   0        0        0     5536 2024-05-10 14:05:44.909966 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/stabilization.py
+-rw-r--r--   0        0        0     1764 2024-05-10 14:05:45.785973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/start_participants.py
+-rw-r--r--   0        0        0     1986 2024-05-10 14:05:45.805973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/step.py
+-rw-r--r--   0        0        0      509 2024-05-10 14:05:43.889959 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/transformation.py
+-rw-r--r--   0        0        0     1837 2024-05-10 14:05:43.881959 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/transformation_child.py
+-rw-r--r--   0        0        0      879 2024-05-10 14:05:45.197968 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/type.py
+-rw-r--r--   0        0        0     5626 2024-05-10 14:05:44.705965 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/unmapped_value_options.py
+-rw-r--r--   0        0        0     1049 2024-05-10 14:05:44.193961 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/update_control.py
+-rw-r--r--   0        0        0     2341 2024-05-10 14:05:45.549971 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/update_participant.py
+-rw-r--r--   0        0        0      411 2024-05-10 14:05:44.105960 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/variable.py
+-rw-r--r--   0        0        0     7234 2024-05-10 14:05:44.097960 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/variable_child.py
+-rw-r--r--   0        0        0      656 2024-05-10 14:05:45.861973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/write_csv_chart_files.py
+-rw-r--r--   0        0        0     1278 2024-05-10 14:05:45.845973 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_2/write_ensight.py
+-rw-r--r--   0        0        0     4210 2024-05-10 14:02:43.500587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/get_status_messages.py
+-rw-r--r--   0        0        0     2489 2024-05-10 14:02:43.500587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/get_syc_version.py
+-rw-r--r--   0        0        0    12693 2024-05-10 14:02:43.500587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/injected_commands.py
+-rw-r--r--   0        0        0    12828 2024-05-10 14:02:43.500587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/root_source.py
+-rw-r--r--   0        0        0    14927 2024-05-10 14:02:43.500587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/static_info.py
+-rw-r--r--   0        0        0     4784 2024-05-10 14:02:43.500587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy.py
+-rw-r--r--   0        0        0     2281 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy_interface.py
+-rw-r--r--   0        0        0    25130 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/types.py
+-rw-r--r--   0        0        0    14735 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/grpc_client.py
+-rw-r--r--   0        0        0     2256 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/services/command_query.py
+-rw-r--r--   0        0        0     2148 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/services/output_stream.py
+-rw-r--r--   0        0        0     1683 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/services/process.py
+-rw-r--r--   0        0        0     2518 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/services/solution.py
+-rw-r--r--   0        0        0     2752 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/syc_container.py
+-rw-r--r--   0        0        0     5635 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/syc_process.py
+-rw-r--r--   0        0        0     3064 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/variant.py
+-rw-r--r--   0        0        0     1223 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/examples/__init__.py
+-rw-r--r--   0        0        0     4101 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/examples/downloads.py
+-rw-r--r--   0        0        0     1188 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/native_api/__init__.py
+-rw-r--r--   0        0        0     1734 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/native_api/command_metadata.py
+-rw-r--r--   0        0        0     4836 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/native_api/datamodel_metadata.py
+-rw-r--r--   0        0        0     1462 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/native_api/meta_wrapper.py
+-rw-r--r--   0        0        0     7116 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/native_api/native_api.py
+-rw-r--r--   0        0        0     4153 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/native_api/object_path.py
+-rw-r--r--   0        0        0     8839 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/participant/manager.py
+-rw-r--r--   0        0        0    11166 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/participant/mapdl.py
+-rw-r--r--   0        0        0     2427 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/participant/protocol.py
+-rw-r--r--   0        0        0    10219 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/session.py
+-rw-r--r--   0        0        0     3783 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/syc_version.py
+-rw-r--r--   0        0        0     5186 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/util/file_transfer.py
+-rw-r--r--   0        0        0     5059 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/util/logging.py
+-rw-r--r--   0        0        0     1470 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/util/name_util.py
+-rw-r--r--   0        0        0     1941 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/util/pathstr.py
+-rw-r--r--   0        0        0     4545 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/util/state_keys.py
+-rw-r--r--   0        0        0     2982 2024-05-10 14:02:43.504587 ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/util/yaml_helper.py
+-rw-r--r--   0        0        0    10946 1970-01-01 00:00:00.000000 ansys_systemcoupling_core-0.5.0/PKG-INFO
```

### Comparing `ansys_systemcoupling_core-0.4.1/LICENSE` & `ansys_systemcoupling_core-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/README.rst` & `ansys_systemcoupling_core-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/pyproject.toml` & `ansys_systemcoupling_core-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-systemcoupling-core"
-version = "0.4.1"
+version = "0.5.0"
 description = "A Python wrapper for Ansys System Coupling."
 readme = "README.rst"
 requires-python = ">=3.9,<3.13"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.support@ansys.com"},
 ]
 maintainers = [
     {name = "PyAnsys developers", email = "pyansys.maintainers@ansys.com"},
 ]
 dependencies = [
 	"ansys-api-systemcoupling==0.1.0",
         "ansys-platform-instancemanagement~=1.0",
 	"grpcio>=1.30.0",
-	"grpcio-status>=1.30.0,<1.60.2",
+	"grpcio-status>=1.30.0,<1.62.2",
 	"googleapis-common-protos>=1.50.0",
 	"protobuf>=3.20.1,<4.0.0",
 	"psutil>=5.7.0",
 	"pyyaml",
 	"appdirs>=1.4.0",
 	"importlib-metadata>=4.0",
 ]
@@ -47,31 +47,31 @@
 	"build",
 ]
 classesgen = [
 	# Dependencies for API class generation from System Coupling metadata
 
 	# NB
 	# black and isort are called programmatically to keep generated code
-	# consistent with style elsewhere. We need to keep the versions in
+	# consistent with style elsewhere. We need to keep these versions in
 	# sync with the precommit dependencies.
-	"black==24.1.1",
+	"black==24.4.2",
 	"isort==5.13.2",
 ]
 doc = [
-	"ansys-sphinx-theme==0.13.3",
+	"ansys-sphinx-theme==0.15.2",
 	"jupyter_sphinx==0.5.3",
 	"matplotlib",
-	"numpydoc==1.6.0",
-	"pypandoc==1.12",
-	"pytest-sphinx==0.6.0",
+	"numpydoc==1.7.0",
+	"pypandoc==1.13",
+	"pytest-sphinx==0.6.3",
 	"Sphinx==7.2.6",
-	"sphinx-autobuild==2024.2.4",
-	"sphinx-autodoc-typehints==1.25.2",
+	"sphinx-autobuild==2024.4.16",
+	"sphinx-autodoc-typehints==2.0.1",
 	"sphinx-copybutton==0.5.2",
-	"sphinx-gallery==0.15.0",
+	"sphinx-gallery==0.16.0",
 	"sphinx-notfound-page==1.0.0",
 	"sphinxcontrib-websupport==1.2.7",
 	"sphinxemoji==0.3.1",
 
 	# pyansys dependencies for sphinx gallery examples
 	"ansys-fluent-core",
 	"ansys-dpf-core",
```

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/__init__.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/_version.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/_version.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/_add_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/_add_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/abort.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/abort.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/activate_hidden.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/activate_hidden.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_data_transfer.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_data_transfer.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_data_transfer_by_display_names.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_data_transfer_by_display_names.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_expression_function.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_expression_function.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_interface.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_interface.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_interface_by_display_names.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_interface_by_display_names.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_named_expression.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_named_expression.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_reference_frame.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_reference_frame.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/add_transformation.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/add_transformation.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/analysis_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/analysis_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/apip.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/apip.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/ascii_output.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/ascii_output.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/attribute_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/attribute_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/available_ports.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/available_ports.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/avoid_data_reconstruction.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/avoid_data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_interface_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_interface_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_participant_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/coupling_participant_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/create_restart_point.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/create_restart_point.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/data_transfer_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/data_transfer_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/delete_transformation.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/delete_transformation.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/dimensionality.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/dimensionality.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/execution_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/execution_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_function_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/expression_function_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/external_data_file.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/external_data_file.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/fluent_input.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/fluent_input.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/fmu_parameter_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/fmu_parameter_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/generate_input_file.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/generate_input_file.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/get_execution_command.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/get_execution_command.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/get_region_names_for_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/get_region_names_for_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/get_setup_summary.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/get_setup_summary.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/get_status_messages.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/get_status_messages.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/global_stabilization.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/global_stabilization.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/has_input_file_changed.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/has_input_file_changed.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/import_system_coupling_input_file.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/import_system_coupling_input_file.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/initialize.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/initialize.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/instancing_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/instancing_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/interrupt.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/interrupt.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/library.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/library.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/mapping_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/mapping_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/open.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/open.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/open_results_in_ensight.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/open_results_in_ensight.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/open_snapshot.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/open_snapshot.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/output_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/output_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/partition_participants.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/partition_participants.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/reference_frame_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/reference_frame_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/region_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/region_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/results.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/results.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/save.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/save.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/save_snapshot.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/save_snapshot.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/setup_root.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/setup_root.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/shutdown.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/shutdown.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/side_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/side_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/solution_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/solution_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/solution_root.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/solution_root.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/solve.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/solve.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/stabilization.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/stabilization.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/start_participants.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/start_participants.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/step.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/step.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/transformation_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/transformation_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/type.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/type.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/unmapped_value_options.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/unmapped_value_options.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/update_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/update_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/update_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/update_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/variable_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/variable_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/write_csv_chart_files.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/write_csv_chart_files.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_1/write_ensight.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/write_ensight.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/_add_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/_add_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/abort.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/abort.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/activate_hidden.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/activate_hidden.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_data_transfer.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_data_transfer.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_data_transfer_by_display_names.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_data_transfer_by_display_names.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_expression_function.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_expression_function.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_interface.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_interface.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_interface_by_display_names.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_interface_by_display_names.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_named_expression.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_named_expression.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_reference_frame.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_reference_frame.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/add_transformation.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/add_transformation.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/analysis_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/analysis_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/apip.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/apip.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/ascii_output.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/ascii_output.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/attribute_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/attribute_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/automatic_alignment_options.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/automatic_alignment_options.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/available_ports.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/available_ports.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/avoid_data_reconstruction.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/avoid_data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_interface_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_interface_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_participant_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/coupling_participant_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/create_restart_point.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/create_restart_point.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/data_transfer_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/data_transfer_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/delete_transformation.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/delete_transformation.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/dimensionality.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/dimensionality.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/execution_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/execution_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_function_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/expression_function_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/external_data_file.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/external_data_file.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/fluent_input.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/fluent_input.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/fmu_parameter_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/fmu_parameter_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/generate_input_file.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/generate_input_file.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/get_execution_command.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_execution_command.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/get_region_names_for_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_region_names_for_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/get_setup_summary.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_setup_summary.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/get_status_messages.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_status_messages.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/get_transformation.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/get_transformation.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/global_stabilization.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/global_stabilization.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/has_input_file_changed.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/has_input_file_changed.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/import_system_coupling_input_file.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/import_system_coupling_input_file.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/initialize.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/initialize.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/instancing_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/instancing_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/interrupt.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/interrupt.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/library.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/library.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/live_visualization_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/live_visualization_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/mapping_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/mapping_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/open.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/open.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/open_results_in_en_sight.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/open_results_in_en_sight.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/open_snapshot.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/open_snapshot.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/output_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/output_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/partition_participants.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/partition_participants.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/reference_frame_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/reference_frame_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/region_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/region_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/results.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/results.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/save.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/save.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/save_snapshot.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/save_snapshot.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/setup_root.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/setup_root.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/shutdown.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/shutdown.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/side_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/side_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/solution_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/solution_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/solution_root.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/solution_root.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/solve.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/solve.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/stabilization.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/stabilization.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/start_participants.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/start_participants.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/step.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/step.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/transformation_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/transformation_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/type.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/type.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/unmapped_value_options.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/unmapped_value_options.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/update_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/update_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/update_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/update_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/variable_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/variable_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/write_csv_chart_files.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/write_csv_chart_files.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_23_2/write_ensight.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_2/write_ensight.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/_add_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/_add_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/abort.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/abort.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/activate_hidden.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/activate_hidden.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_aerodamping_data_transfers.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_aerodamping_data_transfers.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_data_transfer.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_data_transfer.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_data_transfer_by_display_names.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_data_transfer_by_display_names.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_expression_function.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_expression_function.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_fsi_data_transfers.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_fsi_data_transfers.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_interface.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_interface.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_interface_by_display_names.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_interface_by_display_names.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_named_expression.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_named_expression.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_ordered_data_transfers.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_ordered_data_transfers.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_reference_frame.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_reference_frame.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_thermal_data_transfers.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_thermal_data_transfers.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/add_transformation.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/add_transformation.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/analysis_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/analysis_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/apip.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/apip.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/ascii_output.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/ascii_output.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/attribute_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/attribute_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/automatic_alignment_options.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/automatic_alignment_options.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/available_ports.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/available_ports.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/avoid_data_reconstruction.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/avoid_data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/case_root.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_23_1/case_root.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,59 @@
 #
 # This is an auto-generated file.  DO NOT EDIT!
 #
 
-SHASH = "430648f7df949b91819d62a5c2d5a5c49d1d67217fb3474ee31e0c78e5ffbd43"
+SHASH = "c6427eb39292f21707811cf7093268eb2b0d3d9f2780ddaf390bf51bb916e546"
 
 from ansys.systemcoupling.core.adaptor.impl.types import *
 
+from ._clear_state import _clear_state
 from .clear_state import clear_state
 from .delete_snapshot import delete_snapshot
+from .get_snapshots import get_snapshots
 from .open import open
 from .open_snapshot import open_snapshot
 from .save import save
 from .save_snapshot import save_snapshot
 
 
 class case_root(Container):
     """
     'root' object
     """
 
     syc_name = "CaseCommands"
 
     command_names = [
+        "_clear_state",
         "clear_state",
         "delete_snapshot",
+        "get_snapshots",
         "open",
         "open_snapshot",
         "save",
         "save_snapshot",
     ]
 
+    _clear_state: _clear_state = _clear_state
+    """
+    _clear_state command of case_root.
+    """
     clear_state: clear_state = clear_state
     """
     clear_state command of case_root.
     """
     delete_snapshot: delete_snapshot = delete_snapshot
     """
     delete_snapshot command of case_root.
     """
+    get_snapshots: get_snapshots = get_snapshots
+    """
+    get_snapshots command of case_root.
+    """
     open: open = open
     """
     open command of case_root.
     """
     open_snapshot: open_snapshot = open_snapshot
     """
     open_snapshot command of case_root.
```

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_interface_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_interface_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_participant_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/coupling_participant_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/create_restart_point.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/create_restart_point.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/data_transfer_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/data_transfer_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/delete_transformation.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/delete_transformation.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/dimensionality.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/dimensionality.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/execution_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/execution_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/expression_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/expression_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/expression_function_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/expression_function_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/external_data_file.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/external_data_file.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/fluent_input.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/fluent_input.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/fmu_parameter_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/fmu_parameter_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/generate_input_file.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/generate_input_file.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_add_data_transfer_group_commands.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_add_data_transfer_group_commands.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_execution_command.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_execution_command.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_mode_shape_variables.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_mode_shape_variables.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_region_names_for_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_region_names_for_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_setup_summary.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_setup_summary.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_status_messages.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_status_messages.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_thermal_data_transfer_options.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_thermal_data_transfer_options.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/get_transformation.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/get_transformation.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/global_stabilization.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/global_stabilization.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/has_input_file_changed.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/has_input_file_changed.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/import_system_coupling_input_file.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/import_system_coupling_input_file.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/initialize.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/initialize.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/instancing_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/instancing_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/interrupt.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/interrupt.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/library.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/library.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/live_visualization_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/live_visualization_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/mapping_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/mapping_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/open.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/open.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/open_results_in_ensight.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/open_results_in_ensight.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/open_snapshot.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/open_snapshot.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/output_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/output_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/parameter_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/parameter_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/partition_participants.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/partition_participants.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/record_interactions.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/record_interactions.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/reference_frame_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/reference_frame_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/region_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/region_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/results.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/results.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/save.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/save.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/save_snapshot.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/save_snapshot.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/setup_root.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/setup_root.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/shutdown.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/shutdown.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/side_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/side_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/solution_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/solution_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/solution_root.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/solution_root.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/solve.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/solve.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/stabilization.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/stabilization.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/start_participants.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/start_participants.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/step.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/step.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/transformation_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/transformation_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/type.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/type.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/unmapped_value_options.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/unmapped_value_options.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/update_control.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/update_control.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/update_participant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/update_participant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/variable_child.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/variable_child.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/write_csv_chart_files.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/write_csv_chart_files.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/api_24_1/write_ensight.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/api_24_1/write_ensight.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/get_status_messages.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/get_status_messages.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/get_syc_version.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/get_syc_version.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/injected_commands.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/injected_commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,21 @@
     if category == "solution":
         ret = {
             "solve": lambda **kwargs: _wrap_solve(root_object, part_mgr, **kwargs),
             "interrupt": lambda **kwargs: rpc.interrupt(**kwargs),
             "abort": lambda **kwargs: rpc.abort(**kwargs),
         }
 
+    if category == "case":
+        ret = {
+            "clear_state": lambda **kwargs: _wrap_clear_state(
+                root_object, part_mgr, **kwargs
+            )
+        }
+
     return ret
 
 
 def _wrap_add_participant(
     server_version: str, root_object: Container, part_mgr: ParticipantManager, **kwargs
 ) -> str:
     if session := kwargs.get("participant_session", None):
@@ -98,14 +105,21 @@
             )
 
         return part_mgr.add_participant(participant_session=session.system_coupling)
 
     return root_object._add_participant(**kwargs)
 
 
+def _wrap_clear_state(
+    root_object: Container, part_mgr: ParticipantManager, **kwargs
+) -> None:
+    part_mgr.clear()
+    root_object._clear_state(**kwargs)
+
+
 def _wrap_solve(root_object: Container, part_mgr: ParticipantManager) -> None:
     if part_mgr is None:
         root_object._solve()
     else:
         part_mgr.solve()
 
 
@@ -305,8 +319,12 @@
 
         ``'coupling_interface["Interface-1"].mapping_control.absolute_gap_tolerance'``
 
 
     essentialArgNames: []
     optionalArgNames: []
     args: []
+-   name: ClearState
+    pyname: clear_state
+    isInjected: true
+    pysyc_internal_name: _clear_state
 """
```

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/root_source.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/root_source.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/static_info.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/static_info.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy_interface.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/syc_proxy_interface.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/adaptor/impl/types.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/adaptor/impl/types.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/grpc_client.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/grpc_client.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/services/command_query.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/services/command_query.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/services/output_stream.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/services/output_stream.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/services/process.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/services/process.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/services/solution.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/services/solution.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/syc_container.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/syc_container.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/syc_process.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/syc_process.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/client/variant.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/client/variant.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/examples/__init__.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/examples/downloads.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/native_api/__init__.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/native_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/native_api/command_metadata.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/native_api/command_metadata.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/native_api/datamodel_metadata.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/native_api/datamodel_metadata.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/native_api/meta_wrapper.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/native_api/meta_wrapper.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/native_api/native_api.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/native_api/native_api.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/native_api/object_path.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/native_api/object_path.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/participant/manager.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/participant/manager.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/participant/mapdl.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/participant/mapdl.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/participant/protocol.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/participant/protocol.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/session.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/session.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/syc_version.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/syc_version.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/util/file_transfer.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/util/file_transfer.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/util/logging.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/util/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     log_to_file(filepath)
         Enable logging to a file.
     disable_log_to_file()
         Disable logging to a file.
     """
 
     def __init__(self, level: Any = logging.ERROR):
-        self.logger = logging.getLogger()
+        self.logger = logging.getLogger("pysystem-coupling")
         self.stream_handler = None
         self.file_handler = None
         self.log_filepath = None
         self.formatter = logging.Formatter(
             "%(asctime)s %(name)-12s %(levelname)-8s %(message)s"
         )
         self.log_to_stdout()
```

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/util/name_util.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/util/name_util.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/util/pathstr.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/util/pathstr.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/util/state_keys.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/util/state_keys.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/src/ansys/systemcoupling/core/util/yaml_helper.py` & `ansys_systemcoupling_core-0.5.0/src/ansys/systemcoupling/core/util/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `ansys_systemcoupling_core-0.4.1/PKG-INFO` & `ansys_systemcoupling_core-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-systemcoupling-core
-Version: 0.4.1
+Version: 0.5.0
 Summary: A Python wrapper for Ansys System Coupling.
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.9,<3.13
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -16,35 +16,35 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ansys-api-systemcoupling==0.1.0
 Requires-Dist: ansys-platform-instancemanagement~=1.0
 Requires-Dist: grpcio>=1.30.0
-Requires-Dist: grpcio-status>=1.30.0,<1.60.2
+Requires-Dist: grpcio-status>=1.30.0,<1.62.2
 Requires-Dist: googleapis-common-protos>=1.50.0
 Requires-Dist: protobuf>=3.20.1,<4.0.0
 Requires-Dist: psutil>=5.7.0
 Requires-Dist: pyyaml
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: importlib-metadata>=4.0
 Requires-Dist: build ; extra == "build"
-Requires-Dist: black==24.1.1 ; extra == "classesgen"
+Requires-Dist: black==24.4.2 ; extra == "classesgen"
 Requires-Dist: isort==5.13.2 ; extra == "classesgen"
-Requires-Dist: ansys-sphinx-theme==0.13.3 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.15.2 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.5.3 ; extra == "doc"
 Requires-Dist: matplotlib ; extra == "doc"
-Requires-Dist: numpydoc==1.6.0 ; extra == "doc"
-Requires-Dist: pypandoc==1.12 ; extra == "doc"
-Requires-Dist: pytest-sphinx==0.6.0 ; extra == "doc"
+Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
+Requires-Dist: pypandoc==1.13 ; extra == "doc"
+Requires-Dist: pytest-sphinx==0.6.3 ; extra == "doc"
 Requires-Dist: Sphinx==7.2.6 ; extra == "doc"
-Requires-Dist: sphinx-autobuild==2024.2.4 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==1.25.2 ; extra == "doc"
+Requires-Dist: sphinx-autobuild==2024.4.16 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==2.0.1 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
-Requires-Dist: sphinx-gallery==0.15.0 ; extra == "doc"
+Requires-Dist: sphinx-gallery==0.16.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==1.0.0 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.7 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.3.1 ; extra == "doc"
 Requires-Dist: ansys-fluent-core ; extra == "doc"
 Requires-Dist: ansys-dpf-core ; extra == "doc"
 Requires-Dist: codespell==2.2.6 ; extra == "style"
 Requires-Dist: flake8==7.0.0 ; extra == "style"
```

