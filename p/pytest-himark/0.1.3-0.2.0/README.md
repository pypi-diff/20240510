# Comparing `tmp/pytest_himark-0.1.3.tar.gz` & `tmp/pytest_himark-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_himark-0.1.3.tar", last modified: Sun Apr 14 08:19:54 2024, max compression
+gzip compressed data, was "pytest_himark-0.2.0.tar", last modified: Fri May 10 05:40:42 2024, max compression
```

## Comparing `pytest_himark-0.1.3.tar` & `pytest_himark-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 08:19:54.229738 pytest_himark-0.1.3/
--rw-rw-rw-   0        0        0     1111 2024-04-07 10:46:35.000000 pytest_himark-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     5990 2024-04-14 08:19:54.229738 pytest_himark-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3233 2024-04-14 08:04:14.000000 pytest_himark-0.1.3/README.rst
--rw-rw-rw-   0        0        0     1642 2024-04-14 08:13:12.000000 pytest_himark-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 08:19:54.229738 pytest_himark-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-14 08:19:54.206738 pytest_himark-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-14 08:19:54.213737 pytest_himark-0.1.3/src/pytest_himark/
--rw-rw-rw-   0        0        0        0 2024-04-07 10:46:35.000000 pytest_himark-0.1.3/src/pytest_himark/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-07 21:08:47.000000 pytest_himark-0.1.3/src/pytest_himark/plugin.py
-drwxrwxrwx   0        0        0        0 2024-04-14 08:19:54.228736 pytest_himark-0.1.3/src/pytest_himark.egg-info/
--rw-rw-rw-   0        0        0     5990 2024-04-14 08:19:54.000000 pytest_himark-0.1.3/src/pytest_himark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-04-14 08:19:54.000000 pytest_himark-0.1.3/src/pytest_himark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 08:19:54.000000 pytest_himark-0.1.3/src/pytest_himark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-14 08:19:54.000000 pytest_himark-0.1.3/src/pytest_himark.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-14 08:19:54.000000 pytest_himark-0.1.3/src/pytest_himark.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-14 08:19:54.000000 pytest_himark-0.1.3/src/pytest_himark.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-14 08:19:54.227736 pytest_himark-0.1.3/tests/
--rw-rw-rw-   0        0        0     5074 2024-04-07 21:08:47.000000 pytest_himark-0.1.3/tests/test_himark.py
+drwxrwxrwx   0        0        0        0 2024-05-10 05:40:42.034252 pytest_himark-0.2.0/
+-rw-rw-rw-   0        0        0     1111 2024-04-07 10:46:35.000000 pytest_himark-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     8904 2024-05-10 05:40:42.033251 pytest_himark-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6370 2024-05-10 05:40:28.000000 pytest_himark-0.2.0/README.rst
+-rw-rw-rw-   0        0        0     3417 2024-05-10 05:39:26.000000 pytest_himark-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 05:40:42.034252 pytest_himark-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 05:40:42.022357 pytest_himark-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 05:40:42.027504 pytest_himark-0.2.0/src/pytest_himark/
+-rw-rw-rw-   0        0        0        0 2024-04-07 10:46:35.000000 pytest_himark-0.2.0/src/pytest_himark/__init__.py
+-rw-rw-rw-   0        0        0     3032 2024-05-09 19:35:33.000000 pytest_himark-0.2.0/src/pytest_himark/plugin.py
+drwxrwxrwx   0        0        0        0 2024-05-10 05:40:42.033251 pytest_himark-0.2.0/src/pytest_himark.egg-info/
+-rw-rw-rw-   0        0        0     8904 2024-05-10 05:40:42.000000 pytest_himark-0.2.0/src/pytest_himark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-05-10 05:40:42.000000 pytest_himark-0.2.0/src/pytest_himark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 05:40:42.000000 pytest_himark-0.2.0/src/pytest_himark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-10 05:40:42.000000 pytest_himark-0.2.0/src/pytest_himark.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-10 05:40:42.000000 pytest_himark-0.2.0/src/pytest_himark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-10 05:40:42.000000 pytest_himark-0.2.0/src/pytest_himark.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 05:40:42.032251 pytest_himark-0.2.0/tests/
+-rw-rw-rw-   0        0        0     6593 2024-05-09 19:35:33.000000 pytest_himark-0.2.0/tests/test_himark.py
```

### Comparing `pytest_himark-0.1.3/LICENSE` & `pytest_himark-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_himark-0.1.3/PKG-INFO` & `pytest_himark-0.2.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,7 @@
-Metadata-Version: 2.1
-Name: pytest-himark
-Version: 0.1.3
-Summary: A plugin that will filter pytest's test collection using a json file. It will read a json file provided with a --json argument in pytest command line (or in pytest.ini), search the markers key and automatically add -m option to the command line for filtering out the tests marked with disabled markers.
-Author-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
-Maintainer-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
-License: 
-        The MIT License (MIT)
-        
-        Copyright (c) 2024 Rodolphe Mete Soyding
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in
-        all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-        THE SOFTWARE.
-        
-Project-URL: Repository, https://github.com/supermete/pytest-himark
-Classifier: Framework :: Pytest
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Testing
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: pytest>=6.2.0
-
 =============
 pytest-himark
 =============
 
 .. image:: https://img.shields.io/pypi/v/pytest-himark.svg
     :target: https://pypi.org/project/pytest-himark
     :alt: PyPI version
