# Comparing `tmp/mwrpy-0.8.3.tar.gz` & `tmp/mwrpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwrpy-0.8.3.tar", last modified: Fri Mar 22 08:36:21 2024, max compression
+gzip compressed data, was "mwrpy-0.9.0.tar", last modified: Fri May 10 11:10:35 2024, max compression
```

## Comparing `mwrpy-0.8.3.tar` & `mwrpy-0.9.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.062267 mwrpy-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-22 08:36:17.000000 mwrpy-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-22 08:36:17.000000 mwrpy-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-03-22 08:36:21.062267 mwrpy-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-03-22 08:36:17.000000 mwrpy-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.046267 mwrpy-0.8.3/mwrpy/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/atmos.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1814 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.046267 mwrpy-0.8.3/mwrpy/level1/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/level1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/level1/lev1_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/level1/met_quality_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    14144 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/level1/quality_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/level1/rpg_bin.py
--rw-r--r--   0 runner    (1001) docker     (127)    20086 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/level1/write_lev1_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.046267 mwrpy-0.8.3/mwrpy/level2/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/level2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12493 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/level2/get_ret_coeff.py
--rw-r--r--   0 runner    (1001) docker     (127)     8572 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/level2/lev2_collocated.py
--rw-r--r--   0 runner    (1001) docker     (127)    12664 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/level2/lev2_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/level2/lwp_offset.py
--rw-r--r--   0 runner    (1001) docker     (127)    25287 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/level2/write_lev2_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.050267 mwrpy-0.8.3/mwrpy/plots/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53935 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/plots/generate_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/plots/plot_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/plots/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/process_mwrpy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/rpg_mwr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.050267 mwrpy-0.8.3/mwrpy/site_config/
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/hatpro.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.050267 mwrpy-0.8.3/mwrpy/site_config/hyytiala/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.054267 mwrpy-0.8.3/mwrpy/site_config/hyytiala/coefficients/
--rw-r--r--   0 runner    (1001) docker     (127)    33953 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (127)    73995 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (127)    73995 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (127)  1208422 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (127)    80385 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (127)    39550 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/hyytiala/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.054267 mwrpy-0.8.3/mwrpy/site_config/juelich/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.058267 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/juelich/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.058267 mwrpy-0.8.3/mwrpy/site_config/lindenberg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.058267 mwrpy-0.8.3/mwrpy/site_config/lindenberg/coefficients/
--rw-r--r--   0 runner    (1001) docker     (127)    47201 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (127)    54562 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (127)    54562 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (127)   209789 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (127)    63954 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (127)    41482 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/lindenberg/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.058267 mwrpy-0.8.3/mwrpy/site_config/palaiseau/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.062267 mwrpy-0.8.3/mwrpy/site_config/palaiseau/coefficients/
--rw-r--r--   0 runner    (1001) docker     (127)    47178 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/palaiseau/coefficients/HPT_NN_FR_SIRTA_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (127)    54539 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/palaiseau/coefficients/IWV_NN_MA_FR_SIRTA_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (127)    54539 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/palaiseau/coefficients/LWP_NN_MA_FR_SIRTA_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (127)   209766 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/palaiseau/coefficients/SPC_NN_MA_INS_FR_SIRTA_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (127)    63931 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/palaiseau/coefficients/TPB_NN_FR_SIRTA_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (127)    41459 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/palaiseau/coefficients/TPT_NN_FR_SIRTA_HATPRO_G5_v121.ret
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/site_config/palaiseau/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    18302 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-22 08:36:17.000000 mwrpy-0.8.3/mwrpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 08:36:21.062267 mwrpy-0.8.3/mwrpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-03-22 08:36:21.000000 mwrpy-0.8.3/mwrpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-22 08:36:21.000000 mwrpy-0.8.3/mwrpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 08:36:21.000000 mwrpy-0.8.3/mwrpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-22 08:36:21.000000 mwrpy-0.8.3/mwrpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-22 08:36:21.000000 mwrpy-0.8.3/mwrpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-22 08:36:17.000000 mwrpy-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 08:36:21.062267 mwrpy-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.353412 mwrpy-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-10 11:10:31.000000 mwrpy-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 11:10:31.000000 mwrpy-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-05-10 11:10:35.353412 mwrpy-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-10 11:10:31.000000 mwrpy-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.337412 mwrpy-0.9.0/mwrpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/atmos.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1814 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.337412 mwrpy-0.9.0/mwrpy/level1/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/level1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/level1/lev1_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/level1/met_quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14464 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/level1/quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16639 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/level1/rpg_bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/level1/write_lev1_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.341412 mwrpy-0.9.0/mwrpy/level2/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/level2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/level2/get_ret_coeff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8572 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/level2/lev2_collocated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12657 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/level2/lev2_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/level2/lwp_offset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24830 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/level2/write_lev2_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.341412 mwrpy-0.9.0/mwrpy/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53935 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/plots/generate_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/plots/plot_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/plots/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/process_mwrpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/rpg_mwr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.341412 mwrpy-0.9.0/mwrpy/site_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/hatpro.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.341412 mwrpy-0.9.0/mwrpy/site_config/hyytiala/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.345412 mwrpy-0.9.0/mwrpy/site_config/hyytiala/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (127)    33953 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (127)    73995 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (127)    73995 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (127)  1208422 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (127)    80385 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (127)    39550 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/hyytiala/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.345412 mwrpy-0.9.0/mwrpy/site_config/juelich/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.345412 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/juelich/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.345412 mwrpy-0.9.0/mwrpy/site_config/lindenberg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.349412 mwrpy-0.9.0/mwrpy/site_config/lindenberg/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (127)    47201 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (127)    54562 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (127)    54562 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (127)   209789 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (127)    63954 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (127)    41482 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/lindenberg/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.349412 mwrpy-0.9.0/mwrpy/site_config/palaiseau/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.349412 mwrpy-0.9.0/mwrpy/site_config/palaiseau/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (127)    47178 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/palaiseau/coefficients/HPT_NN_FR_SIRTA_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (127)    54539 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/palaiseau/coefficients/IWV_NN_MA_FR_SIRTA_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (127)    54539 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/palaiseau/coefficients/LWP_NN_MA_FR_SIRTA_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (127)   209766 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/palaiseau/coefficients/SPC_NN_MA_INS_FR_SIRTA_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (127)    63931 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/palaiseau/coefficients/TPB_NN_FR_SIRTA_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (127)    41459 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/palaiseau/coefficients/TPT_NN_FR_SIRTA_HATPRO_G5_v121.ret
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/site_config/palaiseau/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 11:10:31.000000 mwrpy-0.9.0/mwrpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:10:35.349412 mwrpy-0.9.0/mwrpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-05-10 11:10:35.000000 mwrpy-0.9.0/mwrpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-10 11:10:35.000000 mwrpy-0.9.0/mwrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:10:35.000000 mwrpy-0.9.0/mwrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-10 11:10:35.000000 mwrpy-0.9.0/mwrpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 11:10:35.000000 mwrpy-0.9.0/mwrpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-10 11:10:31.000000 mwrpy-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:10:35.353412 mwrpy-0.9.0/setup.cfg
```

### Comparing `mwrpy-0.8.3/LICENSE` & `mwrpy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/PKG-INFO` & `mwrpy-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwrpy
-Version: 0.8.3
+Version: 0.9.0
 Summary: Python package for Microwave Radiometer processing in ACTRIS
 Author-email: University of Cologne <actris-ccres-mwr@uni-koeln.de>
 License: MIT License
         
         Copyright (c) 2021-2023 University of Cologne
         Copyright (c) 2023 Finnish Meteorological Institute
