# Comparing `tmp/FlowTutor-0.10.9.tar.gz` & `tmp/FlowTutor-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowTutor-0.10.9.tar", last modified: Tue Dec 12 15:24:01 2023, max compression
+gzip compressed data, was "FlowTutor-0.9.0.tar", last modified: Sat Jul 29 13:34:15 2023, max compression
```

## Comparing `FlowTutor-0.10.9.tar` & `FlowTutor-0.9.0.tar`

### file list

```diff
@@ -1,103 +1,94 @@
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-12-12 15:24:01.588647 FlowTutor-0.10.9/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7651 2023-07-29 13:30:08.000000 FlowTutor-0.10.9/LICENSE
--rw-r--r--   0 thomas    (1000) thomas    (1000)       90 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/MANIFEST.in
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4027 2023-12-12 15:24:01.588647 FlowTutor-0.10.9/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2325 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/README.md
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2146 2023-12-12 15:23:55.000000 FlowTutor-0.10.9/pyproject.toml
--rw-r--r--   0 thomas    (1000) thomas    (1000)       70 2023-12-12 15:24:01.588647 FlowTutor-0.10.9/setup.cfg
--rw-r--r--   0 thomas    (1000) thomas    (1000)       69 2023-10-16 18:05:08.000000 FlowTutor-0.10.9/setup.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-12-12 15:24:01.572647 FlowTutor-0.10.9/src/
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-12-12 15:24:01.588647 FlowTutor-0.10.9/src/FlowTutor.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4027 2023-12-12 15:24:01.000000 FlowTutor-0.10.9/src/FlowTutor.egg-info/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3374 2023-12-12 15:24:01.000000 FlowTutor-0.10.9/src/FlowTutor.egg-info/SOURCES.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-12-12 15:24:01.000000 FlowTutor-0.10.9/src/FlowTutor.egg-info/dependency_links.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       97 2023-12-12 15:24:01.000000 FlowTutor-0.10.9/src/FlowTutor.egg-info/entry_points.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)      241 2023-12-12 15:24:01.000000 FlowTutor-0.10.9/src/FlowTutor.egg-info/requires.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       10 2023-12-12 15:24:01.000000 FlowTutor-0.10.9/src/FlowTutor.egg-info/top_level.txt
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-12-12 15:24:01.576647 FlowTutor-0.10.9/src/flowtutor/
--rw-r--r--   0 thomas    (1000) thomas    (1000)       37 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     9300 2023-10-16 08:42:21.000000 FlowTutor-0.10.9/src/flowtutor/codegenerator.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      806 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/containers.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-12-12 15:24:01.576647 FlowTutor-0.10.9/src/flowtutor/debugger/
--rw-r--r--   0 thomas    (1000) thomas    (1000)       71 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/debugger/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2474 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/debugger/debugsession.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4327 2023-10-15 19:27:35.000000 FlowTutor-0.10.9/src/flowtutor/debugger/ftdb.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2853 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/debugger/ftdbsession.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    10659 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/debugger/gdbsession.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      556 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/debugger/stdinqueue.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-12-12 15:24:01.580647 FlowTutor-0.10.9/src/flowtutor/flowchart/
--rw-r--r--   0 thomas    (1000) thomas    (1000)       81 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/flowchart/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     6933 2023-10-16 11:47:23.000000 FlowTutor-0.10.9/src/flowtutor/flowchart/connection.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      906 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/flowchart/connector.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    16231 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/flowchart/flowchart.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1421 2023-10-16 18:15:41.000000 FlowTutor-0.10.9/src/flowtutor/flowchart/functionend.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1917 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/flowchart/functionstart.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    13522 2023-10-16 11:56:30.000000 FlowTutor-0.10.9/src/flowtutor/flowchart/node.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      607 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/flowchart/parameter.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      769 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/flowchart/struct_definition.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1791 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/flowchart/struct_member.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7224 2023-10-16 11:47:23.000000 FlowTutor-0.10.9/src/flowtutor/flowchart/template.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      738 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/flowchart/type_definition.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-12-12 15:24:01.580647 FlowTutor-0.10.9/src/flowtutor/gui/
--rw-r--r--   0 thomas    (1000) thomas    (1000)       71 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/gui/__init__.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-12-12 15:24:01.584647 FlowTutor-0.10.9/src/flowtutor/gui/assets/
--rw-r--r--   0 thomas    (1000) thomas    (1000)       72 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/gui/assets/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3538 2023-10-08 16:04:36.000000 FlowTutor-0.10.9/src/flowtutor/gui/assets/c.png
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1852 2023-07-29 13:30:08.000000 FlowTutor-0.10.9/src/flowtutor/gui/assets/hammer.png
--rw-r--r--   0 thomas    (1000) thomas    (1000)    98400 2023-07-29 13:30:08.000000 FlowTutor-0.10.9/src/flowtutor/gui/assets/inconsolata.ttf
--rw-r--r--   0 thomas    (1000) thomas    (1000)      428 2023-07-29 13:30:08.000000 FlowTutor-0.10.9/src/flowtutor/gui/assets/pencil.png
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7460 2023-10-08 16:04:36.000000 FlowTutor-0.10.9/src/flowtutor/gui/assets/python.png
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1829 2023-07-29 13:30:08.000000 FlowTutor-0.10.9/src/flowtutor/gui/assets/run.png
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1728 2023-07-29 13:30:08.000000 FlowTutor-0.10.9/src/flowtutor/gui/assets/step_into.png
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1737 2023-07-29 13:30:08.000000 FlowTutor-0.10.9/src/flowtutor/gui/assets/step_over.png
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1595 2023-07-29 13:30:08.000000 FlowTutor-0.10.9/src/flowtutor/gui/assets/stop.png
--rw-r--r--   0 thomas    (1000) thomas    (1000)      332 2023-07-29 13:30:08.000000 FlowTutor-0.10.9/src/flowtutor/gui/assets/trash.png
--rw-r--r--   0 thomas    (1000) thomas    (1000)    17240 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/gui/debugger.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    29988 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/gui/gui.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4839 2023-10-16 11:47:23.000000 FlowTutor-0.10.9/src/flowtutor/gui/menubar_main.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2544 2023-10-16 18:15:41.000000 FlowTutor-0.10.9/src/flowtutor/gui/section_node_extras.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     9579 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/gui/section_structs.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3344 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/gui/section_typedefs.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      368 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/gui/sidebar.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1485 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/gui/sidebar_functionend.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     8091 2023-10-16 18:15:41.000000 FlowTutor-0.10.9/src/flowtutor/gui/sidebar_functionstart.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      717 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/gui/sidebar_multi.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     6575 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/gui/sidebar_none.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4323 2023-10-16 18:15:41.000000 FlowTutor-0.10.9/src/flowtutor/gui/sidebar_template.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      889 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/gui/window_types.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    18337 2023-10-16 11:47:23.000000 FlowTutor-0.10.9/src/flowtutor/language_service.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1999 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/main.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    14056 2023-10-16 11:47:23.000000 FlowTutor-0.10.9/src/flowtutor/modal_service.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:30:08.000000 FlowTutor-0.10.9/src/flowtutor/py.typed
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1199 2023-10-15 18:19:40.000000 FlowTutor-0.10.9/src/flowtutor/settings_service.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-12-12 15:24:01.584647 FlowTutor-0.10.9/src/flowtutor/templates/
--rw-r--r--   0 thomas    (1000) thomas    (1000)       67 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/__init__.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-12-12 15:24:01.584647 FlowTutor-0.10.9/src/flowtutor/templates/c/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      341 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/assignment.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      243 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/call.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      275 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/close_file.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      238 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/conditional.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1268 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/declaration.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      244 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/dowhileloop.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      638 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/forloop.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      884 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/input.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      807 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/language.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      603 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/open_file.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      414 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/output.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      242 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/snippet.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      236 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/whileloop.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      386 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/c/write_file.template.json
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-12-12 15:24:01.584647 FlowTutor-0.10.9/src/flowtutor/templates/python/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      340 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/python/assignment.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      242 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/python/call.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      238 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/python/conditional.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      398 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/python/forloop.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      281 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/python/input.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      218 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/python/language.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      240 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/python/output.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      242 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/python/snippet.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)      236 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/templates/python/whileloop.template.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)    18708 2023-12-12 15:22:49.000000 FlowTutor-0.10.9/src/flowtutor/util_service.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-12-12 15:24:01.584647 FlowTutor-0.10.9/tests/
--rw-r--r--   0 thomas    (1000) thomas    (1000)    23115 2023-10-08 16:04:36.000000 FlowTutor-0.10.9/tests/test_flowtutor_codegenerator.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    10661 2023-10-08 16:04:36.000000 FlowTutor-0.10.9/tests/test_flowtutor_flowchart.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:34:15.558286 FlowTutor-0.9.0/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7651 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/LICENSE
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       34 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/MANIFEST.in
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3890 2023-07-29 13:34:15.558286 FlowTutor-0.9.0/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2814 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/README.md
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1475 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/pyproject.toml
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      626 2023-07-29 13:34:15.562286 FlowTutor-0.9.0/setup.cfg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       69 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/setup.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:34:15.542286 FlowTutor-0.9.0/src/
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:34:15.546285 FlowTutor-0.9.0/src/FlowTutor.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3890 2023-07-29 13:34:15.000000 FlowTutor-0.9.0/src/FlowTutor.egg-info/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2871 2023-07-29 13:34:15.000000 FlowTutor-0.9.0/src/FlowTutor.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2023-07-29 13:34:15.000000 FlowTutor-0.9.0/src/FlowTutor.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       97 2023-07-29 13:34:15.000000 FlowTutor-0.9.0/src/FlowTutor.egg-info/entry_points.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      191 2023-07-29 13:34:15.000000 FlowTutor-0.9.0/src/FlowTutor.egg-info/requires.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       10 2023-07-29 13:34:15.000000 FlowTutor-0.9.0/src/FlowTutor.egg-info/top_level.txt
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:34:15.546285 FlowTutor-0.9.0/src/flowtutor/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    10350 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/codegenerator.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      745 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/containers.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     6690 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/debugsession.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:34:15.550286 FlowTutor-0.9.0/src/flowtutor/flowchart/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1914 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/assignment.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2655 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/call.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3054 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/conditional.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5826 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/connection.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      938 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/connector.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4871 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/declaration.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3941 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/declarations.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3027 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/dowhileloop.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    11112 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/flowchart.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4243 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/forloop.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1415 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/functionend.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1778 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/functionstart.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1350 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/input.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     8922 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/node.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1742 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/output.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      477 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/parameter.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1254 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/snippet.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      640 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/struct_definition.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1466 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/struct_member.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2308 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/template.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      624 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/type_definition.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2849 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/flowchart/whileloop.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:34:15.558286 FlowTutor-0.9.0/src/flowtutor/gui/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/__init__.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:34:15.558286 FlowTutor-0.9.0/src/flowtutor/gui/assets/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/assets/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4102 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/assets/c.png
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1852 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/assets/hammer.png
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    98400 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/assets/inconsolata.ttf
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      428 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/assets/pencil.png
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3676 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/assets/python.png
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1829 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/assets/run.png
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1728 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/assets/step_into.png
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1737 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/assets/step_over.png
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1595 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/assets/stop.png
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      332 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/assets/trash.png
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    12776 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/debugger.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    23965 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/gui.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4369 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/menubar_main.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1925 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/section_node_extras.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     9277 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/section_structs.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3281 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/section_typedefs.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      310 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2971 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_assignment.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1326 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_call.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1231 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_conditional.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5424 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_declaration.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     8130 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_declarations.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1233 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_dowhileloop.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2874 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_forloop.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1340 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_functionend.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     6923 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_functionstart.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1448 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_input.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      664 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_multi.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5468 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_none.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1650 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_output.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1244 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_snippet.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2210 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_template.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1218 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/sidebar_whileloop.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    20547 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/themes.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      834 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/gui/window_types.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3955 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/language.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1328 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/main.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     6732 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/modal_service.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2123 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/nodes_service.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/py.typed
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      692 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/settings_service.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5446 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/src/flowtutor/util_service.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-29 13:34:15.558286 FlowTutor-0.9.0/tests/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    23969 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/tests/test_flowtutor_codegenerator.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    10581 2023-07-29 13:30:08.000000 FlowTutor-0.9.0/tests/test_flowtutor_flowchart.py
```

### Comparing `FlowTutor-0.10.9/LICENSE` & `FlowTutor-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowTutor-0.10.9/README.md` & `FlowTutor-0.9.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,146 +1,176 @@
 00000000: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
