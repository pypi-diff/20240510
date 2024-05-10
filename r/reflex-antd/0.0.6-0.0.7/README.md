# Comparing `tmp/reflex_antd-0.0.6.tar.gz` & `tmp/reflex_antd-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_antd-0.0.6.tar", last modified: Wed May  8 11:41:22 2024, max compression
+gzip compressed data, was "reflex_antd-0.0.7.tar", last modified: Fri May 10 13:51:16 2024, max compression
```

## Comparing `reflex_antd-0.0.6.tar` & `reflex_antd-0.0.7.tar`

### file list

```diff
@@ -1,158 +1,159 @@
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:41:22.811942 reflex_antd-0.0.6/
--rwxrwxrwx   0 see       (1000) see       (1000)    11357 2024-03-25 11:08:46.000000 reflex_antd-0.0.6/LICENSE
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-05-08 11:41:22.804683 reflex_antd-0.0.6/PKG-INFO
--rwxrwxrwx   0 see       (1000) see       (1000)      336 2024-04-19 06:20:21.000000 reflex_antd-0.0.6/README.md
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:41:19.050568 reflex_antd-0.0.6/custom_components/
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:41:19.325560 reflex_antd-0.0.6/custom_components/reflex_antd/
--rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/__init__.py
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:41:22.768139 reflex_antd-0.0.6/custom_components/reflex_antd/antd/
--rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/__init__.py
--rwxrwxrwx   0 see       (1000) see       (1000)      679 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/affix.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3101 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/affix.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/alert.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5909 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/alert.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1028 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/anchor.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3655 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/anchor.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1549 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/auto_complete.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4382 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/auto_complete.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1025 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/avatar.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5934 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/avatar.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      825 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/badge.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6130 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/badge.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     3547 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/base.py
--rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/breadcrumb.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5451 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/breadcrumb.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      922 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/button.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3644 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/button.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1318 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/calendar.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3605 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/calendar.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1366 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/card.py
--rwxrwxrwx   0 see       (1000) see       (1000)     8612 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/card.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      814 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/carousel.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3386 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/carousel.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2282 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/cascader.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5957 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/cascader.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1269 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/checkbox.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6026 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/checkbox.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      935 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/collapse.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3580 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/collapse.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1439 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/color_picker.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4599 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/color_picker.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     4993 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/date_picker.py
--rwxrwxrwx   0 see       (1000) see       (1000)    17831 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/date_picker.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      709 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/descriptions.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3597 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/descriptions.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      506 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/divider.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3200 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/divider.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1398 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/drawer.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4497 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/drawer.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1518 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/dropdown.py
--rwxrwxrwx   0 see       (1000) see       (1000)     7254 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/dropdown.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      340 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/empty.py
--rwxrwxrwx   0 see       (1000) see       (1000)     2839 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/empty.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      494 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/flex.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3049 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/flex.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1568 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/float_button.py
--rwxrwxrwx   0 see       (1000) see       (1000)     9924 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/float_button.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     5458 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/form.py
--rwxrwxrwx   0 see       (1000) see       (1000)    14023 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/form.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      907 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/grid.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5943 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/grid.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2234 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/icon.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4456 2024-04-17 06:35:31.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/icon.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      973 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/image.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5829 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/image.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1934 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/input.py
--rwxrwxrwx   0 see       (1000) see       (1000)    16141 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/input.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1565 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/input_number.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4745 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/input_number.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1645 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/layout.py
--rwxrwxrwx   0 see       (1000) see       (1000)    18024 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/layout.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1114 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/list.py
--rwxrwxrwx   0 see       (1000) see       (1000)     8602 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/list.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1383 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/mentions.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4545 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/mentions.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2022 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/menu.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4675 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/menu.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     4551 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/message.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3176 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/message.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     4041 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/modal.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4678 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/modal.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2011 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/notification.py
--rwxrwxrwx   0 see       (1000) see       (1000)     1169 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/pagination.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3794 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/pagination.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      972 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/popconfirm.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3709 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/popconfirm.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      473 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/popover.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4413 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/popover.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1039 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/progress.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4279 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/progress.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      941 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/qrcode.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3635 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/qrcode.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1221 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/radio.py
--rwxrwxrwx   0 see       (1000) see       (1000)     8759 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/radio.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/rate.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3600 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/rate.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      545 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/result.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3263 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/result.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      850 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/segmented.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3432 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/segmented.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2862 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/select.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6924 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/select.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      575 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/skeleton.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3161 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/skeleton.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1272 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/slider.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4053 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/slider.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      755 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/space.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6085 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/space.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      588 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/spin.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3247 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/spin.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1213 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/statistic.py
--rwxrwxrwx   0 see       (1000) see       (1000)     9147 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/statistic.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1036 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/steps.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3976 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/steps.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1042 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/switch.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3595 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/switch.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2690 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/table.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5782 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/table.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2108 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tabs.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5235 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tabs.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1063 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tag.py
--rwxrwxrwx   0 see       (1000) see       (1000)     5717 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tag.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      566 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/timeline.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3170 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/timeline.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1352 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tooltip.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4395 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tooltip.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1237 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tour.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4192 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tour.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1997 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/transfer.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3910 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/transfer.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2609 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6180 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     2869 2024-05-08 11:29:15.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree_select.py
--rwxrwxrwx   0 see       (1000) see       (1000)     6424 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree_select.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1763 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/typography.py
--rwxrwxrwx   0 see       (1000) see       (1000)    15437 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/typography.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1584 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/upload.py
--rwxrwxrwx   0 see       (1000) see       (1000)     4500 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/upload.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-05-08 11:29:17.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/watermark.py
--rwxrwxrwx   0 see       (1000) see       (1000)     3397 2024-04-17 06:35:32.000000 reflex_antd-0.0.6/custom_components/reflex_antd/antd/watermark.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)    25316 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/base.py
--rwxrwxrwx   0 see       (1000) see       (1000)    11261 2024-04-17 06:35:23.000000 reflex_antd-0.0.6/custom_components/reflex_antd/base.pyi
--rwxrwxrwx   0 see       (1000) see       (1000)     1919 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/constant.py
--rwxrwxrwx   0 see       (1000) see       (1000)      996 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/display.py
--rwxrwxrwx   0 see       (1000) see       (1000)      899 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/entry.py
--rwxrwxrwx   0 see       (1000) see       (1000)      515 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/feedback.py
--rwxrwxrwx   0 see       (1000) see       (1000)      289 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/general.py
--rwxrwxrwx   0 see       (1000) see       (1000)      152 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/helper.py
--rwxrwxrwx   0 see       (1000) see       (1000)      243 2024-05-08 11:29:14.000000 reflex_antd-0.0.6/custom_components/reflex_antd/layout.py
--rwxrwxrwx   0 see       (1000) see       (1000)      288 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/navigation.py
--rwxrwxrwx   0 see       (1000) see       (1000)     1654 2024-05-08 11:29:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd/util.py
-drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-08 11:41:22.795683 reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/
--rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-05-08 11:41:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/PKG-INFO
--rwxrwxrwx   0 see       (1000) see       (1000)     6855 2024-05-08 11:41:19.000000 reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/SOURCES.txt
--rwxrwxrwx   0 see       (1000) see       (1000)        1 2024-05-08 11:41:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/dependency_links.txt
--rwxrwxrwx   0 see       (1000) see       (1000)       33 2024-05-08 11:41:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/requires.txt
--rwxrwxrwx   0 see       (1000) see       (1000)       12 2024-05-08 11:41:18.000000 reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/top_level.txt
--rwxrwxrwx   0 see       (1000) see       (1000)      794 2024-05-08 11:40:05.000000 reflex_antd-0.0.6/pyproject.toml
--rwxrwxrwx   0 see       (1000) see       (1000)       38 2024-05-08 11:41:22.812478 reflex_antd-0.0.6/setup.cfg
+drwxr-xr-x   0 see       (1000) see       (1000)        0 2024-05-10 13:51:15.993543 reflex_antd-0.0.7/
+-rw-r--r--   0 see       (1000) see       (1000)    11558 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/LICENSE
+-rw-r--r--   0 see       (1000) see       (1000)      977 2024-05-10 13:51:15.993543 reflex_antd-0.0.7/PKG-INFO
+-rw-r--r--   0 see       (1000) see       (1000)      362 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/README.md
+drwxr-xr-x   0 see       (1000) see       (1000)        0 2024-05-10 13:51:15.953543 reflex_antd-0.0.7/custom_components/
+drwxr-xr-x   0 see       (1000) see       (1000)        0 2024-05-10 13:51:15.953543 reflex_antd-0.0.7/custom_components/reflex_antd/
+-rw-r--r--   0 see       (1000) see       (1000)        0 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/__init__.py
+drwxr-xr-x   0 see       (1000) see       (1000)        0 2024-05-10 13:51:15.993543 reflex_antd-0.0.7/custom_components/reflex_antd/antd/
+-rw-r--r--   0 see       (1000) see       (1000)        0 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/__init__.py
+-rw-r--r--   0 see       (1000) see       (1000)      709 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/affix.py
+-rw-r--r--   0 see       (1000) see       (1000)     3101 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/affix.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1015 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/alert.py
+-rw-r--r--   0 see       (1000) see       (1000)     5909 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/alert.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1063 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/anchor.py
+-rw-r--r--   0 see       (1000) see       (1000)     3655 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/anchor.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1595 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/auto_complete.py
+-rw-r--r--   0 see       (1000) see       (1000)     4382 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/auto_complete.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1065 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/avatar.py
+-rw-r--r--   0 see       (1000) see       (1000)     5934 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/avatar.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      856 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/badge.py
+-rw-r--r--   0 see       (1000) see       (1000)     6130 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/badge.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     3811 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/base.py
+-rw-r--r--   0 see       (1000) see       (1000)      769 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/breadcrumb.py
+-rw-r--r--   0 see       (1000) see       (1000)     5451 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/breadcrumb.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      957 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/button.py
+-rw-r--r--   0 see       (1000) see       (1000)     3644 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/button.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1364 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/calendar.py
+-rw-r--r--   0 see       (1000) see       (1000)     3605 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/calendar.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1418 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/card.py
+-rw-r--r--   0 see       (1000) see       (1000)     8612 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/card.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      844 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/carousel.py
+-rw-r--r--   0 see       (1000) see       (1000)     3386 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/carousel.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     2342 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/cascader.py
+-rw-r--r--   0 see       (1000) see       (1000)     5957 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/cascader.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1316 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/checkbox.py
+-rw-r--r--   0 see       (1000) see       (1000)     6026 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/checkbox.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      966 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/collapse.py
+-rw-r--r--   0 see       (1000) see       (1000)     3580 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/collapse.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1483 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/color_picker.py
+-rw-r--r--   0 see       (1000) see       (1000)     4599 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/color_picker.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     5135 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/date_picker.py
+-rw-r--r--   0 see       (1000) see       (1000)    17831 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/date_picker.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      733 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/descriptions.py
+-rw-r--r--   0 see       (1000) see       (1000)     3597 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/descriptions.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      509 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/divider.py
+-rw-r--r--   0 see       (1000) see       (1000)     3200 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/divider.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1442 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/drawer.py
+-rw-r--r--   0 see       (1000) see       (1000)     4497 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/drawer.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1572 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/dropdown.py
+-rw-r--r--   0 see       (1000) see       (1000)     7254 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/dropdown.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      356 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/empty.py
+-rw-r--r--   0 see       (1000) see       (1000)     2839 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/empty.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      499 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/flex.py
+-rw-r--r--   0 see       (1000) see       (1000)     3049 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/flex.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1624 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/float_button.py
+-rw-r--r--   0 see       (1000) see       (1000)     9924 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/float_button.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     6100 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/form.py
+-rw-r--r--   0 see       (1000) see       (1000)    14023 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/form.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      945 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/grid.py
+-rw-r--r--   0 see       (1000) see       (1000)     5943 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/grid.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      491 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/helper.py
+-rw-r--r--   0 see       (1000) see       (1000)     2315 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/icon.py
+-rw-r--r--   0 see       (1000) see       (1000)     4456 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/icon.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1011 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/image.py
+-rw-r--r--   0 see       (1000) see       (1000)     5829 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/image.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     2006 2024-05-08 14:18:11.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/input.py
+-rw-r--r--   0 see       (1000) see       (1000)    16141 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/input.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1612 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/input_number.py
+-rw-r--r--   0 see       (1000) see       (1000)     4745 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/input_number.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1696 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/layout.py
+-rw-r--r--   0 see       (1000) see       (1000)    18024 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/layout.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1158 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/list.py
+-rw-r--r--   0 see       (1000) see       (1000)     8602 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/list.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1422 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/mentions.py
+-rw-r--r--   0 see       (1000) see       (1000)     4545 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/mentions.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     2050 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/menu.py
+-rw-r--r--   0 see       (1000) see       (1000)     4675 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/menu.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     4741 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/message.py
+-rw-r--r--   0 see       (1000) see       (1000)     3176 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/message.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     4559 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/modal.py
+-rw-r--r--   0 see       (1000) see       (1000)     4678 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/modal.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     2077 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/notification.py
+-rw-r--r--   0 see       (1000) see       (1000)     1208 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/pagination.py
+-rw-r--r--   0 see       (1000) see       (1000)     3794 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/pagination.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1005 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/popconfirm.py
+-rw-r--r--   0 see       (1000) see       (1000)     3709 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/popconfirm.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      493 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/popover.py
+-rw-r--r--   0 see       (1000) see       (1000)     4413 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/popover.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1074 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/progress.py
+-rw-r--r--   0 see       (1000) see       (1000)     4279 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/progress.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      975 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/qrcode.py
+-rw-r--r--   0 see       (1000) see       (1000)     3635 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/qrcode.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1267 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/radio.py
+-rw-r--r--   0 see       (1000) see       (1000)     8759 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/radio.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1010 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/rate.py
+-rw-r--r--   0 see       (1000) see       (1000)     3600 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/rate.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      568 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/result.py
+-rw-r--r--   0 see       (1000) see       (1000)     3263 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/result.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      880 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/segmented.py
+-rw-r--r--   0 see       (1000) see       (1000)     3432 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/segmented.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     2935 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/select.py
+-rw-r--r--   0 see       (1000) see       (1000)     6924 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/select.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      598 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/skeleton.py
+-rw-r--r--   0 see       (1000) see       (1000)     3161 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/skeleton.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1314 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/slider.py
+-rw-r--r--   0 see       (1000) see       (1000)     4053 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/slider.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      787 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/space.py
+-rw-r--r--   0 see       (1000) see       (1000)     6085 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/space.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      612 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/spin.py
+-rw-r--r--   0 see       (1000) see       (1000)     3247 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/spin.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1258 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/statistic.py
+-rw-r--r--   0 see       (1000) see       (1000)     9147 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/statistic.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1074 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/steps.py
+-rw-r--r--   0 see       (1000) see       (1000)     3976 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/steps.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1075 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/switch.py
+-rw-r--r--   0 see       (1000) see       (1000)     3595 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/switch.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     2753 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/table.py
+-rw-r--r--   0 see       (1000) see       (1000)     5782 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/table.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     2169 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tabs.py
+-rw-r--r--   0 see       (1000) see       (1000)     5235 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tabs.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1105 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tag.py
+-rw-r--r--   0 see       (1000) see       (1000)     5717 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tag.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      588 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/timeline.py
+-rw-r--r--   0 see       (1000) see       (1000)     3170 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/timeline.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1394 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tooltip.py
+-rw-r--r--   0 see       (1000) see       (1000)     4395 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tooltip.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1277 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tour.py
+-rw-r--r--   0 see       (1000) see       (1000)     4192 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tour.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     2053 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/transfer.py
+-rw-r--r--   0 see       (1000) see       (1000)     3910 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/transfer.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     2679 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tree.py
+-rw-r--r--   0 see       (1000) see       (1000)     6180 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tree.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     2941 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tree_select.py
+-rw-r--r--   0 see       (1000) see       (1000)     6424 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/tree_select.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1824 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/typography.py
+-rw-r--r--   0 see       (1000) see       (1000)    15437 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/typography.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1631 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/upload.py
+-rw-r--r--   0 see       (1000) see       (1000)     4500 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/upload.pyi
+-rw-r--r--   0 see       (1000) see       (1000)      766 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/watermark.py
+-rw-r--r--   0 see       (1000) see       (1000)     3397 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/antd/watermark.pyi
+-rw-r--r--   0 see       (1000) see       (1000)    26524 2024-05-10 13:22:20.000000 reflex_antd-0.0.7/custom_components/reflex_antd/base.py
+-rw-r--r--   0 see       (1000) see       (1000)    11261 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/base.pyi
+-rw-r--r--   0 see       (1000) see       (1000)     1967 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/constant.py
+-rw-r--r--   0 see       (1000) see       (1000)     1018 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/display.py
+-rw-r--r--   0 see       (1000) see       (1000)      918 2024-05-08 14:18:11.000000 reflex_antd-0.0.7/custom_components/reflex_antd/entry.py
+-rw-r--r--   0 see       (1000) see       (1000)      526 2024-05-08 14:18:11.000000 reflex_antd-0.0.7/custom_components/reflex_antd/feedback.py
+-rw-r--r--   0 see       (1000) see       (1000)      295 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/general.py
+-rw-r--r--   0 see       (1000) see       (1000)      153 2024-05-08 14:18:11.000000 reflex_antd-0.0.7/custom_components/reflex_antd/helper.py
+-rw-r--r--   0 see       (1000) see       (1000)      248 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/layout.py
+-rw-r--r--   0 see       (1000) see       (1000)      295 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/navigation.py
+-rw-r--r--   0 see       (1000) see       (1000)     1715 2024-04-26 13:27:12.000000 reflex_antd-0.0.7/custom_components/reflex_antd/util.py
+drwxr-xr-x   0 see       (1000) see       (1000)        0 2024-05-10 13:51:15.993543 reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/
+-rw-r--r--   0 see       (1000) see       (1000)      977 2024-05-10 13:51:15.000000 reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/PKG-INFO
+-rw-r--r--   0 see       (1000) see       (1000)     6900 2024-05-10 13:51:15.000000 reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/SOURCES.txt
+-rw-r--r--   0 see       (1000) see       (1000)        1 2024-05-10 13:51:15.000000 reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/dependency_links.txt
+-rw-r--r--   0 see       (1000) see       (1000)       33 2024-05-10 13:51:15.000000 reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/requires.txt
+-rw-r--r--   0 see       (1000) see       (1000)       12 2024-05-10 13:51:15.000000 reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/top_level.txt
+-rw-r--r--   0 see       (1000) see       (1000)      833 2024-05-10 13:40:49.000000 reflex_antd-0.0.7/pyproject.toml
+-rw-r--r--   0 see       (1000) see       (1000)       38 2024-05-10 13:51:15.993543 reflex_antd-0.0.7/setup.cfg
```

### Comparing `reflex_antd-0.0.6/LICENSE` & `reflex_antd-0.0.7/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `reflex_antd-0.0.6/PKG-INFO` & `reflex_antd-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-antd
-Version: 0.0.6
+Version: 0.0.7
 Summary: Reflex custom component antd
 Author-email: seewind <seewindcn@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: source, https://github.com/seewindcn/reflex-antd
 Keywords: reflex,reflex-custom-components
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/affix.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/affix.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import OrientationType, DirectionType
-
-
-class Affix(AntdComponent):
-    tag = 'Affix'
-
-    offset_bottom: Optional[Var[int]]
-    offset_top: Optional[Var[int]]
-    target: Optional[Var[JsValue]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda affixed: [affixed],
-        })
-        return _triggers
-
-
-affix = Affix.create
-
-
-
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import OrientationType, DirectionType
+
+
+class Affix(AntdComponent):
+    tag = 'Affix'
+
+    offset_bottom: Optional[Var[int]]
+    offset_top: Optional[Var[int]]
+    target: Optional[Var[JsValue]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda affixed: [affixed],
+        })
+        return _triggers
+
+
+affix = Affix.create
+
+
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/affix.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/affix.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/alert.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/alert.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType
-
-
-class Alert(AntdComponent):
-    tag = 'Alert'
-
-    action: Optional[Var[ReactNode]]
-    banner: Optional[Var[bool]]
-    closable: Optional[Var[Union[bool, dict]]]
-    description: Optional[ReactNode]
-    icon: Optional[ReactNode]
-    message: Optional[ReactNode]
-    show_icon: Optional[bool]
-    type: Optional[StatusType]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_close": lambda event: [],
-            "after_close": lambda: [],
-        })
-        return _triggers
-
-
-class AlertErrorBoundary(AntdComponent):
-    tag = 'Alert.ErrorBoundary'
-
-    description: Optional[ReactNode]
-    message: Optional[ReactNode]
-
-
-alert = Alert.create
-alert_error_boundary = AlertErrorBoundary.create
+from typing import Optional, Union, Dict, Any, List
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType
+
+
+class Alert(AntdComponent):
+    tag = 'Alert'
+
+    action: Optional[Var[ReactNode]]
+    banner: Optional[Var[bool]]
+    closable: Optional[Var[Union[bool, dict]]]
+    description: Optional[ReactNode]
+    icon: Optional[ReactNode]
+    message: Optional[ReactNode]
+    show_icon: Optional[bool]
+    type: Optional[StatusType]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_close": lambda event: [],
+            "after_close": lambda: [],
+        })
+        return _triggers
+
+
+class AlertErrorBoundary(AntdComponent):
+    tag = 'Alert.ErrorBoundary'
+
+    description: Optional[ReactNode]
+    message: Optional[ReactNode]
+
+
+alert = Alert.create
+alert_error_boundary = AlertErrorBoundary.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/alert.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/alert.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/anchor.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/rate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsNode
-from ..constant import OrientationType, DirectionType
-
-
-class Anchor(AntdComponent):
-    tag = 'Anchor'
-
-    affix: Optional[Var[bool]]
-    bounds: Optional[Var[int]]
-    get_container: Optional[Var[JsNode]]
-    get_current_anchor: Optional[Var[JsNode]]
-    offset_top: Optional[Var[int]]
-    show_ink_in_fixed: Optional[Var[bool]]
-    target_offset: Optional[Var[int]]
-    items: Optional[Var[Union[List, ContainVar]]]
-    direction: Optional[Var[DirectionType]]
-    replace: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda link: [link],
-            EventTriggers.ON_CLICK: lambda ev, link: [ev, link],
-        })
-        return _triggers
-
-
-anchor = Anchor.create
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import StatusType, SizeType, RadioStyleType, RadioType
+
+
+class Rate(AntdComponent):
+    tag = 'Rate'
+
+    allow_clear: Optional[Var[bool]]
+    allow_half: Optional[Var[bool]]
+    auto_focus: Optional[Var[bool]]
+    character: Optional[Var[Union[Component, JsValue]]]
+    count: Optional[Var[int]]
+    default_value: Optional[Var[int]]
+    disabled: Optional[Var[bool]]
+    tooltips: Optional[Var[List[str]]]
+    value: Optional[Var[int]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda v: [v],
+            "on_hover_change": lambda v: [v],
+            EventTriggers.ON_KEY_DOWN: lambda e: [e],
+        })
+        return _triggers
+
+
+rate = Rate.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/anchor.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/anchor.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/auto_complete.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/dropdown.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,54 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import VariantType, SizeType
-
-
-class AutoComplete(AntdComponent):
-    tag = "AutoComplete"
-
-    allow_clear: Optional[Var[bool]]
-    auto_focus: Optional[Var[bool]]
-    backfill: Optional[Var[bool]]
-    default_active_first_option: Optional[Var[bool]]
-    default_open: Optional[Var[bool]]
-    default_value: Optional[Var[str]]
-    disabled: Optional[Var[bool]]
-    popup_class_name: Optional[Var[str]]
-    dropdown_match_select_width: Optional[Var[Union[bool, int]]]
-    filter_option: Optional[Var[bool]]
-    not_found_content: Optional[Var[ReactNode]]
-    open: Optional[Var[bool]]
-    options: Optional[Var[list]]
-    placeholder: Optional[Var[str]]
-    status: Optional[Var[str]]
-    size: Optional[Var[SizeType]]
-    value: Optional[Var[str]]
-    variant: Optional[Var[VariantType]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_BLUR: lambda: [],
-            "on_dropdown_visible_change": lambda open: [open],
-            EventTriggers.ON_FOCUS: lambda: [],
-            "on_search": lambda value: [value],
-            EventTriggers.ON_SELECT: lambda value, option: [value, option],
-            "on_clear": lambda: [],
-        })
-        return _triggers
-
-
-auto_complete = AutoComplete.create
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import PlacementType, DirectionType
+
+
+class Dropdown(AntdComponent):
+    tag = 'Dropdown'
+
+    arrow: Optional[Var[bool]]
+    auto_adjust_overflow: Optional[Var[bool]]
+    auto_focus: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    destroy_popup_on_hide: Optional[Var[bool]]
+    dropdown_render: Optional[Var[JsValue]]
+    menu: Optional[Var[Union[ContainVar, list]]]
+    placement: Optional[Var[PlacementType]]
+    trigger: Optional[Var[ContainVar]]
+    open: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        _triggers.update({
+            EventTriggers.ON_OPEN_CHANGE: lambda open, info: [open, info],
+        })
+        return _triggers
+
+
+class DropdownButton(Dropdown):
+    tag = 'Dropdown.Button'
+
+    buttons_render: Optional[Var[JsValue]]
+    loading: Optional[Var[bool]]
+    danger: Optional[Var[bool]]
+    icon: Optional[Var[ReactNode]]
+    size: Optional[Var[str]]
+    type: Optional[Var[str]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        _triggers.update({
+            EventTriggers.ON_CLICK: lambda: [],
+        })
+        return _triggers
+
+
+dropdown = Dropdown.create
+dropdown_button = DropdownButton.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/auto_complete.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/auto_complete.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/avatar.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/avatar.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-
-
-class Avatar(AntdComponent):
-    tag = 'Avatar'
-
-    alt: Optional[Var[str]]
-    gap: Optional[Var[int]]
-    icon: Optional[Var[ReactNode]]
-    shape: Optional[Var[str]]
-    size: Optional[Var[Union[str, int, Dict]]]
-    src: Optional[Var[ReactNode]]
-    src_set: Optional[Var[str]]
-    draggable: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_error": lambda: [],
-        })
-        return _triggers
-
-
-class AvatarGroup(AntdComponent):
-    tag = 'Avatar.Group'
-
-    max_count: Optional[Var[int]]
-    max_popover_placement: Optional[Var[str]]
-    max_popover_trigger: Optional[Var[str]]
-    max_style: Optional[Var[Dict]]
-    size: Optional[Var[Union[str, int, Dict]]]
-    shape: Optional[Var[str]]
-
-
-avatar = Avatar.create
-avatar_group = AvatarGroup.create
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+
+
+class Avatar(AntdComponent):
+    tag = 'Avatar'
+
+    alt: Optional[Var[str]]
+    gap: Optional[Var[int]]
+    icon: Optional[Var[ReactNode]]
+    shape: Optional[Var[str]]
+    size: Optional[Var[Union[str, int, Dict]]]
+    src: Optional[Var[ReactNode]]
+    src_set: Optional[Var[str]]
+    draggable: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_error": lambda: [],
+        })
+        return _triggers
+
+
+class AvatarGroup(AntdComponent):
+    tag = 'Avatar.Group'
+
+    max_count: Optional[Var[int]]
+    max_popover_placement: Optional[Var[str]]
+    max_popover_trigger: Optional[Var[str]]
+    max_style: Optional[Var[Dict]]
+    size: Optional[Var[Union[str, int, Dict]]]
+    shape: Optional[Var[str]]
+
+
+avatar = Avatar.create
+avatar_group = AvatarGroup.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/avatar.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/badge.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/breadcrumb.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/button.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-from typing import Optional, Union, Dict, Any
-from reflex import Var
-
-from ..base import AntdComponent, ContainVar, ReactNode
-
-
-class Breadcrumb(AntdComponent):
-    tag = "Breadcrumb"
-
-    params: Optional[Var[dict]]
-    items: Optional[Var[Union[ContainVar, list]]]
-    separator: Optional[Var[ReactNode]]
-
-
-class RouteItemType(AntdComponent):
-    tag = "RouteItemType"
-
-    class_name: Optional[Var[str]]
-    href: Optional[Var[str]]
-    path: Optional[Var[str]]
-    title: Optional[Var[ReactNode]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_click': lambda e: [e],
-        })
-        return _triggers
-
-
-breadcrumb = Breadcrumb.create
+from typing import Optional, Union, Dict, Any
+
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, ReactNode
+from ..constant import TypeType, ButtonShape, SizeType
+
+
+class Button(AntdComponent):
+    tag = "Button"
+
+    block: Optional[Var[bool]]
+    danger: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    ghost: Optional[Var[bool]]
+    href: Optional[Var[str]]
+    target: Optional[Var[str]]
+    html_type: Optional[Var[str]]
+    icon: Optional[Var[ReactNode]]
+    loading: Optional[Var[bool]]
+    shape: Optional[Var[ButtonShape]]
+    size: Optional[Var[SizeType]]
+    type: Optional[Var[TypeType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        _triggers.update({
+            EventTriggers.ON_CLICK: lambda: [],
+        })
+        return _triggers
+
+
+button = Button.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/breadcrumb.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/breadcrumb.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/button.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/switch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, ReactNode
-from ..constant import TypeType, ButtonShape, SizeType
-
-
-class Button(AntdComponent):
-    tag = "Button"
-
-    block: Optional[Var[bool]]
-    danger: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    ghost: Optional[Var[bool]]
-    href: Optional[Var[str]]
-    target: Optional[Var[str]]
-    html_type: Optional[Var[str]]
-    icon: Optional[Var[ReactNode]]
-    loading: Optional[Var[bool]]
-    shape: Optional[Var[ButtonShape]]
-    size: Optional[Var[SizeType]]
-    type: Optional[Var[TypeType]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            EventTriggers.ON_CLICK: lambda: [],
-        })
-        return _triggers
-
-
-button = Button.create
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
+
+
+class Switch(AntdComponent):
+    tag = 'Switch'
+
+    auto_focus: Optional[Var[bool]]
+    checked: Optional[Var[bool]]
+    checked_children: Optional[Var[ReactNode]]
+    default_checked: Optional[Var[bool]]
+    default_value: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    loading: Optional[Var[bool]]
+    size: Optional[Var[SizeType]]
+    un_checked_children: Optional[Var[ReactNode]]
+    value: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda checked, e: [checked, e],
+            EventTriggers.ON_CLICK: lambda checked, e: [checked, e],
+        })
+        return _triggers
+
+
+switch = Switch.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/button.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/calendar.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/calendar.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue
-from reflex.constants import EventTriggers
-from .base import Locale
-from reflex.utils import imports
-
-
-class DayJS(JsValue):
-    def serialize(self) -> str:
-        return f"dayjs('{self.value}')"
-
-
-class Calendar(AntdComponent):
-    tag = 'Calendar'
-
-    cell_render: Optional[Var[JsValue]]
-    full_cell_render: Optional[Var[JsValue]]
-    default_value: Optional[Var[JsValue]]
-    disabled_date: Optional[Var[JsValue]]
-    fullscreen: Optional[Var[bool]]
-    header_render: Optional[Var[JsValue]]
-    locale: Optional[Var[Locale]]
-    mode: Optional[Var[str]]
-    value: Optional[Var[JsValue]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_select': lambda value, mode: [value, mode],
-            'on_panel_change': lambda value, mode: [value, mode],
-        })
-        return _triggers
-
-    def _get_imports(self) -> imports.ImportDict:
-        _imports = super()._get_imports()
-        _imports.setdefault("dayjs", []).append(
-            imports.ImportVar(tag="dayjs", is_default=True, install=False),
-        )
-        return _imports
-
-
-dayjs = DayJS
-calendar = Calendar.create
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue
+from reflex.constants import EventTriggers
+from .base import Locale
+from reflex.utils import imports
+
+
+class DayJS(JsValue):
+    def serialize(self) -> str:
+        return f"dayjs('{self.value}')"
+
+
+class Calendar(AntdComponent):
+    tag = 'Calendar'
+
+    cell_render: Optional[Var[JsValue]]
+    full_cell_render: Optional[Var[JsValue]]
+    default_value: Optional[Var[JsValue]]
+    disabled_date: Optional[Var[JsValue]]
+    fullscreen: Optional[Var[bool]]
+    header_render: Optional[Var[JsValue]]
+    locale: Optional[Var[Locale]]
+    mode: Optional[Var[str]]
+    value: Optional[Var[JsValue]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            'on_select': lambda value, mode: [value, mode],
+            'on_panel_change': lambda value, mode: [value, mode],
+        })
+        return _triggers
+
+    def _get_imports(self) -> imports.ImportDict:
+        _imports = super()._get_imports()
+        _imports.setdefault("dayjs", []).append(
+            imports.ImportVar(tag="dayjs", is_default=True, install=False),
+        )
+        return _imports
+
+
+dayjs = DayJS
+calendar = Calendar.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/calendar.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/calendar.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/card.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/card.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-
-
-class Card(AntdComponent):
-    tag = 'Card'
-
-    actions: Optional[Var[ContainVar]]
-    active_tab_key: Optional[Var[str]]
-    bordered: Optional[Var[bool]]
-    cover: Optional[Var[ReactNode]]
-    default_active_tab_key: Optional[Var[str]]
-    extra: Optional[Var[ReactNode]]
-    hoverable: Optional[Var[bool]]
-    loading: Optional[Var[bool]]
-    size: Optional[Var[str]]
-    tab_bar_extra_content: Optional[Var[ReactNode]]
-    tab_list: Optional[Var[list[ContainVar]]]
-    title: Optional[Var[ReactNode]]
-    type: Optional[Var[str]]
-    tab_props: Optional[Var[Union[ContainVar, dict]]]
-    class_names: Optional[Var[dict]]
-    styles: Optional[Var[dict]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_tab_change': lambda key: [key],
-        })
-        return _triggers
-
-
-class CardGrid(AntdComponent):
-    tag = 'Card.Grid'
-
-    hoverable: Optional[Var[bool]]
-
-
-class CardMeta(AntdComponent):
-    tag = 'Card.Meta'
-
-    avatar: Optional[Var[ReactNode]]
-    description: Optional[Var[ReactNode]]
-    title: Optional[Var[ReactNode]]
-
-
-card = Card.create
-card_grid = CardGrid.create
-card_meta = CardMeta.create
+from typing import Optional, Union, Dict, Any, List
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+
+
+class Card(AntdComponent):
+    tag = 'Card'
+
+    actions: Optional[Var[ContainVar]]
+    active_tab_key: Optional[Var[str]]
+    bordered: Optional[Var[bool]]
+    cover: Optional[Var[ReactNode]]
+    default_active_tab_key: Optional[Var[str]]
+    extra: Optional[Var[ReactNode]]
+    hoverable: Optional[Var[bool]]
+    loading: Optional[Var[bool]]
+    size: Optional[Var[str]]
+    tab_bar_extra_content: Optional[Var[ReactNode]]
+    tab_list: Optional[Var[list[ContainVar]]]
+    title: Optional[Var[ReactNode]]
+    type: Optional[Var[str]]
+    tab_props: Optional[Var[Union[ContainVar, dict]]]
+    class_names: Optional[Var[dict]]
+    styles: Optional[Var[dict]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            'on_tab_change': lambda key: [key],
+        })
+        return _triggers
+
+
+class CardGrid(AntdComponent):
+    tag = 'Card.Grid'
+
+    hoverable: Optional[Var[bool]]
+
+
+class CardMeta(AntdComponent):
+    tag = 'Card.Meta'
+
+    avatar: Optional[Var[ReactNode]]
+    description: Optional[Var[ReactNode]]
+    title: Optional[Var[ReactNode]]
+
+
+card = Card.create
+card_grid = CardGrid.create
+card_meta = CardMeta.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/card.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/carousel.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/result.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,23 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue
-
-
-class Carousel(AntdComponent):
-    tag = 'Carousel'
-
-    autoplay: Optional[Var[bool]]
-    autoplay_speed: Optional[Var[int]]
-    dot_position: Optional[Var[str]]
-    dots: Optional[Var[Union[bool, dict]]]
-    fade: Optional[Var[bool]]
-    infinite: Optional[Var[bool]]
-    speed: Optional[Var[int]]
-    easing: Optional[Var[str]]
-    wait_for_animate: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'after_change': lambda current: [],
-            'before_change': lambda current, next: [],
-        })
-        return _triggers
-
-
-carousel = Carousel.create
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType
+
+
+class Result(AntdComponent):
+    tag = 'Result'
+
+    extra: Optional[Var[ReactNode]]
+    icon: Optional[Var[ReactNode]]
+    status: Optional[Var[Union[StatusType, str]]]
+    sub_title: Optional[Var[ReactNode]]
+    title: Optional[Var[ReactNode]]
+
+
+result = Result.create
+
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/carousel.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/carousel.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/cascader.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/cascader.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import TriggerType, PlacementType, SizeType, StatusType, VariantType
-
-
-class Cascader(AntdComponent):
-    tag = 'Cascader'
-
-    allow_clear: Optional[Var[bool]]
-    auto_clear_search_value: Optional[Var[bool]]
-    auto_focus: Optional[Var[bool]]
-    change_on_select: Optional[Var[bool]]
-    default_value: Optional[Var[Union[List[int], List[str]]]]
-    disabled: Optional[Var[bool]]
-    display_render: Optional[Var[JsValue]]
-    tag_render: Optional[Var[JsValue]]
-    popup_class_name: Optional[Var[str]]
-    dropdown_render: Optional[Var[JsValue]]
-    expand_icon: Optional[Var[ReactNode]]
-    expand_trigger: Optional[Var[TriggerType]]
-    field_names: Optional[Var[ContainVar]]
-    get_popup_container: Optional[Var[JsValue]]
-    load_data: Optional[Var[JsValue]]
-    max_tag_count: Optional[Var[int]]
-    max_tag_placeholder: Optional[Var[Union[ReactNode, JsValue]]]
-    max_tag_text_length: Optional[Var[int]]
-    not_found_content: Optional[Var[str]]
-    open: Optional[Var[bool]]
-    options: Optional[Var[Union[ContainVar, list]]]
-    placeholder: Optional[Var[ReactNode]]
-    placement: Optional[Var[PlacementType]]
-    show_search: Optional[Var[Union[bool, ContainVar]]]
-    size: Optional[Var[SizeType]]
-    status: Optional[Var[StatusType]]
-    suffix_icon: Optional[Var[ReactNode]]
-    value: Optional[Var[Union[List[str], List[int]]]]
-    variant: Optional[Var[VariantType]]
-    multiple: Optional[Var[bool]]
-    remove_icon: Optional[Var[ReactNode]]
-    show_checked_strategy: Optional[Var[str]]
-    search_value: Optional[Var[str]]
-    dropdown_menu_column_style: Optional[Var[ContainVar]]
-    loading_icon: Optional[Var[ReactNode]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda value, options: [value, options],
-            "on_dropdown_visible_change": lambda value: [value],
-            "on_search": lambda search: [search]
-        })
-        return _triggers
-
-
-cascader = Cascader.create
+from typing import Optional, Union, Dict, Any, List
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import TriggerType, PlacementType, SizeType, StatusType, VariantType
+
+
+class Cascader(AntdComponent):
+    tag = 'Cascader'
+
+    allow_clear: Optional[Var[bool]]
+    auto_clear_search_value: Optional[Var[bool]]
+    auto_focus: Optional[Var[bool]]
+    change_on_select: Optional[Var[bool]]
+    default_value: Optional[Var[Union[List[int], List[str]]]]
+    disabled: Optional[Var[bool]]
+    display_render: Optional[Var[JsValue]]
+    tag_render: Optional[Var[JsValue]]
+    popup_class_name: Optional[Var[str]]
+    dropdown_render: Optional[Var[JsValue]]
+    expand_icon: Optional[Var[ReactNode]]
+    expand_trigger: Optional[Var[TriggerType]]
+    field_names: Optional[Var[ContainVar]]
+    get_popup_container: Optional[Var[JsValue]]
+    load_data: Optional[Var[JsValue]]
+    max_tag_count: Optional[Var[int]]
+    max_tag_placeholder: Optional[Var[Union[ReactNode, JsValue]]]
+    max_tag_text_length: Optional[Var[int]]
+    not_found_content: Optional[Var[str]]
+    open: Optional[Var[bool]]
+    options: Optional[Var[Union[ContainVar, list]]]
+    placeholder: Optional[Var[ReactNode]]
+    placement: Optional[Var[PlacementType]]
+    show_search: Optional[Var[Union[bool, ContainVar]]]
+    size: Optional[Var[SizeType]]
+    status: Optional[Var[StatusType]]
+    suffix_icon: Optional[Var[ReactNode]]
+    value: Optional[Var[Union[List[str], List[int]]]]
+    variant: Optional[Var[VariantType]]
+    multiple: Optional[Var[bool]]
+    remove_icon: Optional[Var[ReactNode]]
+    show_checked_strategy: Optional[Var[str]]
+    search_value: Optional[Var[str]]
+    dropdown_menu_column_style: Optional[Var[ContainVar]]
+    loading_icon: Optional[Var[ReactNode]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda value, options: [value, options],
+            "on_dropdown_visible_change": lambda value: [value],
+            "on_search": lambda search: [search]
+        })
+        return _triggers
+
+
+cascader = Cascader.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/cascader.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/cascader.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/checkbox.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/checkbox.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar
-from ..constant import StatusType, SizeType
-
-
-class Checkbox(AntdComponent):
-    tag = "Checkbox"
-
-    auto_focus: Optional[Var[bool]]
-    checked: Optional[Var[bool]]
-    default_checked: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    indeterminate: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda e: [e],
-        })
-        return _triggers
-
-
-class CheckboxGroup(AntdComponent):
-    tag = 'Checkbox.Group'
-
-    default_value: Optional[Var[List[Union[int, str]]]]
-    disabled: Optional[Var[bool]]
-    name: Optional[Var[str]]
-    options: Optional[Var[List[Union[str, int, Dict]]]]
-    value: Optional[Var[List[Union[int, str, bool]]]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda checked_value: [checked_value],
-        })
-        return _triggers
-
-
-checkbox = Checkbox.create
-checkbox_group = CheckboxGroup.create
-
-
-
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar
+from ..constant import StatusType, SizeType
+
+
+class Checkbox(AntdComponent):
+    tag = "Checkbox"
+
+    auto_focus: Optional[Var[bool]]
+    checked: Optional[Var[bool]]
+    default_checked: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    indeterminate: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda e: [e],
+        })
+        return _triggers
+
+
+class CheckboxGroup(AntdComponent):
+    tag = 'Checkbox.Group'
+
+    default_value: Optional[Var[List[Union[int, str]]]]
+    disabled: Optional[Var[bool]]
+    name: Optional[Var[str]]
+    options: Optional[Var[List[Union[str, int, Dict]]]]
+    value: Optional[Var[List[Union[int, str, bool]]]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda checked_value: [checked_value],
+        })
+        return _triggers
+
+
+checkbox = Checkbox.create
+checkbox_group = CheckboxGroup.create
+
+
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/checkbox.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/collapse.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/drawer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,44 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-
-
-class Collapse(AntdComponent):
-    tag = 'Collapse'
-
-    accordion: Optional[Var[bool]]
-    active_key: Optional[Var[Union[list[str], str, list[int], int]]]
-    bordered: Optional[Var[bool]]
-    default_active_key: Optional[Var[Union[list[str], str, list[int], int]]]
-    destroy_inactive_panel: Optional[Var[bool]]
-    expand_icon: Optional[Var[ReactNode]]
-    collapsible: Optional[Var[str]]
-    expand_icon_position: Optional[Var[str]]
-    ghost: Optional[Var[bool]]
-    size: Optional[Var[str]]
-    items: Optional[Var[Union[ContainVar, list]]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_change': lambda: [],
-        })
-        return _triggers
-
-
-collapse = Collapse.create
+from typing import Optional, Union, Dict, Any, List
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import OrientationType, SizeType
+
+
+class Drawer(AntdComponent):
+    tag = 'Drawer'
+
+    auto_focus: Optional[Var[bool]]
+    class_name: Optional[Var[str]]
+    class_names: Optional[Var[ContainVar]]
+    close_icon: Optional[Var[Union[ReactNode, bool]]]
+    destroy_on_close: Optional[Var[bool]]
+    extra: Optional[Var[ReactNode]]
+    footer: Optional[Var[ReactNode]]
+    force_render: Optional[Var[bool]]
+    get_container: Optional[Var[Union[ContainVar, bool]]]
+    height: Optional[Var[Union[str, int]]]
+    keyboard: Optional[Var[bool]]
+    mask: Optional[Var[bool]]
+    mask_closable: Optional[Var[bool]]
+    placement: Optional[Var[OrientationType]]
+    push: Optional[Var[Union[bool, dict]]]
+    root_style: Optional[Var[dict]]
+    size: Optional[Var[SizeType]]
+    styles: Optional[Var[ContainVar]]
+    title: Optional[Var[ReactNode]]
+    open: Optional[Var[bool]]
+    width: Optional[Var[Union[str, int]]]
+    z_index: Optional[Var[int]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "after_open_change": lambda open: [open],
+            "on_close": lambda e: [e],
+        })
+        return _triggers
+
+
+drawer = Drawer.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/collapse.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/collapse.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/color_picker.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/qrcode.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,34 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue,ReactNode
-from ..constant import ColorFormatType, SizeType, PlacementType, TriggerType
-
-
-class ColorPicker(AntdComponent):
-    tag = 'ColorPicker'
-
-    allow_clear: Optional[Var[bool]]
-    arrow: Optional[Var[bool]]
-    default_value: Optional[Var[str]]
-    default_format: Optional[Var[str]]
-    disabled: Optional[Var[bool]]
-    disabled_alpha: Optional[Var[bool]]
-    destroy_tooltip_on_hide: Optional[Var[bool]]
-    format: Optional[Var[ColorFormatType]]
-    open: Optional[Var[bool]]
-    presets: Optional[Var[ContainVar]]
-    placement: Optional[Var[PlacementType]]
-    panel_render: Optional[Var[JsValue]]
-    show_text: Optional[Var[Union[bool, JsValue]]]
-    size: Optional[Var[SizeType]]
-    trigger: Optional[Var[TriggerType]]
-    value: Optional[Var[str]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda value, hex: [value, hex],
-            'on_change_complete': lambda value: [value],
-            'on_format_change': lambda format: [format],
-            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
-            'on_clear': lambda: [],
-        })
-        return _triggers
-
-
-color_picker = ColorPicker.create
-
-
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import SizeType, QRCodeType, QRCodeErrorLevelType, QRCodeStatusType
+
+
+class QRCode(AntdComponent):
+    tag = 'QRCode'
+
+    value: Optional[Var[str]]
+    type: Optional[Var[QRCodeType]]
+    icon: Optional[Var[str]]
+    size: Optional[Var[int]]
+    icon_size: Optional[Var[int]]
+    color: Optional[Var[str]]
+    bg_color: Optional[Var[str]]
+    bordered: Optional[Var[bool]]
+    error_level: Optional[Var[QRCodeErrorLevelType]]
+    status: Optional[Var[QRCodeStatusType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_refresh": lambda: [],
+        })
+        return _triggers
+
+
+qrcode = QRCode.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/color_picker.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/color_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/date_picker.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/date_picker.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import DatePickerModeType, DatePickerType, SizeType, PlacementType, StatusType, VariantType
-
-from .base import Locale
-
-
-class DayJS(JsValue):
-    def serialize(self) -> str:
-        return f"dayjs('{self.value}')"
-
-
-class BaseDatePicker(AntdComponent):
-
-    allow_clear: Optional[Var[bool]]
-    auto_focus: Optional[Var[bool]]
-    date_render: Optional[Var[JsValue]]
-    cell_render: Optional[Var[JsValue]]
-    components: Optional[Var[Union[ReactNode, list, dict, ContainVar]]]
-    disabled: Optional[Var[bool]]
-    disabled_date: Optional[Var[JsValue]]
-    format: Optional[Var[ContainVar]]
-    order: Optional[Var[bool]]
-    popup_class_name: Optional[Var[str]]
-    preserve_invalidOn_blur: Optional[Var[bool]]
-    getPopup_container: Optional[Var[JsValue]]
-    input_readOnly: Optional[Var[bool]]
-    locale: Optional[Var[Locale]]
-    min_date: Optional[Var[JsValue]]
-    max_date: Optional[Var[JsValue]]
-    mode: Optional[Var[DatePickerModeType]]
-    need_confirm: Optional[Var[bool]]
-    next_icon: Optional[Var[ReactNode]]
-    open: Optional[Var[bool]]
-    panel_render: Optional[Var[JsValue]]
-    picker: Optional[Var[DatePickerType]]
-    placeholder: Optional[Var[Union[str, List[str]]]]
-    placement: Optional[Var[PlacementType]]
-    popup_style: Optional[Var[ContainVar]]
-    presets: Optional[Var[ContainVar]]
-    prev_icon: Optional[Var[ReactNode]]
-    size: Optional[Var[SizeType]]
-    status: Optional[Var[StatusType]]
-    suffix_icon: Optional[Var[ReactNode]]
-    super_next_icon: Optional[Var[ReactNode]]
-    super_prev_icon: Optional[Var[ReactNode]]
-    variant: Optional[Var[VariantType]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
-            'on_panel_change': lambda value, mode: [value, mode],
-        })
-        return _triggers
-
-    def _get_imports(self) -> imports.ImportDict:
-        _imports = super()._get_imports()
-        _imports.setdefault("dayjs", []).append(
-            imports.ImportVar(tag="dayjs", is_default=True, install=False),
-        )
-        return _imports
-
-
-class DatePicker(BaseDatePicker):
-    tag = 'DatePicker'
-
-    default_picker_value: Optional[Var[JsValue]]
-    default_value: Optional[Var[ContainVar]]
-    disabled_time: Optional[Var[JsValue]]
-    format: Optional[Var[ContainVar]]
-    multiple: Optional[Var[bool]]
-    picker_value: Optional[Var[ContainVar]]
-    render_extra_footer: Optional[Var[JsValue]]
-    show_now: Optional[Var[bool]]
-    show_time: Optional[Var[Union[bool, ContainVar]]]
-    # showTime.defaultValue
-    show_week: Optional[Var[bool]]
-    value: Optional[Var[ContainVar]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda date, sdate: [date, sdate],
-            "on_ok": lambda: [],
-            "on_panel_change": lambda value, mode: [value, mode],
-        })
-        return _triggers
-
-
-class RangePicker(BaseDatePicker):
-    tag = 'RangePicker'
-
-    allow_empty: Optional[Var[Tuple[bool, bool]]]
-    cell_render: Optional[Var[JsValue]]
-    date_render: Optional[Var[JsValue]]
-    default_picker_value: Optional[Var[ContainVar]]
-    default_value: Optional[Var[ContainVar]]
-    disabled: Optional[Var[Tuple[bool, bool]]]
-    disabled_time: Optional[Var[JsValue]]
-    format: Optional[Var[ContainVar]]
-    id: Optional[Var[Dict[str, str]]]
-    picker_value: Optional[Var[ContainVar]]
-    presets: Optional[Var[ContainVar]]
-    render_extra_footer: Optional[Var[JsValue]]
-    separator: Optional[Var[ReactNode]]
-    show_time: Optional[Var[Union[bool, ContainVar]]]
-    # showTime.defaultValue
-    value: Optional[Var[ContainVar]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_calendar_change": lambda dates, sdates, info: [dates, sdates, info],
-            EventTriggers.ON_CHANGE: lambda dates, sdates: [dates, sdates],
-            EventTriggers.ON_FOCUS: lambda ev, range: [ev, range],
-            EventTriggers.ON_BLUR: lambda ev, range: [ev, range],
-        })
-        return _triggers
-
-    def _get_imports(self) -> imports.ImportDict:
-        _imports = super()._get_imports()
-        _vars: List = [v for v in _imports[self.library] if v.tag != "RangePicker"]
-        _vars.append(
-            imports.ImportVar(tag="DatePicker"),
-        )
-        _imports[self.library] = _vars
-
-        return _imports
-
-    def _get_hooks(self) -> str | None:
-        return "const { RangePicker } = DatePicker;"
-
-
-dayjs = DayJS
-date_picker = DatePicker.create
-range_picker = RangePicker.create
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import DatePickerModeType, DatePickerType, SizeType, PlacementType, StatusType, VariantType
+
+from .base import Locale
+
+
+class DayJS(JsValue):
+    def serialize(self) -> str:
+        return f"dayjs('{self.value}')"
+
+
+class BaseDatePicker(AntdComponent):
+
+    allow_clear: Optional[Var[bool]]
+    auto_focus: Optional[Var[bool]]
+    date_render: Optional[Var[JsValue]]
+    cell_render: Optional[Var[JsValue]]
+    components: Optional[Var[Union[ReactNode, list, dict, ContainVar]]]
+    disabled: Optional[Var[bool]]
+    disabled_date: Optional[Var[JsValue]]
+    format: Optional[Var[ContainVar]]
+    order: Optional[Var[bool]]
+    popup_class_name: Optional[Var[str]]
+    preserve_invalidOn_blur: Optional[Var[bool]]
+    getPopup_container: Optional[Var[JsValue]]
+    input_readOnly: Optional[Var[bool]]
+    locale: Optional[Var[Locale]]
+    min_date: Optional[Var[JsValue]]
+    max_date: Optional[Var[JsValue]]
+    mode: Optional[Var[DatePickerModeType]]
+    need_confirm: Optional[Var[bool]]
+    next_icon: Optional[Var[ReactNode]]
+    open: Optional[Var[bool]]
+    panel_render: Optional[Var[JsValue]]
+    picker: Optional[Var[DatePickerType]]
+    placeholder: Optional[Var[Union[str, List[str]]]]
+    placement: Optional[Var[PlacementType]]
+    popup_style: Optional[Var[ContainVar]]
+    presets: Optional[Var[ContainVar]]
+    prev_icon: Optional[Var[ReactNode]]
+    size: Optional[Var[SizeType]]
+    status: Optional[Var[StatusType]]
+    suffix_icon: Optional[Var[ReactNode]]
+    super_next_icon: Optional[Var[ReactNode]]
+    super_prev_icon: Optional[Var[ReactNode]]
+    variant: Optional[Var[VariantType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
+            'on_panel_change': lambda value, mode: [value, mode],
+        })
+        return _triggers
+
+    def _get_imports(self) -> imports.ImportDict:
+        _imports = super()._get_imports()
+        _imports.setdefault("dayjs", []).append(
+            imports.ImportVar(tag="dayjs", is_default=True, install=False),
+        )
+        return _imports
+
+
+class DatePicker(BaseDatePicker):
+    tag = 'DatePicker'
+
+    default_picker_value: Optional[Var[JsValue]]
+    default_value: Optional[Var[ContainVar]]
+    disabled_time: Optional[Var[JsValue]]
+    format: Optional[Var[ContainVar]]
+    multiple: Optional[Var[bool]]
+    picker_value: Optional[Var[ContainVar]]
+    render_extra_footer: Optional[Var[JsValue]]
+    show_now: Optional[Var[bool]]
+    show_time: Optional[Var[Union[bool, ContainVar]]]
+    # showTime.defaultValue
+    show_week: Optional[Var[bool]]
+    value: Optional[Var[ContainVar]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda date, sdate: [date, sdate],
+            "on_ok": lambda: [],
+            "on_panel_change": lambda value, mode: [value, mode],
+        })
+        return _triggers
+
+
+class RangePicker(BaseDatePicker):
+    tag = 'RangePicker'
+
+    allow_empty: Optional[Var[Tuple[bool, bool]]]
+    cell_render: Optional[Var[JsValue]]
+    date_render: Optional[Var[JsValue]]
+    default_picker_value: Optional[Var[ContainVar]]
+    default_value: Optional[Var[ContainVar]]
+    disabled: Optional[Var[Tuple[bool, bool]]]
+    disabled_time: Optional[Var[JsValue]]
+    format: Optional[Var[ContainVar]]
+    id: Optional[Var[Dict[str, str]]]
+    picker_value: Optional[Var[ContainVar]]
+    presets: Optional[Var[ContainVar]]
+    render_extra_footer: Optional[Var[JsValue]]
+    separator: Optional[Var[ReactNode]]
+    show_time: Optional[Var[Union[bool, ContainVar]]]
+    # showTime.defaultValue
+    value: Optional[Var[ContainVar]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_calendar_change": lambda dates, sdates, info: [dates, sdates, info],
+            EventTriggers.ON_CHANGE: lambda dates, sdates: [dates, sdates],
+            EventTriggers.ON_FOCUS: lambda ev, range: [ev, range],
+            EventTriggers.ON_BLUR: lambda ev, range: [ev, range],
+        })
+        return _triggers
+
+    def _get_imports(self) -> imports.ImportDict:
+        _imports = super()._get_imports()
+        _vars: List = [v for v in _imports[self.library] if v.tag != "RangePicker"]
+        _vars.append(
+            imports.ImportVar(tag="DatePicker"),
+        )
+        _imports[self.library] = _vars
+
+        return _imports
+
+    def _get_hooks(self) -> str | None:
+        return "const { RangePicker } = DatePicker;"
+
+
+dayjs = DayJS
+date_picker = DatePicker.create
+range_picker = RangePicker.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/date_picker.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/descriptions.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/progress.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,35 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue,ReactNode
-from ..constant import VariantType, SizeType,DirectionType
-
-
-class Descriptions(AntdComponent):
-    tag = 'Descriptions'
-
-    bordered: Optional[Var[bool]]
-    colon: Optional[Var[bool]]
-    column: Optional[Var[Union[int,dict]]]
-    content_style: Optional[Var[Union[dict,ContainVar]]]
-    extra: Optional[Var[ReactNode]]
-    items: Optional[Var[Union[ContainVar,list]]]
-    label_style: Optional[Var[dict]]
-    layout: Optional[Var[DirectionType]]
-    size: Optional[Var[SizeType]]
-    title: Optional[Var[ReactNode]]
-
-
-descriptions = Descriptions.create
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import StatusType, ProgressType, SizeType, OrientationType
+
+
+class Progress(AntdComponent):
+    tag = 'Progress'
+
+    format: Optional[Var[JsValue]]
+    percent: Optional[Var[int]]
+    show_info: Optional[Var[bool]]
+    status: Optional[Var[StatusType]]
+    stroke_color: Optional[Var[str]]
+    stroke_linecap: Optional[Var[str]]
+    success: Optional[Var[Dict]]
+    trail_color: Optional[Var[str]]
+    type: Optional[Var[ProgressType]]
+    size: Optional[Var[Union[int, SizeType, List[Union[int, SizeType]]]]]
+    # type=...
+    steps: Optional[Var[Union[int, Dict]]]
+    stroke_color: Optional[Var[Union[str, List[str], Dict]]]
+    stroke_width: Optional[Var[int]]
+    # dashboard
+    gap_degree: Optional[Var[int]]
+    gap_position: Optional[Var[OrientationType]]
+
+
+progress = Progress.create
+
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/descriptions.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/descriptions.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/divider.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/divider.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/drawer.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/list.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import OrientationType, SizeType
-
-
-class Drawer(AntdComponent):
-    tag = 'Drawer'
-
-    auto_focus: Optional[Var[bool]]
-    class_name: Optional[Var[str]]
-    class_names: Optional[Var[ContainVar]]
-    close_icon: Optional[Var[Union[ReactNode, bool]]]
-    destroy_on_close: Optional[Var[bool]]
-    extra: Optional[Var[ReactNode]]
-    footer: Optional[Var[ReactNode]]
-    force_render: Optional[Var[bool]]
-    get_container: Optional[Var[Union[ContainVar, bool]]]
-    height: Optional[Var[Union[str, int]]]
-    keyboard: Optional[Var[bool]]
-    mask: Optional[Var[bool]]
-    mask_closable: Optional[Var[bool]]
-    placement: Optional[Var[OrientationType]]
-    push: Optional[Var[Union[bool, dict]]]
-    root_style: Optional[Var[dict]]
-    size: Optional[Var[SizeType]]
-    styles: Optional[Var[ContainVar]]
-    title: Optional[Var[ReactNode]]
-    open: Optional[Var[bool]]
-    width: Optional[Var[Union[str, int]]]
-    z_index: Optional[Var[int]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "after_open_change": lambda open: [open],
-            "on_close": lambda e: [e],
-        })
-        return _triggers
-
-
-drawer = Drawer.create
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import SizeType
+
+
+class AList(AntdComponent):
+    tag = 'List'
+
+    bordered: Optional[Var[bool]]
+    data_source: Optional[Var[Any]]
+    footer: Optional[Var[ReactNode]]
+    grid: Optional[Var[dict]]
+    header: Optional[Var[ReactNode]]
+    item_layout: Optional[Var[str]]
+    loading: Optional[Var[Union[bool, dict]]]
+    load_more: Optional[Var[ReactNode]]
+    locale: Optional[Var[dict]]
+    pagination: Optional[Var[Union[bool, dict]]]
+    render_item: Optional[Var[JsValue]]
+    size: Optional[Var[SizeType]]
+    split: Optional[Var[bool]]
+
+
+class ListItem(AntdComponent):
+    tag = 'List.Item'
+
+    actions: Optional[Var[list[ContainVar]]]
+    extra: Optional[Var[ReactNode]]
+
+
+class ListItemMeta(AntdComponent):
+    tag = 'List.Item.Meta'
+
+    avatar: Optional[Var[ReactNode]]
+    description: Optional[Var[ReactNode]]
+    title: Optional[Var[ReactNode]]
+
+
+alist = AList.create
+list_item = ListItem.create
+list_item_meta = ListItemMeta.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/drawer.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/dropdown.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tour.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,40 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import PlacementType, DirectionType
-
-
-class Dropdown(AntdComponent):
-    tag = 'Dropdown'
-
-    arrow: Optional[Var[bool]]
-    auto_adjust_overflow: Optional[Var[bool]]
-    auto_focus: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    destroy_popup_on_hide: Optional[Var[bool]]
-    dropdown_render: Optional[Var[JsValue]]
-    menu: Optional[Var[Union[ContainVar, list]]]
-    placement: Optional[Var[PlacementType]]
-    trigger: Optional[Var[ContainVar]]
-    open: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            EventTriggers.ON_OPEN_CHANGE: lambda open, info: [open, info],
-        })
-        return _triggers
-
-
-class DropdownButton(Dropdown):
-    tag = 'Dropdown.Button'
-
-    buttons_render: Optional[Var[JsValue]]
-    loading: Optional[Var[bool]]
-    danger: Optional[Var[bool]]
-    icon: Optional[Var[ReactNode]]
-    size: Optional[Var[str]]
-    type: Optional[Var[str]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            EventTriggers.ON_CLICK: lambda: [],
-        })
-        return _triggers
-
-
-dropdown = Dropdown.create
-dropdown_button = DropdownButton.create
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, PlacementType, TypeType
+
+
+class Tour(AntdComponent):
+    tag = 'Tour'
+
+    arrow: Optional[Var[bool]]
+    close_icon: Optional[Var[ReactNode]]
+    disabled_interaction: Optional[Var[bool]]
+    placement: Optional[Var[PlacementType]]
+    mask: Optional[Var[Union[bool, Dict]]]
+    type: Optional[Var[TypeType]]
+    open: Optional[Var[bool]]
+    current: Optional[Var[int]]
+    scroll_into_view_options: Optional[Var[Union[bool, Dict]]]
+    steps: Optional[Var[ContainVar]]
+    indicators_render: Optional[Var[JsValue]]
+    z_index: Optional[Var[int]]
+    get_popup_container: Optional[Var[JsValue]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            'on_close': lambda: [],
+            'on_finish': lambda: [],
+            EventTriggers.ON_CHANGE: lambda current: [current],
+            'steps.*.on_close': lambda: [],
+        })
+        return _triggers
+
+
+tour = Tour.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/dropdown.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/dropdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/empty.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/empty.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/flex.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/float_button.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/float_button.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from typing import Optional, Union, Dict, Any
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, ReactNode, JsValue
-from ..constant import TypeType, TriggerType, FloatGroupShapeType
-
-from .badge import Badge
-
-
-class FloatButton(AntdComponent):
-    tag = "FloatButton"
-
-    icon: Optional[Var[ReactNode]]
-    description: Optional[Var[ReactNode]]
-    tooltip: Optional[Var[Union[ReactNode, JsValue]]]
-    type: Optional[Var[TypeType]]
-    shape: Optional[Var[FloatGroupShapeType]]
-    href: Optional[Var[str]]
-    target: Optional[Var[str]]
-    badge: Optional[Var[Union[Dict]]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CLICK: lambda: [],
-        })
-        return _triggers
-
-
-class FloatGroup(FloatButton):
-    tag = "FloatButton.Group"
-
-    open: Optional[Var[bool]]
-    trigger: Optional[Var[TriggerType]]
-    close_icon: Optional[Var[ReactNode]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
-        })
-        return _triggers
-
-
-class FloatBackTop(FloatButton):
-    tag = "FloatButton.BackTop"
-
-    duration: Optional[Var[int]]
-    target: Optional[Var[Union[ReactNode, JsValue]]]
-    visibility_height: Optional[Var[int]]
-
-
-float_button = FloatButton.create
-float_group = FloatGroup.create
-float_back_top = FloatBackTop.create
+from typing import Optional, Union, Dict, Any
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, ReactNode, JsValue
+from ..constant import TypeType, TriggerType, FloatGroupShapeType
+
+from .badge import Badge
+
+
+class FloatButton(AntdComponent):
+    tag = "FloatButton"
+
+    icon: Optional[Var[ReactNode]]
+    description: Optional[Var[ReactNode]]
+    tooltip: Optional[Var[Union[ReactNode, JsValue]]]
+    type: Optional[Var[TypeType]]
+    shape: Optional[Var[FloatGroupShapeType]]
+    href: Optional[Var[str]]
+    target: Optional[Var[str]]
+    badge: Optional[Var[Union[Dict]]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CLICK: lambda: [],
+        })
+        return _triggers
+
+
+class FloatGroup(FloatButton):
+    tag = "FloatButton.Group"
+
+    open: Optional[Var[bool]]
+    trigger: Optional[Var[TriggerType]]
+    close_icon: Optional[Var[ReactNode]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
+        })
+        return _triggers
+
+
+class FloatBackTop(FloatButton):
+    tag = "FloatButton.BackTop"
+
+    duration: Optional[Var[int]]
+    target: Optional[Var[Union[ReactNode, JsValue]]]
+    visibility_height: Optional[Var[int]]
+
+
+float_button = FloatButton.create
+float_group = FloatGroup.create
+float_back_top = FloatBackTop.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/float_button.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/float_button.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/form.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/form.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,159 +1,167 @@
-import uuid
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode, js_value
-from ..constant import AlignType, DirectionType, SizeType, VariantType
-
-
-class Form(AntdComponent):
-    tag = 'Form'
-
-    colon: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    fields: Optional[Var[ContainVar]]
-    form: Optional[Var[str]]
-    initial_values: Optional[Var[Dict]]
-    label_align: Optional[Var[AlignType]]
-    label_wrap: Optional[Var[bool]]
-    label_col: Optional[Var[Dict]]
-    layout: Optional[Var[DirectionType]]
-    name: Optional[Var[str]]
-    preserve: Optional[Var[bool]]
-    required_mark: Optional[Var[Union[bool, JsValue]]]
-    scrollTo_first_error: Optional[Var[Union[bool, Dict]]]
-    size: Optional[Var[SizeType]]
-    validate_messages: Optional[Var[Dict]]
-    validate_trigger: Optional[Var[Union[str, List[str]]]]
-    variant: Optional[Var[VariantType]]
-    wrapper_col: Optional[Var[Dict]]
-
-    @classmethod
-    def create(cls, *children, **props) -> Component:
-        if 'form' in props and isinstance(props['form'], str):
-            props['form'] = Var.create_safe(f'{props["form"]}', _var_is_local=False)
-        rs = super().create(*children, **props)
-        return rs
-
-    def _get_hooks(self) -> str | None:
-        if hasattr(self, 'form') and self.form is not None:
-            return f"const [{str(self.form).strip('{}')}] = Form.useForm();"
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_fields_change": lambda changed, all: [changed],
-            'on_finish': lambda values: [values],
-            "on_finish_failed": lambda ev: [ev.values, ev.errorFields, ev.outOfDate],
-            "on_values_change": lambda changed, all: [changed, all],
-        })
-        return _triggers
-
-
-class FormItem(AntdComponent):
-    tag = 'Form.Item'
-
-    colon: Optional[Var[bool]]
-    dependencies: Optional[Var[List[Union[str, int, List[Union[str, int]]]]]]
-    extra: Optional[Var[ReactNode]]
-    getValue_from_event: Optional[Var[JsValue]]
-    get_value_props: Optional[Var[JsValue]]
-    has_feedback: Optional[Var[Union[bool, ContainVar]]]
-    help: Optional[Var[ReactNode]]
-    hidden: Optional[Var[bool]]
-    html_for: Optional[Var[str]]
-    initial_value: Optional[Var[str]]
-    label: Optional[Var[str]]
-    label_align: Optional[Var[AlignType]]
-    label_col: Optional[Var[Dict]]
-    message_variables: Optional[Var[JsValue]]
-    name: Optional[Var[Union[str, int, List[Union[str, int]]]]]
-    normalize: Optional[Var[JsValue]]
-    no_style: Optional[Var[bool]]
-    preserve: Optional[Var[bool]]
-    required: Optional[Var[bool]]
-    rules: Optional[Var[Union[List[Dict], ContainVar]]]
-    should_update: Optional[Var[bool]]
-    tooltip: Optional[Var[Union[Component, ContainVar]]]
-    trigger: Optional[Var[str]]
-    validate_debounce: Optional[Var[float]]
-    validate_first: Optional[Var[Union[bool, str]]]
-    validate_status: Optional[Var[str]]
-    validate_trigger: Optional[Var[Union[str, List[str]]]]
-    value_prop_name: Optional[Var[str]]
-    wrapper_col: Optional[Var[Dict]]
-
-    rules: Optional[Var[List[Dict]]]
-
-
-class FormList(AntdComponent):
-    tag = 'Form.List'
-
-    # children: Optional[Var[JsValue]]
-    initial_value: Optional[Var[List]]
-    name: Optional[Var[Union[str, int, List[Union[str, int]]]]]
-    rules: Optional[Var[ContainVar]]
-
-
-class FormProvider(AntdComponent):
-    tag = 'Form.Provider'
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_form_change": lambda form_name, info: [form_name, info],
-            'on_form_finish': lambda form_name, info: [form_name, info],
-        })
-        return _triggers
-
-
-form = Form.create
-form_item = FormItem.create
-form_list = FormList.create
-form_provider = FormProvider.create
-
-
-def _modal_form(modal_type: str, *children, modal_config=None, form_id: str = None, **props) -> JsValue | Component:
-    from . import modal
-    if form_id is None:
-        form_id = f'form_{uuid.uuid4().hex}'
-    props.update(
-        form=form_id,
-        preserve=False,
-    )
-    f = form(*children, **props)
-
-    modal_config['on_ok'] = js_value(f"""() => {{
-        return new Promise((resolve, reject) => {{
-    {form_id}
-      .validateFields({{
-        validateOnly: false,
-      }})
-      .then(() => {{
-        {form_id}.submit();
-      resolve()}})
-      .catch(() => {{
-      reject()}});
-      }});//if catch will close the form //.catch(() => console.log('Oops errors!'));
-      }}
-    """)
-    op = getattr(modal, modal_type)
-    if modal_type == 'confirm':
-        modal_config['content'] = f
-        return op(config=modal_config)
-    else:
-        modal_config['after_open_change'] = js_value(f"""(open) => {{{form_id}.resetFields()}}""")
-        return op(
-            f,
-            **modal_config)
-
-
-def modal_form(*children, modal_config=None, form_id: str = None, **props) -> Component:
-    return _modal_form('modal',
-                       *children, modal_config=modal_config, form_id=form_id, **props)
-
-
-def confirm_form(*children, confirm_config=None, form_id: str = None, **props) -> JsValue:
-    return _modal_form('confirm',
-                       *children, modal_config=confirm_config, form_id=form_id, **props)
+import uuid
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers, MemoizationMode, MemoizationDisposition
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode, js_value
+from ..constant import AlignType, DirectionType, SizeType, VariantType
+
+
+class Form(AntdComponent):
+    tag = 'Form'
+
+    colon: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    fields: Optional[Var[ContainVar]]
+    form: Optional[Var[str]]
+    initial_values: Optional[Var[Dict]]
+    label_align: Optional[Var[AlignType]]
+    label_wrap: Optional[Var[bool]]
+    label_col: Optional[Var[Dict]]
+    layout: Optional[Var[DirectionType]]
+    name: Optional[Var[str]]
+    preserve: Optional[Var[bool]]
+    required_mark: Optional[Var[Union[bool, JsValue]]]
+    scrollTo_first_error: Optional[Var[Union[bool, Dict]]]
+    size: Optional[Var[SizeType]]
+    validate_messages: Optional[Var[Dict]]
+    validate_trigger: Optional[Var[Union[str, List[str]]]]
+    variant: Optional[Var[VariantType]]
+    wrapper_col: Optional[Var[Dict]]
+
+    @classmethod
+    def create(cls, *children, **props) -> Component:
+        if 'form' in props and isinstance(props['form'], str):
+            props['form'] = Var.create_safe(f'{props["form"]}', _var_is_local=False)
+        rs = super().create(*children, **props)
+        # form and form.item can not split, if split some components like select don't work;
+        rs._memoization_mode = MemoizationMode()
+        rs._memoization_mode.disposition = MemoizationDisposition.NEVER
+        rs._memoization_mode.recursive = False
+        return rs
+
+    def _get_hooks(self) -> str | None:
+        if hasattr(self, 'form') and self.form is not None:
+            return f"const [{str(self.form).strip('{}')}] = Form.useForm();"
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_fields_change": lambda changed, all: [changed],
+            'on_finish': lambda values: [values],
+            "on_finish_failed": lambda ev: [ev.values, ev.errorFields, ev.outOfDate],
+            "on_values_change": lambda changed, all: [changed, all],
+        })
+        return _triggers
+
+
+class FormItem(AntdComponent):
+    tag = 'Form.Item'
+
+    colon: Optional[Var[bool]]
+    dependencies: Optional[Var[List[Union[str, int, List[Union[str, int]]]]]]
+    extra: Optional[Var[ReactNode]]
+    getValue_from_event: Optional[Var[JsValue]]
+    get_value_props: Optional[Var[JsValue]]
+    has_feedback: Optional[Var[Union[bool, ContainVar]]]
+    help: Optional[Var[ReactNode]]
+    hidden: Optional[Var[bool]]
+    html_for: Optional[Var[str]]
+    initial_value: Optional[Var[str]]
+    label: Optional[Var[str]]
+    label_align: Optional[Var[AlignType]]
+    label_col: Optional[Var[Dict]]
+    message_variables: Optional[Var[JsValue]]
+    name: Optional[Var[Union[str, int, List[Union[str, int]]]]]
+    normalize: Optional[Var[JsValue]]
+    no_style: Optional[Var[bool]]
+    preserve: Optional[Var[bool]]
+    required: Optional[Var[bool]]
+    rules: Optional[Var[Union[List[Dict], ContainVar]]]
+    should_update: Optional[Var[bool]]
+    tooltip: Optional[Var[Union[Component, ContainVar]]]
+    trigger: Optional[Var[str]]
+    validate_debounce: Optional[Var[float]]
+    validate_first: Optional[Var[Union[bool, str]]]
+    validate_status: Optional[Var[str]]
+    validate_trigger: Optional[Var[Union[str, List[str]]]]
+    value_prop_name: Optional[Var[str]]
+    wrapper_col: Optional[Var[Dict]]
+
+    rules: Optional[Var[List[Dict]]]
+
+
+class FormList(AntdComponent):
+    tag = 'Form.List'
+
+    # children: Optional[Var[JsValue]]
+    initial_value: Optional[Var[List]]
+    name: Optional[Var[Union[str, int, List[Union[str, int]]]]]
+    rules: Optional[Var[ContainVar]]
+
+
+class FormProvider(AntdComponent):
+    tag = 'Form.Provider'
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "on_form_change": lambda form_name, info: [form_name, info],
+            'on_form_finish': lambda form_name, info: [form_name, info],
+        })
+        return _triggers
+
+
+form = Form.create
+form_item = FormItem.create
+form_list = FormList.create
+form_provider = FormProvider.create
+
+
+def _modal_form(modal_type: str, *children, modal_config=None, form_id: str = None, **props) -> JsValue | Component:
+    from . import modal
+    if form_id is None:
+        form_id = f'form_{uuid.uuid4().hex}'
+    props.update(
+        form=form_id,
+        preserve=False,
+    )
+    f = form(*children, **props)
+
+    modal_config = modal_config or {}
+    modal_config.update(destroy_on_close=True)
+    modal_config['on_ok'] = js_value(f"""() => {{
+        return new Promise((resolve, reject) => {{
+    {form_id}
+      .validateFields({{
+        validateOnly: false,
+      }})
+      .then(() => {{
+        {form_id}.submit();
+      resolve()}})
+      .catch(() => {{
+      reject()}});
+      }});//if catch, modal will close the form //.catch(() => console.log('Oops errors!'));
+      }}
+    """)
+    op = getattr(modal, modal_type)
+    if modal_type == 'confirm':
+        modal_config['content'] = f
+        return op(config=modal_config)
+    else:
+        modal_config['after_open_change'] = js_value(f"""(open) => {{{form_id}.resetFields()}}""")
+        modal = op(
+            f,
+            # on_open=JsValue(f'{form_id}.resetFields()'),
+            **modal_config)
+        return modal
+
+
+def modal_form(*children, modal_config=None, form_id: str = None, **props) -> Component:
+    return _modal_form('modal',
+                       *children, modal_config=modal_config, form_id=form_id, **props)
+
+
+def confirm_form(*children, confirm_config=None, form_id: str = None, **props) -> JsValue:
+    return _modal_form('confirm',
+                       *children, modal_config=confirm_config, form_id=form_id, **props)
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/form.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/grid.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/grid.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import Optional, Union, Dict
-
-from reflex import Component, Var
-from reflex.utils import imports
-
-from ..base import AntdComponent, ContainVar
-from ..constant import OrientationType, DirectionType
-
-
-class Row(AntdComponent):
-    tag = 'Row'
-
-    align: Optional[Var[str]]
-    gutter: Optional[Var[Union[int, ContainVar]]]
-    justify: Optional[Var[str]]
-    wrap: Optional[Var[str]]
-
-
-class Col(AntdComponent):
-    tag = 'Col'
-
-    flex: Optional[Var[Union[str, int]]]
-    offset: Optional[Var[int]]
-    order: Optional[Var[int]]
-    pull: Optional[Var[int]]
-    push: Optional[Var[int]]
-    span: Optional[Var[int]]
-
-    xs: Optional[Var[Union[int, Dict]]]
-    sm: Optional[Var[Union[int, Dict]]]
-    md: Optional[Var[Union[int, Dict]]]
-    lg: Optional[Var[Union[int, Dict]]]
-    xl: Optional[Var[Union[int, Dict]]]
-    xxl: Optional[Var[Union[int, Dict]]]
-
-
-row = Row.create
-col = Col.create
+from typing import Optional, Union, Dict
+
+from reflex import Component, Var
+from reflex.utils import imports
+
+from ..base import AntdComponent, ContainVar
+from ..constant import OrientationType, DirectionType
+
+
+class Row(AntdComponent):
+    tag = 'Row'
+
+    align: Optional[Var[str]]
+    gutter: Optional[Var[Union[int, ContainVar]]]
+    justify: Optional[Var[str]]
+    wrap: Optional[Var[str]]
+
+
+class Col(AntdComponent):
+    tag = 'Col'
+
+    flex: Optional[Var[Union[str, int]]]
+    offset: Optional[Var[int]]
+    order: Optional[Var[int]]
+    pull: Optional[Var[int]]
+    push: Optional[Var[int]]
+    span: Optional[Var[int]]
+
+    xs: Optional[Var[Union[int, Dict]]]
+    sm: Optional[Var[Union[int, Dict]]]
+    md: Optional[Var[Union[int, Dict]]]
+    lg: Optional[Var[Union[int, Dict]]]
+    xl: Optional[Var[Union[int, Dict]]]
+    xxl: Optional[Var[Union[int, Dict]]]
+
+
+row = Row.create
+col = Col.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/grid.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/icon.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/icon.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from typing import Optional
-
-from reflex import Component, Var
-from reflex.utils import format
-
-from ..base import VarDataMixin
-
-
-class BaseIconComponent(Component):
-    library = "@ant-design/icons"
-
-
-class IconComponent(BaseIconComponent):
-    tag = "None"
-
-    rotate: Optional[Var[int]]
-    spin: Optional[Var[bool]]
-    two_tone_color: Optional[Var[str]]
-
-    @classmethod
-    def create(cls, *children, **props) -> Component:
-        """Initialize the Icon component.
-        """
-        if children:
-            if len(children) == 1 and type(children[0]) == str:
-                props["tag"] = children[0]
-                children = []
-            else:
-                raise AttributeError(
-                    f"Passing multiple children to Icon component is not allowed: remove positional arguments {children[1:]} to fix"
-                )
-        if "tag" not in props.keys():
-            raise AttributeError("Missing 'tag' keyword-argument for Icon")
-
-        # if (
-        #     type(props["tag"]) != str
-        #     or format.to_snake_case(props["tag"]) not in LUCIDE_ICON_LIST
-        # ):
-        #     raise ValueError(
-        #         f"Invalid icon tag: {props['tag']}. Please use one of the following: {', '.join(LUCIDE_ICON_LIST[0:25])}, ..."
-        #         "\nSee full list at https://lucide.dev/icons."
-        #     )
-
-        # props["tag"] = format.to_title_case(format.to_snake_case(props["tag"]))
-        # props["alias"] = f"antd{props['tag']}"
-        return super().create(*children, **props)
-
-
-icon = IconComponent.create
-
-
-# class CustomerServiceOutlined(BaseIconComponent):
-#     tag = 'CustomerServiceOutlined'
-#
-#
-# class CommentOutlined(BaseIconComponent):
-#     tag = 'CommentOutlined'
-#
-#
-# class QuestionCircleOutlined(BaseIconComponent):
-#     tag = 'QuestionCircleOutlined'
-#
-#
-# class LaptopOutlined(BaseIconComponent):
-#     tag = 'LaptopOutlined'
-#
-#
-# class NotificationOutlined(BaseIconComponent):
-#     tag = 'NotificationOutlined'
-#
-#
-# class CloseCircleOutlined(BaseIconComponent):
-#     tag = 'CloseCircleOutlined'
-#
-#
-# class CloseSquareOutlined(BaseIconComponent):
-#     tag = 'CloseSquareOutlined'
-#
-#
-# class UserOutlined(BaseIconComponent):
-#     tag = 'UserOutlined'
+from typing import Optional
+
+from reflex import Component, Var
+from reflex.utils import format
+
+from ..base import VarDataMixin
+
+
+class BaseIconComponent(Component):
+    library = "@ant-design/icons"
+
+
+class IconComponent(BaseIconComponent):
+    tag = "None"
+
+    rotate: Optional[Var[int]]
+    spin: Optional[Var[bool]]
+    two_tone_color: Optional[Var[str]]
+
+    @classmethod
+    def create(cls, *children, **props) -> Component:
+        """Initialize the Icon component.
+        """
+        if children:
+            if len(children) == 1 and type(children[0]) == str:
+                props["tag"] = children[0]
+                children = []
+            else:
+                raise AttributeError(
+                    f"Passing multiple children to Icon component is not allowed: remove positional arguments {children[1:]} to fix"
+                )
+        if "tag" not in props.keys():
+            raise AttributeError("Missing 'tag' keyword-argument for Icon")
+
+        # if (
+        #     type(props["tag"]) != str
+        #     or format.to_snake_case(props["tag"]) not in LUCIDE_ICON_LIST
+        # ):
+        #     raise ValueError(
+        #         f"Invalid icon tag: {props['tag']}. Please use one of the following: {', '.join(LUCIDE_ICON_LIST[0:25])}, ..."
+        #         "\nSee full list at https://lucide.dev/icons."
+        #     )
+
+        # props["tag"] = format.to_title_case(format.to_snake_case(props["tag"]))
+        # props["alias"] = f"antd{props['tag']}"
+        return super().create(*children, **props)
+
+
+icon = IconComponent.create
+
+
+# class CustomerServiceOutlined(BaseIconComponent):
+#     tag = 'CustomerServiceOutlined'
+#
+#
+# class CommentOutlined(BaseIconComponent):
+#     tag = 'CommentOutlined'
+#
+#
+# class QuestionCircleOutlined(BaseIconComponent):
+#     tag = 'QuestionCircleOutlined'
+#
+#
+# class LaptopOutlined(BaseIconComponent):
+#     tag = 'LaptopOutlined'
+#
+#
+# class NotificationOutlined(BaseIconComponent):
+#     tag = 'NotificationOutlined'
+#
+#
+# class CloseCircleOutlined(BaseIconComponent):
+#     tag = 'CloseCircleOutlined'
+#
+#
+# class CloseSquareOutlined(BaseIconComponent):
+#     tag = 'CloseSquareOutlined'
+#
+#
+# class UserOutlined(BaseIconComponent):
+#     tag = 'UserOutlined'
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/icon.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/image.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/image.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-
-
-class Image(AntdComponent):
-    tag = 'Image'
-
-    alt: Optional[Var[str]]
-    fallback: Optional[Var[str]]
-    height: Optional[Var[Union[str, int]]]
-    placeholder: Optional[Var[ReactNode]]
-    description: Optional[Var[ReactNode]]
-    preview: Optional[Var[Union[bool, dict]]]
-    src: Optional[Var[str]]
-    width: Optional[Var[Union[str, int]]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            "on_error": lambda event: [],
-        })
-        return _triggers
-
-
-class ImagePreviewGroup(AntdComponent):
-    tag = 'Image.PreviewGroup'
-
-    preview: Optional[Var[Union[bool, Component]]]
-    items: Optional[Var[list]]
-    fallback: Optional[Var[str]]
-
-
-image = Image.create
-image_preview_group = ImagePreviewGroup.create
+from typing import Optional, Union, Dict, Any, List
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+
+
+class Image(AntdComponent):
+    tag = 'Image'
+
+    alt: Optional[Var[str]]
+    fallback: Optional[Var[str]]
+    height: Optional[Var[Union[str, int]]]
+    placeholder: Optional[Var[ReactNode]]
+    description: Optional[Var[ReactNode]]
+    preview: Optional[Var[Union[bool, dict]]]
+    src: Optional[Var[str]]
+    width: Optional[Var[Union[str, int]]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        _triggers.update({
+            "on_error": lambda event: [],
+        })
+        return _triggers
+
+
+class ImagePreviewGroup(AntdComponent):
+    tag = 'Image.PreviewGroup'
+
+    preview: Optional[Var[Union[bool, Component]]]
+    items: Optional[Var[list]]
+    fallback: Optional[Var[str]]
+
+
+image = Image.create
+image_preview_group = ImagePreviewGroup.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/image.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/input.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/input.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from typing import Optional, Union, Dict, Any
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType, SizeType, VariantType
-
-
-class Input(AntdComponent):
-    tag = "Input"
-
-    addon_after: Optional[Var[ReactNode]]
-    addon_before: Optional[Var[ReactNode]]
-    allow_clear: Optional[Var[Union[bool, ContainVar]]]
-    count: Optional[Var[Union[Dict, ContainVar]]]
-    default_value: Optional[Var[str]]
-    disabled: Optional[Var[bool]]
-    id: Optional[Var[str]]
-    max_length: Optional[Var[int]]
-    prefix: Optional[Var[ReactNode]]
-    show_count: Optional[Var[Union[bool, JsValue]]]
-    status: Optional[Var[StatusType]]
-    size: Optional[Var[SizeType]]
-    suffix: Optional[Var[ReactNode]]
-    type: Optional[Var[str]]
-    value: Optional[Var[str]]
-    variant: Optional[Var[VariantType]]
-    placeholder: Optional[Var[str]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda e: [e],
-            'on_press_enter': lambda e: [e],
-        })
-        return _triggers
-
-
-class TextArea(Input):
-    tag = "Input.TextArea"
-
-    auto_size: Optional[Var[Union[bool, Dict]]]
-
-
-class Search(Input):
-    tag = 'Input.Search'
-
-    enter_button: Optional[Var[ReactNode]]
-    loading: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_search': lambda value, event, info: [value],
-        })
-        return _triggers
-
-
-class Password(Input):
-    tag = 'Input.Password'
-
-    icon_render: Optional[Var[JsValue]]
-    visibility_toggle: Optional[Var[Union[bool, ContainVar]]]
-
-
-input = Input.create  # noqa
-text_area = TextArea.create
-search = Search.create
-password = Password.create
-
-
-
+from typing import Optional, Union, Dict, Any
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, VariantType
+
+
+class Input(AntdComponent):
+    tag = "Input"
+
+    addon_after: Optional[Var[ReactNode]]
+    addon_before: Optional[Var[ReactNode]]
+    allow_clear: Optional[Var[Union[bool, ContainVar]]]
+    count: Optional[Var[Union[Dict, ContainVar]]]
+    default_value: Optional[Var[str]]
+    disabled: Optional[Var[bool]]
+    id: Optional[Var[str]]
+    max_length: Optional[Var[int]]
+    prefix: Optional[Var[ReactNode]]
+    show_count: Optional[Var[Union[bool, JsValue]]]
+    status: Optional[Var[StatusType]]
+    size: Optional[Var[SizeType]]
+    suffix: Optional[Var[ReactNode]]
+    type: Optional[Var[str]]
+    value: Optional[Var[str]]
+    variant: Optional[Var[VariantType]]
+    placeholder: Optional[Var[str]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda e: [e],
+            'on_press_enter': lambda e: [e],
+        })
+        return _triggers
+
+
+class TextArea(Input):
+    tag = "Input.TextArea"
+
+    auto_size: Optional[Var[Union[bool, Dict]]]
+
+
+class Search(Input):
+    tag = 'Input.Search'
+
+    enter_button: Optional[Var[ReactNode]]
+    loading: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            'on_search': lambda value, event, info: [value],
+        })
+        return _triggers
+
+
+class Password(Input):
+    tag = 'Input.Password'
+
+    icon_render: Optional[Var[JsValue]]
+    visibility_toggle: Optional[Var[Union[bool, ContainVar]]]
+
+
+input = Input.create  # noqa
+text_area = TextArea.create
+search = Search.create
+password = Password.create
+
+
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/input.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/input.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/input_number.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/upload.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from typing import Optional, Union, Dict, Any
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType, SizeType, VariantType
-
-
-class InputNumber(AntdComponent):
-    tag = "InputNumber"
-
-    addon_after: Optional[Var[ReactNode]]
-    addon_before: Optional[Var[ReactNode]]
-    auto_focus: Optional[Var[bool]]
-    change_on_blur: Optional[Var[bool]]
-    change_on_wheel: Optional[Var[bool]]
-    controls: Optional[Var[Union[bool, ContainVar]]]
-    decimal_separator: Optional[Var[str]]
-    placeholder: Optional[Var[str]]
-    default_value: Optional[Var[int]]
-    disabled: Optional[Var[bool]]
-    formatter: Optional[Var[JsValue]]
-    keyboard: Optional[Var[bool]]
-    max: Optional[Var[int]]
-    min: Optional[Var[int]]
-    parser: Optional[Var[JsValue]]
-    precision: Optional[Var[int]]
-    read_only: Optional[Var[bool]]
-    status: Optional[Var[StatusType]]
-    prefix: Optional[Var[ReactNode]]
-    size: Optional[Var[SizeType]]
-    step: Optional[Var[Union[int, str]]]
-    string_mode: Optional[Var[bool]]
-    value: Optional[Var[int]]
-    variant: Optional[Var[VariantType]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda value: [value],
-            'on_press_enter': lambda e: [e],
-            "on_step": lambda value, info: [value, info],
-        })
-        return _triggers
-
-
-input_number = InputNumber.create
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+
+
+class Upload(AntdComponent):
+    tag = 'Upload'
+
+    accept: Optional[Var[str]]
+    action: Optional[Var[Union[str, JsValue]]]
+    before_upload: Optional[Var[JsValue]]
+    custom_request: Optional[Var[JsValue]]
+    data: Optional[Var[Union[ContainVar, JsValue]]]
+    default_file_list: Optional[Var[List[ContainVar]]]
+    directory: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    file_list: Optional[Var[List[ContainVar]]]
+    headers: Optional[Var[Dict]]
+    icon_render: Optional[Var[JsValue]]
+    is_image_url: Optional[Var[JsValue]]
+    list_type: Optional[Var[str]]
+    max_count: Optional[Var[int]]
+    method: Optional[Var[str]]
+    multiple: Optional[Var[bool]]
+    name: Optional[Var[str]]
+    open_file_dialog_on_click: Optional[Var[bool]]
+    preview_file: Optional[Var[JsValue]]
+    progress: Optional[Var[Dict]]
+    show_upload_list: Optional[Var[Union[bool, Dict]]]
+    with_credentials: Optional[Var[Union[bool]]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda file, file_list: [file, file_list],
+            "on_drop": lambda event: [event],
+            "on_download": lambda file: [file],
+            "on_preview": lambda file: [file],
+            "on_remove": lambda file: [file]
+        })
+        return _triggers
+
+
+upload = Upload.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/input_number.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/input_number.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/layout.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/layout.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, AntdSubComponent, ReactNode, ContainVar
-from ..constant import BreakpointType, ThemeType
-
-
-class LayoutBase(AntdComponent):
-    pass
-
-
-class Layout(LayoutBase):
-    tag = 'Layout'
-
-    has_sider: Optional[Var[bool]]
-
-    # def _get_custom_code(self) -> str | None:
-    #     return """
-    #     const { Header, Content, Footer, Sider } = Layout;
-    #     """
-
-
-class SubLayout(AntdComponent):
-    width: Optional[Var[Union[int, str]]]
-
-
-class Header(SubLayout):
-    tag = 'Layout.Header'
-
-
-class Content(SubLayout):
-    tag = 'Layout.Content'
-
-
-class Footer(SubLayout):
-    tag = 'Layout.Footer'
-
-
-class Sider(SubLayout):
-    tag = 'Layout.Sider'
-
-    breakpoint: Optional[Var[Union[BreakpointType, Dict]]]
-    collapsed: Optional[Var[bool]]
-    collapsed_width: Optional[Var[int]]
-    collapsible: Optional[Var[bool]]
-    default_collapsed: Optional[Var[bool]]
-    reverse_arrow: Optional[Var[bool]]
-    theme: Optional[Var[ThemeType]]
-    trigger: Optional[Var[ReactNode]]
-    zero_width_trigger_style: Optional[Var[Union[Dict, ContainVar]]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_breakpoint': lambda broken: [broken],
-            'on_collapse': lambda collapsed, type: [collapsed, type],
-        })
-        return _triggers
-
-
-layout = Layout.create
-header = Header.create
-content = Content.create
-footer = Footer.create
-sider = Sider.create
-
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ReactNode, ContainVar
+from ..constant import BreakpointType, ThemeType
+
+
+class LayoutBase(AntdComponent):
+    pass
+
+
+class Layout(LayoutBase):
+    tag = 'Layout'
+
+    has_sider: Optional[Var[bool]]
+
+    # def _get_custom_code(self) -> str | None:
+    #     return """
+    #     const { Header, Content, Footer, Sider } = Layout;
+    #     """
+
+
+class SubLayout(AntdComponent):
+    width: Optional[Var[Union[int, str]]]
+
+
+class Header(SubLayout):
+    tag = 'Layout.Header'
+
+
+class Content(SubLayout):
+    tag = 'Layout.Content'
+
+
+class Footer(SubLayout):
+    tag = 'Layout.Footer'
+
+
+class Sider(SubLayout):
+    tag = 'Layout.Sider'
+
+    breakpoint: Optional[Var[Union[BreakpointType, Dict]]]
+    collapsed: Optional[Var[bool]]
+    collapsed_width: Optional[Var[int]]
+    collapsible: Optional[Var[bool]]
+    default_collapsed: Optional[Var[bool]]
+    reverse_arrow: Optional[Var[bool]]
+    theme: Optional[Var[ThemeType]]
+    trigger: Optional[Var[ReactNode]]
+    zero_width_trigger_style: Optional[Var[Union[Dict, ContainVar]]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            'on_breakpoint': lambda broken: [broken],
+            'on_collapse': lambda collapsed, type: [collapsed, type],
+        })
+        return _triggers
+
+
+layout = Layout.create
+header = Header.create
+content = Content.create
+footer = Footer.create
+sider = Sider.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/layout.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/layout.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/list.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/mentions.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/mentions.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType, SizeType, VariantType, PlacementType
-
-
-class Mention(AntdComponent):
-    tag = 'Mention'
-
-    allow_clear: Optional[Var[Union[bool, ContainVar]]]
-    auto_focus: Optional[Var[bool]]
-    auto_size: Optional[Var[Union[bool, Dict]]]
-    default_value: Optional[Var[str]]
-    filter_option: Optional[Var[Union[bool, JsValue]]]
-    get_popup_container: Optional[Var[JsValue]]
-    not_found_content: Optional[Var[ReactNode]]
-    placement: Optional[Var[PlacementType]]
-    prefix: Optional[Var[Union[str, List[str]]]]
-    split: Optional[Var[str]]
-    status: Optional[Var[StatusType]]
-    validate_search: Optional[Var[JsValue]]
-    value: Optional[Var[str]]
-    variant: Optional[Var[VariantType]]
-    options: Optional[Var[ContainVar]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda text: [text],
-            "on_resize": lambda ev: [ev],
-            'on_search': lambda text, prefix: [text, prefix],
-            "on_select": lambda option, prefix: [option, prefix],
-        })
-        return _triggers
-
-
-mention = Mention.create
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, VariantType, PlacementType
+
+
+class Mention(AntdComponent):
+    tag = 'Mention'
+
+    allow_clear: Optional[Var[Union[bool, ContainVar]]]
+    auto_focus: Optional[Var[bool]]
+    auto_size: Optional[Var[Union[bool, Dict]]]
+    default_value: Optional[Var[str]]
+    filter_option: Optional[Var[Union[bool, JsValue]]]
+    get_popup_container: Optional[Var[JsValue]]
+    not_found_content: Optional[Var[ReactNode]]
+    placement: Optional[Var[PlacementType]]
+    prefix: Optional[Var[Union[str, List[str]]]]
+    split: Optional[Var[str]]
+    status: Optional[Var[StatusType]]
+    validate_search: Optional[Var[JsValue]]
+    value: Optional[Var[str]]
+    variant: Optional[Var[VariantType]]
+    options: Optional[Var[ContainVar]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda text: [text],
+            "on_resize": lambda ev: [ev],
+            'on_search': lambda text, prefix: [text, prefix],
+            "on_select": lambda option, prefix: [option, prefix],
+        })
+        return _triggers
+
+
+mention = Mention.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/mentions.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/mentions.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/menu.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/menu.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,69 @@
-from typing import Optional, Union, Type, Dict, List, Any, Iterator
-from reflex.base import pydantic
-from reflex import Component, Var, EventChain, Base
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, AntdSubComponent, ContainVar, ReactNode
-from ..constant import ThemeType, DirectionType, TriggerType
-
-
-class MenuItem(pydantic.BaseModel):
-    key: str
-    label: str
-    icon: Component
-    children: Optional[List["MenuItem"]] = None
-
-
-# class MenuItems(ContainVar):
-#     pass
-
-class OnSelectEvent(Base):
-    item: Any
-    key: Any
-    keyPath: Any
-    selectedKeys: List[str]
-
-
-class Menu(AntdComponent):
-    tag = 'Menu'
-
-    default_open_keys: Optional[Var[List[str]]]
-    default_selected_keys: Optional[Var[List[str]]]
-    expand_icon: Optional[Var[ReactNode]]
-    force_sub_menu_render: Optional[Var[bool]]
-    inline_collapsed: Optional[Var[bool]]
-    inline_indent: Optional[Var[bool]]
-
-    items: Var[Union[ContainVar, list]]
-    mode: Optional[Var[DirectionType]]
-    multiple: Optional[Var[bool]]
-    open_keys: Optional[Var[List[str]]]
-    overflowed_indicator: Optional[Var[ReactNode]]
-    selectable: Optional[Var[bool]]
-    selected_keys: Optional[Var[List[str]]]
-    sub_menu_close_delay: Optional[Var[float]]
-    sub_menu_open_delay: Optional[Var[float]]
-
-    theme: Optional[Var[ThemeType]]
-    trigger_sub_menu_action: Optional[Var[TriggerType]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        def _on_select(ev: OnSelectEvent):
-            return [ev.selectedKeys]
-
-        def _on_click(ev: OnSelectEvent):
-            return [ev.key, ev.keyPath]
-
-        _triggers.update({
-            EventTriggers.ON_OPEN_CHANGE: lambda open_keys: [open_keys],
-            EventTriggers.ON_SELECT: _on_select,
-            EventTriggers.ON_CLICK: _on_click,
-            'on_deselect': _on_click,
-        })
-        return _triggers
-
-
-menu = Menu.create
-# menu_items = ContainVar.create
+from typing import Optional, Union, Type, Dict, List, Any, Iterator
+from reflex import Component, Var, EventChain, Base
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, ReactNode, pydantic
+from ..constant import ThemeType, DirectionType, TriggerType
+
+
+class MenuItem(pydantic.BaseModel):
+    key: str
+    label: str
+    icon: Component
+    children: Optional[List["MenuItem"]] = None
+
+
+# class MenuItems(ContainVar):
+#     pass
+
+class OnSelectEvent(Base):
+    item: Any
+    key: Any
+    keyPath: Any
+    selectedKeys: List[str]
+
+
+class Menu(AntdComponent):
+    tag = 'Menu'
+
+    default_open_keys: Optional[Var[List[str]]]
+    default_selected_keys: Optional[Var[List[str]]]
+    expand_icon: Optional[Var[ReactNode]]
+    force_sub_menu_render: Optional[Var[bool]]
+    inline_collapsed: Optional[Var[bool]]
+    inline_indent: Optional[Var[bool]]
+
+    items: Var[Union[ContainVar, list]]
+    mode: Optional[Var[DirectionType]]
+    multiple: Optional[Var[bool]]
+    open_keys: Optional[Var[List[str]]]
+    overflowed_indicator: Optional[Var[ReactNode]]
+    selectable: Optional[Var[bool]]
+    selected_keys: Optional[Var[List[str]]]
+    sub_menu_close_delay: Optional[Var[float]]
+    sub_menu_open_delay: Optional[Var[float]]
+
+    theme: Optional[Var[ThemeType]]
+    trigger_sub_menu_action: Optional[Var[TriggerType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        def _on_select(ev: OnSelectEvent):
+            return [ev.selectedKeys]
+
+        def _on_click(ev: OnSelectEvent):
+            return [ev.key, ev.keyPath]
+
+        _triggers.update({
+            EventTriggers.ON_OPEN_CHANGE: lambda open_keys: [open_keys],
+            EventTriggers.ON_SELECT: _on_select,
+            EventTriggers.ON_CLICK: _on_click,
+            'on_deselect': _on_click,
+        })
+        return _triggers
+
+
+menu = Menu.create
+# menu_items = ContainVar.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/menu.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/message.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/message.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-from typing import Optional, Union, Dict, Any, List, Set, Iterator
-import uuid
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.components.base.bare import Bare
-from reflex.vars import BaseVar
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode, ExStateItem, version
-from ..constant import MessageType
-
-
-class Message(JsValue):
-    is_global: bool = True
-    class_name: Optional[Var[str]]
-    content: Optional[Var[ReactNode]]
-    duration: Optional[Var[Union[int, float]]]
-    icon: Optional[Var[ReactNode]]
-    key: Optional[Var[Union[str, int]]]
-    style: Optional[Var[dict]]
-    type: Optional[MessageType] = 'info'
-    config: Optional[Var[dict]]
-
-    top: Optional[Var[int]]
-    rtl: Optional[Var[bool]]
-    prefix_cls: Optional[Var[str]]
-    max_count: Optional[Var[int]]
-
-    @property
-    def config_item(self) -> Optional[ExStateItem]:
-        if not hasattr(self, 'config') or self.config is None:
-            return None
-        try:
-            return self._config_item
-        except AttributeError:
-            self._config_item = ExStateItem(self.config, self)
-            return self._config_item
-
-    @property
-    def uid(self) -> str:
-        try:
-            return self._uid
-        except AttributeError:
-            self._uid = uuid.uuid4().hex
-            return self._uid
-
-    def get_open_message(self) -> str:
-        return f'openMessage_{self.uid}'
-
-    def get_imports(self) -> imports.ImportDict:
-        _imports = {
-            "antd": [imports.ImportVar(tag='message')],
-            "react": [imports.ImportVar(tag="useEffect")],
-        }
-        return _imports
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        if self.config_item is not None:
-            open_func = """const %(name)s = () => {
-                           %(mn)s.open(%(cfg)s);
-                       };""" % dict(
-                name=self.get_open_message(),
-                mn='messageApi' if not self.is_global else 'message',
-                cfg=self.config_item.serialize(),
-            )
-        else:
-            key_s = f'{self.key},' if hasattr(self, 'key') else ''
-            duration_s = f'duration: {self.duration},' if hasattr(self, 'duration') else ''
-            top_s = f'top: {self.top},' if hasattr(self, 'top') else ''
-
-            open_func = """
-            const %(name)s = () => {
-                %(mn)s.open({
-                  %(key)s
-                  type: '%(type)s',
-                  content: '%(content)s',
-                  %(duration)s %(top)s
-                });
-            };
-            """ % dict(
-                name=self.get_open_message(),
-                mn='messageApi' if not self.is_global else 'message',
-                key=key_s, type=self.type, content=self.content,
-                duration=duration_s,
-                top=top_s,
-            )
-        others = []
-        if self.config_item:
-            others.extend([
-                *self.config_item.get_hooks(),
-                """useEffect(() => {
-    if (%(state)s === null) {messageApi.destroy(); return;}
-    %(name)s(%(state)s);
-}, [%(state)s]); """ % dict(
-                    state=self.config_item.serialize(),
-                    name=self.get_open_message(),
-                ),
-            ])
-
-        _hooks = []
-        if self.is_global:
-            _hooks.extend([
-                open_func
-            ])
-        else:
-            _hooks.extend([
-                """const [messageApi, contextHolder] = message.useMessage();""",
-                open_func,
-                *others,
-            ])
-        if version <= '000.004.006':
-            return set(_hooks)
-        return dict((h, None) for h in _hooks)
-
-    def serialize(self) -> str:
-        # if self.config_item is not None:
-        #     return '{contextHolder}'
-        return self.get_open_message()
-
-
-class MessageHolder(Bare):
-    msg: Optional[Message]
-
-    @classmethod
-    def create(cls, msg: Message) -> Component:
-        cs = ['<>']
-        if not msg.is_global:
-            cs.append('{contextHolder}')
-        cs.append('</>')
-        return cls(
-            msg=msg,
-            contents='\n'.join(cs),
-        )
-
-    def _get_vars(self, include_children: bool = False) -> Iterator[Var]:
-        yield self.contents
-        yield BaseVar(
-            _var_name='',
-            _var_is_local=True,
-            _var_data=self.msg.get_var_data(),
-        )
-
-
-message = Message
-message_holder = MessageHolder.create
-
-# def message_holder():
-#     return Var.create_safe('{contextHolder}')
+from typing import Optional, Union, Dict, Any, List, Set, Iterator
+import uuid
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.components.base.bare import Bare
+from reflex.vars import BaseVar
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode, ExStateItem, version
+from ..constant import MessageType
+from . import helper
+
+
+class Message(JsValue):
+    is_global: bool = True
+    class_name: Optional[Var[str]]
+    content: Optional[Var[ReactNode]]
+    duration: Optional[Var[Union[int, float]]]
+    icon: Optional[Var[ReactNode]]
+    key: Optional[Var[Union[str, int]]]
+    style: Optional[Var[dict]]
+    type: Optional[MessageType] = 'info'
+    config: Optional[Var[dict]]
+
+    top: Optional[Var[int]]
+    rtl: Optional[Var[bool]]
+    prefix_cls: Optional[Var[str]]
+    max_count: Optional[Var[int]]
+
+    @property
+    def config_item(self) -> Optional[ExStateItem]:
+        if not hasattr(self, 'config') or self.config is None:
+            return None
+        try:
+            return self._config_item
+        except AttributeError:
+            self._config_item = ExStateItem(self.config, self)
+            return self._config_item
+
+    @property
+    def uid(self) -> str:
+        try:
+            return self._uid
+        except AttributeError:
+            self._uid = uuid.uuid4().hex
+            return self._uid
+
+    def get_open_message(self) -> str:
+        return f'openMessage_{self.uid}'
+
+    def get_imports(self) -> imports.ImportDict:
+        _imports = {
+            "antd": [imports.ImportVar(tag='message')],
+            "react": [imports.ImportVar(tag="useEffect")],
+        }
+        return _imports
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        if self.config_item is not None:
+            open_func = """const %(name)s = () => {
+                           %(mn)s.open(%(cfg)s);
+                       };""" % dict(
+                name=self.get_open_message(),
+                mn='messageApi' if not self.is_global else 'message',
+                cfg=self.config_item.serialize(),
+            )
+        else:
+            key_s = f'{self.key},' if hasattr(self, 'key') else ''
+            duration_s = f'duration: {self.duration},' if hasattr(self, 'duration') else ''
+            top_s = f'top: {self.top},' if hasattr(self, 'top') else ''
+
+            open_func = """
+            const %(name)s = () => {
+                %(mn)s.open({
+                  %(key)s
+                  type: '%(type)s',
+                  content: '%(content)s',
+                  %(duration)s %(top)s
+                });
+            };
+            """ % dict(
+                name=self.get_open_message(),
+                mn='messageApi' if not self.is_global else 'message',
+                key=key_s, type=self.type, content=self.content,
+                duration=duration_s,
+                top=top_s,
+            )
+        others = []
+        if self.config_item:
+            state = self.config_item.serialize()
+            others.extend([
+                *self.config_item.get_hooks(),
+                helper.hook_state(
+                    state_field=state,
+                    on_update='%(name)s(%(state)s)' % dict(name=self.get_open_message(), state=state),
+                    on_null='messageApi.destroy()',
+                ),
+            ])
+
+        _hooks = []
+        if self.is_global:
+            _hooks.extend([
+                open_func
+            ])
+        else:
+            _hooks.extend([
+                """const [messageApi, contextHolder] = message.useMessage();""",
+                open_func,
+                *others,
+            ])
+        if version <= '000.004.006':
+            return set(_hooks)
+        return dict((h, None) for h in _hooks)
+
+    def serialize(self) -> str:
+        # if self.config_item is not None:
+        #     return '{contextHolder}'
+        return self.get_open_message()
+
+
+class MessageHolder(Bare):
+    msg: Optional[Message]
+
+    @classmethod
+    def create(cls, msg: Message) -> Component:
+        cs = ['<>']
+        if not msg.is_global:
+            cs.append('{contextHolder}')
+        cs.append('</>')
+        return cls(
+            msg=msg,
+            contents='\n'.join(cs),
+        )
+
+    def _get_vars(self, include_children: bool = False) -> Iterator[Var]:
+        yield self.contents
+        yield BaseVar(
+            _var_name='',
+            _var_is_local=True,
+            _var_data=self.msg.get_var_data(),
+        )
+
+
+message = Message
+message_holder = MessageHolder.create
+
+# def message_holder():
+#     return Var.create_safe('{contextHolder}')
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/message.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/message.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/modal.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/modal.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/notification.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/notification.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from typing import Optional, Union, Dict, Any, List, Set
-
-from reflex import Component, Var
-from reflex.utils import imports
-import uuid
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode, version
-from ..constant import PlacementType, RoleType
-
-
-class Notification(JsValue):
-    btn: Optional[Var[ReactNode]]
-    class_name: Optional[Var[str]]
-    close_icon: Optional[Var[ReactNode]]
-    description: Optional[Var[str]]
-    duration: Optional[Var[int]]
-    icon: Optional[Var[ReactNode]]
-    key: Optional[Var[str]]
-    message: Optional[Var[str]]
-    placement: Optional[Var[PlacementType]]
-    role: Optional[Var[RoleType]]
-    props: Optional[Var[Union[dict, ContainVar]]]
-
-    def get_imports(self) -> imports.ImportDict:
-        _imports = {
-            "antd": [imports.ImportVar(tag='notification')],
-        }
-        return _imports
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        open_func = """
-        const %(name)s = () => {
-          notification.open({
-            message: '%(message)s',
-            description:'%(description)s',
-            placement:'%(placement)s',
-            duration:'%(duration)s',
-          });
-        };
-        """ % dict(name=self.get_open_notification(), message=self.message, description=self.description,
-                   placement=self.placement, duration=self.duration)
-
-        _hooks = []
-        _hooks.extend([
-            """const [api, contextHolder] = notification.useNotification();""",
-            open_func,
-        ])
-        if version <= '000.004.006':
-            return set(_hooks)
-        return dict((h, None) for h in _hooks)
-
-    @property
-    def uid(self) -> str:
-        try:
-            return self._uid
-        except AttributeError:
-            self._uid = uuid.uuid4().hex
-            return self._uid
-
-    def get_open_notification(self) -> str:
-        return f'openNotification_{self.uid}'
-
-    def serialize(self) -> str:
-        return self.get_open_notification()
-
-
-notification = Notification
+from typing import Optional, Union, Dict, Any, List, Set
+
+from reflex import Component, Var
+from reflex.utils import imports
+import uuid
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode, version
+from ..constant import PlacementType, RoleType
+
+
+class Notification(JsValue):
+    btn: Optional[Var[ReactNode]]
+    class_name: Optional[Var[str]]
+    close_icon: Optional[Var[ReactNode]]
+    description: Optional[Var[str]]
+    duration: Optional[Var[int]]
+    icon: Optional[Var[ReactNode]]
+    key: Optional[Var[str]]
+    message: Optional[Var[str]]
+    placement: Optional[Var[PlacementType]]
+    role: Optional[Var[RoleType]]
+    props: Optional[Var[Union[dict, ContainVar]]]
+
+    def get_imports(self) -> imports.ImportDict:
+        _imports = {
+            "antd": [imports.ImportVar(tag='notification')],
+        }
+        return _imports
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        open_func = """
+        const %(name)s = () => {
+          notification.open({
+            message: '%(message)s',
+            description:'%(description)s',
+            placement:'%(placement)s',
+            duration:'%(duration)s',
+          });
+        };
+        """ % dict(name=self.get_open_notification(), message=self.message, description=self.description,
+                   placement=self.placement, duration=self.duration)
+
+        _hooks = []
+        _hooks.extend([
+            """const [api, contextHolder] = notification.useNotification();""",
+            open_func,
+        ])
+        if version <= '000.004.006':
+            return set(_hooks)
+        return dict((h, None) for h in _hooks)
+
+    @property
+    def uid(self) -> str:
+        try:
+            return self._uid
+        except AttributeError:
+            self._uid = uuid.uuid4().hex
+            return self._uid
+
+    def get_open_notification(self) -> str:
+        return f'openNotification_{self.uid}'
+
+    def serialize(self) -> str:
+        return self.get_open_notification()
+
+
+notification = Notification
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/pagination.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/pagination.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from typing import Optional, List, Dict, Any
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent
-
-
-class Pagination(AntdComponent):
-    tag = 'Pagination'
-
-    current: Optional[Var[int]]
-    default_current: Optional[Var[int]]
-    default_page_size: Optional[Var[int]]
-    disabled: Optional[Var[bool]]
-    hide_on_single_page: Optional[Var[bool]]
-    page_size: Optional[Var[int]]
-    page_size_options: Optional[Var[List[int]]]
-    responsive: Optional[Var[bool]]
-    show_less_items: Optional[Var[bool]]
-    show_quick_jumper: Optional[Var[bool]]
-    show_size_changer: Optional[Var[bool]]
-    show_title: Optional[Var[bool]]
-    # showTotal
-    simple: Optional[Var[bool]]
-    size: Optional[Var[int]]
-    total: Optional[Var[int]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda page, page_size: [page, page_size],
-            "show_total": lambda total,range: [total,range],
-        })
-        return _triggers
-
-
-pagination = Pagination.create
+from typing import Optional, List, Dict, Any
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent
+
+
+class Pagination(AntdComponent):
+    tag = 'Pagination'
+
+    current: Optional[Var[int]]
+    default_current: Optional[Var[int]]
+    default_page_size: Optional[Var[int]]
+    disabled: Optional[Var[bool]]
+    hide_on_single_page: Optional[Var[bool]]
+    page_size: Optional[Var[int]]
+    page_size_options: Optional[Var[List[int]]]
+    responsive: Optional[Var[bool]]
+    show_less_items: Optional[Var[bool]]
+    show_quick_jumper: Optional[Var[bool]]
+    show_size_changer: Optional[Var[bool]]
+    show_title: Optional[Var[bool]]
+    # showTotal
+    simple: Optional[Var[bool]]
+    size: Optional[Var[int]]
+    total: Optional[Var[int]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda page, page_size: [page, page_size],
+            "show_total": lambda total,range: [total,range],
+        })
+        return _triggers
+
+
+pagination = Pagination.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/pagination.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/pagination.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/popconfirm.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tooltip.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,42 @@
-from typing import Optional, Union, Dict, Any, List
-
-from reflex import Component, Var
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import TypeType
-
-class Popconfirm(AntdComponent):
-    tag = 'Popconfirm'
-
-    cancel_button_orops: Optional[Var[dict]]
-    cancel_text: Optional[Var[str]]
-    disabled: Optional[Var[bool]]
-    icon: Optional[Var[ReactNode]]
-    ok_button_props: Optional[Var[dict]]
-    ok_text: Optional[Var[str]]
-    ok_type: Optional[Var[TypeType]]
-    open: Optional[Var[bool]]
-    show_cancel: Optional[Var[bool]]
-    title: Optional[Var[ReactNode]]
-    description: Optional[Var[ReactNode]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_cancel": lambda e: [e],
-            "on_confirm": lambda e: [e],
-            "on_popup_click": lambda e: [e],
-        })
-        return _triggers
-
-
-popconfirm = Popconfirm.create
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import StatusType, PlacementType, TriggerType
+
+
+class Tooltip(AntdComponent):
+    tag = "Tooltip"
+
+    title: Optional[Var[Union[str, Component, JsValue]]]
+    align: Optional[Var[str]]
+    arrow: Optional[Var[Union[bool, Dict]]]
+    auto_adjust_overflow: Optional[Var[bool]]
+    color: Optional[Var[str]]
+    default_open: Optional[Var[bool]]
+    destroy_tooltip_on_hide: Optional[Var[bool]]
+    fresh: Optional[Var[bool]]
+    get_popup_container: Optional[Var[JsValue]]
+    mouse_enter_delay: Optional[Var[int]]
+    mouse_leave_delay: Optional[Var[int]]
+    overlay_class_name: Optional[Var[str]]
+    overlay_style: Optional[Var[Dict]]
+    overlay_inner_style: Optional[Var[Dict]]
+    placement: Optional[Var[PlacementType]]
+    trigger: Optional[Var[Union[TriggerType, List[TriggerType]]]]
+    open: Optional[Var[bool]]
+    z_index: Optional[Var[int]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
+        })
+        return _triggers
+
+
+tooltip = Tooltip.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/popconfirm.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/popconfirm.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/popover.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/progress.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/radio.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,46 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, ProgressType, SizeType, OrientationType
-
-
-class Progress(AntdComponent):
-    tag = 'Progress'
-
-    format: Optional[Var[JsValue]]
-    percent: Optional[Var[int]]
-    show_info: Optional[Var[bool]]
-    status: Optional[Var[StatusType]]
-    stroke_color: Optional[Var[str]]
-    stroke_linecap: Optional[Var[str]]
-    success: Optional[Var[Dict]]
-    trail_color: Optional[Var[str]]
-    type: Optional[Var[ProgressType]]
-    size: Optional[Var[Union[int, SizeType, List[Union[int, SizeType]]]]]
-    # type=...
-    steps: Optional[Var[Union[int, Dict]]]
-    stroke_color: Optional[Var[Union[str, List[str], Dict]]]
-    stroke_width: Optional[Var[int]]
-    # dashboard
-    gap_degree: Optional[Var[int]]
-    gap_position: Optional[Var[OrientationType]]
-
-
-progress = Progress.create
-
-
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import StatusType, SizeType, RadioStyleType, RadioType
+
+
+class Radio(AntdComponent):
+    tag = 'Radio'
+
+    auto_focus: Optional[Var[bool]]
+    checked: Optional[Var[bool]]
+    default_checked: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    value: Optional[Var[Any]]
+
+
+class RadioButton(Radio):
+    tag = 'Radio.Button'
+
+
+class RadioGroup(AntdComponent):
+    tag = 'Radio.Group'
+
+    button_style: Optional[Var[RadioStyleType]]
+    default_value: Optional[Var[Any]]
+    disabled: Optional[Var[bool]]
+    name: Optional[Var[str]]
+    options: Optional[Var[Union[List[Union[str, int]], ContainVar]]]
+    optionType: Optional[Var[RadioType]]
+    size: Optional[Var[SizeType]]
+    value: Optional[Var[Any]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda e: [e],
+        })
+        return _triggers
+
+
+radio = Radio.create
+radio_button = RadioButton.create
+radio_group = RadioGroup.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/progress.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/qrcode.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/qrcode.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/radio.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/color_picker.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, SizeType, RadioStyleType, RadioType
-
-
-class Radio(AntdComponent):
-    tag = 'Radio'
-
-    auto_focus: Optional[Var[bool]]
-    checked: Optional[Var[bool]]
-    default_checked: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    value: Optional[Var[Any]]
-
-
-class RadioButton(Radio):
-    tag = 'Radio.Button'
-
-
-class RadioGroup(AntdComponent):
-    tag = 'Radio.Group'
-
-    button_style: Optional[Var[RadioStyleType]]
-    default_value: Optional[Var[Any]]
-    disabled: Optional[Var[bool]]
-    name: Optional[Var[str]]
-    options: Optional[Var[Union[List[Union[str, int]], ContainVar]]]
-    optionType: Optional[Var[RadioType]]
-    size: Optional[Var[SizeType]]
-    value: Optional[Var[Any]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda e: [e],
-        })
-        return _triggers
-
-
-radio = Radio.create
-radio_button = RadioButton.create
-radio_group = RadioGroup.create
-
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue,ReactNode
+from ..constant import ColorFormatType, SizeType, PlacementType, TriggerType
+
+
+class ColorPicker(AntdComponent):
+    tag = 'ColorPicker'
+
+    allow_clear: Optional[Var[bool]]
+    arrow: Optional[Var[bool]]
+    default_value: Optional[Var[str]]
+    default_format: Optional[Var[str]]
+    disabled: Optional[Var[bool]]
+    disabled_alpha: Optional[Var[bool]]
+    destroy_tooltip_on_hide: Optional[Var[bool]]
+    format: Optional[Var[ColorFormatType]]
+    open: Optional[Var[bool]]
+    presets: Optional[Var[ContainVar]]
+    placement: Optional[Var[PlacementType]]
+    panel_render: Optional[Var[JsValue]]
+    show_text: Optional[Var[Union[bool, JsValue]]]
+    size: Optional[Var[SizeType]]
+    trigger: Optional[Var[TriggerType]]
+    value: Optional[Var[str]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda value, hex: [value, hex],
+            'on_change_complete': lambda value: [value],
+            'on_format_change': lambda format: [format],
+            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
+            'on_clear': lambda: [],
+        })
+        return _triggers
+
+
+color_picker = ColorPicker.create
+
+
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/radio.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/rate.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/rate.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/result.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/result.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/segmented.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tag.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,42 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import SizeType, PlacementType, TabsType
-
-
-class Segmented(AntdComponent):
-    tag = 'Segmented'
-
-    block: Optional[Var[bool]]
-    default_value: Optional[Var[Union[str, int]]]
-    disabled: Optional[Var[bool]]
-    options: Optional[Union[List[str], List[int], List[Dict]]]
-    size: Optional[Var[SizeType]]
-    value: Optional[Var[Union[str, int]]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda value: [value],
-        })
-        return _triggers
-
-
-segmented = Segmented.create
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import TimelineModeType
+
+
+class Tag(AntdComponent):
+    tag = 'Tag'
+
+    close_icon: Optional[Var[Union[bool, ReactNode]]]
+    color: Optional[Var[str]]
+    icon: Optional[Var[ReactNode]]
+    bordered: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            'on_close': lambda e: [e],
+        })
+        return _triggers
+
+
+class CheckableTag(AntdComponent):
+    tag = 'Tag.CheckableTag'
+
+    checked: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda checked: [checked],
+        })
+        return _triggers
+
+
+tag = Tag.create
+checkable_tag = CheckableTag.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/segmented.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/segmented.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/select.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/select.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
-
-
-class Select(AntdComponent):
-    tag = 'Select'
-
-    allow_clear: Optional[Var[bool]]
-    auto_clear_search_value: Optional[Var[bool]]
-    auto_focus: Optional[Var[bool]]
-    default_active_first_option: Optional[Var[bool]]
-    default_open: Optional[Var[bool]]
-    default_value: Optional[Var[Union[int, str, List[str], List[int], ContainVar]]]
-    disabled: Optional[Var[bool]]
-    popup_class_name: Optional[Var[str]]
-    popup_match_select_width: Optional[Var[Union[bool, int]]]
-    dropdown_render: Optional[Var[JsValue]]
-    dropdown_style: Optional[Var[Dict]]
-    field_names: Optional[Var[Dict]]
-    filter_option: Optional[Var[Union[bool, JsValue]]]
-    filter_sort: Optional[Var[JsValue]]
-    get_popup_container: Optional[Var[JsValue]]
-    label_in_value: Optional[Var[bool]]
-    list_height: Optional[Var[int]]
-    loading: Optional[Var[bool]]
-    max_count: Optional[Var[int]]
-    max_tag_count: Optional[Var[Union[int, str]]]
-    max_tag_placeholder: Optional[Var[Union[ReactNode, JsValue]]]
-    max_tag_text_length: Optional[Var[int]]
-    menu_item_selected_icon: Optional[Var[ReactNode]]
-    mode: Optional[Var[SelectModeType]]
-    not_found_content: Optional[Var[ReactNode]]
-    open: Optional[Var[bool]]
-    option_filter_prop: Optional[Var[str]]
-    option_label_prop: Optional[Var[str]]
-    options: Optional[Var[Union[list, ContainVar]]]
-    option_render: Optional[Var[JsValue]]
-    placeholder: Optional[Var[ReactNode]]
-    placement: Optional[Var[PlacementType]]
-    remove_icon: Optional[Var[ReactNode]]
-    search_value: Optional[Var[str]]
-    show_search: Optional[Var[bool]]
-    size: Optional[Var[SizeType]]
-    status: Optional[Var[StatusType]]
-    suffix_icon: Optional[Var[ReactNode]]
-    tag_render: Optional[Var[JsValue]]
-    label_render: Optional[Var[JsValue]]
-    token_separators: Optional[Var[List[str]]]
-    value: Optional[Var[Union[str, int, List[str], List[int], ContainVar]]]
-    variant: Optional[Var[VariantType]]
-    virtual: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda v, option: [v, option],
-            "on_clear": lambda: [],
-            "on_deselect": lambda v: [v],
-            "on_dropdown_visible_change": lambda open: [open],
-            "on_input_key_down": lambda: [],
-            "on_popup_scroll": lambda: [],
-            "on_search": lambda v: [v],
-            "on_select": lambda v, option: [v, option],
-        })
-        return _triggers
-
-
-select = Select.create
-
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
+
+
+class Select(AntdComponent):
+    tag = 'Select'
+
+    allow_clear: Optional[Var[bool]]
+    auto_clear_search_value: Optional[Var[bool]]
+    auto_focus: Optional[Var[bool]]
+    default_active_first_option: Optional[Var[bool]]
+    default_open: Optional[Var[bool]]
+    default_value: Optional[Var[Union[int, str, List[str], List[int], ContainVar]]]
+    disabled: Optional[Var[bool]]
+    popup_class_name: Optional[Var[str]]
+    popup_match_select_width: Optional[Var[Union[bool, int]]]
+    dropdown_render: Optional[Var[JsValue]]
+    dropdown_style: Optional[Var[Dict]]
+    field_names: Optional[Var[Dict]]
+    filter_option: Optional[Var[Union[bool, JsValue]]]
+    filter_sort: Optional[Var[JsValue]]
+    get_popup_container: Optional[Var[JsValue]]
+    label_in_value: Optional[Var[bool]]
+    list_height: Optional[Var[int]]
+    loading: Optional[Var[bool]]
+    max_count: Optional[Var[int]]
+    max_tag_count: Optional[Var[Union[int, str]]]
+    max_tag_placeholder: Optional[Var[Union[ReactNode, JsValue]]]
+    max_tag_text_length: Optional[Var[int]]
+    menu_item_selected_icon: Optional[Var[ReactNode]]
+    mode: Optional[Var[SelectModeType]]
+    not_found_content: Optional[Var[ReactNode]]
+    open: Optional[Var[bool]]
+    option_filter_prop: Optional[Var[str]]
+    option_label_prop: Optional[Var[str]]
+    options: Optional[Var[Union[list, ContainVar]]]
+    option_render: Optional[Var[JsValue]]
+    placeholder: Optional[Var[ReactNode]]
+    placement: Optional[Var[PlacementType]]
+    remove_icon: Optional[Var[ReactNode]]
+    search_value: Optional[Var[str]]
+    show_search: Optional[Var[bool]]
+    size: Optional[Var[SizeType]]
+    status: Optional[Var[StatusType]]
+    suffix_icon: Optional[Var[ReactNode]]
+    tag_render: Optional[Var[JsValue]]
+    label_render: Optional[Var[JsValue]]
+    token_separators: Optional[Var[List[str]]]
+    value: Optional[Var[Union[str, int, List[str], List[int], ContainVar]]]
+    variant: Optional[Var[VariantType]]
+    virtual: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda v, option: [v, option],
+            "on_clear": lambda: [],
+            "on_deselect": lambda v: [v],
+            "on_dropdown_visible_change": lambda open: [open],
+            "on_input_key_down": lambda: [],
+            "on_popup_scroll": lambda: [],
+            "on_search": lambda v: [v],
+            "on_select": lambda v, option: [v, option],
+        })
+        return _triggers
+
+
+select = Select.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/select.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/skeleton.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/skeleton.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import SizeType
-
-
-class Skeleton(AntdComponent):
-    tag = 'Skeleton'
-
-    active: Optional[Var[bool]]
-    avatar: Optional[Var[Union[bool, Dict]]]
-    loading: Optional[Var[bool]]
-    paragraph: Optional[Var[Union[bool, Dict]]]
-    round: Optional[Var[bool]]
-    title: Optional[Var[Union[bool, Dict]]]
-
-
-skeleton = Skeleton.create
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import SizeType
+
+
+class Skeleton(AntdComponent):
+    tag = 'Skeleton'
+
+    active: Optional[Var[bool]]
+    avatar: Optional[Var[Union[bool, Dict]]]
+    loading: Optional[Var[bool]]
+    paragraph: Optional[Var[Union[bool, Dict]]]
+    round: Optional[Var[bool]]
+    title: Optional[Var[Union[bool, Dict]]]
+
+
+skeleton = Skeleton.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/skeleton.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/slider.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/collapse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,31 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
-
-
-class Slider(AntdComponent):
-    tag = 'Slider'
-
-    auto_adjust_overflow: Optional[Var[bool]]
-    auto_focus: Optional[Var[bool]]
-    default_value: Optional[Var[Union[int, List[int]]]]
-    disabled: Optional[Var[bool]]
-    keyboard: Optional[Var[bool]]
-    dots: Optional[Var[bool]]
-    included: Optional[Var[bool]]
-    marks: Optional[Var[Union[Dict, ContainVar]]]
-    max: Optional[Var[int]]
-    min: Optional[Var[int]]
-    range: Optional[Var[bool]]
-    reverse: Optional[Var[bool]]
-    step: Optional[Var[int]]
-    tooltip: Optional[Var[Union[Dict, ContainVar]]]
-    value: Optional[Var[Union[int, List[int]]]]
-    vertical: Optional[Var[bool]]
-    # range
-    draggable_track: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            "on_change_complete": lambda v: [v],
-            EventTriggers.ON_CHANGE: lambda v: [v],
-        })
-        return _triggers
-
-
-slider = Slider.create
-
-
+from typing import Optional, Union, Dict, Any, List
+
+from reflex import Component, Var
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+
+
+class Collapse(AntdComponent):
+    tag = 'Collapse'
+
+    accordion: Optional[Var[bool]]
+    active_key: Optional[Var[Union[list[str], str, list[int], int]]]
+    bordered: Optional[Var[bool]]
+    default_active_key: Optional[Var[Union[list[str], str, list[int], int]]]
+    destroy_inactive_panel: Optional[Var[bool]]
+    expand_icon: Optional[Var[ReactNode]]
+    collapsible: Optional[Var[str]]
+    expand_icon_position: Optional[Var[str]]
+    ghost: Optional[Var[bool]]
+    size: Optional[Var[str]]
+    items: Optional[Var[Union[ContainVar, list]]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            'on_change': lambda: [],
+        })
+        return _triggers
+
+
+collapse = Collapse.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/slider.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/space.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/space.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from typing import Optional, Union, Dict
-
-from reflex import Component, Var
-from reflex.utils import imports
-
-from ..base import AntdComponent, ContainVar, ReactNode
-from ..constant import AlignType, DirectionType, SizeType
-
-
-class Space(AntdComponent):
-    tag = 'Space'
-
-    align: Optional[Var[AlignType]]
-    class_names: Optional[Var[Dict]]
-    direction: Optional[Var[DirectionType]]
-    size: Optional[Var[SizeType]]
-    split: Optional[Var[ReactNode]]
-    styles: Optional[Var[Dict]]
-    wrap: Optional[Var[bool]]
-
-
-class SpaceCompact(AntdComponent):
-    tag = 'Space.Compact'
-
-    block: Optional[Var[bool]]
-    direction: Optional[Var[DirectionType]]
-    size: Optional[Var[SizeType]]
-
-
-space = Space.create
-space_compact = SpaceCompact.create
-
+from typing import Optional, Union, Dict
+
+from reflex import Component, Var
+from reflex.utils import imports
+
+from ..base import AntdComponent, ContainVar, ReactNode
+from ..constant import AlignType, DirectionType, SizeType
+
+
+class Space(AntdComponent):
+    tag = 'Space'
+
+    align: Optional[Var[AlignType]]
+    class_names: Optional[Var[Dict]]
+    direction: Optional[Var[DirectionType]]
+    size: Optional[Var[SizeType]]
+    split: Optional[Var[ReactNode]]
+    styles: Optional[Var[Dict]]
+    wrap: Optional[Var[bool]]
+
+
+class SpaceCompact(AntdComponent):
+    tag = 'Space.Compact'
+
+    block: Optional[Var[bool]]
+    direction: Optional[Var[DirectionType]]
+    size: Optional[Var[SizeType]]
+
+
+space = Space.create
+space_compact = SpaceCompact.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/space.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/space.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/spin.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/spin.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/statistic.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/statistic.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/steps.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/steps.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import Optional, Union, Dict, Any
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import PlacementType, DirectionType, SizeType, StepsStatusType, StepsType
-
-
-class Steps(AntdComponent):
-    tag = 'Steps'
-
-    current: Optional[Var[int]]
-    direction: Optional[Var[DirectionType]]
-    initial: Optional[Var[int]]
-    label_placement: Optional[Var[DirectionType]]
-    percent: Optional[Var[int]]
-    progress_dot: Optional[Var[Union[bool, JsValue]]]
-    responsive: Optional[Var[bool]]
-    size: Optional[Var[SizeType]]
-    status: Optional[Var[StepsStatusType]]
-    type: Optional[Var[StepsType]]
-
-    items: Optional[Var[ContainVar]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda current: [current],
-        })
-        return _triggers
-
-
-steps = Steps.create
-
-
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import PlacementType, DirectionType, SizeType, StepsStatusType, StepsType
+
+
+class Steps(AntdComponent):
+    tag = 'Steps'
+
+    current: Optional[Var[int]]
+    direction: Optional[Var[DirectionType]]
+    initial: Optional[Var[int]]
+    label_placement: Optional[Var[DirectionType]]
+    percent: Optional[Var[int]]
+    progress_dot: Optional[Var[Union[bool, JsValue]]]
+    responsive: Optional[Var[bool]]
+    size: Optional[Var[SizeType]]
+    status: Optional[Var[StepsStatusType]]
+    type: Optional[Var[StepsType]]
+
+    items: Optional[Var[ContainVar]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda current: [current],
+        })
+        return _triggers
+
+
+steps = Steps.create
+
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/steps.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/steps.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/switch.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/segmented.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType, SizeType, SelectModeType, PlacementType, VariantType
-
-
-class Switch(AntdComponent):
-    tag = 'Switch'
-
-    auto_focus: Optional[Var[bool]]
-    checked: Optional[Var[bool]]
-    checked_children: Optional[Var[ReactNode]]
-    default_checked: Optional[Var[bool]]
-    default_value: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    loading: Optional[Var[bool]]
-    size: Optional[Var[SizeType]]
-    un_checked_children: Optional[Var[ReactNode]]
-    value: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda checked, e: [checked, e],
-            EventTriggers.ON_CLICK: lambda checked, e: [checked, e],
-        })
-        return _triggers
-
-
-switch = Switch.create
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import SizeType, PlacementType, TabsType
+
+
+class Segmented(AntdComponent):
+    tag = 'Segmented'
+
+    block: Optional[Var[bool]]
+    default_value: Optional[Var[Union[str, int]]]
+    disabled: Optional[Var[bool]]
+    options: Optional[Union[List[str], List[int], List[Dict]]]
+    size: Optional[Var[SizeType]]
+    value: Optional[Var[Union[str, int]]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda value: [value],
+        })
+        return _triggers
+
+
+segmented = Segmented.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/switch.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/table.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/table.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-from reflex.utils import imports
-
-from ..base import AntdComponent, ContainVar, JsValue, JsEvent
-from ..constant import StatusType, SizeType
-
-
-class Table(AntdComponent):
-    tag = 'Table'
-
-    bordered: Optional[Var[bool]]
-    columns: Optional[Var[Union[ContainVar, list]]]
-    data_source: Optional[Var[List[Dict[str, Any]]]]
-    expandable: Optional[Var[ContainVar]]
-    footer: Optional[Var[JsValue]]
-    get_popup_container: Optional[Var[JsValue]]
-    loading: Optional[Var[bool]]
-    locale: Optional[Var[ContainVar]]
-    pagination: Optional[Var[Union[bool, ContainVar]]]
-    row_key: Optional[Var[Union[str, JsValue]]]
-    row_selection: Optional[Var[ContainVar]]
-    scroll: Optional[Var[Union[ContainVar, Dict]]]
-    show_header: Optional[Var[bool]]
-    show_sorter_tooltip: Optional[Var[Union[bool, ContainVar]]]
-    size: Optional[Var[SizeType]] = 'middle'
-    sort_directions: Optional[Var[ContainVar]]
-    sticky: Optional[Var[Union[bool, JsValue]]]
-    summary: Optional[Var[JsValue]]
-    table_layout: Optional[Var[str]]
-    title: Optional[Var[JsValue]]
-    virtual: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda pagination, filters, sorter: [pagination, filters, sorter],
-            'on_header_row': lambda columns, index: [columns, index],
-            'on_row': lambda record, index: [record, index],
-            'on_scroll': lambda ev: [ev],
-
-            'columns.*.on_header_cell': lambda column: [column],
-            'columns.*.on_cell': lambda record, row_index: [record, row_index],
-            'columns.*.on_filter': lambda: [],
-            'columns.*.on_filter_dropdown_open_change': lambda visible: [visible],
-
-            'pagination.on_change': lambda page, size: [page, size],
-            'pagination.on_show_size_change': lambda current, size: [current, size],
-
-            'expandable.on_expand': lambda record, event: [record, event],
-            'expandable.on_expanded_rows_change': lambda rows: [rows],
-
-            'row_selection.on_cell': lambda record, index: [record, index],
-            'row_selection.on_change': lambda keys, rows, info: [keys, info],
-            'row_selection.on_select': lambda record, selected, selected_rows: [record, selected, selected_rows],
-            'row_selection.on_select_all':
-                lambda selected, selected_rows, change_rows: [selected, selected_rows, change_rows],
-        })
-        return _triggers
-
-
-table = Table.create
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+from reflex.utils import imports
+
+from ..base import AntdComponent, ContainVar, JsValue, JsEvent
+from ..constant import StatusType, SizeType
+
+
+class Table(AntdComponent):
+    tag = 'Table'
+
+    bordered: Optional[Var[bool]]
+    columns: Optional[Var[Union[ContainVar, list]]]
+    data_source: Optional[Var[List[Dict[str, Any]]]]
+    expandable: Optional[Var[ContainVar]]
+    footer: Optional[Var[JsValue]]
+    get_popup_container: Optional[Var[JsValue]]
+    loading: Optional[Var[bool]]
+    locale: Optional[Var[ContainVar]]
+    pagination: Optional[Var[Union[bool, ContainVar]]]
+    row_key: Optional[Var[Union[str, JsValue]]]
+    row_selection: Optional[Var[ContainVar]]
+    scroll: Optional[Var[Union[ContainVar, Dict]]]
+    show_header: Optional[Var[bool]]
+    show_sorter_tooltip: Optional[Var[Union[bool, ContainVar]]]
+    size: Optional[Var[SizeType]] = 'middle'
+    sort_directions: Optional[Var[ContainVar]]
+    sticky: Optional[Var[Union[bool, JsValue]]]
+    summary: Optional[Var[JsValue]]
+    table_layout: Optional[Var[str]]
+    title: Optional[Var[JsValue]]
+    virtual: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda pagination, filters, sorter: [pagination, filters, sorter],
+            'on_header_row': lambda columns, index: [columns, index],
+            'on_row': lambda record, index: [record, index],
+            'on_scroll': lambda ev: [ev],
+
+            'columns.*.on_header_cell': lambda column: [column],
+            'columns.*.on_cell': lambda record, row_index: [record, row_index],
+            'columns.*.on_filter': lambda: [],
+            'columns.*.on_filter_dropdown_open_change': lambda visible: [visible],
+
+            'pagination.on_change': lambda page, size: [page, size],
+            'pagination.on_show_size_change': lambda current, size: [current, size],
+
+            'expandable.on_expand': lambda record, event: [record, event],
+            'expandable.on_expanded_rows_change': lambda rows: [rows],
+
+            'row_selection.on_cell': lambda record, index: [record, index],
+            'row_selection.on_change': lambda keys, rows, info: [keys, info],
+            'row_selection.on_select': lambda record, selected, selected_rows: [record, selected, selected_rows],
+            'row_selection.on_select_all':
+                lambda selected, selected_rows, change_rows: [selected, selected_rows, change_rows],
+        })
+        return _triggers
+
+
+table = Table.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/table.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tabs.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tabs.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-from dataclasses import dataclass
-
-from reflex import Component, Var, Base
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import SizeType, PlacementType, TabsType
-
-
-@dataclass(frozen=True)
-class TabItem:
-    close_icon: Optional[Var[ReactNode]] = None
-    destroy_inactive_tab_pane: Optional[Var[bool]] = None
-    disabled: Optional[Var[bool]] = None
-    force_render: Optional[Var[bool]] = None
-    key: Optional[Union[str, Var[str]]] = None
-    label: Optional[Union[ReactNode, Var[ReactNode]]] = None
-    icon: Optional[Var[ReactNode]] = None
-    children: Optional[Union[ReactNode, Var[ReactNode]]] = None
-    closable: Optional[Var[bool]] = None
-
-
-class Tabs(AntdComponent):
-    tag = 'Tabs'
-
-    active_key: Optional[Var[str]]
-    add_icon: Optional[Var[ReactNode]]
-    animated: Optional[Var[Union[bool, Dict]]]
-    centered: Optional[Var[bool]]
-    default_active_key: Optional[Var[str]]
-    hide_add: Optional[Var[bool]]
-    indicator: Optional[Var[Union[Dict, ContainVar]]]
-    items: Optional[Var[Union[ContainVar, List]]]
-    more_icon: Optional[Var[ReactNode]]
-    remove_icon: Optional[Var[ReactNode]]
-    popup_class_name: Optional[Var[str]]
-    render_tab_bar: Optional[Var[JsValue]]
-    size: Optional[Var[SizeType]]
-    tab_bar_extra_content: Optional[Var[Union[ReactNode, ContainVar]]]
-    tab_bar_gutter: Optional[Var[int]]
-    tab_bar_style: Optional[Var[Dict]]
-    tab_position: Optional[Var[PlacementType]]
-    destroy_inactive_tab_pane: Optional[Var[bool]]
-    type: Optional[Var[TabsType]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda key: [key],
-            EventTriggers.ON_EDIT: lambda e0, e1: [e0, e1],
-            "on_tab_click": lambda key, ev: [key, ev],
-            "on_tab_scroll": lambda ev: [ev],
-        })
-        return _triggers
-
-
-tabs = Tabs.create
-tab_item = TabItem
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+from dataclasses import dataclass
+
+from reflex import Component, Var, Base
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import SizeType, PlacementType, TabsType
+
+
+@dataclass(frozen=True)
+class TabItem:
+    close_icon: Optional[Var[ReactNode]] = None
+    destroy_inactive_tab_pane: Optional[Var[bool]] = None
+    disabled: Optional[Var[bool]] = None
+    force_render: Optional[Var[bool]] = None
+    key: Optional[Union[str, Var[str]]] = None
+    label: Optional[Union[ReactNode, Var[ReactNode]]] = None
+    icon: Optional[Var[ReactNode]] = None
+    children: Optional[Union[ReactNode, Var[ReactNode]]] = None
+    closable: Optional[Var[bool]] = None
+
+
+class Tabs(AntdComponent):
+    tag = 'Tabs'
+
+    active_key: Optional[Var[str]]
+    add_icon: Optional[Var[ReactNode]]
+    animated: Optional[Var[Union[bool, Dict]]]
+    centered: Optional[Var[bool]]
+    default_active_key: Optional[Var[str]]
+    hide_add: Optional[Var[bool]]
+    indicator: Optional[Var[Union[Dict, ContainVar]]]
+    items: Optional[Var[Union[ContainVar, List]]]
+    more_icon: Optional[Var[ReactNode]]
+    remove_icon: Optional[Var[ReactNode]]
+    popup_class_name: Optional[Var[str]]
+    render_tab_bar: Optional[Var[JsValue]]
+    size: Optional[Var[SizeType]]
+    tab_bar_extra_content: Optional[Var[Union[ReactNode, ContainVar]]]
+    tab_bar_gutter: Optional[Var[int]]
+    tab_bar_style: Optional[Var[Dict]]
+    tab_position: Optional[Var[PlacementType]]
+    destroy_inactive_tab_pane: Optional[Var[bool]]
+    type: Optional[Var[TabsType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda key: [key],
+            EventTriggers.ON_EDIT: lambda e0, e1: [e0, e1],
+            "on_tab_click": lambda key, ev: [key, ev],
+            "on_tab_scroll": lambda ev: [ev],
+        })
+        return _triggers
+
+
+tabs = Tabs.create
+tab_item = TabItem
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tabs.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tag.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tag.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/timeline.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/timeline.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tooltip.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/auto_complete.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import StatusType, PlacementType, TriggerType
-
-
-class Tooltip(AntdComponent):
-    tag = "Tooltip"
-
-    title: Optional[Var[Union[str, Component, JsValue]]]
-    align: Optional[Var[str]]
-    arrow: Optional[Var[Union[bool, Dict]]]
-    auto_adjust_overflow: Optional[Var[bool]]
-    color: Optional[Var[str]]
-    default_open: Optional[Var[bool]]
-    destroy_tooltip_on_hide: Optional[Var[bool]]
-    fresh: Optional[Var[bool]]
-    get_popup_container: Optional[Var[JsValue]]
-    mouse_enter_delay: Optional[Var[int]]
-    mouse_leave_delay: Optional[Var[int]]
-    overlay_class_name: Optional[Var[str]]
-    overlay_style: Optional[Var[Dict]]
-    overlay_inner_style: Optional[Var[Dict]]
-    placement: Optional[Var[PlacementType]]
-    trigger: Optional[Var[Union[TriggerType, List[TriggerType]]]]
-    open: Optional[Var[bool]]
-    z_index: Optional[Var[int]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_OPEN_CHANGE: lambda open: [open],
-        })
-        return _triggers
-
-
-tooltip = Tooltip.create
-
+from typing import Optional, Union, Dict, Any
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import VariantType, SizeType
+
+
+class AutoComplete(AntdComponent):
+    tag = "AutoComplete"
+
+    allow_clear: Optional[Var[bool]]
+    auto_focus: Optional[Var[bool]]
+    backfill: Optional[Var[bool]]
+    default_active_first_option: Optional[Var[bool]]
+    default_open: Optional[Var[bool]]
+    default_value: Optional[Var[str]]
+    disabled: Optional[Var[bool]]
+    popup_class_name: Optional[Var[str]]
+    dropdown_match_select_width: Optional[Var[Union[bool, int]]]
+    filter_option: Optional[Var[bool]]
+    not_found_content: Optional[Var[ReactNode]]
+    open: Optional[Var[bool]]
+    options: Optional[Var[list]]
+    placeholder: Optional[Var[str]]
+    status: Optional[Var[str]]
+    size: Optional[Var[SizeType]]
+    value: Optional[Var[str]]
+    variant: Optional[Var[VariantType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_BLUR: lambda: [],
+            "on_dropdown_visible_change": lambda open: [open],
+            EventTriggers.ON_FOCUS: lambda: [],
+            "on_search": lambda value: [value],
+            EventTriggers.ON_SELECT: lambda value, option: [value, option],
+            "on_clear": lambda: [],
+        })
+        return _triggers
+
+
+auto_complete = AutoComplete.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tooltip.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tour.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/input_number.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,47 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode
-from ..constant import StatusType, PlacementType, TypeType
-
-
-class Tour(AntdComponent):
-    tag = 'Tour'
-
-    arrow: Optional[Var[bool]]
-    close_icon: Optional[Var[ReactNode]]
-    disabled_interaction: Optional[Var[bool]]
-    placement: Optional[Var[PlacementType]]
-    mask: Optional[Var[Union[bool, Dict]]]
-    type: Optional[Var[TypeType]]
-    open: Optional[Var[bool]]
-    current: Optional[Var[int]]
-    scroll_into_view_options: Optional[Var[Union[bool, Dict]]]
-    steps: Optional[Var[ContainVar]]
-    indicators_render: Optional[Var[JsValue]]
-    z_index: Optional[Var[int]]
-    get_popup_container: Optional[Var[JsValue]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            'on_close': lambda: [],
-            'on_finish': lambda: [],
-            EventTriggers.ON_CHANGE: lambda current: [current],
-            'steps.*.on_close': lambda: [],
-        })
-        return _triggers
-
-
-tour = Tour.create
-
+from typing import Optional, Union, Dict, Any
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode
+from ..constant import StatusType, SizeType, VariantType
+
+
+class InputNumber(AntdComponent):
+    tag = "InputNumber"
+
+    addon_after: Optional[Var[ReactNode]]
+    addon_before: Optional[Var[ReactNode]]
+    auto_focus: Optional[Var[bool]]
+    change_on_blur: Optional[Var[bool]]
+    change_on_wheel: Optional[Var[bool]]
+    controls: Optional[Var[Union[bool, ContainVar]]]
+    decimal_separator: Optional[Var[str]]
+    placeholder: Optional[Var[str]]
+    default_value: Optional[Var[int]]
+    disabled: Optional[Var[bool]]
+    formatter: Optional[Var[JsValue]]
+    keyboard: Optional[Var[bool]]
+    max: Optional[Var[int]]
+    min: Optional[Var[int]]
+    parser: Optional[Var[JsValue]]
+    precision: Optional[Var[int]]
+    read_only: Optional[Var[bool]]
+    status: Optional[Var[StatusType]]
+    prefix: Optional[Var[ReactNode]]
+    size: Optional[Var[SizeType]]
+    step: Optional[Var[Union[int, str]]]
+    string_mode: Optional[Var[bool]]
+    value: Optional[Var[int]]
+    variant: Optional[Var[VariantType]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda value: [value],
+            'on_press_enter': lambda e: [e],
+            "on_step": lambda value, info: [value, info],
+        })
+        return _triggers
+
+
+input_number = InputNumber.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tour.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tour.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/transfer.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/transfer.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tree.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree_select.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tree_select.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsNode, ReactNode
-
-
-class TreeSelect(AntdComponent):
-    tag = 'TreeSelect'
-
-    allow_clear: Optional[Var[Union[bool, ReactNode]]]
-    auto_clear_search_value: Optional[Var[bool]]
-    default_value: Optional[Var[Union[str, List[str]]]]
-    disabled: Optional[Var[bool]]
-    popup_class_name: Optional[Var[str]]
-    popup_match_select_width: Optional[Var[Union[bool, int]]]
-    dropdown_render: Optional[Var[JsNode]]
-    dropdown_style: Optional[Var[Dict]]
-    field_names: Optional[Var[Dict]]
-    filter_tree_node: Optional[Var[Union[bool, JsNode]]]
-    get_popup_container: Optional[Var[JsNode]]
-    label_in_value: Optional[Var[bool]]
-    list_height: Optional[Var[int]]
-    load_data: Optional[Var[JsNode]]
-    max_tag_count: Optional[Var[int]]
-    max_tag_placeholder: Optional[Var[Union[ReactNode, JsNode]]]
-    max_tag_text_length: Optional[Var[int]]
-    multiple: Optional[Var[bool]]
-    not_found_content: Optional[Var[ReactNode]]
-    placeholder: Optional[Var[str]]
-    placement: Optional[Var[str]]
-    search_value: Optional[Var[str]]
-    show_checked_strategy: Optional[Var[str]]
-    show_search: Optional[Var[bool]]
-    size: Optional[Var[str]]
-    status: Optional[Var[str]]
-    suffix_icon: Optional[Var[ReactNode]]
-    switcher_icon: Optional[Var[Union[ReactNode, ContainVar]]]
-    tag_render: Optional[Var[JsNode]]
-    tree_checkable: Optional[Var[bool]]
-    tree_check_strictly: Optional[Var[bool]]
-    tree_data: Optional[Var[List[Dict]]]
-    tree_data_simple_mode: Optional[Var[Union[bool, Dict]]]
-    tree_default_expand_all: Optional[Var[bool]]
-    tree_default_expanded_keys: Optional[Var[List]]
-    tree_expand_action: Optional[Var[Union[str, bool]]]
-    tree_expanded_keys: Optional[Var[List[str]]]
-    tree_icon: Optional[Var[bool]]
-    tree_line: Optional[Var[Union[bool, Dict]]]
-    tree_loaded_keys: Optional[Var[List[str]]]
-    tree_node_filter_prop: Optional[Var[str]]
-    tree_node_label_prop: Optional[Var[str]]
-    value: Optional[Var[Union[str, List[str]]]]
-    variant: Optional[Var[str]]
-    virtual: Optional[Var[str]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda value, label, extra: [value, label, extra],
-            EventTriggers.ON_SELECT: lambda value, node, extra: [value, node, extra],
-            "on_dropdown_visible_change": lambda open: [open],
-            "on_search": lambda value: [value],
-            "on_tree_expand": lambda keys: [keys],
-
-            "filter_tree_node": lambda node: [node],
-            "load_data": lambda node: [node],
-        })
-        return _triggers
-
-
-tree_select = TreeSelect.create
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsNode, ReactNode
+
+
+class TreeSelect(AntdComponent):
+    tag = 'TreeSelect'
+
+    allow_clear: Optional[Var[Union[bool, ReactNode]]]
+    auto_clear_search_value: Optional[Var[bool]]
+    default_value: Optional[Var[Union[str, List[str]]]]
+    disabled: Optional[Var[bool]]
+    popup_class_name: Optional[Var[str]]
+    popup_match_select_width: Optional[Var[Union[bool, int]]]
+    dropdown_render: Optional[Var[JsNode]]
+    dropdown_style: Optional[Var[Dict]]
+    field_names: Optional[Var[Dict]]
+    filter_tree_node: Optional[Var[Union[bool, JsNode]]]
+    get_popup_container: Optional[Var[JsNode]]
+    label_in_value: Optional[Var[bool]]
+    list_height: Optional[Var[int]]
+    load_data: Optional[Var[JsNode]]
+    max_tag_count: Optional[Var[int]]
+    max_tag_placeholder: Optional[Var[Union[ReactNode, JsNode]]]
+    max_tag_text_length: Optional[Var[int]]
+    multiple: Optional[Var[bool]]
+    not_found_content: Optional[Var[ReactNode]]
+    placeholder: Optional[Var[str]]
+    placement: Optional[Var[str]]
+    search_value: Optional[Var[str]]
+    show_checked_strategy: Optional[Var[str]]
+    show_search: Optional[Var[bool]]
+    size: Optional[Var[str]]
+    status: Optional[Var[str]]
+    suffix_icon: Optional[Var[ReactNode]]
+    switcher_icon: Optional[Var[Union[ReactNode, ContainVar]]]
+    tag_render: Optional[Var[JsNode]]
+    tree_checkable: Optional[Var[bool]]
+    tree_check_strictly: Optional[Var[bool]]
+    tree_data: Optional[Var[List[Dict]]]
+    tree_data_simple_mode: Optional[Var[Union[bool, Dict]]]
+    tree_default_expand_all: Optional[Var[bool]]
+    tree_default_expanded_keys: Optional[Var[List]]
+    tree_expand_action: Optional[Var[Union[str, bool]]]
+    tree_expanded_keys: Optional[Var[List[str]]]
+    tree_icon: Optional[Var[bool]]
+    tree_line: Optional[Var[Union[bool, Dict]]]
+    tree_loaded_keys: Optional[Var[List[str]]]
+    tree_node_filter_prop: Optional[Var[str]]
+    tree_node_label_prop: Optional[Var[str]]
+    value: Optional[Var[Union[str, List[str]]]]
+    variant: Optional[Var[str]]
+    virtual: Optional[Var[str]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda value, label, extra: [value, label, extra],
+            EventTriggers.ON_SELECT: lambda value, node, extra: [value, node, extra],
+            "on_dropdown_visible_change": lambda open: [open],
+            "on_search": lambda value: [value],
+            "on_tree_expand": lambda keys: [keys],
+
+            "filter_tree_node": lambda node: [node],
+            "load_data": lambda node: [node],
+        })
+        return _triggers
+
+
+tree_select = TreeSelect.create
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/tree_select.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/tree_select.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/typography.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/typography.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import TypographyTextType
-
-
-class TypographyBase(AntdComponent):
-    code: Optional[Var[bool]]
-    copyable: Optional[Var[Union[bool, ContainVar]]]
-    delete: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    editable: Optional[Var[Union[bool, ContainVar]]]
-    ellipsis: Optional[Var[Union[bool, ContainVar]]]
-
-    mark: Optional[Var[bool]]
-    italic: Optional[Var[bool]]
-    type: Optional[Var[TypographyTextType]]
-    underline: Optional[Var[bool]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CLICK: lambda ev: [ev],
-            'copyable.on_copy': lambda ev: [ev],
-            'editable.on_change': lambda s: [s],
-            'editable.on_cancel': lambda: [],
-            'editable.on_start': lambda: [],
-            'editable.on_end': lambda: [],
-            'ellipsis.on_expand': lambda ev, info: [ev, info],
-            'ellipsis.on_ellipsis': lambda ellipsis: [ellipsis],
-        })
-        return _triggers
-
-
-class TypographyText(TypographyBase):
-    tag = 'Typography.Text'
-
-    keyboard: Optional[Var[bool]]
-    strong: Optional[Var[bool]]
-
-
-class TypographyTitle(TypographyBase):
-    tag = 'Typography.Title'
-
-    level: Optional[Var[int]]
-
-
-class TypographyParagraph(TypographyBase):
-    tag = 'Typography.Paragraph'
-
-    strong: Optional[Var[bool]]
-
-
-typography_text = TypographyText.create
-typography_title = TypographyTitle.create
-typography_paragraph = TypographyParagraph.create
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import TypographyTextType
+
+
+class TypographyBase(AntdComponent):
+    code: Optional[Var[bool]]
+    copyable: Optional[Var[Union[bool, ContainVar]]]
+    delete: Optional[Var[bool]]
+    disabled: Optional[Var[bool]]
+    editable: Optional[Var[Union[bool, ContainVar]]]
+    ellipsis: Optional[Var[Union[bool, ContainVar]]]
+
+    mark: Optional[Var[bool]]
+    italic: Optional[Var[bool]]
+    type: Optional[Var[TypographyTextType]]
+    underline: Optional[Var[bool]]
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CLICK: lambda ev: [ev],
+            'copyable.on_copy': lambda ev: [ev],
+            'editable.on_change': lambda s: [s],
+            'editable.on_cancel': lambda: [],
+            'editable.on_start': lambda: [],
+            'editable.on_end': lambda: [],
+            'ellipsis.on_expand': lambda ev, info: [ev, info],
+            'ellipsis.on_ellipsis': lambda ellipsis: [ellipsis],
+        })
+        return _triggers
+
+
+class TypographyText(TypographyBase):
+    tag = 'Typography.Text'
+
+    keyboard: Optional[Var[bool]]
+    strong: Optional[Var[bool]]
+
+
+class TypographyTitle(TypographyBase):
+    tag = 'Typography.Title'
+
+    level: Optional[Var[int]]
+
+
+class TypographyParagraph(TypographyBase):
+    tag = 'Typography.Paragraph'
+
+    strong: Optional[Var[bool]]
+
+
+typography_text = TypographyText.create
+typography_title = TypographyTitle.create
+typography_paragraph = TypographyParagraph.create
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/typography.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/typography.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/upload.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/transfer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,56 @@
-from typing import Optional, Union, Dict, Any, List
-from reflex import Var, Component
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-
-
-class Upload(AntdComponent):
-    tag = 'Upload'
-
-    accept: Optional[Var[str]]
-    action: Optional[Var[Union[str, JsValue]]]
-    before_upload: Optional[Var[JsValue]]
-    custom_request: Optional[Var[JsValue]]
-    data: Optional[Var[Union[ContainVar, JsValue]]]
-    default_file_list: Optional[Var[List[ContainVar]]]
-    directory: Optional[Var[bool]]
-    disabled: Optional[Var[bool]]
-    file_list: Optional[Var[List[ContainVar]]]
-    headers: Optional[Var[Dict]]
-    icon_render: Optional[Var[JsValue]]
-    is_image_url: Optional[Var[JsValue]]
-    list_type: Optional[Var[str]]
-    max_count: Optional[Var[int]]
-    method: Optional[Var[str]]
-    multiple: Optional[Var[bool]]
-    name: Optional[Var[str]]
-    open_file_dialog_on_click: Optional[Var[bool]]
-    preview_file: Optional[Var[JsValue]]
-    progress: Optional[Var[Dict]]
-    show_upload_list: Optional[Var[Union[bool, Dict]]]
-    with_credentials: Optional[Var[Union[bool]]]
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        _triggers = super().get_event_triggers()
-        _triggers.update({
-            EventTriggers.ON_CHANGE: lambda file, file_list: [file, file_list],
-            "on_drop": lambda event: [event],
-            "on_download": lambda file: [file],
-            "on_preview": lambda file: [file],
-            "on_remove": lambda file: [file]
-        })
-        return _triggers
-
-
-upload = Upload.create
-
+from typing import Optional, Union, Dict, Any, List
+from reflex import Var, Component
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue, js_value, ReactNode
+from ..constant import StatusType
+
+
+class Transfer(AntdComponent):
+    tag = 'Transfer'
+    _rename_props: Dict[str, str] = {"itemRender": "render"}
+
+    data_source: Optional[Var[List]]
+    disabled: Optional[Var[bool]]
+    selections_icon: Optional[Var[ReactNode]]
+    filter_option: Optional[Var[JsValue]]
+    footer: Optional[Var[JsValue]]
+    list_style: Optional[Var[Union[Dict, JsValue]]]
+    locale: Optional[Var[Union[Dict, ContainVar]]]
+    one_way: Optional[Var[bool]]
+    operations: Optional[Var[List[str]]]
+    operation_style: Optional[Var[Dict]]
+    pagination: Optional[Var[Union[bool, ContainVar]]]
+    item_render: Optional[Var[Union[JsValue, ContainVar]]]
+    row_key: Optional[Var[JsValue]]
+    select_all_labels: Optional[Var[JsValue]]
+    selected_keys: Optional[Var[List[str]]]
+    show_search: Optional[Var[bool]]
+    showSelect_all: Optional[Var[bool]]
+    status: Optional[Var[StatusType]]
+    target_keys: Optional[Var[List[str]]]
+    titles: Optional[Var[ContainVar]]
+
+    @classmethod
+    def create(cls, *children, **props) -> Component:
+        if 'item_render' not in props:
+            props['item_render'] = js_value(lambda record: 'return record.title;')
+        com = super().create(*children, **props)
+        return com
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            EventTriggers.ON_CHANGE: lambda target_keys, direction, move_keys: [target_keys, direction, move_keys],
+            EventTriggers.ON_SCROLL: lambda direction, ev: [direction, ev],
+            "on_search": lambda direction, value: [direction, value],
+            "on_select_change": lambda s_keys, t_keys: [s_keys, t_keys],
+        })
+        return _triggers
+
+
+transfer = Transfer.create
+
+
+
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/upload.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/upload.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/watermark.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/watermark.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Optional, Union, Dict, Any, List, Tuple
-
-from reflex import Component, Var
-from reflex.utils import imports
-from reflex.constants import EventTriggers
-
-from ..base import AntdComponent, ContainVar, JsValue
-from ..constant import OrientationType, DirectionType
-
-
-class Watermark(AntdComponent):
-    tag = 'Watermark'
-
-    width: Optional[Var[int]]
-    height: Optional[Var[int]]
-    inherit: Optional[Var[bool]]
-    rotate: Optional[Var[int]]
-    z_index: Optional[Var[int]]
-    image: Optional[Var[str]]
-    content: Optional[Var[Union[str, List[str]]]]
-    font: Optional[Var[Union[Dict, ContainVar]]]
-    gap: Optional[Var[Tuple[int, int]]]
-    offset: Optional[Var[Tuple[int, int]]]
-
-
-watermark = Watermark.create
-
-
+from typing import Optional, Union, Dict, Any, List, Tuple
+
+from reflex import Component, Var
+from reflex.utils import imports
+from reflex.constants import EventTriggers
+
+from ..base import AntdComponent, ContainVar, JsValue
+from ..constant import OrientationType, DirectionType
+
+
+class Watermark(AntdComponent):
+    tag = 'Watermark'
+
+    width: Optional[Var[int]]
+    height: Optional[Var[int]]
+    inherit: Optional[Var[bool]]
+    rotate: Optional[Var[int]]
+    z_index: Optional[Var[int]]
+    image: Optional[Var[str]]
+    content: Optional[Var[Union[str, List[str]]]]
+    font: Optional[Var[Union[Dict, ContainVar]]]
+    gap: Optional[Var[Tuple[int, int]]]
+    offset: Optional[Var[Tuple[int, int]]]
+
+
+watermark = Watermark.create
+
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/antd/watermark.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/antd/watermark.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/base.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,828 +1,838 @@
-from typing import Type, Any, Tuple, Dict, List, Iterable, Callable, Set, Union, Optional, Self
-import sys
-from os import path
-from abc import ABC, abstractmethod
-from functools import lru_cache, wraps
-from hashlib import md5
-import uuid
-import dataclasses
-import inspect
-import re
-
-import reflex as rx
-from reflex import Component, Var, State, Base
-from reflex.base import pydantic
-from reflex.components.component import BaseComponent, CustomComponent, StatefulComponent
-from reflex.constants import Hooks, Reflex, MemoizationDisposition
-from reflex.utils import imports, format
-from reflex.vars import BaseVar, VarData
-from reflex.event import EventHandler, EventSpec, EventChain
-
-from .constant import SizeType
-from .util import OrderedSet
-
-# 0.4.6 -> 000.004.006
-version = '.'.join(map(lambda x: x.zfill(3), Reflex.VERSION.split('.')))
-
-my_path = path.abspath(path.dirname(__file__))
-template_path = path.join(my_path, '.templates')
-
-APP_ROUTER = False
-RE_KEY_IDX = re.compile(r'\.\d+\.')
-
-
-def stateful(hd: Callable[..., Component] = None, forced=True) -> Callable:
-    """ render a component into a function """
-
-    def _my(_hd: Callable[..., Component]) -> Callable:
-        @wraps(_hd)
-        def _wrap(*args, **kwargs):
-            _com = _hd(*args, **kwargs)
-            if forced:
-                _com._memoization_mode = _com._memoization_mode.__class__()
-                _com._memoization_mode.disposition = MemoizationDisposition.ALWAYS
-                # _com._memoization_mode.recursive = False
-            _sc = StatefulComponent.create(_com)
-            return _sc if _sc is not None else _com
-        return _wrap
-
-    if hd is None:
-        return _my
-    else:
-        return _my(hd)
-
-
-def pretty_dumps(value: Any, indent=2) -> str:
-    return format.json.dumps(value, ensure_ascii=False, default=format.serialize, indent=indent)
-
-
-class ExItem(ABC):
-    @classmethod
-    def isinstance(cls, item: Any) -> bool:
-        pass
-
-    def __init__(self, item: Any, parent: Component, key: str = ''):
-        self.item = item
-        self.key = key
-        self.parent = parent
-
-    @abstractmethod
-    def serialize(self) -> str:
-        ...
-
-    def get_imports(self) -> imports.ImportDict:
-        return {}
-
-    def get_state(self) -> str:
-        return ''
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        if version <= '000.004.006':
-            return set()
-        return {}
-
-    def get_interpolations(self) -> List[Tuple[int, int]]:
-        return []
-
-    def get_var_data(self) -> VarData:
-        return VarData(
-            state=self.get_state(),
-            imports=self.get_imports(),
-            hooks=self.get_hooks(),
-            interpolations=self.get_interpolations(),
-        )
-
-    def get_custom_components(self) -> set[CustomComponent]:
-        return set()
-
-    def get_custom_code(self) -> set[str]:
-        return set()
-
-
-class ExComponentItemBase(ExItem):
-    item: Component
-
-    @classmethod
-    def isinstance(cls, item: Any) -> bool:
-        return isinstance(item, Component)
-
-    def serialize(self) -> str:
-        return str(self.item)
-
-    def get_imports(self) -> imports.ImportDict:
-        if version <= '000.004.006':
-            return self.item.get_imports()
-        else:
-            return self.item._get_all_imports()
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        if version <= '000.004.006':
-            return self.item.get_hooks_internal() | self.item.get_hooks()
-        else:
-            return self.item._get_all_hooks_internal() | self.item._get_all_hooks()
-
-    def get_custom_components(self) -> set[CustomComponent]:
-        return {self.item} if isinstance(self.item, CustomComponent) else set()
-
-    def get_custom_code(self) -> set[str]:
-        if version <= '000.004.006':
-            return self.item.get_custom_code() if isinstance(self.item, BaseComponent) else set()
-        return self.item._get_all_custom_code() if isinstance(self.item, BaseComponent) else set()
-
-
-class ExComponentItem(ExComponentItemBase):
-    item: Component
-
-
-class ExStatefulComponentItem(ExComponentItemBase):
-    item: StatefulComponent
-
-    @classmethod
-    def isinstance(cls, item: Any) -> bool:
-        return isinstance(item, StatefulComponent)
-
-    def serialize(self) -> str:
-        return f'<{self.item.tag}/>'
-
-
-class JsEvent:
-    hd: EventHandler
-    # event_trigger use for custom trigger, must work with fmt=True
-    event_trigger: Callable
-
-    def __init__(self, hd: Any, js: str = '', fmt: bool = False, event_trigger: Callable = None):
-        assert isinstance(hd, EventHandler)
-        self.hd = hd
-        self.js = js
-        self.fmt = fmt
-        self.event_trigger = event_trigger
-
-    def get_state_full_name(self) -> str:
-        name = str(self.hd.fn).split(' ')[1]
-        _base = format.to_snake_case(name)
-        return f'state.{_base}'
-
-    def get_event_args(self) -> str:
-        _args = inspect.getfullargspec(self.hd.fn)
-        rs = []
-        for idx, _arg in enumerate(_args.args):
-            if idx == 0:  # ignore self
-                continue
-            rs.append(f'{_arg}:{self.args[idx-1]}')
-        return ','.join(rs)
-
-    def get_ex_item(self, parent, key) -> ExItem:
-        item = ExEventHandlerItem(self, parent, key=key)
-        return item
-
-
-js_event = JsEvent
-
-
-class ExEventHandlerItem(ExItem):
-    item: JsEvent
-
-    @classmethod
-    def isinstance(cls, item: Any) -> bool:
-        return isinstance(item, JsEvent)
-
-    @property
-    def hd_item(self) -> 'ExLambdaHandlerItem':
-        try:
-            return self._hd_item
-        except AttributeError:
-            self._hd_item = ExLambdaHandlerItem(self.item.hd, self.parent, key=self.key)
-            self._hd_item.event_trigger = self.item.event_trigger
-            return self._hd_item
-
-    def _get_fn_name(self) -> str:
-        return f"{self.key.replace('.', '_')}_{md5(f'{str(self.item.hd)}'.encode('utf-8')).hexdigest()}_{id(self)}"
-
-    def serialize(self) -> str:
-        hd_name = self.hd_item.serialize()
-        trigger = self.hd_item._get_event_trigger()
-        args = inspect.getfullargspec(trigger).args
-
-        if not self.item.fmt:
-            return f"""({','.join(args)}) => {{
-                {self.item.js}
-                {hd_name}({','.join(args)})
-            }}
-            """
-        else:
-            return self.item.js % dict(name=hd_name)
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        return self.hd_item.get_hooks()
-
-    def get_imports(self) -> imports.ImportDict:
-        return self.hd_item.get_imports()
-
-
-class ExLambdaHandlerItem(ExItem):
-    item: Callable
-    event_trigger: Callable = None
-
-    @classmethod
-    def isinstance(cls, item: Any) -> bool:
-        return isinstance(item, Callable)
-
-    def _get_fn_name(self) -> str:
-        return f"{self.key.replace('.', '_')}_{md5(f'{str(self.item)}'.encode('utf-8')).hexdigest()}_{id(self)}"
-
-    def _get_event_trigger_key(self) -> str:
-        return RE_KEY_IDX.sub('.*.', self.key)
-
-    def _get_event_trigger(self) -> Callable:
-        if self.event_trigger is not None:
-            return self.event_trigger
-        triggers = self.parent.get_event_triggers()
-        rs = triggers.get(self._get_event_trigger_key(), lambda: [])
-        return rs
-
-    def serialize(self) -> str:
-        return self._get_fn_name()
-
-    def get_imports(self) -> imports.ImportDict:
-        return {"react": [imports.ImportVar(tag="useCallback")]}
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        if version <= '000.004.005':
-            key = self._get_event_trigger_key()
-            chain = self.parent._create_event_chain(key, self.item)
-        else:
-            key = self._get_event_trigger()
-            chain = self.parent._create_event_chain(key, self.item)
-        rendered_chain = format.format_prop(chain).strip("{}")
-        _hook = f"""const {self._get_fn_name()} = useCallback({rendered_chain}, [addEvents, Event]);"""
-
-        if version <= '000.004.006':
-            return {_hook}
-        return {_hook: None}
-
-
-class ExCallableItem(ExItem):
-    item: Callable
-
-    @classmethod
-    def isinstance(cls, item: Any) -> bool:
-        return isinstance(item, Callable)
-
-    def serialize(self) -> str:
-        return str(self.item())
-
-    def get_imports(self) -> imports.ImportDict:
-        if version <= '000.004.006':
-            return self.item().get_imports()
-        else:
-            return self.item()._get_all_imports()
-
-    def get_hooks(self) -> Set[str] |Dict[str, None]:
-        _item = self.item()
-        if version <= '000.004.006':
-            return _item.get_hooks_internal() | _item.get_hooks()
-        return _item._get_all_hooks_internal() | _item._get_all_hooks()
-
-
-class ExStateItem(ExItem):
-    item: BaseVar
-
-    @classmethod
-    def isinstance(cls, item: Any) -> bool:
-        return isinstance(item, BaseVar) and item._var_full_name.startswith("state__")
-
-    def serialize(self) -> str:
-        return self.item._var_full_name
-
-    def get_imports(self) -> imports.ImportDict:
-        return self.item._var_data.imports
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        return self.item._var_data.hooks
-
-    def get_state(self) -> str:
-        return self.item._var_data.state
-
-
-class FakeComponentMixin:
-    def _create_event_chain(self, *args, **kwargs):
-        return Component._create_event_chain(self, *args, **kwargs)
-
-    def get_event_triggers(self) -> Dict[str, Any]:
-        return {}
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        return {}
-
-    def get_imports(self) -> imports.ImportDict:
-        return {}
-
-
-class JsValue:
-    value: Callable | str
-
-    def __init__(self, value: Union[str, Callable, Any] = None, **kwargs):
-        self.value = value
-        self._init(**kwargs)
-
-    def _init(self, **kwargs) -> None:
-        for k, v in kwargs.items():
-            setattr(self, k, v)
-
-    def get_ex_item(self, parent, key) -> ExItem:
-        item = ExJsItem(self, parent, key=key)
-        return item
-
-    def serialize(self) -> str:
-        return self.value
-
-    def get_imports(self) -> imports.ImportDict:
-        return {}
-
-    def get_state(self) -> str:
-        return ''
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        if version <= '000.004.006':
-            return set()
-        return {}
-
-    def get_var_data(self) -> VarData:
-        return VarData(
-            state=self.get_state(),
-            imports=self.get_imports(),
-            hooks=self.get_hooks(),
-        )
-
-    def get_custom_components(self) -> set[CustomComponent]:
-        return set()
-
-
-class JsFunctionValue(JsValue):
-    _value: Union[str, Component]
-
-    def _init(self, **kwargs) -> None:
-        super()._init(**kwargs)
-        self._args = inspect.getfullargspec(self.value)
-        args = self._args.args
-        self._value = self.value(*args)
-
-    def serialize(self) -> str:
-        is_component = False
-        if isinstance(self._value, str):
-            v = self._value
-        elif isinstance(self._value, Component):
-            is_component = True
-            v = str(self._value)
-        else:
-            raise TypeError(self._value)
-        sep_1, sep_2 = ('{{', '}}') if not is_component else ('(', ')')
-        return f"""({','.join(self._args.args)}) => 
-        {sep_1} {v} {sep_2} """
-
-    def get_imports(self) -> imports.ImportDict:
-        if version <= '000.004.006':
-            return {} if isinstance(self._value, str) else self._value.get_imports()
-        return {} if isinstance(self._value, str) else self._value._get_all_imports()
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        if version <= '000.004.006':
-            return set() if isinstance(self._value, str) else self._value.get_hooks()
-        return set() if isinstance(self._value, str) \
-            else self._value._get_all_hooks_internal() | self._value._get_all_hooks()
-
-    def get_custom_components(self) -> set[CustomComponent]:
-        return set() if not isinstance(self._value, CustomComponent) else {self._value}
-
-
-def js_value(value: Union[str, Callable], **kwargs) -> JsValue:
-    if isinstance(value, str):
-        return JsValue(value, **kwargs)
-    if isinstance(value, Callable):
-        return JsFunctionValue(value, **kwargs)
-    raise NotImplemented("Not implemented: %s(%s)" % (type(value), value))
-
-
-class ExJsItem(ExItem):
-    item: JsValue
-
-    @classmethod
-    def isinstance(cls, item: Any) -> bool:
-        return isinstance(item, JsValue)
-
-    def serialize(self) -> str:
-        return self.item.serialize()
-
-    def get_imports(self) -> imports.ImportDict:
-        return self.item.get_imports()
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        return self.item.get_hooks()
-
-    def get_custom_components(self) -> set[CustomComponent]:
-        return self.item.get_custom_components()
-
-
-class ExVarItem(ExItem):
-    item: Var
-
-    @classmethod
-    def isinstance(cls, item: Any) -> bool:
-        return isinstance(item, Var)
-
-    def serialize(self) -> str:
-        return str(self.item).strip('{}')
-
-    def get_imports(self) -> imports.ImportDict:
-        return self.item._var_data.imports if self.item._var_data else {}
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        return self.item._var_data.hooks if self.item._var_data else {}
-
-    def get_state(self) -> str:
-        return self.item._var_data.state if self.item._var_data else ""
-
-    def get_interpolations(self) -> List[Tuple[int, int]]:
-        return self.item._var_data.interpolations if self.item._var_data else []
-
-
-class ExFormatter:
-    items: List[Type[ExItem]] = [
-        ExVarItem,
-        ExStatefulComponentItem,
-        ExComponentItem,
-        ExStateItem,
-        ExJsItem,
-        ExEventHandlerItem,
-        ExLambdaHandlerItem,
-        # ExCallableItem,
-    ]
-
-    def __init__(self, value: Any, parent: Component, name: str = ''):
-        self.name = name
-        self.value = value
-        self.parent = parent
-        self._coms: Dict[str, ExItem] = {}
-        self._value: Any = None
-        self._extract()
-
-    def _extract(self):
-        value = self.value
-        self._coms.clear()
-
-        def _op(_v: Any, key: str):
-            if isinstance(_v, (list, tuple)):
-                return _list(_v, pkey=key)
-            elif isinstance(_v, dict):
-                return _dict(_v, pkey=key)
-            elif isinstance(_v, (int, float, str, bool)):
-                return _v
-
-            _id = _v
-            for ex in self.items:
-                if ex.isinstance(_v):
-                    _id = uuid.uuid4().hex
-                    self._coms[_id] = ex(_v, self.parent, key=key)
-                    return _id
-
-            if isinstance(_v, Base):
-                _d = dict(_v._iter(exclude_unset=True, exclude_none=True, to_dict=False))
-                return _dict(_d, pkey=key)
-            elif dataclasses.is_dataclass(_v):
-                _d = dataclasses.asdict(_v)
-                return _dict(_d, pkey=key)
-
-            return _v
-
-        def _list(_v: List, pkey: str) -> List[Any]:
-            return [_op(i, key=f'{pkey}.{idx}') for idx, i in enumerate(_v)]
-
-        def _dict(_v: Dict, pkey: str) -> Dict[str, Any]:
-            return dict((format.to_camel_case(k), _op(v, key=f'{pkey}.{k}')) for k, v in _v.items() if v is not None)
-
-        rs = _op(value, key=self.name)
-        self._value = rs
-
-    def get_ex_item(self, key: str) -> ExItem | None:
-        for i in self._coms.values():
-            if i.key == key:
-                return i
-
-    def get_value(self) -> str:
-        v = pretty_dumps(self._value)
-        for k, ex in self._coms.items():
-            v = v.replace(f'"{k}"', ex.serialize())
-        return v
-
-    def get_imports(self) -> imports.ImportDict:
-        _imports = imports.merge_imports(
-            *(c.get_imports() for c in self._coms.values()),
-        )
-        return _imports
-
-    def get_state(self) -> str:
-        for _, ex in self._coms.items():
-            _state = ex.get_state()
-            if _state != '':
-                return _state
-        return ''
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        if version <= '000.004.006':
-            hooks = set()
-        else:
-            hooks = {}
-        for _, ex in self._coms.items():
-            _hooks = ex.get_hooks()
-            hooks.update(_hooks)
-        return hooks
-
-    def get_interpolations(self) -> List[Tuple[int, int]]:
-        rs = []
-        for _, ex in self._coms.items():
-            rs += ex.get_interpolations()
-        return rs
-
-    def get_var_data(self) -> VarData:
-        return VarData(
-            state=self.get_state(),
-            imports=self.get_imports(),
-            hooks=self.get_hooks(),
-            interpolations=self.get_interpolations(),
-        )
-
-
-@dataclasses.dataclass(
-    eq=False,
-    **{"slots": True} if sys.version_info >= (3, 10) else {},
-)
-class ExVar(BaseVar):
-    _var_value: Any = dataclasses.field(default=Any)
-
-
-class NodeVar(ExVar):
-    """
-    support:
-        . base types: int, float, bool, str
-        . js, like: {show ? 11 : 0}
-     """
-    pass
-
-
-@dataclasses.dataclass(
-    eq=False,
-    **{"slots": True} if sys.version_info >= (3, 10) else {},
-)
-class ContainVar(ExVar):
-    _var_fmt: ExFormatter = dataclasses.field(default=None)
-
-    @property
-    def _var_full_name(self) -> str:
-        return self._var_name
-
-    @classmethod
-    def create(cls, _args_: Any = None, **kwargs) -> Self:
-        value = _args_ if _args_ is not None else kwargs
-        # v: BaseVar = super().create(_name, _var_is_local=_var_is_local, _var_is_string=_var_is_string)
-        return cls(
-            _var_name='',
-            _var_type=cls,
-            _var_is_local=True,
-            _var_is_string=False,
-            _var_data=None,
-            _var_value=value,
-        )
-
-    def init(self, parent: Component, name: str) -> Self:
-        fmt = ExFormatter(self._var_value, parent=parent, name=name)
-        self._var_fmt = fmt
-        self._var_name = fmt.get_value()
-        self._var_data = fmt.get_var_data()
-        return self
-
-    def get_custom_components(self) -> set[CustomComponent]:
-        rs = set()
-        for ex in self._var_fmt._coms.values():
-            rs |= ex.get_custom_components()
-        return rs
-
-    def get_custom_code(self) -> Set[str]:
-        rs = set()
-        for ex in self._var_fmt._coms.values():
-            rs |= ex.get_custom_code()
-        return rs
-
-    def get_hooks(self) -> Set[str] | Dict[str, None]:
-        return self._var_data.hooks
-
-    def get_imports(self) -> imports.ImportDict:
-        return self._var_data.imports
-
-
-contain = ContainVar.create
-
-
-# no use
-class VarDataMixin:
-    def __iter__(self):
-        v = Var()
-        v._var_data = VarData(
-            imports=self.get_imports(),
-        )
-        yield from [v]
-
-
-class AntdBaseMixin:
-    def _get_all_custom_components(
-            self, seen: set[str] | None = None
-    ) -> Set[CustomComponent]:
-        _coms = super()._get_all_custom_components(seen=seen)
-        if hasattr(self, '_custom_components') and self._custom_components:
-            _coms |= self._custom_components
-        return _coms
-
-    def _get_all_custom_code(self) -> Set[str]:
-        code = super()._get_all_custom_code()
-        for k, v in self._iter_contains():
-            code.update(v.get_custom_code())
-        return code
-
-    def _get_style(self) -> dict:
-        """Get the style for the component.
-
-        Returns:
-            The dictionary of the component style as value and the style notation as key.
-        """
-        return {"style": self.style}
-
-    def _get_events_hooks(self) -> set[str] | Dict[str, None]:
-        _hooks = super()._get_events_hooks()
-        js_events: List[BaseVar] = [
-            v for k, v in self.event_triggers.items()
-            if isinstance(v, BaseVar) and v._var_data is not None and v._var_data.hooks]
-
-        if version <= '000.004.006':
-            rs = OrderedSet(_hooks)
-        else:
-            rs = _hooks
-
-        if js_events:
-            for ev in js_events:
-                rs |= ev._var_data.hooks
-        return rs
-
-    def _get_hooks_internal(self) -> Set[str] | Dict[str, None]:
-        """Get the React hooks for this component managed by the framework.
-
-        Downstream components should NOT override this method to avoid breaking
-        framework functionality.
-
-        Returns:
-            Set of internally managed hooks.
-        """
-        # need order hooks, useContext code need first
-        if version <= '000.004.006':
-            s = OrderedSet(
-                hook
-                for hook in [self._get_mount_lifecycle_hook(), self._get_ref_hook()]
-                if hook
-            )
-
-            s |= self._get_events_hooks()
-            var_hooks = self._get_vars_hooks()
-            if [h for h in var_hooks if 'addEvents' in h]:
-                s.add(Hooks.EVENTS)
-            s |= var_hooks
-            s |= self._get_special_hooks()
-            return s
-        else:
-            s = {
-                hook: None
-                for hook in [self._get_ref_hook(), self._get_mount_lifecycle_hook()]
-                if hook is not None
-            }
-            var_hooks = self._get_vars_hooks()
-            if [h for h in var_hooks if 'addEvents' in h]:
-                s[Hooks.EVENTS] = None
-            s |= var_hooks
-            s |= self._get_events_hooks()
-            s |= self._get_special_hooks()
-            return s
-
-    def _iter_contains(self) -> Iterable[Tuple[str, ContainVar]]:
-        for k in self.get_fields().keys():
-            v = getattr(self, k, None)
-            if isinstance(v, ContainVar):
-                yield k, v
-
-    def _init_contains(self, contains: Dict[str, ContainVar], exs: Dict[str, Any]):
-        for k, v in contains.items():
-            v.init(self, k)
-            self._custom_components |= v.get_custom_components()
-            setattr(self, k, v)
-
-        event_keys = self.get_event_triggers().keys()
-        for k, v in exs.items():
-            if isinstance(v, (JsValue, JsEvent)):
-                item = v.get_ex_item(self, k)
-            else:
-                raise NotImplementedError(f"Unsupported type: {type(v)}")
-            self._custom_components |= item.get_custom_components()
-            _v = BaseVar(
-                _var_name=item.serialize(),
-                _var_is_local=True,
-                _var_data=item.get_var_data(),
-            )
-            if k in event_keys:
-                self.event_triggers[k] = _v
-            else:
-                setattr(self, k, _v)
-
-
-class AntdComponent(AntdBaseMixin, Component):
-    """A component that wraps a Chakra component."""
-
-    library = "antd"
-
-    _custom_components: Set[CustomComponent] = pydantic.PrivateAttr(default_factory=set)
-
-    @staticmethod
-    @lru_cache(maxsize=None)
-    def _get_app_wrap_components() -> dict[tuple[int, str], Component]:
-        from .antd.base import config_provider
-        return {
-            (40, "AntdProvider"): _config_provider if _config_provider is not None else config_provider(),
-        }
-
-    def __init__(self, *args, **kwargs):
-        contains = {}
-        exs = {}
-        kw = {}
-        for k, v in kwargs.items():
-            if isinstance(v, ContainVar):
-                contains[k] = v
-            elif isinstance(v, (JsValue, JsEvent)):
-                exs[k] = v
-            else:
-                kw[k] = v
-        # super().__init__(*args, **kw)
-        try:
-            super().__init__(*args, **kw)
-        except Exception as err:
-            print(f"class<{self}>, args={args}, kw={kw}, error: {err}")
-            raise
-        self._init_contains(contains, exs)
-
-
-class AntdSubComponent(AntdBaseMixin, Component):
-    base_tag: str = None
-
-    def _get_imports(self) -> imports.ImportDict:
-        _imports = super()._get_imports()
-        return {}
-
-
-_config_provider: Optional[Component] = None
-
-
-def default_config(provider: Component):
-    global _config_provider
-    from .antd.base import ConfigProvider
-    assert isinstance(provider, ConfigProvider)
-    _config_provider = provider
-
-
-def patch_all():
-    from reflex import constants, vars
-    from reflex.compiler import templates
-
-    constants.Templates.Dirs.JINJA_TEMPLATE = [path.join(template_path, 'jinja'),
-                                               constants.Templates.Dirs.JINJA_TEMPLATE]
-
-    templates.DOCUMENT_ROOT = templates.get_template("web/pages/_document.js.jinja2")
-
-    old_extract_var_data = vars._extract_var_data
-    def _my_extract_var_data(value: Union[Iterable, Component]) -> list[VarData | None]:
-        if isinstance(value, Component):
-            if version <= '000.004.006':
-                return [
-                    VarData(
-                        imports=value.get_imports(),
-                        hooks=set(value.get_hooks()),
-                    )
-                ]
-            return [
-                VarData(
-                    imports=value._get_all_imports(),
-                    hooks=value._get_all_hooks_internal() | value._get_all_hooks(),
-                )
-            ]
-        var_datas = old_extract_var_data(value)
-        return var_datas
-
-    vars._extract_var_data = _my_extract_var_data
-
-
-ReactNode = Union[str, Component]
-JsNode = Union[JsValue, JsEvent]
-
+from typing import Type, Any, Tuple, Dict, List, Iterable, Callable, Set, Union, Optional, Self
+import sys
+from os import path
+from abc import ABC, abstractmethod
+from functools import lru_cache, wraps
+from hashlib import md5
+import uuid
+import dataclasses
+import inspect
+import re
+
+import reflex as rx
+from reflex import Component, Var, State, Base
+from reflex.base import pydantic
+from reflex.components.component import BaseComponent, CustomComponent, StatefulComponent
+from reflex.constants import Hooks, Reflex, MemoizationDisposition
+from reflex.utils import imports, format
+from reflex.vars import BaseVar, VarData
+from reflex.event import EventHandler, EventSpec, EventChain
+
+from .constant import SizeType
+from .util import OrderedSet
+
+# 0.4.6 -> 000.004.006
+version = '.'.join(map(lambda x: x.zfill(3), Reflex.VERSION.split('.')))
+
+my_path = path.abspath(path.dirname(__file__))
+template_path = path.join(my_path, '.templates')
+
+APP_ROUTER = False
+RE_KEY_IDX = re.compile(r'\.\d+\.')
+
+
+def stateful(hd: Callable[..., Component] = None, forced=True) -> Callable:
+    """ render a component into a function """
+
+    def _my(_hd: Callable[..., Component]) -> Callable:
+        @wraps(_hd)
+        def _wrap(*args, **kwargs):
+            _com = _hd(*args, **kwargs)
+            if forced:
+                _com._memoization_mode = _com._memoization_mode.__class__()
+                _com._memoization_mode.disposition = MemoizationDisposition.ALWAYS
+                # _com._memoization_mode.recursive = False
+            # _sc = StatefulComponent.create(_com)
+            # return _sc if _sc is not None else _com
+            return _com
+        return _wrap
+
+    if hd is None:
+        return _my
+    else:
+        return _my(hd)
+
+
+def pretty_dumps(value: Any, indent=2) -> str:
+    return format.json.dumps(value, ensure_ascii=False, default=format.serialize, indent=indent)
+
+
+class ExItem(ABC):
+    @classmethod
+    def isinstance(cls, item: Any) -> bool:
+        pass
+
+    def __init__(self, item: Any, parent: Component, key: str = ''):
+        self.item = item
+        self.key = key
+        self.parent = parent
+
+    @abstractmethod
+    def serialize(self) -> str:
+        ...
+
+    def get_imports(self) -> imports.ImportDict:
+        return {}
+
+    def get_state(self) -> str:
+        return ''
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        if version <= '000.004.006':
+            return set()
+        return {}
+
+    def get_interpolations(self) -> List[Tuple[int, int]]:
+        return []
+
+    def get_var_data(self) -> VarData:
+        return VarData(
+            state=self.get_state(),
+            imports=self.get_imports(),
+            hooks=self.get_hooks(),
+            interpolations=self.get_interpolations(),
+        )
+
+    def get_custom_components(self) -> set[CustomComponent]:
+        return set()
+
+    def get_custom_code(self) -> set[str]:
+        return set()
+
+
+class ExComponentItemBase(ExItem):
+    item: Component
+
+    @classmethod
+    def isinstance(cls, item: Any) -> bool:
+        return isinstance(item, Component)
+
+    def serialize(self) -> str:
+        return str(self.item)
+
+    def get_imports(self) -> imports.ImportDict:
+        if version <= '000.004.006':
+            return self.item.get_imports()
+        else:
+            return self.item._get_all_imports()
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        if version <= '000.004.006':
+            return self.item.get_hooks_internal() | self.item.get_hooks()
+        else:
+            return self.item._get_all_hooks_internal() | self.item._get_all_hooks()
+
+    def get_custom_components(self) -> set[CustomComponent]:
+        return {self.item} if isinstance(self.item, CustomComponent) else set()
+
+    def get_custom_code(self) -> set[str]:
+        if version <= '000.004.006':
+            return self.item.get_custom_code() if isinstance(self.item, BaseComponent) else set()
+        return self.item._get_all_custom_code() if isinstance(self.item, BaseComponent) else set()
+
+
+class ExComponentItem(ExComponentItemBase):
+    item: Component
+
+
+class ExStatefulComponentItem(ExComponentItemBase):
+    item: StatefulComponent
+
+    @classmethod
+    def isinstance(cls, item: Any) -> bool:
+        return isinstance(item, StatefulComponent)
+
+    def serialize(self) -> str:
+        return f'<{self.item.tag}/>'
+
+
+class JsEvent:
+    hd: EventHandler
+    # event_trigger use for custom trigger, must work with fmt=True
+    event_trigger: Callable
+
+    def __init__(self, hd: Any, js: str = '', fmt: bool = False, event_trigger: Callable = None):
+        assert isinstance(hd, EventHandler)
+        self.hd = hd
+        self.js = js
+        self.fmt = fmt
+        self.event_trigger = event_trigger
+
+    def get_state_full_name(self) -> str:
+        name = str(self.hd.fn).split(' ')[1]
+        _base = format.to_snake_case(name)
+        return f'state.{_base}'
+
+    def get_event_args(self) -> str:
+        _args = inspect.getfullargspec(self.hd.fn)
+        rs = []
+        for idx, _arg in enumerate(_args.args):
+            if idx == 0:  # ignore self
+                continue
+            rs.append(f'{_arg}:{self.args[idx-1]}')
+        return ','.join(rs)
+
+    def get_ex_item(self, parent, key) -> ExItem:
+        item = ExEventHandlerItem(self, parent, key=key)
+        return item
+
+
+js_event = JsEvent
+
+
+class ExEventHandlerItem(ExItem):
+    item: JsEvent
+
+    @classmethod
+    def isinstance(cls, item: Any) -> bool:
+        return isinstance(item, JsEvent)
+
+    @property
+    def hd_item(self) -> 'ExLambdaHandlerItem':
+        try:
+            return self._hd_item
+        except AttributeError:
+            self._hd_item = ExLambdaHandlerItem(self.item.hd, self.parent, key=self.key)
+            self._hd_item.event_trigger = self.item.event_trigger
+            return self._hd_item
+
+    def _get_fn_name(self) -> str:
+        return f"{self.key.replace('.', '_')}_{md5(f'{str(self.item.hd)}'.encode('utf-8')).hexdigest()}_{id(self)}"
+
+    def serialize(self) -> str:
+        hd_name = self.hd_item.serialize()
+        trigger = self.hd_item._get_event_trigger()
+        args = inspect.getfullargspec(trigger).args
+
+        if not self.item.fmt:
+            return f"""({','.join(args)}) => {{
+                {self.item.js}
+                {hd_name}({','.join(args)})
+            }}
+            """
+        else:
+            return self.item.js % dict(name=hd_name)
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        return self.hd_item.get_hooks()
+
+    def get_imports(self) -> imports.ImportDict:
+        return self.hd_item.get_imports()
+
+
+class ExLambdaHandlerItem(ExItem):
+    item: Callable
+    event_trigger: Callable = None
+
+    @classmethod
+    def isinstance(cls, item: Any) -> bool:
+        return isinstance(item, Callable)
+
+    def _get_fn_name(self) -> str:
+        return f"{self.key.replace('.', '_')}_{md5(f'{str(self.item)}'.encode('utf-8')).hexdigest()}_{id(self)}"
+
+    def _get_event_trigger_key(self) -> str:
+        return RE_KEY_IDX.sub('.*.', self.key)
+
+    def _get_event_trigger(self) -> Callable:
+        if self.event_trigger is not None:
+            return self.event_trigger
+        triggers = self.parent.get_event_triggers()
+        rs = triggers.get(self._get_event_trigger_key(), lambda: [])
+        return rs
+
+    def serialize(self) -> str:
+        return self._get_fn_name()
+
+    def get_imports(self) -> imports.ImportDict:
+        return {"react": [imports.ImportVar(tag="useCallback")]}
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        if version <= '000.004.005':
+            key = self._get_event_trigger_key()
+            chain = self.parent._create_event_chain(key, self.item)
+        else:
+            key = self._get_event_trigger()
+            chain = self.parent._create_event_chain(key, self.item)
+        rendered_chain = format.format_prop(chain).strip("{}")
+        _hook = f"""const {self._get_fn_name()} = useCallback({rendered_chain}, [addEvents, Event]);"""
+
+        if version <= '000.004.006':
+            return {_hook}
+        return {_hook: None}
+
+
+class ExCallableItem(ExItem):
+    item: Callable
+
+    @classmethod
+    def isinstance(cls, item: Any) -> bool:
+        return isinstance(item, Callable)
+
+    def serialize(self) -> str:
+        return str(self.item())
+
+    def get_imports(self) -> imports.ImportDict:
+        if version <= '000.004.006':
+            return self.item().get_imports()
+        else:
+            return self.item()._get_all_imports()
+
+    def get_hooks(self) -> Set[str] |Dict[str, None]:
+        _item = self.item()
+        if version <= '000.004.006':
+            return _item.get_hooks_internal() | _item.get_hooks()
+        return _item._get_all_hooks_internal() | _item._get_all_hooks()
+
+
+class ExStateItem(ExItem):
+    item: BaseVar
+
+    @classmethod
+    def isinstance(cls, item: Any) -> bool:
+        return isinstance(item, BaseVar) and item._var_full_name.startswith("state__")
+
+    def serialize(self) -> str:
+        return self.item._var_full_name
+
+    def get_imports(self) -> imports.ImportDict:
+        return self.item._var_data.imports
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        return self.item._var_data.hooks
+
+    def get_state(self) -> str:
+        return self.item._var_data.state
+
+
+class FakeComponentMixin:
+    def _create_event_chain(self, *args, **kwargs):
+        return Component._create_event_chain(self, *args, **kwargs)
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        return {}
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        return {}
+
+    def get_imports(self) -> imports.ImportDict:
+        return {}
+
+
+class JsValue:
+    value: Callable | str
+
+    def __init__(self, value: Union[str, Callable, Any] = None, **kwargs):
+        self.value = value
+        self._init(**kwargs)
+
+    def _init(self, **kwargs) -> None:
+        for k, v in kwargs.items():
+            setattr(self, k, v)
+
+    def get_ex_item(self, parent, key) -> ExItem:
+        item = ExJsItem(self, parent, key=key)
+        return item
+
+    def serialize(self) -> str:
+        return f"({self.value})"
+
+    def get_imports(self) -> imports.ImportDict:
+        return {}
+
+    def get_state(self) -> str:
+        return ''
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        if version <= '000.004.006':
+            return set()
+        return {}
+
+    def get_var_data(self) -> VarData:
+        return VarData(
+            state=self.get_state(),
+            imports=self.get_imports(),
+            hooks=self.get_hooks(),
+        )
+
+    def get_custom_components(self) -> set[CustomComponent]:
+        return set()
+
+
+class JsFunctionValue(JsValue):
+    _value: Union[str, Component]
+
+    def _init(self, **kwargs) -> None:
+        super()._init(**kwargs)
+        self._args = inspect.getfullargspec(self.value)
+        args = self._args.args
+        self._value = self.value(*args)
+
+    def serialize(self) -> str:
+        is_component = False
+        if isinstance(self._value, str):
+            v = self._value
+        elif isinstance(self._value, Component):
+            is_component = True
+            v = str(self._value)
+        else:
+            raise TypeError(self._value)
+        sep_1, sep_2 = ('{{', '}}') if not is_component else ('(', ')')
+        return f"""(({','.join(self._args.args)}) => 
+        {sep_1} {v} {sep_2} )"""
+
+    def get_imports(self) -> imports.ImportDict:
+        if version <= '000.004.006':
+            return {} if isinstance(self._value, str) else self._value.get_imports()
+        return {} if isinstance(self._value, str) else self._value._get_all_imports()
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        if version <= '000.004.006':
+            return set() if isinstance(self._value, str) else self._value.get_hooks()
+        return set() if isinstance(self._value, str) \
+            else self._value._get_all_hooks_internal() | self._value._get_all_hooks()
+
+    def get_custom_components(self) -> set[CustomComponent]:
+        return set() if not isinstance(self._value, CustomComponent) else {self._value}
+
+
+def js_value(value: Union[str, Callable], **kwargs) -> JsValue:
+    if isinstance(value, str):
+        return JsValue(value, **kwargs)
+    if isinstance(value, Callable):
+        return JsFunctionValue(value, **kwargs)
+    raise NotImplemented("Not implemented: %s(%s)" % (type(value), value))
+
+
+class ExJsItem(ExItem):
+    item: JsValue
+
+    @classmethod
+    def isinstance(cls, item: Any) -> bool:
+        return isinstance(item, JsValue)
+
+    def serialize(self) -> str:
+        return self.item.serialize()
+
+    def get_imports(self) -> imports.ImportDict:
+        return self.item.get_imports()
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        return self.item.get_hooks()
+
+    def get_custom_components(self) -> set[CustomComponent]:
+        return self.item.get_custom_components()
+
+
+class ExVarItem(ExItem):
+    item: Var
+
+    @classmethod
+    def isinstance(cls, item: Any) -> bool:
+        return isinstance(item, Var)
+
+    def serialize(self) -> str:
+        return str(self.item).strip('{}')
+
+    def get_imports(self) -> imports.ImportDict:
+        return self.item._var_data.imports if self.item._var_data else {}
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        return self.item._var_data.hooks if self.item._var_data else {}
+
+    def get_state(self) -> str:
+        return self.item._var_data.state if self.item._var_data else ""
+
+    def get_interpolations(self) -> List[Tuple[int, int]]:
+        return self.item._var_data.interpolations if self.item._var_data else []
+
+
+class ExFormatter:
+    items: List[Type[ExItem]] = [
+        ExVarItem,
+        ExStatefulComponentItem,
+        ExComponentItem,
+        ExStateItem,
+        ExJsItem,
+        ExEventHandlerItem,
+        ExLambdaHandlerItem,
+        # ExCallableItem,
+    ]
+
+    def __init__(self, value: Any, parent: Component, name: str = ''):
+        self.name = name
+        self.value = value
+        self.parent = parent
+        self._coms: Dict[str, ExItem] = {}
+        self._value: Any = None
+        self._extract()
+
+    def _extract(self):
+        value = self.value
+        self._coms.clear()
+
+        def _op(_v: Any, key: str):
+            if isinstance(_v, (list, tuple)):
+                return _list(_v, pkey=key)
+            elif isinstance(_v, dict):
+                return _dict(_v, pkey=key)
+            elif isinstance(_v, (int, float, str, bool)):
+                return _v
+
+            _id = _v
+            for ex in self.items:
+                if ex.isinstance(_v):
+                    _id = uuid.uuid4().hex
+                    self._coms[_id] = ex(_v, self.parent, key=key)
+                    return _id
+
+            if isinstance(_v, Base):
+                _d = dict(_v._iter(exclude_unset=True, exclude_none=True, to_dict=False))
+                return _dict(_d, pkey=key)
+            elif dataclasses.is_dataclass(_v):
+                _d = dataclasses.asdict(_v)
+                return _dict(_d, pkey=key)
+
+            return _v
+
+        def _list(_v: List, pkey: str) -> List[Any]:
+            return [_op(i, key=f'{pkey}.{idx}') for idx, i in enumerate(_v)]
+
+        def _dict(_v: Dict, pkey: str) -> Dict[str, Any]:
+            return dict((format.to_camel_case(k), _op(v, key=f'{pkey}.{k}')) for k, v in _v.items() if v is not None)
+
+        rs = _op(value, key=self.name)
+        self._value = rs
+
+    def get_ex_item(self, key: str) -> ExItem | None:
+        for i in self._coms.values():
+            if i.key == key:
+                return i
+
+    def get_value(self) -> str:
+        v = pretty_dumps(self._value)
+        for k, ex in self._coms.items():
+            v = v.replace(f'"{k}"', ex.serialize())
+        return v
+
+    def get_imports(self) -> imports.ImportDict:
+        _imports = imports.merge_imports(
+            *(c.get_imports() for c in self._coms.values()),
+        )
+        return _imports
+
+    def get_state(self) -> str:
+        for _, ex in self._coms.items():
+            _state = ex.get_state()
+            if _state != '':
+                return _state
+        return ''
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        if version <= '000.004.006':
+            hooks = set()
+        else:
+            hooks = {}
+        for _, ex in self._coms.items():
+            _hooks = ex.get_hooks()
+            hooks.update(_hooks)
+        return hooks
+
+    def get_interpolations(self) -> List[Tuple[int, int]]:
+        rs = []
+        for _, ex in self._coms.items():
+            rs += ex.get_interpolations()
+        return rs
+
+    def get_var_data(self) -> VarData:
+        return VarData(
+            state=self.get_state(),
+            imports=self.get_imports(),
+            hooks=self.get_hooks(),
+            interpolations=self.get_interpolations(),
+        )
+
+
+@dataclasses.dataclass(
+    eq=False,
+    **{"slots": True} if sys.version_info >= (3, 10) else {},
+)
+class ExVar(BaseVar):
+    _var_value: Any = dataclasses.field(default=Any)
+
+
+class NodeVar(ExVar):
+    """
+    support:
+        . base types: int, float, bool, str
+        . js, like: {show ? 11 : 0}
+     """
+    pass
+
+
+@dataclasses.dataclass(
+    eq=False,
+    **{"slots": True} if sys.version_info >= (3, 10) else {},
+)
+class ContainVar(ExVar):
+    _var_fmt: ExFormatter = dataclasses.field(default=None)
+
+    @property
+    def _var_full_name(self) -> str:
+        return self._var_name
+
+    @classmethod
+    def create(cls, _args_: Any = None, **kwargs) -> Self:
+        value = _args_ if _args_ is not None else kwargs
+        # v: BaseVar = super().create(_name, _var_is_local=_var_is_local, _var_is_string=_var_is_string)
+        return cls(
+            _var_name='',
+            _var_type=cls,
+            _var_is_local=True,
+            _var_is_string=False,
+            _var_data=None,
+            _var_value=value,
+        )
+
+    def init(self, parent: Component, name: str) -> Self:
+        fmt = ExFormatter(self._var_value, parent=parent, name=name)
+        self._var_fmt = fmt
+        self._var_name = fmt.get_value()
+        self._var_data = fmt.get_var_data()
+        return self
+
+    def get_custom_components(self) -> set[CustomComponent]:
+        rs = set()
+        for ex in self._var_fmt._coms.values():
+            rs |= ex.get_custom_components()
+        return rs
+
+    def get_custom_code(self) -> Set[str]:
+        rs = set()
+        for ex in self._var_fmt._coms.values():
+            rs |= ex.get_custom_code()
+        return rs
+
+    def get_hooks(self) -> Set[str] | Dict[str, None]:
+        return self._var_data.hooks
+
+    def get_imports(self) -> imports.ImportDict:
+        return self._var_data.imports
+
+
+contain = ContainVar.create
+
+
+# no use
+class VarDataMixin:
+    def __iter__(self):
+        v = Var()
+        v._var_data = VarData(
+            imports=self.get_imports(),
+        )
+        yield from [v]
+
+
+class AntdBaseComponent(Component):
+    _custom_components: Set[CustomComponent] = pydantic.PrivateAttr(default_factory=set)
+
+    def __init__(self, *args, **kwargs):
+        contains = {}
+        exs = {}
+        kw = {}
+        for k, v in kwargs.items():
+            if isinstance(v, ContainVar):
+                contains[k] = v
+            elif isinstance(v, (JsValue, JsEvent)):
+                exs[k] = v
+            else:
+                kw[k] = v
+        # super().__init__(*args, **kw)
+        try:
+            super().__init__(*args, **kw)
+        except Exception as err:
+            print(f"class<{self}>, args={args}, kw={kw}, error: {err}")
+            raise
+        self._init_contains(contains, exs)
+
+    def _get_all_custom_components(
+            self, seen: set[str] | None = None
+    ) -> Set[CustomComponent]:
+        _coms = super()._get_all_custom_components(seen=seen)
+        if hasattr(self, '_custom_components') and self._custom_components:
+            _coms |= self._custom_components
+        return _coms
+
+    def _get_all_custom_code(self) -> Set[str]:
+        code = super()._get_all_custom_code()
+        for k, v in self._iter_contains():
+            code.update(v.get_custom_code())
+        return code
+
+    def _get_style(self) -> dict:
+        """Get the style for the component.
+
+        Returns:
+            The dictionary of the component style as value and the style notation as key.
+        """
+        return {"style": self.style}
+
+    def _get_events_hooks(self) -> set[str] | Dict[str, None]:
+        _hooks = super()._get_events_hooks()
+        js_events: List[BaseVar] = [
+            v for k, v in self.event_triggers.items()
+            if isinstance(v, BaseVar) and v._var_data is not None and v._var_data.hooks]
+
+        if version <= '000.004.006':
+            rs = OrderedSet(_hooks)
+        else:
+            rs = _hooks
+
+        if js_events:
+            for ev in js_events:
+                rs |= ev._var_data.hooks
+        return rs
+
+    def _get_hooks_internal(self) -> Set[str] | Dict[str, None]:
+        """Get the React hooks for this component managed by the framework.
+
+        Downstream components should NOT override this method to avoid breaking
+        framework functionality.
+
+        Returns:
+            Set of internally managed hooks.
+        """
+        # need order hooks, useContext code need first
+        if version <= '000.004.006':
+            s = OrderedSet(
+                hook
+                for hook in [self._get_mount_lifecycle_hook(), self._get_ref_hook()]
+                if hook
+            )
+
+            s |= self._get_events_hooks()
+            var_hooks = self._get_vars_hooks()
+            if [h for h in var_hooks if 'addEvents' in h]:
+                s.add(Hooks.EVENTS)
+            s |= var_hooks
+            s |= self._get_special_hooks()
+            return s
+        else:
+            s = {
+                hook: None
+                for hook in [self._get_ref_hook(), self._get_mount_lifecycle_hook()]
+                if hook is not None
+            }
+            var_hooks = self._get_vars_hooks()
+            if [h for h in var_hooks if 'addEvents' in h]:
+                s[Hooks.EVENTS] = None
+            s |= var_hooks
+            s |= self._get_events_hooks()
+            s |= self._get_special_hooks()
+            return s
+
+    def _iter_contains(self) -> Iterable[Tuple[str, ContainVar]]:
+        for k in self.get_fields().keys():
+            v = getattr(self, k, None)
+            if isinstance(v, ContainVar):
+                yield k, v
+
+    def _init_contains(self, contains: Dict[str, ContainVar], exs: Dict[str, Any]):
+        for k, v in contains.items():
+            v.init(self, k)
+            self._custom_components |= v.get_custom_components()
+            setattr(self, k, v)
+
+        event_keys = self.get_event_triggers().keys()
+        for k, v in exs.items():
+            if isinstance(v, (JsValue, JsEvent)):
+                item = v.get_ex_item(self, k)
+            else:
+                raise NotImplementedError(f"Unsupported type: {type(v)}")
+            self._custom_components |= item.get_custom_components()
+            _v = ExVar(
+                _var_name=item.serialize(),
+                _var_is_local=True,
+                _var_data=item.get_var_data(),
+                _var_value=v,
+            )
+            if k in event_keys:
+                self.event_triggers[k] = _v
+            else:
+                setattr(self, k, _v)
+
+
+class AntdComponent(AntdBaseComponent):
+    """A component that wraps an Antd component."""
+    library = "antd"
+
+    @staticmethod
+    @lru_cache(maxsize=None)
+    def _get_app_wrap_components() -> dict[tuple[int, str], Component]:
+        from .antd.base import config_provider
+        return {
+            (40, "AntdProvider"): _config_provider if _config_provider is not None else config_provider(),
+        }
+
+
+class AntdSubComponent(AntdBaseComponent, Component):
+    base_tag: str = None
+
+    def _get_imports(self) -> imports.ImportDict:
+        _imports = super()._get_imports()
+        return {}
+
+
+_config_provider: Optional[Component] = None
+
+
+def default_config(provider: Component):
+    global _config_provider
+    from .antd.base import ConfigProvider
+    assert isinstance(provider, ConfigProvider)
+    _config_provider = provider
+
+
+def patch_all():
+    from reflex import constants, vars
+    from reflex.compiler import templates
+
+    constants.Templates.Dirs.JINJA_TEMPLATE = [path.join(template_path, 'jinja'),
+                                               constants.Templates.Dirs.JINJA_TEMPLATE]
+
+    templates.DOCUMENT_ROOT = templates.get_template("web/pages/_document.js.jinja2")
+
+    old_extract_var_data = vars._extract_var_data
+    def _my_extract_var_data(value: Union[Iterable, Component]) -> list[VarData | None]:
+        if isinstance(value, Component):
+            if version <= '000.004.006':
+                return [
+                    VarData(
+                        imports=value.get_imports(),
+                        hooks=set(value.get_hooks()),
+                    )
+                ]
+            return [
+                VarData(
+                    imports=value._get_all_imports(),
+                    hooks=value._get_all_hooks_internal() | value._get_all_hooks(),
+                )
+            ]
+        var_datas = old_extract_var_data(value)
+        return var_datas
+
+    vars._extract_var_data = _my_extract_var_data
+
+    def _my_get_memoized_event_triggers(
+            cls,
+            component: Component,
+    ) -> dict[str, tuple[Var, str]]:
+        """ fix: some js function can not memo """
+        pass
+
+    # StatefulComponent._get_memoized_event_triggers = classmethod(_my_get_memoized_event_triggers)
+
+
+ReactNode = Union[str, Component]
+JsNode = Union[JsValue, JsEvent]
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/base.pyi` & `reflex_antd-0.0.7/custom_components/reflex_antd/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/constant.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/constant.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing import Literal
-
-
-ThemeType = Literal["light", "dark"]
-PlacementType = Literal["start", "end", "bottom", "bottomLeft", "bottomRight", "top", "topLeft", "topRight"]
-AlignType = Literal["start", "end", "center", "baseline", "left", "right"]
-OrientationType = Literal["left", "right", "top", "bottom", "center"]
-DirectionType = Literal["vertical", "horizontal", "inline"]
-SizeType = Literal["default", "small", "medium", "middle", "large"]
-StatusType = Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']
-TriggerType = Literal["click", "hover", "focus", 'contextMenu']
-VariantType = Literal['outlined', 'borderless', 'filled']
-TypeType = Literal['default', 'primary']
-RoleType = Literal['alert', 'status']
-BreakpointType = Literal['xs', 'sm', 'md', 'lg', 'xl', 'xxl']
-
-ColorFormatType = Literal['rgb', 'hex', 'hsb']
-
-ButtonShape = Literal['default', 'circle', 'round']
-
-TypographyTextType = Literal['secondary', 'success', 'warning', 'danger']
-
-FloatGroupShapeType = Literal["circle", "square"]
-
-BadgeStatusType = Literal["success", 'processing', 'default', 'error', 'warning']
-
-StepsStatusType = Literal['wait', 'process', 'finish', 'error']
-StepsType = Literal['default', 'navigation', 'inline']
-
-DatePickerModeType = Literal['time', 'date', 'month', 'year', 'decade']
-DatePickerType = Literal['date', 'week', 'month', 'quarter', 'year']
-
-RadioStyleType = Literal['outline', 'solid']
-RadioType = Literal['default', 'button']
-
-SelectModeType = Literal['multiple', 'tags']
-
-ProgressType = Literal['line', 'circle', 'dashboard']
-
-TimelineModeType = Literal['left', 'alternate', 'right']
-
-TabsType = Literal['line', 'card', 'editable-card']
-
-QRCodeType = Literal['canvas', 'svg']
-QRCodeErrorLevelType = Literal['L', 'M', 'Q', 'H']
-QRCodeStatusType = Literal['active', 'expired', 'loading', 'scanned']
-
-MessageType = Literal['info', 'success', 'error', 'loading', 'warning']
+from typing import Literal
+
+
+ThemeType = Literal["light", "dark"]
+PlacementType = Literal["start", "end", "bottom", "bottomLeft", "bottomRight", "top", "topLeft", "topRight"]
+AlignType = Literal["start", "end", "center", "baseline", "left", "right"]
+OrientationType = Literal["left", "right", "top", "bottom", "center"]
+DirectionType = Literal["vertical", "horizontal", "inline"]
+SizeType = Literal["default", "small", "medium", "middle", "large"]
+StatusType = Literal['default', 'success', 'error', 'warning', 'info', 'exception', 'normal', 'active']
+TriggerType = Literal["click", "hover", "focus", 'contextMenu']
+VariantType = Literal['outlined', 'borderless', 'filled']
+TypeType = Literal['default', 'primary']
+RoleType = Literal['alert', 'status']
+BreakpointType = Literal['xs', 'sm', 'md', 'lg', 'xl', 'xxl']
+
+ColorFormatType = Literal['rgb', 'hex', 'hsb']
+
+ButtonShape = Literal['default', 'circle', 'round']
+
+TypographyTextType = Literal['secondary', 'success', 'warning', 'danger']
+
+FloatGroupShapeType = Literal["circle", "square"]
+
+BadgeStatusType = Literal["success", 'processing', 'default', 'error', 'warning']
+
+StepsStatusType = Literal['wait', 'process', 'finish', 'error']
+StepsType = Literal['default', 'navigation', 'inline']
+
+DatePickerModeType = Literal['time', 'date', 'month', 'year', 'decade']
+DatePickerType = Literal['date', 'week', 'month', 'quarter', 'year']
+
+RadioStyleType = Literal['outline', 'solid']
+RadioType = Literal['default', 'button']
+
+SelectModeType = Literal['multiple', 'tags']
+
+ProgressType = Literal['line', 'circle', 'dashboard']
+
+TimelineModeType = Literal['left', 'alternate', 'right']
+
+TabsType = Literal['line', 'card', 'editable-card']
+
+QRCodeType = Literal['canvas', 'svg']
+QRCodeErrorLevelType = Literal['L', 'M', 'Q', 'H']
+QRCodeStatusType = Literal['active', 'expired', 'loading', 'scanned']
+
+MessageType = Literal['info', 'success', 'error', 'loading', 'warning']
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/display.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/display.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from .antd.badge import badge, badge_ribbon  # noqa
-from .antd.table import table  # noqa
-from .antd.tree import tree  # noqa
-from .antd.avatar import avatar,avatar_group  # noqa
-from .antd.calendar import calendar,dayjs  # noqa
-from .antd.card import card,card_grid,card_meta  # noqa
-from .antd.carousel import carousel  # noqa
-from .antd.collapse import collapse  # noqa
-from .antd.descriptions import descriptions  # noqa
-from .antd.empty import empty  # noqa
-from .antd.image import image,image_preview_group  # noqa
-from .antd.list import alist,list_item,list_item_meta  # noqa
-from .antd.popover import popover  # noqa
-from .antd.qrcode import qrcode  # noqa
-from .antd.segmented import segmented  # noqa
-from .antd.statistic import statistic, statistic_countdown  # noqa
-from .antd.tabs import tabs, tab_item  # noqa
-from .antd.tag import tag, checkable_tag  # noqa
-from .antd.timeline import timeline  # noqa
-from .antd.tooltip import tooltip  # noqa
-from .antd.tour import tour  # noqa
-
+from .antd.badge import badge, badge_ribbon  # noqa
+from .antd.table import table  # noqa
+from .antd.tree import tree  # noqa
+from .antd.avatar import avatar,avatar_group  # noqa
+from .antd.calendar import calendar,dayjs  # noqa
+from .antd.card import card,card_grid,card_meta  # noqa
+from .antd.carousel import carousel  # noqa
+from .antd.collapse import collapse  # noqa
+from .antd.descriptions import descriptions  # noqa
+from .antd.empty import empty  # noqa
+from .antd.image import image,image_preview_group  # noqa
+from .antd.list import alist,list_item,list_item_meta  # noqa
+from .antd.popover import popover  # noqa
+from .antd.qrcode import qrcode  # noqa
+from .antd.segmented import segmented  # noqa
+from .antd.statistic import statistic, statistic_countdown  # noqa
+from .antd.tabs import tabs, tab_item  # noqa
+from .antd.tag import tag, checkable_tag  # noqa
+from .antd.timeline import timeline  # noqa
+from .antd.tooltip import tooltip  # noqa
+from .antd.tour import tour  # noqa
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/entry.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/entry.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from .antd.auto_complete import auto_complete  # noqa
-from .antd.cascader import cascader  # noqa
-from .antd.checkbox import checkbox_group, checkbox  # noqa
-from .antd.color_picker import color_picker  # noqa
-from .antd.date_picker import dayjs, date_picker, range_picker  # noqa
-from .antd.form import form, form_item, form_list, form_provider, confirm_form, modal_form  # noqa
-from .antd.input import input, text_area, search, password  # noqa
-from .antd.input_number import input_number  # noqa
-from .antd.mentions import mention  # noqa
-from .antd.radio import radio, radio_button, radio_group  # noqa
-from .antd.rate import rate  # noqa
-from .antd.select import select  # noqa
-from .antd.tree_select import tree_select  # noqa
-from .antd.slider import slider  # noqa
-from .antd.switch import switch  # noqa
-from .antd.transfer import transfer  # noqa
-from .antd.upload import upload  # noqa
-
-
+from .antd.auto_complete import auto_complete  # noqa
+from .antd.cascader import cascader  # noqa
+from .antd.checkbox import checkbox_group, checkbox  # noqa
+from .antd.color_picker import color_picker  # noqa
+from .antd.date_picker import dayjs, date_picker, range_picker  # noqa
+from .antd.form import form, form_item, form_list, form_provider, confirm_form, modal_form  # noqa
+from .antd.input import input, text_area, search, password  # noqa
+from .antd.input_number import input_number  # noqa
+from .antd.mentions import mention  # noqa
+from .antd.radio import radio, radio_button, radio_group  # noqa
+from .antd.rate import rate  # noqa
+from .antd.select import select  # noqa
+from .antd.tree_select import tree_select  # noqa
+from .antd.slider import slider  # noqa
+from .antd.switch import switch  # noqa
+from .antd.transfer import transfer  # noqa
+from .antd.upload import upload  # noqa
+
+
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd/feedback.py` & `reflex_antd-0.0.7/custom_components/reflex_antd/feedback.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .antd.progress import progress  # noqa
-from .antd.result import result  # noqa
-from .antd.skeleton import skeleton  # noqa
-from .antd.spin import spin  # noqa
-from .antd.watermark import watermark  # noqa
-from .antd.alert import alert, alert_error_boundary  # noqa
-from .antd.drawer import drawer  # noqa
-from .antd.message import message, message_holder  # noqa
-from .antd.notification import notification  # noqa
-from .antd.modal import modal, confirm  # noqa
-from .antd.popconfirm import popconfirm  # noqa
+from .antd.progress import progress  # noqa
+from .antd.result import result  # noqa
+from .antd.skeleton import skeleton  # noqa
+from .antd.spin import spin  # noqa
+from .antd.watermark import watermark  # noqa
+from .antd.alert import alert, alert_error_boundary  # noqa
+from .antd.drawer import drawer  # noqa
+from .antd.message import message, message_holder  # noqa
+from .antd.notification import notification  # noqa
+from .antd.modal import modal, confirm  # noqa
+from .antd.popconfirm import popconfirm  # noqa
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/PKG-INFO` & `reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-antd
-Version: 0.0.6
+Version: 0.0.7
 Summary: Reflex custom component antd
 Author-email: seewind <seewindcn@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: homepage, https://github.com/seewindcn/reflex-antd
 Project-URL: source, https://github.com/seewindcn/reflex-antd
 Keywords: reflex,reflex-custom-components
```

