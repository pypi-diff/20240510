# Comparing `tmp/django-pipeline-3.0.0.tar.gz` & `tmp/django_pipeline-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pipeline-3.0.0.tar", last modified: Wed Dec 27 11:18:54 2023, max compression
+gzip compressed data, was "django_pipeline-3.1.0.tar", last modified: Thu Apr 18 02:04:53 2024, max compression
```

## Comparing `django-pipeline-3.0.0.tar` & `django_pipeline-3.1.0.tar`

### file list

```diff
@@ -1,183 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.064877 django-pipeline-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.032877 django-pipeline-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.036877 django-pipeline-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2023-12-27 11:18:54.064877 django-pipeline-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.064877 django-pipeline-3.0.0/django_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2023-12-27 11:18:53.000000 django-pipeline-3.0.0/django_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2023-12-27 11:18:54.000000 django-pipeline-3.0.0/django_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 11:18:53.000000 django-pipeline-3.0.0/django_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 11:18:53.000000 django-pipeline-3.0.0/django_pipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-27 11:18:53.000000 django-pipeline-3.0.0/django_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.040877 django-pipeline-3.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/docs/compilers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/docs/compressors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/docs/signals.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/docs/storages.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/docs/templates.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/docs/using.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.040877 django-pipeline-3.0.0/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/img/django-pipeline.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.044877 django-pipeline-3.0.0/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.044877 django-pipeline-3.0.0/pipeline/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compilers/coffee.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compilers/es6.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compilers/less.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compilers/livescript.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compilers/sass.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compilers/stylus.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compilers/typescript.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.048877 django-pipeline-3.0.0/pipeline/compressors/
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compressors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compressors/closure.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compressors/csshtmljsminify.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compressors/cssmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compressors/csstidy.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compressors/jsmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compressors/terser.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compressors/uglifyjs.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compressors/yuglify.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/compressors/yui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/finders.py
--rw-r--r--   0 runner    (1001) docker     (127)     9287 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/glob.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.048877 django-pipeline-3.0.0/pipeline/jinja2/
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/jinja2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.048877 django-pipeline-3.0.0/pipeline/jinja2/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/jinja2/pipeline/css.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/jinja2/pipeline/inline_js.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/jinja2/pipeline/js.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      928 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/packager.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.032877 django-pipeline-3.0.0/pipeline/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.048877 django-pipeline-3.0.0/pipeline/templates/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/templates/pipeline/compile_error.html
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/templates/pipeline/css.html
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/templates/pipeline/css.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/templates/pipeline/inline_js.html
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/templates/pipeline/inline_js.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/templates/pipeline/js.html
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/templates/pipeline/js.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.048877 django-pipeline-3.0.0/pipeline/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/templatetags/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pipeline/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-27 11:18:54.064877 django-pipeline-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.052877 django-pipeline-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.036877 django-pipeline-3.0.0/tests/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.032877 django-pipeline-3.0.0/tests/assets/compilers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.052877 django-pipeline-3.0.0/tests/assets/compilers/coffee/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/coffee/expected.js
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/coffee/input.coffee
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.052877 django-pipeline-3.0.0/tests/assets/compilers/es6/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/es6/expected.js
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/es6/input.es6
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.052877 django-pipeline-3.0.0/tests/assets/compilers/less/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/less/expected.css
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/less/input.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.052877 django-pipeline-3.0.0/tests/assets/compilers/livescript/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/livescript/expected.js
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/livescript/input.ls
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.052877 django-pipeline-3.0.0/tests/assets/compilers/scss/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/scss/expected.css
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/scss/input.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.052877 django-pipeline-3.0.0/tests/assets/compilers/stylus/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/stylus/expected.css
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/stylus/input.styl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.052877 django-pipeline-3.0.0/tests/assets/compilers/typescript/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/typescript/expected.js
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compilers/typescript/input.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.056877 django-pipeline-3.0.0/tests/assets/compressors/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compressors/closure.js
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compressors/csshtmljsminify.css
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compressors/csshtmljsminify.js
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compressors/cssmin.css
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compressors/csstidy.css
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compressors/jsmin.js
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compressors/slimit.js
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compressors/terser.js
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compressors/uglifyjs.js
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compressors/yuglify.css
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compressors/yuglify.js
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compressors/yui.css
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/compressors/yui.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.056877 django-pipeline-3.0.0/tests/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/css/first.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.056877 django-pipeline-3.0.0/tests/assets/css/nested/
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/css/nested/nested.css
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/css/second.css
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/css/unicode.css
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/css/urls.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.056877 django-pipeline-3.0.0/tests/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/fonts/pipeline.eot
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/fonts/pipeline.svg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/fonts/pipeline.ttf
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/fonts/pipeline.woff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.060877 django-pipeline-3.0.0/tests/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/images/arrow.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.060877 django-pipeline-3.0.0/tests/assets/images/embed/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/images/embed/arrow.png
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/images/sprite-buttons.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.060877 django-pipeline-3.0.0/tests/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/js/application.js
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/js/dummy.coffee
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/js/first.js
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/js/second.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.036877 django-pipeline-3.0.0/tests/assets/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.060877 django-pipeline-3.0.0/tests/assets/templates/photo/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/templates/photo/detail.jst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/templates/photo/list.jst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.060877 django-pipeline-3.0.0/tests/assets/templates/video/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/assets/templates/video/detail.jst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.060877 django-pipeline-3.0.0/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/templates/empty.html
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:54.064877 django-pipeline-3.0.0/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     9802 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15662 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/test_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6773 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/test_glob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/test_packager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/test_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 11:18:42.000000 django-pipeline-3.0.0/tests/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.117423 django_pipeline-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.089423 django_pipeline-3.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.097422 django_pipeline-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13292 2024-04-18 02:04:53.117423 django_pipeline-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.117423 django_pipeline-3.1.0/django_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13292 2024-04-18 02:04:53.000000 django_pipeline-3.1.0/django_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-18 02:04:53.000000 django_pipeline-3.1.0/django_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 02:04:53.000000 django_pipeline-3.1.0/django_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 02:04:53.000000 django_pipeline-3.1.0/django_pipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 02:04:53.000000 django_pipeline-3.1.0/django_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.097422 django_pipeline-3.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/docs/compilers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/docs/compressors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/docs/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/docs/storages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/docs/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/docs/using.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.097422 django_pipeline-3.1.0/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/img/django-pipeline.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.101423 django_pipeline-3.1.0/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.101423 django_pipeline-3.1.0/pipeline/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compilers/coffee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compilers/es6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compilers/less.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compilers/livescript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compilers/sass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compilers/stylus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compilers/typescript.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.105423 django_pipeline-3.1.0/pipeline/compressors/
+-rw-r--r--   0 runner    (1001) docker     (127)    15335 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compressors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compressors/closure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compressors/csshtmljsminify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compressors/cssmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compressors/csstidy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compressors/jsmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compressors/terser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compressors/uglifyjs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compressors/yuglify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/compressors/yui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/finders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/glob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.105423 django_pipeline-3.1.0/pipeline/jinja2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/jinja2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.105423 django_pipeline-3.1.0/pipeline/jinja2/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/jinja2/pipeline/css.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/jinja2/pipeline/inline_js.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/jinja2/pipeline/js.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/packager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.089423 django_pipeline-3.1.0/pipeline/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.105423 django_pipeline-3.1.0/pipeline/templates/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/templates/pipeline/compile_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/templates/pipeline/css.html
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/templates/pipeline/css.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/templates/pipeline/inline_js.html
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/templates/pipeline/inline_js.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/templates/pipeline/js.html
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/templates/pipeline/js.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.105423 django_pipeline-3.1.0/pipeline/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8025 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/templatetags/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pipeline/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-18 02:04:53.117423 django_pipeline-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.105423 django_pipeline-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.093423 django_pipeline-3.1.0/tests/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.089423 django_pipeline-3.1.0/tests/assets/compilers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.109423 django_pipeline-3.1.0/tests/assets/compilers/coffee/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/coffee/expected.js
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/coffee/input.coffee
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.109423 django_pipeline-3.1.0/tests/assets/compilers/es6/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/es6/expected.js
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/es6/input.es6
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.109423 django_pipeline-3.1.0/tests/assets/compilers/less/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/less/expected.css
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/less/input.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.109423 django_pipeline-3.1.0/tests/assets/compilers/livescript/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/livescript/expected.js
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/livescript/input.ls
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.109423 django_pipeline-3.1.0/tests/assets/compilers/scss/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/scss/expected.css
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/scss/input.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.109423 django_pipeline-3.1.0/tests/assets/compilers/stylus/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/stylus/expected.css
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/stylus/input.styl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.109423 django_pipeline-3.1.0/tests/assets/compilers/typescript/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/typescript/expected.js
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compilers/typescript/input.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.113423 django_pipeline-3.1.0/tests/assets/compressors/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compressors/closure.js
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compressors/csshtmljsminify.css
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compressors/csshtmljsminify.js
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compressors/cssmin.css
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compressors/csstidy.css
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compressors/jsmin.js
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compressors/slimit.js
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compressors/terser.js
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compressors/uglifyjs.js
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compressors/yuglify.css
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compressors/yuglify.js
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compressors/yui.css
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/compressors/yui.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.113423 django_pipeline-3.1.0/tests/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/css/first.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.113423 django_pipeline-3.1.0/tests/assets/css/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/css/nested/nested.css
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/css/second.css
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/css/sourcemap.css
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/css/unicode.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/css/urls.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.113423 django_pipeline-3.1.0/tests/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/fonts/pipeline.eot
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/fonts/pipeline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/fonts/pipeline.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/fonts/pipeline.woff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.113423 django_pipeline-3.1.0/tests/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/images/arrow.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.113423 django_pipeline-3.1.0/tests/assets/images/embed/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/images/embed/arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/images/sprite-buttons.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.113423 django_pipeline-3.1.0/tests/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/js/application.js
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/js/dummy.coffee
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/js/first.js
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/js/second.js
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/js/sourcemap.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.093423 django_pipeline-3.1.0/tests/assets/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.113423 django_pipeline-3.1.0/tests/assets/templates/photo/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/templates/photo/detail.jst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/templates/photo/list.jst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.113423 django_pipeline-3.1.0/tests/assets/templates/video/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/assets/templates/video/detail.jst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.117423 django_pipeline-3.1.0/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/templates/empty.html
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:53.117423 django_pipeline-3.1.0/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27204 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/test_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/test_glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/test_packager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:04:40.000000 django_pipeline-3.1.0/tests/views.py
```

### Comparing `django-pipeline-3.0.0/.github/workflows/release.yml` & `django_pipeline-3.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/.github/workflows/test.yml` & `django_pipeline-3.1.0/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -87,8 +87,8 @@
         name: Python ${{ matrix.python-version }}
 
   ruff:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - run: pip install --user ruff
