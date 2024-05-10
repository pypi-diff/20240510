# Comparing `tmp/skillsnetwork_jupyter_extension-2.3.0rc1.tar.gz` & `tmp/skillsnetwork_jupyter_extension-2.3.0rc2.tar.gz`

## Comparing `skillsnetwork_jupyter_extension-2.3.0rc1.tar` & `skillsnetwork_jupyter_extension-2.3.0rc2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.copier-answers.yml
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.prettierignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.tool-versions
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.whitesource
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.yarnrc.yml
--rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/CHANGELOG.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/CODEOWNERS
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/RELEASE.md
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/install.json
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/setup.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/tsconfig.json
--rw-r--r--   0        0        0   227036 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/yarn.lock
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/jupyter-config/server-config/skillsnetwork_jupyter_extension.json
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/schema/toolbar.json
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/__init__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/_version.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/handlers.py
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/package.json
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json
--rw-r--r--   0        0        0    21440 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/496.6b8b1c179401632c8943.js
--rw-r--r--   0        0        0    30112 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/736.1176de539f275bcd21aa.js
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/956.9f7a54c8b777ce434d6b.js
--rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.1114a7d16c81f17285d7.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/style.js
--rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/config.ts
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/dialog.ts
--rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/handler.ts
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/index.ts
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/sn-file-library.ts
--rw-r--r--   0        0        0    23077 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/tools.ts
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/menu/index.ts
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/theme/index.ts
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/src/toolbar/index.ts
--rw-r--r--   0        0        0   880991 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/static/extension_demo.gif
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/style/index.js
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/LICENSE
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/README.md
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0    19094 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.copier-answers.yml
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.prettierignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.tool-versions
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.whitesource
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.yarnrc.yml
+-rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/CHANGELOG.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/CODEOWNERS
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/RELEASE.md
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/install.json
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/setup.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/tsconfig.json
+-rw-r--r--   0        0        0   227036 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/yarn.lock
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/jupyter-config/server-config/skillsnetwork_jupyter_extension.json
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/schema/toolbar.json
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/_version.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/handlers.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/package.json
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json
+-rw-r--r--   0        0        0    21429 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/496.0bb690d99ba98d842975.js
+-rw-r--r--   0        0        0    30112 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/736.7b5f76df818add15df8b.js
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/956.9f7a54c8b777ce434d6b.js
+-rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.12441616b46d94b2507f.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/config.ts
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/dialog.ts
+-rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/handler.ts
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/index.ts
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/sn-file-library.ts
+-rw-r--r--   0        0        0    23531 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/tools.ts
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/menu/index.ts
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/theme/index.ts
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/src/toolbar/index.ts
+-rw-r--r--   0        0        0   880991 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/static/extension_demo.gif
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/style/index.js
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/LICENSE
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/README.md
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    19094 2020-02-02 00:00:00.000000 skillsnetwork_jupyter_extension-2.3.0rc2/PKG-INFO
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/.copier-answers.yml` & `skillsnetwork_jupyter_extension-2.3.0rc2/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/CHANGELOG.md` & `skillsnetwork_jupyter_extension-2.3.0rc2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
-## 2.3.0rc1
+## 2.3.0rc2
 
 No merged PRs
 
 <!-- <END NEW CHANGELOG ENTRY> -->
 
+## 2.3.0rc1
+
+No merged PRs
+
 ## 2.3.0rc0
 
 No merged PRs
 
 ## 2.2.0
 
 ([Full Changelog](https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension/compare/v2.1.0...6ecc041eaf538ff525cd250c17eed9a45350b4f6))
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/CODEOWNERS` & `skillsnetwork_jupyter_extension-2.3.0rc2/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/RELEASE.md` & `skillsnetwork_jupyter_extension-2.3.0rc2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/package.json` & `skillsnetwork_jupyter_extension-2.3.0rc2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'2.3.0-rc2'"}*

```diff
@@ -202,9 +202,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.3.0-rc1"
+    "version": "2.3.0-rc2"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/tsconfig.json` & `skillsnetwork_jupyter_extension-2.3.0rc2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/yarn.lock` & `skillsnetwork_jupyter_extension-2.3.0rc2/yarn.lock`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/schema/toolbar.json` & `skillsnetwork_jupyter_extension-2.3.0rc2/schema/toolbar.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/__init__.py` & `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/handlers.py` & `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/handlers.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/package.json` & `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9788194444444445%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.12441616b46d94b2507f.js'}}",*

 * * "'version'": "'2.3.0-rc2'"}*

