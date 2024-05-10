# Comparing `tmp/pysarpro-0.1.3.tar.gz` & `tmp/pysarpro-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysarpro-0.1.3.tar", last modified: Fri May 10 07:52:09 2024, max compression
+gzip compressed data, was "pysarpro-0.1.4.tar", last modified: Fri May 10 09:09:37 2024, max compression
```

## Comparing `pysarpro-0.1.3.tar` & `pysarpro-0.1.4.tar`

### file list

```diff
@@ -1,246 +1,246 @@
--rw-r--r--   0        0        0     2766 2024-05-10 07:25:06.000000 pysarpro-0.1.3/.spin/cmds.py
--rw-r--r--   0        0        0       64 2024-05-10 07:25:06.000000 pysarpro-0.1.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    22141 2024-05-10 07:25:06.000000 pysarpro-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0        0        0      978 2024-05-10 07:25:06.000000 pysarpro-0.1.3/CONTRIBUTORS.txt
--rw-r--r--   0        0        0    12883 2024-05-10 07:25:06.000000 pysarpro-0.1.3/INSTALL.rst
--rw-r--r--   0        0        0     3822 2024-05-10 07:25:06.000000 pysarpro-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0      647 2024-05-10 07:25:06.000000 pysarpro-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0     2734 2024-05-10 07:25:06.000000 pysarpro-0.1.3/Makefile
--rw-r--r--   0        0        0     2092 2024-05-10 07:25:06.000000 pysarpro-0.1.3/README.md
--rw-r--r--   0        0        0     8052 2024-05-10 07:25:06.000000 pysarpro-0.1.3/RELEASE.txt
--rw-r--r--   0        0        0      590 2024-05-10 07:25:06.000000 pysarpro-0.1.3/asv.conf.json
--rw-r--r--   0        0        0      209 2024-05-10 07:25:06.000000 pysarpro-0.1.3/conda/dev.yaml
--rw-r--r--   0        0        0     4540 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/Makefile
--rw-r--r--   0        0        0      363 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/examples/README.txt
--rw-r--r--   0        0        0       10 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/examples/data/README.txt
--rw-r--r--   0        0        0        0 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/ext/__init__.py
--rw-r--r--   0        0        0     1769 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/ext/doi_role.py
--rw-r--r--   0        0        0     4040 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/ext/pysarpro_extensions.py
--rw-r--r--   0        0        0     4479 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/gh-pages.py
--rw-r--r--   0        0        0      828 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/_static/docversions.js
--rw-r--r--   0        0        0    15406 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/_static/favicon.ico
--rw-r--r--   0        0        0   104344 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/_static/logo.png
--rw-r--r--   0        0        0      637 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/_static/theme_overrides.css
--rw-r--r--   0        0        0      548 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/_static/version_switcher.json
--rw-r--r--   0        0        0     8140 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/about/code_of_conduct.md
--rw-r--r--   0        0        0      228 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/about/index.rst
--rw-r--r--   0        0        0    11104 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/about/report_handling_manual.rst
--rw-r--r--   0        0        0     3968 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/about/values.md
--rw-r--r--   0        0        0    11358 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/conf.py
--rw-r--r--   0        0        0       39 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/development/contribute.rst
--rw-r--r--   0        0        0    11595 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/development/core_developer.md
--rw-r--r--   0        0        0      196 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/development/index.rst
--rw-r--r--   0        0        0    16311 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/branch_dropdown.png
--rw-r--r--   0        0        0     4792 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/configure_git.rst
--rw-r--r--   0        0        0    13819 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/development_workflow.rst
--rw-r--r--   0        0        0      853 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/following_latest.rst
--rw-r--r--   0        0        0    13092 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/forking_button.png
--rw-r--r--   0        0        0     1216 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/forking_hell.rst
--rw-r--r--   0        0        0      224 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/git_development.rst
--rw-r--r--   0        0        0      599 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/git_install.rst
--rw-r--r--   0        0        0      545 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/git_intro.rst
--rw-r--r--   0        0        0     3235 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/git_links.inc
--rw-r--r--   0        0        0     1766 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/git_resources.rst
--rw-r--r--   0        0        0      239 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/index.rst
--rw-r--r--   0        0        0     1477 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/known_projects.inc
--rw-r--r--   0        0        0      113 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/links.inc
--rw-r--r--   0        0        0     3072 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/maintainer_workflow.rst
--rw-r--r--   0        0        0     4049 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/patching.rst
--rw-r--r--   0        0        0    12893 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/pull_button.png
--rw-r--r--   0        0        0     2035 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/set_up_fork.rst
--rw-r--r--   0        0        0      215 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/gitwash/this_project.inc
--rw-r--r--   0        0        0     2571 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/index.rst
--rw-r--r--   0        0        0       54 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/license.md
--rw-r--r--   0        0        0      289 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/release_notes/index.rst
--rw-r--r--   0        0        0      252 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/release_notes/release_0.1.rst
--rw-r--r--   0        0        0     1508 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/release_notes/release_dev.rst
--rw-r--r--   0        0        0      621 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/release_notes/release_template.rst
--rw-r--r--   0        0        0    12075 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/skips/0-skip-process.rst
--rw-r--r--   0        0        0     8541 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/skips/1-governance.rst
--rw-r--r--   0        0        0     6979 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/skips/2-values.rst
--rw-r--r--   0        0        0    15188 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/skips/3-transition-to-v1.rst
--rw-r--r--   0        0        0    14707 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/skips/4-transition-to-v2.rst
--rw-r--r--   0        0        0    12925 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/skips/_static/skip-flowchart.png
--rw-r--r--   0        0        0      250 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/skips/index.md
--rw-r--r--   0        0        0     3109 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/skips/template.rst
--rw-r--r--   0        0        0    10065 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/data_types.rst
--rw-r--r--   0        0        0      694 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/geometrical_transform.rst
--rw-r--r--   0        0        0     1545 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/getting_help.rst
--rw-r--r--   0        0        0      362 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/getting_started.rst
--rw-r--r--   0        0        0     3958 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/glossary.md
--rw-r--r--   0        0        0      443 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/index.rst
--rw-r--r--   0        0        0       34 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/install.rst
--rw-r--r--   0        0        0    10525 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/numpy_images.rst
--rw-r--r--   0        0        0     2364 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/plugins.rst
--rw-r--r--   0        0        0     6632 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/transforming_image_data.rst
--rw-r--r--   0        0        0     1920 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/tutorial_parallelization.rst
--rw-r--r--   0        0        0     4764 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/tutorial_segmentation.rst
--rw-r--r--   0        0        0      104 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/tutorials.rst
--rw-r--r--   0        0        0     5018 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/video.rst
--rw-r--r--   0        0        0     1054 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/source/user_guide/visualization.rst
--rw-r--r--   0        0        0      200 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/tools/LICENSE.txt
--rw-r--r--   0        0        0    16835 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/tools/apigen.py
--rw-r--r--   0        0        0     1811 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/tools/build_modref_templates.py
--rw-r--r--   0        0        0     4089 2024-05-10 07:25:06.000000 pysarpro-0.1.3/doc/tools/plot_pr.py
--rw-r--r--   0        0        0     2701 2024-05-10 07:25:06.000000 pysarpro-0.1.3/meson.build
--rw-r--r--   0        0        0     4545 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4647 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/__init__.py
--rw-r--r--   0        0        0      135 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/__init__.pyi
--rw-r--r--   0        0        0      778 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_build_utils/__init__.py
--rw-r--r--   0        0        0      449 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_build_utils/copyfiles.py
--rw-r--r--   0        0        0      672 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_build_utils/cythoner.py
--rw-r--r--   0        0        0      528 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_build_utils/gcc_build_bitness.py
--rw-r--r--   0        0        0       32 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_build_utils/link-version-pyinit.map
--rw-r--r--   0        0        0     1651 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_build_utils/tempita.py
--rw-r--r--   0        0        0      371 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_build_utils/version.py
--rw-r--r--   0        0        0        0 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/__init__.py
--rw-r--r--   0        0        0       94 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/_dependency_checks.py
--rw-r--r--   0        0        0     1343 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/_geometry.py
--rw-r--r--   0        0        0      764 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/_tempfile.py
--rw-r--r--   0        0        0     5070 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/_warnings.py
--rw-r--r--   0        0        0     4330 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/coord.py
--rw-r--r--   0        0        0     1246 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/fast_exp.h
--rw-r--r--   0        0        0      471 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/fast_exp.pxd
--rw-r--r--   0        0        0      178 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/fast_exp.pyx
--rw-r--r--   0        0        0     5321 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/filters.py
--rw-r--r--   0        0        0      533 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/fused_numerics.pxd
--rw-r--r--   0        0        0      470 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/geometry.pxd
--rw-r--r--   0        0        0     2740 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/geometry.pyx
--rw-r--r--   0        0        0    12483 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/interpolation.pxd
--rw-r--r--   0        0        0      207 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/interpolation.pyx
--rw-r--r--   0        0        0     1189 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/meson.build
--rw-r--r--   0        0        0     3592 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/tester.py
--rw-r--r--   0        0        0    10690 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/testing.py
--rw-r--r--   0        0        0        0 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/tests/__init__.py
--rw-r--r--   0        0        0      341 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/tests/meson.build
--rw-r--r--   0        0        0     3050 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/tests/test_coord.py
--rw-r--r--   0        0        0      490 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/tests/test_fast_exp.py
--rw-r--r--   0        0        0     2120 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/tests/test_geometry.py
--rw-r--r--   0        0        0     1139 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/tests/test_interpolation.py
--rw-r--r--   0        0        0     1426 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/tests/test_safe_as_int.py
--rw-r--r--   0        0        0     2952 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/tests/test_testing.py
--rw-r--r--   0        0        0    20613 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/tests/test_utils.py
--rw-r--r--   0        0        0     1078 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/tests/test_version_requirements.py
--rw-r--r--   0        0        0     1256 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/tests/test_warnings.py
--rw-r--r--   0        0        0      243 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/transform.pxd
--rw-r--r--   0        0        0     1142 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/transform.pyx
--rw-r--r--   0        0        0    33407 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/utils.py
--rw-r--r--   0        0        0     5332 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/_shared/version_requirements.py
--rw-r--r--   0        0        0      482 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/conftest.py
--rw-r--r--   0        0        0      157 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/01-sar/meson.build
--rw-r--r--   0        0        0   159872 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/01-sar/signal1_ac.npy
--rw-r--r--   0        0        0    60480 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/01-sar/signal1_rc.npy
--rw-r--r--   0        0        0   159872 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/01-sar/signal2_ac.npy
--rw-r--r--   0        0        0    60480 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/01-sar/signal2_rc.npy
--rw-r--r--   0        0        0      277 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/README.txt
--rw-r--r--   0        0        0      384 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/__init__.py
--rw-r--r--   0        0        0      193 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/__init__.pyi
--rw-r--r--   0        0        0     2323 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/_binary_blobs.py
--rw-r--r--   0        0        0    12549 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/_fetchers.py
--rw-r--r--   0        0        0    22153 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/_registry.py
--rw-r--r--   0        0        0   791555 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/astronaut.png
--rw-r--r--   0        0        0   104344 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/logo.png
--rw-r--r--   0        0        0      476 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/meson.build
--rw-r--r--   0        0        0        0 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/tests/__init__.py
--rw-r--r--   0        0        0      144 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/tests/meson.build
--rw-r--r--   0        0        0     1526 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/data/tests/test_data.py
--rw-r--r--   0        0        0     1790 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/__init__.py
--rw-r--r--   0        0        0      570 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_image_stack.py
--rw-r--r--   0        0        0     5898 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_io.py
--rw-r--r--   0        0        0        0 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/__init__.py
--rw-r--r--   0        0        0    13042 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/_colormixer.pyx
--rw-r--r--   0        0        0     2114 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/_histograms.pyx
--rw-r--r--   0        0        0       88 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/fits_plugin.ini
--rw-r--r--   0        0        0     4408 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/fits_plugin.py
--rw-r--r--   0        0        0       89 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/gdal_plugin.ini
--rw-r--r--   0        0        0      349 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/gdal_plugin.py
--rw-r--r--   0        0        0       88 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/imageio_plugin.ini
--rw-r--r--   0        0        0      330 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/imageio_plugin.py
--rw-r--r--   0        0        0       86 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/imread_plugin.ini
--rw-r--r--   0        0        0      956 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/imread_plugin.py
--rw-r--r--   0        0        0      123 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/matplotlib_plugin.ini
--rw-r--r--   0        0        0     6402 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/matplotlib_plugin.py
--rw-r--r--   0        0        0      916 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/meson.build
--rw-r--r--   0        0        0       91 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/pil_plugin.ini
--rw-r--r--   0        0        0     7843 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/pil_plugin.py
--rw-r--r--   0        0        0       92 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/simpleitk_plugin.ini
--rw-r--r--   0        0        0      531 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/simpleitk_plugin.py
--rw-r--r--   0        0        0      110 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/tifffile_plugin.ini
--rw-r--r--   0        0        0     2071 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/_plugins/tifffile_plugin.py
--rw-r--r--   0        0        0    14923 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/collection.py
--rw-r--r--   0        0        0    10378 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/manage_plugins.py
--rw-r--r--   0        0        0      366 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/meson.build
--rw-r--r--   0        0        0     2562 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/sift.py
--rw-r--r--   0        0        0    47634 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/ste.py
--rw-r--r--   0        0        0        0 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/tests/__init__.py
--rw-r--r--   0        0        0      330 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/tests/meson.build
--rw-r--r--   0        0        0      844 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/tests/test_fits.py
--rw-r--r--   0        0        0      742 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/tests/test_histograms.py
--rw-r--r--   0        0        0     1741 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/tests/test_imageio.py
--rw-r--r--   0        0        0     1018 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/tests/test_imread.py
--rw-r--r--   0        0        0     2711 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/tests/test_io.py
--rw-r--r--   0        0        0     4206 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/tests/test_mpl_imshow.py
--rw-r--r--   0        0        0     2289 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/tests/test_plugin.py
--rw-r--r--   0        0        0     3337 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/tests/test_sift.py
--rw-r--r--   0        0        0     1203 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/tests/test_simpleitk.py
--rw-r--r--   0        0        0     1489 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/tests/test_tifffile.py
--rw-r--r--   0        0        0     1283 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/io/util.py
--rw-r--r--   0        0        0     4860 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/meson.build
--rw-r--r--   0        0        0       16 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/models/__init__.py
--rw-r--r--   0        0        0      264 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/models/meson.build
--rw-r--r--   0        0        0        0 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/models/predict_model.py
--rw-r--r--   0        0        0        0 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/models/train_model.py
--rw-r--r--   0        0        0        0 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/py.typed
--rw-r--r--   0        0        0     1246 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/__init__.py
--rw-r--r--   0        0        0     2560 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/_invert.py
--rw-r--r--   0        0        0     1569 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/_label.py
--rw-r--r--   0        0        0     6691 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/_map_array.py
--rw-r--r--   0        0        0     3885 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/_regular_grid.py
--rw-r--r--   0        0        0      968 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/_remap.pyx
--rw-r--r--   0        0        0     2234 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/_slice_along_axes.py
--rw-r--r--   0        0        0     7650 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/apply_parallel.py
--rw-r--r--   0        0        0     2486 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/arraycrop.py
--rw-r--r--   0        0        0     2058 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/compare.py
--rw-r--r--   0        0        0    18089 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/dtype.py
--rw-r--r--   0        0        0      598 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/lookfor.py
--rw-r--r--   0        0        0      744 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/meson.build
--rw-r--r--   0        0        0     8692 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/noise.py
--rw-r--r--   0        0        0     7831 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/shape.py
--rw-r--r--   0        0        0        0 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/tests/__init__.py
--rw-r--r--   0        0        0      378 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/tests/meson.build
--rw-r--r--   0        0        0     1850 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/tests/test_arraycrop.py
--rw-r--r--   0        0        0     2393 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/tests/test_compare.py
--rw-r--r--   0        0        0     5123 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/tests/test_dtype.py
--rw-r--r--   0        0        0     2418 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/tests/test_invert.py
--rw-r--r--   0        0        0     1792 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/tests/test_labels.py
--rw-r--r--   0        0        0     2900 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/tests/test_map_array.py
--rw-r--r--   0        0        0     7799 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/tests/test_random_noise.py
--rw-r--r--   0        0        0      982 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/tests/test_regular_grid.py
--rw-r--r--   0        0        0     4551 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/tests/test_shape.py
--rw-r--r--   0        0        0     1680 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/tests/test_slice_along_axes.py
--rw-r--r--   0        0        0     1102 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/tests/test_unique_rows.py
--rw-r--r--   0        0        0     1516 2024-05-10 07:25:06.000000 pysarpro-0.1.3/pysarpro/util/unique.py
--rw-r--r--   0        0        0      823 2024-05-10 07:25:06.000000 pysarpro-0.1.3/requirements/README.md
--rw-r--r--   0        0        0       16 2024-05-10 07:25:06.000000 pysarpro-0.1.3/requirements/_release_tools.txt
--rw-r--r--   0        0        0      234 2024-05-10 07:25:06.000000 pysarpro-0.1.3/requirements/build.txt
--rw-r--r--   0        0        0      137 2024-05-10 07:25:06.000000 pysarpro-0.1.3/requirements/data.txt
--rw-r--r--   0        0        0      238 2024-05-10 07:25:06.000000 pysarpro-0.1.3/requirements/default.txt
--rw-r--r--   0        0        0      174 2024-05-10 07:25:06.000000 pysarpro-0.1.3/requirements/developer.txt
--rw-r--r--   0        0        0      435 2024-05-10 07:25:06.000000 pysarpro-0.1.3/requirements/docs.txt
--rw-r--r--   0        0        0      259 2024-05-10 07:25:06.000000 pysarpro-0.1.3/requirements/optional.txt
--rw-r--r--   0        0        0      241 2024-05-10 07:25:06.000000 pysarpro-0.1.3/requirements/test.txt
--rw-r--r--   0        0        0       83 2024-05-10 07:25:06.000000 pysarpro-0.1.3/requirements.txt
--rw-r--r--   0        0        0     2121 2024-05-10 07:25:06.000000 pysarpro-0.1.3/tools/check_sdist.py
--rw-r--r--   0        0        0     1177 2024-05-10 07:25:06.000000 pysarpro-0.1.3/tools/generate_requirements.py
--rwxr-xr-x   0        0        0     1282 2024-05-10 07:25:06.000000 pysarpro-0.1.3/tools/github/before_install.sh
--rwxr-xr-x   0        0        0     1378 2024-05-10 07:25:06.000000 pysarpro-0.1.3/tools/github/script.sh
--rw-r--r--   0        0        0      260 2024-05-10 07:25:06.000000 pysarpro-0.1.3/tools/header.py
--rw-r--r--   0        0        0     1652 2024-05-10 07:25:06.000000 pysarpro-0.1.3/tools/mailmap.py
--rw-r--r--   0        0        0   158924 2024-05-10 07:25:06.000000 pysarpro-0.1.3/tools/precompute/mc_meta/LookUpTable.h
--rw-r--r--   0        0        0      454 2024-05-10 07:25:06.000000 pysarpro-0.1.3/tools/precompute/mc_meta/README.md
--rw-r--r--   0        0        0     3680 2024-05-10 07:25:06.000000 pysarpro-0.1.3/tools/precompute/mc_meta/createluts.py
--rw-r--r--   0        0        0     2430 2024-05-10 07:25:06.000000 pysarpro-0.1.3/tools/precompute/mc_meta/visual_test.py
--rw-r--r--   0        0        0     3865 2024-05-10 07:25:06.000000 pysarpro-0.1.3/tools/precompute/moments_sympy.py
--rw-r--r--   0        0        0      233 2024-05-10 07:25:06.000000 pysarpro-0.1.3/tools/rm_pyx_assoc_c_cpp.sh
--rw-r--r--   0        0        0      711 2024-05-10 07:25:06.000000 pysarpro-0.1.3/tools/upload_wheels.sh
--rw-r--r--   0        0        0    10736 2024-05-10 07:52:09.940515 pysarpro-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2766 2024-05-10 08:56:51.000000 pysarpro-0.1.4/.spin/cmds.py
+-rw-r--r--   0        0        0       64 2024-05-10 08:56:51.000000 pysarpro-0.1.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    22141 2024-05-10 08:56:51.000000 pysarpro-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      978 2024-05-10 08:56:51.000000 pysarpro-0.1.4/CONTRIBUTORS.txt
+-rw-r--r--   0        0        0    12883 2024-05-10 08:56:51.000000 pysarpro-0.1.4/INSTALL.rst
+-rw-r--r--   0        0        0     3822 2024-05-10 08:56:51.000000 pysarpro-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      647 2024-05-10 08:56:51.000000 pysarpro-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0     2734 2024-05-10 08:56:51.000000 pysarpro-0.1.4/Makefile
+-rw-r--r--   0        0        0     2092 2024-05-10 08:56:51.000000 pysarpro-0.1.4/README.md
+-rw-r--r--   0        0        0     8052 2024-05-10 08:56:51.000000 pysarpro-0.1.4/RELEASE.txt
+-rw-r--r--   0        0        0      590 2024-05-10 08:56:51.000000 pysarpro-0.1.4/asv.conf.json
+-rw-r--r--   0        0        0      209 2024-05-10 08:56:51.000000 pysarpro-0.1.4/conda/dev.yaml
+-rw-r--r--   0        0        0     4540 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/Makefile
+-rw-r--r--   0        0        0      363 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/examples/README.txt
+-rw-r--r--   0        0        0       10 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/examples/data/README.txt
+-rw-r--r--   0        0        0        0 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/ext/__init__.py
+-rw-r--r--   0        0        0     1769 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/ext/doi_role.py
+-rw-r--r--   0        0        0     4040 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/ext/pysarpro_extensions.py
+-rw-r--r--   0        0        0     4479 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/gh-pages.py
+-rw-r--r--   0        0        0      828 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/_static/docversions.js
+-rw-r--r--   0        0        0    15406 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/_static/favicon.ico
+-rw-r--r--   0        0        0   104344 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/_static/logo.png
+-rw-r--r--   0        0        0      637 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/_static/theme_overrides.css
+-rw-r--r--   0        0        0      699 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/_static/version_switcher.json
+-rw-r--r--   0        0        0     8140 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/about/code_of_conduct.md
+-rw-r--r--   0        0        0      228 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/about/index.rst
+-rw-r--r--   0        0        0    11104 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/about/report_handling_manual.rst
+-rw-r--r--   0        0        0     3968 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/about/values.md
+-rw-r--r--   0        0        0    11358 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/conf.py
+-rw-r--r--   0        0        0       39 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/development/contribute.rst
+-rw-r--r--   0        0        0    11595 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/development/core_developer.md
+-rw-r--r--   0        0        0      196 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/development/index.rst
+-rw-r--r--   0        0        0    16311 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/branch_dropdown.png
+-rw-r--r--   0        0        0     4792 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/configure_git.rst
+-rw-r--r--   0        0        0    13819 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/development_workflow.rst
+-rw-r--r--   0        0        0      853 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/following_latest.rst
+-rw-r--r--   0        0        0    13092 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/forking_button.png
+-rw-r--r--   0        0        0     1216 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/forking_hell.rst
+-rw-r--r--   0        0        0      224 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/git_development.rst
+-rw-r--r--   0        0        0      599 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/git_install.rst
+-rw-r--r--   0        0        0      545 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/git_intro.rst
+-rw-r--r--   0        0        0     3235 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/git_links.inc
+-rw-r--r--   0        0        0     1766 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/git_resources.rst
+-rw-r--r--   0        0        0      239 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/index.rst
+-rw-r--r--   0        0        0     1477 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/known_projects.inc
+-rw-r--r--   0        0        0      113 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/links.inc
+-rw-r--r--   0        0        0     3072 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/maintainer_workflow.rst
+-rw-r--r--   0        0        0     4049 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/patching.rst
+-rw-r--r--   0        0        0    12893 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/pull_button.png
+-rw-r--r--   0        0        0     2035 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/set_up_fork.rst
+-rw-r--r--   0        0        0      215 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/gitwash/this_project.inc
+-rw-r--r--   0        0        0     2571 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/index.rst
+-rw-r--r--   0        0        0       54 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/license.md
+-rw-r--r--   0        0        0      289 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/release_notes/index.rst
+-rw-r--r--   0        0        0      252 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/release_notes/release_0.1.rst
+-rw-r--r--   0        0        0     1508 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/release_notes/release_dev.rst
+-rw-r--r--   0        0        0      621 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/release_notes/release_template.rst
+-rw-r--r--   0        0        0    12075 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/skips/0-skip-process.rst
+-rw-r--r--   0        0        0     8541 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/skips/1-governance.rst
+-rw-r--r--   0        0        0     6979 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/skips/2-values.rst
+-rw-r--r--   0        0        0    15188 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/skips/3-transition-to-v1.rst
+-rw-r--r--   0        0        0    14707 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/skips/4-transition-to-v2.rst
+-rw-r--r--   0        0        0    12925 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/skips/_static/skip-flowchart.png
+-rw-r--r--   0        0        0      250 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/skips/index.md
+-rw-r--r--   0        0        0     3109 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/skips/template.rst
+-rw-r--r--   0        0        0    10065 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/data_types.rst
+-rw-r--r--   0        0        0      694 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/geometrical_transform.rst
+-rw-r--r--   0        0        0     1545 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/getting_help.rst
+-rw-r--r--   0        0        0      362 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/getting_started.rst
+-rw-r--r--   0        0        0     3958 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/glossary.md
+-rw-r--r--   0        0        0      443 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/index.rst
+-rw-r--r--   0        0        0       34 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/install.rst
+-rw-r--r--   0        0        0    10525 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/numpy_images.rst
+-rw-r--r--   0        0        0     2364 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/plugins.rst
+-rw-r--r--   0        0        0     6632 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/transforming_image_data.rst
+-rw-r--r--   0        0        0     1920 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/tutorial_parallelization.rst
+-rw-r--r--   0        0        0     4764 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/tutorial_segmentation.rst
+-rw-r--r--   0        0        0      104 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/tutorials.rst
+-rw-r--r--   0        0        0     5018 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/video.rst
+-rw-r--r--   0        0        0     1054 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/source/user_guide/visualization.rst
+-rw-r--r--   0        0        0      200 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/tools/LICENSE.txt
+-rw-r--r--   0        0        0    16835 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/tools/apigen.py
+-rw-r--r--   0        0        0     1811 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/tools/build_modref_templates.py
+-rw-r--r--   0        0        0     4089 2024-05-10 08:56:51.000000 pysarpro-0.1.4/doc/tools/plot_pr.py
+-rw-r--r--   0        0        0     2701 2024-05-10 08:56:51.000000 pysarpro-0.1.4/meson.build
+-rw-r--r--   0        0        0     4545 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4647 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/__init__.py
+-rw-r--r--   0        0        0      135 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/__init__.pyi
+-rw-r--r--   0        0        0      778 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_build_utils/__init__.py
+-rw-r--r--   0        0        0      449 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_build_utils/copyfiles.py
+-rw-r--r--   0        0        0      672 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_build_utils/cythoner.py
+-rw-r--r--   0        0        0      528 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_build_utils/gcc_build_bitness.py
+-rw-r--r--   0        0        0       32 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_build_utils/link-version-pyinit.map
+-rw-r--r--   0        0        0     1651 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_build_utils/tempita.py
+-rw-r--r--   0        0        0      371 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_build_utils/version.py
+-rw-r--r--   0        0        0        0 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/__init__.py
+-rw-r--r--   0        0        0       94 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/_dependency_checks.py
+-rw-r--r--   0        0        0     1343 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/_geometry.py
+-rw-r--r--   0        0        0      764 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/_tempfile.py
+-rw-r--r--   0        0        0     5070 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/_warnings.py
+-rw-r--r--   0        0        0     4330 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/coord.py
+-rw-r--r--   0        0        0     1246 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/fast_exp.h
+-rw-r--r--   0        0        0      471 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/fast_exp.pxd
+-rw-r--r--   0        0        0      178 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/fast_exp.pyx
+-rw-r--r--   0        0        0     5321 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/filters.py
+-rw-r--r--   0        0        0      533 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/fused_numerics.pxd
+-rw-r--r--   0        0        0      470 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/geometry.pxd
+-rw-r--r--   0        0        0     2740 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/geometry.pyx
+-rw-r--r--   0        0        0    12483 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/interpolation.pxd
+-rw-r--r--   0        0        0      207 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/interpolation.pyx
+-rw-r--r--   0        0        0     1189 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/meson.build
+-rw-r--r--   0        0        0     3592 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/tester.py
+-rw-r--r--   0        0        0    10690 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/testing.py
+-rw-r--r--   0        0        0        0 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/tests/__init__.py
+-rw-r--r--   0        0        0      341 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/tests/meson.build
+-rw-r--r--   0        0        0     3050 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/tests/test_coord.py
+-rw-r--r--   0        0        0      490 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/tests/test_fast_exp.py
+-rw-r--r--   0        0        0     2120 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/tests/test_geometry.py
+-rw-r--r--   0        0        0     1139 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/tests/test_interpolation.py
+-rw-r--r--   0        0        0     1426 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/tests/test_safe_as_int.py
+-rw-r--r--   0        0        0     2952 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/tests/test_testing.py
+-rw-r--r--   0        0        0    20613 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/tests/test_utils.py
+-rw-r--r--   0        0        0     1078 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/tests/test_version_requirements.py
+-rw-r--r--   0        0        0     1256 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/tests/test_warnings.py
+-rw-r--r--   0        0        0      243 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/transform.pxd
+-rw-r--r--   0        0        0     1142 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/transform.pyx
+-rw-r--r--   0        0        0    33407 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/utils.py
+-rw-r--r--   0        0        0     5332 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/_shared/version_requirements.py
+-rw-r--r--   0        0        0      482 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/conftest.py
+-rw-r--r--   0        0        0      157 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/01-sar/meson.build
+-rw-r--r--   0        0        0   159872 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/01-sar/signal1_ac.npy
+-rw-r--r--   0        0        0    60480 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/01-sar/signal1_rc.npy
+-rw-r--r--   0        0        0   159872 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/01-sar/signal2_ac.npy
+-rw-r--r--   0        0        0    60480 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/01-sar/signal2_rc.npy
+-rw-r--r--   0        0        0      277 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/README.txt
+-rw-r--r--   0        0        0      384 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/__init__.pyi
+-rw-r--r--   0        0        0     2323 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/_binary_blobs.py
+-rw-r--r--   0        0        0    12773 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/_fetchers.py
+-rw-r--r--   0        0        0    22153 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/_registry.py
+-rw-r--r--   0        0        0   791555 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/astronaut.png
+-rw-r--r--   0        0        0   104344 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/logo.png
+-rw-r--r--   0        0        0      476 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/meson.build
+-rw-r--r--   0        0        0        0 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/tests/__init__.py
+-rw-r--r--   0        0        0      144 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/tests/meson.build
+-rw-r--r--   0        0        0     1526 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/data/tests/test_data.py
+-rw-r--r--   0        0        0     1790 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/__init__.py
+-rw-r--r--   0        0        0      570 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_image_stack.py
+-rw-r--r--   0        0        0     5898 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_io.py
+-rw-r--r--   0        0        0        0 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/__init__.py
+-rw-r--r--   0        0        0    13042 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/_colormixer.pyx
+-rw-r--r--   0        0        0     2114 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/_histograms.pyx
+-rw-r--r--   0        0        0       88 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/fits_plugin.ini
+-rw-r--r--   0        0        0     4408 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/fits_plugin.py
+-rw-r--r--   0        0        0       89 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/gdal_plugin.ini
+-rw-r--r--   0        0        0      349 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/gdal_plugin.py
+-rw-r--r--   0        0        0       88 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/imageio_plugin.ini
+-rw-r--r--   0        0        0      330 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/imageio_plugin.py
+-rw-r--r--   0        0        0       86 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/imread_plugin.ini
+-rw-r--r--   0        0        0      956 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/imread_plugin.py
+-rw-r--r--   0        0        0      123 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/matplotlib_plugin.ini
+-rw-r--r--   0        0        0     6402 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/matplotlib_plugin.py
+-rw-r--r--   0        0        0      916 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/meson.build
+-rw-r--r--   0        0        0       91 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/pil_plugin.ini
+-rw-r--r--   0        0        0     7843 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/pil_plugin.py
+-rw-r--r--   0        0        0       92 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/simpleitk_plugin.ini
+-rw-r--r--   0        0        0      531 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/simpleitk_plugin.py
+-rw-r--r--   0        0        0      110 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/tifffile_plugin.ini
+-rw-r--r--   0        0        0     2071 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/_plugins/tifffile_plugin.py
+-rw-r--r--   0        0        0    14923 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/collection.py
+-rw-r--r--   0        0        0    10378 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/manage_plugins.py
+-rw-r--r--   0        0        0      366 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/meson.build
+-rw-r--r--   0        0        0     2562 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/sift.py
+-rw-r--r--   0        0        0    47634 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/ste.py
+-rw-r--r--   0        0        0        0 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/tests/__init__.py
+-rw-r--r--   0        0        0      330 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/tests/meson.build
+-rw-r--r--   0        0        0      844 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/tests/test_fits.py
+-rw-r--r--   0        0        0      742 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/tests/test_histograms.py
+-rw-r--r--   0        0        0     1741 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/tests/test_imageio.py
+-rw-r--r--   0        0        0     1018 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/tests/test_imread.py
+-rw-r--r--   0        0        0     2711 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/tests/test_io.py
+-rw-r--r--   0        0        0     4206 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/tests/test_mpl_imshow.py
+-rw-r--r--   0        0        0     2289 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/tests/test_plugin.py
+-rw-r--r--   0        0        0     3337 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/tests/test_sift.py
+-rw-r--r--   0        0        0     1203 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/tests/test_simpleitk.py
+-rw-r--r--   0        0        0     1489 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/tests/test_tifffile.py
+-rw-r--r--   0        0        0     1283 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/io/util.py
+-rw-r--r--   0        0        0     4860 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/meson.build
+-rw-r--r--   0        0        0       16 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/models/__init__.py
+-rw-r--r--   0        0        0      264 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/models/meson.build
+-rw-r--r--   0        0        0        0 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/models/predict_model.py
+-rw-r--r--   0        0        0        0 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/models/train_model.py
+-rw-r--r--   0        0        0        0 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/py.typed
+-rw-r--r--   0        0        0     1246 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/__init__.py
+-rw-r--r--   0        0        0     2560 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/_invert.py
+-rw-r--r--   0        0        0     1569 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/_label.py
+-rw-r--r--   0        0        0     6691 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/_map_array.py
+-rw-r--r--   0        0        0     3885 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/_regular_grid.py
+-rw-r--r--   0        0        0      968 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/_remap.pyx
+-rw-r--r--   0        0        0     2234 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/_slice_along_axes.py
+-rw-r--r--   0        0        0     7650 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/apply_parallel.py
+-rw-r--r--   0        0        0     2486 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/arraycrop.py
+-rw-r--r--   0        0        0     2058 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/compare.py
+-rw-r--r--   0        0        0    18089 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/dtype.py
+-rw-r--r--   0        0        0      598 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/lookfor.py
+-rw-r--r--   0        0        0      744 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/meson.build
+-rw-r--r--   0        0        0     8692 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/noise.py
+-rw-r--r--   0        0        0     7831 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/shape.py
+-rw-r--r--   0        0        0        0 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/tests/__init__.py
+-rw-r--r--   0        0        0      378 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/tests/meson.build
+-rw-r--r--   0        0        0     1850 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/tests/test_arraycrop.py
+-rw-r--r--   0        0        0     2393 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/tests/test_compare.py
+-rw-r--r--   0        0        0     5123 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/tests/test_dtype.py
+-rw-r--r--   0        0        0     2418 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/tests/test_invert.py
+-rw-r--r--   0        0        0     1792 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/tests/test_labels.py
+-rw-r--r--   0        0        0     2900 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/tests/test_map_array.py
+-rw-r--r--   0        0        0     7799 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/tests/test_random_noise.py
+-rw-r--r--   0        0        0      982 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/tests/test_regular_grid.py
+-rw-r--r--   0        0        0     4551 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/tests/test_shape.py
+-rw-r--r--   0        0        0     1680 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/tests/test_slice_along_axes.py
+-rw-r--r--   0        0        0     1102 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/tests/test_unique_rows.py
+-rw-r--r--   0        0        0     1516 2024-05-10 08:56:51.000000 pysarpro-0.1.4/pysarpro/util/unique.py
+-rw-r--r--   0        0        0      823 2024-05-10 08:56:51.000000 pysarpro-0.1.4/requirements/README.md
+-rw-r--r--   0        0        0       16 2024-05-10 08:56:51.000000 pysarpro-0.1.4/requirements/_release_tools.txt
+-rw-r--r--   0        0        0      234 2024-05-10 08:56:51.000000 pysarpro-0.1.4/requirements/build.txt
+-rw-r--r--   0        0        0      137 2024-05-10 08:56:51.000000 pysarpro-0.1.4/requirements/data.txt
+-rw-r--r--   0        0        0      238 2024-05-10 08:56:51.000000 pysarpro-0.1.4/requirements/default.txt
+-rw-r--r--   0        0        0      174 2024-05-10 08:56:51.000000 pysarpro-0.1.4/requirements/developer.txt
+-rw-r--r--   0        0        0      435 2024-05-10 08:56:51.000000 pysarpro-0.1.4/requirements/docs.txt
+-rw-r--r--   0        0        0      259 2024-05-10 08:56:51.000000 pysarpro-0.1.4/requirements/optional.txt
+-rw-r--r--   0        0        0      241 2024-05-10 08:56:51.000000 pysarpro-0.1.4/requirements/test.txt
+-rw-r--r--   0        0        0       83 2024-05-10 08:56:51.000000 pysarpro-0.1.4/requirements.txt
+-rw-r--r--   0        0        0     2121 2024-05-10 08:56:51.000000 pysarpro-0.1.4/tools/check_sdist.py
+-rw-r--r--   0        0        0     1177 2024-05-10 08:56:51.000000 pysarpro-0.1.4/tools/generate_requirements.py
+-rwxr-xr-x   0        0        0     1282 2024-05-10 08:56:51.000000 pysarpro-0.1.4/tools/github/before_install.sh
+-rwxr-xr-x   0        0        0     1378 2024-05-10 08:56:51.000000 pysarpro-0.1.4/tools/github/script.sh
+-rw-r--r--   0        0        0      260 2024-05-10 08:56:51.000000 pysarpro-0.1.4/tools/header.py
+-rw-r--r--   0        0        0     1652 2024-05-10 08:56:51.000000 pysarpro-0.1.4/tools/mailmap.py
+-rw-r--r--   0        0        0   158924 2024-05-10 08:56:51.000000 pysarpro-0.1.4/tools/precompute/mc_meta/LookUpTable.h
+-rw-r--r--   0        0        0      454 2024-05-10 08:56:51.000000 pysarpro-0.1.4/tools/precompute/mc_meta/README.md
+-rw-r--r--   0        0        0     3680 2024-05-10 08:56:51.000000 pysarpro-0.1.4/tools/precompute/mc_meta/createluts.py
+-rw-r--r--   0        0        0     2430 2024-05-10 08:56:51.000000 pysarpro-0.1.4/tools/precompute/mc_meta/visual_test.py
+-rw-r--r--   0        0        0     3865 2024-05-10 08:56:51.000000 pysarpro-0.1.4/tools/precompute/moments_sympy.py
+-rw-r--r--   0        0        0      233 2024-05-10 08:56:51.000000 pysarpro-0.1.4/tools/rm_pyx_assoc_c_cpp.sh
+-rw-r--r--   0        0        0      711 2024-05-10 08:56:51.000000 pysarpro-0.1.4/tools/upload_wheels.sh
+-rw-r--r--   0        0        0    10736 2024-05-10 09:09:37.440024 pysarpro-0.1.4/PKG-INFO
```

### Comparing `pysarpro-0.1.3/.spin/cmds.py` & `pysarpro-0.1.4/.spin/cmds.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/CONTRIBUTING.rst` & `pysarpro-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/CONTRIBUTORS.txt` & `pysarpro-0.1.4/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/INSTALL.rst` & `pysarpro-0.1.4/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/LICENSE.txt` & `pysarpro-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/MANIFEST.in` & `pysarpro-0.1.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/Makefile` & `pysarpro-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/README.md` & `pysarpro-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/RELEASE.txt` & `pysarpro-0.1.4/RELEASE.txt`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/asv.conf.json` & `pysarpro-0.1.4/asv.conf.json`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/Makefile` & `pysarpro-0.1.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/ext/doi_role.py` & `pysarpro-0.1.4/doc/ext/doi_role.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/ext/pysarpro_extensions.py` & `pysarpro-0.1.4/doc/ext/pysarpro_extensions.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/gh-pages.py` & `pysarpro-0.1.4/doc/gh-pages.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/_static/docversions.js` & `pysarpro-0.1.4/doc/source/_static/docversions.js`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/_static/favicon.ico` & `pysarpro-0.1.4/doc/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/_static/logo.png` & `pysarpro-0.1.4/doc/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/_static/theme_overrides.css` & `pysarpro-0.1.4/doc/source/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/_static/version_switcher.json` & `pysarpro-0.1.4/doc/source/_static/version_switcher.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {'1': "{'version': '0.1.4'}",*

 * * '3': "{'name': '0.1.3'}",*

 * * 'insert': "[(2, OrderedDict([('name', '0.1'), ('version', '0.1.4'), ('url', "*

 * *           "'https://pol-insar.github.io/docs/stable/'), ('preferred', True)]))]"}*

```diff
@@ -4,20 +4,26 @@
         "url": "https://pol-insar.github.io/docs/dev/",
         "version": "dev"
     },
     {
         "name": "0.1 (stable)",
         "preferred": true,
         "url": "https://pol-insar.github.io/docs/stable/",
-        "version": "0.1.3"
+        "version": "0.1.4"
     },
     {
         "name": "0.1",
         "preferred": true,
         "url": "https://pol-insar.github.io/docs/stable/",
+        "version": "0.1.4"
+    },
+    {
+        "name": "0.1.3",
+        "preferred": true,
+        "url": "https://pol-insar.github.io/docs/stable/",
         "version": "0.1.3"
     },
     {
         "name": "0.1.2",
         "url": "https://pol-insar.github.io/docs/0.1/",
         "version": "0.1.2"
     }