@@ -60,18 +10,15 @@
     :target: https://pypi.org/project/pytest-himark
     :alt: Python versions
 
 .. image:: https://github.com/supermete/pytest-himark/actions/workflows/main.yml/badge.svg
     :target: https://github.com/supermete/pytest-himark/actions/workflows/main.yml
     :alt: See Build Status on GitHub Actions
 
-A plugin that will filter pytest's test collection using a json file.
-It will read a json file provided with a --json argument in pytest command line
-(or in pytest.ini), search the 'markers' key and automatically add -m option to
-the command line for filtering out the tests marked with disabled markers.
+pytest-himark is a plugin that creates markers from a json configuration to filter pytest's test collection.
 
 ----
 
 This `pytest`_ plugin was generated with `Cookiecutter`_ along with `@hackebrot`_'s `cookiecutter-pytest-plugin`_ template.
 
 
 Requirements
@@ -92,42 +39,183 @@
 -----
 
 After installing this plugin, pytest will automatically load it when launching tests.
 You will simply need to add the --json option to the command line with the path to the
 json containing the markers you want to enable. Alternatively, you can add the --json
 option and the path in the pytest.ini directly, in the addopts variable.
 
-Example:
-    - pytest.ini:
+- In pytest.ini:
 
     .. code-block:: INI
 
         addopts = --json=path/to/my/config.json
 
-    - config.json:
+    ..
+
+- Or by command line:
+
+    .. code-block::
+
+        >> pytest --json=path/to/my/config.json
+
+    ..
+
+The markers can be configured in 4 ways to give more flexibility to the end user.
+The first way is having a 'markers' key containing a dictionary with the name of the markers as key, and a boolean as value.
+If the boolean is true, the marker with the specified name will be created.
+
+Example:
+
+.. code-block:: JSON
+
+    {
+        'markers': {
+            'marker1': true,
+            'marker2': true,
+            'marker3': false,
+            'marker4': false
+        }
+    }
+..
+
+This json will result in the following marker filtering:
+
+.. code-block::
+
+    -m '(marker1 or marker2)'
+..
+
+Another way of specifying marker is to define a 'devices' key, with a list of dictionaries as value.
+Each key from the 'devices' list can be refered to as a 'device' and should contain a key named 'name' as a string and a key named 'used' as a boolean.
+If the 'used' key of a device is set to true, a marker will be created and named with the 'name' string.
+
+Example:
+
+.. code-block:: JSON
+
+    {
+        'devices': [
+             {
+                'name': "device1",
+                'used': true,
+             },
+             {
+                'name': "device2",
+                'used': false,
+             }
+        ]
+    }
+..
+
+This json will result in the following marker filtering:
+
+.. code-block::
+
+    -m '(device1)'
+..
+
+Another way to specifying marker is to have a key named 'type' in a device-specific dictionary (see above), defined as a string.
+A marker with the string value of the 'type' will be created.
+
+Example:
+
+.. code-block:: JSON
+
+    {
+        'devices': [
+             {
+                'name': "device1",
+                'type': "my_type"
+                'used': true,
+             },
+             {
+                'name': "device2",
+                'used': false,
+             }
+        ]
+    }
+..
+
+This json will result in the following marker filtering:
+
+.. code-block::
+
+    -m '(device1 or my_type)'
+..
+
+One last way to specifying marker is to have keys named 'do', 'di' and/or 'ai' in a device-specific dictionary (see above), defined as list of strings.
+A marker will be created for every string in those arrays.
+
+Example:
+
+.. code-block:: JSON
+
+    {
+        'devices': [
+            {
+                "name": "device1",
+                "do": [
+                    "do1"
+                ],
+                "di": [
+                    "di1"
+                ],
+                "ai": [
+                    "ai1"
+                ],
+                "used": true,
+             }
+            {
+                "name": "device2",
+                "used": false,
+             }
+        ]
+    }
+
+..
+
+This json will result in the following marker filtering:
+
+.. code-block::
+
+    -m '(device1 or do1 or di1 or ai1)'
+..
+
+
+Launching pytest now will then automatically add the filter to the command line, e.g.:
+
+.. code-block:: python
+
+    >> pytest -m '(device1 or do1 or di1 or ai1)'
+..
+
+Finally, after pytest test collection has completed, this plugin will also filter out any test that is marked with an undefined marker.
+For example consider the following config:
 
 .. code-block:: JSON
 
