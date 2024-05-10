# Comparing `tmp/nicegui_tabulator-0.1.0.tar.gz` & `tmp/nicegui_tabulator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicegui_tabulator-0.1.0.tar", max compression
+gzip compressed data, was "nicegui_tabulator-0.1.1.tar", max compression
```

## Comparing `nicegui_tabulator-0.1.0.tar` & `nicegui_tabulator-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1094 2024-05-08 17:39:27.737805 nicegui_tabulator-0.1.0/LICENSE
--rw-r--r--   0        0        0      128 2024-05-08 14:53:27.237225 nicegui_tabulator-0.1.0/nicegui_tabulator/__init__.py
--rw-r--r--   0        0        0      298 2024-05-08 17:33:19.252414 nicegui_tabulator-0.1.0/nicegui_tabulator/core/events.py
--rw-r--r--   0        0        0    33593 2024-05-08 15:00:49.017552 nicegui_tabulator-0.1.0/nicegui_tabulator/core/libs/tabulator.min.css
--rw-r--r--   0        0        0   484963 2024-05-08 15:01:02.793045 nicegui_tabulator-0.1.0/nicegui_tabulator/core/libs/tabulator.min.js
--rw-r--r--   0        0        0     2143 2024-05-08 17:36:39.253263 nicegui_tabulator-0.1.0/nicegui_tabulator/core/tabulator.js
--rw-r--r--   0        0        0     2480 2024-05-08 18:00:42.829317 nicegui_tabulator-0.1.0/nicegui_tabulator/core/tabulator.py
--rw-r--r--   0        0        0       97 2024-05-08 14:40:20.875090 nicegui_tabulator-0.1.0/nicegui_tabulator/version.py
--rw-r--r--   0        0        0      511 2024-05-08 17:52:15.529996 nicegui_tabulator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1830 2024-05-08 17:38:13.156421 nicegui_tabulator-0.1.0/README.md
--rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 nicegui_tabulator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-05-08 17:39:27.737805 nicegui_tabulator-0.1.1/LICENSE
+-rw-r--r--   0        0        0      128 2024-05-08 14:53:27.237225 nicegui_tabulator-0.1.1/nicegui_tabulator/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-08 17:33:19.252414 nicegui_tabulator-0.1.1/nicegui_tabulator/core/events.py
+-rw-r--r--   0        0        0    33593 2024-05-08 15:00:49.017552 nicegui_tabulator-0.1.1/nicegui_tabulator/core/libs/tabulator.min.css
+-rw-r--r--   0        0        0   484963 2024-05-08 15:01:02.793045 nicegui_tabulator-0.1.1/nicegui_tabulator/core/libs/tabulator.min.js
+-rw-r--r--   0        0        0     2575 2024-05-10 14:29:33.793888 nicegui_tabulator-0.1.1/nicegui_tabulator/core/tabulator.js
+-rw-r--r--   0        0        0     5674 2024-05-10 14:29:33.793888 nicegui_tabulator-0.1.1/nicegui_tabulator/core/tabulator.py
+-rw-r--r--   0        0        0       97 2024-05-08 14:40:20.875090 nicegui_tabulator-0.1.1/nicegui_tabulator/version.py
+-rw-r--r--   0        0        0      565 2024-05-10 14:32:42.352222 nicegui_tabulator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1830 2024-05-08 17:38:13.156421 nicegui_tabulator-0.1.1/README.md
+-rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 nicegui_tabulator-0.1.1/PKG-INFO
```

### Comparing `nicegui_tabulator-0.1.0/LICENSE` & `nicegui_tabulator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nicegui_tabulator-0.1.0/nicegui_tabulator/core/libs/tabulator.min.css` & `nicegui_tabulator-0.1.1/nicegui_tabulator/core/libs/tabulator.min.css`

 * *Files identical despite different names*

### Comparing `nicegui_tabulator-0.1.0/nicegui_tabulator/core/libs/tabulator.min.js` & `nicegui_tabulator-0.1.1/nicegui_tabulator/core/libs/tabulator.min.js`

 * *Files identical despite different names*

### Comparing `nicegui_tabulator-0.1.0/nicegui_tabulator/core/tabulator.js` & `nicegui_tabulator-0.1.1/nicegui_tabulator/core/tabulator.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,13 @@
 import {
     loadResource
 } from "../../static/utils/resources.js";
+import {
+    convertDynamicProperties
+} from "../../static/utils/dynamic_properties.js";
 
 
 const eventArgsExtractor = new Map([
     ['dataFiltering', filters => ({
         filters
     })],
     ['dataFiltered', (filters, rows) => ({
@@ -69,15 +72,15 @@
     },
     async mounted() {
         await this.$nextTick(); // NOTE: wait for window.path_prefix to be set
         await Promise.all([
             loadResource(window.path_prefix + `${this.resource_path}/tabulator.min.css`),
         ]);
 
-
+        convertDynamicProperties(this.options, true);
         this.table = new Tabulator(this.$el, this.options);
 
     },
 
     methods: {
         onEvent(eventName) {
 
@@ -92,9 +95,20 @@
         run_table_method(name, ...args) {
             if (name.startsWith(":")) {
                 name = name.slice(1);
                 args = args.map((arg) => new Function(`return (${arg})`)());
             }
             return runMethod(this.table, name, args);
         },
+
+        setColumns(columns) {
+            convertDynamicProperties(columns, true);
+            this.table.setColumns(columns);
+        },
+
+        updateColumnDefinition(field, definition) {
+            convertDynamicProperties(definition, true);
+            this.table.updateColumnDefinition(field, definition);
+        },
+
     },
 };
```

### Comparing `nicegui_tabulator-0.1.0/README.md` & `nicegui_tabulator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nicegui_tabulator-0.1.0/PKG-INFO` & `nicegui_tabulator-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nicegui-tabulator
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is a Python package that provides a simple way to create tables using the Tabulator library. It is built on top of the NiceGUI library.
 Author: CrystalWindSnake
 Author-email: 568166495@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

