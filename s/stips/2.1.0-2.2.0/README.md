# Comparing `tmp/stips-2.1.0.tar.gz` & `tmp/stips-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stips-2.1.0.tar", last modified: Wed Nov 15 19:24:05 2023, max compression
+gzip compressed data, was "stips-2.2.0.tar", last modified: Fri May 10 13:25:57 2024, max compression
```

## Comparing `stips-2.1.0.tar` & `stips-2.2.0.tar`

### file list

```diff
@@ -1,142 +1,107 @@
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.320165 stips-2.1.0/
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.243959 stips-2.1.0/.git/
--rw-r--r--   0 jotor     (2330)     1031       23 2023-11-15 18:57:29.000000 stips-2.1.0/.git/HEAD
--rw-r--r--   0 jotor     (2330)     1031      319 2023-11-15 18:57:29.000000 stips-2.1.0/.git/config
--rw-r--r--   0 jotor     (2330)     1031       73 2023-11-15 18:57:21.000000 stips-2.1.0/.git/description
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.251652 stips-2.1.0/.git/hooks/
--rwxr-xr-x   0 jotor     (2330)     1031      478 2023-11-15 18:57:21.000000 stips-2.1.0/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 jotor     (2330)     1031      896 2023-11-15 18:57:21.000000 stips-2.1.0/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 jotor     (2330)     1031     3327 2023-11-15 18:57:21.000000 stips-2.1.0/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 jotor     (2330)     1031      189 2023-11-15 18:57:21.000000 stips-2.1.0/.git/hooks/post-update.sample
--rwxr-xr-x   0 jotor     (2330)     1031      424 2023-11-15 18:57:21.000000 stips-2.1.0/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 jotor     (2330)     1031     1638 2023-11-15 18:57:21.000000 stips-2.1.0/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 jotor     (2330)     1031      416 2023-11-15 18:57:21.000000 stips-2.1.0/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 jotor     (2330)     1031     1348 2023-11-15 18:57:21.000000 stips-2.1.0/.git/hooks/pre-push.sample
--rwxr-xr-x   0 jotor     (2330)     1031     4898 2023-11-15 18:57:21.000000 stips-2.1.0/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 jotor     (2330)     1031      544 2023-11-15 18:57:21.000000 stips-2.1.0/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 jotor     (2330)     1031     1492 2023-11-15 18:57:21.000000 stips-2.1.0/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 jotor     (2330)     1031     3610 2023-11-15 18:57:21.000000 stips-2.1.0/.git/hooks/update.sample
--rw-r--r--   0 jotor     (2330)     1031     7850 2023-11-15 18:57:30.000000 stips-2.1.0/.git/index
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.252192 stips-2.1.0/.git/info/
--rw-r--r--   0 jotor     (2330)     1031      240 2023-11-15 18:57:21.000000 stips-2.1.0/.git/info/exclude
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.252874 stips-2.1.0/.git/logs/
--rw-r--r--   0 jotor     (2330)     1031      206 2023-11-15 18:57:29.000000 stips-2.1.0/.git/logs/HEAD
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.227059 stips-2.1.0/.git/logs/refs/
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.253457 stips-2.1.0/.git/logs/refs/heads/
--rw-r--r--   0 jotor     (2330)     1031      206 2023-11-15 18:57:29.000000 stips-2.1.0/.git/logs/refs/heads/master
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.227291 stips-2.1.0/.git/logs/refs/remotes/
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.254044 stips-2.1.0/.git/logs/refs/remotes/origin/
--rw-r--r--   0 jotor     (2330)     1031      206 2023-11-15 18:57:29.000000 stips-2.1.0/.git/logs/refs/remotes/origin/HEAD
--rw-r--r--   0 jotor     (2330)     1031      855 2023-11-15 18:57:29.000000 stips-2.1.0/.git/packed-refs
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.228161 stips-2.1.0/.git/refs/
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.254627 stips-2.1.0/.git/refs/heads/
--rw-r--r--   0 jotor     (2330)     1031       41 2023-11-15 18:57:29.000000 stips-2.1.0/.git/refs/heads/master
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.228299 stips-2.1.0/.git/refs/remotes/
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.255180 stips-2.1.0/.git/refs/remotes/origin/
--rw-r--r--   0 jotor     (2330)     1031       32 2023-11-15 18:57:29.000000 stips-2.1.0/.git/refs/remotes/origin/HEAD
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.228642 stips-2.1.0/.github/
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.255763 stips-2.1.0/.github/workflows/
--rw-r--r--   0 jotor     (2330)     1031     1682 2023-11-15 18:57:29.000000 stips-2.1.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 jotor     (2330)     1031     3045 2023-11-15 18:57:29.000000 stips-2.1.0/.gitignore
--rw-r--r--   0 jotor     (2330)     1031      565 2023-11-15 18:57:29.000000 stips-2.1.0/.readthedocs.yaml
--rw-r--r--   0 jotor     (2330)     1031      282 2023-11-15 18:57:29.000000 stips-2.1.0/.rtd-environment.yml
--rw-r--r--   0 jotor     (2330)     1031     2952 2023-11-15 18:57:29.000000 stips-2.1.0/CHANGES.rst
--rw-r--r--   0 jotor     (2330)     1031      266 2023-11-15 18:57:29.000000 stips-2.1.0/CITATION
--rw-r--r--   0 jotor     (2330)     1031     3207 2023-11-15 18:57:29.000000 stips-2.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jotor     (2330)     1031      721 2023-11-15 18:57:29.000000 stips-2.1.0/CONTRIBUTING.md
--rw-r--r--   0 jotor     (2330)     1031      673 2023-11-15 18:57:29.000000 stips-2.1.0/Dockerfile
--rw-r--r--   0 jotor     (2330)     1031      376 2023-11-15 18:57:29.000000 stips-2.1.0/MANIFEST.in
--rw-r--r--   0 jotor     (2330)     1031      753 2023-11-15 19:24:05.319876 stips-2.1.0/PKG-INFO
--rw-r--r--   0 jotor     (2330)     1031     2352 2023-11-15 18:57:29.000000 stips-2.1.0/README.md
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.262853 stips-2.1.0/docs/
--rw-r--r--   0 jotor     (2330)     1031     4810 2023-11-15 18:57:29.000000 stips-2.1.0/docs/Makefile
--rw-r--r--   0 jotor     (2330)     1031     9635 2023-11-15 18:57:29.000000 stips-2.1.0/docs/basic_tutorial.rst
--rw-r--r--   0 jotor     (2330)     1031     2865 2023-11-15 18:57:29.000000 stips-2.1.0/docs/bugs.rst
--rw-r--r--   0 jotor     (2330)     1031     7430 2023-11-15 18:57:29.000000 stips-2.1.0/docs/conf.py
--rw-r--r--   0 jotor     (2330)     1031     2355 2023-11-15 18:57:29.000000 stips-2.1.0/docs/examples.rst
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.263527 stips-2.1.0/docs/exts/
--rw-r--r--   0 jotor     (2330)     1031     3319 2023-11-15 18:57:29.000000 stips-2.1.0/docs/exts/numfig.py
--rw-r--r--   0 jotor     (2330)     1031      164 2023-11-15 18:57:29.000000 stips-2.1.0/docs/help.rst
--rw-r--r--   0 jotor     (2330)     1031     2227 2023-11-15 18:57:29.000000 stips-2.1.0/docs/index.rst
--rw-r--r--   0 jotor     (2330)     1031     5572 2023-11-15 18:57:29.000000 stips-2.1.0/docs/installation.rst
--rw-r--r--   0 jotor     (2330)     1031     4513 2023-11-15 18:57:29.000000 stips-2.1.0/docs/make.bat
--rw-r--r--   0 jotor     (2330)     1031      141 2023-11-15 18:57:29.000000 stips-2.1.0/docs/requirements.txt
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.267247 stips-2.1.0/docs/roman_figures/
--rw-r--r--   0 jotor     (2330)     1031   415382 2023-11-15 18:57:29.000000 stips-2.1.0/docs/roman_figures/stips_basic_tutorial.png
--rw-r--r--   0 jotor     (2330)     1031   404340 2023-11-15 18:57:29.000000 stips-2.1.0/docs/roman_figures/stips_demo.png
--rw-r--r--   0 jotor     (2330)     1031      141 2023-11-15 18:57:29.000000 stips-2.1.0/docs/rtd-pip-requirements
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.269984 stips-2.1.0/docs/using_stips/
--rw-r--r--   0 jotor     (2330)     1031     8768 2023-11-15 18:57:29.000000 stips-2.1.0/docs/using_stips/catalogue_formats.rst
--rw-r--r--   0 jotor     (2330)     1031     7358 2023-11-15 18:57:29.000000 stips-2.1.0/docs/using_stips/config_file.rst
--rw-r--r--   0 jotor     (2330)     1031     1135 2023-11-15 18:57:29.000000 stips-2.1.0/docs/using_stips/psf_grid.rst
--rw-r--r--   0 jotor     (2330)     1031      203 2023-11-15 18:57:29.000000 stips-2.1.0/docs/using_stips.rst
--rw-r--r--   0 jotor     (2330)     1031     1676 2023-11-15 18:57:29.000000 stips-2.1.0/environment.yml
--rw-r--r--   0 jotor     (2330)     1031     2225 2023-11-15 18:57:29.000000 stips-2.1.0/environment_dev.yml
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.271720 stips-2.1.0/licenses/
--rw-r--r--   0 jotor     (2330)     1031     1539 2023-11-15 18:57:29.000000 stips-2.1.0/licenses/LICENSE.rst
--rw-r--r--   0 jotor     (2330)     1031      372 2023-11-15 18:57:29.000000 stips-2.1.0/licenses/README.rst
--rw-r--r--   0 jotor     (2330)     1031     1659 2023-11-15 18:57:29.000000 stips-2.1.0/licenses/TEMPLATE_LICENCE.rst
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.274537 stips-2.1.0/notebooks/
--rw-r--r--   0 jotor     (2330)     1031    23150 2023-11-15 18:57:29.000000 stips-2.1.0/notebooks/STIPS Advanced I – Further Observations, Noise and Distortion.ipynb
--rw-r--r--   0 jotor     (2330)     1031    12688 2023-11-15 18:57:29.000000 stips-2.1.0/notebooks/STIPS Advanced II - PSFs.ipynb
--rw-r--r--   0 jotor     (2330)     1031    13384 2023-11-15 18:57:29.000000 stips-2.1.0/notebooks/STIPS Basic Tutorial.ipynb
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.275309 stips-2.1.0/notebooks/notebooks_data/
--rw-r--r--   0 jotor     (2330)     1031  2263680 2023-11-15 18:57:30.000000 stips-2.1.0/notebooks/notebooks_data/psf_WFI_2.0.0_F129_sca01.fits
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.281787 stips-2.1.0/ref_data/
--rw-r--r--   0 jotor     (2330)     1031      696 2023-11-15 18:57:30.000000 stips-2.1.0/ref_data/retrieve_stips_data.py
--rw-r--r--   0 jotor     (2330)     1031     1740 2023-11-15 19:24:05.321685 stips-2.1.0/setup.cfg
--rwxr-xr-x   0 jotor     (2330)     1031      126 2023-11-15 18:57:30.000000 stips-2.1.0/setup.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.283064 stips-2.1.0/stips/
--rwxr-xr-x   0 jotor     (2330)     1031      802 2023-11-15 18:57:30.000000 stips-2.1.0/stips/__init__.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.288774 stips-2.1.0/stips/astro_image/
--rwxr-xr-x   0 jotor     (2330)     1031       83 2023-11-15 18:57:30.000000 stips-2.1.0/stips/astro_image/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031    59374 2023-11-15 18:57:30.000000 stips-2.1.0/stips/astro_image/astro_image.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.292046 stips-2.1.0/stips/astro_image/tests/
--rwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 18:57:30.000000 stips-2.1.0/stips/astro_image/tests/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031     4206 2023-11-15 18:57:30.000000 stips-2.1.0/stips/astro_image/tests/test_AstroImage.py
--rwxr-xr-x   0 jotor     (2330)     1031      468 2023-11-15 18:57:30.000000 stips-2.1.0/stips/astro_image/tests/test_header.py
--rwxr-xr-x   0 jotor     (2330)     1031     3821 2023-11-15 18:57:30.000000 stips-2.1.0/stips/astro_image/tests/test_wcs.py
--rwxr-xr-x   0 jotor     (2330)     1031      344 2023-11-15 18:57:30.000000 stips-2.1.0/stips/conftest.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.301129 stips-2.1.0/stips/data/
--rwxr-xr-x   0 jotor     (2330)     1031    15321 2023-11-15 18:57:30.000000 stips-2.1.0/stips/data/CreateIsochroneGrid.py
--rwxr-xr-x   0 jotor     (2330)     1031     6532 2023-11-15 18:57:30.000000 stips-2.1.0/stips/data/CreatePhoenixGrid.py
--rwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 18:57:30.000000 stips-2.1.0/stips/data/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031  2263680 2023-11-15 18:57:30.000000 stips-2.1.0/stips/data/psf_WFI_2.0.0_F129_sca01.fits
--rwxr-xr-x   0 jotor     (2330)     1031     2420 2023-11-15 18:57:30.000000 stips-2.1.0/stips/data/stips_config.yaml
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.302421 stips-2.1.0/stips/errors/
--rwxr-xr-x   0 jotor     (2330)     1031      116 2023-11-15 18:57:30.000000 stips-2.1.0/stips/errors/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031     3932 2023-11-15 18:57:30.000000 stips-2.1.0/stips/errors/make_cosmic_ray.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.305749 stips-2.1.0/stips/instruments/
--rwxr-xr-x   0 jotor     (2330)     1031      102 2023-11-15 18:57:30.000000 stips-2.1.0/stips/instruments/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031    51558 2023-11-15 18:57:30.000000 stips-2.1.0/stips/instruments/instrument.py
--rwxr-xr-x   0 jotor     (2330)     1031     1476 2023-11-15 18:57:30.000000 stips-2.1.0/stips/instruments/roman_instrument.py
--rwxr-xr-x   0 jotor     (2330)     1031    11345 2023-11-15 18:57:30.000000 stips-2.1.0/stips/instruments/wfi.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.307277 stips-2.1.0/stips/observation_module/
--rwxr-xr-x   0 jotor     (2330)     1031       99 2023-11-15 18:57:30.000000 stips-2.1.0/stips/observation_module/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031    13450 2023-11-15 18:57:30.000000 stips-2.1.0/stips/observation_module/observation_module.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.309818 stips-2.1.0/stips/scene_module/
--rwxr-xr-x   0 jotor     (2330)     1031       98 2023-11-15 18:57:30.000000 stips-2.1.0/stips/scene_module/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031     6710 2023-11-15 18:57:30.000000 stips-2.1.0/stips/scene_module/convert_units.py
--rwxr-xr-x   0 jotor     (2330)     1031    23804 2023-11-15 18:57:30.000000 stips-2.1.0/stips/scene_module/scene_module.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.312454 stips-2.1.0/stips/stellar_module/
--rwxr-xr-x   0 jotor     (2330)     1031       91 2023-11-15 18:57:30.000000 stips-2.1.0/stips/stellar_module/__init__.py
--rwxr-xr-x   0 jotor     (2330)     1031    14428 2023-11-15 18:57:30.000000 stips-2.1.0/stips/stellar_module/star_generator.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.313106 stips-2.1.0/stips/tests/
--rwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 18:57:30.000000 stips-2.1.0/stips/tests/__init__.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.317139 stips-2.1.0/stips/utilities/
--rwxr-xr-x   0 jotor     (2330)     1031     8114 2023-11-15 18:57:30.000000 stips-2.1.0/stips/utilities/DataTable.py
--rwxr-xr-x   0 jotor     (2330)     1031      385 2023-11-15 18:57:30.000000 stips-2.1.0/stips/utilities/__init__.py
--rw-r--r--   0 jotor     (2330)     1031    12110 2023-11-15 18:57:30.000000 stips-2.1.0/stips/utilities/makePSF.py
--rwxr-xr-x   0 jotor     (2330)     1031     3612 2023-11-15 18:57:30.000000 stips-2.1.0/stips/utilities/testing.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.318594 stips-2.1.0/stips/utilities/tests/
--rwxr-xr-x   0 jotor     (2330)     1031     2091 2023-11-15 18:57:30.000000 stips-2.1.0/stips/utilities/tests/test_config.py
--rwxr-xr-x   0 jotor     (2330)     1031    12282 2023-11-15 18:57:30.000000 stips-2.1.0/stips/utilities/tests/test_makePSF.py
--rwxr-xr-x   0 jotor     (2330)     1031    25229 2023-11-15 18:57:30.000000 stips-2.1.0/stips/utilities/utilities.py
-drwxr-xr-x   0 jotor     (2330)     1031        0 2023-11-15 19:24:05.287266 stips-2.1.0/stips.egg-info/
--rw-r--r--   0 jotor     (2330)     1031      753 2023-11-15 19:24:05.000000 stips-2.1.0/stips.egg-info/PKG-INFO
--rw-r--r--   0 jotor     (2330)     1031     2822 2023-11-15 19:24:05.000000 stips-2.1.0/stips.egg-info/SOURCES.txt
--rw-r--r--   0 jotor     (2330)     1031        1 2023-11-15 19:24:05.000000 stips-2.1.0/stips.egg-info/dependency_links.txt
--rw-r--r--   0 jotor     (2330)     1031        1 2023-11-15 18:57:48.000000 stips-2.1.0/stips.egg-info/not-zip-safe
--rw-r--r--   0 jotor     (2330)     1031      136 2023-11-15 19:24:05.000000 stips-2.1.0/stips.egg-info/requires.txt
--rw-r--r--   0 jotor     (2330)     1031        6 2023-11-15 19:24:05.000000 stips-2.1.0/stips.egg-info/top_level.txt
--rw-r--r--   0 jotor     (2330)     1031      310 2023-11-15 18:57:30.000000 stips-2.1.0/tox.ini
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.297964 stips-2.2.0/
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.222033 stips-2.2.0/.github/
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.235329 stips-2.2.0/.github/workflows/
+-rw-r--r--   0 jotor     (2330)     1031     1780 2024-05-10 13:21:12.000000 stips-2.2.0/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 jotor     (2330)     1031     3045 2024-05-10 13:21:12.000000 stips-2.2.0/.gitignore
+-rw-r--r--   0 jotor     (2330)     1031     1018 2024-05-10 13:21:12.000000 stips-2.2.0/.readthedocs.yaml
+-rw-r--r--   0 jotor     (2330)     1031      282 2024-05-10 13:21:12.000000 stips-2.2.0/.rtd-environment.yml
+-rw-r--r--   0 jotor     (2330)     1031     3279 2024-05-10 13:21:12.000000 stips-2.2.0/CHANGES.rst
+-rw-r--r--   0 jotor     (2330)     1031      266 2024-05-10 13:21:12.000000 stips-2.2.0/CITATION
+-rw-r--r--   0 jotor     (2330)     1031     3207 2024-05-10 13:21:12.000000 stips-2.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jotor     (2330)     1031      721 2024-05-10 13:21:12.000000 stips-2.2.0/CONTRIBUTING.md
+-rw-r--r--   0 jotor     (2330)     1031      673 2024-05-10 13:21:12.000000 stips-2.2.0/Dockerfile
+-rw-r--r--   0 jotor     (2330)     1031      376 2024-05-10 13:21:12.000000 stips-2.2.0/MANIFEST.in
+-rw-r--r--   0 jotor     (2330)     1031      753 2024-05-10 13:25:57.297515 stips-2.2.0/PKG-INFO
+-rw-r--r--   0 jotor     (2330)     1031     2346 2024-05-10 13:21:12.000000 stips-2.2.0/README.md
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.243025 stips-2.2.0/docs/
+-rw-r--r--   0 jotor     (2330)     1031     4810 2024-05-10 13:21:12.000000 stips-2.2.0/docs/Makefile
+-rw-r--r--   0 jotor     (2330)     1031     9600 2024-05-10 13:21:12.000000 stips-2.2.0/docs/basic_tutorial.rst
+-rw-r--r--   0 jotor     (2330)     1031     2865 2024-05-10 13:21:12.000000 stips-2.2.0/docs/bugs.rst
+-rw-r--r--   0 jotor     (2330)     1031     7430 2024-05-10 13:21:12.000000 stips-2.2.0/docs/conf.py
+-rw-r--r--   0 jotor     (2330)     1031     3654 2024-05-10 13:21:12.000000 stips-2.2.0/docs/examples.rst
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.243599 stips-2.2.0/docs/exts/
+-rw-r--r--   0 jotor     (2330)     1031     3319 2024-05-10 13:21:12.000000 stips-2.2.0/docs/exts/numfig.py
+-rw-r--r--   0 jotor     (2330)     1031      164 2024-05-10 13:21:12.000000 stips-2.2.0/docs/help.rst
+-rw-r--r--   0 jotor     (2330)     1031     2144 2024-05-10 13:21:12.000000 stips-2.2.0/docs/index.rst
+-rw-r--r--   0 jotor     (2330)     1031     5528 2024-05-10 13:21:12.000000 stips-2.2.0/docs/installation.rst
+-rw-r--r--   0 jotor     (2330)     1031     4513 2024-05-10 13:21:12.000000 stips-2.2.0/docs/make.bat
+-rw-r--r--   0 jotor     (2330)     1031      273 2024-05-10 13:21:12.000000 stips-2.2.0/docs/requirements.txt
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.245670 stips-2.2.0/docs/roman_figures/
+-rw-r--r--   0 jotor     (2330)     1031   415382 2024-05-10 13:21:12.000000 stips-2.2.0/docs/roman_figures/stips_basic_tutorial.png
+-rw-r--r--   0 jotor     (2330)     1031   404340 2024-05-10 13:21:12.000000 stips-2.2.0/docs/roman_figures/stips_demo.png
+-rw-r--r--   0 jotor     (2330)     1031      141 2024-05-10 13:21:12.000000 stips-2.2.0/docs/rtd-pip-requirements
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.248488 stips-2.2.0/docs/using_stips/
+-rw-r--r--   0 jotor     (2330)     1031     8768 2024-05-10 13:21:12.000000 stips-2.2.0/docs/using_stips/catalogue_formats.rst
+-rw-r--r--   0 jotor     (2330)     1031     7358 2024-05-10 13:21:12.000000 stips-2.2.0/docs/using_stips/config_file.rst
+-rw-r--r--   0 jotor     (2330)     1031     1120 2024-05-10 13:21:12.000000 stips-2.2.0/docs/using_stips/psf_grid.rst
+-rw-r--r--   0 jotor     (2330)     1031      203 2024-05-10 13:21:12.000000 stips-2.2.0/docs/using_stips.rst
+-rw-r--r--   0 jotor     (2330)     1031     1682 2024-05-10 13:21:12.000000 stips-2.2.0/environment.yml
+-rw-r--r--   0 jotor     (2330)     1031     2230 2024-05-10 13:21:12.000000 stips-2.2.0/environment_dev.yml
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.250372 stips-2.2.0/licenses/
+-rw-r--r--   0 jotor     (2330)     1031     1539 2024-05-10 13:21:12.000000 stips-2.2.0/licenses/LICENSE.rst
+-rw-r--r--   0 jotor     (2330)     1031      372 2024-05-10 13:21:12.000000 stips-2.2.0/licenses/README.rst
+-rw-r--r--   0 jotor     (2330)     1031     1659 2024-05-10 13:21:12.000000 stips-2.2.0/licenses/TEMPLATE_LICENCE.rst
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.251976 stips-2.2.0/notebooks/
+-rw-r--r--   0 jotor     (2330)     1031    23150 2024-05-10 13:21:12.000000 stips-2.2.0/notebooks/STIPS Advanced I – Further Observations, Noise and Distortion.ipynb
+-rw-r--r--   0 jotor     (2330)     1031    12688 2024-05-10 13:21:12.000000 stips-2.2.0/notebooks/STIPS Advanced II - PSFs.ipynb
+-rw-r--r--   0 jotor     (2330)     1031    13384 2024-05-10 13:21:12.000000 stips-2.2.0/notebooks/STIPS Basic Tutorial.ipynb
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.252689 stips-2.2.0/notebooks/notebooks_data/
+-rw-r--r--   0 jotor     (2330)     1031  2263680 2024-05-10 13:21:12.000000 stips-2.2.0/notebooks/notebooks_data/psf_WFI_2.0.0_F129_sca01.fits
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.257837 stips-2.2.0/ref_data/
+-rw-r--r--   0 jotor     (2330)     1031      696 2024-05-10 13:21:12.000000 stips-2.2.0/ref_data/retrieve_stips_data.py
+-rw-r--r--   0 jotor     (2330)     1031     1740 2024-05-10 13:25:57.300022 stips-2.2.0/setup.cfg
+-rwxr-xr-x   0 jotor     (2330)     1031      126 2024-05-10 13:21:12.000000 stips-2.2.0/setup.py
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.259206 stips-2.2.0/stips/
+-rwxr-xr-x   0 jotor     (2330)     1031      802 2024-05-10 13:21:12.000000 stips-2.2.0/stips/__init__.py
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.265113 stips-2.2.0/stips/astro_image/
+-rwxr-xr-x   0 jotor     (2330)     1031       83 2024-05-10 13:21:12.000000 stips-2.2.0/stips/astro_image/__init__.py
+-rwxr-xr-x   0 jotor     (2330)     1031    61362 2024-05-10 13:21:12.000000 stips-2.2.0/stips/astro_image/astro_image.py
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.268325 stips-2.2.0/stips/astro_image/tests/
+-rwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:21:12.000000 stips-2.2.0/stips/astro_image/tests/__init__.py
+-rwxr-xr-x   0 jotor     (2330)     1031     4206 2024-05-10 13:21:12.000000 stips-2.2.0/stips/astro_image/tests/test_AstroImage.py
+-rwxr-xr-x   0 jotor     (2330)     1031      468 2024-05-10 13:21:12.000000 stips-2.2.0/stips/astro_image/tests/test_header.py
+-rwxr-xr-x   0 jotor     (2330)     1031     3821 2024-05-10 13:21:12.000000 stips-2.2.0/stips/astro_image/tests/test_wcs.py
+-rwxr-xr-x   0 jotor     (2330)     1031      344 2024-05-10 13:21:12.000000 stips-2.2.0/stips/conftest.py
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.277840 stips-2.2.0/stips/data/
+-rwxr-xr-x   0 jotor     (2330)     1031    15321 2024-05-10 13:21:12.000000 stips-2.2.0/stips/data/CreateIsochroneGrid.py
+-rwxr-xr-x   0 jotor     (2330)     1031     6532 2024-05-10 13:21:12.000000 stips-2.2.0/stips/data/CreatePhoenixGrid.py
+-rwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:21:12.000000 stips-2.2.0/stips/data/__init__.py
+-rwxr-xr-x   0 jotor     (2330)     1031  2263680 2024-05-10 13:21:12.000000 stips-2.2.0/stips/data/psf_WFI_2.0.0_F129_sca01.fits
+-rwxr-xr-x   0 jotor     (2330)     1031     2420 2024-05-10 13:21:12.000000 stips-2.2.0/stips/data/stips_config.yaml
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.279590 stips-2.2.0/stips/errors/
+-rwxr-xr-x   0 jotor     (2330)     1031      116 2024-05-10 13:21:12.000000 stips-2.2.0/stips/errors/__init__.py
+-rwxr-xr-x   0 jotor     (2330)     1031     3932 2024-05-10 13:21:12.000000 stips-2.2.0/stips/errors/make_cosmic_ray.py
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.282919 stips-2.2.0/stips/instruments/
+-rwxr-xr-x   0 jotor     (2330)     1031      102 2024-05-10 13:21:12.000000 stips-2.2.0/stips/instruments/__init__.py
+-rwxr-xr-x   0 jotor     (2330)     1031    51688 2024-05-10 13:21:12.000000 stips-2.2.0/stips/instruments/instrument.py
+-rwxr-xr-x   0 jotor     (2330)     1031     1476 2024-05-10 13:21:12.000000 stips-2.2.0/stips/instruments/roman_instrument.py
+-rwxr-xr-x   0 jotor     (2330)     1031    11345 2024-05-10 13:21:12.000000 stips-2.2.0/stips/instruments/wfi.py
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.284494 stips-2.2.0/stips/observation_module/
+-rwxr-xr-x   0 jotor     (2330)     1031       99 2024-05-10 13:21:12.000000 stips-2.2.0/stips/observation_module/__init__.py
+-rwxr-xr-x   0 jotor     (2330)     1031    13571 2024-05-10 13:21:12.000000 stips-2.2.0/stips/observation_module/observation_module.py
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.286580 stips-2.2.0/stips/scene_module/
+-rwxr-xr-x   0 jotor     (2330)     1031       98 2024-05-10 13:21:12.000000 stips-2.2.0/stips/scene_module/__init__.py
+-rwxr-xr-x   0 jotor     (2330)     1031     6710 2024-05-10 13:21:12.000000 stips-2.2.0/stips/scene_module/convert_units.py
+-rwxr-xr-x   0 jotor     (2330)     1031    23804 2024-05-10 13:21:12.000000 stips-2.2.0/stips/scene_module/scene_module.py
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.288805 stips-2.2.0/stips/stellar_module/
+-rwxr-xr-x   0 jotor     (2330)     1031       91 2024-05-10 13:21:12.000000 stips-2.2.0/stips/stellar_module/__init__.py
+-rwxr-xr-x   0 jotor     (2330)     1031    14428 2024-05-10 13:21:12.000000 stips-2.2.0/stips/stellar_module/star_generator.py
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.289833 stips-2.2.0/stips/tests/
+-rwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:21:12.000000 stips-2.2.0/stips/tests/__init__.py
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.293512 stips-2.2.0/stips/utilities/
+-rwxr-xr-x   0 jotor     (2330)     1031     8114 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/DataTable.py
+-rwxr-xr-x   0 jotor     (2330)     1031      385 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/__init__.py
+-rw-r--r--   0 jotor     (2330)     1031    12110 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/makePSF.py
+-rwxr-xr-x   0 jotor     (2330)     1031     3612 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/testing.py
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.295012 stips-2.2.0/stips/utilities/tests/
+-rwxr-xr-x   0 jotor     (2330)     1031     2091 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/tests/test_config.py
+-rwxr-xr-x   0 jotor     (2330)     1031    12282 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/tests/test_makePSF.py
+-rwxr-xr-x   0 jotor     (2330)     1031    25231 2024-05-10 13:21:12.000000 stips-2.2.0/stips/utilities/utilities.py
+drwxr-xr-x   0 jotor     (2330)     1031        0 2024-05-10 13:25:57.296478 stips-2.2.0/stips.egg-info/
+-rw-r--r--   0 jotor     (2330)     1031      753 2024-05-10 13:25:57.000000 stips-2.2.0/stips.egg-info/PKG-INFO
+-rw-r--r--   0 jotor     (2330)     1031     2232 2024-05-10 13:25:57.000000 stips-2.2.0/stips.egg-info/SOURCES.txt
+-rw-r--r--   0 jotor     (2330)     1031        1 2024-05-10 13:25:57.000000 stips-2.2.0/stips.egg-info/dependency_links.txt
+-rw-r--r--   0 jotor     (2330)     1031        1 2024-05-10 13:25:57.000000 stips-2.2.0/stips.egg-info/not-zip-safe
+-rw-r--r--   0 jotor     (2330)     1031      136 2024-05-10 13:25:57.000000 stips-2.2.0/stips.egg-info/requires.txt
+-rw-r--r--   0 jotor     (2330)     1031        6 2024-05-10 13:25:57.000000 stips-2.2.0/stips.egg-info/top_level.txt
+-rw-r--r--   0 jotor     (2330)     1031      310 2024-05-10 13:21:12.000000 stips-2.2.0/tox.ini
```

### Comparing `stips-2.1.0/.github/workflows/ci_workflows.yml` & `stips-2.2.0/.github/workflows/ci_workflows.yml`

 * *Files 6% similar despite different names*

```diff
@@ -10,65 +10,72 @@
   ci_tests:
     name: ${{ matrix.name }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         include:
 
-          - name: Python 3.8
+          - name: Python 3.10
             os: ubuntu-latest
-            python: 3.8
+            python: "3.10"
 
-          - name: Python 3.9
+          - name: Python 3.11
             os: ubuntu-latest
-            python: 3.9
+            python: 3.11
 
-          - name: Python 3.9 Mac
+          - name: Python 3.11 Mac
             os: macos-latest
-            python: 3.9
+            python: 3.11
 
           - name: Python Long
             os: ubuntu-latest
-            python: 3.9
+            python: 3.11
 
     steps:
     - name: Checkout code
       uses: actions/checkout@v2
       with:
         fetch-depth: 0
+
     - name: Set up environment
       uses: conda-incubator/setup-miniconda@v2
       with:
         activate-environment: stips
         environment-file: environment.yml
         python-version: ${{ matrix.python }}
         auto-activate-base: false
+        miniconda-version: "latest"  # Ensure Miniconda is installed if not found
+
     - name: Test with tox
       shell: bash -l {0}
       if: ${{ matrix.name != 'Python Long' }}
       run: |
         tox -e test
+
     - name: Test slow tests with pytest
       shell: bash -l {0}
       if: ${{ matrix.name == 'Python Long' }}
       run: |
         tox -e test-all
 
   docs_test:
     name: "docs_test"
     runs-on: ubuntu-latest
     steps:
+
     - name: Checkout code
       uses: actions/checkout@v2
       with:
         fetch-depth: 0
+
     - name: Set up environment
       uses: conda-incubator/setup-miniconda@v2
       with:
         activate-environment: stips
         environment-file: environment.yml
-        python-version: 3.9
+        python-version: 3.11
         auto-activate-base: false
+
     - name: Build Docs
       shell: bash -l {0}
       run: |
         tox -e build_docs
```

### Comparing `stips-2.1.0/.gitignore` & `stips-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/CHANGES.rst` & `stips-2.2.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 #############
 Release Notes
 #############
 
 Version History and Change Log
 ------------------------------
 
+Version 2.2.0
+=============
+- Added a functionality to allow for faster simulations of extended sources.
+- Fixed a bug related to the simulation of extended sources.
+- Fixed a bug related to the WCS.
+- Updated pandeia to version 3.1 and its corresponding reference files.
+- Changed the minimum required Python version to 3.10
+
 Version 2.1.0
 =============
 - Updated the Flux PHOTFNU values to match Pandeia
 - Updated the background and noise estimates to use Pandeia
 - Updated webbpsf to version 1.1
 - Updated pandeia to version 2.0
```

### Comparing `stips-2.1.0/CODE_OF_CONDUCT.md` & `stips-2.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/CONTRIBUTING.md` & `stips-2.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/Dockerfile` & `stips-2.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/PKG-INFO` & `stips-2.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: stips
-Version: 2.1.0
+Version: 2.2.0
 Summary: STIPS is the Space Telescope Imaging Product Simulator.
 Home-page: https://github.com/spacetelescope/STScI-STIPS
 Author: Space Telescope Science Institute
 Author-email: york@stsci.edu
 License: BSD 3-Clause
 Requires-Dist: astropy
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: photutils
 Requires-Dist: synphot==1.1.1
 Requires-Dist: stsynphot==1.1.0
 Requires-Dist: webbpsf==1.1.1
-Requires-Dist: pandeia.engine==3.0
+Requires-Dist: pandeia.engine==3.1
 Requires-Dist: montage-wrapper
 Requires-Dist: pyyaml
 Requires-Dist: soc_roman_tools
 
 STIPS is the Space Telescope Imaging Product Simulator. It is designed to create simulations of full-detector post-pipeline astronomical scenes for the Nancy Grace Roman Space Telescope.
```

### Comparing `stips-2.1.0/README.md` & `stips-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # STScI-STIPS
 
 [![Build Status](https://travis-ci.com/spacetelescope/STScI-STIPS.svg?branch=master)](https://travis-ci.com/spacetelescope/STScI-STIPS)
 [![STScI](https://img.shields.io/badge/powered%20by-STScI-blue.svg?colorA=707170&colorB=3e8ddd&style=flat)](http://www.stsci.edu)
 
-For documentation and installation instructions please visit https://stsci-stips.readthedocs.io
+For documentation and installation instructions please visit https://stips.readthedocs.io
 
 ## Table of Contents
 
 * [Overview](#overview)
 * [Why use STIPS?](#why-use-stips)
 
 ## Overview
```

### Comparing `stips-2.1.0/docs/Makefile` & `stips-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/docs/basic_tutorial.rst` & `stips-2.2.0/docs/basic_tutorial.rst`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 
 We will use a single offset with:
 
   * An ID of 1
 
   * No centering (if an offset is centered, then, for a multi-detector observation, each
     detector is centered on the offset co-coordinates individually rather than the instrument
-    as a whole beinf centered there)
+    as a whole being centered there)
 
   * No change in RA, DEC, or PA from the center of the observation
 
 We will use the following residual settings:
 
   * Flatfield residual: off
 
@@ -233,15 +233,15 @@
 
 Observing the Created Scene
 ---------------------------
 
 In order to observe the scene, we must add the scene catalogues created above to it, add
 in error residuals, and finalize the observation.  In so doing, we create output catalogues
 which are taken from the input catalogues, but only contain the sources visible to the
-detectors, and convert source brightness into unites of counts/s for the detectors.
+detectors, and convert source brightness into units of counts/s for the detectors.
 
 .. code-block:: python
 
   output_stellar_catalogues = obm.addCatalogue(stellar_cat_file)
   output_galaxy_catalogues = obm.addCatalogue(galaxy_cat_file)
 
   print("Output Catalogues are {} and {}".format(output_stellar_catalogues, output_galaxy_catalogues))
@@ -263,20 +263,19 @@
   Fig. 1: Output from running the STIPS basic tutorial code. Detail from detector center.
 
 We use ``matplotlib`` to plot the resulting simulated image.
 
 .. code-block:: python
 
   import matplotlib
-  from matplotlib import style
+  import matplotlib.pyplot as plt
+  from astropy.io import fits
   matplotlib.rcParams['axes.grid'] = False
   matplotlib.rcParams['image.origin'] = 'lower'
-  import matplotlib.pyplot as plot
-  from astropy.io import fits
 
   with fits.open(fits_file) as result_file:
     result_data = result_file[1].data
 
-  fig1 = plot.figure()
-  im = plot.matshow(result_data)
+  fig1 = plt.figure()
+  im = plt.matshow(result_data)
 
 Alternatively, you can open the final ``.fits`` file in your preferred imaging software.
```

### Comparing `stips-2.1.0/docs/bugs.rst` & `stips-2.2.0/docs/bugs.rst`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/docs/conf.py` & `stips-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/docs/examples.rst` & `stips-2.2.0/docs/examples.rst`

 * *Files 26% similar despite different names*

```diff
@@ -61,9 +61,42 @@
     output_stellar_catalogues = obm.addCatalogue(stellar_cat_file)
     output_galaxy_catalogues = obm.addCatalogue(galaxy_cat_file)
 
     obm.addError()
 
     fits_file, mosaic_file, params = obm.finalize(mosaic=False)
 
-In this case, the output catalog(s) will show the actual applied count rates. Whether there 
-is only one output catalog or two depends on the input catalog format.
+In this case, the output catalog(s) will show the actual applied count rates.
+Whether there is only one output catalog or two depends on the input catalog format.
+
+
+Fast Extended Sources
+----------------------
+
+As of version 2.2, STIPS includes an option to inject extended sources in scenes
+using a Sersic-profile approximation. This approximation is ~8 times faster than
+the current implementation, but it is also less accurate.
+
+To activate this feature, users must turn on the ``fast_galaxy`` flag. This is how the syntax
+looks, starting from the examples listed in the :doc:`STIPS Basic Tutorial <basic_tutorial>`.
+
+.. code-block:: python
+
+    observation_parameters = {
+                              'instrument': 'WFI',
+                              'filters': ['F129'],
+                              'detectors': 1,
+                              'distortion': False,
+                              'background': 0.15,
+                              'fast_galaxy': True,
+                              'observations_id': 1,
+                              'exptime': 1000,
+                              'offsets': [offset]
+                              }
+
+.. note::
+
+    We caution however that while this method is a useful approximation, the resulting
+    integrated flux measurements can be off by a factor of ~2. Furthermore, the central
+    pixel at the core of the galaxy should not be trusted, since this can be off by
+    multiple orders of magnitude.
+
```

### Comparing `stips-2.1.0/docs/exts/numfig.py` & `stips-2.2.0/docs/exts/numfig.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/docs/index.rst` & `stips-2.2.0/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Documentation
 =============
 
 .. note::
 
-  STIPS 2.0 no longer supports HST or JWST. STIPS 1.0.8 is the most recent version to 
-  offer support for those telescopes and instruments.
+  As of version 2.0, STIPS no longer offers support for HST or JWST.
 
 Overview
 --------
-STIPS is the Space Telescope Imaging Product Simulator. It is designed to create 
-simulations of full-detector post-pipeline astronomical scenes for the Nancy Grace Roman 
-Space Telescope's Wide-Field Instrument (WFI). STIPS has the ability to add 
+STIPS is the Space Telescope Imaging Product Simulator. It is designed to create
+simulations of full-detector post-pipeline astronomical scenes for the Nancy Grace Roman
+Space Telescope's Wide-Field Instrument (WFI). STIPS has the ability to add
 instrumental distortion (if available) as well as calibration residuals from flatfields,
 dark currents, and cosmic rays. It automatically includes Poisson noise and readout noise.
 It does not include instrument saturation effects.
 
 Why use STIPS?
 --------------
-STIPS is intended to produce quick simulations of Level 2 (L2) images, and is provided for 
+STIPS is intended to produce quick simulations of Level 2 (L2) images, and is provided for
 cases where `Pandeia <https://pypi.org/project/pandeia.engine/>`_ does not
 provide a large enough simulation area (e.g., full-detector or multiple-detector
 observations). STIPS obtains its Roman instrument and filter values from
 Pandeia, so it should produce output within 10% of output produced by Pandeia.
 
-STIPS does not start with Level 1 (L1) images and propagate instrumental calibrations 
+STIPS does not start with Level 1 (L1) images and propagate instrumental calibrations
 through the simulations. While it does have the ability to add error residuals (representing
-the remaining uncertainty after pipeline calibration), these residuals are not validated 
-against actual pipeline calibrations of L1 images. STIPS is not the ideal choice if 
-extremely good instrumental accuracy is needed. Pandeia is the preferred tool for 
+the remaining uncertainty after pipeline calibration), these residuals are not validated
+against actual pipeline calibrations of L1 images. STIPS is not the ideal choice if
+extremely good instrumental accuracy is needed. Pandeia is the preferred tool for
 high-accuracy observations.
 
 Developed by Brian York (`@york-stsci <https://github.com/york-stsci>`_),
-Robel Geda (`@robelgeda <https://github.com/robelgeda>`_), 
-and O. Justin Otor (`@ojustino <https://github.com/ojustino>`_). 
-Python ePSF code developed by 
+Robel Geda (`@robelgeda <https://github.com/robelgeda>`_),
+and O. Justin Otor (`@ojustino <https://github.com/ojustino>`_).
+Python ePSF code developed by
 Sebastian Gomez (`@gmzsebastian <https://github.com/gmzsebastian>`_) based on Fortran code
 developed by Andrea Bellini (`@AndreaBellini <https://github.com/AndreaBellini>`_).
 
 .. figure:: roman_figures/stips_demo.png
 
   Fig. 1: Simulated WFI image of a star cluster and background galaxies.
```

### Comparing `stips-2.1.0/docs/installation.rst` & `stips-2.2.0/docs/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 STIPS is a simulation tool that depends on other modules such as PSF and exposure time calculators.  These underlying submodules need to be
 installed for STIPS to function properly along with their supporting datasets.  There are multiple options for installation and they are listed
 in this section along with instructions.
 
 STIPS Requirements
 ##################
 
-* ``pandeia>=3.0``: Exposure time calculator.
+* ``pandeia>=3.1``: Exposure time calculator.
 
 * ``webbpsf==1.1.1``: Nancy Grace Roman PSF calculator. STIPS also requires that ``poppy``, a
   support package used by WebbPSF, have version ``>=1.0.3``.
 
 * ``astropy``: STIPS uses Astropy in order to:
 
     * Read and write FITS files.
@@ -76,17 +76,17 @@
 
    * To create a new Conda environment named ``stips``::
 
         conda env create -f environment.yml
         conda activate stips
 
 
-   * Or, to install to or update an existing and currently active Conda environment::
+   * Or, to install to or update an existing Conda environment::
 
-        conda env update --file environment.yml
+        conda env update --name EXISTING-ENV --file environment.yml
 
 Installing as a Developer
 *************************
 
 #. This step is identical to the first step of :ref:`installing-as-a-user`.
 
 #. Follow the second step of :ref:`installing-as-a-user` but using the
@@ -122,16 +122,16 @@
 
 Testing Installation
 *********************
 
 To test if all the required files have been installed, please import STIPS in Python::
 
     bash-3.2$ python
-    Python 3.7.3 | packaged by conda-forge | (default, Dec  6 2019, 08:36:57)
-    [Clang 9.0.0 (tags/RELEASE_900/final)] :: Anaconda, Inc. on darwin
+    Python 3.11.9 | packaged by conda-forge | (main, Apr 19 2024, 18:45:13)
+    [Clang 16.0.6 ] on darwin
     Type "help", "copyright", "credits" or "license" for more information.
 
     >>> import stips
 
     >>> print(stips.__env__report__)
 
 You should receive an output of the following form:
```

### Comparing `stips-2.1.0/docs/make.bat` & `stips-2.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/docs/roman_figures/stips_basic_tutorial.png` & `stips-2.2.0/docs/roman_figures/stips_basic_tutorial.png`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/docs/roman_figures/stips_demo.png` & `stips-2.2.0/docs/roman_figures/stips_demo.png`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/docs/using_stips/catalogue_formats.rst` & `stips-2.2.0/docs/using_stips/catalogue_formats.rst`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/docs/using_stips/config_file.rst` & `stips-2.2.0/docs/using_stips/config_file.rst`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/docs/using_stips/psf_grid.rst` & `stips-2.2.0/docs/using_stips/psf_grid.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 The STIPS PSF Grid
 ==================
 
 Overview
 --------
 
-Starting with STIPS 2.0.0, STIPS uses WebbPSF PSF grids to implement an ePSF. The ePSF 
-uses a 3x3 grid of PSFs to handle PSF variation across the detector, and an oversample of 
+As of version 2.0.0, STIPS uses WebbPSF PSF grids to implement an ePSF. The ePSF
+uses a 3x3 grid of PSFs to handle PSF variation across the detector, and an oversample of
 4x4 to handle sub-pixel positioning. Each point source has its PSF calculated individually
 as it is added to the detector.
 
 Internal Image Size
 -------------------
 
-The size of the STIPS pre-convolution image is set by the size of the detector. In 
-addition, the image is padded by half of the PSF size on each side in order to include 
+The size of the STIPS pre-convolution image is set by the size of the detector. In
+addition, the image is padded by half of the PSF size on each side in order to include
 sources that fall off the detector, but whose PSF may land on the detector.
 
 PSF Image Size
 --------------
 
-The size of the STIPS generated PSF image depends on the source brightness. For most 
-sources, a 45x45-pixel PSF is created via an ePSF oversampled to a factor of 4. For bright 
-sources (magnitude < the bright limit, default 14), a 91x91-pixel PSF is created to 
-provide flux from the extended wings. For extra-bright sources 
-(magnitude < the extra-bright limit, default 3), a 181x181-pixel PSF is created to provide 
+The size of the STIPS generated PSF image depends on the source brightness. For most
+sources, a 45x45-pixel PSF is created via an ePSF oversampled to a factor of 4. For bright
+sources (magnitude < the bright limit, default 14), a 91x91-pixel PSF is created to
+provide flux from the extended wings. For extra-bright sources
+(magnitude < the extra-bright limit, default 3), a 181x181-pixel PSF is created to provide
 even more wing flux to the model.
```

### Comparing `stips-2.1.0/environment.yml` & `stips-2.2.0/environment.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file describes a conda environment that can be to install STIPS
+# This file describes a conda environment that can be used to install STIPS
 #
 # Run the following command to set up this environment:
 # $ conda env create -f environment.yml
 #
 # The environment name can be overridden with the following command:
 # $ conda env create -n <custom name> -f environment.yml
 #
@@ -21,26 +21,26 @@
   - conda-forge
   - astropy
   - defaults
 
 dependencies:
   # Base dependencies
   - pip
-  - python>=3.8
+  - python>=3.10
   - jupyter
   - Cython
   - esutil # installed from conda because you need the pre-compiled binaries.
 
   - pip:
     # Special Modules. These are temporary entries and require documentation.
     - poppy==1.0.3
 
     # Core Modules
     - webbpsf==1.1.1
-    - pandeia.engine==3.0
+    - pandeia.engine==3.1
     - synphot==1.1.1
     - stsynphot==1.1.0
     - soc_roman_tools
 
     # Major modules
     - astropy
     - photutils
```

### Comparing `stips-2.1.0/environment_dev.yml` & `stips-2.2.0/environment_dev.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# This file describes a conda environment that can be to install STIPS for development and
-# testing purposes. Note that this environment set-up installs the STIPS module in
+# This file describes a conda environment that can be used to install STIPS for development and
+# testing purposes. Note that this environment setup installs the STIPS module in
 # editable mode, so any changes you make to the STIPS source will be reflected the next
 # time you run python.
 #
 # Run the following command to set up this environment:
 # $ conda env create -f environment.yml
 #
 # The environment name can be overridden with the following command:
@@ -24,15 +24,15 @@
   - conda-forge
   - astropy
   - defaults
 
 dependencies:
   # Base dependencies
   - pip
-  - python>=3.8
+  - python>=3.10
   - jupyter
   - Cython
   - esutil # installed from conda because you need the pre-compiled binaries.
 
   - pip:
     #
     # Special Modules. These are temporary entries and require documentation.
@@ -41,15 +41,15 @@
     # values. Currently this is the only way to ensure that webbpsf picks up the correct
     # poppy version. This peg should be removed as soon as webbpsf has updated to only
     # use poppy versions that include this fix.
     - poppy==1.0.3
 
     # Core Modules
     - webbpsf==1.1.1
-    - pandeia.engine==3.0
+    - pandeia.engine==3.1
     - synphot==1.1.1
     - stsynphot==1.1.0
     - soc_roman_tools
 
     # Major modules
     - astropy
     - photutils
```

### Comparing `stips-2.1.0/licenses/LICENSE.rst` & `stips-2.2.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/licenses/TEMPLATE_LICENCE.rst` & `stips-2.2.0/licenses/TEMPLATE_LICENCE.rst`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/notebooks/STIPS Advanced I – Further Observations, Noise and Distortion.ipynb` & `stips-2.2.0/notebooks/STIPS Advanced I – Further Observations, Noise and Distortion.ipynb`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/notebooks/STIPS Advanced II - PSFs.ipynb` & `stips-2.2.0/notebooks/STIPS Advanced II - PSFs.ipynb`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/notebooks/STIPS Basic Tutorial.ipynb` & `stips-2.2.0/notebooks/STIPS Basic Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/notebooks/notebooks_data/psf_WFI_2.0.0_F129_sca01.fits` & `stips-2.2.0/notebooks/notebooks_data/psf_WFI_2.0.0_F129_sca01.fits`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/ref_data/retrieve_stips_data.py` & `stips-2.2.0/ref_data/retrieve_stips_data.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/setup.cfg` & `stips-2.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = stips
-version = 2.1.0
+version = 2.2.0
 author = Space Telescope Science Institute
 author_email = york@stsci.edu
 description = STIPS is the Space Telescope Imaging Product Simulator.
 long_description = STIPS is the Space Telescope Imaging Product Simulator. It is designed to create simulations of full-detector post-pipeline astronomical scenes for the Nancy Grace Roman Space Telescope.
 license = BSD 3-Clause
 url = https://github.com/spacetelescope/STScI-STIPS
 edit_on_github = False
@@ -19,15 +19,15 @@
 	astropy
 	numpy
 	scipy
 	photutils
 	synphot==1.1.1
 	stsynphot==1.1.0
 	webbpsf==1.1.1
-	pandeia.engine==3.0
+	pandeia.engine==3.1
 	montage-wrapper
 	pyyaml
 	soc_roman_tools
 zip_safe = False
 use_2to3 = False
 include_package_data = True
```

### Comparing `stips-2.1.0/stips/__init__.py` & `stips-2.2.0/stips/__init__.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/astro_image/astro_image.py` & `stips-2.2.0/stips/astro_image/astro_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 
         if 'parent' in kwargs:
             self.parent = kwargs['parent']
             self.logger = self.parent.logger
             self.out_path = self.parent.out_path
             self.prefix = self.parent.prefix
             self.seed = self.parent.seed
+            self.fast_galaxy = self.parent.fast_galaxy
+            self.convolve_galaxy = self.parent.convolve_galaxy
             self.telescope = self.parent.TELESCOPE.lower()
             self.instrument = self.parent.PSF_INSTRUMENT
             self.filter = self.parent.filter
             self.bright_limit = self.parent.bright_limit
             self.xbright_limit = self.parent.xbright_limit
             self.shape = self.parent.DETECTOR_SIZE
             self._scale = self.parent.SCALE
@@ -89,14 +91,16 @@
                     stream_handler = logging.StreamHandler(sys.stderr)
                     format = '%(asctime)s %(levelname)s: %(message)s'
                     stream_handler.setFormatter(logging.Formatter(format))
                     self.logger.addHandler(stream_handler)
             self.out_path = SelectParameter('out_path', kwargs)
             self.bright_limit = SelectParameter('psf_bright_limit', kwargs)
             self.xbright_limit = SelectParameter('psf_xbright_limit', kwargs)
+            self.fast_galaxy = SelectParameter('fast_galaxy', kwargs)
+            self.convolve_galaxy = SelectParameter('convolve_galaxy', kwargs)
             self.shape = kwargs.get('shape', default['shape'])
             self._scale = kwargs.get('scale', np.array(default['scale']))
             self.prefix = kwargs.get('prefix', '')
             self.cat_type = SelectParameter('cat_type', kwargs)
             self.seed = SelectParameter('seed', kwargs)
             self.zeropoint = kwargs.get('zeropoint', default['zeropoint'])
             self.photflam = kwargs.get('photflam', default['photflam'])
@@ -350,15 +354,15 @@
         self._log("info", "Creating Extension HDU from AstroImage {}".format(self.name))
         hdu = fits.ImageHDU(self.data, header=self.wcs.to_header(relax=True), name=self.name)
         if 'CDELT1' not in hdu.header:
             hdu.header['CDELT1'] = self.scale[0]/3600.
             hdu.header['CDELT2'] = self.scale[0]/3600.
         # Apparently astropy refuses to add the identity matrix to a header
         if ('PA1_1' not in hdu.header) and ('CD1_1' not in hdu.header):
-            hdu.header['CD1_1'] = -self.scale[0]/3600.
+            hdu.header['CD1_1'] = self.scale[0]/3600.
             hdu.header['CD1_2'] = 0.
             hdu.header['CD2_1'] = 0.
             hdu.header['CD2_2'] = self.scale[0]/3600.
         for k, v in self.header.items():
             hdu.header[k] = v
         for item in self.history:
             hdu.header.add_history(item)
@@ -387,15 +391,15 @@
         """
         self.header[k] = v
 
     def addHistory(self, v):
         """Adds an entry to the header history list."""
         self.history.append(v)
 
-    def addTable(self, t, dist=False, *args, **kwargs):
+    def addTable(self, t, dist=False, fast_galaxy=False, convolve_galaxy=True, *args, **kwargs):
         """
         Add a catalogue table to the Image. The Table must have the following columns:
             RA: RA of source
             DEC: DEC of source
             FLUX: flux of source
             TYPE: type of source (point, sersic)
             N: sersic index
@@ -456,15 +460,18 @@
                 gids = ids[gals_idx]
                 counter = 1
                 total = len(gxs)
                 self._log('info', 'Starting Sersic Profiles at {}'.format(time.ctime()))
                 for (x, y, flux, n, re, phi, ratio, id) in zip(gxs, gys, gfluxes, gns, gres, gphis, gratios, gids):
                     item_index = np.where(ids == id)[0][0]
                     self._log("info", "Index is {}".format(item_index))
-                    central_flux = self.addSersicProfile(x, y, flux, n, re, phi, ratio, *args, **kwargs)
+                    if fast_galaxy:
+                        central_flux = self.oldSersicProfile(x, y, flux, n, re, phi, ratio, convolve_galaxy, *args, **kwargs)
+                    else:
+                        central_flux = self.addSersicProfile(x, y, flux, n, re, phi, ratio, *args, **kwargs)
                     fluxes_observed[item_index] = central_flux
                     notes[item_index] = "{}: surface brightness {:.3f} yielded flux {:.3f}".format(notes[item_index], flux, central_flux)
                     self._log("info", "Finished Galaxy {} of {}".format(counter, total))
                     counter += 1
                 self._log('info', 'Finishing Sersic Profiles at {}'.format(time.ctime()))
             ot = Table()
             ot['x'] = Column(data=xfs+self.out_origin, unit='pixel')
@@ -506,15 +513,15 @@
         in_data = StipsDataTable.dataTableFromFile(cat)
         out_data = StipsDataTable.dataTableFromFile(obsname)
         out_data.meta = {'name': 'Observed Catalogue', 'type': 'observed', 'detector': self.name, 'input_catalogue': catname}
         counter = 0
         current_chunk = in_data.read_chunk()
         while current_chunk is not None:
             table_length = len(current_chunk['id'])
-            out_chunk = self.addTable(current_chunk, dist, *args, **kwargs)
+            out_chunk = self.addTable(current_chunk, dist, fast_galaxy = self.fast_galaxy, *args, **kwargs)
             if out_chunk is not None:
                 out_data.write_chunk(out_chunk)
             counter += table_length
             current_chunk = in_data.read_chunk()
         self._log("info", "Added catalogue {} to AstroImage {}".format(catname, self.name))
         return obsname
 
@@ -712,99 +719,137 @@
         else:
             sip = None
         self.wcs = self._wcs(self.ra, self.dec, self.pa, self.scale, crpix=crpix, sip=sip)
         self.data = fp_crop
         self.shape = self.base_shape
         self.has_psf = False
 
-    def addSersicProfile(self, posX, posY, flux, n, re, phi, axialRatio, *args, **kwargs):
+    def addSersicProfile(self, posX, posY, flux, n, re, phi, axialRatio,
+                         *args, **kwargs):
         """
-        Creates a simulated Sersic profile, including PSF convolution, using pandeia's
-        SersicDistribution.
+        Create a simulated Sersic profile, including PSF convolution, using
+        Pandeia's SersicDistribution.
 
         Parameters
         ----------
-        id: int
-            The source ID of the sersic profile
-        gal_params: dict
-            A dictionary containing the galaxy parameters. These parameters are:
-            x, y: float
-                The position of the profile centre on the detector
-            flux: float
-                The surface brightness (in counts/s/pixel) at the half-light radius
-            n: float
-                The Sersic index. This must be between 0.3 and 6.2.
-            re: float
-                The half-light radius, in pixels.
-            phi: float
-                The position angle of the major axis, in degrees east of north
-            ratio: float
-                The ratio between the major and minor axes
-        psf_params: dict
-            A dictionary containing the PSF parameters. These parameters are:
-
-            psf_file: string
-                The name and location of the PSF file
-        xsize, ysize: int
-            The size of the detector
-        dir: string
-            The working directory to write model arrays to.
-        overrides: dict
-            Holds a copy of the AstroImage dictionary used to provide runtime parameter
-            setting.
-        logger: logging.logger
-            Logger to use for logging messages.
+        posX: float
+            The X position of the profile center on the detector.
+        posX: float
+            The Y position of the profile center on the detector.
+        flux: float
+            The surface brightness (in counts/s/pixel) at the half-light radius.
+        n: float
+            The Sersic index. This must be between 0.3 and 6.2.
+        re: float
+            The half-light radius, in pixels.
+        phi: float
+            The position angle of the major axis, in degrees east of north.
+        axialRatio: float
+            The ratio between the major and minor axes.
 
         Returns
         -------
-        fname: string
-            The name of the file in which the output numpy array was saved.
-        x,y: int
-            The position on the detector of the model centre
         central_flux: float
             The flux at the central pixel of the model
         """
         ix, iy = rind(posX), rind(posY)
         if flux == 0.:
             return 0.
 
         flux = sersic_lum(flux, re, n)
 
         source_dict = {'id': id}
         source_dict['shape'] = {'geometry': 'sersic'}
         source_dict['shape']['major'] = re
         source_dict['shape']['minor'] = re*axialRatio
-        source_dict['sersic_index'] = n
+        source_dict['shape']['sersic_index'] = n
         source_dict['spectrum'] = {'redshift': 0., 'sed': {'sed_type': 'flat'}}
         source_dict['normalization'] = {'type': 'none'}
         source_dict['position'] = {'orientation': 90-phi}
-        source_dict['position']['x_offset'] = self.xsize - posX
-        source_dict['position']['y_offset'] = self.ysize - posY
+        source_dict['position']['x_offset'] = posX - self.xsize / 2
+        source_dict['position']['y_offset'] = self.ysize / 2 - posY
         g = coords.Grid(1., 1., self.xsize, self.ysize)
         xc, yc = ix, iy
 
         # Roman is the only telescope supported
         src = source.Source('roman', config=source_dict)
         src.grid = g
-        sersic = profile.SersicDistribution(src)
+        sersic = profile.SersicDistribution(src, 1)
         img = deepcopy(sersic.prof)*flux/np.sum(sersic.prof)
         central_flux = img[yc, xc]
 
         # Read input PSF files
         psf_array, psf_middle = self.make_epsf_array()
         boxsize = rind(np.floor(psf_middle)/PSF_UPSCALE)
         epsf = interpolate_epsf(posX, posY, psf_array, self.shape[0])
         psf_data = np.zeros((boxsize, boxsize), dtype=np.float32)
         psf_x, psf_y = rind(boxsize/2), rind(boxsize/2)
         psf_data = place_source(psf_x, psf_y, 1., psf_data, epsf, boxsize=boxsize, psf_center=psf_middle)
-
         result = convolve_fft(img, psf_data)
         self.data += result
         return central_flux
 
+
+    def oldSersicProfile(self, posX, posY, flux, n, re, phi, axialRatio,
+                         convolve_galaxy, *args, **kwargs):
+        """
+        Create a simulated Sersic profile, including PSF convolution, using
+        the old (and faster) Astropy Sersic2D model.
+
+        Parameters
+        ----------
+        posX: float
+            The X position of the profile center on the detector.
+        posX: float
+            The Y position of the profile center on the detector.
+        flux: float
+            The surface brightness (in counts/s/pixel) at the half-light radius.
+        n: float
+            The Sersic index. This must be between 0.3 and 6.2.
+        re: float
+            The half-light radius, in pixels.
+        phi: float
+            The position angle of the major axis, in degrees east of north.
+        axialRatio: float
+            The ratio between the major and minor axes.
+        convolve_galaxy : bool
+            Whether to convolve the final image with the Roman PSF.
+            [default: True]
+
+        Returns
+        -------
+        central_flux: float
+            The flux at the central pixel of the model
+        """
+        if flux == 0.:
+            return 0.
+
+        # Generate 2D Sersic profile
+        from astropy.modeling.models import Sersic2D
+        x, y = np.meshgrid(np.arange(self.xsize), np.arange(self.ysize))
+        mod = Sersic2D(amplitude=flux, r_eff=re, n=n, x_0=posX, y_0=posY, ellip=(1.-axialRatio), theta=(np.radians(phi) + 0.5*np.pi))
+        img = mod(x, y)
+
+        # Convolve with Roman PSF
+        if convolve_galaxy:
+            psf_array, psf_middle = self.make_epsf_array()
+            boxsize = rind(np.floor(psf_middle)/PSF_UPSCALE)
+            epsf = interpolate_epsf(posX, posY, psf_array, self.shape[0])
+            psf_data = np.zeros((boxsize, boxsize), dtype=np.float32)
+            psf_x, psf_y = rind(boxsize/2), rind(boxsize/2)
+            psf_data = place_source(psf_x, psf_y, 1., psf_data, epsf, boxsize=boxsize, psf_center=psf_middle)
+            result = convolve_fft(img, psf_data)
+            self.data += result
+        else:
+            self.data += img
+
+        # Calculate central flux
+        central_flux = mod(posX, posY)
+        return central_flux
+
     def rotate(self, angle, reshape=False):
         """
         Rotate the image a number of degrees as specified
 
         ..warning:: This function is not necessarily flux-conserving
         """
         self.addHistory("Rotating by {} degrees".format(angle))
```

### Comparing `stips-2.1.0/stips/astro_image/tests/test_AstroImage.py` & `stips-2.2.0/stips/astro_image/tests/test_AstroImage.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/astro_image/tests/test_wcs.py` & `stips-2.2.0/stips/astro_image/tests/test_wcs.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/data/CreateIsochroneGrid.py` & `stips-2.2.0/stips/data/CreateIsochroneGrid.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/data/CreatePhoenixGrid.py` & `stips-2.2.0/stips/data/CreatePhoenixGrid.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/data/psf_WFI_2.0.0_F129_sca01.fits` & `stips-2.2.0/stips/data/psf_WFI_2.0.0_F129_sca01.fits`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/data/stips_config.yaml` & `stips-2.2.0/stips/data/stips_config.yaml`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/errors/make_cosmic_ray.py` & `stips-2.2.0/stips/errors/make_cosmic_ray.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/instruments/instrument.py` & `stips-2.2.0/stips/instruments/instrument.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,16 @@
         self.ra = kwargs.get('ra', 0.)
         self.dec = kwargs.get('dec', 0.)
         self.pa = kwargs.get('pa', 0.)
         self.distortion = SelectParameter('distortion', kwargs)
         self.exptime = kwargs.get('exptime', 1.)
         self.bright_limit = kwargs.get('bright_limit', kwargs)
         self.xbright_limit = kwargs.get('xbright_limit', kwargs)
+        self.fast_galaxy = kwargs.get('fast_galaxy', kwargs)
+        self.convolve_galaxy = kwargs.get('convolve_galaxy', kwargs)
         self.filter = None
         self.detectors = None
         self.instrument = kwargs.get('instrument', 'wfi')
         self.background_value = SelectParameter('background', kwargs)
         self.custom_background = kwargs.get('custom_background', 0.)
         self.CENTRAL_OFFSET = (0., 0., 0.)
```

### Comparing `stips-2.1.0/stips/instruments/roman_instrument.py` & `stips-2.2.0/stips/instruments/roman_instrument.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/instruments/wfi.py` & `stips-2.2.0/stips/instruments/wfi.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/observation_module/observation_module.py` & `stips-2.2.0/stips/observation_module/observation_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,16 @@
         self._log('info', "Got offsets as {}".format(self.offsets))
         self.background = SelectParameter('background', obs)
         self.custom_background = obs.get('custom_background', 0.)
         self.id = obs.get('observations_id', '0')
         self.detectors = int(obs.get('detectors', 1))
         self.excludes = obs.get('excludes', [])
         self.exptime = float(obs.get('exptime', 1.))
+        self.fast_galaxy = obs.get('fast_galaxy', False)
+        self.convolve_galaxy = obs.get('convolve_galaxy', True)
         self.bright_limit = obs.get('bright_limit', 14.)
         self.xbright_limit = obs.get('xbright_limit', 3.)
         if len(self.filters) == 0 and 'filter' in obs:
             self.filters.append(obs['filter'])
 
         # initialize parameters from the supplied keyword arguments
         self.prefix = kwargs.get('out_prefix', 'sim')
```

### Comparing `stips-2.1.0/stips/scene_module/convert_units.py` & `stips-2.2.0/stips/scene_module/convert_units.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/scene_module/scene_module.py` & `stips-2.2.0/stips/scene_module/scene_module.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/stellar_module/star_generator.py` & `stips-2.2.0/stips/stellar_module/star_generator.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/utilities/DataTable.py` & `stips-2.2.0/stips/utilities/DataTable.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/utilities/makePSF.py` & `stips-2.2.0/stips/utilities/makePSF.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/utilities/testing.py` & `stips-2.2.0/stips/utilities/testing.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/utilities/tests/test_config.py` & `stips-2.2.0/stips/utilities/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/utilities/tests/test_makePSF.py` & `stips-2.2.0/stips/utilities/tests/test_makePSF.py`

 * *Files identical despite different names*

### Comparing `stips-2.1.0/stips/utilities/utilities.py` & `stips-2.2.0/stips/utilities/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,22 +334,22 @@
         get_compressed_file(webbpsf_url, webbpsf_data_file, webbpsf_data_path,
                             "webbpsf-data/")
     else:
         print("Found at {}".format(webbpsf_data_path))
 
     # pandeia
     print("Checking pandeia data")
-    pandeia_data_file = "pandeia_data-3.0.tar.gz"
-    pandeia_url = "https://stsci.box.com/shared/static/3n9e05mxkjzquxaq1gl6nqp6l0ksz5c2.gz"
+    pandeia_data_file = "pandeia_data-3.1_roman.tar.gz"
+    pandeia_url = "https://stsci.box.com/shared/static/cmljh0lsffz4345064eso7lix70f9477.gz"
     pandeia_data_path = os.environ[GetParameter("pandeia_data_name", use_data=False)]
     if not os.path.isdir(pandeia_data_path):
         print("Downloading pandeia data to {}".format(pandeia_data_path))
         os.makedirs(pandeia_data_path)
         get_compressed_file(pandeia_url, pandeia_data_file, pandeia_data_path,
-                            "pandeia_data-3.0_roman_rc3/")
+                            "pandeia_data-3.1_roman/")
     else:
         print("Found at {}".format(pandeia_data_path))
 
     # Done.
 
 
 def GetStipsDataDir():
```

### Comparing `stips-2.1.0/stips.egg-info/PKG-INFO` & `stips-2.2.0/stips.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: stips
-Version: 2.1.0
+Version: 2.2.0
 Summary: STIPS is the Space Telescope Imaging Product Simulator.
 Home-page: https://github.com/spacetelescope/STScI-STIPS
 Author: Space Telescope Science Institute
 Author-email: york@stsci.edu
 License: BSD 3-Clause
 Requires-Dist: astropy
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: photutils
 Requires-Dist: synphot==1.1.1
 Requires-Dist: stsynphot==1.1.0
 Requires-Dist: webbpsf==1.1.1
-Requires-Dist: pandeia.engine==3.0
+Requires-Dist: pandeia.engine==3.1
 Requires-Dist: montage-wrapper
 Requires-Dist: pyyaml
 Requires-Dist: soc_roman_tools
 
 STIPS is the Space Telescope Imaging Product Simulator. It is designed to create simulations of full-detector post-pipeline astronomical scenes for the Nancy Grace Roman Space Telescope.
```

