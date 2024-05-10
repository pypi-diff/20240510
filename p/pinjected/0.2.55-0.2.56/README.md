# Comparing `tmp/pinjected-0.2.55.tar.gz` & `tmp/pinjected-0.2.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.2.55.tar", max compression
+gzip compressed data, was "pinjected-0.2.56.tar", max compression
```

## Comparing `pinjected-0.2.55.tar` & `pinjected-0.2.56.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.55/LICENSE
--rw-r--r--   0        0        0      489 2024-05-01 08:00:14.716375 pinjected-0.2.55/pinjected/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.55/pinjected/__main__.py
--rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.55/pinjected/decoration.py
--rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.55/pinjected/demo.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.55/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.55/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     5817 2024-04-24 10:38:38.128103 pinjected-0.2.55/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.55/pinjected/di/applicative.py
--rw-r--r--   0        0        0     7345 2024-04-24 10:43:24.249513 pinjected-0.2.55/pinjected/di/ast.py
--rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.55/pinjected/di/async_injected.py
--rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.55/pinjected/di/bindings.py
--rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.55/pinjected/di/decorators.py
--rw-r--r--   0        0        0    14766 2024-05-08 06:09:38.125434 pinjected-0.2.55/pinjected/di/design.py
--rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.55/pinjected/di/design_bind_contextx.py
--rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.55/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.55/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.55/pinjected/di/graph.py
--rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.55/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    54296 2024-05-05 06:25:12.645054 pinjected-0.2.55/pinjected/di/injected.py
--rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.55/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.55/pinjected/di/metadata/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.55/pinjected/di/metadata/bind_metadata.py
--rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.55/pinjected/di/metadata/location_data.py
--rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.55/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.55/pinjected/di/monadic.py
--rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.55/pinjected/di/overload_experimental.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.55/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.55/pinjected/di/provider.py
--rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.55/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.55/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.55/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.55/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.55/pinjected/di/test_ast.py
--rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.55/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1514 2024-04-24 11:23:19.343247 pinjected-0.2.55/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.55/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.55/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.55/pinjected/di/tools/__init__.py
--rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.55/pinjected/di/tools/add_overload.py
--rw-r--r--   0        0        0    15534 2024-05-05 06:03:05.073926 pinjected-0.2.55/pinjected/di/util.py
--rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.55/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.55/pinjected/exporter/__init__.py
--rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.55/pinjected/exporter/llm_export_v2.py
--rw-r--r--   0        0        0    31460 2024-05-05 06:25:12.638593 pinjected-0.2.55/pinjected/exporter/llm_exporter.py
--rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.55/pinjected/exporter/optimize_import_stmts.py
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.55/pinjected/global_configs.py
--rw-r--r--   0        0        0     3039 2024-05-03 14:38:08.493688 pinjected-0.2.55/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.55/pinjected/helper_structure.py
--rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.55/pinjected/helpers.py
--rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.55/pinjected/ide_supports/__init__.py
--rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.55/pinjected/ide_supports/console_run_helper.py
--rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.55/pinjected/ide_supports/create_configs.py
--rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.55/pinjected/ide_supports/default_design.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.55/pinjected/llm_support/__init__.py
--rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.55/pinjected/llm_support/inspect_module.py
--rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.55/pinjected/llm_support/inspect_module_prompts.py
--rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.55/pinjected/logging_helper.py
--rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.55/pinjected/main_impl.py
--rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.55/pinjected/maybe_patch.py
--rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.55/pinjected/meta_main.py
--rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.55/pinjected/module_helper.py
--rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.55/pinjected/module_inspector.py
--rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.55/pinjected/module_var_path.py
--rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.55/pinjected/notification.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.55/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.55/pinjected/providable.py
--rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.55/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.55/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.55/pinjected/run_helpers/__init__.py
--rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.55/pinjected/run_helpers/config.py
--rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.55/pinjected/run_helpers/pinjected_environments.py
--rw-r--r--   0        0        0     9601 2024-05-01 11:59:22.455243 pinjected-0.2.55/pinjected/run_helpers/run_injected.py
--rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.55/pinjected/runnables.py
--rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.55/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.55/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.55/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.55/pinjected/test_package/child/module_with.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.55/pinjected/v2/__init__.py
--rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.55/pinjected/v2/ainjected.py
--rw-r--r--   0        0        0     7032 2024-05-05 05:55:33.403415 pinjected-0.2.55/pinjected/v2/binds.py
--rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.55/pinjected/v2/di.py
--rw-r--r--   0        0        0      524 2024-05-01 08:03:21.521914 pinjected-0.2.55/pinjected/v2/keys.py
--rw-r--r--   0        0        0      518 2024-05-08 06:06:09.223799 pinjected-0.2.55/pinjected/v2/provide_context.py
--rw-r--r--   0        0        0    14293 2024-05-08 07:26:48.558931 pinjected-0.2.55/pinjected/v2/resolver.py
--rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.55/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.55/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.55/pinjected/viz/graph.py
--rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.55/pinjected/with_context.py
--rw-r--r--   0        0        0      656 2024-05-08 07:27:01.071659 pinjected-0.2.55/pyproject.toml
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.55/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.56/LICENSE
+-rw-r--r--   0        0        0      489 2024-05-01 08:00:14.716375 pinjected-0.2.56/pinjected/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.56/pinjected/__main__.py
+-rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.56/pinjected/decoration.py
+-rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.56/pinjected/demo.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.56/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.56/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     5851 2024-05-10 02:53:28.124125 pinjected-0.2.56/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.56/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     7866 2024-05-10 03:03:16.666241 pinjected-0.2.56/pinjected/di/ast.py
+-rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.56/pinjected/di/async_injected.py
+-rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.56/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     9753 2024-03-26 02:52:38.838842 pinjected-0.2.56/pinjected/di/decorators.py
+-rw-r--r--   0        0        0    14766 2024-05-08 06:09:38.125434 pinjected-0.2.56/pinjected/di/design.py
+-rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.56/pinjected/di/design_bind_contextx.py
+-rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.56/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.56/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.56/pinjected/di/graph.py
+-rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.56/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    54691 2024-05-10 03:24:47.083934 pinjected-0.2.56/pinjected/di/injected.py
+-rw-r--r--   0        0        0     1892 2023-11-06 06:59:52.887127 pinjected-0.2.56/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.56/pinjected/di/metadata/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.56/pinjected/di/metadata/bind_metadata.py
+-rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.56/pinjected/di/metadata/location_data.py
+-rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.56/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.56/pinjected/di/monadic.py
+-rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.56/pinjected/di/overload_experimental.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.56/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.56/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.56/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.56/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.56/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.56/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.56/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0      997 2024-03-26 02:52:38.844108 pinjected-0.2.56/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1514 2024-04-24 11:23:19.343247 pinjected-0.2.56/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.56/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      452 2024-03-26 02:52:38.845073 pinjected-0.2.56/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.56/pinjected/di/tools/__init__.py
+-rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.56/pinjected/di/tools/add_overload.py
+-rw-r--r--   0        0        0    15534 2024-05-05 06:03:05.073926 pinjected-0.2.56/pinjected/di/util.py
+-rw-r--r--   0        0        0     1071 2023-08-25 06:23:59.157878 pinjected-0.2.56/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.56/pinjected/exporter/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.56/pinjected/exporter/llm_export_v2.py
+-rw-r--r--   0        0        0    31460 2024-05-05 06:25:12.638593 pinjected-0.2.56/pinjected/exporter/llm_exporter.py
+-rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.56/pinjected/exporter/optimize_import_stmts.py
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.56/pinjected/global_configs.py
+-rw-r--r--   0        0        0     3039 2024-05-03 14:38:08.493688 pinjected-0.2.56/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.56/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.56/pinjected/helpers.py
+-rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.56/pinjected/ide_supports/__init__.py
+-rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.56/pinjected/ide_supports/console_run_helper.py
+-rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.56/pinjected/ide_supports/create_configs.py
+-rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.56/pinjected/ide_supports/default_design.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.56/pinjected/llm_support/__init__.py
+-rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.56/pinjected/llm_support/inspect_module.py
+-rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.56/pinjected/llm_support/inspect_module_prompts.py
+-rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.56/pinjected/logging_helper.py
+-rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.56/pinjected/main_impl.py
+-rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.56/pinjected/maybe_patch.py
+-rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.56/pinjected/meta_main.py
+-rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.56/pinjected/module_helper.py
+-rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.56/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.56/pinjected/module_var_path.py
+-rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.56/pinjected/notification.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.56/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.56/pinjected/providable.py
+-rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.56/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.56/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.56/pinjected/run_helpers/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.56/pinjected/run_helpers/config.py
+-rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.56/pinjected/run_helpers/pinjected_environments.py
+-rw-r--r--   0        0        0     9601 2024-05-01 11:59:22.455243 pinjected-0.2.56/pinjected/run_helpers/run_injected.py
+-rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.56/pinjected/runnables.py
+-rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.56/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.56/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.56/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.56/pinjected/test_package/child/module_with.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.56/pinjected/v2/__init__.py
+-rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.56/pinjected/v2/ainjected.py
+-rw-r--r--   0        0        0     7032 2024-05-05 05:55:33.403415 pinjected-0.2.56/pinjected/v2/binds.py
+-rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.56/pinjected/v2/di.py
+-rw-r--r--   0        0        0      524 2024-05-01 08:03:21.521914 pinjected-0.2.56/pinjected/v2/keys.py
+-rw-r--r--   0        0        0      627 2024-05-10 02:30:28.919876 pinjected-0.2.56/pinjected/v2/provide_context.py
+-rw-r--r--   0        0        0    22124 2024-05-10 04:00:45.338307 pinjected-0.2.56/pinjected/v2/resolver.py
+-rw-r--r--   0        0        0    19384 2024-03-26 02:52:38.852889 pinjected-0.2.56/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.56/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.56/pinjected/viz/graph.py
+-rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.56/pinjected/with_context.py
+-rw-r--r--   0        0        0      656 2024-05-10 04:00:49.264141 pinjected-0.2.56/pyproject.toml
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.56/PKG-INFO
```

### Comparing `pinjected-0.2.55/LICENSE` & `pinjected-0.2.56/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/decoration.py` & `pinjected-0.2.56/pinjected/decoration.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/demo.py` & `pinjected-0.2.56/pinjected/demo.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/app_designed.py` & `pinjected-0.2.56/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/app_injected.py` & `pinjected-0.2.56/pinjected/di/app_injected.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 class EvaledInjected(Injected[T]):
     # TODO I think this class has issue with serialization of ast.
     value: Injected[T]
     ast: Expr[Injected[T]]
 
     def __post_init__(self):
         assert isinstance(self.ast, Expr)