-00000010: 7222 3e0a 2020 2020 3c69 6d67 2073 7263  r">.    <img src
-00000020: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
-00000030: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00000040: 636f 6d2f 7468 6f6d 6173 726f 6573 736c  com/thomasroessl
-00000050: 2f46 6c6f 7754 7574 6f72 2f6d 6173 7465  /FlowTutor/maste
-00000060: 722f 6c6f 676f 2e70 6e67 2220 616c 743d  r/logo.png" alt=
-00000070: 2266 6c6f 7774 7574 6f72 2d6c 6f67 6f22  "flowtutor-logo"
-00000080: 2073 7479 6c65 3d22 6d61 782d 7769 6474   style="max-widt
-00000090: 683d 3531 3270 783b 6d61 782d 6865 6967  h=512px;max-heig
-000000a0: 6874 3a31 3431 7078 3b22 2f3e 0a3c 2f68  ht:141px;"/>.</h
-000000b0: 313e 0a0a 3c68 3420 616c 6967 6e3d 2263  1>..<h4 align="c
-000000c0: 656e 7465 7222 3e0a 2020 2020 4120 6772  enter">.    A gr
-000000d0: 6170 6869 6361 6c20 7072 6f67 7261 6d6d  aphical programm
-000000e0: 696e 6720 656e 7669 726f 6e6d 656e 7420  ing environment 
-000000f0: 7573 696e 6720 666c 6f77 6368 6172 7473  using flowcharts
-00000100: 2e0a 3c2f 6834 3e0a 0a3c 6831 3e3c 2f68  ..</h4>..<h1></h
-00000110: 313e 0a0a 3c70 2061 6c69 676e 3d22 6365  1>..<p align="ce
-00000120: 6e74 6572 223e 0a20 203c 6120 6872 6566  nter">.  <a href
-00000130: 3d22 223e 3c69 6d67 2073 7263 3d22 6874  =""><img src="ht
-00000140: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000150: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
-00000160: 696f 6e73 2f66 6c6f 7774 7574 6f72 2220  ions/flowtutor" 
-00000170: 616c 743d 2250 7974 686f 6e20 7665 7273  alt="Python vers
-00000180: 696f 6e73 223e 3c2f 613e 0a20 203c 6120  ions"></a>.  <a 
-00000190: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
-000001a0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f66  pi.org/project/f
-000001b0: 6c6f 7774 7574 6f72 2f22 3e3c 696d 6720  lowtutor/"><img 
-000001c0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-000001d0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-000001e0: 2f76 2f66 6c6f 7774 7574 6f72 2220 616c  /v/flowtutor" al
-000001f0: 743d 2250 5950 4922 3e3c 2f61 3e0a 2020  t="PYPI"></a>.  
-00000200: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000210: 2f63 642e 726f 6573 736c 2e6f 7267 2f6a  /cd.roessl.org/j
-00000220: 6f62 2f46 6c6f 7754 7574 6f72 2f22 3e3c  ob/FlowTutor/"><
-00000230: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000240: 2f63 642e 726f 6573 736c 2e6f 7267 2f6a  /cd.roessl.org/j
-00000250: 6f62 2f46 6c6f 7754 7574 6f72 2f62 6164  ob/FlowTutor/bad
-00000260: 6765 2f69 636f 6e22 2061 6c74 3d22 4a65  ge/icon" alt="Je
-00000270: 6e6b 696e 7322 3e3c 2f61 3e0a 3c2f 703e  nkins"></a>.</p>
-00000280: 0a0a 2323 2050 7265 7265 7175 6973 6974  ..## Prerequisit
-00000290: 6573 0a0a 5468 6520 666f 6c6c 6f77 696e  es..The followin
-000002a0: 6720 7072 6f67 7261 6d73 2068 6176 6520  g programs have 
-000002b0: 746f 2062 6520 6176 6169 6c61 626c 6520  to be available 
-000002c0: 6f6e 2074 6865 2073 7973 7465 6d20 666f  on the system fo
-000002d0: 7220 466c 6f77 5475 746f 7220 746f 2062  r FlowTutor to b
-000002e0: 6520 6162 6c65 2074 6f20 7275 6e3a 0a0a  e able to run:..
-000002f0: 2d20 5b50 7974 686f 6e5d 203e 3d20 332e  - [Python] >= 3.
-00000300: 390a 2d20 466f 7220 4320 7072 6f67 7261  9.- For C progra
-00000310: 6d73 206f 6e6c 793a 0a20 2020 202d 205b  ms only:.    - [
-00000320: 4743 435d 202d 2043 2d43 6f6d 7069 6c65  GCC] - C-Compile
-00000330: 720a 2020 2020 2d20 5b47 4442 5d20 2d20  r.    - [GDB] - 
-00000340: 4465 6275 6767 6572 0a0a 2323 2044 6f63  Debugger..## Doc
-00000350: 756d 656e 7461 7469 6f6e 0a0a 416e 206f  umentation..An o
-00000360: 7665 7276 6965 7720 6f66 2046 6c6f 7754  verview of FlowT
-00000370: 7574 6f72 7320 6675 6e63 7469 6f6e 616c  utors functional
-00000380: 6974 7920 6361 6e20 6265 2066 6f75 6e64  ity can be found
-00000390: 2069 6e20 7468 6520 7072 6f6a 6563 7473   in the projects
-000003a0: 205b 5769 6b69 5d0a 0a23 2320 5275 6e6e   [Wiki]..## Runn
-000003b0: 696e 670a 0a46 6c6f 7754 7574 6f72 2069  ing..FlowTutor i
-000003c0: 7320 6176 6169 6c61 626c 6520 7468 726f  s available thro
-000003d0: 7567 6820 7468 6520 5079 7468 6f6e 2050  ugh the Python P
-000003e0: 6163 6b61 6765 2049 6e64 6578 3a0a 0a60  ackage Index:..`
-000003f0: 6060 7368 0a70 7974 686f 6e20 2d6d 2070  ``sh.python -m p
-00000400: 6970 2069 6e73 7461 6c6c 2066 6c6f 7774  ip install flowt
-00000410: 7574 6f72 0a60 6060 0a0a 2323 2052 756e  utor.```..## Run
-00000420: 6e69 6e67 2043 2070 726f 6772 616d 7320  ning C programs 
-00000430: 6f6e 206d 6163 4f53 0a0a 3e20 2a2a 5761  on macOS..> **Wa
-00000440: 726e 696e 672a 2a20 0a3e 2041 7320 6f66  rning** .> As of
-00000450: 204a 756e 6520 3230 3233 2074 6865 7265   June 2023 there
-00000460: 2065 7869 7374 7320 6120 6275 6720 696e   exists a bug in
-00000470: 204d 6163 4f53 2f47 4442 2c20 7468 6174   MacOS/GDB, that
-00000480: 2070 7265 7665 6e74 7320 7468 6520 6465   prevents the de
-00000490: 6275 6767 696e 6720 6675 6e63 7469 6f6e  bugging function
-000004a0: 616c 6974 7920 6f66 2046 6c6f 7754 7574  ality of FlowTut
-000004b0: 6f72 2066 726f 6d20 6675 6e63 7469 6f6e  or from function
-000004c0: 696e 6720 636f 7272 6563 746c 792e 0a0a  ing correctly...
-000004d0: 466c 6f77 7475 746f 7220 7573 6573 2047  Flowtutor uses G
-000004e0: 4442 2066 6f72 2069 7473 2043 2064 6562  DB for its C deb
-000004f0: 7567 6769 6e67 2066 756e 6374 696f 6e61  ugging functiona
-00000500: 6c69 7479 2e0a 4d6f 6465 726e 2044 6172  lity..Modern Dar
-00000510: 7769 6e20 6b65 726e 656c 7320 2875 7365  win kernels (use
-00000520: 6420 696e 206d 6163 4f53 2920 7265 7374  d in macOS) rest
-00000530: 7269 6374 2074 6865 2063 6170 6162 696c  rict the capabil
-00000540: 6974 7920 746f 2061 7373 756d 6520 636f  ity to assume co
-00000550: 6e74 726f 6c20 6f76 6572 2061 6e6f 7468  ntrol over anoth
-00000560: 6572 2070 726f 6365 7373 2c20 7768 6963  er process, whic
-00000570: 6820 4744 4220 6e65 6564 7320 746f 2064  h GDB needs to d
-00000580: 6562 7567 2074 6865 2070 726f 6772 616d  ebug the program
-00000590: 2e0a 546f 2067 6976 6520 7468 6520 636f  ..To give the co
-000005a0: 7272 6563 7420 7065 726d 6973 7369 6f6e  rrect permission
-000005b0: 7320 746f 2047 4442 2069 7420 6e65 6564  s to GDB it need
-000005c0: 7320 746f 2062 6520 5b63 6f64 6520 7369  s to be [code si
-000005d0: 676e 6564 5d2e 0a0a 2323 2320 312e 2043  gned]...### 1. C
-000005e0: 7265 6174 6520 6120 6365 7274 6966 6963  reate a certific
-000005f0: 6174 650a 0a52 756e 2074 6865 2073 6372  ate..Run the scr
-00000600: 6970 7420 606d 6163 6f73 2d73 6574 7570  ipt `macos-setup
-00000610: 2d63 6f64 6573 6967 6e2e 7368 6020 6672  -codesign.sh` fr
-00000620: 6f6d 2074 6865 2060 6764 622d 636f 6465  om the `gdb-code
-00000630: 7369 676e 6020 666f 6c64 6572 2e0a 5468  sign` folder..Th
-00000640: 6973 2073 6574 7320 7570 2061 2063 6572  is sets up a cer
-00000650: 7469 6669 6361 7465 2069 6e20 7468 6520  tificate in the 
-00000660: 5379 7374 656d 204b 6579 6368 6169 6e20  System Keychain 
-00000670: 616e 6420 7472 7573 7473 2074 6865 2063  and trusts the c
-00000680: 6572 7469 6669 6361 7465 2066 6f72 2063  ertificate for c
-00000690: 6f64 6520 7369 676e 696e 672e 0a0a 2323  ode signing...##
-000006a0: 2320 322e 2053 6967 6e20 616e 6420 656e  # 2. Sign and en
-000006b0: 7469 746c 6520 7468 6520 6764 6220 6269  title the gdb bi
-000006c0: 6e61 7279 0a0a 4578 6563 7574 6520 7468  nary..Execute th
-000006d0: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
-000006e0: 616e 6420 7769 7468 2060 6764 622d 656e  and with `gdb-en
-000006f0: 7469 746c 656d 656e 742e 786d 6c60 2066  titlement.xml` f
-00000700: 726f 6d20 7468 6520 6067 6462 2d63 6f64  rom the `gdb-cod
-00000710: 6573 6967 6e60 2066 6f6c 6465 723a 0a0a  esign` folder:..
-00000720: 6060 6073 680a 636f 6465 7369 676e 202d  ```sh.codesign -
-00000730: 2d65 6e74 6974 6c65 6d65 6e74 7320 6764  -entitlements gd
-00000740: 622d 656e 7469 746c 656d 656e 742e 786d  b-entitlement.xm
-00000750: 6c20 2d66 7320 6764 622d 6365 7274 2024  l -fs gdb-cert $
-00000760: 2877 6869 6368 2067 6462 290a 6060 600a  (which gdb).```.
-00000770: 0a23 2323 2033 2e20 5265 626f 6f74 0a0a  .### 3. Reboot..
-00000780: 5468 6973 2072 6566 7265 7368 6573 2074  This refreshes t
-00000790: 6865 2073 7973 7465 6d27 7320 6365 7274  he system's cert
-000007a0: 6966 6963 6174 6573 2061 6e64 2063 6f64  ificates and cod
-000007b0: 652d 7369 676e 696e 6720 6461 7461 2e0a  e-signing data..
-000007c0: 0a23 2320 5769 6e64 6f77 7320 496e 7374  .## Windows Inst
-000007d0: 616c 6c65 7220 5061 636b 6167 6573 0a0a  aller Packages..
-000007e0: 5468 6520 6170 706c 6963 6174 696f 6e20  The application 
-000007f0: 6973 2070 6163 6b61 6765 6420 7769 7468  is packaged with
-00000800: 2050 796e 7369 7374 2066 6f72 2065 6173   Pynsist for eas
-00000810: 6965 7220 6469 7374 7269 6275 7469 6f6e  ier distribution
-00000820: 206f 6e20 5769 6e64 6f77 732e 0a0a 0a5b   on Windows....[
-00000830: 5079 7468 6f6e 5d3a 203c 6874 7470 733a  Python]: <https:
-00000840: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
-00000850: 2f3e 0a5b 4743 435d 3a20 3c68 7474 7073  />.[GCC]: <https
-00000860: 3a2f 2f67 6363 2e67 6e75 2e6f 7267 2f3e  ://gcc.gnu.org/>
-00000870: 0a5b 4744 425d 3a20 3c68 7474 7073 3a2f  .[GDB]: <https:/
-00000880: 2f77 7777 2e73 6f75 7263 6577 6172 652e  /www.sourceware.
-00000890: 6f72 672f 6764 622f 3e0a 5b63 6f64 6520  org/gdb/>.[code 
-000008a0: 7369 676e 6564 5d3a 203c 6874 7470 733a  signed]: <https:
-000008b0: 2f2f 736f 7572 6365 7761 7265 2e6f 7267  //sourceware.org
-000008c0: 2f67 6462 2f77 696b 692f 5065 726d 6973  /gdb/wiki/Permis
-000008d0: 7369 6f6e 7344 6172 7769 6e3e 0a5b 5769  sionsDarwin>.[Wi
-000008e0: 6b69 5d3a 203c 6874 7470 733a 2f2f 6769  ki]: <https://gi
-000008f0: 7468 7562 2e63 6f6d 2f74 686f 6d61 7372  thub.com/thomasr
-00000900: 6f65 7373 6c2f 466c 6f77 5475 746f 722f  oessl/FlowTutor/
-00000910: 7769 6b69 3e                             wiki>
+00000010: 7222 3e46 6c6f 7754 7574 6f72 3c2f 6831  r">FlowTutor</h1
+00000020: 3e0a 0a3c 7020 616c 6967 6e3d 2263 656e  >..<p align="cen
+00000030: 7465 7222 3e0a 2020 3c69 6d67 2073 7263  ter">.  <img src
+00000040: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+00000050: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000060: 636f 6d2f 7468 6f6d 6173 726f 6573 736c  com/thomasroessl
+00000070: 2f46 6c6f 7754 7574 6f72 2f6d 6173 7465  /FlowTutor/maste
+00000080: 722f 6c6f 676f 2e70 6e67 2220 616c 743d  r/logo.png" alt=
+00000090: 2266 6c6f 7774 7574 6f72 2d6c 6f67 6f22  "flowtutor-logo"
+000000a0: 2077 6964 7468 3d22 3531 3270 7822 2068   width="512px" h
+000000b0: 6569 6768 743d 2231 3431 7078 222f 3e0a  eight="141px"/>.
+000000c0: 2020 3c62 723e 0a20 203c 656d 3e46 6c6f    <br>.  <em>Flo
+000000d0: 7754 7574 6f72 2069 7320 6120 6772 6170  wTutor is a grap
+000000e0: 6869 6361 6c20 7072 6f67 7261 6d6d 696e  hical programmin
+000000f0: 6720 656e 7669 726f 6e6d 656e 7420 6465  g environment de
+00000100: 7369 676e 6564 2074 6f20 6361 7465 7220  signed to cater 
+00000110: 746f 2074 6865 206e 6565 6473 206f 6620  to the needs of 
+00000120: 656e 6769 6e65 6572 696e 6720 7374 7564  engineering stud
+00000130: 656e 7473 2e3c 2f65 6d3e 0a20 203c 6272  ents.</em>.  <br
+00000140: 3e0a 3c2f 703e 0a0a 2323 2050 7265 7265  >.</p>..## Prere
+00000150: 7175 6973 6974 6573 0a0a 5468 6520 666f  quisites..The fo
+00000160: 6c6c 6f77 696e 6720 7072 6f67 7261 6d73  llowing programs
+00000170: 2068 6176 6520 746f 2062 6520 6176 6169   have to be avai
+00000180: 6c61 626c 6520 6f6e 2074 6865 2073 7973  lable on the sys
+00000190: 7465 6d20 666f 7220 466c 6f77 5475 746f  tem for FlowTuto
+000001a0: 7220 746f 2062 6520 6162 6c65 2074 6f20  r to be able to 
+000001b0: 7275 6e3a 0a0a 2d20 5b50 7974 686f 6e5d  run:..- [Python]
+000001c0: 203e 3d20 332e 390a 2d20 5b74 6b69 6e74   >= 3.9.- [tkint
+000001d0: 6572 5d20 2d20 466f 7220 7379 7374 656d  er] - For system
+000001e0: 2066 696c 6520 6469 616c 6f67 730a 2d20   file dialogs.- 
+000001f0: 5b47 4343 5d20 2d20 432d 436f 6d70 696c  [GCC] - C-Compil
+00000200: 6572 0a2d 205b 4744 425d 202d 2044 6562  er.- [GDB] - Deb
+00000210: 7567 6765 720a 0a23 2320 446f 6375 6d65  ugger..## Docume
+00000220: 6e74 6174 696f 6e0a 0a41 6e20 6f76 6572  ntation..An over
+00000230: 7669 6577 206f 6620 466c 6f77 5475 746f  view of FlowTuto
+00000240: 7273 2066 756e 6374 696f 6e61 6c69 7479  rs functionality
+00000250: 2063 616e 2062 6520 666f 756e 6420 696e   can be found in
+00000260: 2074 6865 2070 726f 6a65 6374 7320 5b57   the projects [W
+00000270: 696b 695d 0a0a 2323 2052 756e 6e69 6e67  iki]..## Running
+00000280: 2074 6865 2050 7974 686f 6e20 7072 6f6a   the Python proj
+00000290: 6563 7420 6672 6f6d 2073 6f75 7263 650a  ect from source.
+000002a0: 0a31 2e20 4372 6561 7465 2061 2076 6972  .1. Create a vir
+000002b0: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
+000002c0: 3a0a 2020 2020 6060 6073 680a 2020 2020  :.    ```sh.    
+000002d0: 7079 7468 6f6e 202d 6d20 7665 6e76 2076  python -m venv v
+000002e0: 656e 760a 2020 2020 6060 600a 0a32 2e20  env.    ```..2. 
+000002f0: 4163 7469 7661 7465 2074 6865 2076 6972  Activate the vir
+00000300: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
+00000310: 3a0a 2020 2020 6060 6073 680a 2020 2020  :.    ```sh.    
+00000320: 736f 7572 6365 2076 656e 762f 6269 6e2f  source venv/bin/
+00000330: 6163 7469 7661 7465 0a20 2020 2060 6060  activate.    ```
+00000340: 0a0a 332e 2049 6e73 7461 6c6c 2074 6865  ..3. Install the
+00000350: 2046 6c6f 7754 7574 6f72 2070 6163 6b61   FlowTutor packa
+00000360: 6765 3a0a 2020 2020 6060 6073 680a 2020  ge:.    ```sh.  
+00000370: 2020 7079 7468 6f6e 202d 6d20 7069 7020    python -m pip 
+00000380: 696e 7374 616c 6c20 2e0a 2020 2020 6060  install ..    ``
+00000390: 600a 0a36 2e20 5275 6e20 466c 6f77 5475  `..6. Run FlowTu
+000003a0: 746f 723a 0a20 2020 2060 6060 7368 0a20  tor:.    ```sh. 
+000003b0: 2020 2066 6c6f 7774 7574 6f72 0a20 2020     flowtutor.   
+000003c0: 2060 6060 0a0a 2323 2052 756e 6e69 6e67   ```..## Running
+000003d0: 206f 6e20 6d61 634f 530a 0a3e 202a 2a57   on macOS..> **W
+000003e0: 6172 6e69 6e67 2a2a 200a 3e20 4173 206f  arning** .> As o
+000003f0: 6620 4a75 6e65 2032 3032 3320 7468 6572  f June 2023 ther
+00000400: 6520 6578 6973 7473 2061 2062 7567 2069  e exists a bug i
+00000410: 6e20 4d61 634f 532f 4744 422c 2074 6861  n MacOS/GDB, tha
+00000420: 7420 7072 6576 656e 7473 2074 6865 2064  t prevents the d
+00000430: 6562 7567 6769 6e67 2066 756e 6374 696f  ebugging functio
+00000440: 6e61 6c69 7479 206f 6620 466c 6f77 5475  nality of FlowTu
+00000450: 746f 7220 6672 6f6d 2066 756e 6374 696f  tor from functio
+00000460: 6e69 6e67 2063 6f72 7265 6374 6c79 2e0a  ning correctly..
+00000470: 0a46 6c6f 7774 7574 6f72 2075 7365 7320  .Flowtutor uses 
+00000480: 4744 4220 666f 7220 6974 7320 6465 6275  GDB for its debu
+00000490: 6767 696e 6720 6675 6e63 7469 6f6e 616c  gging functional
+000004a0: 6974 792e 0a4d 6f64 6572 6e20 4461 7277  ity..Modern Darw
+000004b0: 696e 206b 6572 6e65 6c73 2028 7573 6564  in kernels (used
+000004c0: 2069 6e20 6d61 634f 5329 2072 6573 7472   in macOS) restr
+000004d0: 6963 7420 7468 6520 6361 7061 6269 6c69  ict the capabili
+000004e0: 7479 2074 6f20 6173 7375 6d65 2063 6f6e  ty to assume con
+000004f0: 7472 6f6c 206f 7665 7220 616e 6f74 6865  trol over anothe
+00000500: 7220 7072 6f63 6573 732c 2077 6869 6368  r process, which
+00000510: 2047 4442 206e 6565 6473 2074 6f20 6465   GDB needs to de
+00000520: 6275 6720 7468 6520 7072 6f67 7261 6d2e  bug the program.
+00000530: 0a54 6f20 6769 7665 2074 6865 2063 6f72  .To give the cor
+00000540: 7265 6374 2070 6572 6d69 7373 696f 6e73  rect permissions
+00000550: 2074 6f20 4744 4220 6974 206e 6565 6473   to GDB it needs
+00000560: 2074 6f20 6265 205b 636f 6465 2073 6967   to be [code sig
+00000570: 6e65 645d 2e0a 0a23 2323 2031 2e20 4372  ned]...### 1. Cr
+00000580: 6561 7465 2061 2063 6572 7469 6669 6361  eate a certifica
+00000590: 7465 0a52 756e 2074 6865 2073 6372 6970  te.Run the scrip
+000005a0: 7420 606d 6163 6f73 2d73 6574 7570 2d63  t `macos-setup-c
+000005b0: 6f64 6573 6967 6e2e 7368 6020 6672 6f6d  odesign.sh` from
+000005c0: 2074 6865 2060 6764 622d 636f 6465 7369   the `gdb-codesi
+000005d0: 676e 6020 666f 6c64 6572 2e0a 5468 6973  gn` folder..This
+000005e0: 2073 6574 7320 7570 2061 2063 6572 7469   sets up a certi
+000005f0: 6669 6361 7465 2069 6e20 7468 6520 5379  ficate in the Sy
+00000600: 7374 656d 204b 6579 6368 6169 6e20 616e  stem Keychain an
+00000610: 6420 7472 7573 7473 2074 6865 2063 6572  d trusts the cer
+00000620: 7469 6669 6361 7465 2066 6f72 2063 6f64  tificate for cod
+00000630: 6520 7369 676e 696e 672e 0a0a 2323 2320  e signing...### 
+00000640: 322e 2053 6967 6e20 616e 6420 656e 7469  2. Sign and enti
+00000650: 746c 6520 7468 6520 6764 6220 6269 6e61  tle the gdb bina
+00000660: 7279 0a45 7865 6375 7465 2074 6865 2066  ry.Execute the f
+00000670: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00000680: 2077 6974 6820 6067 6462 2d65 6e74 6974   with `gdb-entit
+00000690: 6c65 6d65 6e74 2e78 6d6c 6020 6672 6f6d  lement.xml` from
+000006a0: 2074 6865 2060 6764 622d 636f 6465 7369   the `gdb-codesi
+000006b0: 676e 6020 666f 6c64 6572 3a0a 6060 6073  gn` folder:.```s
+000006c0: 680a 636f 6465 7369 676e 202d 2d65 6e74  h.codesign --ent
+000006d0: 6974 6c65 6d65 6e74 7320 6764 622d 656e  itlements gdb-en
+000006e0: 7469 746c 656d 656e 742e 786d 6c20 2d66  titlement.xml -f
+000006f0: 7320 6764 622d 6365 7274 2024 2877 6869  s gdb-cert $(whi
+00000700: 6368 2067 6462 290a 6060 600a 0a23 2323  ch gdb).```..###
+00000710: 2033 2e20 5265 626f 6f74 0a54 6869 7320   3. Reboot.This 
+00000720: 7265 6672 6573 6865 7320 7468 6520 7379  refreshes the sy
+00000730: 7374 656d 2773 2063 6572 7469 6669 6361  stem's certifica
+00000740: 7465 7320 616e 6420 636f 6465 2d73 6967  tes and code-sig
+00000750: 6e69 6e67 2064 6174 612e 0a0a 2323 2057  ning data...## W
+00000760: 696e 646f 7773 2049 6e73 7461 6c6c 6572  indows Installer
+00000770: 2050 6163 6b61 6765 730a 0a54 6865 2061   Packages..The a
+00000780: 7070 6c69 6361 7469 6f6e 2069 7320 7061  pplication is pa
+00000790: 636b 6167 6564 2077 6974 6820 5079 6e73  ckaged with Pyns
+000007a0: 6973 7420 666f 7220 6561 7369 6572 2064  ist for easier d
+000007b0: 6973 7472 6962 7574 696f 6e20 6f6e 2057  istribution on W
+000007c0: 696e 646f 7773 2e0a 0a42 6563 6175 7365  indows...Because
+000007d0: 2050 796e 7369 7374 206d 616b 6573 2075   Pynsist makes u
+000007e0: 7365 206f 6620 7468 6520 e280 9c62 756e  se of the ...bun
+000007f0: 646c 6564 e280 9d20 7665 7273 696f 6e73  dled... versions
+00000800: 206f 6620 5079 7468 6f6e 2074 6865 2060   of Python the `
+00000810: 746b 696e 7465 7260 206d 6f64 756c 6520  tkinter` module 
+00000820: 6973 6ee2 8099 7420 696e 636c 7564 6564  isn...t included
+00000830: 2062 7920 6465 6661 756c 742e 0a0a 466f   by default...Fo
+00000840: 7220 7468 6520 6375 7272 656e 746c 7920  r the currently 
+00000850: 7573 6564 2076 6572 7369 6f6e 206f 6620  used version of 
+00000860: 5079 7468 6f6e 2074 6865 205b 6e65 6365  Python the [nece
+00000870: 7373 6172 7920 6669 6c65 735d 2c20 6e61  ssary files], na
+00000880: 6d65 6c79 2060 5f74 6b69 6e74 6572 2e6c  mely `_tkinter.l
+00000890: 6962 602c 2060 5f74 6b69 6e74 6572 2e70  ib`, `_tkinter.p
+000008a0: 7964 602c 2060 5f74 6b69 6e74 6572 2e6c  yd`, `_tkinter.l
+000008b0: 6962 602c 2060 7463 6c38 3674 2e64 6c6c  ib`, `tcl86t.dll
+000008c0: 6020 616e 6420 6074 6b38 3674 2e64 6c6c  ` and `tk86t.dll
+000008d0: 6020 696e 2060 7079 6e73 6973 745f 706b  ` in `pynsist_pk
+000008e0: 732f 6020 616e 6420 7468 6520 636f 6e74  s/` and the cont
+000008f0: 656e 7473 206f 6620 606c 6962 2f60 2066  ents of `lib/` f
+00000900: 6f6c 6465 722c 2068 6176 6520 6265 656e  older, have been
+00000910: 2063 6f72 7265 6374 6c79 2069 6e63 6c75   correctly inclu
+00000920: 6465 642e 0a0a 5368 6f75 6c64 2074 6865  ded...Should the
+00000930: 2062 756e 646c 6564 2050 7974 686f 6e20   bundled Python 
+00000940: 7665 7273 696f 6e20 6368 616e 6765 2c20  version change, 
+00000950: 7468 6573 6520 6669 6c65 7320 6861 7665  these files have
+00000960: 2074 6f20 6265 2072 6570 6c61 6365 6420   to be replaced 
+00000970: 6163 636f 7264 696e 676c 792e 0a0a 5b50  accordingly...[P
+00000980: 7974 686f 6e5d 3a20 3c68 7474 7073 3a2f  ython]: <https:/
+00000990: 2f77 7777 2e70 7974 686f 6e2e 6f72 672f  /www.python.org/
+000009a0: 3e0a 5b74 6b69 6e74 6572 5d3a 203c 6874  >.[tkinter]: <ht
+000009b0: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
+000009c0: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
+000009d0: 746b 696e 7465 722e 6874 6d6c 3e0a 5b47  tkinter.html>.[G
+000009e0: 4343 5d3a 203c 6874 7470 733a 2f2f 6763  CC]: <https://gc
+000009f0: 632e 676e 752e 6f72 672f 3e0a 5b47 4442  c.gnu.org/>.[GDB
+00000a00: 5d3a 203c 6874 7470 733a 2f2f 7777 772e  ]: <https://www.
+00000a10: 736f 7572 6365 7761 7265 2e6f 7267 2f67  sourceware.org/g
+00000a20: 6462 2f3e 0a5b 636f 6465 2073 6967 6e65  db/>.[code signe
+00000a30: 645d 3a20 3c68 7474 7073 3a2f 2f73 6f75  d]: <https://sou
+00000a40: 7263 6577 6172 652e 6f72 672f 6764 622f  rceware.org/gdb/
+00000a50: 7769 6b69 2f50 6572 6d69 7373 696f 6e73  wiki/Permissions
+00000a60: 4461 7277 696e 3e0a 5b6e 6563 6573 7361  Darwin>.[necessa
+00000a70: 7279 2066 696c 6573 5d3a 203c 6874 7470  ry files]: <http
+00000a80: 733a 2f2f 7079 6e73 6973 742e 7265 6164  s://pynsist.read
+00000a90: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00000aa0: 7465 7374 2f66 6171 2e68 746d 6c23 7061  test/faq.html#pa
+00000ab0: 636b 6167 696e 672d 7769 7468 2d74 6b69  ckaging-with-tki
+00000ac0: 6e74 6572 3e0a 5b57 696b 695d 3a20 3c68  nter>.[Wiki]: <h
+00000ad0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ae0: 6d2f 7468 6f6d 6173 726f 6573 736c 2f46  m/thomasroessl/F
+00000af0: 6c6f 7754 7574 6f72 2f77 696b 693e       lowTutor/wiki>
```

### Comparing `FlowTutor-0.10.9/pyproject.toml` & `FlowTutor-0.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,37 @@
 [project]
 name = "FlowTutor"
 description = "A graphical programming environment using flowcharts."
