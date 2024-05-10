# Comparing `tmp/Phanatic-2.2.3.tar.gz` & `tmp/Phanatic-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Phanatic-2.2.3.tar", last modified: Tue May 23 10:06:39 2023, max compression
+gzip compressed data, was "Phanatic-2.2.4.tar", last modified: Fri May 10 06:53:18 2024, max compression
```

## Comparing `Phanatic-2.2.3.tar` & `Phanatic-2.2.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-23 10:06:39.862907 Phanatic-2.2.3/
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)    34523 2023-05-20 02:23:00.000000 Phanatic-2.2.3/LICENSE.md
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      723 2023-05-23 10:06:39.862907 Phanatic-2.2.3/PKG-INFO
-drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-23 10:06:39.862907 Phanatic-2.2.3/Phanatic/
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-20 02:23:00.000000 Phanatic-2.2.3/Phanatic/__init__.py
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)     4116 2023-05-23 10:03:17.000000 Phanatic-2.2.3/Phanatic/main.py
-drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-05-23 10:06:39.862907 Phanatic-2.2.3/Phanatic.egg-info/
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      723 2023-05-23 10:06:39.000000 Phanatic-2.2.3/Phanatic.egg-info/PKG-INFO
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      251 2023-05-23 10:06:39.000000 Phanatic-2.2.3/Phanatic.egg-info/SOURCES.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        1 2023-05-23 10:06:39.000000 Phanatic-2.2.3/Phanatic.egg-info/dependency_links.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       51 2023-05-23 10:06:39.000000 Phanatic-2.2.3/Phanatic.egg-info/entry_points.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        7 2023-05-23 10:06:39.000000 Phanatic-2.2.3/Phanatic.egg-info/requires.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        9 2023-05-23 10:06:39.000000 Phanatic-2.2.3/Phanatic.egg-info/top_level.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       38 2023-05-23 10:06:39.862907 Phanatic-2.2.3/setup.cfg
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)     1008 2023-05-23 10:03:27.000000 Phanatic-2.2.3/setup.py
+drwxrwxr-x   0 hermes    (1000) hermes    (1000)        0 2024-05-10 06:53:18.217877 Phanatic-2.2.4/
+-rwxrwxr-x   0 hermes    (1000) hermes    (1000)    34523 2023-10-22 01:54:17.000000 Phanatic-2.2.4/LICENSE.md
+-rw-rw-r--   0 hermes    (1000) hermes    (1000)      718 2024-05-10 06:53:18.217877 Phanatic-2.2.4/PKG-INFO
+drwxrwxr-x   0 hermes    (1000) hermes    (1000)        0 2024-05-10 06:53:18.217877 Phanatic-2.2.4/Phanatic/
+-rwxrwxr-x   0 hermes    (1000) hermes    (1000)        0 2023-10-22 01:54:17.000000 Phanatic-2.2.4/Phanatic/__init__.py
+-rwxrwxr-x   0 hermes    (1000) hermes    (1000)     3057 2024-05-10 06:42:09.000000 Phanatic-2.2.4/Phanatic/check.py
+-rwxrwxr-x   0 hermes    (1000) hermes    (1000)     5424 2024-05-10 06:42:09.000000 Phanatic-2.2.4/Phanatic/main.py
+drwxrwxr-x   0 hermes    (1000) hermes    (1000)        0 2024-05-10 06:53:18.217877 Phanatic-2.2.4/Phanatic.egg-info/
+-rw-rw-r--   0 hermes    (1000) hermes    (1000)      718 2024-05-10 06:53:18.000000 Phanatic-2.2.4/Phanatic.egg-info/PKG-INFO
+-rw-rw-r--   0 hermes    (1000) hermes    (1000)      269 2024-05-10 06:53:18.000000 Phanatic-2.2.4/Phanatic.egg-info/SOURCES.txt
+-rw-rw-r--   0 hermes    (1000) hermes    (1000)        1 2024-05-10 06:53:18.000000 Phanatic-2.2.4/Phanatic.egg-info/dependency_links.txt
+-rw-rw-r--   0 hermes    (1000) hermes    (1000)       52 2024-05-10 06:53:18.000000 Phanatic-2.2.4/Phanatic.egg-info/entry_points.txt
+-rw-rw-r--   0 hermes    (1000) hermes    (1000)        7 2024-05-10 06:53:18.000000 Phanatic-2.2.4/Phanatic.egg-info/requires.txt
+-rw-rw-r--   0 hermes    (1000) hermes    (1000)        9 2024-05-10 06:53:18.000000 Phanatic-2.2.4/Phanatic.egg-info/top_level.txt
+-rw-rw-r--   0 hermes    (1000) hermes    (1000)       38 2024-05-10 06:53:18.217877 Phanatic-2.2.4/setup.cfg
+-rwxrwxr-x   0 hermes    (1000) hermes    (1000)      956 2024-05-10 06:42:09.000000 Phanatic-2.2.4/setup.py
```

### Comparing `Phanatic-2.2.3/LICENSE.md` & `Phanatic-2.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Phanatic-2.2.3/Phanatic/main.py` & `Phanatic-2.2.4/Phanatic/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,74 +2,95 @@
 
     import os
     import sys
     import subprocess
     import argparse
     import random
     import pandas as pd
