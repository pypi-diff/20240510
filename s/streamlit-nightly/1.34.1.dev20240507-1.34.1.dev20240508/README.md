# Comparing `tmp/streamlit_nightly-1.34.1.dev20240507.tar.gz` & `tmp/streamlit_nightly-1.34.1.dev20240508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_nightly-1.34.1.dev20240507.tar", last modified: Wed May  8 13:33:33 2024, max compression
+gzip compressed data, was "streamlit_nightly-1.34.1.dev20240508.tar", last modified: Thu May  9 11:52:58 2024, max compression
```

## Comparing `streamlit_nightly-1.34.1.dev20240507.tar` & `streamlit_nightly-1.34.1.dev20240508.tar`

### file list

```diff
@@ -1,576 +1,576 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.331549 streamlit_nightly-1.34.1.dev20240507/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-08 13:33:33.331549 streamlit_nightly-1.34.1.dev20240507/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.219549 streamlit_nightly-1.34.1.dev20240507/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/bin/streamlit.cmd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:33:33.331549 streamlit_nightly-1.34.1.dev20240507/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.223549 streamlit_nightly-1.34.1.dev20240507/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/case_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/code_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/column_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.227549 streamlit_nightly-1.34.1.dev20240507/streamlit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/commands/execution_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/commands/experimental_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/commands/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/commands/page_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.227549 streamlit_nightly-1.34.1.dev20240507/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.227549 streamlit_nightly-1.34.1.dev20240507/streamlit/components/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/components/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/components/lib/local_component_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.227549 streamlit_nightly-1.34.1.dev20240507/streamlit/components/types/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/components/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/components/types/base_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/components/types/base_custom_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.227549 streamlit_nightly-1.34.1.dev20240507/streamlit/components/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/components/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/components/v1/component_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/components/v1/component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/components/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/components/v1/custom_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.227549 streamlit_nightly-1.34.1.dev20240507/streamlit/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/connections/snowflake_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/connections/snowpark_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/connections/sql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/connections/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/delta_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/deprecation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/development.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/echo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.235549 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    14558 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/balloons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/bokeh_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/deck_gl_json_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/dialog_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/doc_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/graphviz_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.235549 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/built_in_chart_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/column_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/dicttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/mutable_status_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/pandas_styler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/streamlit_plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/subtitle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/map.py
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    15332 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/pyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/snow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/toast.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    38336 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/vega_charts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.239549 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32277 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/camera_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/data_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/number_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/select_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/selectbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    22333 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/text_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/time_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/elements/write.py
--rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/error_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.239549 streamlit_nightly-1.34.1.dev20240507/streamlit/external/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.239549 streamlit_nightly-1.34.1.dev20240507/streamlit/external/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/external/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/external/langchain/streamlit_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/folder_black_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/git_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.239549 streamlit_nightly-1.34.1.dev20240507/streamlit/hello/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/hello/Hello.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/hello/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.239549 streamlit_nightly-1.34.1.dev20240507/streamlit/hello/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/hello/pages/0_Animation_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/hello/pages/1_Plotting_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/hello/pages/2_Mapping_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/hello/pages/3_DataFrame_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/hello/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/js_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/material_icon_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/net_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.263549 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Alert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Alert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/AppPage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/AppPage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ArrowNamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Arrow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Arrow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Audio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Audio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/AutoRerun_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/AutoRerun_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/BackMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/BackMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Balloons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Balloons_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Block_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Block_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/BokehChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/BokehChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Button_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Button_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/CameraInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/CameraInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ChatInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ChatInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Checkbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Checkbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ClientState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ClientState_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ColorPicker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ColorPicker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Components_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DataFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DataFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DateInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DateInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DeckGlJsonChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Delta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Delta_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DocString_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DocString_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DownloadButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DownloadButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Element_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Element_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Empty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Exception_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Exception_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Favicon_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Favicon_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/FileUploader_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/FileUploader_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ForwardMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ForwardMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/GitInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/GitInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/GraphVizChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/GraphVizChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Heading_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Heading_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Html_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Html_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/IFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/IFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Json_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Json_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/LabelVisibilityMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/LabelVisibilityMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/LinkButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/LinkButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Logo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Logo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Markdown_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Markdown_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Metric_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/MultiSelect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/MultiSelect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/NamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/NamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/NewSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/NewSession_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/NumberInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/NumberInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageConfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageConfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageLink_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageLink_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageNotFound_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageNotFound_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageProfile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageProfile_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PagesChanged_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PagesChanged_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ParentMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ParentMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PlotlyChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PlotlyChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Progress_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Progress_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Radio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Radio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/RootContainer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/RootContainer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Selectbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Selectbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/SessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/SessionEvent_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/SessionStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/SessionStatus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Skeleton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Skeleton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Slider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Slider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Snow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Snow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Spinner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Spinner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/TextArea_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/TextArea_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/TextInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/TextInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Text_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/TimeInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/TimeInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Toast_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Toast_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/VegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/VegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Video_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Video_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/WidgetStates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/WidgetStates_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/openmetrics_data_model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-08 13:29:40.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/proto/openmetrics_data_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.267549 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36646 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/app_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.267549 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/cache_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/cache_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/cache_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/cache_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/cached_message_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.267549 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/storage/cache_storage_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/storage/dummy_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/storage/local_disk_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/forward_msg_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/forward_msg_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/fragment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.271549 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/legacy_caching/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/legacy_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/legacy_caching/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/legacy_caching/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/media_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/memory_media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/memory_session_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/memory_uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/metrics_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    29438 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.271549 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/magic_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/script_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/script_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/script_run_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/session_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.271549 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/query_params_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/safe_session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/session_state_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/websocket_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/source_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.271549 streamlit_nightly-1.34.1.dev20240507/streamlit/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-08 13:30:09.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.215549 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.271549 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/css/3092.95a45cfe.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/css/3466.8b8f33d6.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/css/5441.e3b876c5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/css/main.3aaaea00.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.307549 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1074.73973756.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1168.7452e363.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1307.0f0cca93.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1451.3b0a3e31.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1479.6709db03.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/178.7bea8c5d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   396783 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1955.426e67ca.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1955.426e67ca.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/2178.90362aae.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/2187.9469f035.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/2469.09ea79bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/2634.1249dc7a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/2736.4336e2b9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3053.7e70ec3b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    47103 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3092.21bb8f7b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/329.464ed8ec.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3301.1d1b10bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3466.05d62820.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3513.ebc278c4.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3631.be5c35fa.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4113.9b2db2e3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4132.49bf3f2c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4177.69f9f18d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4319.bf1c86bf.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4477.1bd49702.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4500.b6f348d1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4666.c4b22a63.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/474.87506447.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5106.44f0ff51.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5117.04bfe5d3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5249.f2f4070d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5345.65c91ee7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5379.6571574f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5441.5bacdeda.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5791.9a42fb4b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/6013.64cd6d28.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/6405.ac5a6f23.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/6718.802da17e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/6853.93dd1c4c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7142.83028745.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7175.be4076bc.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7323.b74cc85b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7483.64f23be7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7602.e8abc06b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7805.acc6316a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8005.43974a35.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8477.de889fe5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8492.0d93bd08.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8536.f8de3d9a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8570.6de19120.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8691.9ccf7f89.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/9330.2b4c99e0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/9336.2d95d840.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/937.a1248039.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/9656.8c935274.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/9758.6e6d8662.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/9865.fd93213d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  4401921 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/main.b84b6de2.js
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/main.b84b6de2.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.323549 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
--rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
--rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-08 13:33:30.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/temporary_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.323549 streamlit_nightly-1.34.1.dev20240507/streamlit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.323549 streamlit_nightly-1.34.1.dev20240507/streamlit/testing/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/testing/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/testing/v1/app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/testing/v1/element_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/testing/v1/local_script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/testing/v1/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    47503 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.323549 streamlit_nightly-1.34.1.dev20240507/streamlit/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.323549 streamlit_nightly-1.34.1.dev20240507/streamlit/vendor/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/vendor/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/vendor/ipython/modified_sys_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.323549 streamlit_nightly-1.34.1.dev20240507/streamlit/vendor/pympler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/vendor/pympler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/vendor/pympler/asizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.327549 streamlit_nightly-1.34.1.dev20240507/streamlit/watcher/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/watcher/event_based_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/watcher/local_sources_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/watcher/path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/watcher/polling_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/watcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.327549 streamlit_nightly-1.34.1.dev20240507/streamlit/web/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/cache_storage_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.327549 streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/app_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/browser_websocket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/component_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/media_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/server_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/stats_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/upload_file_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/websocket_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.331549 streamlit_nightly-1.34.1.dev20240507/streamlit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-08 13:33:31.000000 streamlit_nightly-1.34.1.dev20240507/streamlit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-05-08 13:33:31.000000 streamlit_nightly-1.34.1.dev20240507/streamlit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:33:31.000000 streamlit_nightly-1.34.1.dev20240507/streamlit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 13:33:31.000000 streamlit_nightly-1.34.1.dev20240507/streamlit_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:29:37.000000 streamlit_nightly-1.34.1.dev20240507/streamlit_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-08 13:33:31.000000 streamlit_nightly-1.34.1.dev20240507/streamlit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 13:33:31.000000 streamlit_nightly-1.34.1.dev20240507/streamlit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:33:33.327549 streamlit_nightly-1.34.1.dev20240507/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-08 13:28:08.000000 streamlit_nightly-1.34.1.dev20240507/tests/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.500038 streamlit_nightly-1.34.1.dev20240508/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-09 11:52:58.500038 streamlit_nightly-1.34.1.dev20240508/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.388038 streamlit_nightly-1.34.1.dev20240508/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/bin/streamlit.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:52:58.500038 streamlit_nightly-1.34.1.dev20240508/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.392038 streamlit_nightly-1.34.1.dev20240508/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/case_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/code_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/column_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.396038 streamlit_nightly-1.34.1.dev20240508/streamlit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/commands/execution_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/commands/experimental_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/commands/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/commands/page_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.396038 streamlit_nightly-1.34.1.dev20240508/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.396038 streamlit_nightly-1.34.1.dev20240508/streamlit/components/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/components/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/components/lib/local_component_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.396038 streamlit_nightly-1.34.1.dev20240508/streamlit/components/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/components/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/components/types/base_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/components/types/base_custom_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.396038 streamlit_nightly-1.34.1.dev20240508/streamlit/components/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/components/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/components/v1/component_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/components/v1/component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/components/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/components/v1/custom_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43895 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.396038 streamlit_nightly-1.34.1.dev20240508/streamlit/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/connections/snowflake_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/connections/snowpark_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/connections/sql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/connections/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/delta_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/deprecation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/echo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.404038 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14558 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/bokeh_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/deck_gl_json_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/dialog_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/doc_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/graphviz_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.404038 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/built_in_chart_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/column_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/dicttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/mutable_status_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/pandas_styler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/streamlit_plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/subtitle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15332 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/pyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/snow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43912 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/vega_charts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.408038 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32860 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/camera_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14320 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9142 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35827 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/data_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/number_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/select_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/selectbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22333 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/text_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/time_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/elements/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/error_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.408038 streamlit_nightly-1.34.1.dev20240508/streamlit/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.408038 streamlit_nightly-1.34.1.dev20240508/streamlit/external/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/external/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/external/langchain/streamlit_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/folder_black_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/git_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.408038 streamlit_nightly-1.34.1.dev20240508/streamlit/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/hello/Hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/hello/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.408038 streamlit_nightly-1.34.1.dev20240508/streamlit/hello/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/hello/pages/0_Animation_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/hello/pages/1_Plotting_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/hello/pages/2_Mapping_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/hello/pages/3_DataFrame_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/hello/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/js_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/material_icon_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/net_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.432038 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Alert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Alert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/AppPage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/AppPage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ArrowNamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Arrow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Arrow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Audio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Audio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/AutoRerun_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/AutoRerun_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/BackMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/BackMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Balloons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Balloons_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Block_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Block_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/BokehChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/BokehChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Button_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Button_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/CameraInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/CameraInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ChatInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ChatInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Checkbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Checkbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ClientState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ClientState_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ColorPicker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ColorPicker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Components_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DataFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DataFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DateInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DateInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DeckGlJsonChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Delta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Delta_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DocString_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DocString_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DownloadButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DownloadButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Element_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Element_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Empty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Exception_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Exception_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Favicon_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Favicon_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/FileUploader_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/FileUploader_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ForwardMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ForwardMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/GitInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/GitInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/GraphVizChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/GraphVizChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Heading_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Heading_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Html_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Html_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/IFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/IFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Json_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Json_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/LabelVisibilityMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/LabelVisibilityMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/LinkButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/LinkButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Logo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Logo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Markdown_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Markdown_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Metric_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/MultiSelect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/MultiSelect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/NamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/NamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/NewSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/NewSession_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/NumberInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/NumberInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageConfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageConfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageLink_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageLink_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageNotFound_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageNotFound_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageProfile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageProfile_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PagesChanged_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PagesChanged_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ParentMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ParentMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PlotlyChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PlotlyChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Progress_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Progress_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Radio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Radio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/RootContainer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/RootContainer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Selectbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Selectbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/SessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/SessionEvent_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/SessionStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/SessionStatus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Skeleton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Skeleton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Slider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Slider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Snow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Snow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Spinner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Spinner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/TextArea_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/TextArea_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/TextInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/TextInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Text_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/TimeInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/TimeInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Toast_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Toast_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/VegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/VegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Video_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Video_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/WidgetStates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/WidgetStates_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/openmetrics_data_model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-09 11:49:11.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/proto/openmetrics_data_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.436038 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36646 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/app_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.440038 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/cache_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/cache_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/cache_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/cache_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/cached_message_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.440038 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/storage/cache_storage_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/storage/dummy_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/storage/local_disk_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/forward_msg_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/forward_msg_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/fragment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.440038 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/legacy_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/legacy_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27873 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/legacy_caching/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35033 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/legacy_caching/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/media_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/memory_media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/memory_session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/memory_uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/metrics_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29438 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.440038 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/magic_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/script_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/script_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/script_run_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.444038 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/query_params_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/safe_session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/session_state_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/websocket_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/source_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.444038 streamlit_nightly-1.34.1.dev20240508/streamlit/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-09 11:49:39.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.384038 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.444038 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/css/3092.95a45cfe.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/css/3466.8b8f33d6.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/css/5441.e3b876c5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/css/main.3aaaea00.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.476038 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1074.73973756.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1168.7452e363.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1307.0f0cca93.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1451.3b0a3e31.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1479.6709db03.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/178.7bea8c5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   396783 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1955.426e67ca.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1955.426e67ca.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/2178.90362aae.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/2187.9469f035.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/2469.09ea79bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/2634.1249dc7a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/2736.4336e2b9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3053.7e70ec3b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    47103 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3092.21bb8f7b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/329.464ed8ec.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3301.1d1b10bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3466.05d62820.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3513.ebc278c4.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3631.be5c35fa.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4113.99983645.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4132.49bf3f2c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4177.69f9f18d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4319.bf1c86bf.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4477.1bd49702.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4500.b6f348d1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4666.c4b22a63.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/474.87506447.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5106.44f0ff51.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5117.04bfe5d3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5249.f2f4070d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5345.65c91ee7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5379.6571574f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5441.5bacdeda.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5791.9a42fb4b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/6013.4ba2d616.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/6405.ac5a6f23.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/6718.802da17e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/6853.93dd1c4c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7142.83028745.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7175.be4076bc.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7323.b74cc85b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7483.64f23be7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7602.e8abc06b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7805.acc6316a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8005.43974a35.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8477.de889fe5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8492.0d93bd08.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8536.f8de3d9a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8570.6de19120.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8691.9ccf7f89.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/9330.2b4c99e0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/9336.2d95d840.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/937.a1248039.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/9656.8c935274.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/9758.6e6d8662.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/9865.fd93213d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4401921 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/main.5a6e0ded.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/main.5a6e0ded.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.492038 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-09 11:52:55.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/temporary_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.492038 streamlit_nightly-1.34.1.dev20240508/streamlit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.492038 streamlit_nightly-1.34.1.dev20240508/streamlit/testing/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/testing/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/testing/v1/app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/testing/v1/element_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/testing/v1/local_script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/testing/v1/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48364 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.492038 streamlit_nightly-1.34.1.dev20240508/streamlit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.496038 streamlit_nightly-1.34.1.dev20240508/streamlit/vendor/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/vendor/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/vendor/ipython/modified_sys_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.496038 streamlit_nightly-1.34.1.dev20240508/streamlit/vendor/pympler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/vendor/pympler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/vendor/pympler/asizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.496038 streamlit_nightly-1.34.1.dev20240508/streamlit/watcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/watcher/event_based_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/watcher/local_sources_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/watcher/path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/watcher/polling_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/watcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.496038 streamlit_nightly-1.34.1.dev20240508/streamlit/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/cache_storage_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.496038 streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/app_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/browser_websocket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/component_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/media_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/stats_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/upload_file_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/websocket_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.500038 streamlit_nightly-1.34.1.dev20240508/streamlit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-09 11:52:57.000000 streamlit_nightly-1.34.1.dev20240508/streamlit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-05-09 11:52:57.000000 streamlit_nightly-1.34.1.dev20240508/streamlit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:52:57.000000 streamlit_nightly-1.34.1.dev20240508/streamlit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-09 11:52:57.000000 streamlit_nightly-1.34.1.dev20240508/streamlit_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:49:08.000000 streamlit_nightly-1.34.1.dev20240508/streamlit_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-09 11:52:57.000000 streamlit_nightly-1.34.1.dev20240508/streamlit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 11:52:57.000000 streamlit_nightly-1.34.1.dev20240508/streamlit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:52:58.500038 streamlit_nightly-1.34.1.dev20240508/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-09 11:47:27.000000 streamlit_nightly-1.34.1.dev20240508/tests/testutil.py
```

### Comparing `streamlit_nightly-1.34.1.dev20240507/PKG-INFO` & `streamlit_nightly-1.34.1.dev20240508/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.34.1.dev20240507
+Version: 1.34.1.dev20240508
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.34.1.dev20240507/bin/streamlit.cmd` & `streamlit_nightly-1.34.1.dev20240508/bin/streamlit.cmd`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/setup.py` & `streamlit_nightly-1.34.1.dev20240508/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 THIS_DIRECTORY = Path(__file__).parent
 
-VERSION = "1.34.1.dev20240507"  # PEP-440
+VERSION = "1.34.1.dev20240508"  # PEP-440
 
 # IMPORTANT: We should try very hard *not* to add dependencies to Streamlit.
 # And if you do add one, make the required version as general as possible:
 # - Include relevant lower bound for any features we use from our dependencies
 # - Always include the lower bound as >= VERSION, to keep testing min versions easy
 # - And include an upper bound that's < NEXT_MAJOR_VERSION
 INSTALL_REQUIRES = [
```

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/__main__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/case_converters.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/cli_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/cli_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/code_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/color_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/color_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/column_config.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/column_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/commands/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/commands/execution_control.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/commands/execution_control.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/commands/experimental_query_params.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/commands/experimental_query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/commands/logo.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/commands/logo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/commands/page_config.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/commands/page_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/components/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/components/lib/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/components/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/components/lib/local_component_registry.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/components/lib/local_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/components/types/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/components/types/base_component_registry.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/components/types/base_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/components/types/base_custom_component.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/components/types/base_custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/components/v1/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/components/v1/component_arrow.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/components/v1/component_registry.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/components/v1/component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/components/v1/components.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/components/v1/custom_component.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/components/v1/custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/config.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/config_option.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/config_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/connections/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/connections/base_connection.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/connections/snowflake_connection.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/connections/snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/connections/snowpark_connection.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/connections/snowpark_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/connections/sql_connection.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/connections/sql_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/connections/util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/connections/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/constants.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/constants.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/cursor.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/delta_generator.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/delta_generator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/deprecation_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/deprecation_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/development.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/echo.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/alert.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/alert.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/arrow.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/balloons.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/bokeh_chart.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/bokeh_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/code.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/code.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/deck_gl_json_chart.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/deck_gl_json_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/dialog_decorator.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/dialog_decorator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/doc_string.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/empty.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/empty.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/exception.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/form.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/form.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/graphviz_chart.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/graphviz_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/heading.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/heading.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/html.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/html.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/iframe.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/image.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/image.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/json.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/layouts.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/built_in_chart_utils.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/built_in_chart_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/column_config_utils.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/column_config_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/column_types.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/column_types.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/dialog.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/dialog.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/dicttools.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/event_utils.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/event_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/mutable_status_container.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/mutable_status_container.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/pandas_styler_utils.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/pandas_styler_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/streamlit_plotly_theme.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/streamlit_plotly_theme.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/lib/subtitle_utils.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/lib/subtitle_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/map.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/map.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/markdown.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/media.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/media.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/metric.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/metric.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/plotly_chart.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/progress.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/progress.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/pyplot.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/snow.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/spinner.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/text.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/toast.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/toast.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/utils.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/vega_charts.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/vega_charts.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Collection of chart commands that are rendered via our vega-lite chart component."""
 
 from __future__ import annotations
 
+import hashlib
 import json
+import re
 from contextlib import nullcontext
 from typing import TYPE_CHECKING, Any, Final, Literal, Sequence, cast
 
 import streamlit.elements.lib.dicttools as dicttools
 from streamlit import type_util
 from streamlit.elements.lib.built_in_chart_utils import (
     AddRowsMetadata,
@@ -28,14 +30,15 @@
     generate_chart,
 )
 from streamlit.errors import StreamlitAPIException
 from streamlit.proto.ArrowVegaLiteChart_pb2 import (
     ArrowVegaLiteChart as ArrowVegaLiteChartProto,
 )
 from streamlit.runtime.metrics_util import gather_metrics
+from streamlit.util import HASHLIB_KWARGS
 
 if TYPE_CHECKING:
     import altair as alt
 
     from streamlit.color_util import Color
     from streamlit.delta_generator import DeltaGenerator
     from streamlit.elements.arrow import Data
@@ -124,21 +127,33 @@
     spec: dict[str, Any],
     data: Data = None,
 ) -> None:
     """Adds the data to the proto and removes it from the spec dict.
     These operations will happen in-place."""
 
     # Pull data out of spec dict when it's in a 'datasets' key:
-    #   datasets: {foo: df1, bar: df2}, ...}
+    #   datasets: {foo: df1_bytes, bar: df2_bytes}, ...}
     if "datasets" in spec:
         for dataset_name, dataset_data in spec["datasets"].items():
             dataset = proto.datasets.add()
             dataset.name = str(dataset_name)
             dataset.has_name = True
-            dataset.data.data = _serialize_data(dataset_data)
+            # The ID transformer (id_transform function registered before conversion to dict)
+            # already serializes the data into Arrow IPC format (bytes) when the Altair object
+            # gets converted into the vega-lite spec dict.
+            # If its already in bytes, we don't need to serialize it here again.
+            # We just need to pass the data information into the correct proto fields.
+
+            # TODO(lukasmasuch): Are there any other cases where we need to serialize the data
+            #                    or can we remove the _serialize_data here?
+            dataset.data.data = (
+                dataset_data
+                if isinstance(dataset_data, bytes)
+                else _serialize_data(dataset_data)
+            )
         del spec["datasets"]
 
     # Pull data out of spec dict when it's in a top-level 'data' key:
     #   {data: df}
     #   {data: {values: df, ...}}
     #   {data: {url: 'url'}}
     #   {data: {name: 'foo'}}
@@ -165,36 +180,128 @@
     # chart into an array of dictionaries. To avoid that, we install a
     # transformer that replaces datasets with a reference by the object id of
     # the dataframe. We then fill in the dataset manually later on.
 
     datasets = {}
 
     def id_transform(data) -> dict[str, str]:
-        """Altair data transformer that returns a fake named dataset with the
-        object id.
+        """Altair data transformer that serializes the data,
+        creates a stable name based on the hash of the data,
+        stores the bytes into the datasets mapping and
+        returns this name to have it be used in Altair.
         """
