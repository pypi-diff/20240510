# Comparing `tmp/skyCatalogs-1.7.0rc2.tar.gz` & `tmp/skycatalogs-1.7.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyCatalogs-1.7.0rc2.tar", last modified: Fri Feb 16 00:59:47 2024, max compression
+gzip compressed data, was "skycatalogs-1.7.0rc3.tar", last modified: Fri May 10 20:47:49 2024, max compression
```

## Comparing `skyCatalogs-1.7.0rc2.tar` & `skycatalogs-1.7.0rc3.tar`

### file list

```diff
@@ -1,109 +1,112 @@
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-02-16 00:59:47.792254 skyCatalogs-1.7.0rc2/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1569 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/LICENSE
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       37 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/MANIFEST.in
--rw-r--r--   0 jrbogart (71218) jrbogart (71218)     3389 2024-02-16 00:59:47.791658 skyCatalogs-1.7.0rc2/PKG-INFO
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1082 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/README.md
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1245 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/pyproject.toml
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       38 2024-02-16 00:59:47.792327 skyCatalogs-1.7.0rc2/setup.cfg
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-02-16 00:59:47.739496 skyCatalogs-1.7.0rc2/skyCatalogs.egg-info/
--rw-r--r--   0 jrbogart (71218) jrbogart (71218)     3389 2024-02-16 00:59:47.737990 skyCatalogs-1.7.0rc2/skyCatalogs.egg-info/PKG-INFO
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     4349 2024-02-16 00:59:47.738450 skyCatalogs-1.7.0rc2/skyCatalogs.egg-info/SOURCES.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)        1 2024-02-16 00:59:47.738821 skyCatalogs-1.7.0rc2/skyCatalogs.egg-info/dependency_links.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       59 2024-02-16 00:59:47.739193 skyCatalogs-1.7.0rc2/skyCatalogs.egg-info/requires.txt
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       12 2024-02-16 00:59:47.739565 skyCatalogs-1.7.0rc2/skyCatalogs.egg-info/top_level.txt
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-02-16 00:59:47.741844 skyCatalogs-1.7.0rc2/skycatalogs/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      137 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       26 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/_version.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    45185 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/catalog_creator.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-02-16 00:59:47.735311 skyCatalogs-1.7.0rc2/skycatalogs/data/
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-02-16 00:59:47.759982 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      568 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/README
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      125 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/cosmodc2_bulge.yaml
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      124 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/cosmodc2_disk.yaml
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      448 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/cosmodc2_galaxy.yaml
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      122 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/cosmodc2_knots.yaml
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      402 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/dc2_star.yaml
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   345332 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9556.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   449782 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9557.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   356762 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9683.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   344612 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9684.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   350704 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9812.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   342882 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9813.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   348427 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9940.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    15585 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_flux_9556.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    15759 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_flux_9683.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    15445 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_flux_9684.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    16195 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_flux_9813.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    16053 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_flux_9940.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    25551 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_9556.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    25360 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_9683.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    25329 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_9684.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    25553 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_9812.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    25729 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_9813.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    25343 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_9940.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    21154 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_flux_9556.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    20998 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_flux_9683.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    21152 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_flux_9684.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    21176 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_flux_9813.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    21178 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_flux_9940.parquet
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-02-16 00:59:47.761133 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      756 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/butler.yaml
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   811008 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/gen3.sqlite3
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-02-16 00:59:47.734900 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-02-16 00:59:47.768474 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   161280 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131072_refcats.fits
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   144000 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131073_refcats.fits
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   155520 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131074_refcats.fits
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   146880 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131075_refcats.fits
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   155520 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131076_refcats.fits
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   158400 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131077_refcats.fits
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   155520 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131078_refcats.fits
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   152640 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131079_refcats.fits
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2731 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/skyCatalog.yaml
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1831 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/skyCatalog_top.yaml
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-02-16 00:59:47.769815 skyCatalogs-1.7.0rc2/skycatalogs/data/gaia_dr2/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   336105 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/gaia_dr2/GaiaDR2_RevisedPassbands.dat
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2500 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/gaia_dr2/gaia_dr2_temp_from_bp-rp_ratio.txt
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-02-16 00:59:47.778413 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   356354 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_9556.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   367622 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_9683.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   355504 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_9684.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   361737 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_9812.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   353853 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_9813.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)   359203 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_9940.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    18968 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_flux_9556.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    19132 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_flux_9683.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    18832 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_flux_9684.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    18958 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_flux_9812.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    19653 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_flux_9813.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    19415 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_flux_9940.parquet
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2732 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/skyCatalog.yaml
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    14476 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/diffsky_sedgen.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-02-16 00:59:47.782115 skyCatalogs-1.7.0rc2/skycatalogs/objects/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       54 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/objects/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    25277 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/objects/base_object.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     5778 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/objects/diffsky_object.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    10261 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/objects/gaia_object.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     6611 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/objects/galaxy_object.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     8078 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/objects/snana_object.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2321 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/objects/sncosmo_object.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1268 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/objects/star_object.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-02-16 00:59:47.783131 skyCatalogs-1.7.0rc2/skycatalogs/readers/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)       30 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/readers/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2390 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/readers/parquet_reader.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    42042 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/skyCatalogs.py
-drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-02-16 00:59:47.790783 skyCatalogs-1.7.0rc2/skycatalogs/utils/
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1083 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/SED_parquet.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      249 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/__init__.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2033 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/add_extinction.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1779 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/catalog_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2008 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/common_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     9330 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/config_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      864 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/creator_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)      744 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/exceptions.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     9150 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/parquet_schema_utils.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    10457 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/sed_tools.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     2524 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/shapes.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     1443 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/sn_tools.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)     3458 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/star_parquet_input.py
--rw-rw----   0 jrbogart (71218) jrbogart (71218)    11160 2024-02-16 00:48:52.000000 skyCatalogs-1.7.0rc2/skycatalogs/utils/translate_utils.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-05-10 20:47:49.603822 skycatalogs-1.7.0rc3/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1569 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/LICENSE
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       37 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/MANIFEST.in
+-rw-r--r--   0 jrbogart (71218) jrbogart (71218)     3359 2024-05-10 20:47:49.603278 skycatalogs-1.7.0rc3/PKG-INFO
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1082 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/README.md
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1224 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/pyproject.toml
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       38 2024-05-10 20:47:49.603884 skycatalogs-1.7.0rc3/setup.cfg
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-05-10 20:47:49.541783 skycatalogs-1.7.0rc3/skyCatalogs.egg-info/
+-rw-r--r--   0 jrbogart (71218) jrbogart (71218)     3359 2024-05-10 20:47:49.539970 skycatalogs-1.7.0rc3/skyCatalogs.egg-info/PKG-INFO
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     4466 2024-05-10 20:47:49.540429 skycatalogs-1.7.0rc3/skyCatalogs.egg-info/SOURCES.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)        1 2024-05-10 20:47:49.540907 skycatalogs-1.7.0rc3/skyCatalogs.egg-info/dependency_links.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       44 2024-05-10 20:47:49.541377 skycatalogs-1.7.0rc3/skyCatalogs.egg-info/requires.txt
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       12 2024-05-10 20:47:49.541838 skycatalogs-1.7.0rc3/skyCatalogs.egg-info/top_level.txt
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-05-10 20:47:49.544347 skycatalogs-1.7.0rc3/skycatalogs/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      137 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       26 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/_version.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    46242 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/catalog_creator.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-05-10 20:47:49.531083 skycatalogs-1.7.0rc3/skycatalogs/data/
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-05-10 20:47:49.563203 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      568 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/README
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      125 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/cosmodc2_bulge.yaml
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      124 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/cosmodc2_disk.yaml
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      448 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/cosmodc2_galaxy.yaml
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      122 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/cosmodc2_knots.yaml
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      402 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/dc2_star.yaml
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      745 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/gaia_skyCatalog.yaml
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   345332 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9556.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   449782 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9557.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   356762 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9683.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   344612 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9684.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   350704 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9812.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   342882 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9813.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   348427 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9940.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    15585 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_flux_9556.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    15759 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_flux_9683.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    15445 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_flux_9684.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    16195 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_flux_9813.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    16053 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_flux_9940.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    25551 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_9556.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    25360 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_9683.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    25329 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_9684.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    25553 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_9812.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    25729 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_9813.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    25343 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_9940.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    21154 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_flux_9556.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    20998 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_flux_9683.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    21152 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_flux_9684.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    21176 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_flux_9813.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    21178 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_flux_9940.parquet
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-05-10 20:47:49.564289 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      756 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/butler.yaml
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   811008 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/gen3.sqlite3
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-05-10 20:47:49.527549 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-05-10 20:47:49.571534 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   161280 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131072_refcats.fits
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   144000 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131073_refcats.fits
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   155520 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131074_refcats.fits
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   146880 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131075_refcats.fits
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   155520 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131076_refcats.fits
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   158400 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131077_refcats.fits
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   155520 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131078_refcats.fits
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   152640 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131079_refcats.fits
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2731 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/skyCatalog.yaml
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1831 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/skyCatalog_top.yaml
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-05-10 20:47:49.572865 skycatalogs-1.7.0rc3/skycatalogs/data/gaia_dr2/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   336105 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/gaia_dr2/GaiaDR2_RevisedPassbands.dat
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2500 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/gaia_dr2/gaia_dr2_temp_from_bp-rp_ratio.txt
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-05-10 20:47:49.586920 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   356354 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_9556.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   367622 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_9683.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   355504 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_9684.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   361737 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_9812.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   353853 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_9813.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)   359203 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_9940.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    18968 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_flux_9556.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    19132 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_flux_9683.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    18832 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_flux_9684.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    18958 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_flux_9812.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    19653 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_flux_9813.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    19415 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_flux_9940.parquet
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2732 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/skyCatalog.yaml
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    14476 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/diffsky_sedgen.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-05-10 20:47:49.591132 skycatalogs-1.7.0rc3/skycatalogs/objects/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       54 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/objects/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    25243 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/objects/base_object.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     5778 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/objects/diffsky_object.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    15604 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/objects/gaia_object.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     6611 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/objects/galaxy_object.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     8096 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/objects/snana_object.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2321 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/objects/sncosmo_object.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     6492 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/objects/sso_object.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1063 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/objects/star_object.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-05-10 20:47:49.592054 skycatalogs-1.7.0rc3/skycatalogs/readers/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)       30 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/readers/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2390 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/readers/parquet_reader.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    34210 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/skyCatalogs.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    10766 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/sso_catalog_creator.py
+drwxrwx---   0 jrbogart (71218) jrbogart (71218)        0 2024-05-10 20:47:49.602636 skycatalogs-1.7.0rc3/skycatalogs/utils/
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1083 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/SED_parquet.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      249 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/__init__.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2033 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/add_extinction.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1779 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/catalog_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     2008 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/common_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    11820 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/config_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      864 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/creator_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)      744 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/exceptions.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     9150 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/parquet_schema_utils.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    11547 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/sed_tools.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     4143 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/shapes.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     1443 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/sn_tools.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)     4676 2024-05-10 20:46:32.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/star_parquet_input.py
+-rw-rw----   0 jrbogart (71218) jrbogart (71218)    11160 2024-02-16 00:48:52.000000 skycatalogs-1.7.0rc3/skycatalogs/utils/translate_utils.py
```

### Comparing `skyCatalogs-1.7.0rc2/LICENSE` & `skycatalogs-1.7.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/PKG-INFO` & `skycatalogs-1.7.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyCatalogs
-Version: 1.7.0rc2
+Version: 1.7.0rc3
 Summary: Writes, reads catalogs input to LSST DESC simulations
 Author-email: Joanne Bogart <jrb@slac.stanford.edu>
 License: Copyright (c) 2018, the skyCatalogs contributors on GitHub, https://github.com/LSSTDESC/skyCatalogs/graphs/contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -38,15 +38,14 @@
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: healpy
 Requires-Dist: astropy
 Requires-Dist: pyarrow
 Requires-Dist: pandas
 Requires-Dist: sncosmo
