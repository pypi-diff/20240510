# Comparing `tmp/reacnetgenerator-1.6.7.tar.gz` & `tmp/reacnetgenerator-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reacnetgenerator-1.6.7.tar", last modified: Sat Nov  5 10:39:53 2022, max compression
+gzip compressed data, was "reacnetgenerator-1.6.8.tar", last modified: Sun Nov 13 23:00:48 2022, max compression
```

## Comparing `reacnetgenerator-1.6.7.tar` & `reacnetgenerator-1.6.8.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:53.000922 reacnetgenerator-1.6.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.980922 reacnetgenerator-1.6.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.984922 reacnetgenerator-1.6.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/.github/workflows/pyright.yml
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/.github/workflows/testjs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/.github/workflows/website.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3634 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/.github/workflows/wheel.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2652 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      962 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12553 2022-11-05 10:39:53.000922 reacnetgenerator-1.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.980922 reacnetgenerator-1.6.7/conda/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.984922 reacnetgenerator-1.6.7/conda/recipe/
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/conda/recipe/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.984922 reacnetgenerator-1.6.7/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.984922 reacnetgenerator-1.6.7/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.984922 reacnetgenerator-1.6.7/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)     1580 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/_static/reacnetgen.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5558 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/develop.rst
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/external.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.988922 reacnetgenerator-1.6.7/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/guide/build.md
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/guide/cli.md
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/guide/faq.md
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/guide/format.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/guide/gui.md
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/guide/hmm.md
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/guide/install.md
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/guide/python.md
--rw-r--r--   0 runner    (1001) docker     (121)     2181 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/guide/report.md
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/guide/run.md
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/overall.md
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/references.rst
--rw-r--r--   0 runner    (1001) docker     (121)    15988 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/refs.bib
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.988922 reacnetgenerator-1.6.7/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (121)    11821 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/tutorial/analysis.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/tutorial/cl20.md
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12791 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/tutorial/install.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     5620 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/docs/tutorial/methane.md
--rw-r--r--   0 runner    (1001) docker     (121)     3430 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.992922 reacnetgenerator-1.6.7/reacnetgenerator/
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15960 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/_detect.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/_download.py
--rw-r--r--   0 runner    (1001) docker     (121)     5223 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/_draw.py
--rw-r--r--   0 runner    (1001) docker     (121)     4543 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/_hmmfilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     5511 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1783 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/_mergeiso.py
--rw-r--r--   0 runner    (1001) docker     (121)    12194 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/_path.py
--rw-r--r--   0 runner    (1001) docker     (121)     6658 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/_reachtml.py
--rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/_reaction.py
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-05 10:39:52.000000 reacnetgenerator-1.6.7/reacnetgenerator/_version2.py
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/c_stack.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/c_stack.h
--rw-r--r--   0 runner    (1001) docker     (121)     5541 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/commandline.py
--rw-r--r--   0 runner    (1001) docker     (121)     3250 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/dps.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     4859 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/gui.py
--rw-r--r--   0 runner    (1001) docker     (121)    13467 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/reacnetgen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.992922 reacnetgenerator-1.6.7/reacnetgenerator/static/
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/img-title.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.996922 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.980922 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/.yarn/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.996922 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/.yarn/releases/
--rwxr-xr-x   0 runner    (1001) docker     (121)  2194904 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/.yarn/releases/yarn-3.2.4.cjs
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/.yarnrc.yml
--rw-r--r--   0 runner    (1001) docker     (121)    31895 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/fire.png
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/formula.js
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/package.json
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/reacnetgen.css
--rw-r--r--   0 runner    (1001) docker     (121)    10872 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/reacnetgen.js
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/reacnetgen.scss
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/reacnetgen_web.scss
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/select.js
--rw-r--r--   0 runner    (1001) docker     (121)    10751 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/template.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:53.000922 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/test/
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/test/test_formula.js
--rw-r--r--   0 runner    (1001) docker     (121)     5178 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (121)   153109 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/yarn.lock
--rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    15881 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/reacnetgenerator/utils_np.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:52.992922 reacnetgenerator-1.6.7/reacnetgenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12553 2022-11-05 10:39:52.000000 reacnetgenerator-1.6.7/reacnetgenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2802 2022-11-05 10:39:52.000000 reacnetgenerator-1.6.7/reacnetgenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-05 10:39:52.000000 reacnetgenerator-1.6.7/reacnetgenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-05 10:39:52.000000 reacnetgenerator-1.6.7/reacnetgenerator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-11-05 10:39:52.000000 reacnetgenerator-1.6.7/reacnetgenerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-05 10:39:52.000000 reacnetgenerator-1.6.7/reacnetgenerator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/renovate.json
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-05 10:39:53.000922 reacnetgenerator-1.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2643 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:53.000922 reacnetgenerator-1.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 10:39:53.000922 reacnetgenerator-1.6.7/tests/inputs/
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/tests/inputs/water.bond
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/tests/inputs/water.dump
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/tests/inputs/water.xyz
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/tests/inputs/water_pbc.dump
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/tests/methane.reactionabcd
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/tests/methane.species
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/tests/test.json
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/tests/test_detect.py
--rw-r--r--   0 runner    (1001) docker     (121)     4817 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/tests/test_reacnetgen.py
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-11-05 10:39:35.000000 reacnetgenerator-1.6.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.802124 reacnetgenerator-1.6.8/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.782124 reacnetgenerator-1.6.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.786124 reacnetgenerator-1.6.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2180 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/.github/workflows/pyright.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/.github/workflows/testjs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/.github/workflows/website.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/.github/workflows/wheel.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2652 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      962 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    12553 2022-11-13 23:00:48.802124 reacnetgenerator-1.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1989 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.782124 reacnetgenerator-1.6.8/conda/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.786124 reacnetgenerator-1.6.8/conda/recipe/
+-rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/conda/recipe/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.790124 reacnetgenerator-1.6.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.790124 reacnetgenerator-1.6.8/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.790124 reacnetgenerator-1.6.8/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (121)     1580 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/_static/reacnetgen.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     5558 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/develop.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/external.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.790124 reacnetgenerator-1.6.8/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/guide/build.md
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/guide/cli.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/guide/faq.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/guide/format.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/guide/gui.md
+-rw-r--r--   0 runner    (1001) docker     (121)      355 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/guide/hmm.md
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/guide/install.md
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/guide/python.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2181 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/guide/report.md
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/guide/run.md
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)     1727 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/overall.md
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/references.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    15988 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/refs.bib
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.790124 reacnetgenerator-1.6.8/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (121)    11821 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/tutorial/analysis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     2607 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/tutorial/cl20.md
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12791 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/tutorial/install.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     5620 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/docs/tutorial/methane.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3430 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.794124 reacnetgenerator-1.6.8/reacnetgenerator/
+-rw-r--r--   0 runner    (1001) docker     (121)      953 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15960 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/_detect.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/_download.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5223 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/_draw.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4543 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/_hmmfilter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5511 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1783 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/_mergeiso.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12194 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6658 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/_reachtml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-13 23:00:48.000000 reacnetgenerator-1.6.8/reacnetgenerator/_version2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      569 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/c_stack.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/c_stack.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5541 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/commandline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3250 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/dps.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     4859 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/gui.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13467 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/reacnetgen.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.794124 reacnetgenerator-1.6.8/reacnetgenerator/static/
+-rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/img-title.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.798124 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.786124 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/.yarn/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.798124 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/.yarn/releases/
+-rwxr-xr-x   0 runner    (1001) docker     (121)  2194904 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/.yarn/releases/yarn-3.2.4.cjs
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/.yarnrc.yml
+-rw-r--r--   0 runner    (1001) docker     (121)    31895 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/fire.png
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/formula.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/package.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/reacnetgen.css
+-rw-r--r--   0 runner    (1001) docker     (121)    10872 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/reacnetgen.js
+-rw-r--r--   0 runner    (1001) docker     (121)      269 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/reacnetgen.scss
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/reacnetgen_web.scss
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/select.js
+-rw-r--r--   0 runner    (1001) docker     (121)    10751 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/template.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.802124 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/test/test_formula.js
+-rw-r--r--   0 runner    (1001) docker     (121)     5178 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (121)   153461 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/yarn.lock
+-rw-r--r--   0 runner    (1001) docker     (121)     4526 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15881 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/reacnetgenerator/utils_np.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.794124 reacnetgenerator-1.6.8/reacnetgenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12553 2022-11-13 23:00:48.000000 reacnetgenerator-1.6.8/reacnetgenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2802 2022-11-13 23:00:48.000000 reacnetgenerator-1.6.8/reacnetgenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-13 23:00:48.000000 reacnetgenerator-1.6.8/reacnetgenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-13 23:00:48.000000 reacnetgenerator-1.6.8/reacnetgenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      417 2022-11-13 23:00:48.000000 reacnetgenerator-1.6.8/reacnetgenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-13 23:00:48.000000 reacnetgenerator-1.6.8/reacnetgenerator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-13 23:00:48.802124 reacnetgenerator-1.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2643 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.802124 reacnetgenerator-1.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 23:00:48.802124 reacnetgenerator-1.6.8/tests/inputs/
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/tests/inputs/water.bond
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/tests/inputs/water.dump
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/tests/inputs/water.xyz
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/tests/inputs/water_pbc.dump
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/tests/methane.reactionabcd
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/tests/methane.species
+-rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/tests/test.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/tests/test_detect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4817 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/tests/test_reacnetgen.py
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2022-11-13 23:00:29.000000 reacnetgenerator-1.6.8/tox.ini
```

### Comparing `reacnetgenerator-1.6.7/.github/workflows/codeql-analysis.yml` & `reacnetgenerator-1.6.8/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/.github/workflows/docker-publish.yml` & `reacnetgenerator-1.6.8/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/.github/workflows/push.yml` & `reacnetgenerator-1.6.8/.github/workflows/push.yml`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/.github/workflows/testjs.yml` & `reacnetgenerator-1.6.8/.github/workflows/testjs.yml`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/.github/workflows/website.yml` & `reacnetgenerator-1.6.8/.github/workflows/website.yml`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/.github/workflows/wheel.yml` & `reacnetgenerator-1.6.8/.github/workflows/wheel.yml`

 * *Files 17% similar despite different names*

