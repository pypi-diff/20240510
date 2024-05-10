# Comparing `tmp/riddlesolver-0.1.8.tar.gz` & `tmp/riddlesolver-0.1.9.tar.gz`

## Comparing `riddlesolver-0.1.8.tar` & `riddlesolver-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/.idea/.gitignore
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/.idea/.name
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/.idea/misc.xml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/.idea/modules.xml
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/.idea/riddlesolver.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/.idea/vcs.xml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/riddlesolver/__init__.py
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/riddlesolver/app.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/riddlesolver/config.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/riddlesolver/constants.py
--rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/riddlesolver/repository.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/riddlesolver/requirements.txt
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/riddlesolver/setup.py
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/riddlesolver/streamlit_app.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/riddlesolver/summary.py
--rw-r--r--   0        0        0    13631 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/riddlesolver/utils.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/LICENSE
--rw-r--r--   0        0        0     8802 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/README.md
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 riddlesolver-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     7752 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/README.zh-CN.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/.idea/.gitignore
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/.idea/.name
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/.idea/misc.xml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/.idea/modules.xml
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/.idea/riddlesolver.iml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/.idea/vcs.xml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/riddlesolver/__init__.py
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/riddlesolver/app.py
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/riddlesolver/config.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/riddlesolver/constants.py
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/riddlesolver/repository.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/riddlesolver/requirements.txt
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/riddlesolver/setup.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/riddlesolver/streamlit_app.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/riddlesolver/summary.py
+-rw-r--r--   0        0        0    13631 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/riddlesolver/utils.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/LICENSE
+-rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/README.md
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     9532 2020-02-02 00:00:00.000000 riddlesolver-0.1.9/PKG-INFO
```

### Comparing `riddlesolver-0.1.8/.github/workflows/python-publish.yml` & `riddlesolver-0.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `riddlesolver-0.1.8/.idea/riddlesolver.iml` & `riddlesolver-0.1.9/.idea/riddlesolver.iml`

 * *Files identical despite different names*

### Comparing `riddlesolver-0.1.8/riddlesolver/app.py` & `riddlesolver-0.1.9/riddlesolver/app.py`

 * *Files identical despite different names*

### Comparing `riddlesolver-0.1.8/riddlesolver/config.py` & `riddlesolver-0.1.9/riddlesolver/config.py`

 * *Files identical despite different names*

### Comparing `riddlesolver-0.1.8/riddlesolver/constants.py` & `riddlesolver-0.1.9/riddlesolver/constants.py`

 * *Files identical despite different names*

### Comparing `riddlesolver-0.1.8/riddlesolver/repository.py` & `riddlesolver-0.1.9/riddlesolver/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import shutil
-import time
 from datetime import datetime, timedelta
 
 from git import Repo, InvalidGitRepositoryError
 