-Requires-Dist: pyyaml-include
 
 # The skyCatalogs package
 
 This package will contain 
 * code to create sky catalogs from input like cosmoDC2 (for galaxies) and similar catalogs for other source types
 * implement an API to access information in the catalogs and products, such as flux calculations, derived from the catalogs
```

### Comparing `skyCatalogs-1.7.0rc2/README.md` & `skycatalogs-1.7.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/pyproject.toml` & `skycatalogs-1.7.0rc3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 dependencies = [
     'numpy',
     'healpy',
     'astropy',
     'pyarrow',
     'pandas',
     'sncosmo',
-    'pyyaml-include'
 ]
 requires-python = ">=3.7" # For setuptools >= 61.0 support
 
 [tool.setuptools.dynamic]
 version = {attr = ".skycatalogs._version.__version__"}
 
 [tool.setuptools]
```

### Comparing `skyCatalogs-1.7.0rc2/skyCatalogs.egg-info/PKG-INFO` & `skycatalogs-1.7.0rc3/skyCatalogs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skyCatalogs
-Version: 1.7.0rc2
+Version: 1.7.0rc3
 Summary: Writes, reads catalogs input to LSST DESC simulations
 Author-email: Joanne Bogart <jrb@slac.stanford.edu>
 License: Copyright (c) 2018, the skyCatalogs contributors on GitHub, https://github.com/LSSTDESC/skyCatalogs/graphs/contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -38,15 +38,14 @@
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: healpy
 Requires-Dist: astropy
 Requires-Dist: pyarrow
 Requires-Dist: pandas
 Requires-Dist: sncosmo
-Requires-Dist: pyyaml-include
 
 # The skyCatalogs package
 
 This package will contain 
 * code to create sky catalogs from input like cosmoDC2 (for galaxies) and similar catalogs for other source types
 * implement an API to access information in the catalogs and products, such as flux calculations, derived from the catalogs
```

### Comparing `skyCatalogs-1.7.0rc2/skyCatalogs.egg-info/SOURCES.txt` & `skycatalogs-1.7.0rc3/skyCatalogs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 skyCatalogs.egg-info/requires.txt
 skyCatalogs.egg-info/top_level.txt
 skycatalogs/__init__.py
 skycatalogs/_version.py
 skycatalogs/catalog_creator.py
 skycatalogs/diffsky_sedgen.py
 skycatalogs/skyCatalogs.py
+skycatalogs/sso_catalog_creator.py
 skycatalogs/data/ci_sample/README
 skycatalogs/data/ci_sample/cosmodc2_bulge.yaml
 skycatalogs/data/ci_sample/cosmodc2_disk.yaml
 skycatalogs/data/ci_sample/cosmodc2_galaxy.yaml
 skycatalogs/data/ci_sample/cosmodc2_knots.yaml
 skycatalogs/data/ci_sample/dc2_star.yaml
+skycatalogs/data/ci_sample/gaia_skyCatalog.yaml
 skycatalogs/data/ci_sample/galaxy_9556.parquet
 skycatalogs/data/ci_sample/galaxy_9557.parquet
 skycatalogs/data/ci_sample/galaxy_9683.parquet
 skycatalogs/data/ci_sample/galaxy_9684.parquet
 skycatalogs/data/ci_sample/galaxy_9812.parquet
 skycatalogs/data/ci_sample/galaxy_9813.parquet
 skycatalogs/data/ci_sample/galaxy_9940.parquet
@@ -71,14 +73,15 @@
 skycatalogs/objects/__init__.py
 skycatalogs/objects/base_object.py
 skycatalogs/objects/diffsky_object.py
 skycatalogs/objects/gaia_object.py
 skycatalogs/objects/galaxy_object.py
 skycatalogs/objects/snana_object.py
 skycatalogs/objects/sncosmo_object.py
+skycatalogs/objects/sso_object.py
 skycatalogs/objects/star_object.py
 skycatalogs/readers/__init__.py
 skycatalogs/readers/parquet_reader.py
 skycatalogs/utils/SED_parquet.py
 skycatalogs/utils/__init__.py
 skycatalogs/utils/add_extinction.py
 skycatalogs/utils/catalog_utils.py