```diff
@@ -34,41 +34,24 @@
             platform_id: manylinux_x86_64
           # macos-x86-64
           - os: macos-latest
             python: 37
             platform_id: macosx_x86_64
           - os: macos-latest
             python: 38
-            platform_id: macosx_x86_64
-          - os: macos-latest
-            python: 39
-            platform_id: macosx_x86_64
-          - os: macos-latest
-            python: 310
-            platform_id: macosx_x86_64
-          - os: macos-latest
-            python: 311
-            platform_id: macosx_x86_64
-          # macos-arm64
-          - os: macos-latest
-            bitness: 64
-            python: 38
-            platform_id: macosx_arm64
+            platform_id: macosx_universal2
           - os: macos-latest
-            bitness: 64
             python: 39
-            platform_id: macosx_arm64
+            platform_id: macosx_universal2
           - os: macos-latest
-            bitness: 64
             python: 310
-            platform_id: macosx_arm64
+            platform_id: macosx_universal2
           - os: macos-latest
-            bitness: 64
             python: 311
-            platform_id: macosx_arm64
+            platform_id: macosx_universal2
           # win-64
           - os: windows-2019
             python: 37
             platform_id: win_amd64
           - os: windows-2019
             python: 38
             platform_id: win_amd64
```

### Comparing `reacnetgenerator-1.6.7/.gitignore` & `reacnetgenerator-1.6.8/.gitignore`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/CITATION.cff` & `reacnetgenerator-1.6.8/CITATION.cff`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/LICENSE` & `reacnetgenerator-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/PKG-INFO` & `reacnetgenerator-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reacnetgenerator
-Version: 1.6.7
+Version: 1.6.8
 Summary: ReacNetGenerator: An automatic reaction network generator for reactive molecular dynamics simulation.
 Author-email: Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `reacnetgenerator-1.6.7/README.md` & `reacnetgenerator-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/conda/recipe/meta.yaml` & `reacnetgenerator-1.6.8/conda/recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/Makefile` & `reacnetgenerator-1.6.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/_static/css/custom.css` & `reacnetgenerator-1.6.8/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/_static/reacnetgen.svg` & `reacnetgenerator-1.6.8/docs/_static/reacnetgen.svg`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/conf.py` & `reacnetgenerator-1.6.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/guide/build.md` & `reacnetgenerator-1.6.8/docs/guide/build.md`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/guide/faq.md` & `reacnetgenerator-1.6.8/docs/guide/faq.md`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/guide/format.md` & `reacnetgenerator-1.6.8/docs/guide/format.md`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/guide/install.md` & `reacnetgenerator-1.6.8/docs/guide/install.md`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/guide/python.md` & `reacnetgenerator-1.6.8/docs/guide/python.md`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/guide/report.md` & `reacnetgenerator-1.6.8/docs/guide/report.md`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/guide/run.md` & `reacnetgenerator-1.6.8/docs/guide/run.md`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/make.bat` & `reacnetgenerator-1.6.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/overall.md` & `reacnetgenerator-1.6.8/docs/overall.md`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/refs.bib` & `reacnetgenerator-1.6.8/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/tutorial/analysis.ipynb` & `reacnetgenerator-1.6.8/docs/tutorial/analysis.ipynb`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/tutorial/cl20.md` & `reacnetgenerator-1.6.8/docs/tutorial/cl20.md`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/tutorial/install.ipynb` & `reacnetgenerator-1.6.8/docs/tutorial/install.ipynb`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/docs/tutorial/methane.md` & `reacnetgenerator-1.6.8/docs/tutorial/methane.md`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/pyproject.toml` & `reacnetgenerator-1.6.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/__init__.py` & `reacnetgenerator-1.6.8/reacnetgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/_detect.py` & `reacnetgenerator-1.6.8/reacnetgenerator/_detect.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/_draw.py` & `reacnetgenerator-1.6.8/reacnetgenerator/_draw.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/_hmmfilter.py` & `reacnetgenerator-1.6.8/reacnetgenerator/_hmmfilter.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/_matrix.py` & `reacnetgenerator-1.6.8/reacnetgenerator/_matrix.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/_mergeiso.py` & `reacnetgenerator-1.6.8/reacnetgenerator/_mergeiso.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/_path.py` & `reacnetgenerator-1.6.8/reacnetgenerator/_path.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/_reachtml.py` & `reacnetgenerator-1.6.8/reacnetgenerator/_reachtml.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/_reaction.py` & `reacnetgenerator-1.6.8/reacnetgenerator/_reaction.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/c_stack.cpp` & `reacnetgenerator-1.6.8/reacnetgenerator/c_stack.cpp`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/commandline.py` & `reacnetgenerator-1.6.8/reacnetgenerator/commandline.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/dps.pyx` & `reacnetgenerator-1.6.8/reacnetgenerator/dps.pyx`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/gui.py` & `reacnetgenerator-1.6.8/reacnetgenerator/gui.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/reacnetgen.py` & `reacnetgenerator-1.6.8/reacnetgenerator/reacnetgen.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/static/img-title.png` & `reacnetgenerator-1.6.8/reacnetgenerator/static/img-title.png`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/.yarn/releases/yarn-3.2.4.cjs` & `reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/.yarn/releases/yarn-3.2.4.cjs`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/fire.png` & `reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/fire.png`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/formula.js` & `reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/formula.js`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/package.json` & `reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930735930735931%*

 * *Differences: {"'dependencies'": "{'jsrender': '1.0.12'}",*

 * * "'devDependencies'": "{'css-loader': '6.7.2', 'postcss': '8.4.19', 'sass': '1.56.1', "*

 * *                      "'sass-loader': '13.2.0', 'webpack': '5.75.0'}"}*

