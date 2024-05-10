# Comparing `tmp/toui-3.5.0a3.tar.gz` & `tmp/toui-3.5.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-3.5.0a3.tar", last modified: Fri May 10 13:44:34 2024, max compression
+gzip compressed data, was "toui-3.5.0a4.tar", last modified: Fri May 10 13:50:50 2024, max compression
```

## Comparing `toui-3.5.0a3.tar` & `toui-3.5.0a4.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 13:44:34.767867 toui-3.5.0a3/
--rw-rw-rw-   0        0        0     1094 2024-05-10 13:17:12.000000 toui-3.5.0a3/LICENSE
--rw-rw-rw-   0        0        0       16 2024-05-10 13:17:12.000000 toui-3.5.0a3/MANIFEST.in
--rw-rw-rw-   0        0        0     5411 2024-05-10 13:44:34.766339 toui-3.5.0a3/PKG-INFO
--rw-rw-rw-   0        0        0     4975 2024-05-10 13:17:12.000000 toui-3.5.0a3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 13:44:34.734242 toui-3.5.0a3/examples/
--rw-rw-rw-   0        0        0        0 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0     1373 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/advanced_example_2_toui_with_javascript.py
--rw-rw-rw-   0        0        0     2119 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/advanced_example_3_toui_with_google_sign_in.py
--rw-rw-rw-   0        0        0     3663 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/advanced_example_4_toui_with_firebase.py
--rw-rw-rw-   0        0        0     2806 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/advanced_example_5_toui_with_sql_user_database.py
--rw-rw-rw-   0        0        0     7653 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/advanced_example_6_widgets.py
--rw-rw-rw-   0        0        0      556 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2024-05-10 13:17:12.000000 toui-3.5.0a3/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:44:34.747713 toui-3.5.0a3/images/
--rw-rw-rw-   0        0        0  2404280 2024-05-10 13:17:12.000000 toui-3.5.0a3/images/calculator.gif
--rw-rw-rw-   0        0        0  2803703 2024-05-10 13:17:12.000000 toui-3.5.0a3/images/home.gif
--rw-rw-rw-   0        0        0    27837 2024-05-10 13:17:12.000000 toui-3.5.0a3/images/icon.png
--rw-rw-rw-   0        0        0    29049 2024-05-10 13:17:12.000000 toui-3.5.0a3/images/logo.png
--rw-rw-rw-   0        0        0       42 2024-05-10 13:44:34.767867 toui-3.5.0a3/setup.cfg
--rw-rw-rw-   0        0        0     1617 2024-05-10 13:44:12.000000 toui-3.5.0a3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:44:34.760175 toui-3.5.0a3/toui/
--rw-rw-rw-   0        0        0      291 2024-05-10 13:17:12.000000 toui-3.5.0a3/toui/__init__.py
--rw-rw-rw-   0        0        0      379 2024-05-10 13:17:12.000000 toui-3.5.0a3/toui/_defaults.py
--rw-rw-rw-   0        0        0     1406 2024-05-10 13:17:12.000000 toui-3.5.0a3/toui/_helpers.py
--rw-rw-rw-   0        0        0    11001 2024-05-10 13:17:12.000000 toui-3.5.0a3/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     8637 2024-05-10 13:17:12.000000 toui-3.5.0a3/toui/_signals.py
--rw-rw-rw-   0        0        0    64253 2024-05-10 13:17:12.000000 toui-3.5.0a3/toui/apps.py
--rw-rw-rw-   0        0        0    27205 2024-05-10 13:17:12.000000 toui-3.5.0a3/toui/elements.py
--rw-rw-rw-   0        0        0      451 2024-05-10 13:17:12.000000 toui-3.5.0a3/toui/exceptions.py
--rw-rw-rw-   0        0        0    22102 2024-05-10 13:17:12.000000 toui-3.5.0a3/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2024-05-10 13:17:12.000000 toui-3.5.0a3/toui/structure.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:44:34.766339 toui-3.5.0a3/toui.egg-info/
--rw-rw-rw-   0        0        0     5411 2024-05-10 13:44:34.000000 toui-3.5.0a3/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2024-05-10 13:44:34.000000 toui-3.5.0a3/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 13:44:34.000000 toui-3.5.0a3/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-10 13:44:34.000000 toui-3.5.0a3/toui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      253 2024-05-10 13:44:34.000000 toui-3.5.0a3/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-10 13:44:34.000000 toui-3.5.0a3/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 13:50:50.824073 toui-3.5.0a4/
+-rw-rw-rw-   0        0        0     1094 2024-05-10 13:17:12.000000 toui-3.5.0a4/LICENSE
+-rw-rw-rw-   0        0        0       16 2024-05-10 13:17:12.000000 toui-3.5.0a4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5411 2024-05-10 13:50:50.824073 toui-3.5.0a4/PKG-INFO
+-rw-rw-rw-   0        0        0     4975 2024-05-10 13:17:12.000000 toui-3.5.0a4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 13:50:50.785944 toui-3.5.0a4/cmd/
+-rw-rw-rw-   0        0        0        0 2024-05-10 13:49:57.000000 toui-3.5.0a4/cmd/__init__.py
+-rw-rw-rw-   0        0        0     2617 2024-05-10 13:17:12.000000 toui-3.5.0a4/cmd/_cmd.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:50:50.801010 toui-3.5.0a4/examples/
+-rw-rw-rw-   0        0        0        0 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0     1373 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/advanced_example_2_toui_with_javascript.py
+-rw-rw-rw-   0        0        0     2119 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/advanced_example_3_toui_with_google_sign_in.py
+-rw-rw-rw-   0        0        0     3663 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/advanced_example_4_toui_with_firebase.py
+-rw-rw-rw-   0        0        0     2806 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/advanced_example_5_toui_with_sql_user_database.py
+-rw-rw-rw-   0        0        0     7653 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/advanced_example_6_widgets.py
+-rw-rw-rw-   0        0        0      556 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2024-05-10 13:17:12.000000 toui-3.5.0a4/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:50:50.811142 toui-3.5.0a4/images/
+-rw-rw-rw-   0        0        0  2404280 2024-05-10 13:17:12.000000 toui-3.5.0a4/images/calculator.gif
+-rw-rw-rw-   0        0        0  2803703 2024-05-10 13:17:12.000000 toui-3.5.0a4/images/home.gif
+-rw-rw-rw-   0        0        0    27837 2024-05-10 13:17:12.000000 toui-3.5.0a4/images/icon.png
+-rw-rw-rw-   0        0        0    29049 2024-05-10 13:17:12.000000 toui-3.5.0a4/images/logo.png
+-rw-rw-rw-   0        0        0       42 2024-05-10 13:50:50.824073 toui-3.5.0a4/setup.cfg
+-rw-rw-rw-   0        0        0     1621 2024-05-10 13:50:26.000000 toui-3.5.0a4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:50:50.819227 toui-3.5.0a4/toui/
+-rw-rw-rw-   0        0        0      291 2024-05-10 13:17:12.000000 toui-3.5.0a4/toui/__init__.py
+-rw-rw-rw-   0        0        0      379 2024-05-10 13:17:12.000000 toui-3.5.0a4/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1406 2024-05-10 13:17:12.000000 toui-3.5.0a4/toui/_helpers.py
+-rw-rw-rw-   0        0        0    11001 2024-05-10 13:17:12.000000 toui-3.5.0a4/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     8637 2024-05-10 13:17:12.000000 toui-3.5.0a4/toui/_signals.py
+-rw-rw-rw-   0        0        0    64253 2024-05-10 13:17:12.000000 toui-3.5.0a4/toui/apps.py
+-rw-rw-rw-   0        0        0    27205 2024-05-10 13:17:12.000000 toui-3.5.0a4/toui/elements.py
+-rw-rw-rw-   0        0        0      451 2024-05-10 13:17:12.000000 toui-3.5.0a4/toui/exceptions.py
+-rw-rw-rw-   0        0        0    22102 2024-05-10 13:17:12.000000 toui-3.5.0a4/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2024-05-10 13:17:12.000000 toui-3.5.0a4/toui/structure.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:50:50.823227 toui-3.5.0a4/toui.egg-info/
+-rw-rw-rw-   0        0        0     5411 2024-05-10 13:50:50.000000 toui-3.5.0a4/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1076 2024-05-10 13:50:50.000000 toui-3.5.0a4/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 13:50:50.000000 toui-3.5.0a4/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-10 13:50:50.000000 toui-3.5.0a4/toui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      253 2024-05-10 13:50:50.000000 toui-3.5.0a4/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 13:50:50.000000 toui-3.5.0a4/toui.egg-info/top_level.txt
```

### Comparing `toui-3.5.0a3/LICENSE` & `toui-3.5.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/PKG-INFO` & `toui-3.5.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 3.5.0a3
+Version: 3.5.0a4
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Home-page: UNKNOWN
 Author: Mubarak Almehairbi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `toui-3.5.0a3/README.md` & `toui-3.5.0a4/README.md`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/examples/advanced_example_1_toui_blueprint.py` & `toui-3.5.0a4/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/examples/advanced_example_2_toui_with_javascript.py` & `toui-3.5.0a4/examples/advanced_example_2_toui_with_javascript.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/examples/advanced_example_3_toui_with_google_sign_in.py` & `toui-3.5.0a4/examples/advanced_example_3_toui_with_google_sign_in.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/examples/advanced_example_4_toui_with_firebase.py` & `toui-3.5.0a4/examples/advanced_example_4_toui_with_firebase.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/examples/advanced_example_5_toui_with_sql_user_database.py` & `toui-3.5.0a4/examples/advanced_example_5_toui_with_sql_user_database.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/examples/advanced_example_6_widgets.py` & `toui-3.5.0a4/examples/advanced_example_6_widgets.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/examples/example_1_simple_website.py` & `toui-3.5.0a4/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/examples/example_2_simple_desktop_app.py` & `toui-3.5.0a4/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/examples/example_3_updating_page.py` & `toui-3.5.0a4/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/examples/example_4_function_with_arg.py` & `toui-3.5.0a4/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/examples/example_5_user_variables.py` & `toui-3.5.0a4/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/images/calculator.gif` & `toui-3.5.0a4/images/calculator.gif`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/images/home.gif` & `toui-3.5.0a4/images/home.gif`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/images/icon.png` & `toui-3.5.0a4/images/icon.png`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/images/logo.png` & `toui-3.5.0a4/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/setup.py` & `toui-3.5.0a4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 small = False
 if "--small" in sys.argv:
     small = True
     sys.argv.remove('--small')
 
 name = "ToUI"
-version = "v3.5.0-alpha.3"
+version = "v3.5.0-alpha.4"
 author = "Mubarak Almehairbi"
 description = "Creates user interfaces (websites and desktop apps) from HTML easily"
 package_name = "toui"
 requirements = []
 optional_requirements = ['flask-login', 'flask-sqlalchemy', 'flask-basicauth']
 
 reqs_txt = open("requirements.txt", "r").read()
@@ -37,15 +37,15 @@
     author=author,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
     package_data={'images': ['images/*']},
-    entry_points={'console_scripts': ['toui=_cmd:main']},
+    entry_points={'console_scripts': ['toui=cmd._cmd:main']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     py_modules=[package_name],
     install_requires=requirements
```

