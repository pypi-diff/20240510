# Comparing `tmp/no_vtf-5.0.0.tar.gz` & `tmp/no_vtf-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "no_vtf-5.0.0.tar", last modified: Fri Feb 16 18:36:56 2024, max compression
+gzip compressed data, was "no_vtf-5.0.1.tar", last modified: Fri May 10 18:21:46 2024, max compression
```

## Comparing `no_vtf-5.0.0.tar` & `no_vtf-5.0.1.tar`

### file list

```diff
@@ -1,203 +1,204 @@
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.497448 no_vtf-5.0.0/
--rw-r--r--   0 build     (1000) build     (1000)     2046 2024-02-16 18:28:23.000000 no_vtf-5.0.0/.build.yml
--rw-r--r--   0 build     (1000) build     (1000)      367 2024-02-16 18:28:23.000000 no_vtf-5.0.0/.gitignore
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.477449 no_vtf-5.0.0/.reuse/
--rw-r--r--   0 build     (1000) build     (1000)      553 2024-02-16 18:28:23.000000 no_vtf-5.0.0/.reuse/dep5
--rw-r--r--   0 build     (1000) build     (1000)     6128 2024-02-16 18:28:23.000000 no_vtf-5.0.0/CONTRIBUTING.md
--rw-r--r--   0 build     (1000) build     (1000)       95 2024-02-16 18:28:23.000000 no_vtf-5.0.0/CONTRIBUTING.md.license
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.477449 no_vtf-5.0.0/LICENSES/
--rw-r--r--   0 build     (1000) build     (1000)    17023 2024-02-16 18:28:23.000000 no_vtf-5.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 build     (1000) build     (1000)     7048 2024-02-16 18:28:23.000000 no_vtf-5.0.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 build     (1000) build     (1000)    34674 2024-02-16 18:28:23.000000 no_vtf-5.0.0/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0 build     (1000) build     (1000)    34670 2024-02-16 18:28:23.000000 no_vtf-5.0.0/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 build     (1000) build     (1000)    42098 2024-02-16 18:28:23.000000 no_vtf-5.0.0/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 build     (1000) build     (1000)    27976 2024-02-16 18:28:23.000000 no_vtf-5.0.0/LICENSES/LicenseRef-WIN10SDK-RTM-AUG-2018.txt
--rw-r--r--   0 build     (1000) build     (1000)    18789 2024-02-16 18:28:23.000000 no_vtf-5.0.0/LICENSES/LicenseRef-mlt687465.txt
--rw-r--r--   0 build     (1000) build     (1000)      227 2024-02-16 18:28:23.000000 no_vtf-5.0.0/MANIFEST.in
--rw-r--r--   0 build     (1000) build     (1000)    11572 2024-02-16 18:36:56.497448 no_vtf-5.0.0/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)     9845 2024-02-16 18:28:23.000000 no_vtf-5.0.0/README.md
--rw-r--r--   0 build     (1000) build     (1000)       95 2024-02-16 18:28:23.000000 no_vtf-5.0.0/README.md.license
--rw-r--r--   0 build     (1000) build     (1000)      799 2024-02-16 18:28:23.000000 no_vtf-5.0.0/SECURITY.md
--rw-r--r--   0 build     (1000) build     (1000)       95 2024-02-16 18:28:23.000000 no_vtf-5.0.0/SECURITY.md.license
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.477449 no_vtf-5.0.0/builds/
--rw-r--r--   0 build     (1000) build     (1000)      589 2024-02-16 18:28:23.000000 no_vtf-5.0.0/builds/common
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.481449 no_vtf-5.0.0/builds/debian/
--rw-r--r--   0 build     (1000) build     (1000)      162 2024-02-16 18:28:23.000000 no_vtf-5.0.0/builds/debian/common
--rwxr-xr-x   0 build     (1000) build     (1000)      409 2024-02-16 18:28:23.000000 no_vtf-5.0.0/builds/debian/env.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      412 2024-02-16 18:28:23.000000 no_vtf-5.0.0/builds/debian/ksc-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      518 2024-02-16 18:28:23.000000 no_vtf-5.0.0/builds/debian/python3.10-build_dep.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      872 2024-02-16 18:28:23.000000 no_vtf-5.0.0/builds/debian/wine-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      199 2024-02-16 18:28:23.000000 no_vtf-5.0.0/builds/diff_generated.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      623 2024-02-16 18:28:23.000000 no_vtf-5.0.0/builds/nox.py
--rwxr-xr-x   0 build     (1000) build     (1000)      652 2024-02-16 18:28:23.000000 no_vtf-5.0.0/builds/publish_frozen.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      474 2024-02-16 18:28:23.000000 no_vtf-5.0.0/builds/python3.10-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      371 2024-02-16 18:28:23.000000 no_vtf-5.0.0/builds/verify_signatures.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      503 2024-02-16 18:28:23.000000 no_vtf-5.0.0/builds/with_clone.sh
--rwxr-xr-x   0 build     (1000) build     (1000)     1003 2024-02-16 18:28:23.000000 no_vtf-5.0.0/builds/with_wine.sh
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.481449 no_vtf-5.0.0/ksy/
--rwxr-xr-x   0 build     (1000) build     (1000)     6987 2024-02-16 18:28:23.000000 no_vtf-5.0.0/ksy/compile.py
--rw-r--r--   0 build     (1000) build     (1000)    10409 2024-02-16 18:28:23.000000 no_vtf-5.0.0/ksy/vtf.ksy
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.481449 no_vtf-5.0.0/no_vtf/
--rw-r--r--   0 build     (1000) build     (1000)      319 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      300 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/__main__.py
--rw-r--r--   0 build     (1000) build     (1000)     6076 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/_alive_progress.py
--rw-r--r--   0 build     (1000) build     (1000)     5298 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/_click.py
--rw-r--r--   0 build     (1000) build     (1000)      411 2024-02-16 18:36:56.000000 no_vtf-5.0.0/no_vtf/_version.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.481449 no_vtf-5.0.0/no_vtf/core/
--rw-r--r--   0 build     (1000) build     (1000)        0 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/__init__.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.481449 no_vtf-5.0.0/no_vtf/core/image/
--rw-r--r--   0 build     (1000) build     (1000)      525 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1725 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/channel_separator.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.481449 no_vtf-5.0.0/no_vtf/core/image/decoder/
--rw-r--r--   0 build     (1000) build     (1000)      178 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/decoder/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      422 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/decoder/decoder.py
--rw-r--r--   0 build     (1000) build     (1000)     3100 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/decoder/dxt.py
--rw-r--r--   0 build     (1000) build     (1000)      895 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/decoder/ndarray.py
--rw-r--r--   0 build     (1000) build     (1000)     6207 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/decoder/raw.py
--rw-r--r--   0 build     (1000) build     (1000)     2507 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/image.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.481449 no_vtf-5.0.0/no_vtf/core/image/io/
--rw-r--r--   0 build     (1000) build     (1000)      702 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/io/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     2289 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/io/file.py
--rw-r--r--   0 build     (1000) build     (1000)    14670 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/io/image.py
--rw-r--r--   0 build     (1000) build     (1000)     2925 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/io/io.py
--rw-r--r--   0 build     (1000) build     (1000)     1997 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/io/raw.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.485448 no_vtf-5.0.0/no_vtf/core/image/modifier/
--rw-r--r--   0 build     (1000) build     (1000)      337 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/modifier/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1838 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/modifier/fp_precision_modifier.py
--rw-r--r--   0 build     (1000) build     (1000)     2416 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/modifier/hdr_to_ldr_modifier.py
--rw-r--r--   0 build     (1000) build     (1000)      795 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/image/modifier/modifier.py
--rw-r--r--   0 build     (1000) build     (1000)    13544 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/pipeline.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.485448 no_vtf-5.0.0/no_vtf/core/texture/
--rw-r--r--   0 build     (1000) build     (1000)      202 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/texture/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      606 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/texture/decoder.py
--rw-r--r--   0 build     (1000) build     (1000)      573 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/texture/extractor.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.485448 no_vtf-5.0.0/no_vtf/core/texture/filter/
--rw-r--r--   0 build     (1000) build     (1000)      496 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/texture/filter/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1343 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/texture/filter/face.py
--rw-r--r--   0 build     (1000) build     (1000)      974 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/texture/filter/filter.py
--rw-r--r--   0 build     (1000) build     (1000)     1358 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/texture/filter/frame.py
--rw-r--r--   0 build     (1000) build     (1000)     1760 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/texture/filter/mipmap.py
--rw-r--r--   0 build     (1000) build     (1000)     2092 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/texture/filter/resolution.py
--rw-r--r--   0 build     (1000) build     (1000)     1358 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/texture/filter/slice.py
--rw-r--r--   0 build     (1000) build     (1000)      515 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/texture/namer.py
--rw-r--r--   0 build     (1000) build     (1000)      993 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/core/texture/texture.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.485448 no_vtf-5.0.0/no_vtf/filesystem/
--rw-r--r--   0 build     (1000) build     (1000)      253 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/filesystem/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     2102 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/filesystem/input_paths.py
--rw-r--r--   0 build     (1000) build     (1000)      998 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/filesystem/output_directories.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.485448 no_vtf-5.0.0/no_vtf/functional/
--rw-r--r--   0 build     (1000) build     (1000)      171 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/functional/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1425 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/functional/deferred.py
--rw-r--r--   0 build     (1000) build     (1000)    27529 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/main.py
--rw-r--r--   0 build     (1000) build     (1000)        0 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/py.typed
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.485448 no_vtf-5.0.0/no_vtf/task_runner/
--rw-r--r--   0 build     (1000) build     (1000)      302 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/task_runner/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     2121 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/task_runner/parallel.py
--rw-r--r--   0 build     (1000) build     (1000)      855 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/task_runner/sequential.py
--rw-r--r--   0 build     (1000) build     (1000)      956 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/task_runner/task_runner.py
--rw-r--r--   0 build     (1000) build     (1000)      422 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/typing.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.485448 no_vtf-5.0.0/no_vtf/vtf/
--rw-r--r--   0 build     (1000) build     (1000)      412 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/vtf/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     5590 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/vtf/extractor.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.485448 no_vtf-5.0.0/no_vtf/vtf/generated/
--rw-r--r--   0 build     (1000) build     (1000)        0 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/vtf/generated/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)    23014 2024-02-16 18:32:53.000000 no_vtf-5.0.0/no_vtf/vtf/generated/parser.py
--rw-r--r--   0 build     (1000) build     (1000)       93 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/vtf/generated/parser.py.license
--rw-r--r--   0 build     (1000) build     (1000)     2939 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/vtf/image_decoder.py
--rw-r--r--   0 build     (1000) build     (1000)     1351 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/vtf/namer.py
--rw-r--r--   0 build     (1000) build     (1000)     1043 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/vtf/texture.py
--rw-r--r--   0 build     (1000) build     (1000)     4612 2024-02-16 18:28:23.000000 no_vtf-5.0.0/no_vtf/vtf/texture_decoder.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.497448 no_vtf-5.0.0/no_vtf.egg-info/
--rw-r--r--   0 build     (1000) build     (1000)    11572 2024-02-16 18:36:56.000000 no_vtf-5.0.0/no_vtf.egg-info/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)     7060 2024-02-16 18:36:56.000000 no_vtf-5.0.0/no_vtf.egg-info/SOURCES.txt
--rw-r--r--   0 build     (1000) build     (1000)        1 2024-02-16 18:36:56.000000 no_vtf-5.0.0/no_vtf.egg-info/dependency_links.txt
--rw-r--r--   0 build     (1000) build     (1000)       49 2024-02-16 18:36:56.000000 no_vtf-5.0.0/no_vtf.egg-info/entry_points.txt
--rw-r--r--   0 build     (1000) build     (1000)        1 2024-02-16 18:32:19.000000 no_vtf-5.0.0/no_vtf.egg-info/not-zip-safe
--rw-r--r--   0 build     (1000) build     (1000)      209 2024-02-16 18:36:56.000000 no_vtf-5.0.0/no_vtf.egg-info/requires.txt
--rw-r--r--   0 build     (1000) build     (1000)        7 2024-02-16 18:36:56.000000 no_vtf-5.0.0/no_vtf.egg-info/top_level.txt
--rw-r--r--   0 build     (1000) build     (1000)    42273 2024-02-16 18:28:23.000000 no_vtf-5.0.0/noxfile.py
--rw-r--r--   0 build     (1000) build     (1000)     1193 2024-02-16 18:28:23.000000 no_vtf-5.0.0/pyproject.toml
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.473449 no_vtf-5.0.0/resources/
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.489448 no_vtf-5.0.0/resources/docs/
--rw-r--r--   0 build     (1000) build     (1000)   123671 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/docs/screencast.gif
--rw-r--r--   0 build     (1000) build     (1000)       95 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/docs/screencast.gif.license
--rw-r--r--   0 build     (1000) build     (1000)  1009090 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/docs/screencast_v4.gif
--rw-r--r--   0 build     (1000) build     (1000)       95 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/docs/screencast_v4.gif.license
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.489448 no_vtf-5.0.0/resources/pyinstaller/
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.489448 no_vtf-5.0.0/resources/pyinstaller/common/
--rw-r--r--   0 build     (1000) build     (1000)     2005 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/common/COPYING.md
--rw-r--r--   0 build     (1000) build     (1000)      163 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/common/COPYING.md.license
--rw-r--r--   0 build     (1000) build     (1000)        6 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/empty.ico
--rw-r--r--   0 build     (1000) build     (1000)       93 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/empty.ico.license
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.473449 no_vtf-5.0.0/resources/pyinstaller/nt/
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.489448 no_vtf-5.0.0/resources/pyinstaller/nt/.reuse/
--rw-r--r--   0 build     (1000) build     (1000)     2029 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/.reuse/dep5
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.497448 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/
--rw-r--r--   0 build     (1000) build     (1000)    21032 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-console-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21024 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-console-l1-2-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    20512 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-datetime-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    20544 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-debug-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    20520 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-errorhandling-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    24104 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-file-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    20520 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-file-l1-2-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    20520 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-file-l2-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    20520 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-handle-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21032 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-heap-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    20520 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-interlocked-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21568 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-libraryloader-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    23080 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-localization-l1-2-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21032 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-memory-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    20520 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-namedpipe-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21544 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-processenvironment-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    22560 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-processthreads-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21056 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-processthreads-l1-1-1.dll
--rw-r--r--   0 build     (1000) build     (1000)    20008 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-profile-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21056 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-rtlsupport-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    20520 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-string-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    22568 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-synch-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21032 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-synch-l1-2-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21544 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-sysinfo-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21032 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-timezone-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    20520 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-util-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21544 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-conio-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    24616 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-convert-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21032 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-environment-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    22568 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-filesystem-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21544 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-heap-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21032 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-locale-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    29528 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-math-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    28736 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-multibyte-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    73048 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-private-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21568 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-process-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    25128 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-runtime-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    26664 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-stdio-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    26664 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-string-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    23080 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-time-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)    21032 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-utility-l1-1-0.dll
--rw-r--r--   0 build     (1000) build     (1000)  1026088 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/ucrtbase.dll
--rw-r--r--   0 build     (1000) build     (1000)   154392 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/nt/_internal/vcomp140.dll
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.497448 no_vtf-5.0.0/resources/pyinstaller/posix/
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.497448 no_vtf-5.0.0/resources/pyinstaller/posix/.reuse/
--rw-r--r--   0 build     (1000) build     (1000)     5070 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/.reuse/dep5
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.497448 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/
--rw-r--r--   0 build     (1000) build     (1000)     1891 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-bzip2.txt
--rw-r--r--   0 build     (1000) build     (1000)     8616 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-fontconfig.txt
--rw-r--r--   0 build     (1000) build     (1000)    46458 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libX11.txt
--rw-r--r--   0 build     (1000) build     (1000)     1148 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libXau.txt
--rw-r--r--   0 build     (1000) build     (1000)     1178 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libXdmcp.txt
--rw-r--r--   0 build     (1000) build     (1000)    11101 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libXext.txt
--rw-r--r--   0 build     (1000) build     (1000)     1105 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libXft.txt
--rw-r--r--   0 build     (1000) build     (1000)     2164 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libXrender.txt
--rw-r--r--   0 build     (1000) build     (1000)     2591 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libXss.txt
--rw-r--r--   0 build     (1000) build     (1000)    23963 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libbsd.txt
--rw-r--r--   0 build     (1000) build     (1000)     8018 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libmd.txt
--rw-r--r--   0 build     (1000) build     (1000)     5345 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libpng.txt
--rw-r--r--   0 build     (1000) build     (1000)     1139 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libtiff.txt
--rw-r--r--   0 build     (1000) build     (1000)     1337 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libxcb.txt
--rw-r--r--   0 build     (1000) build     (1000)     2775 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-xz.txt
--rwxr-xr-x   0 build     (1000) build     (1000)      494 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/pyinstaller/posix/no_vtf.desktop
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.473449 no_vtf-5.0.0/resources/test/
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-02-16 18:36:56.497448 no_vtf-5.0.0/resources/test/samples/
--rw-r--r--   0 build     (1000) build     (1000)      264 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/test/samples/CONTENTS
--rw-r--r--   0 build     (1000) build     (1000)       93 2024-02-16 18:28:23.000000 no_vtf-5.0.0/resources/test/samples/CONTENTS.license
--rw-r--r--   0 build     (1000) build     (1000)     2587 2024-02-16 18:36:56.501448 no_vtf-5.0.0/setup.cfg
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.935999 no_vtf-5.0.1/
+-rw-r--r--   0 build     (1000) build     (1000)     2046 2024-05-10 18:14:21.000000 no_vtf-5.0.1/.build.yml
+-rw-r--r--   0 build     (1000) build     (1000)      367 2024-05-10 18:14:21.000000 no_vtf-5.0.1/.gitignore
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.915999 no_vtf-5.0.1/.reuse/
+-rw-r--r--   0 build     (1000) build     (1000)      553 2024-05-10 18:14:21.000000 no_vtf-5.0.1/.reuse/dep5
+-rw-r--r--   0 build     (1000) build     (1000)     6128 2024-05-10 18:14:21.000000 no_vtf-5.0.1/CONTRIBUTING.md
+-rw-r--r--   0 build     (1000) build     (1000)       95 2024-05-10 18:14:21.000000 no_vtf-5.0.1/CONTRIBUTING.md.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.915999 no_vtf-5.0.1/LICENSES/
+-rw-r--r--   0 build     (1000) build     (1000)    17023 2024-05-10 18:14:21.000000 no_vtf-5.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 build     (1000) build     (1000)     7048 2024-05-10 18:14:21.000000 no_vtf-5.0.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 build     (1000) build     (1000)    34674 2024-05-10 18:14:21.000000 no_vtf-5.0.1/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0 build     (1000) build     (1000)    34670 2024-05-10 18:14:21.000000 no_vtf-5.0.1/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 build     (1000) build     (1000)    42098 2024-05-10 18:14:21.000000 no_vtf-5.0.1/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 build     (1000) build     (1000)    27976 2024-05-10 18:14:21.000000 no_vtf-5.0.1/LICENSES/LicenseRef-WIN10SDK-RTM-AUG-2018.txt
+-rw-r--r--   0 build     (1000) build     (1000)    18789 2024-05-10 18:14:21.000000 no_vtf-5.0.1/LICENSES/LicenseRef-mlt687465.txt
+-rw-r--r--   0 build     (1000) build     (1000)      227 2024-05-10 18:14:21.000000 no_vtf-5.0.1/MANIFEST.in
+-rw-r--r--   0 build     (1000) build     (1000)    12010 2024-05-10 18:21:46.935999 no_vtf-5.0.1/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)    10291 2024-05-10 18:14:21.000000 no_vtf-5.0.1/README.md
+-rw-r--r--   0 build     (1000) build     (1000)       95 2024-05-10 18:14:21.000000 no_vtf-5.0.1/README.md.license
+-rw-r--r--   0 build     (1000) build     (1000)      799 2024-05-10 18:14:21.000000 no_vtf-5.0.1/SECURITY.md
+-rw-r--r--   0 build     (1000) build     (1000)       95 2024-05-10 18:14:21.000000 no_vtf-5.0.1/SECURITY.md.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.915999 no_vtf-5.0.1/builds/
+-rw-r--r--   0 build     (1000) build     (1000)      589 2024-05-10 18:14:21.000000 no_vtf-5.0.1/builds/common
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.919999 no_vtf-5.0.1/builds/debian/
+-rw-r--r--   0 build     (1000) build     (1000)      162 2024-05-10 18:14:21.000000 no_vtf-5.0.1/builds/debian/common
+-rwxr-xr-x   0 build     (1000) build     (1000)      409 2024-05-10 18:14:21.000000 no_vtf-5.0.1/builds/debian/env.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      412 2024-05-10 18:14:21.000000 no_vtf-5.0.1/builds/debian/ksc-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      518 2024-05-10 18:14:21.000000 no_vtf-5.0.1/builds/debian/python3.10-build_dep.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      872 2024-05-10 18:14:21.000000 no_vtf-5.0.1/builds/debian/wine-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      199 2024-05-10 18:14:21.000000 no_vtf-5.0.1/builds/diff_generated.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      647 2024-05-10 18:14:21.000000 no_vtf-5.0.1/builds/nox.py
+-rwxr-xr-x   0 build     (1000) build     (1000)      652 2024-05-10 18:14:21.000000 no_vtf-5.0.1/builds/publish_frozen.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      474 2024-05-10 18:14:21.000000 no_vtf-5.0.1/builds/python3.10-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      675 2024-05-10 18:14:21.000000 no_vtf-5.0.1/builds/verify_signatures.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      503 2024-05-10 18:14:21.000000 no_vtf-5.0.1/builds/with_clone.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)     1003 2024-05-10 18:14:21.000000 no_vtf-5.0.1/builds/with_wine.sh
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.919999 no_vtf-5.0.1/ksy/
+-rwxr-xr-x   0 build     (1000) build     (1000)     7011 2024-05-10 18:14:21.000000 no_vtf-5.0.1/ksy/compile.py
+-rw-r--r--   0 build     (1000) build     (1000)    10409 2024-05-10 18:14:21.000000 no_vtf-5.0.1/ksy/vtf.ksy
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.919999 no_vtf-5.0.1/no_vtf/
+-rw-r--r--   0 build     (1000) build     (1000)      319 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      300 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/__main__.py
+-rw-r--r--   0 build     (1000) build     (1000)     6076 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/_alive_progress.py
+-rw-r--r--   0 build     (1000) build     (1000)     5298 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/_click.py
+-rw-r--r--   0 build     (1000) build     (1000)    15537 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/_main.py
+-rw-r--r--   0 build     (1000) build     (1000)      411 2024-05-10 18:21:46.000000 no_vtf-5.0.1/no_vtf/_version.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.919999 no_vtf-5.0.1/no_vtf/core/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/__init__.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.919999 no_vtf-5.0.1/no_vtf/core/image/
+-rw-r--r--   0 build     (1000) build     (1000)      525 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1725 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/channel_separator.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.919999 no_vtf-5.0.1/no_vtf/core/image/decoder/
+-rw-r--r--   0 build     (1000) build     (1000)      178 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/decoder/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      422 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/decoder/decoder.py
+-rw-r--r--   0 build     (1000) build     (1000)     3100 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/decoder/dxt.py
+-rw-r--r--   0 build     (1000) build     (1000)      895 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/decoder/ndarray.py
+-rw-r--r--   0 build     (1000) build     (1000)     6207 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/decoder/raw.py
+-rw-r--r--   0 build     (1000) build     (1000)     2523 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/image.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.919999 no_vtf-5.0.1/no_vtf/core/image/io/
+-rw-r--r--   0 build     (1000) build     (1000)      702 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/io/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     2289 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/io/file.py
+-rw-r--r--   0 build     (1000) build     (1000)    14670 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/io/image.py
+-rw-r--r--   0 build     (1000) build     (1000)     2925 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/io/io.py
+-rw-r--r--   0 build     (1000) build     (1000)     1997 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/io/raw.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.919999 no_vtf-5.0.1/no_vtf/core/image/modifier/
+-rw-r--r--   0 build     (1000) build     (1000)      337 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/modifier/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1838 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/modifier/fp_precision_modifier.py
+-rw-r--r--   0 build     (1000) build     (1000)     2508 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/modifier/hdr_to_ldr_modifier.py
+-rw-r--r--   0 build     (1000) build     (1000)      795 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/image/modifier/modifier.py
+-rw-r--r--   0 build     (1000) build     (1000)    13544 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/pipeline.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.923999 no_vtf-5.0.1/no_vtf/core/texture/
+-rw-r--r--   0 build     (1000) build     (1000)      202 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/texture/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      606 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/texture/decoder.py
+-rw-r--r--   0 build     (1000) build     (1000)      573 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/texture/extractor.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.923999 no_vtf-5.0.1/no_vtf/core/texture/filter/
+-rw-r--r--   0 build     (1000) build     (1000)      496 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/texture/filter/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1343 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/texture/filter/face.py
+-rw-r--r--   0 build     (1000) build     (1000)      974 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/texture/filter/filter.py
+-rw-r--r--   0 build     (1000) build     (1000)     1358 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/texture/filter/frame.py
+-rw-r--r--   0 build     (1000) build     (1000)     1760 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/texture/filter/mipmap.py
+-rw-r--r--   0 build     (1000) build     (1000)     2092 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/texture/filter/resolution.py
+-rw-r--r--   0 build     (1000) build     (1000)     1358 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/texture/filter/slice.py
+-rw-r--r--   0 build     (1000) build     (1000)      515 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/texture/namer.py
+-rw-r--r--   0 build     (1000) build     (1000)      993 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/core/texture/texture.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.923999 no_vtf-5.0.1/no_vtf/filesystem/
+-rw-r--r--   0 build     (1000) build     (1000)      253 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/filesystem/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     2102 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/filesystem/input_paths.py
+-rw-r--r--   0 build     (1000) build     (1000)      998 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/filesystem/output_directories.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.923999 no_vtf-5.0.1/no_vtf/functional/
+-rw-r--r--   0 build     (1000) build     (1000)      171 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/functional/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1425 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/functional/deferred.py
+-rw-r--r--   0 build     (1000) build     (1000)    14116 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/main.py
+-rw-r--r--   0 build     (1000) build     (1000)        0 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/py.typed
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.923999 no_vtf-5.0.1/no_vtf/task_runner/
+-rw-r--r--   0 build     (1000) build     (1000)      302 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/task_runner/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     2121 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/task_runner/parallel.py
+-rw-r--r--   0 build     (1000) build     (1000)      855 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/task_runner/sequential.py
+-rw-r--r--   0 build     (1000) build     (1000)      956 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/task_runner/task_runner.py
+-rw-r--r--   0 build     (1000) build     (1000)      422 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/typing.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.923999 no_vtf-5.0.1/no_vtf/vtf/
+-rw-r--r--   0 build     (1000) build     (1000)      412 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/vtf/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     6036 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/vtf/extractor.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.923999 no_vtf-5.0.1/no_vtf/vtf/generated/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/vtf/generated/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)    23014 2024-05-10 18:18:16.000000 no_vtf-5.0.1/no_vtf/vtf/generated/parser.py
+-rw-r--r--   0 build     (1000) build     (1000)       93 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/vtf/generated/parser.py.license
+-rw-r--r--   0 build     (1000) build     (1000)     2939 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/vtf/image_decoder.py
+-rw-r--r--   0 build     (1000) build     (1000)     1351 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/vtf/namer.py
+-rw-r--r--   0 build     (1000) build     (1000)     1229 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/vtf/texture.py
+-rw-r--r--   0 build     (1000) build     (1000)     4861 2024-05-10 18:14:21.000000 no_vtf-5.0.1/no_vtf/vtf/texture_decoder.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.935999 no_vtf-5.0.1/no_vtf.egg-info/
+-rw-r--r--   0 build     (1000) build     (1000)    12010 2024-05-10 18:21:46.000000 no_vtf-5.0.1/no_vtf.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)     7076 2024-05-10 18:21:46.000000 no_vtf-5.0.1/no_vtf.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1000)        1 2024-05-10 18:21:46.000000 no_vtf-5.0.1/no_vtf.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1000)       49 2024-05-10 18:21:46.000000 no_vtf-5.0.1/no_vtf.egg-info/entry_points.txt
+-rw-r--r--   0 build     (1000) build     (1000)        1 2024-05-10 18:17:46.000000 no_vtf-5.0.1/no_vtf.egg-info/not-zip-safe
+-rw-r--r--   0 build     (1000) build     (1000)      201 2024-05-10 18:21:46.000000 no_vtf-5.0.1/no_vtf.egg-info/requires.txt
+-rw-r--r--   0 build     (1000) build     (1000)        7 2024-05-10 18:21:46.000000 no_vtf-5.0.1/no_vtf.egg-info/top_level.txt
+-rw-r--r--   0 build     (1000) build     (1000)    42273 2024-05-10 18:14:21.000000 no_vtf-5.0.1/noxfile.py
+-rw-r--r--   0 build     (1000) build     (1000)     1193 2024-05-10 18:14:21.000000 no_vtf-5.0.1/pyproject.toml
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.911999 no_vtf-5.0.1/resources/
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.923999 no_vtf-5.0.1/resources/docs/
+-rw-r--r--   0 build     (1000) build     (1000)   123671 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/docs/screencast.gif
+-rw-r--r--   0 build     (1000) build     (1000)       95 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/docs/screencast.gif.license
+-rw-r--r--   0 build     (1000) build     (1000)  1009090 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/docs/screencast_v4.gif
+-rw-r--r--   0 build     (1000) build     (1000)       95 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/docs/screencast_v4.gif.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.927999 no_vtf-5.0.1/resources/pyinstaller/
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.927999 no_vtf-5.0.1/resources/pyinstaller/common/
+-rw-r--r--   0 build     (1000) build     (1000)     2005 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/common/COPYING.md
+-rw-r--r--   0 build     (1000) build     (1000)      163 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/common/COPYING.md.license
+-rw-r--r--   0 build     (1000) build     (1000)        6 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/empty.ico
+-rw-r--r--   0 build     (1000) build     (1000)       93 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/empty.ico.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.911999 no_vtf-5.0.1/resources/pyinstaller/nt/
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.927999 no_vtf-5.0.1/resources/pyinstaller/nt/.reuse/
+-rw-r--r--   0 build     (1000) build     (1000)     2029 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/.reuse/dep5
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.931999 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/
+-rw-r--r--   0 build     (1000) build     (1000)    21032 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-console-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21024 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-console-l1-2-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    20512 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-datetime-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    20544 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-debug-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    20520 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-errorhandling-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    24104 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-file-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    20520 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-file-l1-2-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    20520 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-file-l2-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    20520 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-handle-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21032 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-heap-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    20520 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-interlocked-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21568 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-libraryloader-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    23080 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-localization-l1-2-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21032 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-memory-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    20520 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-namedpipe-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21544 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-processenvironment-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    22560 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-processthreads-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21056 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-processthreads-l1-1-1.dll
+-rw-r--r--   0 build     (1000) build     (1000)    20008 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-profile-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21056 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-rtlsupport-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    20520 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-string-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    22568 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-synch-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21032 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-synch-l1-2-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21544 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-sysinfo-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21032 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-timezone-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    20520 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-util-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21544 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-conio-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    24616 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-convert-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21032 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-environment-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    22568 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-filesystem-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21544 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-heap-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21032 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-locale-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    29528 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-math-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    28736 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-multibyte-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    73048 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-private-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21568 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-process-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    25128 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-runtime-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    26664 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-stdio-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    26664 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-string-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    23080 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-time-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)    21032 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-utility-l1-1-0.dll
+-rw-r--r--   0 build     (1000) build     (1000)  1026088 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/ucrtbase.dll
+-rw-r--r--   0 build     (1000) build     (1000)   154392 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/nt/_internal/vcomp140.dll
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.935999 no_vtf-5.0.1/resources/pyinstaller/posix/
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.935999 no_vtf-5.0.1/resources/pyinstaller/posix/.reuse/
+-rw-r--r--   0 build     (1000) build     (1000)     5070 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/.reuse/dep5
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.935999 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/
+-rw-r--r--   0 build     (1000) build     (1000)     1891 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-bzip2.txt
+-rw-r--r--   0 build     (1000) build     (1000)     8616 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-fontconfig.txt
+-rw-r--r--   0 build     (1000) build     (1000)    46458 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libX11.txt
+-rw-r--r--   0 build     (1000) build     (1000)     1148 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libXau.txt
+-rw-r--r--   0 build     (1000) build     (1000)     1178 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libXdmcp.txt
+-rw-r--r--   0 build     (1000) build     (1000)    11101 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libXext.txt
+-rw-r--r--   0 build     (1000) build     (1000)     1105 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libXft.txt
+-rw-r--r--   0 build     (1000) build     (1000)     2164 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libXrender.txt
+-rw-r--r--   0 build     (1000) build     (1000)     2591 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libXss.txt
+-rw-r--r--   0 build     (1000) build     (1000)    23963 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libbsd.txt
+-rw-r--r--   0 build     (1000) build     (1000)     8018 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libmd.txt
+-rw-r--r--   0 build     (1000) build     (1000)     5345 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libpng.txt
+-rw-r--r--   0 build     (1000) build     (1000)     1139 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libtiff.txt
+-rw-r--r--   0 build     (1000) build     (1000)     1337 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libxcb.txt
+-rw-r--r--   0 build     (1000) build     (1000)     2775 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-xz.txt
+-rwxr-xr-x   0 build     (1000) build     (1000)      494 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/pyinstaller/posix/no_vtf.desktop
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.911999 no_vtf-5.0.1/resources/test/
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2024-05-10 18:21:46.935999 no_vtf-5.0.1/resources/test/samples/
+-rw-r--r--   0 build     (1000) build     (1000)      264 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/test/samples/CONTENTS
+-rw-r--r--   0 build     (1000) build     (1000)       93 2024-05-10 18:14:21.000000 no_vtf-5.0.1/resources/test/samples/CONTENTS.license
+-rw-r--r--   0 build     (1000) build     (1000)     2597 2024-05-10 18:21:46.935999 no_vtf-5.0.1/setup.cfg
```

### Comparing `no_vtf-5.0.0/.build.yml` & `no_vtf-5.0.1/.build.yml`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/.reuse/dep5` & `no_vtf-5.0.1/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/CONTRIBUTING.md` & `no_vtf-5.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/LICENSES/CC-BY-4.0.txt` & `no_vtf-5.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/LICENSES/CC0-1.0.txt` & `no_vtf-5.0.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/LICENSES/GPL-3.0-only.txt` & `no_vtf-5.0.1/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/LICENSES/GPL-3.0-or-later.txt` & `no_vtf-5.0.1/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/LICENSES/LGPL-3.0-or-later.txt` & `no_vtf-5.0.1/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/LICENSES/LicenseRef-WIN10SDK-RTM-AUG-2018.txt` & `no_vtf-5.0.1/LICENSES/LicenseRef-WIN10SDK-RTM-AUG-2018.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/LICENSES/LicenseRef-mlt687465.txt` & `no_vtf-5.0.1/LICENSES/LicenseRef-mlt687465.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/PKG-INFO` & `no_vtf-5.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: no_vtf
-Version: 5.0.0
+Version: 5.0.1
 Summary: Valve Texture Format Converter
 Home-page: https://git.sr.ht/~b5327157/no_vtf
 Author: b5327157
 Author-email: b5327157@protonmail.com
 License: GPL-3.0-only
 Project-URL: Download, https://git.sr.ht/~b5327157/no_vtf/#application-bundle
 Project-URL: Changelog, https://git.sr.ht/~b5327157/no_vtf/refs
@@ -27,15 +27,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; variant=CommonMark
 License-File: LICENSES/GPL-3.0-only.txt
 Requires-Dist: alive-progress<4,>=3.1.5
 Requires-Dist: click<9,>=8.1.7
 Requires-Dist: click-option-group<1,>=0.5.6
-Requires-Dist: imageio[pillow]<3,>=2.34.0
+Requires-Dist: imageio<3,>=2.34.0
 Requires-Dist: kaitaistruct<1,>=0.10
 Requires-Dist: numpy<2,>=1.26.4
 Requires-Dist: pillow<11,>=10.2.0
 Requires-Dist: tifffile<2025,>=2024.2.12
 Requires-Dist: typing-extensions<5,>=4.9.0
 
 # no_vtf
@@ -51,20 +51,20 @@
 [![Badge showing compliance with OpenSSF Best Practices](https://www.bestpractices.dev/projects/8316/badge)](https://www.bestpractices.dev/en/projects/8316)
 [![Badge showing Nox as the chosen Python automation toolkit](https://img.shields.io/badge/🦊-Nox-D85E00.svg)](https://github.com/wntrblm/nox)
 
 ![Screencast showing conversion of sprays downloaded in Team Fortress 2 using no_vtf](https://git.sr.ht/~b5327157/no_vtf/blob/HEAD/resources/docs/screencast_v4.gif)
 
 ---
 
-⌂ [Project pages](https://sr.ht/~b5327157/no_vtf/sources)
-\# [Source code](https://git.sr.ht/~b5327157/no_vtf/tree)
-~ [Changelog](https://git.sr.ht/~b5327157/no_vtf/refs)
-\> [Mailing list](https://lists.sr.ht/~b5327157/no_vtf)
-\+ [Ticket tracker](https://todo.sr.ht/~b5327157/no_vtf)
-❡ [Wiki](https://developer.valvesoftware.com/wiki/no_vtf)
+⌂&thinsp;[**Project pages**](https://sr.ht/~b5327157/no_vtf/sources)&nbsp;&nbsp;
+\#&thinsp;[**Source code**](https://git.sr.ht/~b5327157/no_vtf/tree)&nbsp;&nbsp;
+\~&thinsp;[**Changelog**](https://git.sr.ht/~b5327157/no_vtf/refs)&nbsp;&nbsp;
+\>&thinsp;[**Mailing list**](https://lists.sr.ht/~b5327157/no_vtf)&nbsp;&nbsp;
+\+&thinsp;[**Ticket tracker**](https://todo.sr.ht/~b5327157/no_vtf)&nbsp;&nbsp;
+❡&thinsp;[**Wiki**](https://developer.valvesoftware.com/wiki/no_vtf)&nbsp;&nbsp;
 
 ---
 
 ## Highlights
 
 - cross-platform – runs on any machine where Python is supported
 - console-only – runs without a graphical interface
@@ -75,26 +75,26 @@
 - test suite against crafted .vtf files and reference output
 - desktop environment integration via [no_vtf-desktop](https://git.sr.ht/~b5327157/no_vtf-desktop) (Linux-only)
 
 ## Installation
 
 ### Application bundle
 
-For Linux and Windows running on x64, there are application bundles with the Python interpreter included. Below are links to the latest version.
+For Linux and Windows running on x64, application bundles (with the Python interpreter included) are available for download. Below are links to the latest version.
 
-- [no_vtf-linux_x64.tar.xz](https://b5327157.srht.site/no_vtf/release/no_vtf-linux_x64.tar.xz) (glibc 2.31 or newer required, i.e. Debian 11, Ubuntu 20.04 LTS, …)
-- [no_vtf-windows_x64.zip](https://b5327157.srht.site/no_vtf/release/no_vtf-windows_x64.zip) (Windows 8.1 or newer required)
+- [**no_vtf-linux_x64.tar.xz**](https://b5327157.srht.site/no_vtf/release/no_vtf-linux_x64.tar.xz) (glibc 2.31 or newer required, i.e. Debian 11, Ubuntu 20.04 LTS, …)
+- [**no_vtf-windows_x64.zip**](https://b5327157.srht.site/no_vtf/release/no_vtf-windows_x64.zip) (Windows 8.1 or newer required)
 
 Starting from v4.2.0, application bundles GPG-signed with [`0x1C3724DFF9CEAF64`](https://keys.openpgp.org/vks/v1/by-fingerprint/46C4ACD8B7B3F77DC8C2E8ED1C3724DFF9CEAF64) are also attached to the [tagged versions](https://git.sr.ht/~b5327157/no_vtf/refs).
 
 Bundles are ready to be used offline – the FreeImage library is already included.
 
 ### Package
 
-If you have Python 3.10 or newer, you can install the [package](https://pypi.org/project/no-vtf/) from PyPI directly. An optional desktop integration is available via the [no_vtf-desktop](https://pypi.org/project/no-vtf-desktop/) package.
+If you have Python 3.10 or newer, you can install the [**no_vtf**](https://pypi.org/project/no-vtf/) package from PyPI directly. An optional desktop integration is available via the [**no_vtf-desktop**](https://pypi.org/project/no-vtf-desktop/) package.
 
 Before the first conversion, the FreeImage library will be downloaded to support the process. Further conversions are supported offline.
 
 As of [PEP 668](https://peps.python.org/pep-0668/), it is recommended to install the package into a virtual environment.
 
 #### Automated installation (via [pipx](https://pipx.pypa.io/stable/))
 
@@ -208,18 +208,20 @@
 
 ### Color space
 
 Color space of LDR textures is inferred from the context in which the texture is used in-game. Since this context is not available when converting the .vtf files directly, color space metadata for the output images cannot be set.
 
 Color space of HDR textures is always linear. It would make sense to set this metadata when converting into the TIFF format, but for technical reasons, this is not done.
 
-### Bit-perfect compatibility with VTF2TGA
+### Compatibility with VTF2TGA
 
 Some textures (notably those using DXT compression) have up to ±1 difference in R/G/B values compared to the output of VTF2TGA. This might be caused by rounding errors in either implementation.
 
+VTF2TGA does not always handle transparency the same as Source Engine and no_vtf does. When converting a DXT1 texture with an alpha flag set, VTF2TGA does not include the alpha channel in the output, but instead replaces it with a solid color.
+
 ### Animated output
 
 Image frames in the output file might not be stored exactly as they appear in the original .vtf file.
 For instance, consecutive identical frames might be merged into a single frame with a longer duration.
 
 ## Benchmark
 
@@ -258,8 +260,8 @@
 
 ## Contributing / Getting help
 
 Please refer to [CONTRIBUTING.md](https://git.sr.ht/~b5327157/no_vtf/tree/master/CONTRIBUTING.md).
 
 ## License
 
-The package is licensed under [GNU LGPL v3.0 or later](https://spdx.org/licenses/LGPL-3.0-or-later.html), except of image IO done with the help of the [ImageIO](https://github.com/imageio/imageio-freeimage) [FreeImage](https://freeimage.sourceforge.io/) plugin. This makes the entire package effectively licensed under [GNU GPL v3.0 only](https://spdx.org/licenses/GPL-3.0-only.html). If you make use of the image IO part (either directly or indirectly) when linking to no_vtf as a library, the combined work is licensed under the latter license.
+This package is free and open-source software, licensed under [GNU LGPL v3.0 or later](https://spdx.org/licenses/LGPL-3.0-or-later.html), except of image IO done with the help of the [ImageIO](https://github.com/imageio/imageio-freeimage) [FreeImage](https://freeimage.sourceforge.io/) plugin. This makes the entire package effectively licensed under [GNU GPL v3.0 only](https://spdx.org/licenses/GPL-3.0-only.html). If you make use of the image IO part (either directly or indirectly) when linking to no_vtf as a library, the combined work is licensed under the latter license.
```