```diff
@@ -4,44 +4,44 @@
         "@njzjz/jsnetworkx": "0.3.5",
         "@popperjs/core": "2.11.6",
         "animejs": "3.2.1",
         "bootstrap": "5.2.2",
         "bootstrap-select": "1.14.0-beta3",
         "d3": "3.5.17",
         "jquery": "3.6.1",
-        "jsrender": "1.0.11",
+        "jsrender": "1.0.12",
         "magnific-popup": "1.1.0",
         "paginationjs": "2.1.5",
         "popper.js": "1.16.1",
         "query-string": "7.1.1",
         "regenerator-runtime": "0.13.10",
         "smiles-drawer": "2.0.3",
         "startbootstrap-creative": "7.0.6"
     },
     "description": "JavaScript files for reacnetgenerator.",
     "devDependencies": {
-        "css-loader": "6.7.1",
+        "css-loader": "6.7.2",
         "css-minimizer-webpack-plugin": "4.2.2",
         "cssnano": "5.1.14",
         "cssnano-preset-advanced": "5.3.9",
         "html-inline-css-webpack-plugin": "1.11.1",
         "html-webpack-plugin": "5.5.0",
         "ifdef-loader": "2.3.2",
         "mini-css-extract-plugin": "2.6.1",
-        "postcss": "8.4.18",
+        "postcss": "8.4.19",
         "postcss-import": "15.0.0",
         "postcss-loader": "7.0.1",
-        "sass": "1.56.0",
-        "sass-loader": "13.1.0",
+        "sass": "1.56.1",
+        "sass-loader": "13.2.0",
         "script-ext-html-webpack-plugin": "2.1.5",
         "string-replace-webpack-plugin": "0.1.3",
         "style-loader": "3.3.1",
         "terser-webpack-plugin": "5.3.6",
         "url-loader": "4.1.1",
-        "webpack": "5.74.0",
+        "webpack": "5.75.0",
         "webpack-cdn-plugin": "3.3.1",
         "webpack-cli": "4.10.0"
     },
     "engines": {
         "node": ">=10.x"
     },
     "keywords": [
```

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/reacnetgen.css` & `reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/reacnetgen.css`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/reacnetgen.js` & `reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/reacnetgen.js`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/select.js` & `reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/select.js`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/template.html` & `reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/template.html`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/webpack.config.js` & `reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/webpack.config.js`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/static/webpack/yarn.lock` & `reacnetgenerator-1.6.8/reacnetgenerator/static/webpack/yarn.lock`

 * *Files 2% similar despite different names*