+    from .check import check_task
 
     # Did you know prompts
     prompts = [
         "Phanatic currently only supports short, paired end, illumina reads (default 'PE_illumina_150').",
         "I (J. Iszatt) made Phanatic to assemble S. aureus phage genomes as part of my PhD project.",
         "This is a short read assembler primarily designed for bacteriophage",
         "My favourite bacteriophage is a Silviavirus named Koomba-kaat_1",
-        "You can use your own config file to customise the assembly and functions"
+        "You can use your own config file to customise the assembly and functions",
+        "If you have host bacterial sequences you can create an index file to perform read mapping and re-assembly, this will be done after an initial assembly run"
     ]
     random_prompt = random.choice(prompts)
 
     # Creating function to check directory path
     def valid_dir(dir_path):
+        if not os.path.exists(dir_path):
+            os.makedirs(dir_path)
         if not os.path.isdir(dir_path):
             raise argparse.ArgumentTypeError(
                 f"{dir_path} is not a valid directory path")
         if not os.access(dir_path, os.R_OK):
             raise argparse.ArgumentTypeError(
                 f"{dir_path} is not a readable directory")
         return dir_path
 
+    def check_dir(dir_path):
+        if not os.path.isdir(dir_path):
+            raise argparse.ArgumentTypeError(
+                f"{dir_path} is not a valid directory path")
+        if not os.access(dir_path, os.R_OK):
+            raise argparse.ArgumentTypeError(
+                f"{dir_path} is not a readable directory")
+        keys = os.path.join(dir_path, '.hash_keys')
+        if not os.path.exists(keys):
+            raise argparse.ArgumentTypeError("no hash file exists")
+        return dir_path
+
     def valid_file(file_path):
         if not os.path.isfile(file_path):
             raise argparse.ArgumentTypeError(
                 f"{file_path} is not a valid file path")
         if not os.access(file_path, os.R_OK):
             raise argparse.ArgumentTypeError(
                 f"{file_path} is not a readable file")
         return file_path
 
     # Parsing arguments
-    image = 'iszatt/phanatic:2.2.3'
-    parser = argparse.ArgumentParser(description=f"Easy short read assembly. Joshua J Iszatt: https://github.com/JoshuaIszatt")
+    image = 'iszatt/phanatic:2.2.4'
+    parser = argparse.ArgumentParser(description=f"Phage genome assembly. Joshua J Iszatt: https://github.com/JoshuaIszatt")
 
     # Input/output options
     parser.add_argument('-i', '--input', type=valid_dir, help='Input reads files')
     parser.add_argument('-o', '--output', type=valid_dir, help='Direct output to this location')
-    parser.add_argument('-r', '--reads', type=str, choices=['PE_illumina_150'], default='PE_illumina_150', help='Pipeline options')
+    parser.add_argument('-r', '--reads', type=str, choices=['PE_illumina', 'ONT'], default='PE_illumina', help='Pipeline options')
     parser.add_argument('-c', '--config', type=valid_file, help='Use config file to customise assembly')
+    parser.add_argument('--host_mapping', type=valid_file, help='Use an index file to specify host bacterial genome')
     parser.add_argument('-v', '--version', action="store_true", help='Print the docker image version')
+    parser.add_argument('--check', type=check_dir, help='Verify data integrity of a phanatic output directory')
     parser.add_argument('--show_console', action="store_true", help='Include this flag to write output to console')
     parser.add_argument('--manual', action="store_true", help='Enter container interactively')
     args = parser.parse_args()
 
     # Printing version
     if args.version:
         print(image)
         sys.exit(0)
 
+    if args.check:
+        check_task(args.check)
+        sys.exit(0)
+
     # Obtaining absolute paths if entered correctly
     if args.input and args.output:
         input_path = os.path.abspath(args.input)
         output_path = os.path.abspath(args.output)
     elif args.input and not args.output:
         sys.exit("No output directory specified\nRun --help to see options")
     elif args.output and not args.input:
         sys.exit("No input directory specified\nRun --help to see options")
     else:
         sys.exit("No input or output directories specified\nRun --help to see options")
-        
 
     # Printing command variables
     print(
         f"Program run: {image}",
         f"Input path: {input_path}",
         f"Output path: {output_path}",
         f"Reads type: {args.reads}",
@@ -78,17 +99,22 @@
         f"{random_prompt}",
         ">>>\n",
         sep='\n'
         )
 
     # Copying config file to output dir
     if args.config:
-        print(f"Using {args.config} file \n")
+        print(f"Using {args.config} file for configuration \n")
         os.system(f"cp {args.config} {args.output}/config.ini")
 
+    # Copying index file for read mapping
+    if args.host_mapping:
+        print(f"Using {args.host_mapping} file for host read mapping \n")
+        os.system(f"cp {args.host_mapping} {args.output}/host_mapping.csv")
+
     if args.show_console:
         docker = "docker run"
     else:
         docker = "docker run -d"
 
     # Running docker
     if args.manual: 
@@ -99,10 +125,9 @@
             {image} sleep 1d) bash")
     else:
         command = ["%s -v %s:/assemble/input -v %s:/assemble/output %s /assemble/bin/assemble.sh" %
                 (docker, input_path, output_path, image)]
         result = subprocess.Popen(command, shell=True)
         print(command)
 
-
 if __name__ == "__main__":
-    exit(main())
+    exit(main())
```

### Comparing `Phanatic-2.2.3/setup.py` & `Phanatic-2.2.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name="Phanatic",
-    version="2.2.3",
+    version="2.2.4",
     description="Python package to run de novo bacteriophage assembly container.",
-    url="https://github.com/JoshuaIszatt/Phanatic",
     author="Joshua Iszatt",
     author_email="joshiszatt@gmail.com",
     license="AGPL-3.0",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Programming Language :: Python :: 3",
```