```

### Comparing `pysarpro-0.1.3/doc/source/about/code_of_conduct.md` & `pysarpro-0.1.4/doc/source/about/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/about/report_handling_manual.rst` & `pysarpro-0.1.4/doc/source/about/report_handling_manual.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/about/values.md` & `pysarpro-0.1.4/doc/source/about/values.md`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/conf.py` & `pysarpro-0.1.4/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/development/core_developer.md` & `pysarpro-0.1.4/doc/source/development/core_developer.md`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/branch_dropdown.png` & `pysarpro-0.1.4/doc/source/gitwash/branch_dropdown.png`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/configure_git.rst` & `pysarpro-0.1.4/doc/source/gitwash/configure_git.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/development_workflow.rst` & `pysarpro-0.1.4/doc/source/gitwash/development_workflow.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/following_latest.rst` & `pysarpro-0.1.4/doc/source/gitwash/following_latest.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/forking_button.png` & `pysarpro-0.1.4/doc/source/gitwash/forking_button.png`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/forking_hell.rst` & `pysarpro-0.1.4/doc/source/gitwash/forking_hell.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/git_install.rst` & `pysarpro-0.1.4/doc/source/gitwash/git_install.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/git_intro.rst` & `pysarpro-0.1.4/doc/source/gitwash/git_intro.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/git_links.inc` & `pysarpro-0.1.4/doc/source/gitwash/git_links.inc`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/git_resources.rst` & `pysarpro-0.1.4/doc/source/gitwash/git_resources.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/known_projects.inc` & `pysarpro-0.1.4/doc/source/gitwash/known_projects.inc`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/maintainer_workflow.rst` & `pysarpro-0.1.4/doc/source/gitwash/maintainer_workflow.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/patching.rst` & `pysarpro-0.1.4/doc/source/gitwash/patching.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/pull_button.png` & `pysarpro-0.1.4/doc/source/gitwash/pull_button.png`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/gitwash/set_up_fork.rst` & `pysarpro-0.1.4/doc/source/gitwash/set_up_fork.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/index.rst` & `pysarpro-0.1.4/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/release_notes/release_dev.rst` & `pysarpro-0.1.4/doc/source/release_notes/release_dev.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/release_notes/release_template.rst` & `pysarpro-0.1.4/doc/source/release_notes/release_template.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/skips/0-skip-process.rst` & `pysarpro-0.1.4/doc/source/skips/0-skip-process.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/skips/1-governance.rst` & `pysarpro-0.1.4/doc/source/skips/1-governance.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/skips/2-values.rst` & `pysarpro-0.1.4/doc/source/skips/2-values.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/skips/3-transition-to-v1.rst` & `pysarpro-0.1.4/doc/source/skips/3-transition-to-v1.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/skips/4-transition-to-v2.rst` & `pysarpro-0.1.4/doc/source/skips/4-transition-to-v2.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/skips/_static/skip-flowchart.png` & `pysarpro-0.1.4/doc/source/skips/_static/skip-flowchart.png`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/skips/template.rst` & `pysarpro-0.1.4/doc/source/skips/template.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/user_guide/data_types.rst` & `pysarpro-0.1.4/doc/source/user_guide/data_types.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/user_guide/geometrical_transform.rst` & `pysarpro-0.1.4/doc/source/user_guide/geometrical_transform.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/user_guide/getting_help.rst` & `pysarpro-0.1.4/doc/source/user_guide/getting_help.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/user_guide/glossary.md` & `pysarpro-0.1.4/doc/source/user_guide/glossary.md`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/user_guide/numpy_images.rst` & `pysarpro-0.1.4/doc/source/user_guide/numpy_images.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/user_guide/plugins.rst` & `pysarpro-0.1.4/doc/source/user_guide/plugins.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/user_guide/transforming_image_data.rst` & `pysarpro-0.1.4/doc/source/user_guide/transforming_image_data.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/user_guide/tutorial_parallelization.rst` & `pysarpro-0.1.4/doc/source/user_guide/tutorial_parallelization.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/user_guide/tutorial_segmentation.rst` & `pysarpro-0.1.4/doc/source/user_guide/tutorial_segmentation.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/user_guide/video.rst` & `pysarpro-0.1.4/doc/source/user_guide/video.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/source/user_guide/visualization.rst` & `pysarpro-0.1.4/doc/source/user_guide/visualization.rst`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/tools/apigen.py` & `pysarpro-0.1.4/doc/tools/apigen.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/tools/build_modref_templates.py` & `pysarpro-0.1.4/doc/tools/build_modref_templates.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/doc/tools/plot_pr.py` & `pysarpro-0.1.4/doc/tools/plot_pr.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/meson.build` & `pysarpro-0.1.4/meson.build`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pyproject.toml` & `pysarpro-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/__init__.py` & `pysarpro-0.1.4/pysarpro/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 img_as_bool
     Convert an image to boolean format, with values either True or False.
 dtype_limits
     Return intensity limits, i.e. (min, max) tuple, of the image's dtype.
 
 """
 
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 from ._shared.version_requirements import ensure_python_version
 
 ensure_python_version((3, 8))
 
 import lazy_loader as lazy
```

