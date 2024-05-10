# Comparing `tmp/bride-of-frankensystem-1.9.3.7.tar.gz` & `tmp/bride-of-frankensystem-2.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\colby\Desktop\git\bride-of-frankensystem\dist\.tmp-v7dxbeu7\bride-of-frankensystem-1.9.3.7.tar", last modified: Thu Apr 18 18:57:04 2024, max compression
+gzip compressed data, was "C:\Users\colby\Desktop\git\bride-of-frankensystem\dist\.tmp-o0ptzm0f\bride-of-frankensystem-2.0.0.0.tar", last modified: Fri May 10 19:36:04 2024, max compression
```

## Comparing `bride-of-frankensystem-1.9.3.7.tar` & `bride-of-frankensystem-2.0.0.0.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/
--rw-rw-rw-   0        0        0    15092 2024-04-18 18:52:52.000000 bride-of-frankensystem-1.9.3.7/BOFS/BOFSFlask.py
--rw-rw-rw-   0        0        0     4026 2024-04-18 18:29:19.000000 bride-of-frankensystem-1.9.3.7/BOFS/BOFSSession.py
--rw-rw-rw-   0        0        0    11154 2024-04-18 18:48:27.000000 bride-of-frankensystem-1.9.3.7/BOFS/JSONQuestionnaire.py
--rw-rw-rw-   0        0        0     6858 2024-04-17 02:53:52.000000 bride-of-frankensystem-1.9.3.7/BOFS/JSONTable.py
--rw-rw-rw-   0        0        0     5672 2024-04-15 21:33:28.000000 bride-of-frankensystem-1.9.3.7/BOFS/PageList.py
--rw-rw-rw-   0        0        0      117 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.7/BOFS/__init__.py
--rw-rw-rw-   0        0        0       65 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.7/BOFS/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/
--rw-rw-rw-   0        0        0    20276 2024-04-18 18:56:00.000000 bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/BOFSFlask.cpython-311.pyc
--rw-rw-rw-   0        0        0     5496 2024-04-18 18:33:26.000000 bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/BOFSSession.cpython-311.pyc
--rw-rw-rw-   0        0        0    16585 2024-04-18 18:49:47.000000 bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/JSONQuestionnaire.cpython-311.pyc
--rw-rw-rw-   0        0        0     9903 2024-04-17 04:31:32.000000 bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/JSONTable.cpython-311.pyc
--rw-rw-rw-   0        0        0     6901 2024-04-15 22:13:05.000000 bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/PageList.cpython-311.pyc
--rw-rw-rw-   0        0        0      384 2024-04-05 21:05:42.000000 bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      337 2024-04-06 05:50:26.000000 bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/__main__.cpython-311.pyc
--rw-rw-rw-   0        0        0     1998 2024-04-06 05:50:26.000000 bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/cli.cpython-311.pyc
--rw-rw-rw-   0        0        0     6221 2024-04-18 18:33:26.000000 bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/create_app.cpython-311.pyc
--rw-rw-rw-   0        0        0     3017 2024-04-15 22:14:27.000000 bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/globals.cpython-311.pyc
--rw-rw-rw-   0        0        0    17284 2024-04-16 04:26:24.000000 bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/util.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/
--rw-rw-rw-   0        0        0    12573 2024-04-18 18:43:43.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/Results.py
--rw-rw-rw-   0        0        0      883 2024-04-17 19:42:01.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/SummaryStats.py
--rw-rw-rw-   0        0        0       22 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/
--rw-rw-rw-   0        0        0    14271 2024-04-18 18:43:53.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/Results.cpython-311.pyc
--rw-rw-rw-   0        0        0     2059 2024-04-17 19:44:37.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/SummaryStats.cpython-311.pyc
--rw-rw-rw-   0        0        0      181 2022-05-18 21:12:21.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      252 2024-01-19 17:54:16.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3420 2022-07-15 22:52:11.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/util.cpython-310.pyc
--rw-rw-rw-   0        0        0     8043 2024-04-15 22:36:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/util.cpython-311.pyc
--rw-rw-rw-   0        0        0    14352 2022-07-15 22:51:49.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0    27621 2024-04-18 18:33:26.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/views.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/
--rw-rw-rw-   0        0        0      844 2024-04-07 19:31:03.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/database_delete.html
--rw-rw-rw-   0        0        0     1648 2024-04-17 06:00:53.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/export.html
--rw-rw-rw-   0        0        0      304 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/export_csv.html
--rw-rw-rw-   0        0        0      877 2024-04-08 06:24:14.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/login_admin.html
--rw-rw-rw-   0        0        0     2490 2024-04-08 04:55:02.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/preview_questionnaire.html
--rw-rw-rw-   0        0        0      283 2024-04-02 04:25:23.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/preview_questionnaire_simple.html
--rw-rw-rw-   0        0        0      606 2024-04-08 05:52:37.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/progress.html
--rw-rw-rw-   0        0        0     2369 2024-04-08 05:37:40.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/progress_ajax.html
--rw-rw-rw-   0        0        0     3196 2024-04-07 19:09:11.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/progress_summary_ajax.html
--rw-rw-rw-   0        0        0     3517 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/questionnaire_results.html
--rw-rw-rw-   0        0        0     2020 2024-04-17 23:32:30.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/results.html
--rw-rw-rw-   0        0        0      572 2024-04-17 23:31:16.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/results_boxplot.html
--rw-rw-rw-   0        0        0     1366 2024-04-07 05:58:54.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/table_ajax.html
--rw-rw-rw-   0        0        0     1056 2024-04-07 18:32:29.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/table_view.html
--rw-rw-rw-   0        0        0     4872 2024-04-18 00:27:25.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/template_admin.html
--rw-rw-rw-   0        0        0     1056 2024-04-07 19:28:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/template_admin_head.html
--rw-rw-rw-   0        0        0     4427 2024-04-15 22:36:03.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/util.py
--rw-rw-rw-   0        0        0    17764 2024-04-18 18:23:22.000000 bride-of-frankensystem-1.9.3.7/BOFS/admin/views.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/bride_of_frankensystem.egg-info/
--rw-rw-rw-   0        0        0    12537 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.7/BOFS/bride_of_frankensystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.7/BOFS/bride_of_frankensystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.7/BOFS/bride_of_frankensystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.7/BOFS/bride_of_frankensystem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       85 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.7/BOFS/bride_of_frankensystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2024-04-05 20:43:15.000000 bride-of-frankensystem-1.9.3.7/BOFS/bride_of_frankensystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1286 2024-01-07 00:02:19.000000 bride-of-frankensystem-1.9.3.7/BOFS/cli.py
--rw-rw-rw-   0        0        0     5299 2024-04-18 18:29:19.000000 bride-of-frankensystem-1.9.3.7/BOFS/create_app.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/default/
--rw-rw-rw-   0        0        0       22 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.7/BOFS/default/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/default/__pycache__/
--rw-rw-rw-   0        0        0      183 2022-05-18 21:12:21.000000 bride-of-frankensystem-1.9.3.7/BOFS/default/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      236 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.7/BOFS/default/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     6970 2022-07-15 22:13:35.000000 bride-of-frankensystem-1.9.3.7/BOFS/default/__pycache__/models.cpython-310.pyc
--rw-rw-rw-   0        0        0    15234 2024-04-18 00:04:57.000000 bride-of-frankensystem-1.9.3.7/BOFS/default/__pycache__/models.cpython-311.pyc
--rw-rw-rw-   0        0        0     9983 2022-07-15 22:13:35.000000 bride-of-frankensystem-1.9.3.7/BOFS/default/__pycache__/views.cpython-310.pyc
--rw-rw-rw-   0        0        0    23768 2024-04-16 20:43:42.000000 bride-of-frankensystem-1.9.3.7/BOFS/default/__pycache__/views.cpython-311.pyc
--rw-rw-rw-   0        0        0     9769 2024-04-17 23:42:26.000000 bride-of-frankensystem-1.9.3.7/BOFS/default/models.py
--rw-rw-rw-   0        0        0    18057 2024-04-16 20:43:36.000000 bride-of-frankensystem-1.9.3.7/BOFS/default/views.py
--rw-rw-rw-   0        0        0     2105 2024-04-15 22:13:58.000000 bride-of-frankensystem-1.9.3.7/BOFS/globals.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/
--rw-rw-rw-   0        0        0   103009 2024-04-06 05:46:45.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/all.min.css
--rw-rw-rw-   0        0        0   232803 2024-04-06 05:38:05.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/img/
--rw-rw-rw-   0        0        0     1235 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/img/check.png
--rw-rw-rw-   0        0        0    26229 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/img/spinner32.gif
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/js/
--rw-rw-rw-   0        0        0    80721 2024-04-06 05:35:59.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0    48036 2024-04-06 05:47:33.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/js/htmx.min.js
--rw-rw-rw-   0        0        0    87533 2024-04-06 05:34:06.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/js/jquery-3.7.1.min.js
--rw-rw-rw-   0        0        0      360 2024-04-06 05:47:54.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/js/json-enc.js
--rw-rw-rw-   0        0        0     9389 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/loading.gif
--rw-rw-rw-   0        0        0      253 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/logo.png
--rw-rw-rw-   0        0        0     2958 2024-04-07 19:19:18.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/style.css
--rw-rw-rw-   0        0        0     2060 2024-04-16 05:00:17.000000 bride-of-frankensystem-1.9.3.7/BOFS/static/style_admin.css
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/
--rw-rw-rw-   0        0        0     3650 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/consent.html
--rw-rw-rw-   0        0        0      651 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/end.html
--rw-rw-rw-   0        0        0     1188 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/external_id.html
--rw-rw-rw-   0        0        0      345 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/instructions.html
--rw-rw-rw-   0        0        0      319 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/questionnaire.html
--rw-rw-rw-   0        0        0     1521 2024-04-02 03:30:14.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/questionnaire_macro.html
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/questions/
--rw-rw-rw-   0        0        0      467 2024-04-02 03:24:53.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/questions/checklist.html
--rw-rw-rw-   0        0        0      426 2024-04-02 04:10:41.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/questions/drop_down.html
--rw-rw-rw-   0        0        0      321 2024-04-02 04:11:05.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/questions/field.html
--rw-rw-rw-   0        0        0      376 2024-04-02 04:11:25.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/questions/multi_field.html
--rw-rw-rw-   0        0        0      374 2024-04-02 04:11:53.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/questions/num_field.html
--rw-rw-rw-   0        0        0     1453 2024-04-02 05:17:59.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/questions/radiogrid.html
--rw-rw-rw-   0        0        0      672 2024-04-02 04:12:29.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/questions/radiolist.html
--rw-rw-rw-   0        0        0      541 2024-04-02 04:12:43.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/questions/slider.html
--rw-rw-rw-   0        0        0       26 2024-04-02 03:06:08.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/questions/textview.html
--rw-rw-rw-   0        0        0      136 2024-04-01 21:52:17.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/simple.html
--rw-rw-rw-   0        0        0     5696 2024-04-18 00:48:06.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/template.html
--rw-rw-rw-   0        0        0     3722 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/unity_webgl.html
--rw-rw-rw-   0        0        0     4224 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.7/BOFS/templates/unity_webgl_fullscreen.html
--rw-rw-rw-   0        0        0    12080 2024-04-16 04:19:29.000000 bride-of-frankensystem-1.9.3.7/BOFS/util.py
--rw-rw-rw-   0        0        0     7817 2022-05-18 16:56:46.000000 bride-of-frankensystem-1.9.3.7/LICENSE
--rw-rw-rw-   0        0        0       46 2024-04-05 20:45:50.000000 bride-of-frankensystem-1.9.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0    12537 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     2731 2024-03-27 04:18:48.000000 bride-of-frankensystem-1.9.3.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/bride_of_frankensystem.egg-info/
--rw-rw-rw-   0        0        0    12537 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/bride_of_frankensystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3805 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/bride_of_frankensystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/bride_of_frankensystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/bride_of_frankensystem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      106 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/bride_of_frankensystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/bride_of_frankensystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1057 2024-04-18 18:55:46.000000 bride-of-frankensystem-1.9.3.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 18:57:04.000000 bride-of-frankensystem-1.9.3.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:04.000000 bride-of-frankensystem-2.0.0.0/
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:03.000000 bride-of-frankensystem-2.0.0.0/BOFS/
+-rw-rw-rw-   0        0        0    15092 2024-04-18 18:52:52.000000 bride-of-frankensystem-2.0.0.0/BOFS/BOFSFlask.py
+-rw-rw-rw-   0        0        0     4026 2024-04-18 18:29:19.000000 bride-of-frankensystem-2.0.0.0/BOFS/BOFSSession.py
+-rw-rw-rw-   0        0        0    11154 2024-04-18 18:48:27.000000 bride-of-frankensystem-2.0.0.0/BOFS/JSONQuestionnaire.py
+-rw-rw-rw-   0        0        0     6858 2024-04-17 02:53:52.000000 bride-of-frankensystem-2.0.0.0/BOFS/JSONTable.py
+-rw-rw-rw-   0        0        0     5672 2024-04-15 21:33:28.000000 bride-of-frankensystem-2.0.0.0/BOFS/PageList.py
+-rw-rw-rw-   0        0        0      117 2024-01-06 23:57:32.000000 bride-of-frankensystem-2.0.0.0/BOFS/__init__.py
+-rw-rw-rw-   0        0        0       65 2024-01-06 23:57:32.000000 bride-of-frankensystem-2.0.0.0/BOFS/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:03.000000 bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/
+-rw-rw-rw-   0        0        0    20276 2024-04-18 18:56:00.000000 bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/BOFSFlask.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5496 2024-04-18 18:33:26.000000 bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/BOFSSession.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16585 2024-04-18 18:49:47.000000 bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/JSONQuestionnaire.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9903 2024-04-17 04:31:32.000000 bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/JSONTable.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6901 2024-04-15 22:13:05.000000 bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/PageList.cpython-311.pyc
+-rw-rw-rw-   0        0        0      384 2024-04-05 21:05:42.000000 bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      337 2024-04-06 05:50:26.000000 bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/__main__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     1998 2024-04-06 05:50:26.000000 bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/cli.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6221 2024-04-18 18:33:26.000000 bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/create_app.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3017 2024-04-15 22:14:27.000000 bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/globals.cpython-311.pyc
+-rw-rw-rw-   0        0        0    17284 2024-04-16 04:26:24.000000 bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/util.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:03.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/
+-rw-rw-rw-   0        0        0    12573 2024-04-18 18:43:43.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/Results.py
+-rw-rw-rw-   0        0        0      883 2024-04-17 19:42:01.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/SummaryStats.py
+-rw-rw-rw-   0        0        0       22 2024-01-19 17:54:15.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:03.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/
+-rw-rw-rw-   0        0        0    14271 2024-04-18 18:43:53.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/Results.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2059 2024-04-17 19:44:37.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/SummaryStats.cpython-311.pyc
+-rw-rw-rw-   0        0        0      181 2022-05-18 21:12:21.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      252 2024-01-19 17:54:16.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3420 2022-07-15 22:52:11.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/util.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8043 2024-04-15 22:36:04.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/util.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14352 2022-07-15 22:51:49.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/views.cpython-310.pyc
+-rw-rw-rw-   0        0        0    27556 2024-04-18 21:58:07.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/views.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:04.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/
+-rw-rw-rw-   0        0        0      844 2024-04-07 19:31:03.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/database_delete.html
+-rw-rw-rw-   0        0        0     1648 2024-04-17 06:00:53.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/export.html
+-rw-rw-rw-   0        0        0      304 2024-01-19 17:54:15.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/export_csv.html
+-rw-rw-rw-   0        0        0      877 2024-04-08 06:24:14.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/login_admin.html
+-rw-rw-rw-   0        0        0     2490 2024-04-08 04:55:02.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/preview_questionnaire.html
+-rw-rw-rw-   0        0        0      283 2024-04-02 04:25:23.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/preview_questionnaire_simple.html
+-rw-rw-rw-   0        0        0      606 2024-04-08 05:52:37.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/progress.html
+-rw-rw-rw-   0        0        0     2369 2024-04-08 05:37:40.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/progress_ajax.html
+-rw-rw-rw-   0        0        0     3196 2024-04-07 19:09:11.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/progress_summary_ajax.html
+-rw-rw-rw-   0        0        0     3517 2024-01-19 17:54:15.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/questionnaire_results.html
+-rw-rw-rw-   0        0        0     2020 2024-04-17 23:32:30.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/results.html
+-rw-rw-rw-   0        0        0      572 2024-04-17 23:31:16.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/results_boxplot.html
+-rw-rw-rw-   0        0        0     1366 2024-04-07 05:58:54.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/table_ajax.html
+-rw-rw-rw-   0        0        0     1056 2024-04-07 18:32:29.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/table_view.html
+-rw-rw-rw-   0        0        0     4872 2024-04-18 00:27:25.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/template_admin.html
+-rw-rw-rw-   0        0        0     1056 2024-04-07 19:28:04.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/template_admin_head.html
+-rw-rw-rw-   0        0        0     4427 2024-04-15 22:36:03.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/util.py
+-rw-rw-rw-   0        0        0    16244 2024-04-18 20:34:04.000000 bride-of-frankensystem-2.0.0.0/BOFS/admin/views.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:04.000000 bride-of-frankensystem-2.0.0.0/BOFS/bride_of_frankensystem.egg-info/
+-rw-rw-rw-   0        0        0    12537 2024-04-05 20:43:15.000000 bride-of-frankensystem-2.0.0.0/BOFS/bride_of_frankensystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2024-04-05 20:43:15.000000 bride-of-frankensystem-2.0.0.0/BOFS/bride_of_frankensystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 20:43:15.000000 bride-of-frankensystem-2.0.0.0/BOFS/bride_of_frankensystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-05 20:43:15.000000 bride-of-frankensystem-2.0.0.0/BOFS/bride_of_frankensystem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       85 2024-04-05 20:43:15.000000 bride-of-frankensystem-2.0.0.0/BOFS/bride_of_frankensystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-04-05 20:43:15.000000 bride-of-frankensystem-2.0.0.0/BOFS/bride_of_frankensystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1286 2024-01-07 00:02:19.000000 bride-of-frankensystem-2.0.0.0/BOFS/cli.py
+-rw-rw-rw-   0        0        0     5299 2024-04-18 18:29:19.000000 bride-of-frankensystem-2.0.0.0/BOFS/create_app.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:04.000000 bride-of-frankensystem-2.0.0.0/BOFS/default/
+-rw-rw-rw-   0        0        0       22 2023-09-28 18:15:44.000000 bride-of-frankensystem-2.0.0.0/BOFS/default/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:04.000000 bride-of-frankensystem-2.0.0.0/BOFS/default/__pycache__/
+-rw-rw-rw-   0        0        0      183 2022-05-18 21:12:21.000000 bride-of-frankensystem-2.0.0.0/BOFS/default/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      236 2023-09-28 18:15:44.000000 bride-of-frankensystem-2.0.0.0/BOFS/default/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6970 2022-07-15 22:13:35.000000 bride-of-frankensystem-2.0.0.0/BOFS/default/__pycache__/models.cpython-310.pyc
+-rw-rw-rw-   0        0        0    15234 2024-04-18 00:04:57.000000 bride-of-frankensystem-2.0.0.0/BOFS/default/__pycache__/models.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9983 2022-07-15 22:13:35.000000 bride-of-frankensystem-2.0.0.0/BOFS/default/__pycache__/views.cpython-310.pyc
+-rw-rw-rw-   0        0        0    23869 2024-04-18 19:50:09.000000 bride-of-frankensystem-2.0.0.0/BOFS/default/__pycache__/views.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9769 2024-04-17 23:42:26.000000 bride-of-frankensystem-2.0.0.0/BOFS/default/models.py
+-rw-rw-rw-   0        0        0    18115 2024-04-18 19:50:00.000000 bride-of-frankensystem-2.0.0.0/BOFS/default/views.py
+-rw-rw-rw-   0        0        0     2105 2024-04-15 22:13:58.000000 bride-of-frankensystem-2.0.0.0/BOFS/globals.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:04.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/
+-rw-rw-rw-   0        0        0   103009 2024-04-06 05:46:45.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/all.min.css
+-rw-rw-rw-   0        0        0   232803 2024-04-06 05:38:05.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:04.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/img/
+-rw-rw-rw-   0        0        0     1235 2023-09-28 18:15:44.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/img/check.png
+-rw-rw-rw-   0        0        0    26229 2023-09-28 18:15:44.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/img/spinner32.gif
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:04.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/js/
+-rw-rw-rw-   0        0        0    80721 2024-04-06 05:35:59.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0    48036 2024-04-06 05:47:33.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/js/htmx.min.js
+-rw-rw-rw-   0        0        0    87533 2024-04-06 05:34:06.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/js/jquery-3.7.1.min.js
+-rw-rw-rw-   0        0        0      360 2024-04-06 05:47:54.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/js/json-enc.js
+-rw-rw-rw-   0        0        0     9389 2023-09-28 18:15:44.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/loading.gif
+-rw-rw-rw-   0        0        0      253 2023-09-28 18:15:44.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/logo.png
+-rw-rw-rw-   0        0        0     2958 2024-04-07 19:19:18.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/style.css
+-rw-rw-rw-   0        0        0     2060 2024-04-16 05:00:17.000000 bride-of-frankensystem-2.0.0.0/BOFS/static/style_admin.css
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:04.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/
+-rw-rw-rw-   0        0        0     3650 2023-09-28 18:15:44.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/consent.html
+-rw-rw-rw-   0        0        0      651 2023-09-28 18:15:44.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/end.html
+-rw-rw-rw-   0        0        0     1188 2023-09-28 18:15:44.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/external_id.html
+-rw-rw-rw-   0        0        0      345 2023-09-28 18:15:44.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/instructions.html
+-rw-rw-rw-   0        0        0      319 2023-09-28 18:15:44.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/questionnaire.html
+-rw-rw-rw-   0        0        0     1521 2024-04-02 03:30:14.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/questionnaire_macro.html
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:04.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/questions/
+-rw-rw-rw-   0        0        0      467 2024-04-02 03:24:53.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/questions/checklist.html
+-rw-rw-rw-   0        0        0      426 2024-04-02 04:10:41.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/questions/drop_down.html
+-rw-rw-rw-   0        0        0      321 2024-04-02 04:11:05.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/questions/field.html
+-rw-rw-rw-   0        0        0      376 2024-04-02 04:11:25.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/questions/multi_field.html
+-rw-rw-rw-   0        0        0      374 2024-04-02 04:11:53.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/questions/num_field.html
+-rw-rw-rw-   0        0        0     1453 2024-04-02 05:17:59.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/questions/radiogrid.html
+-rw-rw-rw-   0        0        0      672 2024-04-02 04:12:29.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/questions/radiolist.html
+-rw-rw-rw-   0        0        0      541 2024-04-02 04:12:43.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/questions/slider.html
+-rw-rw-rw-   0        0        0       26 2024-04-02 03:06:08.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/questions/textview.html
+-rw-rw-rw-   0        0        0      136 2024-04-01 21:52:17.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/simple.html
+-rw-rw-rw-   0        0        0     5696 2024-04-18 00:48:06.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/template.html
+-rw-rw-rw-   0        0        0     3722 2023-09-28 18:15:44.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/unity_webgl.html
+-rw-rw-rw-   0        0        0     4224 2023-09-28 18:15:44.000000 bride-of-frankensystem-2.0.0.0/BOFS/templates/unity_webgl_fullscreen.html
+-rw-rw-rw-   0        0        0    12080 2024-04-16 04:19:29.000000 bride-of-frankensystem-2.0.0.0/BOFS/util.py
+-rw-rw-rw-   0        0        0     7817 2022-05-18 16:56:46.000000 bride-of-frankensystem-2.0.0.0/LICENSE
+-rw-rw-rw-   0        0        0       46 2024-04-05 20:45:50.000000 bride-of-frankensystem-2.0.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12801 2024-05-10 19:36:04.000000 bride-of-frankensystem-2.0.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2995 2024-04-18 20:38:35.000000 bride-of-frankensystem-2.0.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 19:36:04.000000 bride-of-frankensystem-2.0.0.0/bride_of_frankensystem.egg-info/
+-rw-rw-rw-   0        0        0    12801 2024-05-10 19:36:03.000000 bride-of-frankensystem-2.0.0.0/bride_of_frankensystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3805 2024-05-10 19:36:03.000000 bride-of-frankensystem-2.0.0.0/bride_of_frankensystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 19:36:03.000000 bride-of-frankensystem-2.0.0.0/bride_of_frankensystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-10 19:36:03.000000 bride-of-frankensystem-2.0.0.0/bride_of_frankensystem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      106 2024-05-10 19:36:03.000000 bride-of-frankensystem-2.0.0.0/bride_of_frankensystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-10 19:36:03.000000 bride-of-frankensystem-2.0.0.0/bride_of_frankensystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1057 2024-05-09 20:29:26.000000 bride-of-frankensystem-2.0.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 19:36:04.000000 bride-of-frankensystem-2.0.0.0/setup.cfg
```

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/BOFSFlask.py` & `bride-of-frankensystem-2.0.0.0/BOFS/BOFSFlask.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/BOFSSession.py` & `bride-of-frankensystem-2.0.0.0/BOFS/BOFSSession.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/JSONQuestionnaire.py` & `bride-of-frankensystem-2.0.0.0/BOFS/JSONQuestionnaire.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/JSONTable.py` & `bride-of-frankensystem-2.0.0.0/BOFS/JSONTable.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/PageList.py` & `bride-of-frankensystem-2.0.0.0/BOFS/PageList.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/BOFSFlask.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/BOFSFlask.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/BOFSSession.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/BOFSSession.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/JSONQuestionnaire.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/JSONQuestionnaire.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/JSONTable.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/JSONTable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/PageList.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/PageList.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/cli.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/create_app.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/create_app.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/globals.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/globals.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/__pycache__/util.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/__pycache__/util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/Results.py` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/Results.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/SummaryStats.py` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/SummaryStats.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/Results.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/Results.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/SummaryStats.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/SummaryStats.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/util.cpython-310.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/util.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/views.cpython-310.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/__pycache__/views.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/__pycache__/views.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x1a652166 (Thu Apr 18 18:23:22 2024 UTC)
-files sz: 17764
+moddate:  0xbc832166 (Thu Apr 18 20:34:04 2024 UTC)
+files sz: 16244
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x97005500640064016c005a00640064016c015a02640064026c036d045a
@@ -474,116 +474,116 @@
               1284 CALL                     0
    
    340        1294 PRECALL                  0
               1298 CALL                     0
    
    342        1308 STORE_NAME              63 (route_questionnaire_html)
    
-   392        1310 LOAD_CONST              57 (<code object table_data, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 392>)
+   357        1310 LOAD_CONST              57 (<code object table_data, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 357>)
               1312 MAKE_FUNCTION            0
               1314 STORE_NAME              64 (table_data)
    
-   409        1316 LOAD_NAME               40 (admin)
+   374        1316 LOAD_NAME               40 (admin)
               1318 LOAD_METHOD             43 (route)
               1340 LOAD_CONST              58 ('/table_view/<tableName>')
               1342 PRECALL                  1
               1346 CALL                     1
    
-   410        1356 LOAD_NAME               26 (verify_admin)
+   375        1356 LOAD_NAME               26 (verify_admin)
    
-   411        1358 LOAD_CONST              59 (<code object route_table_view, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 409>)
+   376        1358 LOAD_CONST              59 (<code object route_table_view, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 374>)
               1360 MAKE_FUNCTION            0
    
-   410        1362 PRECALL                  0
+   375        1362 PRECALL                  0
               1366 CALL                     0
    
-   409        1376 PRECALL                  0
+   374        1376 PRECALL                  0
               1380 CALL                     0
    
-   411        1390 STORE_NAME              65 (route_table_view)
+   376        1390 STORE_NAME              65 (route_table_view)
    
-   416        1392 LOAD_NAME               40 (admin)
+   381        1392 LOAD_NAME               40 (admin)
               1394 LOAD_METHOD             43 (route)
               1416 LOAD_CONST              60 ('/table_ajax/<tableName>')
               1418 PRECALL                  1
               1422 CALL                     1
    
-   417        1432 LOAD_NAME               26 (verify_admin)
+   382        1432 LOAD_NAME               26 (verify_admin)
    
-   418        1434 LOAD_CONST              61 (<code object route_table_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 416>)
+   383        1434 LOAD_CONST              61 (<code object route_table_ajax, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 381>)
               1436 MAKE_FUNCTION            0
    
-   417        1438 PRECALL                  0
+   382        1438 PRECALL                  0
               1442 CALL                     0
    
-   416        1452 PRECALL                  0
+   381        1452 PRECALL                  0
               1456 CALL                     0
    
-   418        1466 STORE_NAME              66 (route_table_ajax)
+   383        1466 STORE_NAME              66 (route_table_ajax)
    
-   423        1468 LOAD_NAME               40 (admin)
+   388        1468 LOAD_NAME               40 (admin)
               1470 LOAD_METHOD             43 (route)
               1492 LOAD_CONST              62 ('/table_csv/<tableName>')
               1494 PRECALL                  1
               1498 CALL                     1
    
-   424        1508 LOAD_NAME               26 (verify_admin)
+   389        1508 LOAD_NAME               26 (verify_admin)
    
-   425        1510 LOAD_CONST              63 (<code object route_table_csv, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 423>)
+   390        1510 LOAD_CONST              63 (<code object route_table_csv, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 388>)
               1512 MAKE_FUNCTION            0
    
-   424        1514 PRECALL                  0
+   389        1514 PRECALL                  0
               1518 CALL                     0
    
-   423        1528 PRECALL                  0
+   388        1528 PRECALL                  0
               1532 CALL                     0
    
-   425        1542 STORE_NAME              67 (route_table_csv)
+   390        1542 STORE_NAME              67 (route_table_csv)
    
-   443        1544 LOAD_NAME               40 (admin)
+   408        1544 LOAD_NAME               40 (admin)
               1546 LOAD_METHOD             43 (route)
               1568 LOAD_CONST              64 ('/database_download')
               1570 PRECALL                  1
               1574 CALL                     1
    
-   444        1584 LOAD_NAME               26 (verify_admin)
+   409        1584 LOAD_NAME               26 (verify_admin)
    
-   445        1586 LOAD_CONST              65 (<code object route_database_download, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 443>)
+   410        1586 LOAD_CONST              65 (<code object route_database_download, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 408>)
               1588 MAKE_FUNCTION            0
    
-   444        1590 PRECALL                  0
+   409        1590 PRECALL                  0
               1594 CALL                     0
    
-   443        1604 PRECALL                  0
+   408        1604 PRECALL                  0
               1608 CALL                     0
    
-   445        1618 STORE_NAME              68 (route_database_download)
+   410        1618 STORE_NAME              68 (route_database_download)
    
-   454        1620 LOAD_NAME               40 (admin)
+   419        1620 LOAD_NAME               40 (admin)
               1622 LOAD_METHOD             43 (route)
               1644 LOAD_CONST              66 ('/database_delete')
               1646 LOAD_CONST              25 ('GET')
               1648 LOAD_CONST              26 ('POST')
               1650 BUILD_LIST               2
               1652 KW_NAMES                27
               1654 PRECALL                  2
               1658 CALL                     2
    
-   455        1668 LOAD_NAME               26 (verify_admin)
+   420        1668 LOAD_NAME               26 (verify_admin)
    
-   456        1670 LOAD_CONST              67 (<code object route_database_delete, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 454>)
+   421        1670 LOAD_CONST              67 (<code object route_database_delete, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 419>)
               1672 MAKE_FUNCTION            0
    
-   455        1674 PRECALL                  0
+   420        1674 PRECALL                  0
               1678 CALL                     0
    
-   454        1688 PRECALL                  0
+   419        1688 PRECALL                  0
               1692 CALL                     0
    
-   456        1702 STORE_NAME              69 (route_database_delete)
+   421        1702 STORE_NAME              69 (route_database_delete)
               1704 LOAD_CONST               1 (None)
               1706 RETURN_VALUE
    consts
       0
       None
       ('Blueprint', 'render_template', 'current_app', 'redirect', 'g', 'request', 'session', 'url_for', 'Response', 'send_file')
       2
@@ -2494,33 +2494,32 @@
          name       'route_results'
          firstlineno 283
          lnotab 0x02032402
       '/results_boxplot/<path:field_name>'
       'field_name'
       code
          argcount  : 1
-         nlocals   : 10
+         nlocals   : 9
          stacksize : 6
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000005c
             0300007d017d027d037c02640119000000000000000000a0010000000000
             000000000000000000000000000000a6000000ab000000000000000000a0
             020000000000000000000000000000000000000000a6000000ab00000000
             00000000007d047c04a00300000000000000000000000000000000000000
-            00a6000000ab000000000000000000010067007d057c0444005d6d7d067c
+            00a6000000ab000000000000000000010067007d057c0444005d597d067c
             026a0400000000000000007c026a0500000000000000007c066b02000000
-            00190000000000000000007d077c07a00600000000000000000000000000
-            00000000000000a6000000ab0000000000000000007d087c077c00190000
-            00000000000000a0070000000000000000000000000000000000000000a6
-            000000ab0000000000000000007411000000000000000000007c06a60100
-            00ab0100000000000000006402640364049c047d097c05a0090000000000
-            0000000000000000000000000000007c09a6010000ab0100000000000000
-            0001008c6e74150000000000000000000064057c007c05ac06a6030000ab
-            0300000000000000005300
+            00190000000000000000007d077c077c0019000000000000000000a00600
+            00000000000000000000000000000000000000a6000000ab000000000000
+            000000740f000000000000000000007c06a6010000ab0100000000000000
+            006402640364049c047d087c05a008000000000000000000000000000000
+            00000000007c08a6010000ab01000000000000000001008c5a7413000000
+            0000000000000064057c007c05ac06a6030000ab03000000000000000053
+            00
          290           0 RESUME                   0
          
          293           2 LOAD_GLOBAL              1 (NULL + calculate_results)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 UNPACK_SEQUENCE          3
                       32 STORE_FAST               1 (results)
@@ -2545,84 +2544,78 @@
                      164 POP_TOP
          
          297         166 BUILD_LIST               0
                      168 STORE_FAST               5 (plot_data)
          
          299         170 LOAD_FAST                4 (unique_conditions)
                      172 GET_ITER
-                 >>  174 FOR_ITER               109 (to 394)
+                 >>  174 FOR_ITER                89 (to 354)
                      176 STORE_FAST               6 (condition)
          
          300         178 LOAD_FAST                2 (df)
                      180 LOAD_ATTR                4 (loc)
                      190 LOAD_FAST                2 (df)
                      192 LOAD_ATTR                5 (condition)
                      202 LOAD_FAST                6 (condition)
                      204 COMPARE_OP               2 (==)
                      210 BINARY_SUBSCR
                      220 STORE_FAST               7 (df_part)
          
-         301         222 LOAD_FAST                7 (df_part)
-                     224 LOAD_METHOD              6 (count)
-                     246 PRECALL                  0
-                     250 CALL                     0
-                     260 STORE_FAST               8 (count)
-         
-         304         262 LOAD_FAST                7 (df_part)
-                     264 LOAD_FAST                0 (field_name)
-                     266 BINARY_SUBSCR
-                     276 LOAD_METHOD              7 (to_list)
-                     298 PRECALL                  0
-                     302 CALL                     0
-         
-         306         312 LOAD_GLOBAL             17 (NULL + str)
-                     324 LOAD_FAST                6 (condition)
-                     326 PRECALL                  1
-                     330 CALL                     1
-         
-         307         340 LOAD_CONST               2 ('box')
-         
-         308         342 LOAD_CONST               3 ('Outliers')
-         
-         303         344 LOAD_CONST               4 (('y', 'name', 'type', 'boxpoints'))
-                     346 BUILD_CONST_KEY_MAP      4
-                     348 STORE_FAST               9 (data)
-         
-         310         350 LOAD_FAST                5 (plot_data)
-                     352 LOAD_METHOD              9 (append)
-                     374 LOAD_FAST                9 (data)
-                     376 PRECALL                  1
-                     380 CALL                     1
-                     390 POP_TOP
-                     392 JUMP_BACKWARD          110 (to 174)
-         
-         312     >>  394 LOAD_GLOBAL             21 (NULL + render_template)
-                     406 LOAD_CONST               5 ('results_boxplot.html')
-                     408 LOAD_FAST                0 (field_name)
-                     410 LOAD_FAST                5 (plot_data)
-                     412 KW_NAMES                 6
-                     414 PRECALL                  3
-                     418 CALL                     3
-                     428 RETURN_VALUE
+         304         222 LOAD_FAST                7 (df_part)
+                     224 LOAD_FAST                0 (field_name)
+                     226 BINARY_SUBSCR
+                     236 LOAD_METHOD              6 (to_list)
+                     258 PRECALL                  0
+                     262 CALL                     0
+         
+         306         272 LOAD_GLOBAL             15 (NULL + str)
+                     284 LOAD_FAST                6 (condition)
+                     286 PRECALL                  1
+                     290 CALL                     1
+         
+         307         300 LOAD_CONST               2 ('box')
+         
+         308         302 LOAD_CONST               3 ('Outliers')
+         
+         303         304 LOAD_CONST               4 (('y', 'name', 'type', 'boxpoints'))
+                     306 BUILD_CONST_KEY_MAP      4
+                     308 STORE_FAST               8 (data)
+         
+         310         310 LOAD_FAST                5 (plot_data)
+                     312 LOAD_METHOD              8 (append)
+                     334 LOAD_FAST                8 (data)
+                     336 PRECALL                  1
+                     340 CALL                     1
+                     350 POP_TOP
+                     352 JUMP_BACKWARD           90 (to 174)
+         
+         312     >>  354 LOAD_GLOBAL             19 (NULL + render_template)
+                     366 LOAD_CONST               5 ('results_boxplot.html')
+                     368 LOAD_FAST                0 (field_name)
+                     370 LOAD_FAST                5 (plot_data)
+                     372 KW_NAMES                 6
+                     374 PRECALL                  3
+                     378 CALL                     3
+                     388 RETURN_VALUE
          consts
             None
             'condition'
             'box'
             'Outliers'
             ('y', 'name', 'type', 'boxpoints')
             'results_boxplot.html'
             ('field_name', 'plot_data')
-         names      ('calculate_results', 'unique', 'tolist', 'sort', 'loc', 'condition', 'count', 'to_list', 'str', 'append', 'render_template')
-         varnames   ('field_name', 'results', 'df', 'summary_stats', 'unique_conditions', 'plot_data', 'condition', 'df_part', 'count', 'data')
+         names      ('calculate_results', 'unique', 'tolist', 'sort', 'loc', 'condition', 'to_list', 'str', 'append', 'render_template')
+         varnames   ('field_name', 'results', 'df', 'summary_stats', 'unique_conditions', 'plot_data', 'condition', 'df_part', 'data')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_results_boxplot'
          firstlineno 290
-         lnotab 0x0203240258012801040208012c01280332021c01020102fb06072c02
+         lnotab 0x0203240258012801040208012c0432021c01020102fb06072c02
       '/preview_questionnaire/<questionnaireName>'
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
@@ -2930,86 +2923,86 @@
             00000000007d047c04a00900000000000000000000000000000000000000
             006401a6010000ab01000000000000000073157c04a00900000000000000
             000000000000000000000000006402a6010000ab01000000000000000072
             0264037d047c036a0a00000000000000007c04a00b000000000000000000
             0000000000000000000000a6000000ab00000000000000000064049c027d
             057c02a00c00000000000000000000000000000000000000007c05a60100
             00ab01000000000000000001008c747c027c0166025300
-         392           0 RESUME                   0
+         357           0 RESUME                   0
          
-         393           2 LOAD_GLOBAL              0 (db)
+         358           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_ATTR                1 (session)
                       24 LOAD_METHOD              2 (query)
                       46 LOAD_GLOBAL              0 (db)
                       58 LOAD_ATTR                3 (metadata)
                       68 LOAD_ATTR                4 (tables)
                       78 LOAD_FAST                0 (tableName)
                       80 BINARY_SUBSCR
                       90 PRECALL                  1
                       94 CALL                     1
                      104 LOAD_METHOD              5 (all)
                      126 PRECALL                  0
                      130 CALL                     0
                      140 STORE_FAST               1 (rows)
          
-         395         142 BUILD_LIST               0
+         360         142 BUILD_LIST               0
                      144 STORE_FAST               2 (columns)
          
-         397         146 LOAD_GLOBAL              0 (db)
+         362         146 LOAD_GLOBAL              0 (db)
                      158 LOAD_ATTR                3 (metadata)
                      168 LOAD_ATTR                4 (tables)
                      178 LOAD_FAST                0 (tableName)
                      180 BINARY_SUBSCR
                      190 LOAD_ATTR                6 (columns)
                      200 GET_ITER
                  >>  202 FOR_ITER               115 (to 434)
                      204 STORE_FAST               3 (c)
          
-         398         206 LOAD_GLOBAL             15 (NULL + str)
+         363         206 LOAD_GLOBAL             15 (NULL + str)
                      218 LOAD_FAST                3 (c)
                      220 LOAD_ATTR                8 (type)
                      230 PRECALL                  1
                      234 CALL                     1
                      244 STORE_FAST               4 (type)
          
-         399         246 LOAD_FAST                4 (type)
+         364         246 LOAD_FAST                4 (type)
                      248 LOAD_METHOD              9 (startswith)
                      270 LOAD_CONST               1 ('VARCHAR')
                      272 PRECALL                  1
                      276 CALL                     1
                      286 POP_JUMP_FORWARD_IF_TRUE    21 (to 330)
                      288 LOAD_FAST                4 (type)
                      290 LOAD_METHOD              9 (startswith)
                      312 LOAD_CONST               2 ('TEXT')
                      314 PRECALL                  1
                      318 CALL                     1
                      328 POP_JUMP_FORWARD_IF_FALSE     2 (to 334)
          
-         400     >>  330 LOAD_CONST               3 ('string')
+         365     >>  330 LOAD_CONST               3 ('string')
                      332 STORE_FAST               4 (type)
          
-         402     >>  334 LOAD_FAST                3 (c)
+         367     >>  334 LOAD_FAST                3 (c)
                      336 LOAD_ATTR               10 (description)
                      346 LOAD_FAST                4 (type)
                      348 LOAD_METHOD             11 (lower)
                      370 PRECALL                  0
                      374 CALL                     0
                      384 LOAD_CONST               4 (('name', 'type'))
                      386 BUILD_CONST_KEY_MAP      2
                      388 STORE_FAST               5 (column)
          
-         404         390 LOAD_FAST                2 (columns)
+         369         390 LOAD_FAST                2 (columns)
                      392 LOAD_METHOD             12 (append)
                      414 LOAD_FAST                5 (column)
                      416 PRECALL                  1
                      420 CALL                     1
                      430 POP_TOP
                      432 JUMP_BACKWARD          116 (to 202)
          
-         406     >>  434 LOAD_FAST                2 (columns)
+         371     >>  434 LOAD_FAST                2 (columns)
                      436 LOAD_FAST                1 (rows)
                      438 BUILD_TUPLE              2
                      440 RETURN_VALUE
          consts
             None
             'VARCHAR'
             'TEXT'
@@ -3017,37 +3010,37 @@
             ('name', 'type')
          names      ('db', 'session', 'query', 'metadata', 'tables', 'all', 'columns', 'str', 'type', 'startswith', 'description', 'lower', 'append')
          varnames   ('tableName', 'rows', 'columns', 'c', 'type', 'column')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'table_data'
-         firstlineno 392
+         firstlineno 357
          lnotab 0x02018c0204023c0128015401040238022c02
       '/table_view/<tableName>'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             005c0200007d017d0274030000000000000000000064017c007c027c01ac
             02a6040000ab0400000000000000005300
-         409           0 RESUME                   0
+         374           0 RESUME                   0
          
-         412           2 LOAD_GLOBAL              1 (NULL + table_data)
+         377           2 LOAD_GLOBAL              1 (NULL + table_data)
                       14 LOAD_FAST                0 (tableName)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 UNPACK_SEQUENCE          2
                       34 STORE_FAST               1 (columns)
                       36 STORE_FAST               2 (rows)
          
-         413          38 LOAD_GLOBAL              3 (NULL + render_template)
+         378          38 LOAD_GLOBAL              3 (NULL + render_template)
                       50 LOAD_CONST               1 ('table_view.html')
                       52 LOAD_FAST                0 (tableName)
                       54 LOAD_FAST                2 (rows)
                       56 LOAD_FAST                1 (columns)
                       58 KW_NAMES                 2
                       60 PRECALL                  4
                       64 CALL                     4
@@ -3058,37 +3051,37 @@
             ('tableName', 'rows', 'columns')
          names      ('table_data', 'render_template')
          varnames   ('tableName', 'columns', 'rows')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_table_view'
-         firstlineno 409
+         firstlineno 374
          lnotab 0x02032401
       '/table_ajax/<tableName>'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             005c0200007d017d0274030000000000000000000064017c027c01ac02a6
             030000ab0300000000000000005300
-         416           0 RESUME                   0
+         381           0 RESUME                   0
          
-         419           2 LOAD_GLOBAL              1 (NULL + table_data)
+         384           2 LOAD_GLOBAL              1 (NULL + table_data)
                       14 LOAD_FAST                0 (tableName)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 UNPACK_SEQUENCE          2
                       34 STORE_FAST               1 (columns)
                       36 STORE_FAST               2 (rows)
          
-         420          38 LOAD_GLOBAL              3 (NULL + render_template)
+         385          38 LOAD_GLOBAL              3 (NULL + render_template)
                       50 LOAD_CONST               1 ('table_ajax.html')
                       52 LOAD_FAST                2 (rows)
                       54 LOAD_FAST                1 (columns)
                       56 KW_NAMES                 2
                       58 PRECALL                  3
                       62 CALL                     3
                       72 RETURN_VALUE
@@ -3098,15 +3091,15 @@
             ('rows', 'columns')
          names      ('table_data', 'render_template')
          varnames   ('tableName', 'columns', 'rows')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_table_ajax'
-         firstlineno 416
+         firstlineno 381
          lnotab 0x02032401
       '/table_csv/<tableName>'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 10
          flags     : 3
@@ -3122,57 +3115,57 @@
             0000000000000000007c036406640764087c0064097a0000007409000000
             000000000000006a050000000000000000a6000000ab0000000000000000
             00a0060000000000000000000000000000000000000000640aa6010000ab
             0100000000000000007a0000007a0600006901ac0ba6030000ab03000000
             00000000005300
                        0 MAKE_CELL                5 (row)
          
-         423           2 RESUME                   0
+         388           2 RESUME                   0
          
-         426           4 LOAD_GLOBAL              1 (NULL + table_data)
+         391           4 LOAD_GLOBAL              1 (NULL + table_data)
                       16 LOAD_FAST                0 (tableName)
                       18 PRECALL                  1
                       22 CALL                     1
                       32 UNPACK_SEQUENCE          2
                       36 STORE_FAST               1 (columns)
                       38 STORE_FAST               2 (rows)
          
-         428          40 LOAD_CONST               1 ('')
+         393          40 LOAD_CONST               1 ('')
                       42 STORE_FAST               3 (csv)
          
-         429          44 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 429>)
+         394          44 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 394>)
                       46 MAKE_FUNCTION            0
                       48 LOAD_FAST                1 (columns)
                       50 GET_ITER
                       52 PRECALL                  0
                       56 CALL                     0
                       66 STORE_FAST               4 (headers)
          
-         430          68 LOAD_FAST                3 (csv)
+         395          68 LOAD_FAST                3 (csv)
                       70 LOAD_CONST               3 (',')
                       72 LOAD_METHOD              1 (join)
                       94 LOAD_FAST                4 (headers)
                       96 PRECALL                  1
                      100 CALL                     1
                      110 LOAD_CONST               4 ('\n')
                      112 BINARY_OP                0 (+)
                      116 BINARY_OP               13 (+=)
                      120 STORE_FAST               3 (csv)
          
-         432         122 LOAD_FAST                2 (rows)
+         397         122 LOAD_FAST                2 (rows)
                      124 GET_ITER
                  >>  126 FOR_ITER                54 (to 236)
                      128 STORE_DEREF              5 (row)
          
-         433         130 LOAD_FAST                3 (csv)
+         398         130 LOAD_FAST                3 (csv)
                      132 LOAD_CONST               3 (',')
                      134 LOAD_METHOD              1 (join)
                      156 LOAD_CLOSURE             5 (row)
                      158 BUILD_TUPLE              1
-                     160 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 433>)
+                     160 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\colby\Desktop\git\bride-of-frankensystem-examples\venv\Lib\site-packages\BOFS\admin\views.py", line 398>)
                      162 MAKE_FUNCTION            8 (closure)
                      164 LOAD_GLOBAL              5 (NULL + enumerate)
                      176 LOAD_FAST                1 (columns)
                      178 PRECALL                  1
                      182 CALL                     1
                      192 GET_ITER
                      194 PRECALL                  0
@@ -3181,55 +3174,55 @@
                      212 CALL                     1
                      222 LOAD_CONST               4 ('\n')
                      224 BINARY_OP                0 (+)
                      228 BINARY_OP               13 (+=)
                      232 STORE_FAST               3 (csv)
                      234 JUMP_BACKWARD           55 (to 126)
          
-         435     >>  236 LOAD_GLOBAL              7 (NULL + Response)
+         400     >>  236 LOAD_GLOBAL              7 (NULL + Response)
                      248 LOAD_FAST                3 (csv)
          
-         436         250 LOAD_CONST               6 ('text/csv')
+         401         250 LOAD_CONST               6 ('text/csv')
          
-         438         252 LOAD_CONST               7 ('Content-disposition')
+         403         252 LOAD_CONST               7 ('Content-disposition')
                      254 LOAD_CONST               8 ('attachment; filename=%s.csv')
          
-         439         256 LOAD_FAST                0 (tableName)
+         404         256 LOAD_FAST                0 (tableName)
                      258 LOAD_CONST               9 ('_')
                      260 BINARY_OP                0 (+)
                      264 LOAD_GLOBAL              9 (NULL + datetime)
                      276 LOAD_ATTR                5 (utcnow)
                      286 PRECALL                  0
                      290 CALL                     0
                      300 LOAD_METHOD              6 (strftime)
                      322 LOAD_CONST              10 ('%Y-%m-%d')
                      324 PRECALL                  1
                      328 CALL                     1
                      338 BINARY_OP                0 (+)
          
-         438         342 BINARY_OP                6 (%)
+         403         342 BINARY_OP                6 (%)
          
-         437         346 BUILD_MAP                1
+         402         346 BUILD_MAP                1
          
-         435         348 KW_NAMES                11
+         400         348 KW_NAMES                11
                      350 PRECALL                  3
                      354 CALL                     3
                      364 RETURN_VALUE
          consts
             None
             ''
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 19
                code
                   0x970067007c005d0a7d017c0164001900000000000000000091028c0b53
                   00
-               429           0 RESUME                   0
+               394           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                10 (to 28)
                              8 STORE_FAST               1 (c)
                             10 LOAD_FAST                1 (c)
                             12 LOAD_CONST               0 ('name')
                             14 BINARY_SUBSCR
@@ -3240,30 +3233,30 @@
                   'name'
                names      ()
                varnames   ('.0', 'c')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
                name       '<listcomp>'
-               firstlineno 429
+               firstlineno 394
                lnotab 0x
             ','
             '\n'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 19
                code
                   0x9501970067007c005d1a5c0200007d017d027401000000000000000000
                   0089037c0119000000000000000000a6010000ab01000000000000000091
                   028c1b5300
                              0 COPY_FREE_VARS           1
                
-               433           2 RESUME                   0
+               398           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                26 (to 62)
                             10 UNPACK_SEQUENCE          2
                             14 STORE_FAST               1 (i)
                             16 STORE_FAST               2 (c)
                             18 LOAD_GLOBAL              1 (NULL + escape_csv)
@@ -3278,29 +3271,29 @@
                consts
                names      ('escape_csv',)
                varnames   ('.0', 'i', 'c')
                freevars   ('row',)
                cellvars   ()
                filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
                name       '<listcomp>'
-               firstlineno 433
+               firstlineno 398
                lnotab 0x
             'text/csv'
             'Content-disposition'
             'attachment; filename=%s.csv'
             '_'
             '%Y-%m-%d'
             ('mimetype', 'headers')
          names      ('table_data', 'join', 'enumerate', 'Response', 'datetime', 'utcnow', 'strftime')
          varnames   ('tableName', 'columns', 'rows', 'csv', 'headers')
          freevars   ()
          cellvars   ('row',)
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_table_csv'
-         firstlineno 423
+         firstlineno 388
          lnotab 0x0403240204011801360208016a020e010202040156ff04ff02fe
       '/database_download'
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 4
          flags     : 3
@@ -3308,41 +3301,41 @@
             0x97007400000000000000000000006a0100000000000000006401190000
             00000000000000a002000000000000000000000000000000000000000064
             02a6010000ab010000000000000000730264035300740000000000000000
             0000006a010000000000000000640119000000000000000000a003000000
             000000000000000000000000000000000064026404a6020000ab02000000
             00000000007d007409000000000000000000007c006405ac06a6020000ab
             0200000000000000005300
-         443           0 RESUME                   0
+         408           0 RESUME                   0
          
-         446           2 LOAD_GLOBAL              0 (current_app)
+         411           2 LOAD_GLOBAL              0 (current_app)
                       14 LOAD_ATTR                1 (config)
                       24 LOAD_CONST               1 ('SQLALCHEMY_DATABASE_URI')
                       26 BINARY_SUBSCR
                       36 LOAD_METHOD              2 (startswith)
                       58 LOAD_CONST               2 ('sqlite:///')
                       60 PRECALL                  1
                       64 CALL                     1
                       74 POP_JUMP_FORWARD_IF_TRUE     2 (to 80)
          
-         447          76 LOAD_CONST               3 ('Not using a SQLite database.')
+         412          76 LOAD_CONST               3 ('Not using a SQLite database.')
                       78 RETURN_VALUE
          
-         449     >>   80 LOAD_GLOBAL              0 (current_app)
+         414     >>   80 LOAD_GLOBAL              0 (current_app)
                       92 LOAD_ATTR                1 (config)
                      102 LOAD_CONST               1 ('SQLALCHEMY_DATABASE_URI')
                      104 BINARY_SUBSCR
                      114 LOAD_METHOD              3 (replace)
                      136 LOAD_CONST               2 ('sqlite:///')
                      138 LOAD_CONST               4 ('')
                      140 PRECALL                  2
                      144 CALL                     2
                      154 STORE_FAST               0 (db_uri)
          
-         451         156 LOAD_GLOBAL              9 (NULL + send_file)
+         416         156 LOAD_GLOBAL              9 (NULL + send_file)
                      168 LOAD_FAST                0 (db_uri)
                      170 LOAD_CONST               5 (True)
                      172 KW_NAMES                 6
                      174 PRECALL                  2
                      178 CALL                     2
                      188 RETURN_VALUE
          consts
@@ -3355,15 +3348,15 @@
             ('as_attachment',)
          names      ('current_app', 'config', 'startswith', 'replace', 'send_file')
          varnames   ('db_uri',)
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_database_download'
-         firstlineno 443
+         firstlineno 408
          lnotab 0x02034a0104024c02
       '/database_delete'
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 7
          flags     : 3
@@ -3390,67 +3383,67 @@
             007c01a6010000ab010000000000000000a0120000000000000000000000
             000000000000000000a6000000ab00000000000000000001008c34741a00
             0000000000000000006a100000000000000000a013000000000000000000
             0000000000000000000000a6000000ab0000000000000000000100742900
             000000000000000000742b00000000000000000000640ea6010000ab0100
             00000000000000a6010000ab0100000000000000005300740d0000000000
             00000000006407a6010000ab0100000000000000005300
-         454           0 RESUME                   0
+         419           0 RESUME                   0
          
-         457           2 LOAD_GLOBAL              0 (current_app)
+         422           2 LOAD_GLOBAL              0 (current_app)
                       14 LOAD_ATTR                1 (config)
                       24 LOAD_CONST               1 ('SQLALCHEMY_DATABASE_URI')
                       26 BINARY_SUBSCR
                       36 LOAD_METHOD              2 (startswith)
                       58 LOAD_CONST               2 ('sqlite:///')
                       60 PRECALL                  1
                       64 CALL                     1
                       74 POP_JUMP_FORWARD_IF_TRUE     2 (to 80)
          
-         458          76 LOAD_CONST               3 ('Not using a SQLite database.')
+         423          76 LOAD_CONST               3 ('Not using a SQLite database.')
                       78 RETURN_VALUE
          
-         460     >>   80 LOAD_GLOBAL              6 (request)
+         425     >>   80 LOAD_GLOBAL              6 (request)
                       92 LOAD_ATTR                4 (method)
                      102 LOAD_CONST               4 ('POST')
                      104 COMPARE_OP               2 (==)
                      110 EXTENDED_ARG             1
                      112 POP_JUMP_FORWARD_IF_FALSE   314 (to 742)
          
-         461         114 LOAD_GLOBAL              6 (request)
+         426         114 LOAD_GLOBAL              6 (request)
                      126 LOAD_ATTR                5 (form)
                      136 LOAD_CONST               5 ('password')
                      138 BINARY_SUBSCR
                      148 LOAD_GLOBAL              0 (current_app)
                      160 LOAD_ATTR                1 (config)
                      170 LOAD_CONST               6 ('ADMIN_PASSWORD')
                      172 BINARY_SUBSCR
                      182 COMPARE_OP               3 (!=)
                      188 POP_JUMP_FORWARD_IF_FALSE    17 (to 224)
          
-         462         190 LOAD_GLOBAL             13 (NULL + render_template)
+         427         190 LOAD_GLOBAL             13 (NULL + render_template)
                      202 LOAD_CONST               7 ('database_delete.html')
                      204 LOAD_CONST               8 ('The password you entered is incorrect.')
                      206 KW_NAMES                 9
                      208 PRECALL                  2
                      212 CALL                     2
                      222 RETURN_VALUE
          
-         464     >>  224 LOAD_GLOBAL              0 (current_app)
+         429     >>  224 LOAD_GLOBAL              0 (current_app)
                      236 LOAD_ATTR                1 (config)
                      246 LOAD_CONST               1 ('SQLALCHEMY_DATABASE_URI')
                      248 BINARY_SUBSCR
                      258 LOAD_METHOD              7 (replace)
                      280 LOAD_CONST               2 ('sqlite:///')
                      282 LOAD_CONST              10 ('')
                      284 PRECALL                  2
                      288 CALL                     2
                      298 STORE_FAST               0 (db_uri)
          
-         465         300 LOAD_GLOBAL             17 (NULL + copyfile)
+         430         300 LOAD_GLOBAL             17 (NULL + copyfile)
                      312 LOAD_FAST                0 (db_uri)
                      314 LOAD_FAST                0 (db_uri)
                      316 LOAD_METHOD              7 (replace)
                      338 LOAD_CONST              11 ('.db')
                      340 LOAD_CONST              10 ('')
                      342 PRECALL                  2
                      346 CALL                     2
@@ -3467,53 +3460,53 @@
                      436 BINARY_OP                0 (+)
                      440 LOAD_CONST              11 ('.db')
                      442 BINARY_OP                0 (+)
                      446 PRECALL                  2
                      450 CALL                     2
                      460 POP_TOP
          
-         468         462 LOAD_GLOBAL             25 (NULL + reversed)
+         433         462 LOAD_GLOBAL             25 (NULL + reversed)
                      474 LOAD_GLOBAL             26 (db)
                      486 LOAD_ATTR               14 (metadata)
                      496 LOAD_ATTR               15 (sorted_tables)
                      506 PRECALL                  1
                      510 CALL                     1
                      520 GET_ITER
                  >>  522 FOR_ITER                51 (to 626)
                      524 STORE_FAST               1 (tbl)
          
-         469         526 LOAD_GLOBAL             26 (db)
+         434         526 LOAD_GLOBAL             26 (db)
                      538 LOAD_ATTR               16 (session)
                      548 LOAD_METHOD             17 (query)
                      570 LOAD_FAST                1 (tbl)
                      572 PRECALL                  1
                      576 CALL                     1
                      586 LOAD_METHOD             18 (delete)
                      608 PRECALL                  0
                      612 CALL                     0
                      622 POP_TOP
                      624 JUMP_BACKWARD           52 (to 522)
          
-         470     >>  626 LOAD_GLOBAL             26 (db)
+         435     >>  626 LOAD_GLOBAL             26 (db)
                      638 LOAD_ATTR               16 (session)
                      648 LOAD_METHOD             19 (commit)
                      670 PRECALL                  0
                      674 CALL                     0
                      684 POP_TOP
          
-         472         686 LOAD_GLOBAL             41 (NULL + redirect)
+         437         686 LOAD_GLOBAL             41 (NULL + redirect)
                      698 LOAD_GLOBAL             43 (NULL + url_for)
                      710 LOAD_CONST              14 ('admin.route_progress')
                      712 PRECALL                  1
                      716 CALL                     1
                      726 PRECALL                  1
                      730 CALL                     1
                      740 RETURN_VALUE
          
-         474     >>  742 LOAD_GLOBAL             13 (NULL + render_template)
+         439     >>  742 LOAD_GLOBAL             13 (NULL + render_template)
                      754 LOAD_CONST               7 ('database_delete.html')
                      756 PRECALL                  1
                      760 CALL                     1
                      770 RETURN_VALUE
          consts
             None
             'SQLALCHEMY_DATABASE_URI'
@@ -3532,15 +3525,15 @@
             'admin.route_progress'
          names      ('current_app', 'config', 'startswith', 'request', 'method', 'form', 'render_template', 'replace', 'copyfile', 'datetime', 'utcnow', 'strftime', 'reversed', 'db', 'metadata', 'sorted_tables', 'session', 'query', 'delete', 'commit', 'redirect', 'url_for')
          varnames   ('db_uri', 'tbl')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
          name       'route_database_delete'
-         firstlineno 454
+         firstlineno 419
          lnotab 0x02034a01040222014c0122024c01a203400164013c023802
    names      ('os', 'pandas', 'pd', 'flask', 'Blueprint', 'render_template', 'current_app', 'redirect', 'g', 'request', 'session', 'url_for', 'Response', 'send_file', '', 'BOFSFlask', 'globals', 'db', 'questionnaires', 'page_list', 'util', 'fetch_condition_count', 'display_time', 'provide_consent', 'int_or_0', 'sqlalchemy_to_json', 'verify_admin', 'escape_csv', 'questionnaire_name_and_tag', 'condition_num_to_label', 'Results', 'json', 'SummaryStats', 'datetime', 'path', 'listdir', 'shutil', 'copyfile', '__annotations__', '__name__', 'admin', 'context_processor', 'inject_template_vars', 'route', 'admin_index', 'admin_login', 'fetch_progress', 'fetch_progress_summary', 'route_progress', 'route_progress_ajax', 'route_progress_summary_ajax', 'post', 'route_update_exclude_from_count', 'route_export_item_timing', 'route_export', 'tuple', 'DataFrame', 'dict', 'str', 'calculate_results', 'route_results', 'route_results_boxplot', 'route_preview_questionnaire', 'route_questionnaire_html', 'table_data', 'route_table_view', 'route_table_ajax', 'route_table_csv', 'route_database_download', 'route_database_delete')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\admin\\views.py'
    name       '<module>'
@@ -3548,10 +3541,10 @@
    lnotab
       0x00ff02010a01080130010c01140118011c010c0108010c010c0110010c
       030a0120030c0104ff0e01022a280104ff0e010204300104ff0e01021d06
       1606192801020104ff0eff0e0202092801020104ff0eff0e020205280102
       0104ff0eff0e020205280104ff0e01020a2801020104ff0eff0e02022728
       012c01020104ff0eff0eff0e03022738132801020104ff0eff0e02020528
       0102010aff0eff0e0202163001020104ff0eff0e0202182801020104ff0e
-      ff0e02023206112801020104ff0eff0e0202052801020104ff0eff0e0202
+      ff0e02020f06112801020104ff0eff0e0202052801020104ff0eff0e0202
       052801020104ff0eff0e0202122801020104ff0eff0e0202093001020104
       ff0eff0e02
```

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/database_delete.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/database_delete.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/export.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/export.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/login_admin.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/login_admin.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/preview_questionnaire.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/preview_questionnaire.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/progress.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/progress.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/progress_ajax.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/progress_ajax.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/progress_summary_ajax.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/progress_summary_ajax.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/questionnaire_results.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/questionnaire_results.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/results.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/results.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/results_boxplot.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/results_boxplot.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/table_ajax.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/table_ajax.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/table_view.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/table_view.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/template_admin.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/template_admin.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/templates/template_admin_head.html` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/templates/template_admin_head.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/util.py` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/admin/views.py` & `bride-of-frankensystem-2.0.0.0/BOFS/admin/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -294,15 +294,15 @@
 
     unique_conditions = df['condition'].unique().tolist()
     unique_conditions.sort()
     plot_data = []
 
     for condition in unique_conditions:
         df_part = df.loc[df.condition == condition]
