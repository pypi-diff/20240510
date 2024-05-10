# Comparing `tmp/ibm-apidocs-cli-0.9.0.tar.gz` & `tmp/ibm-apidocs-cli-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ibm-apidocs-cli-0.9.0.tar", last modified: Mon Aug  5 16:02:29 2019, max compression
+gzip compressed data, was "dist/ibm-apidocs-cli-0.9.1.tar", last modified: Fri Aug 30 15:37:19 2019, max compression
```

## Comparing `ibm-apidocs-cli-0.9.0.tar` & `ibm-apidocs-cli-0.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 16:02:29.000000 ibm-apidocs-cli-0.9.0/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 16:02:29.000000 ibm-apidocs-cli-0.9.0/ibm_apidocs_cli/
--rwxr-xr-x   0 travis    (2000) travis    (2000)      683 2019-08-05 16:00:27.000000 ibm-apidocs-cli-0.9.0/ibm_apidocs_cli/__init__.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)    18372 2019-08-05 16:00:27.000000 ibm-apidocs-cli-0.9.0/ibm_apidocs_cli/main.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)       37 2019-08-05 16:00:27.000000 ibm-apidocs-cli-0.9.0/ibm_apidocs_cli/version.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 16:02:29.000000 ibm-apidocs-cli-0.9.0/ibm_apidocs_cli.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     9461 2019-08-05 16:02:29.000000 ibm-apidocs-cli-0.9.0/ibm_apidocs_cli.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      397 2019-08-05 16:02:29.000000 ibm-apidocs-cli-0.9.0/ibm_apidocs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2019-08-05 16:02:29.000000 ibm-apidocs-cli-0.9.0/ibm_apidocs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       63 2019-08-05 16:02:29.000000 ibm-apidocs-cli-0.9.0/ibm_apidocs_cli.egg-info/entry_points.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       60 2019-08-05 16:02:29.000000 ibm-apidocs-cli-0.9.0/ibm_apidocs_cli.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       16 2019-08-05 16:02:29.000000 ibm-apidocs-cli-0.9.0/ibm_apidocs_cli.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2019-08-05 16:01:07.000000 ibm-apidocs-cli-0.9.0/ibm_apidocs_cli.egg-info/zip-safe
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 16:02:29.000000 ibm-apidocs-cli-0.9.0/test/
--rw-r--r--   0 travis    (2000) travis    (2000)     4824 2019-08-05 16:00:27.000000 ibm-apidocs-cli-0.9.0/test/test_main.py
--rwxr-xr-x   0 travis    (2000) travis    (2000)      125 2019-08-05 16:00:27.000000 ibm-apidocs-cli-0.9.0/MANIFEST.in
--rwxr-xr-x   0 travis    (2000) travis    (2000)     7011 2019-08-05 16:00:27.000000 ibm-apidocs-cli-0.9.0/README.md
--rwxr-xr-x   0 travis    (2000) travis    (2000)     2486 2019-08-05 16:00:27.000000 ibm-apidocs-cli-0.9.0/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     9461 2019-08-05 16:02:29.000000 ibm-apidocs-cli-0.9.0/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)       38 2019-08-05 16:02:29.000000 ibm-apidocs-cli-0.9.0/setup.cfg
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2019-08-30 15:37:19.000000 ibm-apidocs-cli-0.9.1/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2019-08-30 15:37:19.000000 ibm-apidocs-cli-0.9.1/ibm_apidocs_cli/
+-rwxr-xr-x   0 travis    (2000) travis    (2000)      683 2019-08-30 15:35:18.000000 ibm-apidocs-cli-0.9.1/ibm_apidocs_cli/__init__.py
+-rwxr-xr-x   0 travis    (2000) travis    (2000)    19908 2019-08-30 15:35:18.000000 ibm-apidocs-cli-0.9.1/ibm_apidocs_cli/main.py
+-rwxr-xr-x   0 travis    (2000) travis    (2000)       37 2019-08-30 15:35:18.000000 ibm-apidocs-cli-0.9.1/ibm_apidocs_cli/version.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2019-08-30 15:37:19.000000 ibm-apidocs-cli-0.9.1/ibm_apidocs_cli.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     9925 2019-08-30 15:37:19.000000 ibm-apidocs-cli-0.9.1/ibm_apidocs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)      397 2019-08-30 15:37:19.000000 ibm-apidocs-cli-0.9.1/ibm_apidocs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2019-08-30 15:37:19.000000 ibm-apidocs-cli-0.9.1/ibm_apidocs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       63 2019-08-30 15:37:19.000000 ibm-apidocs-cli-0.9.1/ibm_apidocs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       60 2019-08-30 15:37:19.000000 ibm-apidocs-cli-0.9.1/ibm_apidocs_cli.egg-info/requires.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       16 2019-08-30 15:37:19.000000 ibm-apidocs-cli-0.9.1/ibm_apidocs_cli.egg-info/top_level.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2019-08-30 15:35:57.000000 ibm-apidocs-cli-0.9.1/ibm_apidocs_cli.egg-info/zip-safe
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2019-08-30 15:37:19.000000 ibm-apidocs-cli-0.9.1/test/
+-rw-r--r--   0 travis    (2000) travis    (2000)     5115 2019-08-30 15:35:18.000000 ibm-apidocs-cli-0.9.1/test/test_main.py
+-rwxr-xr-x   0 travis    (2000) travis    (2000)      125 2019-08-30 15:35:18.000000 ibm-apidocs-cli-0.9.1/MANIFEST.in
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     7404 2019-08-30 15:35:18.000000 ibm-apidocs-cli-0.9.1/README.md
+-rwxr-xr-x   0 travis    (2000) travis    (2000)     2486 2019-08-30 15:35:18.000000 ibm-apidocs-cli-0.9.1/setup.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     9925 2019-08-30 15:37:19.000000 ibm-apidocs-cli-0.9.1/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)       38 2019-08-30 15:37:19.000000 ibm-apidocs-cli-0.9.1/setup.cfg
```

### Comparing `ibm-apidocs-cli-0.9.0/ibm_apidocs_cli/__init__.py` & `ibm-apidocs-cli-0.9.1/ibm_apidocs_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-apidocs-cli-0.9.0/ibm_apidocs_cli/main.py` & `ibm-apidocs-cli-0.9.1/ibm_apidocs_cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 from __future__ import print_function
 import os
 import argparse