-version = "0.10.9"
+version = "0.9.0"
 readme = "README.md"
 authors = [
   {name = "Thomas Rößl", email = "e11775192@student.tuwien.ac.at"}
 ]
 requires-python = ">=3.9"
-dependencies = [
-    "appdirs>=1.4",
-    "blinker>=1.6",
-    "dearpygui>=1.10",
-    "Shapely>=2.0",
-    "dependency-injector>=4.41",
-    "pygdbmi>=0.11",
-    "urllib3>=1.26",
-    "Jinja2>=3.1"
-]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Topic :: Education",
     "Topic :: Software Development",
     "Intended Audience :: Education",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)"
 ]
 
-[project.optional-dependencies]
-testing = [
-    "pytest>=7.4",
-    "pytest-cov>=4.1",
-    "mypy>=1.6",
-    "flake8>=6.1",
-    "tox>=4.11"
-]
-deployment = [
-    "pynsist>=2.8",
-    "twine>=4.0",
-    "build>=1.0"
-]
-
 [project.urls]
-Documentation = "https://github.com/thomasroessl/FlowTutor/wiki"
-Source = "https://github.com/thomasroessl/FlowTutor"
-Changelog = "https://github.com/thomasroessl/FlowTutor/releases"
-
-[project.scripts]
-flowtutor = "flowtutor.main:main"
-
-[project.gui-scripts]
-flowtutor = "flowtutor.main:main"
-
-[tool.setuptools]
-package-dir = {"" = "src"}
-
-[tool.setuptools.packages.find]
-where = ["src"]
-
-[tool.setuptools.package-data]
-flowtutor = ["py.typed"]
+documentation = "https://github.com/thomasroessl/FlowTutor/wiki"
+source = "https://github.com/thomasroessl/FlowTutor"
+changelog = "https://github.com/thomasroessl/FlowTutor/releases"
 
 [build-system]