```

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/catalog_creator.py` & `skycatalogs-1.7.0rc3/skycatalogs/catalog_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .utils.parquet_schema_utils import make_galaxy_schema
 from .utils.parquet_schema_utils import make_galaxy_flux_schema
 from .utils.parquet_schema_utils import make_star_flux_schema
 from .utils.parquet_schema_utils import make_pointsource_schema
 from .utils.creator_utils import make_MW_extinction_av, make_MW_extinction_rv
 from .objects.base_object import LSST_BANDS
 from .objects.base_object import ROMAN_BANDS
+from .sso_catalog_creator import SsoCatalogCreator
 
 """
 Code to create a sky catalog for particular object types
 """
 
 __all__ = ['CatalogCreator']
 
@@ -193,15 +194,16 @@
                  output_type='parquet', mag_cut=None,
                  sed_subdir='galaxyTopHatSED', knots_mag_cut=27.0,
                  knots=True, logname='skyCatalogs.creator',
                  pkg_root=None, skip_done=False, no_main=False,
                  no_flux=False, flux_parallel=16, galaxy_nside=32,
                  galaxy_stride=1000000, provenance=None,
                  dc2=False, sn_object_type='sncosmo', galaxy_type='cosmodc2',
-                 include_roman_flux=False, star_input_fmt='sqlite'):
+                 include_roman_flux=False, star_input_fmt='sqlite',
+                 sso_truth=None, sso_sed=None, sso_partition='healpixel'):
         """
         Store context for catalog creation
 
         Parameters
         ----------
         parts           Segments for which catalog is to be generated. If
                         partition type is HEALpix, parts will be a collection
@@ -240,25 +242,29 @@
         provenance      Whether to write per-output-file git repo provenance
         dc2             Whether to adjust values to provide input comparable
                         to that for the DC2 run
         sn_object_type  Which object type to use for SNe.
         galaxy_type     Currently allowed values are cosmodc2 and diffsky
         include_roman_flux Calculate and write Roman flux values
         star_input_fmt  May be either 'sqlite' or 'parquet'
+        sso_truth       Directory containing Sorcha output
+        sso_sed         Path to sed file to be used for all SSOs
+        sso_partition   Whether to partition by time or by healpixels
 
         Might want to add a way to specify template for output file name
         and template for input sedLookup file name.
         """
 
         _cosmo_cat = 'cosmodc2_v1.1.4_image_addon_knots'
         _diffsky_cat = 'roman_rubin_2023_v1.1.2_elais'
         _star_db = '/global/cfs/cdirs/lsst/groups/SSim/DC2/dc2_stellar_healpixel.db'
         _sn_db = '/global/cfs/cdirs/lsst/groups/SSim/DC2/cosmoDC2_v1.1.4/sne_cosmoDC2_v1.1.4_MS_DDF_healpix.db'
 
-        _star_parquet = '/global/cfs/cdirs/descssim/postDC2/UW_star_catalog'
+#        _star_parquet = '/global/cfs/cdirs/descssim/postDC2/UW_star_catalog'
+        _star_parquet = '/sdf/data/rubin/shared/ops-rehearsal-3/imSim_catalogs/UW_stars'
 
         self._galaxy_stride = galaxy_stride
         if pkg_root:
             self._pkg_root = pkg_root
         else:
             self._pkg_root = os.path.join(os.path.dirname(__file__),
                                           '..')
@@ -287,14 +293,15 @@
         self._star_truth = star_truth
         self._star_input_fmt = star_input_fmt
         if self._star_truth is None:
             if self._star_input_fmt == 'sqlite':
                 self._star_truth = _star_db
             elif self._star_input_fmt == 'parquet':
                 self._star_truth = _star_parquet
+
         self._cat = None
 
         self._parts = parts
         if skycatalog_root:
             self._skycatalog_root = skycatalog_root
         else:
             self._skycatalog_root = './'
@@ -322,14 +329,19 @@
         self._no_flux = no_flux
         self._flux_parallel = flux_parallel
         self._galaxy_nside = galaxy_nside
         self._provenance = provenance
         self._dc2 = dc2
         self._include_roman_flux = include_roman_flux
         self._obs_sed_factory = None
+        self._sso_sed_factory = None               # do we need this?
+        self._sso_creator = SsoCatalogCreator(self, sso_truth, sso_sed)
+        self._sso_truth = self._sso_creator.sso_truth
+        self._sso_sed = self._sso_creator.sso_sed
+        self._sso_partition = sso_partition
 
     def _make_tophat_columns(self, dat, names, cmp):
         '''
         Create columns sed_val_cmp, cmp_magnorm where cmp is one of "disk",
         "bulge", "knots"
 
         Parameters
@@ -353,30 +365,36 @@
 
     def create(self, catalog_type):
         """
         Create catalog of specified type, using stored context.
 
         Parameters
         ----------
-        catalog_type   string    Currently 'galaxy' and 'pointsource' are
-                                 the only values allowed
+        catalog_type   string    Currently 'galaxy', 'pointsource'
+                                 and 'sso' are the only values allowed
         Return
         ------
         None
         """
         if catalog_type == ('galaxy'):
             if not self._no_main:
                 self.create_galaxy_catalog()
             if not self._no_flux:
                 self.create_galaxy_flux_catalog()
         elif catalog_type == ('pointsource'):
             if not self._no_main:
                 self.create_pointsource_catalog()
             if not self._no_flux:
                 self.create_pointsource_flux_catalog()
+        elif catalog_type == ('sso'):
+            if not self._flux_only:
+                self._sso_creator.create_sso_catalog()
+            if not self._main_only:
+                self._sso_creator.create_sso_flux_catalog()
+
         else:
             raise NotImplementedError(f'CatalogCreator.create: unsupported catalog type {catalog_type}')
 
     def create_galaxy_catalog(self):
         """
         Create the 'main' galaxy catalog, including everything except
         LSST fluxes
@@ -1077,14 +1095,17 @@
         config.add_key('knots_magnitude_cut', self._knots_mag_cut)
 
         inputs = {'galaxy_truth': self._galaxy_truth}
         if self._sn_truth:
             inputs['sn_truth'] = self._sn_truth
         if self._star_truth:
             inputs['star_truth'] = self._star_truth
+        if self._sso_truth:
+            inputs['sso_truth'] = self._sso_truth
+            inputs['sso_sed'] = self._sso_sed
         config.add_key('provenance', assemble_provenance(self._pkg_root,
                                                          inputs=inputs))
 
         self._written_config = config.write_config(self._config_path,
                                                    overwrite=overwrite)
 
     def write_provenance_file(self, datafile_path):
```

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/README` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/README`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9556.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9556.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9557.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9557.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9683.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9683.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9684.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9684.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9812.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9812.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9813.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9813.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_9940.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_9940.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_flux_9556.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_flux_9556.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_flux_9683.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_flux_9683.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_flux_9684.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_flux_9684.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_flux_9813.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_flux_9813.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/galaxy_flux_9940.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/galaxy_flux_9940.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_9556.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_9556.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_9683.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_9683.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_9684.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_9684.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_9812.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_9812.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_9813.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_9813.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_9940.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_9940.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_flux_9556.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_flux_9556.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_flux_9683.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_flux_9683.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_flux_9684.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_flux_9684.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_flux_9813.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_flux_9813.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/pointsource_flux_9940.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/pointsource_flux_9940.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/butler.yaml` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/butler.yaml`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/gen3.sqlite3` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/gen3.sqlite3`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131072_refcats.fits` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131072_refcats.fits`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131073_refcats.fits` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131073_refcats.fits`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131074_refcats.fits` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131074_refcats.fits`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131075_refcats.fits` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131075_refcats.fits`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131076_refcats.fits` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131076_refcats.fits`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131077_refcats.fits` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131077_refcats.fits`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131078_refcats.fits` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131078_refcats.fits`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131079_refcats.fits` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/repo/refcats/gaia_dr2_20200414/gaia_dr2_20200414_131079_refcats.fits`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/skyCatalog.yaml` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/skyCatalog.yaml`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/ci_sample/skyCatalog_top.yaml` & `skycatalogs-1.7.0rc3/skycatalogs/data/ci_sample/skyCatalog_top.yaml`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/gaia_dr2/GaiaDR2_RevisedPassbands.dat` & `skycatalogs-1.7.0rc3/skycatalogs/data/gaia_dr2/GaiaDR2_RevisedPassbands.dat`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/gaia_dr2/gaia_dr2_temp_from_bp-rp_ratio.txt` & `skycatalogs-1.7.0rc3/skycatalogs/data/gaia_dr2/gaia_dr2_temp_from_bp-rp_ratio.txt`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_9556.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_9556.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_9683.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_9683.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_9684.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_9684.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_9812.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_9812.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_9813.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_9813.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_9940.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_9940.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_flux_9556.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_flux_9556.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_flux_9683.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_flux_9683.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_flux_9684.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_flux_9684.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_flux_9812.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_flux_9812.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_flux_9813.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_flux_9813.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/galaxy_flux_9940.parquet` & `skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/galaxy_flux_9940.parquet`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/data/row_groups/skyCatalog.yaml` & `skycatalogs-1.7.0rc3/skycatalogs/data/row_groups/skyCatalog.yaml`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/diffsky_sedgen.py` & `skycatalogs-1.7.0rc3/skycatalogs/diffsky_sedgen.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/objects/base_object.py` & `skycatalogs-1.7.0rc3/skycatalogs/objects/base_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 
     def _get_sed_from_file(self, fpath, redshift=0):
         sed = galsim.SED(fpath, wave_type='nm', flux_type='flambda')
         if redshift > 0:
             sed = sed.atRedshift(redshift)
         return sed
 
-    def get_gsobject_components(self, gsparams=None, rng=None):
+    def get_gsobject_components(self, gsparams=None, rng=None, exposure=None):
         """
         Return a dictionary of the GSObject components for the
         sky catalogs object, keyed by component name.
         Must be implemented by subclass
         """
         raise NotImplementedError('Subclass must implement get_gsobject_components')
 
@@ -566,15 +566,18 @@
             if isinstance(obj, BaseObject):
                 id = obj.id
             else:
                 raise TypeError
         return id in self._id
 
     def __len__(self):
-        return len(self._id)
+        if self._id is not None:
+            return len(self._id)
+        else:
+            return 0
 
     # def __iter__(self):   Standard impl based on __getitem__ should be ok
     # def __reversed__(self):   Default implementation ok
 
     def __getitem__(self, key):
         '''
         Parameters
@@ -593,25 +596,18 @@
         if isinstance(key, int) or isinstance(key, np.int64):
             return self._object_class(self._ra[key], self._dec[key],
                                       self._id[key], object_type, self, key)
 
         elif type(key) == slice:
             if key.start is None:
                 key.start = 0
-            ixdata = [i for i in range(min(key.stop, len(self._ra)))]
-            ixes = itertools.islice(ixdata, key.start, key.stop, key.step)
-            return [self._object_class(self._ra[i], self._dec[i], self._id[i],
-                                       object_type, self, i)
-                    for i in ixes]
+            return [self.__getitem__(i) for i in range(self.__len__())[key]]
 
         elif type(key) == tuple and isinstance(key[0], Iterable):
-            #  check it's a list of int-like?
-            return [self._object_class(self._ra[i], self._dec[i], self._id[i],
-                                       object_type, self, i)
-                    for i in key[0]]
+            return[self.__getitem__(i) for i in key[0]]
 
     def get_partition_id(self):
         return self._partition_id
 
     def count(self, obj):
         '''
         returns # of occurrences of obj.  It can only be 0 or 1
@@ -650,16 +646,22 @@
         # Elements of _located are named tuples:
         #   (collection, first_index, upper_bound)
         self._located = []
         self._total_len = 0
 
     def append_collection(self, coll):
         old = self._total_len
-        self._total_len += len(coll)
-        self._located.append(LocatedCollection(coll, old, self._total_len))
+        if isinstance(coll, ObjectCollection):
+            self._total_len += len(coll)
+            self._located.append(LocatedCollection(coll, old, self._total_len))
+        else:  #  list of collections
+            for c in coll:
+                self._total_len += len(c)
+                self._located.append(LocatedCollection(c, old, self._total_len))
+                old = self._total_len
 
     def append_object_list(self, object_list):
         for e in object_list._located:
             self.append_collection(e.collection)
 
     def get_native_attribute(self, attribute_name):
         '''
@@ -712,16 +714,16 @@
         '''
         Parameters
         ----------
         If key is an int return a single base object
         If key is a slice return a list of object
         '''
         one_only = isinstance(key, int) or isinstance(key, np.int64)
-        is_slice = type(key) == slice
-        is_list = type(key) == tuple and isinstance(key[0], Iterable)
+        is_slice = isinstance(key, slice)
+        is_list = isinstance(key, tuple) and isinstance(key[0], Iterable)
 
         if one_only:
             start = key
         elif is_slice:
             start = key.start
         elif is_list:
             start_ix = 0
```

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/objects/diffsky_object.py` & `skycatalogs-1.7.0rc3/skycatalogs/objects/diffsky_object.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/objects/gaia_object.py` & `skycatalogs-1.7.0rc3/skycatalogs/objects/gaia_object.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import os
 import warnings
 from functools import wraps
 import itertools
 from collections.abc import Iterable
 from pathlib import PurePath
 import numpy as np
+import numpy.ma as ma
+import pandas as pd
 import erfa
 import astropy.modeling
 from astropy import units as u
 import galsim
-import lsst.daf.butler as daf_butler
 import lsst.geom
+# ## Next two lines needed only for butler access
+import lsst.daf.butler as daf_butler
 from lsst.meas.algorithms import ReferenceObjectLoader
-from skycatalogs.utils.shapes import Disk, PolygonalRegion
+
+# ## Need these for direct access and processing of fits files
+import lsst.afw.table as afwtable
+from lsst.sphgeom import HtmPixelization, Circle, LonLat
+
+from skycatalogs.utils.shapes import Disk, PolygonalRegion, compute_region_mask
 from skycatalogs.objects.base_object import BaseObject, ObjectCollection
 
 
 __all__ = ['GaiaObject', 'GaiaCollection']
 
 
 def ignore_erfa_warnings(func):
@@ -63,25 +71,28 @@
 
     def __init__(self, obj_pars, parent_collection, index):
         """
         Parameters
         ----------
         obj_pars: dict-like
             Dictionary of object parameters as read directly from the
-            reference catalog.
+            complete object collection
         parent_collection: ObjectCollection
             Parent collection of this object.
         index: int
             Index of this object in the parent collection
         """
-        ra = np.degrees(obj_pars['coord_ra'])
-        dec = np.degrees(obj_pars['coord_dec'])
-        # Form the object id from the GAIA catalog id with the string
-        # 'gaia_dr2_' prepended.
-        obj_id = f"gaia_dr2_{obj_pars['id']}"
+        # ra = np.degrees(obj_pars['coord_ra'])
+        # dec = np.degrees(obj_pars['coord_dec'])
+        ra = obj_pars['ra_deg']
+        dec = obj_pars['dec_deg']
+        # Form the object id from the GAIA catalog id with a string
+        # like 'gaia_dr2_' prepended.
+        id_prefix = GaiaCollection._id_prefix
+        obj_id = f"{id_prefix}{obj_pars['id']}"
         super().__init__(ra, dec, obj_id, 'gaia_star',
                          belongs_to=parent_collection, belongs_index=index)
         self.use_lut = self._belongs_to._use_lut
         bp_flux = obj_pars['phot_bp_mean_flux']
         rp_flux = obj_pars['phot_rp_mean_flux']
         if rp_flux == 0.0 or bp_flux == 0.0:
             self.stellar_temp = None
@@ -122,22 +133,113 @@
             gsparams = galsim.GSParams(**gsparams)
         return {'this_object': galsim.DeltaFunction(gsparams=gsparams)}
 
     def set_use_lut(self, use_lut):
         self.use_lut = use_lut
 
 
+def _read_fits(htm_id, gaia_config, sky_root, out_dict, logger, region=None):
+    '''
+    Read data for columns in keys from fits file belonging to htm_id.
+    Append to arrays in out_dict.  If region is not None, filter out
+    entries not in region before appending.
+    Note ra, dec must be in degrees for filtering, but
+    coord_ra and coord_dec as stored in out_dict are in radians.
+
+    Parameters
+    ----------
+    htm_id         int
+    gaia_config    dict     gaia_star portion of skyCatalg config
+    sky_root       string   absolute skycatalog_root path.  Data
+                            is found relative to this
+    out_dict       dict     out_dict.keys() are the columns to store
+    region         lsst.sphgeom.Region or None
+    '''
+    f_dir = gaia_config['data_dir']
+    f_name = gaia_config['basename_template'].replace('(?P<htm>\\d+)',
+                                                      f'{htm_id}')
+    f_path = os.path.join(sky_root, f_dir, f_name)
+    if not os.path.isfile(f_path):
+        logger.info(f'No file for requested htm id {htm_id}')
+        return
+
+    tbl = afwtable.SimpleCatalog.readFits(f_path)
+    if region is None:
+        for k in out_dict.keys():
+            out_dict[k] += list(tbl.get(k))
+        return
+
+    # Otherwise start with ra, dec and create mask
+    ra_full = tbl.get('coord_ra')
+    dec_full = tbl.get('coord_dec')
+
+    ra_full_deg = np.degrees(ra_full)
+    dec_full_deg = np.degrees(dec_full)
+
+    if isinstance(region, Disk):
+        mask = compute_region_mask(region, ra_full_deg, dec_full_deg)
+        if all(mask):
+            return
+
+    elif isinstance(region, PolygonalRegion):
+        # First mask off points outside a bounding circle because it's
+        # relatively fast
+        circle = region._convex_polygon.getBoundingCircle()
+        v = circle.getCenter()
+        ra_c = LonLat.longitudeOf(v).asDegrees()
+        dec_c = LonLat.latitudeOf(v).asDegrees()
+        rad_as = circle.getOpeningAngle().asDegrees() * 3600
+        disk = Disk(ra_c, dec_c, rad_as)
+        mask = compute_region_mask(disk, ra_full_deg, dec_full_deg)
+        if all(mask):
+            return
+        if any(mask):
+            ra_compress = ma.array(ra_full, mask=mask).compressed()
+            dec_compress = ma.array(dec_full, mask=mask).compressed()
+        else:
+            ra_compress = ra_full
+            dec_compress = dec_full
+        poly_mask = compute_region_mask(region, np.degrees(ra_compress),
+                                        np.degrees(dec_compress))
+        if all(poly_mask):
+            return
+
+        # Get indices of unmasked
+        ixes = np.where(~mask)
+
+        mask[ixes] |= poly_mask
+
+    if any(mask):
+        ra_compress = ma.array(ra_full, mask=mask).compressed()
+        dec_compress = ma.array(dec_full, mask=mask).compressed()
+    else:
+        ra_compress = ra_full
+        dec_compress = dec_full
+
+    out_dict['coord_ra'] += list(ra_compress)
+    out_dict['coord_dec'] += list(dec_compress)
+
+    for k in out_dict.keys():
+        if k in ('coord_ra', 'coord_dec'):
+            continue
+        full = tbl.get(k)
+        if any(mask):
+            out_dict[k] += list(ma.array(full, mask=mask).compressed())
+        else:
+            out_dict[k] += list(full)
+
+
 class GaiaCollection(ObjectCollection):
     # Class methods
     _gaia_config = None
 
     @classmethod
     def set_config(cls, config):
         GaiaCollection._gaia_config = config
