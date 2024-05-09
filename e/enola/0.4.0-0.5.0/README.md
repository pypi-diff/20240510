# Comparing `tmp/enola-0.4.0.tar.gz` & `tmp/enola-0.5.0.tar.gz`

## Comparing `enola-0.4.0.tar` & `enola-0.5.0.tar`

### file list

```diff
@@ -1,616 +1,46 @@
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 enola-0.4.0/.pypirc
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 enola-0.4.0/requirements.txt
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 enola-0.4.0/.vscode/launch.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/pyvenv.cfg
--rw-r--r--   0        0        0    26199 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/Activate.ps1
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/activate
--rwxr-xr-x   0        0        0     1039 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/activate.bat
--rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/deactivate.bat
--rwxr-xr-x   0        0        0   108448 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/normalizer.exe
--rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/pip.exe
--rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/pip3.11.exe
--rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/pip3.exe
--rwxr-xr-x   0        0        0   270608 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/python.exe
--rwxr-xr-x   0        0        0   259352 2020-02-02 00:00:00.000000 enola-0.4.0/mi_entorno/Scripts/pythonw.exe
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 enola-0.4.0/src/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/__init__.py
--rw-r--r--   0        0        0    16095 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/agent.py
--rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/step.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/connect.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/enola_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/__init__.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_common.py
--rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_connection.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_datetime_part.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_error.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_functions.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_http_info.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_logging.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_param.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_response_error.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_response_provider.py
--rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/huemul_response_to_bloc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/auth/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/auth/auth_model.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/auth/auth_service_bloc.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/auth/auth_service_model.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/common/auth/auth_service_provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/internal/__init__.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/internal/enola_agent.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/internal/enola_agent_bloc.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 enola-0.4.0/src/enola/base/internal/enola_agent_provider.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/pyvenv.cfg
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/INSTALLER
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/LICENSE
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/METADATA
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/WHEEL
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/build-1.0.3.dist-info/entry_points.txt
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/INSTALLER
--rw-r--r--   0        0        0    17158 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/METADATA
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/RECORD
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/WHEEL
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/colorama-0.4.6.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_elffile.py
--rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_manylinux.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_musllinux.py
--rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/markers.py
--rw-r--r--   0        0        0    32750 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/py.typed
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/requirements.py
--rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/specifiers.py
--rw-r--r--   0        0        0    18355 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/tags.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/utils.py
--rw-r--r--   0        0        0    16236 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging/version.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/INSTALLER
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/LICENSE
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/LICENSE.BSD
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/METADATA
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/packaging-23.2.dist-info/WHEEL
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/__init__.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/py.typed
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10429 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    13839 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    23737 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7161 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    11842 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    30030 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18440 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    28934 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12457 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16504 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     6556 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15365 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    20819 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    20541 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18607 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    28868 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0    27475 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    16610 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17872 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    33084 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24678 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24128 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    18969 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    27845 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9824 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    11642 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    22343 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0   111130 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   278952 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10032 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12176 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14537 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27055 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30391 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    14848 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10678 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6741 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
--rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
--rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    49330 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34544 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   109364 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0    20155 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    34618 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63223 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     5424 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35610 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    12130 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    72281 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53424 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9116 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6567 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    13387 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   224445 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    38646 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    26692 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13488 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    24215 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    19697 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35288 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33460 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    20511 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_fileno.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    99218 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14007 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14273 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10574 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    35852 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59706 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4602 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24247 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    27073 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    35173 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39684 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    45525 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    29604 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0     8746 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20300 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39990 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19752 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30641 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11036 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17081 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22003 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14296 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/AUTHORS.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/METADATA
--rw-r--r--   0        0        0    77283 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/REQUESTED
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/WHEEL
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pip-23.2.1.dist-info/top_level.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/METADATA
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/RECORD
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Lib/site-packages/pyproject_hooks-1.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0    26199 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/Activate.ps1
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/activate
--rwxr-xr-x   0        0        0     1045 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/activate.bat
--rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/deactivate.bat
--rwxr-xr-x   0        0        0   108438 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/pip.exe
--rwxr-xr-x   0        0        0   108438 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/pip3.12.exe
--rwxr-xr-x   0        0        0   108438 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/pip3.exe
--rwxr-xr-x   0        0        0   108442 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/pyproject-build.exe
--rwxr-xr-x   0        0        0   270616 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/python.exe
--rwxr-xr-x   0        0        0   259352 2020-02-02 00:00:00.000000 enola-0.4.0/tutorial_env/Scripts/pythonw.exe
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 enola-0.4.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.4.0/LICENSE
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 enola-0.4.0/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 enola-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 enola-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 enola-0.5.0/requirements.txt
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 enola-0.5.0/.vscode/launch.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 enola-0.5.0/mi_entorno/pyvenv.cfg
+-rw-r--r--   0        0        0    26199 2020-02-02 00:00:00.000000 enola-0.5.0/mi_entorno/Scripts/Activate.ps1
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 enola-0.5.0/mi_entorno/Scripts/activate
+-rwxr-xr-x   0        0        0     1039 2020-02-02 00:00:00.000000 enola-0.5.0/mi_entorno/Scripts/activate.bat
+-rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 enola-0.5.0/mi_entorno/Scripts/deactivate.bat
+-rwxr-xr-x   0        0        0   108448 2020-02-02 00:00:00.000000 enola-0.5.0/mi_entorno/Scripts/normalizer.exe
+-rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.5.0/mi_entorno/Scripts/pip.exe
+-rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.5.0/mi_entorno/Scripts/pip3.11.exe
+-rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.5.0/mi_entorno/Scripts/pip3.exe
+-rwxr-xr-x   0        0        0   270608 2020-02-02 00:00:00.000000 enola-0.5.0/mi_entorno/Scripts/python.exe
+-rwxr-xr-x   0        0        0   259352 2020-02-02 00:00:00.000000 enola-0.5.0/mi_entorno/Scripts/pythonw.exe
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 enola-0.5.0/src/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/__init__.py
+-rw-r--r--   0        0        0    16261 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/agent.py
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/step.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/connect.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/enola_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/__init__.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/huemul_common.py
+-rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/huemul_connection.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/huemul_datetime_part.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/huemul_error.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/huemul_functions.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/huemul_http_info.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/huemul_logging.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/huemul_param.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/huemul_response_error.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/huemul_response_provider.py
+-rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/huemul_response_to_bloc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/auth/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/auth/auth_model.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/auth/auth_service_bloc.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/auth/auth_service_model.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/common/auth/auth_service_provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/internal/__init__.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/internal/enola_agent.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/internal/enola_agent_bloc.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 enola-0.5.0/src/enola/base/internal/enola_agent_provider.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 enola-0.5.0/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.5.0/LICENSE
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 enola-0.5.0/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 enola-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 enola-0.5.0/PKG-INFO
```

