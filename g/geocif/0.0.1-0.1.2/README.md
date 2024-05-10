# Comparing `tmp/geocif-0.0.1.tar.gz` & `tmp/geocif-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocif-0.0.1.tar", last modified: Thu Mar  9 21:05:16 2023, max compression
+gzip compressed data, was "geocif-0.1.2.tar", last modified: Fri May 10 00:48:08 2024, max compression
```

## Comparing `geocif-0.0.1.tar` & `geocif-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 21:05:16.014794 geocif-0.0.1/
--rw-rw-rw-   0        0        0      313 2022-07-31 03:05:49.000000 geocif-0.0.1/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-03-09 21:05:15.407851 geocif-0.0.1/.github/
-drwxrwxrwx   0        0        0        0 2023-03-09 21:05:15.571203 geocif-0.0.1/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      531 2022-07-31 03:05:49.000000 geocif-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      516 2022-07-31 03:05:49.000000 geocif-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-rw-   0        0        0      459 2022-07-31 03:05:49.000000 geocif-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxrwx   0        0        0        0 2023-03-09 21:05:15.623546 geocif-0.0.1/.github/workflows/
--rw-rw-rw-   0        0        0     1382 2022-07-31 03:05:49.000000 geocif-0.0.1/.github/workflows/build.yml
--rw-rw-rw-   0        0        0      845 2022-07-31 03:05:49.000000 geocif-0.0.1/.github/workflows/docs.yml
--rw-rw-rw-   0        0        0      876 2022-07-31 03:05:49.000000 geocif-0.0.1/.github/workflows/pypi.yml
--rw-rw-rw-   0        0        0     1310 2022-07-31 03:05:49.000000 geocif-0.0.1/.gitignore
--rw-rw-rw-   0        0        0     1096 2022-07-31 03:05:49.000000 geocif-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2022-07-31 03:05:49.000000 geocif-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1375 2023-03-09 21:05:16.015785 geocif-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      602 2022-07-31 03:05:49.000000 geocif-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-09 21:05:15.735722 geocif-0.0.1/docs/
--rw-rw-rw-   0        0        0       96 2022-07-31 03:05:49.000000 geocif-0.0.1/docs/changelog.md
--rw-rw-rw-   0        0        0     3243 2022-07-31 03:05:49.000000 geocif-0.0.1/docs/contributing.md
--rw-rw-rw-   0        0        0        7 2022-07-31 03:05:49.000000 geocif-0.0.1/docs/faq.md
--rw-rw-rw-   0        0        0       39 2022-07-31 03:05:49.000000 geocif-0.0.1/docs/geocif.md
--rw-rw-rw-   0        0        0      506 2022-07-31 03:05:49.000000 geocif-0.0.1/docs/index.md
--rw-rw-rw-   0        0        0      612 2022-07-31 03:05:49.000000 geocif-0.0.1/docs/installation.md
-drwxrwxrwx   0        0        0        0 2023-03-09 21:05:15.748647 geocif-0.0.1/docs/overrides/
--rw-rw-rw-   0        0        0      285 2022-07-31 03:05:49.000000 geocif-0.0.1/docs/overrides/main.html
--rw-rw-rw-   0        0        0       67 2022-07-31 03:05:49.000000 geocif-0.0.1/docs/usage.md
-drwxrwxrwx   0        0        0        0 2023-03-09 21:05:15.894425 geocif-0.0.1/geocif/
--rw-rw-rw-   0        0        0      206 2023-03-06 15:53:46.000000 geocif-0.0.1/geocif/__init__.py
--rw-rw-rw-   0        0        0       47 2023-03-06 19:19:39.000000 geocif-0.0.1/geocif/base.py
-drwxrwxrwx   0        0        0        0 2023-03-09 21:05:15.960492 geocif-0.0.1/geocif/config/
--rw-rw-rw-   0        0        0      778 2023-03-09 18:44:52.000000 geocif-0.0.1/geocif/config/geocif.txt
--rw-rw-rw-   0        0        0       10 2023-03-09 00:39:51.000000 geocif-0.0.1/geocif/constants.py
--rw-rw-rw-   0        0        0       59 2022-08-15 02:41:03.000000 geocif-0.0.1/geocif/features.py
--rw-rw-rw-   0        0        0     7460 2023-03-09 18:56:48.000000 geocif-0.0.1/geocif/geoagmet.py
--rw-rw-rw-   0        0        0     7927 2023-03-09 18:36:54.000000 geocif-0.0.1/geocif/geocif.py
--rw-rw-rw-   0        0        0       59 2022-08-15 02:41:03.000000 geocif-0.0.1/geocif/models.py
--rw-rw-rw-   0        0        0    21917 2023-03-09 18:41:10.000000 geocif-0.0.1/geocif/plot.py
--rw-rw-rw-   0        0        0     3172 2023-03-09 00:43:50.000000 geocif-0.0.1/geocif/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-09 21:05:15.958491 geocif-0.0.1/geocif.egg-info/
--rw-rw-rw-   0        0        0     1375 2023-03-09 21:05:14.000000 geocif-0.0.1/geocif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      827 2023-03-09 21:05:15.000000 geocif-0.0.1/geocif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 21:05:14.000000 geocif-0.0.1/geocif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-06 15:54:57.000000 geocif-0.0.1/geocif.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-03-09 21:05:14.000000 geocif-0.0.1/geocif.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1217 2022-07-31 03:05:49.000000 geocif-0.0.1/mkdocs.yml
--rw-rw-rw-   0        0        0        0 2022-07-31 03:05:49.000000 geocif-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       82 2022-07-31 03:05:49.000000 geocif-0.0.1/requirements_dev.txt
--rw-rw-rw-   0        0        0      414 2023-03-09 21:05:16.046711 geocif-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1763 2022-07-31 03:05:49.000000 geocif-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 21:05:16.010790 geocif-0.0.1/tests/
--rw-rw-rw-   0        0        0       37 2022-07-31 03:05:49.000000 geocif-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0      403 2022-07-31 03:05:49.000000 geocif-0.0.1/tests/test_geocif.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:48:08.192232 geocif-0.1.2/
+-rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2557 2024-05-10 00:48:08.191213 geocif-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      602 2023-07-27 15:12:03.000000 geocif-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 00:48:08.028521 geocif-0.1.2/geocif/
+-rw-rw-rw-   0        0        0      148 2024-05-09 17:33:59.000000 geocif-0.1.2/geocif/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:48:08.116655 geocif-0.1.2/geocif/agmet/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.2/geocif/agmet/__init__.py
+-rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.2/geocif/agmet/geoagmet.py
+-rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.2/geocif/agmet/plot.py
+-rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.2/geocif/agmet/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:48:08.136478 geocif-0.1.2/geocif/backup/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.2/geocif/backup/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.2/geocif/backup/constants.py
+-rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.2/geocif/backup/features.py
+-rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.2/geocif/backup/geo.py
+-rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.2/geocif/backup/geocif.py
+-rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.2/geocif/backup/metadata.py
+-rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.2/geocif/backup/models.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:48:08.145477 geocif-0.1.2/geocif/cei/
+-rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.2/geocif/cei/__init__.py
+-rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.2/geocif/cei/definitions.py
+-rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.2/geocif/cei/indices.py
+-rw-rw-rw-   0        0        0    40714 2024-05-10 00:43:12.000000 geocif-0.1.2/geocif/geocif.py
+-rw-rw-rw-   0        0        0     6426 2024-05-09 19:50:03.000000 geocif-0.1.2/geocif/indices_runner.py
+-rw-rw-rw-   0        0        0     1846 2024-05-10 00:43:12.000000 geocif-0.1.2/geocif/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:48:08.186207 geocif-0.1.2/geocif/ml/
+-rw-rw-rw-   0        0        0        0 2024-05-09 17:32:51.000000 geocif-0.1.2/geocif/ml/__init__.py
+-rw-rw-rw-   0        0        0    31393 2024-05-09 15:38:37.000000 geocif-0.1.2/geocif/ml/analysis.py
+-rw-rw-rw-   0        0        0    12251 2024-05-09 21:07:36.000000 geocif-0.1.2/geocif/ml/correlations.py
+-rw-rw-rw-   0        0        0     5054 2024-05-09 20:41:26.000000 geocif-0.1.2/geocif/ml/embedding.py
+-rw-rw-rw-   0        0        0    12505 2024-05-09 22:33:28.000000 geocif-0.1.2/geocif/ml/feature_engineering.py
+-rw-rw-rw-   0        0        0     6562 2024-05-09 20:18:20.000000 geocif-0.1.2/geocif/ml/feature_selection.py
+-rw-rw-rw-   0        0        0    12461 2024-05-09 15:38:37.000000 geocif-0.1.2/geocif/ml/misc.py
+-rw-rw-rw-   0        0        0     9769 2024-05-09 15:38:36.000000 geocif-0.1.2/geocif/ml/outliers.py
+-rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.2/geocif/ml/outlook.py
+-rw-rw-rw-   0        0        0     3542 2024-05-09 19:16:41.000000 geocif-0.1.2/geocif/ml/output.py
+-rw-rw-rw-   0        0        0     8044 2024-05-09 19:16:41.000000 geocif-0.1.2/geocif/ml/stages.py
+-rw-rw-rw-   0        0        0     4961 2024-05-09 19:26:37.000000 geocif-0.1.2/geocif/ml/stats.py
+-rw-rw-rw-   0        0        0     9718 2024-05-09 21:02:58.000000 geocif-0.1.2/geocif/ml/trainers.py
+-rw-rw-rw-   0        0        0     3149 2024-05-09 19:24:05.000000 geocif-0.1.2/geocif/ml/trend.py
+-rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.2/geocif/ml/xai.py
+-rw-rw-rw-   0        0        0    18972 2024-05-09 19:38:53.000000 geocif-0.1.2/geocif/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:48:08.104592 geocif-0.1.2/geocif.egg-info/
+-rw-rw-rw-   0        0        0     2557 2024-05-10 00:48:07.000000 geocif-0.1.2/geocif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1031 2024-05-10 00:48:07.000000 geocif-0.1.2/geocif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      657 2024-05-10 00:48:07.000000 geocif-0.1.2/geocif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.2/geocif.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      656 2024-05-10 00:48:07.000000 geocif-0.1.2/geocif.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-10 00:48:07.000000 geocif-0.1.2/geocif.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      696 2024-05-10 00:44:31.000000 geocif-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0      414 2024-05-10 00:48:08.202269 geocif-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1619 2024-05-10 00:38:01.000000 geocif-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 00:48:08.188208 geocif-0.1.2/tests/
+-rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.2/tests/test_geocif.py
```

### Comparing `geocif-0.0.1/LICENSE` & `geocif-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geocif-0.0.1/README.md` & `geocif-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `geocif-0.0.1/geocif/geoagmet.py` & `geocif-0.1.2/geocif/agmet/geoagmet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,94 +1,56 @@
-import os
-
-import arrow as ar
 import pandas as pd
 from tqdm import tqdm
 
-from geocif import geocif, plot, utils
+from geocif.backup import geo
+from geocif.agmet import plot, utils
 
 
 def create_title_for_plot(obj):
-    region_name = obj.region.replace('_', ' ').title()
-    calendar_region_name = obj.calendar_region.replace('_', ' ').title()
-    country_name = obj.country.replace('_', ' ').title()
+    """
+
+    Args:
+        obj:
+
+    Returns:
+
+    """
+    region_name = obj.region.replace("_", " ").title()
+    calendar_region_name = obj.calendar_region.replace("_", " ").title()
+    country_name = obj.country.replace("_", " ").title()
     long_crop_name = utils.get_crop_name(obj.crop)
 
     # Get name of crop based on metadata/crop_per_season.csv file
-    df_crop_per_season = pd.read_csv(obj.dir_metadata / 'crop_per_season.csv')
+    df_crop_per_season = pd.read_csv(obj.dir_metadata / "crop_per_season.csv")
 
-    crop_name = df_crop_per_season[(df_crop_per_season['country'] == obj.country) &
-                                   (df_crop_per_season['crop'] == obj.crop) &
-                                   (df_crop_per_season['season'] == int(obj.growing_season))]['name'].values
+    crop_name = df_crop_per_season[
+        (df_crop_per_season["country"] == obj.country)
+        & (df_crop_per_season["crop"] == obj.crop)
+        & (df_crop_per_season["season"] == int(obj.growing_season))
+    ]["name"].values
 
-    crop_name = crop_name[0] if crop_name else long_crop_name.replace('_', ' ').title()
+    crop_name = crop_name[0] if crop_name else long_crop_name.replace("_", " ").title()
 
     title_line_1 = f"{region_name} ({calendar_region_name}, {country_name})"
     title_line_2 = f"{crop_name} {obj.plot_season}"
 
-    sup_title = f'{title_line_1}\n{title_line_2}'
+    sup_title = f"{title_line_1}\n{title_line_2}"
 
     return sup_title
 
 
-def plot_agmet(obj):
-    # Get crop calendar dates for region
-    dates_calendar = [obj.date_planting, obj.date_greenup, obj.date_senescence, obj.date_harvesting]
-
-    # TODO: Only plot if dates_calendar has valid dates
-    # Create title for plot
-    sup_title = create_title_for_plot(obj)
-
-    # Admin_1 level plots
-    plot.plots_ts_cur_yr(obj.df_region,
-                         obj.eo_plot,
-                         closest=obj.closest,
-                         dates_cal=dates_calendar,
-                         frcast_yr=obj.plot_season,
-                         logos=[obj.logo_harvest, obj.logo_geoglam],
-                         dir_out=obj.dir_output / obj.scale,
-                         sup_title=sup_title,
-                         fname=f'{obj.region}.png')
-
-    if obj.category == 'ewcm':
-        columns_v2 = ['cumulative_precip', 'daily_precip', 'soil_moisture_as1']
-        plot.plots_ts_cur_yr_v2(obj.df_region,
-                                columns_v2,
-                                closest=obj.closest,
-                                dates_cal=dates_calendar,
-                                frcast_yr=obj.plot_season,
-                                dir_out=obj.dir_condition / 'v2' / 'admin_1',
-                                sup_title=sup_title,
-                                sname_crop=obj.crop,
-                                fname=f'{obj.region}.png')
-
-        columns_v3 = ['cumulative_precip', 'ndvi', 'soil_moisture_as1']
-        plot.plots_ts_cur_yr_v3(obj.df_region,
-                                columns_v3,
-                                closest=obj.closest,
-                                dates_cal=dates_calendar,
-                                frcast_yr=obj.plot_season,
-                                dir_out=obj.dir_condition / 'v2' / 'admin_1',
-                                sup_title=sup_title,
-                                sname_crop=obj.crop,
-                                fname=f'{obj.region}.png')
-
-
 def loop_agmet(path_config_file=None):
     """
     Args:
     """
-    # Create GeoCif object
-    obj = geocif.GeoCif(path_config_file)
+    # Create geo object
+    obj = geo.geo(path_config_file)
 
-    # Parse configuration files
-    obj.parse_config()
-
-    # Read in statistics: area, yield, production, metadata
-    obj.read_statistics()
+    # Read in data on crop names in each country
+    obj.read_statistics(read_countries=True)
 
     # Create combinations of run parameters
     all_combinations = obj.create_run_combinations()
 
     pbar = tqdm(all_combinations, total=len(all_combinations))
     for country, scale, crop, growing_season in pbar:
         # Setup country information
@@ -97,72 +59,112 @@
         # Loop through seasons and plot for each admin_1 region and calendar region
         for plot_season in obj.plot_seasons:
             # Get list of the years that are closest to the year which we want to plot
             obj.get_closest_season(plot_season)
 
             for region in obj.list_regions:
                 # Setup the region information
-                obj.setup_region(region, plot_season, 'region')
+                obj.setup_region(region, plot_season, "region")
 
                 # If available, add CHIRPS-GEFS data to the dataframe
-                if obj.precip_var == 'chirps':
+                if obj.precip_var == "chirps":
                     obj.add_precip_forecast(plot_season)
 
                 # Get crop calendar dates for region
-                dates_calendar = [obj.date_planting, obj.date_greenup, obj.date_senescence, obj.date_harvesting]
+                dates_calendar = [
+                    obj.date_planting,
+                    obj.date_greenup,
+                    obj.date_senescence,
+                    obj.date_harvesting,
+                ]
 
                 # TODO: Only plot if dates_calendar has valid dates
                 # Create title for plot
                 sup_title = create_title_for_plot(obj)
 
                 ###############################################################
                 # Agmet plots for regions
                 ###############################################################
-                plot.plots_ts_cur_yr(obj.df_region,
-                                     obj.eo_plot,
-                                     closest=obj.closest,
-                                     dates_cal=dates_calendar,
-                                     frcast_yr=obj.plot_season,
-                                     logos=[obj.logo_harvest, obj.logo_geoglam],
-                                     dir_out=obj.dir_output / obj.scale,
-                                     sup_title=sup_title,
-                                     fname=f'{obj.region}.png')
+                # D:\Dropbox\Projects\GEOGLAM\crop_condition\AMIS\argentina
+                plot.plots_ts_cur_yr(
+                    obj.df_region,
+                    obj.eo_plot,
+                    closest=obj.closest,
+                    dates_cal=dates_calendar,
+                    frcast_yr=obj.plot_season,
+                    logos=[obj.logo_harvest, obj.logo_geoglam],
+                    dir_out=obj.dir_agmet / obj.scale,
+                    sup_title=sup_title,
+                    fname=f"{obj.region}.png",
+                )
 
                 ###############################################################
                 # Agmet plots for calendar regions
                 ###############################################################
-                columns = obj.eo_model + ['month', 'day', 'yield']
-                if 'chirps' in obj.df_region.columns:
-                    bool_year_check, bool_date_check = obj.check_date(obj.df_region, obj.plot_season)
+                columns = obj.eo_model + ["month", "day", "yield"]
+                if "chirps" in obj.df_region.columns:
+                    bool_year_check, bool_date_check = obj.check_date(
+                        obj.df_region, obj.plot_season
+                    )
 
                     if bool_date_check and bool_year_check:
-                        columns = obj.eo_plot + ['month', 'day', 'chirps_gefs', 'yield']
-
-                df_calendar_region = obj.df_region.groupby(['country', 'calendar_region', 'harvest_season', 'doy', 'datetime'])[columns].mean().reset_index()
-                df_calendar_region.set_index(pd.DatetimeIndex(df_calendar_region['datetime']), inplace=True, drop=True)
+                        columns = obj.eo_model + [
+                            "month",
+                            "day",
+                            "chirps_gefs",
+                            "yield",
+                        ]
+
+                df_calendar_region = (
+                    obj.df_region.groupby(
+                        [
+                            "country",
+                            "calendar_region",
+                            "harvest_season",
+                            "doy",
+                            "datetime",
+                        ]
+                    )[columns]
+                    .mean()
+                    .reset_index()
+                )
+                df_calendar_region.loc[:, "average_temperature"] = (
+                    df_calendar_region["cpc_tmax"] + df_calendar_region["cpc_tmin"]
+                ) / 2.0
+                df_calendar_region.set_index(
+                    pd.DatetimeIndex(df_calendar_region["datetime"]),
+                    inplace=True,
+                    drop=True,
+                )
                 df_calendar_region.index.name = None
-                df_calendar_region.sort_values(by='datetime', inplace=True)
+                df_calendar_region.sort_values(by="datetime", inplace=True)
 
                 # TODO: Only plot if dates_calendar has valid dates
                 # Create title for plot
                 sup_title = create_title_for_plot(obj)
 
                 if not df_calendar_region.empty:
-                    plot.plots_ts_cur_yr(df_calendar_region,
-                                         obj.eo_plot,
-                                         closest=obj.closest,
-                                         dates_cal=dates_calendar,
-                                         frcast_yr=obj.plot_season,
-                                         logos=[obj.logo_harvest, obj.logo_geoglam],
-                                         dir_out=obj.dir_output / 'district',
-                                         sup_title=sup_title,
-                                         fname=f'{obj.calendar_region}.png')
+                    plot.plots_ts_cur_yr(
+                        df_calendar_region,
+                        obj.eo_plot,
+                        closest=obj.closest,
+                        dates_cal=dates_calendar,
+                        frcast_yr=obj.plot_season,
+                        logos=[obj.logo_harvest, obj.logo_geoglam],
+                        dir_out=obj.dir_agmet / "district",
+                        sup_title=sup_title,
+                        fname=f"{obj.calendar_region}.png",
+                    )
 
 
 def run():
-    loop_agmet(['D:/Users/ritvik/projects/geoprepare/geoprepare/geoprepare.txt',
-                'D:/Users/ritvik/projects/geoprepare/geoprepare/geoextract.txt',
-                'D:/Users/ritvik/projects/geocif/geocif/config/geocif.txt'])
+    loop_agmet(
+        [
+            "D:/Users/ritvik/projects/geoprepare/geoprepare/geoprepare.txt",
+            "D:/Users/ritvik/projects/geoprepare/geoprepare/geoextract.txt",
+            "D:/Users/ritvik/projects/geocif/geocif/config/geocif.txt",
+        ]
+    )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     run()
```