-
+        GaiaCollection._id_prefix = config['id_prefix']
     @classmethod
     def get_config(cls):
         return GaiaCollection._gaia_config
 
     @ignore_erfa_warnings
     @staticmethod
     def load_collection(region, skycatalog, mjd=None):
@@ -145,50 +247,75 @@
         region      One of Disk, PolygonalRegion from skyCatalogs.utils.shapes.
                     Box is not currently supported
         skycatalog  An instance of the SkyCatalog class
         mjd         Time at which objects are to be assembled. Ignored for
                     Gaia stars
         '''
         if not skycatalog:
-            raise ValueError(f'GaiaCollection.load_collection: skycatalog cannot be None')
+            raise ValueError('GaiaCollection.load_collection: skycatalog cannot be None')
         if isinstance(region, Disk):
             ra = lsst.geom.Angle(region.ra, lsst.geom.degrees)
             dec = lsst.geom.Angle(region.dec, lsst.geom.degrees)
             center = lsst.geom.SpherePoint(ra, dec)
             radius = lsst.geom.Angle(region.radius_as, lsst.geom.arcseconds)
-            refcat_region = lsst.sphgeom.Circle(center.getVector(), radius)
+            refcat_region = Circle(center.getVector(), radius)
         elif isinstance(region, PolygonalRegion):
             refcat_region = region._convex_polygon
         else:
             raise TypeError(f'GaiaCollection.load_collection: {region} not supported')
-
-        source_type = 'gaia_star'
-
         if GaiaCollection.get_config() is None:
             gaia_section = skycatalog.raw_config['object_types']['gaia_star']
             GaiaCollection.set_config(gaia_section)
+        gaia_section = GaiaCollection.get_config()
 
-        butler_params = GaiaCollection.get_config()['butler_parameters']
-        butler = daf_butler.Butler(butler_params['repo'],
-                                   collections=butler_params['collections'])
-        refs = set(butler.registry.queryDatasets(butler_params['dstype']))
-        refCats = [daf_butler.DeferredDatasetHandle(butler, _, {})
-                   for _ in refs]
-        dataIds = [butler.registry.expandDataId(_.dataId) for _ in refs]
-        config = ReferenceObjectLoader.ConfigClass()
-        config.filterMap = {f'{_}': f'phot_{_}_mean' for _ in ('g', 'bp', 'rp')}
-        ref_obj_loader = ReferenceObjectLoader(dataIds=dataIds,
-                                               refCats=refCats,
-                                               config=config)
-
+        source_type = 'gaia_star'
         sed_method = GaiaCollection.get_config().get('sed_method', 'use_lut')
         use_lut = (sed_method.strip().lower() == 'use_lut')
-        band = 'bp'
-        cat = ref_obj_loader.loadRegion(refcat_region, band).refCat
-        df = cat.asAstropy().to_pandas().sort_values('id')
+        if gaia_section['data_file_type'] == 'butler_refcat':
+
+            butler_params = gaia_section['butler_parameters']
+            butler = daf_butler.Butler(butler_params['repo'],
+                                       collections=butler_params['collections'])
+            refs = set(butler.registry.queryDatasets(butler_params['dstype']))
+            refCats = [daf_butler.DeferredDatasetHandle(butler, _, {})
+                       for _ in refs]
+            dataIds = [butler.registry.expandDataId(_.dataId) for _ in refs]
+            config = ReferenceObjectLoader.ConfigClass()
+            config.filterMap = {f'{_}': f'phot_{_}_mean' for _ in ('g', 'bp', 'rp')}
+            ref_obj_loader = ReferenceObjectLoader(dataIds=dataIds,
+                                                   refCats=refCats,
+                                                   config=config)
+
+            band = 'bp'
+            cat = ref_obj_loader.loadRegion(refcat_region, band).refCat
+            df = cat.asAstropy().to_pandas().sort_values('id')
+
+        else:    # access fits files directly
+            # find htms intersecting region
+            level = gaia_section['area_partition']['level']
+            htm_pix = HtmPixelization(level)
+
+            overlap_ranges = htm_pix.envelope(refcat_region)
+            interior_ranges = htm_pix.interior(refcat_region)
+            partial_ranges = overlap_ranges - interior_ranges
+            keys = ['id', 'coord_ra', 'coord_dec', 'parallax', 'pm_ra',
+                    'pm_dec', 'epoch']
+            keys += [f'phot_{_}_mean_flux' for _ in ('g', 'bp', 'rp')]
+            out_dict = {k: [] for k in keys}
+
+            config = GaiaCollection.get_config()
+            for i_r in interior_ranges:
+                for i_htm in i_r:
+                    _read_fits(i_htm, config, skycatalog._sky_root, out_dict,
+                               skycatalog._logger, region=None)
+            for p_r in partial_ranges:
+                for i_htm in p_r:
+                    _read_fits(i_htm, config, skycatalog._sky_root,
+                               out_dict, skycatalog._logger, region=region)
+            df = pd.DataFrame(out_dict).sort_values('id')
 
         if mjd is None:
             raise RuntimeError("MJD needs to be provided for Gaia "
                                "proper motion calculations.")
         # The erfa.pmsafe code
         # (https://pyerfa.readthedocs.io/en/latest/api/erfa.pmsafe.html)
         # expects ra, dec in units of radians and pm_ra, pm_dec
@@ -199,28 +326,34 @@
         arcsec_per_radian = (1.0*u.radian).to(u.arcsec).value
         df['parallax'] *= arcsec_per_radian
         # radial velocity is missing from the Gaia DR2 refcats, so pass
         # an array of zeros.
         rv1 = np.zeros(len(df))
         epNa = 2400000.5  # "part A" of starting and ending epochs for MJDs.
         ep2b = mjd
-        pm_outputs = erfa.pmsafe(df['coord_ra'], df['coord_dec'],
-                                 df['pm_ra'], df['pm_dec'], df['parallax'],
-                                 rv1, epNa, df['epoch'], epNa, ep2b)
+        pm_outputs = erfa.pmsafe(np.array(df['coord_ra']),
+                                 np.array(df['coord_dec']),
+                                 np.array(df['pm_ra']), np.array(df['pm_dec']),
+                                 np.array(df['parallax']),
+                                 rv1, epNa, np.array(df['epoch']), epNa, ep2b)
         # Update ra, dec values.
         df['coord_ra'] = pm_outputs[0]
         df['coord_dec'] = pm_outputs[1]
 
+        # and also store degrees version
+        # is there any reason to keep coord_ra & coord_dec?
+        df['ra_deg'] = np.degrees(pm_outputs[0])
+        df['dec_deg'] = np.degrees(pm_outputs[1])
+
         return GaiaCollection(df, skycatalog, source_type, use_lut, mjd)
 
     def __init__(self, df, sky_catalog, source_type, use_lut, mjd):
         self.df = df
         self._sky_catalog = sky_catalog
         self._partition_id = None
-        self._id = np.array([f"gaia_dr2_{df.iloc[key]['id']}" for key in range(len(df))])
         self._mask = None
         self._object_type_unique = source_type
         self._use_lut = use_lut
         self._rdrs = []
         self._object_class = GaiaObject
         self._use_lut = use_lut
         self._mjd = mjd
@@ -234,22 +367,24 @@
         return self._use_lut
 
     @property
     def mjd(self):
         return self._mjd
 
     def __getitem__(self, key):
+        cols = ('id', 'ra_deg', 'dec_deg', 'phot_bp_mean_flux',
+                'phot_rp_mean_flux')
         if isinstance(key, int) or isinstance(key, np.int64):
-            return GaiaObject(self.df.iloc[key], self, key)
+            row = {col: self.df[col][key] for col in cols}
+            return GaiaObject(row, self, key)
 
-        elif type(key) == slice:
-            ixdata = [i for i in range(min(key.stop, len(self._id)))]
-            ixes = itertools.islice(ixdata, key.start, key.stop, key.step)
-            return [self._object_class(self.df.iloc[i], self, i) for i in ixes]
+        elif isinstance(key, slice):
+            # ixdata = [i for i in range(min(key.stop, len(self.df['id'])))]
+            # ixes = itertools.islice(ixdata, key.start, key.stop, key.step)
+            # return [self.__getitem__(i) for i in ixes]
+            return [self.__getitem__(i) for i in range(len(self.df))[key]]
 
         elif type(key) == tuple and isinstance(key[0], Iterable):
-            #  check it's a list of int-like?
-            return [self._object_class(self.df.iloc[i], self,
-                                       i) for i in key[0]]
+            return [self.__getitem__(i) for i in key[0]]
 
     def __len__(self):
         return len(self.df)
```

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/objects/galaxy_object.py` & `skycatalogs-1.7.0rc3/skycatalogs/objects/galaxy_object.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/objects/snana_object.py` & `skycatalogs-1.7.0rc3/skycatalogs/objects/snana_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             gsparams = galsim.GSParams(**gsparams)
         return {'this_object': galsim.DeltaFunction(gsparams=gsparams)}
 
     def get_observer_sed_component(self, component, mjd=None):
         if mjd is None:
             mjd = self._belongs_to._mjd
         if mjd is None:
-            txt = 'SnananObject._get_sed: no mjd specified for this call\n'
+            txt = 'SnananObject.get_observer_sed_component: no mjd specified for this call\n'
             txt += 'nor when generating object list'
             raise ValueError(txt)
         sed, _ = self._get_sed(mjd=mjd)
         if sed is not None:
             sed = self._apply_component_extinction(sed)
         return sed
```

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/objects/sncosmo_object.py` & `skycatalogs-1.7.0rc3/skycatalogs/objects/sncosmo_object.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/readers/parquet_reader.py` & `skycatalogs-1.7.0rc3/skycatalogs/readers/parquet_reader.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/skyCatalogs.py` & `skycatalogs-1.7.0rc3/skycatalogs/skyCatalogs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import os
-import sys
 import re
-import yaml
-from yamlinclude import YamlIncludeConstructor
 import logging
 import healpy
 import numpy as np
 import numpy.ma as ma
 from astropy import units as u
 import lsst.sphgeom
 from skycatalogs.objects.base_object import load_lsst_bandpasses, load_roman_bandpasses
 from skycatalogs.utils.catalog_utils import CatalogContext
-from skycatalogs.objects.base_object import ObjectList
+from skycatalogs.objects.base_object import ObjectList, ObjectCollection
 from skycatalogs.objects.gaia_object import GaiaObject, GaiaCollection
+from skycatalogs.objects.sso_object import SsoObject, SsoCollection
+from skycatalogs.objects.sso_object import EXPOSURE_DEFAULT
+# from skycatalogs.objects.sso_object import find_sso_files
 from skycatalogs.readers import ParquetReader
 from skycatalogs.utils.sed_tools import TophatSedFactory, DiffskySedFactory
+from skycatalogs.utils.sed_tools import SsoSedFactory
 from skycatalogs.utils.sed_tools import MilkyWayExtinction
 from skycatalogs.utils.config_utils import Config
 from skycatalogs.utils.shapes import Box, Disk, PolygonalRegion
+from skycatalogs.utils.shapes import compute_region_mask
 from skycatalogs.objects.sncosmo_object import SncosmoObject, SncosmoCollection
 from skycatalogs.objects.star_object import StarObject
 from skycatalogs.objects.galaxy_object import GalaxyObject
 from skycatalogs.objects.diffsky_object import DiffskyObject
 from skycatalogs.objects.snana_object import SnanaObject, SnanaCollection
 
 __all__ = ['SkyCatalog', 'open_catalog']
@@ -64,48 +66,49 @@
 
     # ensure pixels are always presented in the same order
     pixels = list(pixels)
     pixels.sort()
     return pixels
 
 
-def _compress_via_mask(tbl, id_column, region, source_type={'galaxy'},
-                       mjd=None):
+def _compress_via_mask(tbl, id_column, region, source_type='galaxy',
+                       mjd=None, exposure=EXPOSURE_DEFAULT):
     '''
     Parameters
     ----------
     tbl          data table including columns named "ra", "dec", and id_column