-        name = str(id(data))
-        datasets[name] = data
+
+        # Already serialize the data to be able to create a stable
+        # dataset name:
+        data_bytes = _serialize_data(data)
+        # Use the md5 hash of the data as the name:
+        h = hashlib.new("md5", **HASHLIB_KWARGS)
+        h.update(str(data_bytes).encode("utf-8"))
+        name = h.hexdigest()
+
+        datasets[name] = data_bytes
         return {"name": name}
 
     alt.data_transformers.register("id", id_transform)  # type: ignore[attr-defined,unused-ignore]
 
     # The default altair theme has some width/height defaults defined
     # which are not useful for Streamlit. Therefore, we change the theme to
     # "none" to avoid those defaults.
     with alt.themes.enable("none") if alt.themes.active == "default" else nullcontext():  # type: ignore[attr-defined,unused-ignore]
         with alt.data_transformers.enable("id"):  # type: ignore[attr-defined,unused-ignore]
             chart_dict = altair_chart.to_dict()
 
-    # Put datasets back into the chart dict but note how they weren't
-    # transformed.
+    # Put datasets back into the chart dict:
     chart_dict["datasets"] = datasets
     return chart_dict
 
 
+def _reset_counter_pattern(prefix: str, vega_spec: str) -> str:
+    """Altair uses a global counter for unnamed parameters and views.
+    We need to reset these counters on a spec-level to make the
+    spec stable across reruns and avoid changes to the element ID.
+    """
+    pattern = re.compile(rf'"{prefix}\d+"')
+    # Get all matches without duplicates in order of appearance.
+    # Using a set here would not guarantee the order of appearance,
+    # which might lead to different replacements on each run.
+    # The order of the spec from Altair is expected to stay stable
+    # within the same session / Altair version.
+    # The order might change with Altair updates, but that's not really
+    # a case that is relevant for us since we mainly care about having
+    # this stable within a session.
+    if matches := list(dict.fromkeys(pattern.findall(vega_spec))):
+        # Add a prefix to the replacement to avoid
+        # replacing instances that already have been replaced before.
+        # The prefix here is arbitrarily chosen with the main goal
+        # that its extremely unlikely to already be part of the spec:
+        replacement_prefix = "__replace_prefix_o9hd101n22e1__"
+
+        # Replace all matches with a counter starting from 1
+        # We start from 1 to imitate the altair behavior.
+        for counter, match in enumerate(matches, start=1):
+            vega_spec = vega_spec.replace(
+                match, f'"{replacement_prefix}{prefix}{counter}"'
+            )
+
+        # Remove the prefix again from all replacements:
+        vega_spec = vega_spec.replace(replacement_prefix, "")
+    return vega_spec
+
+
+def _stabilize_vega_json_spec(vega_spec: str) -> str:
+    """Makes the chart spec stay stable across reruns and sessions.
+
+    Altair auto creates names for unnamed parameters & views. It uses a global counter
+    for the naming which will result in a different spec on every rerun.
+    In Streamlit, we need the spec to be stable across reruns and sessions to prevent the chart
+    from getting a new identity. So we need to replace the names with counter with a stable name.
+    Having a stable chart spec is also important for features like forward message cache,
+    where we don't want to have changing messages on every rerun.
+
+    Parameter counter:
+    https://github.com/vega/altair/blob/f345cd9368ae2bbc98628e9245c93fa9fb582621/altair/vegalite/v5/api.py#L196
+
+    View counter:
+    https://github.com/vega/altair/blob/f345cd9368ae2bbc98628e9245c93fa9fb582621/altair/vegalite/v5/api.py#L2885
+
+    This is temporary solution waiting for a fix for this issue:
+    https://github.com/vega/altair/issues/3416
+
+    Other solutions we considered:
+     - working on the dict object: this would require to iterate through the object and do the
+       same kind of replacement; though we would need to know the structure and since we need
+       the spec in String-format anyways, we deemed that executing the replacement on the
+       String is the better alternative
+     - resetting the counter: the counter is incremented already when the chart object is created
+       (see this GitHub issue comment https://github.com/vega/altair/issues/3416#issuecomment-2098530464),
+       so it would be too late here to reset the counter with a thread-lock to prevent interference
+       between sessions
+    """
+
+    # We only want to apply these replacements if it is really necessary
+    # since there is a risk that we replace names that where chosen by the user
+    # and thereby introduce unwanted side effects.
+
+    # We only need to apply the param_ fix if there are actually parameters defined
+    # somewhere in the spec. We can check for this by looking for the '"params"' key.
+    # This isn't a perfect check, but good enough to prevent unnecessary executions
+    # for the majority of charts.
+    if '"params"' in vega_spec:
+        vega_spec = _reset_counter_pattern("param_", vega_spec)
+
+    # Simple check if the spec contains a composite chart:
+    # https://vega.github.io/vega-lite/docs/composition.html
+    # Other charts will not contain the `view_` name,
+    # so its better to not replace this pattern.
+    if re.search(r'"(vconcat|hconcat|facet|layer|concat|repeat)"', vega_spec):
+        vega_spec = _reset_counter_pattern("view_", vega_spec)
+    return vega_spec
+
+
 class VegaChartsMixin:
     """Mix-in class for all vega-related chart commands.
 
     Altair is a python wrapper on top of the vega-lite spec. And our
     built-in chart commands are just another layer on-top of Altair.
     All of these chart commands will be eventually converted to a vega-lite
     spec and rendered using the same vega-lite chart component.
@@ -1016,15 +1123,16 @@
             data = None
 
         proto = ArrowVegaLiteChartProto()
 
         spec = _prepare_vega_lite_spec(spec, use_container_width, **kwargs)
         _marshall_chart_data(proto, spec, data)
 
-        proto.spec = json.dumps(spec)
+        # Prevent the spec from changing across reruns:
+        proto.spec = _stabilize_vega_json_spec(json.dumps(spec))
         proto.use_container_width = use_container_width
         proto.theme = theme or ""
 
         return self.dg._enqueue(
             "arrow_vega_lite_chart", proto, add_rows_metadata=add_rows_metadata
         )
```

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/button.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from streamlit.runtime.state import (
     WidgetArgs,
     WidgetCallback,
     WidgetKwargs,
     register_widget,
 )
 from streamlit.runtime.state.common import compute_widget_id, save_for_app_testing
-from streamlit.string_util import validate_emoji
+from streamlit.string_util import validate_icon_or_emoji
 from streamlit.type_util import Key, to_key
 
 if TYPE_CHECKING:
     from streamlit.delta_generator import DeltaGenerator
 
 FORM_DOCS_INFO: Final = """
 
