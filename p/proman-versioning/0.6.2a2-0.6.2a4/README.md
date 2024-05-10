# Comparing `tmp/proman-versioning-0.6.2a2.tar.gz` & `tmp/proman_versioning-0.6.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proman-versioning-0.6.2a2.tar", last modified: Mon Nov 14 22:38:24 2022, max compression
+gzip compressed data, was "proman_versioning-0.6.2a4.tar", last modified: Fri May 10 04:38:16 2024, max compression
```

## Comparing `proman-versioning-0.6.2a2.tar` & `proman_versioning-0.6.2a4.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 kuwv      (1000) kuwv      (1000)        0 2022-11-14 22:38:24.208821 proman-versioning-0.6.2a2/
--rw-rw-r--   0 kuwv      (1000) kuwv      (1000)     7440 2022-02-11 13:09:13.000000 proman-versioning-0.6.2a2/LICENSE.md
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)       39 2022-11-14 20:22:19.000000 proman-versioning-0.6.2a2/MANIFEST.in
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)     4008 2022-11-14 22:38:24.208821 proman-versioning-0.6.2a2/PKG-INFO
--rw-rw-r--   0 kuwv      (1000) kuwv      (1000)     2762 2022-05-12 17:20:59.000000 proman-versioning-0.6.2a2/README.md
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)     2910 2022-11-14 22:37:45.000000 proman-versioning-0.6.2a2/pyproject.toml
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)       38 2022-11-14 22:38:24.208821 proman-versioning-0.6.2a2/setup.cfg
-drwxr-xr-x   0 kuwv      (1000) kuwv      (1000)        0 2022-11-14 22:38:24.206821 proman-versioning-0.6.2a2/src/
-drwxr-xr-x   0 kuwv      (1000) kuwv      (1000)        0 2022-11-14 22:38:24.207821 proman-versioning-0.6.2a2/src/proman_versioning.egg-info/
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)     4008 2022-11-14 22:38:24.000000 proman-versioning-0.6.2a2/src/proman_versioning.egg-info/PKG-INFO
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)      687 2022-11-14 22:38:24.000000 proman-versioning-0.6.2a2/src/proman_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)        1 2022-11-14 22:38:24.000000 proman-versioning-0.6.2a2/src/proman_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)       53 2022-11-14 22:38:24.000000 proman-versioning-0.6.2a2/src/proman_versioning.egg-info/entry_points.txt
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)      524 2022-11-14 22:38:24.000000 proman-versioning-0.6.2a2/src/proman_versioning.egg-info/requires.txt
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)       11 2022-11-14 22:38:24.000000 proman-versioning-0.6.2a2/src/proman_versioning.egg-info/top_level.txt
-drwxr-xr-x   0 kuwv      (1000) kuwv      (1000)        0 2022-11-14 22:38:24.207821 proman-versioning-0.6.2a2/src/versioning/
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)     1349 2022-11-14 22:37:45.000000 proman-versioning-0.6.2a2/src/versioning/__init__.py
--rw-rw-r--   0 kuwv      (1000) kuwv      (1000)      383 2022-05-12 17:20:59.000000 proman-versioning-0.6.2a2/src/versioning/__main__.py
--rw-rw-r--   0 kuwv      (1000) kuwv      (1000)     4332 2022-05-12 17:20:59.000000 proman-versioning-0.6.2a2/src/versioning/changelog.py
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)     3028 2022-11-05 00:06:41.000000 proman-versioning-0.6.2a2/src/versioning/cli.py
--rw-rw-r--   0 kuwv      (1000) kuwv      (1000)     5570 2022-11-14 19:20:36.000000 proman-versioning-0.6.2a2/src/versioning/config.py
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)     9474 2022-11-05 00:06:41.000000 proman-versioning-0.6.2a2/src/versioning/controller.py
--rw-rw-r--   0 kuwv      (1000) kuwv      (1000)      215 2022-02-11 13:09:13.000000 proman-versioning-0.6.2a2/src/versioning/exception.py
-drwxr-xr-x   0 kuwv      (1000) kuwv      (1000)        0 2022-11-14 22:38:24.208821 proman-versioning-0.6.2a2/src/versioning/grammars/
--rw-rw-r--   0 kuwv      (1000) kuwv      (1000)       36 2021-12-09 17:40:27.000000 proman-versioning-0.6.2a2/src/versioning/grammars/__init__.py
--rwxrwxr-x   0 kuwv      (1000) kuwv      (1000)     1363 2022-06-06 13:28:18.000000 proman-versioning-0.6.2a2/src/versioning/grammars/conventional_commits.lark
--rw-rw-r--   0 kuwv      (1000) kuwv      (1000)     3193 2022-05-12 17:20:59.000000 proman-versioning-0.6.2a2/src/versioning/grammars/conventional_commits.py
--rw-r--r--   0 kuwv      (1000) kuwv      (1000)     5198 2022-11-05 00:06:41.000000 proman-versioning-0.6.2a2/src/versioning/vcs.py
--rw-rw-r--   0 kuwv      (1000) kuwv      (1000)    15991 2022-10-02 23:31:11.000000 proman-versioning-0.6.2a2/src/versioning/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:16.390022 proman_versioning-0.6.2a4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-10 04:38:16.390022 proman_versioning-0.6.2a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-10 04:37:25.000000 proman_versioning-0.6.2a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 04:38:16.390022 proman_versioning-0.6.2a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:16.382022 proman_versioning-0.6.2a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:16.386022 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-10 04:38:16.000000 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-10 04:38:16.000000 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 04:38:16.000000 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 04:38:16.000000 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-10 04:38:16.000000 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 04:38:16.000000 proman_versioning-0.6.2a4/src/proman_versioning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:16.386022 proman_versioning-0.6.2a4/src/versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-10 04:37:25.000000 proman_versioning-0.6.2a4/src/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:16.386022 proman_versioning-0.6.2a4/src/versioning/grammars/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/grammars/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1363 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/grammars/conventional_commits.lark
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/grammars/conventional_commits.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16146 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/src/versioning/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 04:38:16.386022 proman_versioning-0.6.2a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-10 04:37:25.000000 proman_versioning-0.6.2a4/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-10 04:38:01.000000 proman_versioning-0.6.2a4/tests/test_versioning.py
```

### Comparing `proman-versioning-0.6.2a2/LICENSE.md` & `proman_versioning-0.6.2a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proman-versioning-0.6.2a2/README.md` & `proman_versioning-0.6.2a4/README.md`

 * *Files identical despite different names*

### Comparing `proman-versioning-0.6.2a2/pyproject.toml` & `proman_versioning-0.6.2a4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proman-versioning"
-version = "0.6.2a2"
+version = "0.6.2a4"
 description = "Project Management Versioning Tool."
 readme = "README.md"
 license = {text = "LGPL-3.0"}
 keywords = ["versioning", "semver", "calver", "pep440", "configuration management"]
 requires-python = ">=3.6.2"
 authors = [{name = "Jesse P. Johnson", email = "jpj6652@gmail.com"}]
 maintainers = [{name = "Jesse P. Johnson", email = "jpj6652@gmail.com"}]