-requires = ["setuptools>=68.2", "wheel"]
+requires = ["setuptools>=68.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.mypy]
 mypy_path = "src"
 strict = true
 check_untyped_defs = true
 disallow_any_generics = true
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/containers.py` & `FlowTutor-0.9.0/src/flowtutor/containers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 from dependency_injector import containers, providers
 
 from flowtutor.codegenerator import CodeGenerator
 from flowtutor.modal_service import ModalService
 from flowtutor.util_service import UtilService
 from flowtutor.settings_service import SettingsService
-from flowtutor.language_service import LanguageService
+
+from flowtutor.nodes_service import NodesService
 
 
 class Container(containers.DeclarativeContainer):
-    '''The container for dependency injection.'''
 
     utils_service = providers.Singleton(
         UtilService
     )
 
     code_generator = providers.Singleton(
         CodeGenerator
@@ -23,10 +23,10 @@
         ModalService
     )
 
     settings_service = providers.Singleton(
         SettingsService
     )
 
-    language_service = providers.Singleton(
-        LanguageService
+    nodes_service = providers.Singleton(
+        NodesService
     )
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/flowchart/connector.py` & `FlowTutor-0.9.0/src/flowtutor/flowchart/connector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 from shapely.geometry import Point
 
 from flowtutor.flowchart.node import Node
 
 
 class Connector(Node):
-    '''A connecting node for connecting the branches after a decision.'''
 
     def __init__(self) -> None:
         super().__init__()
-        self._shape_data = [list(Point(25, 25).buffer(25).exterior.coords)]
+        self._shape_points = list(Point(25, 25).buffer(25).exterior.coords)
 
     @property
     def shape_width(self) -> int:
         return 50
 
     @property
     def shape_height(self) -> int:
@@ -28,13 +27,17 @@
         return [(25, 50)]
 
     @property
     def color(self) -> tuple[int, int, int]:
         return (255, 170, 170)
 
     @property
+    def shape_points(self) -> list[tuple[float, float]]:
+        return self._shape_points
+
+    @property
     def label(self) -> str:
         return ''
 
     @property
     def is_initialized(self) -> bool:
         return True
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/flowchart/functionend.py` & `FlowTutor-0.9.0/src/flowtutor/flowchart/functionend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-from dependency_injector.wiring import Provide, inject
-
 from flowtutor.flowchart.node import Node
-from flowtutor.language_service import LanguageService
+from flowtutor.language import Language
 
 
 class FunctionEnd(Node):
 
-    @inject
-    def __init__(self, name: str = '', language_service: LanguageService = Provide['language_service']):
+    def __init__(self, name: str = ''):
         super().__init__()
-        self._shape_data, self.default_color = language_service.get_node_shape_data('terminator')
+        self._shape_points, self.default_color = Language.get_node_shape_data('terminator')
         self._name = name
         self._return_value = '0'
 
     @property
     def shape_width(self) -> int:
         return 150
 
@@ -30,14 +27,18 @@
         return []
 
     @property
     def color(self) -> tuple[int, int, int]:
         return self.default_color
 
     @property
+    def shape_points(self) -> list[tuple[float, float]]:
+        return self._shape_points
+
+    @property
     def name(self) -> str:
         return self._name
 
     @name.setter
     def name(self, name: str) -> None:
         self._name = name
 
@@ -47,12 +48,12 @@
 
     @return_value.setter
     def return_value(self, return_value: str) -> None:
         self._return_value = return_value
 
     @property
     def label(self) -> str:
-        return f'return {self.return_value}'
+        return f'return {self.return_value};'
 
     @property
     def is_initialized(self) -> bool:
-        return True
+        return self.is_comment or len(self.return_value) > 0
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/flowchart/functionstart.py` & `FlowTutor-0.9.0/src/flowtutor/flowchart/assignment.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING
-from dependency_injector.wiring import Provide, inject
 
 from flowtutor.flowchart.node import Node
-from flowtutor.flowchart.parameter import Parameter
+from flowtutor.language import Language
 
-if TYPE_CHECKING:
-    from flowtutor.language_service import LanguageService
 
+class Assignment(Node):
 
-class FunctionStart(Node):
-
-    @inject
-    def __init__(self, name: str = '', language_service: LanguageService = Provide['language_service']) -> None:
+    def __init__(self) -> None:
         super().__init__()
-        self._shape_data, self.default_color = language_service.get_node_shape_data('terminator')
-        self._name = name
-        self._return_type = 'int'
-        self._parameters: list[Parameter] = []
+        self._shape_points, self.default_color = Language.get_node_shape_data('process')
+        self._var_name = ''
+        self._var_offset = ''
+        self._var_value = ''
 
     @property
     def shape_width(self) -> int:
         return 150
 
     @property
     def shape_height(self) -> int:
@@ -33,41 +27,47 @@
 
     @property
     def raw_out_points(self) -> list[tuple[float, float]]:
         return [(75, 75)]
 
     @property
     def color(self) -> tuple[int, int, int]:
-        return self.default_color
+        return self.default_color if self.is_initialized else (255, 0, 0)
 
     @property
-    def name(self) -> str:
-        return self._name
+    def shape_points(self) -> list[tuple[float, float]]:
+        return self._shape_points
 
-    @name.setter
-    def name(self, name: str) -> None:
-        self._name = name
+    @property
+    def label(self) -> str:
+        if self.var_name and self.var_value:
+            return f'{self.var_name}{f"[{self.var_offset}]" if len(self.var_offset) > 0 else ""} = {self.var_value}'
+        else:
+            return self.__class__.__name__
 
     @property
-    def return_type(self) -> str:
-        return self._return_type
+    def var_name(self) -> str:
+        return self._var_name
 
-    @return_type.setter
-    def return_type(self, return_type: str) -> None:
-        self._return_type = return_type
+    @var_name.setter
+    def var_name(self, var_name: str) -> None:
+        self._var_name = var_name
 
     @property
-    def parameters(self) -> list[Parameter]:
-        if not hasattr(self, '_parameters'):
-            self._parameters = []
-        return self._parameters
+    def var_offset(self) -> str:
+        return self._var_offset
+
+    @var_offset.setter
+    def var_offset(self, var_offset: str) -> None:
+        self._var_offset = var_offset
 
     @property
-    def label(self) -> str:
-        return self.name
+    def var_value(self) -> str:
+        return self._var_value
+
+    @var_value.setter
+    def var_value(self, var_value: str) -> None:
+        self._var_value = var_value
 
     @property
     def is_initialized(self) -> bool:
-        if hasattr(self, '_parameters'):
-            return self.is_comment or all(len(p.name) > 0 for p in self.parameters)
-        else:
-            return True
+        return self.is_comment or (len(self.var_name) > 0 and len(self.var_value) > 0)
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/flowchart/struct_definition.py` & `FlowTutor-0.9.0/src/flowtutor/flowchart/struct_definition.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 
 from flowtutor.flowchart.struct_member import StructMember
 
 
 class StructDefinition:
-    '''A struct definition for C style structs.'''
 
     def __init__(self) -> None:
         self._name = ''
         self._members: list[StructMember] = [StructMember()]
 
     @property
     def name(self) -> str:
-        '''The name of the struct.'''
         return self._name
 
     @name.setter
     def name(self, name: str) -> None:
         self._name = name
 
     @property
     def members(self) -> list[StructMember]:
-        '''A list of struct members.'''
         return self._members
 
     def __repr__(self) -> str:
         members = '\n  '.join([m for m in map(lambda m: str(m), self.members)])
         return f'typedef struct {self.name}_s {{\n  { members }\n}} {self.name}_t;'
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/flowchart/struct_member.py` & `FlowTutor-0.9.0/src/flowtutor/flowchart/struct_member.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,54 @@
 class StructMember:
-    '''A member of a C style struct.'''
 
     def __init__(self) -> None:
         self._name = ''
         self._type = 'int'
         self._array_size = ''
         self._is_array = False
         self._is_pointer = False
 
     @property
     def name(self) -> str:
-        '''The name of the struct member.'''
         return self._name
 
     @name.setter
     def name(self, name: str) -> None:
         self._name = name
 
     @property
     def type(self) -> str:
-        '''The data type of the struct member.'''
         return self._type
 
     @type.setter
     def type(self, type: str) -> None:
         self._type = type
 
     @property
     def is_array(self) -> bool:
-        '''True if the struct member is an array.'''
         return self._is_array
 
     @is_array.setter
     def is_array(self, is_array: bool) -> None:
         self._is_array = is_array
         if not is_array:
             self.array_size = ''
         else:
             self.is_pointer = False
 
     @property
     def array_size(self) -> str:
-        '''The size of the array.
-
-        Only applicable for arrays.
-        '''
         return self._array_size
 
     @array_size.setter
     def array_size(self, array_size: str) -> None:
         self._array_size = array_size
 
     @property
     def is_pointer(self) -> bool:
-        '''True if the struct member is a pointer.'''
         return self._is_pointer
 
     @is_pointer.setter
     def is_pointer(self, is_pointer: bool) -> None:
         self._is_pointer = is_pointer
         if is_pointer:
             self.is_array = False
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/flowchart/type_definition.py` & `FlowTutor-0.9.0/src/flowtutor/flowchart/type_definition.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 
 
 class TypeDefinition:
-    '''Represents a C style type definition.'''
 
     def __init__(self) -> None:
         self._name = ''
         self._definition = ''
 
     @property
     def name(self) -> str:
-        '''The name of the type.'''
         return self._name
 
     @name.setter
     def name(self, name: str) -> None:
         self._name = name
 
     @property
     def definition(self) -> str:
-        '''The definition.'''
         return self._definition
 
     @definition.setter
     def definition(self, definition: str) -> None:
         self._definition = definition
 
     def __repr__(self) -> str:
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/assets/hammer.png` & `FlowTutor-0.9.0/src/flowtutor/gui/assets/hammer.png`

 * *Files identical despite different names*

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/assets/inconsolata.ttf` & `FlowTutor-0.9.0/src/flowtutor/gui/assets/inconsolata.ttf`

 * *Files identical despite different names*

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/assets/run.png` & `FlowTutor-0.9.0/src/flowtutor/gui/assets/run.png`

 * *Files identical despite different names*

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/assets/step_into.png` & `FlowTutor-0.9.0/src/flowtutor/gui/assets/step_into.png`

 * *Files identical despite different names*

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/assets/step_over.png` & `FlowTutor-0.9.0/src/flowtutor/gui/assets/step_over.png`

 * *Files identical despite different names*

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/assets/stop.png` & `FlowTutor-0.9.0/src/flowtutor/gui/assets/stop.png`

 * *Files identical despite different names*

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/debugger.py` & `FlowTutor-0.9.0/src/flowtutor/gui/debugger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,43 @@
-from __future__ import annotations
-from re import sub
-from subprocess import run
-from sys import stderr
+import re
+import subprocess
+import sys
 from time import sleep
-from typing import TYPE_CHECKING, Any, Optional, Union
+from typing import Any, Optional, Union
 import dearpygui.dearpygui as dpg
 from blinker import signal
 from dependency_injector.wiring import Provide, inject
 
-from flowtutor.debugger.debugsession import DebugSession
-from flowtutor.debugger.ftdbsession import FtdbSession
-from flowtutor.debugger.gdbsession import GdbSession
-
-if TYPE_CHECKING:
-    from flowtutor.util_service import UtilService
-    from flowtutor.flowchart.flowchart import Flowchart
-    from flowtutor.language_service import LanguageService
-
+from flowtutor.util_service import UtilService
+from flowtutor.debugsession import DebugSession
 
 LOADING_INDICATOR_TAG = 'loading_indicator'
 
 
 class Debugger:
-    '''The GUI for debugging.'''
+
+    debug_session: Optional[DebugSession] = None
 
     @inject
-    def __init__(self,
-                 parent: Union[str, int],
-                 utils_service: UtilService = Provide['utils_service'],
-                 language_service: LanguageService = Provide['language_service']) -> None:
+    def __init__(self, parent: Union[str, int], utils_service: UtilService = Provide['utils_service']) -> None:
+
         self.utils = utils_service
-        self.language_service = language_service
-        self._auto_scroll = True
 
-        self.debug_session: Optional[DebugSession] = None
-        '''The DebugSession object used for debugging.'''
-        self.flowchart: Optional[Flowchart] = None
-        '''The flowchart to be debugged.'''
-        self.filter_id: Optional[Union[int, str]] = None
-        '''The tag of the dpg filter item.'''
-        self.input_id: Optional[Union[int, str]] = None
-        '''The tag of the dpg input item used for user input.'''
-        self.window_id: Union[int, str] = parent
-        '''The tag of the parent dpg window.'''
+        self.log_level = 0
+        self._auto_scroll = True
+        self.filter_id = None
+        self.input_id = None
+        self.window_id = parent
         self.log_count = 0
-        '''The number of logged lines.'''
+        self.log_flush_count = 1000
         self.log_last_line: Optional[Union[int, str]] = None
-        '''The tag of th elast log line dpg item.'''
 
         signal('program-finished').connect(self.on_program_finished)
         signal('program-kiled').connect(self.on_program_killed)
-        signal('recieve-output').connect(self.on_recieve_output)
+        signal('recieve_output').connect(self.on_recieve_output)
         signal('program-error').connect(self.on_program_error)
 
         with dpg.group(horizontal=True, parent=self.window_id) as self.controls_group:
             self.build_button = dpg.add_image_button('hammer_image', callback=self.on_build)
 
             with dpg.group(horizontal=True):
                 self.run_button = dpg.add_image_button('run_image',
@@ -77,38 +60,37 @@
                 self.auto_scroll_cb = dpg.add_checkbox(label='Auto-scroll',
                                                        default_value=True,
                                                        pos=(205, 3),
                                                        callback=lambda sender: self.auto_scroll(dpg.get_value(sender)))
                 self.clear_button = dpg.add_button(label='Clear Log',
                                                    pos=(340, 0),
                                                    callback=lambda: dpg.delete_item(self.filter_id, children_only=True))
-                # Set the padding of the dpg group
                 with dpg.theme() as item_theme:
                     with dpg.theme_component(dpg.mvGroup):
                         dpg.add_theme_style(dpg.mvStyleVar_CellPadding, 0.0, category=dpg.mvThemeCat_Core)
                 dpg.bind_item_theme(g1, item_theme)
 
-            # Set the paddin goof the tool buttons
             with dpg.theme() as tool_button_theme:
                 with dpg.theme_component(dpg.mvImageButton):
                     dpg.add_theme_style(dpg.mvStyleVar_FramePadding, 5, 5, category=dpg.mvThemeCat_Core)
                 with dpg.theme_component(dpg.mvImageButton, enabled_state=False):
                     dpg.add_theme_style(dpg.mvStyleVar_FramePadding, 5, 5, category=dpg.mvThemeCat_Core)
+
             dpg.bind_item_theme(self.build_button, tool_button_theme)
             dpg.bind_item_theme(self.run_button, tool_button_theme)
             dpg.bind_item_theme(self.step_over_button, tool_button_theme)
             dpg.bind_item_theme(self.step_into_button, tool_button_theme)
             dpg.bind_item_theme(self.stop_button, tool_button_theme)
 
-            # Set the padding of the clear button
             with dpg.theme() as clear_button_theme:
                 with dpg.theme_component(dpg.mvButton):
                     dpg.add_theme_style(dpg.mvStyleVar_FramePadding, 12, 6, category=dpg.mvThemeCat_Core)
                 with dpg.theme_component(dpg.mvButton, enabled_state=False):
                     dpg.add_theme_style(dpg.mvStyleVar_FramePadding, 5, 5, category=dpg.mvThemeCat_Core)
+
             dpg.bind_item_theme(self.clear_button, clear_button_theme)
 
         self.child_id = dpg.add_child_window(parent=self.window_id, autosize_x=True, autosize_y=True)
         self.filter_id = dpg.add_filter_set(parent=self.child_id)
 
         if not self.utils.is_windows:
             dpg.configure_item(self.child_id, autosize_y=False, height=190)
@@ -136,108 +118,62 @@
             with dpg.theme_component(0):
                 dpg.add_theme_color(dpg.mvThemeCol_Text, (255, 191, 0, 255))
 
         with dpg.theme() as self.error_theme:
             with dpg.theme_component(0):
                 dpg.add_theme_color(dpg.mvThemeCol_Text, (255, 0, 0, 255))
 
-    def refresh(self, flowchart: Flowchart) -> None:
-        '''Refresh the GUI for the current language.
-
-        Compiled lanuages like C get a build button, others do not.
-        '''
-        self.flowchart = flowchart
-        if self.language_service.is_compiled(self.flowchart):
-            dpg.show_item(self.build_button)
-        else:
-            dpg.hide_item(self.build_button)
-
     def on_input(self) -> None:
-        '''Handle user input.'''
-        input_value = dpg.get_value(self.input_id)
-        if self.debug_session:
-            self.debug_session.write(input_value)
+        self.utils.write_tty(dpg.get_value(self.input_id))
         dpg.configure_item(self.input_id, default_value='')
 
     def disable_all(self) -> None:
-        '''Diable all controls of the debugger.'''
         self.disable_children(self.controls_group)
         dpg.enable_item(self.auto_scroll_cb)
         dpg.enable_item(self.clear_button)
 
-    def enable_build_only(self, flowchart: Flowchart) -> None:
-        '''Enable only the build button. For non-compiled languages this enables the run button.
-
-        Parameters:
-            flowchart (Flowchart): The flowchart to debug.
-        '''
-        self.flowchart = flowchart
+    def enable_build_only(self) -> None:
         self.disable_all()
-        if self.language_service.is_compiled(self.flowchart):
-            dpg.enable_item(self.build_button)
-            dpg.show_item(self.build_button)
-        else:
-            dpg.enable_item(self.run_button)
-            dpg.hide_item(self.build_button)
+        dpg.enable_item(self.build_button)
 
     def enable_build_and_run(self) -> None:
-        '''Enables the build and run buttons.'''
         self.disable_all()
         dpg.enable_item(self.build_button)
         dpg.enable_item(self.run_button)
 
     def enable_all(self) -> None:
-        '''Enables all controls of the debugger.'''
         self.enable_children(self.controls_group)
 
     def disable_children(self, item: Union[int, str]) -> None:
-        '''Disables all children of a dpg item.
-
-        Parameters:
-            item (Union[int, str]): The tag of the dpg item.
-        '''
         slots = dpg.get_item_children(item)
         for slot in slots.values():
             for child in slot:
                 if dpg.get_item_info(child).get('type') == 'mvAppItemType::mvGroup':
                     self.disable_children(child)
                 else:
                     dpg.disable_item(child)
 
     def enable_children(self, item: Union[int, str]) -> None:
-        '''Enables all children of a dpg item.
-
-        Parameters:
-            item (Union[int, str]): The tag of the dpg item.
-        '''
         slots = dpg.get_item_children(item)
         for slot in slots.values():
             for child in slot:
                 if dpg.get_item_info(child).get('type') == 'mvAppItemType::mvGroup':
                     self.enable_children(child)
                 else:
                     dpg.enable_item(child)
 
     def auto_scroll(self, value: bool) -> None:
-        '''Sets if the log window should automatically scroll down for new messages.
-
-        Parameters:
-            value (bool): True if auto scrolling is on.
-        '''
         self._auto_scroll = value
 
     def _log(self, message: str, level: int) -> None:
-        '''Logs the message in the logger window.
 
-        Parameters:
-            message (str): The message to dispaly.
-            level (int): The log level of the message.
-        '''
+        if level < self.log_level:
+            return
 
-        if self.log_count > 1000:
+        if self.log_count > self.log_flush_count:
             self.clear_log()
 
         theme = None
         # For log-level 0 the messages are processed per character
         # For all other levels the message is processed per line
         if level == 0:
             if not self.log_last_line:
@@ -266,111 +202,77 @@
             if theme:
                 dpg.bind_item_theme(new_log, theme)
 
         if self._auto_scroll:
             dpg.set_y_scroll(self.child_id, -1.0)
 
     def log(self, character: str) -> None:
-        '''Logs the character in the logger window.
-
-        Parameters:
-            character (str): The character to display.
-        '''
         self._log(character, 0)
 
     def log_debug(self, message: str) -> None:
-        '''Logs the message in the logger window in DEBUG style.
-
-        Parameters:
-            message (str): The message to display.
-        '''
         self._log(message, 1)
 
     def log_info(self, message: str) -> None:
-        '''Logs the message in the logger window in INFO style.
-
-        Parameters:
-            message (str): The message to display.
-        '''
         self._log(message, 2)
 
     def log_warning(self, message: str) -> None:
-        '''Logs the message in the logger window in WARNING style.
-
-        Parameters:
-            message (str): The message to display.
-        '''
         self._log(message, 3)
 
     def log_error(self, message: str) -> None:
-        '''Logs the message in the logger window in ERROR style.
-
-        Parameters:
-            message (str): The message to display.
-        '''
         self._log(message, 4)
 
     def clear_log(self) -> None:
-        '''Clears the logger window of a ll messages.'''
         dpg.delete_item(self.filter_id, children_only=True)
         self.log_count = 0
 
     def load_start(self) -> None:
-        '''Shows a loading indicator.'''
         dpg.add_loading_indicator(tag=LOADING_INDICATOR_TAG, parent=self.filter_id)
         if self._auto_scroll:
             dpg.set_y_scroll(self.child_id, -1.0)
 
     def load_end(self) -> None:
-        '''Removes the loading indicator.'''
         dpg.delete_item(LOADING_INDICATOR_TAG)
 
     def on_debug_run(self) -> None:
-        '''Starts the debugger and runs the program.'''
-        if self.flowchart:
-            if not self.debug_session:
-                # Start debugger
-                if self.flowchart.lang_data['debugger'] == 'pdb':
-                    self.debug_session = FtdbSession(self)
-                else:
-                    self.debug_session = GdbSession(self)
-                self.debug_session.run(self.flowchart)
-            else:
-                self.debug_session.cont(self.flowchart)
+        if not self.debug_session:
+            # Start debugger
+            self.debug_session = DebugSession(self)
+            self.debug_session.run()
+        else:
+            self.debug_session.cont()
 
     def on_build(self) -> None:
-        '''Compiles the C program using GCC.'''
         self.disable_all()
         self.load_start()
 
         try:
             gcc_exe = self.utils.get_gcc_exe()
         except FileNotFoundError as error:
             self.log_error(str(error))
             self.load_end()
             return
 
-        print(gcc_exe, file=stderr)
+        print(gcc_exe, file=sys.stderr)
 
         # Build the executable
-        result = run([
+        result = subprocess.run([
             gcc_exe,
-            self.utils.get_source_path('.c'),
+            self.utils.get_c_source_path(),
             '-g',
             '-o',
             self.utils.get_exe_path(),
             '-lm'],
             capture_output=True)
 
         output = '\n'.join(filter(lambda s: s, [result.stdout.decode('utf-8'), result.stderr.decode('utf-8')]))
         output_lines = output.split('\n')
 
         log = self.log_info
         for line in output_lines:
-            output_line = sub(r'.*?:(\d+:\d+:)?', '', line, count=1)
+            output_line = re.sub(r'.*?:(\d+:\d+:)?', '', line, count=1)
             stripped = output_line.lstrip()
             if stripped.startswith('warning'):
                 log = self.log_warning
             elif stripped.startswith('error'):
                 log = self.log_error
             elif stripped.startswith('note'):
                 log = self.log_info
@@ -381,44 +283,37 @@
             self.is_code_built = True
             self.log_info('Code built!')
             self.enable_build_and_run()
 
         self.load_end()
 
     def on_debug_step_over(self) -> None:
-        '''Excecute a single step of the program, stepping over functions.'''
-        if not self.debug_session or not self.flowchart:
+        if not self.debug_session:
             return
-        self.debug_session.next(self.flowchart)
+        self.debug_session.next()
 
     def on_debug_step_into(self) -> None:
-        '''Excecute a single step of the program, stepping into functions.'''
-        if not self.debug_session or not self.flowchart:
+        if not self.debug_session:
             return
-        self.debug_session.step(self.flowchart)
+        self.debug_session.step()
 
     def on_debug_stop(self) -> None:
-        '''Stop execution of the program.'''
         if not self.debug_session:
             return
         self.debug_session.stop()
 
     def on_program_finished(self, _: Any, **kw: Any) -> None:
-        '''Log a message after program has finished'''
-        sleep(0.3)
+        sleep(1.0)
         self.log_info('Program ended.')
         self.debug_session = None
 
     def on_program_error(self, _: Any, **kw: str) -> None:
-        '''Log a message on program errors.'''
         error = kw['error']
         self.log_error(error)
 
     def on_program_killed(self, _: Any, **kw: Any) -> None:
-        '''Log a message if the program gets killed.'''
         self.log_info('Program killed.')
         self.debug_session = None
 
     def on_recieve_output(self, _: Any, **kw: str) -> None:
-        '''Log outputs to the logger window.'''
         output = kw['output']
         self.log(output)
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/section_node_extras.py` & `FlowTutor-0.9.0/src/flowtutor/gui/section_node_extras.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,51 +5,36 @@
 from flowtutor.flowchart.node import Node
 
 if TYPE_CHECKING:
     from flowtutor.gui.gui import GUI
 
 
 class SectionNodeExtras:
-    '''A GUI section for additional node options.'''
-
     def __init__(self, gui: GUI) -> None:
         self.gui = gui
         with dpg.group(show=False) as self.main_group:
             dpg.add_spacer(height=5)
             dpg.add_separator()
 
             with dpg.group():
                 dpg.add_text('Comment')
                 self.node_comment = dpg.add_input_text(
                     width=-1,
                     callback=lambda _, data: (self.gui.selected_node.__setattr__('comment', data),
-                                              self.gui.selected_node.__setattr__('needs_refresh', True),
                                               self.gui.redraw_all()))
-
-            dpg.add_spacer(height=3)
-            dpg.add_separator()
-            dpg.add_spacer(height=3)
-
-            with dpg.group(horizontal=True):
+            with dpg.group():
                 dpg.add_text('Break Point')
                 self.node_break_point = dpg.add_checkbox(
                     callback=lambda _, data: (self.gui.selected_node.__setattr__('break_point', data),
-                                              self.gui.selected_node.__setattr__('needs_refresh', True),
                                               self.gui.redraw_all()))
-
-            dpg.add_spacer(height=3)
-            dpg.add_separator()
-            dpg.add_spacer(height=3)
-
-            with dpg.group(horizontal=True) as self.node_is_comment_group:
+            with dpg.group() as self.node_is_comment_group:
                 dpg.add_text('Disabled')
                 self.node_is_comment = dpg.add_checkbox(
                     callback=lambda _, data: (self.gui.selected_node.__setattr__('is_comment', data),
-                                              self.gui.selected_node.__setattr__('needs_refresh', True),
-                                              self.gui.redraw_all(True)))
+                                              self.gui.redraw_all()))
 
     def toggle(self, node: Optional[Node]) -> None:
         self.show(node) if node else self.hide()
 
     def hide(self) -> None:
         dpg.hide_item(self.main_group)
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/section_structs.py` & `FlowTutor-0.9.0/src/flowtutor/gui/section_structs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union
 import dearpygui.dearpygui as dpg
-from dependency_injector.wiring import Provide, inject
+from flowtutor.flowchart.flowchart import Flowchart
 from flowtutor.flowchart.struct_definition import StructDefinition
 from flowtutor.flowchart.struct_member import StructMember
+from flowtutor.language import Language
 
 if TYPE_CHECKING:
     from flowtutor.gui.gui import GUI
-    from flowtutor.language_service import LanguageService
-    from flowtutor.flowchart.flowchart import Flowchart
 
 
 class SectionStructs:
-    '''A GUI section for struct definitions.'''
-
-    @inject
-    def __init__(self, gui: GUI, language_service: LanguageService = Provide['language_service']) -> None:
+    def __init__(self, gui: GUI) -> None:
         self.gui = gui
-        self.language_service = language_service
         with dpg.theme() as self.delete_button_theme:
             with dpg.theme_component(dpg.mvImageButton):
                 dpg.add_theme_style(dpg.mvStyleVar_FramePadding, 3, 3, category=dpg.mvThemeCat_Core)
         self.main_header = dpg.add_collapsing_header(label='Structures')
         self.refresh()
 
     def refresh(self) -> None:
@@ -36,15 +31,15 @@
                                    width=-33,
                                    no_spaces=True,
                                    default_value=d.name,
                                    user_data=i,
                                    callback=lambda s, data: (
                                        self.struct_definitions()[dpg.get_item_user_data(
                                            s)].__setattr__('name', data),
-                                       self.gui.redraw_all(True)))
+                                       self.gui.redraw_all()))
                 delete_button = dpg.add_image_button(
                     'trash_image', height=18, width=18, user_data=i,
                     callback=lambda s: self.on_delete_definition(dpg.get_item_user_data(s)))
                 dpg.bind_item_theme(delete_button, self.delete_button_theme)
             with dpg.group(parent=self.main_header):
                 with dpg.table(header_row=True, sortable=False, hideable=False, reorderable=False,
                                borders_innerH=True, borders_outerH=True, borders_innerV=True,
@@ -75,20 +70,20 @@
             dpg.add_separator(parent=self.main_header)
         dpg.add_spacer(height=5, parent=self.main_header)
         dpg.add_button(label='Add Structure', parent=self.main_header, width=-1, callback=self.on_add_definition)
 
     def on_add_definition(self) -> None:
         self.struct_definitions().append(StructDefinition())
         self.refresh()
-        self.gui.redraw_all(True)
+        self.gui.redraw_all()
 
     def on_delete_definition(self, index: int) -> None:
         del self.struct_definitions()[index]
         self.refresh()
-        self.gui.redraw_all(True)
+        self.gui.redraw_all()
 
     def main_node(self) -> Flowchart:
         return self.gui.flowcharts['main']
 
     def struct_definitions(self) -> list[StructDefinition]:
         return self.main_node().struct_definitions
 
@@ -123,59 +118,59 @@
 
         for j, member in enumerate(members):
             with dpg.table_row(parent=table):
                 dpg.add_input_text(width=-1,
                                    user_data=(i, j),
                                    callback=lambda s, data: (self.member(dpg.get_item_user_data(s))
                                                              .__setattr__('name', data),
-                                                             self.gui.redraw_all(True)),
+                                                             self.gui.redraw_all()),
                                    no_spaces=True, default_value=member.name)
 
