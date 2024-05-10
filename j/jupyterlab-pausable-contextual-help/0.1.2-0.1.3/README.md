# Comparing `tmp/jupyterlab_pausable_contextual_help-0.1.2.tar.gz` & `tmp/jupyterlab_pausable_contextual_help-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_pausable_contextual_help-0.1.2.tar", last modified: Thu Feb 23 14:32:24 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab_pausable_contextual_help-0.1.2.tar` & `jupyterlab_pausable_contextual_help-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-02-23 14:32:24.610241 jupyterlab_pausable_contextual_help-0.1.2/
--rw-rw-r--   0 frz       (1000) frz       (1000)       86 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/CHANGELOG.md
--rw-rw-r--   0 frz       (1000) frz       (1000)     1520 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/LICENSE
--rw-rw-r--   0 frz       (1000) frz       (1000)      442 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/MANIFEST.in
--rw-rw-r--   0 frz       (1000) frz       (1000)     3554 2023-02-23 14:32:24.610241 jupyterlab_pausable_contextual_help-0.1.2/PKG-INFO
--rw-rw-r--   0 frz       (1000) frz       (1000)     2431 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/README.md
--rw-rw-r--   0 frz       (1000) frz       (1000)     1917 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/RELEASE.md
--rw-rw-r--   0 frz       (1000) frz       (1000)      231 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/install.json
-drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-02-23 14:32:24.600241 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/
--rw-rw-r--   0 frz       (1000) frz       (1000)      321 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/__init__.py
--rw-rw-r--   0 frz       (1000) frz       (1000)      625 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/_version.py
-drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-02-23 14:32:24.610241 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/
--rw-rw-r--   0 frz       (1000) frz       (1000)    20226 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/build_log.json
--rw-rw-r--   0 frz       (1000) frz       (1000)     3989 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/package.json
-drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-02-23 14:32:24.600241 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/schemas/
-drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-02-23 14:32:24.610241 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/schemas/jupyterlab_pausable_contextual_help/
--rw-rw-r--   0 frz       (1000) frz       (1000)     1094 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/schemas/jupyterlab_pausable_contextual_help/inspector.json
--rw-rw-r--   0 frz       (1000) frz       (1000)     4242 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/schemas/jupyterlab_pausable_contextual_help/package.json.orig
-drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-02-23 14:32:24.610241 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/
--rw-rw-r--   0 frz       (1000) frz       (1000)    32048 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/lib_index_js.3589c3b38b1e1b0c1f10.js
--rw-rw-r--   0 frz       (1000) frz       (1000)    27840 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/lib_index_js.3589c3b38b1e1b0c1f10.js.map
--rw-rw-r--   0 frz       (1000) frz       (1000)    30725 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/remoteEntry.bba643b4b9733f60248c.js
--rw-rw-r--   0 frz       (1000) frz       (1000)    29836 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/remoteEntry.bba643b4b9733f60248c.js.map
--rw-rw-r--   0 frz       (1000) frz       (1000)      178 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/style.js
--rw-rw-r--   0 frz       (1000) frz       (1000)     6456 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/style_index_js.1eebcf1c283efc5e22d0.js
--rw-rw-r--   0 frz       (1000) frz       (1000)     3825 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/style_index_js.1eebcf1c283efc5e22d0.js.map
--rw-rw-r--   0 frz       (1000) frz       (1000)    12100 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.547b99950c80d08ebd47.js
--rw-rw-r--   0 frz       (1000) frz       (1000)    13853 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.547b99950c80d08ebd47.js.map
--rw-rw-r--   0 frz       (1000) frz       (1000)    26914 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/vendors-node_modules_lumino_polling_dist_index_es6_js.35868735457bf9c961c0.js
--rw-rw-r--   0 frz       (1000) frz       (1000)    48430 2023-02-23 14:22:01.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/vendors-node_modules_lumino_polling_dist_index_es6_js.35868735457bf9c961c0.js.map
-drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-02-23 14:32:24.610241 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help.egg-info/
--rw-rw-r--   0 frz       (1000) frz       (1000)     3554 2023-02-23 14:32:24.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help.egg-info/PKG-INFO
--rw-rw-r--   0 frz       (1000) frz       (1000)     2287 2023-02-23 14:32:24.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help.egg-info/SOURCES.txt
--rw-rw-r--   0 frz       (1000) frz       (1000)        1 2023-02-23 14:32:24.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help.egg-info/dependency_links.txt
--rw-rw-r--   0 frz       (1000) frz       (1000)        1 2023-02-23 13:48:25.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help.egg-info/not-zip-safe
--rw-rw-r--   0 frz       (1000) frz       (1000)       36 2023-02-23 14:32:24.000000 jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help.egg-info/top_level.txt
--rw-rw-r--   0 frz       (1000) frz       (1000)     4242 2023-02-23 14:31:51.000000 jupyterlab_pausable_contextual_help-0.1.2/package.json
--rw-rw-r--   0 frz       (1000) frz       (1000)      675 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/pyproject.toml
-drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-02-23 14:32:24.610241 jupyterlab_pausable_contextual_help-0.1.2/schema/
--rw-rw-r--   0 frz       (1000) frz       (1000)     1094 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/schema/inspector.json
--rw-rw-r--   0 frz       (1000) frz       (1000)       38 2023-02-23 14:32:24.610241 jupyterlab_pausable_contextual_help-0.1.2/setup.cfg
--rw-rw-r--   0 frz       (1000) frz       (1000)     2902 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/setup.py
-drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-02-23 14:32:24.610241 jupyterlab_pausable_contextual_help-0.1.2/src/
--rw-rw-r--   0 frz       (1000) frz       (1000)     7526 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/src/handler.ts
--rw-rw-r--   0 frz       (1000) frz       (1000)    12883 2023-02-23 14:21:33.000000 jupyterlab_pausable_contextual_help-0.1.2/src/index.ts
--rw-rw-r--   0 frz       (1000) frz       (1000)     4493 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/src/inspector.ts
--rw-rw-r--   0 frz       (1000) frz       (1000)     2154 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/src/kernelconnector.ts
--rw-rw-r--   0 frz       (1000) frz       (1000)     2020 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/src/tokens.ts
-drwxrwxr-x   0 frz       (1000) frz       (1000)        0 2023-02-23 14:32:24.610241 jupyterlab_pausable_contextual_help-0.1.2/style/
--rw-rw-r--   0 frz       (1000) frz       (1000)      436 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/style/base.css
--rw-rw-r--   0 frz       (1000) frz       (1000)     1315 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/style/index.css
--rw-rw-r--   0 frz       (1000) frz       (1000)     1213 2023-02-23 13:46:38.000000 jupyterlab_pausable_contextual_help-0.1.2/style/index.js
--rw-rw-r--   0 frz       (1000) frz       (1000)      554 2023-02-23 14:07:26.000000 jupyterlab_pausable_contextual_help-0.1.2/tsconfig.json
--rw-rw-r--   0 frz       (1000) frz       (1000)   216396 2023-02-23 14:04:46.000000 jupyterlab_pausable_contextual_help-0.1.2/yarn.lock
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/.copier-answers.yml
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/.gitattributes
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/RELEASE.md
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/install.json
+-rw-r--r--   0        0        0     6766 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/tsconfig.json
+-rw-r--r--   0        0        0   229145 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/yarn.lock
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/_version.py
+-rw-r--r--   0        0        0    22651 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/build_log.json
+-rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/package.json
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/schemas/jupyterlab_pausable_contextual_help/myinspector.json
+-rw-r--r--   0        0        0     6766 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/schemas/jupyterlab_pausable_contextual_help/package.json.orig
+-rw-r--r--   0        0        0   203030 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/373c04fd2418f5c77eea.eot
+-rw-r--r--   0        0        0   101648 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/3f6d3488cf65374f6f67.woff
+-rw-r--r--   0        0        0    34034 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/79d088064beb3826054f.eot
+-rw-r--r--   0        0        0    76736 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/8ea8791754915a898a31.woff2
+-rw-r--r--   0        0        0   918991 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/9674eb1bd55047179038.svg
+-rw-r--r--   0        0        0    78268 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/9834b82ad26e2a37583d.woff2
+-rw-r--r--   0        0        0   747927 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/a3b9817780214caf01e8.svg
+-rw-r--r--   0        0        0   202744 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/af6397503fcefbd61397.ttf
+-rw-r--r--   0        0        0   144714 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/be0a084962d8066884f7.svg
+-rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/cb9e9e693192413cde2b.woff
+-rw-r--r--   0        0        0   133988 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/cda59d6efffa685830fd.ttf
+-rw-r--r--   0        0        0   134294 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/e4299464e7b012968eed.eot
+-rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/e42a88444448ac3d6054.woff2
+-rw-r--r--   0        0        0    33736 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/e8711bbb871afd8e9dea.ttf
+-rw-r--r--   0        0        0    89988 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/f9217f66874b0c01cd8c.woff
+-rw-r--r--   0        0        0    33565 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/lib_index_js.48d46625a03ec356bfc7.js
+-rw-r--r--   0        0        0    45728 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/lib_index_js.48d46625a03ec356bfc7.js.map
+-rw-r--r--   0        0        0    31087 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/remoteEntry.f72bb70dee94e59ad703.js
+-rw-r--r--   0        0        0    30137 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/remoteEntry.f72bb70dee94e59ad703.js.map
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/style.js
+-rw-r--r--   0        0        0    15132 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/style_index_js-data_image_png_base64_iVBORw0KGgoAAAANSUhEUgAAAAgAAAAFCAYAAAB4ka1VAAAAsElEQVQI-adaf50.2b034a8fa2de53285adf.js
+-rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/style_index_js-data_image_png_base64_iVBORw0KGgoAAAANSUhEUgAAAAgAAAAFCAYAAAB4ka1VAAAAsElEQVQI-adaf50.2b034a8fa2de53285adf.js.map
+-rw-r--r--   0        0        0  1183941 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/vendors-node_modules_jupyterlab_application_style_index_js-node_modules_jupyterlab_console_st-8dc7b3.f3e7c133ec1940ded4f9.js
+-rw-r--r--   0        0        0  1060211 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/vendors-node_modules_jupyterlab_application_style_index_js-node_modules_jupyterlab_console_st-8dc7b3.f3e7c133ec1940ded4f9.js.map
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/schema/myinspector.json
+-rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/src/handler.ts
+-rw-r--r--   0        0        0    12472 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/src/index.ts
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/src/kernelconnector.ts
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/src/myinspector.ts
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/src/tokens.ts
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/style/base.css
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/style/index.css
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/style/index.js
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/README.md
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 jupyterlab_pausable_contextual_help-0.1.3/PKG-INFO
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/LICENSE` & `jupyterlab_pausable_contextual_help-0.1.3/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Feiran Zhang
+Copyright (c) 2024, Frz
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/PKG-INFO` & `jupyterlab_pausable_contextual_help-0.1.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,18 @@
-Metadata-Version: 2.1
-Name: jupyterlab_pausable_contextual_help
-Version: 0.1.2
-Summary: Customized Jupyterlab Contextual Help Panel That Allows Manually Update When Press F1.
-Home-page: https://github.com/zhangfeiran/jupyterlab_pausable_contextual_help
-Author: Feiran Zhang
-Author-email: feiranzhang@outlook.com
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Framework :: Jupyter
-Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
-Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # jupyterlab_pausable_contextual_help
 
+[![Github Actions Status](/workflows/Build/badge.svg)](/actions/workflows/build.yml)
+
 Customized Jupyterlab Contextual Help Panel That Allows Manually Update When Press F1.
 
 Auto update can still be enabled in the context menu.
 
 ## Requirements
 
-- JupyterLab >= 3.0
+- JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
 pip install jupyterlab_pausable_contextual_help
@@ -62,15 +36,15 @@
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
 # Change directory to the jupyterlab_pausable_contextual_help directory
 # Install package in development mode
-pip install -e .
+pip install -e "."
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Rebuild extension Typescript source after making changes
 jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/schemas/jupyterlab_pausable_contextual_help/package.json.orig` & `jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/package.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7082473987365293%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.2.0', '@jupyterlab/console': '^4.2.0', "*

 * *                   "'@jupyterlab/inspector': '^4.2.0', '@jupyterlab/launcher': '^4.2.0', "*

 * *                   "'@jupyterlab/notebook': '^4.2.0', '@jupyterlab/settingregistry': '^4.0.0', "*

 * *                   "delete: ['@jupyterlab/apputils', '@jupyterlab/translation', "*

 * *                   "'@jupyterlab/ui-components']}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@typescript-eslint/eslint-plugin': "*

 * *   […]*