### Comparing `geocif-0.0.1/geocif/geocif.py` & `geocif-0.1.2/geocif/backup/geo.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,204 +2,290 @@
 import ast
 import itertools
 import math
 
 import arrow as ar
 import numpy as np
 import pandas as pd
-import neptune.new as neptune
+import neptune
 from pathlib import Path
 
 from geoprepare import base, log
 
 
-class GeoCif(base.BaseGeo):
+class geo(base.BaseGeo):
     def __init__(self, path_config_file):
         super().__init__(path_config_file)
 
-    def parse_config(self, section='DEFAULT'):
+        # Parse configuration files
+        self.parse_config()
+
+    def parse_config(self, section="DEFAULT"):
         """
 
         Args:
             section ():
 
         Returns:
 
         """
-        super().parse_config(section='DEFAULT')
+        super().parse_config(section="DEFAULT")
 
-        self.countries = ast.literal_eval(self.parser.get('DEFAULT', 'countries'))
-        self.forecast_seasons = ast.literal_eval(self.parser.get('DEFAULT', 'forecast_seasons'))
-        self.plot_seasons = ast.literal_eval(self.parser.get('DEFAULT', 'plot_seasons'))
-        self.models = ast.literal_eval(self.parser.get('DEFAULT', 'models'))
-        self.eo_plot = ast.literal_eval(self.parser.get('DEFAULT', 'eo_plot'))
-        self.eo_model = ast.literal_eval(self.parser.get('DEFAULT', 'eo_model'))
-        self.logo_harvest = self.dir_metadata / self.parser.get('METADATA', 'logo_harvest')
-        self.logo_geoglam = self.dir_metadata / self.parser.get('METADATA', 'logo_geoglam')
+        self.countries = ast.literal_eval(self.parser.get("DEFAULT", "countries"))
+        self.forecast_seasons = ast.literal_eval(
+            self.parser.get("DEFAULT", "forecast_seasons")
+        )
+        self.plot_seasons = ast.literal_eval(self.parser.get("DEFAULT", "plot_seasons"))
+        self.models = ast.literal_eval(self.parser.get("DEFAULT", "models"))
+        self.eo_plot = ast.literal_eval(self.parser.get("DEFAULT", "eo_plot"))
+        self.eo_model = ast.literal_eval(self.parser.get("DEFAULT", "eo_model"))
+        self.logo_harvest = self.dir_metadata / self.parser.get(
+            "METADATA", "logo_harvest"
+        )
+        self.logo_geoglam = self.dir_metadata / self.parser.get(
+            "METADATA", "logo_geoglam"
+        )
 
         # self.lag_area_as_feature = self.parser.getboolean('DEFAULT', 'lag_area_as_feature')
         # self.location_as_feature = self.parser.getboolean('DEFAULT', 'location_as_feature')
 
         # MLOPS