@@ -483,19 +483,30 @@
               supported colors: blue, green, orange, red, violet, gray/grey, rainbow.
               For example, you can use ``:orange[your text here]`` or
               ``:blue-background[your text here]``.
 
             Unsupported elements are unwrapped so only their children (text contents)
             render. Display unsupported elements as literal characters by
             backslash-escaping them. E.g. ``1\. Not an ordered list``.
-        icon : str
-            An optional argument that specifies an emoji to use as
-            the icon for the link. Shortcodes are not allowed. Please use a
-            single character instead. E.g. "🚨", "🔥", "🤖", etc.
-            Defaults to ``None``, which means no icon is displayed.
+        icon : str, None
+            An optional emoji or icon to display next to the button label. If ``icon``
+            is ``None`` (default), no icon is displayed. If ``icon`` is a
+            string, the following options are valid:
+
+            * A single-character emoji. For example, you can set ``icon="🚨"``
+              or ``icon="🔥"``. Emoji short codes are not supported.
+
+            * An icon from the Material Symbols library (outlined style) in the
+              format ``":material/icon_name:"`` where "icon_name" is the name
+              of the icon in snake case.
+
+              For example, ``icon=":material/thumb_up:"`` will display the
+              Thumb Up icon. Find additional icons in the `Material Symbols \
+              <https://fonts.google.com/icons?icon.set=Material+Symbols&icon.style=Outlined>`_
+              font library.
         help : str
             An optional tooltip that gets displayed when the link is
             hovered over.
         disabled : bool
             An optional boolean, which disables the page link if set to
             ``True``. The default is ``False``.
         use_container_width : bool
