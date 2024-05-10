# Comparing `tmp/aim_flask-1.0.6-py3-none-any.whl.zip` & `tmp/aim_flask-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 5176 bytes, number of entries: 7
 -rw-r--r--  2.0 fat     1079 b- defN 80-Jan-01 00:00 aim_flask/__init__.py
--rw-r--r--  2.0 fat     8833 b- defN 80-Jan-01 00:00 aim_flask/main.py
--rw-r--r--  2.0 fat       38 b- defN 80-Jan-01 00:00 aim_flask-1.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 fat     1087 b- defN 80-Jan-01 00:00 aim_flask-1.0.6.dist-info/LICENSE
--rw-r--r--  2.0 fat      321 b- defN 80-Jan-01 00:00 aim_flask-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 aim_flask-1.0.6.dist-info/WHEEL
-?rw-r--r--  2.0 fat      550 b- defN 16-Jan-01 00:00 aim_flask-1.0.6.dist-info/RECORD
-7 files, 11996 bytes uncompressed, 4202 bytes compressed:  65.0%
+-rw-r--r--  2.0 fat     8821 b- defN 80-Jan-01 00:00 aim_flask/main.py
+-rw-r--r--  2.0 fat       38 b- defN 80-Jan-01 00:00 aim_flask-1.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 fat     1087 b- defN 80-Jan-01 00:00 aim_flask-1.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 fat      321 b- defN 80-Jan-01 00:00 aim_flask-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 aim_flask-1.0.7.dist-info/WHEEL
+?rw-r--r--  2.0 fat      550 b- defN 16-Jan-01 00:00 aim_flask-1.0.7.dist-info/RECORD
+7 files, 11984 bytes uncompressed, 4202 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: aim_flask/__init__.py
 Comment: 
 
 Filename: aim_flask/main.py
 Comment: 
 
-Filename: aim_flask-1.0.6.dist-info/entry_points.txt
+Filename: aim_flask-1.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: aim_flask-1.0.6.dist-info/LICENSE
+Filename: aim_flask-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: aim_flask-1.0.6.dist-info/METADATA
+Filename: aim_flask-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: aim_flask-1.0.6.dist-info/WHEEL
+Filename: aim_flask-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: aim_flask-1.0.6.dist-info/RECORD
+Filename: aim_flask-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aim_flask/main.py

```diff
@@ -2,15 +2,15 @@
 import os
 import subprocess
 import platform
 import logging
 
 # aim_flask.py
 
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 
 # Configure logging
 logging.basicConfig(filename='../setup.log', level=logging.INFO, format='%(asctime)s - %(levelname)s: %(message)s')
 logger = logging.getLogger(__name__)
 
 # GitHub repository URL for feedback and logs
 GITHUB_REPO_URL = "https://github.com/MrMayami/AIM.git"
@@ -57,23 +57,23 @@
     log("Creating project structure...")
     directories = ["app", "app/static", "app/templates"]
     for directory in directories:
         os.makedirs(directory, exist_ok=True)
     log("Project structure created successfully.")
 
     # Create __init__.py in app directory
-    with open("../app/__init__.py", "w") as f:
+    with open("/app/__init__.py", "w") as f:
         f.write("# This file initializes the app package.")
 
     # Create routes.py in app directory
-    with open("../app/routes.py", "w") as f:
+    with open("/app/routes.py", "w") as f:
         f.write("# This file defines the application routes.")
 
     # Create run.py in project root
-    with open("../run.py", "w") as f:
+    with open("/run.py", "w") as f:
         f.write("# This file is used to run the application.")
 
 def install_flask(verbose=False):
     log("Installing Flask...")
     try:
         subprocess.run(["pip", "install", "Flask"], check=True, capture_output=verbose)
         log("Flask installed successfully.")
@@ -121,15 +121,15 @@
 
     - name: Run tests
       run: pytest --collect-only
 
     - name: Build and Deploy
       run: python aim_flask.py :setup
 """
-    with open("../.github/workflows/ci-cd.yml", "w") as wf:
+    with open("/.github/workflows/ci-cd.yml", "w") as wf:
         wf.write(workflow_content)
     log("Workflow file created successfully.")
 
 def run_help():
     help_text = """
     AIM CLI - Environment Setup and Installation
 
@@ -151,15 +151,15 @@
     print(help_text)
 
 def integrate_bootstrap(verbose=False):
     log("Bootstrap integration is pending. Please integrate Bootstrap manually.")
 
 def create_requirements_file(verbose=False):
     log("Creating requirements.txt...")
-    with open("../requirements.txt", "w") as f:
+    with open("/requirements.txt", "w") as f:
         f.write("# Installed dependencies\n")
         # Add other dependencies as needed
     log("requirements.txt created successfully.")
 
     log("Installing dependencies from requirements.txt...")
     try:
         subprocess.run(["pip", "install", "-r", "requirements.txt"], check=True, capture_output=verbose)
@@ -228,15 +228,15 @@
     else:
         log("Git is already installed.")
 
     log("Setup completed successfully.")
 
 def run_feedback(message):
     log("Saving feedback to file...")
-    with open("../feedback.txt", "a") as f:
+    with open("/feedback.txt", "a") as f:
         f.write(message + "\n")
     log("Feedback saved successfully.")
 
     log("Pushing feedback to GitHub...")
     try:
         subprocess.run(["git", "add", "feedback.txt"], check=True, capture_output=True)
         subprocess.run(["git", "commit", "-m", "Added feedback"], check=True, capture_output=True)
```

## Comparing `aim_flask-1.0.6.dist-info/LICENSE` & `aim_flask-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