```

### Comparing `mwrpy-0.8.3/README.md` & `mwrpy-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/atmos.py` & `mwrpy-0.9.0/mwrpy/atmos.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,18 +87,18 @@
         masked_array(T, data_units="K"), masked_array(q, data_units="")
     ).magnitude
     p_baro = ma.masked_all(T.shape)
     p_baro[
         (~ma.getmaskarray(q).any(axis=1)) & (~ma.getmaskarray(T).any(axis=1)), 0
     ] = p[(~ma.getmaskarray(q).any(axis=1)) & (~ma.getmaskarray(T).any(axis=1))]
     for ialt in np.arange(len(z) - 1) + 1:
-        p_baro[:, ialt] = p_baro[:, ialt - 1] * np.exp(
+        p_baro[:, ialt] = p_baro[:, ialt - 1] * ma.exp(
             -scipy.constants.g
             * (z[ialt] - z[ialt - 1])
-            / (con.RS * np.mean([Tv[:, ialt], Tv[:, ialt - 1]]))
+            / (con.RS * (Tv[:, ialt] + Tv[:, ialt - 1]) / 2.0)
         )
 
     return p_baro
 
 
 def calc_saturation_vapor_pressure(temperature: np.ndarray) -> np.ndarray:
     """Goff-Gratch formula for saturation vapor pressure (Pa) over water adopted by WMO.
@@ -175,15 +175,15 @@
         ).max()
 
         tb_wv = np.squeeze(lev1["tb"][:, freq_22])
         tb_rat = pd.DataFrame({"Tb": tb_wv / tb}, index=ind)
         tb_rat = tb_rat.rolling(
             pd.tseries.frequencies.to_offset("20min"), center=True, min_periods=100
         ).max()
-        index[tb_mx["Tb"] < np.median(tb_rat["Tb"]) * 0.1] = 0
+        index[tb_mx["Tb"] < np.nanmedian(tb_rat["Tb"]) * 0.1] = 0
 
         df = pd.DataFrame({"index": index}, index=ind)
         df = df.bfill(limit=120)
         df = df.ffill(limit=120)
         index = np.array(df["index"])
         index[(lev1["elevation_angle"][:] < 89.0) & (index != 0)] = 2
```

### Comparing `mwrpy-0.8.3/mwrpy/cli.py` & `mwrpy-0.9.0/mwrpy/cli.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/level1/lev1_meta_nc.py` & `mwrpy-0.9.0/mwrpy/level1/lev1_meta_nc.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,15 +317,15 @@
     ),
     "wind_speed": MetaData(
         long_name="Wind speed",
         standard_name="wind_speed",
         units="m s-1",
     ),
     "met_quality_flag": MetaData(
-        long_name="Meterological data quality flag",
+        long_name="Meteorological data quality flag",
         units="1",
         definition=DEFINITIONS_1B21["met_quality_flag"],
         comment="0=ok, 1=problem. Note: should also be set to 1\n"
         "if corresponding sensor not available",
     ),
 }
```

### Comparing `mwrpy-0.8.3/mwrpy/level1/met_quality_control.py` & `mwrpy-0.9.0/mwrpy/level1/met_quality_control.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/level1/quality_control.py` & `mwrpy-0.9.0/mwrpy/level1/quality_control.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 from numpy import ma
 
 from mwrpy.level1.rpg_bin import RpgBin
 from mwrpy.level2.get_ret_coeff import get_mvr_coeff
 from mwrpy.level2.write_lev2_nc import retrieval_input
 from mwrpy.utils import get_coeff_list, setbit
 
-Fill_Value_Float = -999.0
-Fill_Value_Int = -99
-
 
 def apply_qc(
     site: str | None, data_in: RpgBin, params: dict, coeff_files: list | None
 ) -> None:
     """This function performs the quality control of level 1 data.
     Args:
         site: Name of site.
@@ -50,15 +47,15 @@
     for freq, _ in enumerate(data["frequency"]):
         # Bit 1: Missing TB-value
         if params["flag_status"][0] == 1:
             data["quality_flag_status"][:, freq] = setbit(
                 data["quality_flag_status"][:, freq], 0
             )
         else:
-            ind = np.where(data["tb"][:, freq] == Fill_Value_Float)
+            ind = np.where(ma.getmaskarray(data["tb"][:, freq]))
             data["quality_flag"][ind, freq] = setbit(data["quality_flag"][ind, freq], 0)
 
         # Bit 2: TB threshold (lower range)
         if params["flag_status"][1] == 1:
             data["quality_flag_status"][:, freq] = setbit(
                 data["quality_flag_status"][:, freq], 1
             )
@@ -122,20 +119,20 @@
 
 
 def orbpos(data: dict, params: dict) -> np.ndarray:
     """Calculates sun & moon elevation/azimuth angles
     and returns index for observations in the direction of the sun"""
 
     sun: dict = {
-        "azimuth_angle": np.zeros(data["time"].shape) * Fill_Value_Float,
-        "elevation_angle": np.zeros(data["time"].shape) * Fill_Value_Float,
+        "azimuth_angle": ma.masked_all(data["time"].shape),
+        "elevation_angle": ma.masked_all(data["time"].shape),
     }
     moon: dict = {
-        "azimuth_angle": np.zeros(data["time"].shape) * Fill_Value_Float,
-        "elevation_angle": np.zeros(data["time"].shape) * Fill_Value_Float,
+        "azimuth_angle": ma.masked_all(data["time"].shape),
+        "elevation_angle": ma.masked_all(data["time"].shape),
     }
 
     sol = ephem.Sun()
     lun = ephem.Moon()
     obs_loc = ephem.Observer()
 
     for ind, time in enumerate(data["time"]):
@@ -166,46 +163,62 @@
     i_moon = np.where(moon["elevation_angle"] > 0.0)[0]
     if len(i_moon) > 0:
         moon["rise"] = data["time"][i_moon[0]]
         moon["set"] = data["time"][i_moon[-1]]
 
     flag_ind = np.where(
         (
-            (data["elevation_angle"] != Fill_Value_Float)
+            (~ma.getmaskarray(data["elevation_angle"]))
             & (data["elevation_angle"] <= np.max(sun["elevation_angle"]) + 10.0)
             & (data["time"] >= sun["rise"])
             & (data["time"] <= sun["set"])
             & (data["elevation_angle"] >= sun["elevation_angle"] - params["saf"])
             & (data["elevation_angle"] <= sun["elevation_angle"] + params["saf"])
-            & (data["azimuth_angle"] >= sun["azimuth_angle"] - params["saf"])
-            & (data["azimuth_angle"] <= sun["azimuth_angle"] + params["saf"])
+            & (
+                data["azimuth_angle"]
+                >= sun["azimuth_angle"]
+                - params["saf"] / np.cos(np.deg2rad(data["elevation_angle"]))
+            )
+            & (
+                data["azimuth_angle"]
+                <= sun["azimuth_angle"]
+                + params["saf"] / np.cos(np.deg2rad(data["elevation_angle"]))
+            )
         )
         | (
             (data["elevation_angle"] <= np.max(moon["elevation_angle"]) + 10.0)
             & (data["time"] >= moon["rise"])
             & (data["time"] <= moon["set"])
             & (data["elevation_angle"] >= moon["elevation_angle"] - params["saf"])
             & (data["elevation_angle"] <= moon["elevation_angle"] + params["saf"])
-            & (data["azimuth_angle"] >= moon["azimuth_angle"] - params["saf"])
-            & (data["azimuth_angle"] <= moon["azimuth_angle"] + params["saf"])
+            & (
+                data["azimuth_angle"]
+                >= moon["azimuth_angle"]
+                - params["saf"] / np.cos(np.deg2rad(data["elevation_angle"]))
+            )
+            & (
+                data["azimuth_angle"]
+                <= moon["azimuth_angle"]
+                + params["saf"] / np.cos(np.deg2rad(data["elevation_angle"]))
+            )
         )
     )[0]
 
     return flag_ind
 
 
 def spectral_consistency(
     data: dict, site: str | None, coeff_files: list | None
 ) -> np.ndarray:
     """Applies spectral consistency coefficients for given frequency index,
     writes 2S02 product and returns indices to be flagged"""
 
     flag_ind = np.zeros(data["tb"].shape, dtype=np.int32)
     abs_diff = ma.masked_all(data["tb"].shape, dtype=np.float32)
-    data["tb_spectrum"] = np.ones(data["tb"].shape) * np.nan
+    data["tb_spectrum"] = ma.masked_all(data["tb"].shape)
 
     c_list = get_coeff_list(site, "spc", coeff_files)
 
     if len(c_list) > 0:
         # pylint: disable=unbalanced-tuple-unpacking
         (
             coeff,
```

### Comparing `mwrpy-0.8.3/mwrpy/level1/rpg_bin.py` & `mwrpy-0.9.0/mwrpy/level1/rpg_bin.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,41 +2,37 @@
 import datetime
 import logging
 from collections.abc import Callable
 from io import SEEK_END
 from typing import Any, BinaryIO, Literal, TypeAlias
 
 import numpy as np
+from numpy import ma
 
 from mwrpy import utils
 from mwrpy.exceptions import InvalidFileError, MissingInputData
 
-Fill_Value_Float = -999.0
-Fill_Value_Int = -99
-
 Dim = int | tuple[int, ...]
 Field = tuple[str, str] | tuple[str, str, Dim]
 
 
 def stack_files(file_list: list[str]) -> tuple[dict, dict]:
     """This function calls extension specific reader and stacks data and header."""
 
     def _stack_data(source: dict, target: dict, fun: Callable):
         for name, value in source.items():
+            value = ma.array(value)
             if value.ndim > 0 and name in target:
                 if target[name].ndim == value.ndim:
                     if (
                         value.ndim > 1
                         and value.shape[1] != target[name].shape[1]
                         and name == "irt"
                     ):
-                        value = np.hstack(
-                            (value, np.ones((len(value), 1)) * Fill_Value_Float)
-                        )
-                        target[name] = fun((target[name], value))
+                        raise NotImplementedError("Inconsistent number of IRT channels")
                     else:
                         target[name] = fun((target[name], value))
             elif value.ndim > 0 and name not in target:
                 target[name] = value
 
     def _stack_header(source: dict, target: dict, fun: Callable):
         for name, value in source.items():
```

### Comparing `mwrpy-0.8.3/mwrpy/level1/write_lev1_nc.py` & `mwrpy-0.9.0/mwrpy/level1/write_lev1_nc.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,14 @@
     add_time_bounds,
     get_file_list,
     isbit,
     read_config,
     update_lev1_attributes,
 )
 
-Fill_Value_Float = -999.0
-Fill_Value_Int = -99
 FuncType: TypeAlias = Callable[[str], np.ndarray]
 
 
 def lev1_to_nc(
     data_type: str,
     path_to_files: str,
     site: str | None = None,
@@ -147,28 +145,28 @@
             _add_bls(rpg_bin, rpg_bls, rpg_hkd, params)
         else:
             file_list_blb = get_file_list(path_to_files, "BLB")
             if len(file_list_blb) > 0 and np.any(rpg_hkd.data["status"][:] & 2**18 > 0):
                 rpg_blb = RpgBin(file_list_blb)
                 _add_blb(rpg_bin, rpg_blb, rpg_hkd, params)
 
-        if params["azi_cor"] != Fill_Value_Float:
+        if params["azi_cor"] != -999.0:
             _azi_correction(rpg_bin.data, params)
 
-        if params["const_azi"] != Fill_Value_Float:
+        if params["const_azi"] != -999.0:
             rpg_bin.data["azimuth_angle"] = (
                 rpg_bin.data["azimuth_angle"] + params["const_azi"]
             ) % 360
 
         if data_type == "1C01":
             if params["ir_flag"]:
                 file_list_irt = get_file_list(path_to_files, "IRT")
                 if len(file_list_irt) > 0:
                     rpg_irt = RpgBin(file_list_irt)
-                    rpg_irt.data["irt"][rpg_irt.data["irt"] <= 125.5] = Fill_Value_Float
+                    rpg_irt.data["irt"][rpg_irt.data["irt"] <= 125.5] = ma.masked
                     rpg_bin.data["ir_wavelength"] = rpg_irt.header["_f"] * 1e-6
                     rpg_bin.data["ir_bandwidth"] = params["ir_bandwidth"] * 1e-6
                     rpg_bin.data["ir_beamwidth"] = params["ir_beamwidth"]
                     add_interpol1d(
                         rpg_bin.data, rpg_irt.data["irt"], rpg_irt.data["time"], "irt"
                     )
                     add_interpol1d(
@@ -273,39 +271,39 @@
         add_interpol1d(
             rpg_bin.data,
             np.ones(len(hkd.data["time"])) * params["latitude"],
             hkd.data["time"],
             "latitude",
         )
     else:
-        idx = np.where(hkd.data["latitude"] != Fill_Value_Float)[0]
+        idx = np.where(~ma.getmaskarray(hkd.data["latitude"]))[0]
         add_interpol1d(
             rpg_bin.data,
             hkd.data["latitude"][idx],
             hkd.data["time"][idx],
             "latitude",
         )
     if "longitude" not in hkd.data:
         add_interpol1d(
             rpg_bin.data,
             np.ones(len(hkd.data["time"])) * params["longitude"],
             hkd.data["time"],
             "longitude",
         )
     else:
-        idx = np.where(hkd.data["longitude"] != Fill_Value_Float)[0]
+        idx = np.where(~ma.getmaskarray(hkd.data["longitude"]))[0]
         add_interpol1d(
             rpg_bin.data,
             hkd.data["longitude"][idx],
             hkd.data["time"][idx],
             "longitude",
         )
 
     if data_type in ("1B01", "1C01"):
-        hkd.data["temp"][hkd.data["temp"] >= 350.0] = Fill_Value_Float
+        hkd.data["temp"][hkd.data["temp"] >= 350.0] = ma.masked
         add_interpol1d(
             rpg_bin.data, hkd.data["temp"][:, 0:2], hkd.data["time"], "t_amb"
         )
         add_interpol1d(
             rpg_bin.data, hkd.data["temp"][:, 2:4], hkd.data["time"], "t_rec"
         )
         add_interpol1d(rpg_bin.data, hkd.data["stab"], hkd.data["time"], "t_sta")
@@ -352,16 +350,16 @@
             ind_hkd = np.argmin(np.abs(hkd.data["time"] - time_bls))
             bls.data["status"][time_ind, :] = hkd_sanity_check(
                 np.array([hkd.data["status"][ind_hkd]], np.int32), params
             )
 
     bls.data["pointing_flag"] = np.ones(len(bls.data["time"]), np.int32)
     bls.data["liquid_cloud_flag"] = np.ones(len(bls.data["time"]), np.int32) * 2
-    bls.data["liquid_cloud_flag_status"] = (
-        np.ones(len(bls.data["time"]), np.int32) * Fill_Value_Int
+    bls.data["liquid_cloud_flag_status"] = ma.masked_all(
+        len(bls.data["time"]), np.int32
     )
     brt.data["time"] = np.concatenate((brt.data["time"], bls.data["time"]))
     ind = np.argsort(brt.data["time"])
     brt.data["time"] = brt.data["time"][ind]
 
     names = [
         "time_bnds",
@@ -399,15 +397,15 @@
     seqs = np.array(
         [
             (key, sum(s[1] for s in seqs_all[:i]), length)
             for i, (key, length) in enumerate(seqs_all)
             if bool(key) is True
         ]
     )
-    scan_time = np.median(seqs[1:-1, 2])
+    scan_time = np.median(seqs[:, 2])
 
     for time_ind, time_blb in enumerate(blb.data["time"]):
         seqi = np.where(
             np.abs(hkd.data["time"][seqs[:, 1] + seqs[:, 2] - 1] - time_blb) < 60
         )[0]
         if len(seqi) != 1:
             time_blb = time_blb + int(scan_time)
@@ -503,15 +501,15 @@
                 status_add = blb_status_add
             else:
                 status_add = np.concatenate((status_add, blb_status_add))
 
     if len(time_add) > 0:
         pointing_flag_add = np.ones(len(time_add), np.int32)
         liquid_cloud_flag_add = np.ones(len(time_add), np.int32) * 2
-        liquid_cloud_flag_status_add = np.ones(len(time_add), np.int32) * Fill_Value_Int
+        liquid_cloud_flag_status_add = ma.masked_all(len(time_add), np.int32)
         brt.data["time"] = np.concatenate((brt.data["time"], time_add))
         ind = np.argsort(brt.data["time"])
         brt.data["time"] = brt.data["time"][ind]
 
         names_add: dict[str, np.ndarray] = {
             "time_bnds": time_bnds_add,
             "elevation_angle": elevation_angle_add,
```

### Comparing `mwrpy-0.8.3/mwrpy/level2/get_ret_coeff.py` & `mwrpy-0.9.0/mwrpy/level2/get_ret_coeff.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Module to load in retrieval coefficient files"""
 import netCDF4 as nc
 import numpy as np
+from numpy import ma
 
 from mwrpy.utils import get_coeff_list
 
-Fill_Value_Float = -999.0
-Fill_Value_Int = -99
-
 
 def get_mvr_coeff(
     site: str | None, prefix: str, freq: np.ndarray, coeff_files: list | None
 ):
     """This function extracts retrieval coefficients for given files.
 
     Args:
@@ -51,20 +49,20 @@
         ]
         for aux_i in aux:
             if aux_i not in coeff:
                 coeff[aux_i] = 0
         coeff["FR_BL"] = coeff["FR"]
 
     elif (str(c_list[0][-2:]).lower() == "nc") and (len(c_list) > 0):
-        coeff["RT"] = Fill_Value_Int
+        coeff["RT"] = -1
         N = len(c_list)
 
         if prefix in ("lwp", "iwv"):
-            coeff["AG"] = np.ones(N) * Fill_Value_Float
-            coeff["FR"] = np.ones([len(freq), N]) * Fill_Value_Float
+            coeff["AG"] = ma.masked_all(N)
+            coeff["FR"] = ma.masked_all([len(freq), N])
             coeff["TL"] = np.zeros([N, len(freq)])
             coeff["TQ"] = np.zeros([N, len(freq)])
             coeff["OS"] = np.zeros(N)
             coeff["AL"] = [0]
 
             for i_file, file in enumerate(c_list):
                 c_file = nc.Dataset(file)
@@ -85,16 +83,16 @@
                     ]
                 coeff["OS"][i_file] = c_file["offset_mvr"][0]
 
         elif prefix in ("tpt", "hpt"):
             c_file = nc.Dataset(c_list[0])
             n_height_grid = c_file.dimensions["n_height_grid"].size
 
-            coeff["AG"] = np.ones(N) * Fill_Value_Float
-            coeff["FR"] = np.ones([len(freq), N]) * Fill_Value_Float
+            coeff["AG"] = ma.masked_all(N)
+            coeff["FR"] = ma.masked_all([len(freq), N])
             coeff["TL"] = np.zeros([N, n_height_grid, len(freq)])
             coeff["TQ"] = np.zeros([N, n_height_grid, len(freq)])
             coeff["OS"] = np.zeros([n_height_grid, N])
             coeff["n_height_grid"] = n_height_grid
             coeff["AL"] = c_file["height_grid"]
 
             for i_file, file in enumerate(c_list):
@@ -141,63 +139,63 @@
                 [
                     "Prefix "
                     + prefix
                     + " not recognized for retrieval coefficient file(s)."
                 ]
             )
 
-    if (coeff["RT"] < 2) & (len(coeff["AL"]) == 1):
+    if (coeff["RT"] < 2) and (len(coeff["AL"]) == 1):
 
         def f_offset(x):
             return np.array(
                 [coeff["OS"][(np.abs(coeff["AG"] - v)).argmin()] for v in x]
             )
 
         if coeff["RT"] in (0, 1):
             coeff["TL"] = coeff["TL"][np.newaxis, :]
 
         def f_lin(x):
             return np.array(
                 [coeff["TL"][(np.abs(coeff["AG"] - v)).argmin(), :] for v in x]
             )
 
-        if coeff["RT"] in (1, Fill_Value_Int):
+        if coeff["RT"] in (1, -1):
             if coeff["RT"] == 1:
                 coeff["TQ"] = coeff["TQ"][np.newaxis, :]
 
             def f_quad(x):
                 return np.array(
                     [coeff["TQ"][(np.abs(coeff["AG"] - v)).argmin(), :] for v in x]
                 )
 
-    elif (coeff["RT"] < 2) & (len(coeff["AL"]) > 1) & (prefix != "tpb"):
+    elif (coeff["RT"] < 2) and (len(coeff["AL"]) > 1) and (prefix != "tpb"):
 
         def f_offset(x):
             return np.array(
                 [coeff["OS"][:, (np.abs(coeff["AG"] - v)).argmin()] for v in x]
             )
 
         if coeff["RT"] in (0, 1):
             coeff["TL"] = coeff["TL"][np.newaxis, :, :]
 
         def f_lin(x):
             return np.array(
                 [coeff["TL"][(np.abs(coeff["AG"] - v)).argmin(), :, :] for v in x]
             )
 
-        if coeff["RT"] in (1, Fill_Value_Int):
+        if coeff["RT"] in (1, -1):
             if coeff["RT"] == 1:
                 coeff["TQ"] = coeff["TQ"][np.newaxis, :, :]
 
             def f_quad(x):
                 return np.array(
                     [coeff["TQ"][(np.abs(coeff["AG"] - v)).argmin(), :, :] for v in x]
                 )
 
-    elif (coeff["RT"] < 2) & (len(coeff["AL"]) > 1) & (prefix == "tpb"):
+    elif (coeff["RT"] < 2) and (len(coeff["AL"]) > 1) and (prefix == "tpb"):
 
         def f_offset(_x):
             return coeff["OS"]
 
         def f_lin(_x):
             return coeff["TL"]
 
@@ -258,26 +256,26 @@
             return np.array(
                 [coeff["NP"][(np.abs(coeff["AG"] - v)).argmin()] for v in x]
             )
 
     if str(c_list[0][-3:]).lower() == "ret":
         retrieval_type = ["linear regression", "quadratic regression", "neural network"]
         coeff["retrieval_type"] = retrieval_type[int(coeff["RT"][0])]
-        coeff["retrieval_elevation_angles"] = str(coeff["AG"])
-        coeff["retrieval_frequencies"] = str(coeff["FR"][:])
+        coeff["retrieval_elevation_angles"] = coeff["AG"]
+        coeff["retrieval_frequencies"] = coeff["FR"]
         if coeff["TS"] == 0:
             coeff["retrieval_auxiliary_input"] = "no_surface"
         else:
             coeff["retrieval_auxiliary_input"] = "surface"
         coeff["retrieval_description"] = "RPG retrieval"
 
     elif str(c_list[0][-2:]).lower() == "nc":
         coeff["retrieval_type"] = c_file.regression_type
-        coeff["retrieval_elevation_angles"] = str(coeff["AG"])
-        coeff["retrieval_frequencies"] = str(c_file["freq"][:])
+        coeff["retrieval_elevation_angles"] = coeff["AG"]
+        coeff["retrieval_frequencies"] = c_file["freq"]
         coeff["retrieval_auxiliary_input"] = c_file.surface_mode
         coeff["retrieval_description"] = c_file.retrieval_version
 
     return (
         (coeff, f_offset, f_lin, f_quad)
         if (coeff["RT"] < 2)
         else (
```

### Comparing `mwrpy-0.8.3/mwrpy/level2/lev2_collocated.py` & `mwrpy-0.9.0/mwrpy/level2/lev2_collocated.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/level2/lev2_meta_nc.py` & `mwrpy-0.9.0/mwrpy/level2/lev2_meta_nc.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     ),
     "altitude": MetaData(
         long_name="Altitude above mean sea level of measurement station",
         standard_name="altitude",
         units="m",
     ),
     "azimuth_angle": MetaData(
-        long_name="Sensor azimuth angle",
+        long_name="Azimuth angle",
         standard_name="sensor_azimuth_angle",
         units="degree",
         comment="0=North, 90=East, 180=South, 270=West",
     ),
     "elevation_angle": MetaData(
         long_name="Sensor elevation angle",
         units="degree",
```

### Comparing `mwrpy-0.8.3/mwrpy/level2/lwp_offset.py` & `mwrpy-0.9.0/mwrpy/level2/lwp_offset.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/level2/write_lev2_nc.py` & `mwrpy-0.9.0/mwrpy/level2/write_lev2_nc.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,19 @@
 from mwrpy import rpg_mwr
 from mwrpy.atmos import eq_pot_tem, pot_tem, rel_hum
 from mwrpy.exceptions import MissingInputData
 from mwrpy.level2.get_ret_coeff import get_mvr_coeff
 from mwrpy.level2.lev2_meta_nc import get_data_attributes
 from mwrpy.level2.lwp_offset import correct_lwp_offset
 from mwrpy.utils import (
-    get_ret_info,
     interpol_2d,
     interpolate_2d,
     read_config,
 )
 
-Fill_Value_Float = -999.0
-Fill_Value_Int = -99
-
 
 def lev2_to_nc(
     data_type: str,
     lev1_file: str,
     output_file: str,
     site: str | None = None,
     temp_file: str | None = None,
@@ -124,20 +120,18 @@
 
         index = np.where(lev1["pointing_flag"][:] == 0)[0]  # type: ignore
         if len(index) == 0:
             raise MissingInputData(
                 f"No suitable data found for processing for data type: {data_type}"
             )
 
-        coeff["retrieval_elevation_angles"] = str(
-            np.sort(np.unique(ele_retrieval(elevation_angle[index], coeff)))
-        )
-        coeff["retrieval_frequencies"] = str(
-            np.sort(np.unique(coeff["FR"][coeff["FR"][:] > 0.0]))
+        coeff["retrieval_elevation_angles"] = _format_attribute_array(
+            ele_retrieval(elevation_angle[index], coeff)
         )
+        coeff["retrieval_frequencies"] = _get_retrieval_frequencies(coeff)
 
         if coeff["RT"] < 2:
             coeff_offset = offset(elevation_angle[index])
             coeff_lin = lin(elevation_angle[index])
             coeff_quad = quad(elevation_angle[index])
             tmp_product = (
                 coeff_offset[:]
@@ -186,22 +180,22 @@
                         * elevation_angle[index]
                     )
                 )
                 <= 0.5,
                 axis=1,
             )
         )[0]  # type: ignore
-        ret_product = np.ones(len(index), np.float32) * Fill_Value_Float
+        ret_product = ma.masked_all(len(index), np.float32)
         ret_product[index_ret] = tmp_product[index_ret]
 
         if product == "lwp":
             freq_win = np.where((np.round(lev1["frequency"][:], 1) == 31.4))[0]
             rpg_dat["lwp"], rpg_dat["lwp_offset"] = (
                 ret_product,
-                np.ones(len(index)) * Fill_Value_Float,
+                ma.masked_all(len(index)),
             )
             if len(freq_win) == 1 and len(index_ret) > 0:
                 (
                     rpg_dat["lwp"][index_ret],
                     rpg_dat["lwp_offset"][index_ret],
                 ) = correct_lwp_offset(
                     lev1.variables, ret_product[index_ret], index[index_ret]
@@ -238,33 +232,32 @@
         ret_in = retrieval_input(lev1, coeff)
 
         index = np.where(lev1["pointing_flag"][:] == 0)[0]  # type: ignore
         if len(index) == 0:
             raise MissingInputData(
                 f"No suitable data found for processing for data type: {data_type}"
             )
-        coeff["retrieval_elevation_angles"] = str(
-            np.sort(np.unique(ele_retrieval(elevation_angle[index], coeff)))
-        )
-        coeff["retrieval_frequencies"] = str(
-            np.sort(np.unique(coeff["FR"][coeff["FR"][:] > 0.0]))
+        coeff["retrieval_elevation_angles"] = _format_attribute_array(
+            ele_retrieval(elevation_angle[index], coeff)
         )
 
+        coeff["retrieval_frequencies"] = _get_retrieval_frequencies(coeff)
+
         rpg_dat["height"] = coeff["AL"][:] + params["altitude"]
 
         if coeff["RT"] < 2:
             coeff_offset = offset(elevation_angle[index])
             coeff_lin = lin(elevation_angle[index])
             coeff_quad = quad(elevation_angle[index])
             tmp_dat = (
                 coeff_offset
                 + np.einsum("ijk,ik->ij", coeff_lin, ret_in[index, :])
                 + np.einsum("ijk,ik->ij", coeff_quad, ret_in[index, :] ** 2)
             )
-            if (coeff["RT"] == 1) & (data_type == "2P03"):
+            if (coeff["RT"] == 1) and (data_type == "2P03"):
                 tmp_dat[:, :] = tmp_dat[:, :] / 1000.0
 
         else:
             c_w1, c_w2, fac = (
                 weights1(elevation_angle[index]),
                 weights2(elevation_angle[index]),
                 factor(elevation_angle[index]),
@@ -309,16 +302,16 @@
                         * elevation_angle[index]
                     )
                 )
                 <= 0.5,
                 axis=1,
             )
         )[0]  # type: ignore
-        rpg_dat[product] = (
-            np.ones((len(index), len(rpg_dat["height"])), np.float32) * Fill_Value_Float
+        rpg_dat[product] = ma.masked_all(
+            (len(index), len(rpg_dat["height"])), np.float32
         )
         rpg_dat[product][index_ret, :] = tmp_dat[index_ret, :]
 
     elif data_type == "2P02":
         coeff = get_mvr_coeff(site, "tpb", lev1["frequency"][:], coeff_files)
         if coeff[0]["RT"] < 2:
             coeff, offset, lin, quad = get_mvr_coeff(
@@ -336,28 +329,25 @@
             coeff["FR"],
             assume_unique=False,
             return_indices=True,
         )
         _, freq_bl, _ = np.intersect1d(
             coeff["FR"], coeff["FR_BL"], assume_unique=False, return_indices=True
         )
-        coeff["retrieval_frequencies"] = str(
-            np.sort(np.unique(coeff["FR"][coeff["FR"][:] > 0.0]))
-        )
+        coeff["retrieval_frequencies"] = _get_retrieval_frequencies(coeff)
 
         ix0 = np.where(
             (elevation_angle[:] > coeff["AG"][0] - 0.5)
             & (elevation_angle[:] < coeff["AG"][0] + 0.5)
             & (lev1["pointing_flag"][:] == 1)
             & (np.arange(len(lev1["time"])) + len(coeff["AG"]) < len(lev1["time"]))
         )[0]
         ibl, tb, scan_time = (
             np.empty([0, len(coeff["AG"])], np.int32),
-            np.ones((len(freq_ind), len(coeff["AG"]), 0), np.float32)
-            * Fill_Value_Float,
+            ma.masked_all((len(freq_ind), len(coeff["AG"]), 0), np.float32),
             np.empty(0, np.int32),
         )
 
         for ix0v in ix0:
             ix1v = ix0v + len(coeff["AG"])
 
             if (ix1v < len(lev1["time"])) & (
@@ -439,44 +429,23 @@
     elif data_type in ("2P04", "2P07", "2P08"):
         assert temp_file is not None
         assert hum_file is not None
         tem_dat = load_product(temp_file)
         hum_dat = load_product(hum_file)
 
         coeff, index = {}, np.empty(0, np.int32)
-        coeff["retrieval_frequencies"] = str(
-            np.unique(
-                np.sort(
-                    np.concatenate(
-                        [
-                            get_ret_info(tem_dat["temperature"].retrieval_frequencies),
-                            get_ret_info(
-                                hum_dat["absolute_humidity"].retrieval_frequencies
-                            ),
-                        ]
-                    )
-                )
-            )
+
+        coeff["retrieval_frequencies"] = _combine_array_attributes(
+            tem_dat, hum_dat, "retrieval_frequencies"
         )
-        coeff["retrieval_elevation_angles"] = str(
-            np.unique(
-                np.sort(
-                    np.concatenate(
-                        [
-                            get_ret_info(
-                                tem_dat["temperature"].retrieval_elevation_angles
-                            ),
-                            get_ret_info(
-                                hum_dat["absolute_humidity"].retrieval_elevation_angles
-                            ),
-                        ]
-                    )
-                )
-            )
+
+        coeff["retrieval_elevation_angles"] = _combine_array_attributes(
+            tem_dat, hum_dat, "retrieval_elevation_angles"
         )
+
         coeff["retrieval_type"] = "derived product"
         coeff["dependencies"] = temp_file + ", " + hum_file
         if len(hum_dat.variables["height"][:]) == len(tem_dat.variables["height"][:]):
             hum_int = interpol_2d(
                 hum_dat.variables["time"][:],
                 hum_dat.variables["absolute_humidity"][:, :],
                 tem_dat.variables["time"][:],
@@ -563,15 +532,15 @@
             if ivars not in lev1.variables:
                 continue
             if (ivars == "time_bnds") & (data_type == "2P02"):
                 rpg_dat[ivars] = np.ndarray((len(index), 2))
                 rpg_dat[ivars][:, 0] = lev1["time"][index] - scan_time
                 rpg_dat[ivars][:, 1] = lev1["time"][index]
             elif (ivars == "time_bnds") & (data_type in ("2P04", "2P07", "2P08")):
-                rpg_dat[ivars] = np.ones(lev1[ivars].shape, np.int32) * Fill_Value_Int
+                rpg_dat[ivars] = ma.masked_all(lev1[ivars].shape, np.int32)
             else:
                 try:
                     rpg_dat[ivars] = lev1[ivars][index]
                 except IndexError:
                     rpg_dat[ivars] = lev1[ivars][:]
 
 
@@ -614,15 +583,15 @@
         return_indices=True,
     )
     bias = np.ones((len(lev1["time"][:]), 1), np.float32)
 
     latitude = float(ma.median(lev1["latitude"][:]))
     longitude = float(ma.median(lev1["longitude"][:]))
 
-    if coeff["RT"] == Fill_Value_Int:
+    if coeff["RT"] == -1:
         ret_in = lev1["tb"][:, :]
     elif coeff["RT"] in (0, 1):
         ret_in = lev1["tb"][:, freq_ind]
     else:
         ret_in = np.concatenate((bias, lev1["tb"][:, freq_ind]), axis=1)
 
         _data = coeff.get("TS")
@@ -672,15 +641,15 @@
                 (
                     ret_in,
                     np.reshape(lev1["irt"][:, 1], (len(lev1["time"][:]), 1)),
                 ),
                 axis=1,
             )
         if coeff.get("DY") == 1:
-            doy = np.ones((len(lev1["time"][:]), 2), np.float32) * Fill_Value_Float
+            doy = ma.masked_all((len(lev1["time"][:]), 2), np.float32)
             tf = TimezoneFinder()
             timezone_str = tf.timezone_at(
                 lng=longitude,
                 lat=latitude,
             )
             assert timezone_str is not None
             timezone = pytz.timezone(timezone_str)
@@ -696,15 +665,15 @@
                 datetime.fromtimestamp(time_median).timetuple().tm_yday
                 / dyear
                 * 2
                 * np.pi
             )
             ret_in = np.concatenate((ret_in, doy), axis=1)
         if coeff.get("SU") == 1:
-            sun = np.ones((len(lev1["time"][:]), 2), np.float32) * Fill_Value_Float
+            sun = ma.masked_all((len(lev1["time"][:]), 2), np.float32)
             tf = TimezoneFinder()
             timezone_str = tf.timezone_at(
                 lng=longitude,
                 lat=latitude,
             )
             assert timezone_str is not None
             timezone = pytz.timezone(timezone_str)
@@ -719,7 +688,26 @@
 
     return ret_in
 
 
 def decimal_hour2unix(date: list, time: np.ndarray) -> np.ndarray | int:
     unix_timestamp = np.datetime64("-".join(date)).astype("datetime64[s]").astype("int")
     return (time * 60 * 60 + unix_timestamp).astype(int)
+
+
+def _get_retrieval_frequencies(coeff: dict) -> np.ndarray:
+    if isinstance(coeff["FR"], ma.MaskedArray):
+        frequencies = coeff["FR"][~coeff["FR"][:].mask]
+    else:
+        frequencies = coeff["FR"]
+    return _format_attribute_array(frequencies)
+
+
+def _combine_array_attributes(tem_dat: dict, hum_dat: dict, name: str) -> np.ndarray:
+    a = getattr(tem_dat["temperature"], name)
+    b = getattr(hum_dat["absolute_humidity"], name)
+    combined = np.hstack((a, b))
+    return _format_attribute_array(combined)
+
+
+def _format_attribute_array(array: np.ndarray | list) -> np.ndarray:
+    return np.round(np.sort(np.unique(array)), 2)
```

### Comparing `mwrpy-0.8.3/mwrpy/plots/generate_plots.py` & `mwrpy-0.9.0/mwrpy/plots/generate_plots.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/plots/plot_meta.py` & `mwrpy-0.9.0/mwrpy/plots/plot_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         name="Sensor elevation angle",
         ylabel=_DEG,
         plot_range=(-1, 93),
         plot_type="bar",
         source="sen",
     ),
     "azimuth_angle": PlotMeta(
-        name="Sensor azimuth angle",
+        name="Azimuth angle",
         ylabel=_DEG,
         plot_range=(-5, 363),
         plot_type="bar",
         source="sen",
     ),
     "quality_flag": PlotMeta(name="Quality flag", source="qf"),
     "quality_flag_0": PlotMeta(
```

### Comparing `mwrpy-0.8.3/mwrpy/plots/plot_utils.py` & `mwrpy-0.9.0/mwrpy/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/process_mwrpy.py` & `mwrpy-0.9.0/mwrpy/process_mwrpy.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/rpg_mwr.py` & `mwrpy-0.9.0/mwrpy/rpg_mwr.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         return attributes
 
     def set_attributes(self, attributes: MetaData) -> None:
         """Overwrites existing instance attributes."""
 
         for key in attributes._fields:  # To iterate namedtuple fields.
             data = getattr(attributes, key)
-            if data:
+            if data is not None:
                 setattr(self, key, data)
 
     def _init_data(self) -> np.ndarray:
         if isinstance(self.variable, netCDF4.Variable):
             return self.variable[:]
         if isinstance(self.variable, np.ndarray):
             return self.variable
@@ -229,30 +229,28 @@
     return tuple(dim_names)
 
 
 def _write_vars2nc(nc_file: netCDF4.Dataset, mwr_variables: dict) -> None:
     """Iterates over RPG instances and write to netCDF file."""
 
     for obj in mwr_variables.values():
-        if obj.data_type == "f4":
-            fill_value = -999.0
-        else:
-            fill_value = -99
+        fill_value = netCDF4.default_fillvals[obj.data_type]
 
         size = obj.dimensions or _get_dimensions(nc_file, obj.data)
         if obj.name == "time_bnds":
             size = ("time", "bnds")
         if obj.name == "receiver_nb":
             size = "receiver_nb"
         if obj.name == "irt":
             size = ("time", "ir_wavelength")
         if obj.name == "ir_wavelength":
             size = "ir_wavelength"
         if obj.name == "t_amb":
             size = ("time", "t_amb_nb")
+
         nc_variable = nc_file.createVariable(
             obj.name, obj.data_type, size, zlib=True, fill_value=fill_value
         )
         nc_variable[:] = obj.data
         for attr in obj.fetch_attributes():
             setattr(nc_variable, attr, getattr(obj, attr))
```

### Comparing `mwrpy-0.8.3/mwrpy/site_config/hatpro.yaml` & `mwrpy-0.9.0/mwrpy/site_config/hatpro.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.9.0/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.9.0/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.9.0/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.9.0/mwrpy/site_config/hyytiala/coefficients/SPC_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.9.0/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.9.0/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/hyytiala/config.yaml` & `mwrpy-0.9.0/mwrpy/site_config/hyytiala/config.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc` & `mwrpy-0.9.0/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/juelich/config.yaml` & `mwrpy-0.9.0/mwrpy/site_config/juelich/config.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.9.0/mwrpy/site_config/lindenberg/coefficients/HPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.9.0/mwrpy/site_config/lindenberg/coefficients/IWV_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.9.0/mwrpy/site_config/lindenberg/coefficients/LWP_NN_MA_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.9.0/mwrpy/site_config/lindenberg/coefficients/SPC_NN_MA_INS_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.9.0/mwrpy/site_config/lindenberg/coefficients/TPB_NN_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret` & `mwrpy-0.9.0/mwrpy/site_config/lindenberg/coefficients/TPT_NN_DE_Lindenberg_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/lindenberg/config.yaml` & `mwrpy-0.9.0/mwrpy/site_config/lindenberg/config.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/palaiseau/coefficients/HPT_NN_FR_SIRTA_HATPRO_G5_v121.ret` & `mwrpy-0.9.0/mwrpy/site_config/palaiseau/coefficients/HPT_NN_FR_SIRTA_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/palaiseau/coefficients/IWV_NN_MA_FR_SIRTA_HATPRO_G5_v121.ret` & `mwrpy-0.9.0/mwrpy/site_config/palaiseau/coefficients/IWV_NN_MA_FR_SIRTA_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/palaiseau/coefficients/LWP_NN_MA_FR_SIRTA_HATPRO_G5_v121.ret` & `mwrpy-0.9.0/mwrpy/site_config/palaiseau/coefficients/LWP_NN_MA_FR_SIRTA_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/palaiseau/coefficients/SPC_NN_MA_INS_FR_SIRTA_HATPRO_G5_v121.ret` & `mwrpy-0.9.0/mwrpy/site_config/palaiseau/coefficients/SPC_NN_MA_INS_FR_SIRTA_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/palaiseau/coefficients/TPB_NN_FR_SIRTA_HATPRO_G5_v121.ret` & `mwrpy-0.9.0/mwrpy/site_config/palaiseau/coefficients/TPB_NN_FR_SIRTA_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/palaiseau/coefficients/TPT_NN_FR_SIRTA_HATPRO_G5_v121.ret` & `mwrpy-0.9.0/mwrpy/site_config/palaiseau/coefficients/TPT_NN_FR_SIRTA_HATPRO_G5_v121.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/site_config/palaiseau/config.yaml` & `mwrpy-0.9.0/mwrpy/site_config/palaiseau/config.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/mwrpy/utils.py` & `mwrpy-0.9.0/mwrpy/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Module for general helper functions."""
 
 import datetime
 import glob
 import logging
 import os
-import re
 import time
 from typing import Any, Iterator, Literal, NamedTuple
 
 import netCDF4
 import numpy as np
 import pandas as pd
 import yaml
@@ -16,16 +15,14 @@
 from scipy import signal
 from scipy.interpolate import RectBivariateSpline
 from yaml.loader import SafeLoader
 
 SECONDS_PER_MINUTE = 60
 SECONDS_PER_HOUR = 3600
 SECONDS_PER_DAY = 86400
-Fill_Value_Float = -999.0
-Fill_Value_Int = -99
 Epoch = tuple[int, int, int]
 
 
 class MetaData(NamedTuple):
     long_name: str
     units: str
     standard_name: str | None = None
@@ -200,32 +197,51 @@
 
     """
     fun = RectBivariateSpline(x, y, z, kx=1, ky=1)
     return fun(x_new, y_new)
 
 
 def add_interpol1d(
-    data0: dict, data1: np.ndarray, time1: np.ndarray, output_name: str
+    data0: dict, data1: ma.MaskedArray, time1: np.ndarray, output_name: str
 ) -> None:
-    """Adds interpolated 1d field to dict
+    """Adds interpolated 1d field to dict, supporting masked arrays.
+
     Args:
         data0: Output dict.
-        data1: Input field to be added & interpolated.
+        data1: Input field to be added & interpolated. Supports masked arrays.
         time1: Time of input field.
+        output_name: Name of output field.
     """
-    if data1.ndim > 1:
-        data0[output_name] = (
-            np.ones([len(data0["time"]), data1.shape[1]], np.float32) * Fill_Value_Float
-        )
-        for ndim in range(data1.shape[1]):
-            data0[output_name][:, ndim] = np.interp(
-                data0["time"], time1, data1[:, ndim]
+
+    interpolated_data: np.ndarray = np.array([])
+    n_time = len(data0["time"])
+
+    itr = data1.T if data1.ndim > 1 else [data1]
+
+    for input_data in itr:
+        valid_mask = ~ma.getmaskarray(input_data)
+        if ~valid_mask.all():
+            result = ma.masked_all(n_time)
+        else:
+            valid_data = input_data[valid_mask]
+            valid_time = time1[valid_mask]
+            interpolated_values = np.interp(data0["time"], valid_time, valid_data)
+            interpolated_mask = (
+                np.interp(data0["time"], valid_time, valid_mask.astype(float)) < 0.5
             )
-    else:
-        data0[output_name] = np.interp(data0["time"], time1, data1)
+            result = ma.masked_array(interpolated_values, mask=interpolated_mask)
+        interpolated_data = (
+            result
+            if len(interpolated_data) == 0
+            else ma.vstack((interpolated_data, result))
+        )
+    if data1.ndim > 1:
+        interpolated_data = np.reshape(interpolated_data.T, (n_time, -1))
+
+    data0[output_name] = interpolated_data
 
 
 def seconds2date(time_in_seconds: float, epoch: Epoch = (1970, 1, 1)) -> list:
     """Converts seconds since some epoch to datetime (UTC).
     Args:
         time_in_seconds: Seconds since some epoch.
         epoch: Epoch, default is (1970, 1, 1) (UTC).
@@ -250,15 +266,15 @@
         return int(value)
     except ValueError:
         return float(value)
 
 
 def add_time_bounds(time_arr: np.ndarray, int_time: int) -> np.ndarray:
     """Adds time bounds"""
-    time_bounds = np.ones([len(time_arr), 2], np.int32) * Fill_Value_Int
+    time_bounds = np.empty((len(time_arr), 2), dtype=np.int32)
     time_bounds[:, 0] = time_arr - int_time
     time_bounds[:, 1] = time_arr
 
     return time_bounds
 
 
 def get_coeff_list(site: str | None, prefix: str, coeff_files: list | None) -> list:
@@ -375,24 +391,14 @@
         attributes["source"] = "In Situ"
 
     for name in list(attributes.keys()):
         if any(x in name for x in att_del) & (name[0:3] != key):
             del attributes[name]
 
 
-def get_ret_info(ret_org: str) -> np.ndarray:
-    """Returns frequencies or angles used in retrieval."""
-    ret_inf = []
-    ret_str = re.split(r"[^0-9.]", ret_org)
-    for ii in ret_str:
-        if ii != "":
-            ret_inf.append(float(ii))
-    return np.array(ret_inf, dtype=np.float32)
-
-
 def read_nc_field_name(nc_file: str, name: str) -> str:
     """Reads selected variable name from a netCDF file.
     Args:
         nc_file: netCDF file name.
         name: Variable to be read, e.g. 'temperature'.
     Returns:
         str
```

### Comparing `mwrpy-0.8.3/mwrpy.egg-info/PKG-INFO` & `mwrpy-0.9.0/mwrpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwrpy
-Version: 0.8.3
+Version: 0.9.0
 Summary: Python package for Microwave Radiometer processing in ACTRIS
 Author-email: University of Cologne <actris-ccres-mwr@uni-koeln.de>
 License: MIT License
         
         Copyright (c) 2021-2023 University of Cologne
         Copyright (c) 2023 Finnish Meteorological Institute
```

### Comparing `mwrpy-0.8.3/mwrpy.egg-info/SOURCES.txt` & `mwrpy-0.9.0/mwrpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mwrpy-0.8.3/pyproject.toml` & `mwrpy-0.9.0/pyproject.toml`

 * *Files identical despite different names*