-        self.neptune_username = self.parser.get('MLOPS', 'neptune_username')
-        self.neptune_project = self.parser.get('MLOPS', 'neptune_project')
+        self.neptune_username = self.parser.get("MLOPS", "neptune_username")
+        self.neptune_project = self.parser.get("MLOPS", "neptune_project")
 
         # Setup experiment logging, check results at https://app.neptune.ai/
-        self.tracker = neptune.init(project=f'{self.neptune_username}/{self.neptune_project}',
-                                    capture_hardware_metrics=False,
-                                    source_files=[],
-                                    capture_stderr=False)
+        self.tracker = neptune.init_run(
+            project=f"{self.neptune_username}/{self.neptune_project}",
+            capture_hardware_metrics=False,
+            source_files=[],
+            capture_stderr=False,
+        )
 
     def get_calendar_region_for_region(self, df, region):
         """
 
         Args:
             df ():
             region ():
 
         Returns:
 
         """
-        calendar_region = df[df['region'] == region]['calendar_region'].values[0]
+        calendar_region = df[df["region"] == region]["calendar_region"].values[0]
 
         return calendar_region
 
     def setup_country(self, country, scale, crop, growing_season):
         self.country = country
         self.scale = scale
         self.crop = crop
         self.growing_season = growing_season
-        self.category = self.parser.get(country, 'category')
-        self.use_cropland_mask = self.parser.getboolean(country, 'USE_CROPLAND_MASK')
+        self.category = self.parser.get(country, "category")
+        self.use_cropland_mask = self.parser.getboolean(country, "USE_CROPLAND_MASK")
 
         self.get_dirname(country)
         self.get_ccs_dataframe(country, scale, crop, growing_season)
 
         # Get list of regions in ccs dataframe
-        self.list_regions = self.df_ccs['region'].unique()
+        self.list_regions = self.df_ccs["region"].unique()
 
         # Get list of calendar regions in ccs dataframe
-        self.list_calendar_regions = self.df_ccs['calendar_region'].unique()
+        self.list_calendar_regions = self.df_ccs["calendar_region"].unique()
+
+        self.precip_var = (
+            "chirps" if "chirps" in self.df_ccs.columns.values else "cpc_precip"
+        )
 
-        self.precip_var = 'chirps' if 'chirps' in self.df_ccs.columns.values else 'cpc_precip'
+        # Append current date to the output directory
+        self.dir_output = self.dir_output / ar.now().format("MMMM_DD_YYYY")
 
-    def setup_region(self, region, plot_season, type_region='region'):
+    def setup_region(self, region, plot_season, type_region="region"):
         self.region = region
         self.calendar_region = self.get_calendar_region_for_region(self.df_ccs, region)
         self.plot_season = plot_season
         self.type_region = type_region
 
         # get ccs dataframe for region/calendar_region
-        if type_region == 'region':
-            self.df_region = self.df_ccs[self.df_ccs['region'] == region]
-        elif type_region == 'calendar_region':
-            self.df_region = self.df_ccs[self.df_ccs['calendar_region'] == self.calendar_region]
+        if type_region == "region":
+            self.df_region = self.df_ccs[self.df_ccs["region"] == region]
+        elif type_region == "calendar_region":
+            self.df_region = self.df_ccs[
+                self.df_ccs["calendar_region"] == self.calendar_region
+            ]
+        elif type_region == "region_year":
+            self.df_region = self.df_ccs[
+                (self.df_ccs["region"] == region) & (self.df_ccs["year"] == plot_season)
+            ]
+        elif type_region == "calendar_region_year":
+            self.df_region = self.df_ccs[
+                (self.df_ccs["calendar_region"] == self.calendar_region)
+                & (self.df_ccs["year"] == plot_season)
+            ]
+        else:
+            raise ValueError(f"Unknown type_region: {type_region}")
 
         # convert df_region index to datetime
         self.df_region.index = pd.to_datetime(self.df_region.index)
 
-        # Get phenological transition dates from crop calendar
-        self.date_planting, self.date_greenup, self.date_senescence, self.date_harvesting = \
-            self.get_calendar(self.region, self.plot_season)
+        # Setup output directory for agmet graphics
+        # Create output directory
+        folder = f"{self.crop}_s{self.growing_season}_{self.plot_season}"
+        self.dir_agmet = (
+            self.dir_output
+            / "crop_condition"
+            / self.category
+            / self.country
+            / folder
+            / "condition"
+        )
+        # dir_output = self.dir_output / 'crop_condition' / self.category / self.country / folder
 
+        # Get phenological transition dates from crop calendar
+        (
+            self.date_planting,
+            self.date_greenup,
+            self.date_senescence,
+            self.date_harvesting,
+        ) = self.get_calendar(self.region, self.plot_season)
 
     def create_run_combinations(self):
         """
         Create combinations of run parameters.
         Returns:
         """
         all_combinations = []
 
         for country in self.countries:
-            scales = ast.literal_eval(self.parser.get(country, 'scales'))
-            crops = ast.literal_eval(self.parser.get(country, 'crops'))
-            growing_seasons = ast.literal_eval(self.parser.get(country, 'growing_seasons'))
+            scales = ast.literal_eval(self.parser.get(country, "scales"))
+            crops = ast.literal_eval(self.parser.get(country, "crops"))
+            growing_seasons = ast.literal_eval(
+                self.parser.get(country, "growing_seasons")
+            )
 
             for scale in scales:
                 for crop in crops:
                     for growing_season in growing_seasons:
-                        all_combinations.extend(list(itertools.product([country], [scale], [crop], [growing_season])))
+                        all_combinations.extend(
+                            list(
+                                itertools.product(
+                                    [country], [scale], [crop], [growing_season]
+                                )
+                            )
+                        )
 
         return all_combinations
 
     def get_calendar(self, region, forecast_season):
         """
         Get calendar information for region
         Args:
             region:
 
         Returns:
 
         """
-        SEASON = 'harvest_season'
-        CAL = 'crop_calendar'
+        SEASON = "harvest_season"
+        CAL = "crop_calendar"
 
-        df_sub = self.df_ccs[self.df_ccs['region'] == region]  # region specific data frame
-
-        sr_cal = df_sub[df_sub[SEASON] == forecast_season][['doy', CAL]]  # Pandas series with calendar info
+        df_sub = self.df_ccs[
+            self.df_ccs["region"] == region
+        ]  # region specific data frame
+        df_sub.index = pd.to_datetime(df_sub.index)
+        sr_cal = df_sub[df_sub[SEASON] == forecast_season][
+            ["doy", CAL]
+        ]  # Pandas series with calendar info
 
         # Change calendar column to int if it is not