### Comparing `pysarpro-0.1.3/pysarpro/_build_utils/__init__.py` & `pysarpro-0.1.4/pysarpro/_build_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_build_utils/cythoner.py` & `pysarpro-0.1.4/pysarpro/_build_utils/cythoner.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_build_utils/gcc_build_bitness.py` & `pysarpro-0.1.4/pysarpro/_build_utils/gcc_build_bitness.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_build_utils/tempita.py` & `pysarpro-0.1.4/pysarpro/_build_utils/tempita.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/_geometry.py` & `pysarpro-0.1.4/pysarpro/_shared/_geometry.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/_tempfile.py` & `pysarpro-0.1.4/pysarpro/_shared/_tempfile.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/_warnings.py` & `pysarpro-0.1.4/pysarpro/_shared/_warnings.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/coord.py` & `pysarpro-0.1.4/pysarpro/_shared/coord.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/fast_exp.h` & `pysarpro-0.1.4/pysarpro/_shared/fast_exp.h`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/filters.py` & `pysarpro-0.1.4/pysarpro/_shared/filters.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/fused_numerics.pxd` & `pysarpro-0.1.4/pysarpro/_shared/fused_numerics.pxd`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/geometry.pyx` & `pysarpro-0.1.4/pysarpro/_shared/geometry.pyx`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/interpolation.pxd` & `pysarpro-0.1.4/pysarpro/_shared/interpolation.pxd`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/meson.build` & `pysarpro-0.1.4/pysarpro/_shared/meson.build`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/tester.py` & `pysarpro-0.1.4/pysarpro/_shared/tester.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/testing.py` & `pysarpro-0.1.4/pysarpro/_shared/testing.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/tests/test_coord.py` & `pysarpro-0.1.4/pysarpro/_shared/tests/test_coord.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/tests/test_geometry.py` & `pysarpro-0.1.4/pysarpro/_shared/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/tests/test_interpolation.py` & `pysarpro-0.1.4/pysarpro/_shared/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/tests/test_safe_as_int.py` & `pysarpro-0.1.4/pysarpro/_shared/tests/test_safe_as_int.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/tests/test_testing.py` & `pysarpro-0.1.4/pysarpro/_shared/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/tests/test_utils.py` & `pysarpro-0.1.4/pysarpro/_shared/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/tests/test_version_requirements.py` & `pysarpro-0.1.4/pysarpro/_shared/tests/test_version_requirements.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/tests/test_warnings.py` & `pysarpro-0.1.4/pysarpro/_shared/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/transform.pyx` & `pysarpro-0.1.4/pysarpro/_shared/transform.pyx`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/utils.py` & `pysarpro-0.1.4/pysarpro/_shared/utils.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/_shared/version_requirements.py` & `pysarpro-0.1.4/pysarpro/_shared/version_requirements.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/data/01-sar/signal1_ac.npy` & `pysarpro-0.1.4/pysarpro/data/01-sar/signal1_ac.npy`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/data/01-sar/signal1_rc.npy` & `pysarpro-0.1.4/pysarpro/data/01-sar/signal1_rc.npy`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/data/01-sar/signal2_ac.npy` & `pysarpro-0.1.4/pysarpro/data/01-sar/signal2_ac.npy`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/data/01-sar/signal2_rc.npy` & `pysarpro-0.1.4/pysarpro/data/01-sar/signal2_rc.npy`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/data/_binary_blobs.py` & `pysarpro-0.1.4/pysarpro/data/_binary_blobs.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/data/_fetchers.py` & `pysarpro-0.1.4/pysarpro/data/_fetchers.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 import os
 import os.path as osp
 import re
 import shutil
 import zipfile
