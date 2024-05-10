# Comparing `tmp/snipinator-1.4.0.tar.gz` & `tmp/snipinator-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/gdrive/code/snipinator.develop/develop/dist/.tmp-89aqwtpv/snipinator-1.4.0.tar", last modified: Tue Apr 30 19:05:23 2024, max compression
+gzip compressed data, was "/mnt/c/gdrive/code/snipinator.develop/develop/dist/.tmp-2k7bney2/snipinator-1.4.1.tar", last modified: Fri May 10 14:17:38 2024, max compression
```

## Comparing `snipinator-1.4.0.tar` & `snipinator-1.4.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-30 19:05:23.823352 snipinator-1.4.0/
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-04-30 19:04:32.000000 snipinator-1.4.0/LICENSE.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)    45946 2024-04-30 19:05:23.813512 snipinator-1.4.0/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)    38974 2024-04-30 19:04:32.000000 snipinator-1.4.0/README.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)     4199 2024-04-30 19:04:32.000000 snipinator-1.4.0/pyproject.toml
--rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-04-30 19:05:23.823352 snipinator-1.4.0/setup.cfg
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-30 19:05:23.681312 snipinator-1.4.0/snipinator/
--rwxrwxrwx   0 realz     (1000) realz     (1000)      514 2024-03-27 14:51:50.000000 snipinator-1.4.0/snipinator/__init__.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    18915 2024-04-26 18:29:05.000000 snipinator-1.4.0/snipinator/cli.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    34778 2024-04-30 19:04:32.000000 snipinator-1.4.0/snipinator/snipinate.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)      866 2024-03-21 17:40:02.000000 snipinator-1.4.0/snipinator/snipinate_test.py
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-30 19:05:23.797223 snipinator-1.4.0/snipinator.egg-info/
--rwxrwxrwx   0 realz     (1000) realz     (1000)    45946 2024-04-30 19:05:23.000000 snipinator-1.4.0/snipinator.egg-info/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)      335 2024-04-30 19:05:23.000000 snipinator-1.4.0/snipinator.egg-info/SOURCES.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-04-30 19:05:23.000000 snipinator-1.4.0/snipinator.egg-info/dependency_links.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       51 2024-04-30 19:05:23.000000 snipinator-1.4.0/snipinator.egg-info/entry_points.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1820 2024-04-30 19:05:23.000000 snipinator-1.4.0/snipinator.egg-info/requires.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       11 2024-04-30 19:05:23.000000 snipinator-1.4.0/snipinator.egg-info/top_level.txt
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-10 14:17:38.692166 snipinator-1.4.1/
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-10 14:17:38.539989 snipinator-1.4.1/.github/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    40430 2024-05-10 14:16:48.000000 snipinator-1.4.1/.github/README.remotified.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-04-30 19:04:32.000000 snipinator-1.4.1/LICENSE.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    47823 2024-05-10 14:17:38.687119 snipinator-1.4.1/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    38860 2024-05-10 14:16:48.000000 snipinator-1.4.1/README.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     4431 2024-05-10 14:16:48.000000 snipinator-1.4.1/pyproject.toml
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-05-10 14:17:38.693158 snipinator-1.4.1/setup.cfg
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-10 14:17:38.587860 snipinator-1.4.1/snipinator/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      514 2024-03-27 14:51:50.000000 snipinator-1.4.1/snipinator/__init__.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    18915 2024-04-26 18:29:05.000000 snipinator-1.4.1/snipinator/cli.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    34778 2024-04-30 19:04:32.000000 snipinator-1.4.1/snipinator/snipinate.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      866 2024-03-21 17:40:02.000000 snipinator-1.4.1/snipinator/snipinate_test.py
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-05-10 14:17:38.672675 snipinator-1.4.1/snipinator.egg-info/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    47823 2024-05-10 14:17:38.000000 snipinator-1.4.1/snipinator.egg-info/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      364 2024-05-10 14:17:38.000000 snipinator-1.4.1/snipinator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-05-10 14:17:38.000000 snipinator-1.4.1/snipinator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       51 2024-05-10 14:17:38.000000 snipinator-1.4.1/snipinator.egg-info/entry_points.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1993 2024-05-10 14:17:38.000000 snipinator-1.4.1/snipinator.egg-info/requires.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       11 2024-05-10 14:17:38.000000 snipinator-1.4.1/snipinator.egg-info/top_level.txt
```

### Comparing `snipinator-1.4.0/LICENSE.md` & `snipinator-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `snipinator-1.4.0/PKG-INFO` & `snipinator-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snipinator
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python code snippets for markdown files, e.g READMEs, from actual (testable) code.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -64,14 +64,16 @@
 Requires-Dist: rich==13.7.1; extra == "prod"
 Requires-Dist: rich-argparse==1.4.0; extra == "prod"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "prod"
 Requires-Dist: typing-extensions==4.10.0; extra == "prod"
 Provides-Extra: dev
 Requires-Dist: argcomplete==3.2.3; extra == "dev"
 Requires-Dist: autoflake==2.3.1; extra == "dev"
+Requires-Dist: beautifulsoup4==4.12.3; extra == "dev"
+Requires-Dist: bs4==0.0.2; extra == "dev"
 Requires-Dist: build==1.0.3; extra == "dev"
 Requires-Dist: certifi==2024.2.2; extra == "dev"
 Requires-Dist: cffi==1.16.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
 Requires-Dist: changeguard==0.3.1; extra == "dev"
 Requires-Dist: charset-normalizer==3.3.2; extra == "dev"
 Requires-Dist: click==8.1.7; extra == "dev"
@@ -92,15 +94,18 @@
 Requires-Dist: keyring==24.3.1; extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; extra == "dev"
 Requires-Dist: markupsafe==2.1.5; extra == "dev"
 Requires-Dist: mdformat==0.7.17; extra == "dev"
 Requires-Dist: mdformat-gfm==0.3.0; extra == "dev"
 Requires-Dist: mdformat-tables==0.4.1; extra == "dev"
 Requires-Dist: mdit-py-plugins==0.4.0; extra == "dev"
+Requires-Dist: mdreftidy==0.3.0; extra == "dev"
+Requires-Dist: mdremotifier==0.3.1; extra == "dev"
 Requires-Dist: mdurl==0.1.2; extra == "dev"
+Requires-Dist: mistletoe==1.3.0; extra == "dev"
 Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
 Requires-Dist: nh3==0.2.15; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
 Requires-Dist: packaging==23.2; extra == "dev"
 Requires-Dist: pathspec==0.12.1; extra == "dev"
@@ -121,19 +126,22 @@
 Requires-Dist: readme-renderer==43.0; extra == "dev"
 Requires-Dist: requests==2.31.0; extra == "dev"
 Requires-Dist: requests-toolbelt==1.0.0; extra == "dev"
 Requires-Dist: rfc3986==2.0.0; extra == "dev"
 Requires-Dist: rich==13.7.1; extra == "dev"
 Requires-Dist: rich-argparse==1.4.0; extra == "dev"
 Requires-Dist: secretstorage==3.3.3; extra == "dev"
+Requires-Dist: soupsieve==2.5; extra == "dev"
 Requires-Dist: toml-sort==0.23.1; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
 Requires-Dist: tomlkit==0.12.4; extra == "dev"
 Requires-Dist: twine==5.0.0; extra == "dev"
+Requires-Dist: types-beautifulsoup4==4.12.0.20240229; extra == "dev"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "dev"
+Requires-Dist: types-html5lib==1.1.11.20240228; extra == "dev"
 Requires-Dist: types-pyyaml==6.0.12.20240311; extra == "dev"
 Requires-Dist: typing-extensions==4.10.0; extra == "dev"
 Requires-Dist: urllib3==2.2.1; extra == "dev"
 Requires-Dist: virtualenv==20.25.0; extra == "dev"
 Requires-Dist: wcwidth==0.2.13; extra == "dev"
 Requires-Dist: wheel==0.43.0; extra == "dev"
 Requires-Dist: xmltodict==0.13.0; extra == "dev"
@@ -153,22 +161,22 @@
 
 
 
 
 
 -->
 
-# <div align="center">[![Snipinator][22]][56]</div>
+# <div align="center">[![Snipinator][1]][2]</div>
 
 <div align="center">
 
 <!-- Icons from https://lucide.dev/icons/users -->
 <!-- Icons from https://lucide.dev/icons/laptop-minimal -->
 
-![**Audience:** Developers][19] ![**Platform:** Linux][20]
+![**Audience:** Developers][3] ![**Platform:** Linux][4]
 
 </div>
 
 <p align="center">
   <strong>
     <a href="https://github.com/realazthat/snipinator">🏠Home</a>
     &nbsp;&bull;&nbsp;
@@ -191,40 +199,40 @@
     &nbsp;&bull;&nbsp;
     <a href="#-gotchas-and-limitations">🚸Gotchas</a>
   </strong>
 </p>
 
 <div align="center">
 
-![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
-[![Python Version][8]][5]
+![Top language][5] [![GitHub License][6]][7] [![PyPI - Version][8]][9]
+[![Python Version][10]][9]
 
 **CLI to embed (testable) snippets from your codebase into your README**
 
 </div>
 
 ---
 
 <div align="center">
 
-|                   | Status                     | Stable                    | Unstable                  |                    |
-| ----------------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
-| **[Master][17]**  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
-| **[Develop][18]** | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+|                   | Status                      | Stable                    | Unstable                  |                    |
+| ----------------- | --------------------------- | ------------------------- | ------------------------- | ------------------ |
+| **[Master][11]**  | [![Build and Test][12]][13] | [![since tagged][14]][15] |                           | ![last commit][16] |
+| **[Develop][17]** | [![Build and Test][18]][13] | [![since tagged][19]][20] | [![since tagged][21]][22] | ![last commit][23] |
 
 </div>
 
-<img src=".github/demo.gif" alt="Demo" width="100%">
+<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/snipinator/v1.4.1/.github/demo.gif" width="100%"/>
 
 ## ❔ What
 
 What it does: **Snipinator** lets you take a `EXAMPLE.md` template
 and include snippets from your (working and tested) codebase.
 
-Turn this ([./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2)):
+Turn this ([./snipinator/examples/EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/EXAMPLE.md.jinja2)):
 
 <!---->
 ```md
 # A README
 
 Here is a code snippet:
 
@@ -232,15 +240,15 @@
 
 Note that `code.py` has a test:
 {{path('./snipinator/examples/code_test.py', link='md')}}.
 
 ```
 <!---->
 
-Into this ([./snipinator/examples/EXAMPLE.generated.md](./snipinator/examples/EXAMPLE.generated.md)):
+Into this ([./snipinator/examples/EXAMPLE.generated.md](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/EXAMPLE.generated.md)):
 
 <!---->
 ````md
 <!--
 
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `snipinator/examples/EXAMPLE.md.jinja2`.
@@ -290,21 +298,21 @@
 ## 🔨 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/snipinator/)
 pip install snipinator
 
 # Install from git (https://github.com/realazthat/snipinator)
-pip install git+https://github.com/realazthat/snipinator.git@v1.4.0
+pip install git+https://github.com/realazthat/snipinator.git@v1.4.1
 ```
 
 ## 🚜 Usage
 
 Example template README:
-([./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2)):
+([./snipinator/examples/EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/EXAMPLE.md.jinja2)):
 
 <!---->
 ```md
 # A README
 
 Here is a code snippet:
 
@@ -350,35 +358,35 @@
 
 ````
 <!---->
 
 ## 💻 Command Line Options
 
 <!---->
-<img src="README.help.generated.svg" alt="Output of `python -m snipinator.cli --help`" />
-<!---->
+<img alt="Output of `python -m snipinator.cli --help`" src="https://raw.githubusercontent.com/realazthat/snipinator/v1.4.1/README.help.generated.svg"/>
+<!-- -->
 
 ## 💡 Examples
 
 - Snipinator's own `README`:
-  - Template: [./README.md.jinja2](./README.md.jinja2).
-  - Generated: [./README.md](./README.md).
-  - Generation script: [./scripts/generate-readme.sh](./scripts/generate-readme.sh).
+  - Template: [./README.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md.jinja2).
+  - Generated: [./README.md](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md).
+  - Generation script: [./scripts/generate-readme.sh](https://github.com/realazthat/snipinator/blob/v1.4.1/scripts/generate-readme.sh).
 - Example:
-  - Template: [./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2).
+  - Template: [./snipinator/examples/EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/EXAMPLE.md.jinja2).
   - Generated:
-    [./snipinator/examples/EXAMPLE.generated.md](./snipinator/examples/EXAMPLE.generated.md).
-  - Generation script: [./snipinator/examples/example.sh](./snipinator/examples/example.sh).
+    [./snipinator/examples/EXAMPLE.generated.md](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/EXAMPLE.generated.md).
+  - Generation script: [./snipinator/examples/example.sh](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/example.sh).
 - Long example of many features:
   - Template:
-    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
+    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/LONG-EXAMPLE.md.jinja2).
   - Generated:
-    [./snipinator/examples/LONG-EXAMPLE.generated.md](./snipinator/examples/LONG-EXAMPLE.generated.md).
+    [./snipinator/examples/LONG-EXAMPLE.generated.md](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/LONG-EXAMPLE.generated.md).
   - Generation script:
-    [./snipinator/examples/long-example.sh](./snipinator/examples/long-example.sh).
+    [./snipinator/examples/long-example.sh](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/long-example.sh).
 - Projects using Snipinator:
   - [realazthat/snipinator](https://github.com/realazthat/snipinator), See
     [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
   - [realazthat/changeguard](https://github.com/realazthat/changeguard), See
     [changeguard/README.md.jinja2](https://github.com/realazthat/changeguard/blob/87d5104b52e651bb9195a3d46dd7f050acbcb534/README.md.jinja2).
   - [realazthat/comfy-catapult](https://github.com/realazthat/comfy-catapult),
     See
@@ -395,15 +403,15 @@
 [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
 Additional (Jinja2) functions made available:
 
 ### 🐍✂ pysnippet
 
 Used several times in
-[./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
+[./snipinator/examples/LONG-EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/LONG-EXAMPLE.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def pysnippet(path: str,
               symbol: Optional[str],
@@ -441,15 +449,15 @@
       Union[str, markupsafe.Markup]: The snippet.
   """
 ```
 <!---->
 
 ### 🐍📖 pysignature
 