```diff
@@ -111,15 +111,15 @@
         "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1114a7d16c81f17285d7.js",
+            "load": "static/remoteEntry.12441616b46d94b2507f.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "skillsnetwork_jupyter_extension"
                 },
@@ -207,9 +207,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.3.0-rc1"
+    "version": "2.3.0-rc2"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig` & `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'2.3.0-rc2'"}*

```diff
@@ -202,9 +202,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "2.3.0-rc1"
+    "version": "2.3.0-rc2"
 }
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json` & `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/schemas/skillsnetwork_jupyter_extension/toolbar.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/496.6b8b1c179401632c8943.js` & `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/496.0bb690d99ba98d842975.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -16,15 +16,15 @@
                         mW: () => a,
                         o7: () => p,
                         qK: () => b,
                         sd: () => _,
                         wr: () => f,
                         xy: () => h
                     });
-                    var a, i, r = o(420);
+                    var a, i, r = o(400);
                     ! function(e) {
                         e.JUPYTERLAB = "jupyterlab", e.JUPYTERLITE = "jupyterlite", e.LOCAL = "local"
                     }(a || (a = {})),
                     function(e) {
                         e.LEARN = "learn", e.AUTHOR = "author"
                     }(i || (i = {}));
                     const e = e => {
@@ -87,15 +87,15 @@
                 KQ: () => d,
                 Sc: () => l,
                 WA: () => s,
                 Zm: () => u,
                 g3: () => c
             });
             var n = o(760),
-                a = o(300);
+                a = o(532);
             class i extends n.Widget {
                 constructor() {
                     const e = document.createElement("div"),
                         t = new a.Spinner;
                     e.appendChild(t.node), e.style.padding = "15px", super({
                         node: e
                     })
@@ -165,15 +165,15 @@
                         iU: () => _,
                         k5: () => k,
                         uU: () => f
                     });
                     var a = o(637),
                         i = o.n(a),
                         r = o(780),
-                        l = o(300),
+                        l = o(532),
                         s = o(904),
                         c = o(96),
                         d = o(500),
                         u = o.n(d),
                         h = o(416),
                         g = o.n(h),
                         p = e([s, c]);