### Comparing `enola-0.4.0/mi_entorno/Scripts/Activate.ps1` & `enola-0.5.0/mi_entorno/Scripts/Activate.ps1`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/mi_entorno/Scripts/activate` & `enola-0.5.0/mi_entorno/Scripts/activate`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/mi_entorno/Scripts/activate.bat` & `enola-0.5.0/mi_entorno/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/mi_entorno/Scripts/normalizer.exe` & `enola-0.5.0/mi_entorno/Scripts/normalizer.exe`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/mi_entorno/Scripts/pip.exe` & `enola-0.5.0/mi_entorno/Scripts/pip.exe`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/mi_entorno/Scripts/pip3.11.exe` & `enola-0.5.0/mi_entorno/Scripts/pip3.11.exe`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/mi_entorno/Scripts/pip3.exe` & `enola-0.5.0/mi_entorno/Scripts/pip3.exe`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/mi_entorno/Scripts/python.exe` & `enola-0.5.0/mi_entorno/Scripts/python.exe`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/mi_entorno/Scripts/pythonw.exe` & `enola-0.5.0/mi_entorno/Scripts/pythonw.exe`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/test.py` & `enola-0.5.0/src/test.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/agent.py` & `enola-0.5.0/src/enola/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         
         #if is empty or not exist assign false
         self.isTest = isTest
         
         #save steps and informations
         self.step_list = []
         self.steps = 0
-        self.first_step = self.new_step(self.name)
+        self.first_step = self.new_step(self.name, message_input= self.message_input)
 
     ########################################################################################
     ###############    A G E N T   M E T H O D S     #######################################
     ########################################################################################
 
 
     def add_data_received(self, name:str, data, type:DataType):
@@ -196,23 +196,23 @@
 
 
     ########################################################################################
     ###############    S T E P   I N F O     ###############################################
     ########################################################################################
 
 
-    def new_step(self, name: str):
+    def new_step(self, name: str, message_input: str = ""):
         """
         start new step
-
         name: name of this step
+        message_input: message received from user or to explain the execution
         """
         #current_step = 
         self.steps += 1