### Comparing `no_vtf-5.0.0/README.md` & `no_vtf-5.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 [![Badge showing compliance with OpenSSF Best Practices](https://www.bestpractices.dev/projects/8316/badge)](https://www.bestpractices.dev/en/projects/8316)
 [![Badge showing Nox as the chosen Python automation toolkit](https://img.shields.io/badge/🦊-Nox-D85E00.svg)](https://github.com/wntrblm/nox)
 
 ![Screencast showing conversion of sprays downloaded in Team Fortress 2 using no_vtf](https://git.sr.ht/~b5327157/no_vtf/blob/HEAD/resources/docs/screencast_v4.gif)
 
 ---
 
-⌂ [Project pages](https://sr.ht/~b5327157/no_vtf/sources)
-\# [Source code](https://git.sr.ht/~b5327157/no_vtf/tree)
-~ [Changelog](https://git.sr.ht/~b5327157/no_vtf/refs)
-\> [Mailing list](https://lists.sr.ht/~b5327157/no_vtf)
-\+ [Ticket tracker](https://todo.sr.ht/~b5327157/no_vtf)
-❡ [Wiki](https://developer.valvesoftware.com/wiki/no_vtf)
+⌂&thinsp;[**Project pages**](https://sr.ht/~b5327157/no_vtf/sources)&nbsp;&nbsp;
+\#&thinsp;[**Source code**](https://git.sr.ht/~b5327157/no_vtf/tree)&nbsp;&nbsp;
+\~&thinsp;[**Changelog**](https://git.sr.ht/~b5327157/no_vtf/refs)&nbsp;&nbsp;
+\>&thinsp;[**Mailing list**](https://lists.sr.ht/~b5327157/no_vtf)&nbsp;&nbsp;
+\+&thinsp;[**Ticket tracker**](https://todo.sr.ht/~b5327157/no_vtf)&nbsp;&nbsp;
+❡&thinsp;[**Wiki**](https://developer.valvesoftware.com/wiki/no_vtf)&nbsp;&nbsp;
 
 ---
 
 ## Highlights
 
 - cross-platform – runs on any machine where Python is supported
 - console-only – runs without a graphical interface
@@ -35,26 +35,26 @@
 - test suite against crafted .vtf files and reference output
 - desktop environment integration via [no_vtf-desktop](https://git.sr.ht/~b5327157/no_vtf-desktop) (Linux-only)
 
 ## Installation
 
 ### Application bundle
 
-For Linux and Windows running on x64, there are application bundles with the Python interpreter included. Below are links to the latest version.
+For Linux and Windows running on x64, application bundles (with the Python interpreter included) are available for download. Below are links to the latest version.
 
-- [no_vtf-linux_x64.tar.xz](https://b5327157.srht.site/no_vtf/release/no_vtf-linux_x64.tar.xz) (glibc 2.31 or newer required, i.e. Debian 11, Ubuntu 20.04 LTS, …)
-- [no_vtf-windows_x64.zip](https://b5327157.srht.site/no_vtf/release/no_vtf-windows_x64.zip) (Windows 8.1 or newer required)
+- [**no_vtf-linux_x64.tar.xz**](https://b5327157.srht.site/no_vtf/release/no_vtf-linux_x64.tar.xz) (glibc 2.31 or newer required, i.e. Debian 11, Ubuntu 20.04 LTS, …)
+- [**no_vtf-windows_x64.zip**](https://b5327157.srht.site/no_vtf/release/no_vtf-windows_x64.zip) (Windows 8.1 or newer required)
 
 Starting from v4.2.0, application bundles GPG-signed with [`0x1C3724DFF9CEAF64`](https://keys.openpgp.org/vks/v1/by-fingerprint/46C4ACD8B7B3F77DC8C2E8ED1C3724DFF9CEAF64) are also attached to the [tagged versions](https://git.sr.ht/~b5327157/no_vtf/refs).
 
 Bundles are ready to be used offline – the FreeImage library is already included.
 
 ### Package
 
-If you have Python 3.10 or newer, you can install the [package](https://pypi.org/project/no-vtf/) from PyPI directly. An optional desktop integration is available via the [no_vtf-desktop](https://pypi.org/project/no-vtf-desktop/) package.
+If you have Python 3.10 or newer, you can install the [**no_vtf**](https://pypi.org/project/no-vtf/) package from PyPI directly. An optional desktop integration is available via the [**no_vtf-desktop**](https://pypi.org/project/no-vtf-desktop/) package.
 
 Before the first conversion, the FreeImage library will be downloaded to support the process. Further conversions are supported offline.
 
 As of [PEP 668](https://peps.python.org/pep-0668/), it is recommended to install the package into a virtual environment.
 
 #### Automated installation (via [pipx](https://pipx.pypa.io/stable/))
 
@@ -168,18 +168,20 @@
 
 ### Color space
 
 Color space of LDR textures is inferred from the context in which the texture is used in-game. Since this context is not available when converting the .vtf files directly, color space metadata for the output images cannot be set.
 
 Color space of HDR textures is always linear. It would make sense to set this metadata when converting into the TIFF format, but for technical reasons, this is not done.
 
-### Bit-perfect compatibility with VTF2TGA
+### Compatibility with VTF2TGA
 
 Some textures (notably those using DXT compression) have up to ±1 difference in R/G/B values compared to the output of VTF2TGA. This might be caused by rounding errors in either implementation.
 
+VTF2TGA does not always handle transparency the same as Source Engine and no_vtf does. When converting a DXT1 texture with an alpha flag set, VTF2TGA does not include the alpha channel in the output, but instead replaces it with a solid color.
+
 ### Animated output
 
 Image frames in the output file might not be stored exactly as they appear in the original .vtf file.
 For instance, consecutive identical frames might be merged into a single frame with a longer duration.
 
 ## Benchmark
 
@@ -218,8 +220,8 @@
 
 ## Contributing / Getting help
 
 Please refer to [CONTRIBUTING.md](https://git.sr.ht/~b5327157/no_vtf/tree/master/CONTRIBUTING.md).
 
 ## License
 
-The package is licensed under [GNU LGPL v3.0 or later](https://spdx.org/licenses/LGPL-3.0-or-later.html), except of image IO done with the help of the [ImageIO](https://github.com/imageio/imageio-freeimage) [FreeImage](https://freeimage.sourceforge.io/) plugin. This makes the entire package effectively licensed under [GNU GPL v3.0 only](https://spdx.org/licenses/GPL-3.0-only.html). If you make use of the image IO part (either directly or indirectly) when linking to no_vtf as a library, the combined work is licensed under the latter license.
+This package is free and open-source software, licensed under [GNU LGPL v3.0 or later](https://spdx.org/licenses/LGPL-3.0-or-later.html), except of image IO done with the help of the [ImageIO](https://github.com/imageio/imageio-freeimage) [FreeImage](https://freeimage.sourceforge.io/) plugin. This makes the entire package effectively licensed under [GNU GPL v3.0 only](https://spdx.org/licenses/GPL-3.0-only.html). If you make use of the image IO part (either directly or indirectly) when linking to no_vtf as a library, the combined work is licensed under the latter license.
```

### Comparing `no_vtf-5.0.0/SECURITY.md` & `no_vtf-5.0.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/builds/common` & `no_vtf-5.0.1/builds/common`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/builds/debian/python3.10-build_dep.sh` & `no_vtf-5.0.1/builds/debian/python3.10-build_dep.sh`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/builds/debian/wine-install.sh` & `no_vtf-5.0.1/builds/debian/wine-install.sh`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/builds/nox.py` & `no_vtf-5.0.1/builds/nox.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 import subprocess
 import sys
```

### Comparing `no_vtf-5.0.0/builds/publish_frozen.sh` & `no_vtf-5.0.1/builds/publish_frozen.sh`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/builds/with_wine.sh` & `no_vtf-5.0.1/builds/with_wine.sh`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/ksy/compile.py` & `no_vtf-5.0.1/ksy/compile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import ast
 import enum
 import pathlib
```

### Comparing `no_vtf-5.0.0/ksy/vtf.ksy` & `no_vtf-5.0.1/ksy/vtf.ksy`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/_alive_progress.py` & `no_vtf-5.0.1/no_vtf/_alive_progress.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/_click.py` & `no_vtf-5.0.1/no_vtf/_click.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/image/__init__.py` & `no_vtf-5.0.1/no_vtf/core/image/__init__.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/image/channel_separator.py` & `no_vtf-5.0.1/no_vtf/core/image/channel_separator.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/image/decoder/dxt.py` & `no_vtf-5.0.1/no_vtf/core/image/decoder/dxt.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/image/decoder/ndarray.py` & `no_vtf-5.0.1/no_vtf/core/image/decoder/ndarray.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/image/decoder/raw.py` & `no_vtf-5.0.1/no_vtf/core/image/decoder/raw.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/image/image.py` & `no_vtf-5.0.1/no_vtf/core/image/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,19 +44,19 @@
         ldr = _is_ldr(self.dtype)
         hdr = _is_hdr(self.dtype)
         assert ldr != hdr
 
         return "hdr" if hdr else "ldr"
 
     @staticmethod
-    def is_ldr(image: Image[_Id_co, _Ic_co]) -> TypeGuard[Image[ImageDataTypesLDR, _Ic_co]]:
+    def is_ldr(image: Image[ImageDataTypes, _Ic_co]) -> TypeGuard[Image[ImageDataTypesLDR, _Ic_co]]:
         return image.dynamic_range == "ldr"
 
     @staticmethod
-    def is_hdr(image: Image[_Id_co, _Ic_co]) -> TypeGuard[Image[ImageDataTypesHDR, _Ic_co]]:
+    def is_hdr(image: Image[ImageDataTypes, _Ic_co]) -> TypeGuard[Image[ImageDataTypesHDR, _Ic_co]]:
         return image.dynamic_range == "hdr"
 
 
 AnyImage: TypeAlias = Image[ImageDataTypes, ImageChannels]
 
 
 @mypyc_attr(allow_interpreted_subclasses=True)
```

### Comparing `no_vtf-5.0.0/no_vtf/core/image/io/__init__.py` & `no_vtf-5.0.1/no_vtf/core/image/io/__init__.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/image/io/file.py` & `no_vtf-5.0.1/no_vtf/core/image/io/file.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/image/io/image.py` & `no_vtf-5.0.1/no_vtf/core/image/io/image.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/image/io/io.py` & `no_vtf-5.0.1/no_vtf/core/image/io/io.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/image/io/raw.py` & `no_vtf-5.0.1/no_vtf/core/image/io/raw.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/image/modifier/fp_precision_modifier.py` & `no_vtf-5.0.1/no_vtf/core/image/modifier/fp_precision_modifier.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/image/modifier/hdr_to_ldr_modifier.py` & `no_vtf-5.0.1/no_vtf/core/image/modifier/hdr_to_ldr_modifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 _Ic = TypeVar("_Ic", bound=ImageChannels)
 
 
 @mypyc_attr(allow_interpreted_subclasses=True)
 class HdrToLdrModifier(ImageModifier[_Id_contra, _Ic, ImageDataTypesLDR, _Ic]):
     def __call__(self, image: Image[_Id_contra, _Ic]) -> Image[ImageDataTypesLDR, _Ic]:
-        if Image.is_ldr(image):
-            return image
+        if Image.is_ldr(image):  # pyright: ignore [reportUnknownMemberType]
+            return image  # pyright: ignore [reportUnknownVariableType]
 
         dtype = np.dtype(np.uint8)
         dtype_info = np.iinfo(dtype)
 
         data = (
             Deferred(image.data)
             .map(lambda data: data.astype(np.dtype(np.float64)))
```

### Comparing `no_vtf-5.0.0/no_vtf/core/image/modifier/modifier.py` & `no_vtf-5.0.1/no_vtf/core/image/modifier/modifier.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/pipeline.py` & `no_vtf-5.0.1/no_vtf/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/texture/decoder.py` & `no_vtf-5.0.1/no_vtf/core/texture/decoder.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/texture/extractor.py` & `no_vtf-5.0.1/no_vtf/core/texture/extractor.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/texture/filter/face.py` & `no_vtf-5.0.1/no_vtf/core/texture/filter/face.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/texture/filter/filter.py` & `no_vtf-5.0.1/no_vtf/core/texture/filter/filter.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/texture/filter/frame.py` & `no_vtf-5.0.1/no_vtf/core/texture/filter/frame.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/texture/filter/mipmap.py` & `no_vtf-5.0.1/no_vtf/core/texture/filter/mipmap.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/texture/filter/resolution.py` & `no_vtf-5.0.1/no_vtf/core/texture/filter/resolution.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/texture/filter/slice.py` & `no_vtf-5.0.1/no_vtf/core/texture/filter/slice.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/texture/namer.py` & `no_vtf-5.0.1/no_vtf/core/texture/namer.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/core/texture/texture.py` & `no_vtf-5.0.1/no_vtf/core/texture/texture.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/filesystem/input_paths.py` & `no_vtf-5.0.1/no_vtf/filesystem/input_paths.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/filesystem/output_directories.py` & `no_vtf-5.0.1/no_vtf/filesystem/output_directories.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/functional/deferred.py` & `no_vtf-5.0.1/no_vtf/functional/deferred.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/task_runner/parallel.py` & `no_vtf-5.0.1/no_vtf/task_runner/parallel.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/task_runner/sequential.py` & `no_vtf-5.0.1/no_vtf/task_runner/sequential.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/task_runner/task_runner.py` & `no_vtf-5.0.1/no_vtf/task_runner/task_runner.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/vtf/extractor.py` & `no_vtf-5.0.1/no_vtf/vtf/extractor.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,40 +107,50 @@
         dynamic_range: Optional[ImageDynamicRange],
     ) -> list[VtfTexture]:
         num_mipmaps = parser.header.v7_0.num_mipmaps
         num_frames = parser.header.v7_0.num_frames
         num_faces = parser.header.logical.num_faces
         num_slices = parser.header.logical.num_slices
 
+        onebitalpha = parser.header.logical.flags.onebitalpha
+        eightbitalpha = parser.header.logical.flags.eightbitalpha
+
         textures = []
         for mipmap_index, mipmap in enumerate(high_res_image.image_mipmaps):
             for frame_index, frame in enumerate(mipmap.image_frames):
                 for face_index, face in enumerate(frame.image_faces):
                     for slice_index, image_slice in enumerate(face.image_slices):
                         texture = VtfTexture(
                             width=image_slice.logical_width,
                             height=image_slice.logical_height,
                             dynamic_range=dynamic_range,
+                            onebitalpha=onebitalpha,
+                            eightbitalpha=eightbitalpha,
                             mipmap=TextureIndex(mipmap_index, count=num_mipmaps),
                             frame=TextureIndex(frame_index, count=num_frames),
                             face=TextureIndex(face_index, count=num_faces),
                             slice=TextureIndex(slice_index, count=num_slices),
                             image=image_slice,
                         )
                         textures.append(texture)
 
         return textures
 
     def _textures_from_low_res_image(
         self, parser: VtfParser, low_res_image: VtfParserImage
     ) -> list[VtfTexture]:
+        onebitalpha = parser.header.logical.flags.onebitalpha
+        eightbitalpha = parser.header.logical.flags.eightbitalpha
+
         texture = VtfTexture(
             width=low_res_image.logical_width,
             height=low_res_image.logical_height,
             dynamic_range="ldr",
+            onebitalpha=onebitalpha,
+            eightbitalpha=eightbitalpha,
             mipmap=None,
             frame=None,
             face=None,
             slice=None,
             image=low_res_image,
         )
         return [texture]
```

### Comparing `no_vtf-5.0.0/no_vtf/vtf/generated/parser.py` & `no_vtf-5.0.1/no_vtf/vtf/generated/parser.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/vtf/image_decoder.py` & `no_vtf-5.0.1/no_vtf/vtf/image_decoder.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/vtf/namer.py` & `no_vtf-5.0.1/no_vtf/vtf/namer.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/no_vtf/vtf/texture.py` & `no_vtf-5.0.1/no_vtf/vtf/texture.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 @mypyc_attr(allow_interpreted_subclasses=True)
 class VtfTexture(Texture):
     def __init__(
         self,
         *,
         dynamic_range: Optional[ImageDynamicRange],
+        onebitalpha: Optional[bool] = None,
+        eightbitalpha: Optional[bool] = None,
         width: int,
         height: int,
         mipmap: Optional[TextureIndex],
         frame: Optional[TextureIndex],
         face: Optional[TextureIndex],
         slice: Optional[TextureIndex],  # noqa: A002
         image: VtfParserImage,
@@ -31,8 +33,10 @@
             mipmap=mipmap,
             frame=frame,
             face=face,
             slice=slice,
         )
 
         self.dynamic_range: Final = dynamic_range
+        self.onebitalpha: Final = onebitalpha
+        self.eightbitalpha: Final = eightbitalpha
         self.image: Final = image
```

### Comparing `no_vtf-5.0.0/no_vtf/vtf/texture_decoder.py` & `no_vtf-5.0.1/no_vtf/vtf/texture_decoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,62 +59,65 @@
 
     def _get_decoder(self, texture: VtfTexture) -> ImageDecoder[AnyImageWithRawData]:
         image_format = texture.image.image_format
 
         dynamic_range = (
             self.dynamic_range if self.dynamic_range is not None else texture.dynamic_range
         )
+        has_alpha_flag = texture.onebitalpha or texture.eightbitalpha
 
         decoder: Optional[ImageDecoder[AnyImageWithRawData]] = None
-        match (image_format, dynamic_range):
-            case VtfParserImageFormat.rgba8888, _:
+        match (image_format, dynamic_range, has_alpha_flag):
+            case VtfParserImageFormat.rgba8888, _, _:
                 decoder = decode_rgba_uint8
-            case VtfParserImageFormat.abgr8888, _:
+            case VtfParserImageFormat.abgr8888, _, _:
                 decoder = decode_abgr_uint8
-            case VtfParserImageFormat.rgb888, _:
+            case VtfParserImageFormat.rgb888, _, _:
                 decoder = decode_rgb_uint8
-            case VtfParserImageFormat.bgr888, _:
+            case VtfParserImageFormat.bgr888, _, _:
                 decoder = decode_bgr_uint8
-            case VtfParserImageFormat.i8, _:
+            case VtfParserImageFormat.i8, _, _:
                 decoder = decode_l_uint8
-            case VtfParserImageFormat.ia88, _:
+            case VtfParserImageFormat.ia88, _, _:
                 decoder = decode_la_uint8
-            case VtfParserImageFormat.a8, _:
+            case VtfParserImageFormat.a8, _, _:
                 decoder = decode_a_uint8
-            case VtfParserImageFormat.rgb888_bluescreen, _:
+            case VtfParserImageFormat.rgb888_bluescreen, _, _:
                 decoder = decode_rgb_uint8_bluescreen
-            case VtfParserImageFormat.bgr888_bluescreen, _:
+            case VtfParserImageFormat.bgr888_bluescreen, _, _:
                 decoder = decode_bgr_uint8_bluescreen
-            case VtfParserImageFormat.argb8888, _:
+            case VtfParserImageFormat.argb8888, _, _:
                 # VTFLib/VTFEdit, Gimp VTF Plugin, and possibly others, decode this format
                 # differently because of mismatched channels (verified against VTF2TGA).
                 decoder = decode_argb_uint8
-            case VtfParserImageFormat.bgra8888, None:
+            case VtfParserImageFormat.bgra8888, None, _:
                 raise RuntimeError("Dynamic range is set neither on VtfTexture nor VtfDecoder")
-            case VtfParserImageFormat.bgra8888, "ldr":
+            case VtfParserImageFormat.bgra8888, "ldr", _:
                 decoder = decode_bgra_uint8
-            case VtfParserImageFormat.bgra8888, "hdr":
+            case VtfParserImageFormat.bgra8888, "hdr", _:
                 decoder = functools.partial(
                     decode_bgra_uint8_hdr, overbright_factor=self.overbright_factor
                 )
-            case VtfParserImageFormat.dxt1, _:
+            case VtfParserImageFormat.dxt1, _, False:
                 decoder = decode_dxt1_rgb
-            case VtfParserImageFormat.dxt3, _:
+            case VtfParserImageFormat.dxt1, _, True:
+                decoder = decode_dxt1_rgba
+            case VtfParserImageFormat.dxt3, _, _:
                 decoder = decode_dxt3
-            case VtfParserImageFormat.dxt5, _:
+            case VtfParserImageFormat.dxt5, _, _:
                 decoder = decode_dxt5
-            case VtfParserImageFormat.bgra4444, _:
+            case VtfParserImageFormat.bgra4444, _, _:
                 decoder = decode_bgra_uint4_le
-            case VtfParserImageFormat.dxt1_onebitalpha, _:
+            case VtfParserImageFormat.dxt1_onebitalpha, _, _:
                 decoder = decode_dxt1_rgba
-            case VtfParserImageFormat.uv88, _:
+            case VtfParserImageFormat.uv88, _, _:
                 decoder = decode_uv_uint8
-            case VtfParserImageFormat.rgba16161616f, _:
+            case VtfParserImageFormat.rgba16161616f, _, _:
                 decoder = decode_rgba_float16_le
-            case VtfParserImageFormat.rgba16161616, _:
+            case VtfParserImageFormat.rgba16161616, _, _:
                 decoder = decode_rgba_uint16_le_hdr
             case _:
                 pass
 
         if not decoder:
             raise NotImplementedError(f"Unsupported Valve texture format: {image_format.name}")
```

### Comparing `no_vtf-5.0.0/no_vtf.egg-info/PKG-INFO` & `no_vtf-5.0.1/no_vtf.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: no_vtf
-Version: 5.0.0
+Version: 5.0.1
 Summary: Valve Texture Format Converter
 Home-page: https://git.sr.ht/~b5327157/no_vtf
 Author: b5327157
 Author-email: b5327157@protonmail.com
 License: GPL-3.0-only
 Project-URL: Download, https://git.sr.ht/~b5327157/no_vtf/#application-bundle
 Project-URL: Changelog, https://git.sr.ht/~b5327157/no_vtf/refs
@@ -27,15 +27,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; variant=CommonMark
 License-File: LICENSES/GPL-3.0-only.txt
 Requires-Dist: alive-progress<4,>=3.1.5
 Requires-Dist: click<9,>=8.1.7
 Requires-Dist: click-option-group<1,>=0.5.6
-Requires-Dist: imageio[pillow]<3,>=2.34.0
+Requires-Dist: imageio<3,>=2.34.0
 Requires-Dist: kaitaistruct<1,>=0.10
 Requires-Dist: numpy<2,>=1.26.4
 Requires-Dist: pillow<11,>=10.2.0
 Requires-Dist: tifffile<2025,>=2024.2.12
 Requires-Dist: typing-extensions<5,>=4.9.0
 
 # no_vtf
@@ -51,20 +51,20 @@
 [![Badge showing compliance with OpenSSF Best Practices](https://www.bestpractices.dev/projects/8316/badge)](https://www.bestpractices.dev/en/projects/8316)
 [![Badge showing Nox as the chosen Python automation toolkit](https://img.shields.io/badge/🦊-Nox-D85E00.svg)](https://github.com/wntrblm/nox)
 
 ![Screencast showing conversion of sprays downloaded in Team Fortress 2 using no_vtf](https://git.sr.ht/~b5327157/no_vtf/blob/HEAD/resources/docs/screencast_v4.gif)
 
 ---
 
-⌂ [Project pages](https://sr.ht/~b5327157/no_vtf/sources)
-\# [Source code](https://git.sr.ht/~b5327157/no_vtf/tree)
-~ [Changelog](https://git.sr.ht/~b5327157/no_vtf/refs)
-\> [Mailing list](https://lists.sr.ht/~b5327157/no_vtf)
-\+ [Ticket tracker](https://todo.sr.ht/~b5327157/no_vtf)
-❡ [Wiki](https://developer.valvesoftware.com/wiki/no_vtf)
+⌂&thinsp;[**Project pages**](https://sr.ht/~b5327157/no_vtf/sources)&nbsp;&nbsp;
+\#&thinsp;[**Source code**](https://git.sr.ht/~b5327157/no_vtf/tree)&nbsp;&nbsp;
+\~&thinsp;[**Changelog**](https://git.sr.ht/~b5327157/no_vtf/refs)&nbsp;&nbsp;
+\>&thinsp;[**Mailing list**](https://lists.sr.ht/~b5327157/no_vtf)&nbsp;&nbsp;
+\+&thinsp;[**Ticket tracker**](https://todo.sr.ht/~b5327157/no_vtf)&nbsp;&nbsp;
+❡&thinsp;[**Wiki**](https://developer.valvesoftware.com/wiki/no_vtf)&nbsp;&nbsp;
 
 ---
 
 ## Highlights
 
 - cross-platform – runs on any machine where Python is supported
 - console-only – runs without a graphical interface
@@ -75,26 +75,26 @@
 - test suite against crafted .vtf files and reference output
 - desktop environment integration via [no_vtf-desktop](https://git.sr.ht/~b5327157/no_vtf-desktop) (Linux-only)
 
 ## Installation
 
 ### Application bundle
 
-For Linux and Windows running on x64, there are application bundles with the Python interpreter included. Below are links to the latest version.
+For Linux and Windows running on x64, application bundles (with the Python interpreter included) are available for download. Below are links to the latest version.
 
-- [no_vtf-linux_x64.tar.xz](https://b5327157.srht.site/no_vtf/release/no_vtf-linux_x64.tar.xz) (glibc 2.31 or newer required, i.e. Debian 11, Ubuntu 20.04 LTS, …)
-- [no_vtf-windows_x64.zip](https://b5327157.srht.site/no_vtf/release/no_vtf-windows_x64.zip) (Windows 8.1 or newer required)
+- [**no_vtf-linux_x64.tar.xz**](https://b5327157.srht.site/no_vtf/release/no_vtf-linux_x64.tar.xz) (glibc 2.31 or newer required, i.e. Debian 11, Ubuntu 20.04 LTS, …)
+- [**no_vtf-windows_x64.zip**](https://b5327157.srht.site/no_vtf/release/no_vtf-windows_x64.zip) (Windows 8.1 or newer required)
 
 Starting from v4.2.0, application bundles GPG-signed with [`0x1C3724DFF9CEAF64`](https://keys.openpgp.org/vks/v1/by-fingerprint/46C4ACD8B7B3F77DC8C2E8ED1C3724DFF9CEAF64) are also attached to the [tagged versions](https://git.sr.ht/~b5327157/no_vtf/refs).
 
 Bundles are ready to be used offline – the FreeImage library is already included.
 
 ### Package
 
-If you have Python 3.10 or newer, you can install the [package](https://pypi.org/project/no-vtf/) from PyPI directly. An optional desktop integration is available via the [no_vtf-desktop](https://pypi.org/project/no-vtf-desktop/) package.
+If you have Python 3.10 or newer, you can install the [**no_vtf**](https://pypi.org/project/no-vtf/) package from PyPI directly. An optional desktop integration is available via the [**no_vtf-desktop**](https://pypi.org/project/no-vtf-desktop/) package.
 
 Before the first conversion, the FreeImage library will be downloaded to support the process. Further conversions are supported offline.
 
 As of [PEP 668](https://peps.python.org/pep-0668/), it is recommended to install the package into a virtual environment.
 
 #### Automated installation (via [pipx](https://pipx.pypa.io/stable/))
 
@@ -208,18 +208,20 @@
 
 ### Color space
 
 Color space of LDR textures is inferred from the context in which the texture is used in-game. Since this context is not available when converting the .vtf files directly, color space metadata for the output images cannot be set.
 
 Color space of HDR textures is always linear. It would make sense to set this metadata when converting into the TIFF format, but for technical reasons, this is not done.
 
-### Bit-perfect compatibility with VTF2TGA
+### Compatibility with VTF2TGA
 
 Some textures (notably those using DXT compression) have up to ±1 difference in R/G/B values compared to the output of VTF2TGA. This might be caused by rounding errors in either implementation.
 
+VTF2TGA does not always handle transparency the same as Source Engine and no_vtf does. When converting a DXT1 texture with an alpha flag set, VTF2TGA does not include the alpha channel in the output, but instead replaces it with a solid color.
+
 ### Animated output
 
 Image frames in the output file might not be stored exactly as they appear in the original .vtf file.
 For instance, consecutive identical frames might be merged into a single frame with a longer duration.
 
 ## Benchmark
 
@@ -258,8 +260,8 @@
 
 ## Contributing / Getting help
 
 Please refer to [CONTRIBUTING.md](https://git.sr.ht/~b5327157/no_vtf/tree/master/CONTRIBUTING.md).
 
 ## License
 
-The package is licensed under [GNU LGPL v3.0 or later](https://spdx.org/licenses/LGPL-3.0-or-later.html), except of image IO done with the help of the [ImageIO](https://github.com/imageio/imageio-freeimage) [FreeImage](https://freeimage.sourceforge.io/) plugin. This makes the entire package effectively licensed under [GNU GPL v3.0 only](https://spdx.org/licenses/GPL-3.0-only.html). If you make use of the image IO part (either directly or indirectly) when linking to no_vtf as a library, the combined work is licensed under the latter license.
+This package is free and open-source software, licensed under [GNU LGPL v3.0 or later](https://spdx.org/licenses/LGPL-3.0-or-later.html), except of image IO done with the help of the [ImageIO](https://github.com/imageio/imageio-freeimage) [FreeImage](https://freeimage.sourceforge.io/) plugin. This makes the entire package effectively licensed under [GNU GPL v3.0 only](https://spdx.org/licenses/GPL-3.0-only.html). If you make use of the image IO part (either directly or indirectly) when linking to no_vtf as a library, the combined work is licensed under the latter license.
```

### Comparing `no_vtf-5.0.0/no_vtf.egg-info/SOURCES.txt` & `no_vtf-5.0.1/no_vtf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 builds/debian/wine-install.sh
 ksy/compile.py
 ksy/vtf.ksy
 no_vtf/__init__.py
 no_vtf/__main__.py
 no_vtf/_alive_progress.py
 no_vtf/_click.py
+no_vtf/_main.py
 no_vtf/_version.py
 no_vtf/main.py
 no_vtf/py.typed
 no_vtf/typing.py
 no_vtf.egg-info/PKG-INFO
 no_vtf.egg-info/SOURCES.txt
 no_vtf.egg-info/dependency_links.txt
```

### Comparing `no_vtf-5.0.0/noxfile.py` & `no_vtf-5.0.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/pyproject.toml` & `no_vtf-5.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/docs/screencast.gif` & `no_vtf-5.0.1/resources/docs/screencast.gif`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/docs/screencast_v4.gif` & `no_vtf-5.0.1/resources/docs/screencast_v4.gif`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/common/COPYING.md` & `no_vtf-5.0.1/resources/pyinstaller/common/COPYING.md`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/.reuse/dep5` & `no_vtf-5.0.1/resources/pyinstaller/nt/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-console-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-console-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-console-l1-2-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-console-l1-2-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-datetime-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-datetime-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-debug-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-debug-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-errorhandling-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-errorhandling-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-file-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-file-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-file-l1-2-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-file-l1-2-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-file-l2-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-file-l2-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-handle-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-handle-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-heap-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-heap-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-interlocked-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-interlocked-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-libraryloader-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-libraryloader-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-localization-l1-2-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-localization-l1-2-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-memory-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-memory-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-namedpipe-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-namedpipe-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-processenvironment-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-processenvironment-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-processthreads-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-processthreads-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-processthreads-l1-1-1.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-processthreads-l1-1-1.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-profile-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-profile-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-rtlsupport-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-rtlsupport-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-string-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-string-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-synch-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-synch-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-synch-l1-2-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-synch-l1-2-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-sysinfo-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-sysinfo-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-timezone-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-timezone-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-core-util-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-core-util-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-conio-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-conio-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-convert-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-convert-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-environment-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-environment-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-filesystem-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-filesystem-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-heap-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-heap-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-locale-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-locale-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-math-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-math-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-multibyte-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-multibyte-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-private-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-private-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-process-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-process-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-runtime-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-runtime-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-stdio-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-stdio-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-string-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-string-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-time-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-time-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/api-ms-win-crt-utility-l1-1-0.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/api-ms-win-crt-utility-l1-1-0.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/ucrtbase.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/ucrtbase.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/nt/_internal/vcomp140.dll` & `no_vtf-5.0.1/resources/pyinstaller/nt/_internal/vcomp140.dll`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/.reuse/dep5` & `no_vtf-5.0.1/resources/pyinstaller/posix/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-bzip2.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-bzip2.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-fontconfig.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-fontconfig.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libX11.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libX11.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libXau.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libXau.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libXdmcp.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libXdmcp.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libXext.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libXext.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libXft.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libXft.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libXrender.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libXrender.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libXss.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libXss.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libbsd.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libbsd.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libmd.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libmd.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libpng.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libpng.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libtiff.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libtiff.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-libxcb.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-libxcb.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/resources/pyinstaller/posix/LICENSES/LicenseRef-xz.txt` & `no_vtf-5.0.1/resources/pyinstaller/posix/LICENSES/LicenseRef-xz.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-5.0.0/setup.cfg` & `no_vtf-5.0.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 url = https://git.sr.ht/~b5327157/no_vtf
 
 [options]
 install_requires = 
 	alive-progress >= 3.1.5, < 4
 	click >= 8.1.7, < 9
 	click-option-group >= 0.5.6, < 1
-	imageio[pillow] >= 2.34.0, < 3
+	imageio >= 2.34.0, < 3
 	kaitaistruct >= 0.10, < 1
 	numpy >= 1.26.4, < 2
 	pillow >= 10.2.0, < 11
 	tifffile >= 2024.2.12, < 2025
 	typing-extensions >= 4.9.0, < 5
 packages = find:
 py_modules = 
@@ -60,16 +60,19 @@
 	no_vtf.*
 
 [flake8]
 exclude = 
 	no_vtf/_version.py
 	generated
 extend-ignore = 
+	E202
 	E203
+	E251
 	A003
+	A005
 max_complexity = 10
 max_line_length = 100
 show_source = True
 
 [isort]
 atomic = True
 color_output = True
```