-    - run: ruff --extend-select=C4,C9,I,PLC,PLE,PLR,U --ignore=C414,I001,UP032 --target-version=py38 .
+    - run: ruff --extend-select=C4,C9,I,PLC,PLE,PLR,U --ignore=C414,I001,PLR0913,UP007,UP032 --target-version=py38 .
```

### Comparing `django-pipeline-3.0.0/AUTHORS` & `django_pipeline-3.1.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/CODE_OF_CONDUCT.md` & `django_pipeline-3.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/CONTRIBUTING.rst` & `django_pipeline-3.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/HISTORY.rst` & `django_pipeline-3.1.0/HISTORY.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 .. :changelog:
 
 History
 =======
 
+3.1.0
+=====
+
+* Fixed concatenation to update relative sourceMappingURL paths (#808). This
+  was effectively breaking pipeline usage on Django 4+.
+* Fixed the django-pipeline-error box that gets injected into HTML pages to
+  hard-code a text color in addition to a background color. This ensures that
+  the text is readable, even on pages that are rendered with light text colors.
+* Added filtering for the django-pipeline-error box to remove ANSI color codes,
+  which are included by some tools.
+
 3.0.0
 =====
 
 * Use Pypy 3.10
 * Drop support for Python 3.7
 * Drop support for Django 2
 * Add Python 3.12 support
```

### Comparing `django-pipeline-3.0.0/LICENSE` & `django_pipeline-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/PKG-INFO` & `django_pipeline-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pipeline
-Version: 3.0.0
+Version: 3.1.0
 Summary: Pipeline is an asset packaging library for Django.
 Home-page: https://github.com/jazzband/django-pipeline
 Author: Timothée Peignier
 Author-email: timothee.peignier@tryphon.org
 License: MIT
 Keywords: django pipeline asset compiling concatenation compression packaging
 Classifier: Development Status :: 5 - Production/Stable
@@ -179,14 +179,25 @@
 
 
 .. :changelog:
 
 History
 =======
 
+3.1.0
+=====
+
+* Fixed concatenation to update relative sourceMappingURL paths (#808). This
+  was effectively breaking pipeline usage on Django 4+.
+* Fixed the django-pipeline-error box that gets injected into HTML pages to
+  hard-code a text color in addition to a background color. This ensures that
+  the text is readable, even on pages that are rendered with light text colors.
+* Added filtering for the django-pipeline-error box to remove ANSI color codes,
+  which are included by some tools.
+
 3.0.0
 =====
 
 * Use Pypy 3.10
 * Drop support for Python 3.7
 * Drop support for Django 2
 * Add Python 3.12 support
```

### Comparing `django-pipeline-3.0.0/README.rst` & `django_pipeline-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/django_pipeline.egg-info/PKG-INFO` & `django_pipeline-3.1.0/django_pipeline.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pipeline
-Version: 3.0.0
+Version: 3.1.0
 Summary: Pipeline is an asset packaging library for Django.
 Home-page: https://github.com/jazzband/django-pipeline
 Author: Timothée Peignier
 Author-email: timothee.peignier@tryphon.org
 License: MIT
 Keywords: django pipeline asset compiling concatenation compression packaging
 Classifier: Development Status :: 5 - Production/Stable
@@ -179,14 +179,25 @@
 
 
 .. :changelog:
 
 History
 =======
 
+3.1.0
+=====
+
+* Fixed concatenation to update relative sourceMappingURL paths (#808). This
+  was effectively breaking pipeline usage on Django 4+.
+* Fixed the django-pipeline-error box that gets injected into HTML pages to
+  hard-code a text color in addition to a background color. This ensures that
+  the text is readable, even on pages that are rendered with light text colors.
+* Added filtering for the django-pipeline-error box to remove ANSI color codes,
+  which are included by some tools.
+
 3.0.0
 =====
 
 * Use Pypy 3.10
 * Drop support for Python 3.7
 * Drop support for Django 2
 * Add Python 3.12 support
```

### Comparing `django-pipeline-3.0.0/django_pipeline.egg-info/SOURCES.txt` & `django_pipeline-3.1.0/django_pipeline.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -107,28 +107,30 @@
 tests/assets/compressors/uglifyjs.js
 tests/assets/compressors/yuglify.css
 tests/assets/compressors/yuglify.js
 tests/assets/compressors/yui.css
 tests/assets/compressors/yui.js
 tests/assets/css/first.css
 tests/assets/css/second.css
+tests/assets/css/sourcemap.css
 tests/assets/css/unicode.css
 tests/assets/css/urls.css
 tests/assets/css/nested/nested.css
 tests/assets/fonts/pipeline.eot
 tests/assets/fonts/pipeline.svg
 tests/assets/fonts/pipeline.ttf
 tests/assets/fonts/pipeline.woff
 tests/assets/images/arrow.png
 tests/assets/images/sprite-buttons.png
 tests/assets/images/embed/arrow.png
 tests/assets/js/application.js
 tests/assets/js/dummy.coffee
 tests/assets/js/first.js
 tests/assets/js/second.js
+tests/assets/js/sourcemap.js
 tests/assets/templates/photo/detail.jst
 tests/assets/templates/photo/list.jst
 tests/assets/templates/video/detail.jst
 tests/templates/empty.html
 tests/templates/index.html
 tests/tests/__init__.py
 tests/tests/models.py
```

### Comparing `django-pipeline-3.0.0/docs/Makefile` & `django_pipeline-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/docs/compilers.rst` & `django_pipeline-3.1.0/docs/compilers.rst`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/docs/compressors.rst` & `django_pipeline-3.1.0/docs/compressors.rst`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/docs/conf.py` & `django_pipeline-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/docs/configuration.rst` & `django_pipeline-3.1.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/docs/index.rst` & `django_pipeline-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/docs/installation.rst` & `django_pipeline-3.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/docs/make.bat` & `django_pipeline-3.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/docs/signals.rst` & `django_pipeline-3.1.0/docs/signals.rst`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/docs/storages.rst` & `django_pipeline-3.1.0/docs/storages.rst`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/docs/templates.rst` & `django_pipeline-3.1.0/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/docs/usage.rst` & `django_pipeline-3.1.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/docs/using.rst` & `django_pipeline-3.1.0/docs/using.rst`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/img/django-pipeline.svg` & `django_pipeline-3.1.0/img/django-pipeline.svg`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/__init__.py` & `django_pipeline-3.1.0/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/collector.py` & `django_pipeline-3.1.0/pipeline/collector.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/compilers/__init__.py` & `django_pipeline-3.1.0/pipeline/compilers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/compilers/coffee.py` & `django_pipeline-3.1.0/pipeline/compilers/coffee.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/compilers/es6.py` & `django_pipeline-3.1.0/pipeline/compilers/es6.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/compilers/less.py` & `django_pipeline-3.1.0/pipeline/compilers/less.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/compilers/livescript.py` & `django_pipeline-3.1.0/pipeline/compilers/livescript.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/compilers/typescript.py` & `django_pipeline-3.1.0/pipeline/compilers/typescript.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/compressors/csstidy.py` & `django_pipeline-3.1.0/pipeline/compressors/csstidy.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/compressors/yuglify.py` & `django_pipeline-3.1.0/pipeline/compressors/yuglify.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/compressors/yui.py` & `django_pipeline-3.1.0/pipeline/compressors/yui.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/conf.py` & `django_pipeline-3.1.0/pipeline/conf.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/finders.py` & `django_pipeline-3.1.0/pipeline/finders.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/forms.py` & `django_pipeline-3.1.0/pipeline/forms.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/glob.py` & `django_pipeline-3.1.0/pipeline/glob.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/jinja2/__init__.py` & `django_pipeline-3.1.0/pipeline/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/middleware.py` & `django_pipeline-3.1.0/pipeline/middleware.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/packager.py` & `django_pipeline-3.1.0/pipeline/packager.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
         return output_filename
 
     def pack_javascripts(self, package, **kwargs):
         return self.pack(
             package,
             self.compressor.compress_js,
             js_compressed,
+            output_filename=package.output_filename,
             templates=package.templates,
             **kwargs,
         )
 
     def pack_templates(self, package):
         return self.compressor.compile_templates(package.templates)
```

### Comparing `django-pipeline-3.0.0/pipeline/storage.py` & `django_pipeline-3.1.0/pipeline/storage.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/templates/pipeline/compile_error.html` & `django_pipeline-3.1.0/pipeline/templates/pipeline/compile_error.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <div id="django-pipeline-error-{{package_name}}" class="django-pipeline-error"
-     style="display: none; border: 2px #DD0000 solid; margin: 1em; padding: 1em; background: white;">
+     style="display: none; border: 2px #DD0000 solid; margin: 1em; padding: 1em; background: white; color: black;">
  <h1>Error compiling {{package_type}} package "{{package_name}}"</h1>
  <p><strong>Command:</strong></p>
  <pre style="white-space: pre-wrap;">{{command}}</pre>
  <p><strong>Errors:</strong></p>
  <pre style="white-space: pre-wrap;">{{errors}}</pre>
 </div>
```

### Comparing `django-pipeline-3.0.0/pipeline/templatetags/pipeline.py` & `django_pipeline-3.1.0/pipeline/templatetags/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import re
 import subprocess
 
 from django import template
 from django.contrib.staticfiles.storage import staticfiles_storage
 from django.template.base import VariableDoesNotExist
 from django.template.loader import render_to_string
 from django.utils.safestring import mark_safe
@@ -105,21 +106,28 @@
                 raise
 
         templates = packager.pack_templates(package)
 
         return method(package, paths, templates=templates)
 
     def render_error(self, package_type, package_name, e):
+        # Remove any ANSI escape sequences in the output.
+        error_output = re.sub(
+            re.compile(r"(?:\x1B[@-_]|[\x80-\x9F])[0-?]*[ -/]*[@-~]"),
+            "",
+            e.error_output,
+        )
+
         return render_to_string(
             "pipeline/compile_error.html",
             {
                 "package_type": package_type,
                 "package_name": package_name,
                 "command": subprocess.list2cmdline(e.command),
-                "errors": e.error_output,
+                "errors": error_output,
             },
         )
 
 
 class StylesheetNode(PipelineMixin, template.Node):
     def __init__(self, name):
         self.name = name
@@ -128,15 +136,15 @@
         super().render(context)
         package_name = template.Variable(self.name).resolve(context)
 
         try:
             package = self.package_for(package_name, "css")
         except PackageNotFound:
             w = "Package %r is unknown. Check PIPELINE['STYLESHEETS'] in your settings."
-            logger.warn(w, package_name)
+            logger.warning(w, package_name)
             # fail silently, do not return anything if an invalid group is specified
             return ""
         return self.render_compressed(package, package_name, "css")
 
     def render_css(self, package, path):
         template_name = package.template_name or "pipeline/css.html"
         context = package.extra_context
@@ -164,15 +172,15 @@
         super().render(context)
         package_name = template.Variable(self.name).resolve(context)
 
         try:
             package = self.package_for(package_name, "js")
         except PackageNotFound:
             w = "Package %r is unknown. Check PIPELINE['JAVASCRIPT'] in your settings."
-            logger.warn(w, package_name)
+            logger.warning(w, package_name)
             # fail silently, do not return anything if an invalid group is specified
             return ""
         return self.render_compressed(package, package_name, "js")
 
     def render_js(self, package, path):
         template_name = package.template_name or "pipeline/js.html"
         context = package.extra_context
```

### Comparing `django-pipeline-3.0.0/pipeline/utils.py` & `django_pipeline-3.1.0/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/pipeline/views.py` & `django_pipeline-3.1.0/pipeline/views.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/setup.py` & `django_pipeline-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/assets/css/nested/nested.css` & `django_pipeline-3.1.0/tests/assets/css/nested/nested.css`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/assets/css/urls.css` & `django_pipeline-3.1.0/tests/assets/css/urls.css`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/settings.py` & `django_pipeline-3.1.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/tests/test_collector.py` & `django_pipeline-3.1.0/tests/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/tests/test_compiler.py` & `django_pipeline-3.1.0/tests/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/tests/test_conf.py` & `django_pipeline-3.1.0/tests/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/tests/test_forms.py` & `django_pipeline-3.1.0/tests/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/tests/test_glob.py` & `django_pipeline-3.1.0/tests/tests/test_glob.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/tests/test_middleware.py` & `django_pipeline-3.1.0/tests/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/tests/test_packager.py` & `django_pipeline-3.1.0/tests/tests/test_packager.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/tests/test_storage.py` & `django_pipeline-3.1.0/tests/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/tests/test_template.py` & `django_pipeline-3.1.0/tests/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/tests/test_utils.py` & `django_pipeline-3.1.0/tests/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/tests/test_views.py` & `django_pipeline-3.1.0/tests/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-pipeline-3.0.0/tests/utils.py` & `django_pipeline-3.1.0/tests/utils.py`

 * *Files identical despite different names*