@@ -276,20 +276,20 @@
         },
         964: (e, t, o) => {
             o.a(e, (async (e, n) => {
                 try {
                     o.d(t, {
                         c: () => b
                     });
-                    var a = o(452),
+                    var a = o(805),
                         i = o(760),
-                        r = o(300),
-                        l = o(628),
-                        s = o(736),
-                        c = o(188),
+                        r = o(532),
+                        l = o(88),
+                        s = o(0),
+                        c = o(569),
                         d = o(780),
                         u = o(904),
                         h = o(96),
                         g = o(416),
                         p = o.n(g),
                         w = e([u, h]);
                     [u, h] = w.then ? (await w)() : w;
@@ -398,15 +398,15 @@
             o.d(t, {
                 c: () => n
             });
             const n = {
                 id: "skillsnetwork_jupyter_extension:theme",
                 description: "Theme toggle plugin for Skills Network Authoring Extension",
                 autoStart: !0,
-                requires: [o(300).IThemeManager],
+                requires: [o(532).IThemeManager],
                 activate: (e, t) => {
                     console.log("Activating skillsnetwork_jupyter_extension theme toggle plugin!"), window.addEventListener("message", (e => {
                             "update_theme" === e.data.type && (console.log("Message received in the iframe:", e.data), "light" === e.data.color ? t.setTheme("JupyterLab Light") : t.setTheme("JupyterLab Dark"))
                         })),
                         function() {
                             try {
                                 return window.self !== window.top
@@ -421,27 +421,27 @@
         },
         808: (e, t, o) => {
             o.a(e, (async (e, n) => {
                 try {
                     o.d(t, {
                         c: () => k
                     });
-                    var a = o(736),
-                        i = o(188),
-                        r = o(300),
+                    var a = o(0),
+                        i = o(569),
+                        r = o(532),
                         l = o(96),
                         s = o(508),
                         c = o(480),
                         d = o(780),
                         u = o(904),
                         h = o(416),
                         g = o.n(h),
-                        p = o(628),
+                        p = o(88),
                         w = o(864),
-                        b = o(468),
+                        b = o(252),
                         m = e([u, c, l, w]);
                     [u, c, l, w] = m.then ? (await m)() : m;
                     const f = {
                         id: "skillsnetwork_jupyter_extension:toolbar",
                         description: "Toolbar plugin for Skills Network Authoring Extension",
                         autoStart: !0,
                         requires: [p.INotebookTracker, a.IDocumentManager, i.IDefaultFileBrowser],
@@ -509,19 +509,17 @@
                                 } catch (e) {
                                     console.error("Error opening lab:", e), r.Dialog.flush(), (0, d.Zm)()
                                 }
                             }))) : console.log("No valid notebook URL found..."))
                         }
                         const i = u.qK,
                             s = u.AP;
-                        console.log("skillsnetwork_jupyter_extension:toolbar extension activated"), e.docRegistry.addWidgetExtension("Notebook", new _);
-                        let c = "";
-                        null !== u.aQ && (c = (0, l.eC)(u.aQ), console.log("Authoring lab file path:", c)), await e.serviceManager.ready, e.restored.then((async () => {
+                        console.log("skillsnetwork_jupyter_extension:toolbar extension activated"), e.docRegistry.addWidgetExtension("Notebook", new _), await e.serviceManager.ready, e.restored.then((async () => {
                             if (await y(t), a !== u.mW.LOCAL && ("NO_TOKEN" !== i || "NO_TOKEN" !== s)) try {
-                                await (0, l.UJ)(i, s, c, o, e.serviceManager.contents, n)
+                                await (0, l.UJ)(i, s, u.aQ, o, e.serviceManager.contents, n)
                             } catch (e) {
                                 console.error("Error opening lab with Atlas/AWB token:", e), r.Dialog.flush(), (0, d.Zm)()
                             }
                         }))
                     }
                     const k = f;
                     n()
@@ -531,20 +529,19 @@
             }))
         },
         96: (e, t, o) => {
             o.a(e, (async (e, n) => {
                 try {
                     o.d(t, {
                         UJ: () => m,
-                        eC: () => E,
                         gv: () => u,
                         ol: () => g,
                         wO: () => f
                     });
-                    var a = o(300),
+                    var a = o(532),
                         i = o(944),
                         r = o(904),
                         l = o(480),
                         s = e([r, l]);
                     [r, l] = s.then ? (await s)() : s;
                     const c = e => {
                             const t = e.model.toJSON().source,
@@ -654,15 +651,19 @@
                                 if ("NO_TOKEN" === t) throw Error("No valid token found.");
                                 ({
                                     labFilename: u,
                                     body: d
                                 } = await (0, l.uU)((0, l.CU)(t), t)), g = t
                             }
                             let p = `${u}`;
-                            p = i.C.join(o, p), p.includes("/") ? (await h(n, p), s.model.path !== o && (console.log(`Opening /${o} in file browser`), await s.model.cd(`/${o}`))) : await s.model.cd("/");
+                            if (null !== o && (p = E(o, u)), console.log("Opening lab:", p), p.includes("/")) {
+                                await h(n, p);
+                                const e = i.C.dirname(p);
+                                s.model.path !== e && (console.log(`Opening /${e} in the file browser`), await s.model.cd(`/${e}`))
+                            } else await s.model.cd("/");
                             let w, b = p;
                             return r.Ut !== r.mW.JUPYTERLITE ? (b = `./${p}`, await v(p, a, n), await _(b, d, a, n)) : await n.deleteFile(b), r.Gq.SHOW_PUBLISH_BUTTON_FOR = p, r.Gq.TOKENS.set(p, g), w = await L(b, a) ? n.openOrReveal(p) : await y(n, p, "NO_TOKEN" !== e ? JSON.parse(d) : d), w
                         }, f = async (e, t, o, n, i) => {
                             const r = await (0, l.Oc)(e),
                                 s = r.data;
                             if (!S(s)) throw Error(`content of ${e} is not a valid JSON! Please let the author know about this issue!`);
                             const c = Date.parse(r.headers["last-modified"] || "");
@@ -683,15 +684,15 @@
                             });
                             if (void 0 === n) throw Error("Error loading lab");
                             return await k(n, o), n
                         };
                     async function _(e, t, o, n) {
                         const i = await L(e, o);
                         if (i && p(t) !== p(i)) try {
-                            await U(i, o, n), await (0, a.showDialog)({
+                            await A(i, o, n), await (0, a.showDialog)({
                                 title: "Your Lab was Updated",
                                 body: `The newest published version of "${e}" is loaded. Your previous version has been backed up under "${e}${r.Gq.BACKUP_EXT}.ipynb"`,
                                 buttons: [a.Dialog.okButton({
                                     label: "Dismiss"
                                 })]
                             })
                         } catch (t) {
@@ -702,28 +703,28 @@
                                     label: "Dismiss"
                                 })]
                             })
                         }
                     }
                     async function v(e, t, o) {
                         const n = await L(e, t);
-                        n && (await A(e, o), w(n) && await t.delete(e))
+                        n && (await U(e, o), w(n) && await t.delete(e))
                     }
                     const k = async (e, t, o) => {
                         if (await e.context.ready, o !== r.mW.LOCAL) {
                             e.context.model.fromJSON(t);
                             try {
                                 await e.context.save()
                             } catch (e) {
                                 console.error("[loadLabContents] Error saving notebook:", e)
                             }
                         } else console.error("[loadLabContents] Notebook model is not initialized or environment is local.")
-                    }, E = e => {
-                        let t = e;
-                        return "" !== i.C.extname(e) && (t = i.C.dirname(e)), t = i.C.removeSlash(t), t.replace(/\/+$/, "")
+                    }, E = (e, t) => {
+                        let o = e;
+                        return e.includes(t) || ("" !== i.C.extname(e) && (o = i.C.dirname(e)), o = i.C.join(o, t)), i.C.removeSlash(o)
                     };
                     async function L(e, t) {
                         try {
                             return await t.get(e)
                         } catch (e) {
                             if (e instanceof Error) {
                                 const t = e;
@@ -737,24 +738,24 @@
                         const o = t.findWidget(e);
                         if (o) try {
                             o.context.model.dirty && await o.context.save(), o.close()
                         } catch (e) {
                             console.error("[saveAndCloseOpenFiles] Error saving or closing widget:", e)
                         }
                     }
-                    async function A(e, t) {
+                    async function U(e, t) {
                         const o = t.findWidget(e);
                         if (o) try {
                             const e = t.contextForWidget(o);
                             e && e.model && (e.model.dirty = !1), o.close()
                         } catch (e) {
                             console.error("[closeWithoutSaving] Error closing widget:", e)
                         }
                     }
-                    async function U(e, t, o) {
+                    async function A(e, t, o) {
                         const n = e.path,
                             a = n.split(".").pop(),
                             i = `${n.replace(/\.[^/.]+$/,"")}${r.Gq.BACKUP_EXT}.${a}`;
                         if (await L(i, t)) try {
                             await t.delete(i)
                         } catch (e) {
                             console.error("[convertFileToBackup] Error deleting existing backup file:", e)
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js` & `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/636.605077303a876f967661.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js` & `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/648.64f5e2269a630e211878.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/736.1176de539f275bcd21aa.js` & `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/736.7b5f76df818add15df8b.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -172,15 +172,15 @@
                 if (t.styleSheet) t.styleSheet.cssText = e;
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
-        355: (e, t, n) => {
+        736: (e, t, n) => {
             n.r(t);
             var r = n(596),
                 o = n.n(r),
                 a = n(520),
                 s = n.n(a),
                 c = n(176),
                 i = n.n(c),
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js` & `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/944.dddd8170d5a83693b53a.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.1114a7d16c81f17285d7.js` & `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/remoteEntry.12441616b46d94b2507f.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, b, v, m, y, g, w, _, k, j, S = {
+    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v, b, m, y, g, w, _, k, j, S = {
             344: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(944), t.e(496)]).then((() => () => t(496))),
                         "./extension": () => Promise.all([t.e(944), t.e(496)]).then((() => () => t(496))),
-                        "./style": () => t.e(736).then((() => () => t(355)))
+                        "./style": () => t.e(736).then((() => () => t(736)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -83,25 +83,25 @@
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
-        496: "6b8b1c179401632c8943",
+        496: "0bb690d99ba98d842975",
         636: "605077303a876f967661",
         648: "64f5e2269a630e211878",
-        736: "1176de539f275bcd21aa",
+        736: "7b5f76df818add15df8b",
         944: "dddd8170d5a83693b53a",
         956: "9f7a54c8b777ce434d6b"
     } [e] + ".js?v=" + {
-        496: "6b8b1c179401632c8943",
+        496: "0bb690d99ba98d842975",
         636: "605077303a876f967661",
         648: "64f5e2269a630e211878",
-        736: "1176de539f275bcd21aa",
+        736: "7b5f76df818add15df8b",
         944: "dddd8170d5a83693b53a",
         956: "9f7a54c8b777ce434d6b"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -155,15 +155,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("axios", "1.6.7", (() => E.e(636).then((() => () => E(636))))), u("form-data", "4.0.0", (() => E.e(956).then((() => () => E(956))))), u("jwt-decode", "3.1.2", (() => E.e(648).then((() => () => E(648))))), u("skillsnetwork_jupyter_extension", "2.3.0-rc1", (() => Promise.all([E.e(944), E.e(496)]).then((() => () => E(496)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("axios", "1.6.7", (() => E.e(636).then((() => () => E(636))))), u("form-data", "4.0.0", (() => E.e(956).then((() => () => E(956))))), u("jwt-decode", "3.1.2", (() => E.e(648).then((() => () => E(648))))), u("skillsnetwork_jupyter_extension", "2.3.0-rc2", (() => Promise.all([E.e(944), E.e(496)]).then((() => () => E(496)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -250,41 +250,41 @@
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && u(e, r) ? r : e), 0)
     }, p = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + l(n) + ")", c = (e, r, t, n) => {
         var o = d(e, t);
-        return f(n, o) || b(p(e, t, o, n)), v(e[t][o])
+        return f(n, o) || v(p(e, t, o, n)), b(e[t][o])
     }, h = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !f(t, r) || e && !u(e, r) ? e : r), 0)) && n[r]
-    }, b = e => {
+    }, v = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, v = e => (e.loaded = 1, e.get()), y = (m = e => function(r, t, n, o) {
+    }, b = e => (e.loaded = 1, e.get()), y = (m = e => function(r, t, n, o) {
         var a = E.I(r);
         return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
     })(((e, r, t, n) => (s(e, t), c(r, 0, t, n)))), g = m(((e, r, t, n, o) => {
         var a = r && E.o(r, t) && h(r, t, n);
-        return a ? v(a) : o()
+        return a ? b(a) : o()
     })), w = {}, _ = {
-        188: () => y("default", "@jupyterlab/filebrowser", [1, 4, 1, 8]),
-        300: () => y("default", "@jupyterlab/apputils", [1, 4, 2, 8]),
+        0: () => y("default", "@jupyterlab/docmanager", [1, 4, 2, 0]),
+        88: () => y("default", "@jupyterlab/notebook", [1, 4, 2, 0]),
+        252: () => y("default", "@jupyterlab/coreutils", [1, 6, 2, 0]),
+        400: () => y("default", "@jupyterlab/services", [1, 7, 2, 0]),
         416: () => g("default", "jwt-decode", [1, 3, 1, 2], (() => E.e(648).then((() => () => E(648))))),
-        420: () => y("default", "@jupyterlab/services", [1, 7, 1, 8]),
-        452: () => y("default", "@jupyterlab/mainmenu", [1, 4, 1, 8]),
-        468: () => y("default", "@jupyterlab/coreutils", [1, 6, 1, 8]),
         500: () => g("default", "axios", [1, 1, 6, 0], (() => E.e(636).then((() => () => E(636))))),
         508: () => y("default", "@lumino/disposable", [1, 2, 0, 0]),
-        628: () => y("default", "@jupyterlab/notebook", [1, 4, 1, 8]),
+        532: () => y("default", "@jupyterlab/apputils", [1, 4, 3, 0]),
+        569: () => y("default", "@jupyterlab/filebrowser", [1, 4, 2, 0]),
         637: () => g("default", "form-data", [1, 4, 0, 0], (() => E.e(956).then((() => () => E(956))))),
-        736: () => y("default", "@jupyterlab/docmanager", [1, 4, 1, 8]),
-        760: () => y("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0])
+        760: () => y("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
+        805: () => y("default", "@jupyterlab/mainmenu", [1, 4, 2, 0])
     }, k = {
-        496: [188, 300, 416, 420, 452, 468, 500, 508, 628, 637, 736, 760]
+        496: [0, 88, 252, 400, 416, 500, 508, 532, 569, 637, 760, 805]
     }, j = {}, E.f.consumes = (e, r) => {
         E.o(k, e) && k[e].forEach((e => {
             if (E.o(w, e)) return r.push(w[e]);
             if (!j[e]) {
                 var t = r => {
                     w[e] = 0, E.m[e] = t => {
                         delete E.c[e], t.exports = r()
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json` & `skillsnetwork_jupyter_extension-2.3.0rc2/skillsnetwork_jupyter_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/src/config.ts` & `skillsnetwork_jupyter_extension-2.3.0rc2/src/config.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/src/dialog.ts` & `skillsnetwork_jupyter_extension-2.3.0rc2/src/dialog.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/src/handler.ts` & `skillsnetwork_jupyter_extension-2.3.0rc2/src/handler.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/src/sn-file-library.ts` & `skillsnetwork_jupyter_extension-2.3.0rc2/src/sn-file-library.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/src/tools.ts` & `skillsnetwork_jupyter_extension-2.3.0rc2/src/tools.ts`

 * *Files 2% similar despite different names*

```diff
@@ -273,24 +273,24 @@
 };
 
 /**
  * Opens a lab from Atlas or AWB
  *
  * @param atlas_token the Atlas token (or 'NO_TOKEN')
  * @param awb_token the AWB token (or 'NO_TOKEN')
- * @param dirPath the directory path to open the lab in
+ * @param filePathArg the path to open the lab in
  * @param docManager the JupyterLab document manager
  * @param contentsManager the JupyterLab contents manager
  * @param fileBrowser the JupyterLab file browser
  * @returns the notebook panel
  */
 export const openLab = async (
   atlas_token: string,
   awb_token: string,
-  dirPath: string,
+  filePathArg: string | null,
   docManager: IDocumentManager,
   contentsManager: Contents.IManager,
   fileBrowser: IDefaultFileBrowser
 ): Promise<NotebookPanel> => {
   let instructions_file_path: string;
   let instructions_content: string;
   let labFilename: string;
@@ -308,22 +308,28 @@
     ));
     token = awb_token;
   } else {
     throw Error('No valid token found.');
   }
 
   let filePath = `${labFilename}`;
-  filePath = PathExt.join(dirPath, filePath);
+
+  if (filePathArg !== null) {
+    filePath = getAuthorLabFilePath(filePathArg, labFilename);
+  }
+
+  console.log('Opening lab:', filePath);
 
   // This allows both the dirPath and lab filename to include a path to create subfolders
   if (filePath.includes('/')) {
     await ensureSubFoldersExist(docManager, filePath);
+    const dirPath = PathExt.dirname(filePath);
 
     if (fileBrowser.model.path !== dirPath) {
-      console.log(`Opening /${dirPath} in file browser`);
+      console.log(`Opening /${dirPath} in the file browser`);
       await fileBrowser.model.cd(`/${dirPath}`);
     }
   } else {
     await fileBrowser.model.cd('/');
   }
 
   let potentialRelativePath = filePath;
@@ -575,26 +581,36 @@
     console.error(
       '[loadLabContents] Notebook model is not initialized or environment is local.'
     );
   }
 };
 
 /**
- * Takes a file path and returns the directory path (no filename if it was included)
- * @param filePath
+ * Takes the file path and the lab filename and returns the full lab file path
+ *
+ * @param filePath the file path (may or may not include the lab filename)
+ * @param labFilename the lab filename (may include one or more directories)
+ * @returns the full lab file path
  */
-export const getAuthorLabFilePath = (filePath: string): string => {
-  let dir = filePath;
-  // Check if the path includes a filename and remove it if so
-  if (PathExt.extname(filePath) !== '') {
-    dir = PathExt.dirname(filePath);
-  }
-  dir = PathExt.removeSlash(dir);
-  // Remove any trailing slashes
-  return dir.replace(/\/+$/, '');
+export const getAuthorLabFilePath = (
+  filePath: string,
+  labFilename: string
+): string => {
+  let finalPath = filePath;
+
+  // See if the filePath includes the lab filename
+  if (!filePath.includes(labFilename)) {
+    // Check if the path includes a filename and remove it if so
+    if (PathExt.extname(filePath) !== '') {
+      finalPath = PathExt.dirname(filePath);
+    }
+    finalPath = PathExt.join(finalPath, labFilename);
+  }
+
+  return PathExt.removeSlash(finalPath);
 };
 
 /**
  * Renames a file to filename.backup.ipynb and overwrites any files with the same name.
  *
  * @param {string} path - path to string.
  * @param {ContentsManager} contentsManager - The JupyterLab contents manager.
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/src/menu/index.ts` & `skillsnetwork_jupyter_extension-2.3.0rc2/src/menu/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/src/theme/index.ts` & `skillsnetwork_jupyter_extension-2.3.0rc2/src/theme/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/src/toolbar/index.ts` & `skillsnetwork_jupyter_extension-2.3.0rc2/src/toolbar/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import { DocumentRegistry } from '@jupyterlab/docregistry';
 import { IDocumentManager } from '@jupyterlab/docmanager';
 import { IDefaultFileBrowser } from '@jupyterlab/filebrowser';
 import { Dialog, showDialog, ToolbarButton } from '@jupyterlab/apputils';
-import {
-  getFileContents,
-  getAuthorLabFilePath,
-  openLab,
-  openLearnerLab
-} from '../tools';
+import { getFileContents, openLab, openLearnerLab } from '../tools';
 import { IDisposable, DisposableDelegate } from '@lumino/disposable';
 import {
   atlasAxiosHandler,
   postAtlasLabModel,
   awbAxiosHandler,
   postAwbLabModel
 } from '../handler';
@@ -212,34 +207,27 @@
   const awb_token = AWB_TOKEN as string;
 
   console.log('skillsnetwork_jupyter_extension:toolbar extension activated');
 
   // Only show toolbar buttons for the lab that's launched via token
   app.docRegistry.addWidgetExtension('Notebook', new ButtonExtension());
 
-  let dirPath = '';
-
-  if (FILE_PATH !== null) {
-    dirPath = getAuthorLabFilePath(FILE_PATH);
-    console.log('Authoring lab file path:', dirPath);
-  }
-
   // Try to load up a notebook when author is using the browser tool (not in local)
   await app.serviceManager.ready;
   app.restored.then(async () => {
     await cleanUpEnvironment(notebookTracker);
     if (
       env_type !== EnvType.LOCAL &&
       (atlas_token !== 'NO_TOKEN' || awb_token !== 'NO_TOKEN')
     ) {
       try {
         await openLab(
           atlas_token,
           awb_token,
-          dirPath,
+          FILE_PATH,
           docManager,
           app.serviceManager.contents,
           fileBrowser
         );
       } catch (e) {
         console.error('Error opening lab with Atlas/AWB token:', e);
         Dialog.flush(); // remove spinner
```

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/static/extension_demo.gif` & `skillsnetwork_jupyter_extension-2.3.0rc2/static/extension_demo.gif`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/.gitignore` & `skillsnetwork_jupyter_extension-2.3.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/LICENSE` & `skillsnetwork_jupyter_extension-2.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/README.md` & `skillsnetwork_jupyter_extension-2.3.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/pyproject.toml` & `skillsnetwork_jupyter_extension-2.3.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skillsnetwork_jupyter_extension-2.3.0rc1/PKG-INFO` & `skillsnetwork_jupyter_extension-2.3.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: skillsnetwork_jupyter_extension
-Version: 2.3.0rc1
+Version: 2.3.0rc2
 Dynamic: Keywords
 Summary: JupterLab/JupyerLite extension for Skills Network Labs
 Project-URL: Homepage, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension
 Project-URL: Bug Tracker, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension/issues
 Project-URL: Repository, https://github.com/ibm-skills-network/skillsnetwork-jupyter-extension.git
 Author-email: IBM Skills Network <skills.network@ibm.com>
 License:                                  Apache License
```