-from riddlesolver.config import get_config_value
-from riddlesolver.utils import (
+from config import get_config_value
+from utils import (
     extract_owner_repo, get_base_branch_map, get_all_unique_commits,
     get_base_branch_map_local, get_all_unique_commits_local
 )
 
 
 def fetch_commits(repo_path, start_date, end_date, branch=None, author=None, access_token=None, repo_type=None):
     """
@@ -26,15 +25,17 @@
         repo_type (str): The repository type (github, gitlab, local, remote).
 
     Returns:
         list: stores the branch, author, datetime ranges and the commits
     """
     if repo_type == "github":
         if not access_token:
-            raise ValueError("GitHub access token is required.")
+            print(f'There is no access token for {repo_path}, pulling remote commits without authentication.')
+            return fetch_commits_from_remote(repo_path, start_date, end_date, branch, author)
+            # raise ValueError("GitHub access token is required.")
         repo_path_result = extract_owner_repo(repo_path)
         if not repo_path_result:
             raise ValueError(f"Invalid GitHub repository link: {repo_path}")
         return fetch_commits_from_github(repo_path_result, start_date, end_date, branch, author, access_token)
     elif repo_type == "gitlab":
         # GitLab is not implemented yet
         return fetch_commits_from_remote(repo_path, start_date, end_date, branch, author)
@@ -204,14 +205,15 @@
             repo = None
     else:
         repo = None
 
     if repo is None:
         # Clone the remote repository and cache it
         os.makedirs(cache_dir, exist_ok=True)
-        repo = Repo.clone_from(repo_url, repo_cache_dir, no_checkout=True, depth=1)  # Clone with minimal history
+        repo = Repo.clone_from(repo_url, repo_cache_dir, no_checkout=True, depth=1,
+                               filter='blob:none')  # Clone with minimal history
         repo.git.fetch(all=True)  # Fetch all branches and tags
 
     # Fetch the commits using the same logic as fetch_commits_from_local()
     results = fetch_commits_from_local(repo_cache_dir, start_date, end_date, branch, author)
 
     return results
```

### Comparing `riddlesolver-0.1.8/riddlesolver/setup.py` & `riddlesolver-0.1.9/riddlesolver/setup.py`

 * *Files identical despite different names*

### Comparing `riddlesolver-0.1.8/riddlesolver/streamlit_app.py` & `riddlesolver-0.1.9/riddlesolver/streamlit_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import configparser
 from datetime import datetime, timedelta
 
 import streamlit as st
 
-from riddlesolver.repository import fetch_commits
-from riddlesolver.summary import generate_commit_summary
-from riddlesolver.utils import get_repository_type
+from repository import fetch_commits
+from summary import generate_commit_summary
+from utils import get_repository_type
 
 # Load the configuration
 config = configparser.ConfigParser()
 config.add_section("github")
 config.add_section("openai")
 
 # Set the page title
```

### Comparing `riddlesolver-0.1.8/riddlesolver/summary.py` & `riddlesolver-0.1.9/riddlesolver/summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import defaultdict
 
 import openai
 
-from riddlesolver.constants import SUMMARY_PROMPT_TEMPLATE
+from constants import SUMMARY_PROMPT_TEMPLATE
 from utils import format_date, handle_error, calculate_days_between_dates
 
 
 def generate_commit_summary(batched_commits, config, output_file=None):
     """
     Generates a summary of commits within the specified date range.
```

### Comparing `riddlesolver-0.1.8/riddlesolver/utils.py` & `riddlesolver-0.1.9/riddlesolver/utils.py`

 * *Files identical despite different names*

### Comparing `riddlesolver-0.1.8/.gitignore` & `riddlesolver-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `riddlesolver-0.1.8/LICENSE` & `riddlesolver-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `riddlesolver-0.1.8/README.md` & `riddlesolver-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,35 @@
+Metadata-Version: 2.3
+Name: riddlesolver
+Version: 0.1.9
+Summary: A command-line tool to summarize Git commits using OpenAI ChatGPT
+Author-email: Siyuan Wu <cushmily@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Requires-Dist: gitpython
+Requires-Dist: openai
+Requires-Dist: requests
+Description-Content-Type: text/markdown
+
 # RiddleSolver 🎩🔍
 
+[English](README.md) | [简体中文](README.zh-CN.md)
+
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
-[![Version](https://img.shields.io/badge/version-0.1.7-blue.svg)](https://github.com/AnomalyBound/riddlesolver)
+[![Version](https://img.shields.io/badge/version-0.1.9-blue.svg)](https://github.com/AnomalyBound/riddlesolver)
 [![Last Commit](https://img.shields.io/github/last-commit/AnomalyBound/riddlesolver)](https://github.com/AnomalyBound/riddlesolver/commits)
 
 [![Code Size](https://img.shields.io/github/languages/code-size/AnomalyBound/riddlesolver)](https://github.com/AnomalyBound/riddlesolver)
 [![Downloads](https://img.shields.io/pypi/dm/riddlesolver)](https://pypi.org/project/riddlesolver/)
 
 Ladies and gentlemen, boys and girls, gather around for the most extraordinary, mind-bending, and side-splitting Git commit summarizer you've ever witnessed! 🤯🎪 Introducing... RiddleSolver! 🎭
 
@@ -53,19 +77,19 @@
 - `-w`, `--weeks`: Specify the number of weeks to include in the summary (e.g., `-w 1` for the last week)
 - `-m`, `--months`: Specify the number of months to include in the summary (e.g., `-m 3` for the last 3 months)
 - `-b`, `--branch`: Specify the branch name to focus the genie's powers on
 - `-a`, `--author`: Specify the author's email or name to filter commits by
 - `-o`, `--output`: Specify the path to save the genie's wisdom as a markdown file
 - `-c`, `--command`: Execute a command (`config` or `grant-auth`)
 
-⚠️ **IMPORTANT**: When using RiddleSolver with GitHub remote repositories, you must ensure that you have a valid access token:
+⚠️ **IMPORTANT**: When using RiddleSolver with GitHub remote repositories, you have two options:
+
+1. Use the `grant-auth` command to grant the necessary permissions and utilize the GitHub API for fetching commits. 
 
-- You can either use the `grant-auth` command to grant the necessary permissions 
-- Or you can manually configure the access token in the configuration file (with 'content read' permission). 
-> Please note that manually configured access tokens may be subject to rate limits imposed by GitHub. It is recommended to use the `grant-auth` command for a more seamless experience.
+2. If you choose not to grant authentication, RiddleSolver will still work and fetch commits without using the GitHub API.
 
 ### Configuring the Genie
 
 To customize the genie's behavior and grant it access to the OpenAI API, use the mystical `config` subcommand:
 
 ```bash
 riddlesolver config <section> <key> <value>
@@ -120,15 +144,15 @@
 **🛠️ Development Toolkit**
 ---------------------------
 
 RiddleSolver not only serves as a command-line tool but also provides a well-structured API for developers to integrate its functionality into their own projects. You can use RiddleSolver as a development toolkit to fetch commits, generate summaries, and save the summaries to files.
 
 ### **API Functions**
 
-1.  `fetch_commits(repo_path, start_date, end_date, branch=None, author=None, access_token=None, repo_type=None)`: Fetches commits from a repository within the specified date range, optionally filtered by branch and author. Returns a list of commit objects.
+1.  `fetch_commits(repo_path, start_date, end_date, branch=None, author=None, access_token=None, repo_type=None)`: Fetches commits from a repository within the specified date range, optionally filtered by branch and author. If `access_token` is provided and `repo_type` is set to `"github"`, it will use the GitHub API to fetch commits. Otherwise, it will fetch commits without using the API. Returns a list of commit objects.
     
 2.  `generate_summary(commit_batches, config)`: Generates a summary of commit batches using the OpenAI API. Returns the generated summary as a string.
     
 3.  `save_summary_to_file(summary, output_file)`: Saves the commit summary to a file at the specified output path.
     
 
 ### **Example Usage**
@@ -188,12 +212,8 @@
 
 RiddleSolver is released under the [MIT License](https://opensource.org/licenses/MIT), granting you the power to use, modify, and distribute the genie as you see fit.
 
 ## 🙏 Acknowledgements
 
 The genie would like to express its gratitude to the mighty OpenAI for granting it the power of language understanding and generation. Without their API, the genie would be just another ordinary commit summarizer.
 
-## 🚀 Version
-
-RiddleSolver is currently at version 0.1.7, ready to unravel the mysteries of your Git commits like never before!
-
 Now, prepare to be amazed as RiddleSolver unravels the mysteries of your Git commits and brings clarity to your development journey! 🎉✨
```

### Comparing `riddlesolver-0.1.8/pyproject.toml` & `riddlesolver-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "riddlesolver"
-version = "0.1.8"
+version = "0.1.9"
 description = "A command-line tool to summarize Git commits using OpenAI ChatGPT"
 authors = [{ name = "Siyuan Wu", email = "cushmily@gmail.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `riddlesolver-0.1.8/PKG-INFO` & `riddlesolver-0.1.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,13 @@
-Metadata-Version: 2.3
-Name: riddlesolver
-Version: 0.1.8
-Summary: A command-line tool to summarize Git commits using OpenAI ChatGPT
-Author-email: Siyuan Wu <cushmily@gmail.com>
-License-Expression: MIT
-License-File: LICENSE
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Requires-Dist: gitpython
-Requires-Dist: openai
-Requires-Dist: requests
-Description-Content-Type: text/markdown
-
 # RiddleSolver 🎩🔍
 
+[English](README.md) | [简体中文](README.zh-CN.md)
+
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
-[![Version](https://img.shields.io/badge/version-0.1.7-blue.svg)](https://github.com/AnomalyBound/riddlesolver)
+[![Version](https://img.shields.io/badge/version-0.1.9-blue.svg)](https://github.com/AnomalyBound/riddlesolver)
 [![Last Commit](https://img.shields.io/github/last-commit/AnomalyBound/riddlesolver)](https://github.com/AnomalyBound/riddlesolver/commits)
 
 [![Code Size](https://img.shields.io/github/languages/code-size/AnomalyBound/riddlesolver)](https://github.com/AnomalyBound/riddlesolver)
 [![Downloads](https://img.shields.io/pypi/dm/riddlesolver)](https://pypi.org/project/riddlesolver/)
 
 Ladies and gentlemen, boys and girls, gather around for the most extraordinary, mind-bending, and side-splitting Git commit summarizer you've ever witnessed! 🤯🎪 Introducing... RiddleSolver! 🎭
 
@@ -75,19 +55,19 @@
 - `-w`, `--weeks`: Specify the number of weeks to include in the summary (e.g., `-w 1` for the last week)
 - `-m`, `--months`: Specify the number of months to include in the summary (e.g., `-m 3` for the last 3 months)
 - `-b`, `--branch`: Specify the branch name to focus the genie's powers on
 - `-a`, `--author`: Specify the author's email or name to filter commits by
 - `-o`, `--output`: Specify the path to save the genie's wisdom as a markdown file
 - `-c`, `--command`: Execute a command (`config` or `grant-auth`)
 
-⚠️ **IMPORTANT**: When using RiddleSolver with GitHub remote repositories, you must ensure that you have a valid access token:
+⚠️ **IMPORTANT**: When using RiddleSolver with GitHub remote repositories, you have two options:
+
+1. Use the `grant-auth` command to grant the necessary permissions and utilize the GitHub API for fetching commits. 
 
-- You can either use the `grant-auth` command to grant the necessary permissions 
-- Or you can manually configure the access token in the configuration file (with 'content read' permission). 
-> Please note that manually configured access tokens may be subject to rate limits imposed by GitHub. It is recommended to use the `grant-auth` command for a more seamless experience.
+2. If you choose not to grant authentication, RiddleSolver will still work and fetch commits without using the GitHub API.
 
 ### Configuring the Genie
 
 To customize the genie's behavior and grant it access to the OpenAI API, use the mystical `config` subcommand:
 
 ```bash
 riddlesolver config <section> <key> <value>
@@ -142,15 +122,15 @@
 **🛠️ Development Toolkit**
 ---------------------------
 
 RiddleSolver not only serves as a command-line tool but also provides a well-structured API for developers to integrate its functionality into their own projects. You can use RiddleSolver as a development toolkit to fetch commits, generate summaries, and save the summaries to files.
 
 ### **API Functions**
 
-1.  `fetch_commits(repo_path, start_date, end_date, branch=None, author=None, access_token=None, repo_type=None)`: Fetches commits from a repository within the specified date range, optionally filtered by branch and author. Returns a list of commit objects.
+1.  `fetch_commits(repo_path, start_date, end_date, branch=None, author=None, access_token=None, repo_type=None)`: Fetches commits from a repository within the specified date range, optionally filtered by branch and author. If `access_token` is provided and `repo_type` is set to `"github"`, it will use the GitHub API to fetch commits. Otherwise, it will fetch commits without using the API. Returns a list of commit objects.
     
 2.  `generate_summary(commit_batches, config)`: Generates a summary of commit batches using the OpenAI API. Returns the generated summary as a string.
     
 3.  `save_summary_to_file(summary, output_file)`: Saves the commit summary to a file at the specified output path.
     
 
 ### **Example Usage**
@@ -210,12 +190,8 @@
 
 RiddleSolver is released under the [MIT License](https://opensource.org/licenses/MIT), granting you the power to use, modify, and distribute the genie as you see fit.
 
 ## 🙏 Acknowledgements
 
 The genie would like to express its gratitude to the mighty OpenAI for granting it the power of language understanding and generation. Without their API, the genie would be just another ordinary commit summarizer.
 
-## 🚀 Version
-
-RiddleSolver is currently at version 0.1.7, ready to unravel the mysteries of your Git commits like never before!
-
 Now, prepare to be amazed as RiddleSolver unravels the mysteries of your Git commits and brings clarity to your development journey! 🎉✨
```