+import base64
 import json
 import logging
 import requests
 import shutil
 import tempfile
 import subprocess
 from collections import OrderedDict
@@ -23,18 +24,18 @@
        argument parser
     """
     parser = argparse.ArgumentParser(description='Generate the apidocs files.')
     # required parameters
     requiredArgs = parser.add_argument_group('Required arguments')
     requiredArgs.add_argument(
         '-i', '--openapi', metavar='input-oas', help='Input OpenAPI specification file path or url', required=True)
-    requiredArgs.add_argument(
-        '-c', '--config', metavar='config-file', help='Name of front matter config file', required=True)
     # Optional parameters
     optionalArgs = parser._action_groups.pop()
+    parser.add_argument('-c', '--config', metavar='config-file', help='Name of front matter config file')
+    parser.add_argument('--mapfile', metavar='map-file', help='Path to mapping file')
     parser.add_argument('--apidocs', metavar='apidocs-dir', help='Path to apidocs repository containing config files. Default is current directory.')
     parser.add_argument('--templates', metavar='templates-dir', help='Path to directory containing custom front matter templates.')
     parser.add_argument('--output_folder', metavar='output-folder', help='Generated apidocs output folder')
     parser.add_argument('--frontmatter', metavar='frontmatter-cli', help='Frontmatter repository or local CLI')
     parser.add_argument('--sdk_generator', metavar='sdkgen-jar', help='Path to location of SDK generator JAR file')
     parser.add_argument('--sdkgen_release', metavar='sdkgen-release', help='Release of SDK generator to download')
     parser.add_argument('--keep_sdk', action='store_true', help='Keep generated SDK files')
@@ -66,20 +67,24 @@
 
     return args
 
 
 def main():
     parser = get_argument_parser()
     args = process_args(parser)
+
     temp_dir = tempfile.mkdtemp()
 
-    # Get the open api filename assistant-v2 from (./public/assistant-v2.json)
+    if not args.config:
+        mapping = get_mapping(args.mapfile)
+    else:
+        mapping = None
+
     openapi_abs = os.path.abspath(args.openapi)
     openapi_file = get_basename(args.openapi)
-    config_file = args.config
     frontmatter_cli = get_frontmatter_cli(args.frontmatter, temp_dir)
     sdk_generator_cli = get_sdk_generator_cli(args.sdk_generator, args.sdkgen_release, temp_dir)
     supported_languages = get_supported_languages(openapi_abs)
     templates_dir = get_frontmatter_templates(frontmatter_cli, args.templates)
 
     if args.output_folder:
         output_folder_abs = os.path.abspath(args.output_folder)
@@ -87,25 +92,22 @@
         output_folder_abs = os.getcwd()
 
     if args.apidocs:
         apidocs_dir = os.path.abspath(args.apidocs)
     else:
         apidocs_dir = os.getcwd()
 
-    if os.path.dirname(args.config) == '':
-        input_frontmatter_config = os.path.join(apidocs_dir, args.config)
-    else:
-        input_frontmatter_config = args.config
-    output_frontmatter_config = os.path.join(
-        output_folder_abs, os.path.basename(args.config))
+    input_frontmatter_config = get_config_file(args.config, openapi_file, apidocs_dir, mapping)
+
+    output_frontmatter_config = os.path.join(output_folder_abs, os.path.basename(input_frontmatter_config))
 
-    frontmatter_md_file = '%s/%s.md' % (output_folder_abs, openapi_file)
+    frontmatter_md_file = os.path.join(output_folder_abs, os.path.splitext(openapi_file)[0])+'.md'
 
     logger.info('openapi_file: %s' % openapi_file)
-    logger.info('config_file: %s' % config_file)
+    logger.info('config_file: %s' % input_frontmatter_config)
     logger.info('frontmatter_cli: %s' % frontmatter_cli)
     logger.info('sdk_generator_cli: %s' % sdk_generator_cli)
     logger.info('supported_languages: %s' % supported_languages)
     logger.info('templates_dir: %s' % templates_dir)
 
     if not os.path.exists(output_folder_abs):
         logger.info('Creating output directory %s' % output_folder_abs)
@@ -127,21 +129,56 @@
                                    openapi_file=openapi_abs, apidocs_folder=apidocs_dir, output_folder=output_folder_abs,
                                    keep_sdk=args.keep_sdk)
 
     if not args.keep_temp:
         logger.info('Removing temporary directory %s' % temp_dir)
         shutil.rmtree(temp_dir)
 
+def get_mapping(mapfile=None):
+    '''If required, loads the API definition mapping file from the specified location, or from GitHub.'''
+
+    if mapfile:
+        with open(mapfile) as f:
+            mapping = json.load(f)
+        logger.info('Loaded map file from %s' % mapfile)
+    else:
+        github_token = os.environ.get('GITHUB_TOKEN')
+        if not github_token:
+            raise ValueError('Cannot download map file without GitHub token. Either set GITHUB_TOKEN or specify local map file.')
+        mapfile_url = 'https://api.github.ibm.com/repos/Watson/developer-cloud--api-definitions/contents/generate-apidocs.json'
+        r = requests.get(mapfile_url,
+                         headers={'Authorization': 'token '+github_token})
+        r.raise_for_status()
+
+        mapping = json.loads(base64.b64decode(r.json()['content']).decode())
+
+        logger.info('Loaded map file from %s' % mapfile_url)
+
+    return mapping
+
+def get_config_file(config_file=None, openapi_file=None, apidocs_dir=None, mapping=None):
+    '''Get config file name either from command-line argument or from mapping file.'''
+
+    if not config_file:
+        config_filename = next(item for item in mapping['public']+mapping['private'] if item['openapi']==openapi_file)['config']
+        config_file = os.path.join(apidocs_dir, config_filename)
+        logger.info('Looked up config file: %s' % config_file)
+    
+    if os.path.dirname(config_file) == '':
+        config_file = os.path.join(apidocs_dir, config_file)
+
+    return config_file
+
 def get_basename(filepath):
     '''Returns the basename of the given filepath without the file extension'''
 
     if not filepath:
         raise ValueError('openapi file path cannot be null or empty')
     basename = os.path.basename(filepath)
-    return os.path.splitext(basename)[0]
+    return basename
 
 def get_frontmatter_cli(frontmatter, temp_dir):
     '''Returns the absolute path to the frontmatter app.js file
 
     Arguments:
       sdk_generator {String} -- The path to the app.js file or the folder where the app.js file is
       temp_dir {String} -- The path to the temp directory, used to clone the repo if necessary
@@ -168,15 +205,15 @@
                          '--prefix',
                          frontmatter])
 
     cli = os.path.join(os.path.abspath(frontmatter), 'app.js')
     logger.info('Using front-matter CLI at %s' % cli)
 
     if not os.path.exists(cli):
-       raise ValueError('Front-matter generator not found at %s.' % cli)
+        raise ValueError('Front-matter generator not found at %s.' % cli)
 
     return cli
 
 def get_frontmatter_templates(frontmatter_cli, templates):
     '''Returns the absolute path to the frontmatter templates to use.
 
     Arguments:
```

### Comparing `ibm-apidocs-cli-0.9.0/ibm_apidocs_cli.egg-info/PKG-INFO` & `ibm-apidocs-cli-0.9.1/ibm_apidocs_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ibm-apidocs-cli
-Version: 0.9.0
+Version: 0.9.1
 Summary: CLI library to automate the API Reference generation
 Home-page: https://cloud.ibm.com/apidocs
 Author: IBM Corp
 Author-email: germanatt@us.ibm.com
 License: MIT
 Description: ibm-apidocs-cli
         ===============
@@ -79,34 +79,36 @@
         ::
         
             ibm-apidocs-cli --help
         
         ::
         
             usage: ibm-apidocs-cli [-h] -i <openapi_file>
-                                   -c <config_file>
+                                   [--config <config_file>]
                                    [--sdk_generator <sdk_generator_path>]
                                    [--sdkgen_release <sdkgen_release>]
                                    [--frontmatter <frontmatter_path>]
                                    [--apidocs <apidocs_path>]
                                    [--templates <templates_path>]
                                    [--output_folder <output_path>]
                                    [--keep_sdk] [--keep_temp] [--verbose] [--version]
         
         Required arguments:
         
         -  ``-i <openapi_file>``: The path to the input OpenAPI definition file
            (e.g. ``assistant-v1.json``).
-        -  ``-c <config_file>``: The front matter config file (e.g.
-           ``assistant-v1-config.json``). You can optionally specify the full
-           path to the config file; if you do not include the path, the file is
-           assumed to be in the ``apidocs`` directory.
         
         Optional arguments:
         
+        -  ``--config <config_file>``: The front matter config file (e.g.
+           ``assistant-v1-config.json``). You can optionally specify the full
+           path to the config file; if you do not include the path, the file is
+           assumed to be in the ``apidocs`` directory. If you do not specify the
+           config file, the file name is looked up from the map file, and the
+           file is assumed to be in the ``apidocs`` directory.
         -  ``--sdk_generator <sdk_generator_path>``: Path to the directory
            containing the SDK generator JAR file, optionally including the file
            name. If you specify a directory but not a file name, the JAR file is
            assumed to be ``openapi-sdkgen.jar``. Use this option if you need to
            use local copy of the SDK generator, or if you do not have a GitHub
            access token configured. If you do not specify this parameter, the
            CLI will automatically download the the ``openapi-sdkgen.jar`` file
@@ -138,14 +140,18 @@
         -  ``--keep_temp``: Preserve the temporary directory containing the
            downloaded front-matter and SDK generators, if applicable. Useful for
            debugging purposes.
         -  ``--no_update``: Use front-matter config file as-is without updating
            SDK versions. If you do not specify this argument, the config file is
            updated with the latest GitHub release for each supported SDK
            language.
+        -  ``--mapfile``: The path to a local map file, including file name (for
+           example, ``generate-apidocs.json``). If you do not specify a local
+           map file, the current map file is downloaded from the
+           ``developer-cloud--api-definitions`` repo as needed.
         -  ``-h``, ``--help``: Show usage information and exit.
         -  ``--verbose``: Verbose flag.
         -  ``--version``: Show program's version number and exit.
         
         Example commands
         ~~~~~~~~~~~~~~~~
         
@@ -170,15 +176,15 @@
                             --output_folder '/Users/my_user/Documents/GitHub/api-apidocs-cli/test/target' \
                             --frontmatter '/Users/my_user/Documents/GitHub/frontmatter-generator' \
                             --sdk_generator '/Users/my_user/Documents/Release/openapi-sdkgen/lib'
         
         Python version
         --------------
         
-        ✅ Tested on Python 2.7, 3.4, 3.5, and 3.6.
+        ✅ Tested on Python 3.5, 3.6, and 3.7.
         
         Contributing
         ------------
         
         See `CONTRIBUTING.md <./CONTRIBUTING.md>`__.
         
         License
```

### Comparing `ibm-apidocs-cli-0.9.0/test/test_main.py` & `ibm-apidocs-cli-0.9.1/test/test_main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 # coding=utf-8
 
 import os
 import json
 import re
 import shutil
-from ibm_apidocs_cli.main import get_basename, get_frontmatter_cli, get_sdk_generator_cli, get_latest_sdk_version, create_frontmatter_config_file, create_frontmatter_md_file, create_language_specific_files, get_argument_parser, process_args
+from ibm_apidocs_cli.main import get_basename, get_mapping, get_config_file, get_frontmatter_cli, get_sdk_generator_cli, get_latest_sdk_version, create_frontmatter_config_file, create_frontmatter_md_file, create_language_specific_files, get_argument_parser, process_args
 
 def test_get_basename_from_file():
-    assert 'assistant-v1' == get_basename('/home/geman/public/assistant-v1.json')
-    assert 'assistant-v1' == get_basename('/assistant-v1.json')
-    assert 'assistant-v1' == get_basename('assistant-v1.json')
-    assert 'assistant-v1' == get_basename('/assistant-v1.txt')
+    assert 'assistant-v1.json' == get_basename('/home/geman/public/assistant-v1.json')
+    assert 'assistant-v1.json' == get_basename('/assistant-v1.json')
+    assert 'assistant-v1.json' == get_basename('assistant-v1.json')
     try:
       name = get_basename('')
       assert '%s should be None' % name
     except ValueError as identifier:
       pass
 
-def test_get_basename_from_url():
-    assert 'assistant-v1' == get_basename('https://raw.github.ibm.com/Watson/developer-cloud--api-definitions/master/apis-public/assistant-v1.json')
-    assert 'assistant-v1' == get_basename('https://ibm.com/assistant-v1.json')
+def test_get_mapping():
+    assert get_mapping('./test/resources/mapping/generate-apidocs.json')['name'] == 'api-mapping'
+    assert get_mapping(None)['name'] == 'api-mapping'    
+
+def test_get_config_file():
+    assert get_config_file('assistant-v1-config.json',
+                           'assistant-v1.json',
+                           './test/resources/apidocs',
+                           None) == './test/resources/apidocs/assistant-v1-config.json'
+    with open('./test/resources/mapping/generate-apidocs.json') as f:
+        mapping = json.load(f)
+    assert get_config_file(None,
+                           'assistant-v1.json',
+                           './test/resources/apidocs',
+                           mapping) == './test/resources/apidocs/assistant-v1-config.json'
 
 def test_get_frontmatter_cli():
   cli = get_frontmatter_cli('./test/resources/frontmatter/', '')
   assert cli is not None
   assert cli.endswith('/test/resources/frontmatter/app.js')
   
   cli = get_frontmatter_cli(frontmatter=None, temp_dir='./test/target/fm_temp')
   assert cli is not None
   assert cli.endswith('/test/target/fm_temp/frontmatter/app.js')
   assert os.path.isfile('./test/target/fm_temp/frontmatter/app.js')
   shutil.rmtree('./test/target/fm_temp')
 
-
 def test_get_sdk_generator_cli():
   cli = get_sdk_generator_cli(sdk_generator='./test/resources/sdk-generator/run.jar', sdkgen_release=None, temp_dir=None)
   assert cli is not None
   assert cli.endswith('/test/resources/sdk-generator/run.jar')
 
   cli = get_sdk_generator_cli(sdk_generator=None, sdkgen_release=None, temp_dir='./test/target')
   assert cli is not None
@@ -74,15 +84,14 @@
 def test_create_frontmatter_md_file():
   create_frontmatter_md_file('./test/resources/frontmatter/app.js', './test/resources/apidocs/personality-insights-v3.json',
     './test/target/personality-insights-v3-config.json', './test/target/personality-insights-v3.md')
 
 def test_create_language_specific_files():
   languages = ['java', 'node', 'python', 'ruby', 'go', 'swift']
   create_language_specific_files('./test/resources/sdk-generator/run.jar', languages, './test/resources/apidocs/personality-insights-v3.json', './test/resources/apidocs/', './test/target', True)
-  create_language_specific_files('./test/resources/sdk-generator/run.jar', languages, './test/resources/apidocs/personality-insights-v3.json', './test/resources/apidocs-missing-mapping/', './test/target', True)
   create_language_specific_files('./test/resources/sdk-generator/run.jar', languages, './test/resources/apidocs/personality-insights-v3.json', './test/resources/', './test/target', True)
 
 def test_main():
   result = os.system('ibm-apidocs-cli --openapi ./test/resources/apidocs/personality-insights-v3.json \
                                       --apidocs ./test/resources/apidocs \
                                       --config personality-insights-v3-config.json \
                                       --output_folder ./test/target \
```

### Comparing `ibm-apidocs-cli-0.9.0/README.md` & `ibm-apidocs-cli-0.9.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -44,40 +44,42 @@
 
 ```
 ibm-apidocs-cli --help
 ```
 
 ```
 usage: ibm-apidocs-cli [-h] -i <openapi_file>
-                       -c <config_file>
+                       [--config <config_file>]
                        [--sdk_generator <sdk_generator_path>]
                        [--sdkgen_release <sdkgen_release>]
                        [--frontmatter <frontmatter_path>]
                        [--apidocs <apidocs_path>]
                        [--templates <templates_path>]
                        [--output_folder <output_path>]
                        [--keep_sdk] [--keep_temp] [--verbose] [--version]
 ```
 
 Required arguments:
 
 - `-i <openapi_file>`: The path to the input OpenAPI definition file (e.g. `assistant-v1.json`).
-- `-c <config_file>`: The front matter config file (e.g. `assistant-v1-config.json`). You can optionally specify the full path to the config file; if you do not include the path, the file is assumed to be in the `apidocs` directory.
 
 Optional arguments:
 
+- `--config <config_file>`: The front matter config file (e.g. `assistant-v1-config.json`). You can optionally specify the full path to the config file; if you do not include the path, the file is assumed to be in the `apidocs` directory. If you do not specify the config file, the file name is looked up from the map file, and the file is assumed to be in the
+`apidocs` directory.
 - `--sdk_generator <sdk_generator_path>`: Path to the directory containing the SDK generator JAR file, optionally including the file name. If you specify a directory but not a file name, the JAR file is assumed to be `openapi-sdkgen.jar`. Use this option if you need to use local copy of the SDK generator, or if you do not have a GitHub access token configured. If you do not specify this parameter, the CLI will automatically download the the `openapi-sdkgen.jar` file to a temporary directory and use that copy.
 - `--sdkgen_release <sdkgen_release>`: Release of the SDK generator to download, if you are allowing the CLI to download the generator automatically. Specify the GitHub release tag (for example, `1.0.0.1`). If you do not specify a release, the most recent release (which might include breaking changes) is used. This argument is ignored if `--sdk_generator` is specified.
 - `--frontmatter <frontmatter_path>`: Path to the directory containing the front-matter generator `app.js` file. Use this option if you need to use a specific version or branch of the front-matter generator code, or if you do not have a GitHub access token configured. If you do not specify a location, the CLI will automatically clone the latest version of the front-matter generator repo to a temporary directory and use that clone.
 - `--apidocs <apidocs_path>`: The path to the `cloud-api-docs` repository or other directory containing `apiref-index.json` and front matter config file. If you do not specify this argument, the current directory is used.
 - `--templates <templates_path>`: Path to a directory containing custom front-matter templates.
 - `--output_folder <output_folder>`: The target directory for generated files. If you do not specify this argument, output files are written to the current directory.
 - `--keep_sdk`: Preserve the `_sdktemp` directory containing generated SDK artifacts. Useful for debugging purposes.
 - `--keep_temp`: Preserve the temporary directory containing the downloaded front-matter and SDK generators, if applicable. Useful for debugging purposes.
 - `--no_update`: Use front-matter config file as-is without updating SDK versions. If you do not specify this argument, the config file is updated with the latest GitHub release for each supported SDK language.
+- `--mapfile`: The path to a local map file, including file name (for example, `generate-apidocs.json`). If you do not specify a local map file, the current map file is downloaded from the `developer-cloud--api-definitions` repo as needed.
 - `-h`, `--help`: Show usage information and exit.
 - `--verbose`: Verbose flag.
 - `--version`: Show program's version number and exit.
 
 ### Example commands
 
 This example assumes that the command is being run from the `apidocs` repo directory containing the API Reference files, and that the CLI is automatically downloading and using the latest code for the front-matter and SDK generators. All output files are written to the current directory:
@@ -94,20 +96,21 @@
                 --output_folder '/Users/my_user/Documents/GitHub/api-apidocs-cli/test/target' \
                 --frontmatter '/Users/my_user/Documents/GitHub/frontmatter-generator' \
                 --sdk_generator '/Users/my_user/Documents/Release/openapi-sdkgen/lib'
 ```
 
 ## Python version
 
-✅ Tested on Python 2.7, 3.4, 3.5, and 3.6.
+✅ Tested on Python 3.5, 3.6, and 3.7.
 
 ## Contributing
 
 See [CONTRIBUTING.md][CONTRIBUTING].
 
+
 ## License
 
 MIT
 
 [ibm_cloud]: https://cloud.ibm.com
 [responses]: https://github.com/getsentry/responses
 [requests]: http://docs.python-requests.org/en/latest/
```

### Comparing `ibm-apidocs-cli-0.9.0/setup.py` & `ibm-apidocs-cli-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 from __future__ import print_function
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 # Convert README.md to README.rst for pypi
 try:
     from pypandoc import convert_file
 
     def read_md(f):
         return convert_file(f, 'rst')
```

### Comparing `ibm-apidocs-cli-0.9.0/PKG-INFO` & `ibm-apidocs-cli-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ibm-apidocs-cli
-Version: 0.9.0
+Version: 0.9.1
 Summary: CLI library to automate the API Reference generation
 Home-page: https://cloud.ibm.com/apidocs
 Author: IBM Corp
 Author-email: germanatt@us.ibm.com
 License: MIT
 Description: ibm-apidocs-cli
         ===============
@@ -79,34 +79,36 @@
         ::
         
             ibm-apidocs-cli --help
         
         ::
         
             usage: ibm-apidocs-cli [-h] -i <openapi_file>
-                                   -c <config_file>
+                                   [--config <config_file>]
                                    [--sdk_generator <sdk_generator_path>]
                                    [--sdkgen_release <sdkgen_release>]
                                    [--frontmatter <frontmatter_path>]
                                    [--apidocs <apidocs_path>]
                                    [--templates <templates_path>]
                                    [--output_folder <output_path>]
                                    [--keep_sdk] [--keep_temp] [--verbose] [--version]
         
         Required arguments:
         
         -  ``-i <openapi_file>``: The path to the input OpenAPI definition file
            (e.g. ``assistant-v1.json``).
-        -  ``-c <config_file>``: The front matter config file (e.g.
-           ``assistant-v1-config.json``). You can optionally specify the full
-           path to the config file; if you do not include the path, the file is
-           assumed to be in the ``apidocs`` directory.
         
         Optional arguments:
         
+        -  ``--config <config_file>``: The front matter config file (e.g.
+           ``assistant-v1-config.json``). You can optionally specify the full
+           path to the config file; if you do not include the path, the file is
+           assumed to be in the ``apidocs`` directory. If you do not specify the
+           config file, the file name is looked up from the map file, and the
+           file is assumed to be in the ``apidocs`` directory.
         -  ``--sdk_generator <sdk_generator_path>``: Path to the directory
            containing the SDK generator JAR file, optionally including the file
            name. If you specify a directory but not a file name, the JAR file is
            assumed to be ``openapi-sdkgen.jar``. Use this option if you need to
            use local copy of the SDK generator, or if you do not have a GitHub
            access token configured. If you do not specify this parameter, the
            CLI will automatically download the the ``openapi-sdkgen.jar`` file
@@ -138,14 +140,18 @@
         -  ``--keep_temp``: Preserve the temporary directory containing the
            downloaded front-matter and SDK generators, if applicable. Useful for
            debugging purposes.
         -  ``--no_update``: Use front-matter config file as-is without updating
            SDK versions. If you do not specify this argument, the config file is
            updated with the latest GitHub release for each supported SDK
            language.
+        -  ``--mapfile``: The path to a local map file, including file name (for
+           example, ``generate-apidocs.json``). If you do not specify a local
+           map file, the current map file is downloaded from the
+           ``developer-cloud--api-definitions`` repo as needed.
         -  ``-h``, ``--help``: Show usage information and exit.
         -  ``--verbose``: Verbose flag.
         -  ``--version``: Show program's version number and exit.
         
         Example commands
         ~~~~~~~~~~~~~~~~
         
@@ -170,15 +176,15 @@
                             --output_folder '/Users/my_user/Documents/GitHub/api-apidocs-cli/test/target' \
                             --frontmatter '/Users/my_user/Documents/GitHub/frontmatter-generator' \
                             --sdk_generator '/Users/my_user/Documents/Release/openapi-sdkgen/lib'
         
         Python version
         --------------
         
-        ✅ Tested on Python 2.7, 3.4, 3.5, and 3.6.
+        ✅ Tested on Python 3.5, 3.6, and 3.7.
         
         Contributing
         ------------
         
         See `CONTRIBUTING.md <./CONTRIBUTING.md>`__.
         
         License
```