-        {
-            "markers": {
-                "my_marker1": true,
-                "my_marker2": true,
-                "my_marker3": false,
-                "my_marker4": false
-            }
+    {
+        'markers': {
+            'marker1': true
         }
+    }
 
 ..
 
-    Launching pytest now will automatically add he following to the command line:
+And the following test:
 
 .. code-block:: python
 
-    >> pytest -m "(my_marker1 or my_marker2) and not (my_marker3 or my_marker4)"
+    @pytest.mark.marker1
+    @pytest.mark.marker2
+    def test_mytest():
+        assert True
+..
 
+This test is marked with *marker1* which is defined in the configuration, but also with *marker2* which is not. Therefore, despite being initially collected by pytest, this plugin will remove it from the selection.
 
 Contributing
 ------------
 Contributions are very welcome. Tests can be run with `tox`_, please ensure
 the coverage at least stays the same before you submit a pull request.
 
 License
```

### Comparing `pytest_himark-0.1.3/src/pytest_himark/plugin.py` & `pytest_himark-0.2.0/src/pytest_himark/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,33 @@
 import json
+import pytest
 
-markers_list = list()
+markers_list = set()
+
+
+@pytest.hookimpl(trylast=True)
+def pytest_collection_finish(session):
+    print(f"filtered: {len(session.items)} selected")
+
+
+@pytest.hookimpl(trylast=True)
+def pytest_collection_modifyitems(config, items):
+    option = config.getoption('-m')
+    if option is not None:
+        markers = option.replace("(", "").replace(")", "")
+        markers = list(filter(lambda x: x != '', markers.split(" or ")))
+
+        new_items = list()
+        for item in items:
+            for marker in item.iter_markers():
+                if marker.name not in markers:
+                    break
+            else:
+                new_items.append(item)
+        items[:] = new_items
 
 
 def pytest_addoption(parser):
     group = parser.getgroup("himark")
     group.addoption(
         '--json',
         action='store',
@@ -20,34 +43,47 @@
             "markers", f"{marker}: Enable if supported."
         )
         
 
 def pytest_load_initial_conftests(args):
     global markers_list
     json_path = None
-    markers_enabled = list()
-    markers_disabled = list()
+    markers_enabled = set()
 
     for arg in args:
         if arg.startswith("--json="):
             json_path = arg.replace("--json=", "")
 
     if json_path is not None:
         with open(json_path, "r") as file:
             config = json.load(file)
+            devices = config.get("devices", list())
             markers = config.get("markers", list())
 
+        # lists the enabled devices and turn them into markers
+        for device in devices:
+            name = device.get("name", None)
+            if device.get("used") is True:
+                markers_enabled.add(name)
+                # if device is enabled, check its do/di/ai/ao lists existence
+                for x in device.get("do", list()):
+                    markers_enabled.add(x)
+                for x in device.get("di", list()):
+                    markers_enabled.add(x)
+                for x in device.get("ai", list()):
+                    markers_enabled.add(x)
+                for x in device.get("ao", list()):
+                    markers_enabled.add(x)
+                # make a marker for 'type' key if it exists
+                if device.get("type", None) is not None:
+                    markers_enabled.add(device.get("type"))
+
         # lists the enabled markers
         for marker in markers:
             if markers.get(marker) is True:
-                markers_enabled.append(marker)
-            else:
-                markers_disabled.append(marker)
+                markers_enabled.add(marker)
 
-    markers_list = markers_enabled + markers_disabled
+    markers_enabled = set(filter(None, markers_enabled))
+    markers_list = markers_enabled
     # make an OR of the previously listed enabled markers and pass it with the -m option to the command line
     if len(markers_enabled) > 0:
-        args[:] = (["-m",
-                   (f'({" or ".join(markers_enabled)})' if len(markers_enabled) > 0 else '') +
-                   (' and ' if len(markers_enabled) > 0 and len(markers_disabled) > 0 else '') +
-                   (f'not ({" or ".join(markers_disabled)})' if len(markers_disabled) > 0 else '')]
-                   + args)
+        args[:] = (["-m", f'({" or ".join(markers_enabled)})'] + args)
```

### Comparing `pytest_himark-0.1.3/tests/test_himark.py` & `pytest_himark-0.2.0/tests/test_himark.py`

 * *Files 23% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         '*::test_marker3 PASSED*'
     )
 
     # make sure that we get a '0' exit code for the testsuite
     assert result.ret == 0
 
 
-def test_json_filte3(pytester):
+def test_json_filter3(pytester):
     """Check that tests that are marked with at least one disabled marker is not executed."""
 
     # create a temporary pytest test module
     pytester.makepyfile("""
         import pytest
         
         @pytest.mark.marker1
@@ -122,76 +122,120 @@
         '*::test_marker3 PASSED*'
     )
 
     # make sure that we get a '0' exit code for the testsuite
     assert result.ret == 0
 
 
-def test_json_filter_none(pytester):
-    """Check that all tests are executed when no json is used."""
+def test_json_filter_device(pytester):
+    """
+    Check that markers are correctly created from 'devices' in json, and properly filters out the test collection.
+    Markers 3, 4, 5 and 6 should be created since device1 and device2 have their 'used' key set to true in config.json.
+    device3 has 'used' set to false in config.json so marker7 and marker8 should not be created.
+    test_device2_type2 is marked by one marker that should be created, and one that shouldn't so it should not pass.
+
+    :param pytester: fixture
+    :return: None
+    """
 
     # create a temporary pytest test module
     pytester.makepyfile("""
         import pytest
-        
-        @pytest.mark.marker2
-        def test_marker1():
+
+        @pytest.mark.marker3
+        def test_device1_output1():
+            assert True
+
+        @pytest.mark.marker4
+        def test_device1_output2():
             assert True
             
-        @pytest.mark.marker1
-        def test_marker2():
+        @pytest.mark.marker5
+        def test_device2_input1():
             assert True
-        
-        def test_marker3():
+            
+        @pytest.mark.marker6
+        def test_device2_input2():
+            assert True
+            
+        @pytest.mark.marker7
+        def test_device3_output1():
+            assert True
+            
+        @pytest.mark.marker8
+        def test_device3_input1():
             assert True
+            
     """)
 
     # run pytest with the following cmd args
     result = pytester.runpytest(
+        f'--json={config_json}',
         '-vvv'
     )
 
     # fnmatch_lines does an assertion internally
     result.stdout.fnmatch_lines([
-        '*::test_marker1 PASSED*',
-        '*::test_marker2 PASSED*',
-        '*::test_marker3 PASSED*',
+        '*::test_device1_output1 PASSED*',
+        '*::test_device1_output2 PASSED*',
+        '*::test_device2_input1 PASSED*',
+        '*::test_device2_input2 PASSED*',
     ])
+    result.stdout.no_fnmatch_line(
+        '*::test_device3_output1 PASSED*',
+    )
+    result.stdout.no_fnmatch_line(
+        '*::test_device3_input1 PASSED*'
+    )
 
     # make sure that we get a '0' exit code for the testsuite
     assert result.ret == 0
 
 
-def test_json_filter_disabled(pytester):
-    """Check that all tests are executed when all markers are disabled."""
+def test_json_undefined_marker(pytester):
+    """
+    Check that collected tests with undefined markers are filtered out.
+    test_device2_type2 is marked by one marker that should be created, and one that shouldn't so it should not pass.
+
+    :param pytester: fixture
+    :return: None
+    """
 
     # create a temporary pytest test module
     pytester.makepyfile("""
         import pytest
+
+        @pytest.mark.type_device2
+        def test_device2_type1():
+            assert True
         
-        @pytest.mark.marker2
-        def test_marker1():
+        @pytest.mark.type_device2
+        @pytest.mark.type_device3
+        def test_device2_type2():
             assert True
             
-        @pytest.mark.marker1
-        def test_marker2():
-            assert True
-        
-        def test_marker3():
+        @pytest.mark.type_device3
+        def test_device3_output1():
             assert True
+            
     """)
 
     # run pytest with the following cmd args
     result = pytester.runpytest(
-        f'--json={config_disabled_json}',
+        f'--json={config_json}',
         '-vvv'
     )
 
     # fnmatch_lines does an assertion internally
     result.stdout.fnmatch_lines([
-        '*::test_marker1 PASSED*',
-        '*::test_marker2 PASSED*',
-        '*::test_marker3 PASSED*',
+        '*filtered: 1 selected*',
+        '*::test_device2_type1 PASSED*',
     ])
+    result.stdout.no_fnmatch_line(
+        '*::test_device2_type2 PASSED*'
+    )
+    result.stdout.no_fnmatch_line(
+        '*::test_device3_output1 PASSED*',
+    )
 
     # make sure that we get a '0' exit code for the testsuite
     assert result.ret == 0
```