```diff
@@ -3,111 +3,197 @@
         "email": "feiranzhang@outlook.com",
         "name": "Feiran Zhang"
     },
     "bugs": {
         "url": "https://github.com/zhangfeiran/jupyterlab_pausable_contextual_help/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.18",
-        "@jupyterlab/apputils": "^3.0.18",
-        "@jupyterlab/console": "^3.0.18",
-        "@jupyterlab/inspector": "^3.0.18",
-        "@jupyterlab/launcher": "^3.0.18",
-        "@jupyterlab/notebook": "^3.0.18",
-        "@jupyterlab/translation": "^3.0.18",
-        "@jupyterlab/ui-components": "^3.0.18"
+        "@jupyterlab/application": "^4.2.0",
+        "@jupyterlab/console": "^4.2.0",
+        "@jupyterlab/inspector": "^4.2.0",
+        "@jupyterlab/launcher": "^4.2.0",
+        "@jupyterlab/notebook": "^4.2.0",
+        "@jupyterlab/settingregistry": "^4.0.0"
     },
     "description": "Customized Jupyterlab Contextual Help Panel That Allows Manually Update When Press F1.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.18",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@types/react-addons-linked-state-mixin": "^0.14.22",
+        "@typescript-eslint/eslint-plugin": "^6.1.0",
+        "@typescript-eslint/parser": "^6.1.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^5.0.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
-        "stylelint-config-prettier": "^9.0.3",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
-        "typescript": "~4.1.3"
-    },
-    "directories": {
-        "lib": "lib/"
+        "prettier": "^3.0.0",
+        "rimraf": "^5.0.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^15.10.1",
+        "stylelint-config-recommended": "^13.0.0",
+        "stylelint-config-standard": "^34.0.0",
+        "stylelint-csstree-validator": "^3.0.0",
+        "stylelint-prettier": "^4.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.0"
+    },
+    "eslintConfig": {
+        "extends": [
+            "eslint:recommended",
+            "plugin:@typescript-eslint/eslint-recommended",
+            "plugin:@typescript-eslint/recommended",
+            "plugin:prettier/recommended"
+        ],
+        "parser": "@typescript-eslint/parser",
+        "parserOptions": {
+            "project": "tsconfig.json",
+            "sourceType": "module"
+        },
+        "plugins": [
+            "@typescript-eslint"
+        ],
+        "rules": {
+            "@typescript-eslint/naming-convention": [
+                "error",
+                {
+                    "custom": {
+                        "match": true,
+                        "regex": "^I[A-Z]"
+                    },
+                    "format": [
+                        "PascalCase"
+                    ],
+                    "selector": "interface"
+                }
+            ],
+            "@typescript-eslint/no-explicit-any": "off",
+            "@typescript-eslint/no-namespace": "off",
+            "@typescript-eslint/no-unused-vars": [
+                "warn",
+                {
+                    "args": "none"
+                }
+            ],
+            "@typescript-eslint/no-use-before-define": "off",
+            "@typescript-eslint/quotes": [
+                "error",
+                "single",
+                {
+                    "allowTemplateLiterals": false,
+                    "avoidEscape": true
+                }
+            ],
+            "curly": [
+                "error",
+                "all"
+            ],
+            "eqeqeq": "error",
+            "prefer-arrow-callback": "error"
+        }
     },
+    "eslintIgnore": [
+        "node_modules",
+        "dist",
+        "coverage",
+        "**/*.d.ts"
+    ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/zhangfeiran/jupyterlab_pausable_contextual_help",
-    "jupyter-releaser": {
-        "hooks": {
-            "before-build-npm": [
-                "python -m pip install jupyterlab~=3.1",
-                "jlpm"
-            ],
-            "before-build-python": [
-                "jlpm clean:all"
-            ]
-        }
-    },
     "jupyterlab": {
-        "disabledExtensions": [
-            "@jupyterlab/inspector-extension"
-        ],
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.f72bb70dee94e59ad703.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "jupyterlab_pausable_contextual_help/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "jupyterlab_pausable_contextual_help",
+    "prettier": {
+        "arrowParens": "avoid",
+        "endOfLine": "auto",
+        "overrides": [
+            {
+                "files": "package.json",
+                "options": {
+                    "tabWidth": 4
+                }
+            }
+        ],
+        "singleQuote": true,
+        "trailingComma": "none"
+    },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/zhangfeiran/jupyterlab_pausable_contextual_help.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
-        "clean:labextension": "rimraf jupyterlab_pausable_contextual_help/labextension",
+        "clean:labextension": "rimraf jupyterlab_pausable_contextual_help/labextension jupyterlab_pausable_contextual_help/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
+    "stylelint": {
+        "extends": [
+            "stylelint-config-recommended",
+            "stylelint-config-standard",
+            "stylelint-prettier/recommended"
+        ],
+        "plugins": [
+            "stylelint-csstree-validator"
+        ],
+        "rules": {
+            "csstree/validator": true,
+            "property-no-vendor-prefix": null,
+            "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
+            "selector-no-vendor-prefix": null,
+            "value-no-vendor-prefix": null
+        }
+    },
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.3"
 }
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/lib_index_js.3589c3b38b1e1b0c1f10.js` & `jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/lib_index_js.48d46625a03ec356bfc7.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
-                    "InspectionHandler": () => ( /* binding */ InspectionHandler)
+                    InspectionHandler: () => ( /* binding */ InspectionHandler)
                     /* harmony export */
                 });
                 /* harmony import */
                 var _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyterlab/coreutils */ "webpack/sharing/consume/default/@jupyterlab/coreutils");
                 /* harmony import */
                 var _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0__);
                 /* harmony import */
@@ -26,15 +26,17 @@
                 /* harmony import */
                 var _jupyterlab_rendermime__WEBPACK_IMPORTED_MODULE_1___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_rendermime__WEBPACK_IMPORTED_MODULE_1__);
                 /* harmony import */
                 var _lumino_coreutils__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__( /*! @lumino/coreutils */ "webpack/sharing/consume/default/@lumino/coreutils");
                 /* harmony import */
                 var _lumino_coreutils__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/ __webpack_require__.n(_lumino_coreutils__WEBPACK_IMPORTED_MODULE_2__);
                 /* harmony import */
-                var _lumino_polling__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__( /*! @lumino/polling */ "./node_modules/@lumino/polling/dist/index.es6.js");
+                var _lumino_polling__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__( /*! @lumino/polling */ "webpack/sharing/consume/default/@lumino/polling");
+                /* harmony import */
+                var _lumino_polling__WEBPACK_IMPORTED_MODULE_3___default = /*#__PURE__*/ __webpack_require__.n(_lumino_polling__WEBPACK_IMPORTED_MODULE_3__);
                 /* harmony import */
                 var _lumino_signaling__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__( /*! @lumino/signaling */ "webpack/sharing/consume/default/@lumino/signaling");
                 /* harmony import */
                 var _lumino_signaling__WEBPACK_IMPORTED_MODULE_4___default = /*#__PURE__*/ __webpack_require__.n(_lumino_signaling__WEBPACK_IMPORTED_MODULE_4__);
                 // Copyright (c) Jupyter Development Team.
                 // Distributed under the terms of the Modified BSD License.
 
@@ -59,27 +61,27 @@
                         this._standby = true;
                         this._lastInspectedReply = null;
                         this._connector = options.connector;
                         this._rendermime = options.rendermime;
                         this._debouncer = new _lumino_polling__WEBPACK_IMPORTED_MODULE_3__.Debouncer(this.onEditorChange.bind(this), 250);
                     }
                     /**
-                     * A signal emitted when the inspector should clear all items.
+                     * A signal emitted when the myinspector should clear all items.
                      */
                     get cleared() {
                         return this._cleared;
                     }
                     /**
                      * A signal emitted when the handler is disposed.
                      */
                     get disposed() {
                         return this._disposed;
                     }
                     /**
-                     * A signal emitted when an inspector value is generated.
+                     * A signal emitted when an myinspector value is generated.
                      */
                     get inspected() {
                         return this._inspected;
                     }
                     /**
                      * The editor widget used by the inspection handler.
                      */
@@ -90,29 +92,29 @@
                         if (newValue === this._editor) {
                             return;
                         }
                         // Remove all of our listeners.
                         _lumino_signaling__WEBPACK_IMPORTED_MODULE_4__.Signal.disconnectReceiver(this);
                         const editor = (this._editor = newValue);
                         if (editor) {
-                            // Clear the inspector in preparation for a new editor.
+                            // Clear the myinspector in preparation for a new editor.
                             this._cleared.emit(void 0);
                             // Call onEditorChange to cover the case where the user changes
                             // the active cell
                             this.onEditorChange();
                             editor.model.selections.changed.connect(this._onChange, this);
-                            editor.model.value.changed.connect(this._onChange, this);
+                            editor.model.sharedModel.changed.connect(this._onChange, this);
                         }
                     }
                     /**
                      * Indicates whether the handler makes API inspection requests or stands by.
                      *
                      * #### Notes
                      * The use case for this attribute is to limit the API traffic when no
-                     * inspector is visible.
+                     * myinspector is visible.
                      */
                     get standby() {
                         return this._standby;
                     }
                     set standby(value) {
                         this._standby = value;
                     }
@@ -129,33 +131,34 @@
                      * Dispose of the resources used by the handler.
                      */
                     dispose() {
                         if (this.isDisposed) {
                             return;
                         }
                         this._isDisposed = true;
+                        this._debouncer.dispose();
                         this._disposed.emit(void 0);
                         _lumino_signaling__WEBPACK_IMPORTED_MODULE_4__.Signal.clearData(this);
                     }
                     /**
                      * Handle a text changed signal from an editor.
                      *
                      * #### Notes
-                     * Update the hints inspector based on a text change.
+                     * Update the hints myinspector based on a text change.
                      */
                     onEditorChange(customText) {
                         // If the handler is in standby mode, bail.
                         if (this._standby) {
                             return;
                         }
                         const editor = this.editor;
                         if (!editor) {
                             return;
                         }
-                        const text = customText ? customText : editor.model.value.text;
+                        const text = customText ? customText : editor.model.sharedModel.getSource();
                         const position = editor.getCursorPosition();
                         const offset = _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0__.Text.jsIndexToCharIndex(editor.getOffsetAt(position), text);
                         const update = {
                             content: null
                         };
                         const pending = ++this._pending;
                         void this._connector
@@ -236,15 +239,15 @@
                 /* harmony import */
                 var _jupyterlab_console__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_console__WEBPACK_IMPORTED_MODULE_2__);
                 /* harmony import */
                 var _tokens__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__( /*! ./tokens */ "./lib/tokens.js");
                 /* harmony import */
                 var _handler__WEBPACK_IMPORTED_MODULE_10__ = __webpack_require__( /*! ./handler */ "./lib/handler.js");
                 /* harmony import */
-                var _inspector__WEBPACK_IMPORTED_MODULE_8__ = __webpack_require__( /*! ./inspector */ "./lib/inspector.js");
+                var _myinspector__WEBPACK_IMPORTED_MODULE_8__ = __webpack_require__( /*! ./myinspector */ "./lib/myinspector.js");
                 /* harmony import */
                 var _kernelconnector__WEBPACK_IMPORTED_MODULE_9__ = __webpack_require__( /*! ./kernelconnector */ "./lib/kernelconnector.js");
                 /* harmony import */
                 var _jupyterlab_launcher__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__( /*! @jupyterlab/launcher */ "webpack/sharing/consume/default/@jupyterlab/launcher");
                 /* harmony import */
                 var _jupyterlab_launcher__WEBPACK_IMPORTED_MODULE_3___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_launcher__WEBPACK_IMPORTED_MODULE_3__);
                 /* harmony import */
@@ -257,182 +260,191 @@
                 var _jupyterlab_translation__WEBPACK_IMPORTED_MODULE_5___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_translation__WEBPACK_IMPORTED_MODULE_5__);
                 /* harmony import */
                 var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__( /*! @jupyterlab/ui-components */ "webpack/sharing/consume/default/@jupyterlab/ui-components");
                 /* harmony import */
                 var _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_6___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_6__);
                 // Copyright (c) Jupyter Development Team.
                 // Distributed under the terms of the Modified BSD License.
+                // export * from './handler';
+                // export * from './myinspector';
+                // export * from './kernelconnector';
+                // export * from './tokens';
+                // Copyright (c) Jupyter Development Team.
+                // Distributed under the terms of the Modified BSD License.
 
+                // import { ISettingRegistry } from '@jupyterlab/settingregistry';
 
 
-                // import {
-                //   IInspector,
-                //   InspectionHandler,
-                //   InspectorPanel,
-                //   KernelConnector
-                // } from '@jupyterlab/inspector';
+                //   import {
+                //     IMyInspector,
+                //     InspectionHandler,
+                //     MyInspectorPanel,
+                //     KernelConnector
+                //   } from '@jupyterlab/inspector';
 
 
 
 
 
 
 
 
                 /**
-                 * The command IDs used by the inspector plugin.
+                 * The command IDs used by the myinspector plugin.
                  */
                 var CommandIDs;
                 (function(CommandIDs) {
                     CommandIDs.open = 'myinspector:open';
                     CommandIDs.close = 'myinspector:close';
                     CommandIDs.toggle = 'myinspector:toggle';
                     CommandIDs.trigger = 'myinspector:trigger';
                     CommandIDs.toggleStandby = 'myinspector:toggleStandby';
                 })(CommandIDs || (CommandIDs = {}));
                 /**
                  * A service providing code introspection.
                  */
-                const inspector = {
-                    id: 'jupyterlab_pausable_contextual_help:inspector',
+                const myinspector = {
+                    id: 'jupyterlab_pausable_contextual_help:myinspector',
+                    description: 'Provides the pausable code introspection widget.',
                     requires: [_jupyterlab_translation__WEBPACK_IMPORTED_MODULE_5__.ITranslator],
                     optional: [_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.ICommandPalette, _jupyterlab_launcher__WEBPACK_IMPORTED_MODULE_3__.ILauncher, _jupyterlab_application__WEBPACK_IMPORTED_MODULE_0__.ILayoutRestorer],
-                    provides: _tokens__WEBPACK_IMPORTED_MODULE_7__.IInspector,
+                    provides: _tokens__WEBPACK_IMPORTED_MODULE_7__.IMyInspector,
                     autoStart: true,
                     activate: (app, translator, palette, launcher, restorer) => {
                         const trans = translator.load('jupyterlab');
                         const {
                             commands,
                             shell
                         } = app;
                         const caption = trans.__('Manually updating code documentation from the active kernel');
                         const openedLabel = trans.__('My Contextual Help');
-                        const namespace = 'inspector';
-                        const datasetKey = 'jpInspector';
+                        const namespace = 'myinspector';
+                        const datasetKey = 'jpMyInspector';
                         const tracker = new _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.WidgetTracker({
                             namespace
                         });
 
-                        function isInspectorOpen() {
-                            return inspector && !inspector.isDisposed;
+                        function isMyInspectorOpen() {
+                            return myinspector && !myinspector.isDisposed;
                         }
 
                         function isStandby() {
-                            // return inspector && inspector.content && inspector.content.source && inspector.content.source.standby;
-                            if (inspector && inspector.content && inspector.content.source) {
-                                return inspector.content.source.standby;
+                            // return myinspector && myinspector.content && myinspector.content.source && myinspector.content.source.standby;
+                            if (myinspector && myinspector.content && myinspector.content.source) {
+                                return myinspector.content.source.standby;
                             }
                             return false;
                         }
                         let source = null;
-                        let inspector;
+                        let myinspector;
 
-                        function openInspector(args) {
+                        function openMyInspector(args) {
                             var _a;
-                            if (!isInspectorOpen()) {
-                                inspector = new _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.MainAreaWidget({
-                                    content: new _inspector__WEBPACK_IMPORTED_MODULE_8__.InspectorPanel({
+                            if (!isMyInspectorOpen()) {
+                                myinspector = new _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.MainAreaWidget({
+                                    content: new _myinspector__WEBPACK_IMPORTED_MODULE_8__.MyInspectorPanel({
                                         translator
                                     })
                                 });
-                                inspector.id = 'jp-inspector';
-                                inspector.title.label = openedLabel;
-                                inspector.title.icon = _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_6__.inspectorIcon;
-                                void tracker.add(inspector);
+                                myinspector.id = 'jp-myinspector';
+                                myinspector.title.label = openedLabel;
+                                myinspector.title.icon = _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_6__.inspectorIcon;
+                                void tracker.add(myinspector);
                                 source = source && !source.isDisposed ? source : null;
-                                inspector.content.source = source;
-                                (_a = inspector.content.source) === null || _a === void 0 ? void 0 : _a.onEditorChange(args);
+                                myinspector.content.source = source;
+                                (_a = myinspector.content.source) === null || _a === void 0 ? void 0 : _a.onEditorChange(args);
                             }
-                            if (!inspector.isAttached) {
-                                shell.add(inspector, 'main', {
+                            if (!myinspector.isAttached) {
+                                shell.add(myinspector, 'main', {
                                     activate: false,
-                                    mode: 'split-right'
+                                    mode: 'split-right',
+                                    type: 'MyInspector'
                                 });
                             }
-                            shell.activateById(inspector.id);
+                            shell.activateById(myinspector.id);
                             document.body.dataset[datasetKey] = 'open';
-                            return inspector;
+                            return myinspector;
                         }
 
-                        function closeInspector() {
-                            inspector.dispose();
+                        function closeMyInspector() {
+                            myinspector.dispose();
                             delete document.body.dataset[datasetKey];
                         }
-                        // Add inspector:open command to registry.
+                        // Add myinspector:open command to registry.
                         const showLabel = trans.__('Open My Contextual Help');
                         commands.addCommand(CommandIDs.open, {
                             caption,
-                            isEnabled: () => !inspector ||
-                                inspector.isDisposed ||
-                                !inspector.isAttached ||
-                                !inspector.isVisible,
+                            isEnabled: () => !myinspector ||
+                                myinspector.isDisposed ||
+                                !myinspector.isAttached ||
+                                !myinspector.isVisible,
                             label: showLabel,
                             icon: args => (args.isLauncher ? _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_6__.inspectorIcon : undefined),
                             execute: args => {
                                 var _a;
                                 const text = args && args.text;
                                 const refresh = args && args.refresh;
-                                // if inspector is open, see if we need a refresh
-                                if (isInspectorOpen() && refresh)
-                                    (_a = inspector.content.source) === null || _a === void 0 ? void 0 : _a.onEditorChange(text);
+                                // if myinspector is open, see if we need a refresh
+                                if (isMyInspectorOpen() && refresh)
+                                    (_a = myinspector.content.source) === null || _a === void 0 ? void 0 : _a.onEditorChange(text);
                                 else
-                                    openInspector(text);
+                                    openMyInspector(text);
                             }
                         });
-                        // Add inspector:close command to registry.
+                        // Add myinspector:close command to registry.
                         const closeLabel = trans.__('Hide My Contextual Help');
                         commands.addCommand(CommandIDs.close, {
                             caption,
-                            isEnabled: () => isInspectorOpen(),
+                            isEnabled: () => isMyInspectorOpen(),
                             label: closeLabel,
                             icon: args => (args.isLauncher ? _jupyterlab_ui_components__WEBPACK_IMPORTED_MODULE_6__.inspectorIcon : undefined),
-                            execute: () => closeInspector()
+                            execute: () => closeMyInspector()
                         });
-                        // Add inspector:toggle command to registry.
+                        // Add myinspector:toggle command to registry.
                         const toggleLabel = trans.__('Show My Contextual Help');
                         commands.addCommand(CommandIDs.toggle, {
                             caption,
                             label: toggleLabel,
-                            isToggled: () => isInspectorOpen(),
+                            isToggled: () => isMyInspectorOpen(),
                             execute: args => {
-                                if (isInspectorOpen()) {
-                                    closeInspector();
+                                if (isMyInspectorOpen()) {
+                                    closeMyInspector();
                                 } else {
                                     const text = args && args.text;
-                                    openInspector(text);
+                                    openMyInspector(text);
                                 }
                             }
                         });
-                        // Add inspector:trigger command to registry.
+                        // Add myinspector:trigger command to registry.
                         const triggerLabel = trans.__('Trigger My Contextual Help');
                         commands.addCommand(CommandIDs.trigger, {
                             caption,
                             isEnabled: () => isStandby(),
                             label: triggerLabel,
                             execute: () => {
                                 var _a;
-                                if (inspector && inspector.content && inspector.content.source && isStandby()) {
-                                    inspector.content.source.standby = false;
-                                    (_a = inspector.content.source) === null || _a === void 0 ? void 0 : _a.onEditorChange();
-                                    inspector.content.source.standby = true;
+                                if (myinspector && myinspector.content && myinspector.content.source && isStandby()) {
+                                    myinspector.content.source.standby = false;
+                                    (_a = myinspector.content.source) === null || _a === void 0 ? void 0 : _a.onEditorChange();
+                                    myinspector.content.source.standby = true;
                                 }
                             }
                         });
-                        // Add inspector:toggleStandby command to registry.
+                        // Add myinspector:toggleStandby command to registry.
                         const toggleStandbyLabel = trans.__('Auto Update My Contextual Help');
                         commands.addCommand(CommandIDs.toggleStandby, {
                             caption,
                             isToggled: () => !isStandby(),
                             label: toggleStandbyLabel,
                             execute: () => {
-                                if (inspector && inspector.content && inspector.content.source) {
+                                if (myinspector && myinspector.content && myinspector.content.source) {
                                     if (isStandby()) {
-                                        inspector.content.source.standby = false;
+                                        myinspector.content.source.standby = false;
                                     } else {
-                                        inspector.content.source.standby = true;
+                                        myinspector.content.source.standby = true;
                                     }
                                 }
                             }
                         });
                         // Add open command to launcher if possible.
                         if (launcher) {
                             launcher.add({
@@ -449,36 +461,38 @@
                                 category: toggleLabel
                             });
                         }
                         // Handle state restoration.
                         if (restorer) {
                             void restorer.restore(tracker, {
                                 command: CommandIDs.toggle,
-                                name: () => 'inspector'
+                                name: () => 'myinspector'
                             });
                         }
-                        // Create a proxy to pass the `source` to the current inspector.
+                        // Create a proxy to pass the `source` to the current myinspector.
                         const proxy = Object.defineProperty({}, 'source', {
-                            get: () => !inspector || inspector.isDisposed ? null : inspector.content.source,
+                            get: () => !myinspector || myinspector.isDisposed ? null : myinspector.content.source,
                             set: (src) => {
                                 source = src && !src.isDisposed ? src : null;
-                                if (inspector && !inspector.isDisposed) {
-                                    inspector.content.source = source;
+                                if (myinspector && !myinspector.isDisposed) {
+                                    myinspector.content.source = source;
                                 }
                             }
                         });
                         return proxy;
                     }
                 };
                 /**
                  * An extension that registers consoles for inspection.
                  */
                 const consoles = {
+                    // FIXME This should be in @jupyterlab/console-extension
                     id: 'jupyterlab_pausable_contextual_help:consoles',
-                    requires: [_tokens__WEBPACK_IMPORTED_MODULE_7__.IInspector, _jupyterlab_console__WEBPACK_IMPORTED_MODULE_2__.IConsoleTracker, _jupyterlab_application__WEBPACK_IMPORTED_MODULE_0__.ILabShell],
+                    description: 'Adds my code introspection support to consoles.',
+                    requires: [_tokens__WEBPACK_IMPORTED_MODULE_7__.IMyInspector, _jupyterlab_console__WEBPACK_IMPORTED_MODULE_2__.IConsoleTracker, _jupyterlab_application__WEBPACK_IMPORTED_MODULE_0__.ILabShell],
                     autoStart: true,
                     activate: (app, manager, consoles, labShell, translator) => {
                         // Maintain association of new consoles with their respective handlers.
                         const handlers = {};
                         // Create a handler for each console that is created.
                         consoles.widgetAdded.connect((sender, parent) => {
                             const sessionContext = parent.console.sessionContext;
@@ -501,41 +515,40 @@
                             });
                             // Listen for parent disposal.
                             parent.disposed.connect(() => {
                                 delete handlers[parent.id];
                                 handler.dispose();
                             });
                         });
-                        // Keep track of console instances and set inspector source.
-                        labShell.currentChanged.connect((_, args) => {
-                            const widget = args.newValue;
-                            if (!widget || !consoles.has(widget)) {
-                                return;
-                            }
-                            const source = handlers[widget.id];
-                            if (source) {
-                                manager.source = source;
+                        // Keep track of console instances and set myinspector source.
+                        const setSource = (widget) => {
+                            if (widget && consoles.has(widget) && handlers[widget.id]) {
+                                manager.source = handlers[widget.id];
                             }
-                        });
+                        };
+                        labShell.currentChanged.connect((_, args) => setSource(args.newValue));
+                        void app.restored.then(() => setSource(labShell.currentWidget));
                         app.contextMenu.addItem({
                             command: CommandIDs.toggle,
                             selector: '.jp-CodeConsole-promptCell'
                         });
                         app.contextMenu.addItem({
                             command: CommandIDs.toggleStandby,
                             selector: '.jp-CodeConsole-promptCell'
                         });
                     }
                 };
                 /**
                  * An extension that registers notebooks for inspection.
                  */
                 const notebooks = {
+                    // FIXME This should be in @jupyterlab/notebook-extension
                     id: 'jupyterlab_pausable_contextual_help:notebooks',
-                    requires: [_tokens__WEBPACK_IMPORTED_MODULE_7__.IInspector, _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_4__.INotebookTracker, _jupyterlab_application__WEBPACK_IMPORTED_MODULE_0__.ILabShell],
+                    description: 'Adds code introspection to notebooks.',
+                    requires: [_tokens__WEBPACK_IMPORTED_MODULE_7__.IMyInspector, _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_4__.INotebookTracker, _jupyterlab_application__WEBPACK_IMPORTED_MODULE_0__.ILabShell],
                     autoStart: true,
                     activate: (app, manager, notebooks, labShell) => {
                         // Maintain association of new notebooks with their respective handlers.
                         const handlers = {};
                         // Create a handler for each notebook that is created.
                         notebooks.widgetAdded.connect((sender, parent) => {
                             const sessionContext = parent.sessionContext;
@@ -550,67 +563,136 @@
                             // Associate the handler to the widget.
                             handlers[parent.id] = handler;
                             // Set the initial editor.
                             const cell = parent.content.activeCell;
                             handler.editor = cell && cell.editor;
                             // Listen for active cell changes.
                             parent.content.activeCellChanged.connect((sender, cell) => {
-                                handler.editor = cell && cell.editor;
+                                void(cell === null || cell === void 0 ? void 0 : cell.ready.then(() => {
+                                    if (cell === parent.content.activeCell) {
+                                        handler.editor = cell.editor;
+                                    }
+                                }));
                             });
                             // Listen for parent disposal.
                             parent.disposed.connect(() => {
                                 delete handlers[parent.id];
                                 handler.dispose();
                             });
                         });
-                        // Keep track of notebook instances and set inspector source.
-                        labShell.currentChanged.connect((sender, args) => {
-                            const widget = args.newValue;
-                            if (!widget || !notebooks.has(widget)) {
-                                return;
-                            }
-                            const source = handlers[widget.id];
-                            if (source) {
-                                manager.source = source;
+                        // Keep track of notebook instances and set myinspector source.
+                        const setSource = (widget) => {
+                            if (widget && notebooks.has(widget) && handlers[widget.id]) {
+                                manager.source = handlers[widget.id];
                             }
-                        });
+                        };
+                        labShell.currentChanged.connect((_, args) => setSource(args.newValue));
+                        void app.restored.then(() => setSource(labShell.currentWidget));
                         app.contextMenu.addItem({
                             command: CommandIDs.toggle,
                             selector: '.jp-Notebook'
                         });
                         app.contextMenu.addItem({
                             command: CommandIDs.toggleStandby,
                             selector: '.jp-Notebook'
                         });
                     }
                 };
                 /**
                  * Export the plugins as default.
                  */
-                const plugins = [inspector, consoles, notebooks];
+                const plugins = [myinspector, consoles, notebooks];
                 /* harmony default export */
                 const __WEBPACK_DEFAULT_EXPORT__ = (plugins);
 
 
                 /***/
             }),
 
         /***/
-        "./lib/inspector.js":
-            /*!**************************!*\
-              !*** ./lib/inspector.js ***!
-              \**************************/
+        "./lib/kernelconnector.js":
+            /*!********************************!*\
+              !*** ./lib/kernelconnector.js ***!
+              \********************************/
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
-                    "InspectorPanel": () => ( /* binding */ InspectorPanel)
+                    KernelConnector: () => ( /* binding */ KernelConnector)
+                    /* harmony export */
+                });
+                /* harmony import */
+                var _jupyterlab_statedb__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyterlab/statedb */ "webpack/sharing/consume/default/@jupyterlab/statedb");
+                /* harmony import */
+                var _jupyterlab_statedb__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_statedb__WEBPACK_IMPORTED_MODULE_0__);
+                // Copyright (c) Jupyter Development Team.
+                // Distributed under the terms of the Modified BSD License.
+
+                /**
+                 * The default connector for making inspection requests from the Jupyter API.
+                 */
+                class KernelConnector extends _jupyterlab_statedb__WEBPACK_IMPORTED_MODULE_0__.DataConnector {
+                    /**
+                     * Create a new kernel connector for inspection requests.
+                     *
+                     * @param options - The instantiation options for the kernel connector.
+                     */
+                    constructor(options) {
+                        super();
+                        this._sessionContext = options.sessionContext;
+                    }
+                    /**
+                     * Fetch inspection requests.
+                     *
+                     * @param request - The inspection request text and details.
+                     */
+                    fetch(request) {
+                        var _a;
+                        const kernel = (_a = this._sessionContext.session) === null || _a === void 0 ? void 0 : _a.kernel;
+                        if (!kernel) {
+                            return Promise.reject(new Error('Inspection fetch requires a kernel.'));
+                        }
+                        const contents = {
+                            code: request.text,
+                            cursor_pos: request.offset,
+                            detail_level: 1
+                        };
+                        return kernel.requestInspect(contents).then(msg => {
+                            const response = msg.content;
+                            if (response.status !== 'ok' || !response.found) {
+                                throw new Error('Inspection fetch failed to return successfully.');
+                            }
+                            return {
+                                data: response.data,
+                                metadata: response.metadata
+                            };
+                        });
+                    }
+                }
+
+
+                /***/
+            }),
+
+        /***/
+        "./lib/myinspector.js":
+            /*!****************************!*\
+              !*** ./lib/myinspector.js ***!
+              \****************************/
+            /***/
+            ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
+
+                __webpack_require__.r(__webpack_exports__);
+                /* harmony export */
+                __webpack_require__.d(__webpack_exports__, {
+                    /* harmony export */
+                    MyInspectorPanel: () => ( /* binding */ MyInspectorPanel)
                     /* harmony export */
                 });
                 /* harmony import */
                 var _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyterlab/apputils */ "webpack/sharing/consume/default/@jupyterlab/apputils");
                 /* harmony import */
                 var _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__);
                 /* harmony import */
@@ -623,102 +705,102 @@
                 var _lumino_widgets__WEBPACK_IMPORTED_MODULE_2___default = /*#__PURE__*/ __webpack_require__.n(_lumino_widgets__WEBPACK_IMPORTED_MODULE_2__);
                 // Copyright (c) Jupyter Development Team.
                 // Distributed under the terms of the Modified BSD License.
 
 
 
                 /**
-                 * The class name added to inspector panels.
+                 * The class name added to myinspector panels.
                  */
-                const PANEL_CLASS = 'jp-Inspector';
+                const PANEL_CLASS = 'jp-MyInspector';
                 /**
-                 * The class name added to inspector content.
+                 * The class name added to myinspector content.
                  */
-                const CONTENT_CLASS = 'jp-Inspector-content';
+                const CONTENT_CLASS = 'jp-MyInspector-content';
                 /**
-                 * The class name added to default inspector content.
+                 * The class name added to default myinspector content.
                  */
-                const DEFAULT_CONTENT_CLASS = 'jp-Inspector-default-content';
+                const DEFAULT_CONTENT_CLASS = 'jp-MyInspector-default-content';
                 /**
-                 * A panel which contains a set of inspectors.
+                 * A panel which contains a set of myinspectors.
                  */
-                class InspectorPanel extends _lumino_widgets__WEBPACK_IMPORTED_MODULE_2__.Panel {
+                class MyInspectorPanel extends _lumino_widgets__WEBPACK_IMPORTED_MODULE_2__.Panel {
                     /**
-                     * Construct an inspector.
+                     * Construct an myinspector.
                      */
                     constructor(options = {}) {
                         super();
                         this._source = null;
                         this.translator = options.translator || _jupyterlab_translation__WEBPACK_IMPORTED_MODULE_1__.nullTranslator;
                         this._trans = this.translator.load('jupyterlab');
                         if (options.initialContent instanceof _lumino_widgets__WEBPACK_IMPORTED_MODULE_2__.Widget) {
                             this._content = options.initialContent;
                         } else if (typeof options.initialContent === 'string') {
-                            this._content = InspectorPanel._generateContentWidget(`<p>${options.initialContent}</p>`);
+                            this._content = MyInspectorPanel._generateContentWidget(`<p>${options.initialContent}</p>`);
                         } else {
-                            this._content = InspectorPanel._generateContentWidget('<p>' +
+                            this._content = MyInspectorPanel._generateContentWidget('<p>' +
                                 this._trans.__('Press F1 on a function to see documentation.') +
                                 '</p>');
                         }
                         this.addClass(PANEL_CLASS);
                         this.layout.addWidget(this._content);
                     }
                     /**
                      * Print in iframe
                      */
                     [_jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.Printing.symbol]() {
                         return () => _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_0__.Printing.printWidget(this);
                     }
                     /**
-                     * The source of events the inspector panel listens for.
+                     * The source of events the myinspector panel listens for.
                      */
                     get source() {
                         return this._source;
                     }
                     set source(source) {
                         if (this._source === source) {
                             return;
                         }
                         // Disconnect old signal handler.
                         if (this._source) {
                             this._source.standby = true;
-                            this._source.inspected.disconnect(this.onInspectorUpdate, this);
+                            this._source.inspected.disconnect(this.onMyInspectorUpdate, this);
                             this._source.disposed.disconnect(this.onSourceDisposed, this);
                         }
                         // Reject a source that is already disposed.
                         if (source && source.isDisposed) {
                             source = null;
                         }
                         // Update source.
                         this._source = source;
                         // Connect new signal handler.
                         if (this._source) {
                             //   this._source.standby = false;
-                            this._source.inspected.connect(this.onInspectorUpdate, this);
+                            this._source.inspected.connect(this.onMyInspectorUpdate, this);
                             this._source.disposed.connect(this.onSourceDisposed, this);
                         }
                     }
                     /**
                      * Dispose of the resources held by the widget.
                      */
                     dispose() {
                         if (this.isDisposed) {
                             return;
                         }
                         this.source = null;
                         super.dispose();
                     }
                     /**
-                     * Handle inspector update signals.
+                     * Handle myinspector update signals.
                      */
-                    onInspectorUpdate(sender, args) {
+                    onMyInspectorUpdate(sender, args) {
                         const {
                             content
                         } = args;
-                        // Update the content of the inspector widget.
+                        // Update the content of the myinspector widget.
                         if (!content || content === this._content) {
                             return;
                         }
                         this._content.dispose();
                         this._content = content;
                         content.addClass(CONTENT_CLASS);
                         this.layout.addWidget(content);
@@ -742,108 +824,41 @@
                 }
 
 
                 /***/
             }),
 
         /***/
-        "./lib/kernelconnector.js":
-            /*!********************************!*\
-              !*** ./lib/kernelconnector.js ***!
-              \********************************/
-            /***/
-            ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
-
-                __webpack_require__.r(__webpack_exports__);
-                /* harmony export */
-                __webpack_require__.d(__webpack_exports__, {
-                    /* harmony export */
-                    "KernelConnector": () => ( /* binding */ KernelConnector)
-                    /* harmony export */
-                });
-                /* harmony import */
-                var _jupyterlab_statedb__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyterlab/statedb */ "webpack/sharing/consume/default/@jupyterlab/statedb");
-                /* harmony import */
-                var _jupyterlab_statedb__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_statedb__WEBPACK_IMPORTED_MODULE_0__);
-                // Copyright (c) Jupyter Development Team.
-                // Distributed under the terms of the Modified BSD License.
-
-                /**
-                 * The default connector for making inspection requests from the Jupyter API.
-                 */
-                class KernelConnector extends _jupyterlab_statedb__WEBPACK_IMPORTED_MODULE_0__.DataConnector {
-                    /**
-                     * Create a new kernel connector for inspection requests.
-                     *
-                     * @param options - The instantiation options for the kernel connector.
-                     */
-                    constructor(options) {
-                        super();
-                        this._sessionContext = options.sessionContext;
-                    }
-                    /**
-                     * Fetch inspection requests.
-                     *
-                     * @param request - The inspection request text and details.
-                     */
-                    fetch(request) {
-                        var _a;
-                        const kernel = (_a = this._sessionContext.session) === null || _a === void 0 ? void 0 : _a.kernel;
-                        if (!kernel) {
-                            return Promise.reject(new Error('Inspection fetch requires a kernel.'));
-                        }
-                        const contents = {
-                            code: request.text,
-                            cursor_pos: request.offset,
-                            detail_level: 1
-                        };
-                        return kernel.requestInspect(contents).then(msg => {
-                            const response = msg.content;
-                            if (response.status !== 'ok' || !response.found) {
-                                throw new Error('Inspection fetch failed to return successfully.');
-                            }
-                            return {
-                                data: response.data,
-                                metadata: response.metadata
-                            };
-                        });
-                    }
-                }
-
-
-                /***/
-            }),
-
-        /***/
         "./lib/tokens.js":
             /*!***********************!*\
               !*** ./lib/tokens.js ***!
               \***********************/
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
-                    "IInspector": () => ( /* binding */ IInspector)
+                    IMyInspector: () => ( /* binding */ IMyInspector)
                     /* harmony export */
                 });
                 /* harmony import */
                 var _lumino_coreutils__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @lumino/coreutils */ "webpack/sharing/consume/default/@lumino/coreutils");
                 /* harmony import */
                 var _lumino_coreutils__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_lumino_coreutils__WEBPACK_IMPORTED_MODULE_0__);
                 // Copyright (c) Jupyter Development Team.
                 // Distributed under the terms of the Modified BSD License.
 
                 /**
-                 * The inspector panel token.
+                 * The myinspector panel token.
                  */
-                const IInspector = new _lumino_coreutils__WEBPACK_IMPORTED_MODULE_0__.Token('@jupyterlab/inspector:IInspector');
+                const IMyInspector = new _lumino_coreutils__WEBPACK_IMPORTED_MODULE_0__.Token('@jupyterlab/inspector:IMyInspector', `A service for adding contextual help to widgets (visible using "Show Contextual Help" from the Help menu).
+  Use this to hook into the contextual help system in your extension.`);
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.3589c3b38b1e1b0c1f10.js.map
+//# sourceMappingURL=lib_index_js.48d46625a03ec356bfc7.js.map
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/remoteEntry.bba643b4b9733f60248c.js` & `jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/remoteEntry.f72bb70dee94e59ad703.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -12,21 +12,21 @@
               !*** container entry ***!
               \***********************/
             /***/
             ((__unused_webpack_module, exports, __webpack_require__) => {
 
                 var moduleMap = {
                     "./index": () => {
-                        return Promise.all([__webpack_require__.e("vendors-node_modules_lumino_polling_dist_index_es6_js"), __webpack_require__.e("lib_index_js")]).then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
+                        return __webpack_require__.e("lib_index_js").then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
                     },
                     "./extension": () => {
-                        return Promise.all([__webpack_require__.e("vendors-node_modules_lumino_polling_dist_index_es6_js"), __webpack_require__.e("lib_index_js")]).then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
+                        return __webpack_require__.e("lib_index_js").then(() => (() => ((__webpack_require__( /*! ./lib/index.js */ "./lib/index.js")))));
                     },
                     "./style": () => {
-                        return Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("style_index_js")]).then(() => (() => ((__webpack_require__( /*! ./style/index.js */ "./style/index.js")))));
+                        return Promise.all([__webpack_require__.e("vendors-node_modules_jupyterlab_application_style_index_js-node_modules_jupyterlab_console_st-8dc7b3"), __webpack_require__.e("style_index_js-data_image_png_base64_iVBORw0KGgoAAAANSUhEUgAAAAgAAAAFCAYAAAB4ka1VAAAAsElEQVQI-adaf50")]).then(() => (() => ((__webpack_require__( /*! ./style/index.js */ "./style/index.js")))));
                     }
                 };
                 var get = (module, getScope) => {
                     __webpack_require__.R = getScope;
                     getScope = (
                         __webpack_require__.o(moduleMap, module) ?
                         moduleMap[module]() :
@@ -182,18 +182,17 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "vendors-node_modules_lumino_polling_dist_index_es6_js": "35868735457bf9c961c0",
-                "lib_index_js": "3589c3b38b1e1b0c1f10",
-                "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "547b99950c80d08ebd47",
-                "style_index_js": "1eebcf1c283efc5e22d0"
+                "lib_index_js": "48d46625a03ec356bfc7",
+                "vendors-node_modules_jupyterlab_application_style_index_js-node_modules_jupyterlab_console_st-8dc7b3": "f3e7c133ec1940ded4f9",
+                "style_index_js-data_image_png_base64_iVBORw0KGgoAAAANSUhEUgAAAAgAAAAFCAYAAAB4ka1VAAAAsElEQVQI-adaf50": "2b034a8fa2de53285adf"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
     /******/
@@ -279,14 +278,15 @@
                     /******/
                     script.setAttribute("nonce", __webpack_require__.nc);
                     /******/
                 }
                 /******/
                 script.setAttribute("data-webpack", dataWebpackPrefix + key);
                 /******/
+                /******/
                 script.src = url;
                 /******/
             }
             /******/
             inProgress[url] = [done];
             /******/
             var onScriptComplete = (prev, event) => {
@@ -302,15 +302,15 @@
                 /******/
                 script.parentNode && script.parentNode.removeChild(script);
                 /******/
                 doneFns && doneFns.forEach((fn) => (fn(event)));
                 /******/
                 if (prev) return prev(event);
                 /******/
-            };
+            }
             /******/
             var timeout = setTimeout(onScriptComplete.bind(null, undefined, {
                 type: 'timeout',
                 target: script
             }), 120000);
             /******/
             script.onerror = onScriptComplete.bind(null, script.onerror);
@@ -376,15 +376,19 @@
             /******/ // creates a new share scope if needed
             /******/
             if (!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};
             /******/ // runs all init snippets from all modules reachable
             /******/
             var scope = __webpack_require__.S[name];
             /******/
-            var warn = (msg) => (typeof console !== "undefined" && console.warn && console.warn(msg));
+            var warn = (msg) => {
+                /******/
+                if (typeof console !== "undefined" && console.warn) console.warn(msg);
+                /******/
+            };
             /******/
             var uniqueName = "jupyterlab_pausable_contextual_help";
             /******/
             var register = (name, version, factory, eager) => {
                 /******/
                 var versions = scope[name] = scope[name] || {};
                 /******/
@@ -424,15 +428,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab_pausable_contextual_help", "0.1.1", () => (Promise.all([__webpack_require__.e("vendors-node_modules_lumino_polling_dist_index_es6_js"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab_pausable_contextual_help", "0.1.3", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -455,21 +459,27 @@
         /******/
         var document = __webpack_require__.g.document;
         /******/
         if (!scriptUrl && document) {
             /******/
             if (document.currentScript)
                 /******/
-                scriptUrl = document.currentScript.src
+                scriptUrl = document.currentScript.src;
             /******/
             if (!scriptUrl) {
                 /******/
                 var scripts = document.getElementsByTagName("script");
                 /******/
-                if (scripts.length) scriptUrl = scripts[scripts.length - 1].src
+                if (scripts.length) {
+                    /******/
+                    var i = scripts.length - 1;
+                    /******/
+                    while (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;
+                    /******/
+                }
                 /******/
             }
             /******/
         }
         /******/ // When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration
         /******/ // or pass an empty string ("") and set the __webpack_public_path__ variable from your code to use your own logic.
         /******/
@@ -634,15 +644,15 @@
             /******/
         };
         /******/
         var getSingletonVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
             var version = findSingletonVersionKey(scope, key);
             /******/
-            if (!satisfy(requiredVersion, version)) typeof console !== "undefined" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));
+            if (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));
             /******/
             return get(scope[key][version]);
             /******/
         };
         /******/
         var getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
@@ -690,17 +700,23 @@
             /******/
             if (entry) return get(entry);
             /******/
             throw new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));
             /******/
         };
         /******/
+        var warn = (msg) => {
+            /******/
+            if (typeof console !== "undefined" && console.warn) console.warn(msg);
+            /******/
+        };
+        /******/
         var warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
-            typeof console !== "undefined" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));
+            warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));
             /******/
         };
         /******/
         var get = (entry) => {
             /******/
             entry.loaded = 1;
             /******/
@@ -813,140 +829,153 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 3, 0, 13])),
+            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 4, 2, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 0, 10])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 3, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/console": () => (loadSingletonVersionCheck("default", "@jupyterlab/console", [1, 3, 0, 12])),
+            "webpack/sharing/consume/default/@jupyterlab/console": () => (loadSingletonVersionCheck("default", "@jupyterlab/console", [1, 4, 2, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/launcher": () => (loadSingletonVersionCheck("default", "@jupyterlab/launcher", [1, 3, 0, 10])),
+            "webpack/sharing/consume/default/@lumino/coreutils": () => (loadSingletonVersionCheck("default", "@lumino/coreutils", [1, 2, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 3, 0, 13])),
+            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 6, 2, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/translation": () => (loadSingletonVersionCheck("default", "@jupyterlab/translation", [1, 3, 0, 10])),
+            "webpack/sharing/consume/default/@jupyterlab/rendermime": () => (loadSingletonVersionCheck("default", "@jupyterlab/rendermime", [1, 4, 2, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 3, 0, 8])),
+            "webpack/sharing/consume/default/@lumino/polling": () => (loadSingletonVersionCheck("default", "@lumino/polling", [1, 2, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@lumino/coreutils": () => (loadSingletonVersionCheck("default", "@lumino/coreutils", [1, 1, 5, 3])),
+            "webpack/sharing/consume/default/@lumino/signaling": () => (loadSingletonVersionCheck("default", "@lumino/signaling", [1, 2, 0, 0])),
             /******/
-            "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 1, 16, 1])),
+            "webpack/sharing/consume/default/@jupyterlab/translation": () => (loadSingletonVersionCheck("default", "@jupyterlab/translation", [1, 4, 2, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/statedb": () => (loadSingletonVersionCheck("default", "@jupyterlab/statedb", [1, 3, 0, 7])),
+            "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 5, 0, 7])),
+            "webpack/sharing/consume/default/@jupyterlab/statedb": () => (loadSingletonVersionCheck("default", "@jupyterlab/statedb", [1, 4, 2, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/rendermime": () => (loadSingletonVersionCheck("default", "@jupyterlab/rendermime", [1, 3, 0, 12])),
+            "webpack/sharing/consume/default/@jupyterlab/launcher": () => (loadSingletonVersionCheck("default", "@jupyterlab/launcher", [1, 4, 2, 0])),
             /******/
-            "webpack/sharing/consume/default/@lumino/signaling": () => (loadSingletonVersionCheck("default", "@lumino/signaling", [1, 1, 4, 3]))
+            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 4, 2, 0])),
+            /******/
+            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 4, 2, 0]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/application",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/apputils",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/console",
                 /******/
-                "webpack/sharing/consume/default/@jupyterlab/launcher",
+                "webpack/sharing/consume/default/@lumino/coreutils",
                 /******/
-                "webpack/sharing/consume/default/@jupyterlab/notebook",
+                "webpack/sharing/consume/default/@jupyterlab/coreutils",
                 /******/
-                "webpack/sharing/consume/default/@jupyterlab/translation",
+                "webpack/sharing/consume/default/@jupyterlab/rendermime",
                 /******/
-                "webpack/sharing/consume/default/@jupyterlab/ui-components",
+                "webpack/sharing/consume/default/@lumino/polling",
                 /******/
-                "webpack/sharing/consume/default/@lumino/coreutils",
+                "webpack/sharing/consume/default/@lumino/signaling",
+                /******/
+                "webpack/sharing/consume/default/@jupyterlab/translation",
                 /******/
                 "webpack/sharing/consume/default/@lumino/widgets",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/statedb",
                 /******/
-                "webpack/sharing/consume/default/@jupyterlab/coreutils",
+                "webpack/sharing/consume/default/@jupyterlab/launcher",
                 /******/
-                "webpack/sharing/consume/default/@jupyterlab/rendermime",
+                "webpack/sharing/consume/default/@jupyterlab/notebook",
                 /******/
-                "webpack/sharing/consume/default/@lumino/signaling"
+                "webpack/sharing/consume/default/@jupyterlab/ui-components"
                 /******/
             ]
             /******/
         };
         /******/
+        var startedInstallModules = {};
+        /******/
         __webpack_require__.f.consumes = (chunkId, promises) => {
             /******/
             if (__webpack_require__.o(chunkMapping, chunkId)) {
                 /******/
                 chunkMapping[chunkId].forEach((id) => {
                     /******/
                     if (__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);
                     /******/
-                    var onFactory = (factory) => {
+                    if (!startedInstallModules[id]) {
                         /******/
-                        installedModules[id] = 0;
-                        /******/
-                        __webpack_require__.m[id] = (module) => {
+                        var onFactory = (factory) => {
                             /******/
-                            delete __webpack_require__.c[id];
+                            installedModules[id] = 0;
                             /******/
-                            module.exports = factory();
+                            __webpack_require__.m[id] = (module) => {
+                                /******/
+                                delete __webpack_require__.c[id];
+                                /******/
+                                module.exports = factory();
+                                /******/
+                            }
                             /******/
-                        }
-                        /******/
-                    };
-                    /******/
-                    var onError = (error) => {
+                        };
                         /******/
-                        delete installedModules[id];
+                        startedInstallModules[id] = true;
                         /******/
-                        __webpack_require__.m[id] = (module) => {
+                        var onError = (error) => {
                             /******/
-                            delete __webpack_require__.c[id];
+                            delete installedModules[id];
                             /******/
-                            throw error;
+                            __webpack_require__.m[id] = (module) => {
+                                /******/
+                                delete __webpack_require__.c[id];
+                                /******/
+                                throw error;
+                                /******/
+                            }
                             /******/
-                        }
-                        /******/
-                    };
-                    /******/
-                    try {
-                        /******/
-                        var promise = moduleToHandlerMapping[id]();
+                        };
                         /******/
-                        if (promise.then) {
+                        try {
                             /******/
-                            promises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));
+                            var promise = moduleToHandlerMapping[id]();
                             /******/
-                        } else onFactory(promise);
+                            if (promise.then) {
+                                /******/
+                                promises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));
+                                /******/
+                            } else onFactory(promise);
+                            /******/
+                        } catch (e) {
+                            onError(e);
+                        }
                         /******/
-                    } catch (e) {
-                        onError(e);
                     }
                     /******/
                 });
                 /******/
             }
             /******/
         }
         /******/
     })();
     /******/
     /******/
     /* webpack/runtime/jsonp chunk loading */
     /******/
     (() => {
-        /******/ // no baseURI
+        /******/
+        __webpack_require__.b = document.baseURI || self.location.href;
         /******/
         /******/ // object to store loaded and loading chunks
         /******/ // undefined = chunk not loaded, null = chunk preloaded/prefetched
         /******/ // [resolve, reject, Promise] = chunk loading, 0 = chunk loaded
         /******/
         var installedChunks = {
             /******/
@@ -1012,15 +1041,15 @@
                                 /******/
                             }
                             /******/
                         };
                         /******/
                         __webpack_require__.l(url, loadingEnded, "chunk-" + chunkId, chunkId);
                         /******/
-                    } else installedChunks[chunkId] = 0;
+                    }
                     /******/
                 }
                 /******/
             }
             /******/
         };
         /******/
@@ -1105,8 +1134,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab_pausable_contextual_help");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).jupyterlab_pausable_contextual_help = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.bba643b4b9733f60248c.js.map
+//# sourceMappingURL=remoteEntry.f72bb70dee94e59ad703.js.map
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/remoteEntry.bba643b4b9733f60248c.js.map` & `jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/remoteEntry.f72bb70dee94e59ad703.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8171428571428571%*

 * *Differences: {"'file'": "'remoteEntry.f72bb70dee94e59ad703.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.bba643b4b9733f60248c.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,2RAA2R;WACzT;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC/LA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
+    "file": "remoteEntry.f72bb70dee94e59ad703.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,kSAAkS;WAChU;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB;WACA,GAAG;WACH;WACA;;;;;WCxMA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab_pausable_contextual_help/webpack/container-entry",
         "webpack://jupyterlab_pausable_contextual_help/webpack/bootstrap",
         "webpack://jupyterlab_pausable_contextual_help/webpack/runtime/compat get default export",
         "webpack://jupyterlab_pausable_contextual_help/webpack/runtime/define property getters",
@@ -20,28 +20,28 @@
         "webpack://jupyterlab_pausable_contextual_help/webpack/runtime/jsonp chunk loading",
         "webpack://jupyterlab_pausable_contextual_help/webpack/runtime/nonce",
         "webpack://jupyterlab_pausable_contextual_help/webpack/before-startup",
         "webpack://jupyterlab_pausable_contextual_help/webpack/startup",
         "webpack://jupyterlab_pausable_contextual_help/webpack/after-startup"
     ],
     "sourcesContent": [
-        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_lumino_polling_dist_index_es6_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_lumino_polling_dist_index_es6_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
+        "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_jupyterlab_application_style_index_js-node_modules_jupyterlab_console_st-8dc7b3\"), __webpack_require__.e(\"style_index_js-data_image_png_base64_iVBORw0KGgoAAAANSUhEUgAAAAgAAAAFCAYAAAB4ka1VAAAAsElEQVQI-adaf50\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_lumino_polling_dist_index_es6_js\":\"35868735457bf9c961c0\",\"lib_index_js\":\"3589c3b38b1e1b0c1f10\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"547b99950c80d08ebd47\",\"style_index_js\":\"1eebcf1c283efc5e22d0\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"48d46625a03ec356bfc7\",\"vendors-node_modules_jupyterlab_application_style_index_js-node_modules_jupyterlab_console_st-8dc7b3\":\"f3e7c133ec1940ded4f9\",\"style_index_js-data_image_png_base64_iVBORw0KGgoAAAANSUhEUgAAAAgAAAAFCAYAAAB4ka1VAAAAsElEQVQI-adaf50\":\"2b034a8fa2de53285adf\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
-        "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab_pausable_contextual_help:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t};\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
+        "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab_pausable_contextual_help:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab_pausable_contextual_help\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab_pausable_contextual_help\", \"0.1.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_lumino_polling_dist_index_es6_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
-        "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,3,0,13])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,0,10])),\n\t\"webpack/sharing/consume/default/@jupyterlab/console\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/console\", [1,3,0,12])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,3,0,10])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,0,13])),\n\t\"webpack/sharing/consume/default/@jupyterlab/translation\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/translation\", [1,3,0,10])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,0,8])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,5,3])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,1,16,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/statedb\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/statedb\", [1,3,0,7])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,5,0,7])),\n\t\"webpack/sharing/consume/default/@jupyterlab/rendermime\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/rendermime\", [1,3,0,12])),\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,1,4,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/console\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/translation\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/statedb\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/rendermime\",\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
-        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab_pausable_contextual_help\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_pausable_contextual_help\"] = self[\"webpackChunkjupyterlab_pausable_contextual_help\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab_pausable_contextual_help\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab_pausable_contextual_help\", \"0.1.3\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,4,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,3,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/console\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/console\", [1,4,2,0])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/rendermime\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/rendermime\", [1,4,2,0])),\n\t\"webpack/sharing/consume/default/@lumino/polling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/polling\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,2,0,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/translation\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/translation\", [1,4,2,0])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,2,3,1,,\"alpha\",0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/statedb\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/statedb\", [1,4,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,4,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,2,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,2,0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/console\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/rendermime\",\n\t\t\"webpack/sharing/consume/default/@lumino/polling\",\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/translation\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/statedb\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\"\n\t]\n};\nvar startedInstallModules = {};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tif(!startedInstallModules[id]) {\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tstartedInstallModules[id] = true;\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t\t}\n\t\t});\n\t}\n}",
+        "__webpack_require__.b = document.baseURI || self.location.href;\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab_pausable_contextual_help\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_pausable_contextual_help\"] = self[\"webpackChunkjupyterlab_pausable_contextual_help\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab_pausable_contextual_help\");\n",
         ""
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/jupyterlab_pausable_contextual_help/labextension/static/vendors-node_modules_lumino_polling_dist_index_es6_js.35868735457bf9c961c0.js.map` & `jupyterlab_pausable_contextual_help-0.1.3/jupyterlab_pausable_contextual_help/labextension/static/lib_index_js.48d46625a03ec356bfc7.js.map`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7142857142857143%*

 * *Differences: {"'file'": "'lib_index_js.48d46625a03ec356bfc7.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;;;;;;;AAAA,0CAA0C;AAC1C,2DAA2D;AAGd;AAC2B;AAER;AAEpB;AACQ;AAGpD;;GAEG;AACI,MAAM,iBAAiB;IAC5B;;OAEG;IACH,YAAY,OAAmC;QA+JvC,aAAQ,GAAG,IAAI,qDAAM,CAA0B,IAAI,CAAC,CAAC;QAMrD,cAAS,GAAG,IAAI,qDAAM,CAAa,IAAI,CAAC,CAAC;QACzC,YAAO,GAA8B,IAAI,CAAC;QAC1C,eAAU,GAAG,IAAI,qDAAM,CAAwC,IAAI,CAAC,CAAC;QACrE,gBAAW,GAAG,KAAK,CAAC;QACpB,aAAQ,GAAG,CAAC,CAAC;QAEb,aAAQ,GAAG,IAAI,CAAC;QAEhB,wBAAmB,GAA4C,IAAI,CAAC;QA5K1E,IAAI,CAAC,UAAU,GAAG,OAAO, […]*

```diff
@@ -1,17 +1,21 @@
 {
-    "file": "vendors-node_modules_lumino_polling_dist_index_es6_js.35868735457bf9c961c0.js",
-    "mappings": "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",
+    "file": "lib_index_js.48d46625a03ec356bfc7.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
-        "webpack://jupyterlab_pausable_contextual_help/./node_modules/@lumino/polling/node_modules/tslib/tslib.es6.js",
-        "webpack://jupyterlab_pausable_contextual_help/./node_modules/@lumino/polling/src/poll.ts",
-        "webpack://jupyterlab_pausable_contextual_help/./node_modules/@lumino/polling/src/ratelimiter.ts"
+        "webpack://jupyterlab_pausable_contextual_help/./src/handler.ts",
+        "webpack://jupyterlab_pausable_contextual_help/./src/index.ts",
+        "webpack://jupyterlab_pausable_contextual_help/./src/kernelconnector.ts",
+        "webpack://jupyterlab_pausable_contextual_help/./src/myinspector.ts",
+        "webpack://jupyterlab_pausable_contextual_help/./src/tokens.ts"
     ],
     "sourcesContent": [
-        "/*! *****************************************************************************\r\nCopyright (c) Microsoft Corporation.\r\n\r\nPermission to use, copy, modify, and/or distribute this software for any\r\npurpose with or without fee is hereby granted.\r\n\r\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH\r\nREGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY\r\nAND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,\r\nINDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM\r\nLOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR\r\nOTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR\r\nPERFORMANCE OF THIS SOFTWARE.\r\n***************************************************************************** */\r\n/* global Reflect, Promise */\r\n\r\nvar extendStatics = function(d, b) {\r\n    extendStatics = Object.setPrototypeOf ||\r\n        ({ __proto__: [] } instanceof Array && function (d, b) { d.__proto__ = b; }) ||\r\n        function (d, b) { for (var p in b) if (Object.prototype.hasOwnProperty.call(b, p)) d[p] = b[p]; };\r\n    return extendStatics(d, b);\r\n};\r\n\r\nexport function __extends(d, b) {\r\n    if (typeof b !== \"function\" && b !== null)\r\n        throw new TypeError(\"Class extends value \" + String(b) + \" is not a constructor or null\");\r\n    extendStatics(d, b);\r\n    function __() { this.constructor = d; }\r\n    d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());\r\n}\r\n\r\nexport var __assign = function() {\r\n    __assign = Object.assign || function __assign(t) {\r\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\r\n            s = arguments[i];\r\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p)) t[p] = s[p];\r\n        }\r\n        return t;\r\n    }\r\n    return __assign.apply(this, arguments);\r\n}\r\n\r\nexport function __rest(s, e) {\r\n    var t = {};\r\n    for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p) && e.indexOf(p) < 0)\r\n        t[p] = s[p];\r\n    if (s != null && typeof Object.getOwnPropertySymbols === \"function\")\r\n        for (var i = 0, p = Object.getOwnPropertySymbols(s); i < p.length; i++) {\r\n            if (e.indexOf(p[i]) < 0 && Object.prototype.propertyIsEnumerable.call(s, p[i]))\r\n                t[p[i]] = s[p[i]];\r\n        }\r\n    return t;\r\n}\r\n\r\nexport function __decorate(decorators, target, key, desc) {\r\n    var c = arguments.length, r = c < 3 ? target : desc === null ? desc = Object.getOwnPropertyDescriptor(target, key) : desc, d;\r\n    if (typeof Reflect === \"object\" && typeof Reflect.decorate === \"function\") r = Reflect.decorate(decorators, target, key, desc);\r\n    else for (var i = decorators.length - 1; i >= 0; i--) if (d = decorators[i]) r = (c < 3 ? d(r) : c > 3 ? d(target, key, r) : d(target, key)) || r;\r\n    return c > 3 && r && Object.defineProperty(target, key, r), r;\r\n}\r\n\r\nexport function __param(paramIndex, decorator) {\r\n    return function (target, key) { decorator(target, key, paramIndex); }\r\n}\r\n\r\nexport function __metadata(metadataKey, metadataValue) {\r\n    if (typeof Reflect === \"object\" && typeof Reflect.metadata === \"function\") return Reflect.metadata(metadataKey, metadataValue);\r\n}\r\n\r\nexport function __awaiter(thisArg, _arguments, P, generator) {\r\n    function adopt(value) { return value instanceof P ? value : new P(function (resolve) { resolve(value); }); }\r\n    return new (P || (P = Promise))(function (resolve, reject) {\r\n        function fulfilled(value) { try { step(generator.next(value)); } catch (e) { reject(e); } }\r\n        function rejected(value) { try { step(generator[\"throw\"](value)); } catch (e) { reject(e); } }\r\n        function step(result) { result.done ? resolve(result.value) : adopt(result.value).then(fulfilled, rejected); }\r\n        step((generator = generator.apply(thisArg, _arguments || [])).next());\r\n    });\r\n}\r\n\r\nexport function __generator(thisArg, body) {\r\n    var _ = { label: 0, sent: function() { if (t[0] & 1) throw t[1]; return t[1]; }, trys: [], ops: [] }, f, y, t, g;\r\n    return g = { next: verb(0), \"throw\": verb(1), \"return\": verb(2) }, typeof Symbol === \"function\" && (g[Symbol.iterator] = function() { return this; }), g;\r\n    function verb(n) { return function (v) { return step([n, v]); }; }\r\n    function step(op) {\r\n        if (f) throw new TypeError(\"Generator is already executing.\");\r\n        while (_) try {\r\n            if (f = 1, y && (t = op[0] & 2 ? y[\"return\"] : op[0] ? y[\"throw\"] || ((t = y[\"return\"]) && t.call(y), 0) : y.next) && !(t = t.call(y, op[1])).done) return t;\r\n            if (y = 0, t) op = [op[0] & 2, t.value];\r\n            switch (op[0]) {\r\n                case 0: case 1: t = op; break;\r\n                case 4: _.label++; return { value: op[1], done: false };\r\n                case 5: _.label++; y = op[1]; op = [0]; continue;\r\n                case 7: op = _.ops.pop(); _.trys.pop(); continue;\r\n                default:\r\n                    if (!(t = _.trys, t = t.length > 0 && t[t.length - 1]) && (op[0] === 6 || op[0] === 2)) { _ = 0; continue; }\r\n                    if (op[0] === 3 && (!t || (op[1] > t[0] && op[1] < t[3]))) { _.label = op[1]; break; }\r\n                    if (op[0] === 6 && _.label < t[1]) { _.label = t[1]; t = op; break; }\r\n                    if (t && _.label < t[2]) { _.label = t[2]; _.ops.push(op); break; }\r\n                    if (t[2]) _.ops.pop();\r\n                    _.trys.pop(); continue;\r\n            }\r\n            op = body.call(thisArg, _);\r\n        } catch (e) { op = [6, e]; y = 0; } finally { f = t = 0; }\r\n        if (op[0] & 5) throw op[1]; return { value: op[0] ? op[1] : void 0, done: true };\r\n    }\r\n}\r\n\r\nexport var __createBinding = Object.create ? (function(o, m, k, k2) {\r\n    if (k2 === undefined) k2 = k;\r\n    Object.defineProperty(o, k2, { enumerable: true, get: function() { return m[k]; } });\r\n}) : (function(o, m, k, k2) {\r\n    if (k2 === undefined) k2 = k;\r\n    o[k2] = m[k];\r\n});\r\n\r\nexport function __exportStar(m, o) {\r\n    for (var p in m) if (p !== \"default\" && !Object.prototype.hasOwnProperty.call(o, p)) __createBinding(o, m, p);\r\n}\r\n\r\nexport function __values(o) {\r\n    var s = typeof Symbol === \"function\" && Symbol.iterator, m = s && o[s], i = 0;\r\n    if (m) return m.call(o);\r\n    if (o && typeof o.length === \"number\") return {\r\n        next: function () {\r\n            if (o && i >= o.length) o = void 0;\r\n            return { value: o && o[i++], done: !o };\r\n        }\r\n    };\r\n    throw new TypeError(s ? \"Object is not iterable.\" : \"Symbol.iterator is not defined.\");\r\n}\r\n\r\nexport function __read(o, n) {\r\n    var m = typeof Symbol === \"function\" && o[Symbol.iterator];\r\n    if (!m) return o;\r\n    var i = m.call(o), r, ar = [], e;\r\n    try {\r\n        while ((n === void 0 || n-- > 0) && !(r = i.next()).done) ar.push(r.value);\r\n    }\r\n    catch (error) { e = { error: error }; }\r\n    finally {\r\n        try {\r\n            if (r && !r.done && (m = i[\"return\"])) m.call(i);\r\n        }\r\n        finally { if (e) throw e.error; }\r\n    }\r\n    return ar;\r\n}\r\n\r\n/** @deprecated */\r\nexport function __spread() {\r\n    for (var ar = [], i = 0; i < arguments.length; i++)\r\n        ar = ar.concat(__read(arguments[i]));\r\n    return ar;\r\n}\r\n\r\n/** @deprecated */\r\nexport function __spreadArrays() {\r\n    for (var s = 0, i = 0, il = arguments.length; i < il; i++) s += arguments[i].length;\r\n    for (var r = Array(s), k = 0, i = 0; i < il; i++)\r\n        for (var a = arguments[i], j = 0, jl = a.length; j < jl; j++, k++)\r\n            r[k] = a[j];\r\n    return r;\r\n}\r\n\r\nexport function __spreadArray(to, from, pack) {\r\n    if (pack || arguments.length === 2) for (var i = 0, l = from.length, ar; i < l; i++) {\r\n        if (ar || !(i in from)) {\r\n            if (!ar) ar = Array.prototype.slice.call(from, 0, i);\r\n            ar[i] = from[i];\r\n        }\r\n    }\r\n    return to.concat(ar || from);\r\n}\r\n\r\nexport function __await(v) {\r\n    return this instanceof __await ? (this.v = v, this) : new __await(v);\r\n}\r\n\r\nexport function __asyncGenerator(thisArg, _arguments, generator) {\r\n    if (!Symbol.asyncIterator) throw new TypeError(\"Symbol.asyncIterator is not defined.\");\r\n    var g = generator.apply(thisArg, _arguments || []), i, q = [];\r\n    return i = {}, verb(\"next\"), verb(\"throw\"), verb(\"return\"), i[Symbol.asyncIterator] = function () { return this; }, i;\r\n    function verb(n) { if (g[n]) i[n] = function (v) { return new Promise(function (a, b) { q.push([n, v, a, b]) > 1 || resume(n, v); }); }; }\r\n    function resume(n, v) { try { step(g[n](v)); } catch (e) { settle(q[0][3], e); } }\r\n    function step(r) { r.value instanceof __await ? Promise.resolve(r.value.v).then(fulfill, reject) : settle(q[0][2], r); }\r\n    function fulfill(value) { resume(\"next\", value); }\r\n    function reject(value) { resume(\"throw\", value); }\r\n    function settle(f, v) { if (f(v), q.shift(), q.length) resume(q[0][0], q[0][1]); }\r\n}\r\n\r\nexport function __asyncDelegator(o) {\r\n    var i, p;\r\n    return i = {}, verb(\"next\"), verb(\"throw\", function (e) { throw e; }), verb(\"return\"), i[Symbol.iterator] = function () { return this; }, i;\r\n    function verb(n, f) { i[n] = o[n] ? function (v) { return (p = !p) ? { value: __await(o[n](v)), done: n === \"return\" } : f ? f(v) : v; } : f; }\r\n}\r\n\r\nexport function __asyncValues(o) {\r\n    if (!Symbol.asyncIterator) throw new TypeError(\"Symbol.asyncIterator is not defined.\");\r\n    var m = o[Symbol.asyncIterator], i;\r\n    return m ? m.call(o) : (o = typeof __values === \"function\" ? __values(o) : o[Symbol.iterator](), i = {}, verb(\"next\"), verb(\"throw\"), verb(\"return\"), i[Symbol.asyncIterator] = function () { return this; }, i);\r\n    function verb(n) { i[n] = o[n] && function (v) { return new Promise(function (resolve, reject) { v = o[n](v), settle(resolve, reject, v.done, v.value); }); }; }\r\n    function settle(resolve, reject, d, v) { Promise.resolve(v).then(function(v) { resolve({ value: v, done: d }); }, reject); }\r\n}\r\n\r\nexport function __makeTemplateObject(cooked, raw) {\r\n    if (Object.defineProperty) { Object.defineProperty(cooked, \"raw\", { value: raw }); } else { cooked.raw = raw; }\r\n    return cooked;\r\n};\r\n\r\nvar __setModuleDefault = Object.create ? (function(o, v) {\r\n    Object.defineProperty(o, \"default\", { enumerable: true, value: v });\r\n}) : function(o, v) {\r\n    o[\"default\"] = v;\r\n};\r\n\r\nexport function __importStar(mod) {\r\n    if (mod && mod.__esModule) return mod;\r\n    var result = {};\r\n    if (mod != null) for (var k in mod) if (k !== \"default\" && Object.prototype.hasOwnProperty.call(mod, k)) __createBinding(result, mod, k);\r\n    __setModuleDefault(result, mod);\r\n    return result;\r\n}\r\n\r\nexport function __importDefault(mod) {\r\n    return (mod && mod.__esModule) ? mod : { default: mod };\r\n}\r\n\r\nexport function __classPrivateFieldGet(receiver, state, kind, f) {\r\n    if (kind === \"a\" && !f) throw new TypeError(\"Private accessor was defined without a getter\");\r\n    if (typeof state === \"function\" ? receiver !== state || !f : !state.has(receiver)) throw new TypeError(\"Cannot read private member from an object whose class did not declare it\");\r\n    return kind === \"m\" ? f : kind === \"a\" ? f.call(receiver) : f ? f.value : state.get(receiver);\r\n}\r\n\r\nexport function __classPrivateFieldSet(receiver, state, value, kind, f) {\r\n    if (kind === \"m\") throw new TypeError(\"Private method is not writable\");\r\n    if (kind === \"a\" && !f) throw new TypeError(\"Private accessor was defined without a setter\");\r\n    if (typeof state === \"function\" ? receiver !== state || !f : !state.has(receiver)) throw new TypeError(\"Cannot write private member to an object whose class did not declare it\");\r\n    return (kind === \"a\" ? f.call(receiver, value) : f ? f.value = value : state.set(receiver, value)), value;\r\n}\r\n",
-        "// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\n\nimport { JSONExt, PromiseDelegate } from '@lumino/coreutils';\n\nimport { IObservableDisposable } from '@lumino/disposable';\n\nimport { ISignal, Signal } from '@lumino/signaling';\n\nimport { IPoll } from './index';\n\n/**\n * A function to defer an action immediately.\n */\nconst defer =\n  typeof requestAnimationFrame === 'function'\n    ? requestAnimationFrame\n    : setImmediate;\n\n/**\n * A function to cancel a deferred action.\n */\nconst cancel: (timeout: any) => void =\n  typeof cancelAnimationFrame === 'function'\n    ? cancelAnimationFrame\n    : clearImmediate;\n\n/**\n * A class that wraps an asynchronous function to poll at a regular interval\n * with exponential increases to the interval length if the poll fails.\n *\n * @typeparam T - The resolved type of the factory's promises.\n * Defaults to `any`.\n *\n * @typeparam U - The rejected type of the factory's promises.\n * Defaults to `any`.\n *\n * @typeparam V - An optional type to extend the phases supported by a poll.\n * Defaults to `standby`, which already exists in the `Phase` type.\n */\nexport class Poll<T = any, U = any, V extends string = 'standby'>\n  implements IObservableDisposable, IPoll<T, U, V> {\n  /**\n   * Instantiate a new poll with exponential backoff in case of failure.\n   *\n   * @param options - The poll instantiation options.\n   */\n  constructor(options: Poll.IOptions<T, U, V>) {\n    this._factory = options.factory;\n    this._standby = options.standby || Private.DEFAULT_STANDBY;\n    this._state = { ...Private.DEFAULT_STATE, timestamp: new Date().getTime() };\n\n    // Normalize poll frequency `max` to be the greater of\n    // default `max`, `options.frequency.max`, or `options.frequency.interval`.\n    const frequency = options.frequency || {};\n    const max = Math.max(\n      frequency.interval || 0,\n      frequency.max || 0,\n      Private.DEFAULT_FREQUENCY.max\n    );\n    this.frequency = { ...Private.DEFAULT_FREQUENCY, ...frequency, ...{ max } };\n\n    this.name = options.name || Private.DEFAULT_NAME;\n\n    if ('auto' in options ? options.auto : true) {\n      defer(() => void this.start());\n    }\n  }\n\n  /**\n   * The name of the poll.\n   */\n  readonly name: string;\n\n  /**\n   * A signal emitted when the poll is disposed.\n   */\n  get disposed(): ISignal<this, void> {\n    return this._disposed;\n  }\n\n  /**\n   * The polling frequency parameters.\n   */\n  get frequency(): IPoll.Frequency {\n    return this._frequency;\n  }\n  set frequency(frequency: IPoll.Frequency) {\n    if (this.isDisposed || JSONExt.deepEqual(frequency, this.frequency || {})) {\n      return;\n    }\n\n    let { backoff, interval, max } = frequency;\n\n    interval = Math.round(interval);\n    max = Math.round(max);\n\n    if (typeof backoff === 'number' && backoff < 1) {\n      throw new Error('Poll backoff growth factor must be at least 1');\n    }\n\n    if ((interval < 0 || interval > max) && interval !== Poll.NEVER) {\n      throw new Error('Poll interval must be between 0 and max');\n    }\n\n    if (max > Poll.MAX_INTERVAL && max !== Poll.NEVER) {\n      throw new Error(`Max interval must be less than ${Poll.MAX_INTERVAL}`);\n    }\n\n    this._frequency = { backoff, interval, max };\n  }\n\n  /**\n   * Whether the poll is disposed.\n   */\n  get isDisposed(): boolean {\n    return this.state.phase === 'disposed';\n  }\n\n  /**\n   * Indicates when the poll switches to standby.\n   */\n  get standby(): Poll.Standby | (() => boolean | Poll.Standby) {\n    return this._standby;\n  }\n  set standby(standby: Poll.Standby | (() => boolean | Poll.Standby)) {\n    if (this.isDisposed || this.standby === standby) {\n      return;\n    }\n\n    this._standby = standby;\n  }\n\n  /**\n   * The poll state, which is the content of the current poll tick.\n   */\n  get state(): IPoll.State<T, U, V> {\n    return this._state;\n  }\n\n  /**\n   * A promise that resolves when the poll next ticks.\n   */\n  get tick(): Promise<this> {\n    return this._tick.promise;\n  }\n\n  /**\n   * A signal emitted when the poll ticks and fires off a new request.\n   */\n  get ticked(): ISignal<this, IPoll.State<T, U, V>> {\n    return this._ticked;\n  }\n\n  /**\n   * Dispose the poll.\n   */\n  dispose(): void {\n    if (this.isDisposed) {\n      return;\n    }\n\n    this._state = {\n      ...Private.DISPOSED_STATE,\n      timestamp: new Date().getTime()\n    };\n    this._tick.promise.catch(_ => undefined);\n    this._tick.reject(new Error(`Poll (${this.name}) is disposed.`));\n    this._disposed.emit(undefined);\n    Signal.clearData(this);\n  }\n\n  /**\n   * Refreshes the poll. Schedules `refreshed` tick if necessary.\n   *\n   * @returns A promise that resolves after tick is scheduled and never rejects.\n   *\n   * #### Notes\n   * The returned promise resolves after the tick is scheduled, but before\n   * the polling action is run. To wait until after the poll action executes,\n   * await the `poll.tick` promise: `await poll.refresh(); await poll.tick;`\n   */\n  refresh(): Promise<void> {\n    return this.schedule({\n      cancel: ({ phase }) => phase === 'refreshed',\n      interval: Poll.IMMEDIATE,\n      phase: 'refreshed'\n    });\n  }\n\n  /**\n   * Schedule the next poll tick.\n   *\n   * @param next - The next poll state data to schedule. Defaults to standby.\n   *\n   * @param next.cancel - Cancels state transition if function returns `true`.\n   *\n   * @returns A promise that resolves when the next poll state is active.\n   *\n   * #### Notes\n   * This method is not meant to be invoked by user code typically. It is public\n   * to allow poll instances to be composed into classes that schedule ticks.\n   */\n  async schedule(\n    next: Partial<\n      IPoll.State<T, U, V> & { cancel: (last: IPoll.State<T, U, V>) => boolean }\n    > = {}\n  ): Promise<void> {\n    if (this.isDisposed) {\n      return;\n    }\n\n    // Check if the phase transition should be canceled.\n    if (next.cancel && next.cancel(this.state)) {\n      return;\n    }\n\n    // Update poll state.\n    const last = this.state;\n    const pending = this._tick;\n    const scheduled = new PromiseDelegate<this>();\n    const state = {\n      interval: this.frequency.interval,\n      payload: null,\n      phase: 'standby',\n      timestamp: new Date().getTime(),\n      ...next\n    } as IPoll.State<T, U, V>;\n    this._state = state;\n    this._tick = scheduled;\n\n    // Clear the schedule if possible.\n    if (last.interval === Poll.IMMEDIATE) {\n      cancel(this._timeout);\n    } else {\n      clearTimeout(this._timeout);\n    }\n\n    // Emit ticked signal, resolve pending promise, and await its settlement.\n    this._ticked.emit(this.state);\n    pending.resolve(this);\n    await pending.promise;\n\n    // Schedule next execution and cache its timeout handle.\n    const execute = () => {\n      if (this.isDisposed || this.tick !== scheduled.promise) {\n        return;\n      }\n\n      this._execute();\n    };\n    this._timeout =\n      state.interval === Poll.IMMEDIATE\n        ? defer(execute)\n        : state.interval === Poll.NEVER\n        ? -1\n        : setTimeout(execute, state.interval);\n  }\n\n  /**\n   * Starts the poll. Schedules `started` tick if necessary.\n   *\n   * @returns A promise that resolves after tick is scheduled and never rejects.\n   */\n  start(): Promise<void> {\n    return this.schedule({\n      cancel: ({ phase }) =>\n        phase !== 'constructed' && phase !== 'standby' && phase !== 'stopped',\n      interval: Poll.IMMEDIATE,\n      phase: 'started'\n    });\n  }\n\n  /**\n   * Stops the poll. Schedules `stopped` tick if necessary.\n   *\n   * @returns A promise that resolves after tick is scheduled and never rejects.\n   */\n  stop(): Promise<void> {\n    return this.schedule({\n      cancel: ({ phase }) => phase === 'stopped',\n      interval: Poll.NEVER,\n      phase: 'stopped'\n    });\n  }\n\n  /**\n   * Execute a new poll factory promise or stand by if necessary.\n   */\n  private _execute(): void {\n    let standby =\n      typeof this.standby === 'function' ? this.standby() : this.standby;\n    standby =\n      standby === 'never'\n        ? false\n        : standby === 'when-hidden'\n        ? !!(typeof document !== 'undefined' && document && document.hidden)\n        : standby;\n\n    // If in standby mode schedule next tick without calling the factory.\n    if (standby) {\n      void this.schedule();\n      return;\n    }\n\n    const pending = this.tick;\n\n    this._factory(this.state)\n      .then((resolved: T) => {\n        if (this.isDisposed || this.tick !== pending) {\n          return;\n        }\n\n        void this.schedule({\n          payload: resolved,\n          phase: this.state.phase === 'rejected' ? 'reconnected' : 'resolved'\n        });\n      })\n      .catch((rejected: U) => {\n        if (this.isDisposed || this.tick !== pending) {\n          return;\n        }\n\n        void this.schedule({\n          interval: Private.sleep(this.frequency, this.state),\n          payload: rejected,\n          phase: 'rejected'\n        });\n      });\n  }\n\n  private _disposed = new Signal<this, void>(this);\n  private _factory: Poll.Factory<T, U, V>;\n  private _frequency: IPoll.Frequency;\n  private _standby: Poll.Standby | (() => boolean | Poll.Standby);\n  private _state: IPoll.State<T, U, V>;\n  private _tick = new PromiseDelegate<this>();\n  private _ticked = new Signal<this, IPoll.State<T, U, V>>(this);\n  private _timeout: any = -1;\n}\n\n/**\n * A namespace for `Poll` types, interfaces, and statics.\n */\nexport namespace Poll {\n  /**\n   * A promise factory that returns an individual poll request.\n   *\n   * @typeparam T - The resolved type of the factory's promises.\n   *\n   * @typeparam U - The rejected type of the factory's promises.\n   *\n   * @typeparam V - The type to extend the phases supported by a poll.\n   */\n  export type Factory<T, U, V extends string> = (\n    state: IPoll.State<T, U, V>\n  ) => Promise<T>;\n\n  /**\n   * Indicates when the poll switches to standby.\n   */\n  export type Standby = 'never' | 'when-hidden';\n\n  /**\n   * Instantiation options for polls.\n   *\n   * @typeparam T - The resolved type of the factory's promises.\n   *\n   * @typeparam U - The rejected type of the factory's promises.\n   *\n   * @typeparam V - The type to extend the phases supported by a poll.\n   */\n  export interface IOptions<T, U, V extends string> {\n    /**\n     * Whether to begin polling automatically; defaults to `true`.\n     */\n    auto?: boolean;\n\n    /**\n     * A factory function that is passed a poll tick and returns a poll promise.\n     */\n    factory: Factory<T, U, V>;\n\n    /**\n     * The polling frequency parameters.\n     */\n    frequency?: Partial<IPoll.Frequency>;\n\n    /**\n     * The name of the poll.\n     * Defaults to `'unknown'`.\n     */\n    name?: string;\n\n    /**\n     * Indicates when the poll switches to standby or a function that returns\n     * a boolean or a `Poll.Standby` value to indicate whether to stand by.\n     * Defaults to `'when-hidden'`.\n     *\n     * #### Notes\n     * If a function is passed in, for any given context, it should be\n     * idempotent and safe to call multiple times. It will be called before each\n     * tick execution, but may be called by clients as well.\n     */\n    standby?: Standby | (() => boolean | Standby);\n  }\n  /**\n   * An interval value that indicates the poll should tick immediately.\n   */\n  export const IMMEDIATE = 0;\n\n  /**\n   * Delays are 32-bit integers in many browsers so intervals need to be capped.\n   *\n   * #### Notes\n   * https://developer.mozilla.org/en-US/docs/Web/API/WindowOrWorkerGlobalScope/setTimeout#Maximum_delay_value\n   */\n  export const MAX_INTERVAL = 2147483647;\n\n  /**\n   * An interval value that indicates the poll should never tick.\n   */\n  export const NEVER = Infinity;\n}\n\n/**\n * A namespace for private module data.\n */\nnamespace Private {\n  /**\n   * The default backoff growth rate if `backoff` is `true`.\n   */\n  export const DEFAULT_BACKOFF = 3;\n\n  /**\n   * The default polling frequency.\n   */\n  export const DEFAULT_FREQUENCY: IPoll.Frequency = {\n    backoff: true,\n    interval: 1000,\n    max: 30 * 1000\n  };\n\n  /**\n   * The default poll name.\n   */\n  export const DEFAULT_NAME = 'unknown';\n\n  /**\n   * The default poll standby behavior.\n   */\n  export const DEFAULT_STANDBY: Poll.Standby = 'when-hidden';\n\n  /**\n   * The first poll tick state's default values superseded in constructor.\n   */\n  export const DEFAULT_STATE: IPoll.State<any, any, any> = {\n    interval: Poll.NEVER,\n    payload: null,\n    phase: 'constructed',\n    timestamp: new Date(0).getTime()\n  };\n\n  /**\n   * The disposed tick state values.\n   */\n  export const DISPOSED_STATE: IPoll.State<any, any, any> = {\n    interval: Poll.NEVER,\n    payload: null,\n    phase: 'disposed',\n    timestamp: new Date(0).getTime()\n  };\n\n  /**\n   * Get a random integer between min and max, inclusive of both.\n   *\n   * #### Notes\n   * From\n   * https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random#Getting_a_random_integer_between_two_values_inclusive\n   *\n   * From the MDN page: It might be tempting to use Math.round() to accomplish\n   * that, but doing so would cause your random numbers to follow a non-uniform\n   * distribution, which may not be acceptable for your needs.\n   */\n  function getRandomIntInclusive(min: number, max: number) {\n    min = Math.ceil(min);\n    max = Math.floor(max);\n    return Math.floor(Math.random() * (max - min + 1)) + min;\n  }\n\n  /**\n   * Returns the number of milliseconds to sleep before the next tick.\n   *\n   * @param frequency - The poll's base frequency.\n   * @param last - The poll's last tick.\n   */\n  export function sleep(\n    frequency: IPoll.Frequency,\n    last: IPoll.State<any, any, any>\n  ): number {\n    const { backoff, interval, max } = frequency;\n\n    if (interval === Poll.NEVER) {\n      return interval;\n    }\n\n    const growth =\n      backoff === true ? DEFAULT_BACKOFF : backoff === false ? 1 : backoff;\n    const random = getRandomIntInclusive(interval, last.interval * growth);\n\n    return Math.min(max, random);\n  }\n}\n",
-        "// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\n\nimport { PromiseDelegate } from '@lumino/coreutils';\n\nimport { IRateLimiter } from './index';\n\nimport { Poll } from './poll';\n\n/**\n * A base class to implement rate limiters with different invocation strategies.\n *\n * @typeparam T - The resolved type of the underlying function.\n *\n * @typeparam U - The rejected type of the underlying function.\n *\n * @typeparam V - Arguments for the underlying function.\n */\nexport abstract class RateLimiter<T, U, V extends any[]>\n  implements IRateLimiter<T, U, V> {\n  /**\n   * Instantiate a rate limiter.\n   *\n   * @param fn - The function to rate limit.\n   *\n   * @param limit - The rate limit; defaults to 500ms.\n   */\n  constructor(fn: (...args: V) => T | Promise<T>, limit = 500) {\n    this.limit = limit;\n    this.poll = new Poll({\n      auto: false,\n      factory: async () => {\n        const { args } = this;\n        this.args = undefined;\n        return fn(...args!);\n      },\n      frequency: { backoff: false, interval: Poll.NEVER, max: Poll.NEVER },\n      standby: 'never'\n    });\n    this.payload = new PromiseDelegate();\n    this.poll.ticked.connect((_, state) => {\n      const { payload } = this;\n\n      if (state.phase === 'resolved') {\n        this.payload = new PromiseDelegate();\n        payload!.resolve(state.payload as T);\n        return;\n      }\n\n      if (state.phase === 'rejected' || state.phase === 'stopped') {\n        this.payload = new PromiseDelegate();\n        payload!.promise.catch(_ => undefined);\n        payload!.reject(state.payload as U);\n        return;\n      }\n    }, this);\n  }\n\n  /**\n   * Whether the rate limiter is disposed.\n   */\n  get isDisposed(): boolean {\n    return this.payload === null;\n  }\n\n  /**\n   * Disposes the rate limiter.\n   */\n  dispose(): void {\n    if (this.isDisposed) {\n      return;\n    }\n    this.args = undefined;\n    this.payload = null;\n    this.poll.dispose();\n  }\n\n  /**\n   * The rate limit in milliseconds.\n   */\n  readonly limit: number;\n\n  /**\n   * Invoke the rate limited function.\n   */\n  abstract invoke(...args: V): Promise<T>;\n\n  /**\n   * Stop the function if it is mid-flight.\n   */\n  async stop(): Promise<void> {\n    return this.poll.stop();\n  }\n\n  /**\n   * Arguments for the underlying function.\n   */\n  protected args: V | undefined = undefined;\n\n  /**\n   * A promise that resolves on each successful invocation.\n   */\n  protected payload: PromiseDelegate<T> | null = null;\n\n  /**\n   * The underlying poll instance used by the rate limiter.\n   */\n  protected poll: Poll<T, U, 'invoked'>;\n}\n\n/**\n * Wraps and debounces a function that can be called multiple times and only\n * executes the underlying function one `interval` after the last invocation.\n *\n * @typeparam T - The resolved type of the underlying function. Defaults to any.\n *\n * @typeparam U - The rejected type of the underlying function. Defaults to any.\n *\n * @typeparam V - Arguments for the underlying function. Defaults to any[].\n */\nexport class Debouncer<\n  T = any,\n  U = any,\n  V extends any[] = any[]\n> extends RateLimiter<T, U, V> {\n  /**\n   * Invokes the function and only executes after rate limit has elapsed.\n   * Each invocation resets the timer.\n   */\n  invoke(...args: V): Promise<T> {\n    this.args = args;\n    void this.poll.schedule({ interval: this.limit, phase: 'invoked' });\n    return this.payload!.promise;\n  }\n}\n\n/**\n * Wraps and throttles a function that can be called multiple times and only\n * executes the underlying function once per `interval`.\n *\n * @typeparam T - The resolved type of the underlying function. Defaults to any.\n *\n * @typeparam U - The rejected type of the underlying function. Defaults to any.\n *\n * @typeparam V - Arguments for the underlying function. Defaults to any[].\n */\nexport class Throttler<\n  T = any,\n  U = any,\n  V extends any[] = any[]\n> extends RateLimiter<T, U, V> {\n  /**\n   * Instantiate a throttler.\n   *\n   * @param fn - The function being throttled.\n   *\n   * @param options - Throttling configuration or throttling limit in ms.\n   *\n   * #### Notes\n   * The `edge` defaults to `leading`; the `limit` defaults to `500`.\n   */\n  constructor(\n    fn: (...args: V) => T | Promise<T>,\n    options?: Throttler.IOptions | number\n  ) {\n    super(fn, typeof options === 'number' ? options : options && options.limit);\n    if (typeof options !== 'number' && options && options.edge === 'trailing') {\n      this._trailing = true;\n    }\n    this._interval = this._trailing ? this.limit : Poll.IMMEDIATE;\n  }\n\n  /**\n   * Throttles function invocations if one is currently in flight.\n   */\n  invoke(...args: V): Promise<T> {\n    const idle = this.poll.state.phase !== 'invoked';\n    if (idle || this._trailing) {\n      this.args = args;\n    }\n    if (idle) {\n      void this.poll.schedule({ interval: this._interval, phase: 'invoked' });\n    }\n    return this.payload!.promise;\n  }\n\n  private _interval: number;\n  private _trailing = false;\n}\n\n/**\n * A namespace for `Throttler` interfaces.\n */\nexport namespace Throttler {\n  /**\n   * Instantiation options for a `Throttler`.\n   */\n  export interface IOptions {\n    /**\n     * The throttling limit; defaults to 500ms.\n     */\n    limit?: number;\n\n    /**\n     * Whether to invoke at the leading or trailing edge of throttle cycle.\n     * Defaults to `leading`.\n     */\n    edge?: 'leading' | 'trailing';\n  }\n}\n"
+        "// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\n\nimport { CodeEditor } from '@jupyterlab/codeeditor';\nimport { Text } from '@jupyterlab/coreutils';\nimport { IRenderMimeRegistry, MimeModel } from '@jupyterlab/rendermime';\nimport { IDataConnector } from '@jupyterlab/statedb';\nimport { JSONExt, ReadonlyJSONObject } from '@lumino/coreutils';\nimport { IDisposable } from '@lumino/disposable';\nimport { Debouncer } from '@lumino/polling';\nimport { ISignal, Signal } from '@lumino/signaling';\nimport { IMyInspector } from './tokens';\n\n/**\n * An object that handles code inspection.\n */\nexport class InspectionHandler implements IDisposable, IMyInspector.IInspectable {\n  /**\n   * Construct a new inspection handler for a widget.\n   */\n  constructor(options: InspectionHandler.IOptions) {\n    this._connector = options.connector;\n    this._rendermime = options.rendermime;\n    this._debouncer = new Debouncer(this.onEditorChange.bind(this), 250);\n  }\n\n  /**\n   * A signal emitted when the myinspector should clear all items.\n   */\n  get cleared(): ISignal<InspectionHandler, void> {\n    return this._cleared;\n  }\n\n  /**\n   * A signal emitted when the handler is disposed.\n   */\n  get disposed(): ISignal<InspectionHandler, void> {\n    return this._disposed;\n  }\n\n  /**\n   * A signal emitted when an myinspector value is generated.\n   */\n  get inspected(): ISignal<InspectionHandler, IMyInspector.IMyInspectorUpdate> {\n    return this._inspected;\n  }\n\n  /**\n   * The editor widget used by the inspection handler.\n   */\n  get editor(): CodeEditor.IEditor | null {\n    return this._editor;\n  }\n  set editor(newValue: CodeEditor.IEditor | null) {\n    if (newValue === this._editor) {\n      return;\n    }\n    // Remove all of our listeners.\n    Signal.disconnectReceiver(this);\n\n    const editor = (this._editor = newValue);\n    if (editor) {\n      // Clear the myinspector in preparation for a new editor.\n      this._cleared.emit(void 0);\n      // Call onEditorChange to cover the case where the user changes\n      // the active cell\n      this.onEditorChange();\n      editor.model.selections.changed.connect(this._onChange, this);\n      editor.model.sharedModel.changed.connect(this._onChange, this);\n    }\n  }\n\n  /**\n   * Indicates whether the handler makes API inspection requests or stands by.\n   *\n   * #### Notes\n   * The use case for this attribute is to limit the API traffic when no\n   * myinspector is visible.\n   */\n  get standby(): boolean {\n    return this._standby;\n  }\n  set standby(value: boolean) {\n    this._standby = value;\n  }\n\n  /**\n   * Get whether the inspection handler is disposed.\n   *\n   * #### Notes\n   * This is a read-only property.\n   */\n  get isDisposed(): boolean {\n    return this._isDisposed;\n  }\n\n  /**\n   * Dispose of the resources used by the handler.\n   */\n  dispose(): void {\n    if (this.isDisposed) {\n      return;\n    }\n    this._isDisposed = true;\n    this._debouncer.dispose();\n    this._disposed.emit(void 0);\n    Signal.clearData(this);\n  }\n\n  /**\n   * Handle a text changed signal from an editor.\n   *\n   * #### Notes\n   * Update the hints myinspector based on a text change.\n   */\n  onEditorChange(customText?: string): void {\n    // If the handler is in standby mode, bail.\n    if (this._standby) {\n      return;\n    }\n\n    const editor = this.editor;\n\n    if (!editor) {\n      return;\n    }\n    const text = customText ? customText : editor.model.sharedModel.getSource();\n    const position = editor.getCursorPosition();\n    const offset = Text.jsIndexToCharIndex(editor.getOffsetAt(position), text);\n    const update: IMyInspector.IMyInspectorUpdate = { content: null };\n\n    const pending = ++this._pending;\n\n    void this._connector\n      .fetch({ offset, text })\n      .then(reply => {\n        // If handler has been disposed or a newer request is pending, bail.\n        if (!reply || this.isDisposed || pending !== this._pending) {\n          this._lastInspectedReply = null;\n          this._inspected.emit(update);\n          return;\n        }\n\n        const { data } = reply;\n\n        // Do not update if there would be no change.\n        if (\n          this._lastInspectedReply &&\n          JSONExt.deepEqual(this._lastInspectedReply, data)\n        ) {\n          return;\n        }\n\n        const mimeType = this._rendermime.preferredMimeType(data);\n        if (mimeType) {\n          const widget = this._rendermime.createRenderer(mimeType);\n          const model = new MimeModel({ data });\n\n          void widget.renderModel(model);\n          update.content = widget;\n        }\n\n        this._lastInspectedReply = reply.data;\n        this._inspected.emit(update);\n      })\n      .catch(reason => {\n        // Since almost all failures are benign, fail silently.\n        this._lastInspectedReply = null;\n        this._inspected.emit(update);\n      });\n  }\n\n  /**\n   * Handle changes to the editor state, debouncing.\n   */\n  private _onChange(): void {\n    void this._debouncer.invoke();\n  }\n\n  private _cleared = new Signal<InspectionHandler, void>(this);\n  private _connector: IDataConnector<\n    InspectionHandler.IReply,\n    void,\n    InspectionHandler.IRequest\n  >;\n  private _disposed = new Signal<this, void>(this);\n  private _editor: CodeEditor.IEditor | null = null;\n  private _inspected = new Signal<this, IMyInspector.IMyInspectorUpdate>(this);\n  private _isDisposed = false;\n  private _pending = 0;\n  private _rendermime: IRenderMimeRegistry;\n  private _standby = true;\n  private _debouncer: Debouncer;\n  private _lastInspectedReply: InspectionHandler.IReply['data'] | null = null;\n}\n\n/**\n * A namespace for inspection handler statics.\n */\nexport namespace InspectionHandler {\n  /**\n   * The instantiation options for an inspection handler.\n   */\n  export interface IOptions {\n    /**\n     * The connector used to make inspection requests.\n     *\n     * #### Notes\n     * The only method of this connector that will ever be called is `fetch`, so\n     * it is acceptable for the other methods to be simple functions that return\n     * rejected promises.\n     */\n    connector: IDataConnector<IReply, void, IRequest>;\n\n    /**\n     * The mime renderer for the inspection handler.\n     */\n    rendermime: IRenderMimeRegistry;\n  }\n\n  /**\n   * A reply to an inspection request.\n   */\n  export interface IReply {\n    /**\n     * The MIME bundle data returned from an inspection request.\n     */\n    data: ReadonlyJSONObject;\n\n    /**\n     * Any metadata that accompanies the MIME bundle returning from a request.\n     */\n    metadata: ReadonlyJSONObject;\n  }\n\n  /**\n   * The details of an inspection request.\n   */\n  export interface IRequest {\n    /**\n     * The cursor offset position within the text being inspected.\n     */\n    offset: number;\n\n    /**\n     * The text being inspected.\n     */\n    text: string;\n  }\n}\n",
+        "// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\n\n// export * from './handler';\n// export * from './myinspector';\n// export * from './kernelconnector';\n// export * from './tokens';\n\n// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  ILabShell,\n  ILayoutRestorer,\n  JupyterFrontEnd,\n  JupyterFrontEndPlugin\n} from '@jupyterlab/application';\n\n// import { ISettingRegistry } from '@jupyterlab/settingregistry';\n\nimport {\n  ICommandPalette,\n  MainAreaWidget,\n  WidgetTracker\n} from '@jupyterlab/apputils';\nimport { IConsoleTracker } from '@jupyterlab/console';\n//   import {\n//     IMyInspector,\n//     InspectionHandler,\n//     MyInspectorPanel,\n//     KernelConnector\n//   } from '@jupyterlab/inspector';\nimport { IMyInspector } from './tokens';\nimport { InspectionHandler } from './handler';\nimport { MyInspectorPanel } from './myinspector';\nimport { KernelConnector } from './kernelconnector';\n\n\nimport { ILauncher } from '@jupyterlab/launcher';\nimport { INotebookTracker } from '@jupyterlab/notebook';\nimport { ITranslator } from '@jupyterlab/translation';\nimport { inspectorIcon } from '@jupyterlab/ui-components';\nimport { Widget } from '@lumino/widgets';\n\n/**\n * The command IDs used by the myinspector plugin.\n */\nnamespace CommandIDs {\n  export const open = 'myinspector:open';\n  export const close = 'myinspector:close';\n  export const toggle = 'myinspector:toggle';\n  export const trigger = 'myinspector:trigger';\n  export const toggleStandby = 'myinspector:toggleStandby';\n}\n\n/**\n * A service providing code introspection.\n */\nconst myinspector: JupyterFrontEndPlugin<IMyInspector> = {\n  id: 'jupyterlab_pausable_contextual_help:myinspector',\n  description: 'Provides the pausable code introspection widget.',\n  requires: [ITranslator],\n  optional: [ICommandPalette, ILauncher, ILayoutRestorer],\n  provides: IMyInspector,\n  autoStart: true,\n  activate: (\n    app: JupyterFrontEnd,\n    translator: ITranslator,\n    palette: ICommandPalette | null,\n    launcher: ILauncher | null,\n    restorer: ILayoutRestorer | null\n  ): IMyInspector => {\n    const trans = translator.load('jupyterlab');\n    const { commands, shell } = app;\n    const caption = trans.__(\n            'Manually updating code documentation from the active kernel'\n    );\n    const openedLabel = trans.__('My Contextual Help');\n    const namespace = 'myinspector';\n    const datasetKey = 'jpMyInspector';\n    const tracker = new WidgetTracker<MainAreaWidget<MyInspectorPanel>>({\n      namespace\n    });\n\n    function isMyInspectorOpen() {\n      return myinspector && !myinspector.isDisposed;\n    }\n\n    function isStandby() {\n      // return myinspector && myinspector.content && myinspector.content.source && myinspector.content.source.standby;\n      if (myinspector && myinspector.content && myinspector.content.source) {\n        return myinspector.content.source.standby;\n      }\n      return false;\n    }\n\n    let source: IMyInspector.IInspectable | null = null;\n    let myinspector: MainAreaWidget<MyInspectorPanel>;\n    function openMyInspector(args: string): MainAreaWidget<MyInspectorPanel> {\n      if (!isMyInspectorOpen()) {\n        myinspector = new MainAreaWidget({\n          content: new MyInspectorPanel({ translator })\n        });\n        myinspector.id = 'jp-myinspector';\n        myinspector.title.label = openedLabel;\n        myinspector.title.icon = inspectorIcon;\n        void tracker.add(myinspector);\n        source = source && !source.isDisposed ? source : null;\n        myinspector.content.source = source;\n        myinspector.content.source?.onEditorChange(args);\n      }\n      if (!myinspector.isAttached) {\n        shell.add(myinspector, 'main', {\n          activate: false,\n          mode: 'split-right',\n          type: 'MyInspector'\n        });\n      }\n      shell.activateById(myinspector.id);\n      document.body.dataset[datasetKey] = 'open';\n      return myinspector;\n    }\n    function closeMyInspector(): void {\n      myinspector.dispose();\n      delete document.body.dataset[datasetKey];\n    }\n\n    // Add myinspector:open command to registry.\n    const showLabel = trans.__('Open My Contextual Help');\n    commands.addCommand(CommandIDs.open, {\n      caption,\n      isEnabled: () =>\n        !myinspector ||\n        myinspector.isDisposed ||\n        !myinspector.isAttached ||\n        !myinspector.isVisible,\n      label: showLabel,\n      icon: args => (args.isLauncher ? inspectorIcon : undefined),\n      execute: args => {\n        const text = args && (args.text as string);\n        const refresh = args && (args.refresh as boolean);\n        // if myinspector is open, see if we need a refresh\n        if (isMyInspectorOpen() && refresh)\n          myinspector.content.source?.onEditorChange(text);\n        else openMyInspector(text);\n      }\n    });\n\n    // Add myinspector:close command to registry.\n    const closeLabel = trans.__('Hide My Contextual Help');\n    commands.addCommand(CommandIDs.close, {\n      caption,\n      isEnabled: () => isMyInspectorOpen(),\n      label: closeLabel,\n      icon: args => (args.isLauncher ? inspectorIcon : undefined),\n      execute: () => closeMyInspector()\n    });\n\n    // Add myinspector:toggle command to registry.\n    const toggleLabel = trans.__('Show My Contextual Help');\n    commands.addCommand(CommandIDs.toggle, {\n      caption,\n      label: toggleLabel,\n      isToggled: () => isMyInspectorOpen(),\n      execute: args => {\n        if (isMyInspectorOpen()) {\n          closeMyInspector();\n        } else {\n          const text = args && (args.text as string);\n          openMyInspector(text);\n        }\n      }\n    });\n\n    // Add myinspector:trigger command to registry.\n    const triggerLabel = trans.__('Trigger My Contextual Help');\n    commands.addCommand(CommandIDs.trigger, {\n      caption,\n      isEnabled: () => isStandby(),\n      label: triggerLabel,\n      execute: () => {\n        if (myinspector && myinspector.content && myinspector.content.source && isStandby()) {\n          myinspector.content.source.standby = false;\n          myinspector.content.source?.onEditorChange();\n          myinspector.content.source.standby = true;\n        }\n      }\n    });\n\n    // Add myinspector:toggleStandby command to registry.\n    const toggleStandbyLabel = trans.__('Auto Update My Contextual Help');\n    commands.addCommand(CommandIDs.toggleStandby, {\n      caption,\n      isToggled: () => !isStandby(),\n      label: toggleStandbyLabel,\n      execute: () => {\n        if (myinspector && myinspector.content && myinspector.content.source) {\n          if (isStandby()) {\n            myinspector.content.source.standby = false;\n          } else {\n            myinspector.content.source.standby = true;\n          }\n        }\n      }\n    });\n\n    // Add open command to launcher if possible.\n    if (launcher) {\n      launcher.add({ command: CommandIDs.open, args: { isLauncher: true } });\n    }\n\n    // Add toggle command to command palette if possible.\n    if (palette) {\n      palette.addItem({ command: CommandIDs.toggle, category: toggleLabel });\n    }\n\n    // Handle state restoration.\n    if (restorer) {\n      void restorer.restore(tracker, {\n        command: CommandIDs.toggle,\n        name: () => 'myinspector'\n      });\n    }\n\n    // Create a proxy to pass the `source` to the current myinspector.\n    const proxy = Object.defineProperty({} as IMyInspector, 'source', {\n      get: (): IMyInspector.IInspectable | null =>\n        !myinspector || myinspector.isDisposed ? null : myinspector.content.source,\n      set: (src: IMyInspector.IInspectable | null) => {\n        source = src && !src.isDisposed ? src : null;\n        if (myinspector && !myinspector.isDisposed) {\n          myinspector.content.source = source;\n        }\n      }\n    });\n\n    return proxy;\n  }\n};\n\n/**\n * An extension that registers consoles for inspection.\n */\nconst consoles: JupyterFrontEndPlugin<void> = {\n  // FIXME This should be in @jupyterlab/console-extension\n  id: 'jupyterlab_pausable_contextual_help:consoles',\n  description: 'Adds my code introspection support to consoles.',\n  requires: [IMyInspector, IConsoleTracker, ILabShell],\n  autoStart: true,\n  activate: (\n    app: JupyterFrontEnd,\n    manager: IMyInspector,\n    consoles: IConsoleTracker,\n    labShell: ILabShell,\n    translator: ITranslator\n  ): void => {\n    // Maintain association of new consoles with their respective handlers.\n    const handlers: { [id: string]: InspectionHandler } = {};\n\n    // Create a handler for each console that is created.\n    consoles.widgetAdded.connect((sender, parent) => {\n      const sessionContext = parent.console.sessionContext;\n      const rendermime = parent.console.rendermime;\n      const connector = new KernelConnector({ sessionContext });\n      const handler = new InspectionHandler({ connector, rendermime });\n\n      // Associate the handler to the widget.\n      handlers[parent.id] = handler;\n\n      // Set the initial editor.\n      const cell = parent.console.promptCell;\n      handler.editor = cell && cell.editor;\n\n      // Listen for prompt creation.\n      parent.console.promptCellCreated.connect((sender, cell) => {\n        handler.editor = cell && cell.editor;\n      });\n\n      // Listen for parent disposal.\n      parent.disposed.connect(() => {\n        delete handlers[parent.id];\n        handler.dispose();\n      });\n    });\n\n    // Keep track of console instances and set myinspector source.\n    const setSource = (widget: Widget | null): void => {\n      if (widget && consoles.has(widget) && handlers[widget.id]) {\n        manager.source = handlers[widget.id];\n      }\n    };\n    labShell.currentChanged.connect((_, args) => setSource(args.newValue));\n    void app.restored.then(() => setSource(labShell.currentWidget));\n\n    app.contextMenu.addItem({\n      command: CommandIDs.toggle,\n      selector: '.jp-CodeConsole-promptCell'\n    });\n\n    app.contextMenu.addItem({\n      command: CommandIDs.toggleStandby,\n      selector: '.jp-CodeConsole-promptCell'\n    });\n\n  }\n};\n\n/**\n * An extension that registers notebooks for inspection.\n */\nconst notebooks: JupyterFrontEndPlugin<void> = {\n  // FIXME This should be in @jupyterlab/notebook-extension\n  id: 'jupyterlab_pausable_contextual_help:notebooks',\n  description: 'Adds code introspection to notebooks.',\n  requires: [IMyInspector, INotebookTracker, ILabShell],\n  autoStart: true,\n  activate: (\n    app: JupyterFrontEnd,\n    manager: IMyInspector,\n    notebooks: INotebookTracker,\n    labShell: ILabShell\n  ): void => {\n    // Maintain association of new notebooks with their respective handlers.\n    const handlers: { [id: string]: InspectionHandler } = {};\n\n    // Create a handler for each notebook that is created.\n    notebooks.widgetAdded.connect((sender, parent) => {\n      const sessionContext = parent.sessionContext;\n      const rendermime = parent.content.rendermime;\n      const connector = new KernelConnector({ sessionContext });\n      const handler = new InspectionHandler({ connector, rendermime });\n\n      // Associate the handler to the widget.\n      handlers[parent.id] = handler;\n\n      // Set the initial editor.\n      const cell = parent.content.activeCell;\n      handler.editor = cell && cell.editor;\n\n      // Listen for active cell changes.\n      parent.content.activeCellChanged.connect((sender, cell) => {\n        void cell?.ready.then(() => {\n          if (cell === parent.content.activeCell) {\n            handler.editor = cell!.editor;\n          }\n        });\n      });\n\n      // Listen for parent disposal.\n      parent.disposed.connect(() => {\n        delete handlers[parent.id];\n        handler.dispose();\n      });\n    });\n\n    // Keep track of notebook instances and set myinspector source.\n    const setSource = (widget: Widget | null): void => {\n      if (widget && notebooks.has(widget) && handlers[widget.id]) {\n        manager.source = handlers[widget.id];\n      }\n    };\n    labShell.currentChanged.connect((_, args) => setSource(args.newValue));\n    void app.restored.then(() => setSource(labShell.currentWidget));\n\n    app.contextMenu.addItem({\n      command: CommandIDs.toggle,\n      selector: '.jp-Notebook'\n    });\n\n    app.contextMenu.addItem({\n      command: CommandIDs.toggleStandby,\n      selector: '.jp-Notebook'\n    });\n\n  }\n};\n\n/**\n * Export the plugins as default.\n */\nconst plugins: JupyterFrontEndPlugin<any>[] = [myinspector, consoles, notebooks];\nexport default plugins;\n",
+        "// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\n\nimport { ISessionContext } from '@jupyterlab/apputils';\nimport { KernelMessage } from '@jupyterlab/services';\nimport { DataConnector } from '@jupyterlab/statedb';\nimport { InspectionHandler } from './handler';\n\n/**\n * The default connector for making inspection requests from the Jupyter API.\n */\nexport class KernelConnector extends DataConnector<\n  InspectionHandler.IReply,\n  void,\n  InspectionHandler.IRequest\n> {\n  /**\n   * Create a new kernel connector for inspection requests.\n   *\n   * @param options - The instantiation options for the kernel connector.\n   */\n  constructor(options: KernelConnector.IOptions) {\n    super();\n    this._sessionContext = options.sessionContext;\n  }\n\n  /**\n   * Fetch inspection requests.\n   *\n   * @param request - The inspection request text and details.\n   */\n  fetch(\n    request: InspectionHandler.IRequest\n  ): Promise<InspectionHandler.IReply> {\n    const kernel = this._sessionContext.session?.kernel;\n\n    if (!kernel) {\n      return Promise.reject(new Error('Inspection fetch requires a kernel.'));\n    }\n\n    const contents: KernelMessage.IInspectRequestMsg['content'] = {\n      code: request.text,\n      cursor_pos: request.offset,\n      detail_level: 1\n    };\n\n    return kernel.requestInspect(contents).then(msg => {\n      const response = msg.content;\n\n      if (response.status !== 'ok' || !response.found) {\n        throw new Error('Inspection fetch failed to return successfully.');\n      }\n\n      return { data: response.data, metadata: response.metadata };\n    });\n  }\n\n  private _sessionContext: ISessionContext;\n}\n\n/**\n * A namespace for kernel connector statics.\n */\nexport namespace KernelConnector {\n  /**\n   * The instantiation options for an inspection handler.\n   */\n  export interface IOptions {\n    /**\n     * The session context used to make API requests to the kernel.\n     */\n    sessionContext: ISessionContext;\n  }\n}\n",
+        "// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\n\nimport { Printing } from '@jupyterlab/apputils';\nimport {\n  ITranslator,\n  nullTranslator,\n  TranslationBundle\n} from '@jupyterlab/translation';\nimport { Panel, PanelLayout, Widget } from '@lumino/widgets';\nimport { IMyInspector } from './tokens';\n\n/**\n * The class name added to myinspector panels.\n */\nconst PANEL_CLASS = 'jp-MyInspector';\n\n/**\n * The class name added to myinspector content.\n */\nconst CONTENT_CLASS = 'jp-MyInspector-content';\n\n/**\n * The class name added to default myinspector content.\n */\nconst DEFAULT_CONTENT_CLASS = 'jp-MyInspector-default-content';\n\n/**\n * A panel which contains a set of myinspectors.\n */\nexport class MyInspectorPanel\n  extends Panel\n  implements IMyInspector, Printing.IPrintable\n{\n  /**\n   * Construct an myinspector.\n   */\n  constructor(options: MyInspectorPanel.IOptions = {}) {\n    super();\n    this.translator = options.translator || nullTranslator;\n    this._trans = this.translator.load('jupyterlab');\n\n    if (options.initialContent instanceof Widget) {\n      this._content = options.initialContent;\n    } else if (typeof options.initialContent === 'string') {\n      this._content = MyInspectorPanel._generateContentWidget(\n        `<p>${options.initialContent}</p>`\n      );\n    } else {\n      this._content = MyInspectorPanel._generateContentWidget(\n        '<p>' +\n                this._trans.__('Press F1 on a function to see documentation.') +\n          '</p>'\n      );\n    }\n\n    this.addClass(PANEL_CLASS);\n    (this.layout as PanelLayout).addWidget(this._content);\n  }\n\n  /**\n   * Print in iframe\n   */\n  [Printing.symbol]() {\n    return (): Promise<void> => Printing.printWidget(this);\n  }\n\n  /**\n   * The source of events the myinspector panel listens for.\n   */\n  get source(): IMyInspector.IInspectable | null {\n    return this._source;\n  }\n  set source(source: IMyInspector.IInspectable | null) {\n    if (this._source === source) {\n      return;\n    }\n\n    // Disconnect old signal handler.\n    if (this._source) {\n      this._source.standby = true;\n      this._source.inspected.disconnect(this.onMyInspectorUpdate, this);\n      this._source.disposed.disconnect(this.onSourceDisposed, this);\n    }\n\n    // Reject a source that is already disposed.\n    if (source && source.isDisposed) {\n      source = null;\n    }\n\n    // Update source.\n    this._source = source;\n\n    // Connect new signal handler.\n    if (this._source) {\n            //   this._source.standby = false;\n      this._source.inspected.connect(this.onMyInspectorUpdate, this);\n      this._source.disposed.connect(this.onSourceDisposed, this);\n    }\n  }\n\n  /**\n   * Dispose of the resources held by the widget.\n   */\n  dispose(): void {\n    if (this.isDisposed) {\n      return;\n    }\n    this.source = null;\n    super.dispose();\n  }\n\n  /**\n   * Handle myinspector update signals.\n   */\n  protected onMyInspectorUpdate(\n    sender: any,\n    args: IMyInspector.IMyInspectorUpdate\n  ): void {\n    const { content } = args;\n\n    // Update the content of the myinspector widget.\n    if (!content || content === this._content) {\n      return;\n    }\n    this._content.dispose();\n\n    this._content = content;\n    content.addClass(CONTENT_CLASS);\n    (this.layout as PanelLayout).addWidget(content);\n  }\n\n  /**\n   * Handle source disposed signals.\n   */\n  protected onSourceDisposed(sender: any, args: void): void {\n    this.source = null;\n  }\n\n  /**\n   * Generate content widget from string\n   */\n  private static _generateContentWidget(message: string): Widget {\n    const widget = new Widget();\n    widget.node.innerHTML = message;\n    widget.addClass(CONTENT_CLASS);\n    widget.addClass(DEFAULT_CONTENT_CLASS);\n\n    return widget;\n  }\n\n  protected translator: ITranslator;\n  private _trans: TranslationBundle;\n  private _content: Widget;\n  private _source: IMyInspector.IInspectable | null = null;\n}\n\nexport namespace MyInspectorPanel {\n  export interface IOptions {\n    initialContent?: Widget | string | undefined;\n\n    /**\n     * The application language translator.\n     */\n    translator?: ITranslator;\n  }\n}\n",
+        "// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\n\nimport { Token } from '@lumino/coreutils';\nimport { ISignal } from '@lumino/signaling';\nimport { Widget } from '@lumino/widgets';\n\n/**\n * The myinspector panel token.\n */\nexport const IMyInspector = new Token<IMyInspector>(\n  '@jupyterlab/inspector:IMyInspector',\n  `A service for adding contextual help to widgets (visible using \"Show Contextual Help\" from the Help menu).\n  Use this to hook into the contextual help system in your extension.`\n);\n\n/**\n * An interface for an myinspector.\n */\nexport interface IMyInspector {\n  /**\n   * The source of events the myinspector listens for.\n   */\n  source: IMyInspector.IInspectable | null;\n}\n\n/**\n * A namespace for myinspector interfaces.\n */\nexport namespace IMyInspector {\n  /**\n   * The definition of an inspectable source.\n   */\n  export interface IInspectable {\n    /**\n     * A signal emitted when the myinspector should clear all items.\n     */\n    cleared: ISignal<any, void>;\n\n    /**\n     * A signal emitted when the inspectable is disposed.\n     */\n    disposed: ISignal<any, void>;\n\n    /**\n     * A signal emitted when an myinspector value is generated.\n     */\n    inspected: ISignal<any, IMyInspectorUpdate>;\n\n    /**\n     * Test whether the inspectable has been disposed.\n     */\n    isDisposed: boolean;\n\n    /**\n     * Indicates whether the inspectable source emits signals.\n     *\n     * #### Notes\n     * The use case for this attribute is to limit the API traffic when no\n     * myinspector is visible. It can be modified by the consumer of the source.\n     */\n    standby: boolean;\n    /**\n     * Handle a text changed signal from an editor.\n     *\n     * #### Notes\n     * Update the hints myinspector based on a text change.\n     */\n    onEditorChange(customText?: string): void;\n  }\n\n  /**\n   * An update value for code myinspectors.\n   */\n  export interface IMyInspectorUpdate {\n    /**\n     * The content being sent to the myinspector for display.\n     */\n    content: Widget | null;\n  }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/package.json` & `jupyterlab_pausable_contextual_help-0.1.3/package.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7111320141211446%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.2.0', '@jupyterlab/console': '^4.2.0', "*

 * *                   "'@jupyterlab/inspector': '^4.2.0', '@jupyterlab/launcher': '^4.2.0', "*

 * *                   "'@jupyterlab/notebook': '^4.2.0', '@jupyterlab/settingregistry': '^4.0.0', "*

 * *                   "delete: ['@jupyterlab/apputils', '@jupyterlab/translation', "*

 * *                   "'@jupyterlab/ui-components']}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@typescript-eslint/eslint-plugin': "*

 * *   […]*

```diff
@@ -3,111 +3,192 @@
         "email": "feiranzhang@outlook.com",
         "name": "Feiran Zhang"
     },
     "bugs": {
         "url": "https://github.com/zhangfeiran/jupyterlab_pausable_contextual_help/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.18",
-        "@jupyterlab/apputils": "^3.0.18",
-        "@jupyterlab/console": "^3.0.18",
-        "@jupyterlab/inspector": "^3.0.18",
-        "@jupyterlab/launcher": "^3.0.18",
-        "@jupyterlab/notebook": "^3.0.18",
-        "@jupyterlab/translation": "^3.0.18",
-        "@jupyterlab/ui-components": "^3.0.18"
+        "@jupyterlab/application": "^4.2.0",
+        "@jupyterlab/console": "^4.2.0",
+        "@jupyterlab/inspector": "^4.2.0",
+        "@jupyterlab/launcher": "^4.2.0",
+        "@jupyterlab/notebook": "^4.2.0",
+        "@jupyterlab/settingregistry": "^4.0.0"
     },
     "description": "Customized Jupyterlab Contextual Help Panel That Allows Manually Update When Press F1.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.18",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@types/react-addons-linked-state-mixin": "^0.14.22",
+        "@typescript-eslint/eslint-plugin": "^6.1.0",
+        "@typescript-eslint/parser": "^6.1.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^5.0.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
-        "stylelint-config-prettier": "^9.0.3",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
-        "stylelint-prettier": "^2.0.0",
-        "typescript": "~4.1.3"
-    },
-    "directories": {
-        "lib": "lib/"
+        "prettier": "^3.0.0",
+        "rimraf": "^5.0.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^15.10.1",
+        "stylelint-config-recommended": "^13.0.0",
+        "stylelint-config-standard": "^34.0.0",
+        "stylelint-csstree-validator": "^3.0.0",
+        "stylelint-prettier": "^4.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.0"
+    },
+    "eslintConfig": {
+        "extends": [
+            "eslint:recommended",
+            "plugin:@typescript-eslint/eslint-recommended",
+            "plugin:@typescript-eslint/recommended",
+            "plugin:prettier/recommended"
+        ],
+        "parser": "@typescript-eslint/parser",
+        "parserOptions": {
+            "project": "tsconfig.json",
+            "sourceType": "module"
+        },
+        "plugins": [
+            "@typescript-eslint"
+        ],
+        "rules": {
+            "@typescript-eslint/naming-convention": [
+                "error",
+                {
+                    "custom": {
+                        "match": true,
+                        "regex": "^I[A-Z]"
+                    },
+                    "format": [
+                        "PascalCase"
+                    ],
+                    "selector": "interface"
+                }
+            ],
+            "@typescript-eslint/no-explicit-any": "off",
+            "@typescript-eslint/no-namespace": "off",
+            "@typescript-eslint/no-unused-vars": [
+                "warn",
+                {
+                    "args": "none"
+                }
+            ],
+            "@typescript-eslint/no-use-before-define": "off",
+            "@typescript-eslint/quotes": [
+                "error",
+                "single",
+                {
+                    "allowTemplateLiterals": false,
+                    "avoidEscape": true
+                }
+            ],
+            "curly": [
+                "error",
+                "all"
+            ],
+            "eqeqeq": "error",
+            "prefer-arrow-callback": "error"
+        }
     },
+    "eslintIgnore": [
+        "node_modules",
+        "dist",
+        "coverage",
+        "**/*.d.ts"
+    ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "src/**/*.{ts,tsx}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/zhangfeiran/jupyterlab_pausable_contextual_help",
-    "jupyter-releaser": {
-        "hooks": {
-            "before-build-npm": [
-                "python -m pip install jupyterlab~=3.1",
-                "jlpm"
-            ],
-            "before-build-python": [
-                "jlpm clean:all"
-            ]
-        }
-    },
     "jupyterlab": {
-        "disabledExtensions": [
-            "@jupyterlab/inspector-extension"
-        ],
         "extension": true,
         "outputDir": "jupyterlab_pausable_contextual_help/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "jupyterlab_pausable_contextual_help",
+    "prettier": {
+        "arrowParens": "avoid",
+        "endOfLine": "auto",
+        "overrides": [
+            {
+                "files": "package.json",
+                "options": {
+                    "tabWidth": 4
+                }
+            }
+        ],
+        "singleQuote": true,
+        "trailingComma": "none"
+    },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/zhangfeiran/jupyterlab_pausable_contextual_help.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
-        "clean:labextension": "rimraf jupyterlab_pausable_contextual_help/labextension",
+        "clean:labextension": "rimraf jupyterlab_pausable_contextual_help/labextension jupyterlab_pausable_contextual_help/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
+    "stylelint": {
+        "extends": [
+            "stylelint-config-recommended",
+            "stylelint-config-standard",
+            "stylelint-prettier/recommended"
+        ],
+        "plugins": [
+            "stylelint-csstree-validator"
+        ],
+        "rules": {
+            "csstree/validator": true,
+            "property-no-vendor-prefix": null,
+            "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
+            "selector-no-vendor-prefix": null,
+            "value-no-vendor-prefix": null
+        }
+    },
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/src/handler.ts` & `jupyterlab_pausable_contextual_help-0.1.3/src/handler.ts`

 * *Files 9% similar despite different names*

```diff
@@ -5,245 +5,246 @@
 import { Text } from '@jupyterlab/coreutils';
 import { IRenderMimeRegistry, MimeModel } from '@jupyterlab/rendermime';
 import { IDataConnector } from '@jupyterlab/statedb';
 import { JSONExt, ReadonlyJSONObject } from '@lumino/coreutils';
 import { IDisposable } from '@lumino/disposable';
 import { Debouncer } from '@lumino/polling';
 import { ISignal, Signal } from '@lumino/signaling';
-import { IInspector } from './tokens';
+import { IMyInspector } from './tokens';
 
 /**
  * An object that handles code inspection.
  */
-export class InspectionHandler implements IDisposable, IInspector.IInspectable {
-    /**
-     * Construct a new inspection handler for a widget.
-     */
-    constructor(options: InspectionHandler.IOptions) {
-        this._connector = options.connector;
-        this._rendermime = options.rendermime;
-        this._debouncer = new Debouncer(this.onEditorChange.bind(this), 250);
-    }
-
-    /**
-     * A signal emitted when the inspector should clear all items.
-     */
-    get cleared(): ISignal<InspectionHandler, void> {
-        return this._cleared;
-    }
+export class InspectionHandler implements IDisposable, IMyInspector.IInspectable {
+  /**
+   * Construct a new inspection handler for a widget.
+   */
+  constructor(options: InspectionHandler.IOptions) {
+    this._connector = options.connector;
+    this._rendermime = options.rendermime;
+    this._debouncer = new Debouncer(this.onEditorChange.bind(this), 250);
+  }
+
+  /**
+   * A signal emitted when the myinspector should clear all items.
+   */
+  get cleared(): ISignal<InspectionHandler, void> {
+    return this._cleared;
+  }
+
+  /**
+   * A signal emitted when the handler is disposed.
+   */
+  get disposed(): ISignal<InspectionHandler, void> {
+    return this._disposed;
+  }
+
+  /**
+   * A signal emitted when an myinspector value is generated.
+   */
+  get inspected(): ISignal<InspectionHandler, IMyInspector.IMyInspectorUpdate> {
+    return this._inspected;
+  }
+
+  /**
+   * The editor widget used by the inspection handler.
+   */
+  get editor(): CodeEditor.IEditor | null {
+    return this._editor;
+  }
+  set editor(newValue: CodeEditor.IEditor | null) {
+    if (newValue === this._editor) {
+      return;
+    }
+    // Remove all of our listeners.
+    Signal.disconnectReceiver(this);
+
+    const editor = (this._editor = newValue);
+    if (editor) {
+      // Clear the myinspector in preparation for a new editor.
+      this._cleared.emit(void 0);
+      // Call onEditorChange to cover the case where the user changes
+      // the active cell
+      this.onEditorChange();
+      editor.model.selections.changed.connect(this._onChange, this);
+      editor.model.sharedModel.changed.connect(this._onChange, this);
+    }
+  }
+
+  /**
+   * Indicates whether the handler makes API inspection requests or stands by.
+   *
+   * #### Notes
+   * The use case for this attribute is to limit the API traffic when no
+   * myinspector is visible.
+   */
+  get standby(): boolean {
+    return this._standby;
+  }
+  set standby(value: boolean) {
+    this._standby = value;
+  }
+
+  /**
+   * Get whether the inspection handler is disposed.
+   *
+   * #### Notes
+   * This is a read-only property.
+   */
+  get isDisposed(): boolean {
+    return this._isDisposed;
+  }
+
+  /**
+   * Dispose of the resources used by the handler.
+   */
+  dispose(): void {
+    if (this.isDisposed) {
+      return;
+    }
+    this._isDisposed = true;
+    this._debouncer.dispose();
+    this._disposed.emit(void 0);
+    Signal.clearData(this);
+  }
+
+  /**
+   * Handle a text changed signal from an editor.
+   *
+   * #### Notes
+   * Update the hints myinspector based on a text change.
+   */
+  onEditorChange(customText?: string): void {
+    // If the handler is in standby mode, bail.
+    if (this._standby) {
+      return;
+    }
+
+    const editor = this.editor;
+
+    if (!editor) {
+      return;
+    }
+    const text = customText ? customText : editor.model.sharedModel.getSource();
+    const position = editor.getCursorPosition();
+    const offset = Text.jsIndexToCharIndex(editor.getOffsetAt(position), text);
+    const update: IMyInspector.IMyInspectorUpdate = { content: null };
+
+    const pending = ++this._pending;
+
+    void this._connector
+      .fetch({ offset, text })
+      .then(reply => {
+        // If handler has been disposed or a newer request is pending, bail.
+        if (!reply || this.isDisposed || pending !== this._pending) {
+          this._lastInspectedReply = null;
+          this._inspected.emit(update);
+          return;
+        }
 
-    /**
-     * A signal emitted when the handler is disposed.
-     */
-    get disposed(): ISignal<InspectionHandler, void> {
-        return this._disposed;
-    }
+        const { data } = reply;
 
-    /**
-     * A signal emitted when an inspector value is generated.
-     */
-    get inspected(): ISignal<InspectionHandler, IInspector.IInspectorUpdate> {
-        return this._inspected;
-    }
-
-    /**
-     * The editor widget used by the inspection handler.
-     */
-    get editor(): CodeEditor.IEditor | null {
-        return this._editor;
-    }
-    set editor(newValue: CodeEditor.IEditor | null) {
-        if (newValue === this._editor) {
-            return;
+        // Do not update if there would be no change.
+        if (
+          this._lastInspectedReply &&
+          JSONExt.deepEqual(this._lastInspectedReply, data)
+        ) {
+          return;
         }
-        // Remove all of our listeners.
-        Signal.disconnectReceiver(this);
 
-        const editor = (this._editor = newValue);
-        if (editor) {
-            // Clear the inspector in preparation for a new editor.
-            this._cleared.emit(void 0);
-            // Call onEditorChange to cover the case where the user changes
-            // the active cell
-            this.onEditorChange();
-            editor.model.selections.changed.connect(this._onChange, this);
-            editor.model.value.changed.connect(this._onChange, this);
+        const mimeType = this._rendermime.preferredMimeType(data);
+        if (mimeType) {
+          const widget = this._rendermime.createRenderer(mimeType);
+          const model = new MimeModel({ data });
+
+          void widget.renderModel(model);
+          update.content = widget;
         }
-    }
 
-    /**
-     * Indicates whether the handler makes API inspection requests or stands by.
-     *
-     * #### Notes
-     * The use case for this attribute is to limit the API traffic when no
-     * inspector is visible.
-     */
-    get standby(): boolean {
-        return this._standby;
-    }
-    set standby(value: boolean) {
-        this._standby = value;
-    }
+        this._lastInspectedReply = reply.data;
+        this._inspected.emit(update);
+      })
+      .catch(reason => {
+        // Since almost all failures are benign, fail silently.
+        this._lastInspectedReply = null;
+        this._inspected.emit(update);
+      });
+  }
+
+  /**
+   * Handle changes to the editor state, debouncing.
+   */
+  private _onChange(): void {
+    void this._debouncer.invoke();
+  }
+
+  private _cleared = new Signal<InspectionHandler, void>(this);
+  private _connector: IDataConnector<
+    InspectionHandler.IReply,
+    void,
+    InspectionHandler.IRequest
+  >;
+  private _disposed = new Signal<this, void>(this);
+  private _editor: CodeEditor.IEditor | null = null;
+  private _inspected = new Signal<this, IMyInspector.IMyInspectorUpdate>(this);
+  private _isDisposed = false;
+  private _pending = 0;
+  private _rendermime: IRenderMimeRegistry;
+  private _standby = true;
+  private _debouncer: Debouncer;
+  private _lastInspectedReply: InspectionHandler.IReply['data'] | null = null;
+}
 
+/**
+ * A namespace for inspection handler statics.
+ */
+export namespace InspectionHandler {
+  /**
+   * The instantiation options for an inspection handler.
+   */
+  export interface IOptions {
     /**
-     * Get whether the inspection handler is disposed.
+     * The connector used to make inspection requests.
      *
      * #### Notes
-     * This is a read-only property.
+     * The only method of this connector that will ever be called is `fetch`, so
+     * it is acceptable for the other methods to be simple functions that return
+     * rejected promises.
      */
-    get isDisposed(): boolean {
-        return this._isDisposed;
-    }
+    connector: IDataConnector<IReply, void, IRequest>;
 
     /**
-     * Dispose of the resources used by the handler.
+     * The mime renderer for the inspection handler.
      */
-    dispose(): void {
-        if (this.isDisposed) {
-            return;
-        }
-        this._isDisposed = true;
-        this._disposed.emit(void 0);
-        Signal.clearData(this);
-    }
+    rendermime: IRenderMimeRegistry;
+  }
 
+  /**
+   * A reply to an inspection request.
+   */
+  export interface IReply {
     /**
-     * Handle a text changed signal from an editor.
-     *
-     * #### Notes
-     * Update the hints inspector based on a text change.
+     * The MIME bundle data returned from an inspection request.
      */
-    onEditorChange(customText?: string): void {
-        // If the handler is in standby mode, bail.
-        if (this._standby) {
-            return;
-        }
-
-        const editor = this.editor;
-
-        if (!editor) {
-            return;
-        }
-        const text = customText ? customText : editor.model.value.text;
-        const position = editor.getCursorPosition();
-        const offset = Text.jsIndexToCharIndex(editor.getOffsetAt(position), text);
-        const update: IInspector.IInspectorUpdate = { content: null };
-
-        const pending = ++this._pending;
-
-        void this._connector
-            .fetch({ offset, text })
-            .then(reply => {
-                // If handler has been disposed or a newer request is pending, bail.
-                if (!reply || this.isDisposed || pending !== this._pending) {
-                    this._lastInspectedReply = null;
-                    this._inspected.emit(update);
-                    return;
-                }
-
-                const { data } = reply;
-
-                // Do not update if there would be no change.
-                if (
-                    this._lastInspectedReply &&
-                    JSONExt.deepEqual(this._lastInspectedReply, data)
-                ) {
-                    return;
-                }
-
-                const mimeType = this._rendermime.preferredMimeType(data);
-                if (mimeType) {
-                    const widget = this._rendermime.createRenderer(mimeType);
-                    const model = new MimeModel({ data });
-
-                    void widget.renderModel(model);
-                    update.content = widget;
-                }
-
-                this._lastInspectedReply = reply.data;
-                this._inspected.emit(update);
-            })
-            .catch(reason => {
-                // Since almost all failures are benign, fail silently.
-                this._lastInspectedReply = null;
-                this._inspected.emit(update);
-            });
-    }
+    data: ReadonlyJSONObject;
 
     /**
-     * Handle changes to the editor state, debouncing.
+     * Any metadata that accompanies the MIME bundle returning from a request.
      */
-    private _onChange(): void {
-        void this._debouncer.invoke();
-    }
-
-    private _cleared = new Signal<InspectionHandler, void>(this);
-    private _connector: IDataConnector<
-        InspectionHandler.IReply,
-        void,
-        InspectionHandler.IRequest
-    >;
-    private _disposed = new Signal<this, void>(this);
-    private _editor: CodeEditor.IEditor | null = null;
-    private _inspected = new Signal<this, IInspector.IInspectorUpdate>(this);
-    private _isDisposed = false;
-    private _pending = 0;
-    private _rendermime: IRenderMimeRegistry;
-    private _standby = true;
-    private _debouncer: Debouncer;
-    private _lastInspectedReply: InspectionHandler.IReply['data'] | null = null;
-}
+    metadata: ReadonlyJSONObject;
+  }
 
-/**
- * A namespace for inspection handler statics.
- */
-export namespace InspectionHandler {
+  /**
+   * The details of an inspection request.
+   */
+  export interface IRequest {
     /**
-     * The instantiation options for an inspection handler.
+     * The cursor offset position within the text being inspected.
      */
-    export interface IOptions {
-        /**
-         * The connector used to make inspection requests.
-         *
-         * #### Notes
-         * The only method of this connector that will ever be called is `fetch`, so
-         * it is acceptable for the other methods to be simple functions that return
-         * rejected promises.
-         */
-        connector: IDataConnector<IReply, void, IRequest>;
-
-        /**
-         * The mime renderer for the inspection handler.
-         */
-        rendermime: IRenderMimeRegistry;
-    }
-
-    /**
-     * A reply to an inspection request.
-     */
-    export interface IReply {
-        /**
-         * The MIME bundle data returned from an inspection request.
-         */
-        data: ReadonlyJSONObject;
-
-        /**
-         * Any metadata that accompanies the MIME bundle returning from a request.
-         */
-        metadata: ReadonlyJSONObject;
-    }
+    offset: number;
 
     /**
-     * The details of an inspection request.
+     * The text being inspected.
      */
-    export interface IRequest {
-        /**
-         * The cursor offset position within the text being inspected.
-         */
-        offset: number;
-
-        /**
-         * The text being inspected.
-         */
-        text: string;
-    }
+    text: string;
+  }
 }
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/src/index.ts` & `jupyterlab_pausable_contextual_help-0.1.3/src/index.ts`

 * *Files 17% similar despite different names*

```diff
@@ -1,365 +1,382 @@
 // Copyright (c) Jupyter Development Team.
 // Distributed under the terms of the Modified BSD License.
 
+// export * from './handler';
+// export * from './myinspector';
+// export * from './kernelconnector';
+// export * from './tokens';
+
+// Copyright (c) Jupyter Development Team.
+// Distributed under the terms of the Modified BSD License.
 
 import {
-    ILabShell,
-    ILayoutRestorer,
-    JupyterFrontEnd,
-    JupyterFrontEndPlugin
+  ILabShell,
+  ILayoutRestorer,
+  JupyterFrontEnd,
+  JupyterFrontEndPlugin
 } from '@jupyterlab/application';
+
+// import { ISettingRegistry } from '@jupyterlab/settingregistry';
+
 import {
-    ICommandPalette,
-    MainAreaWidget,
-    WidgetTracker
+  ICommandPalette,
+  MainAreaWidget,
+  WidgetTracker
 } from '@jupyterlab/apputils';
 import { IConsoleTracker } from '@jupyterlab/console';
-// import {
-//   IInspector,
-//   InspectionHandler,
-//   InspectorPanel,
-//   KernelConnector
-// } from '@jupyterlab/inspector';
-import { IInspector } from './tokens';
+//   import {
+//     IMyInspector,
+//     InspectionHandler,
+//     MyInspectorPanel,
+//     KernelConnector
+//   } from '@jupyterlab/inspector';
+import { IMyInspector } from './tokens';
 import { InspectionHandler } from './handler';
-import { InspectorPanel } from './inspector';
+import { MyInspectorPanel } from './myinspector';
 import { KernelConnector } from './kernelconnector';
 
 
 import { ILauncher } from '@jupyterlab/launcher';
 import { INotebookTracker } from '@jupyterlab/notebook';
 import { ITranslator } from '@jupyterlab/translation';
 import { inspectorIcon } from '@jupyterlab/ui-components';
+import { Widget } from '@lumino/widgets';
 
 /**
- * The command IDs used by the inspector plugin.
+ * The command IDs used by the myinspector plugin.
  */
 namespace CommandIDs {
-    export const open = 'myinspector:open';
-    export const close = 'myinspector:close';
-    export const toggle = 'myinspector:toggle';
-    export const trigger = 'myinspector:trigger';
-    export const toggleStandby = 'myinspector:toggleStandby';
+  export const open = 'myinspector:open';
+  export const close = 'myinspector:close';
+  export const toggle = 'myinspector:toggle';
+  export const trigger = 'myinspector:trigger';
+  export const toggleStandby = 'myinspector:toggleStandby';
 }
 
 /**
  * A service providing code introspection.
  */
-const inspector: JupyterFrontEndPlugin<IInspector> = {
-    id: 'jupyterlab_pausable_contextual_help:inspector',
-    requires: [ITranslator],
-    optional: [ICommandPalette, ILauncher, ILayoutRestorer],
-    provides: IInspector,
-    autoStart: true,
-    activate: (
-        app: JupyterFrontEnd,
-        translator: ITranslator,
-        palette: ICommandPalette | null,
-        launcher: ILauncher | null,
-        restorer: ILayoutRestorer | null
-    ): IInspector => {
-        const trans = translator.load('jupyterlab');
-        const { commands, shell } = app;
-        const caption = trans.__(
+const myinspector: JupyterFrontEndPlugin<IMyInspector> = {
+  id: 'jupyterlab_pausable_contextual_help:myinspector',
+  description: 'Provides the pausable code introspection widget.',
+  requires: [ITranslator],
+  optional: [ICommandPalette, ILauncher, ILayoutRestorer],
+  provides: IMyInspector,
+  autoStart: true,
+  activate: (
+    app: JupyterFrontEnd,
+    translator: ITranslator,
+    palette: ICommandPalette | null,
+    launcher: ILauncher | null,
+    restorer: ILayoutRestorer | null
+  ): IMyInspector => {
+    const trans = translator.load('jupyterlab');
+    const { commands, shell } = app;
+    const caption = trans.__(
             'Manually updating code documentation from the active kernel'
-        );
-        const openedLabel = trans.__('My Contextual Help');
-        const namespace = 'inspector';
-        const datasetKey = 'jpInspector';
-        const tracker = new WidgetTracker<MainAreaWidget<InspectorPanel>>({
-            namespace
-        });
+    );
+    const openedLabel = trans.__('My Contextual Help');
+    const namespace = 'myinspector';
+    const datasetKey = 'jpMyInspector';
+    const tracker = new WidgetTracker<MainAreaWidget<MyInspectorPanel>>({
+      namespace
+    });
 
-        function isInspectorOpen() {
-            return inspector && !inspector.isDisposed;
-        }
-
-        function isStandby() {
-            // return inspector && inspector.content && inspector.content.source && inspector.content.source.standby;
-            if (inspector && inspector.content && inspector.content.source) {
-                return inspector.content.source.standby;
-            }
-            return false;
-        }
-
-        let source: IInspector.IInspectable | null = null;
-        let inspector: MainAreaWidget<InspectorPanel>;
-        function openInspector(args: string): MainAreaWidget<InspectorPanel> {
-            if (!isInspectorOpen()) {
-                inspector = new MainAreaWidget({
-                    content: new InspectorPanel({ translator })
-                });
-                inspector.id = 'jp-inspector';
-                inspector.title.label = openedLabel;
-                inspector.title.icon = inspectorIcon;
-                void tracker.add(inspector);
-                source = source && !source.isDisposed ? source : null;
-                inspector.content.source = source;
-                inspector.content.source?.onEditorChange(args);
-            }
-            if (!inspector.isAttached) {
-                shell.add(inspector, 'main', {
-                    activate: false,
-                    mode: 'split-right'
-                });
-            }
-            shell.activateById(inspector.id);
-            document.body.dataset[datasetKey] = 'open';
-            return inspector;
-        }
-        function closeInspector(): void {
-            inspector.dispose();
-            delete document.body.dataset[datasetKey];
-        }
-
-        // Add inspector:open command to registry.
-        const showLabel = trans.__('Open My Contextual Help');
-        commands.addCommand(CommandIDs.open, {
-            caption,
-            isEnabled: () =>
-                !inspector ||
-                inspector.isDisposed ||
-                !inspector.isAttached ||
-                !inspector.isVisible,
-            label: showLabel,
-            icon: args => (args.isLauncher ? inspectorIcon : undefined),
-            execute: args => {
-                const text = args && (args.text as string);
-                const refresh = args && (args.refresh as boolean);
-                // if inspector is open, see if we need a refresh
-                if (isInspectorOpen() && refresh)
-                    inspector.content.source?.onEditorChange(text);
-                else openInspector(text);
-            }
-        });
-        // Add inspector:close command to registry.
-        const closeLabel = trans.__('Hide My Contextual Help');
-        commands.addCommand(CommandIDs.close, {
-            caption,
-            isEnabled: () => isInspectorOpen(),
-            label: closeLabel,
-            icon: args => (args.isLauncher ? inspectorIcon : undefined),
-            execute: () => closeInspector()
-        });
-
-        // Add inspector:toggle command to registry.
-        const toggleLabel = trans.__('Show My Contextual Help');
-        commands.addCommand(CommandIDs.toggle, {
-            caption,
-            label: toggleLabel,
-            isToggled: () => isInspectorOpen(),
-            execute: args => {
-                if (isInspectorOpen()) {
-                    closeInspector();
-                } else {
-                    const text = args && (args.text as string);
-                    openInspector(text);
-                }
-            }
-        });
+    function isMyInspectorOpen() {
+      return myinspector && !myinspector.isDisposed;
+    }
 
-        // Add inspector:trigger command to registry.
-        const triggerLabel = trans.__('Trigger My Contextual Help');
-        commands.addCommand(CommandIDs.trigger, {
-            caption,
-            isEnabled: () => isStandby(),
-            label: triggerLabel,
-            execute: () => {
-                if (inspector && inspector.content && inspector.content.source && isStandby()) {
-                    inspector.content.source.standby = false;
-                    inspector.content.source?.onEditorChange();
-                    inspector.content.source.standby = true;
-                }
-            }
-        });
+    function isStandby() {
+      // return myinspector && myinspector.content && myinspector.content.source && myinspector.content.source.standby;
+      if (myinspector && myinspector.content && myinspector.content.source) {
+        return myinspector.content.source.standby;
+      }
+      return false;
+    }
 
-        // Add inspector:toggleStandby command to registry.
-        const toggleStandbyLabel = trans.__('Auto Update My Contextual Help');
-        commands.addCommand(CommandIDs.toggleStandby, {
-            caption,
-            isToggled: () => !isStandby(),
-            label: toggleStandbyLabel,
-            execute: () => {
-                if (inspector && inspector.content && inspector.content.source) {
-                    if (isStandby()) {
-                        inspector.content.source.standby = false;
-                    } else {
-                        inspector.content.source.standby = true;
-                    }
-                }
-            }
-        });
+    let source: IMyInspector.IInspectable | null = null;
+    let myinspector: MainAreaWidget<MyInspectorPanel>;
+    function openMyInspector(args: string): MainAreaWidget<MyInspectorPanel> {
+      if (!isMyInspectorOpen()) {
+        myinspector = new MainAreaWidget({
+          content: new MyInspectorPanel({ translator })
+        });
+        myinspector.id = 'jp-myinspector';
+        myinspector.title.label = openedLabel;
+        myinspector.title.icon = inspectorIcon;
+        void tracker.add(myinspector);
+        source = source && !source.isDisposed ? source : null;
+        myinspector.content.source = source;
+        myinspector.content.source?.onEditorChange(args);
+      }
+      if (!myinspector.isAttached) {
+        shell.add(myinspector, 'main', {
+          activate: false,
+          mode: 'split-right',
+          type: 'MyInspector'
+        });
+      }
+      shell.activateById(myinspector.id);
+      document.body.dataset[datasetKey] = 'open';
+      return myinspector;
+    }
+    function closeMyInspector(): void {
+      myinspector.dispose();
+      delete document.body.dataset[datasetKey];
+    }
 
-        // Add open command to launcher if possible.
-        if (launcher) {
-            launcher.add({ command: CommandIDs.open, args: { isLauncher: true } });
+    // Add myinspector:open command to registry.
+    const showLabel = trans.__('Open My Contextual Help');
+    commands.addCommand(CommandIDs.open, {
+      caption,
+      isEnabled: () =>
+        !myinspector ||
+        myinspector.isDisposed ||
+        !myinspector.isAttached ||
+        !myinspector.isVisible,
+      label: showLabel,
+      icon: args => (args.isLauncher ? inspectorIcon : undefined),
+      execute: args => {
+        const text = args && (args.text as string);
+        const refresh = args && (args.refresh as boolean);
+        // if myinspector is open, see if we need a refresh
+        if (isMyInspectorOpen() && refresh)
+          myinspector.content.source?.onEditorChange(text);
+        else openMyInspector(text);
+      }
+    });
+
+    // Add myinspector:close command to registry.
+    const closeLabel = trans.__('Hide My Contextual Help');
+    commands.addCommand(CommandIDs.close, {
+      caption,
+      isEnabled: () => isMyInspectorOpen(),
+      label: closeLabel,
+      icon: args => (args.isLauncher ? inspectorIcon : undefined),
+      execute: () => closeMyInspector()
+    });
+
+    // Add myinspector:toggle command to registry.
+    const toggleLabel = trans.__('Show My Contextual Help');
+    commands.addCommand(CommandIDs.toggle, {
+      caption,
+      label: toggleLabel,
+      isToggled: () => isMyInspectorOpen(),
+      execute: args => {
+        if (isMyInspectorOpen()) {
+          closeMyInspector();
+        } else {
+          const text = args && (args.text as string);
+          openMyInspector(text);
         }
+      }
+    });
 
-        // Add toggle command to command palette if possible.
-        if (palette) {
-            palette.addItem({ command: CommandIDs.toggle, category: toggleLabel });
+    // Add myinspector:trigger command to registry.
+    const triggerLabel = trans.__('Trigger My Contextual Help');
+    commands.addCommand(CommandIDs.trigger, {
+      caption,
+      isEnabled: () => isStandby(),
+      label: triggerLabel,
+      execute: () => {
+        if (myinspector && myinspector.content && myinspector.content.source && isStandby()) {
+          myinspector.content.source.standby = false;
+          myinspector.content.source?.onEditorChange();
+          myinspector.content.source.standby = true;
         }
+      }
+    });
 
-        // Handle state restoration.
-        if (restorer) {
-            void restorer.restore(tracker, {
-                command: CommandIDs.toggle,
-                name: () => 'inspector'
-            });
+    // Add myinspector:toggleStandby command to registry.
+    const toggleStandbyLabel = trans.__('Auto Update My Contextual Help');
+    commands.addCommand(CommandIDs.toggleStandby, {
+      caption,
+      isToggled: () => !isStandby(),
+      label: toggleStandbyLabel,
+      execute: () => {
+        if (myinspector && myinspector.content && myinspector.content.source) {
+          if (isStandby()) {
+            myinspector.content.source.standby = false;
+          } else {
+            myinspector.content.source.standby = true;
+          }
         }
+      }
+    });
 
-        // Create a proxy to pass the `source` to the current inspector.
-        const proxy = Object.defineProperty({} as IInspector, 'source', {
-            get: (): IInspector.IInspectable | null =>
-                !inspector || inspector.isDisposed ? null : inspector.content.source,
-            set: (src: IInspector.IInspectable | null) => {
-                source = src && !src.isDisposed ? src : null;
-                if (inspector && !inspector.isDisposed) {
-                    inspector.content.source = source;
-                }
-            }
-        });
+    // Add open command to launcher if possible.
+    if (launcher) {
+      launcher.add({ command: CommandIDs.open, args: { isLauncher: true } });
+    }
+
+    // Add toggle command to command palette if possible.
+    if (palette) {
+      palette.addItem({ command: CommandIDs.toggle, category: toggleLabel });
+    }
 
-        return proxy;
+    // Handle state restoration.
+    if (restorer) {
+      void restorer.restore(tracker, {
+        command: CommandIDs.toggle,
+        name: () => 'myinspector'
+      });
     }
+
+    // Create a proxy to pass the `source` to the current myinspector.
+    const proxy = Object.defineProperty({} as IMyInspector, 'source', {
+      get: (): IMyInspector.IInspectable | null =>
+        !myinspector || myinspector.isDisposed ? null : myinspector.content.source,
+      set: (src: IMyInspector.IInspectable | null) => {
+        source = src && !src.isDisposed ? src : null;
+        if (myinspector && !myinspector.isDisposed) {
+          myinspector.content.source = source;
+        }
+      }
+    });
+
+    return proxy;
+  }
 };
 
 /**
  * An extension that registers consoles for inspection.
  */
 const consoles: JupyterFrontEndPlugin<void> = {
-    id: 'jupyterlab_pausable_contextual_help:consoles',
-    requires: [IInspector, IConsoleTracker, ILabShell],
-    autoStart: true,
-    activate: (
-        app: JupyterFrontEnd,
-        manager: IInspector,
-        consoles: IConsoleTracker,
-        labShell: ILabShell,
-        translator: ITranslator
-    ): void => {
-        // Maintain association of new consoles with their respective handlers.
-        const handlers: { [id: string]: InspectionHandler } = {};
-
-        // Create a handler for each console that is created.
-        consoles.widgetAdded.connect((sender, parent) => {
-            const sessionContext = parent.console.sessionContext;
-            const rendermime = parent.console.rendermime;
-            const connector = new KernelConnector({ sessionContext });
-            const handler = new InspectionHandler({ connector, rendermime });
-
-            // Associate the handler to the widget.
-            handlers[parent.id] = handler;
-
-            // Set the initial editor.
-            const cell = parent.console.promptCell;
-            handler.editor = cell && cell.editor;
-
-            // Listen for prompt creation.
-            parent.console.promptCellCreated.connect((sender, cell) => {
-                handler.editor = cell && cell.editor;
-            });
-
-            // Listen for parent disposal.
-            parent.disposed.connect(() => {
-                delete handlers[parent.id];
-                handler.dispose();
-            });
-        });
-
-        // Keep track of console instances and set inspector source.
-        labShell.currentChanged.connect((_, args) => {
-            const widget = args.newValue;
-            if (!widget || !consoles.has(widget)) {
-                return;
-            }
-            const source = handlers[widget.id];
-            if (source) {
-                manager.source = source;
-            }
-        });
-
-        app.contextMenu.addItem({
-            command: CommandIDs.toggle,
-            selector: '.jp-CodeConsole-promptCell'
-        });
+  // FIXME This should be in @jupyterlab/console-extension
+  id: 'jupyterlab_pausable_contextual_help:consoles',
+  description: 'Adds my code introspection support to consoles.',
+  requires: [IMyInspector, IConsoleTracker, ILabShell],
+  autoStart: true,
+  activate: (
+    app: JupyterFrontEnd,
+    manager: IMyInspector,
+    consoles: IConsoleTracker,
+    labShell: ILabShell,
+    translator: ITranslator
+  ): void => {
+    // Maintain association of new consoles with their respective handlers.
+    const handlers: { [id: string]: InspectionHandler } = {};
+
+    // Create a handler for each console that is created.
+    consoles.widgetAdded.connect((sender, parent) => {
+      const sessionContext = parent.console.sessionContext;
+      const rendermime = parent.console.rendermime;
+      const connector = new KernelConnector({ sessionContext });
+      const handler = new InspectionHandler({ connector, rendermime });
+
+      // Associate the handler to the widget.
+      handlers[parent.id] = handler;
+
+      // Set the initial editor.
+      const cell = parent.console.promptCell;
+      handler.editor = cell && cell.editor;
+
+      // Listen for prompt creation.
+      parent.console.promptCellCreated.connect((sender, cell) => {
+        handler.editor = cell && cell.editor;
+      });
+
+      // Listen for parent disposal.
+      parent.disposed.connect(() => {
+        delete handlers[parent.id];
+        handler.dispose();
+      });
+    });
+
+    // Keep track of console instances and set myinspector source.
+    const setSource = (widget: Widget | null): void => {
+      if (widget && consoles.has(widget) && handlers[widget.id]) {
+        manager.source = handlers[widget.id];
+      }
+    };
+    labShell.currentChanged.connect((_, args) => setSource(args.newValue));
+    void app.restored.then(() => setSource(labShell.currentWidget));
+
+    app.contextMenu.addItem({
+      command: CommandIDs.toggle,
+      selector: '.jp-CodeConsole-promptCell'
+    });
+
+    app.contextMenu.addItem({
+      command: CommandIDs.toggleStandby,
+      selector: '.jp-CodeConsole-promptCell'
+    });
 
-        app.contextMenu.addItem({
-            command: CommandIDs.toggleStandby,
-            selector: '.jp-CodeConsole-promptCell'
-        });
-    }
+  }
 };
 
 /**
  * An extension that registers notebooks for inspection.
  */
 const notebooks: JupyterFrontEndPlugin<void> = {
-    id: 'jupyterlab_pausable_contextual_help:notebooks',
-    requires: [IInspector, INotebookTracker, ILabShell],
-    autoStart: true,
-    activate: (
-        app: JupyterFrontEnd,
-        manager: IInspector,
-        notebooks: INotebookTracker,
-        labShell: ILabShell
-    ): void => {
-        // Maintain association of new notebooks with their respective handlers.
-        const handlers: { [id: string]: InspectionHandler } = {};
-
-        // Create a handler for each notebook that is created.
-        notebooks.widgetAdded.connect((sender, parent) => {
-            const sessionContext = parent.sessionContext;
-            const rendermime = parent.content.rendermime;
-            const connector = new KernelConnector({ sessionContext });
-            const handler = new InspectionHandler({ connector, rendermime });
-
-            // Associate the handler to the widget.
-            handlers[parent.id] = handler;
-
-            // Set the initial editor.
-            const cell = parent.content.activeCell;
-            handler.editor = cell && cell.editor;
-
-            // Listen for active cell changes.
-            parent.content.activeCellChanged.connect((sender, cell) => {
-                handler.editor = cell && cell.editor;
-            });
-
-            // Listen for parent disposal.
-            parent.disposed.connect(() => {
-                delete handlers[parent.id];
-                handler.dispose();
-            });
-        });
-
-        // Keep track of notebook instances and set inspector source.
-        labShell.currentChanged.connect((sender, args) => {
-            const widget = args.newValue;
-            if (!widget || !notebooks.has(widget)) {
-                return;
-            }
-            const source = handlers[widget.id];
-            if (source) {
-                manager.source = source;
-            }
-        });
+  // FIXME This should be in @jupyterlab/notebook-extension
+  id: 'jupyterlab_pausable_contextual_help:notebooks',
+  description: 'Adds code introspection to notebooks.',
+  requires: [IMyInspector, INotebookTracker, ILabShell],
+  autoStart: true,
+  activate: (
+    app: JupyterFrontEnd,
+    manager: IMyInspector,
+    notebooks: INotebookTracker,
+    labShell: ILabShell
+  ): void => {
+    // Maintain association of new notebooks with their respective handlers.
+    const handlers: { [id: string]: InspectionHandler } = {};
+
+    // Create a handler for each notebook that is created.
+    notebooks.widgetAdded.connect((sender, parent) => {
+      const sessionContext = parent.sessionContext;
+      const rendermime = parent.content.rendermime;
+      const connector = new KernelConnector({ sessionContext });
+      const handler = new InspectionHandler({ connector, rendermime });
+
+      // Associate the handler to the widget.
+      handlers[parent.id] = handler;
+
+      // Set the initial editor.
+      const cell = parent.content.activeCell;
+      handler.editor = cell && cell.editor;
+
+      // Listen for active cell changes.
+      parent.content.activeCellChanged.connect((sender, cell) => {
+        void cell?.ready.then(() => {
+          if (cell === parent.content.activeCell) {
+            handler.editor = cell!.editor;
+          }
+        });
+      });
+
+      // Listen for parent disposal.
+      parent.disposed.connect(() => {
+        delete handlers[parent.id];
+        handler.dispose();
+      });
+    });
+
+    // Keep track of notebook instances and set myinspector source.
+    const setSource = (widget: Widget | null): void => {
+      if (widget && notebooks.has(widget) && handlers[widget.id]) {
+        manager.source = handlers[widget.id];
+      }
+    };
+    labShell.currentChanged.connect((_, args) => setSource(args.newValue));
+    void app.restored.then(() => setSource(labShell.currentWidget));
+
+    app.contextMenu.addItem({
+      command: CommandIDs.toggle,
+      selector: '.jp-Notebook'
+    });
+
+    app.contextMenu.addItem({
+      command: CommandIDs.toggleStandby,
+      selector: '.jp-Notebook'
+    });
 
-        app.contextMenu.addItem({
-            command: CommandIDs.toggle,
-            selector: '.jp-Notebook'
-        });
-
-        app.contextMenu.addItem({
-            command: CommandIDs.toggleStandby,
-            selector: '.jp-Notebook'
-        });
-
-    }
+  }
 };
 
 /**
  * Export the plugins as default.
  */
-const plugins: JupyterFrontEndPlugin<any>[] = [inspector, consoles, notebooks];
+const plugins: JupyterFrontEndPlugin<any>[] = [myinspector, consoles, notebooks];
 export default plugins;
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/src/inspector.ts` & `jupyterlab_pausable_contextual_help-0.1.3/src/myinspector.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,166 +1,167 @@
 // Copyright (c) Jupyter Development Team.
 // Distributed under the terms of the Modified BSD License.
 
 import { Printing } from '@jupyterlab/apputils';
 import {
-    ITranslator,
-    nullTranslator,
-    TranslationBundle
+  ITranslator,
+  nullTranslator,
+  TranslationBundle
 } from '@jupyterlab/translation';
 import { Panel, PanelLayout, Widget } from '@lumino/widgets';
-import { IInspector } from './tokens';
+import { IMyInspector } from './tokens';
 
 /**
- * The class name added to inspector panels.
+ * The class name added to myinspector panels.
  */
-const PANEL_CLASS = 'jp-Inspector';
+const PANEL_CLASS = 'jp-MyInspector';
 
 /**
- * The class name added to inspector content.
+ * The class name added to myinspector content.
  */
-const CONTENT_CLASS = 'jp-Inspector-content';
+const CONTENT_CLASS = 'jp-MyInspector-content';
 
 /**
- * The class name added to default inspector content.
+ * The class name added to default myinspector content.
  */
-const DEFAULT_CONTENT_CLASS = 'jp-Inspector-default-content';
+const DEFAULT_CONTENT_CLASS = 'jp-MyInspector-default-content';
 
 /**
- * A panel which contains a set of inspectors.
+ * A panel which contains a set of myinspectors.
  */
-export class InspectorPanel
-    extends Panel
-    implements IInspector, Printing.IPrintable {
-    /**
-     * Construct an inspector.
-     */
-    constructor(options: InspectorPanel.IOptions = {}) {
-        super();
-        this.translator = options.translator || nullTranslator;
-        this._trans = this.translator.load('jupyterlab');
-
-        if (options.initialContent instanceof Widget) {
-            this._content = options.initialContent;
-        } else if (typeof options.initialContent === 'string') {
-            this._content = InspectorPanel._generateContentWidget(
-                `<p>${options.initialContent}</p>`
-            );
-        } else {
-            this._content = InspectorPanel._generateContentWidget(
-                '<p>' +
+export class MyInspectorPanel
+  extends Panel
+  implements IMyInspector, Printing.IPrintable
+{
+  /**
+   * Construct an myinspector.
+   */
+  constructor(options: MyInspectorPanel.IOptions = {}) {
+    super();
+    this.translator = options.translator || nullTranslator;
+    this._trans = this.translator.load('jupyterlab');
+
+    if (options.initialContent instanceof Widget) {
+      this._content = options.initialContent;
+    } else if (typeof options.initialContent === 'string') {
+      this._content = MyInspectorPanel._generateContentWidget(
+        `<p>${options.initialContent}</p>`
+      );
+    } else {
+      this._content = MyInspectorPanel._generateContentWidget(
+        '<p>' +
                 this._trans.__('Press F1 on a function to see documentation.') +
-                '</p>'
-            );
-        }
-
-        this.addClass(PANEL_CLASS);
-        (this.layout as PanelLayout).addWidget(this._content);
+          '</p>'
+      );
     }
 
-    /**
-     * Print in iframe
-     */
-    [Printing.symbol]() {
-        return (): Promise<void> => Printing.printWidget(this);
-    }
+    this.addClass(PANEL_CLASS);
+    (this.layout as PanelLayout).addWidget(this._content);
+  }
 
-    /**
-     * The source of events the inspector panel listens for.
-     */
-    get source(): IInspector.IInspectable | null {
-        return this._source;
-    }
-    set source(source: IInspector.IInspectable | null) {
-        if (this._source === source) {
-            return;
-        }
-
-        // Disconnect old signal handler.
-        if (this._source) {
-            this._source.standby = true;
-            this._source.inspected.disconnect(this.onInspectorUpdate, this);
-            this._source.disposed.disconnect(this.onSourceDisposed, this);
-        }
-
-        // Reject a source that is already disposed.
-        if (source && source.isDisposed) {
-            source = null;
-        }
-
-        // Update source.
-        this._source = source;
+  /**
+   * Print in iframe
+   */
+  [Printing.symbol]() {
+    return (): Promise<void> => Printing.printWidget(this);
+  }
 
-        // Connect new signal handler.
-        if (this._source) {
-            //   this._source.standby = false;
-            this._source.inspected.connect(this.onInspectorUpdate, this);
-            this._source.disposed.connect(this.onSourceDisposed, this);
-        }
+  /**
+   * The source of events the myinspector panel listens for.
+   */
+  get source(): IMyInspector.IInspectable | null {
+    return this._source;
+  }
+  set source(source: IMyInspector.IInspectable | null) {
+    if (this._source === source) {
+      return;
     }
 
-    /**
-     * Dispose of the resources held by the widget.
-     */
-    dispose(): void {
-        if (this.isDisposed) {
-            return;
-        }
-        this.source = null;
-        super.dispose();
+    // Disconnect old signal handler.
+    if (this._source) {
+      this._source.standby = true;
+      this._source.inspected.disconnect(this.onMyInspectorUpdate, this);
+      this._source.disposed.disconnect(this.onSourceDisposed, this);
     }
 
-    /**
-     * Handle inspector update signals.
-     */
-    protected onInspectorUpdate(
-        sender: any,
-        args: IInspector.IInspectorUpdate
-    ): void {
-        const { content } = args;
-
-        // Update the content of the inspector widget.
-        if (!content || content === this._content) {
-            return;
-        }
-        this._content.dispose();
-
-        this._content = content;
-        content.addClass(CONTENT_CLASS);
-        (this.layout as PanelLayout).addWidget(content);
+    // Reject a source that is already disposed.
+    if (source && source.isDisposed) {
+      source = null;
     }
 
-    /**
-     * Handle source disposed signals.
-     */
-    protected onSourceDisposed(sender: any, args: void): void {
-        this.source = null;
-    }
+    // Update source.
+    this._source = source;
 
-    /**
-     * Generate content widget from string
-     */
-    private static _generateContentWidget(message: string): Widget {
-        const widget = new Widget();
-        widget.node.innerHTML = message;
-        widget.addClass(CONTENT_CLASS);
-        widget.addClass(DEFAULT_CONTENT_CLASS);
-
-        return widget;
+    // Connect new signal handler.
+    if (this._source) {
+            //   this._source.standby = false;
+      this._source.inspected.connect(this.onMyInspectorUpdate, this);
+      this._source.disposed.connect(this.onSourceDisposed, this);
     }
+  }
 
-    protected translator: ITranslator;
-    private _trans: TranslationBundle;
-    private _content: Widget;
-    private _source: IInspector.IInspectable | null = null;
+  /**
+   * Dispose of the resources held by the widget.
+   */
+  dispose(): void {
+    if (this.isDisposed) {
+      return;
+    }
+    this.source = null;
+    super.dispose();
+  }
+
+  /**
+   * Handle myinspector update signals.
+   */
+  protected onMyInspectorUpdate(
+    sender: any,
+    args: IMyInspector.IMyInspectorUpdate
+  ): void {
+    const { content } = args;
+
+    // Update the content of the myinspector widget.
+    if (!content || content === this._content) {
+      return;
+    }
+    this._content.dispose();
+
+    this._content = content;
+    content.addClass(CONTENT_CLASS);
+    (this.layout as PanelLayout).addWidget(content);
+  }
+
+  /**
+   * Handle source disposed signals.
+   */
+  protected onSourceDisposed(sender: any, args: void): void {
+    this.source = null;
+  }
+
+  /**
+   * Generate content widget from string
+   */
+  private static _generateContentWidget(message: string): Widget {
+    const widget = new Widget();
+    widget.node.innerHTML = message;
+    widget.addClass(CONTENT_CLASS);
+    widget.addClass(DEFAULT_CONTENT_CLASS);
+
+    return widget;
+  }
+
+  protected translator: ITranslator;
+  private _trans: TranslationBundle;
+  private _content: Widget;
+  private _source: IMyInspector.IInspectable | null = null;
 }
 
-export namespace InspectorPanel {
-    export interface IOptions {
-        initialContent?: Widget | string | undefined;
-
-        /**
-         * The application language translator.
-         */
-        translator?: ITranslator;
-    }
+export namespace MyInspectorPanel {
+  export interface IOptions {
+    initialContent?: Widget | string | undefined;
+
+    /**
+     * The application language translator.
+     */
+    translator?: ITranslator;
+  }
 }
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/src/kernelconnector.ts` & `jupyterlab_pausable_contextual_help-0.1.3/src/kernelconnector.ts`

 * *Files 16% similar despite different names*

```diff
@@ -6,69 +6,69 @@
 import { DataConnector } from '@jupyterlab/statedb';
 import { InspectionHandler } from './handler';
 
 /**
  * The default connector for making inspection requests from the Jupyter API.
  */
 export class KernelConnector extends DataConnector<
-    InspectionHandler.IReply,
-    void,
-    InspectionHandler.IRequest
+  InspectionHandler.IReply,
+  void,
+  InspectionHandler.IRequest
 > {
-    /**
-     * Create a new kernel connector for inspection requests.
-     *
-     * @param options - The instantiation options for the kernel connector.
-     */
-    constructor(options: KernelConnector.IOptions) {
-        super();
-        this._sessionContext = options.sessionContext;
-    }
-
-    /**
-     * Fetch inspection requests.
-     *
-     * @param request - The inspection request text and details.
-     */
-    fetch(
-        request: InspectionHandler.IRequest
-    ): Promise<InspectionHandler.IReply> {
-        const kernel = this._sessionContext.session?.kernel;
-
-        if (!kernel) {
-            return Promise.reject(new Error('Inspection fetch requires a kernel.'));
-        }
-
-        const contents: KernelMessage.IInspectRequestMsg['content'] = {
-            code: request.text,
-            cursor_pos: request.offset,
-            detail_level: 1
-        };
-
-        return kernel.requestInspect(contents).then(msg => {
-            const response = msg.content;
-
-            if (response.status !== 'ok' || !response.found) {
-                throw new Error('Inspection fetch failed to return successfully.');
-            }
+  /**
+   * Create a new kernel connector for inspection requests.
+   *
+   * @param options - The instantiation options for the kernel connector.
+   */
+  constructor(options: KernelConnector.IOptions) {
+    super();
+    this._sessionContext = options.sessionContext;
+  }
+
+  /**
+   * Fetch inspection requests.
+   *
+   * @param request - The inspection request text and details.
+   */
+  fetch(
+    request: InspectionHandler.IRequest
+  ): Promise<InspectionHandler.IReply> {
+    const kernel = this._sessionContext.session?.kernel;
 
-            return { data: response.data, metadata: response.metadata };
-        });
+    if (!kernel) {
+      return Promise.reject(new Error('Inspection fetch requires a kernel.'));
     }
 
-    private _sessionContext: ISessionContext;
+    const contents: KernelMessage.IInspectRequestMsg['content'] = {
+      code: request.text,
+      cursor_pos: request.offset,
+      detail_level: 1
+    };
+
+    return kernel.requestInspect(contents).then(msg => {
+      const response = msg.content;
+
+      if (response.status !== 'ok' || !response.found) {
+        throw new Error('Inspection fetch failed to return successfully.');
+      }
+
+      return { data: response.data, metadata: response.metadata };
+    });
+  }
+
+  private _sessionContext: ISessionContext;
 }
 
 /**
  * A namespace for kernel connector statics.
  */
 export namespace KernelConnector {
+  /**
+   * The instantiation options for an inspection handler.
+   */
+  export interface IOptions {
     /**
-     * The instantiation options for an inspection handler.
+     * The session context used to make API requests to the kernel.
      */
-    export interface IOptions {
-        /**
-         * The session context used to make API requests to the kernel.
-         */
-        sessionContext: ISessionContext;
-    }
+    sessionContext: ISessionContext;
+  }
 }
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/style/index.css` & `jupyterlab_pausable_contextual_help-0.1.3/style/index.css`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 /*-----------------------------------------------------------------------------
 | Copyright (c) Jupyter Development Team.
 | Distributed under the terms of the Modified BSD License.
 |----------------------------------------------------------------------------*/
 
 /* This file was auto-generated by ensurePackage() in @jupyterlab/buildutils */
-/* @import url('~@lumino/widgets/style/index.css');
+@import url('~@lumino/widgets/style/index.css');
 @import url('~@jupyterlab/apputils/style/index.css');
 @import url('~@jupyterlab/codeeditor/style/index.css');
 @import url('~@jupyterlab/rendermime/style/index.css');
 @import url('~@jupyterlab/ui-components/style/index.css');
 @import url('~@jupyterlab/application/style/index.css');
 @import url('~@jupyterlab/console/style/index.css');
 @import url('~@jupyterlab/inspector/style/index.css');
 @import url('~@jupyterlab/launcher/style/index.css');
-@import url('~@jupyterlab/notebook/style/index.css'); */
-/* @import url('~@jupyterlab/ui-components/style/index.css');
-@import url('~@jupyterlab/apputils/style/index.css');
-@import url('~@jupyterlab/application/style/index.css');
-@import url('~@jupyterlab/console/style/index.css');
-@import url('~@jupyterlab/inspector/style/index.css');
-@import url('~@jupyterlab/launcher/style/index.css');
-@import url('~@jupyterlab/notebook/style/index.css'); */
-
-@import url('./base.css');
+@import url('~@jupyterlab/notebook/style/index.css');
+@import url('./base.css');
```

### Comparing `jupyterlab_pausable_contextual_help-0.1.2/tsconfig.json` & `jupyterlab_pausable_contextual_help-0.1.3/tsconfig.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9802631578947368%*

 * *Differences: {"'compilerOptions'": "{'target': 'ES2018', delete: ['types']}"}*

```diff
@@ -13,14 +13,13 @@
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
         "strictNullChecks": true,
-        "target": "es2018",
-        "types": []
+        "target": "ES2018"
     },
     "include": [
         "src/*"
     ]
 }
```