-                dpg.add_combo(self.language_service.get_data_types(self.gui.flowcharts['main']),
+                dpg.add_combo(Language.get_data_types(self.gui.flowcharts['main']),
                               width=-1,
                               user_data=(i, j),
                               callback=lambda s, data: (self.member(dpg.get_item_user_data(s))
                                                         .__setattr__('type', data),
-                                                        self.gui.redraw_all(True)),
+                                                        self.gui.redraw_all()),
                               default_value=member.type)
 
                 dpg.add_checkbox(user_data=(i, j),
                                  tag=f'struct_member_is_pointer_{i}_{j}',
                                  callback=lambda s, data: (self.member(dpg.get_item_user_data(s))
                                                            .__setattr__('is_pointer', data),
                                                            self.toggle_is_pointer(s),
-                                                           self.gui.redraw_all(True)),
+                                                           self.gui.redraw_all()),
                                  default_value=member.is_pointer)
 
                 dpg.add_checkbox(user_data=(i, j),
                                  tag=f'struct_member_is_array_{i}_{j}',
                                  callback=lambda s, data: (self.member(dpg.get_item_user_data(s))
                                                            .__setattr__('is_array', data),
                                                            self.toggle_is_array(data, s),
-                                                           self.gui.redraw_all(True)),
+                                                           self.gui.redraw_all()),
                                  default_value=member.is_array)
 
                 dpg.add_input_text(user_data=(i, j),
                                    tag=f'struct_member_array_size_{i}_{j}',
                                    width=-1,
                                    callback=lambda s, data: (self.member(dpg.get_item_user_data(s))
                                                              .__setattr__('array_size', data),
-                                                             self.gui.redraw_all(True)),
+                                                             self.gui.redraw_all()),
                                    default_value=member.array_size,
                                    show=member.is_array)
 
                 delete_button = dpg.add_image_button(
                     'trash_image',
                     user_data=(i, j),
                     callback=lambda s: (
                         self.members(dpg.get_item_user_data(s)[0]).pop(dpg.get_item_user_data(s)[1]),
                         self.refresh_members(
                             dpg.get_item_user_data(s)[0],
                             table,
                             self.members(dpg.get_item_user_data(s)[0])),
-                        self.gui.redraw_all(True)))
+                        self.gui.redraw_all()))
 
                 with dpg.theme() as delete_button_theme:
                     with dpg.theme_component(dpg.mvImageButton):
                         dpg.add_theme_style(dpg.mvStyleVar_FramePadding, 5, 4, category=dpg.mvThemeCat_Core)
 
                 dpg.bind_item_theme(delete_button, delete_button_theme)
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/section_typedefs.py` & `FlowTutor-0.9.0/src/flowtutor/gui/section_typedefs.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from flowtutor.flowchart.type_definition import TypeDefinition
 
 if TYPE_CHECKING:
     from flowtutor.gui.gui import GUI
 
 
 class SectionTypedefs:
-    '''A GUI section for type definitions.'''
-
     def __init__(self, gui: GUI) -> None:
         self.gui = gui
         with dpg.theme() as self.delete_button_theme:
             with dpg.theme_component(dpg.mvImageButton):
                 dpg.add_theme_style(dpg.mvStyleVar_FramePadding, 3, 3, category=dpg.mvThemeCat_Core)
         self.main_header = dpg.add_collapsing_header(label='Type Definitions')
         self.refresh()
@@ -31,43 +29,43 @@
                                    width=-33,
                                    no_spaces=True,
                                    default_value=d.name,
                                    user_data=i,
                                    callback=lambda s, data: (
                                        self.type_definitions()[dpg.get_item_user_data(
                                            s)].__setattr__('name', data),
-                                       self.gui.redraw_all(True)))
+                                       self.gui.redraw_all()))
                 delete_button = dpg.add_image_button(
                     'trash_image', height=18, width=18, user_data=i,
                     callback=lambda s: self.on_delete_definition(dpg.get_item_user_data(s)))
                 dpg.bind_item_theme(delete_button, self.delete_button_theme)
             with dpg.group(horizontal=True, parent=self.main_header):
                 dpg.add_text('Definition')
                 dpg.add_input_text(indent=100,
                                    width=-1,
                                    default_value=d.name,
                                    user_data=i,
                                    callback=lambda s, data: (
                                        self.type_definitions()[dpg.get_item_user_data(
                                            s)].__setattr__('definition', data),
-                                       self.gui.redraw_all(True)))
+                                       self.gui.redraw_all()))
 
             dpg.add_spacer(height=5, parent=self.main_header)
             dpg.add_separator(parent=self.main_header)
         dpg.add_spacer(height=5, parent=self.main_header)
         dpg.add_button(label='Add Type Definition', parent=self.main_header, width=-1, callback=self.on_add_definition)
 
     def on_add_definition(self) -> None:
         self.type_definitions().append(TypeDefinition())
         self.refresh()
-        self.gui.redraw_all(True)
+        self.gui.redraw_all()
 
     def on_delete_definition(self, index: int) -> None:
         del self.type_definitions()[index]
         self.refresh()
-        self.gui.redraw_all(True)
+        self.gui.redraw_all()
 
     def main_node(self) -> Flowchart:
         return self.gui.flowcharts['main']
 
     def type_definitions(self) -> list[TypeDefinition]:
         return self.main_node().type_definitions
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/sidebar_functionend.py` & `FlowTutor-0.9.0/src/flowtutor/gui/sidebar_functionend.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,26 +7,24 @@
 from flowtutor.gui.sidebar import Sidebar
 
 if TYPE_CHECKING:
     from flowtutor.gui.gui import GUI
 
 
 class SidebarFunctionEnd(Sidebar):
-    '''A GUI sidebar for FunctionEnd nodes.'''
 
     def __init__(self, gui: GUI) -> None:
         self.gui = gui
         with dpg.group(tag='selected_function_end', show=False) as self.main_group:
             with dpg.group():
                 dpg.add_text('Return Value')
                 dpg.add_input_text(tag='selected_function_return_value',
                                    width=-1,
                                    callback=lambda _, data: (
                                        gui.selected_node.__setattr__('return_value', data),
-                                       self.gui.selected_node.__setattr__('needs_refresh', True),
                                        gui.redraw_all()))
 
     def hide(self) -> None:
         dpg.hide_item(self.main_group)
 
     def show(self, node: Optional[Node]) -> None:
         if not isinstance(node, FunctionEnd):
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/sidebar_functionstart.py` & `FlowTutor-0.9.0/src/flowtutor/gui/sidebar_functionstart.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,75 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
 import dearpygui.dearpygui as dpg
 from dependency_injector.wiring import Provide, inject
 
+from flowtutor.flowchart.functionstart import FunctionStart
+from flowtutor.flowchart.node import Node
 from flowtutor.flowchart.parameter import Parameter
 from flowtutor.gui.sidebar import Sidebar
-from flowtutor.flowchart.functionstart import FunctionStart
+from flowtutor.language import Language
+from flowtutor.modal_service import ModalService
 
 if TYPE_CHECKING:
     from flowtutor.gui.gui import GUI
-    from flowtutor.language_service import LanguageService
-    from flowtutor.modal_service import ModalService
-    from flowtutor.flowchart.node import Node
 
 
 class SidebarFunctionStart(Sidebar):
-    '''A GUI sidebar for FunctionStart nodes.'''
 
     @inject
-    def __init__(self,
-                 gui: GUI,
-                 modal_service: ModalService = Provide['modal_service'],
-                 language_service: LanguageService = Provide['language_service']) -> None:
+    def __init__(self, gui: GUI, modal_service: ModalService = Provide['modal_service']) -> None:
         self.gui = gui
         self.modal_service = modal_service
-        self.language_service = language_service
         with dpg.group(show=False) as self.main_group:
             dpg.configure_item(gui.rename_button, callback=self.on_rename)
             dpg.configure_item(gui.delete_button, callback=self.on_delete)
 
             with dpg.group(tag='selected_function_parameters_group', show=False):
                 dpg.add_text('Parameters')
                 with dpg.table(header_row=True, sortable=False, hideable=False, reorderable=False,
                                borders_innerH=True, borders_outerH=True, borders_innerV=True,
                                borders_outerV=True) as self.table:
 
-                    self.name_column = dpg.add_table_column(label='Name')
-                    self.type_column = dpg.add_table_column(label='Type')
+                    dpg.add_table_column(label='Name')
+                    dpg.add_table_column(label='Type')
                     dpg.add_table_column(label='', width_fixed=True, width=12)
 
                     self.refresh_entries([])
 
                     with dpg.theme() as item_theme:
                         with dpg.theme_component(dpg.mvTable):
                             dpg.add_theme_style(dpg.mvStyleVar_CellPadding, 0, 1, category=dpg.mvThemeCat_Core)
                     dpg.bind_item_theme(self.table, item_theme)
 
                 dpg.add_button(label='Add Parameter',
                                callback=lambda: (gui.selected_node.__getattribute__('parameters')
                                                  .append(Parameter()),
                                                  self.refresh_entries(
                                    gui.selected_node.__getattribute__('parameters')),
-                                   self.gui.selected_node.__setattr__('needs_refresh', True),
                                    gui.redraw_all()))
 
                 dpg.add_spacer(height=5)
                 dpg.add_separator()
 
             with dpg.group(tag='selected_function_return_type_group'):
                 dpg.add_text('Return Type')
-                dpg.add_combo(language_service.get_data_types(self.gui.flowcharts['main']),
+                dpg.add_combo(Language.get_data_types(self.gui.flowcharts['main']),
                               tag='selected_function_return_type',
                               width=-1,
                               callback=lambda _, data: (gui.selected_node.__setattr__('return_type', data),
-                                                        self.gui.selected_node.__setattr__('needs_refresh', True),
                                                         gui.redraw_all()))
 
     def parameters(self) -> list[Parameter]:
         result: list[Parameter] = self.gui.selected_node.__getattribute__('parameters')
         return result
 
     def on_delete(self) -> None:
         if isinstance(self.gui.selected_node, FunctionStart):
             del self.gui.flowcharts[self.gui.selected_node.name]
-            self.gui.selected_flowchart_name = next(iter(self.gui.flowcharts))
             self.gui.refresh_function_tabs()
 
     def on_rename(self) -> None:
         if isinstance(self.gui.selected_node, FunctionStart):
             self.modal_service.show_input_text_modal(
                 'Rename', 'Function Name', self.gui.selected_node.name, self.rename)
 
@@ -90,43 +82,34 @@
             self.gui.refresh_function_tabs()
 
     def refresh_entries(self, entries: list[Parameter]) -> None:
         # delete existing rows in the table to avoid duplicates
         for child in dpg.get_item_children(self.table)[1]:
             dpg.delete_item(child)
 
-        # The types column gets removed, if the language has no types.
-        # It gets readded, if it had been removed before and the language has types.
-        has_types = self.language_service.has_types(self.gui.selected_flowchart)
-        if has_types and not dpg.does_item_exist(self.type_column):
-            self.type_column = dpg.add_table_column(label='Type', parent=self.table, before=self.name_column)
-        elif dpg.does_item_exist(self.type_column):
-            dpg.delete_item(self.type_column)
-
         for i, entry in enumerate(entries):
             with dpg.table_row(parent=self.table):
                 dpg.add_input_text(width=-1,
                                    height=-1,
                                    user_data=i,
                                    callback=lambda s, data: (self.parameters()[dpg.get_item_user_data(s)]
                                                              .__setattr__('name', data),
-                                                             self.gui.redraw_all(True)),
+                                                             self.gui.redraw_all()),
                                    no_spaces=True, default_value=entry.name)