-Used several times in [./README.md.jinja2](./README.md.jinja2).
+Used several times in [./README.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def pysignature(path: str,
                 symbol: str,
@@ -488,15 +496,15 @@
       str: The signature and docstring.
   """
 ```
 <!---->
 
 ### ✂ rawsnippet
 
-Used several times in [./README.md.jinja2](./README.md.jinja2).
+Used several times in [./README.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def rawsnippet(path: str,
                *,
@@ -532,15 +540,15 @@
   """
 
 ```
 <!---->
 
 ### ✂ snippet
 
-Example in [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
+Example in [./snipinator/examples/LONG-EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/LONG-EXAMPLE.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def snippet(path: str,
             start: str,
@@ -582,15 +590,15 @@
   """
 
 ```
 <!---->
 
 ### 🐚 shell
 
-Used several times in [./README.md.jinja2](./README.md.jinja2).
+Used several times in [./README.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def shell(args: str,
           *,
@@ -678,15 +686,15 @@
       Union[str, markupsafe.Markup]: Returns the output of the command.
   """
 ```
 <!---->
 
 ### 🌀 path
 
-Used several times in [./README.md.jinja2](./README.md.jinja2).
+Used several times in [./README.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def path(path: str,
          *,
@@ -742,15 +750,15 @@
 - Python 3.8+
   - Why: Some dev dependencies require Python 3.8+.
 
 ### Tested Platforms
 
 - WSL2 Ubuntu 20.04, Python `3.8.0`.
 - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions
-  workflow ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
+  workflow ([build-and-test.yml](https://github.com/realazthat/snipinator/blob/v1.4.1/.github/workflows/build-and-test.yml)).
 
 ## 🚸 Gotchas and Limitations
 
 - **Security:** This tool is NOT designed to be used with untrusted input. It is
   designed to be used with your own codebase. Even when using your own input, be
   careful that your own code won't be doing anything that might inadvertently
   include untrusted input.
@@ -772,15 +780,15 @@
   ` ````language ```My Snippet``` ```` ` and this is a method that Markdown uses
   to allow embedded backticks inside a code block.
 - Formatting: The `{{` `}}` used to
   surround the snippet calls will unfortunately be formatted by a Markdown
   formatter and make the call invalid. Workarounds:
   - **Decommentify**: Put the snippet call inside a HTML comment, then use
     `decommentify` parameter. See
-    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2) for
+    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/LONG-EXAMPLE.md.jinja2) for
     examples.
   - [prettier](https://prettier.io/) formatter is pretty good at leaving the
     Jinja2 calls alone, especially if you don't have any spaces. This especially
     helps for markdown "reference-style links" that have Jinja2 calls in them
     generating part of the URL, mdformat will URL encode the Jinja2 calls,
     and/or split them on spaces, which is not what we want. prettier will leave
     them alone.
@@ -806,15 +814,15 @@
 
 We use SemVer for versioning. For the versions available, see the tags on this
 repository.
 
 ## 🔑 License
 
 This project is licensed under the MIT License - see the
-[./LICENSE.md](./LICENSE.md) file for details.
+[./LICENSE.md](https://github.com/realazthat/snipinator/blob/v1.4.1/LICENSE.md) file for details.
 
 ## 🙏 Thanks
 
 Main libraries used in Snipinator are:
 
 - Templating: [Jinja2](https://github.com/pallets/jinja).
 - Snippet inclusion: Python's AST library.
@@ -826,98 +834,98 @@
 ## 🤝 Related Projects
 
 Not complete, and not necessarily up to date. Make a PR
 ([contributions](#-contributions)) to insert/modify.
 
 | Project                                                           | Stars     | Last Update  | Language   | Platform         | Similarity X Obviousness |
 | ----------------------------------------------------------------- | --------- | ------------ | ---------- | ---------------- | ------------------------ |
-| [mdx-js/mdx][54]                                                  | 16.8k     | `2024/04/17` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [zakhenry/embedme][24]                                            | 222       | `2023/11/08` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [cmacmackin/markdown-include][53]                                 | 95        | `2023/02/07` | Python     | N/A              | ⭐⭐⭐⭐⭐               |
-| [SimonCropp/MarkdownSnippets][31]                                 | 23        | `2024/04/23` | .NET       | N/A              | ⭐⭐⭐⭐⭐               |
-| [endocode/snippetextractor][41]                                   | 4         | `2014/08/16` | C++        | N/A              | ⭐⭐⭐⭐⭐               |
-| [polywrap/doc-snippets][45]                                       | 3         | `2023/09/26` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [JulianCataldo/remark-embed][34]                                  | 2         | `2022/09/22` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [xrd/oreilly-snippets][47]                                        | 2         | `2015/10/15` | Ruby       | N/A              | ⭐⭐⭐⭐⭐               |
-| [DamonOehlman/injectcode][48]                                     | 1         | `2021/08/01` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [electrovir/markdown-code-example-inserter][25]                   | 1         | `2024/02/19` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets][46] | 1         | `2021/02/12` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [ildar-shaimordanov/git-markdown-snippet][36]                     | 0         | `2021/09/14` | Perl       | N/A              | ⭐⭐⭐⭐⭐               |
-| [teyc/markdown-snippet][50]                                       | 0         | `2024/01/22` | Powershell | N/A              | ⭐⭐⭐⭐⭐               |
-| [marc-bouvier-graveyard/baldir_markdown][51]                      | 0         | `2020/06/15` | Python     | N/A              | ⭐⭐⭐⭐⭐               |
-| [dineshsonachalam/markdown-autodocs][26]                          | 176       | `2022/09/19` | JS         | GH Action        | ⭐⭐⭐⭐                 |
-| [tokusumi/markdown-embed-code][29]                                | 28        | `2022/01/05` | Python     | VSCode Extension | ⭐⭐⭐⭐                 |
-| [sammndhr/gridsome-remark-embed-snippet][37]                      | 2         | `2021/06/14` | JS         | [Gridsome][38]   | ⭐⭐⭐⭐                 |
-| [NativeScript/markdown-snippet-injector][44]                      | 4         | `2019/01/24` | JS         | N/A              | ⭐⭐⭐⭐                 |
-| [fuxingloh/remark-code-import-replace][49]                        | 0         | `2022/12/21` | JS         | Remark?          | ⭐⭐⭐⭐                 |
-| [szkiba/mdcode][55]                                               | 15        | `2014/02/12` | Go         | N/A              | ⭐⭐⭐                   |
-| [devincornell/pymddoc][43]                                        | 0         | `2023/12/01` | Python     | Python           | ⭐⭐⭐                   |
-| [shiftkey/scribble][32] ([docs][33])                              | 40        | `2013/08/08` | .NET       | N/A              | ⭐⭐                     |
-| [calebpeterson/jest-transformer-test-md][35]                      | 2         | `2020/08/21` | JS         | Jest Tests       | ⭐⭐                     |
-| [tjstankus/commitate][52]                                         | 0         | `2014/05/29` | Ruby       | N/A              | ⭐                       |
-| [GitHub Docs: Creating a permanent link to a code snippet][23]    | N/A       | N/A          | N/A        | N/A              | ⭐                       |
-| [javierfernandes/markdown-exercises][42]                          | 1         | `2017/05/01` | JS         | N/A              | ⭐                       |
-| [gatsby-remark-embed-snippet][39]                                 | N/A (55k) | `2024/01/23` | JS         | [Gatsby][40]     | ⭐                       |
-| [ARMmbed/snippet][30]                                             | 6         | `2021/08/05` | Python     | N/A              | ?                        |
-| [drewavis/markdowninclude][28]                                    | 1         | `2024/04/06` | JS         | VSCode Extension | ?                        |
-| [romnn/embedme][27]                                               | 0         | `2024/04/18` | Go         | N/A              | ?                        |
+| [mdx-js/mdx][24]                                                  | 16.8k     | `2024/04/17` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [zakhenry/embedme][25]                                            | 222       | `2023/11/08` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [cmacmackin/markdown-include][26]                                 | 95        | `2023/02/07` | Python     | N/A              | ⭐⭐⭐⭐⭐                    |
+| [SimonCropp/MarkdownSnippets][27]                                 | 23        | `2024/04/23` | .NET       | N/A              | ⭐⭐⭐⭐⭐                    |
+| [endocode/snippetextractor][28]                                   | 4         | `2014/08/16` | C++        | N/A              | ⭐⭐⭐⭐⭐                    |
+| [polywrap/doc-snippets][29]                                       | 3         | `2023/09/26` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [JulianCataldo/remark-embed][30]                                  | 2         | `2022/09/22` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [xrd/oreilly-snippets][31]                                        | 2         | `2015/10/15` | Ruby       | N/A              | ⭐⭐⭐⭐⭐                    |
+| [DamonOehlman/injectcode][32]                                     | 1         | `2021/08/01` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [electrovir/markdown-code-example-inserter][33]                   | 1         | `2024/02/19` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets][34] | 1         | `2021/02/12` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [ildar-shaimordanov/git-markdown-snippet][35]                     | 0         | `2021/09/14` | Perl       | N/A              | ⭐⭐⭐⭐⭐                    |
+| [teyc/markdown-snippet][36]                                       | 0         | `2024/01/22` | Powershell | N/A              | ⭐⭐⭐⭐⭐                    |
+| [marc-bouvier-graveyard/baldir_markdown][37]                      | 0         | `2020/06/15` | Python     | N/A              | ⭐⭐⭐⭐⭐                    |
+| [dineshsonachalam/markdown-autodocs][38]                          | 176       | `2022/09/19` | JS         | GH Action        | ⭐⭐⭐⭐                     |
+| [tokusumi/markdown-embed-code][39]                                | 28        | `2022/01/05` | Python     | VSCode Extension | ⭐⭐⭐⭐                     |
+| [sammndhr/gridsome-remark-embed-snippet][40]                      | 2         | `2021/06/14` | JS         | [Gridsome][41]   | ⭐⭐⭐⭐                     |
+| [NativeScript/markdown-snippet-injector][42]                      | 4         | `2019/01/24` | JS         | N/A              | ⭐⭐⭐⭐                     |
+| [fuxingloh/remark-code-import-replace][43]                        | 0         | `2022/12/21` | JS         | Remark?          | ⭐⭐⭐⭐                     |
+| [szkiba/mdcode][44]                                               | 15        | `2014/02/12` | Go         | N/A              | ⭐⭐⭐                      |
+| [devincornell/pymddoc][45]                                        | 0         | `2023/12/01` | Python     | Python           | ⭐⭐⭐                      |
+| [shiftkey/scribble][46] ([docs][47])                              | 40        | `2013/08/08` | .NET       | N/A              | ⭐⭐                       |
+| [calebpeterson/jest-transformer-test-md][48]                      | 2         | `2020/08/21` | JS         | Jest Tests       | ⭐⭐                       |
+| [tjstankus/commitate][49]                                         | 0         | `2014/05/29` | Ruby       | N/A              | ⭐                        |
+| [GitHub Docs: Creating a permanent link to a code snippet][50]    | N/A       | N/A          | N/A        | N/A              | ⭐                        |
+| [javierfernandes/markdown-exercises][51]                          | 1         | `2017/05/01` | JS         | N/A              | ⭐                        |
+| [gatsby-remark-embed-snippet][52]                                 | N/A (55k) | `2024/01/23` | JS         | [Gatsby][53]     | ⭐                        |
+| [ARMmbed/snippet][54]                                             | 6         | `2021/08/05` | Python     | N/A              | ?                        |
+| [drewavis/markdowninclude][55]                                    | 1         | `2024/04/06` | JS         | VSCode Extension | ?                        |
+| [romnn/embedme][56]                                               | 0         | `2024/04/18` | Go         | N/A              | ?                        |
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
 
-  - From [./.github/dependencies.yml](./.github/dependencies.yml), which is used for
+  - From [./.github/dependencies.yml](https://github.com/realazthat/snipinator/blob/v1.4.1/.github/dependencies.yml), which is used for
     the GH Action to do a fresh install of everything:
 
     ```yaml
     bash: scripts.
     findutils: scripts.
     grep: tests.
     xxd: tests.
     git: scripts, tests.
     xxhash: scripts (changeguard).
     rsync: out-of-directory test.
     expect: for `unbuffer`, useful to grab and compare ansi color symbols.
     jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
       the README; the README generator needs to use `tomlq` (which is a part of `yq`)
       to query `pyproject.toml`.
-    
+
     ```
 
   - Requires `pyenv`, or an exact matching version of python as in
-    [.python-version](.python-version) (which is currently
+    [.python-version](https://github.com/realazthat/snipinator/blob/v1.4.1/.python-version) (which is currently
     `3.8.0`).
   - act (to run the GH Action locally):
     - Requires nodejs.
     - Requires Go.
     - docker.
   - Generate animation:
     - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
 4. `git status` check if anything changed (generated
-   [./README.md](./README.md) for example), if so, `git add` the
+   [./README.md](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md) for example), if so, `git add` the
    changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## 🔄🚀 Release Process
 
 These instructions are for maintainers of the project.
 
 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
 2. In the `develop` branch, bump the version in
-   [./pyproject.toml](./pyproject.toml), following semantic versioning
+   [./pyproject.toml](https://github.com/realazthat/snipinator/blob/v1.4.1/pyproject.toml), following semantic versioning
    principles. Also modify the `last_unstable_release` and `last_stable_release`
    in the `[tool.snipinator-project-metadata]` table as appropriate. Run
    `bash ./scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
@@ -929,92 +937,63 @@
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
-[1]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=master&style=plastic
-[2]:
-  https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
-[3]:
-  https://img.shields.io/github/license/realazthat/snipinator?style=plastic&color=0A1E1E
-[4]:
-  https://img.shields.io/pypi/v/snipinator?style=plastic&color=0A1E1E
-[5]: https://pypi.org/project/snipinator/
-[6]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/master?style=plastic
-[7]:
-  https://img.shields.io/github/last-commit/realazthat/snipinator/master?style=plastic
-[8]:
-  https://img.shields.io/pypi/pyversions/snipinator?style=plastic&color=0A1E1E
-[9]:
-  https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
-[10]:
-  https://github.com/realazthat/snipinator/compare/v1.4.0...master
-[11]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=develop&style=plastic
-[12]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/develop?style=plastic
-[13]:
-  https://github.com/realazthat/snipinator/compare/v1.4.0...develop
-[14]:
-  https://img.shields.io/github/last-commit/realazthat/snipinator/develop?style=plastic
-[15]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/develop?style=plastic
-[16]:
-  https://github.com/realazthat/snipinator/compare/v1.4.0...develop
-[17]: https://github.com/realazthat/snipinator/tree/master
-[18]: https://github.com/realazthat/snipinator/tree/develop
-
-<!-- Logo from https://lucide.dev/icons/users -->
-
-[19]:
-  https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
-
-<!-- Logo from https://lucide.dev/icons/laptop-minimal -->
-
-[20]:
-  https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
-[21]: ./LICENSE.md
-[22]: ./.github/logo-exported.svg
-[23]:
-  https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
-[24]: https://github.com/zakhenry/embedme
-[25]: https://github.com/electrovir/markdown-code-example-inserter
-[26]: https://github.com/dineshsonachalam/markdown-autodocs
-[27]: https://github.com/romnn/embedme
-[28]: https://github.com/drewavis/markdowninclude
-[29]: https://github.com/tokusumi/markdown-embed-code
-[30]: https://github.com/ARMmbed/snippet
-[31]: https://github.com/SimonCropp/MarkdownSnippets
-[32]: https://github.com/shiftkey/scribble
-[33]:
-  https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
-[34]: https://github.com/JulianCataldo/remark-embed
-[35]: https://github.com/calebpeterson/jest-transformer-test-md
-[36]: https://github.com/ildar-shaimordanov/git-markdown-snippet
-[37]: https://github.com/sammndhr/gridsome-remark-embed-snippet
-[38]: https://gridsome.org/
-[39]:
-  https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
-[40]: https://github.com/gatsbyjs/gatsby
-[41]: https://github.com/endocode/snippetextractor
-[42]: https://github.com/javierfernandes/markdown-exercises
-[43]: https://github.com/devincornell/pymddoc
-[44]: https://github.com/NativeScript/markdown-snippet-injector
-[45]: https://github.com/polywrap/doc-snippets
-[46]:
-  https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
-[47]: https://github.com/xrd/oreilly-snippets
-[48]: https://github.com/DamonOehlman/injectcode
-[49]: https://github.com/fuxingloh/remark-code-import-replace
-[50]: https://github.com/teyc/markdown-snippet
-[51]: https://github.com/marc-bouvier-graveyard/baldir_markdown
-[52]: https://github.com/tjstankus/commitate
-[53]: https://github.com/cmacmackin/markdown-include
-[54]: https://github.com/mdx-js/mdx
-[55]:
-  https://github.com/szkiba/mdcode
-  "Extracts code blocks from README and produces tests; a similar approach, but quite different"
-[56]: https://github.com/realazthat/snipinator
+[1]: https://raw.githubusercontent.com/realazthat/snipinator/v1.4.1/.github/logo-exported.svg
+[2]: https://github.com/realazthat/snipinator
+[3]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
+[4]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
+[5]: https://img.shields.io/github/languages/top/realazthat/snipinator.svg?cacheSeconds=28800&style=plastic&color=0A1E1E
+[6]: https://img.shields.io/github/license/realazthat/snipinator?style=plastic&color=0A1E1E
+[7]: https://github.com/realazthat/snipinator/blob/v1.4.1/LICENSE.md
+[8]: https://img.shields.io/pypi/v/snipinator?style=plastic&color=0A1E1E
+[9]: https://pypi.org/project/snipinator/
+[10]: https://img.shields.io/pypi/pyversions/snipinator?style=plastic&color=0A1E1E
+[11]: https://github.com/realazthat/snipinator/tree/master
+[12]: https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=master&style=plastic
+[13]: https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
+[14]: https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.1/master?style=plastic
+[15]: https://github.com/realazthat/snipinator/compare/v1.4.1...master
+[16]: https://img.shields.io/github/last-commit/realazthat/snipinator/master?style=plastic
+[17]: https://github.com/realazthat/snipinator/tree/develop
+[18]: https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=develop&style=plastic
+[19]: https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.1/develop?style=plastic
+[20]: https://github.com/realazthat/snipinator/compare/v1.4.1...develop
+[21]: https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.1/develop?style=plastic
+[22]: https://github.com/realazthat/snipinator/compare/v1.4.1...develop
+[23]: https://img.shields.io/github/last-commit/realazthat/snipinator/develop?style=plastic
+[24]: https://github.com/mdx-js/mdx
+[25]: https://github.com/zakhenry/embedme
+[26]: https://github.com/cmacmackin/markdown-include
+[27]: https://github.com/SimonCropp/MarkdownSnippets
+[28]: https://github.com/endocode/snippetextractor
+[29]: https://github.com/polywrap/doc-snippets
+[30]: https://github.com/JulianCataldo/remark-embed
+[31]: https://github.com/xrd/oreilly-snippets
+[32]: https://github.com/DamonOehlman/injectcode
+[33]: https://github.com/electrovir/markdown-code-example-inserter
+[34]: https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
+[35]: https://github.com/ildar-shaimordanov/git-markdown-snippet
+[36]: https://github.com/teyc/markdown-snippet
+[37]: https://github.com/marc-bouvier-graveyard/baldir_markdown
+[38]: https://github.com/dineshsonachalam/markdown-autodocs
+[39]: https://github.com/tokusumi/markdown-embed-code
+[40]: https://github.com/sammndhr/gridsome-remark-embed-snippet
+[41]: https://gridsome.org/
+[42]: https://github.com/NativeScript/markdown-snippet-injector
+[43]: https://github.com/fuxingloh/remark-code-import-replace
+[44]: https://github.com/szkiba/mdcode "Extracts code blocks from README and produces tests; a similar approach, but quite different"
+[45]: https://github.com/devincornell/pymddoc
+[46]: https://github.com/shiftkey/scribble
+[47]: https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
+[48]: https://github.com/calebpeterson/jest-transformer-test-md
+[49]: https://github.com/tjstankus/commitate
+[50]: https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
+[51]: https://github.com/javierfernandes/markdown-exercises
+[52]: https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
+[53]: https://github.com/gatsbyjs/gatsby
+[54]: https://github.com/ARMmbed/snippet
+[55]: https://github.com/drewavis/markdowninclude
+[56]: https://github.com/romnn/embedme
```

### Comparing `snipinator-1.4.0/README.md` & `snipinator-1.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 
 
 
 
 -->
 
-# <div align="center">[![Snipinator][22]][56]</div>
+# <div align="center">[![Snipinator][1]][2]</div>
 
 <div align="center">
 
 <!-- Icons from https://lucide.dev/icons/users -->
 <!-- Icons from https://lucide.dev/icons/laptop-minimal -->
 
-![**Audience:** Developers][19] ![**Platform:** Linux][20]
+![**Audience:** Developers][3] ![**Platform:** Linux][4]
 
 </div>
 
 <p align="center">
   <strong>
     <a href="https://github.com/realazthat/snipinator">🏠Home</a>
     &nbsp;&bull;&nbsp;
@@ -48,29 +48,29 @@
     &nbsp;&bull;&nbsp;
     <a href="#-gotchas-and-limitations">🚸Gotchas</a>
   </strong>
 </p>
 
 <div align="center">
 
-![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
-[![Python Version][8]][5]
+![Top language][5] [![GitHub License][6]][7] [![PyPI - Version][8]][9]
+[![Python Version][10]][9]
 
 **CLI to embed (testable) snippets from your codebase into your README**
 
 </div>
 
 ---
 
 <div align="center">
 
-|                   | Status                     | Stable                    | Unstable                  |                    |
-| ----------------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
-| **[Master][17]**  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
-| **[Develop][18]** | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+|                   | Status                      | Stable                    | Unstable                  |                    |
+| ----------------- | --------------------------- | ------------------------- | ------------------------- | ------------------ |
+| **[Master][11]**  | [![Build and Test][12]][13] | [![since tagged][14]][15] |                           | ![last commit][16] |
+| **[Develop][17]** | [![Build and Test][18]][13] | [![since tagged][19]][20] | [![since tagged][21]][22] | ![last commit][23] |
 
 </div>
 
 <img src=".github/demo.gif" alt="Demo" width="100%">
 
 ## ❔ What
 
@@ -147,15 +147,15 @@
 ## 🔨 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/snipinator/)
 pip install snipinator
 
 # Install from git (https://github.com/realazthat/snipinator)
-pip install git+https://github.com/realazthat/snipinator.git@v1.4.0
+pip install git+https://github.com/realazthat/snipinator.git@v1.4.1
 ```
 
 ## 🚜 Usage
 
 Example template README:
 ([./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2)):
 
@@ -683,44 +683,44 @@
 ## 🤝 Related Projects
 
 Not complete, and not necessarily up to date. Make a PR
 ([contributions](#-contributions)) to insert/modify.
 
 | Project                                                           | Stars     | Last Update  | Language   | Platform         | Similarity X Obviousness |
 | ----------------------------------------------------------------- | --------- | ------------ | ---------- | ---------------- | ------------------------ |
-| [mdx-js/mdx][54]                                                  | 16.8k     | `2024/04/17` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [zakhenry/embedme][24]                                            | 222       | `2023/11/08` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [cmacmackin/markdown-include][53]                                 | 95        | `2023/02/07` | Python     | N/A              | ⭐⭐⭐⭐⭐               |
-| [SimonCropp/MarkdownSnippets][31]                                 | 23        | `2024/04/23` | .NET       | N/A              | ⭐⭐⭐⭐⭐               |
-| [endocode/snippetextractor][41]                                   | 4         | `2014/08/16` | C++        | N/A              | ⭐⭐⭐⭐⭐               |
-| [polywrap/doc-snippets][45]                                       | 3         | `2023/09/26` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [JulianCataldo/remark-embed][34]                                  | 2         | `2022/09/22` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [xrd/oreilly-snippets][47]                                        | 2         | `2015/10/15` | Ruby       | N/A              | ⭐⭐⭐⭐⭐               |
-| [DamonOehlman/injectcode][48]                                     | 1         | `2021/08/01` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [electrovir/markdown-code-example-inserter][25]                   | 1         | `2024/02/19` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets][46] | 1         | `2021/02/12` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [ildar-shaimordanov/git-markdown-snippet][36]                     | 0         | `2021/09/14` | Perl       | N/A              | ⭐⭐⭐⭐⭐               |
-| [teyc/markdown-snippet][50]                                       | 0         | `2024/01/22` | Powershell | N/A              | ⭐⭐⭐⭐⭐               |
-| [marc-bouvier-graveyard/baldir_markdown][51]                      | 0         | `2020/06/15` | Python     | N/A              | ⭐⭐⭐⭐⭐               |
-| [dineshsonachalam/markdown-autodocs][26]                          | 176       | `2022/09/19` | JS         | GH Action        | ⭐⭐⭐⭐                 |
-| [tokusumi/markdown-embed-code][29]                                | 28        | `2022/01/05` | Python     | VSCode Extension | ⭐⭐⭐⭐                 |
-| [sammndhr/gridsome-remark-embed-snippet][37]                      | 2         | `2021/06/14` | JS         | [Gridsome][38]   | ⭐⭐⭐⭐                 |
-| [NativeScript/markdown-snippet-injector][44]                      | 4         | `2019/01/24` | JS         | N/A              | ⭐⭐⭐⭐                 |
-| [fuxingloh/remark-code-import-replace][49]                        | 0         | `2022/12/21` | JS         | Remark?          | ⭐⭐⭐⭐                 |
-| [szkiba/mdcode][55]                                               | 15        | `2014/02/12` | Go         | N/A              | ⭐⭐⭐                   |
-| [devincornell/pymddoc][43]                                        | 0         | `2023/12/01` | Python     | Python           | ⭐⭐⭐                   |
-| [shiftkey/scribble][32] ([docs][33])                              | 40        | `2013/08/08` | .NET       | N/A              | ⭐⭐                     |
-| [calebpeterson/jest-transformer-test-md][35]                      | 2         | `2020/08/21` | JS         | Jest Tests       | ⭐⭐                     |
-| [tjstankus/commitate][52]                                         | 0         | `2014/05/29` | Ruby       | N/A              | ⭐                       |
-| [GitHub Docs: Creating a permanent link to a code snippet][23]    | N/A       | N/A          | N/A        | N/A              | ⭐                       |
-| [javierfernandes/markdown-exercises][42]                          | 1         | `2017/05/01` | JS         | N/A              | ⭐                       |
-| [gatsby-remark-embed-snippet][39]                                 | N/A (55k) | `2024/01/23` | JS         | [Gatsby][40]     | ⭐                       |
-| [ARMmbed/snippet][30]                                             | 6         | `2021/08/05` | Python     | N/A              | ?                        |
-| [drewavis/markdowninclude][28]                                    | 1         | `2024/04/06` | JS         | VSCode Extension | ?                        |
-| [romnn/embedme][27]                                               | 0         | `2024/04/18` | Go         | N/A              | ?                        |
+| [mdx-js/mdx][24]                                                  | 16.8k     | `2024/04/17` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [zakhenry/embedme][25]                                            | 222       | `2023/11/08` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [cmacmackin/markdown-include][26]                                 | 95        | `2023/02/07` | Python     | N/A              | ⭐⭐⭐⭐⭐               |
+| [SimonCropp/MarkdownSnippets][27]                                 | 23        | `2024/04/23` | .NET       | N/A              | ⭐⭐⭐⭐⭐               |
+| [endocode/snippetextractor][28]                                   | 4         | `2014/08/16` | C++        | N/A              | ⭐⭐⭐⭐⭐               |
+| [polywrap/doc-snippets][29]                                       | 3         | `2023/09/26` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [JulianCataldo/remark-embed][30]                                  | 2         | `2022/09/22` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [xrd/oreilly-snippets][31]                                        | 2         | `2015/10/15` | Ruby       | N/A              | ⭐⭐⭐⭐⭐               |
+| [DamonOehlman/injectcode][32]                                     | 1         | `2021/08/01` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [electrovir/markdown-code-example-inserter][33]                   | 1         | `2024/02/19` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets][34] | 1         | `2021/02/12` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
+| [ildar-shaimordanov/git-markdown-snippet][35]                     | 0         | `2021/09/14` | Perl       | N/A              | ⭐⭐⭐⭐⭐               |
+| [teyc/markdown-snippet][36]                                       | 0         | `2024/01/22` | Powershell | N/A              | ⭐⭐⭐⭐⭐               |
+| [marc-bouvier-graveyard/baldir_markdown][37]                      | 0         | `2020/06/15` | Python     | N/A              | ⭐⭐⭐⭐⭐               |
+| [dineshsonachalam/markdown-autodocs][38]                          | 176       | `2022/09/19` | JS         | GH Action        | ⭐⭐⭐⭐                 |
+| [tokusumi/markdown-embed-code][39]                                | 28        | `2022/01/05` | Python     | VSCode Extension | ⭐⭐⭐⭐                 |
+| [sammndhr/gridsome-remark-embed-snippet][40]                      | 2         | `2021/06/14` | JS         | [Gridsome][41]   | ⭐⭐⭐⭐                 |
+| [NativeScript/markdown-snippet-injector][42]                      | 4         | `2019/01/24` | JS         | N/A              | ⭐⭐⭐⭐                 |
+| [fuxingloh/remark-code-import-replace][43]                        | 0         | `2022/12/21` | JS         | Remark?          | ⭐⭐⭐⭐                 |
+| [szkiba/mdcode][44]                                               | 15        | `2014/02/12` | Go         | N/A              | ⭐⭐⭐                   |
+| [devincornell/pymddoc][45]                                        | 0         | `2023/12/01` | Python     | Python           | ⭐⭐⭐                   |
+| [shiftkey/scribble][46] ([docs][47])                              | 40        | `2013/08/08` | .NET       | N/A              | ⭐⭐                     |
+| [calebpeterson/jest-transformer-test-md][48]                      | 2         | `2020/08/21` | JS         | Jest Tests       | ⭐⭐                     |
+| [tjstankus/commitate][49]                                         | 0         | `2014/05/29` | Ruby       | N/A              | ⭐                       |
+| [GitHub Docs: Creating a permanent link to a code snippet][50]    | N/A       | N/A          | N/A        | N/A              | ⭐                       |
+| [javierfernandes/markdown-exercises][51]                          | 1         | `2017/05/01` | JS         | N/A              | ⭐                       |
+| [gatsby-remark-embed-snippet][52]                                 | N/A (55k) | `2024/01/23` | JS         | [Gatsby][53]     | ⭐                       |
+| [ARMmbed/snippet][54]                                             | 6         | `2021/08/05` | Python     | N/A              | ?                        |
+| [drewavis/markdowninclude][55]                                    | 1         | `2024/04/06` | JS         | VSCode Extension | ?                        |
+| [romnn/embedme][56]                                               | 0         | `2024/04/18` | Go         | N/A              | ?                        |
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
 
@@ -786,92 +786,86 @@
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
-[1]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=master&style=plastic
-[2]:
-  https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
+[1]: ./.github/logo-exported.svg
+[2]: https://github.com/realazthat/snipinator
 [3]:
-  https://img.shields.io/github/license/realazthat/snipinator?style=plastic&color=0A1E1E
+  https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
 [4]:
-  https://img.shields.io/pypi/v/snipinator?style=plastic&color=0A1E1E
-[5]: https://pypi.org/project/snipinator/
+  https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
+[5]:
+  https://img.shields.io/github/languages/top/realazthat/snipinator.svg?cacheSeconds=28800&style=plastic&color=0A1E1E
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/master?style=plastic
-[7]:
-  https://img.shields.io/github/last-commit/realazthat/snipinator/master?style=plastic
+  https://img.shields.io/github/license/realazthat/snipinator?style=plastic&color=0A1E1E
+[7]: ./LICENSE.md
 [8]:
-  https://img.shields.io/pypi/pyversions/snipinator?style=plastic&color=0A1E1E
-[9]:
-  https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
+  https://img.shields.io/pypi/v/snipinator?style=plastic&color=0A1E1E
+[9]: https://pypi.org/project/snipinator/
 [10]:
-  https://github.com/realazthat/snipinator/compare/v1.4.0...master
-[11]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=develop&style=plastic
+  https://img.shields.io/pypi/pyversions/snipinator?style=plastic&color=0A1E1E
+[11]: https://github.com/realazthat/snipinator/tree/master
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/develop?style=plastic
+  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=master&style=plastic
 [13]:
-  https://github.com/realazthat/snipinator/compare/v1.4.0...develop
+  https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
 [14]:
-  https://img.shields.io/github/last-commit/realazthat/snipinator/develop?style=plastic
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.1/master?style=plastic
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/develop?style=plastic
+  https://github.com/realazthat/snipinator/compare/v1.4.1...master
 [16]:
-  https://github.com/realazthat/snipinator/compare/v1.4.0...develop
-[17]: https://github.com/realazthat/snipinator/tree/master
-[18]: https://github.com/realazthat/snipinator/tree/develop
-
-<!-- Logo from https://lucide.dev/icons/users -->
-
+  https://img.shields.io/github/last-commit/realazthat/snipinator/master?style=plastic
+[17]: https://github.com/realazthat/snipinator/tree/develop
+[18]:
+  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=develop&style=plastic
 [19]:
-  https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
-
-<!-- Logo from https://lucide.dev/icons/laptop-minimal -->
-
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.1/develop?style=plastic
 [20]:
-  https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
-[21]: ./LICENSE.md
-[22]: ./.github/logo-exported.svg
+  https://github.com/realazthat/snipinator/compare/v1.4.1...develop
+[21]:
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.1/develop?style=plastic
+[22]:
+  https://github.com/realazthat/snipinator/compare/v1.4.1...develop
 [23]:
-  https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
-[24]: https://github.com/zakhenry/embedme
-[25]: https://github.com/electrovir/markdown-code-example-inserter
-[26]: https://github.com/dineshsonachalam/markdown-autodocs
-[27]: https://github.com/romnn/embedme
-[28]: https://github.com/drewavis/markdowninclude
-[29]: https://github.com/tokusumi/markdown-embed-code
-[30]: https://github.com/ARMmbed/snippet
-[31]: https://github.com/SimonCropp/MarkdownSnippets
-[32]: https://github.com/shiftkey/scribble
-[33]:
-  https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
-[34]: https://github.com/JulianCataldo/remark-embed
-[35]: https://github.com/calebpeterson/jest-transformer-test-md
-[36]: https://github.com/ildar-shaimordanov/git-markdown-snippet
-[37]: https://github.com/sammndhr/gridsome-remark-embed-snippet
-[38]: https://gridsome.org/
-[39]:
-  https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
-[40]: https://github.com/gatsbyjs/gatsby
-[41]: https://github.com/endocode/snippetextractor
-[42]: https://github.com/javierfernandes/markdown-exercises
-[43]: https://github.com/devincornell/pymddoc
-[44]: https://github.com/NativeScript/markdown-snippet-injector
-[45]: https://github.com/polywrap/doc-snippets
-[46]:
+  https://img.shields.io/github/last-commit/realazthat/snipinator/develop?style=plastic
+[24]: https://github.com/mdx-js/mdx
+[25]: https://github.com/zakhenry/embedme
+[26]: https://github.com/cmacmackin/markdown-include
+[27]: https://github.com/SimonCropp/MarkdownSnippets
+[28]: https://github.com/endocode/snippetextractor
+[29]: https://github.com/polywrap/doc-snippets
+[30]: https://github.com/JulianCataldo/remark-embed
+[31]: https://github.com/xrd/oreilly-snippets
+[32]: https://github.com/DamonOehlman/injectcode
+[33]: https://github.com/electrovir/markdown-code-example-inserter
+[34]:
   https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
-[47]: https://github.com/xrd/oreilly-snippets
-[48]: https://github.com/DamonOehlman/injectcode
-[49]: https://github.com/fuxingloh/remark-code-import-replace
-[50]: https://github.com/teyc/markdown-snippet
-[51]: https://github.com/marc-bouvier-graveyard/baldir_markdown
-[52]: https://github.com/tjstankus/commitate
-[53]: https://github.com/cmacmackin/markdown-include
-[54]: https://github.com/mdx-js/mdx
-[55]:
+[35]: https://github.com/ildar-shaimordanov/git-markdown-snippet
+[36]: https://github.com/teyc/markdown-snippet
+[37]: https://github.com/marc-bouvier-graveyard/baldir_markdown
+[38]: https://github.com/dineshsonachalam/markdown-autodocs
+[39]: https://github.com/tokusumi/markdown-embed-code
+[40]: https://github.com/sammndhr/gridsome-remark-embed-snippet
+[41]: https://gridsome.org/
+[42]: https://github.com/NativeScript/markdown-snippet-injector
+[43]: https://github.com/fuxingloh/remark-code-import-replace
+[44]:
   https://github.com/szkiba/mdcode
   "Extracts code blocks from README and produces tests; a similar approach, but quite different"
-[56]: https://github.com/realazthat/snipinator
+[45]: https://github.com/devincornell/pymddoc
+[46]: https://github.com/shiftkey/scribble
+[47]:
+  https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
+[48]: https://github.com/calebpeterson/jest-transformer-test-md
+[49]: https://github.com/tjstankus/commitate
+[50]:
+  https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
+[51]: https://github.com/javierfernandes/markdown-exercises
+[52]:
+  https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
+[53]: https://github.com/gatsbyjs/gatsby
+[54]: https://github.com/ARMmbed/snippet
+[55]: https://github.com/drewavis/markdowninclude
+[56]: https://github.com/romnn/embedme
```

### Comparing `snipinator-1.4.0/pyproject.toml` & `snipinator-1.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snipinator"
-version = "1.4.0"
+version = "1.4.1"
 description = "Python code snippets for markdown files, e.g READMEs, from actual (testable) code."
 authors = [{name = "AYF", email = "realazthat@gmail.com"}]
 license = {file = "LICENSE.md"}
-readme = "README.md"
+readme = ".github/README.remotified.md"
 requires-python = ">=3.8"
 classifiers = [
   "Operating System :: OS Independent",
   'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
@@ -73,14 +73,16 @@
 ]
 # Set of dev dependencies, all pinned, so that they are known to work. To add a
 # new dependency here, add the unpinned package name here, and then run
 # `EXTRA=dev bash scripts/pin-extra-reqs.sh`.
 dev = [
   "argcomplete==3.2.3",
   "autoflake==2.3.1",
+  "beautifulsoup4==4.12.3",
+  "bs4==0.0.2",
   "build==1.0.3",
   "certifi==2024.2.2",
   "cffi==1.16.0",
   "cfgv==3.4.0",
   "changeguard==0.3.1",
   "charset-normalizer==3.3.2",
   "click==8.1.7",
@@ -101,15 +103,18 @@
   "keyring==24.3.1",
   "markdown-it-py==3.0.0",
   "markupsafe==2.1.5",
   "mdformat==0.7.17",
   "mdformat-gfm==0.3.0",
   "mdformat-tables==0.4.1",
   "mdit-py-plugins==0.4.0",
+  "mdreftidy==0.3.0",
+  "mdremotifier==0.3.1",
   "mdurl==0.1.2",
+  "mistletoe==1.3.0",
   "more-itertools==10.2.0",
   "mypy==1.8.0",
   "mypy-extensions==1.0.0",
   "nh3==0.2.15",
   "nodeenv==1.8.0",
   "packaging==23.2",
   "pathspec==0.12.1",
@@ -130,19 +135,22 @@
   "readme-renderer==43.0",
   "requests==2.31.0",
   "requests-toolbelt==1.0.0",
   "rfc3986==2.0.0",
   "rich==13.7.1",
   "rich-argparse==1.4.0",
   "secretstorage==3.3.3",
+  "soupsieve==2.5",
   "toml-sort==0.23.1",
   "tomli==2.0.1",
   "tomlkit==0.12.4",
   "twine==5.0.0",
+  "types-beautifulsoup4==4.12.0.20240229",
   "types-colorama==0.4.15.20240311",
+  "types-html5lib==1.1.11.20240228",
   "types-pyyaml==6.0.12.20240311",
   "typing-extensions==4.10.0",
   "urllib3==2.2.1",
   "virtualenv==20.25.0",
   "wcwidth==0.2.13",
   "wheel==0.43.0",
   "xmltodict==0.13.0",
@@ -159,11 +167,11 @@
 Documentation = "https://github.com/realazthat/snipinator"
 Repository = "https://github.com/realazthat/snipinator"
 
 [tool.setuptools]
 packages = ["snipinator"]
 
 [tool.snipinator-project-metadata]
-last_unstable_release = "1.4.0"
-last_stable_release = "1.4.0"
+last_unstable_release = "1.4.1"
+last_stable_release = "1.4.1"
 
 [tool.tomlsort]
```

### Comparing `snipinator-1.4.0/snipinator/__init__.py` & `snipinator-1.4.1/snipinator/__init__.py`

 * *Files identical despite different names*

### Comparing `snipinator-1.4.0/snipinator/cli.py` & `snipinator-1.4.1/snipinator/cli.py`

 * *Files identical despite different names*

### Comparing `snipinator-1.4.0/snipinator/snipinate.py` & `snipinator-1.4.1/snipinator/snipinate.py`

 * *Files identical despite different names*

### Comparing `snipinator-1.4.0/snipinator/snipinate_test.py` & `snipinator-1.4.1/snipinator/snipinate_test.py`

 * *Files identical despite different names*

### Comparing `snipinator-1.4.0/snipinator.egg-info/PKG-INFO` & `snipinator-1.4.1/snipinator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snipinator
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python code snippets for markdown files, e.g READMEs, from actual (testable) code.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -64,14 +64,16 @@
 Requires-Dist: rich==13.7.1; extra == "prod"
 Requires-Dist: rich-argparse==1.4.0; extra == "prod"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "prod"
 Requires-Dist: typing-extensions==4.10.0; extra == "prod"
 Provides-Extra: dev
 Requires-Dist: argcomplete==3.2.3; extra == "dev"
 Requires-Dist: autoflake==2.3.1; extra == "dev"
+Requires-Dist: beautifulsoup4==4.12.3; extra == "dev"
+Requires-Dist: bs4==0.0.2; extra == "dev"
 Requires-Dist: build==1.0.3; extra == "dev"
 Requires-Dist: certifi==2024.2.2; extra == "dev"
 Requires-Dist: cffi==1.16.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
 Requires-Dist: changeguard==0.3.1; extra == "dev"
 Requires-Dist: charset-normalizer==3.3.2; extra == "dev"
 Requires-Dist: click==8.1.7; extra == "dev"
@@ -92,15 +94,18 @@
 Requires-Dist: keyring==24.3.1; extra == "dev"
 Requires-Dist: markdown-it-py==3.0.0; extra == "dev"
 Requires-Dist: markupsafe==2.1.5; extra == "dev"
 Requires-Dist: mdformat==0.7.17; extra == "dev"
 Requires-Dist: mdformat-gfm==0.3.0; extra == "dev"
 Requires-Dist: mdformat-tables==0.4.1; extra == "dev"
 Requires-Dist: mdit-py-plugins==0.4.0; extra == "dev"
+Requires-Dist: mdreftidy==0.3.0; extra == "dev"
+Requires-Dist: mdremotifier==0.3.1; extra == "dev"
 Requires-Dist: mdurl==0.1.2; extra == "dev"
+Requires-Dist: mistletoe==1.3.0; extra == "dev"
 Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
 Requires-Dist: nh3==0.2.15; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
 Requires-Dist: packaging==23.2; extra == "dev"
 Requires-Dist: pathspec==0.12.1; extra == "dev"
@@ -121,19 +126,22 @@
 Requires-Dist: readme-renderer==43.0; extra == "dev"
 Requires-Dist: requests==2.31.0; extra == "dev"
 Requires-Dist: requests-toolbelt==1.0.0; extra == "dev"
 Requires-Dist: rfc3986==2.0.0; extra == "dev"
 Requires-Dist: rich==13.7.1; extra == "dev"
 Requires-Dist: rich-argparse==1.4.0; extra == "dev"
 Requires-Dist: secretstorage==3.3.3; extra == "dev"
+Requires-Dist: soupsieve==2.5; extra == "dev"
 Requires-Dist: toml-sort==0.23.1; extra == "dev"
 Requires-Dist: tomli==2.0.1; extra == "dev"
 Requires-Dist: tomlkit==0.12.4; extra == "dev"
 Requires-Dist: twine==5.0.0; extra == "dev"
+Requires-Dist: types-beautifulsoup4==4.12.0.20240229; extra == "dev"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "dev"
+Requires-Dist: types-html5lib==1.1.11.20240228; extra == "dev"
 Requires-Dist: types-pyyaml==6.0.12.20240311; extra == "dev"
 Requires-Dist: typing-extensions==4.10.0; extra == "dev"
 Requires-Dist: urllib3==2.2.1; extra == "dev"
 Requires-Dist: virtualenv==20.25.0; extra == "dev"
 Requires-Dist: wcwidth==0.2.13; extra == "dev"
 Requires-Dist: wheel==0.43.0; extra == "dev"
 Requires-Dist: xmltodict==0.13.0; extra == "dev"
@@ -153,22 +161,22 @@
 
 
 
 
 
 -->
 
-# <div align="center">[![Snipinator][22]][56]</div>
+# <div align="center">[![Snipinator][1]][2]</div>
 
 <div align="center">
 
 <!-- Icons from https://lucide.dev/icons/users -->
 <!-- Icons from https://lucide.dev/icons/laptop-minimal -->
 
-![**Audience:** Developers][19] ![**Platform:** Linux][20]
+![**Audience:** Developers][3] ![**Platform:** Linux][4]
 
 </div>
 
 <p align="center">
   <strong>
     <a href="https://github.com/realazthat/snipinator">🏠Home</a>
     &nbsp;&bull;&nbsp;
@@ -191,40 +199,40 @@
     &nbsp;&bull;&nbsp;
     <a href="#-gotchas-and-limitations">🚸Gotchas</a>
   </strong>
 </p>
 
 <div align="center">
 
-![Top language][9] [![GitHub License][3]][21] [![PyPI - Version][4]][5]
-[![Python Version][8]][5]
+![Top language][5] [![GitHub License][6]][7] [![PyPI - Version][8]][9]
+[![Python Version][10]][9]
 
 **CLI to embed (testable) snippets from your codebase into your README**
 
 </div>
 
 ---
 
 <div align="center">
 
-|                   | Status                     | Stable                    | Unstable                  |                    |
-| ----------------- | -------------------------- | ------------------------- | ------------------------- | ------------------ |
-| **[Master][17]**  | [![Build and Test][1]][2]  | [![since tagged][6]][10]  |                           | ![last commit][7]  |
-| **[Develop][18]** | [![Build and Test][11]][2] | [![since tagged][12]][13] | [![since tagged][15]][16] | ![last commit][14] |
+|                   | Status                      | Stable                    | Unstable                  |                    |
+| ----------------- | --------------------------- | ------------------------- | ------------------------- | ------------------ |
+| **[Master][11]**  | [![Build and Test][12]][13] | [![since tagged][14]][15] |                           | ![last commit][16] |
+| **[Develop][17]** | [![Build and Test][18]][13] | [![since tagged][19]][20] | [![since tagged][21]][22] | ![last commit][23] |
 
 </div>
 
-<img src=".github/demo.gif" alt="Demo" width="100%">
+<img alt="Demo" src="https://raw.githubusercontent.com/realazthat/snipinator/v1.4.1/.github/demo.gif" width="100%"/>
 
 ## ❔ What
 
 What it does: **Snipinator** lets you take a `EXAMPLE.md` template
 and include snippets from your (working and tested) codebase.
 
-Turn this ([./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2)):
+Turn this ([./snipinator/examples/EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/EXAMPLE.md.jinja2)):
 
 <!---->
 ```md
 # A README
 
 Here is a code snippet:
 
@@ -232,15 +240,15 @@
 
 Note that `code.py` has a test:
 {{path('./snipinator/examples/code_test.py', link='md')}}.
 
 ```
 <!---->
 
-Into this ([./snipinator/examples/EXAMPLE.generated.md](./snipinator/examples/EXAMPLE.generated.md)):
+Into this ([./snipinator/examples/EXAMPLE.generated.md](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/EXAMPLE.generated.md)):
 
 <!---->
 ````md
 <!--
 
 WARNING: This file is auto-generated by snipinator. Do not edit directly.
 SOURCE: `snipinator/examples/EXAMPLE.md.jinja2`.
@@ -290,21 +298,21 @@
 ## 🔨 Installation
 
 ```bash
 # Install from pypi (https://pypi.org/project/snipinator/)
 pip install snipinator
 
 # Install from git (https://github.com/realazthat/snipinator)
-pip install git+https://github.com/realazthat/snipinator.git@v1.4.0
+pip install git+https://github.com/realazthat/snipinator.git@v1.4.1
 ```
 
 ## 🚜 Usage
 
 Example template README:
-([./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2)):
+([./snipinator/examples/EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/EXAMPLE.md.jinja2)):
 
 <!---->
 ```md
 # A README
 
 Here is a code snippet:
 
@@ -350,35 +358,35 @@
 
 ````
 <!---->
 
 ## 💻 Command Line Options
 
 <!---->
-<img src="README.help.generated.svg" alt="Output of `python -m snipinator.cli --help`" />
-<!---->
+<img alt="Output of `python -m snipinator.cli --help`" src="https://raw.githubusercontent.com/realazthat/snipinator/v1.4.1/README.help.generated.svg"/>
+<!-- -->
 
 ## 💡 Examples
 
 - Snipinator's own `README`:
-  - Template: [./README.md.jinja2](./README.md.jinja2).
-  - Generated: [./README.md](./README.md).
-  - Generation script: [./scripts/generate-readme.sh](./scripts/generate-readme.sh).
+  - Template: [./README.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md.jinja2).
+  - Generated: [./README.md](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md).
+  - Generation script: [./scripts/generate-readme.sh](https://github.com/realazthat/snipinator/blob/v1.4.1/scripts/generate-readme.sh).
 - Example:
-  - Template: [./snipinator/examples/EXAMPLE.md.jinja2](./snipinator/examples/EXAMPLE.md.jinja2).
+  - Template: [./snipinator/examples/EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/EXAMPLE.md.jinja2).
   - Generated:
-    [./snipinator/examples/EXAMPLE.generated.md](./snipinator/examples/EXAMPLE.generated.md).
-  - Generation script: [./snipinator/examples/example.sh](./snipinator/examples/example.sh).
+    [./snipinator/examples/EXAMPLE.generated.md](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/EXAMPLE.generated.md).
+  - Generation script: [./snipinator/examples/example.sh](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/example.sh).
 - Long example of many features:
   - Template:
-    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
+    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/LONG-EXAMPLE.md.jinja2).
   - Generated:
-    [./snipinator/examples/LONG-EXAMPLE.generated.md](./snipinator/examples/LONG-EXAMPLE.generated.md).
+    [./snipinator/examples/LONG-EXAMPLE.generated.md](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/LONG-EXAMPLE.generated.md).
   - Generation script:
-    [./snipinator/examples/long-example.sh](./snipinator/examples/long-example.sh).
+    [./snipinator/examples/long-example.sh](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/long-example.sh).
 - Projects using Snipinator:
   - [realazthat/snipinator](https://github.com/realazthat/snipinator), See
     [snipinator/README.md.jinja2](https://github.com/realazthat/snipinator/blob/61cb88593baa099dc375cf5fd40679e4be673fc5/README.md.jinja2).
   - [realazthat/changeguard](https://github.com/realazthat/changeguard), See
     [changeguard/README.md.jinja2](https://github.com/realazthat/changeguard/blob/87d5104b52e651bb9195a3d46dd7f050acbcb534/README.md.jinja2).
   - [realazthat/comfy-catapult](https://github.com/realazthat/comfy-catapult),
     See
@@ -395,15 +403,15 @@
 [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
 Additional (Jinja2) functions made available:
 
 ### 🐍✂ pysnippet
 
 Used several times in
-[./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
+[./snipinator/examples/LONG-EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/LONG-EXAMPLE.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def pysnippet(path: str,
               symbol: Optional[str],
@@ -441,15 +449,15 @@
       Union[str, markupsafe.Markup]: The snippet.
   """
 ```
 <!---->
 
 ### 🐍📖 pysignature
 
-Used several times in [./README.md.jinja2](./README.md.jinja2).
+Used several times in [./README.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def pysignature(path: str,
                 symbol: str,
@@ -488,15 +496,15 @@
       str: The signature and docstring.
   """
 ```
 <!---->
 
 ### ✂ rawsnippet
 
-Used several times in [./README.md.jinja2](./README.md.jinja2).
+Used several times in [./README.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def rawsnippet(path: str,
                *,
@@ -532,15 +540,15 @@
   """
 
 ```
 <!---->
 
 ### ✂ snippet
 
-Example in [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2).
+Example in [./snipinator/examples/LONG-EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/LONG-EXAMPLE.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def snippet(path: str,
             start: str,
@@ -582,15 +590,15 @@
   """
 
 ```
 <!---->
 
 ### 🐚 shell
 
-Used several times in [./README.md.jinja2](./README.md.jinja2).
+Used several times in [./README.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def shell(args: str,
           *,
@@ -678,15 +686,15 @@
       Union[str, markupsafe.Markup]: Returns the output of the command.
   """
 ```
 <!---->
 
 ### 🌀 path
 
-Used several times in [./README.md.jinja2](./README.md.jinja2).
+Used several times in [./README.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md.jinja2).
 
 Documentation:
 
 <!---->
 ```py
 def path(path: str,
          *,
@@ -742,15 +750,15 @@
 - Python 3.8+
   - Why: Some dev dependencies require Python 3.8+.
 
 ### Tested Platforms
 
 - WSL2 Ubuntu 20.04, Python `3.8.0`.
 - Ubuntu 20.04, Python `3.8.0, 3.9.0, 3.10.0, 3.11.0, 3.12.0`, tested in GitHub Actions
-  workflow ([build-and-test.yml](./.github/workflows/build-and-test.yml)).
+  workflow ([build-and-test.yml](https://github.com/realazthat/snipinator/blob/v1.4.1/.github/workflows/build-and-test.yml)).
 
 ## 🚸 Gotchas and Limitations
 
 - **Security:** This tool is NOT designed to be used with untrusted input. It is
   designed to be used with your own codebase. Even when using your own input, be
   careful that your own code won't be doing anything that might inadvertently
   include untrusted input.
@@ -772,15 +780,15 @@
   ` ````language ```My Snippet``` ```` ` and this is a method that Markdown uses
   to allow embedded backticks inside a code block.
 - Formatting: The `{{` `}}` used to
   surround the snippet calls will unfortunately be formatted by a Markdown
   formatter and make the call invalid. Workarounds:
   - **Decommentify**: Put the snippet call inside a HTML comment, then use
     `decommentify` parameter. See
-    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](./snipinator/examples/LONG-EXAMPLE.md.jinja2) for
+    [./snipinator/examples/LONG-EXAMPLE.md.jinja2](https://github.com/realazthat/snipinator/blob/v1.4.1/snipinator/examples/LONG-EXAMPLE.md.jinja2) for
     examples.
   - [prettier](https://prettier.io/) formatter is pretty good at leaving the
     Jinja2 calls alone, especially if you don't have any spaces. This especially
     helps for markdown "reference-style links" that have Jinja2 calls in them
     generating part of the URL, mdformat will URL encode the Jinja2 calls,
     and/or split them on spaces, which is not what we want. prettier will leave
     them alone.
@@ -806,15 +814,15 @@
 
 We use SemVer for versioning. For the versions available, see the tags on this
 repository.
 
 ## 🔑 License
 
 This project is licensed under the MIT License - see the
-[./LICENSE.md](./LICENSE.md) file for details.
+[./LICENSE.md](https://github.com/realazthat/snipinator/blob/v1.4.1/LICENSE.md) file for details.
 
 ## 🙏 Thanks
 
 Main libraries used in Snipinator are:
 
 - Templating: [Jinja2](https://github.com/pallets/jinja).
 - Snippet inclusion: Python's AST library.
@@ -826,98 +834,98 @@
 ## 🤝 Related Projects
 
 Not complete, and not necessarily up to date. Make a PR
 ([contributions](#-contributions)) to insert/modify.
 
 | Project                                                           | Stars     | Last Update  | Language   | Platform         | Similarity X Obviousness |
 | ----------------------------------------------------------------- | --------- | ------------ | ---------- | ---------------- | ------------------------ |
-| [mdx-js/mdx][54]                                                  | 16.8k     | `2024/04/17` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [zakhenry/embedme][24]                                            | 222       | `2023/11/08` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [cmacmackin/markdown-include][53]                                 | 95        | `2023/02/07` | Python     | N/A              | ⭐⭐⭐⭐⭐               |
-| [SimonCropp/MarkdownSnippets][31]                                 | 23        | `2024/04/23` | .NET       | N/A              | ⭐⭐⭐⭐⭐               |
-| [endocode/snippetextractor][41]                                   | 4         | `2014/08/16` | C++        | N/A              | ⭐⭐⭐⭐⭐               |
-| [polywrap/doc-snippets][45]                                       | 3         | `2023/09/26` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [JulianCataldo/remark-embed][34]                                  | 2         | `2022/09/22` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [xrd/oreilly-snippets][47]                                        | 2         | `2015/10/15` | Ruby       | N/A              | ⭐⭐⭐⭐⭐               |
-| [DamonOehlman/injectcode][48]                                     | 1         | `2021/08/01` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [electrovir/markdown-code-example-inserter][25]                   | 1         | `2024/02/19` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets][46] | 1         | `2021/02/12` | JS         | N/A              | ⭐⭐⭐⭐⭐               |
-| [ildar-shaimordanov/git-markdown-snippet][36]                     | 0         | `2021/09/14` | Perl       | N/A              | ⭐⭐⭐⭐⭐               |
-| [teyc/markdown-snippet][50]                                       | 0         | `2024/01/22` | Powershell | N/A              | ⭐⭐⭐⭐⭐               |
-| [marc-bouvier-graveyard/baldir_markdown][51]                      | 0         | `2020/06/15` | Python     | N/A              | ⭐⭐⭐⭐⭐               |
-| [dineshsonachalam/markdown-autodocs][26]                          | 176       | `2022/09/19` | JS         | GH Action        | ⭐⭐⭐⭐                 |
-| [tokusumi/markdown-embed-code][29]                                | 28        | `2022/01/05` | Python     | VSCode Extension | ⭐⭐⭐⭐                 |
-| [sammndhr/gridsome-remark-embed-snippet][37]                      | 2         | `2021/06/14` | JS         | [Gridsome][38]   | ⭐⭐⭐⭐                 |
-| [NativeScript/markdown-snippet-injector][44]                      | 4         | `2019/01/24` | JS         | N/A              | ⭐⭐⭐⭐                 |
-| [fuxingloh/remark-code-import-replace][49]                        | 0         | `2022/12/21` | JS         | Remark?          | ⭐⭐⭐⭐                 |
-| [szkiba/mdcode][55]                                               | 15        | `2014/02/12` | Go         | N/A              | ⭐⭐⭐                   |
-| [devincornell/pymddoc][43]                                        | 0         | `2023/12/01` | Python     | Python           | ⭐⭐⭐                   |
-| [shiftkey/scribble][32] ([docs][33])                              | 40        | `2013/08/08` | .NET       | N/A              | ⭐⭐                     |
-| [calebpeterson/jest-transformer-test-md][35]                      | 2         | `2020/08/21` | JS         | Jest Tests       | ⭐⭐                     |
-| [tjstankus/commitate][52]                                         | 0         | `2014/05/29` | Ruby       | N/A              | ⭐                       |
-| [GitHub Docs: Creating a permanent link to a code snippet][23]    | N/A       | N/A          | N/A        | N/A              | ⭐                       |
-| [javierfernandes/markdown-exercises][42]                          | 1         | `2017/05/01` | JS         | N/A              | ⭐                       |
-| [gatsby-remark-embed-snippet][39]                                 | N/A (55k) | `2024/01/23` | JS         | [Gatsby][40]     | ⭐                       |
-| [ARMmbed/snippet][30]                                             | 6         | `2021/08/05` | Python     | N/A              | ?                        |
-| [drewavis/markdowninclude][28]                                    | 1         | `2024/04/06` | JS         | VSCode Extension | ?                        |
-| [romnn/embedme][27]                                               | 0         | `2024/04/18` | Go         | N/A              | ?                        |
+| [mdx-js/mdx][24]                                                  | 16.8k     | `2024/04/17` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [zakhenry/embedme][25]                                            | 222       | `2023/11/08` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [cmacmackin/markdown-include][26]                                 | 95        | `2023/02/07` | Python     | N/A              | ⭐⭐⭐⭐⭐                    |
+| [SimonCropp/MarkdownSnippets][27]                                 | 23        | `2024/04/23` | .NET       | N/A              | ⭐⭐⭐⭐⭐                    |
+| [endocode/snippetextractor][28]                                   | 4         | `2014/08/16` | C++        | N/A              | ⭐⭐⭐⭐⭐                    |
+| [polywrap/doc-snippets][29]                                       | 3         | `2023/09/26` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [JulianCataldo/remark-embed][30]                                  | 2         | `2022/09/22` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [xrd/oreilly-snippets][31]                                        | 2         | `2015/10/15` | Ruby       | N/A              | ⭐⭐⭐⭐⭐                    |
+| [DamonOehlman/injectcode][32]                                     | 1         | `2021/08/01` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [electrovir/markdown-code-example-inserter][33]                   | 1         | `2024/02/19` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets][34] | 1         | `2021/02/12` | JS         | N/A              | ⭐⭐⭐⭐⭐                    |
+| [ildar-shaimordanov/git-markdown-snippet][35]                     | 0         | `2021/09/14` | Perl       | N/A              | ⭐⭐⭐⭐⭐                    |
+| [teyc/markdown-snippet][36]                                       | 0         | `2024/01/22` | Powershell | N/A              | ⭐⭐⭐⭐⭐                    |
+| [marc-bouvier-graveyard/baldir_markdown][37]                      | 0         | `2020/06/15` | Python     | N/A              | ⭐⭐⭐⭐⭐                    |
+| [dineshsonachalam/markdown-autodocs][38]                          | 176       | `2022/09/19` | JS         | GH Action        | ⭐⭐⭐⭐                     |
+| [tokusumi/markdown-embed-code][39]                                | 28        | `2022/01/05` | Python     | VSCode Extension | ⭐⭐⭐⭐                     |
+| [sammndhr/gridsome-remark-embed-snippet][40]                      | 2         | `2021/06/14` | JS         | [Gridsome][41]   | ⭐⭐⭐⭐                     |
+| [NativeScript/markdown-snippet-injector][42]                      | 4         | `2019/01/24` | JS         | N/A              | ⭐⭐⭐⭐                     |
+| [fuxingloh/remark-code-import-replace][43]                        | 0         | `2022/12/21` | JS         | Remark?          | ⭐⭐⭐⭐                     |
+| [szkiba/mdcode][44]                                               | 15        | `2014/02/12` | Go         | N/A              | ⭐⭐⭐                      |
+| [devincornell/pymddoc][45]                                        | 0         | `2023/12/01` | Python     | Python           | ⭐⭐⭐                      |
+| [shiftkey/scribble][46] ([docs][47])                              | 40        | `2013/08/08` | .NET       | N/A              | ⭐⭐                       |
+| [calebpeterson/jest-transformer-test-md][48]                      | 2         | `2020/08/21` | JS         | Jest Tests       | ⭐⭐                       |
+| [tjstankus/commitate][49]                                         | 0         | `2014/05/29` | Ruby       | N/A              | ⭐                        |
+| [GitHub Docs: Creating a permanent link to a code snippet][50]    | N/A       | N/A          | N/A        | N/A              | ⭐                        |
+| [javierfernandes/markdown-exercises][51]                          | 1         | `2017/05/01` | JS         | N/A              | ⭐                        |
+| [gatsby-remark-embed-snippet][52]                                 | N/A (55k) | `2024/01/23` | JS         | [Gatsby][53]     | ⭐                        |
+| [ARMmbed/snippet][54]                                             | 6         | `2021/08/05` | Python     | N/A              | ?                        |
+| [drewavis/markdowninclude][55]                                    | 1         | `2024/04/06` | JS         | VSCode Extension | ?                        |
+| [romnn/embedme][56]                                               | 0         | `2024/04/18` | Go         | N/A              | ?                        |
 
 ## 🫡 Contributions
 
 ### Development environment: Linux-like
 
 - For running `pre.sh` (Linux-like environment).
 
-  - From [./.github/dependencies.yml](./.github/dependencies.yml), which is used for
+  - From [./.github/dependencies.yml](https://github.com/realazthat/snipinator/blob/v1.4.1/.github/dependencies.yml), which is used for
     the GH Action to do a fresh install of everything:
 
     ```yaml
     bash: scripts.
     findutils: scripts.
     grep: tests.
     xxd: tests.
     git: scripts, tests.
     xxhash: scripts (changeguard).
     rsync: out-of-directory test.
     expect: for `unbuffer`, useful to grab and compare ansi color symbols.
     jq: dependency for [yq](https://github.com/kislyuk/yq), which is used to generate
       the README; the README generator needs to use `tomlq` (which is a part of `yq`)
       to query `pyproject.toml`.
-    
+
     ```
 
   - Requires `pyenv`, or an exact matching version of python as in
-    [.python-version](.python-version) (which is currently
+    [.python-version](https://github.com/realazthat/snipinator/blob/v1.4.1/.python-version) (which is currently
     `3.8.0`).
   - act (to run the GH Action locally):
     - Requires nodejs.
     - Requires Go.
     - docker.
   - Generate animation:
     - docker
 
 ### Commit Process
 
 1. (Optionally) Fork the `develop` branch.
 2. Stage your files: `git add path/to/file.py`.
 3. `bash ./scripts/pre.sh`, this will format, lint, and test the code.
 4. `git status` check if anything changed (generated
-   [./README.md](./README.md) for example), if so, `git add` the
+   [./README.md](https://github.com/realazthat/snipinator/blob/v1.4.1/README.md) for example), if so, `git add` the
    changes, and go back to the previous step.
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## 🔄🚀 Release Process
 
 These instructions are for maintainers of the project.
 
 1. In the `develop` branch, run `bash ./scripts/pre.sh` to ensure
    everything is in order.
 2. In the `develop` branch, bump the version in
-   [./pyproject.toml](./pyproject.toml), following semantic versioning
+   [./pyproject.toml](https://github.com/realazthat/snipinator/blob/v1.4.1/pyproject.toml), following semantic versioning
    principles. Also modify the `last_unstable_release` and `last_stable_release`
    in the `[tool.snipinator-project-metadata]` table as appropriate. Run
    `bash ./scripts/pre.sh` to ensure everything is in order.
 3. In the `develop` branch, commit these changes with a message like
    `"Prepare release X.Y.Z"`. (See the contributions section
    [above](#commit-process)).
 4. Merge the `develop` branch into the `master` branch:
@@ -929,92 +937,63 @@
 7. Push to GitHub: Push the commit and tags to GitHub with
    `git push && git push --tags`.
 8. The `--no-ff` option adds a commit to the master branch for the merge, so
    refork the develop branch from the master branch:
    `git checkout develop && git merge master`.
 9. Push the develop branch to GitHub: `git push origin develop`.
 
-[1]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=master&style=plastic
-[2]:
-  https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
-[3]:
-  https://img.shields.io/github/license/realazthat/snipinator?style=plastic&color=0A1E1E
-[4]:
-  https://img.shields.io/pypi/v/snipinator?style=plastic&color=0A1E1E
-[5]: https://pypi.org/project/snipinator/
-[6]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/master?style=plastic
-[7]:
-  https://img.shields.io/github/last-commit/realazthat/snipinator/master?style=plastic
-[8]:
-  https://img.shields.io/pypi/pyversions/snipinator?style=plastic&color=0A1E1E
-[9]:
-  https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800&style=plastic&color=0A1E1E
-[10]:
-  https://github.com/realazthat/snipinator/compare/v1.4.0...master
-[11]:
-  https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=develop&style=plastic
-[12]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/develop?style=plastic
-[13]:
-  https://github.com/realazthat/snipinator/compare/v1.4.0...develop
-[14]:
-  https://img.shields.io/github/last-commit/realazthat/snipinator/develop?style=plastic
-[15]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.0/develop?style=plastic
-[16]:
-  https://github.com/realazthat/snipinator/compare/v1.4.0...develop
-[17]: https://github.com/realazthat/snipinator/tree/master
-[18]: https://github.com/realazthat/snipinator/tree/develop
-
-<!-- Logo from https://lucide.dev/icons/users -->
-
-[19]:
-  https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
-
-<!-- Logo from https://lucide.dev/icons/laptop-minimal -->
-
-[20]:
-  https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
-[21]: ./LICENSE.md
-[22]: ./.github/logo-exported.svg
-[23]:
-  https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
-[24]: https://github.com/zakhenry/embedme
-[25]: https://github.com/electrovir/markdown-code-example-inserter
-[26]: https://github.com/dineshsonachalam/markdown-autodocs
-[27]: https://github.com/romnn/embedme
-[28]: https://github.com/drewavis/markdowninclude
-[29]: https://github.com/tokusumi/markdown-embed-code
-[30]: https://github.com/ARMmbed/snippet
-[31]: https://github.com/SimonCropp/MarkdownSnippets
-[32]: https://github.com/shiftkey/scribble
-[33]:
-  https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
-[34]: https://github.com/JulianCataldo/remark-embed
-[35]: https://github.com/calebpeterson/jest-transformer-test-md
-[36]: https://github.com/ildar-shaimordanov/git-markdown-snippet
-[37]: https://github.com/sammndhr/gridsome-remark-embed-snippet
-[38]: https://gridsome.org/
-[39]:
-  https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
-[40]: https://github.com/gatsbyjs/gatsby
-[41]: https://github.com/endocode/snippetextractor
-[42]: https://github.com/javierfernandes/markdown-exercises
-[43]: https://github.com/devincornell/pymddoc
-[44]: https://github.com/NativeScript/markdown-snippet-injector
-[45]: https://github.com/polywrap/doc-snippets
-[46]:
-  https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
-[47]: https://github.com/xrd/oreilly-snippets
-[48]: https://github.com/DamonOehlman/injectcode
-[49]: https://github.com/fuxingloh/remark-code-import-replace
-[50]: https://github.com/teyc/markdown-snippet
-[51]: https://github.com/marc-bouvier-graveyard/baldir_markdown
-[52]: https://github.com/tjstankus/commitate
-[53]: https://github.com/cmacmackin/markdown-include
-[54]: https://github.com/mdx-js/mdx
-[55]:
-  https://github.com/szkiba/mdcode
-  "Extracts code blocks from README and produces tests; a similar approach, but quite different"
-[56]: https://github.com/realazthat/snipinator
+[1]: https://raw.githubusercontent.com/realazthat/snipinator/v1.4.1/.github/logo-exported.svg
+[2]: https://github.com/realazthat/snipinator
+[3]: https://img.shields.io/badge/Audience-Developers-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLXVzZXJzIj48cGF0aCBkPSJNMTYgMjF2LTJhNCA0IDAgMCAwLTQtNEg2YTQgNCAwIDAgMC00IDR2MiIvPjxjaXJjbGUgY3g9IjkiIGN5PSI3IiByPSI0Ii8+PHBhdGggZD0iTTIyIDIxdi0yYTQgNCAwIDAgMC0zLTMuODciLz48cGF0aCBkPSJNMTYgMy4xM2E0IDQgMCAwIDEgMCA3Ljc1Ii8+PC9zdmc+
+[4]: https://img.shields.io/badge/Platform-Linux-0A1E1E?style=plastic&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9ImN1cnJlbnRDb2xvciIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWxhcHRvcC1taW5pbWFsIj48cmVjdCB3aWR0aD0iMTgiIGhlaWdodD0iMTIiIHg9IjMiIHk9IjQiIHJ4PSIyIiByeT0iMiIvPjxsaW5lIHgxPSIyIiB4Mj0iMjIiIHkxPSIyMCIgeTI9IjIwIi8+PC9zdmc+
+[5]: https://img.shields.io/github/languages/top/realazthat/snipinator.svg?cacheSeconds=28800&style=plastic&color=0A1E1E
+[6]: https://img.shields.io/github/license/realazthat/snipinator?style=plastic&color=0A1E1E
+[7]: https://github.com/realazthat/snipinator/blob/v1.4.1/LICENSE.md
+[8]: https://img.shields.io/pypi/v/snipinator?style=plastic&color=0A1E1E
+[9]: https://pypi.org/project/snipinator/
+[10]: https://img.shields.io/pypi/pyversions/snipinator?style=plastic&color=0A1E1E
+[11]: https://github.com/realazthat/snipinator/tree/master
+[12]: https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=master&style=plastic
+[13]: https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
+[14]: https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.1/master?style=plastic
+[15]: https://github.com/realazthat/snipinator/compare/v1.4.1...master
+[16]: https://img.shields.io/github/last-commit/realazthat/snipinator/master?style=plastic
+[17]: https://github.com/realazthat/snipinator/tree/develop
+[18]: https://img.shields.io/github/actions/workflow/status/realazthat/snipinator/build-and-test.yml?branch=develop&style=plastic
+[19]: https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.1/develop?style=plastic
+[20]: https://github.com/realazthat/snipinator/compare/v1.4.1...develop
+[21]: https://img.shields.io/github/commits-since/realazthat/snipinator/v1.4.1/develop?style=plastic
+[22]: https://github.com/realazthat/snipinator/compare/v1.4.1...develop
+[23]: https://img.shields.io/github/last-commit/realazthat/snipinator/develop?style=plastic
+[24]: https://github.com/mdx-js/mdx
+[25]: https://github.com/zakhenry/embedme
+[26]: https://github.com/cmacmackin/markdown-include
+[27]: https://github.com/SimonCropp/MarkdownSnippets
+[28]: https://github.com/endocode/snippetextractor
+[29]: https://github.com/polywrap/doc-snippets
+[30]: https://github.com/JulianCataldo/remark-embed
+[31]: https://github.com/xrd/oreilly-snippets
+[32]: https://github.com/DamonOehlman/injectcode
+[33]: https://github.com/electrovir/markdown-code-example-inserter
+[34]: https://github.com/andersfischernielsen/Simple-Embedded-Markdown-Code-Snippets
+[35]: https://github.com/ildar-shaimordanov/git-markdown-snippet
+[36]: https://github.com/teyc/markdown-snippet
+[37]: https://github.com/marc-bouvier-graveyard/baldir_markdown
+[38]: https://github.com/dineshsonachalam/markdown-autodocs
+[39]: https://github.com/tokusumi/markdown-embed-code
+[40]: https://github.com/sammndhr/gridsome-remark-embed-snippet
+[41]: https://gridsome.org/
+[42]: https://github.com/NativeScript/markdown-snippet-injector
+[43]: https://github.com/fuxingloh/remark-code-import-replace
+[44]: https://github.com/szkiba/mdcode "Extracts code blocks from README and produces tests; a similar approach, but quite different"
+[45]: https://github.com/devincornell/pymddoc
+[46]: https://github.com/shiftkey/scribble
+[47]: https://github.com/shiftkey/scribble/blob/master/docs/features/code-snippets.md
+[48]: https://github.com/calebpeterson/jest-transformer-test-md
+[49]: https://github.com/tjstankus/commitate
+[50]: https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet
+[51]: https://github.com/javierfernandes/markdown-exercises
+[52]: https://github.com/gatsbyjs/gatsby/tree/master/packages/gatsby-remark-embed-snippet
+[53]: https://github.com/gatsbyjs/gatsby
+[54]: https://github.com/ARMmbed/snippet
+[55]: https://github.com/drewavis/markdowninclude
+[56]: https://github.com/romnn/embedme
```

### Comparing `snipinator-1.4.0/snipinator.egg-info/requires.txt` & `snipinator-1.4.1/snipinator.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 [:python_version < "3.8"]
 importlib-metadata
 
 [dev]
 argcomplete==3.2.3
 autoflake==2.3.1
+beautifulsoup4==4.12.3
+bs4==0.0.2
 build==1.0.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 changeguard==0.3.1
 charset-normalizer==3.3.2
 click==8.1.7
@@ -41,15 +43,18 @@
 keyring==24.3.1
 markdown-it-py==3.0.0
 markupsafe==2.1.5
 mdformat==0.7.17
 mdformat-gfm==0.3.0
 mdformat-tables==0.4.1
 mdit-py-plugins==0.4.0
+mdreftidy==0.3.0
+mdremotifier==0.3.1
 mdurl==0.1.2
+mistletoe==1.3.0
 more-itertools==10.2.0
 mypy==1.8.0
 mypy-extensions==1.0.0
 nh3==0.2.15
 nodeenv==1.8.0
 packaging==23.2
 pathspec==0.12.1
@@ -70,19 +75,22 @@
 readme-renderer==43.0
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
 rich-argparse==1.4.0
 secretstorage==3.3.3
+soupsieve==2.5
 toml-sort==0.23.1
 tomli==2.0.1
 tomlkit==0.12.4
 twine==5.0.0
+types-beautifulsoup4==4.12.0.20240229
 types-colorama==0.4.15.20240311
+types-html5lib==1.1.11.20240228
 types-pyyaml==6.0.12.20240311
 typing-extensions==4.10.0
 urllib3==2.2.1
 virtualenv==20.25.0
 wcwidth==0.2.13
 wheel==0.43.0
 xmltodict==0.13.0
```