+from pathlib import Path
 
 from .. import __version__
 from ._registry import registry, registry_urls
 
 _LEGACY_DATA_DIR = osp.dirname(__file__)
 _DISTRIBUTION_DIR = osp.dirname(_LEGACY_DATA_DIR)
 
@@ -286,27 +287,30 @@
             directory = osp.expanduser(directory)
             _image_fetcher.path = directory
         _ensure_cache_dir(target_dir=_image_fetcher.path)
 
         for data_filename in _image_fetcher.registry:
             if pattern is not None and not re.search(pattern, data_filename):
                 continue
+            # If the directory of unzipped folder exist, skipp downloading the data zip file
+            if Path(directory).joinpath(data_filename).with_suffix('').is_dir():
+                continue
             file_path = _fetch(data_filename)
 
             # Copy to `directory` or implicit cache if it is not already there
             if not file_path.startswith(str(_image_fetcher.path)):
                 dest_path = osp.join(_image_fetcher.path, data_filename)
                 os.makedirs(osp.dirname(dest_path), exist_ok=True)
                 shutil.copy2(file_path, dest_path)
 
             # If the file is a zip file, unzip it and remove the zipped file
             if data_filename.endswith('.zip'):
-                with zipfile.ZipFile(dest_path, 'r') as zip_ref:
-                    zip_ref.extractall(osp.dirname(dest_path))
-                os.remove(dest_path)
+                with zipfile.ZipFile(file_path, 'r') as zip_ref:
+                    zip_ref.extractall(osp.dirname(file_path))
+                os.remove(file_path)
     finally:
         _image_fetcher.path = old_dir
 
 
 def lbp_frontal_face_cascade_filename():
     """Return the path to the XML file containing the weak classifier cascade.
```

### Comparing `pysarpro-0.1.3/pysarpro/data/_registry.py` & `pysarpro-0.1.4/pysarpro/data/_registry.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/data/astronaut.png` & `pysarpro-0.1.4/pysarpro/data/astronaut.png`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/data/logo.png` & `pysarpro-0.1.4/pysarpro/data/logo.png`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/data/tests/test_data.py` & `pysarpro-0.1.4/pysarpro/data/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/__init__.py` & `pysarpro-0.1.4/pysarpro/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/_image_stack.py` & `pysarpro-0.1.4/pysarpro/io/_image_stack.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/_io.py` & `pysarpro-0.1.4/pysarpro/io/_io.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/_plugins/_colormixer.pyx` & `pysarpro-0.1.4/pysarpro/io/_plugins/_colormixer.pyx`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/_plugins/_histograms.pyx` & `pysarpro-0.1.4/pysarpro/io/_plugins/_histograms.pyx`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/_plugins/fits_plugin.py` & `pysarpro-0.1.4/pysarpro/io/_plugins/fits_plugin.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/_plugins/imread_plugin.py` & `pysarpro-0.1.4/pysarpro/io/_plugins/imread_plugin.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/_plugins/matplotlib_plugin.py` & `pysarpro-0.1.4/pysarpro/io/_plugins/matplotlib_plugin.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/_plugins/meson.build` & `pysarpro-0.1.4/pysarpro/io/_plugins/meson.build`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/_plugins/pil_plugin.py` & `pysarpro-0.1.4/pysarpro/io/_plugins/pil_plugin.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/_plugins/simpleitk_plugin.py` & `pysarpro-0.1.4/pysarpro/io/_plugins/simpleitk_plugin.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/_plugins/tifffile_plugin.py` & `pysarpro-0.1.4/pysarpro/io/_plugins/tifffile_plugin.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/collection.py` & `pysarpro-0.1.4/pysarpro/io/collection.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/manage_plugins.py` & `pysarpro-0.1.4/pysarpro/io/manage_plugins.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/sift.py` & `pysarpro-0.1.4/pysarpro/io/sift.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/ste.py` & `pysarpro-0.1.4/pysarpro/io/ste.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/tests/test_fits.py` & `pysarpro-0.1.4/pysarpro/io/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/tests/test_histograms.py` & `pysarpro-0.1.4/pysarpro/io/tests/test_histograms.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/tests/test_imageio.py` & `pysarpro-0.1.4/pysarpro/io/tests/test_imageio.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/tests/test_imread.py` & `pysarpro-0.1.4/pysarpro/io/tests/test_imread.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/tests/test_io.py` & `pysarpro-0.1.4/pysarpro/io/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/tests/test_mpl_imshow.py` & `pysarpro-0.1.4/pysarpro/io/tests/test_mpl_imshow.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/tests/test_plugin.py` & `pysarpro-0.1.4/pysarpro/io/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/tests/test_sift.py` & `pysarpro-0.1.4/pysarpro/io/tests/test_sift.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/tests/test_simpleitk.py` & `pysarpro-0.1.4/pysarpro/io/tests/test_simpleitk.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/tests/test_tifffile.py` & `pysarpro-0.1.4/pysarpro/io/tests/test_tifffile.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/io/util.py` & `pysarpro-0.1.4/pysarpro/io/util.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/meson.build` & `pysarpro-0.1.4/pysarpro/meson.build`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/__init__.py` & `pysarpro-0.1.4/pysarpro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/_invert.py` & `pysarpro-0.1.4/pysarpro/util/_invert.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/_label.py` & `pysarpro-0.1.4/pysarpro/util/_label.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/_map_array.py` & `pysarpro-0.1.4/pysarpro/util/_map_array.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/_regular_grid.py` & `pysarpro-0.1.4/pysarpro/util/_regular_grid.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/_remap.pyx` & `pysarpro-0.1.4/pysarpro/util/_remap.pyx`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/_slice_along_axes.py` & `pysarpro-0.1.4/pysarpro/util/_slice_along_axes.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/apply_parallel.py` & `pysarpro-0.1.4/pysarpro/util/apply_parallel.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/arraycrop.py` & `pysarpro-0.1.4/pysarpro/util/arraycrop.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/compare.py` & `pysarpro-0.1.4/pysarpro/util/compare.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/dtype.py` & `pysarpro-0.1.4/pysarpro/util/dtype.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/lookfor.py` & `pysarpro-0.1.4/pysarpro/util/lookfor.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/meson.build` & `pysarpro-0.1.4/pysarpro/util/meson.build`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/noise.py` & `pysarpro-0.1.4/pysarpro/util/noise.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/shape.py` & `pysarpro-0.1.4/pysarpro/util/shape.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/tests/test_arraycrop.py` & `pysarpro-0.1.4/pysarpro/util/tests/test_arraycrop.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/tests/test_compare.py` & `pysarpro-0.1.4/pysarpro/util/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/tests/test_dtype.py` & `pysarpro-0.1.4/pysarpro/util/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/tests/test_invert.py` & `pysarpro-0.1.4/pysarpro/util/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/tests/test_labels.py` & `pysarpro-0.1.4/pysarpro/util/tests/test_labels.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/tests/test_map_array.py` & `pysarpro-0.1.4/pysarpro/util/tests/test_map_array.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/tests/test_random_noise.py` & `pysarpro-0.1.4/pysarpro/util/tests/test_random_noise.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/tests/test_regular_grid.py` & `pysarpro-0.1.4/pysarpro/util/tests/test_regular_grid.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/tests/test_shape.py` & `pysarpro-0.1.4/pysarpro/util/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/tests/test_slice_along_axes.py` & `pysarpro-0.1.4/pysarpro/util/tests/test_slice_along_axes.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/tests/test_unique_rows.py` & `pysarpro-0.1.4/pysarpro/util/tests/test_unique_rows.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/pysarpro/util/unique.py` & `pysarpro-0.1.4/pysarpro/util/unique.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/requirements/README.md` & `pysarpro-0.1.4/requirements/README.md`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/tools/check_sdist.py` & `pysarpro-0.1.4/tools/check_sdist.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/tools/generate_requirements.py` & `pysarpro-0.1.4/tools/generate_requirements.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/tools/github/before_install.sh` & `pysarpro-0.1.4/tools/github/before_install.sh`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/tools/github/script.sh` & `pysarpro-0.1.4/tools/github/script.sh`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/tools/mailmap.py` & `pysarpro-0.1.4/tools/mailmap.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/tools/precompute/mc_meta/LookUpTable.h` & `pysarpro-0.1.4/tools/precompute/mc_meta/LookUpTable.h`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/tools/precompute/mc_meta/createluts.py` & `pysarpro-0.1.4/tools/precompute/mc_meta/createluts.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/tools/precompute/mc_meta/visual_test.py` & `pysarpro-0.1.4/tools/precompute/mc_meta/visual_test.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/tools/precompute/moments_sympy.py` & `pysarpro-0.1.4/tools/precompute/moments_sympy.py`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/tools/upload_wheels.sh` & `pysarpro-0.1.4/tools/upload_wheels.sh`

 * *Files identical despite different names*

### Comparing `pysarpro-0.1.3/PKG-INFO` & `pysarpro-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysarpro
-Version: 0.1.3
+Version: 0.1.4
 Summary: SAR processing in Python
 Home-page: https://pol-insar.github.io
 Maintainer-Email: pysarpro developers <pysarpro-core@@imansour.net>
 License: Files: *
         Copyright: 2021-2023 the Pol-InSAR team
         License: BSD-3-Clause
```