-                if has_types:
-                    dpg.add_combo(self.language_service.get_data_types(self.gui.flowcharts['main']),
-                                  user_data=i,
-                                  callback=lambda s, data: (self.parameters()[dpg.get_item_user_data(s)]
-                                                            .__setattr__('type', data),
-                                                            self.gui.redraw_all(True)),
-                                  width=-1, default_value=entry.type)
+                dpg.add_combo(Language.get_data_types(self.gui.flowcharts['main']),
+                              user_data=i,
+                              callback=lambda s, data: (self.parameters()[dpg.get_item_user_data(s)]
+                                                        .__setattr__('type', data),
+                                                        self.gui.redraw_all()),
+                              width=-1, default_value=entry.type)
 
                 delete_button = dpg.add_image_button('trash_image', user_data=i, callback=lambda s: (
                     self.parameters().pop(dpg.get_item_user_data(s)),
                     self.refresh_entries(self.parameters()),
-                    self.gui.redraw_all(True)
+                    self.gui.redraw_all()
                 ))
                 with dpg.theme() as delete_button_theme:
                     with dpg.theme_component(dpg.mvImageButton):
                         dpg.add_theme_style(dpg.mvStyleVar_FramePadding, 5, 4, category=dpg.mvThemeCat_Core)
 
                 dpg.bind_item_theme(delete_button, delete_button_theme)
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/sidebar_none.py` & `FlowTutor-0.9.0/src/flowtutor/gui/sidebar_none.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional, Union
 import dearpygui.dearpygui as dpg
-from dependency_injector.wiring import Provide, inject
-
+from flowtutor.flowchart.node import Node
 from flowtutor.gui.sidebar import Sidebar
 
+from flowtutor.language import Language
+
 if TYPE_CHECKING:
     from flowtutor.flowchart.flowchart import Flowchart
     from flowtutor.gui.gui import GUI
-    from flowtutor.language_service import LanguageService
-    from flowtutor.flowchart.node import Node
 
 
 class SidebarNone(Sidebar):
-    '''A GUI sidebar for no selected nodes.'''
 
-    @inject
-    def __init__(self, gui: GUI, language_service: LanguageService = Provide['language_service']) -> None:
+    def __init__(self, gui: GUI) -> None:
         self.gui = gui
-        self.language_service = language_service
         with dpg.group() as self.main_group:
-            dpg.add_text('File head')
-            with dpg.collapsing_header(label='Import') as self.import_header:
-                pass
-            with dpg.collapsing_header(label='Define') as self.define_header:
+            dpg.add_text('Preprocessor')
+            with dpg.collapsing_header(label='Include', tag='selected_includes'):
+                for header in Language.get_standard_headers():
+                    dpg.add_checkbox(
+                        label=header,
+                        default_value=header in self.includes(),
+                        user_data=header,
+                        callback=self.on_header_checkbox_change)
+            with dpg.collapsing_header(label='Define'):
                 with dpg.table(sortable=False, hideable=False, reorderable=False,
                                borders_innerH=True, borders_outerH=True, borders_innerV=True,
                                borders_outerV=True) as self.table:
 
                     dpg.add_table_column()
                     dpg.add_table_column(width_fixed=True, width=12)
 
@@ -38,101 +39,80 @@
                             dpg.add_theme_style(dpg.mvStyleVar_CellPadding, 0, 1, category=dpg.mvThemeCat_Core)
                     dpg.bind_item_theme(self.table, item_theme)
 
                 dpg.add_button(label='Add Definition',
                                callback=lambda: (self.preprocessor_definitions().append(''),
                                                  self.refresh_definitions(
                                    self.preprocessor_definitions()),
-                                   gui.redraw_all(True)))
+                                   gui.redraw_all()))
+
             with dpg.collapsing_header(label='Custom'):
                 dpg.add_input_text(tag='selected_preprocessor_custom',
                                    width=-1,
                                    height=-46,
                                    multiline=True,
                                    callback=lambda _, data:
                                    (self.main_node().__setattr__('preprocessor_custom', data),
-                                    gui.redraw_all(True)))
+                                    gui.redraw_all()))
             dpg.add_spacer(height=3)
             dpg.add_separator()
             dpg.add_spacer(height=3)
-            self.types_button = dpg.add_button(label='Types', width=-1,
-                                               callback=lambda: (dpg.show_item('type_window'),
-                                                                 gui.redraw_all(True)))
+            dpg.add_button(label='Types', width=-1,
+                           callback=lambda: (dpg.show_item('type_window'), gui.redraw_all()))
 
     def main_node(self) -> Flowchart:
         return self.gui.flowcharts['main']
 
-    def imports(self) -> list[str]:
-        result: list[str] = self.main_node().__getattribute__('imports')
+    def includes(self) -> list[str]:
+        result: list[str] = self.main_node().__getattribute__('includes')
         return result
 
     def preprocessor_definitions(self) -> list[str]:
         result: list[str] = self.main_node().__getattribute__('preprocessor_definitions')
         return result
 
     def on_header_checkbox_change(self, sender: Union[int, str], is_checked: bool) -> None:
         header = dpg.get_item_user_data(sender)
         if is_checked:
-            self.imports().append(header)
+            self.includes().append(header)
         else:
-            self.imports().remove(header)
-        self.gui.redraw_all(True)
+            self.includes().remove(header)
+        self.gui.redraw_all()
 
     def refresh_definitions(self, entries: list[str]) -> None:
         # delete existing rows in the table to avoid duplicates
         for child in dpg.get_item_children(self.table)[1]:
             dpg.delete_item(child)
 
         for i, entry in enumerate(entries):
             with dpg.table_row(parent=self.table):
                 dpg.add_input_text(width=-1, height=-1, user_data=i,
                                    callback=lambda s, data: (self.preprocessor_definitions()
                                                              .__setitem__(dpg.get_item_user_data(s), data),
-                                                             self.gui.redraw_all(True)),
+                                                             self.gui.redraw_all()),
                                    default_value=entry)
 
                 delete_button = dpg.add_image_button('trash_image', user_data=i, callback=lambda s: (
                     self.preprocessor_definitions().pop(dpg.get_item_user_data(s)),
                     self.refresh_definitions(self.preprocessor_definitions()),
-                    self.gui.redraw_all(True)
+                    self.gui.redraw_all()
                 ))
                 with dpg.theme() as delete_button_theme:
                     with dpg.theme_component(dpg.mvImageButton):
                         dpg.add_theme_style(dpg.mvStyleVar_FramePadding, 5, 4, category=dpg.mvThemeCat_Core)
 
                 dpg.bind_item_theme(delete_button, delete_button_theme)
 
     def refresh(self) -> None:
-        if self.gui.selected_flowchart.lang_data['lang_id'] == 'c':
-            dpg.show_item(self.types_button)
-            dpg.show_item(self.define_header)
-        else:
-            dpg.hide_item(self.types_button)
-            dpg.hide_item(self.define_header)
-        if 'import' in self.gui.selected_flowchart.lang_data and\
-           'standard_imports' in self.gui.selected_flowchart.lang_data:
-            dpg.show_item(self.import_header)
-        else:
-            dpg.hide_item(self.import_header)
         self.refresh_definitions(self.preprocessor_definitions())
         dpg.configure_item(
             'selected_preprocessor_custom',
             default_value=self.main_node().__getattribute__('preprocessor_custom'))
-        # delete existing entries to avoid duplicates
-        for child in dpg.get_item_children(self.import_header)[1]:
-            dpg.delete_item(child)
-        for header in self.language_service.get_standard_headers(self.gui.selected_flowchart):
-            dpg.add_checkbox(
-                parent=self.import_header,
-                label=header,
-                default_value=header in self.imports(),
-                user_data=header,
-                callback=self.on_header_checkbox_change)
-        for checkbox in dpg.get_item_children(self.import_header)[1]:
-            dpg.configure_item(checkbox, default_value=dpg.get_item_user_data(checkbox) in self.imports())
+        for checkbox in dpg.get_item_children('selected_includes')[1]:
+            dpg.configure_item(checkbox, default_value=dpg.get_item_user_data(checkbox) in self.includes())
 
     def hide(self) -> None:
         dpg.hide_item(self.main_group)
 
     def show(self, node: Optional[Node]) -> None:
         self.gui.set_sidebar_title('Program')
         dpg.show_item(self.main_group)
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/gui/window_types.py` & `FlowTutor-0.9.0/src/flowtutor/gui/window_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from flowtutor.gui.section_typedefs import SectionTypedefs
 
 if TYPE_CHECKING:
     from flowtutor.gui.gui import GUI
 
 
 class WindowTypes:
-    '''A GUI windo for type and struct definitions.'''
 
     def __init__(self, gui: GUI) -> None:
         with dpg.window(tag='type_window',
                         label='Types',
                         pos=(300, 75),
                         width=600,
                         height=500,
```

### Comparing `FlowTutor-0.10.9/src/flowtutor/main.py` & `FlowTutor-0.9.0/src/flowtutor/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,42 @@
 from __future__ import annotations
-from dependency_injector.wiring import Provide, inject
-from platform import system
-from typing import TYPE_CHECKING
+import platform
 import dearpygui.dearpygui as dpg
+from dependency_injector.wiring import Provide, inject
 
 from flowtutor.containers import Container
 from flowtutor.gui.gui import GUI
-
-if TYPE_CHECKING:
-    from flowtutor.util_service import UtilService
+from flowtutor.util_service import UtilService
 
 
 @inject
 def start(utils_service: UtilService = Provide['utils_service']) -> None:
-    if system() != 'Windows':
+    if platform.system() != 'Windows':
         utils_service.open_tty()
     gui = GUI(2000, 2000)
-
     # Calls the redraw function after the first frame is rendered
     if dpg.is_dearpygui_running():
         dpg.render_dearpygui_frame()
-        gui.redraw_all(True)
-
-    # Shows the welcome modal after the second frame
-    if dpg.is_dearpygui_running():
-        dpg.render_dearpygui_frame()
-        gui.modal_service.show_welcome_modal(gui)
-
+        gui.redraw_all()
     dpg.start_dearpygui()
-    if system() != 'Windows':
+    if platform.system() != 'Windows':
         utils_service.stop_tty()
     dpg.destroy_context()
     utils_service.cleanup_temp()
 
 
 def main() -> None:
     container = Container()
     container.init_resources()
     container.wire(modules=[__name__,
                             'flowtutor.codegenerator',
-                            'flowtutor.debugger.debugsession',
+                            'flowtutor.debugsession',
                             'flowtutor.gui.debugger',
                             'flowtutor.gui.gui',
-                            'flowtutor.gui.menubar_main',
-                            'flowtutor.gui.sidebar_none',
                             'flowtutor.gui.sidebar_functionstart',
-                            'flowtutor.gui.sidebar_template',
-                            'flowtutor.gui.section_structs',
                             'flowtutor.modal_service',
-                            'flowtutor.language_service',
-                            'flowtutor.flowchart.template',
-                            'flowtutor.flowchart.functionstart',
-                            'flowtutor.flowchart.functionend'])
+                            'flowtutor.nodes_service'])
     start()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `FlowTutor-0.10.9/tests/test_flowtutor_codegenerator.py` & `FlowTutor-0.9.0/tests/test_flowtutor_codegenerator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,227 +1,205 @@
-from typing import Any
 from unittest.mock import patch
 import pytest
 
 from flowtutor.codegenerator import CodeGenerator
 from flowtutor.containers import Container
+from flowtutor.flowchart.assignment import Assignment
+from flowtutor.flowchart.conditional import Conditional
+from flowtutor.flowchart.declaration import Declaration
+from flowtutor.flowchart.declarations import Declarations
+from flowtutor.flowchart.dowhileloop import DoWhileLoop
 from flowtutor.flowchart.flowchart import Flowchart
+from flowtutor.flowchart.forloop import ForLoop
 from flowtutor.flowchart.struct_definition import StructDefinition
 from flowtutor.flowchart.struct_member import StructMember
 from flowtutor.flowchart.type_definition import TypeDefinition
+from flowtutor.flowchart.whileloop import WhileLoop
+from flowtutor.flowchart.input import Input
+from flowtutor.flowchart.output import Output
 from flowtutor.flowchart.parameter import Parameter
+from flowtutor.flowchart.snippet import Snippet
 from flowtutor.flowchart.template import Template
 
+from flowtutor.language import Language
 from flowtutor.flowchart.node import dpg as node_dpg
-from flowtutor.language_service import LanguageService
-
-C_TYPES = [
-    'char',
-    'unsigned char',
-    'short',
-    'unsigned short',
-    'int',
-    'unsigned int',
-    'long',
-    'unsigned long',
-    'float',
-    'double',
-    'long double'
-]
-
-C_FORMAT_SPECIFIERS = [
-    [
-        '%c',
-        '%c',
-        '%hd',
-        '%hu',
-        '%d',
-        '%u',
-        '%ld',
-        '%lu',
-        '%f',
-        '%lf',
-        '%Lf'
-    ]
-]
 
 
 @patch.object(node_dpg, 'get_text_size', lambda _: (0, 0))
 class TestCodeGenerator:
 
     @pytest.fixture(scope='session')
     def code_generator(self) -> CodeGenerator:
         container = Container()
         container.init_resources()
-        container.wire(modules=[
-            'flowtutor.codegenerator',
-            'flowtutor.language_service',
-            'flowtutor.flowchart.functionstart',
-            'flowtutor.flowchart.functionend'])
-        code_generator = CodeGenerator()
-        flowchart = Flowchart('main', {
-            'lang_id': 'c'
-        })
-        code_generator.language_service.finish_init(flowchart)
-        return code_generator
-
-    @pytest.fixture(scope='session')
-    def nodes(self) -> dict[str, Any]:
-        container = Container()
-        container.init_resources()
-        container.wire(modules=[
-            'flowtutor.language_service',
-            'flowtutor.flowchart.template',
-            'flowtutor.flowchart.functionstart',
-            'flowtutor.flowchart.functionend'])
-        language_service = LanguageService()
-        flowchart = Flowchart('main', {
-            'lang_id': 'c'
-        })
-        language_service.finish_init(flowchart)
-        return language_service.get_node_templates(flowchart)
-
-    @pytest.fixture()
-    def flowchart(self) -> Flowchart:
-        flowchart = Flowchart('main', {
-            'lang_id': 'c',
-            'import': '#include <{{IMPORT}}>',
-            'function_declaration': '{{RETURN_TYPE}} {{FUN_NAME}}({% for p in PARAMETERS %}{{p.type}} {{p.name}}{{ \",'
-            ' \" if not loop.last else \"\" }}{% endfor %});'
-        })
-        flowchart.imports.append('stdio.h')
-        return flowchart
+        container.wire(modules=['flowtutor.codegenerator'])
+        return CodeGenerator()
 
-    def test_code_from_empty_flowchart(self, flowchart: Flowchart, code_generator: CodeGenerator):
+    def test_code_from_empty_flowchart(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
         code, _ = code_generator.generate_code([flowchart])
         print(code)
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             '  return 0;',
             '}'])
         print(expected)
         assert code == expected, 'An empty flowchart should produce a main function, which returns 0.'
 
-    def test_code_from_imports(self, flowchart: Flowchart, code_generator: CodeGenerator):
-        flowchart.imports.append('test1.h')
-        flowchart.imports.append('test2.h')
+    def test_code_from_includes(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        flowchart.includes.append('test1')
+        flowchart.includes.append('test2')
         code, _ = code_generator.generate_code([flowchart])
         print(code)
         expected = '\n'.join([
             '#include <stdio.h>',
             '#include <test1.h>',
             '#include <test2.h>',
             '',
             'int main() {',
             '  return 0;',
             '}'])
         print(expected)
         assert code == expected, 'Selected headers should be included in the source file.'
 
-    @pytest.mark.parametrize('data_type', C_TYPES)
-    def test_code_from_declaration(self,
-                                   data_type: str,
-                                   flowchart: Flowchart,
-                                   code_generator: CodeGenerator,
-                                   nodes: dict[str, Any]):
-        declaration = Template(nodes['Declaration'])
-        declaration.values['VAR_NAME'] = 'x'
-        declaration.values['VAR_TYPE'] = data_type
-        declaration.values['VAR_VALUE'] = '3'
+    @pytest.mark.parametrize('data_type', Language.get_data_types())
+    def test_code_from_declaration(self, data_type, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        declaration = Declaration()
+        declaration.var_name = 'x'
+        declaration.var_type = data_type
+        declaration.var_value = '3'
         flowchart.add_node(flowchart.root, declaration)
         code, _ = code_generator.generate_code([flowchart])
-        print('---------------------OUTPUT:---------------------------------')
         print(code)
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             f'  {data_type} x = 3;',
             '  return 0;',
             '}'])
-        print('---------------------EXPECTED:-------------------------------')
         print(expected)
         assert code == expected, 'Declaration with value.'
 
-    @pytest.mark.parametrize('data_type', C_TYPES)
-    def test_code_from_static_declaration(self,
-                                          data_type: str,
-                                          flowchart: Flowchart,
-                                          code_generator: CodeGenerator,
-                                          nodes: dict[str, Any]):
-        declaration = Template(nodes['Declaration'])
-        declaration.values['VAR_NAME'] = 'x'
-        declaration.values['IS_STATIC'] = True
-        declaration.values['VAR_TYPE'] = data_type
-        declaration.values['VAR_VALUE'] = '3'
+    @pytest.mark.parametrize('data_type', Language.get_data_types())
+    def test_code_from_static_declaration(self, data_type, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        declaration = Declaration()
+        declaration.var_name = 'x'
+        declaration.is_static = True
+        declaration.var_type = data_type
+        declaration.var_value = '3'
         flowchart.add_node(flowchart.root, declaration)
         code, _ = code_generator.generate_code([flowchart])
         print(code)
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             f'  static {data_type} x = 3;',
             '  return 0;',
             '}'])
         print(expected)
         assert code == expected, 'Static declaration with initialization.'
 
-    @pytest.mark.parametrize('data_type', C_TYPES)
-    def test_code_from_pointer_declaration(self,
-                                           data_type: str,
-                                           flowchart: Flowchart,
-                                           code_generator: CodeGenerator,
-                                           nodes: dict[str, Any]):
-        declaration = Template(nodes['Declaration'])
-        declaration.values['VAR_NAME'] = 'x'
-        declaration.values['IS_POINTER'] = True
-        declaration.values['VAR_TYPE'] = data_type
+    @pytest.mark.parametrize('data_type', Language.get_data_types())
+    def test_code_from_pointer_declaration(self, data_type, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        declaration = Declaration()
+        declaration.var_name = 'x'
+        declaration.var_type = data_type
+        declaration.is_pointer = True
         flowchart.add_node(flowchart.root, declaration)
         code, _ = code_generator.generate_code([flowchart])
         print(code)
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             f'  {data_type} *x;',
             '  return 0;',
             '}'])
         print(expected)
         assert code == expected, 'Pointer declaration.'
 
-    def test_code_from_assignment(self,
-                                  flowchart: Flowchart,
-                                  code_generator: CodeGenerator,
-                                  nodes: dict[str, Any]):
-        assignment = Template(nodes['Assignment'])
-        assignment.values['VAR_NAME'] = 'x'
-        assignment.values['VAR_VALUE'] = '3'
+    @pytest.mark.parametrize('data_type', Language.get_data_types())
+    def test_code_from_declarations(self, data_type, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        declarations = Declarations()
+        declarations.declarations = [
+            {
+                'var_name': 'x',
+                'var_type': data_type,
+                'var_value': '1',
+                'array_size': '',
+                'is_array': False,
+                'is_pointer':  False,
+                'is_static':  False
+            },
+            {
+                'var_name': 'y',
+                'var_type': data_type,
+                'var_value': '2',
+                'array_size': '',
+                'is_array': False,
+                'is_pointer':  False,
+                'is_static':  True
+            },
+            {
+                'var_name': 'z',
+                'var_type': data_type,
+                'var_value': '',
+                'array_size': '',
+                'is_array': False,
+                'is_pointer':  True,
+                'is_static':  False
+            }
+        ]
+        flowchart.add_node(flowchart.root, declarations)
+        code, _ = code_generator.generate_code([flowchart])
+        print(code)
+        expected = '\n'.join([
+            '#include <stdio.h>',
+            '',
+            'int main() {',
+            f'  {data_type} x = 1;',
+            f'  static {data_type} y = 2;',
+            f'  {data_type} *z;',
+            '  return 0;',
+            '}'])
+        print(expected)
+        assert code == expected, 'Multiple Declarations with values.'
+
+    def test_code_from_assignment(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        assignment = Assignment()
+        assignment.var_name = 'x'
+        assignment.var_value = '3'
         flowchart.add_node(flowchart.root, assignment)
         code, _ = code_generator.generate_code([flowchart])
         print(code)
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             '  x = 3;',
             '  return 0;',
             '}'])
         print(expected)
         assert code == expected, 'Assignment.'
 
-    def test_code_from_assignment_with_comment(self,
-                                               flowchart: Flowchart,
-                                               code_generator: CodeGenerator,
-                                               nodes: dict[str, Any]):
-        assignment = Template(nodes['Assignment'])
-        assignment.values['VAR_NAME'] = 'x'
-        assignment.values['VAR_VALUE'] = '3'
+    def test_code_from_assignment_with_comment(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        assignment = Assignment()
+        assignment.var_name = 'x'
+        assignment.var_value = '3'
         assignment.comment = 'This is a comment'
         flowchart.add_node(flowchart.root, assignment)
         code, _ = code_generator.generate_code([flowchart])
         print(code)
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
@@ -229,97 +207,92 @@
             '  // This is a comment',
             '  x = 3;',
             '  return 0;',
             '}'])
         print(expected)
         assert code == expected, 'Assignment.'
 
-    def test_code_from_array_assignment(self,
-                                        flowchart: Flowchart,
-                                        code_generator: CodeGenerator,
-                                        nodes: dict[str, Any]):
-        assignment = Template(nodes['Assignment'])
-        assignment.values['VAR_NAME'] = 'x[0]'
-        assignment.values['VAR_VALUE'] = '3'
+    def test_code_from_array_assignment(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        assignment = Assignment()
+        assignment.var_name = 'x'
+        assignment.var_offset = '0'
+        assignment.var_value = '3'
         flowchart.add_node(flowchart.root, assignment)
         code, _ = code_generator.generate_code([flowchart])
         print(code)
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             '  x[0] = 3;',
             '  return 0;',
             '}'])
         print(expected)
         assert code == expected, 'Assignment.'
 
-    def test_code_from_conditional(self,
-                                   flowchart: Flowchart,
-                                   code_generator: CodeGenerator,
-                                   nodes: dict[str, Any]):
-        conditional = Template(nodes['Conditional'])
-        conditional.values['CONDITION'] = 'x > 5'
+    def test_code_from_conditional(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        conditional = Conditional()
+        conditional.condition = 'x > 5'
         flowchart.add_node(flowchart.root, conditional)
         code, _ = code_generator.generate_code([flowchart])
-        print(code)
+        print(repr(code))
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             '  if(x > 5) {',
             '  }',
             '  return 0;',
             '}'])
-        print(expected)
+        print(repr(expected))
         assert code == expected, 'Conditional.'
 
-    def test_code_from_conditional_with_one_branch(self,
-                                                   flowchart: Flowchart,
-                                                   code_generator: CodeGenerator,
-                                                   nodes: dict[str, Any]):
-        conditional = Template(nodes['Conditional'])
-        conditional.values['CONDITION'] = 'x > 5'
+    def test_code_from_conditional_with_one_branch(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        conditional = Conditional()
+        conditional.condition = 'x > 5'
         flowchart.add_node(flowchart.root, conditional)
 
-        assignment = Template(nodes['Assignment'])
-        assignment.values['VAR_NAME'] = 'x'
-        assignment.values['VAR_VALUE'] = '3'
+        assignment = Assignment()
+        assignment.var_name = 'x'
+        assignment.var_value = '3'
         flowchart.add_node(conditional, assignment, 1)
 
         code, _ = code_generator.generate_code([flowchart])
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             '  if(x > 5) {',
             '    x = 3;',
             '  }',
             '  return 0;',
             '}'])
         print(code)
         print(expected)
+        print(repr(code))
+        print(repr(expected))
         assert code == expected, 'Conditional.'
 
-    def test_code_from_conditional_with_two_branches(self,
-                                                     flowchart: Flowchart,
-                                                     code_generator: CodeGenerator,
-                                                     nodes: dict[str, Any]):
-        conditional = Template(nodes['Conditional'])
-        conditional.values['CONDITION'] = 'x > 5'
+    def test_code_from_conditional_with_two_branches(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        conditional = Conditional()
+        conditional.condition = 'x > 5'
         flowchart.add_node(flowchart.root, conditional)
 
-        assignment1 = Template(nodes['Assignment'])
-        assignment1.values['VAR_NAME'] = 'x'
-        assignment1.values['VAR_VALUE'] = '3'
+        assignment1 = Assignment()
+        assignment1.var_name = 'x'
+        assignment1.var_value = '3'
         flowchart.add_node(conditional, assignment1, 1)
 
-        assignment2 = Template(nodes['Assignment'])
-        assignment2.values['VAR_NAME'] = 'x'
-        assignment2.values['VAR_VALUE'] = '5'
+        assignment2 = Assignment()
+        assignment2.var_name = 'x'
+        assignment2.var_value = '5'
         flowchart.add_node(conditional, assignment2, 0)
 
         code, _ = code_generator.generate_code([flowchart])
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
@@ -328,103 +301,114 @@
             '  } else {',
             '    x = 5;',
             '  }',
             '  return 0;',
             '}'])
         print(code)
         print(expected)
+        print(repr(code))
+        print(repr(expected))
         assert code == expected, 'Conditional.'
 
-    def test_code_from_whileloop(self, flowchart: Flowchart, code_generator: CodeGenerator, nodes: dict[str, Any]):
-        loop = Template(nodes['While loop'])
-        loop.values['CONDITION'] = 'x > 5'
+    def test_code_from_whileloop(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        loop = WhileLoop()
+        loop.condition = 'x > 5'
         flowchart.add_node(flowchart.root, loop)
 
-        assignment = Template(nodes['Assignment'])
-        assignment.values['VAR_NAME'] = 'x'
-        assignment.values['VAR_VALUE'] = '3'
+        assignment = Assignment()
+        assignment.var_name = 'x'
+        assignment.var_value = '3'
         flowchart.add_node(loop, assignment, 1)
 
         code, _ = code_generator.generate_code([flowchart])
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             '  while(x > 5) {',
             '    x = 3;',
             '  }',
             '  return 0;',
             '}'])
         print(code)
         print(expected)
+        print(repr(code))
+        print(repr(expected))
         assert code == expected, 'While-Loop.'
 
-    def test_code_from_do_while_loop(self, flowchart: Flowchart, code_generator: CodeGenerator, nodes: dict[str, Any]):
-        loop = Template(nodes['Do-While loop'])
-        loop.values['CONDITION'] = 'x > 5'
+    def test_code_from_do_while_loop(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        loop = DoWhileLoop()
+        loop.condition = 'x > 5'
         flowchart.add_node(flowchart.root, loop)
 
-        assignment = Template(nodes['Assignment'])
-        assignment.values['VAR_NAME'] = 'x'
-        assignment.values['VAR_VALUE'] = '3'
+        assignment = Assignment()
+        assignment.var_name = 'x'
+        assignment.var_value = '3'
         flowchart.add_node(loop, assignment, 1)
 
         code, _ = code_generator.generate_code([flowchart])
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             '  do {',
             '    x = 3;',
             '  } while(x > 5);',
             '  return 0;',
             '}'])
         print(code)
         print(expected)
+        print(repr(code))
+        print(repr(expected))
         assert code == expected, 'While-Loop.'
+        pass
 
-    def test_code_from_forloop(self, flowchart: Flowchart, code_generator: CodeGenerator, nodes: dict[str, Any]):
-        loop = Template(nodes['For loop'])
-        loop.values['CONDITION'] = 'i < 10'
+    def test_code_from_forloop(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+        loop = ForLoop()
+        loop.var_name = 'i'
+        loop.start_value = '0'
+        loop.condition = 'i < 10'
+        loop.update = 'i++'
         flowchart.add_node(flowchart.root, loop)
 
-        assignment = Template(nodes['Assignment'])
-        assignment.values['VAR_NAME'] = 'x'
-        assignment.values['VAR_VALUE'] = 'x + 3'
+        assignment = Assignment()
+        assignment.var_name = 'x'
+        assignment.var_value = 'x + 3'
         flowchart.add_node(loop, assignment, 1)
 
         code, _ = code_generator.generate_code([flowchart])
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             '  for(int i = 0; i < 10; i++) {',
             '    x = x + 3;',
             '  }',
             '  return 0;',
             '}'])
         print(code)
         print(expected)
+        print(repr(code))
+        print(repr(expected))
         assert code == expected, 'For-Loop.'
 
-    @pytest.mark.parametrize('data_type_format', list(zip(C_TYPES, C_FORMAT_SPECIFIERS)))
-    def test_code_from_input(self,
-                             data_type_format: tuple[str, str],
-                             flowchart: Flowchart,
-                             code_generator: CodeGenerator,
-                             nodes: dict[str, Any]):
+    @pytest.mark.parametrize('data_type_format', list(zip(Language.get_data_types(), Language.get_format_specifiers())))
+    def test_code_from_input(self, data_type_format, code_generator: CodeGenerator):
         data_type, format_specifier = data_type_format
+        flowchart = Flowchart('main')
+
+        declaration = Declaration()
+        declaration.var_name = 'x'
+        declaration.var_type = data_type
 
-        declaration = Template(nodes['Declaration'])
-        declaration.values['VAR_NAME'] = 'x'
-        declaration.values['VAR_TYPE'] = data_type
-
-        input = Template(nodes['Input'])
-        input.values['VAR_NAME'] = 'x'
-        input.values['TEMPLATE_SPECIFIER'] = format_specifier
+        input = Input()
+        input.var_name = 'x'
 
         flowchart.add_node(flowchart.root, declaration)
         flowchart.add_node(declaration, input)
 
         code, _ = code_generator.generate_code([flowchart])
         expected = '\n'.join([
             '#include <stdio.h>',
@@ -432,81 +416,116 @@
             'int main() {',
             f'  {data_type} x;',
             f'  scanf("{format_specifier}", &x);',
             '  return 0;',
             '}'])
         print(code)
         print(expected)
+        print(repr(code))
+        print(repr(expected))
         assert code == expected, 'Input.'
 
-    def test_code_from_output(self, flowchart: Flowchart, code_generator: CodeGenerator, nodes: dict[str, Any]):
-        output = Template(nodes['Output'])
-        output.values['TEMPLATE'] = 'This is the output.'
+    def test_code_from_input_undeclared(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+
+        input = Input()
+        input.var_name = 'x'
+
+        flowchart.add_node(flowchart.root, input)
+
+        code, _ = code_generator.generate_code([flowchart])
+        expected = '\n'.join([
+            '#include <stdio.h>',
+            '',
+            'int main() {',
+            '  // x is not declared!',
+            '  return 0;',
+            '}'])
+        print(code)
+        print(expected)
+        print(repr(code))
+        print(repr(expected))
+        assert code == expected, 'Input undeclared.'
+
+    def test_code_from_output(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+
+        output = Output()
+        output.format_string = 'This is the output.'
 
         flowchart.add_node(flowchart.root, output)
 
         code, _ = code_generator.generate_code([flowchart])
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             '  printf("This is the output.");',
             '  return 0;',
             '}'])
         print(code)
         print(expected)
+        print(repr(code))
+        print(repr(expected))
         assert code == expected, 'Output.'
 
-    def test_code_from_snippet(self, flowchart: Flowchart, code_generator: CodeGenerator, nodes: dict[str, Any]):
-        snippet = Template(nodes['Snippet'])
-        snippet.values['CODE'] = 'printf("Test Code line 1");\nprintf("Test Code line 2");'
+    def test_code_from_snippet(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+
+        snippet = Snippet()
+        snippet.code = 'printf("Test Code line 1");\nprintf("Test Code line 2");'
 
         flowchart.add_node(flowchart.root, snippet)
 
         code, _ = code_generator.generate_code([flowchart])
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             '  printf("Test Code line 1");',
             '  printf("Test Code line 2");',
             '  return 0;',
             '}'])
         print(code)
         print(expected)
+        print(repr(code))
+        print(repr(expected))
         assert code == expected, 'Snippet.'
 
-    def test_code_from_output_with_arguments(self,
-                                             flowchart: Flowchart,
-                                             code_generator: CodeGenerator,
-                                             nodes: dict[str, Any]):
-        output = Template(nodes['Output'])
-        output.values['TEMPLATE'] = 'This is the output: %d'
-        output.values['ARGUMENTS'] = '5'
+    def test_code_from_output_with_arguments(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+
+        output = Output()
+        output.format_string = 'This is the output: %d'
+        output.arguments = '5'
 
         flowchart.add_node(flowchart.root, output)
 
         code, _ = code_generator.generate_code([flowchart])
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int main() {',
             '  printf("This is the output: %d", 5);',
             '  return 0;',
             '}'])
         print(code)
         print(expected)
+        print(repr(code))
+        print(repr(expected))
         assert code == expected, 'Output with arguments.'
 
-    def test_code_from_multiple_empty_functions(self, flowchart: Flowchart, code_generator: CodeGenerator):
-        flowchart2 = Flowchart('func1', flowchart.lang_data)
+    def test_code_from_multiple_empty_functions(self, code_generator: CodeGenerator):
+        flowchart1 = Flowchart('main')
 
-        flowchart3 = Flowchart('func2', flowchart.lang_data)
+        flowchart2 = Flowchart('func1')
 
-        code, _ = code_generator.generate_code([flowchart, flowchart2, flowchart3])
+        flowchart3 = Flowchart('func2')
+
+        code, _ = code_generator.generate_code([flowchart1, flowchart2, flowchart3])
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int func1();',
             'int func2();',
             '',
             'int main() {',
@@ -519,22 +538,24 @@
             '',
             'int func2() {',
             '  return 0;',
             '}'
         ])
         print(code)
         print(expected)
+        print(repr(code))
+        print(repr(expected))
         assert code == expected, 'Declaration of multiple empty functions.'
 
-    def test_code_from_multiple_empty_functions_with_arguments(self,
-                                                               flowchart: Flowchart,
-                                                               code_generator: CodeGenerator):
-        flowchart2 = Flowchart('func1', flowchart.lang_data)
+    def test_code_from_multiple_empty_functions_with_arguments(self, code_generator: CodeGenerator):
+        flowchart1 = Flowchart('main')
+
+        flowchart2 = Flowchart('func1')
 
-        flowchart3 = Flowchart('func2', flowchart.lang_data)
+        flowchart3 = Flowchart('func2')
         flowchart3.root.return_type = 'float'
 
         parameter1 = Parameter()
         parameter1.name = 'x'
         parameter1.type = 'int'
         parameter2 = Parameter()
         parameter2.name = 'y'
@@ -542,15 +563,15 @@
         parameter3 = Parameter()
         parameter3.name = 'z'
         parameter3.type = 'unsigned int'
         flowchart2.root.parameters.append(parameter1)
         flowchart2.root.parameters.append(parameter2)
         flowchart3.root.parameters.append(parameter3)
 
-        code, _ = code_generator.generate_code([flowchart, flowchart2, flowchart3])
+        code, _ = code_generator.generate_code([flowchart1, flowchart2, flowchart3])
         expected = '\n'.join([
             '#include <stdio.h>',
             '',
             'int func1(int x, long y);',
             'float func2(unsigned int z);',
             '',
             'int main() {',
@@ -563,17 +584,20 @@
             '',
             'float func2(unsigned int z) {',
             '  return 0;',
             '}'
         ])
         print(code)
         print(expected)
+        print(repr(code))
+        print(repr(expected))
         assert code == expected, 'Declaration of multiple empty functions.'
 
-    def test_code_from_typedef(self, flowchart: Flowchart, code_generator: CodeGenerator):
+    def test_code_from_typedef(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
         type_definition1 = TypeDefinition()
         type_definition1.definition = 'char *'
         type_definition1.name = 'string'
         flowchart.type_definitions.append(type_definition1)
         type_definition2 = TypeDefinition()
         type_definition2.definition = 'int'
         type_definition2.name = 'testtype'
@@ -593,15 +617,16 @@
             '',
             'int main() {',
             '  return 0;',
             '}'])
         print(expected)
         assert code == expected, 'Type definitions should be included in the source file.'
 
-    def test_code_from_struct(self, flowchart: Flowchart, code_generator: CodeGenerator):
+    def test_code_from_struct(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
         struct_definition = StructDefinition()
         struct_definition.members.clear()
         struct_definition.name = 'Test'
         struct_member1 = StructMember()
         struct_member1.name = 'x'
         struct_member1.type = 'int'
         struct_definition.members.append(struct_member1)
@@ -629,7 +654,66 @@
             '} Test_t;',
             '',
             'int main() {',
             '  return 0;',
             '}'])
         print(expected)
         assert code == expected, 'Structure definitions should be included in the source file.'
+
+    def test_code_from_template(self, code_generator: CodeGenerator):
+        flowchart = Flowchart('main')
+
+        template = Template(
+            {
+                'label': 'Open File',
+                'shape_id': 'data',
+                'color': '(147, 171, 255)',
+                'parameters': [
+                    {
+                        'name': 'VAR_NAME',
+                        'label': 'Name'
+                    },
+                    {
+                        'name': 'FILE',
+                        'label': 'File Path'
+                    },
+                    {
+                        'name': 'MODE',
+                        'label': 'Mode',
+                        'default': 'r',
+                        'options': [
+                            'r',
+                            'r+',
+                            'w',
+                            'w+',
+                            'a',
+                            'a+'
+                        ]
+                    }
+                ],
+                'body': [
+                    'FILE *${VAR_NAME};',
+                    '${VAR_NAME} = fopen(${FILE}, \"${MODE}\");'
+                ]
+            }
+        )
+
+        template.values['VAR_NAME'] = 'x'
+        template.values['FILE'] = '"/test/path/to/file"'
+        template.values['MODE'] = 'w+'
+
+        flowchart.add_node(flowchart.root, template)
+
+        code, _ = code_generator.generate_code([flowchart])
+        expected = '\n'.join([
+            '#include <stdio.h>',
+            '',
+            'int main() {',
+            '  FILE *x;',
+            '  x = fopen("/test/path/to/file", "w+");',
+            '  return 0;',
+            '}'])
+        print(code)
+        print(expected)
+        print(repr(code))
+        print(repr(expected))
+        assert code == expected, 'Template.'
```