@@ -658,15 +669,15 @@
         page_link_proto = PageLinkProto()
         page_link_proto.disabled = disabled
 
         if label is not None:
             page_link_proto.label = label
 
         if icon is not None:
-            page_link_proto.icon = validate_emoji(icon)
+            page_link_proto.icon = validate_icon_or_emoji(icon)
 
         if help is not None:
             page_link_proto.help = dedent(help)
 
         if use_container_width is not None:
             page_link_proto.use_container_width = use_container_width
```

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/camera_input.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/camera_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/chat.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/checkbox.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/color_picker.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/color_picker.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/data_editor.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/data_editor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/file_uploader.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/file_uploader.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/multiselect.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/multiselect.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/number_input.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/number_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/radio.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/select_slider.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/select_slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/selectbox.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/selectbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/slider.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/text_widgets.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/text_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/widgets/time_widgets.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/widgets/time_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/elements/write.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/emojis.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/emojis.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/env_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/error_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/errors.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/external/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/external/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/external/langchain/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/external/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/external/langchain/streamlit_callback_handler.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/external/langchain/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/file_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/folder_black_list.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/git_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/hello/Hello.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/hello/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/hello/pages/0_Animation_Demo.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/hello/pages/0_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/hello/pages/1_Plotting_Demo.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/hello/pages/1_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/hello/pages/2_Mapping_Demo.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/hello/pages/2_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/hello/pages/3_DataFrame_Demo.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/hello/pages/3_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/hello/utils.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/js_number.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/logger.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/material_icon_names.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/material_icon_names.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/net_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/net_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/platform.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/platform.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Alert_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Alert_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/AppPage_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/AppPage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/AppPage_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/AppPage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ArrowNamedDataSet_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ArrowNamedDataSet_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ArrowNamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ArrowVegaLiteChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ArrowVegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Arrow_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Arrow_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Arrow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Audio_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Audio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Audio_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Audio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/AutoRerun_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/AutoRerun_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/AutoRerun_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/AutoRerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/BackMsg_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/BackMsg_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/BackMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Balloons_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Balloons_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Balloons_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Block_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Block_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Block_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/BokehChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/BokehChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/BokehChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Button_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Button_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Button_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/CameraInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/CameraInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/CameraInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ChatInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ChatInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ChatInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ChatInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Checkbox_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Checkbox_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Checkbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ClientState_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ClientState_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ClientState_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Code_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Code_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ColorPicker_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ColorPicker_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ColorPicker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Common_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Common_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Components_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Components_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Components_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DataFrame_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DataFrame_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DataFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DateInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DateInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DateInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DeckGlJsonChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DeckGlJsonChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DeckGlJsonChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Delta_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Delta_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Delta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DocString_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DocString_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DocString_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DownloadButton_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/DownloadButton_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/DownloadButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Element_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Element_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Element_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Empty_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Empty_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Exception_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Exception_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Exception_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Favicon_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Favicon_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Favicon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/FileUploader_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/FileUploader_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/FileUploader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ForwardMsg_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ForwardMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ForwardMsg_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ForwardMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/GitInfo_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/GitInfo_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/GitInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/GraphVizChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/GraphVizChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/GraphVizChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Heading_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Heading_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Heading_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Heading_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Html_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Html_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Html_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Html_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/IFrame_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/IFrame_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/IFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Image_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Image_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Json_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Json_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Json_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/LabelVisibilityMessage_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/LabelVisibilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/LabelVisibilityMessage_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/LabelVisibilityMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/LinkButton_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/LinkButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/LinkButton_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/LinkButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Logo_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Logo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Logo_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Logo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Markdown_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Markdown_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Markdown_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Metric_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Metric_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/MultiSelect_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/MultiSelect_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/MultiSelect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/NamedDataSet_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/NamedDataSet_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/NamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/NewSession_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/NewSession_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/NewSession_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/NewSession_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/NumberInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/NumberInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/NumberInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageConfig_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageConfig_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageConfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageInfo_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageInfo_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageLink_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageLink_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageLink_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageLink_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageNotFound_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageNotFound_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageNotFound_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageProfile_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageProfile_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PageProfile_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PageProfile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PagesChanged_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PagesChanged_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PagesChanged_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ParentMessage_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ParentMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/ParentMessage_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/ParentMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PlotlyChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/PlotlyChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/PlotlyChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Progress_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Progress_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Progress_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Radio_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Radio_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Radio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/RootContainer_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/RootContainer_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/RootContainer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Selectbox_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Selectbox_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Selectbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/SessionEvent_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/SessionEvent_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/SessionEvent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/SessionStatus_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/SessionStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/SessionStatus_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/SessionStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Skeleton_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Skeleton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Skeleton_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Skeleton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Slider_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Slider_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Slider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Snow_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Snow_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Snow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Spinner_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Spinner_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Spinner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/TextArea_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/TextArea_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/TextArea_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/TextInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/TextInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/TextInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Text_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Text_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Text_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/TimeInput_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/TimeInput_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/TimeInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Toast_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Toast_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Toast_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Toast_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/VegaLiteChart_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/VegaLiteChart_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/VegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Video_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Video_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/Video_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/Video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/WidgetStates_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/WidgetStates_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/WidgetStates_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/openmetrics_data_model_pb2.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/proto/openmetrics_data_model_pb2.pyi` & `streamlit_nightly-1.34.1.dev20240508/streamlit/proto/openmetrics_data_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/app_session.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/app_session.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/cache_data_api.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/cache_data_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/cache_errors.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/cache_errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/cache_resource_api.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/cache_resource_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/cache_type.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/cache_type.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/cache_utils.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/cache_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/cached_message_replay.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/cached_message_replay.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/hashing.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/storage/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/storage/cache_storage_protocol.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/storage/cache_storage_protocol.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/storage/dummy_cache_storage.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/storage/dummy_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/caching/storage/local_disk_cache_storage.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/caching/storage/local_disk_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/connection_factory.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/connection_factory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/credentials.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/credentials.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/forward_msg_cache.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/forward_msg_queue.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/fragment.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/fragment.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/legacy_caching/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/legacy_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/legacy_caching/caching.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/legacy_caching/caching.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/legacy_caching/hashing.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/legacy_caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/media_file_manager.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/media_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/media_file_storage.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/memory_media_file_storage.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/memory_media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/memory_session_storage.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/memory_session_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/memory_uploaded_file_manager.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/memory_uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/metrics_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/metrics_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/runtime.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/runtime_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/runtime_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/script_data.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/script_data.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/magic.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/magic.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/magic_funcs.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/magic_funcs.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/script_cache.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/script_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/script_requests.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/script_run_context.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/script_run_context.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/scriptrunner/script_runner.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/scriptrunner/script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/secrets.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/secrets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/session_manager.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/common.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/common.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/query_params.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/query_params_proxy.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/query_params_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/safe_session_state.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/session_state.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/session_state_proxy.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/state/widgets.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/state/widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/stats.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/uploaded_file_manager.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/runtime/websocket_session_manager.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/runtime/websocket_session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/source_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/source_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/asset-manifest.json` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/asset-manifest.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8259320175438596%*

 * *Differences: {"'entrypoints'": "{insert: [(1, 'static/js/main.5a6e0ded.js')], delete: [1]}",*

 * * "'files'": "{'main.js': './static/js/main.5a6e0ded.js', 'static/js/4113.99983645.chunk.js': "*

 * *            "'./static/js/4113.99983645.chunk.js', 'static/js/6013.4ba2d616.chunk.js': "*

 * *            "'./static/js/6013.4ba2d616.chunk.js', delete: ['static/js/4113.9b2db2e3.chunk.js', "*

 * *            "'static/js/6013.64cd6d28.chunk.js']}"}*