+        self.__expr__ = self.ast
 
     def dependencies(self) -> Set[str]:
         return self.value.dependencies()
 
     def get_provider(self):
         return self.value.get_provider()
 
@@ -64,14 +65,15 @@
     def __hash__(self):
         return hash((self.value, self.ast))
 
     def dynamic_dependencies(self) -> Set[str]:
         return self.value.dynamic_dependencies()
 
 
+
 def reduce_injected_expr(expr: Expr):
     match expr:
         case Object(InjectedPure(value)):
             return str(value)
         case Object(InjectedFunction(func, kwargs)):
             reduced = reduce_injected_expr(Object(kwargs))
             return f"{func.__name__}({reduced})"
```

### Comparing `pinjected-0.2.55/pinjected/di/applicative.py` & `pinjected-0.2.56/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/ast.py` & `pinjected-0.2.56/pinjected/di/ast.py`

 * *Files 14% similar despite different names*

```diff
@@ -207,31 +207,49 @@
         # what if the data is not hashable?
         try:
             return hash(self.data)
         except TypeError as e:
             return hash(id(self.data))
 
 
+@dataclass
+class Cache(Expr):
+    src: Expr
+
+    def __post_init__(self):
+        assert isinstance(self.src, Expr), f"{self.src} is not an Expr"
+
+    def __getstate__(self):
+        return self.src
+
+    def __setstate__(self, state):
+        self.src = state
+
+    def __hash__(self):
+        return hash(f"cached") + hash(self.src)
+
 def show_expr(expr: Expr[T], custom: Callable[[Expr[T]], Optional[str]] = lambda x: None) -> str:
     from pinjected.di.proxiable import DelegatedVar
     def _show_expr(expr):
         def eval_tuple(expr):
             return tuple(_show_expr(i) for i in expr)
 
         def eval_dict(expr):
             return {k: _show_expr(e) for k, e in expr.items()}
 
         reduced = custom(expr)
         if reduced:
             return reduced
         match expr:
+            case Object(x) if hasattr(x,"__repr_expr__"):
+                return x.__repr_expr__()
             case Object(str() as x):
                 return f'"{x}"'
             case Object(x):
-                return str(x)
+                return f"{str(x)}"
             case Call(f, args, kwargs):
                 # hmm, this is complicated.
                 func_str = _show_expr(f)
                 args = list(eval_tuple(args))
                 kwargs = eval_dict(kwargs)
                 kwargs = [f"{k}={v}" for k, v in kwargs.items()]
                 return f"{func_str}({','.join(args + kwargs)})"
@@ -241,12 +259,14 @@
                 return f"{_show_expr(data)}.{attr_name}"
             case GetItem(Expr() as data, key):
                 return f"{_show_expr(data)}[{_show_expr(key)}]"
             case DelegatedVar(wrapped, cxt):
                 return f"{_show_expr(wrapped)}"
             case UnaryOp('await',Expr() as tgt):
                 return f"(await {_show_expr(tgt)})"
-
+            case Cache(Expr() as tgt):
+                return f"{_show_expr(tgt)}"
             case _:
                 raise RuntimeError(f"unsupported ast found!:{type(expr)}")
 
     return _show_expr(expr)
+
```

### Comparing `pinjected-0.2.55/pinjected/di/decorators.py` & `pinjected-0.2.56/pinjected/di/decorators.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/design.py` & `pinjected-0.2.56/pinjected/di/design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/designed.py` & `pinjected-0.2.56/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/dynamic_proxy.py` & `pinjected-0.2.56/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/graph.py` & `pinjected-0.2.56/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/injected.py` & `pinjected-0.2.56/pinjected/di/injected.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import functools
 import hashlib
 import inspect
 import sys
 from copy import copy
 from dataclasses import dataclass, field
 from inspect import Traceback