@@ -36,47 +36,45 @@
     "compendium>=0.1.3",
 ]
 
 [project.optional-dependencies]
 changelog = [
     "mdutils",
 ]
-
 build = [
     "build",
     "proman-versioning>=0.5.0-alpha.2",
-    "proman-workflows>=0.1.0-alpha.8",
-    "invoke>=1.4.1",
-    "twine",
-]
-docs = [
-    "docstr-coverage>=1.2.0",
-    "pydocstyle[toml]>=6.1.1",
-    "mkdocs>=1.2.2",
-    "mkdocs-material>=7.2.0",
-    "mkdocstrings>=0.16.2",
+    "twine"
 ]
-test = [
-    "pyfakefs>=4.5.3",
+dev = [
+    # test
+    "pyfakefs>=5.4.1",
     "pytest>=6.2.5",
     "pytest-cov>=2.10.0",
     "tox>=3.25.0",
-]
-sca = [
+    # sca
+    "mypy>=1",
+    "pylint>=3",
+    # style
+    "black==22.3.0",
+    "isort>=5.10.1",
     "flake8>=3.8.3",
-    "mypy>=0.942",
+    # sast
     "bandit>=1.6.2",
-    "safety>=1.9.0",
-    # "pylint>=2.9.5"
+    "safety>=1.9.0"
 ]
-style = [
-    "black==22.3.0",
-    "isort>=5.10.1",
+docs = [
+    "docstr-coverage>=1.2.0",
+    "mkdocs>=1.2.2",
+    "mkdocs-material>=7.2.0",
+    "mkdocstrings[python]>=0.16.2",
+    "pydocstyle[toml]>=6.1.1"
 ]
 
+
 [project.scripts]
 version = "versioning.__main__:main"
 
 [project.urls]
 homepage = "https://github.com/python-proman/proman-versioning"
 repository = "https://github.com/python-proman/proman-versioning"
 
@@ -121,12 +119,29 @@
     | \.pytest_cache
     | build
     | dist
   )
 )
 '''
 
+[tool.pylint]
+fail-under = 9.0
+
+[tool.pylint."FORMAT"]
+max-line-length = 79
+
+[tool.pylint."MESSAGES CONTROL"]
+disable = [
+    "C0103",
+    "R0903",
+    "W0212",
+    "W0715"
+]
+
+[tool.pylint."MISCELLANEOUS"]
+notes = []
+
 [tool.mypy]
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_untyped_defs = true
 ignore_missing_imports = true
```

### Comparing `proman-versioning-0.6.2a2/src/proman_versioning.egg-info/SOURCES.txt` & `proman_versioning-0.6.2a4/src/proman_versioning.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -11,12 +11,16 @@
 src/versioning/__init__.py
 src/versioning/__main__.py
 src/versioning/changelog.py
 src/versioning/cli.py
 src/versioning/config.py
 src/versioning/controller.py
 src/versioning/exception.py
+src/versioning/py.typed
 src/versioning/vcs.py
 src/versioning/version.py
 src/versioning/grammars/__init__.py
 src/versioning/grammars/conventional_commits.lark
-src/versioning/grammars/conventional_commits.py
+src/versioning/grammars/conventional_commits.py
+tests/test_controller.py
+tests/test_version.py
+tests/test_versioning.py
```

### Comparing `proman-versioning-0.6.2a2/src/versioning/__init__.py` & `proman_versioning-0.6.2a4/src/versioning/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,39 +5,39 @@
 import logging
 from typing import Any
 
 from pygit2 import Repository
 
 from versioning.config import CONFIG_FILES, REPO_DIR, Config
 from versioning.controller import ReleaseController
-from versioning.exception import PromanVersioningException
+from versioning.exception import VersioningException
 from versioning.vcs import Git
 from versioning.version import Version  # noqa
 
 __author__ = 'Jesse P. Johnson'
 __author_email__ = 'jpj6652@gmail.com'
 __title__ = 'proman-versioning'
 __description__ = 'Workflows to manage project versioning.'
-__version__ = '0.6.2a2'
+__version__ = '0.6.2a4'
 __license__ = 'LGPL-3.0'
 __copyright__ = 'Copyright 2021 Jesse Johnson.'
 __all__ = (
     'ReleaseController',
     'get_release_controller',
     'Version',
 )
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 
-def get_release_controller(*args: Any, **kwargs: Any) -> ReleaseController:
+def get_release_controller(**kwargs: Any) -> ReleaseController:
     """Create and return a release controller."""
     try:
         repo_dir = kwargs.pop('repo_dir', REPO_DIR)
         repo = Git(Repository(repo_dir))
 
         config_files = kwargs.pop('config_files', CONFIG_FILES)
         config = Config(filepaths=config_files)
 
         return ReleaseController(config=config, repo=repo, **kwargs)
     except Exception as err:
-        raise PromanVersioningException(err)
+        raise VersioningException(err) from err
```

### Comparing `proman-versioning-0.6.2a2/src/versioning/changelog.py` & `proman_versioning-0.6.2a4/src/versioning/changelog.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import re
 from collections import deque
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Dict, Generator, List, Tuple
 
-from mdutils.mdutils import MdUtils
+from mdutils.mdutils import MdUtils  # pylint: disable=import-error
 
 from versioning.grammars.conventional_commits import CommitMessageParser
 
 if TYPE_CHECKING:
     from pygit2 import Commit, Repository
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
@@ -30,39 +30,31 @@
         """Get tagged commit."""
         # iterate tags and add each commit since preious tag to a section
         regex = re.compile('^refs/tags/')
         tags = [r for r in self.repo.references if regex.match(r)]
         for tag in tags:
             yield self.repo.revparse_single(tag)
 
-    def _categorize_commit(
-        self, commit: 'Commit'
-    ) -> Tuple[str, List[str]]:
+    def _categorize_commit(self, commit: 'Commit') -> Tuple[str, List[str]]:
         """Get changes associated with a release."""
         parser = CommitMessageParser()
         parser.parse(commit.message.rstrip())
         # scope = parser.title['scope']
         row = [
             commit.hex,
             parser.title['type'],
             parser.title['description'],
         ]
 
         if parser.title['type'] == 'feat':
             section = 'added'
         elif parser.title['type'] == 'fix':
             section = 'fixed'
-        elif (
-            parser.title['type'] == 'refactor'
-            or parser.title['type'] == 'ci'
-            or parser.title['type'] == 'build'
-            or parser.title['type'] == 'docs'
-            or parser.title['type'] == 'test'
-            or parser.title['type'] == 'style'
-            or parser.title['type'] == 'perf'
+        elif parser.title['type'] in (
+            'refactor' 'ci' 'build' 'docs' 'test' 'style' 'perf'
         ):
             section = 'changed'
         else:
             section = 'misc'
         return section, row
 
     def generate_changelog(self) -> None:
@@ -105,26 +97,23 @@
         """Generate changelog file."""
         # stopgap until better parser is found
         md = MdUtils(
             file_name='CHANGELOG.md',
             title='Changelog',
             # author='Jesse P. Johnson'
         )
-        md.new_header(
-            level=1,
-            title='ProMan Versioning Changelog'
-        )
+        md.new_header(level=1, title='ProMan Versioning Changelog')
         sections = ['commit', 'type', 'description']
 
         for release in reversed(releases):
             dt = datetime.fromtimestamp(release['time'])
             md.new_header(
                 level=2,
                 # title=f"[v{tag.name}]({url}) - ({dt.strftime('%Y-%m-%d')})"
-                title=f"v{release['name']} - ({dt.strftime('%Y-%m-%d')})"
+                title=f"v{release['name']} - ({dt.strftime('%Y-%m-%d')})",
             )
 
             for k, v in release['changes'].items():
                 if v != []:
                     md.new_header(level=3, title=k)
                     md.new_table(
                         columns=len(sections),
```

### Comparing `proman-versioning-0.6.2a2/src/versioning/cli.py` & `proman_versioning-0.6.2a4/src/versioning/cli.py`

 * *Files identical despite different names*

### Comparing `proman-versioning-0.6.2a2/src/versioning/config.py` & `proman_versioning-0.6.2a4/src/versioning/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 import os
 from dataclasses import InitVar, asdict, dataclass, field
 from typing import Any, Dict, List
 
 from compendium.config_manager import ConfigManager
 from pygit2 import discover_repository
 
-from versioning.exception import PromanVersioningException
+from versioning.exception import VersioningException
 from versioning.version import Version
 
 # from urllib.parse import urljoin, urlparse
 
 # TODO check VCS for paths
 CURRENT_DIR = os.getcwd()
 REPO_DIR = (
     f"{CURRENT_DIR}/.git"
     if os.path.exists(f"{CURRENT_DIR}/.git")
     else discover_repository(CURRENT_DIR)
 )
 if REPO_DIR is None:
-    raise PromanVersioningException('Unable to locate git repository.')
+    raise VersioningException('Unable to locate git repository.')
 PROJECT_DIR = os.path.abspath(os.path.join(REPO_DIR, os.pardir))
 CONFIG_FILES = [
     os.path.join(PROJECT_DIR, '.versioning'),
     os.path.join(PROJECT_DIR, 'pyproject.toml'),
     # TODO: add setup.cfg
 ]
 
@@ -148,15 +148,15 @@
         if (
             self.templates == []
             and 'files' in config
             and config['files'] != []
         ):
             self.templates = config['files']
         # else:
-        #     raise PromanVersioningException('no versioned files provided')
+        #     raise VersioningException('no versioned files provided')
 
         if 'types' not in config:
             angular_convention = [
                 'build',
                 'ci',
                 'docs',
                 'perf',
@@ -170,14 +170,14 @@
         config_version = self.lookup(
             'project.version',
             'proman.version',
             'tool.proman.version',
             'tool.poetry.version',
         )
         # if config_version is None:
-        #     raise PromanVersioningException('no version found in filepaths')
+        #     raise VersioningException('no version found in filepaths')
 
         # TODO: use different version based on config
         self.version = Version(
             version=str(config_version),
             **asdict(ReleaseConfig(config=config)),
         )
```

### Comparing `proman-versioning-0.6.2a2/src/versioning/controller.py` & `proman_versioning-0.6.2a4/src/versioning/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import re
 import sys
 from copy import deepcopy
 from string import Template
 from typing import TYPE_CHECKING, Any, Dict
 
 # from transitions import Machine
-from versioning.exception import PromanVersioningException
+from versioning.exception import VersioningException
 from versioning.grammars.conventional_commits import CommitMessageParser
 from versioning.version import Version
 
 if 'mdutils' not in sys.modules:
     enable_changelog = False
 else:
     from versioning.changelog import Changelog
@@ -69,18 +69,18 @@
         self.vcs = repo
         self.changelog = Changelog(self.vcs.repo) if enable_changelog else None
 
         if message is None:
             head = self.vcs.repo.head
             target = self.vcs.repo[head.target]
             self.parse(target.message)
-            log.debug(f"provided commit message: '{message}'")
+            log.debug('provided commit message: %r', message)
         else:
             self.parse(message)
-            log.debug(f"found commit message: '{message}'")
+            log.debug('found commit message: %r', message)
 
     @property
     def release(self) -> str:
         """Get the current version release state."""
         return self.config.version.state  # type: ignore
 
     def __update_config(
@@ -106,47 +106,47 @@
         if 'compat' in config:
             version.compat = config['compat']
             new_version.compat = config['compat']
 
         filepath = os.path.join(self.vcs.working_dir, config['filepath'])
 
         # TODO: handle when file does not exist
-        with open(filepath, 'r+') as f:
+        with open(filepath, 'r+', encoding='utf-8') as f:
             file_contents = f.read()
 
             if 'patterns' in config:
                 patterns = config['patterns']
             else:
                 patterns = [config['pattern']]
             for pattern in patterns:
                 template = Template(pattern).substitute(version=version.query)
                 match = re.compile(
                     # XXX: escape not compiling correctly
                     template,  # re.escape(template),
                     flags=0,
                 )
-                log.debug(f"using pattern for source version {match}")
+                log.debug('using pattern for source version %s', match)
 
                 # substitute the expression in file
                 file_update = match.sub(
                     Template(pattern).substitute(version=str(new_version)),
                     file_contents,
                 )
 
             if not dry_run:
                 # save the file
                 try:
                     f.seek(0)
                     f.truncate()
                     f.write(file_update)
-                    log.info(f"writting file at: '{filepath}'")
+                    log.info('writting file at: %r', filepath)
                 except Exception as err:
                     print(err, file=sys.stderr)
             else:
-                log.info(f"dry-run skipping file write at: '{filepath}'")
+                log.info('dry-run skipping file write at: %r', filepath)
                 # print the file changes
                 deltas = difflib.unified_diff(
                     file_contents.splitlines(),
                     file_update.splitlines(),
                     fromfile=filepath,
                 )
                 for x in deltas:
@@ -176,30 +176,30 @@
                             f['filepath'] for f in self.config.templates
                         ],
                         message=(
                             f"ci({scope}): apply {str(new_version)} updates"
                         ),
                         dry_run=dry_run,
                     )
-                    log.info(f"commiting version changes: {str(new_version)}")
+                    log.info('commiting version changes: %s', str(new_version))
 
                     if make_tag:
                         self.vcs.tag(
                             name=str(new_version),
                             ref='HEAD',
                             message=None,
                             dry_run=dry_run,
                         )
-                        log.info(f"applying tag: {str(new_version)}")
+                        log.info('applying tag: %s', str(new_version))
             else:
-                raise PromanVersioningException(
+                raise VersioningException(
                     'no version update could be determined'
                 )
         else:
-            raise PromanVersioningException('repository is not clean')
+            raise VersioningException('repository is not clean')
 
     def update_version(self, **kwargs: Any) -> Version:
         """Update the version of the project."""
         new_version = deepcopy(self.config.version)
         if self.changelog:
             self.changelog.generate_changelog()
         if (
@@ -220,15 +220,15 @@
                 elif self.title['type'] == 'fix':
                     new_version.bump_micro()  # type: ignore
                 elif self.title['type'] in self.config.parser.types:
                     # new_version = self.__bump_release(new_version)
                     new_version.bump_release()  # type: ignore
                 else:
                     # TODO: need debug statement here instead
-                    raise PromanVersioningException(
+                    raise VersioningException(
                         'received unsupported commit type'
                     )
 
             # TODO: configure local version handling
             if build is not None:
                 new_version._new_local(local=build)
         self.update_configs(new_version, **kwargs)
```

### Comparing `proman-versioning-0.6.2a2/src/versioning/grammars/conventional_commits.lark` & `proman_versioning-0.6.2a4/src/versioning/grammars/conventional_commits.lark`

 * *Files identical despite different names*

### Comparing `proman-versioning-0.6.2a2/src/versioning/grammars/conventional_commits.py` & `proman_versioning-0.6.2a4/src/versioning/grammars/conventional_commits.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # copyright: (c) 2021 by Jesse Johnson.
 # license: LGPL-3.0, see LICENSE.md for more details.
 """Parse Git commit messages."""
 
 # import logging
 from collections import defaultdict
-from typing import Any, Callable, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional
 
 from lark import Lark
 
 from versioning.config import GRAMMAR_PATH
 
+if TYPE_CHECKING:
+    from lark import UnexpectedInput
+    from lark.tree import Tree
+
 
 class CommitMessageParser:
     """Parse commit messages."""
 
+    __tree: 'Tree'
+
     def __init__(
         self,
         grammar_path: str = GRAMMAR_PATH,
         start: str = 'message',
         **kwargs: Any
     ) -> None:
         """Initialize commit message parser."""
@@ -26,19 +32,19 @@
         self.scopes = kwargs.pop('scopes', [])
         self.__parser = Lark.open(grammar_path, start=start, **kwargs)
 
     def parse(
         self,
         text: str,
         start: Optional[str] = None,
-        on_error: Optional[Callable] = None
+        on_error: Optional[Callable[['UnexpectedInput'], bool]] = None,
     ) -> None:
         """Parse commit message."""
-        self.__tree = self.__parser.parse(  # type: ignore
-            text, start=start, on_error=on_error
+        self.__tree = self.__parser.parse(
+            text, start=start, on_error=on_error  # type: ignore
         )
 
     def _get_section(self, name: str) -> Optional[Any]:
         """Get commit message section."""
         for arg in self.__tree.children:
             # NOTE: will not have parse tree for non-match
             if hasattr(arg, '__dict__') and vars(arg)['data'] == name:
@@ -57,16 +63,15 @@
 
     @property
     def body(self) -> List[str]:
         """Get body section of commit message."""
         section = self._get_section('body')
         if section:
             return [arg.value for arg in section.children]
-        else:
-            return []
+        return []
 
     @property
     def footer(self) -> Dict[str, Any]:
         """Get footer section of commit message."""
         footer: Dict[str, Any] = defaultdict(lambda: None)
         footer['issues'] = []
 
@@ -84,11 +89,10 @@
                             footer['trailer']['email'] = y.value
                 if arg.data == 'issue':
                     footer['issues'].append(
                         {arg.children[0].value: arg.children[1].value}
                     )
                 if arg.data == 'breaking_change':
                     footer['breaking_change'] = next(
-                        (x.value for x in arg.children),
-                        'Unknown'
+                        (x.value for x in arg.children), 'Unknown'
                     )
         return footer
```

### Comparing `proman-versioning-0.6.2a2/src/versioning/vcs.py` & `proman_versioning-0.6.2a4/src/versioning/vcs.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     RemoteCallbacks,
     Repository,
     Signature,
     Tag,
     UserPass,
 )
 
-from versioning.exception import PromanVersioningException
+from versioning.exception import VersioningException
 
 
 class Git:
     """Provide settings for git repositories."""
 
     def __init__(self, repo: Repository) -> None:
         """Initialize git object."""
@@ -29,29 +29,29 @@
         self.config = os.path.join(self.repo.path, 'config')
 
     @property
     def username(self) -> str:
         """Return username from git configuration."""
         try:
             return self.repo.config['user.name']
-        except Exception:
-            raise PromanVersioningException('git user.name not configured')
+        except Exception as exc:
+            raise VersioningException('git user.name not configured') from exc
 
     @property
     def branch(self) -> str:
         """Return branch name of current branch."""
         return self.repo.head.shorthand
 
     @property
     def email(self) -> str:
         """Return email from git configuration."""
         try:
             return self.repo.config['user.email']
-        except Exception:
-            raise PromanVersioningException('git user.email not configured')
+        except Exception as exc:
+            raise VersioningException('git user.email not configured') from exc
 
     @property
     def repo_dir(self) -> str:
         """Return directory of repository."""
         return self.repo.path
 
     @property
@@ -65,40 +65,40 @@
         return self.repo.head.name
 
     def add_remote(
         self,
         name: str,
         url: str,
         fetch: Optional[str] = None,
-        **kwargs: Any,
+        # **kwargs: Any,
     ) -> None:
         """Add remote."""
         if name not in [x.name for x in self.repo.remotes]:
             if fetch is None:
                 fetch = f"+refs/heads/*:refs/remotes/{name}/*"
             self.repo.remotes.create(name, url, fetch)
         elif self.repo.remotes[name].url != url:
             self.repo.remotes.set_url(name, url)
 
     def commit(
         self,
         branch: Optional[str] = None,
-        filepaths: List[str] = [],
+        filepaths: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> Optional[Commit]:
         """Create commit."""
         ref = f"refs/heads/{branch}" if branch else self.ref
 
         author = Signature(self.username, self.email)
         committer = kwargs.get('commiter', author)
         message = kwargs.get('message', 'ci: bump version')
 
         # populate index
         index = self.repo.index
-        if filepaths == []:
+        if not filepaths:
             index.add_all()
         else:
             for filepath in filepaths:
                 index.add(
                     os.path.relpath(
                         filepath, os.path.join(self.repo.path, os.pardir)
                     )
```

### Comparing `proman-versioning-0.6.2a2/src/versioning/version.py` & `proman_versioning-0.6.2a4/src/versioning/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,40 +22,40 @@
 
     def __post_init__(self) -> None:
         """Initialize local version configuration."""
         self.states = ['non_local', 'local']
 
         # add build number
         self.transitions.append(
-            dict(
-                trigger='update_local',
-                source='non_local',
-                dest='local',
-                before='_update_local',
-            )
+            {
+                'trigger': 'update_local',
+                'source': 'non_local',
+                'dest': 'local',
+                'before': '_update_local',
+            }
         )
 
         # update build number
         self.transitions.append(
-            dict(
-                trigger='update_local',
-                source='local_local',
-                dest='=',
-                before='_update_local',
-            )
+            {
+                'trigger': 'update_local',
+                'source': 'local_local',
+                'dest': '',
+                'before': '_update_local',
+            }
         )
 
         # remove build number
         self.transitions.append(
-            dict(
-                trigger='update_local',
-                source='local',
-                dest='non_local',
-                before='_update_local',
-            )
+            {
+                'trigger': 'update_local',
+                'source': 'local',
+                'dest': 'non_local',
+                'before': '_update_local',
+            }
         )
 
 
 @dataclass
 class ReleaseConfig:
     """Manage versioning flow."""
 
@@ -65,198 +65,198 @@
 
     def __post_init__(self, default_release_type: str) -> None:
         """Initialize versioning config."""
         self.states = ['dev', 'alpha', 'beta', 'candidate', 'final', 'post']
 
         # XXX: need to calver as alternative first
         # self.transitions.append(
-        #     dict(
-        #         trigger='bump_epoch',
-        #         source='*',
-        #         dest=default_release_type,
-        #         before='_bump_epoch',
-        #         after='new_release',
-        #         conditions=['autostart_default_release'],
-        #     )
+        #     {
+        #         'trigger': 'bump_epoch',
+        #         'source': '*',
+        #         'dest': default_release_type,
+        #         'before': '_bump_epoch',
+        #         'after': 'new_release',
+        #         'conditions': ['autostart_default_release'],
+        #     }
         # )
 
         self.transitions.append(
-            dict(
-                trigger='bump_major',
-                source='*',
-                dest=default_release_type,
-                before='_bump_major',
-                after='new_release',
-                conditions=['autostart_default_release'],
-            )
+            {
+                'trigger': 'bump_major',
+                'source': '*',
+                'dest': default_release_type,
+                'before': '_bump_major',
+                'after': 'new_release',
+                'conditions': ['autostart_default_release'],
+            }
         )
 
         self.transitions.append(
-            dict(
-                trigger='bump_minor',
-                source='*',
-                dest=default_release_type,
-                before='_bump_minor',
-                after='new_release',
-                conditions=['autostart_default_release'],
-            )
+            {
+                'trigger': 'bump_minor',
+                'source': '*',
+                'dest': default_release_type,
+                'before': '_bump_minor',
+                'after': 'new_release',
+                'conditions': ['autostart_default_release'],
+            }
         )
 
         self.transitions.append(
-            dict(
-                trigger='bump_micro',
-                source='*',
-                dest=default_release_type,
-                before='_bump_micro',
-                after='new_release',
-                conditions=['autostart_default_release'],
-            )
+            {
+                'trigger': 'bump_micro',
+                'source': '*',
+                'dest': default_release_type,
+                'before': '_bump_micro',
+                'after': 'new_release',
+                'conditions': ['autostart_default_release'],
+            }
         )
 
         self.transitions.append(
-            dict(
-                trigger='bump_epoch',
-                source='*',
-                dest='final',
-                before='_bump_epoch',
-                # unless=['autostart_default_release'],
-            )
+            {
+                'trigger': 'bump_epoch',
+                'source': '*',
+                'dest': 'final',
+                'before': '_bump_epoch',
+                # 'unless': ['autostart_default_release'],
+            }
         )
 
         self.transitions.append(
-            dict(
-                trigger='bump_major',
-                source='*',
-                dest='final',
-                before='_bump_major',
-                unless=['autostart_default_release'],
-            )
+            {
+                'trigger': 'bump_major',
+                'source': '*',
+                'dest': 'final',
+                'before': '_bump_major',
+                'unless': ['autostart_default_release'],
+            }
         )
 
         self.transitions.append(
-            dict(
-                trigger='bump_minor',
-                source='*',
-                dest='final',
-                before='_bump_minor',
-                unless=['autostart_default_release'],
-            )
+            {
+                'trigger': 'bump_minor',
+                'source': '*',
+                'dest': 'final',
+                'before': '_bump_minor',
+                'unless': ['autostart_default_release'],
+            }
         )
 
         self.transitions.append(
-            dict(
-                trigger='bump_micro',
-                source='*',
-                dest='final',
-                before='_bump_micro',
-                unless=['autostart_default_release'],
-            )
+            {
+                'trigger': 'bump_micro',
+                'source': '*',
+                'dest': 'final',
+                'before': '_bump_micro',
+                'unless': ['autostart_default_release'],
+            }
         )
 
         # development releases
         self.transitions.append(
-            dict(
-                trigger='start_release',
-                source=['final', 'post'],
-                dest='dev',
-                before='_new_devrelease',
-                conditions=['enable_devreleases'],
-            )
+            {
+                'trigger': 'start_release',
+                'source': ['final', 'post'],
+                'dest': 'dev',
+                'before': '_new_devrelease',
+                'conditions': ['enable_devreleases'],
+            }
         )
 
         # pre-releases
         self.transitions.append(
-            dict(
-                trigger='start_release',
-                source=['final', 'post'],
-                dest='alpha',
-                before='_new_prerelease',
-                conditions=['enable_prereleases'],
-                unless=['enable_devreleases'],
-            )
-        )
-        self.transitions.append(
-            dict(
-                trigger='start_release',
-                source='dev',
-                dest='alpha',
-                before='_new_prerelease',
-                conditions=['enable_devreleases', 'enable_prereleases'],
-            )
-        )
-        self.transitions.append(
-            dict(
-                trigger='start_release',
-                source='alpha',
-                dest='beta',
-                before='_new_prerelease',
-                conditions=['enable_prereleases'],
-            )
-        )
-        self.transitions.append(
-            dict(
-                trigger='start_release',
-                source='beta',
-                dest='candidate',
-                before='_new_prerelease',
-                conditions=['enable_prereleases'],
-            )
+            {
+                'trigger': 'start_release',
+                'source': ['final', 'post'],
+                'dest': 'alpha',
+                'before': '_new_prerelease',
+                'conditions': ['enable_prereleases'],
+                'unless': ['enable_devreleases'],
+            }
+        )
+        self.transitions.append(
+            {
+                'trigger': 'start_release',
+                'source': 'dev',
+                'dest': 'alpha',
+                'before': '_new_prerelease',
+                'conditions': ['enable_devreleases', 'enable_prereleases'],
+            }
+        )
+        self.transitions.append(
+            {
+                'trigger': 'start_release',
+                'source': 'alpha',
+                'dest': 'beta',
+                'before': '_new_prerelease',
+                'conditions': ['enable_prereleases'],
+            }
+        )
+        self.transitions.append(
+            {
+                'trigger': 'start_release',
+                'source': 'beta',
+                'dest': 'candidate',
+                'before': '_new_prerelease',
+                'conditions': ['enable_prereleases'],
+            }
         )
 
         # final release
         self.transitions.append(
-            dict(
-                trigger='start_release',
-                source='dev',
-                dest='final',
-                before='_finalize_release',
-                conditions=['enable_devreleases'],
-                unless=['enable_prereleases'],
-            )
+            {
+                'trigger': 'start_release',
+                'source': 'dev',
+                'dest': 'final',
+                'before': '_finalize_release',
+                'conditions': ['enable_devreleases'],
+                'unless': ['enable_prereleases'],
+            }
         )
 
         self.transitions.append(
-            dict(
-                trigger='start_release',
-                source='candidate',
-                dest='final',
-                before='_finalize_release',
-                conditions=['enable_prereleases'],
-            )
-        )
-        self.transitions.append(
-            dict(
-                trigger='start_release',
-                source='post',
-                dest='final',
-                before='_finalize_release',
-                conditions=['enable_postreleases'],
-                unless=['enable_devreleases', 'enable_prereleases'],
-            )
+            {
+                'trigger': 'start_release',
+                'source': 'candidate',
+                'dest': 'final',
+                'before': '_finalize_release',
+                'conditions': ['enable_prereleases'],
+            }
+        )
+        self.transitions.append(
+            {
+                'trigger': 'start_release',
+                'source': 'post',
+                'dest': 'final',
+                'before': '_finalize_release',
+                'conditions': ['enable_postreleases'],
+                'unless': ['enable_devreleases', 'enable_prereleases'],
+            }
         )
 
         # post-releases
         self.transitions.append(
-            dict(
-                trigger='start_postrelease',
-                source='final',
-                dest='post',
-                before='_new_postrelease',
-                conditions=['enable_postreleases'],
-            )
+            {
+                'trigger': 'start_postrelease',
+                'source': 'final',
+                'dest': 'post',
+                'before': '_new_postrelease',
+                'conditions': ['enable_postreleases'],
+            }
         )
 
         # bump release number
         self.transitions.append(
-            dict(
-                trigger='bump_release',
-                source='*',
-                dest=None,
-                before='_bump_release',
-            )
+            {
+                'trigger': 'bump_release',
+                'source': '*',
+                'dest': None,
+                'before': '_bump_release',
+            }
         )
 
 
 class Version(PackageVersion):
     """Provide PEP440 compliant versioning."""
 
     def __init__(self, version: str, **kwargs: Any) -> None:
@@ -335,33 +335,32 @@
     def release_type(self) -> str:
         """Get the current state of package release."""
         if self.is_devrelease:
             state = 'dev'
         elif self.is_prerelease and self.pre:
             if self.pre[0] == 'a':
                 return 'alpha'
-            elif self.pre[0] == 'b':
+            if self.pre[0] == 'b':
                 return 'beta'
-            elif self.pre[0] == 'rc':
+            if self.pre[0] == 'rc':
                 return 'candidate'
         elif self.is_postrelease:
             state = 'post'
         else:
             state = 'final'
         return state
 
     @property
     def default_release_type(self) -> str:
         """Get the starting release type."""
         if self.enable_devreleases:
             return 'dev'
-        elif self.enable_prereleases:
+        if self.enable_prereleases:
             return 'alpha'
-        else:
-            return 'final'
+        return 'final'
 
     @property
     def query(self) -> str:
         """Get PEP-440 compliant regex query for version."""
         r = '.'.join(str(x) for x in self.release)
         if self.dev:
             v = f"{r}[-_\\.]?dev[-_\\.]?{self.dev or '0?'}"
@@ -375,27 +374,26 @@
                 v = f"{r}[-_\\.]?(?:a|alpha)[-_\\.]?{inst or '0?'}"
             if pre == 'b':
                 v = f"{r}[-_\\.]?(?:b|beta)[-_\\.]?{inst or '0?'}"
             if pre == 'rc':
                 candidate = 'c|candidate|rc|release'
                 v = f"{r}[-_\\.]?(?:{candidate})[-_\\.]?{inst or '0?'}"
             return v
-        elif self.post:
+        if self.post:
             v = f"{r}[-_\\.]?(?:post[-_\\.]?)?{self.post}"
             return v
-        else:
-            return str(self)
+        return str(self)
 
     def __update_version(
         self,
         epoch: Optional[int] = None,
         release: Optional[Tuple[Any, ...]] = None,
-        pre: Optional[Tuple[str, Optional[int]]] = None,
-        post: Optional[Tuple[Optional[str], Optional[int]]] = None,
-        dev: Optional[Tuple[str, Optional[int]]] = None,
+        pre: Optional[Tuple[str, int]] = None,
+        post: Optional[Tuple[str, int]] = None,
+        dev: Optional[Tuple[str, int]] = None,
         local: Optional[str] = None,
     ) -> None:
         """Update the internal version state."""
         if not (epoch or release):
             pre = pre or self.pre
             post = post or (None if self.post is None else ('post', self.post))
             dev = dev or (None if self.dev is None else ('dev', self.dev))
```