-        count = df_part.count()
+        #count = df_part.count()
 
         data = {
             "y": df_part[field_name].to_list(),
             #"x": [condition] * count,
             "name": str(condition),
             "type": "box",
             "boxpoints": "Outliers"
@@ -350,49 +350,14 @@
         f.close()
     except Exception as e:
         errors = list(e.args)
 
     return render_template("preview_questionnaire_simple.html", q=json_data)
 
 
-#@admin.route("/analyze_questionnaire/<questionnaireName>/<tag>")
-#@admin.route("/analyze_questionnaire/<questionnaireName>")
-#@verify_admin
-#def route_analyze_questionnaire(questionnaireName, tag=0):
-#    questionnaire = questionnaires[questionnaireName]
-#
-#    gridPlotData = {}
-#    gridPlotJSVars = []
-#
-#    numericResults = NumericResults(questionnaire.dbClass, questionnaire.fields, tag)
-#
-#    for condition, valueDict in list(numericResults.dataDescriptive.items()):
-#        gpd = {
-#            'name': condition,
-#            'type': 'bar',
-#            'x': [field for (field, descriptives) in list(valueDict.items())],
-#            'y': [descriptives.mean for (field, descriptives) in list(valueDict.items())],
-#            'error_y': {
-#                'type': 'data',
-#                'visible': True,
-#                'array': [descriptives.sem for (field, descriptives) in list(valueDict.items())]
-#            }
-#        }
-#        gridPlotData[condition] = json.dumps(gpd)
-#        gridPlotJSVars.append("gpd_{}".format(condition))
-#
-#    return render_template("questionnaire_results.html",
-#                           questionnaireName=questionnaireName,
-#                           tag=tag,
-#                           conditionCount=fetch_condition_count(),
-#                           gridPlotData=gridPlotData,
-#                           gridPlotJSVars=json.dumps(gridPlotJSVars).replace('"', ''),
-#                           numericResults=numericResults)
-
-
 def table_data(tableName):
     rows = db.session.query(db.metadata.tables[tableName]).all()
 
     columns = []
 
     for c in db.metadata.tables[tableName].columns:
         type = str(c.type)
```

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/bride_of_frankensystem.egg-info/PKG-INFO` & `bride-of-frankensystem-2.0.0.0/BOFS/bride_of_frankensystem.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/bride_of_frankensystem.egg-info/SOURCES.txt` & `bride-of-frankensystem-2.0.0.0/BOFS/bride_of_frankensystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/cli.py` & `bride-of-frankensystem-2.0.0.0/BOFS/cli.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/create_app.py` & `bride-of-frankensystem-2.0.0.0/BOFS/create_app.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/default/__pycache__/models.cpython-310.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/default/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/default/__pycache__/models.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/default/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/default/__pycache__/views.cpython-310.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/default/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/default/__pycache__/views.cpython-311.pyc` & `bride-of-frankensystem-2.0.0.0/BOFS/default/__pycache__/views.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xf8e21e66 (Tue Apr 16 20:43:36 2024 UTC)
-files sz: 18057
+moddate:  0x68792166 (Thu Apr 18 19:50:00 2024 UTC)
+files sz: 18115
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a036d045a046d055a0501
@@ -892,15 +892,15 @@
       code
          argcount  : 0
          nlocals   : 8
          stacksize : 6
          flags     : 3
          code
             0x97007400000000000000000000006a01000000000000000064016b0200
-            000000900372267404000000000000000000006a0300000000000000006a
+            000000900372457404000000000000000000006a0300000000000000006a
             040000000000000000a00500000000000000000000000000000000000000
             00740c00000000000000000000640219000000000000000000a6010000ab
             0100000000000000007d00740f0000000000000000000074000000000000
             00000000006a080000000000000000640319000000000000000000a60100
             00ab010000000000000000a0090000000000000000000000000000000000
             000000a6000000ab0000000000000000007c005f0a00000000000000007c
             006a0a0000000000000000740c0000000000000000000064033c00000074
@@ -915,58 +915,60 @@
             000000000000007c006a0a00000000000000006b0200000000a6010000ab
             010000000000000000a01200000000000000000000000000000000000000
             007405000000000000000000006a13000000000000000074040000000000
             00000000006a1000000000000000006a140000000000000000a6010000ab
             010000000000000000a6010000ab010000000000000000a0150000000000
             000000000000000000000000000000a6000000ab0000000000000000007d
             017416000000000000000000006a0c000000000000000064061900000000
-            00000000007d027c01900172a3742d000000000000000000007c01a60100
-            00ab01000000000000000064076b04000000009001728f74040000000000
+            00000000007d027c01900172c2742d000000000000000000007c01a60100
+            00ab01000000000000000064076b0400000000900172ae74040000000000
             00000000006a060000000000000000a00400000000000000000000000000
             000000000000007404000000000000000000006a030000000000000000a6
             010000ab010000000000000000a011000000000000000000000000000000
             00000000007404000000000000000000006a0300000000000000006a0a00
             000000000000007c006a0a00000000000000006b02000000007404000000
             000000000000006a0300000000000000006a1700000000000000007c0164
             07190000000000000000006a1700000000000000006b0200000000a60200
-            00ab0200000000000000007d037c0272287c03a011000000000000000000
+            00ab0200000000000000007d037c0272477c03a011000000000000000000
             00000000000000000000007404000000000000000000006a030000000000
-            0000006a18000000000000000064086b0300000000a6010000ab01000000
-            00000000007d037c03a01500000000000000000000000000000000000000
-            00a6000000ab0000000000000000007d037c0372dc742d00000000000000
-            0000007c03a6010000ab01000000000000000064076b040000000072c974
-            32000000000000000000006a1a0000000000000000a01b00000000000000
-            000000000000000000000000007c016407190000000000000000006a1c00
-            00000000000000a6010000ab0100000000000000007d047c04a01d000000
-            0000000000000000000000000000000000a6000000ab0000000000000000
-            0044005d127d057c047c0519000000000000000000740c00000000000000
-            0000007c053c0000008c1364097c005f1e00000000000000007404000000
-            000000000000006a060000000000000000a01f0000000000000000000000
-            000000000000000000a6000000ab00000000000000000001007c0344005d
-            237d067c066a1e000000000000000064076b030000000072167c066a1e00
-            00000000000000810f7c066a1e0000000000000000740c00000000000000
-            000000640a3c0000008c24640b7c0476007229740c000000000000000000
-            00640b19000000000000000000640c7601721a741b000000000000000000
-            00740c00000000000000000000640b19000000000000000000a6010000ab
-            0100000000000000005300741b00000000000000000000741d0000000000
-            000000000064057400000000000000000000006a0f0000000000000000a6
-            020000ab020000000000000000a6010000ab010000000000000000530064
-            097d076403740c000000000000000000007600722b742d00000000000000
-            000000740c00000000000000000000640319000000000000000000a60100
-            00ab01000000000000000064076b0400000000720d740c00000000000000
-            0000006403190000000000000000007d0774410000000000000000000064
-            0d7c07ac0ea6020000ab0200000000000000005300
+            0000006a18000000000000000064086b0300000000740400000000000000
+            0000006a0300000000000000006a170000000000000000740c0000000000
+            00000000006402190000000000000000006b0300000000a6020000ab0200
+            000000000000007d037c03a0150000000000000000000000000000000000
+            000000a6000000ab0000000000000000007d037c0372dc742d0000000000
+            00000000007c03a6010000ab01000000000000000064076b040000000072
+            c97432000000000000000000006a1a0000000000000000a01b0000000000
+            0000000000000000000000000000007c016407190000000000000000006a
+            1c0000000000000000a6010000ab0100000000000000007d047c04a01d00
+            00000000000000000000000000000000000000a6000000ab000000000000
+            00000044005d127d057c047c0519000000000000000000740c0000000000
+            00000000007c053c0000008c1364097c005f1e0000000000000000740400
+            0000000000000000006a060000000000000000a01f000000000000000000
+            0000000000000000000000a6000000ab00000000000000000001007c0344
+            005d237d067c066a1e000000000000000064076b030000000072167c066a
+            1e0000000000000000810f7c066a1e0000000000000000740c0000000000
+            0000000000640a3c0000008c24640b7c0476007229740c00000000000000
+            000000640b19000000000000000000640c7601721a741b00000000000000
+            000000740c00000000000000000000640b19000000000000000000a60100
+            00ab0100000000000000005300741b00000000000000000000741d000000
+            0000000000000064057400000000000000000000006a0f00000000000000
+            00a6020000ab020000000000000000a6010000ab01000000000000000053
+            0064097d076403740c000000000000000000007600722b742d0000000000
+            0000000000740c00000000000000000000640319000000000000000000a6
+            010000ab01000000000000000064076b0400000000720d740c0000000000
+            00000000006403190000000000000000007d077441000000000000000000
+            00640d7c07ac0ea6020000ab0200000000000000005300
          111           0 RESUME                   0
          
          124           2 LOAD_GLOBAL              0 (request)
                       14 LOAD_ATTR                1 (method)
                       24 LOAD_CONST               1 ('POST')
                       26 COMPARE_OP               2 (==)
                       32 EXTENDED_ARG             3
-                      34 POP_JUMP_FORWARD_IF_FALSE   806 (to 1648)
+                      34 POP_JUMP_FORWARD_IF_FALSE   837 (to 1710)
          
          125          36 LOAD_GLOBAL              4 (db)
                       48 LOAD_ATTR                3 (Participant)
                       58 LOAD_ATTR                4 (query)
                       68 LOAD_METHOD              5 (get)
                       90 LOAD_GLOBAL             12 (session)
                      102 LOAD_CONST               2 ('participantID')
@@ -1049,23 +1051,23 @@
                      702 LOAD_ATTR               12 (config)
                      712 LOAD_CONST               6 ('ALLOW_RETAKES')
                      714 BINARY_SUBSCR
                      724 STORE_FAST               2 (allowRetakes)
          
          143         726 LOAD_FAST                1 (sessionFromMTurkID)
                      728 EXTENDED_ARG             1
-                     730 POP_JUMP_FORWARD_IF_FALSE   419 (to 1570)
+                     730 POP_JUMP_FORWARD_IF_FALSE   450 (to 1632)
                      732 LOAD_GLOBAL             45 (NULL + len)
                      744 LOAD_FAST                1 (sessionFromMTurkID)
                      746 PRECALL                  1
                      750 CALL                     1
                      760 LOAD_CONST               7 (0)
                      762 COMPARE_OP               4 (>)
                      768 EXTENDED_ARG             1
-                     770 POP_JUMP_FORWARD_IF_FALSE   399 (to 1570)
+                     770 POP_JUMP_FORWARD_IF_FALSE   430 (to 1632)
          
          144         772 LOAD_GLOBAL              4 (db)
                      784 LOAD_ATTR                6 (session)
                      794 LOAD_METHOD              4 (query)
                      816 LOAD_GLOBAL              4 (db)
                      828 LOAD_ATTR                3 (Participant)
                      838 PRECALL                  1
@@ -1091,161 +1093,168 @@
          
          145         986 PRECALL                  2
                      990 CALL                     2
          
          144        1000 STORE_FAST               3 (pFromMTurkID)
          
          150        1002 LOAD_FAST                2 (allowRetakes)
-                    1004 POP_JUMP_FORWARD_IF_FALSE    40 (to 1086)
+                    1004 POP_JUMP_FORWARD_IF_FALSE    71 (to 1148)
          
          152        1006 LOAD_FAST                3 (pFromMTurkID)
                     1008 LOAD_METHOD             17 (filter)
                     1030 LOAD_GLOBAL              4 (db)
                     1042 LOAD_ATTR                3 (Participant)
                     1052 LOAD_ATTR               24 (finished)
                     1062 LOAD_CONST               8 (True)
                     1064 COMPARE_OP               3 (!=)
-                    1070 PRECALL                  1
-                    1074 CALL                     1
-                    1084 STORE_FAST               3 (pFromMTurkID)
-         
-         154     >> 1086 LOAD_FAST                3 (pFromMTurkID)
-                    1088 LOAD_METHOD             21 (all)
-                    1110 PRECALL                  0
-                    1114 CALL                     0
-                    1124 STORE_FAST               3 (pFromMTurkID)
-         
-         157        1126 LOAD_FAST                3 (pFromMTurkID)
-                    1128 POP_JUMP_FORWARD_IF_FALSE   220 (to 1570)
-                    1130 LOAD_GLOBAL             45 (NULL + len)
-                    1142 LOAD_FAST                3 (pFromMTurkID)
-                    1144 PRECALL                  1
-                    1148 CALL                     1
-                    1158 LOAD_CONST               7 (0)
-                    1160 COMPARE_OP               4 (>)
-                    1166 POP_JUMP_FORWARD_IF_FALSE   201 (to 1570)
-         
-         158        1168 LOAD_GLOBAL             50 (BOFSSessionInterface)
-                    1180 LOAD_ATTR               26 (serializer)
-                    1190 LOAD_METHOD             27 (loads)
-                    1212 LOAD_FAST                1 (sessionFromMTurkID)
-                    1214 LOAD_CONST               7 (0)
-                    1216 BINARY_SUBSCR
-                    1226 LOAD_ATTR               28 (data)
-                    1236 PRECALL                  1
-                    1240 CALL                     1
-                    1250 STORE_FAST               4 (dictData)
-         
-         159        1252 LOAD_FAST                4 (dictData)
-                    1254 LOAD_METHOD             29 (keys)
-                    1276 PRECALL                  0
-                    1280 CALL                     0
-                    1290 GET_ITER
-                 >> 1292 FOR_ITER                18 (to 1330)
-                    1294 STORE_FAST               5 (key)
-         
-         160        1296 LOAD_FAST                4 (dictData)
-                    1298 LOAD_FAST                5 (key)
-                    1300 BINARY_SUBSCR
-                    1310 LOAD_GLOBAL             12 (session)
-                    1322 LOAD_FAST                5 (key)
-                    1324 STORE_SUBSCR
-                    1328 JUMP_BACKWARD           19 (to 1292)
-         
-         163     >> 1330 LOAD_CONST               9 (None)
-                    1332 LOAD_FAST                0 (p)
-                    1334 STORE_ATTR              30 (condition)
-         
-         164        1344 LOAD_GLOBAL              4 (db)
-                    1356 LOAD_ATTR                6 (session)
-                    1366 LOAD_METHOD             31 (commit)
-                    1388 PRECALL                  0
-                    1392 CALL                     0
-                    1402 POP_TOP
-         
-         167        1404 LOAD_FAST                3 (pFromMTurkID)
-                    1406 GET_ITER
-                 >> 1408 FOR_ITER                35 (to 1480)
-                    1410 STORE_FAST               6 (pPastAttempt)
-         
-         169        1412 LOAD_FAST                6 (pPastAttempt)
-                    1414 LOAD_ATTR               30 (condition)
-                    1424 LOAD_CONST               7 (0)
-                    1426 COMPARE_OP               3 (!=)
-                    1432 POP_JUMP_FORWARD_IF_FALSE    22 (to 1478)
-                    1434 LOAD_FAST                6 (pPastAttempt)
-                    1436 LOAD_ATTR               30 (condition)
-                    1446 POP_JUMP_FORWARD_IF_NONE    15 (to 1478)
-         
-         170        1448 LOAD_FAST                6 (pPastAttempt)
-                    1450 LOAD_ATTR               30 (condition)
-                    1460 LOAD_GLOBAL             12 (session)
-                    1472 LOAD_CONST              10 ('condition')
-                    1474 STORE_SUBSCR
-                 >> 1478 JUMP_BACKWARD           36 (to 1408)
-         
-         174     >> 1480 LOAD_CONST              11 ('currentUrl')
-                    1482 LOAD_FAST                4 (dictData)
-                    1484 CONTAINS_OP              0
-                    1486 POP_JUMP_FORWARD_IF_FALSE    41 (to 1570)
-                    1488 LOAD_GLOBAL             12 (session)
-                    1500 LOAD_CONST              11 ('currentUrl')
-                    1502 BINARY_SUBSCR
-                    1512 LOAD_CONST              12 (('startMTurk', 'start_mturk', 'external_id', 'consent'))
-                    1514 CONTAINS_OP              1
-                    1516 POP_JUMP_FORWARD_IF_FALSE    26 (to 1570)
-         
-         175        1518 LOAD_GLOBAL             27 (NULL + redirect)
-                    1530 LOAD_GLOBAL             12 (session)
-                    1542 LOAD_CONST              11 ('currentUrl')
-                    1544 BINARY_SUBSCR
-                    1554 PRECALL                  1
-                    1558 CALL                     1
-                    1568 RETURN_VALUE
-         
-         177     >> 1570 LOAD_GLOBAL             27 (NULL + redirect)
-                    1582 LOAD_GLOBAL             29 (NULL + join_urls)
-                    1594 LOAD_CONST               5 ('/redirect_from_page')
-                    1596 LOAD_GLOBAL              0 (request)
-                    1608 LOAD_ATTR               15 (path)
-                    1618 PRECALL                  2
-                    1622 CALL                     2
-                    1632 PRECALL                  1
-                    1636 CALL                     1
-                    1646 RETURN_VALUE
-         
-         179     >> 1648 LOAD_CONST               9 (None)
-                    1650 STORE_FAST               7 (mTurkID)
-         
-         180        1652 LOAD_CONST               3 ('mTurkID')
-                    1654 LOAD_GLOBAL             12 (session)
-                    1666 CONTAINS_OP              0
-                    1668 POP_JUMP_FORWARD_IF_FALSE    43 (to 1756)
-                    1670 LOAD_GLOBAL             45 (NULL + len)
-                    1682 LOAD_GLOBAL             12 (session)
-                    1694 LOAD_CONST               3 ('mTurkID')
-                    1696 BINARY_SUBSCR
-                    1706 PRECALL                  1
-                    1710 CALL                     1
-                    1720 LOAD_CONST               7 (0)
-                    1722 COMPARE_OP               4 (>)
-                    1728 POP_JUMP_FORWARD_IF_FALSE    13 (to 1756)
-         
-         181        1730 LOAD_GLOBAL             12 (session)
-                    1742 LOAD_CONST               3 ('mTurkID')
-                    1744 BINARY_SUBSCR
-                    1754 STORE_FAST               7 (mTurkID)
-         
-         183     >> 1756 LOAD_GLOBAL             65 (NULL + render_template)
-                    1768 LOAD_CONST              13 ('external_id.html')
-                    1770 LOAD_FAST                7 (mTurkID)
-                    1772 KW_NAMES                14
-                    1774 PRECALL                  2
-                    1778 CALL                     2
-                    1788 RETURN_VALUE
+                    1070 LOAD_GLOBAL              4 (db)
+                    1082 LOAD_ATTR                3 (Participant)
+                    1092 LOAD_ATTR               23 (participantID)
+                    1102 LOAD_GLOBAL             12 (session)
+                    1114 LOAD_CONST               2 ('participantID')
+                    1116 BINARY_SUBSCR
+                    1126 COMPARE_OP               3 (!=)
+                    1132 PRECALL                  2
+                    1136 CALL                     2
+                    1146 STORE_FAST               3 (pFromMTurkID)
+         
+         154     >> 1148 LOAD_FAST                3 (pFromMTurkID)
+                    1150 LOAD_METHOD             21 (all)
+                    1172 PRECALL                  0
+                    1176 CALL                     0
+                    1186 STORE_FAST               3 (pFromMTurkID)
+         
+         157        1188 LOAD_FAST                3 (pFromMTurkID)
+                    1190 POP_JUMP_FORWARD_IF_FALSE   220 (to 1632)
+                    1192 LOAD_GLOBAL             45 (NULL + len)
+                    1204 LOAD_FAST                3 (pFromMTurkID)
+                    1206 PRECALL                  1
+                    1210 CALL                     1
+                    1220 LOAD_CONST               7 (0)
+                    1222 COMPARE_OP               4 (>)
+                    1228 POP_JUMP_FORWARD_IF_FALSE   201 (to 1632)
+         
+         158        1230 LOAD_GLOBAL             50 (BOFSSessionInterface)
+                    1242 LOAD_ATTR               26 (serializer)
+                    1252 LOAD_METHOD             27 (loads)
+                    1274 LOAD_FAST                1 (sessionFromMTurkID)
+                    1276 LOAD_CONST               7 (0)
+                    1278 BINARY_SUBSCR
+                    1288 LOAD_ATTR               28 (data)
+                    1298 PRECALL                  1
+                    1302 CALL                     1
+                    1312 STORE_FAST               4 (dictData)
+         
+         159        1314 LOAD_FAST                4 (dictData)
+                    1316 LOAD_METHOD             29 (keys)
+                    1338 PRECALL                  0
+                    1342 CALL                     0
+                    1352 GET_ITER
+                 >> 1354 FOR_ITER                18 (to 1392)
+                    1356 STORE_FAST               5 (key)
+         
+         160        1358 LOAD_FAST                4 (dictData)
+                    1360 LOAD_FAST                5 (key)
+                    1362 BINARY_SUBSCR
+                    1372 LOAD_GLOBAL             12 (session)
+                    1384 LOAD_FAST                5 (key)
+                    1386 STORE_SUBSCR
+                    1390 JUMP_BACKWARD           19 (to 1354)
+         
+         163     >> 1392 LOAD_CONST               9 (None)
+                    1394 LOAD_FAST                0 (p)
+                    1396 STORE_ATTR              30 (condition)
+         
+         164        1406 LOAD_GLOBAL              4 (db)
+                    1418 LOAD_ATTR                6 (session)
+                    1428 LOAD_METHOD             31 (commit)
+                    1450 PRECALL                  0
+                    1454 CALL                     0
+                    1464 POP_TOP
+         
+         167        1466 LOAD_FAST                3 (pFromMTurkID)
+                    1468 GET_ITER
+                 >> 1470 FOR_ITER                35 (to 1542)
+                    1472 STORE_FAST               6 (pPastAttempt)
+         
+         169        1474 LOAD_FAST                6 (pPastAttempt)
+                    1476 LOAD_ATTR               30 (condition)
+                    1486 LOAD_CONST               7 (0)
+                    1488 COMPARE_OP               3 (!=)
+                    1494 POP_JUMP_FORWARD_IF_FALSE    22 (to 1540)
+                    1496 LOAD_FAST                6 (pPastAttempt)
+                    1498 LOAD_ATTR               30 (condition)
+                    1508 POP_JUMP_FORWARD_IF_NONE    15 (to 1540)
+         
+         170        1510 LOAD_FAST                6 (pPastAttempt)
+                    1512 LOAD_ATTR               30 (condition)
+                    1522 LOAD_GLOBAL             12 (session)
+                    1534 LOAD_CONST              10 ('condition')
+                    1536 STORE_SUBSCR
+                 >> 1540 JUMP_BACKWARD           36 (to 1470)
+         
+         174     >> 1542 LOAD_CONST              11 ('currentUrl')
+                    1544 LOAD_FAST                4 (dictData)
+                    1546 CONTAINS_OP              0
+                    1548 POP_JUMP_FORWARD_IF_FALSE    41 (to 1632)
+                    1550 LOAD_GLOBAL             12 (session)
+                    1562 LOAD_CONST              11 ('currentUrl')
+                    1564 BINARY_SUBSCR
+                    1574 LOAD_CONST              12 (('startMTurk', 'start_mturk', 'external_id', 'consent'))
+                    1576 CONTAINS_OP              1
+                    1578 POP_JUMP_FORWARD_IF_FALSE    26 (to 1632)
+         
+         175        1580 LOAD_GLOBAL             27 (NULL + redirect)
+                    1592 LOAD_GLOBAL             12 (session)
+                    1604 LOAD_CONST              11 ('currentUrl')
+                    1606 BINARY_SUBSCR
+                    1616 PRECALL                  1
+                    1620 CALL                     1
+                    1630 RETURN_VALUE
+         
+         177     >> 1632 LOAD_GLOBAL             27 (NULL + redirect)
+                    1644 LOAD_GLOBAL             29 (NULL + join_urls)
+                    1656 LOAD_CONST               5 ('/redirect_from_page')
+                    1658 LOAD_GLOBAL              0 (request)
+                    1670 LOAD_ATTR               15 (path)
+                    1680 PRECALL                  2
+                    1684 CALL                     2
+                    1694 PRECALL                  1
+                    1698 CALL                     1
+                    1708 RETURN_VALUE
+         
+         179     >> 1710 LOAD_CONST               9 (None)
+                    1712 STORE_FAST               7 (mTurkID)
+         
+         180        1714 LOAD_CONST               3 ('mTurkID')
+                    1716 LOAD_GLOBAL             12 (session)
+                    1728 CONTAINS_OP              0
+                    1730 POP_JUMP_FORWARD_IF_FALSE    43 (to 1818)
+                    1732 LOAD_GLOBAL             45 (NULL + len)
+                    1744 LOAD_GLOBAL             12 (session)
+                    1756 LOAD_CONST               3 ('mTurkID')
+                    1758 BINARY_SUBSCR
+                    1768 PRECALL                  1
+                    1772 CALL                     1
+                    1782 LOAD_CONST               7 (0)
+                    1784 COMPARE_OP               4 (>)
+                    1790 POP_JUMP_FORWARD_IF_FALSE    13 (to 1818)
+         
+         181        1792 LOAD_GLOBAL             12 (session)
+                    1804 LOAD_CONST               3 ('mTurkID')
+                    1806 BINARY_SUBSCR
+                    1816 STORE_FAST               7 (mTurkID)
+         
+         183     >> 1818 LOAD_GLOBAL             65 (NULL + render_template)
+                    1830 LOAD_CONST              13 ('external_id.html')
+                    1832 LOAD_FAST                7 (mTurkID)
+                    1834 KW_NAMES                14
+                    1836 PRECALL                  2
+                    1840 CALL                     2
+                    1850 RETURN_VALUE
          consts
             '\n    ``/external_id`` or (for backwards compatibility) ``/startMTurk`` or ``/start_mturk``\n\n    If we are using a platform where the user has a unique (and anonymous) ID associated with their account,\n    then you can use this page to request that ID. This is set up to work with Mechanical Turk, but the\n    template can be overwritten to request different types of ID.\n    :return:\n    '
             'POST'
             'participantID'
             'mTurkID'
             'RETRIEVE_SESSIONS'
             '/redirect_from_page'
@@ -1263,15 +1272,15 @@
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\colby\\Desktop\\git\\bride-of-frankensystem-examples\\venv\\Lib\\site-packages\\BOFS\\default\\views.py'
          name       'route_external_id'
          firstlineno 111
          lnotab
             0x020d22015e016c021e0324014e02500156018cfe020424052e01500116
-            0132013efe0eff02060402500228032a0154012c0122030e013c03080224
+            0132013efe0eff020604028e0228032a0154012c0122030e013c03080224
             012004260134024e0204014e011a02
       '/table/<tableName>'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 2
          flags     : 3
```

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/default/models.py` & `bride-of-frankensystem-2.0.0.0/BOFS/default/models.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/default/views.py` & `bride-of-frankensystem-2.0.0.0/BOFS/default/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
                 filter(
                     db.Participant.mTurkID == p.mTurkID,
                     db.Participant.participantID == sessionFromMTurkID[0].participantID
                 )
 
             if allowRetakes:
                 # If allow retakes is True, then don't try to re-load data from past attempts that were completed.
-                pFromMTurkID = pFromMTurkID.filter(db.Participant.finished != True)
+                pFromMTurkID = pFromMTurkID.filter(db.Participant.finished != True, db.Participant.participantID != session['participantID'])
 
             pFromMTurkID = pFromMTurkID.all()
 
             # Load their old session
             if pFromMTurkID and len(pFromMTurkID) > 0:
                 dictData = BOFSSessionInterface.serializer.loads(sessionFromMTurkID[0].data)
                 for key in dictData.keys():
```

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/globals.py` & `bride-of-frankensystem-2.0.0.0/BOFS/globals.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/static/all.min.css` & `bride-of-frankensystem-2.0.0.0/BOFS/static/all.min.css`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/static/bootstrap.min.css` & `bride-of-frankensystem-2.0.0.0/BOFS/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/static/img/check.png` & `bride-of-frankensystem-2.0.0.0/BOFS/static/img/check.png`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/static/img/spinner32.gif` & `bride-of-frankensystem-2.0.0.0/BOFS/static/img/spinner32.gif`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/static/js/bootstrap.bundle.min.js` & `bride-of-frankensystem-2.0.0.0/BOFS/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/static/js/htmx.min.js` & `bride-of-frankensystem-2.0.0.0/BOFS/static/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/static/js/jquery-3.7.1.min.js` & `bride-of-frankensystem-2.0.0.0/BOFS/static/js/jquery-3.7.1.min.js`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/static/loading.gif` & `bride-of-frankensystem-2.0.0.0/BOFS/static/loading.gif`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/static/style.css` & `bride-of-frankensystem-2.0.0.0/BOFS/static/style.css`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/static/style_admin.css` & `bride-of-frankensystem-2.0.0.0/BOFS/static/style_admin.css`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/templates/consent.html` & `bride-of-frankensystem-2.0.0.0/BOFS/templates/consent.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/templates/end.html` & `bride-of-frankensystem-2.0.0.0/BOFS/templates/end.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/templates/external_id.html` & `bride-of-frankensystem-2.0.0.0/BOFS/templates/external_id.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/templates/questionnaire_macro.html` & `bride-of-frankensystem-2.0.0.0/BOFS/templates/questionnaire_macro.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/templates/questions/radiogrid.html` & `bride-of-frankensystem-2.0.0.0/BOFS/templates/questions/radiogrid.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/templates/questions/radiolist.html` & `bride-of-frankensystem-2.0.0.0/BOFS/templates/questions/radiolist.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/templates/questions/slider.html` & `bride-of-frankensystem-2.0.0.0/BOFS/templates/questions/slider.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/templates/template.html` & `bride-of-frankensystem-2.0.0.0/BOFS/templates/template.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/templates/unity_webgl.html` & `bride-of-frankensystem-2.0.0.0/BOFS/templates/unity_webgl.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/templates/unity_webgl_fullscreen.html` & `bride-of-frankensystem-2.0.0.0/BOFS/templates/unity_webgl_fullscreen.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/BOFS/util.py` & `bride-of-frankensystem-2.0.0.0/BOFS/util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/LICENSE` & `bride-of-frankensystem-2.0.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/PKG-INFO` & `bride-of-frankensystem-2.0.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bride-of-frankensystem
-Version: 1.9.3.7
+Version: 2.0.0.0
 Summary: A framework that allows for the development of custom online experiments and surveys.
 Author-email: Colby Johanson <colby.johanson@usask.ca>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -209,17 +209,20 @@
 
 Dependencies
 ============
 BOF requires Python 3.9+, along with the following Python packages.
 
 * `flask` - The web framework that BOF is based off of.
 * `sqlalchemy` - An object-relational manager that is used for database table definitions and query access.
-* `flask-sqlalchemy` - A bridge between Flask and SQLAlchemy
+* `flask-sqlalchemy` - A bridge between Flask and SQLAlchemy.
+* `flask-compressed` - To support the compressed files that Unity WebGL builds use.
 * `eventlet` - This is used as the production (live) web server, as an alternative to Flask's built in web server or the Apache web server.
 * `toml` - The configuration files use the toml format.
+* `crawlerdetect` - To detect web crawlers so that they don't get counted as actual participants.
+* `pandas` - Used to process data for the export and for the results preview.
 
 
 Installing and Running BOFS
 ===========================
 Please refer to the [installation instructions](https://bride-of-frankensystem.readthedocs.io/en/latest/installation.html) in the documentation.
```

### Comparing `bride-of-frankensystem-1.9.3.7/README.md` & `bride-of-frankensystem-2.0.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,20 @@
 
 Dependencies
 ============
 BOF requires Python 3.9+, along with the following Python packages.
 
 * `flask` - The web framework that BOF is based off of.
 * `sqlalchemy` - An object-relational manager that is used for database table definitions and query access.
-* `flask-sqlalchemy` - A bridge between Flask and SQLAlchemy
+* `flask-sqlalchemy` - A bridge between Flask and SQLAlchemy.
+* `flask-compressed` - To support the compressed files that Unity WebGL builds use.
 * `eventlet` - This is used as the production (live) web server, as an alternative to Flask's built in web server or the Apache web server.
 * `toml` - The configuration files use the toml format.
+* `crawlerdetect` - To detect web crawlers so that they don't get counted as actual participants.
+* `pandas` - Used to process data for the export and for the results preview.
 
 
 Installing and Running BOFS
 ===========================
 Please refer to the [installation instructions](https://bride-of-frankensystem.readthedocs.io/en/latest/installation.html) in the documentation.
```

### Comparing `bride-of-frankensystem-1.9.3.7/bride_of_frankensystem.egg-info/PKG-INFO` & `bride-of-frankensystem-2.0.0.0/bride_of_frankensystem.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bride-of-frankensystem
-Version: 1.9.3.7
+Version: 2.0.0.0
 Summary: A framework that allows for the development of custom online experiments and surveys.
 Author-email: Colby Johanson <colby.johanson@usask.ca>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -209,17 +209,20 @@
 
 Dependencies
 ============
 BOF requires Python 3.9+, along with the following Python packages.
 
 * `flask` - The web framework that BOF is based off of.
 * `sqlalchemy` - An object-relational manager that is used for database table definitions and query access.
-* `flask-sqlalchemy` - A bridge between Flask and SQLAlchemy
+* `flask-sqlalchemy` - A bridge between Flask and SQLAlchemy.
+* `flask-compressed` - To support the compressed files that Unity WebGL builds use.
 * `eventlet` - This is used as the production (live) web server, as an alternative to Flask's built in web server or the Apache web server.
 * `toml` - The configuration files use the toml format.
+* `crawlerdetect` - To detect web crawlers so that they don't get counted as actual participants.
+* `pandas` - Used to process data for the export and for the results preview.
 
 
 Installing and Running BOFS
 ===========================
 Please refer to the [installation instructions](https://bride-of-frankensystem.readthedocs.io/en/latest/installation.html) in the documentation.
```

### Comparing `bride-of-frankensystem-1.9.3.7/bride_of_frankensystem.egg-info/SOURCES.txt` & `bride-of-frankensystem-2.0.0.0/bride_of_frankensystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.7/pyproject.toml` & `bride-of-frankensystem-2.0.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bride-of-frankensystem"
-version = "1.9.3.7"
+version = "2.0.0.0"
 description = "A framework that allows for the development of custom online experiments and surveys."
 readme = "README.md"
 authors = [{ name = "Colby Johanson", email = "colby.johanson@usask.ca" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Programming Language :: Python",
```