```diff
@@ -1,16 +1,16 @@
 {
     "entrypoints": [
         "static/css/main.3aaaea00.css",
-        "static/js/main.b84b6de2.js"
+        "static/js/main.5a6e0ded.js"
     ],
     "files": {
         "index.html": "./index.html",
         "main.css": "./static/css/main.3aaaea00.css",
-        "main.js": "./static/js/main.b84b6de2.js",
+        "main.js": "./static/js/main.5a6e0ded.js",
         "static/css/3092.95a45cfe.chunk.css": "./static/css/3092.95a45cfe.chunk.css",
         "static/css/3466.8b8f33d6.chunk.css": "./static/css/3466.8b8f33d6.chunk.css",
         "static/css/5441.e3b876c5.chunk.css": "./static/css/5441.e3b876c5.chunk.css",
         "static/js/1074.73973756.chunk.js": "./static/js/1074.73973756.chunk.js",
         "static/js/1168.7452e363.chunk.js": "./static/js/1168.7452e363.chunk.js",
         "static/js/1307.0f0cca93.chunk.js": "./static/js/1307.0f0cca93.chunk.js",
         "static/js/1451.3b0a3e31.chunk.js": "./static/js/1451.3b0a3e31.chunk.js",
@@ -26,30 +26,30 @@
         "static/js/3053.7e70ec3b.chunk.js": "./static/js/3053.7e70ec3b.chunk.js",
         "static/js/3092.21bb8f7b.chunk.js": "./static/js/3092.21bb8f7b.chunk.js",
         "static/js/329.464ed8ec.chunk.js": "./static/js/329.464ed8ec.chunk.js",
         "static/js/3301.1d1b10bb.chunk.js": "./static/js/3301.1d1b10bb.chunk.js",
         "static/js/3466.05d62820.chunk.js": "./static/js/3466.05d62820.chunk.js",
         "static/js/3513.ebc278c4.chunk.js": "./static/js/3513.ebc278c4.chunk.js",
         "static/js/3631.be5c35fa.chunk.js": "./static/js/3631.be5c35fa.chunk.js",
-        "static/js/4113.9b2db2e3.chunk.js": "./static/js/4113.9b2db2e3.chunk.js",
+        "static/js/4113.99983645.chunk.js": "./static/js/4113.99983645.chunk.js",
         "static/js/4132.49bf3f2c.chunk.js": "./static/js/4132.49bf3f2c.chunk.js",
         "static/js/4177.69f9f18d.chunk.js": "./static/js/4177.69f9f18d.chunk.js",
         "static/js/4319.bf1c86bf.chunk.js": "./static/js/4319.bf1c86bf.chunk.js",
         "static/js/4477.1bd49702.chunk.js": "./static/js/4477.1bd49702.chunk.js",
         "static/js/4500.b6f348d1.chunk.js": "./static/js/4500.b6f348d1.chunk.js",
         "static/js/4666.c4b22a63.chunk.js": "./static/js/4666.c4b22a63.chunk.js",
         "static/js/474.87506447.chunk.js": "./static/js/474.87506447.chunk.js",
         "static/js/5106.44f0ff51.chunk.js": "./static/js/5106.44f0ff51.chunk.js",
         "static/js/5117.04bfe5d3.chunk.js": "./static/js/5117.04bfe5d3.chunk.js",
         "static/js/5249.f2f4070d.chunk.js": "./static/js/5249.f2f4070d.chunk.js",
         "static/js/5345.65c91ee7.chunk.js": "./static/js/5345.65c91ee7.chunk.js",
         "static/js/5379.6571574f.chunk.js": "./static/js/5379.6571574f.chunk.js",
         "static/js/5441.5bacdeda.chunk.js": "./static/js/5441.5bacdeda.chunk.js",
         "static/js/5791.9a42fb4b.chunk.js": "./static/js/5791.9a42fb4b.chunk.js",
-        "static/js/6013.64cd6d28.chunk.js": "./static/js/6013.64cd6d28.chunk.js",
+        "static/js/6013.4ba2d616.chunk.js": "./static/js/6013.4ba2d616.chunk.js",
         "static/js/6405.ac5a6f23.chunk.js": "./static/js/6405.ac5a6f23.chunk.js",
         "static/js/6718.802da17e.chunk.js": "./static/js/6718.802da17e.chunk.js",
         "static/js/6853.93dd1c4c.chunk.js": "./static/js/6853.93dd1c4c.chunk.js",
         "static/js/7142.83028745.chunk.js": "./static/js/7142.83028745.chunk.js",
         "static/js/7175.be4076bc.chunk.js": "./static/js/7175.be4076bc.chunk.js",
         "static/js/7323.b74cc85b.chunk.js": "./static/js/7323.b74cc85b.chunk.js",
         "static/js/7483.64f23be7.chunk.js": "./static/js/7483.64f23be7.chunk.js",
```

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/favicon.png` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/index.html` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.b84b6de2.js"></script><link href="./static/css/main.3aaaea00.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1,shrink-to-fit=no"/><link rel="shortcut icon" href="./favicon.png"/><link rel="preload" href="./static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2" as="font" type="font/woff2" crossorigin><link rel="preload" href="./static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2" as="font" type="font/woff2" crossorigin><title>Streamlit</title><script>window.prerenderReady=!1</script><script defer="defer" src="./static/js/main.5a6e0ded.js"></script><link href="./static/css/main.3aaaea00.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/css/3092.95a45cfe.chunk.css` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/css/3092.95a45cfe.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/css/3466.8b8f33d6.chunk.css` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/css/3466.8b8f33d6.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/css/5441.e3b876c5.chunk.css` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/css/5441.e3b876c5.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/css/main.3aaaea00.css` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/css/main.3aaaea00.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1074.73973756.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1074.73973756.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1168.7452e363.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1168.7452e363.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1307.0f0cca93.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1307.0f0cca93.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1451.3b0a3e31.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1451.3b0a3e31.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1479.6709db03.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1479.6709db03.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/178.7bea8c5d.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/178.7bea8c5d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1792.8bd6ce2a.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1792.8bd6ce2a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/1955.426e67ca.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/1955.426e67ca.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/2178.90362aae.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/2178.90362aae.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/2187.9469f035.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/2187.9469f035.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/2469.09ea79bb.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/2469.09ea79bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/2634.1249dc7a.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/2634.1249dc7a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/2736.4336e2b9.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/2736.4336e2b9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3053.7e70ec3b.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3053.7e70ec3b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3092.21bb8f7b.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3092.21bb8f7b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/329.464ed8ec.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/329.464ed8ec.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3301.1d1b10bb.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3301.1d1b10bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3466.05d62820.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3466.05d62820.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3513.ebc278c4.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3513.ebc278c4.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/3631.be5c35fa.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/3631.be5c35fa.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4113.9b2db2e3.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4113.99983645.chunk.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -2,31 +2,32 @@
 (self.webpackChunk_streamlit_app = self.webpackChunk_streamlit_app || []).push([
     [4113], {
         34113: (e, r, t) => {
             t.r(r), t.d(r, {
                 default: () => f
             });
             var o = t(66845),
-                a = t(46927),
-                n = t(68411),
-                l = t(27446),
-                i = t(63730),
-                s = t(66694),
-                d = t(84457),
-                c = t(1515);
-            const g = (0, c.Z)("div", {
+                a = t(25621),
+                n = t(22704),
+                l = t(68411),
+                i = t(27446),
+                s = t(63730),
+                d = t(66694),
+                c = t(84457),
+                g = t(1515);
+            const p = (0, g.Z)("div", {
                     target: "e11k5jya2"
                 })((e => {
                     let {} = e;
                     return {
                         display: "flex",
                         flexDirection: "column"
                     }
                 }), ""),
-                p = (0, c.Z)("a", {
+                u = (0, g.Z)("a", {
                     target: "e11k5jya1"
                 })((e => {
                     let {
                         disabled: r,
                         isCurrentPage: t,
                         fluidWidth: o,
                         theme: a
@@ -69,15 +70,15 @@
                             "&:hover": {
                                 color: a.colors.fadedText40,
                                 backgroundColor: a.colors.transparent
                             }
                         } : {}
                     }
                 }), ""),
-                u = (0, c.Z)("span", {
+                h = (0, g.Z)("span", {
                     target: "e11k5jya0"
                 })((e => {
                     let {
                         disabled: r,
                         theme: t
                     } = e;
                     return {
@@ -90,57 +91,60 @@
                             borderColor: t.colors.fadedText10,
                             backgroundColor: t.colors.transparent,
                             color: t.colors.fadedText40,
                             cursor: "not-allowed"
                         } : {}
                     }
                 }), "");
-            var h = t(40864);
+            var x = t(40864);
             const f = function(e) {
                 const {
                     onPageChange: r,
                     currentPageScriptHash: t
-                } = o.useContext(s.E), c = o.useContext(d.Z), {
-                    disabled: f,
-                    element: x,
-                    width: b
-                } = e, k = {
-                    width: b
-                }, m = function(e, r) {
+                } = o.useContext(d.E), g = o.useContext(c.Z), {
+                    colors: f
+                } = (0, a.u)(), {
+                    disabled: b,
+                    element: k,
+                    width: m
+                } = e, C = {
+                    width: m
+                }, w = function(e, r) {
                     return !(null !== e || !r) || !(null === e && !r) && !0 === e
-                }(x.useContainerWidth, c), C = t === x.pageScriptHash;
-                return (0, h.jsx)("div", {
+                }(k.useContainerWidth, g), v = t === k.pageScriptHash;
+                return (0, x.jsx)("div", {
                     className: "row-widget stPageLink",
                     "data-testid": "stPageLink",
-                    style: k,
-                    children: (0, h.jsx)(l.t, {
-                        help: x.help,
-                        placement: n.u.TOP_RIGHT,
-                        children: (0, h.jsx)(g, {
-                            children: (0, h.jsxs)(p, {
+                    style: C,
+                    children: (0, x.jsx)(i.t, {
+                        help: k.help,
+                        placement: l.u.TOP_RIGHT,
+                        children: (0, x.jsx)(p, {
+                            children: (0, x.jsxs)(u, {
                                 "data-testid": "stPageLink-NavLink",
-                                disabled: f,
-                                isCurrentPage: C,
-                                fluidWidth: !!m && b,
-                                href: x.page,
-                                target: x.external ? "_blank" : "",
+                                disabled: b,
+                                isCurrentPage: v,
+                                fluidWidth: !!w && m,
+                                href: k.page,
+                                target: k.external ? "_blank" : "",
                                 rel: "noreferrer",
                                 onClick: e => {
-                                    x.external ? f && e.preventDefault() : (e.preventDefault(), f || r(x.pageScriptHash))
+                                    k.external ? b && e.preventDefault() : (e.preventDefault(), b || r(k.pageScriptHash))
                                 },
-                                children: [x.icon && (0, h.jsx)(a.S, {
+                                children: [k.icon && (0, x.jsx)(n.p, {
                                     size: "lg",
-                                    children: x.icon
-                                }), (0, h.jsx)(u, {
-                                    disabled: f,
-                                    children: (0, h.jsx)(i.ZP, {
-                                        source: x.label,
+                                    color: f.bodyText,
+                                    iconValue: k.icon
+                                }), (0, x.jsx)(h, {
+                                    disabled: b,
+                                    children: (0, x.jsx)(s.ZP, {
+                                        source: k.label,
                                         allowHTML: !1,
                                         isLabel: !0,
-                                        boldLabel: C,
+                                        boldLabel: v,
                                         largerLabel: !0,
                                         disableLinks: !0
                                     })
                                 })]
                             })
                         })
                     })
```

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4132.49bf3f2c.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4132.49bf3f2c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4177.69f9f18d.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4177.69f9f18d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4319.bf1c86bf.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4319.bf1c86bf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4477.1bd49702.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4477.1bd49702.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4500.b6f348d1.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4500.b6f348d1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/4666.c4b22a63.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/4666.c4b22a63.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/474.87506447.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/474.87506447.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5106.44f0ff51.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5106.44f0ff51.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5117.04bfe5d3.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5117.04bfe5d3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5249.f2f4070d.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5249.f2f4070d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5345.65c91ee7.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5345.65c91ee7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5379.6571574f.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5379.6571574f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5441.5bacdeda.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5441.5bacdeda.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/5791.9a42fb4b.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/5791.9a42fb4b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/6013.64cd6d28.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/6013.4ba2d616.chunk.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -6,16 +6,16 @@
                 Z: () => d
             });
             r(66845);
             var n, o = r(50641),
                 i = r(86659),
                 a = r(50669),
                 s = r(1515);
-            const l = (0, r(7865).F4)(n || (n = (0, a.Z)(["\n  50% {\n    color: rgba(0, 0, 0, 0);\n  }\n"]))),
-                c = (0, s.Z)("span", {
+            const c = (0, r(7865).F4)(n || (n = (0, a.Z)(["\n  50% {\n    color: rgba(0, 0, 0, 0);\n  }\n"]))),
+                l = (0, s.Z)("span", {
                     target: "edlqvik0"
                 })((e => {
                     let {
                         includeDot: t,
                         shouldBlink: r,
                         theme: n
                     } = e;
@@ -27,41 +27,41 @@
                                 animation: "none",
                                 color: n.colors.gray,
                                 margin: "0 5px"
                             }
                         } : {},
                         ...r ? {
                             color: n.colors.red,
-                            animationName: "".concat(l),
+                            animationName: "".concat(c),
                             animationDuration: "0.5s",
                             animationIterationCount: 5
                         } : {}
                     }
                 }), "");
             var u = r(40864);
             const d = e => {
                 let {
                     dirty: t,
                     value: r,
                     maxLength: n,
                     className: a,
                     type: s = "single",
-                    inForm: l
+                    inForm: c
                 } = e;
                 const d = [],
                     p = function(e) {
                         let t = arguments.length > 1 && void 0 !== arguments[1] && arguments[1];
-                        d.push((0, u.jsx)(c, {
+                        d.push((0, u.jsx)(l, {
                             includeDot: d.length > 0,
                             shouldBlink: t,
                             children: e
                         }, d.length))
                     };
                 if (t) {
-                    const e = l ? "submit form" : "apply";
+                    const e = c ? "submit form" : "apply";
                     if ("multiline" === s) {
                         const t = (0, o.Ge)() ? "\u2318" : "Ctrl";
                         p("Press ".concat(t, "+Enter to ").concat(e))
                     } else "single" === s && p("Press Enter to ".concat(e))
                 }
                 return n && ("chat" !== s || t) && p("".concat(r.length, "/").concat(n), t && r.length >= n), (0, u.jsx)(i.X7, {
                     "data-testid": "InputInstructions",
@@ -93,16 +93,16 @@
                         height: 24,
                         fill: "none"
                     }), n.createElement("path", {
                         d: "M3 5.51v3.71c0 .46.31.86.76.97L11 12l-7.24 1.81c-.45.11-.76.51-.76.97v3.71c0 .72.73 1.2 1.39.92l15.42-6.49c.82-.34.82-1.5 0-1.84L4.39 4.58C3.73 4.31 3 4.79 3 5.51z"
                     }))
                 }));
             s.displayName = "Send";
-            var l = r(118),
-                c = r(46927),
+            var c = r(118),
+                l = r(46927),
                 u = r(79986),
                 d = r(27466),
                 p = r(48266),
                 f = r(1515);
             const h = (0, f.Z)("div", {
                     target: "e1d2x3se4"
                 })((e => {
@@ -207,15 +207,15 @@
                     [C, S] = (0, n.useState)(0),
                     P = (0, n.useRef)(null),
                     R = (0, n.useRef)({
                         minHeight: 0,
                         maxHeight: 0
                     }),
                     k = () => {
-                        O && (i.setStringTriggerValue(r, O, {
+                        P.current && P.current.focus(), O && (i.setStringTriggerValue(r, O, {
                             fromUi: !0
                         }, a), w(!1), j(""), S(0))
                     };
                 (0, n.useEffect)((() => {
                     if (r.setValue) {
                         r.setValue = !1;
                         const e = r.value || "";
@@ -238,15 +238,15 @@
                     maxHeight: Z
                 } = R.current, z = T ? f.colors.gray70 : f.colors.gray80, A = !!(C > 0 && P.current) && Math.abs(C - F) > 1;
                 return (0, v.jsx)(h, {
                     className: "stChatInput",
                     "data-testid": "stChatInput",
                     width: t,
                     children: (0, v.jsxs)(y, {
-                        children: [(0, v.jsx)(l.Z, {
+                        children: [(0, v.jsx)(c.Z, {
                             inputRef: P,
                             value: O,
                             placeholder: E,
                             onChange: e => {
                                 const {
                                     value: t
                                 } = e.target, {
@@ -328,15 +328,15 @@
                             })
                         }), (0, v.jsx)(b, {
                             children: (0, v.jsx)(g, {
                                 onClick: k,
                                 disabled: !x || I,
                                 extended: A,
                                 "data-testid": "stChatInputSubmitButton",
-                                children: (0, v.jsx)(c.Z, {
+                                children: (0, v.jsx)(l.Z, {
                                     content: s,
                                     size: "xl",
                                     color: "inherit"
                                 })
                             })
                         })]
                     })
@@ -348,33 +348,33 @@
                 Z: () => P
             });
             var n = r(66845),
                 o = r(80318),
                 i = r(9656),
                 a = r(38254),
                 s = r(80745),
-                l = r(98479);
+                c = r(98479);
 
-            function c(e, t) {
+            function l(e, t) {
                 var r = Object.keys(e);
                 if (Object.getOwnPropertySymbols) {
                     var n = Object.getOwnPropertySymbols(e);
                     t && (n = n.filter((function(t) {
                         return Object.getOwnPropertyDescriptor(e, t).enumerable
                     }))), r.push.apply(r, n)
                 }
                 return r
             }
 
             function u(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var r = null != arguments[t] ? arguments[t] : {};
-                    t % 2 ? c(Object(r), !0).forEach((function(t) {
+                    t % 2 ? l(Object(r), !0).forEach((function(t) {
                         d(e, t, r[t])
-                    })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : c(Object(r)).forEach((function(t) {
+                    })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(r)) : l(Object(r)).forEach((function(t) {
                         Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(r, t))
                     }))
                 }
                 return e
             }
 
             function d(e, t, r) {
@@ -382,31 +382,31 @@
                     value: r,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[t] = r, e
             }
             var p = (0, s.zo)("div", (function(e) {
-                return u(u({}, (0, l.d5)(u(u({
+                return u(u({}, (0, c.d5)(u(u({
                     $positive: !1
                 }, e), {}, {
                     $hasIconTrailing: !1
                 }))), {}, {
                     width: e.$resize ? "fit-content" : "100%"
                 })
             }));
             p.displayName = "StyledTextAreaRoot", p.displayName = "StyledTextAreaRoot";
             var f = (0, s.zo)("div", (function(e) {
-                return (0, l.hB)(u({
+                return (0, c.hB)(u({
                     $positive: !1
                 }, e))
             }));
             f.displayName = "StyledTextareaContainer", f.displayName = "StyledTextareaContainer";
             var h = (0, s.zo)("textarea", (function(e) {
-                return u(u({}, (0, l.Hx)(e)), {}, {
+                return u(u({}, (0, c.Hx)(e)), {}, {
                     resize: e.$resize || "none"
                 })
             }));
 
             function y(e) {
                 return y = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                     return typeof e
@@ -432,16 +432,16 @@
                     var r = null == e ? null : "undefined" !== typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                     if (null == r) return;
                     var n, o, i = [],
                         a = !0,
                         s = !1;
                     try {
                         for (r = r.call(e); !(a = (n = r.next()).done) && (i.push(n.value), !t || i.length !== t); a = !0);
-                    } catch (l) {
-                        s = !0, o = l
+                    } catch (c) {
+                        s = !0, o = c
                     } finally {
                         try {
                             a || null == r.return || r.return()
                         } finally {
                             if (s) throw o
                         }
                     }
@@ -530,44 +530,44 @@
                             value: e,
                             writable: !0,
                             configurable: !0
                         }
                     }), Object.defineProperty(e, "prototype", {
                         writable: !1
                     }), t && x(e, t)
-                }(c, e);
-                var t, r, s, l = w(c);
+                }(l, e);
+                var t, r, s, c = w(l);
 
-                function c() {
+                function l() {
                     var e;
                     ! function(e, t) {
                         if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                    }(this, c);
+                    }(this, l);
                     for (var t = arguments.length, r = new Array(t), n = 0; n < t; n++) r[n] = arguments[n];
-                    return C(O(e = l.call.apply(l, [this].concat(r))), "state", {
+                    return C(O(e = c.call.apply(c, [this].concat(r))), "state", {
                         isFocused: e.props.autoFocus || !1
                     }), C(O(e), "onFocus", (function(t) {
                         e.setState({
                             isFocused: !0
                         }), e.props.onFocus(t)
                     })), C(O(e), "onBlur", (function(t) {
                         e.setState({
                             isFocused: !1
                         }), e.props.onBlur(t)
                     })), e
                 }
-                return t = c, (r = [{
+                return t = l, (r = [{
                     key: "render",
                     value: function() {
                         var e = this.props.overrides,
                             t = void 0 === e ? {} : e,
                             r = b((0, o.jb)(t.Root, p), 2),
                             s = r[0],
-                            l = r[1],
-                            c = (0, o.aO)({
+                            c = r[1],
+                            l = (0, o.aO)({
                                 Input: {
                                     component: h
                                 },
                                 InputContainer: {
                                     component: f
                                 }
                             }, t);
@@ -576,25 +576,25 @@
                             $isFocused: this.state.isFocused,
                             $isReadOnly: this.props.readOnly,
                             $disabled: this.props.disabled,
                             $error: this.props.error,
                             $positive: this.props.positive,
                             $required: this.props.required,
                             $resize: this.props.resize
-                        }, l), n.createElement(i.Z, g({}, this.props, {
+                        }, c), n.createElement(i.Z, g({}, this.props, {
                             type: a.iB.textarea,
-                            overrides: c,
+                            overrides: l,
                             onFocus: this.onFocus,
                             onBlur: this.onBlur,
                             resize: this.props.resize
                         })))
                     }
                 }]) && v(t.prototype, r), s && v(t, s), Object.defineProperty(t, "prototype", {
                     writable: !1
-                }), c
+                }), l
             }(n.Component);
             C(S, "defaultProps", {
                 autoFocus: !1,
                 disabled: !1,
                 readOnly: !1,
                 error: !1,
                 name: "",
```

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/6405.ac5a6f23.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/6405.ac5a6f23.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/6718.802da17e.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/6718.802da17e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/6853.93dd1c4c.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/6853.93dd1c4c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7142.83028745.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7142.83028745.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7175.be4076bc.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7175.be4076bc.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7323.b74cc85b.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7323.b74cc85b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7483.64f23be7.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7483.64f23be7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7602.e8abc06b.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7602.e8abc06b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/7805.acc6316a.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/7805.acc6316a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8005.43974a35.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8005.43974a35.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8427.bd0a7cf3.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8427.bd0a7cf3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8477.de889fe5.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8477.de889fe5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8492.0d93bd08.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8492.0d93bd08.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8536.f8de3d9a.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8536.f8de3d9a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8570.6de19120.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8570.6de19120.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/8691.9ccf7f89.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/8691.9ccf7f89.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/9330.2b4c99e0.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/9330.2b4c99e0.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/9336.2d95d840.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/9336.2d95d840.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/937.a1248039.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/937.a1248039.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/9656.8c935274.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/9656.8c935274.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/9758.6e6d8662.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/9758.6e6d8662.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/9865.fd93213d.chunk.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/9865.fd93213d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/main.b84b6de2.js` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/main.5a6e0ded.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.b84b6de2.js.LICENSE.txt */
+/*! For license information please see main.5a6e0ded.js.LICENSE.txt */
 (() => {
     var __webpack_modules__ = {
             68785: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     B: () => i,
                     Id: () => r,
@@ -115976,29 +115976,29 @@
         2736: "4336e2b9",
         3053: "7e70ec3b",
         3092: "21bb8f7b",
         3301: "1d1b10bb",
         3466: "05d62820",
         3513: "ebc278c4",
         3631: "be5c35fa",
-        4113: "9b2db2e3",
+        4113: "99983645",
         4132: "49bf3f2c",
         4177: "69f9f18d",
         4319: "bf1c86bf",
         4477: "1bd49702",
         4500: "b6f348d1",
         4666: "c4b22a63",
         5106: "44f0ff51",
         5117: "04bfe5d3",
         5249: "f2f4070d",
         5345: "65c91ee7",
         5379: "6571574f",
         5441: "5bacdeda",
         5791: "9a42fb4b",
-        6013: "64cd6d28",
+        6013: "4ba2d616",
         6405: "ac5a6f23",
         6718: "802da17e",
         6853: "93dd1c4c",
         7142: "83028745",
         7175: "be4076bc",
         7323: "b74cc85b",
         7483: "64f23be7",
```

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/js/main.b84b6de2.js.LICENSE.txt` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/js/main.5a6e0ded.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg` & `streamlit_nightly-1.34.1.dev20240508/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/string_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/temporary_directory.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/testing/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/testing/v1/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/testing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/testing/v1/app_test.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/testing/v1/app_test.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/testing/v1/element_tree.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/testing/v1/element_tree.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/testing/v1/local_script_runner.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/testing/v1/local_script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/testing/v1/util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/testing/v1/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/time_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/time_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/type_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/type_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -778,38 +778,85 @@
     v : str
         Version string, e.g. "0.25.0"
 
     Returns
     -------
     bool
 
+
+    Raises
+    ------
+    InvalidVersion
+        If the version strings are not valid.
     """
     import pandas as pd
-    from packaging import version
 
-    return version.parse(pd.__version__) < version.parse(v)
+    return is_version_less_than(pd.__version__, v)
 
 
 def is_pyarrow_version_less_than(v: str) -> bool:
     """Return True if the current Pyarrow version is less than the input version.
 
     Parameters
     ----------
     v : str
         Version string, e.g. "0.25.0"
 
     Returns
     -------
     bool
 
+
+    Raises
+    ------
+    InvalidVersion
+        If the version strings are not valid.
+
     """
     import pyarrow as pa
+
+    return is_version_less_than(pa.__version__, v)
+
+
+def is_altair_version_less_than(v: str) -> bool:
+    """Return True if the current Altair version is less than the input version.
+
+    Parameters
+    ----------
+    v : str
+        Version string, e.g. "0.25.0"
+
+    Returns
+    -------
+    bool
+
+
+    Raises
+    ------
+    InvalidVersion
+        If the version strings are not valid.
+
+    """
+    import altair as alt
+
+    return is_version_less_than(alt.__version__, v)
+
+
+def is_version_less_than(v1: str, v2: str) -> bool:
+    """Return True if the v1 version string is less than the v2 version string
+    based on semantic versioning.
+
+    Raises
+    ------
+    InvalidVersion
+        If the version strings are not valid.
+    """
     from packaging import version
 
-    return version.parse(pa.__version__) < version.parse(v)
+    return version.parse(v1) < version.parse(v2)
 
 
 def _maybe_truncate_table(
     table: pa.Table, truncated_rows: int | None = None
 ) -> pa.Table:
     """Experimental feature to automatically truncate tables that
     are larger than the maximum allowed message size. It needs to be enabled
```

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/url_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/user_info.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/user_info.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/vendor/ipython/modified_sys_path.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/vendor/ipython/modified_sys_path.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/vendor/pympler/asizeof.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/vendor/pympler/asizeof.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/version.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/watcher/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/watcher/event_based_path_watcher.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/watcher/local_sources_watcher.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/watcher/local_sources_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/watcher/path_watcher.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/watcher/polling_path_watcher.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/watcher/util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/bootstrap.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/bootstrap.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/cache_storage_manager_config.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/cache_storage_manager_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/cli.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/cli.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/__init__.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/app_static_file_handler.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/app_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/browser_websocket_handler.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/browser_websocket_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/component_request_handler.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/component_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/media_file_handler.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/media_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/routes.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/routes.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/server.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/server.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/server_util.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/server_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/stats_request_handler.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/stats_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/upload_file_request_handler.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit/web/server/websocket_headers.py` & `streamlit_nightly-1.34.1.dev20240508/streamlit/web/server/websocket_headers.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit_nightly.egg-info/PKG-INFO` & `streamlit_nightly-1.34.1.dev20240508/streamlit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.34.1.dev20240507
+Version: 1.34.1.dev20240508
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.34.1.dev20240507/streamlit_nightly.egg-info/SOURCES.txt` & `streamlit_nightly-1.34.1.dev20240508/streamlit_nightly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
 streamlit/static/static/js/329.464ed8ec.chunk.js
 streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
 streamlit/static/static/js/3301.1d1b10bb.chunk.js
 streamlit/static/static/js/3466.05d62820.chunk.js
 streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
 streamlit/static/static/js/3513.ebc278c4.chunk.js
 streamlit/static/static/js/3631.be5c35fa.chunk.js
-streamlit/static/static/js/4113.9b2db2e3.chunk.js
+streamlit/static/static/js/4113.99983645.chunk.js
 streamlit/static/static/js/4132.49bf3f2c.chunk.js
 streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
 streamlit/static/static/js/4177.69f9f18d.chunk.js
 streamlit/static/static/js/4319.bf1c86bf.chunk.js
 streamlit/static/static/js/4477.1bd49702.chunk.js
 streamlit/static/static/js/4500.b6f348d1.chunk.js
 streamlit/static/static/js/4666.c4b22a63.chunk.js
@@ -376,15 +376,15 @@
 streamlit/static/static/js/5106.44f0ff51.chunk.js
 streamlit/static/static/js/5117.04bfe5d3.chunk.js
 streamlit/static/static/js/5249.f2f4070d.chunk.js
 streamlit/static/static/js/5345.65c91ee7.chunk.js
 streamlit/static/static/js/5379.6571574f.chunk.js
 streamlit/static/static/js/5441.5bacdeda.chunk.js
 streamlit/static/static/js/5791.9a42fb4b.chunk.js
-streamlit/static/static/js/6013.64cd6d28.chunk.js
+streamlit/static/static/js/6013.4ba2d616.chunk.js
 streamlit/static/static/js/6405.ac5a6f23.chunk.js
 streamlit/static/static/js/6718.802da17e.chunk.js
 streamlit/static/static/js/6853.93dd1c4c.chunk.js
 streamlit/static/static/js/7142.83028745.chunk.js
 streamlit/static/static/js/7175.be4076bc.chunk.js
 streamlit/static/static/js/7323.b74cc85b.chunk.js
 streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
@@ -402,16 +402,16 @@
 streamlit/static/static/js/9330.2b4c99e0.chunk.js
 streamlit/static/static/js/9336.2d95d840.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js
 streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
 streamlit/static/static/js/9656.8c935274.chunk.js
 streamlit/static/static/js/9758.6e6d8662.chunk.js
 streamlit/static/static/js/9865.fd93213d.chunk.js
-streamlit/static/static/js/main.b84b6de2.js
-streamlit/static/static/js/main.b84b6de2.js.LICENSE.txt
+streamlit/static/static/js/main.5a6e0ded.js
+streamlit/static/static/js/main.5a6e0ded.js.LICENSE.txt
 streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
 streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
 streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
 streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
 streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
```

### Comparing `streamlit_nightly-1.34.1.dev20240507/tests/testutil.py` & `streamlit_nightly-1.34.1.dev20240508/tests/testutil.py`

 * *Files identical despite different names*