-                 (and also "object_type" colum if galaxy is False, possibly
+                 (and also "object_type" colum if source_type is "star"
+                 or "Gaia_star", possibly
                  start_mjd and end_mjd if galaxy is False and mjd is not
                  None)
     id_column    string
     region       mask should restrict to this region (or not at all if None)
-    source_type  string or set (or other container) of expected object type(s).
-                 For now, must be a singleton
-    mjd          if not none, may be used to filter transient objects
+    source_type  string of expected object type
+    mjd          if not none, may be used to filter transient or variable
+                 objects
+    exposure     length of exposure if mjd is not None
 
     Returns
     -------
     4 values for galaxies and snana: ra, dec, id, mask
     5 values for pointsources: ra, dec, id, object_type, mask
+    5 values for SSO: ra, dec, id, mjd, mask
     If objects are in the region, ra, dec, id correspond to those objects.
     mask will mask off unused objects
     If there are no objects in the region, all return values are None
 
     '''
     if isinstance(tbl[id_column][0], (int, np.int64)):
         tbl[id_column] = [str(an_id) for an_id in tbl[id_column]]
 
-    if not isinstance(source_type, str):
-        source_type = set(source_type)
-        if len(source_type) != 1:
-            raise NotImplementedError('_compress_via_mask only accepts singleton object_type')
-        source_type = source_type.pop()
-    no_obj_type_return = (source_type in {'galaxy', 'diffsky_galaxy', 'snana'})
-    time_filter = ('start_mjd' in tbl) and ('end_mjd' in tbl) and mjd is not None
+    no_obj_type_return = (source_type in {'galaxy', 'diffsky_galaxy',
+                                          'snana', 'sso'})
+    no_mjd_return = (source_type != 'sso')   # for now
+    transient_filter = ('start_mjd' in tbl) and ('end_mjd' in tbl) and mjd is not None
+    variable_filter = ('mjd' in tbl)
 
     if region is not None:
         if isinstance(region, PolygonalRegion):
             # Using native PolygonalRegion selection is slow, so
             # pre-mask the RA, Dec values using an acceptance
             # cone that encloses all of the vertices.
 
@@ -122,129 +125,138 @@
 
             # Construct a "Disk" enclosing the polygonal region.
             lon_lat = lsst.sphgeom.LonLat(mean_dir)
             ra = lon_lat.getLon().asDegrees()
             dec = lon_lat.getLat().asDegrees()
             disk_region = Disk(ra, dec, max_offset)
 
-            mask = _compute_region_mask(disk_region, tbl['ra'], tbl['dec'])
+            mask = compute_region_mask(disk_region, tbl['ra'], tbl['dec'])
             if all(mask):
-                if no_obj_type_return:
+                if no_obj_type_return and no_mjd_return:
                     return None, None, None, None
-                else:
+                else:    # currently if object type is returned, mjd is not
                     return None, None, None, None, None
 
             # Get compressed ra, dec
             ra_compress = ma.array(tbl['ra'], mask=mask).compressed()
             dec_compress = ma.array(tbl['dec'], mask=mask).compressed()
-            poly_mask = _compute_region_mask(region, ra_compress, dec_compress)
+            poly_mask = compute_region_mask(region, ra_compress, dec_compress)
 
             # Get indices of unmasked
             ixes = np.where(~mask)
 
             # Update bounding box mask with polygonal mask
             mask[ixes] |= poly_mask
         else:
-            mask = _compute_region_mask(region, tbl['ra'], tbl['dec'])
+            mask = compute_region_mask(region, tbl['ra'], tbl['dec'])
 
-        if time_filter:
-            time_mask = _compute_time_mask(mjd, tbl['start_mjd'],
-                                           tbl['end_mjd'])
+        if transient_filter:
+            time_mask = _compute_transient_mask(mjd, tbl['start_mjd'],
+                                                tbl['end_mjd'])
+            mask = np.logical_or(mask, time_mask)
+        elif variable_filter:
+            time_mask = _compute_variable_mask(mjd, tbl['mjd'], exposure)
             mask = np.logical_or(mask, time_mask)
 
         if all(mask):
-            if no_obj_type_return:
+            if no_obj_type_return and no_mjd_return:
                 return None, None, None, None
             else:
                 return None, None, None, None, None
         else:
             ra_compress = ma.array(tbl['ra'], mask=mask).compressed()
             dec_compress = ma.array(tbl['dec'], mask=mask).compressed()
             id_compress = ma.array(tbl[id_column], mask=mask).compressed()
             if no_obj_type_return:
-                return ra_compress, dec_compress, id_compress, mask
+                if no_mjd_return:
+                    return ra_compress, dec_compress, id_compress, mask
+                else:
+                    mjd_compress = ma.array(tbl['mjd'], mask=mask).compressed()
+                    return ra_compress, dec_compress, id_compress, mjd_compress, mask
             else:
 
                 object_type_compress = ma.array(tbl['object_type'],
                                                 mask=mask).compressed()
                 return ra_compress, dec_compress, id_compress, object_type_compress, mask
     else:
         if no_obj_type_return:
-            if time_filter:
-                time_mask = _compute_time_mask(mjd, tbl['start_mjd'],
-                                               tbl['end_mjd'])
+            if transient_filter:
+                time_mask = _compute_transient_mask(mjd, tbl['start_mjd'],
+                                                    tbl['end_mjd'])
                 ra_compress = ma.array(tbl['ra'], mask=time_mask).compressed()
                 dec_compress = ma.array(tbl['dec'],
                                         mask=time_mask).compressed()
                 id_compress = ma.array(tbl[id_column],
                                        mask=time_mask).compressed()
                 return ra_compress, dec_compress, id_compress, time_mask
+            elif variable_filter:
+                time_mask = _compute_variable_mask(mjd, tbl['mjd'], exposure)
+                if time_mask is not None:
+                    ra_compress = ma.array(tbl['ra'], mask=time_mask).compressed()
+                    dec_compress = ma.array(tbl['dec'],
+                                            mask=time_mask).compressed()
+                    id_compress = ma.array(tbl[id_column],
+                                           mask=time_mask).compressed()
+                    mjd_compress = ma.array(tbl['mjd'], mask=time_mask).compressed()
+                    return ra_compress, dec_compress, id_compress, mjd_compress, time_mask
+                else:
+                    return tbl['ra'], tbl['dec'], tbl[id_column], tbl['mjd'], None
             else:
                 return tbl['ra'], tbl['dec'], tbl[id_column], None
         else:
             return tbl['ra'], tbl['dec'], tbl[id_column], tbl['object_type'], None
 
 
-def _compute_region_mask(region, ra, dec):
+def _compute_transient_mask(current_mjd, start_mjd, end_mjd):
     '''
-    Compute mask according to region for provided data
+    Starting with an existing mask of excluded objects, exclude additional
+    objects not visible at time current_mjd
     Parameters
     ----------
-    region         Supported shape (box, disk)  or None
-    ra,dec         Coordinates for data to be masked, in degrees
+    current_mjd    Float  Time for which mask will be computed
+    start_mjd      Array of float. Bound on when object starts being
+                   detectable
+    end_mjd        Array of float. Bound on when object ceases being
+                   visible
     Returns
     -------
-    mask of elements in ra, dec arrays to be omitted
-
+    mask of objects detectable at specified time
     '''
-    mask = None
-    if isinstance(region, Box):
-        mask = np.logical_or((ra < region.ra_min),
-                             (ra > region.ra_max))
-        mask = np.logical_or(mask, (dec < region.dec_min))
-        mask = np.logical_or(mask, (dec > region.dec_max))
-    if isinstance(region, Disk):
-        # Change positions to 3d vectors to measure distance
-        p_vec = healpy.pixelfunc.ang2vec(ra, dec, lonlat=True)
-
-        c_vec = healpy.pixelfunc.ang2vec(region.ra,
-                                         region.dec,
-                                         lonlat=True)
-        radius_rad = (region.radius_as * u.arcsec).to_value('radian')
+    mask = np.logical_or((current_mjd > end_mjd), (current_mjd < start_mjd))
 
-        # Rather than comparing arcs, it is equivalent to compare chords
-        # (or square of chord length)
-        obj_chord_sq = np.sum(np.square(p_vec - c_vec), axis=1)
-
-        # This is to be compared to square of chord for angle a corresponding
-        # to disk radius.  That's 4(sin(a/2)^2)
-        rad_chord_sq = 4 * np.square(np.sin(0.5 * radius_rad))
-        mask = obj_chord_sq > rad_chord_sq
-    if isinstance(region, PolygonalRegion):
-        mask = region.get_containment_mask(ra, dec, included=False)
     return mask
 
 
-def _compute_time_mask(current_mjd, start_mjd, end_mjd):
+SECONDS_PER_DAY = 24.0*3600.0
+MJD_EPS = 0.1/SECONDS_PER_DAY
+JD_SEC = 1.0/SECONDS_PER_DAY
+
+
+def _compute_variable_mask(current_mjd, mjd_column, exposure, epsilon=MJD_EPS):
     '''
-    Starting with an existing mask of excluded objects, exclude additional
-    objects not visible at time current_mjd
+    Compute mask to exclude all entries with
+    mjd_column  > current_mjd - epsilon and mjd < current_mjd + exposure
+
     Parameters
     ----------
-    current_mjd    Float  Time for which mask will be computed
-    start_mjd      Array of float. Bound on when object starts being
-                   detectable
-    end_mjd        Array of float. Bound on when object ceases being
-                   visible
+    current_mjd  float            mjd of interest
+    mjd_column   array of float   mjd for each entry
+    exposure     float            exposure in seconds
+    epsilon      float            tolerance for matching mjd entry
+
     Returns
     -------
-    mask of objects detectable at specified time
+    mask
     '''
-    mask = np.logical_or((current_mjd > end_mjd), (current_mjd < start_mjd))
+    if not current_mjd:
+        return None
 
+    exposure_jd = exposure * JD_SEC
+    mask = np.logical_or(mjd_column < (current_mjd - epsilon),
+                         mjd_column > (current_mjd + exposure_jd))
     return mask
 
 
 class SkyCatalog(object):
     '''
     A base class with derived classes for galaxies, static (w.r.t. coordinates)
     point sources, SSOs
@@ -285,14 +297,16 @@
             else:
                 sky_root_env = os.getenv('SKYCATALOG_ROOT', None)
                 if sky_root_env:
                     sky_root = sky_root_env
 
             self._cat_dir = os.path.join(sky_root, config['catalog_dir'])
 
+        self._sky_root = os.path.abspath(sky_root)
+
         self._logger.info(f'Catalog data will be read from {self._cat_dir}')
         # There may be more to do at this point but not too much.
         # In particular, don't read in anything from data files
 
         self.verbose = verbose
         self._validate_config()
 
@@ -313,15 +327,19 @@
                 TophatSedFactory(th_parameters, config['Cosmology'])
         elif 'diffsky_galaxy' in config['object_types']:
             self._observed_sed_factory =\
                 DiffskySedFactory(self._cat_dir,
                                   config['object_types']['diffsky_galaxy']
                                   ['sed_file_template'],
                                   config['Cosmology'])
+        if 'sso' in config['object_types']:
+            self._sso_sed_path = config['provenance']['inputs'].get('sso_sed',
+                                                                    'sso_sed.db')
 
+            self._sso_sed_factory = SsoSedFactory(self._sso_sed_path)
         self._extinguisher = MilkyWayExtinction()
 
         # Make our properties accessible to BaseObject, etc.
         self.cat_cxt = CatalogContext(self)
 
         # register object types which are in the config
         if 'gaia_star' in config['object_types']:
@@ -343,14 +361,18 @@
         if 'snana' in config['object_types']:
             self.cat_cxt.register_source_type('snana',
                                               object_class=SnanaObject,
                                               collection_class=SnanaCollection)
         if 'diffsky_galaxy' in config['object_types']:
             self.cat_cxt.register_source_type('diffsky_galaxy',
                                               object_class=DiffskyObject)
+        if 'sso' in config['object_types']:
+            self.cat_cxt.register_source_type('sso',
+                                              object_class=SsoObject,
+                                              collection_class=SsoCollection)
 
     @property
     def observed_sed_factory(self):
         return self._observed_sed_factory
 
     @property
     def extinguisher(self):
@@ -404,31 +426,32 @@
         hp_set = set()
         for f in files:
             if rel_dir == '':
                 fpath = f
             else:
                 fpath = os.path.join(rel_dir, f)
             for k in tmpl_keys:
-                m = re.fullmatch(k, f)
-                if m:
-                    hp = int(m['healpix'])
-                    hp_set.add(hp)
-
-                    if hp not in self._hp_info:
-                        self._hp_info[hp] = {'files': {fpath: None},
-                                             'object_types': {name: [fpath]}}
-                    else:
-                        this_hp = self._hp_info[hp]
-                        # Value of 'object_types' is now a list
-                        if fpath not in this_hp['files']:
-                            this_hp['files'][fpath] = None
-                        if name in this_hp['object_types']:
-                            this_hp['object_types'][name].append(fpath)
+                if k.find('?P<healpix>') != -1:
+                    m = re.fullmatch(k, f)
+                    if m:
+                        hp = int(m['healpix'])
+                        hp_set.add(hp)
+
+                        if hp not in self._hp_info:
+                            self._hp_info[hp] = {'files': {fpath: None},
+                                                 'object_types': {name: [fpath]}}
                         else:
-                            this_hp['object_types'][name] = [fpath]
+                            this_hp = self._hp_info[hp]
+                            # Value of 'object_types' is now a list
+                            if fpath not in this_hp['files']:
+                                this_hp['files'][fpath] = None
+                            if name in this_hp['object_types']:
+                                this_hp['object_types'][name].append(fpath)
+                            else:
+                                this_hp['object_types'][name] = [fpath]
         return hp_set
 
     def _find_all_hps(self):
         '''
         For each healpix with files matching pattern in or under the
         directory containing the config file, update _hp_info as needed to keep
         track of all files for that healpix and the object types included in
@@ -526,23 +549,25 @@
         for obj in object_types:
             parent = self._config.get_object_parent(obj)
             if parent is not None:
                 objs_copy.remove(obj)
                 objs_copy.add(parent)
         return objs_copy
 
-    def get_objects_by_region(self, region, obj_type_set=None, mjd=None):
+    def get_objects_by_region(self, region, obj_type_set=None, mjd=None,
+                              exposure=EXPOSURE_DEFAULT):
         '''
         Parameters
         ----------
         region         region is a named tuple(may be box or circle)
                        or object of type PolygonalRegion
         obj_type_set   Return only these objects. Defaults to value in config if
                        specified; else default to all defined in config
         mjd            MJD of observation epoch.
+        exposure       exposure length (seconds)
 
         Returns
         -------
         ObjectList containing sky objects visible in the region
         [at the specified time]
         '''
         # Take intersection of obj_type_list and available object types
@@ -560,91 +585,104 @@
         obj_types = self.toplevel_only(obj_types)
 
         # Ensure they're always ordered the same way
         obj_types = list(obj_types)
         obj_types.sort()
 
         for ot in obj_types:
-            new_list = self.get_object_type_by_region(region, ot, mjd=mjd)
+            new_list = self.get_object_type_by_region(region, ot, mjd=mjd,
+                                                      exposure=exposure)
             object_list.append_object_list(new_list)
 
         return object_list
 
-    def get_object_type_by_region(self, region, object_type, mjd=None):
+    def get_object_type_by_region(self, region, object_type, mjd=None,
+                                  exposure=EXPOSURE_DEFAULT):
         '''
         Parameters
         ----------
         region        box, circle or PolygonalRegion. Supported region
                       types made depend on object_type
         object_type   known object type without parent
         mjd           MJD of observation epoch.
+        exposure      exposure (seconds)
+
+        Returns
+        -------
+        an ObjectList containing all objects found.
 
-        Returns all objects found
         '''
 
         out_list = ObjectList()
         if self._global_partition is not None:
             partition = self._global_partition
         else:
             partition = self._config['object_types'][object_type]['area_partition']
 
         coll_type = self.cat_cxt.lookup_collection_type(object_type)
         if coll_type is not None:
             if self.cat_cxt.use_custom_load(object_type):
-                out_list.append_collection(coll_type.load_collection(region,
-                                                                     self,
-                                                                     mjd=mjd))
+                coll = coll_type.load_collection(region, self, mjd=mjd,
+                                                 exposure=EXPOSURE_DEFAULT)
+                if isinstance(coll, ObjectCollection):
+                    out_list.append_collection(coll)
+                else:  # ObjectList
+                    out_list.append_object_list(coll)
                 return out_list
 
         if partition != 'None':
             if partition['type'] == 'healpix':
                 hps = self.get_hps_by_region(region, object_type)
                 for hp in hps:
-                    c = self.get_object_type_by_hp(hp, object_type,
-                                                   region, mjd)
+                    c = self.get_object_type_by_hp(hp, object_type, region,
+                                                   mjd,
+                                                   exposure=EXPOSURE_DEFAULT)
                     if len(c) > 0:
                         out_list.append_object_list(c)
                 return out_list
         else:
             raise NotImplementedError(f'Unsupported object type {object_type}')
 
-    def get_object_type_by_hp(self, hp, object_type, region=None, mjd=None):
+    def get_object_type_by_hp(self, hp, object_type, region=None, mjd=None,
+                              exposure=EXPOSURE_DEFAULT):
         object_list = ObjectList()
 
         #  Do we need to check more specifically by object type?
         # if hp not in self._hp_info:
         if hp not in self.hps_by_type(object_type):
             msg = f'In SkyCatalog.get_object_type_by_hp, healpix {hp}  '
             msg += f'intersects region but has no data file for {object_type}'
             self._logger.warning(msg)
             return object_list
 
         if object_type in ['galaxy', 'diffsky_galaxy']:
-            COLUMNS = ['galaxy_id', 'ra', 'dec']
+            columns = ['galaxy_id', 'ra', 'dec']
             id_name = 'galaxy_id'
         elif object_type in ['snana']:
-            COLUMNS = ['id', 'ra', 'dec', 'start_mjd', 'end_mjd']
+            columns = ['id', 'ra', 'dec', 'start_mjd', 'end_mjd']
             id_name = 'id'
         elif object_type in ['star', 'sncosmo']:
-            COLUMNS = ['object_type', 'id', 'ra', 'dec']
+            columns = ['object_type', 'id', 'ra', 'dec']
+            id_name = 'id'
+        elif object_type in ['sso']:
             id_name = 'id'
+            columns = ['id', 'ra', 'dec', 'mjd']
         else:
             raise NotImplementedError(f'Unsupported object type {object_type}')
 
         coll_class = self.cat_cxt.lookup_collection_type(object_type)
 
         if self.verbose:
             print('Working on healpix pixel ', hp)
         rdr_ot = dict()   # maps readers to set of object types it reads
 
         if 'file_template' in self._config['object_types'][object_type]:
             f_list = self._hp_info[hp]['object_types'][object_type] \
                 if object_type in self._hp_info[hp]['object_types'] else []
         elif 'parent' in self._config['object_types'][object_type]:
-            # ##f_list = self._hp_info[hp]['object_types'][self._config['object_types'][ot]['parent']]
             f_list = self._hp_info[hp]['object_types'][self._config['object_types'][object_type]['parent']]
 
         for f in f_list:
             if self._hp_info[hp]['files'][f] is None:        # no reader yet
                 full_path = os.path.join(self._cat_dir, f)
                 the_reader = ParquetReader(full_path, mask=None)
                 self._hp_info[hp]['files'][f] = the_reader
@@ -667,21 +705,21 @@
         # There will have to be some "if galaxy... else ... code"
         for rdr in the_readers:
             if 'ra' not in rdr.columns:
                 continue
 
             # Make a collection for each row group
             for rg in range(rdr.n_row_groups):
-                arrow_t = rdr.read_columns(COLUMNS, None, rg)
+                arrow_t = rdr.read_columns(columns, None, rg)
                 if object_type in {'galaxy', 'diffsky_galaxy', 'snana'}:
                     ra_c, dec_c, id_c, mask =\
                         _compress_via_mask(arrow_t,
                                            id_name,
                                            region,
-                                           source_type={object_type},
+                                           source_type=object_type,
                                            mjd=mjd)
                     if ra_c is not None:
                         new_collection = coll_class(ra_c, dec_c, id_c,
                                                     object_type, hp, self,
                                                     region=region,
                                                     mjd=mjd,
                                                     mask=mask,
@@ -689,15 +727,31 @@
                                                     row_group=rg)
                         if object_type == 'snana':
                             # file pattern really should come from cfg
                             base = f'snana_{hp}.hdf5'
                             SED_file = os.path.join(self._cat_dir, base)
                             new_collection.set_SED_file(SED_file)
                         object_list.append_collection(new_collection)
-
+                elif object_type in {'sso'}:
+                    ra_c, dec_c, id_c, mjd_c, mask =\
+                        _compress_via_mask(arrow_t,
+                                           id_name,
+                                           region,
+                                           source_type=object_type,
+                                           mjd=mjd, exposure=exposure)
+                    if ra_c is not None:
+                        new_collection = SsoCollection(ra_c, dec_c, id_c, hp,
+                                                       self,
+                                                       mjd_individual=mjd_c,
+                                                       region=region,
+                                                       mjd=mjd, mask=mask,
+                                                       readers=the_readers,
+                                                       row_group=rg,
+                                                       exposure=exposure)
+                        object_list.append_collection(new_collection)
                 else:
                     ra_c, dec_c, id_c, object_type_c, mask =\
                         _compress_via_mask(arrow_t, id_name, region,
                                            source_type={object_type})
                     if ra_c is not None and object_type_c[0] == object_type:
                         new_collection = coll_class(ra_c, dec_c, id_c,
                                                     object_type_c[0], hp,
@@ -747,288 +801,13 @@
     Returns
     -------
     SkyCatalog
     '''
     # Get bandpasses in case we need to compute fluxes
     _ = load_lsst_bandpasses()
     _ = load_roman_bandpasses()
-    base_dir = os.path.dirname(config_file)
-    YamlIncludeConstructor.add_to_loader_class(loader_class=yaml.SafeLoader,
-                                               base_dir=base_dir)
-    with open(config_file) as f:
-        return SkyCatalog(yaml.safe_load(f), skycatalog_root=skycatalog_root,
-                          mp=mp, verbose=verbose)
-
-
-if __name__ == '__main__':
-    import time
-    cfg_file_name = 'skyCatalog.yaml'
-    skycatalog_root = os.getenv('SKYCATALOG_ROOT')
-    catalog_dir = 'reorg'
-    if len(sys.argv) > 1:
-        catalog_dir = sys.argv[1]
-    if len(sys.argv) > 2:
-        cfg_file_name = sys.argv[2]
-
-    cfg_file = os.path.join(skycatalog_root, catalog_dir, cfg_file_name)
-
-    write_sed = False
-    if len(sys.argv) > 3:
-        write_sed = True
-
-    # For tract 3828
-    #   55.73604 < ra < 57.563452
-    #  -37.19001 < dec < -35.702481
-
-    cat = open_catalog(cfg_file, skycatalog_root=skycatalog_root)
-    hps = cat._find_all_hps()
-    print('Found {} healpix pixels '.format(len(hps)))
-    for h in hps:
-        print(h)
-    ra_min_tract = 55.736
-    ra_max_tract = 57.564
-    dec_min_tract = -37.190
-    dec_max_tract = -35.702
-    # ra_min_small = 56.0
-    # ra_max_small = 56.2
-    ra_min_small = 55.9
-    ra_max_small = 56.1
-    dec_min_small = -36.2
-    dec_max_small = -36.0
-
-    sed_fmt = 'lambda: {:.1f}  f_lambda: {:g}'
-
-    rgn = Box(ra_min_small, ra_max_small, dec_min_small, dec_max_small)
-    vertices = [(ra_min_small, dec_min_small), (ra_min_small, dec_max_small),
-                (ra_max_small, dec_max_small), (ra_max_small, dec_min_small)]
-    rgn_poly = PolygonalRegion(vertices_radec=vertices)
-
-    intersect_hps = _get_intersecting_hps('ring', 32, rgn)
-
-    print("For region ", rgn)
-    print("intersecting pixels are ", intersect_hps)
-
-    intersect_poly_hps = _get_intersecting_hps('ring', 32, rgn_poly)
-    print("For region ", rgn_poly)
-    print("intersecting pixels are ", intersect_poly_hps)
-
-    at_slac = os.getenv('HOME').startswith('/sdf/home/')
-    if not at_slac:
-        obj_types = {'star', 'galaxy', 'sncosmo', 'snana'}
-    else:
-        obj_types = {'star', 'galaxy', 'sncosmo', 'snana', 'gaia_star'}
-
-    print('Invoke get_objects_by_region with box region, no gaia')
-    t0 = time.time()
-    object_list = cat.get_objects_by_region(rgn,
-                                            obj_type_set={'star', 'galaxy',
-                                                          'sncosmo'},
-                                            mjd=63200.0)
-    t_done = time.time()
-    print('Took ', t_done - t0)
-    # #### temporary obj_type_set={'galaxy', 'star'} )
-    #                                        obj_type_set=set(['galaxy']) )
-    # Try out get_objects_by_hp with no region
-    # colls = cat.get_objects_by_hp(9812, None, set(['galaxy']) )
-
-    print('Number of collections returned for box:  ',
-          object_list.collection_count)
-    print('Object count for box: ', len(object_list))
-
-    print('Invoke get_objects_by_region with polygonal region')
-    t0 = time.time()
-    object_list_poly = cat.get_objects_by_region(rgn_poly,
-                                                 obj_type_set=obj_types)
-    t_done = time.time()
-    print('Took ', t_done - t0)
-
-    print('Number of collections returned for polygon:  ',
-          object_list_poly.collection_count)
-    assert(object_list.collection_count == object_list_poly.collection_count)
-    print('Object count for polygon: ', len(object_list_poly))
-
-    fudge = 5
-    assert(len(object_list_poly) > len(object_list) - fudge)
-    assert(len(object_list_poly) < len(object_list) + fudge)
-
-    print('Now try inscribed polygon which is not a box')
-    ra_avg = (ra_min_small + ra_max_small) * 0.5
-    dec_avg = (dec_min_small + dec_max_small) * 0.5
-    diamond_vertices = [(ra_min_small, dec_avg), (ra_avg, dec_max_small),
-                        (ra_max_small, dec_avg), (ra_avg, dec_min_small)]
-    rgn_diamond = PolygonalRegion(vertices_radec=diamond_vertices)
-
-    intersect_diamond_hps = _get_intersecting_hps('ring', 32, rgn_diamond)
-    print("for diamond region ", rgn_diamond)
-    print("intersecting pixels are ", intersect_diamond_hps)
-
-    print('Invoke get_objects_by_region with diamond region')
-    t0 = time.time()
-    object_list_diamond = cat.get_objects_by_region(rgn_diamond,
-                                                    obj_type_set=obj_types)
-    t_done = time.time()
-    print('Took ', t_done - t0)
-
-    print('Number of collections returned for diamond:  ',
-          object_list_diamond.collection_count)
-    print('Object count for diamond: ', len(object_list_diamond))
-
-    # ### TEMP FOR DEBUGGING
-    # ## exit(0)
-
-    # For now SIMS_SED_LIBRARY_DIR is undefined at SLAC, making it impossible
-    # to get SEDs for stars. So (crudely) determine whether or not
-    # we're running at SLAC
-
-    colls = object_list.get_collections()
-    got_a_sed = False
-    for c in colls:
-        n_obj = len(c)
-        print("For hpid ", c.get_partition_id(), "found ", n_obj, " objects")
-        if (n_obj) < 1:
-            continue
-        print("First object: ")
-        print(c[0], '\nid=', c[0].id, ' ra=', c[0].ra, ' dec=', c[0].dec,
-              ' belongs_index=', c[0]._belongs_index,
-              ' object_type: ', c[0].object_type)
-
-        if (n_obj < 3):
-            continue
-        print("Slice [1:3]")
-        slice13 = c[1:3]
-        for o in slice13:
-            print('id=', o.id, ' ra=', o.ra, ' dec=', o.dec, ' belongs_index=',
-                  o._belongs_index,  ' object_type: ', o.object_type)
-            print(o.object_type)
-            if o.object_type == 'star':
-                if not at_slac:
-                    print(o.get_instcat_entry())
-                    sed, magnorm = o._get_sed()
-                    print('For star magnorm: ', magnorm)
-                    if magnorm < 1000:
-                        print('Length of sed: ', len(sed.wave_list))
-            elif o.object_type == 'sncosmo':
-                print(o.get_instcat_entry())
-                for b in {'u', 'g', 'r', 'i', 'z', 'y'}:
-                    print(o.get_LSST_flux(b))
-            elif o.object_type == 'galaxy':
-                for cmp in ['disk', 'bulge', 'knots']:
-                    print(cmp)
-                    if cmp in o.subcomponents:
-                        # broken for galaxies currently
-                        # print(o.get_instcat_entry(component=cmp))
-                        sed, _ = o._get_sed(cmp)
-                        if sed:
-                            print('Length of sed table: ', len(sed.wave_list))
-                            if not got_a_sed:
-                                got_a_sed = True
-                                th = o.get_native_attribute(f'sed_val_{cmp}')
-                                print('Tophat values: ', th)
-                                sed, _ = o._get_sed(component=cmp)
-                                print('Simple sed wavelengths:')
-                                print(sed.wave_list)
-                                print('Simple sed values:')
-                                print([sed(w) for w in sed.wave_list])
-                                if write_sed:
-                                    o.write_sed('simple_sed.txt',
-                                                component=cmp)
-                                sed_fine, _ = o._get_sed(component=cmp,
-                                                         resolution=1.0)
-                                print('Bin width = 1 nm')
-                                print('Initial wl values',
-                                      sed_fine.wave_list[:20])
-                                print('Start at bin 100',
-                                      sed_fine.wave_list[100:120])
-                                print('Initial values')
-                                print([sed_fine(w) for w in sed_fine.wave_list[:20]])
-                                print('Start at bin 100')
-                                print([sed_fine(w) for w in sed_fine.wave_list[100:120]])
-                        else:
-                            print('All-zero sed')
 
-                # Try out old wrapper functions
-                print("\nget_dust:")
-                i_av, i_rv, g_av, g_rv = o._get_dust()
-                print(f'i_av={i_av} i_rv={i_rv} g_av={g_av} g_rv={g_rv}')
-                print("\nget_wl_params")
-                g1, g2, mu = o.get_wl_params()
-                print(f'g1={g1} g2={g2} mu={mu}')
-                print("\nget_gsobject_components. Keys of returned dict:")
-                gs_dict = o.get_gsobject_components()
-                print(gs_dict.keys())
-                print("\nget_observer_sed_components.  Keys of returned dict:")
-                o_seds = o.get_observer_sed_components()
-                print(o_seds.keys())
-
-                f = o.get_LSST_flux('i')
-                print(f'Flux for i bandpass: {f}')
-                fluxes = o.get_LSST_fluxes()
-                for k, v in fluxes.items():
-                    print(f'Bandpass {k} has flux {v}')
-
-        if n_obj > 200:
-            print("Object 200")
-            print(c[200], '\nid=', c[200].id, ' ra=', c[200].ra, ' dec=',
-                  c[200].dec,
-                  ' belongs_index=', c[200]._belongs_index)
-        if n_obj > 163997:
-            slice_late = c[163994:163997]
-            print('\nobjects indexed 163994 through 163996')
-            for o in slice_late:
-                print('id=', o.id, ' ra=', o.ra, ' dec=', o.dec,
-                      ' belongs_index=', o._belongs_index)
-
-    print('Total object count: ', len(object_list))
-
-    if len(object_list) == 0:
-        print('Empty object list. All done')
-        exit(0)
-
-    obj = object_list[0]
-    print("Type of element in object_list:", type(obj))
-
-    if object_list[0].object_type == 'galaxy':
-        redshift0 = object_list[0].get_native_attribute('redshift')
-        print('First redshift: ', redshift0)
-
-    sum = 0
-    for obj in object_list:
-        sum = sum + 1
-        if sum > 7216:
-            print("Sum is now ", sum)
-            print("obj id: ", obj.id)
-        if sum > 7220:
-            break
-
-    print(f'Object list len:  {len(object_list)}')
-    print(f'Objects found with "in":  {sum}')
-
-    if len(object_list) < 5:
-        print('Very short object list (< 5 elements).  done')
-        exit(0)
-
-    segment = object_list[2:5]
-    print('Information for slice 2:5 ')
-    for o in segment:
-        print(f'object {o.id} of type {o.object_type} belongs to collection {o._belongs_to}')
-
-    if len(object_list) < 304:
-        print('Object list len < 304.  All done')
-        exit(0)
-    print('\nInformation for slice 285:300')
-    segment = object_list[285:300]
-    for o in segment:
-        print(f'object {o.id} of type {o.object_type} belongs to collection {o._belongs_to}')
-
-    # ixes = ([3,5,8],)
-    ixes = (np.array([3, 5, 8, 300, 303]),)
-    print(f'\nObjects with indexes {ixes[0]}')
-    for o in object_list[ixes]:
-        print(o.id)
-    print('\nObjects in slice [3:9]')
-    for o in object_list[3:9]:
-        print(o.id)
-    print('\nObjects in slice [300:304]')
-    for o in object_list[300:304]:
-        print(o.id)
+    from skycatalogs.utils.config_utils import open_config_file
 
-    print('all done')
+    config_dict = open_config_file(config_file)
+    return SkyCatalog(config_dict, skycatalog_root=skycatalog_root, mp=mp,
+                      verbose=verbose)
```

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/utils/SED_parquet.py` & `skycatalogs-1.7.0rc3/skycatalogs/utils/SED_parquet.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/utils/add_extinction.py` & `skycatalogs-1.7.0rc3/skycatalogs/utils/add_extinction.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/utils/catalog_utils.py` & `skycatalogs-1.7.0rc3/skycatalogs/utils/catalog_utils.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/utils/common_utils.py` & `skycatalogs-1.7.0rc3/skycatalogs/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/utils/config_utils.py` & `skycatalogs-1.7.0rc3/skycatalogs/utils/config_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,99 @@
 import os
+import sys
 import yaml
-import git
 import logging
+from typing import Any
 from .exceptions import ConfigDuplicateKeyError
-# import jsonschema
-
 from collections import namedtuple
 
 __all__ = ['Config', 'open_config_file', 'Tophat', 'create_config',
            'assemble_SED_models', 'assemble_MW_extinction',
            'assemble_cosmology', 'assemble_object_types',
            'assemble_provenance', 'assemble_variability_models', 'write_yaml',
            'CURRENT_SCHEMA_VERSION']
 
 CURRENT_SCHEMA_VERSION = '1.2.0'
 
 
+class YamlIncludeLoader(yaml.SafeLoader):
+
+    """YAML Loader that supports file include directives.
+
+    Uses ``!include`` directive in a YAML file to point to another
+    YAML file to be included. The path in the include directive is relative
+    to the top-level file
+
+        storageClasses: !include storageClasses.yaml
+
+    Examples
+    --------
+    >>> with open("document.yaml", "r") as f:
+           data = yaml.load(f, Loader=YamlIncludeLoader)
+
+    Parameters
+    ----------
+    stream :  text io stream
+        The stream to parse.
+
+    This code was adapted from the LSST Science Pipelines Butler.
+    See in particular the Loader class in
+    daf_butler/python/lsst/daf/butler/_config.py in the daf_butler repo
+    https://github.com/lsst/daf_butler
+    """
+    def __init__(self, filestream):
+        super().__init__(filestream)
+        self._logger =  logging.getLogger('YamlIncludeLoader')
+        self._current_dir = os.path.dirname(filestream.name)
+        self.add_constructor("!include", YamlIncludeLoader.include)
+
+    def include(self, node: yaml.Node) -> list[Any] | dict[str, Any]:
+        result: list[Any] | dict[str, Any]
+        if isinstance(node, yaml.ScalarNode):
+            return self.extractFile(self.construct_scalar(node))  # type: ignore[arg-type]
+
+        elif isinstance(node, yaml.SequenceNode):
+            result = []
+            for filename in self.construct_sequence(node):
+                result.append(self.extractFile(filename))
+            return result
+
+        elif isinstance(node, yaml.MappingNode):
+            result = {}
+            for k, v in self.construct_mapping(node).items():
+                if not isinstance(k, str):
+                    raise TypeError(f"Expected only strings in YAML mapping; got {k!r} of type {type(k)}.")
+                result[k] = self.extractFile(v)
+            return result
+
+        else:
+            self._logger.error("Unrecognised node type in !include statement",
+                  file=sys.stderr)
+            raise yaml.constructor.ConstructorError
+
+    def extractFile(self, filepath: str) -> Any:
+        if filepath.startswith('/'):
+            actual_path = filepath
+        else:
+            actual_path = os.path.join(self._current_dir, filepath)
+        self._logger.info("Opening YAML file via !include: %s", actual_path)
+
+        # Read all the data from the resource
+        with open(actual_path) as f:
+            content = yaml.load(f, YamlIncludeLoader)
+        return content
+
+
 def open_config_file(config_file):
     '''
     Given path to config file, return a Config object
     '''
     with open(config_file) as f:
-        return Config(yaml.safe_load(f))
+        content = yaml.load(f, Loader=YamlIncludeLoader)
+        return Config(content)
 
 
 Tophat = namedtuple('Tophat', ['start', 'width'])
 
 
 def _custom_dir(c, add):
     '''
@@ -87,14 +155,17 @@
     def __getitem__(self, k):
         '''
         Specific override of __getitem__, delegating to dict member
         so that [ ] syntax will be handled properly
         '''
         return self._cfg.__getitem__(k)
 
+    def __contains__(self, k):
+        return k in self._cfg
+
     def list_sed_models(self):
         return self._cfg['SED_models'].keys()
 
     def list_object_types(self):
         return self._cfg['object_types'].keys()
 
     def get_sed_model(self, modelname):
@@ -206,16 +277,14 @@
             yaml.dump(input_dict, f)
 
     return outpath
 
 
 def create_config(catalog_name, logname=None):
     return Config({'catalog_name': catalog_name}, logname)
-#                  'schema_version': schema_version,
-#                  'code_version': desc.skycatalogs.__version__}, logname)
 
 
 def assemble_cosmology(cosmology):
     d = {k: cosmology.__getattribute__(k) for k in ('Om0', 'Ob0', 'sigma8',
                                                     'n_s')}
     d['H0'] = float(cosmology.H0.value)
     return d
@@ -243,14 +312,15 @@
     tophat_d = {'units': 'angstrom', 'bin_parameters': ['start', 'width']}
     tophat_d['bins'] = bins
     file_nm_d = {'units': 'nm'}
     return {'tophat': tophat_d, 'file_nm': file_nm_d}
 
 
 def assemble_provenance(pkg_root, inputs={}, schema_version=None):
+    import git
 
     if not schema_version:
         schema_version = CURRENT_SCHEMA_VERSION
     import skycatalogs
     version_d = {'schema_version': schema_version}
     if '__version__' in dir(skycatalogs):
         code_version = skycatalogs.__version__
```

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/utils/creator_utils.py` & `skycatalogs-1.7.0rc3/skycatalogs/utils/creator_utils.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/utils/exceptions.py` & `skycatalogs-1.7.0rc3/skycatalogs/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/utils/parquet_schema_utils.py` & `skycatalogs-1.7.0rc3/skycatalogs/utils/parquet_schema_utils.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/utils/sed_tools.py` & `skycatalogs-1.7.0rc3/skycatalogs/utils/sed_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import os
 import re
 from astropy import units as u
 from astropy.cosmology import FlatLambdaCDM
 import astropy.constants
 import h5py
+import sqlite3
+import pandas as pd
 
 import numpy as np
 from dust_extinction.parameter_averages import F19
 import galsim
 
-__all__ = ['TophatSedFactory', 'DiffskySedFactory', 'MilkyWayExtinction',
-           'get_star_sed_path', 'generate_sed_path']
+__all__ = ['TophatSedFactory', 'DiffskySedFactory', 'SsoSedFactory',
+           'MilkyWayExtinction', 'get_star_sed_path', 'generate_sed_path']
 
 
 class TophatSedFactory:
     '''
     Used for modeling cosmoDC2 galaxy SEDs, which are represented with
     a small number of wide bins
     '''
@@ -192,24 +194,51 @@
         f = self._load_file(pixel)
 
         sed_array = f['galaxy/'+str(int(galaxy_id)//100000)+'/'+str(galaxy_id)][:].astype('float')
         sed_array /= (4.0*np.pi*(self.dl(redshift_hubble))**2)
 
         seds = {}
         for i, component in enumerate(['bulge', 'disk', 'knots']):
-            lut = galsim.LookupTable(x=self._wave_list, f=sed_array[i,:],
+            lut = galsim.LookupTable(x=self._wave_list, f=sed_array[i, :],
                                      interpolant='linear')
             # Create the SED object and apply redshift.
             sed = galsim.SED(lut, wave_type='angstrom', flux_type='fnu')\
                         .atRedshift(redshift)
             seds[component] = sed
 
         return seds
 
 
+class SsoSedFactory():
+    '''
+    Load the single SED used for SSO objects and make it available as galsim
+    SED
+    '''
+    def __init__(self, sed_path, fmt='db'):
+        '''
+        For now only support db format.  In fact we're hardcoding additional
+        assumptions: that the table name is "SED" and that the columns are
+        "wavelength" (units angstroms) and "flux" (units flambda)
+        '''
+        if fmt != 'db':
+            raise ValueError(f'SsoSedFactory: Unsupport input format {fmt}; must be "db"')
+        wave_type = 'angstrom'
+        flux_type = 'flambda'
+        q = 'select wavelength, flux as flambda from SED order by wavelength'
+        with sqlite3.connect(sed_path) as conn:
+            sed_df = pd.read_sql_query(q, conn)
+        lut = galsim.LookupTable(x=sed_df['wavelength'], f=sed_df['flambda'],
+                                 interpolant='linear')
+        sed = galsim.SED(lut, wave_type=wave_type, flux_type=flux_type)
+        self.sed = sed
+
+    def create(self):
+        return self.sed
+
+
 class MilkyWayExtinction:
     '''
     Applies extinction to a SED
     '''
     def __init__(self, delta_wl=1.0, mwRv=3.1, eps=1e-7):
         """
         Parameters
```

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/utils/sn_tools.py` & `skycatalogs-1.7.0rc3/skycatalogs/utils/sn_tools.py`

 * *Files identical despite different names*

### Comparing `skyCatalogs-1.7.0rc2/skycatalogs/utils/translate_utils.py` & `skycatalogs-1.7.0rc3/skycatalogs/utils/translate_utils.py`

 * *Files identical despite different names*