-        return Step(name=name)
+        return Step(name=name, message_input=message_input)
 
     def close_step_token(self, step: Step, successfull: bool, message_output: str ="", token_input_num: int=0, token_output_num: int=0, token_total_num: int=0, token_input_cost: float=0, token_output_cost: float=0, token_total_cost: float=0, enola_id: str="", agent_deploy_id: str="", step_id:str=""):
         """
         close step with token information
         enola_id: If this step was a call to another Enola agent, whether from your own company or another, this is the ID of that agent
         agent_deploy_id: include this if you want to link this step to another agent of another company
         step_id: id of this step, you can use it to link with external calls
```

### Comparing `enola-0.4.0/src/enola/step.py` & `enola-0.5.0/src/enola/step.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,21 +45,21 @@
     def __init__(self):
         self.num_char = 0
         self.token_input = 0
         self.token_output = 0
         self.token_total = 0
 
 class Step:
-    def __init__(self, name: str):
+    def __init__(self, name: str, message_input: str = ""):
         self.hf = HuemulFunctions()
         self.name = name
         self.enola_id = ""
         self.agent_deploy_id = ""
         self.step_id = ""
-        self.message_input = ""
+        self.message_input = message_input
         self.message_output = ""
         self.num_iterations = 0
         self.step_api_code = ""
         self.step_id_prev = ""
         self.date_start = self.hf.getDateForApi()
         self.date_end = self.date_start
         #self.result_list = []
```

### Comparing `enola-0.4.0/src/enola/base/connect.py` & `enola-0.5.0/src/enola/base/connect.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/enola_types.py` & `enola-0.5.0/src/enola/base/enola_types.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/common/huemul_common.py` & `enola-0.5.0/src/enola/base/common/huemul_common.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/common/huemul_connection.py` & `enola-0.5.0/src/enola/base/common/huemul_connection.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/common/huemul_error.py` & `enola-0.5.0/src/enola/base/common/huemul_error.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/common/huemul_functions.py` & `enola-0.5.0/src/enola/base/common/huemul_functions.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/common/huemul_logging.py` & `enola-0.5.0/src/enola/base/common/huemul_logging.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/common/huemul_response_provider.py` & `enola-0.5.0/src/enola/base/common/huemul_response_provider.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/common/huemul_response_to_bloc.py` & `enola-0.5.0/src/enola/base/common/huemul_response_to_bloc.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/common/auth/auth_model.py` & `enola-0.5.0/src/enola/base/common/auth/auth_model.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/common/auth/auth_service_bloc.py` & `enola-0.5.0/src/enola/base/common/auth/auth_service_bloc.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/common/auth/auth_service_provider.py` & `enola-0.5.0/src/enola/base/common/auth/auth_service_provider.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/internal/enola_agent.py` & `enola-0.5.0/src/enola/base/internal/enola_agent.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/internal/enola_agent_bloc.py` & `enola-0.5.0/src/enola/base/internal/enola_agent_bloc.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/src/enola/base/internal/enola_agent_provider.py` & `enola-0.5.0/src/enola/base/internal/enola_agent_provider.py`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/.gitignore` & `enola-0.5.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
+.pypirc
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
 var/
+tutorial_env/
 wheels/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
 
@@ -154,7 +156,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+.pypirc
```

### Comparing `enola-0.4.0/README.md` & `enola-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `enola-0.4.0/pyproject.toml` & `enola-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "enola"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
   { name="Sebastian Rodriguez Robotham", email="sebastian.rodriguez@huemulsolutions.com" },
   { name="Developer Code", email="developer.code@huemulsolutions.com" },
 ]
 description = "Observability & Governance of Intelligence Agents"
 keywords = ["AI", "Observability", "agent", "Intelligence"]
 readme = "README.md"
```

### Comparing `enola-0.4.0/PKG-INFO` & `enola-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: enola
-Version: 0.4.0
+Version: 0.5.0
 Summary: Observability & Governance of Intelligence Agents
 Project-URL: Homepage, https://github.com/huemulsolutions/enola
 Project-URL: Bug Tracker, https://github.com/huemulsolutions/enola/issues
 Author-email: Sebastian Rodriguez Robotham <sebastian.rodriguez@huemulsolutions.com>, Developer Code <developer.code@huemulsolutions.com>
 License-File: LICENSE
 Keywords: AI,Intelligence,Observability,agent
 Classifier: License :: OSI Approved :: MIT License
```