-        sr_cal[CAL] = pd.to_numeric(sr_cal[CAL], errors='coerce')
+        sr_cal[CAL] = pd.to_numeric(sr_cal[CAL], errors="coerce")
 
         # Get the crop calendar dates
         if sr_cal.empty:
             return np.NaN, np.NaN, np.NaN, np.NaN
         else:
             date_planting = (sr_cal[CAL] == 1).idxmax()
-            date_greenup = (sr_cal[CAL] == 2).idxmax() if len(sr_cal[sr_cal[CAL] == 2]) else None
-            date_senesc = (sr_cal[CAL][::-1] == 2).idxmax() if len(sr_cal[sr_cal[CAL] == 3]) else None
-            date_harvesting = (sr_cal[CAL][::-1] == 3).idxmax() if len(sr_cal[sr_cal[CAL] == 3]) else None
+            date_greenup = (
+                (sr_cal[CAL] == 2).idxmax() if len(sr_cal[sr_cal[CAL] == 2]) else None
+            )
+            date_senesc = (
+                (sr_cal[CAL][::-1] == 2).idxmax()
+                if len(sr_cal[sr_cal[CAL] == 3])
+                else None
+            )
+            date_harvesting = (
+                (sr_cal[CAL][::-1] == 3).idxmax()
+                if len(sr_cal[sr_cal[CAL] == 3])
+                else None
+            )
 
             return date_planting, date_greenup, date_senesc, date_harvesting
 
     def get_ccs_dataframe(self, country, scale, crop, growing_season):
         # Read in ccs file using geomerge object
         dir_ccs = self.dir_input / self.dir_threshold / country / scale
 
-        self.df_ccs = pd.read_csv(dir_ccs / f"{crop}_s{growing_season}.csv", index_col=0)
+        self.df_ccs = pd.read_csv(
+            dir_ccs / f"{crop}_s{growing_season}.csv", index_col=0
+        )
 
-        # convert datetime column to type datetime and set as index
-        self.df_ccs.index = pd.to_datetime(self.df_ccs['datetime'])
+        # convert index to datetime column with type datetime
+        self.df_ccs["datetime"] = pd.to_datetime(self.df_ccs.index)
         self.df_ccs.index.name = None
 
-    def get_closest_season(self, plot_season):
+    def get_closest_season(self, season):
         from heapq import nsmallest
 
-        self.closest = nsmallest(5 + 1, range(2001, ar.utcnow().year), key=lambda x: abs(x - plot_season))
+        self.closest = nsmallest(
+            5 + 1, range(2001, ar.utcnow().year), key=lambda x: abs(x - season)
+        )
 
-        if plot_season in self.closest:
-            self.closest.remove(plot_season)
+        if season in self.closest:
+            self.closest.remove(season)
 
     def check_date(self, df, plot_season):
         # Check if the last date in the CHIRPS-GEFS data is within the growing season
-        last_valid_date = pd.to_datetime(df['chirps'].last_valid_index()).date()
+        last_valid_date = pd.to_datetime(df["chirps"].last_valid_index()).date()
 
         bool_year_check = ar.utcnow().year <= plot_season
-        bool_date_check = ((last_valid_date > self.date_planting.date()) & (last_valid_date < self.date_harvesting.date()))
+        bool_date_check = (last_valid_date > self.date_planting.date()) & (
+            last_valid_date < self.date_harvesting.date()
+        )
 
         return bool_year_check, bool_date_check
 
     def add_precip_forecast(self, plot_season):
         bool_year_check, bool_date_check = self.check_date(self.df_ccs, plot_season)
 
         if bool_year_check & bool_date_check:
             # Get CHIRPS-GEFS data for region
-            base_dir = self.dir_input / self.dir_threshold / 'chirps_gefs' / self.country
-            path_gefs = base_dir / 'cr' if self.use_cropland_mask else base_dir / self.crop
-
-            df_gefs = pd.read_csv(list(path_gefs.glob(self.df_region[self.scale].unique()[0] + '*.csv'))[0], header=None)
-            val_gefs = df_gefs.values[0][5] if not math.isnan(df_gefs.values[0][5]) else 0.
+            base_dir = self.dir_input / self.dir_threshold / self.country / self.scale
+            path_gefs = (
+                base_dir / "cr" / "chirps_gefs"
+                if self.use_cropland_mask
+                else base_dir / self.crop / "chirps_gefs"
+            )
+
+            df_gefs = pd.read_csv(
+                list(path_gefs.glob(self.df_region["region"].unique()[0] + "*.csv"))[0],
+                header=None,
+            )
+            val_gefs = (
+                float(df_gefs.values[1][5])
+                if not math.isnan(float(df_gefs.values[1][5]))
+                else 0.0
+            )
 
             # Add CHIRPS-GEFS
             start_date = ar.utcnow().shift(days=+15).date()
             end_date = ar.utcnow().shift(days=+16).date()
 
-            self.df_region.loc[start_date:end_date, 'chirps_gefs'] = val_gefs
-            self.df_ccs.loc[start_date.strftime('%Y-%m-%d'), 'chirps_gefs'] = val_gefs
+            self.df_region.loc[start_date:end_date, "chirps_gefs"] = val_gefs
+            self.df_ccs.loc[start_date.strftime("%Y-%m-%d"), "chirps_gefs"] = val_gefs
+
 
 def run(params=None):
     import time
-    time.sleep(60*25)
+
+    time.sleep(60 * 25)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     pass
```

### Comparing `geocif-0.0.1/geocif/plot.py` & `geocif-0.1.2/geocif/agmet/plot.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,70 +7,73 @@
 import bottleneck as bn
 import arrow as ar
 import matplotlib.pyplot as plt
 import palettable as pal
 from cycler import cycler
 from matplotlib import rcParams
 
-from geocif import constants, utils
+from geocif.backup import constants
+from geocif.agmet import utils
 
 
 def set_matplotlib_params():
     """
     Set matplotlib defaults to nicer values
     Returns:
 
     """
     # rcParams dict
-    rcParams['mathtext.default'] = 'regular'
-    rcParams['axes.labelsize'] = 12
-    rcParams['xtick.labelsize'] = 12
-    rcParams['ytick.labelsize'] = 12
-    rcParams['legend.fontsize'] = 12
-    rcParams['font.family'] = 'sans-serif'
-    rcParams['font.serif'] = ['Helvetica']
-    rcParams['legend.numpoints'] = 1
+    rcParams["mathtext.default"] = "regular"
+    rcParams["axes.labelsize"] = 12
+    rcParams["xtick.labelsize"] = 12
+    rcParams["ytick.labelsize"] = 12
+    rcParams["legend.fontsize"] = 12
+    rcParams["font.family"] = "sans-serif"
+    rcParams["font.serif"] = ["Helvetica"]
+    rcParams["legend.numpoints"] = 1
     # rcParams['figure.figsize'] = 7.3, 4.2
 
 
-def get_colors(palette='colorbrewer', cmap=False, only_colors=False):
+def get_colors(palette="colorbrewer", cmap=False, only_colors=False):
     """
     Get palettable colors, which are nicer
     Args:
         palette:
         cmap:
 
     Returns:
 
     """
-    if palette == 'colorbrewer':
+    if palette == "colorbrewer":
         bmap = pal.colorbrewer.diverging.PRGn_11.mpl_colors
         if cmap:
             bmap = pal.colorbrewer.diverging.PRGn_11.mpl_colormap
-    elif palette == 'tableau':
+    elif palette == "tableau":
         bmap = pal.tableau.Tableau_20.mpl_colors
         if cmap:
             bmap = pal.tableau.Tableau_20.mpl_colormap
-    elif palette == 'cubehelix':
+    elif palette == "cubehelix":
         bmap = pal.cubehelix.cubehelix2_16.mpl_colors
         if cmap:
             bmap = pal.cubehelix.cubehelix2_16.mpl_colormap
-    elif palette == 'qualitative':
+    elif palette == "qualitative":
         bmap = pal.tableau.GreenOrange_12.mpl_colors
         if cmap:
             bmap = pal.tableau.GreenOrange_12.mpl_colormap
 
     if cmap:
         return bmap
 
     if only_colors:
-        color_cycle = cycler('color', bmap)  # color cycle
+        color_cycle = cycler("color", bmap)  # color cycle
     else:
-        color_cycle = (cycler(marker=['*', 'o']) * cycler('ls', ['-', '--'])) * cycler('color', bmap)  # color cycle
-    plt.rc('axes', prop_cycle=color_cycle)
+        color_cycle = (cycler(marker=["*", "o"]) * cycler("ls", ["-", "--"])) * cycler(
+            "color", bmap
+        )  # color cycle
+    plt.rc("axes", prop_cycle=color_cycle)
 
     return bmap
 
 
 def compute_stats(df_current, df_last, df_previous, var, window):
     """
 
@@ -80,34 +83,55 @@
         df_previous:
         var:
         window:
 
     Returns:
 
     """
-    df_mean_vals = df_previous.groupby(df_previous['doy'])[var].mean()
-    df_mean_vals = df_mean_vals.reindex(index=df_current['doy'])  # reorder to match current season dates
-
-    df_min_vals = df_previous.groupby(df_previous['doy'])[var].min()
-    df_min_vals = df_min_vals.reindex(index=df_current['doy'])  # reorder to match current season dates
-
-    df_max_vals = df_previous.groupby(df_previous['doy'])[var].max()
-    df_max_vals = df_max_vals.reindex(index=df_current['doy'])  # reorder to match current season dates
+    df_mean_vals = df_previous.groupby(df_previous["doy"])[var].mean()
+    df_mean_vals = df_mean_vals.reindex(
+        index=df_current["doy"]
+    )  # reorder to match current season dates
+
+    df_min_vals = df_previous.groupby(df_previous["doy"])[var].min()
+    df_min_vals = df_min_vals.reindex(
+        index=df_current["doy"]
+    )  # reorder to match current season dates
+
+    df_max_vals = df_previous.groupby(df_previous["doy"])[var].max()
+    df_max_vals = df_max_vals.reindex(
+        index=df_current["doy"]
+    )  # reorder to match current season dates
 
     curr_vals = bn.move_mean(df_current[var].values, window=window, min_count=1)
     last_vals = bn.move_mean(df_last[var].values, window=window, min_count=1)
     past_vals = bn.move_mean(df_mean_vals.values, window=window, min_count=1)
 
