# Comparing `tmp/flet_contrib_core-2024.5.3.1625.tar.gz` & `tmp/flet_contrib_core-2024.5.9.2200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_contrib_core-2024.5.3.1625.tar", max compression
+gzip compressed data, was "flet_contrib_core-2024.5.9.2200.tar", max compression
```

## Comparing `flet_contrib_core-2024.5.3.1625.tar` & `flet_contrib_core-2024.5.9.2200.tar`

### file list

```diff
@@ -1,230 +1,230 @@
--rw-r--r--   0        0        0      189 2024-05-03 16:24:44.674319 flet_contrib_core-2024.5.3.1625/README.md
--rw-r--r--   0        0        0      673 2024-05-03 16:25:38.474630 flet_contrib_core-2024.5.3.1625/pyproject.toml
--rw-r--r--   0        0        0    10950 2024-05-03 16:24:44.674319 flet_contrib_core-2024.5.3.1625/src/flet_core/__init__.py
--rw-r--r--   0        0        0      434 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/adaptive_control.py
--rw-r--r--   0        0        0    13342 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/alert_dialog.py
--rw-r--r--   0        0        0      407 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/alignment.py
--rw-r--r--   0        0        0     6757 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/animated_switcher.py
--rw-r--r--   0        0        0     1955 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/animation.py
--rw-r--r--   0        0        0    11031 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/app_bar.py
--rw-r--r--   0        0        0     7915 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/audio.py
--rw-r--r--   0        0        0     8439 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/audio_recorder.py
--rw-r--r--   0        0        0     5781 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/badge.py
--rw-r--r--   0        0        0     8099 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/banner.py
--rw-r--r--   0        0        0      326 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/blur.py
--rw-r--r--   0        0        0     1079 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/border.py
--rw-r--r--   0        0        0      958 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/border_radius.py
--rw-r--r--   0        0        0     5930 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/bottom_app_bar.py
--rw-r--r--   0        0        0     5830 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/bottom_sheet.py
--rw-r--r--   0        0        0     2103 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/buttons.py
--rw-r--r--   0        0        0      514 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__init__.py
--rw-r--r--   0        0        0      853 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3531 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/arc.cpython-39.pyc
--rw-r--r--   0        0        0     4806 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/canvas.cpython-39.pyc
--rw-r--r--   0        0        0     2359 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/circle.cpython-39.pyc
--rw-r--r--   0        0        0     1807 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/color.cpython-39.pyc
--rw-r--r--   0        0        0     1446 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/fill.cpython-39.pyc
--rw-r--r--   0        0        0     2603 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/line.cpython-39.pyc
--rw-r--r--   0        0        0     2613 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/oval.cpython-39.pyc
--rw-r--r--   0        0        0     4863 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/path.cpython-39.pyc
--rw-r--r--   0        0        0     2497 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/points.cpython-39.pyc
--rw-r--r--   0        0        0     3012 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/rect.cpython-39.pyc
--rw-r--r--   0        0        0     2541 2024-05-03 16:24:44.682319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/shadow.cpython-39.pyc
--rw-r--r--   0        0        0      711 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/shape.cpython-39.pyc
--rw-r--r--   0        0        0     4886 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/text.cpython-39.pyc
--rw-r--r--   0        0        0     2910 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/arc.py
--rw-r--r--   0        0        0     4813 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/canvas.py
--rw-r--r--   0        0        0     1646 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/circle.py
--rw-r--r--   0        0        0     1236 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/color.py
--rw-r--r--   0        0        0      844 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/fill.py
--rw-r--r--   0        0        0     1869 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/line.py
--rw-r--r--   0        0        0     1891 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/oval.py
--rw-r--r--   0        0        0     3493 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/path.py
--rw-r--r--   0        0        0     1813 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/points.py
--rw-r--r--   0        0        0     2345 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/rect.py
--rw-r--r--   0        0        0     1951 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/shadow.py
--rw-r--r--   0        0        0      347 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/shape.py
--rw-r--r--   0        0        0     4172 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/text.py
--rw-r--r--   0        0        0     8220 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/card.py
--rw-r--r--   0        0        0     9191 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/bar_chart.cpython-39.pyc
--rw-r--r--   0        0        0     2768 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/bar_chart_group.cpython-39.pyc
--rw-r--r--   0        0        0     7271 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/bar_chart_rod.cpython-39.pyc
--rw-r--r--   0        0        0     2649 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/bar_chart_rod_stack_item.cpython-39.pyc
--rw-r--r--   0        0        0     3321 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/chart_axis.cpython-39.pyc
--rw-r--r--   0        0        0     1874 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/chart_axis_label.cpython-39.pyc
--rw-r--r--   0        0        0      700 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/chart_grid_lines.cpython-39.pyc
--rw-r--r--   0        0        0      661 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/chart_point_line.cpython-39.pyc
--rw-r--r--   0        0        0     1548 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/chart_point_shape.cpython-39.pyc
--rw-r--r--   0        0        0    10724 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/line_chart.cpython-39.pyc
--rw-r--r--   0        0        0     9164 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/line_chart_data.cpython-39.pyc
--rw-r--r--   0        0        0     5943 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/line_chart_data_point.cpython-39.pyc
--rw-r--r--   0        0        0     5571 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/pie_chart.cpython-39.pyc
--rw-r--r--   0        0        0     4518 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/pie_chart_section.cpython-39.pyc
--rw-r--r--   0        0        0     9932 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/bar_chart.py
--rw-r--r--   0        0        0     2044 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/bar_chart_group.py
--rw-r--r--   0        0        0     6679 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/bar_chart_rod.py
--rw-r--r--   0        0        0     1932 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/bar_chart_rod_stack_item.py
--rw-r--r--   0        0        0     2923 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/chart_axis.py
--rw-r--r--   0        0        0     1293 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/chart_axis_label.py
--rw-r--r--   0        0        0      338 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/chart_grid_lines.py
--rw-r--r--   0        0        0      286 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/chart_point_line.py
--rw-r--r--   0        0        0     1006 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/chart_point_shape.py
--rw-r--r--   0        0        0    11305 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/line_chart.py
--rw-r--r--   0        0        0     9357 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/line_chart_data.py
--rw-r--r--   0        0        0     5338 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/line_chart_data_point.py
--rw-r--r--   0        0        0     5965 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/pie_chart.py
--rw-r--r--   0        0        0     3807 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/charts/pie_chart_section.py
--rw-r--r--   0        0        0    12179 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/checkbox.py
--rw-r--r--   0        0        0    14830 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/chip.py
--rw-r--r--   0        0        0     9261 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/circle_avatar.py
--rw-r--r--   0        0        0     3097 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/client_storage.py
--rw-r--r--   0        0        0    10869 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/colors.py
--rw-r--r--   0        0        0     6968 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/column.py
--rw-r--r--   0        0        0      877 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/connection.py
--rw-r--r--   0        0        0     7224 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/constrained_control.py
--rw-r--r--   0        0        0    15069 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/container.py
--rw-r--r--   0        0        0    17732 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/control.py
--rw-r--r--   0        0        0      260 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/control_event.py
--rw-r--r--   0        0        0     4387 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_action_sheet.py
--rw-r--r--   0        0        0     4507 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_action_sheet_action.py
--rw-r--r--   0        0        0     3102 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_activity_indicator.py
--rw-r--r--   0        0        0     3947 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_alert_dialog.py
--rw-r--r--   0        0        0     5453 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_app_bar.py
--rw-r--r--   0        0        0     3108 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_bottom_sheet.py
--rw-r--r--   0        0        0     7697 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_button.py
--rw-r--r--   0        0        0     6851 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_checkbox.py
--rw-r--r--   0        0        0     2260 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_colors.py
--rw-r--r--   0        0        0     2464 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_context_menu.py
--rw-r--r--   0        0        0     3016 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_context_menu_action.py
--rw-r--r--   0        0        0     8126 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_date_picker.py
--rw-r--r--   0        0        0     3667 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_dialog_action.py
--rw-r--r--   0        0        0     2706 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_filled_button.py
--rw-r--r--   0        0        0    61696 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_icons.py
--rw-r--r--   0        0        0     9207 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_list_tile.py
--rw-r--r--   0        0        0     6378 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_navigation_bar.py
--rw-r--r--   0        0        0     6847 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_picker.py
--rw-r--r--   0        0        0     6833 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_radio.py
--rw-r--r--   0        0        0     5590 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_segmented_button.py
--rw-r--r--   0        0        0     6429 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_slider.py
--rw-r--r--   0        0        0     4722 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_sliding_segmented_button.py
--rw-r--r--   0        0        0     7545 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_switch.py
--rw-r--r--   0        0        0    10254 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_textfield.py
--rw-r--r--   0        0        0     5308 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_timer_picker.py
--rw-r--r--   0        0        0    21708 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/datatable.py
--rw-r--r--   0        0        0    11675 2024-05-03 16:24:44.686319 flet_contrib_core-2024.5.3.1625/src/flet_core/date_picker.py
--rw-r--r--   0        0        0    10163 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/dismissible.py
--rw-r--r--   0        0        0     3081 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/divider.py
--rw-r--r--   0        0        0     7147 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/drag_target.py
--rw-r--r--   0        0        0     6701 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/draggable.py
--rw-r--r--   0        0        0    14762 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/dropdown.py
--rw-r--r--   0        0        0    10571 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/elevated_button.py
--rw-r--r--   0        0        0     1978 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/embed_json_encoder.py
--rw-r--r--   0        0        0      166 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/event.py
--rw-r--r--   0        0        0     1250 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/event_handler.py
--rw-r--r--   0        0        0     9795 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/expansion_panel.py
--rw-r--r--   0        0        0    13461 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/expansion_tile.py
--rw-r--r--   0        0        0     9659 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/file_picker.py
--rw-r--r--   0        0        0     2886 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/filled_button.py
--rw-r--r--   0        0        0     3020 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/filled_tonal_button.py
--rw-r--r--   0        0        0     3608 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/flet_app.py
--rw-r--r--   0        0        0    11149 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/floating_action_button.py
--rw-r--r--   0        0        0    15979 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/form_field_control.py
--rw-r--r--   0        0        0    27285 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/gesture_detector.py
--rw-r--r--   0        0        0     1432 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/gradients.py
--rw-r--r--   0        0        0     8485 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/grid_view.py
--rw-r--r--   0        0        0     2315 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/haptic_feedback.py
--rw-r--r--   0        0        0     3849 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/icon.py
--rw-r--r--   0        0        0    13137 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/icon_button.py
--rw-r--r--   0        0        0   362386 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/icons.py
--rw-r--r--   0        0        0     7812 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/image.py
--rw-r--r--   0        0        0      367 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/inline_span.py
--rw-r--r--   0        0        0    17916 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/list_tile.py
--rw-r--r--   0        0        0     8075 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/list_view.py
--rw-r--r--   0        0        0    10049 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/local_connection.py
--rw-r--r--   0        0        0      219 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/locks.py
--rw-r--r--   0        0        0     5591 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/lottie.py
--rw-r--r--   0        0        0      583 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/margin.py
--rw-r--r--   0        0        0     5894 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/markdown.py
--rw-r--r--   0        0        0     5015 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/matplotlib_chart.py
--rw-r--r--   0        0        0     4319 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/menu_bar.py
--rw-r--r--   0        0        0     7484 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/menu_item_button.py
--rw-r--r--   0        0        0     1486 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/merge_semantics.py
--rw-r--r--   0        0        0    11864 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/navigation_bar.py
--rw-r--r--   0        0        0     9992 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/navigation_drawer.py
--rw-r--r--   0        0        0    15476 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/navigation_rail.py
--rw-r--r--   0        0        0     8550 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/outlined_button.py
--rw-r--r--   0        0        0      587 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/padding.py
--rw-r--r--   0        0        0    63608 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/page.py
--rw-r--r--   0        0        0    10503 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/pagelet.py
--rw-r--r--   0        0        0     2746 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/painting.py
--rw-r--r--   0        0        0     4235 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/plotly_chart.py
--rw-r--r--   0        0        0    13789 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/popup_menu_button.py
--rw-r--r--   0        0        0     5600 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/progress_bar.py
--rw-r--r--   0        0        0     5663 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/progress_ring.py
--rw-r--r--   0        0        0     4163 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/protocol.py
--rw-r--r--   0        0        0      106 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/pubsub/__init__.py
--rw-r--r--   0        0        0      317 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/pubsub/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4527 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/pubsub/__pycache__/pubsub_client.cpython-39.pyc
--rw-r--r--   0        0        0     5627 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/pubsub/__pycache__/pubsub_hub.cpython-39.pyc
--rw-r--r--   0        0        0     3393 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/pubsub/pubsub_client.py
--rw-r--r--   0        0        0     5873 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/pubsub/pubsub_hub.py
--rw-r--r--   0        0        0     3419 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/querystring.py
--rw-r--r--   0        0        0     9309 2024-05-03 16:24:44.690319 flet_contrib_core-2024.5.3.1625/src/flet_core/radio.py
--rw-r--r--   0        0        0     2350 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/radio_group.py
--rw-r--r--   0        0        0     8133 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/range_slider.py
--rw-r--r--   0        0        0      291 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/ref.py
--rw-r--r--   0        0        0     6438 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/responsive_row.py
--rw-r--r--   0        0        0     5326 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/rive.py
--rw-r--r--   0        0        0     6989 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/row.py
--rw-r--r--   0        0        0     5151 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/safe_area.py
--rw-r--r--   0        0        0     4513 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/scrollable_control.py
--rw-r--r--   0        0        0    14078 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/search_bar.py
--rw-r--r--   0        0        0     8430 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/segmented_button.py
--rw-r--r--   0        0        0     1690 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/selection_area.py
--rw-r--r--   0        0        0    16317 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/semantics.py
--rw-r--r--   0        0        0     1186 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/semantics_service.py
--rw-r--r--   0        0        0      576 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/session_storage.py
--rw-r--r--   0        0        0     5260 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/shader_mask.py
--rw-r--r--   0        0        0      572 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/shadow.py
--rw-r--r--   0        0        0     2938 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/shake_detector.py
--rw-r--r--   0        0        0    10403 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/slider.py
--rw-r--r--   0        0        0     8473 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/snack_bar.py
--rw-r--r--   0        0        0     5651 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/stack.py
--rw-r--r--   0        0        0     8403 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/submenu_button.py
--rw-r--r--   0        0        0    11516 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/switch.py
--rw-r--r--   0        0        0    14308 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/tabs.py
--rw-r--r--   0        0        0      632 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/template_route.py
--rw-r--r--   0        0        0    10900 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/text.py
--rw-r--r--   0        0        0     8065 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/text_button.py
--rw-r--r--   0        0        0     3282 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/text_span.py
--rw-r--r--   0        0        0     1375 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/text_style.py
--rw-r--r--   0        0        0    18286 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/textfield.py
--rw-r--r--   0        0        0    32507 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/theme.py
--rw-r--r--   0        0        0     8094 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/time_picker.py
--rw-r--r--   0        0        0     9157 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/tooltip.py
--rw-r--r--   0        0        0      544 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/transform.py
--rw-r--r--   0        0        0     2847 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/transparent_pointer.py
--rw-r--r--   0        0        0     3476 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/two_dimensional_scrollables.py
--rw-r--r--   0        0        0     6265 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/types.py
--rw-r--r--   0        0        0      450 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/user_control.py
--rw-r--r--   0        0        0      311 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__init__.py
--rw-r--r--   0        0        0      574 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      830 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/classproperty.cpython-39.pyc
--rw-r--r--   0        0        0      569 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/concurrency_utils.cpython-39.pyc
--rw-r--r--   0        0        0     1227 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/deprecated.cpython-39.pyc
--rw-r--r--   0        0        0      699 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/slugify.cpython-39.pyc
--rw-r--r--   0        0        0      572 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/strings.cpython-39.pyc
--rw-r--r--   0        0        0     4694 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/vector.cpython-39.pyc
--rw-r--r--   0        0        0      271 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/classproperty.py
--rw-r--r--   0        0        0      243 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/concurrency_utils.py
--rw-r--r--   0        0        0      835 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/deprecated.py
--rw-r--r--   0        0        0      465 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/slugify.py
--rw-r--r--   0        0        0      178 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/strings.py
--rw-r--r--   0        0        0     3207 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/utils/vector.py
--rw-r--r--   0        0        0       96 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/version.py
--rw-r--r--   0        0        0     3123 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/vertical_divider.py
--rw-r--r--   0        0        0    17853 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/video.py
--rw-r--r--   0        0        0     8864 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/view.py
--rw-r--r--   0        0        0     6042 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/webview.py
--rw-r--r--   0        0        0     4181 2024-05-03 16:24:44.694319 flet_contrib_core-2024.5.3.1625/src/flet_core/window_drag_area.py
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 flet_contrib_core-2024.5.3.1625/PKG-INFO
+-rw-r--r--   0        0        0      189 2024-05-09 22:00:04.998540 flet_contrib_core-2024.5.9.2200/README.md
+-rw-r--r--   0        0        0      673 2024-05-09 22:00:53.967443 flet_contrib_core-2024.5.9.2200/pyproject.toml
+-rw-r--r--   0        0        0    10950 2024-05-09 22:00:04.998540 flet_contrib_core-2024.5.9.2200/src/flet_core/__init__.py
+-rw-r--r--   0        0        0      434 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/adaptive_control.py
+-rw-r--r--   0        0        0    13342 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/alert_dialog.py
+-rw-r--r--   0        0        0      407 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/alignment.py
+-rw-r--r--   0        0        0     6757 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/animated_switcher.py
+-rw-r--r--   0        0        0     1955 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/animation.py
+-rw-r--r--   0        0        0    11031 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/app_bar.py
+-rw-r--r--   0        0        0     7915 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/audio.py
+-rw-r--r--   0        0        0     8439 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/audio_recorder.py
+-rw-r--r--   0        0        0     5781 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/badge.py
+-rw-r--r--   0        0        0     8099 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/banner.py
+-rw-r--r--   0        0        0      326 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/blur.py
+-rw-r--r--   0        0        0     1079 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/border.py
+-rw-r--r--   0        0        0      958 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/border_radius.py
+-rw-r--r--   0        0        0     5930 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/bottom_app_bar.py
+-rw-r--r--   0        0        0     5830 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/bottom_sheet.py
+-rw-r--r--   0        0        0     2103 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/buttons.py
+-rw-r--r--   0        0        0      514 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__init__.py
+-rw-r--r--   0        0        0      853 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3531 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/arc.cpython-39.pyc
+-rw-r--r--   0        0        0     4806 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/canvas.cpython-39.pyc
+-rw-r--r--   0        0        0     2359 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/circle.cpython-39.pyc
+-rw-r--r--   0        0        0     1807 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/color.cpython-39.pyc
+-rw-r--r--   0        0        0     1446 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/fill.cpython-39.pyc
+-rw-r--r--   0        0        0     2603 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/line.cpython-39.pyc
+-rw-r--r--   0        0        0     2613 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/oval.cpython-39.pyc
+-rw-r--r--   0        0        0     4863 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/path.cpython-39.pyc
+-rw-r--r--   0        0        0     2497 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/points.cpython-39.pyc
+-rw-r--r--   0        0        0     3012 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/rect.cpython-39.pyc
+-rw-r--r--   0        0        0     2541 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/shadow.cpython-39.pyc
+-rw-r--r--   0        0        0      711 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/shape.cpython-39.pyc
+-rw-r--r--   0        0        0     4886 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/text.cpython-39.pyc
+-rw-r--r--   0        0        0     2910 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/arc.py
+-rw-r--r--   0        0        0     4813 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/canvas.py
+-rw-r--r--   0        0        0     1646 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/circle.py
+-rw-r--r--   0        0        0     1236 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/color.py
+-rw-r--r--   0        0        0      844 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/fill.py
+-rw-r--r--   0        0        0     1869 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/line.py
+-rw-r--r--   0        0        0     1891 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/oval.py
+-rw-r--r--   0        0        0     3493 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/path.py
+-rw-r--r--   0        0        0     1813 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/points.py
+-rw-r--r--   0        0        0     2345 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/rect.py
+-rw-r--r--   0        0        0     1951 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/shadow.py
+-rw-r--r--   0        0        0      347 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/shape.py
+-rw-r--r--   0        0        0     4172 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/text.py
+-rw-r--r--   0        0        0     8220 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/card.py
+-rw-r--r--   0        0        0     9191 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/bar_chart.cpython-39.pyc
+-rw-r--r--   0        0        0     2768 2024-05-09 22:00:05.010540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/bar_chart_group.cpython-39.pyc
+-rw-r--r--   0        0        0     7271 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/bar_chart_rod.cpython-39.pyc
+-rw-r--r--   0        0        0     2649 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/bar_chart_rod_stack_item.cpython-39.pyc
+-rw-r--r--   0        0        0     3321 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/chart_axis.cpython-39.pyc
+-rw-r--r--   0        0        0     1874 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/chart_axis_label.cpython-39.pyc
+-rw-r--r--   0        0        0      700 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/chart_grid_lines.cpython-39.pyc
+-rw-r--r--   0        0        0      661 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/chart_point_line.cpython-39.pyc
+-rw-r--r--   0        0        0     1548 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/chart_point_shape.cpython-39.pyc
+-rw-r--r--   0        0        0    10724 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/line_chart.cpython-39.pyc
+-rw-r--r--   0        0        0     9164 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/line_chart_data.cpython-39.pyc
+-rw-r--r--   0        0        0     5943 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/line_chart_data_point.cpython-39.pyc
+-rw-r--r--   0        0        0     5571 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/pie_chart.cpython-39.pyc
+-rw-r--r--   0        0        0     4518 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/pie_chart_section.cpython-39.pyc
+-rw-r--r--   0        0        0     9932 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/bar_chart.py
+-rw-r--r--   0        0        0     2044 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/bar_chart_group.py
+-rw-r--r--   0        0        0     6679 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/bar_chart_rod.py
+-rw-r--r--   0        0        0     1932 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/bar_chart_rod_stack_item.py
+-rw-r--r--   0        0        0     2923 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/chart_axis.py
+-rw-r--r--   0        0        0     1293 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/chart_axis_label.py
+-rw-r--r--   0        0        0      338 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/chart_grid_lines.py
+-rw-r--r--   0        0        0      286 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/chart_point_line.py
+-rw-r--r--   0        0        0     1006 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/chart_point_shape.py
+-rw-r--r--   0        0        0    11305 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/line_chart.py
+-rw-r--r--   0        0        0     9357 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/line_chart_data.py
+-rw-r--r--   0        0        0     5338 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/line_chart_data_point.py
+-rw-r--r--   0        0        0     5965 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/pie_chart.py
+-rw-r--r--   0        0        0     3807 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/charts/pie_chart_section.py
+-rw-r--r--   0        0        0    12179 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/checkbox.py
+-rw-r--r--   0        0        0    14830 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/chip.py
+-rw-r--r--   0        0        0     9261 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/circle_avatar.py
+-rw-r--r--   0        0        0     3097 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/client_storage.py
+-rw-r--r--   0        0        0    10869 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/colors.py
+-rw-r--r--   0        0        0     6968 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/column.py
+-rw-r--r--   0        0        0      877 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/connection.py
+-rw-r--r--   0        0        0     7224 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/constrained_control.py
+-rw-r--r--   0        0        0    15069 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/container.py
+-rw-r--r--   0        0        0    17732 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/control.py
+-rw-r--r--   0        0        0      260 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/control_event.py
+-rw-r--r--   0        0        0     4387 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_action_sheet.py
+-rw-r--r--   0        0        0     4507 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_action_sheet_action.py
+-rw-r--r--   0        0        0     3102 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_activity_indicator.py
+-rw-r--r--   0        0        0     3947 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_alert_dialog.py
+-rw-r--r--   0        0        0     5453 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_app_bar.py
+-rw-r--r--   0        0        0     3108 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_bottom_sheet.py
+-rw-r--r--   0        0        0     7697 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_button.py
+-rw-r--r--   0        0        0     6851 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_checkbox.py
+-rw-r--r--   0        0        0     2260 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_colors.py
+-rw-r--r--   0        0        0     2464 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_context_menu.py
+-rw-r--r--   0        0        0     3016 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_context_menu_action.py
+-rw-r--r--   0        0        0     8126 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_date_picker.py
+-rw-r--r--   0        0        0     3667 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_dialog_action.py
+-rw-r--r--   0        0        0     2706 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_filled_button.py
+-rw-r--r--   0        0        0    61696 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_icons.py
+-rw-r--r--   0        0        0     9207 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_list_tile.py
+-rw-r--r--   0        0        0     6378 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_navigation_bar.py
+-rw-r--r--   0        0        0     6847 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_picker.py
+-rw-r--r--   0        0        0     6833 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_radio.py
+-rw-r--r--   0        0        0     5590 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_segmented_button.py
+-rw-r--r--   0        0        0     6429 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_slider.py
+-rw-r--r--   0        0        0     4722 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_sliding_segmented_button.py
+-rw-r--r--   0        0        0     7545 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_switch.py
+-rw-r--r--   0        0        0    10254 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_textfield.py
+-rw-r--r--   0        0        0     5308 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_timer_picker.py
+-rw-r--r--   0        0        0    21708 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/datatable.py
+-rw-r--r--   0        0        0    11675 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/date_picker.py
+-rw-r--r--   0        0        0    10163 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/dismissible.py
+-rw-r--r--   0        0        0     3081 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/divider.py
+-rw-r--r--   0        0        0     7147 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/drag_target.py
+-rw-r--r--   0        0        0     6701 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/draggable.py
+-rw-r--r--   0        0        0    14762 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/dropdown.py
+-rw-r--r--   0        0        0    10571 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/elevated_button.py
+-rw-r--r--   0        0        0     1978 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/embed_json_encoder.py
+-rw-r--r--   0        0        0      166 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/event.py
+-rw-r--r--   0        0        0     1250 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/event_handler.py
+-rw-r--r--   0        0        0     9795 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/expansion_panel.py
+-rw-r--r--   0        0        0    13461 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/expansion_tile.py
+-rw-r--r--   0        0        0     9659 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/file_picker.py
+-rw-r--r--   0        0        0     2886 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/filled_button.py
+-rw-r--r--   0        0        0     3020 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/filled_tonal_button.py
+-rw-r--r--   0        0        0     3608 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/flet_app.py
+-rw-r--r--   0        0        0    11149 2024-05-09 22:00:05.014540 flet_contrib_core-2024.5.9.2200/src/flet_core/floating_action_button.py
+-rw-r--r--   0        0        0    15979 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/form_field_control.py
+-rw-r--r--   0        0        0    27285 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/gesture_detector.py
+-rw-r--r--   0        0        0     1432 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/gradients.py
+-rw-r--r--   0        0        0     8485 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/grid_view.py
+-rw-r--r--   0        0        0     2315 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/haptic_feedback.py
+-rw-r--r--   0        0        0     3849 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/icon.py
+-rw-r--r--   0        0        0    13137 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/icon_button.py
+-rw-r--r--   0        0        0   362386 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/icons.py
+-rw-r--r--   0        0        0     7812 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/image.py
+-rw-r--r--   0        0        0      367 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/inline_span.py
+-rw-r--r--   0        0        0    17916 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/list_tile.py
+-rw-r--r--   0        0        0     8075 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/list_view.py
+-rw-r--r--   0        0        0    10049 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/local_connection.py
+-rw-r--r--   0        0        0      219 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/locks.py
+-rw-r--r--   0        0        0     5591 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/lottie.py
+-rw-r--r--   0        0        0      583 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/margin.py
+-rw-r--r--   0        0        0     5894 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/markdown.py
+-rw-r--r--   0        0        0     5015 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/matplotlib_chart.py
+-rw-r--r--   0        0        0     4319 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/menu_bar.py
+-rw-r--r--   0        0        0     7484 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/menu_item_button.py
+-rw-r--r--   0        0        0     1486 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/merge_semantics.py
+-rw-r--r--   0        0        0    11864 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/navigation_bar.py
+-rw-r--r--   0        0        0     9992 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/navigation_drawer.py
+-rw-r--r--   0        0        0    15476 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/navigation_rail.py
+-rw-r--r--   0        0        0     8550 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/outlined_button.py
+-rw-r--r--   0        0        0      587 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/padding.py
+-rw-r--r--   0        0        0    63608 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/page.py
+-rw-r--r--   0        0        0    10503 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/pagelet.py
+-rw-r--r--   0        0        0     2746 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/painting.py
+-rw-r--r--   0        0        0     4235 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/plotly_chart.py
+-rw-r--r--   0        0        0    13789 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/popup_menu_button.py
+-rw-r--r--   0        0        0     5600 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/progress_bar.py
+-rw-r--r--   0        0        0     5663 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/progress_ring.py
+-rw-r--r--   0        0        0     4163 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/protocol.py
+-rw-r--r--   0        0        0      106 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/pubsub/__init__.py
+-rw-r--r--   0        0        0      317 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/pubsub/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4527 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/pubsub/__pycache__/pubsub_client.cpython-39.pyc
+-rw-r--r--   0        0        0     5627 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/pubsub/__pycache__/pubsub_hub.cpython-39.pyc
+-rw-r--r--   0        0        0     3393 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/pubsub/pubsub_client.py
+-rw-r--r--   0        0        0     5873 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/pubsub/pubsub_hub.py
+-rw-r--r--   0        0        0     3419 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/querystring.py
+-rw-r--r--   0        0        0     9309 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/radio.py
+-rw-r--r--   0        0        0     2350 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/radio_group.py
+-rw-r--r--   0        0        0     8133 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/range_slider.py
+-rw-r--r--   0        0        0      291 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/ref.py
+-rw-r--r--   0        0        0     6438 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/responsive_row.py
+-rw-r--r--   0        0        0     5326 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/rive.py
+-rw-r--r--   0        0        0     6989 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/row.py
+-rw-r--r--   0        0        0     5151 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/safe_area.py
+-rw-r--r--   0        0        0     4513 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/scrollable_control.py
+-rw-r--r--   0        0        0    14078 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/search_bar.py
+-rw-r--r--   0        0        0     8430 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/segmented_button.py
+-rw-r--r--   0        0        0     1690 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/selection_area.py
+-rw-r--r--   0        0        0    16317 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/semantics.py
+-rw-r--r--   0        0        0     1186 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/semantics_service.py
+-rw-r--r--   0        0        0      576 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/session_storage.py
+-rw-r--r--   0        0        0     5260 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/shader_mask.py
+-rw-r--r--   0        0        0      572 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/shadow.py
+-rw-r--r--   0        0        0     2938 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/shake_detector.py
+-rw-r--r--   0        0        0    10403 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/slider.py
+-rw-r--r--   0        0        0     8473 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/snack_bar.py
+-rw-r--r--   0        0        0     5651 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/stack.py
+-rw-r--r--   0        0        0     8403 2024-05-09 22:00:05.018540 flet_contrib_core-2024.5.9.2200/src/flet_core/submenu_button.py
+-rw-r--r--   0        0        0    11516 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/switch.py
+-rw-r--r--   0        0        0    14308 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/tabs.py
+-rw-r--r--   0        0        0      632 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/template_route.py
+-rw-r--r--   0        0        0    10900 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/text.py
+-rw-r--r--   0        0        0     8065 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/text_button.py
+-rw-r--r--   0        0        0     3282 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/text_span.py
+-rw-r--r--   0        0        0     1375 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/text_style.py
+-rw-r--r--   0        0        0    18286 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/textfield.py
+-rw-r--r--   0        0        0    32507 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/theme.py
+-rw-r--r--   0        0        0     8094 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/time_picker.py
+-rw-r--r--   0        0        0     9157 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/tooltip.py
+-rw-r--r--   0        0        0      544 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/transform.py
+-rw-r--r--   0        0        0     2847 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/transparent_pointer.py
+-rw-r--r--   0        0        0     4003 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/two_dimensional_scrollables.py
+-rw-r--r--   0        0        0     6265 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/types.py
+-rw-r--r--   0        0        0      450 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/user_control.py
+-rw-r--r--   0        0        0      311 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__init__.py
+-rw-r--r--   0        0        0      574 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      830 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/classproperty.cpython-39.pyc
+-rw-r--r--   0        0        0      569 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/concurrency_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     1227 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/deprecated.cpython-39.pyc
+-rw-r--r--   0        0        0      699 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/slugify.cpython-39.pyc
+-rw-r--r--   0        0        0      572 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/strings.cpython-39.pyc
+-rw-r--r--   0        0        0     4694 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/vector.cpython-39.pyc
+-rw-r--r--   0        0        0      271 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/classproperty.py
+-rw-r--r--   0        0        0      243 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/concurrency_utils.py
+-rw-r--r--   0        0        0      835 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/deprecated.py
+-rw-r--r--   0        0        0      465 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/slugify.py
+-rw-r--r--   0        0        0      178 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/strings.py
+-rw-r--r--   0        0        0     3207 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/utils/vector.py
+-rw-r--r--   0        0        0       96 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/version.py
+-rw-r--r--   0        0        0     3123 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/vertical_divider.py
+-rw-r--r--   0        0        0    17853 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/video.py
+-rw-r--r--   0        0        0     8864 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/view.py
+-rw-r--r--   0        0        0     6042 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/webview.py
+-rw-r--r--   0        0        0     4181 2024-05-09 22:00:05.022540 flet_contrib_core-2024.5.9.2200/src/flet_core/window_drag_area.py
+-rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 flet_contrib_core-2024.5.9.2200/PKG-INFO
```

### Comparing `flet_contrib_core-2024.5.3.1625/pyproject.toml` & `flet_contrib_core-2024.5.9.2200/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-contrib-core"
-version = "2024.05.03.1625"
+version = "2024.05.09.2200"
 description = "Flet core library"
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_core", from = "src" },
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/__init__.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/alert_dialog.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/animated_switcher.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/animated_switcher.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/animation.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/animation.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/app_bar.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/audio.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/audio.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/audio_recorder.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/audio_recorder.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/badge.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/badge.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/banner.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/banner.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/border.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/border.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/border_radius.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/border_radius.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/bottom_app_bar.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/bottom_app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/bottom_sheet.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/buttons.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/buttons.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__init__.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/__init__.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 514 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 0202 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 0202 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 9c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6400 6407 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/arc.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/arc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 2910 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 5e0b 0000  a.........3f^...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 5e0b 0000  a.........<f^...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6504 8303  ..G.d.d...d.e...
 00000070: 5a09 6407 5300 2908 e900 0000 0029 02da  Z.d.S.)......)..
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/canvas.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/canvas.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 4813 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 cd12 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 cd12 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/circle.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/circle.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 1646 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 6e06 0000  a.........3fn...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 6e06 0000  a.........<fn...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6504 8303  ..G.d.d...d.e...
 00000070: 5a09 6407 5300 2908 e900 0000 0029 02da  Z.d.S.)......)..
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/color.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/color.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 1236 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 d404 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 d404 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6504 8303 5a07 6406 5300 2907 e900 0000  e...Z.d.S.).....
 00000070: 0029 02da 0341 6e79 da08 4f70 7469 6f6e  .)...Any..Option
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/fill.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/fill.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 844 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 4c03 0000  a.........3fL...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 4c03 0000  a.........<fL...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6504 8303 5a07 6406 5300 2907 e900 0000  e...Z.d.S.).....
 00000070: 0029 02da 0341 6e79 da08 4f70 7469 6f6e  .)...Any..Option
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/line.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/line.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 1869 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 4d07 0000  a.........3fM...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 4d07 0000  a.........<fM...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6504 8303  ..G.d.d...d.e...
 00000070: 5a09 6407 5300 2908 e900 0000 0029 02da  Z.d.S.)......)..
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/oval.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/oval.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 1891 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 6307 0000  a.........3fc...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 6307 0000  a.........<fc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 4700 6405 6406 8400 6406 6504 8303  ..G.d.d...d.e...
 00000070: 5a09 6407 5300 2908 e900 0000 0029 02da  Z.d.S.)......)..
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/path.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/path.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 3493 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 a50d 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 a50d 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6406 6407 8400 6407 6506 8303 5a0b 6401  d.d...d.e...Z.d.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/points.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/points.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 1813 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 1507 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 1507 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6406 6407 8400 6407 6501 8303  ..G.d.d...d.e...
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/rect.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/rect.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 2345 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 2909 0000  a.........3f)...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 2909 0000  a.........<f)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 4700  ..d.d.l.m.Z...G.
 00000070: 6406 6407 8400 6407 6504 8303 5a0b 6408  d.d...d.e...Z.d.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/shadow.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/shadow.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 1951 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 9f07 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 9f07 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 6507 8303 5a0a 6407 5300 2908 e900 0000  e...Z.d.S.).....
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/shape.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/shape.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 347 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 5b01 0000  a.........3f[...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 5b01 0000  a.........<f[...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 6504 8303 5a05 6405 5300 2906  ..d.e...Z.d.S.).
 00000060: e900 0000 0029 02da 0341 6e79 da08 4f70  .....)...Any..Op
 00000070: 7469 6f6e 616c 2901 da07 436f 6e74 726f  tional)...Contro
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/__pycache__/text.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/__pycache__/text.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 4172 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 4c10 0000  a.........3fL...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 4c10 0000  a.........<fL...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/arc.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/arc.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/canvas.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/circle.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/circle.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/color.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/color.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/fill.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/fill.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/line.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/line.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/oval.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/oval.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/path.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/path.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/points.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/points.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/rect.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/rect.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/shadow.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/canvas/text.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/canvas/text.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/card.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/card.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/bar_chart.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/bar_chart.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 9932 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 cc26 0000  a.........3f.&..
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 cc26 0000  a.........<f.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/bar_chart_group.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/bar_chart_group.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 2044 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 fc07 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 fc07 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 6d08 5a08 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000070: 8400 6406 6507 8303 5a0b 6407 5300 2908  ..d.e...Z.d.S.).
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/bar_chart_rod.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/bar_chart_rod.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 6679 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 171a 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 171a 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/bar_chart_rod_stack_item.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/bar_chart_rod_stack_item.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 1932 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 8c07 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 8c07 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 4700 6405 6406 8400 6406  m.Z...G.d.d...d.
 00000070: 6506 8303 5a0a 6407 5300 2908 e900 0000  e...Z.d.S.).....
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/chart_axis.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/chart_axis.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 2923 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 6b0b 0000  a.........3fk...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 6b0b 0000  a.........<fk...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 6d08 5a08 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000070: 8400 6406 6507 8303 5a0b 6407 5300 2908  ..d.e...Z.d.S.).
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/chart_axis_label.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/chart_axis_label.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 1293 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 0d05 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 0d05 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000060: 8400 6405 6504 8303 5a08 6406 5300 2907  ..d.e...Z.d.S.).
 00000070: e900 0000 0029 02da 0341 6e79 da08 4f70  .....)...Any..Op
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/chart_grid_lines.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/chart_point_line.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 338 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 5201 0000  a.........3fR...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 1e01 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c02 6d03 5a03 6d04 5a04  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6500 6a05 4700 6404 6405 8400 6405  ..e.j.G.d.d...d.
 00000060: 8302 8301 5a06 6401 5300 2906 e900 0000  ....Z.d.S.).....
 00000070: 004e 2901 da05 6669 656c 6429 02da 044c  .N)...field)...L
 00000080: 6973 74da 084f 7074 696f 6e61 6c63 0000  ist..Optionalc..
 00000090: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-000000a0: 0000 4000 0000 736a 0000 0065 005a 0164  ..@...sj...e.Z.d