### Comparing `reflex_antd-0.0.6/custom_components/reflex_antd.egg-info/SOURCES.txt` & `reflex_antd-0.0.7/custom_components/reflex_antd.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 custom_components/reflex_antd/antd/flex.pyi
 custom_components/reflex_antd/antd/float_button.py
 custom_components/reflex_antd/antd/float_button.pyi
 custom_components/reflex_antd/antd/form.py
 custom_components/reflex_antd/antd/form.pyi
 custom_components/reflex_antd/antd/grid.py
 custom_components/reflex_antd/antd/grid.pyi
+custom_components/reflex_antd/antd/helper.py
 custom_components/reflex_antd/antd/icon.py
 custom_components/reflex_antd/antd/icon.pyi
 custom_components/reflex_antd/antd/image.py
 custom_components/reflex_antd/antd/image.pyi
 custom_components/reflex_antd/antd/input.py
 custom_components/reflex_antd/antd/input.pyi
 custom_components/reflex_antd/antd/input_number.py
```

### Comparing `reflex_antd-0.0.6/pyproject.toml` & `reflex_antd-0.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-[build-system]
-requires = [
-    "setuptools",
-    "wheel",
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "reflex-antd"
-version = "0.0.6"
-description = "Reflex custom component antd"
-readme = "README.md"
-license = { text = "Apache-2.0" }
-requires-python = ">=3.8"
-authors = [{ name = "seewind", email = "seewindcn@gmail.com" }]
-keywords = [
-    "reflex",
-    "reflex-custom-components"]
-
-dependencies = [
-    "reflex>=0.4.2"
-]
-
-classifiers = [
-  "Development Status :: 4 - Beta",
-]
-
-[project.urls]
-Homepage = "https://github.com/seewindcn/reflex-antd"
-homepage = "https://github.com/seewindcn/reflex-antd"
-source = "https://github.com/seewindcn/reflex-antd"
-
-[project.optional-dependencies]
-dev = ["build", "twine"]
-
-
-
-[tool.setuptools.packages.find]
-where = ["custom_components"]
+[build-system]
+requires = [
+    "setuptools",
+    "wheel",
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "reflex-antd"
+version = "0.0.7"
+description = "Reflex custom component antd"
+readme = "README.md"
+license = { text = "Apache-2.0" }
+requires-python = ">=3.8"
+authors = [{ name = "seewind", email = "seewindcn@gmail.com" }]
+keywords = [
+    "reflex",
+    "reflex-custom-components"]
+
+dependencies = [
+    "reflex>=0.4.2"
+]
+
+classifiers = [
+  "Development Status :: 4 - Beta",
+]
+
+[project.urls]
+Homepage = "https://github.com/seewindcn/reflex-antd"
+homepage = "https://github.com/seewindcn/reflex-antd"
+source = "https://github.com/seewindcn/reflex-antd"
+
+[project.optional-dependencies]
+dev = ["build", "twine"]
+
+
+
+[tool.setuptools.packages.find]
+where = ["custom_components"]
```