-    min_vals = bn.move_mean(np.minimum(df_min_vals.values, df_mean_vals.values), window=window, min_count=1)
-    max_vals = bn.move_mean(np.maximum(df_max_vals.values, df_mean_vals.values), window=window, min_count=1)
+    min_vals = bn.move_mean(
+        np.minimum(df_min_vals.values, df_mean_vals.values), window=window, min_count=1
+    )
+    max_vals = bn.move_mean(
+        np.maximum(df_max_vals.values, df_mean_vals.values), window=window, min_count=1
+    )
 
     return df_mean_vals, curr_vals, last_vals, past_vals, min_vals, max_vals
 
 
-def plots_ts_cur_yr(df, names_cols, closest=None, dates_cal=None, frcast_yr=None, logos=None, window=5, dir_out='', sup_title='', fname=''):
+def plots_ts_cur_yr(
+    df,
+    names_cols,
+    closest=None,
+    dates_cal=None,
+    frcast_yr=None,
+    logos=None,
+    window=5,
+    dir_out="",
+    sup_title="",
+    fname="",
+):
     """
     Expectes dataframe to have a time-series index
     Args:
         df:
         names_cols:
         closest:
         dates_cal:
@@ -120,346 +144,627 @@
 
     Returns:
 
     """
     use_forecast = False
     os.makedirs(dir_out, exist_ok=True)
 
-    color_list = get_colors('tableau', only_colors=True)
+    color_list = get_colors("tableau", only_colors=True)
 
-    # If all values of column to be plotted are NaN, then return
+    # Figure out source of precip (chirps or cpc_precip)
+    precip_var = "chirps" if "chirps" in df.columns.values else "cpc_precip"
+
+    # # If all values of column to be plotted are NaN, then return
     available_cols = []
-    for col in names_cols:
+    for col in names_cols + [precip_var]:
         if col in df.columns.values:
             available_cols.append(col)
-    if df[available_cols].isnull().values.all():
-        return pd.DataFrame()
-
-    # Figure out source of precip (chirps or cpc_precip)
-    precip_var = 'chirps' if 'chirps' in df.columns.values else 'cpc_precip'
+    # if df[available_cols].isnull().values.all():
+    #     return pd.DataFrame()
 
     # Specify number of columns, should not exceed 3
-    ncols = 3 if int(len(names_cols) / 2.) >= 2 else int(math.floor(len(names_cols) / 2.))
-    nrows = int(math.ceil(len(names_cols) / 3.))
-
-    # compute average daily temp
-    df['average_temperature'] = (df['cpc_tmax'] + df['cpc_tmin'])/2.
+    ncols = (
+        3 if int(len(names_cols) / 2.0) >= 2 else int(math.floor(len(names_cols) / 2.0))
+    )
+    nrows = int(math.ceil(len(names_cols) / 3.0))
 
     # Get data frame of current year
-    df_current = df[df['harvest_season'] == frcast_yr]
-    df_last = df[df['harvest_season'] == frcast_yr - 1]
+    df_current = df[df["harvest_season"] == frcast_yr]
+    df_last = df[df["harvest_season"] == frcast_yr - 1]
 
     # If df_current has no non NaN data for current season then do not plot
     _num_nans = 0
     for idx in range(len(available_cols)):
         # TODO: replace sliding_mean with numpy convolve function
-        if np.all(np.isnan(utils.sliding_mean(df_current[available_cols[idx]].values, window=window))):
+        if np.all(
+            np.isnan(
+                utils.sliding_mean(
+                    df_current[available_cols[idx]].values, window=window
+                )
+            )
+        ):
             _num_nans += 1
 
     if _num_nans == len(available_cols):
         return pd.DataFrame()
 
     # Get data frame of previous years for the same month and days as df_current
-    df_previous = df[np.in1d(df['month'], df_current.index.month) &
-                 np.in1d(df['day'], df_current.index.day) &
-                 (df['harvest_season'].isin(closest))]
+    df_previous = df[
+        np.in1d(df["month"], df_current.index.month)
+        & np.in1d(df["day"], df_current.index.day)
+        & (df["harvest_season"].isin(closest))
+    ]
 
     # Drop rows where harvest_season is missing i.e. NaN
-    df_previous = df_previous[np.isfinite(df_previous['harvest_season'])]
+    df_previous = df_previous[np.isfinite(df_previous["harvest_season"])]
 
     # Drop rows for year greater than current year
-    df_previous = df_previous[df_previous['harvest_season'] < datetime.datetime.now().year]
-
-    if df_current.empty or df_previous.empty or df_current['cpc_tmax'].isnull().values.all():
+    df_previous = df_previous[
+        df_previous["harvest_season"] < datetime.datetime.now().year
+    ]
+
+    if (
+        df_current.empty
+        or df_previous.empty
+        or df_current["cpc_tmax"].isnull().values.all()
+    ):
         return pd.DataFrame()
 
     # Plot current year
     fig, ax = plt.subplots(nrows, ncols, squeeze=False, figsize=(20, 10))
     # delete empty axes
     for i in range(len(names_cols), nrows * ncols):
         fig.delaxes(ax.flatten()[i])
 
     # ax[0, 0].grid(True)
-    fig.suptitle(sup_title, fontsize=16, fontweight='bold')
-    rcParams['xtick.labelsize'] = 12
-    rcParams['ytick.labelsize'] = 12
-    rcParams['axes.labelsize'] = 12
+    fig.suptitle(sup_title, fontsize=16, fontweight="bold")
+    rcParams["xtick.labelsize"] = 12
+    rcParams["ytick.labelsize"] = 12
+    rcParams["axes.labelsize"] = 12
 
     # Create individual plots
     for idx in range(len(names_cols)):
         # 'ndvi', 'cumulative_precip', 'cpc_tmax', 'yearly_ndvi', 'daily_precip', 'cpc_tmax', 'esi_4wk', 'cpc_tmin', 'soil_moisture_as1'
-        if names_cols[idx] in ['cumulative_precip', 'daily_precip']:
+        if names_cols[idx] in ["cumulative_precip", "daily_precip"]:
             cur_var = precip_var