### Comparing `FlowTutor-0.10.9/tests/test_flowtutor_flowchart.py` & `FlowTutor-0.9.0/tests/test_flowtutor_flowchart.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,96 @@
-from typing import Any
 from unittest.mock import patch
 import pytest
 
-
+from flowtutor.flowchart.assignment import Assignment
+from flowtutor.flowchart.declaration import Declaration
+from flowtutor.flowchart.conditional import Conditional
 from flowtutor.flowchart.flowchart import Flowchart
+from flowtutor.flowchart.forloop import ForLoop
+from flowtutor.flowchart.input import Input
+from flowtutor.flowchart.output import Output
+from flowtutor.flowchart.snippet import Snippet
+from flowtutor.flowchart.whileloop import WhileLoop
 from flowtutor.flowchart.functionstart import FunctionStart
 from flowtutor.flowchart.functionend import FunctionEnd
 from flowtutor.flowchart.connector import Connector
-from flowtutor.containers import Container
-from flowtutor.flowchart.template import Template
 
 from flowtutor.flowchart.node import dpg as node_dpg
-from flowtutor.language_service import LanguageService
+
+SIMPLE_NODES = [  # Nodes with exactly one input and one output
+    Declaration,
+    Assignment,
+    Input,
+    Output,
+    Snippet
+]
+
+ALL_NODES = [
+    Declaration,
+    Assignment,
+    Conditional,
+    Input,
+    WhileLoop,
+    ForLoop,
+    Output,
+    Snippet,
+    FunctionStart
+]
 
 
 @patch.object(node_dpg, 'get_text_size', lambda _: (0, 0))
 class TestFlowchart:
 
-    @pytest.fixture(scope='session')
-    def nodes(self) -> dict[str, Any]:
-        container = Container()
-        container.init_resources()
-        container.wire(modules=[
-            'flowtutor.language_service',
-            'flowtutor.flowchart.template',
-            'flowtutor.flowchart.functionstart',
-            'flowtutor.flowchart.functionend'])
-        language_service = LanguageService()
-        flowchart = Flowchart('main', {
-            'lang_id': 'c'
-        })
-        language_service.finish_init(flowchart)
-        return language_service.get_node_templates(flowchart)
+    @pytest.mark.parametrize('node_class', ALL_NODES)
+    def test_new_node_has_tag(self, node_class):
+        node = node_class()
+        assert node.tag
 
     def check_roots(self, flowchart):
         for i, node in enumerate(flowchart):
             if i == 0:
                 assert isinstance(node, FunctionStart), 'The first node must be the function start'
             elif i == 1:
                 assert isinstance(node, FunctionEnd), 'The last node must be the function end'
 
     def test_flowchart_initialize_root(self):
-        flowchart = Flowchart('main', {})
+        flowchart = Flowchart('main')
         assert len(flowchart) == 2, 'A new flowchart should contain exactly 2 Nodes ("main" and "End")'
         self.check_roots(flowchart)
 
-    def test_flowchart_add_nodes(self, nodes: dict[str, Any]):
-        flowchart = Flowchart('main', {})
-        node1 = Template(nodes['Declaration'])
-        node2 = Template(nodes['Declaration'])
+    @pytest.mark.parametrize('node_class', SIMPLE_NODES)
+    def test_flowchart_add_nodes(self, node_class):
+        flowchart = Flowchart('main')
+        node1 = node_class()
+        node2 = node_class()
         flowchart.add_node(flowchart.root, node1)
         flowchart.add_node(node1, node2)
         assert len(flowchart) == 4, 'After adding 2 nodes, there should be 4 nodes in the flowchart'
         root_connection_0 = flowchart.root.find_connection(0)
         assert root_connection_0
         assert root_connection_0.dst_node == node1, 'There should be a connection from root to node1'
         node1_connection_0 = node1.find_connection(0)
         assert node1_connection_0
         assert node1_connection_0.dst_node == node2, 'There should be a connection from node1 to node2'
 
-    def test_flowchart_add_loop(self, nodes: dict[str, Any]):
-        flowchart = Flowchart('main', {})
-        loop1 = Template(nodes['While loop'])
+    def test_flowchart_add_loop(self):
+        flowchart = Flowchart('main')
+        loop1 = WhileLoop()
         flowchart.add_node(flowchart.root, loop1)
         assert len(flowchart) == 3, 'After adding a loop, there should be 3 nodes in the flowchart'
         root_connection_0 = flowchart.root.find_connection(0)
         assert root_connection_0
         assert root_connection_0.dst_node == loop1, 'There should be a connection from root to the loop'
         loop1_connection_1 = loop1.find_connection(1)
         assert loop1_connection_1
         assert loop1_connection_1.dst_node == loop1, 'There should be a connection from the loop to itself'
 
-    def test_flowchart_add_conditional(self, nodes: dict[str, Any]):
-        flowchart = Flowchart('main', {})
-        node1 = Template(nodes['Conditional'])
+    def test_flowchart_add_conditional(self):
+        flowchart = Flowchart('main')
+        node1 = Conditional()
         flowchart.add_node(flowchart.root, node1)
         assert len(flowchart) == 4, ('After adding a conditional, there should be 4 nodes in the flowchart'
                                      ' (including the conditional connector)')
         root_connection_0 = flowchart.root.find_connection(0)
         assert root_connection_0
         assert root_connection_0.dst_node == node1, 'There should be a connection from root to the conditional'
         node1_connection_0 = node1.find_connection(0)
@@ -87,104 +100,108 @@
         node1_connection_1 = node1.find_connection(1)
         assert node1_connection_1
         connector_1 = node1_connection_1.dst_node
         assert isinstance(connector_1, Connector), ('There should be a second connection '
                                                     'from the conditional to the connector')
         assert connector_0 == connector_1, 'The connections of the conditional should be to the same connector'
 
-    def test_flowchart_add_and_remove_node(self, nodes: dict[str, Any]):
-        flowchart = Flowchart('main', {})
-        node1 = Template(nodes['Declaration'])
+    @pytest.mark.parametrize('node_class', SIMPLE_NODES)
+    def test_flowchart_add_and_remove_node(self, node_class):
+        flowchart = Flowchart('main')
+        node1 = node_class()
         flowchart.add_node(flowchart.root, node1)
         assert len(flowchart) == 3, 'After adding a node, there should be 3 nodes in the flowchart'
         flowchart.remove_node(node1)
         assert len(flowchart) == 2, 'After removing the node, there should be 2 node in the flowchart'
         self.check_roots(flowchart)  # The remaining nodes should be the roots
 
-    def test_flowchart_add_and_remove_conditional(self, nodes: dict[str, Any]):
-        flowchart = Flowchart('main', {})
-        conditional1 = Template(nodes['Conditional'])
+    def test_flowchart_add_and_remove_conditional(self):
+        flowchart = Flowchart('main')
+        conditional1 = Conditional()
         flowchart.add_node(flowchart.root, conditional1)
         assert len(flowchart) == 4, 'After adding a conditional, there should be 4 nodes in the flowchart'
         flowchart.remove_node(conditional1)
         assert len(flowchart) == 2, 'After removing the conditional, there should be 2 nodes in the flowchart'
         self.check_roots(flowchart)  # The remaining nodes should be the roots
 
-    def test_flowchart_node_in_loop_body(self, nodes: dict[str, Any]):
-        flowchart = Flowchart('main', {})
-        loop1 = Template(nodes['While loop'])
-        node1 = Template(nodes['Declaration'])
+    @pytest.mark.parametrize('node_class', SIMPLE_NODES)
+    def test_flowchart_node_in_loop_body(self, node_class):
+        flowchart = Flowchart('main')
+        loop1 = WhileLoop()
+        node1 = node_class()
         flowchart.add_node(flowchart.root, loop1)
         flowchart.add_node(loop1, node1, 1)
         assert len(flowchart) == 4, ('After adding a loop and a node in the loop body, '
                                      'there should be 4 nodes in the flowchart')
         loop_connection_1 = loop1.find_connection(1)
         assert loop_connection_1
         assert loop_connection_1.dst_node == node1, 'There should be a connection from the loop to the node'
         assert loop1.tag == node1.scope[-1], 'The scope of the node should be the loop'
         node1_connection_0 = node1.find_connection(0)
         assert node1_connection_0
         assert node1_connection_0.dst_node == loop1, 'There should be a connection from the node to the loop'
 
-    def test_flowchart_add_and_remove_nested_conditional(self, nodes: dict[str, Any]):
-        flowchart = Flowchart('main', {})
+    @pytest.mark.parametrize('node_class', SIMPLE_NODES)
+    def test_flowchart_add_and_remove_nested_conditional(self, node_class):
+        flowchart = Flowchart('main')
 
-        conditional1 = Template(nodes['Conditional'])
+        conditional1 = Conditional()
         flowchart.add_node(flowchart.root, conditional1)
         assert len(flowchart) == 4, 'After adding a conditional, there should be 4 nodes in the flowchart'
 
-        conditional2 = Template(nodes['Conditional'])
+        conditional2 = Conditional()
         flowchart.add_node(conditional1, conditional2, 1)
         assert len(flowchart) == 6, 'After adding a second conditional, there should be 6 nodes in the flowchart'
         conditional1_connection_1 = conditional1.find_connection(1)
         assert conditional1_connection_1
         assert conditional1_connection_1.dst_node == conditional2, ('There should be a connection '
                                                                     'from the first to the second conditional')
 
         assert conditional1.tag == conditional2.scope[-1], ('The scope of the second conditional '
                                                             'should be the first conditional')
 
-        node1 = Template(nodes['Declaration'])
+        node1 = node_class()
         flowchart.add_node(conditional2, node1, 0)
         assert len(flowchart) == 7, ('After adding a node to the second conditional, '
                                      'there should be 7 nodes in the flowchart')
         assert conditional2.tag == node1.scope[-1], 'The inner scope of node1 should be the second conditional'
         assert conditional1.tag == node1.scope[-2], 'The outer scope of node1 should be the first conditional'
 
-        node2 = Template(nodes['Declaration'])
+        node2 = node_class()
         flowchart.add_node(conditional2, node2, 0)
         assert len(flowchart) == 8, ('After adding another node to the second conditional, '
                                      'there should be 8 nodes in the flowchart')
         assert conditional2.tag == node2.scope[-1], 'The inner scope of node2 should be the second conditional'
         assert conditional1.tag == node2.scope[-2], 'The outer scope of node2 should be the first conditional'
 
         flowchart.remove_node(conditional1)
         assert len(flowchart) == 2, 'After removing the outer conditional, there should be 2 nodes in the flowchart'
         self.check_roots(flowchart)  # The remaining nodes should be the roots
 
-    def test_flowchart_add_and_remove_nested_loops(self, nodes: dict[str, Any]):
-        flowchart = Flowchart('main', {})
+    @pytest.mark.parametrize('node_class', SIMPLE_NODES)
+    def test_flowchart_add_and_remove_nested_loops(self, node_class):
+        flowchart = Flowchart('main')
 
-        loop1 = Template(nodes['While loop'])
+        loop1 = WhileLoop()
         flowchart.add_node(flowchart.root, loop1)
         assert len(flowchart) == 3, 'After adding a loop, there should be 3 nodes in the flowchart'
 
-        loop2 = Template(nodes['While loop'])
+        loop2 = WhileLoop()
         flowchart.add_node(loop1, loop2, 1)
         assert len(flowchart) == 4, 'After adding another loop, there should be 4 nodes in the flowchart'
         assert loop1.tag == loop2.scope[-1], ('The scope of the second loop should be the first loop')
 
-        node1 = Template(nodes['Declaration'])
+        node1 = node_class()
         flowchart.add_node(loop2, node1, 1)
         assert len(flowchart) == 5, ('After adding a node to the second loop body,'
                                      'there should be 5 nodes in the flowchart')
         assert loop2.tag == node1.scope[-1], 'The inner scope of node1 should be the second conditional'
         assert loop1.tag == node1.scope[-2], 'The outer scope of node1 should be the first conditional'
 
-        node2 = Template(nodes['Declaration'])
+        node2 = node_class()
         flowchart.add_node(loop2, node2, 1)
         assert len(flowchart) == 6, ('After adding another node to the second loop body, '
                                      'there should be 6 nodes in the flowchart')
         assert loop2.tag == node2.scope[-1], 'The inner scope of node2 should be the second conditional'
         assert loop1.tag == node2.scope[-2], 'The outer scope of node2 should be the first conditional'
 
         flowchart.remove_node(loop1)
```