+from pathlib import Path
 from typing import List, Generic, Union, Callable, TypeVar, Tuple, Set, Dict, Any, Awaitable
 
 from frozendict import frozendict
 from loguru import logger
 from makefun import create_function
 from returns.result import safe
 
@@ -1115,14 +1116,21 @@
         return res
 
     # def __str__(self):
     #    return f"""InjectedFunction(target={self.target_function},kwargs_mapping={self.kwargs_mapping})"""
     def dynamic_dependencies(self) -> Set[str]:
         return set()
 
+    def __repr_expr__(self):
+        func_name = self.original_function.__name__
+        orig_file = Path(self.original_function.__original_file__)
+        orig_line = self.original_function.__original_code__
+        #return f"<f {func_name}@{orig_file.name}>"
+        return self.original_function.__name__
+
 
 class InjectedPure(Injected[T]):
     __match_args__ = ("value",)
 
     def __init__(self, value):
         super().__init__()
         self.value = value
@@ -1167,14 +1175,17 @@
 
     def __repr__(self):
         return str(self)
 
     def dynamic_dependencies(self) -> Set[str]:
         return set()
 
+    def __repr_expr__(self):
+        return f"${self.name}"
+
 
 class ZippedInjected(Injected[Tuple[A, B]]):
     __match_args__ = ("a", "b")
 
     def __init__(self, a: Injected[A], b: Injected[B]):
         super().__init__()
         raise RuntimeError("deprecated")