```diff
@@ -51,25 +51,25 @@
   resolution: "@jest/schemas@npm:29.0.0"
   dependencies:
     "@sinclair/typebox": ^0.24.1
   checksum: 41355c78f09eb1097e57a3c5d0ca11c9099e235e01ea5fa4e3953562a79a6a9296c1d300f1ba50ca75236048829e056b00685cd2f1ff8285e56fd2ce01249acb
   languageName: node
   linkType: hard
 
-"@jest/types@npm:^29.2.1":
-  version: 29.2.1
-  resolution: "@jest/types@npm:29.2.1"
+"@jest/types@npm:^29.3.1":
+  version: 29.3.1
+  resolution: "@jest/types@npm:29.3.1"
   dependencies:
     "@jest/schemas": ^29.0.0
     "@types/istanbul-lib-coverage": ^2.0.0
     "@types/istanbul-reports": ^3.0.0
     "@types/node": "*"
     "@types/yargs": ^17.0.8
     chalk: ^4.0.0
-  checksum: a83f20727425179aa05974aa7553c307d207fbb6b7ae5ab1e37fbb6ba9b6655f26655301fc804f2545d33f4c4a6b59d41eed1737c005d2b83fce9e14841b4150
+  checksum: 6f9faf27507b845ff3839c1adc6dbd038d7046d03d37e84c9fc956f60718711a801a5094c7eeee6b39ccf42c0ab61347fdc0fa49ab493ae5a8efd2fd41228ee8
   languageName: node
   linkType: hard
 
 "@jridgewell/gen-mapping@npm:^0.3.0":
   version: 0.3.2
   resolution: "@jridgewell/gen-mapping@npm:0.3.2"
   dependencies:
@@ -187,20 +187,20 @@
     "@types/eslint": "*"
     "@types/estree": "*"
   checksum: ea6a9363e92f301cd3888194469f9ec9d0021fe0a397a97a6dd689e7545c75de0bd2153dfb13d3ab532853a278b6572c6f678ce846980669e41029d205653460
   languageName: node
   linkType: hard
 
 "@types/eslint@npm:*":
-  version: 8.4.9
-  resolution: "@types/eslint@npm:8.4.9"
+  version: 8.4.10
+  resolution: "@types/eslint@npm:8.4.10"
   dependencies:
     "@types/estree": "*"
     "@types/json-schema": "*"
-  checksum: 9eda34e000f1e09850f447d8d65b671f59153aa5b580aca5b95185cf42b047b9cfda86eea83a6295aa883931b769a79236ce439601be7ab4485be88ce77b69ad
+  checksum: 21e009ed9ed9bc8920fdafc6e11ff321c4538b4cc18a56fdd59dc5184ea7bbf363c71638c9bdb59fc1254dddcdd567485136ed68b0ee4750948d4e32cb79c689
   languageName: node
   linkType: hard
 
 "@types/estree@npm:*":
   version: 1.0.0
   resolution: "@types/estree@npm:1.0.0"
   checksum: 910d97fb7092c6738d30a7430ae4786a38542023c6302b95d46f49420b797f21619cdde11fa92b338366268795884111c2eb10356e4bd2c8ad5b92941e9e6443
@@ -250,17 +250,17 @@
   version: 7.0.11
   resolution: "@types/json-schema@npm:7.0.11"
   checksum: 527bddfe62db9012fccd7627794bd4c71beb77601861055d87e3ee464f2217c85fca7a4b56ae677478367bbd248dbde13553312b7d4dbc702a2f2bbf60c4018d
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
-  version: 18.11.8
-  resolution: "@types/node@npm:18.11.8"
-  checksum: 60b358f97c1a029722dc785811b217615ef20249c3fbde60a65869cfd7a5cd5b1872ee95c79c187ef70e5a078f4ac7670d2129803985268b1f021ad6e8040af8
+  version: 18.11.9
+  resolution: "@types/node@npm:18.11.9"
+  checksum: cc0aae109e9b7adefc32eecb838d6fad931663bb06484b5e9cbbbf74865c721b03d16fd8d74ad90e31dbe093d956a7c2c306ba5429ba0c00f3f7505103d7a496
   languageName: node
   linkType: hard
 
 "@types/parse-json@npm:^4.0.0":
   version: 4.0.0
   resolution: "@types/parse-json@npm:4.0.0"
   checksum: fd6bce2b674b6efc3db4c7c3d336bd70c90838e8439de639b909ce22f3720d21344f52427f1d9e57b265fcb7f6c018699b99e5e0c208a1a4823014269a6bf35b
@@ -895,17 +895,17 @@
     lodash.memoize: ^4.1.2
     lodash.uniq: ^4.5.0
   checksum: db2a229383b20d0529b6b589dde99d7b6cb56ba371366f58cbbfa2929c9f42c01f873e2b6ef641d4eda9f0b4118de77dbb2805814670bdad4234bf08e720b0b4
   languageName: node
   linkType: hard
 
 "caniuse-lite@npm:^1.0.0, caniuse-lite@npm:^1.0.30001400, caniuse-lite@npm:^1.0.30001426":
-  version: 1.0.30001427
-  resolution: "caniuse-lite@npm:1.0.30001427"
-  checksum: 7b21a7d1f10c07130cecb7e7c7c38fd031f3dbd49afaee53fa4bb07355f9765686cad14f6296fbb49838f525c35292278b2c5ee9109c363edea5e134514ab6bb
+  version: 1.0.30001431
+  resolution: "caniuse-lite@npm:1.0.30001431"
+  checksum: bc8ab55cd194e240152946b54bfaff7456180cc018674fc7ed134f4f502192405f6643f422feaa0a5e7cc02b5bac564cfac7771ac6d29f5d129482fcfe335ba1
   languageName: node
   linkType: hard
 
 "caseless@npm:~0.12.0":
   version: 0.12.0
   resolution: "caseless@npm:0.12.0"
   checksum: b43bd4c440aa1e8ee6baefee8063b4850fd0d7b378f6aabc796c9ec8cb26d27fb30b46885350777d9bd079c5256c0e1329ad0dc7c2817e0bb466810ebb353751
@@ -1135,29 +1135,29 @@
   resolution: "css-declaration-sorter@npm:6.3.1"
   peerDependencies:
     postcss: ^8.0.9
   checksum: ff0d9989ee21ec4c42430b9bb86c43f973ed5024d68f30edc1e3fb07a22828ce3c3e5b922019f2ccbff606722e43c407c5c76e3cddac523ac4afcb31e4b2601c
   languageName: node
   linkType: hard
 
-"css-loader@npm:6.7.1":
-  version: 6.7.1
-  resolution: "css-loader@npm:6.7.1"
+"css-loader@npm:6.7.2":
+  version: 6.7.2
+  resolution: "css-loader@npm:6.7.2"
   dependencies:
     icss-utils: ^5.1.0
-    postcss: ^8.4.7
+    postcss: ^8.4.18
     postcss-modules-extract-imports: ^3.0.0
     postcss-modules-local-by-default: ^4.0.0
     postcss-modules-scope: ^3.0.0
     postcss-modules-values: ^4.0.0
     postcss-value-parser: ^4.2.0
-    semver: ^7.3.5
+    semver: ^7.3.8
   peerDependencies:
     webpack: ^5.0.0
-  checksum: 170fdbc630a05a43679ef60fa97694766b568dbde37adccc0faafa964fc675f08b976bc68837bb73b61d60240e8d2cbcbf51540fe94ebc9dafc56e7c46ba5527
+  checksum: f3c980cc9c033a02e60df7e5a2f33a1e8c2c3dd552f017485d2d81b383be623ae8c4189404e7a4a7403b52744683ae4b516def0f7ccf125c2b198cb647e46543
   languageName: node
   linkType: hard
 
 "css-loader@npm:^0.9.1":
   version: 0.9.1
   resolution: "css-loader@npm:0.9.1"
   dependencies:
@@ -2183,25 +2183,25 @@
 "isstream@npm:~0.1.2":
   version: 0.1.2
   resolution: "isstream@npm:0.1.2"
   checksum: 1eb2fe63a729f7bdd8a559ab552c69055f4f48eb5c2f03724430587c6f450783c8f1cd936c1c952d0a927925180fcc892ebd5b174236cf1065d4bd5bdb37e963
   languageName: node
   linkType: hard
 
-"jest-util@npm:^29.2.1":
-  version: 29.2.1
-  resolution: "jest-util@npm:29.2.1"
+"jest-util@npm:^29.3.1":
+  version: 29.3.1
+  resolution: "jest-util@npm:29.3.1"
   dependencies:
-    "@jest/types": ^29.2.1
+    "@jest/types": ^29.3.1
     "@types/node": "*"
     chalk: ^4.0.0
     ci-info: ^3.2.0
     graceful-fs: ^4.2.9
     picomatch: ^2.2.3
-  checksum: 781bd14a65599d24b7449877020f4da32e8cb8fbc31c4e849c589ffde58f0eec27de9f690dba182e3ca369fe651c0bb9c307de29a0927d12777677ded56bafb8
+  checksum: f67c60f062b94d21cb60e84b3b812d64b7bfa81fe980151de5c17a74eb666042d0134e2e756d099b7606a1fcf1d633824d2e58197d01d76dde1e2dc00dfcd413
   languageName: node
   linkType: hard
 
 "jest-worker@npm:^27.4.5":
   version: 27.5.1
   resolution: "jest-worker@npm:27.5.1"
   dependencies:
@@ -2209,22 +2209,22 @@
     merge-stream: ^2.0.0
     supports-color: ^8.0.0
   checksum: 98cd68b696781caed61c983a3ee30bf880b5bd021c01d98f47b143d4362b85d0737f8523761e2713d45e18b4f9a2b98af1eaee77afade4111bb65c77d6f7c980
   languageName: node
   linkType: hard
 
 "jest-worker@npm:^29.1.2":
-  version: 29.2.1
-  resolution: "jest-worker@npm:29.2.1"
+  version: 29.3.1
+  resolution: "jest-worker@npm:29.3.1"
   dependencies:
     "@types/node": "*"
-    jest-util: ^29.2.1
+    jest-util: ^29.3.1
     merge-stream: ^2.0.0
     supports-color: ^8.0.0
-  checksum: 10365612fae02412376e963de9f069d854deaf5aec8ff818ce49c299cd0373256a387a2da68db8225fb0f18483f2cc9072a52d1846881d44b756b1e36bc7f4ed
+  checksum: 38687fcbdc2b7ddc70bbb5dfc703ae095b46b3c7f206d62ecdf5f4d16e336178e217302138f3b906125576bb1cfe4cfe8d43681276fa5899d138ed9422099fb3
   languageName: node
   linkType: hard
 
 "jquery@npm:3.6.1":
   version: 3.6.1
   resolution: "jquery@npm:3.6.1"
   checksum: 6177d866a74f1137cad800f142c7cdbd5ab19cd4282546f8bdb4890c9f933b1d542ab96f2aa15d007e43c98de7315b0513e849ec5359d3ac5640f720892fe547
@@ -2317,20 +2317,20 @@
     extsprintf: 1.3.0
     json-schema: 0.4.0
     verror: 1.10.0
   checksum: 2ad1b9fdcccae8b3d580fa6ced25de930eaa1ad154db21bbf8478a4d30bbbec7925b5f5ff29b933fba9412b16a17bd484a8da4fdb3663b5e27af95dd693bab2a
   languageName: node
   linkType: hard
 
-"jsrender@npm:1.0.11":
-  version: 1.0.11
-  resolution: "jsrender@npm:1.0.11"
+"jsrender@npm:1.0.12":
+  version: 1.0.12
+  resolution: "jsrender@npm:1.0.12"
   dependencies:
     through2: ^3.0.1
-  checksum: 38913a7179b6ef34145ed7ca8a5470df72f4416914e0881e7fa543b4fba6a2d2aee6f3bbeafa2011d3a36beffc2f86ead0a5f117f542d95b0f33fe2f0a129584
+  checksum: d80bd3a99d43c79b3883ad887ca8a46c069cdb1bed68260e9e8f9d87b2c2b91ea7f20e5fd1f06cf1352bdf976de1f32d00d02e6c9ed8abea928c45d0affb449f
   languageName: node
   linkType: hard
 
 "kind-of@npm:^6.0.2":
   version: 6.0.3
   resolution: "kind-of@npm:6.0.3"
   checksum: 3ab01e7b1d440b22fe4c31f23d8d38b4d9b91d9f291df683476576493d5dfd2e03848a8b05813dd0c3f0e835bc63f433007ddeceb71f05cb25c45ae1b19c6d3b
@@ -2374,21 +2374,21 @@
     json5: ^0.5.0
     object-assign: ^4.0.1
   checksum: 3045c83ef8b19d66d4c25e3245120c579883f473fe0d0559552f55502be913725c4d558a7c866191a74b19ef2af20b094afe3b144ae1e717ea4c245d52f60a09
   languageName: node
   linkType: hard
 
 "loader-utils@npm:^1.1.0":
-  version: 1.4.0
-  resolution: "loader-utils@npm:1.4.0"
+  version: 1.4.1
+  resolution: "loader-utils@npm:1.4.1"
   dependencies:
     big.js: ^5.2.2
     emojis-list: ^3.0.0
     json5: ^1.0.1
-  checksum: d150b15e7a42ac47d935c8b484b79e44ff6ab4c75df7cc4cb9093350cf014ec0b17bdb60c5d6f91a37b8b218bd63b973e263c65944f58ca2573e402b9a27e717
+  checksum: ea0b648cba0194e04a90aab6270619f0e35be009e33a443d9e642e93056cd49e6ca4c9678bd1c777a2392551bc5f4d0f24a87f5040608da1274aa84c6eebb502
   languageName: node
   linkType: hard
 
 "loader-utils@npm:^2.0.0":
   version: 2.0.3
   resolution: "loader-utils@npm:2.0.3"
   dependencies:
@@ -2444,17 +2444,17 @@
   dependencies:
     yallist: ^4.0.0
   checksum: f97f499f898f23e4585742138a22f22526254fdba6d75d41a1c2526b3b6cc5747ef59c5612ba7375f42aca4f8461950e925ba08c991ead0651b4918b7c978297
   languageName: node
   linkType: hard
 
 "lru-cache@npm:^7.7.1":
-  version: 7.14.0
-  resolution: "lru-cache@npm:7.14.0"
-  checksum: efdd329f2c1bb790b71d497c6c59272e6bc2d7dd060ba55fc136becd3dd31fc8346edb446275504d94cb60d3c8385dbf5267b79b23789e409b2bdf302d13f0d7
+  version: 7.14.1
+  resolution: "lru-cache@npm:7.14.1"
+  checksum: d72c6713c6a6d86836a7a6523b3f1ac6764768cca47ec99341c3e76db06aacd4764620e5e2cda719a36848785a52a70e531822dc2b33fb071fa709683746c104
   languageName: node
   linkType: hard
 
 "magnific-popup@npm:1.1.0":
   version: 1.1.0
   resolution: "magnific-popup@npm:1.1.0"
   checksum: 97ff185208d5fc3c49ba2f7b22d9353c1d21ca1a6daf07fae0ef07dda07281f174e3da0ad4e7f04c5f5cf332a611f0f64c3db444002d12f9de37ab14999f0a06
@@ -3373,15 +3373,26 @@
   resolution: "postcss-zindex@npm:5.1.0"
   peerDependencies:
     postcss: ^8.2.15
   checksum: 8581e0ee552622489dcb9fb9609a3ccc261a67a229ba91a70bd138fe102a2d04cedb14642b82b673d4cac7b559ef32574f2dafde2ff7816eecac024d231c5ead
   languageName: node
   linkType: hard
 
-"postcss@npm:8.4.18, postcss@npm:^8.4.17, postcss@npm:^8.4.7":
+"postcss@npm:8.4.19, postcss@npm:^8.4.18":
+  version: 8.4.19
+  resolution: "postcss@npm:8.4.19"
+  dependencies:
+    nanoid: ^3.3.4
+    picocolors: ^1.0.0
+    source-map-js: ^1.0.2
+  checksum: 62782723a385f92b7525f66d29614624de7c5643855423db3a5efd9287e677650300192749adddbbb6734cea9b1d5f5fd4f6ea00ca3f9a95dbbb88f835f5ca64
+  languageName: node
+  linkType: hard
+
+"postcss@npm:^8.4.17":
   version: 8.4.18
   resolution: "postcss@npm:8.4.18"
   dependencies:
     nanoid: ^3.3.4
     picocolors: ^1.0.0
     source-map-js: ^1.0.2
   checksum: 9349fd99849b2e3d2e134ff949b7770ecb12375f352723ce2bcc06167eba3850ea7844c1b191a85cd915d6a396b4e8ee9a5267e6cc5d8d003d0cbc7a97555d39
@@ -3462,43 +3473,43 @@
   resolution: "reacnetgenerator-js@workspace:."
   dependencies:
     "@njzjz/jsnetworkx": 0.3.5
     "@popperjs/core": 2.11.6
     animejs: 3.2.1
     bootstrap: 5.2.2
     bootstrap-select: 1.14.0-beta3
-    css-loader: 6.7.1
+    css-loader: 6.7.2
     css-minimizer-webpack-plugin: 4.2.2
     cssnano: 5.1.14
     cssnano-preset-advanced: 5.3.9
     d3: 3.5.17
     html-inline-css-webpack-plugin: 1.11.1
     html-webpack-plugin: 5.5.0
     ifdef-loader: 2.3.2
     jquery: 3.6.1
-    jsrender: 1.0.11
+    jsrender: 1.0.12
     magnific-popup: 1.1.0
     mini-css-extract-plugin: 2.6.1
     paginationjs: 2.1.5
     popper.js: 1.16.1
-    postcss: 8.4.18
+    postcss: 8.4.19
     postcss-import: 15.0.0
     postcss-loader: 7.0.1
     query-string: 7.1.1
     regenerator-runtime: 0.13.10
-    sass: 1.56.0
-    sass-loader: 13.1.0
+    sass: 1.56.1
+    sass-loader: 13.2.0
     script-ext-html-webpack-plugin: 2.1.5
     smiles-drawer: 2.0.3
     startbootstrap-creative: 7.0.6
     string-replace-webpack-plugin: 0.1.3
     style-loader: 3.3.1
     terser-webpack-plugin: 5.3.6
     url-loader: 4.1.1
-    webpack: 5.74.0
+    webpack: 5.75.0
     webpack-cdn-plugin: 3.3.1
     webpack-cli: 4.10.0
   languageName: unknown
   linkType: soft
 
 "read-cache@npm:^1.0.0":
   version: 1.0.0
@@ -3677,49 +3688,49 @@
 "safer-buffer@npm:>= 2.1.2 < 3.0.0, safer-buffer@npm:^2.0.2, safer-buffer@npm:^2.1.0, safer-buffer@npm:~2.1.0":
   version: 2.1.2
   resolution: "safer-buffer@npm:2.1.2"
   checksum: cab8f25ae6f1434abee8d80023d7e72b598cf1327164ddab31003c51215526801e40b66c5e65d658a0af1e9d6478cadcb4c745f4bd6751f97d8644786c0978b0
   languageName: node
   linkType: hard
 
-"sass-loader@npm:13.1.0":
-  version: 13.1.0
-  resolution: "sass-loader@npm:13.1.0"
+"sass-loader@npm:13.2.0":
+  version: 13.2.0
+  resolution: "sass-loader@npm:13.2.0"
   dependencies:
     klona: ^2.0.4
     neo-async: ^2.6.2
   peerDependencies:
     fibers: ">= 3.1.0"
-    node-sass: ^4.0.0 || ^5.0.0 || ^6.0.0 || ^7.0.0
+    node-sass: ^4.0.0 || ^5.0.0 || ^6.0.0 || ^7.0.0 || ^8.0.0
     sass: ^1.3.0
     sass-embedded: "*"
     webpack: ^5.0.0
   peerDependenciesMeta:
     fibers:
       optional: true
     node-sass:
       optional: true
     sass:
       optional: true
     sass-embedded:
       optional: true
-  checksum: 6b3b6c0e070a32c594001cee98c85a72afb6081c46d56a4283269e6c1802b0e26128bc8363fcd8d8c941abe1f9e441e3efcd401fcf3ef436e1f1fbeb6e0a1374
+  checksum: ed6cdb5f5508e1a8a020d1451160a5e94805d0c2a97be5719c6a44ed28a258b5f37a1478d01b9d545f269367ae91ccb88adc93bd6202bfd609dbe3193228d51e
   languageName: node
   linkType: hard
 
-"sass@npm:1.56.0":
-  version: 1.56.0
-  resolution: "sass@npm:1.56.0"
+"sass@npm:1.56.1":
+  version: 1.56.1
+  resolution: "sass@npm:1.56.1"
   dependencies:
     chokidar: ">=3.0.0 <4.0.0"
     immutable: ^4.0.0
     source-map-js: ">=0.6.2 <2.0.0"
   bin:
     sass: sass.js
-  checksum: 37fb48b838f7a12f3c3efbf27bfc5f2b7fba015ed4b11effe32bd9488e30e1d5cefcbfef1e5c5dbd95557889fe2c7ec72f33e898cfc76182ea34eae03b1a4fb1
+  checksum: 78e693e5992b149574c95d5adfe39ca3e5b97d80befa11191a20d1daa41fe201a98ac099beab726cd3095e2d2e7991a2c408ba0fcc3fa9f525879de7eee18dad
   languageName: node
   linkType: hard
 
 "schema-utils@npm:^3.0.0, schema-utils@npm:^3.1.0, schema-utils@npm:^3.1.1":
   version: 3.1.1
   resolution: "schema-utils@npm:3.1.1"
   dependencies:
@@ -3750,15 +3761,15 @@
   peerDependencies:
     html-webpack-plugin: ^3.0.0 || ^4.0.0
     webpack: ^1.0.0 || ^2.0.0 || ^3.0.0 || ^4.0.0
   checksum: 7a4a281fb78b2790c61ee41b6b5e11b1e145430e0531d16d026794dba7f4a60ddf744d041d7bfcb8543ad60d1db385d94d48a0dfc2962296b5ed0b37e45b0921
   languageName: node
   linkType: hard
 
-"semver@npm:^7.3.5, semver@npm:^7.3.7":
+"semver@npm:^7.3.5, semver@npm:^7.3.7, semver@npm:^7.3.8":
   version: 7.3.8
   resolution: "semver@npm:7.3.8"
   dependencies:
     lru-cache: ^6.0.0
   bin:
     semver: bin/semver.js
   checksum: ba9c7cbbf2b7884696523450a61fee1a09930d888b7a8d7579025ad93d459b2d1949ee5bbfeb188b2be5f4ac163544c5e98491ad6152df34154feebc2cc337c1
@@ -4096,24 +4107,24 @@
   version: 2.2.1
   resolution: "tapable@npm:2.2.1"
   checksum: 3b7a1b4d86fa940aad46d9e73d1e8739335efd4c48322cb37d073eb6f80f5281889bf0320c6d8ffcfa1a0dd5bfdbd0f9d037e252ef972aca595330538aac4d51
   languageName: node
   linkType: hard
 
 "tar@npm:^6.1.11, tar@npm:^6.1.2":
-  version: 6.1.11
-  resolution: "tar@npm:6.1.11"
+  version: 6.1.12
+  resolution: "tar@npm:6.1.12"
   dependencies:
     chownr: ^2.0.0
     fs-minipass: ^2.0.0
     minipass: ^3.0.0
     minizlib: ^2.1.1
     mkdirp: ^1.0.3
     yallist: ^4.0.0
-  checksum: a04c07bb9e2d8f46776517d4618f2406fb977a74d914ad98b264fc3db0fe8224da5bec11e5f8902c5b9bcb8ace22d95fbe3c7b36b8593b7dfc8391a25898f32f
+  checksum: 49d72e4420944e7ede2782d6b0826a6ede6cdab23c7de63470917e7a78166bc4d5b1a96279d3d79a85f1ba5a17cd37c0acbb3cbff19a07447691445b8b051c55
   languageName: node
   linkType: hard
 
 "terser-webpack-plugin@npm:5.3.6, terser-webpack-plugin@npm:^5.1.3":
   version: 5.3.6
   resolution: "terser-webpack-plugin@npm:5.3.6"
   dependencies:
@@ -4196,17 +4207,17 @@
   version: 1.14.1
   resolution: "tslib@npm:1.14.1"
   checksum: dbe628ef87f66691d5d2959b3e41b9ca0045c3ee3c7c7b906cc1e328b39f199bb1ad9e671c39025bd56122ac57dfbf7385a94843b1cc07c60a4db74795829acd
   languageName: node
   linkType: hard
 
 "tslib@npm:^2.0.3":
-  version: 2.4.0
-  resolution: "tslib@npm:2.4.0"
-  checksum: 8c4aa6a3c5a754bf76aefc38026134180c053b7bd2f81338cb5e5ebf96fefa0f417bff221592bf801077f5bf990562f6264fecbc42cd3309b33872cb6fc3b113
+  version: 2.4.1
+  resolution: "tslib@npm:2.4.1"
+  checksum: 19480d6e0313292bd6505d4efe096a6b31c70e21cf08b5febf4da62e95c265c8f571f7b36fcc3d1a17e068032f59c269fab3459d6cd3ed6949eafecf64315fca
   languageName: node
   linkType: hard
 
 "tunnel-agent@npm:^0.6.0":
   version: 0.6.0
   resolution: "tunnel-agent@npm:0.6.0"
   dependencies:
@@ -4381,17 +4392,17 @@
 "webpack-sources@npm:^3.2.3":
   version: 3.2.3
   resolution: "webpack-sources@npm:3.2.3"
   checksum: 989e401b9fe3536529e2a99dac8c1bdc50e3a0a2c8669cbafad31271eadd994bc9405f88a3039cd2e29db5e6d9d0926ceb7a1a4e7409ece021fe79c37d9c4607
   languageName: node
   linkType: hard
 
-"webpack@npm:5.74.0":
-  version: 5.74.0
-  resolution: "webpack@npm:5.74.0"
+"webpack@npm:5.75.0":
+  version: 5.75.0
+  resolution: "webpack@npm:5.75.0"
   dependencies:
     "@types/eslint-scope": ^3.7.3
     "@types/estree": ^0.0.51
     "@webassemblyjs/ast": 1.11.1
     "@webassemblyjs/wasm-edit": 1.11.1
     "@webassemblyjs/wasm-parser": 1.11.1
     acorn: ^8.7.1
@@ -4414,15 +4425,15 @@
     watchpack: ^2.4.0
     webpack-sources: ^3.2.3
   peerDependenciesMeta:
     webpack-cli:
       optional: true
   bin:
     webpack: bin/webpack.js
-  checksum: 320c41369a75051b19e18c63f408b3dcc481852e992f83d311771c5ec0f05f2946385e8ebef62030cf3587f0a3d2f12779ffdb191569a966847289ba7313f946
+  checksum: 2bcc5f3c195f375944e8af2f00bf2feea39cb9fda5f763b0d1b00077f1c51783db25c94d3fae96a07dead9fa085e6ae7474417e5ab31719c9776ea5969ceb83a
   languageName: node
   linkType: hard
 
 "which@npm:^2.0.1, which@npm:^2.0.2":
   version: 2.0.2
   resolution: "which@npm:2.0.2"
   dependencies:
```

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/tools.py` & `reacnetgenerator-1.6.8/reacnetgenerator/tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -74,15 +74,16 @@
             occs.append((int(s[0]), Counter(s[1].split('->')[0].split('+')), s[1]))
     return occs
 
 
 def calculate_rate(specfile: Union[str, Path], reacfile: Union[str, Path], cell: np.ndarray, timestep: float) -> Dict[str, float]:
     """Calculate the rate constant of each reaction.
 
-    The rate constants are calculated by the method developed in [1].
+    The rate constants are calculated by the method developed in [1]_.
+    The time interval of the trajectory is assumed to be uniform.
 
     Parameters
     ----------
     specfile : str
         The species file.
     reacfile : str
         The reactions file.
@@ -91,15 +92,15 @@
     timestep : float
         The time step. Unit: femtosecond.
 
     Returns
     -------
     rates : Dict[str, float]
         The rate of each reaction. The dict key is the reaction SMILES.
-        The value is in unit of [(cm^3/mol)s^(-1)].
+        The value is in unit of [(cm^3/mol)^(n-1)s^(-1)], where n is the reaction order.
 
     References
     ----------
     .. [1] Yanze Wu, Huai Sun, Liang Wu, Joshua D. Deetz, Extracting the mechanisms
        and kinetic models of complex reactions from atomistic simulation data, J.
        Comput. Chem. 40, 16, 1586-1592.
 
@@ -112,25 +113,25 @@
     ase_cell = ase.geometry.Cell(cell)
     
     timestep *= 10**-15 # fs to s
     #N, step_tot =read_species(specfile)
     step_idx, n_species = read_species(specfile)
     occs = read_reactions(reacfile)
 
-    # total time during simulation
-    time_tot = (step_idx[-1] - step_idx[0]) * timestep
+    # time interval between two frames
+    time_int = (step_idx[1] - step_idx[0]) * timestep
     # volume of the cell
     volume = ase_cell.volume
     volume *= 10**-24 # Ang^3 to cm^3
     volume_times_na = volume * ase.units.mol # V * NA
     
     rates = {}
     for occ, reacts, reactions in occs:
         # k = occ_tot / ( V * time_tot * c_tot )
         # c_tot = N_tot / (V * NA)
         n_react = np.array([n_species[kk] for kk in reacts.keys()])
         nu = np.array(list(reacts.values()))
         c_po = np.power(n_react / volume_times_na, np.repeat(nu, n_react.shape[1]).reshape(n_react.shape))
         c_tot = np.sum(np.prod(c_po, axis=0))
-        k = occ / (volume_times_na * time_tot * c_tot)
+        k = occ / (volume_times_na * time_int * c_tot)
         rates[reactions] = k
     return rates
```

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/utils.py` & `reacnetgenerator-1.6.8/reacnetgenerator/utils.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator/utils_np.pyx` & `reacnetgenerator-1.6.8/reacnetgenerator/utils_np.pyx`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator.egg-info/PKG-INFO` & `reacnetgenerator-1.6.8/reacnetgenerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reacnetgenerator
-Version: 1.6.7
+Version: 1.6.8
 Summary: ReacNetGenerator: An automatic reaction network generator for reactive molecular dynamics simulation.
 Author-email: Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `reacnetgenerator-1.6.7/reacnetgenerator.egg-info/SOURCES.txt` & `reacnetgenerator-1.6.8/reacnetgenerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/setup.py` & `reacnetgenerator-1.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/tests/methane.species` & `reacnetgenerator-1.6.8/tests/methane.species`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/tests/test.json` & `reacnetgenerator-1.6.8/tests/test.json`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/tests/test_detect.py` & `reacnetgenerator-1.6.8/tests/test_detect.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/tests/test_reacnetgen.py` & `reacnetgenerator-1.6.8/tests/test_reacnetgen.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/tests/test_tools.py` & `reacnetgenerator-1.6.8/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `reacnetgenerator-1.6.7/tox.ini` & `reacnetgenerator-1.6.8/tox.ini`

 * *Files identical despite different names*