### Comparing `toui-3.5.0a3/toui/_helpers.py` & `toui-3.5.0a4/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/toui/_javascript_templates.py` & `toui-3.5.0a4/toui/_javascript_templates.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/toui/_signals.py` & `toui-3.5.0a4/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/toui/apps.py` & `toui-3.5.0a4/toui/apps.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/toui/elements.py` & `toui-3.5.0a4/toui/elements.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/toui/pages.py` & `toui-3.5.0a4/toui/pages.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/toui/structure.py` & `toui-3.5.0a4/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-3.5.0a3/toui.egg-info/PKG-INFO` & `toui-3.5.0a4/toui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 3.5.0a3
+Version: 3.5.0a4
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Home-page: UNKNOWN
 Author: Mubarak Almehairbi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `toui-3.5.0a3/toui.egg-info/SOURCES.txt` & `toui-3.5.0a4/toui.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+cmd/__init__.py
+cmd/_cmd.py
 examples/__init__.py
 examples/advanced_example_1_toui_blueprint.py
 examples/advanced_example_2_toui_with_javascript.py
 examples/advanced_example_3_toui_with_google_sign_in.py
 examples/advanced_example_4_toui_with_firebase.py
 examples/advanced_example_5_toui_with_sql_user_database.py
 examples/advanced_example_6_widgets.py
```