-        elif names_cols[idx] in ['ndvi', 'yearly_ndvi']:
-            cur_var = 'ndvi'
-        elif names_cols[idx] in ['gcvi', 'yearly_gcvi']:
-            cur_var = 'gcvi'
+        elif names_cols[idx] in ["ndvi", "yearly_ndvi"]:
+            cur_var = "ndvi"
+        elif names_cols[idx] in ["gcvi", "yearly_gcvi"]:
+            cur_var = "gcvi"
         else:
             cur_var = names_cols[idx]
 
         _window = window
 
         ax[idx // 3, idx % 3] = plt.subplot(nrows, ncols, idx + 1)
 
         # Setup major and minor locations for time on x axis
         ax[idx // 3, idx % 3].xaxis.set_major_locator(matplotlib.dates.YearLocator())
-        ax[idx // 3, idx % 3].xaxis.set_minor_locator(matplotlib.dates.MonthLocator(range(1, 13)))
-
-        ax[idx // 3, idx % 3].xaxis.set_major_formatter(matplotlib.dates.DateFormatter("\n%Y"))
-        ax[idx // 3, idx % 3].xaxis.set_minor_formatter(matplotlib.dates.DateFormatter("%b"))
+        ax[idx // 3, idx % 3].xaxis.set_minor_locator(
+            matplotlib.dates.MonthLocator(range(1, 13))
+        )
+
+        ax[idx // 3, idx % 3].xaxis.set_major_formatter(
+            matplotlib.dates.DateFormatter("\n%Y")
+        )
+        ax[idx // 3, idx % 3].xaxis.set_minor_formatter(
+            matplotlib.dates.DateFormatter("%b")
+        )
 
         # Plot title for each subplot except cpc_tmax; y label for all though
         # if names_cols[idx] != 'cpc_tmax':
         #     plt.title(cc.dict_vars.get(cur_var)[0], fontsize=14)
         plt.title(utils.dict_vars.get(cur_var)[0], fontsize=14)
         plt.ylabel(utils.dict_vars.get(cur_var)[1], fontsize=10)
         try:
             if np.all(np.isnan(df_current[cur_var].values)):
-                ax[idx // 3, idx % 3].text(0.3, 0.5, 'No within season data available yet')
+                ax[idx // 3, idx % 3].text(
+                    0.3, 0.5, "No within season data available yet"
+                )
                 continue
         except:
             breakpoint()
 
-        df_mean_vals, curr_vals, last_vals, past_vals, min_vals, max_vals = compute_stats(df_current, df_last, df_previous, cur_var, _window)
+        (
+            df_mean_vals,
+            curr_vals,
+            last_vals,
+            past_vals,
+            min_vals,
+            max_vals,
+        ) = compute_stats(df_current, df_last, df_previous, cur_var, _window)
 
-        if cur_var in ['ndvi', 'gcvi']:
+        if cur_var in ["ndvi", "gcvi"]:
             import statsmodels.api as sm
+
             lowess_sm = sm.nonparametric.lowess
-            curr_vals = lowess_sm(curr_vals, range(len(curr_vals)), frac=1./5., it=3, return_sorted=False)
-            last_vals = lowess_sm(last_vals, range(len(last_vals)), frac=1./5., it=3, return_sorted=False)
-            min_vals = lowess_sm(min_vals, range(len(min_vals)), frac=1./5., it=3, return_sorted=False)
-            max_vals = lowess_sm(max_vals, range(len(max_vals)), frac=1./5., it=3, return_sorted=False)
+            curr_vals = lowess_sm(
+                curr_vals,
+                range(len(curr_vals)),
+                frac=1.0 / 5.0,
+                it=3,
+                return_sorted=False,
+            )
+            last_vals = lowess_sm(
+                last_vals,
+                range(len(last_vals)),
+                frac=1.0 / 5.0,
+                it=3,
+                return_sorted=False,
+            )
+            min_vals = lowess_sm(
+                min_vals,
+                range(len(min_vals)),
+                frac=1.0 / 5.0,
+                it=3,
+                return_sorted=False,
+            )
+            max_vals = lowess_sm(
+                max_vals,
+                range(len(max_vals)),
+                frac=1.0 / 5.0,
+                it=3,
+                return_sorted=False,
+            )
 
         if np.isnan(curr_vals).all():
-            ax[idx // 3, idx % 3].text(0.3, 0.5, 'No within season data available yet')
+            ax[idx // 3, idx % 3].text(0.3, 0.5, "No within season data available yet")
             continue
 
         # Create nice-looking grid for ease of visualization
-        ax[idx // 3, idx % 3].grid(which='major', alpha=0.5, linestyle='--')
-        ax[idx // 3, idx % 3].grid(which='minor', alpha=0.5, linestyle='--')
+        ax[idx // 3, idx % 3].grid(which="major", alpha=0.5, linestyle="--")
+        ax[idx // 3, idx % 3].grid(which="minor", alpha=0.5, linestyle="--")
 
-        if names_cols[idx] in ['daily_precip']:
-            plt.title('Precipitation (Daily)', fontsize=14)
+        if names_cols[idx] in ["daily_precip"]:
+            plt.title("Precipitation (Daily)", fontsize=14)
 
             df_c = df_current[precip_var].resample("D").sum()
-            ax[idx // 3, idx % 3].bar(df_c.index, df_c.values, color='b', label=frcast_yr if idx == 0 else '', width=1.)
-        elif names_cols[idx] in ['cumulative_precip']:
-            plt.title('Cumulative Precipitation (vs 5 year mean)', fontsize=14)
+            ax[idx // 3, idx % 3].bar(
+                df_c.index,
+                df_c.values,
+                color="b",
+                label=frcast_yr if idx == 0 else "",
+                width=1.0,
+            )
+        elif names_cols[idx] in ["cumulative_precip"]:
+            plt.title("Cumulative Precipitation (vs 5 year mean)", fontsize=14)
 
             df_c = df_current[cur_var].cumsum()
             df_m = df_mean_vals.cumsum()
             y1 = df_c.values
             y2 = df_m.values
-            a1, = ax[idx // 3, idx % 3].plot(df_c.index, y1, color='b')
-            a9, = ax[idx // 3, idx % 3].plot(df_c.index, y2, color='k')
+            (a1,) = ax[idx // 3, idx % 3].plot(df_c.index, y1, color="b")
+            (a9,) = ax[idx // 3, idx % 3].plot(df_c.index, y2, color="k")
 
             # Plot CHIRPS_GEFS if last date in dataframe exceeds current date for CHIRPS
-            if df_c.index[-1].date() > ar.utcnow().date() and \
-                    precip_var == 'chirps' and \
-                    'chirps_gefs' in df_current.columns and \
-                    not df_current['chirps_gefs'].isnull().values.all():
+            if (
+                df_c.index[-1].date() > ar.utcnow().date()
+                and precip_var == "chirps"
+                and "chirps_gefs" in df_current.columns
+                and not df_current["chirps_gefs"].isnull().values.all()
+            ):
                 use_forecast = True
-                val_gefs = np.nanmax(df_c.values) + df_current.loc[df_current['chirps_gefs'].idxmax()]['chirps_gefs']
-
-                df_tmp = pd.DataFrame({'date': [ar.utcnow().shift(days=+15).date()], 'val': [val_gefs]})
-                df_tmp = df_tmp.set_index('date')
+                val_gefs = (
+                    np.nanmax(df_c.values)
+                    + df_current.loc[df_current["chirps_gefs"].idxmax()]["chirps_gefs"]
+                )
+
+                df_tmp = pd.DataFrame(
+                    {"date": [ar.utcnow().shift(days=+15).date()], "val": [val_gefs]}
+                )
+                df_tmp = df_tmp.set_index("date")
                 df_tmp.index = pd.to_datetime(df_tmp.index)
 
                 try:
                     mean_precip = df_m[ar.utcnow().shift(days=+15).timetuple().tm_yday]
                 except:
-                    mean_precip = df_m[ar.utcnow().shift(days=+15).timetuple().tm_yday - 1]
-                which_col = 'red' if val_gefs < mean_precip else 'green'
-                ax[idx // 3, idx % 3].plot_date(df_tmp.index, np.asarray([val_gefs]), 'o', color=which_col)
-                p4 = ax[idx // 3, idx % 3].plot(np.NaN, np.NaN, 'o', color=which_col, alpha=0.2, label='Forecast (15 day)')
-
-            ax[idx // 3, idx % 3].fill_between(df_c.index, y1, y2, where=y2 >= y1, lw=1., facecolor='red', alpha=0.2)
-            ax[idx // 3, idx % 3].fill_between(df_c.index, y1, y2, where=y2 <= y1, lw=1., facecolor='green', alpha=0.2)
-
-            p2 = ax[idx // 3, idx % 3].fill(np.NaN, np.NaN, 'red', alpha=0.2, label='< 5 year mean')
-            p3 = ax[idx // 3, idx % 3].fill(np.NaN, np.NaN, 'green', alpha=0.2, label='> 5 year mean')
-            ax[idx // 3, idx % 3].legend(loc='upper left', fontsize='small')
-        elif names_cols[idx] in ['yearly_ndvi']:
+                    mean_precip = df_m[
+                        ar.utcnow().shift(days=+15).timetuple().tm_yday - 1
+                    ]
+                which_col = "red" if val_gefs < mean_precip else "green"
+                ax[idx // 3, idx % 3].plot_date(
+                    df_tmp.index, np.asarray([val_gefs]), "o", color=which_col
+                )
+                p4 = ax[idx // 3, idx % 3].plot(
+                    np.NaN,
+                    np.NaN,
+                    "o",
+                    color=which_col,
+                    alpha=0.2,
+                    label="Forecast (15 day)",
+                )
+
+            ax[idx // 3, idx % 3].fill_between(
+                df_c.index, y1, y2, where=y2 >= y1, lw=1.0, facecolor="red", alpha=0.2
+            )
+            ax[idx // 3, idx % 3].fill_between(
+                df_c.index, y1, y2, where=y2 <= y1, lw=1.0, facecolor="green", alpha=0.2
+            )
+
+            p2 = ax[idx // 3, idx % 3].fill(
+                np.NaN, np.NaN, "red", alpha=0.2, label="< 5 year mean"
+            )
+            p3 = ax[idx // 3, idx % 3].fill(
+                np.NaN, np.NaN, "green", alpha=0.2, label="> 5 year mean"
+            )
+            ax[idx // 3, idx % 3].legend(loc="upper left", fontsize="small")
+        elif names_cols[idx] in ["yearly_ndvi"]:
             from heapq import nsmallest
             import statsmodels.api as sm
+
             lowess_sm = sm.nonparametric.lowess
 
-            closest = nsmallest(6, range(2001, max(ar.utcnow().year, frcast_yr)), key=lambda x: abs(x - frcast_yr))
+            closest = nsmallest(
+                6,
+                range(2001, max(ar.utcnow().year, frcast_yr)),
+                key=lambda x: abs(x - frcast_yr),
+            )
             closest.extend([frcast_yr])
             closest = list(set(closest))
             closest.sort()
             if len(closest) > 6:
-                closest = closest[(len(closest) - 6):]
+                closest = closest[(len(closest) - 6) :]
 
             for y in closest:
-                _cur = df[df['harvest_season'] == y]
-                _tmp = _cur['yield']
+                _cur = df[df["harvest_season"] == y]
+                _tmp = _cur["yield"]
                 if not _tmp.isnull().all():
                     _yld = np.unique(_tmp[~np.isnan(_tmp)])[0]
                 else:
                     _yld = np.NaN
-                vals = _cur['ndvi'].values
+                vals = _cur["ndvi"].values
                 vals = bn.move_mean(vals, window=_window, min_count=1)
-                vals = lowess_sm(vals, range(len(vals)), frac=1. / 5., it=3, return_sorted=False)
+                vals = lowess_sm(
+                    vals, range(len(vals)), frac=1.0 / 5.0, it=3, return_sorted=False
+                )
 
                 if y == frcast_yr:
                     if np.isnan(_yld):
-                        ax[idx // 3, idx % 3].plot(df_current.index, vals, lw=1.5, color='b', label=str(y))
+                        ax[idx // 3, idx % 3].plot(
+                            df_current.index, vals, lw=1.5, color="b", label=str(y)
+                        )
                     else:
-                        ax[idx // 3, idx % 3].plot(df_current.index, vals, lw=1.5, color='b', label=str(y) + ', ' + '{0:.2f}'.format(_yld) + ' MT/ha')
+                        ax[idx // 3, idx % 3].plot(
+                            df_current.index,
+                            vals,
+                            lw=1.5,
+                            color="b",
+                            label=str(y) + ", " + "{0:.2f}".format(_yld) + " MT/ha",
+                        )
                 else:
                     if np.isnan(_yld):
                         if y == frcast_yr - 1:
-                            ax[idx // 3, idx % 3].plot(df_current.index, vals, lw=1., alpha=0.75, color=color_list[8], label=str(y))
+                            ax[idx // 3, idx % 3].plot(
+                                df_current.index,
+                                vals,
+                                lw=1.0,
+                                alpha=0.75,
+                                color=color_list[8],
+                                label=str(y),
+                            )
                         else:
-                            ax[idx // 3, idx % 3].plot(df_current.index, vals, lw=1., alpha=0.75, label=str(y))
+                            ax[idx // 3, idx % 3].plot(
+                                df_current.index, vals, lw=1.0, alpha=0.75, label=str(y)
+                            )
                     else:
                         if y == frcast_yr - 1:
-                            ax[idx // 3, idx % 3].plot(df_current.index, vals, lw=1., alpha=0.75, color=color_list[8], label=str(y) + ', ' + '{0:.2f}'.format(_yld) + ' MT/ha')
+                            ax[idx // 3, idx % 3].plot(
+                                df_current.index,
+                                vals,
+                                lw=1.0,
+                                alpha=0.75,
+                                color=color_list[8],
+                                label=str(y) + ", " + "{0:.2f}".format(_yld) + " MT/ha",
+                            )
                         else:
-                            ax[idx // 3, idx % 3].plot(df_current.index, vals, lw=1., alpha=0.75, label=str(y) + ', ' + '{0:.2f}'.format(_yld) + ' MT/ha')
-            plt.title('Recent 5 Years NDVI Comparison', fontsize=14)
-            ax[idx // 3, idx % 3].legend(loc='upper left', fontsize='small')
-        elif names_cols[idx] in ['yearly_gcvi']:
+                            ax[idx // 3, idx % 3].plot(
+                                df_current.index,
+                                vals,
+                                lw=1.0,
+                                alpha=0.75,
+                                label=str(y) + ", " + "{0:.2f}".format(_yld) + " MT/ha",
+                            )
+            plt.title("Recent 5 Years NDVI Comparison", fontsize=14)
+            ax[idx // 3, idx % 3].legend(loc="upper left", fontsize="small")
+        elif names_cols[idx] in ["yearly_gcvi"]:
             from heapq import nsmallest
             import statsmodels.api as sm
+
             lowess_sm = sm.nonparametric.lowess
 
-            closest = nsmallest(6, range(2001, max(ar.utcnow().year, frcast_yr)), key=lambda x: abs(x - frcast_yr))
+            closest = nsmallest(
+                6,
+                range(2001, max(ar.utcnow().year, frcast_yr)),
+                key=lambda x: abs(x - frcast_yr),
+            )
             closest.extend([frcast_yr])
             closest = list(set(closest))
             closest.sort()
             if len(closest) > 6:
-                closest = closest[(len(closest) - 6):]
+                closest = closest[(len(closest) - 6) :]
 
             for y in closest:
-                _cur = df[df['harvest_season'] == y]
-                _tmp = _cur['yield']
+                _cur = df[df["harvest_season"] == y]
+                _tmp = _cur["yield"]
                 if not _tmp.isnull().all():
                     _yld = np.unique(_tmp[~np.isnan(_tmp)])[0]
                 else:
                     _yld = np.NaN
-                vals = _cur['gcvi'].values
+                vals = _cur["gcvi"].values
                 vals = bn.move_mean(vals, window=_window, min_count=1)
-                vals = lowess_sm(vals, range(len(vals)), frac=1. / 5., it=3, return_sorted=False)
+                vals = lowess_sm(
+                    vals, range(len(vals)), frac=1.0 / 5.0, it=3, return_sorted=False
+                )
 
                 if y == frcast_yr:
                     if np.isnan(_yld):
-                        ax[idx // 3, idx % 3].plot(df_current.index, vals, lw=1.5, color='b', label=str(y))
+                        ax[idx // 3, idx % 3].plot(
+                            df_current.index, vals, lw=1.5, color="b", label=str(y)
+                        )
                     else:
-                        ax[idx // 3, idx % 3].plot(df_current.index, vals, lw=1.5, color='b', label=str(y) + ', ' + '{0:.2f}'.format(_yld) + ' MT/ha')
+                        ax[idx // 3, idx % 3].plot(
+                            df_current.index,
+                            vals,
+                            lw=1.5,
+                            color="b",
+                            label=str(y) + ", " + "{0:.2f}".format(_yld) + " MT/ha",
+                        )
                 else:
                     if np.isnan(_yld):
                         if y == frcast_yr - 1:
-                            ax[idx // 3, idx % 3].plot(df_current.index, vals, lw=1., alpha=0.75, color=color_list[8], label=str(y))
+                            ax[idx // 3, idx % 3].plot(
+                                df_current.index,
+                                vals,
+                                lw=1.0,
+                                alpha=0.75,
+                                color=color_list[8],
+                                label=str(y),
+                            )
                         else:
-                            ax[idx // 3, idx % 3].plot(df_current.index, vals, lw=1., alpha=0.75, label=str(y))
+                            ax[idx // 3, idx % 3].plot(
+                                df_current.index, vals, lw=1.0, alpha=0.75, label=str(y)
+                            )
                     else:
                         if y == frcast_yr - 1:
-                            ax[idx // 3, idx % 3].plot(df_current.index, vals, lw=1., alpha=0.75, color=color_list[8], label=str(y) + ', ' + '{0:.2f}'.format(_yld) + ' MT/ha')
+                            ax[idx // 3, idx % 3].plot(
+                                df_current.index,
+                                vals,
+                                lw=1.0,
+                                alpha=0.75,
+                                color=color_list[8],
+                                label=str(y) + ", " + "{0:.2f}".format(_yld) + " MT/ha",
+                            )
                         else:
-                            ax[idx // 3, idx % 3].plot(df_current.index, vals, lw=1., alpha=0.75, label=str(y) + ', ' + '{0:.2f}'.format(_yld) + ' MT/ha')
-            plt.title('Recent 5 Years GCVI Comparison', fontsize=14)
-            ax[idx // 3, idx % 3].legend(loc='upper left', fontsize='small')
-        elif names_cols[idx] in ['cpc_tmax']:
-            plt.title('Temperature (daily mean)', fontsize=14)
+                            ax[idx // 3, idx % 3].plot(
+                                df_current.index,
+                                vals,
+                                lw=1.0,
+                                alpha=0.75,
+                                label=str(y) + ", " + "{0:.2f}".format(_yld) + " MT/ha",
+                            )
+            plt.title("Recent 5 Years GCVI Comparison", fontsize=14)
+            ax[idx // 3, idx % 3].legend(loc="upper left", fontsize="small")
+        elif names_cols[idx] in ["cpc_tmax"]:
+            plt.title("Temperature (daily mean)", fontsize=14)
 
             # Plot average_temperature
-            df_mean_vals, curr_vals, last_vals, past_vals, min_vals, max_vals = compute_stats(df_current, df_last, df_previous, 'average_temperature', _window)
+            (
+                df_mean_vals,
+                curr_vals,
+                last_vals,
+                past_vals,
+                min_vals,
+                max_vals,
+            ) = compute_stats(
+                df_current, df_last, df_previous, "average_temperature", _window
+            )
+
+            (a1,) = ax[idx // 3, idx % 3].plot(
+                df_current.index,
+                curr_vals,
+                color="b",
+                lw=1.5,
+                label=frcast_yr if idx == 0 else "",
+            )
+            (a2,) = ax[idx // 3, idx % 3].plot(
+                df_current.index,
+                last_vals,
+                color=color_list[8],
+                lw=1.25,
+                label=frcast_yr - 1 if idx == 0 else "",
+            )
+            (a3,) = ax[idx // 3, idx % 3].plot(
+                df_current.index,
+                past_vals,
+                color="k",
+                lw=1.25,
+                label="Mean" if idx == 0 else "",
+            )
+
+            a4 = ax[idx // 3, idx % 3].fill_between(
+                df_current.index,
+                min_vals,
+                max_vals,
+                color="lightgray",
+                label="Min/Max" if idx == 0 else "",
+                alpha=0.7,
+                lw=0,
+            )
 
-            a1, = ax[idx // 3, idx % 3].plot(df_current.index, curr_vals, color='b', lw=1.5, label=frcast_yr if idx == 0 else '')
-            a2, = ax[idx // 3, idx % 3].plot(df_current.index, last_vals, color=color_list[8], lw=1.25, label=frcast_yr - 1 if idx == 0 else '')
-            a3, = ax[idx // 3, idx % 3].plot(df_current.index, past_vals, color='k', lw=1.25, label='Mean' if idx == 0 else '')
-
-            a4 = ax[idx // 3, idx % 3].fill_between(df_current.index, min_vals, max_vals, color='lightgray', label='Min/Max' if idx == 0 else '',
-                                                    alpha=0.7, lw=0)
-
-            mask_max = df_current['cpc_tmax'] > 30
-            mask_min = df_current['cpc_tmin'] < 5
+            mask_max = df_current["cpc_tmax"] > 30
+            mask_min = df_current["cpc_tmin"] < 5
 
             # Plot temperatures that fall above or below the GDD threshold
-            p2 = ax[idx // 3, idx % 3].plot(df_current.index[mask_max], df_current[mask_max]['cpc_tmax'], 'ro', markersize=2, label='Max temp > 30°C')
-            p3 = ax[idx // 3, idx % 3].plot(df_current.index[mask_min], df_current[mask_min]['cpc_tmin'], 'co', markersize=2, label='Min temp < 5°C')
+            p2 = ax[idx // 3, idx % 3].plot(
+                df_current.index[mask_max],
+                df_current[mask_max]["cpc_tmax"],
+                "ro",
+                markersize=2,
+                label="Max temp > 30°C",
+            )
+            p3 = ax[idx // 3, idx % 3].plot(
+                df_current.index[mask_min],
+                df_current[mask_min]["cpc_tmin"],
+                "co",
+                markersize=2,
+                label="Min temp < 5°C",
+            )
 
-            ax[idx // 3, idx % 3].legend(loc='upper left', fontsize='small')
+            ax[idx // 3, idx % 3].legend(loc="upper left", fontsize="small")
         else:
             # Plot mean value
-            a1, = ax[idx // 3, idx % 3].plot(df_current.index, curr_vals, color='b', lw=1.5, label=frcast_yr if idx == 0 else '')
-            a2, = ax[idx // 3, idx % 3].plot(df_current.index, last_vals, color=color_list[8], lw=1.25, label=frcast_yr-1 if idx == 0 else '')
-            a3, = ax[idx // 3, idx % 3].plot(df_current.index, past_vals, color='k', lw=1.25, label='Mean' if idx == 0 else '')
+            (a1,) = ax[idx // 3, idx % 3].plot(
+                df_current.index,
+                curr_vals,
+                color="b",
+                lw=1.5,
+                label=frcast_yr if idx == 0 else "",
+            )
+            (a2,) = ax[idx // 3, idx % 3].plot(
+                df_current.index,
+                last_vals,
+                color=color_list[8],
+                lw=1.25,
+                label=frcast_yr - 1 if idx == 0 else "",
+            )
+            (a3,) = ax[idx // 3, idx % 3].plot(
+                df_current.index,
+                past_vals,
+                color="k",
+                lw=1.25,
+                label="Mean" if idx == 0 else "",
+            )
             # a9, = ax[idx // 3, idx % 3].plot(df_current.index, new_past_vals, color='b', linestyle='-.', lw=1.25, label='Mean' if idx == 0 else '')
 
-            a4 = ax[idx // 3, idx % 3].fill_between(df_current.index, min_vals, max_vals, color='lightgray', label='Min/Max' if idx == 0 else '', alpha=0.7, lw=0)
+            a4 = ax[idx // 3, idx % 3].fill_between(
+                df_current.index,
+                min_vals,
+                max_vals,
+                color="lightgray",
+                label="Min/Max" if idx == 0 else "",
+                alpha=0.7,
+                lw=0,
+            )
 
         if dates_cal:
             if dates_cal[0]:
-                a5 = ax[idx // 3, idx % 3].axvline(dates_cal[0], color=color_list[10], label='Planting', lw=1.5, linestyle='--')
+                a5 = ax[idx // 3, idx % 3].axvline(
+                    dates_cal[0],
+                    color=color_list[10],
+                    label="Planting",
+                    lw=1.5,
+                    linestyle="--",
+                )
 
             if dates_cal[1]:
-                a6 = ax[idx // 3, idx % 3].axvline(dates_cal[1], color=color_list[4], label='Greenup', lw=1.5)
+                a6 = ax[idx // 3, idx % 3].axvline(
+                    dates_cal[1], color=color_list[4], label="Greenup", lw=1.5
+                )
 
             if dates_cal[2]:
-                a7 = ax[idx // 3, idx % 3].axvline(dates_cal[2], color='darkgoldenrod', label='Senescence', lw=1.5)
+                a7 = ax[idx // 3, idx % 3].axvline(
+                    dates_cal[2], color="darkgoldenrod", label="Senescence", lw=1.5
+                )
 
             if dates_cal[3]:
-                a8 = ax[idx // 3, idx % 3].axvline(dates_cal[3], color=color_list[6], label='Harvest', lw=1.5, linestyle='--')
+                a8 = ax[idx // 3, idx % 3].axvline(
+                    dates_cal[3],
+                    color=color_list[6],
+                    label="Harvest",
+                    lw=1.5,
+                    linestyle="--",
+                )
 
         # Create a legend with transparent box around it (inside first subplot)
         # leg = ax[idx // 3, idx % 3].legend(loc='upper left', fancybox=None, prop={'size': 'large'}, ncol=2)
         # leg.get_frame().set_linewidth(0.0)  # remove only the border of the box of the legend
 
     # Plot legend outside of subplots
     if dates_cal:
         # all_labels = [str(frcast_yr), 'Median Analog years (OND 2021)', str(frcast_yr - 1), '5 year Mean', '10 year Min/Max', 'Planting', 'Greenup', 'Senescence', 'Harvest']
         # leg = plt.figlegend([a1, a9, a2, a3, a4, a5, a6, a7, a8], all_labels, loc='lower center', bbox_to_anchor=[0.76, 0.06])
-        all_labels = [str(frcast_yr), str(frcast_yr - 1), '5 year Mean', '10 year Min/Max', 'Planting', 'Greenup', 'Senescence', 'Harvest']
-        leg = plt.figlegend([a1, a2, a3, a4, a5, a6, a7, a8], all_labels, loc='lower center', bbox_to_anchor=[0.76, 0.06])
+        all_labels = [
+            str(frcast_yr),
+            str(frcast_yr - 1),
+            "5 year Mean",
+            "10 year Min/Max",
+            "Planting",
+            "Greenup",
+            "Senescence",
+            "Harvest",
+        ]
+        leg = plt.figlegend(
+            [a1, a2, a3, a4, a5, a6, a7, a8],
+            all_labels,
+            loc="lower center",
+            bbox_to_anchor=[0.76, 0.06],
+        )
     else:
-        all_labels = [str(frcast_yr), '5 year Mean', '5 year Min/Max']
-        leg = plt.figlegend([a1, a2, a3], all_labels, loc='lower center', bbox_to_anchor=[0.76, 0.06])
+        all_labels = [str(frcast_yr), "5 year Mean", "5 year Min/Max"]
+        leg = plt.figlegend(
+            [a1, a2, a3], all_labels, loc="lower center", bbox_to_anchor=[0.76, 0.06]
+        )
 
     # Add Harvest and GEOGLAM logos
     import matplotlib.image as image
+
     im = image.imread(str(logos[0]))
     fig.figimage(im, 3800, 2270, zorder=3)
     im = image.imread(str(logos[1]))
     fig.figimage(im, 4100, 2300, zorder=3)
 
     # TODO: Should be updated every time a new data source is added or previous one deleted or modified
-    fig.text(0.83, 0.25, 'Data Sources\n', fontsize=14, fontweight='bold')
-    precip_var = 'chirps' if 'chirps' in df.columns.values else 'cpc_precip'
-    precip_str = 'Precipitation: CHIRPS\n' if precip_var == 'chirps' else 'Precipitation: NOAA CPC\n'
+    fig.text(0.83, 0.25, "Data Sources\n", fontsize=14, fontweight="bold")
+    precip_var = "chirps" if "chirps" in df.columns.values else "cpc_precip"
+    precip_str = (
+        "Precipitation: CHIRPS\n"
+        if precip_var == "chirps"
+        else "Precipitation: NOAA CPC\n"
+    )
     if use_forecast:
-        precip_str += 'Precipitation Forecast: CHIRPS-GEFS\n'
-    if precip_var == 'chirps':
-        fig.text(0.83, 0.14,
-                 'NDVI: UMD GLAM system\n' +
-                 'Temperature: NOAA CPC\n' +
-                 precip_str +
-                 'Evaporative Stress Index: NASA ESI\n' +
-                 'Soil Moisture: NASA-USDA Global Soil Moisture\n',
-                 # 'Growing degree days: NOAA CPC temperature',
-                 linespacing=1.5)
+        precip_str += "Precipitation Forecast: CHIRPS-GEFS\n"
+    if precip_var == "chirps":
+        fig.text(
+            0.83,
+            0.14,
+            "NDVI: UMD GLAM system\n"
+            + "Temperature: NOAA CPC\n"
+            + precip_str
+            + "Evaporative Stress Index: NASA ESI\n"
+            + "Soil Moisture: NASA-USDA Global Soil Moisture\n",
+            # 'Growing degree days: NOAA CPC temperature',
+            linespacing=1.5,
+        )
     else:
-        fig.text(0.83, 0.15,
-                 'NDVI: UMD GLAM system\n' +
-                 'Temperature: NOAA CPC\n' +
-                 precip_str +
-                 'Evaporative Stress Index: NASA ESI\n' +
-                 'Soil Moisture: NASA-USDA Global Soil Moisture\n',
-                 # 'Growing degree days: NOAA CPC temperature',
-                 linespacing=1.5)
-
-    fig.text(0.67, 0.04, r'$\blacktriangleright$ Crop growth stage dates are based on the 5 year average GEOGLAM best available crop calendars', fontsize=9)
-    fig.text(0.91, 0.02, f"Produced on: {ar.utcnow().format('MMM DD YYYY')}", fontsize=9)
+        fig.text(
+            0.83,
+            0.15,
+            "NDVI: UMD GLAM system\n"
+            + "Temperature: NOAA CPC\n"
+            + precip_str
+            + "Evaporative Stress Index: NASA ESI\n"
+            + "Soil Moisture: NASA-USDA Global Soil Moisture\n",
+            # 'Growing degree days: NOAA CPC temperature',
+            linespacing=1.5,
+        )
+
+    fig.text(
+        0.67,
+        0.04,
+        r"$\blacktriangleright$ Crop growth stage dates are based on the 5 year average GEOGLAM best available crop calendars",
+        fontsize=9,
+    )
+    fig.text(
+        0.91, 0.02, f"Produced on: {ar.utcnow().format('MMM DD YYYY')}", fontsize=9
+    )
 
-    leg.get_frame().set_facecolor('none')
-    leg.set_title('Legend', prop={'size': 14, 'weight': 'heavy'})
+    leg.get_frame().set_facecolor("none")
+    leg.set_title("Legend", prop={"size": 14, "weight": "heavy"})
     leg.get_frame().set_linewidth(0.0)
-    leg._legend_box.align = 'left'
+    leg._legend_box.align = "left"
 
     # Final layout adjustment and output
     plt.tight_layout()
     plt.subplots_adjust(top=0.88)
 
     plt.savefig(dir_out / fname, dpi=constants.DPI)
     plt.close()
```

### Comparing `geocif-0.0.1/setup.py` & `geocif-0.1.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,55 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-import io
-from os import path as op
-from setuptools import setup, find_packages
-
-with open('README.md') as readme_file:
-    readme = readme_file.read()
-
-here = op.abspath(op.dirname(__file__))
-
-# get the dependencies and installs
-with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
-    all_reqs = f.read().split("\n")
-
-install_requires = [x.strip() for x in all_reqs if "git+" not in x]
-dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
-
-requirements = [ ]
-
-setup_requirements = [ ]
-
-test_requirements = [ ]
-
-setup(
-    author="Ritvik Sahajpal",
-    author_email='ritvik@umd.edu',
-    python_requires='>=3.7',
-    classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-    ],
-    description="Models to visualize and forecast crop conditions and yields",
-    install_requires=install_requires,
-    dependency_links=dependency_links,
-    license="MIT license",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    include_package_data=True,
-    keywords='geocif',
-    name='geocif',
-    packages=find_packages(include=['geocif', 'geocif.*']),
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/ritviksahajpal/geocif',
-    version='0.0.1',
-    zip_safe=False,
-)
+#!/usr/bin/env python
+
+"""The setup script."""
+
+import io
+from os import path as op
+from setuptools import setup, find_packages
+
+with open('README.md') as readme_file:
+    readme = readme_file.read()
+
+here = op.abspath(op.dirname(__file__))
+
+# get the dependencies and installs
+with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
+    all_reqs = f.read().split("\n")
+
+install_requires = [x.strip() for x in all_reqs if "git+" not in x]
+dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
+
+requirements = [ ]
+
+setup_requirements = [ ]
+
+test_requirements = [ ]
+
+setup(
+    author="Ritvik Sahajpal",
+    author_email='ritvik@umd.edu',
+    python_requires='>=3.9',
+    classifiers=[
+        'Development Status :: 2 - Pre-Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.9',
+    ],
+    description="Models to visualize and forecast crop conditions and yields",
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="MIT license",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    include_package_data=True,
+    keywords='geocif',
+    name='geocif',
+    packages=find_packages(include=['geocif', 'geocif.*']),
+    setup_requires=setup_requirements,
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://ritviksahajpal.github.io/yield_forecasting/',
+    version='0.1.2',
+    zip_safe=False,
+)
```