+000000a0: 0000 4000 0000 7354 0000 0065 005a 0164  ..@...sT...e.Z.d
 000000b0: 005a 0255 0065 0364 0164 028d 015a 0465  .Z.U.e.d.d...Z.e
 000000c0: 0565 0619 0065 0764 033c 0065 0364 0164  .e...e.d.<.e.d.d
 000000d0: 028d 015a 0865 0565 0919 0065 0764 043c  ...Z.e.e...e.d.<
-000000e0: 0065 0364 0164 028d 015a 0a65 0565 0619  .e.d.d...Z.e.e..
-000000f0: 0065 0764 053c 0065 0364 0164 028d 015a  .e.d.<.e.d.d...Z
-00000100: 0b65 0565 0c65 0d19 0019 0065 0764 063c  .e.e.e.....e.d.<
-00000110: 0064 0153 0029 07da 0e43 6861 7274 4772  .d.S.)...ChartGr
-00000120: 6964 4c69 6e65 734e 2901 da07 6465 6661  idLinesN)...defa
-00000130: 756c 74da 0869 6e74 6572 7661 6cda 0563  ult..interval..c
-00000140: 6f6c 6f72 da05 7769 6474 68da 0c64 6173  olor..width..das
-00000150: 685f 7061 7474 6572 6e29 0eda 085f 5f6e  h_pattern)...__n
-00000160: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000170: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00000180: 0200 0000 7207 0000 0072 0400 0000 da05  ....r....r......
-00000190: 666c 6f61 74da 0f5f 5f61 6e6e 6f74 6174  float..__annotat
-000001a0: 696f 6e73 5f5f 7208 0000 00da 0373 7472  ions__r......str
-000001b0: 7209 0000 0072 0a00 0000 7203 0000 00da  r....r....r.....
-000001c0: 0369 6e74 a900 7212 0000 0072 1200 0000  .int..r....r....
-000001d0: fa6a 2f77 6f72 6b73 7061 6365 732f 636f  .j/workspaces/co
-000001e0: 6e74 7269 6266 6c65 742f 666c 6574 636f  ntribflet/fletco
-000001f0: 6e74 7269 622f 7364 6b2f 7079 7468 6f6e  ntrib/sdk/python
-00000200: 2f70 6163 6b61 6765 732f 666c 6574 2d63  /packages/flet-c
-00000210: 6f72 652f 7372 632f 666c 6574 5f63 6f72  ore/src/flet_cor
-00000220: 652f 6368 6172 7473 2f63 6861 7274 5f67  e/charts/chart_g
-00000230: 7269 645f 6c69 6e65 732e 7079 7205 0000  rid_lines.pyr...
-00000240: 0006 0000 0073 0800 0000 0a02 1601 1601  .....s..........
-00000250: 1601 7205 0000 0029 07da 0b64 6174 6163  ..r....)...datac
-00000260: 6c61 7373 6573 7202 0000 00da 0674 7970  lassesr......typ
-00000270: 696e 6772 0300 0000 7204 0000 00da 0964  ingr....r......d
-00000280: 6174 6163 6c61 7373 7205 0000 0072 1200  ataclassr....r..
-00000290: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-000002a0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000002b0: 0800 0000 0801 0c01 1003 0401            ............
+000000e0: 0065 0364 0164 028d 015a 0a65 0565 0b65  .e.d.d...Z.e.e.e
+000000f0: 0c19 0019 0065 0764 053c 0064 0153 0029  .....e.d.<.d.S.)
+00000100: 06da 0e43 6861 7274 506f 696e 744c 696e  ...ChartPointLin
+00000110: 654e 2901 da07 6465 6661 756c 74da 0563  eN)...default..c
+00000120: 6f6c 6f72 da05 7769 6474 68da 0c64 6173  olor..width..das
+00000130: 685f 7061 7474 6572 6e29 0dda 085f 5f6e  h_pattern)...__n
+00000140: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000150: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+00000160: 0200 0000 7207 0000 0072 0400 0000 da03  ....r....r......
+00000170: 7374 72da 0f5f 5f61 6e6e 6f74 6174 696f  str..__annotatio
+00000180: 6e73 5f5f 7208 0000 00da 0566 6c6f 6174  ns__r......float
+00000190: 7209 0000 0072 0300 0000 da03 696e 74a9  r....r......int.
+000001a0: 0072 1100 0000 7211 0000 00fa 6a2f 776f  .r....r.....j/wo
+000001b0: 726b 7370 6163 6573 2f63 6f6e 7472 6962  rkspaces/contrib
+000001c0: 666c 6574 2f66 6c65 7463 6f6e 7472 6962  flet/fletcontrib
+000001d0: 2f73 646b 2f70 7974 686f 6e2f 7061 636b  /sdk/python/pack
+000001e0: 6167 6573 2f66 6c65 742d 636f 7265 2f73  ages/flet-core/s
+000001f0: 7263 2f66 6c65 745f 636f 7265 2f63 6861  rc/flet_core/cha
+00000200: 7274 732f 6368 6172 745f 706f 696e 745f  rts/chart_point_
+00000210: 6c69 6e65 2e70 7972 0500 0000 0600 0000  line.pyr........
+00000220: 7306 0000 000a 0216 0116 0172 0500 0000  s..........r....
+00000230: 2907 da0b 6461 7461 636c 6173 7365 7372  )...dataclassesr
+00000240: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
+00000250: 0072 0400 0000 da09 6461 7461 636c 6173  .r......dataclas
+00000260: 7372 0500 0000 7211 0000 0072 1100 0000  sr....r....r....
+00000270: 7211 0000 0072 1200 0000 da08 3c6d 6f64  r....r......<mod
+00000280: 756c 653e 0100 0000 7308 0000 0008 010c  ule>....s.......
+00000290: 0110 0304 01                             .....
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/chart_point_shape.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/chart_point_shape.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 1006 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 ee03 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 ee03 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 5a00 6400 6402 6c00 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c02 6d03 5a03 0100 6500  ..d.d.l.m.Z...e.
 00000050: 6a04 4700 6404 6405 8400 6405 8302 8301  j.G.d.d...d.....
 00000060: 5a05 6500 6a04 4700 6406 6407 8400 6407  Z.e.j.G.d.d...d.
 00000070: 6505 8303 8301 5a06 6500 6a04 4700 6408  e.....Z.e.j.G.d.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/line_chart.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/line_chart.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 11305 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 292c 0000  a.........3f),..
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 292c 0000  a.........<f),..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 da00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/line_chart_data.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/line_chart_data.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 9357 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 8d24 0000  a.........3f.$..
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 8d24 0000  a.........<f.$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6400 6402 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6400 6406 6c0e  m.Z.m.Z...d.d.l.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/line_chart_data_point.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/line_chart_data_point.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 5338 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 da14 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 da14 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/pie_chart.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/pie_chart.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 5965 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 4d17 0000  a.........3fM...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 4d17 0000  a.........<fM...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/__pycache__/pie_chart_section.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/__pycache__/pie_chart_section.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 3807 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 df0e 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 df0e 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 4700 6406 6407 8400 6407 6506 8303  ..G.d.d...d.e...
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/bar_chart.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/bar_chart_group.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/bar_chart_group.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/bar_chart_rod.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/bar_chart_rod.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/bar_chart_rod_stack_item.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/bar_chart_rod_stack_item.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/chart_axis.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/chart_axis.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/chart_axis_label.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/chart_axis_label.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/chart_point_shape.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/chart_point_shape.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/line_chart.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/line_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/line_chart_data.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/line_chart_data.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/line_chart_data_point.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/line_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/pie_chart.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/charts/pie_chart_section.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/charts/pie_chart_section.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/checkbox.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/checkbox.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/chip.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/chip.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/circle_avatar.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/circle_avatar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/client_storage.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/client_storage.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/colors.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/colors.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/column.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/column.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/connection.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/connection.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/constrained_control.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/constrained_control.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/container.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/container.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/control.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/control.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_action_sheet.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_action_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_action_sheet_action.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_action_sheet_action.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_activity_indicator.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_activity_indicator.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_alert_dialog.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_app_bar.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_bottom_sheet.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_checkbox.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_checkbox.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_colors.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_colors.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_context_menu.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_context_menu.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_context_menu_action.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_context_menu_action.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_date_picker.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_date_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_dialog_action.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_dialog_action.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_filled_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_filled_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_icons.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_icons.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_list_tile.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_list_tile.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_navigation_bar.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_picker.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_radio.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_radio.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_segmented_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_segmented_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_slider.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_slider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_sliding_segmented_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_sliding_segmented_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_switch.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_switch.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_textfield.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_textfield.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/cupertino_timer_picker.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/cupertino_timer_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/datatable.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/datatable.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/date_picker.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/date_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/dismissible.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/dismissible.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/divider.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/divider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/drag_target.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/drag_target.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/draggable.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/draggable.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/dropdown.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/dropdown.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/elevated_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/elevated_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/embed_json_encoder.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/embed_json_encoder.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/event_handler.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/event_handler.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/expansion_panel.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/expansion_panel.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/expansion_tile.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/expansion_tile.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/file_picker.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/file_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/filled_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/filled_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/filled_tonal_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/filled_tonal_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/flet_app.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/flet_app.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/floating_action_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/floating_action_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/form_field_control.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/form_field_control.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/gesture_detector.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/gesture_detector.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/gradients.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/gradients.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/grid_view.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/grid_view.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/haptic_feedback.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/haptic_feedback.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/icon.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/icon.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/icon_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/icon_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/icons.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/icons.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/image.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/image.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/list_tile.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/list_tile.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/list_view.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/list_view.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/local_connection.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/local_connection.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/lottie.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/lottie.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/margin.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/margin.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/markdown.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/markdown.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/matplotlib_chart.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/matplotlib_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/menu_bar.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/menu_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/menu_item_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/menu_item_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/merge_semantics.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/merge_semantics.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/navigation_bar.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/navigation_drawer.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/navigation_drawer.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/navigation_rail.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/navigation_rail.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/outlined_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/outlined_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/padding.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/padding.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/page.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/page.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/pagelet.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/pagelet.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/painting.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/painting.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/plotly_chart.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/popup_menu_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/popup_menu_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/progress_bar.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/progress_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/progress_ring.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/progress_ring.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/protocol.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/protocol.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/pubsub/__pycache__/pubsub_client.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/pubsub/__pycache__/pubsub_client.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 3393 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 410d 0000  a.........3fA...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 410d 0000  a.........<fA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6401 6c04 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c05 6d06 5a06 0100 6400 6404 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6500 a009 6504 6a0a a101  m.Z...e...e.j...
 00000070: 5a0b 4700 6405 6406 8400 6406 8302 5a0c  Z.G.d.d...d...Z.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/pubsub/__pycache__/pubsub_hub.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/pubsub/__pycache__/pubsub_hub.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 5873 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 f116 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 f116 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 0100 6400 6401 6c0d 5a0d 6400  m.Z...d.d.l.Z.d.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/pubsub/pubsub_client.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/pubsub/pubsub_client.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/pubsub/pubsub_hub.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/pubsub/pubsub_hub.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/querystring.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/querystring.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/radio.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/radio.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/radio_group.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/radio_group.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/range_slider.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/range_slider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/responsive_row.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/responsive_row.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/rive.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/rive.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/row.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/row.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/safe_area.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/safe_area.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/scrollable_control.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/scrollable_control.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/search_bar.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/search_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/segmented_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/segmented_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/selection_area.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/selection_area.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/semantics.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/semantics.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/semantics_service.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/semantics_service.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/session_storage.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/session_storage.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/shader_mask.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/shader_mask.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/shadow.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/shake_detector.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/shake_detector.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/slider.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/slider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/snack_bar.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/snack_bar.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/stack.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/stack.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/submenu_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/submenu_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/switch.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/switch.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/tabs.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/tabs.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/template_route.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/template_route.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/text.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/text.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/text_button.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/text_button.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/text_span.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/text_span.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/text_style.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/text_style.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/textfield.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/textfield.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/theme.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/theme.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/time_picker.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/time_picker.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/tooltip.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/tooltip.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/transform.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/transform.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/transparent_pointer.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/transparent_pointer.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/two_dimensional_scrollables.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/two_dimensional_scrollables.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     -----
 
     Online docs: https://flet.dev/docs/controls/two_dimensional_scrollables_control
     """
 
     def __init__(
         self,
+        current_action: Optional[str]= "",
+        current_cell: Optional[str] = "",
         cell_content: Optional[str] = "",
-        current_sheet_index: Optional[int] = 1,
-
-
+        on_change=None,
 
         
         
         #
         # ConstrainedControl
         #
         ref: Optional[Ref] = None,
@@ -92,34 +92,53 @@
             tooltip=tooltip,
             visible=visible,
             disabled=disabled,
             data=data,
             rtl=rtl,
         )
 
+        
+        self.current_action = current_action
+        self.current_cell = current_cell 
         self.cell_content = cell_content
-        self.current_sheet_index = current_sheet_index
+        self.on_change = on_change
         
     def _get_control_name(self):
         return "two_dimensional_scrollables"
 
     # Implement properties and setters    
+
+    
+    @property
+    def current_action(self):
+        return self._get_attr("currentAction")
+
+    @current_action.setter
+    def current_action(self, value):
+        self._set_attr("currentAction", value)
+    
+    @property
+    def current_cell(self):
+        return self._get_attr("currentCell")
+
+    @current_cell.setter
+    def current_cell(self, value):
+        self._set_attr("currentCell", value)
+
     @property
     def cell_content(self):
         return self._get_attr("cellContent")
 
     @cell_content.setter
     def cell_content(self, value):
         self._set_attr("cellContent", value)
     
+    # on_change
     @property
-    def current_sheet_index(self):
-        return self._get_attr("currentSheetIndex")
+    def on_change(self):
+        return self._get_event_handler("change")
 
-    @cell_content.setter
-    def current_sheet_index(self, value):
-        self._set_attr("currentSheetIndex", value)
-
-  
-    
+    @on_change.setter
+    def on_change(self, handler):
+        self._add_event_handler("change", handler)
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/types.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/types.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/__init__.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 311 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 3701 0000  a.........3f7...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 3701 0000  a.........<f7...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6407 5300 2908  d.l.m.Z...d.S.).
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/classproperty.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/classproperty.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 271 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 0f01 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 0f01 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 6d04 5a04 0100 6501 6402 8301 5a05 4700  m.Z...e.d...Z.G.
 00000050: 6403 6404 8400 6404 8302 5a06 6405 5300  d.d...d...Z.d.S.
 00000060: 2906 e900 0000 0029 04da 0754 7970 6556  )......)...TypeV
 00000070: 6172 da04 5479 7065 da03 416e 79da 0843  ar..Type..Any..C
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/concurrency_utils.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/concurrency_utils.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 243 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 f300 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 f300 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 8400 5a02 6404 6405 8400 5a03 6401  d...Z.d.d...Z.d.
 00000050: 5300 2906 e900 0000 004e 6300 0000 0000  S.)......Nc.....
 00000060: 0000 0000 0000 0000 0000 0008 0000 0043  ...............C
 00000070: 0000 0073 3200 0000 7a18 7400 a001 a100  ...s2...z.t.....
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/deprecated.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/deprecated.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 835 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 4303 0000  a.........3fC...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 4303 0000  a.........<fC...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 8400 5a02 6401 5300 2904 e900 0000  d...Z.d.S.).....
 00000050: 004e 6303 0000 0000 0000 0000 0000 0004  .Nc.............
 00000060: 0000 0003 0000 0003 0000 0073 1400 0000  ...........s....
 00000070: 8700 8701 8702 6603 6401 6402 8408 7d03  ......f.d.d...}.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/slugify.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/slugify.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 465 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 d101 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 d101 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6502  d.l.Z.d.d.l.Z.e.
 00000040: 6502 6402 9c02 6403 6404 8404 5a03 6401  e.d...d.d...Z.d.
 00000050: 5300 2905 e900 0000 004e 2902 da05 7661  S.)......N)...va
 00000060: 6c75 65da 0672 6574 7572 6e63 0100 0000  lue..returnc....
 00000070: 0000 0000 0000 0000 0100 0000 0500 0000  ................
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/strings.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/strings.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 178 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 b200 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 b200 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 8400 5a02 6401 5300 2904 e900 0000  d...Z.d.S.).....
 00000050: 004e 6301 0000 0000 0000 0000 0000 0001  .Nc.............
 00000060: 0000 0005 0000 0003 0000 0073 2800 0000  ...........s(...
 00000070: 7400 6a01 7400 6a02 1700 8900 6401 a003  t.j.t.j.....d...
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/utils/__pycache__/vector.cpython-39.pyc` & `flet_contrib_core-2024.5.9.2200/src/flet_core/utils/__pycache__/vector.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 3207 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 870c 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 870c 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 6501 8303 5a02 6401 5300 2904 e900 0000  e...Z.d.S.).....
 00000050: 004e 6300 0000 0000 0000 0000 0000 0000  .Nc.............
 00000060: 0000 0003 0000 0040 0000 0073 d200 0000  .......@...s....
 00000070: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
```

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/utils/deprecated.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/utils/vector.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/utils/vector.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/vertical_divider.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/vertical_divider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/video.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/video.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/view.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/view.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/webview.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/webview.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/src/flet_core/window_drag_area.py` & `flet_contrib_core-2024.5.9.2200/src/flet_core/window_drag_area.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_core-2024.5.3.1625/PKG-INFO` & `flet_contrib_core-2024.5.9.2200/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-contrib-core
-Version: 2024.5.3.1625
+Version: 2024.5.9.2200
 Summary: Flet core library
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