```

### Comparing `pinjected-0.2.55/pinjected/di/injected_analysis.py` & `pinjected-0.2.56/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/modular_injected.py` & `pinjected-0.2.56/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/overload_experimental.py` & `pinjected-0.2.56/pinjected/di/overload_experimental.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/proxiable.py` & `pinjected-0.2.56/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/session.py` & `pinjected-0.2.56/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/sessioned.py` & `pinjected-0.2.56/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/static_proxy.py` & `pinjected-0.2.56/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.2.56/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/test_graph.py` & `pinjected-0.2.56/pinjected/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/test_injected.py` & `pinjected-0.2.56/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/tools/add_overload.py` & `pinjected-0.2.56/pinjected/di/tools/add_overload.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/di/util.py` & `pinjected-0.2.56/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/exceptions.py` & `pinjected-0.2.56/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/exporter/llm_exporter.py` & `pinjected-0.2.56/pinjected/exporter/llm_exporter.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/exporter/optimize_import_stmts.py` & `pinjected-0.2.56/pinjected/exporter/optimize_import_stmts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/graph_inspection.py` & `pinjected-0.2.56/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/helper_structure.py` & `pinjected-0.2.56/pinjected/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/helpers.py` & `pinjected-0.2.56/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/ide_supports/console_run_helper.py` & `pinjected-0.2.56/pinjected/ide_supports/console_run_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/ide_supports/create_configs.py` & `pinjected-0.2.56/pinjected/ide_supports/create_configs.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/ide_supports/default_design.py` & `pinjected-0.2.56/pinjected/ide_supports/default_design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/llm_support/inspect_module.py` & `pinjected-0.2.56/pinjected/llm_support/inspect_module.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/llm_support/inspect_module_prompts.py` & `pinjected-0.2.56/pinjected/llm_support/inspect_module_prompts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/main_impl.py` & `pinjected-0.2.56/pinjected/main_impl.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/maybe_patch.py` & `pinjected-0.2.56/pinjected/maybe_patch.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/module_helper.py` & `pinjected-0.2.56/pinjected/module_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/module_inspector.py` & `pinjected-0.2.56/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/module_var_path.py` & `pinjected-0.2.56/pinjected/module_var_path.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/notification.py` & `pinjected-0.2.56/pinjected/notification.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/nx_graph_util.py` & `pinjected-0.2.56/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/run_config_utils.py` & `pinjected-0.2.56/pinjected/run_config_utils.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/run_config_utils_v2.py` & `pinjected-0.2.56/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/run_helpers/config.py` & `pinjected-0.2.56/pinjected/run_helpers/config.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/run_helpers/run_injected.py` & `pinjected-0.2.56/pinjected/run_helpers/run_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/runnables.py` & `pinjected-0.2.56/pinjected/runnables.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/test_package/__init__.py` & `pinjected-0.2.56/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/test_package/child/module1.py` & `pinjected-0.2.56/pinjected/test_package/child/module1.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/v2/ainjected.py` & `pinjected-0.2.56/pinjected/v2/ainjected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/v2/binds.py` & `pinjected-0.2.56/pinjected/v2/binds.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/v2/di.py` & `pinjected-0.2.56/pinjected/v2/di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/v2/keys.py` & `pinjected-0.2.56/pinjected/v2/keys.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pinjected/visualize_di.py` & `pinjected-0.2.56/pinjected/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.55/pyproject.toml` & `pinjected-0.2.56/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.2.55"
+version = "0.2.56"
 description = "Immutable Dependency Injection for Python."
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "*"
```

### Comparing `pinjected-0.2.55/PKG-INFO` & `pinjected-0.2.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.2.55
+Version: 0.2.56
 Summary: Immutable Dependency Injection for Python.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

