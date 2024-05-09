# Comparing `tmp/pyearth-0.1.8.tar.gz` & `tmp/pyearth-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyearth-0.1.8.tar", last modified: Wed Feb 23 03:42:19 2022, max compression
+gzip compressed data, was "pyearth-0.1.9.tar", last modified: Thu Feb 24 07:27:30 2022, max compression
```

## Comparing `pyearth-0.1.8.tar` & `pyearth-0.1.9.tar`

### file list

```diff
@@ -1,128 +1,132 @@
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:19.819013 pyearth-0.1.8/
--rw-r--r--   0 liao313  (231954) users      (100)     1071 2021-04-06 17:36:32.000000 pyearth-0.1.8/LICENSE.md
--rw-r--r--   0 liao313  (231954) users      (100)       59 2021-04-05 18:59:06.000000 pyearth-0.1.8/MANIFEST.in
--rw-r--r--   0 liao313  (231954) users      (100)     2243 2022-02-23 03:42:19.824177 pyearth-0.1.8/PKG-INFO
--rw-r--r--   0 liao313  (231954) users      (100)     1556 2022-02-16 17:46:11.000000 pyearth-0.1.8/README.md
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:16.989410 pyearth-0.1.8/pyearth/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-10-13 20:17:13.000000 pyearth-0.1.8/pyearth/__init__.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:17.173850 pyearth-0.1.8/pyearth/gis/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-08-07 02:54:45.000000 pyearth-0.1.8/pyearth/gis/__init__.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:17.212963 pyearth-0.1.8/pyearth/gis/cartopy/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-08-07 02:54:45.000000 pyearth-0.1.8/pyearth/gis/cartopy/__init__.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:17.260640 pyearth-0.1.8/pyearth/gis/envi/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-08-07 02:54:45.000000 pyearth-0.1.8/pyearth/gis/envi/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     1973 2022-02-01 00:30:22.000000 pyearth-0.1.8/pyearth/gis/envi/envi_write_header.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:17.340987 pyearth-0.1.8/pyearth/gis/gdal/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-08-07 02:54:45.000000 pyearth-0.1.8/pyearth/gis/gdal/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     5923 2022-02-01 20:01:01.000000 pyearth-0.1.8/pyearth/gis/gdal/gdal_function.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:17.429089 pyearth-0.1.8/pyearth/gis/gdal/read/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:12:41.000000 pyearth-0.1.8/pyearth/gis/gdal/read/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     3873 2022-02-01 00:30:16.000000 pyearth-0.1.8/pyearth/gis/gdal/read/gdal_read_envi_file.py
--rw-r--r--   0 liao313  (231954) users      (100)     4182 2022-02-01 00:30:12.000000 pyearth-0.1.8/pyearth/gis/gdal/read/gdal_read_geotiff_file.py
--rw-r--r--   0 liao313  (231954) users      (100)     1456 2022-02-01 00:30:49.000000 pyearth-0.1.8/pyearth/gis/gdal/read/gdal_read_shapefile.py
--rw-r--r--   0 liao313  (231954) users      (100)      658 2022-02-01 20:07:01.000000 pyearth-0.1.8/pyearth/gis/gdal/world2Pixel.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:17.508278 pyearth-0.1.8/pyearth/gis/gdal/write/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:12:43.000000 pyearth-0.1.8/pyearth/gis/gdal/write/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     4149 2022-02-01 17:23:42.000000 pyearth-0.1.8/pyearth/gis/gdal/write/gdal_write_envi_file.py
--rw-r--r--   0 liao313  (231954) users      (100)     3988 2022-02-01 17:33:47.000000 pyearth-0.1.8/pyearth/gis/gdal/write/gdal_write_geotiff_file.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:17.629122 pyearth-0.1.8/pyearth/gis/location/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2021-05-20 16:20:42.000000 pyearth-0.1.8/pyearth/gis/location/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     1197 2022-02-01 20:19:00.000000 pyearth-0.1.8/pyearth/gis/location/calculate_distance_based_on_lon_lat.py
--rw-r--r--   0 liao313  (231954) users      (100)     3257 2022-02-09 19:13:56.000000 pyearth-0.1.8/pyearth/gis/location/calculate_polygon_area.py
--rw-r--r--   0 liao313  (231954) users      (100)      768 2022-02-01 20:24:45.000000 pyearth-0.1.8/pyearth/gis/location/convert_lat_lon_range.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:17.703179 pyearth-0.1.8/pyearth/system/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-10-13 20:17:24.000000 pyearth-0.1.8/pyearth/system/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     1219 2022-02-01 00:06:02.000000 pyearth-0.1.8/pyearth/system/define_global_variables.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:17.715906 pyearth-0.1.8/pyearth/toolbox/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:39:46.000000 pyearth-0.1.8/pyearth/toolbox/__init__.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:17.883021 pyearth-0.1.8/pyearth/toolbox/data/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:27:11.000000 pyearth-0.1.8/pyearth/toolbox/data/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)      420 2022-02-01 20:39:42.000000 pyearth-0.1.8/pyearth/toolbox/data/check_if_duplicates.py
--rw-r--r--   0 liao313  (231954) users      (100)     3922 2022-02-17 18:51:08.000000 pyearth-0.1.8/pyearth/toolbox/data/convert_time_series_daily_to_monthly.py
--rw-r--r--   0 liao313  (231954) users      (100)      849 2022-02-01 21:17:57.000000 pyearth-0.1.8/pyearth/toolbox/data/remove_outliers.py
--rw-r--r--   0 liao313  (231954) users      (100)       29 2022-02-23 03:27:29.000000 pyearth-0.1.8/pyearth/toolbox/data/shift_array.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:18.050866 pyearth-0.1.8/pyearth/toolbox/date/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:27:08.000000 pyearth-0.1.8/pyearth/toolbox/date/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)      721 2022-02-17 18:50:33.000000 pyearth-0.1.8/pyearth/toolbox/date/day_in_month.py
--rw-r--r--   0 liao313  (231954) users      (100)     1138 2022-02-01 21:49:45.000000 pyearth-0.1.8/pyearth/toolbox/date/day_of_year.py
--rw-r--r--   0 liao313  (231954) users      (100)     1009 2020-06-09 22:29:48.000000 pyearth-0.1.8/pyearth/toolbox/date/dt2cal.py
--rw-r--r--   0 liao313  (231954) users      (100)      352 2022-02-01 21:50:54.000000 pyearth-0.1.8/pyearth/toolbox/date/leap_year.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:18.112546 pyearth-0.1.8/pyearth/toolbox/geometry/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:28:48.000000 pyearth-0.1.8/pyearth/toolbox/geometry/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)      301 2022-02-01 21:51:46.000000 pyearth-0.1.8/pyearth/toolbox/geometry/calculate_hexagon_area.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:18.167965 pyearth-0.1.8/pyearth/toolbox/math/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:28:52.000000 pyearth-0.1.8/pyearth/toolbox/math/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     2708 2022-02-02 00:05:05.000000 pyearth-0.1.8/pyearth/toolbox/math/gap_fill_by_window.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:18.201252 pyearth-0.1.8/pyearth/toolbox/math/stat/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2021-04-16 20:49:09.000000 pyearth-0.1.8/pyearth/toolbox/math/stat/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     1942 2022-02-01 23:56:15.000000 pyearth-0.1.8/pyearth/toolbox/math/stat/scipy_bivariate_kde.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:18.417871 pyearth-0.1.8/pyearth/toolbox/reader/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-07-12 05:05:01.000000 pyearth-0.1.8/pyearth/toolbox/reader/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)      466 2022-02-02 00:05:56.000000 pyearth-0.1.8/pyearth/toolbox/reader/line_count.py
--rw-r--r--   0 liao313  (231954) users      (100)     2267 2022-02-02 00:21:44.000000 pyearth-0.1.8/pyearth/toolbox/reader/parse_xml_file.py
--rw-r--r--   0 liao313  (231954) users      (100)      815 2022-02-02 00:23:27.000000 pyearth-0.1.8/pyearth/toolbox/reader/read_configuration_file.py
--rw-r--r--   0 liao313  (231954) users      (100)      589 2022-02-02 00:26:53.000000 pyearth-0.1.8/pyearth/toolbox/reader/split_string_into_chunk.py
--rw-r--r--   0 liao313  (231954) users      (100)     5486 2022-02-02 00:20:25.000000 pyearth-0.1.8/pyearth/toolbox/reader/text_reader_string.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:18.558876 pyearth-0.1.8/pyearth/toolbox/slurm/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:29:08.000000 pyearth-0.1.8/pyearth/toolbox/slurm/__init__.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:18.577099 pyearth-0.1.8/pyearth/toolbox/slurm/mpi/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:29:16.000000 pyearth-0.1.8/pyearth/toolbox/slurm/mpi/__init__.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:18.652631 pyearth-0.1.8/pyearth/toolbox/slurm/parafly/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:29:11.000000 pyearth-0.1.8/pyearth/toolbox/slurm/parafly/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     1258 2022-02-02 17:24:19.000000 pyearth-0.1.8/pyearth/toolbox/slurm/parafly/prepare_parafly_python_command_file.py
--rw-r--r--   0 liao313  (231954) users      (100)     3875 2022-02-02 17:28:47.000000 pyearth-0.1.8/pyearth/toolbox/slurm/parafly/prepare_parafly_slurm_job_script.py
--rw-r--r--   0 liao313  (231954) users      (100)     4502 2022-02-02 17:37:38.000000 pyearth-0.1.8/pyearth/toolbox/slurm/slurm_prepare_job_script_python.py
--rw-r--r--   0 liao313  (231954) users      (100)     5441 2022-02-02 17:37:10.000000 pyearth-0.1.8/pyearth/toolbox/slurm/slurm_prepare_job_script_python_checkpoint.py
--rw-r--r--   0 liao313  (231954) users      (100)      683 2022-02-02 00:40:32.000000 pyearth-0.1.8/pyearth/toolbox/slurm/slurm_update_checkpoint_file.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:18.737320 pyearth-0.1.8/pyearth/visual/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-12-05 18:41:52.000000 pyearth-0.1.8/pyearth/visual/__init__.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:18.877687 pyearth-0.1.8/pyearth/visual/barplot/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2020-12-22 05:55:12.000000 pyearth-0.1.8/pyearth/visual/barplot/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     4208 2021-04-19 17:01:35.000000 pyearth-0.1.8/pyearth/visual/barplot/barplot_data.py
--rw-r--r--   0 liao313  (231954) users      (100)     4908 2022-02-13 19:34:12.000000 pyearth-0.1.8/pyearth/visual/barplot/barplot_data_with_reference.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:19.017964 pyearth-0.1.8/pyearth/visual/color/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:15:36.000000 pyearth-0.1.8/pyearth/visual/color/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     2953 2021-05-24 22:04:07.000000 pyearth-0.1.8/pyearth/visual/color/choose_n_color.py
--rw-r--r--   0 liao313  (231954) users      (100)     3229 2021-08-20 22:11:01.000000 pyearth-0.1.8/pyearth/visual/color/create_diverge_rgb_color_hex.py
--rw-r--r--   0 liao313  (231954) users      (100)     3547 2021-04-19 17:08:52.000000 pyearth-0.1.8/pyearth/visual/color/create_qualitative_rgb_color_hex.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:19.081138 pyearth-0.1.8/pyearth/visual/histogram/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2020-05-04 17:07:18.000000 pyearth-0.1.8/pyearth/visual/histogram/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     3019 2021-04-19 17:22:06.000000 pyearth-0.1.8/pyearth/visual/histogram/histogram_plot.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:19.168473 pyearth-0.1.8/pyearth/visual/map/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2021-05-24 21:15:02.000000 pyearth-0.1.8/pyearth/visual/map/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     3072 2021-12-10 18:20:20.000000 pyearth-0.1.8/pyearth/visual/map/map_raster_data.py
--rw-r--r--   0 liao313  (231954) users      (100)     8775 2022-02-15 21:33:55.000000 pyearth-0.1.8/pyearth/visual/plot_xy_data.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:19.302730 pyearth-0.1.8/pyearth/visual/scatter/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:15:44.000000 pyearth-0.1.8/pyearth/visual/scatter/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     1480 2021-01-17 02:59:12.000000 pyearth-0.1.8/pyearth/visual/scatter/scatter_lowess.py
--rw-r--r--   0 liao313  (231954) users      (100)    10975 2021-12-10 18:20:19.000000 pyearth-0.1.8/pyearth/visual/scatter/scatter_plot_data.py
--rw-r--r--   0 liao313  (231954) users      (100)    10404 2021-04-19 17:40:51.000000 pyearth-0.1.8/pyearth/visual/scatter/scatter_plot_data_density.py
--rw-r--r--   0 liao313  (231954) users      (100)    12203 2022-02-17 19:26:36.000000 pyearth-0.1.8/pyearth/visual/scatter/scatter_plot_multiple_data.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:19.369619 pyearth-0.1.8/pyearth/visual/surface/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2020-04-20 23:57:01.000000 pyearth-0.1.8/pyearth/visual/surface/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     4533 2021-04-19 17:44:41.000000 pyearth-0.1.8/pyearth/visual/surface/convert_array_to_vtk_polygon.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:19.501389 pyearth-0.1.8/pyearth/visual/timeseries/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-12-05 18:41:42.000000 pyearth-0.1.8/pyearth/visual/timeseries/__init__.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:19.560809 pyearth-0.1.8/pyearth/visual/timeseries/analysis/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:15:56.000000 pyearth-0.1.8/pyearth/visual/timeseries/analysis/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     7980 2022-02-16 00:23:55.000000 pyearth-0.1.8/pyearth/visual/timeseries/analysis/plot_time_series_analysis.py
--rw-r--r--   0 liao313  (231954) users      (100)      881 2021-04-07 20:21:45.000000 pyearth-0.1.8/pyearth/visual/timeseries/calculate_ticks_space.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:19.731140 pyearth-0.1.8/pyearth/visual/timeseries/fill/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:15:55.000000 pyearth-0.1.8/pyearth/visual/timeseries/fill/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     5714 2021-04-16 16:05:07.000000 pyearth-0.1.8/pyearth/visual/timeseries/fill/plot3d_time_series_data_fill.py
--rw-r--r--   0 liao313  (231954) users      (100)     4935 2021-04-16 16:04:59.000000 pyearth-0.1.8/pyearth/visual/timeseries/fill/plot_time_series_data_monthly_fill.py
--rw-r--r--   0 liao313  (231954) users      (100)     5727 2021-04-16 16:05:03.000000 pyearth-0.1.8/pyearth/visual/timeseries/fill/plot_time_series_data_multiple_temporal_resolution_fill.py
--rw-r--r--   0 liao313  (231954) users      (100)     9169 2021-05-24 22:14:46.000000 pyearth-0.1.8/pyearth/visual/timeseries/plot_time_series_data.py
--rw-r--r--   0 liao313  (231954) users      (100)     6099 2021-04-19 17:47:11.000000 pyearth-0.1.8/pyearth/visual/timeseries/plot_time_series_data_with_two_y_axis.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:19.796794 pyearth-0.1.8/pyearth/visual/timeseries/zoom/
--rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:15:52.000000 pyearth-0.1.8/pyearth/visual/timeseries/zoom/__init__.py
--rw-r--r--   0 liao313  (231954) users      (100)     5744 2021-04-19 17:47:39.000000 pyearth-0.1.8/pyearth/visual/timeseries/zoom/plot_time_series_data_monthly_fill_with_zoom.py
-drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:42:17.144966 pyearth-0.1.8/pyearth.egg-info/
--rw-r--r--   0 liao313  (231954) users      (100)     2243 2022-02-23 03:42:15.000000 pyearth-0.1.8/pyearth.egg-info/PKG-INFO
--rw-r--r--   0 liao313  (231954) users      (100)     3904 2022-02-23 03:42:15.000000 pyearth-0.1.8/pyearth.egg-info/SOURCES.txt
--rw-r--r--   0 liao313  (231954) users      (100)        1 2022-02-23 03:42:15.000000 pyearth-0.1.8/pyearth.egg-info/dependency_links.txt
--rw-r--r--   0 liao313  (231954) users      (100)       69 2022-02-23 03:42:15.000000 pyearth-0.1.8/pyearth.egg-info/requires.txt
--rw-r--r--   0 liao313  (231954) users      (100)        8 2022-02-23 03:42:15.000000 pyearth-0.1.8/pyearth.egg-info/top_level.txt
--rw-r--r--   0 liao313  (231954) users      (100)      103 2021-04-05 21:04:48.000000 pyearth-0.1.8/pyproject.toml
--rw-r--r--   0 liao313  (231954) users      (100)      378 2022-02-23 03:42:19.849929 pyearth-0.1.8/setup.cfg
--rw-r--r--   0 liao313  (231954) users      (100)     1448 2022-02-23 03:42:08.000000 pyearth-0.1.8/setup.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.554901 pyearth-0.1.9/
+-rw-r--r--   0 liao313  (231954) users      (100)     1071 2021-04-06 17:36:32.000000 pyearth-0.1.9/LICENSE.md
+-rw-r--r--   0 liao313  (231954) users      (100)       59 2021-04-05 18:59:06.000000 pyearth-0.1.9/MANIFEST.in
+-rw-r--r--   0 liao313  (231954) users      (100)     2243 2022-02-24 07:27:30.559553 pyearth-0.1.9/PKG-INFO
+-rw-r--r--   0 liao313  (231954) users      (100)     1556 2022-02-16 17:46:11.000000 pyearth-0.1.9/README.md
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:29.611227 pyearth-0.1.9/pyearth/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-10-13 20:17:13.000000 pyearth-0.1.9/pyearth/__init__.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:29.706804 pyearth-0.1.9/pyearth/gis/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-08-07 02:54:45.000000 pyearth-0.1.9/pyearth/gis/__init__.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:29.716360 pyearth-0.1.9/pyearth/gis/cartopy/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-08-07 02:54:45.000000 pyearth-0.1.9/pyearth/gis/cartopy/__init__.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:29.731789 pyearth-0.1.9/pyearth/gis/envi/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-08-07 02:54:45.000000 pyearth-0.1.9/pyearth/gis/envi/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     1973 2022-02-01 00:30:22.000000 pyearth-0.1.9/pyearth/gis/envi/envi_write_header.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:29.760541 pyearth-0.1.9/pyearth/gis/gdal/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-08-07 02:54:45.000000 pyearth-0.1.9/pyearth/gis/gdal/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     5923 2022-02-01 20:01:01.000000 pyearth-0.1.9/pyearth/gis/gdal/gdal_function.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:29.801284 pyearth-0.1.9/pyearth/gis/gdal/read/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:12:41.000000 pyearth-0.1.9/pyearth/gis/gdal/read/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     3873 2022-02-01 00:30:16.000000 pyearth-0.1.9/pyearth/gis/gdal/read/gdal_read_envi_file.py
+-rw-r--r--   0 liao313  (231954) users      (100)     4182 2022-02-01 00:30:12.000000 pyearth-0.1.9/pyearth/gis/gdal/read/gdal_read_geotiff_file.py
+-rw-r--r--   0 liao313  (231954) users      (100)     1456 2022-02-01 00:30:49.000000 pyearth-0.1.9/pyearth/gis/gdal/read/gdal_read_shapefile.py
+-rw-r--r--   0 liao313  (231954) users      (100)      658 2022-02-01 20:07:01.000000 pyearth-0.1.9/pyearth/gis/gdal/world2Pixel.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:29.830143 pyearth-0.1.9/pyearth/gis/gdal/write/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:12:43.000000 pyearth-0.1.9/pyearth/gis/gdal/write/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     4149 2022-02-01 17:23:42.000000 pyearth-0.1.9/pyearth/gis/gdal/write/gdal_write_envi_file.py
+-rw-r--r--   0 liao313  (231954) users      (100)     3988 2022-02-01 17:33:47.000000 pyearth-0.1.9/pyearth/gis/gdal/write/gdal_write_geotiff_file.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:29.876660 pyearth-0.1.9/pyearth/gis/location/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2021-05-20 16:20:42.000000 pyearth-0.1.9/pyearth/gis/location/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     1197 2022-02-01 20:19:00.000000 pyearth-0.1.9/pyearth/gis/location/calculate_distance_based_on_lon_lat.py
+-rw-r--r--   0 liao313  (231954) users      (100)     3257 2022-02-09 19:13:56.000000 pyearth-0.1.9/pyearth/gis/location/calculate_polygon_area.py
+-rw-r--r--   0 liao313  (231954) users      (100)      768 2022-02-01 20:24:45.000000 pyearth-0.1.9/pyearth/gis/location/convert_lat_lon_range.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:29.896174 pyearth-0.1.9/pyearth/system/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-10-13 20:17:24.000000 pyearth-0.1.9/pyearth/system/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     1219 2022-02-01 00:06:02.000000 pyearth-0.1.9/pyearth/system/define_global_variables.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:29.905634 pyearth-0.1.9/pyearth/toolbox/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:39:46.000000 pyearth-0.1.9/pyearth/toolbox/__init__.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:29.950242 pyearth-0.1.9/pyearth/toolbox/data/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:27:11.000000 pyearth-0.1.9/pyearth/toolbox/data/__init__.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:29.978324 pyearth-0.1.9/pyearth/toolbox/data/beta/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-24 06:53:23.000000 pyearth-0.1.9/pyearth/toolbox/data/beta/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     1872 2022-02-24 07:22:03.000000 pyearth-0.1.9/pyearth/toolbox/data/beta/add_variable_to_netcdf.py
+-rw-r--r--   0 liao313  (231954) users      (100)     1736 2022-02-24 07:00:47.000000 pyearth-0.1.9/pyearth/toolbox/data/beta/replace_variable_in_netcdf.py
+-rw-r--r--   0 liao313  (231954) users      (100)      420 2022-02-01 20:39:42.000000 pyearth-0.1.9/pyearth/toolbox/data/check_if_duplicates.py
+-rw-r--r--   0 liao313  (231954) users      (100)     3922 2022-02-17 18:51:08.000000 pyearth-0.1.9/pyearth/toolbox/data/convert_time_series_daily_to_monthly.py
+-rw-r--r--   0 liao313  (231954) users      (100)      849 2022-02-01 21:17:57.000000 pyearth-0.1.9/pyearth/toolbox/data/remove_outliers.py
+-rw-r--r--   0 liao313  (231954) users      (100)       29 2022-02-23 03:27:29.000000 pyearth-0.1.9/pyearth/toolbox/data/shift_array.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.025231 pyearth-0.1.9/pyearth/toolbox/date/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:27:08.000000 pyearth-0.1.9/pyearth/toolbox/date/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)      721 2022-02-17 18:50:33.000000 pyearth-0.1.9/pyearth/toolbox/date/day_in_month.py
+-rw-r--r--   0 liao313  (231954) users      (100)     1138 2022-02-01 21:49:45.000000 pyearth-0.1.9/pyearth/toolbox/date/day_of_year.py
+-rw-r--r--   0 liao313  (231954) users      (100)     1009 2020-06-09 22:29:48.000000 pyearth-0.1.9/pyearth/toolbox/date/dt2cal.py
+-rw-r--r--   0 liao313  (231954) users      (100)      352 2022-02-01 21:50:54.000000 pyearth-0.1.9/pyearth/toolbox/date/leap_year.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.041932 pyearth-0.1.9/pyearth/toolbox/geometry/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:28:48.000000 pyearth-0.1.9/pyearth/toolbox/geometry/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)      301 2022-02-01 21:51:46.000000 pyearth-0.1.9/pyearth/toolbox/geometry/calculate_hexagon_area.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.059043 pyearth-0.1.9/pyearth/toolbox/math/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:28:52.000000 pyearth-0.1.9/pyearth/toolbox/math/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     2708 2022-02-02 00:05:05.000000 pyearth-0.1.9/pyearth/toolbox/math/gap_fill_by_window.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.077242 pyearth-0.1.9/pyearth/toolbox/math/stat/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2021-04-16 20:49:09.000000 pyearth-0.1.9/pyearth/toolbox/math/stat/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     1942 2022-02-01 23:56:15.000000 pyearth-0.1.9/pyearth/toolbox/math/stat/scipy_bivariate_kde.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.134009 pyearth-0.1.9/pyearth/toolbox/reader/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-07-12 05:05:01.000000 pyearth-0.1.9/pyearth/toolbox/reader/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)      466 2022-02-02 00:05:56.000000 pyearth-0.1.9/pyearth/toolbox/reader/line_count.py
+-rw-r--r--   0 liao313  (231954) users      (100)     2267 2022-02-02 00:21:44.000000 pyearth-0.1.9/pyearth/toolbox/reader/parse_xml_file.py
+-rw-r--r--   0 liao313  (231954) users      (100)      815 2022-02-02 00:23:27.000000 pyearth-0.1.9/pyearth/toolbox/reader/read_configuration_file.py
+-rw-r--r--   0 liao313  (231954) users      (100)      589 2022-02-02 00:26:53.000000 pyearth-0.1.9/pyearth/toolbox/reader/split_string_into_chunk.py
+-rw-r--r--   0 liao313  (231954) users      (100)     5486 2022-02-02 00:20:25.000000 pyearth-0.1.9/pyearth/toolbox/reader/text_reader_string.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.173397 pyearth-0.1.9/pyearth/toolbox/slurm/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:29:08.000000 pyearth-0.1.9/pyearth/toolbox/slurm/__init__.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.187068 pyearth-0.1.9/pyearth/toolbox/slurm/mpi/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:29:16.000000 pyearth-0.1.9/pyearth/toolbox/slurm/mpi/__init__.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.211762 pyearth-0.1.9/pyearth/toolbox/slurm/parafly/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-23 03:29:11.000000 pyearth-0.1.9/pyearth/toolbox/slurm/parafly/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     1258 2022-02-02 17:24:19.000000 pyearth-0.1.9/pyearth/toolbox/slurm/parafly/prepare_parafly_python_command_file.py
+-rw-r--r--   0 liao313  (231954) users      (100)     3875 2022-02-02 17:28:47.000000 pyearth-0.1.9/pyearth/toolbox/slurm/parafly/prepare_parafly_slurm_job_script.py
+-rw-r--r--   0 liao313  (231954) users      (100)     4502 2022-02-02 17:37:38.000000 pyearth-0.1.9/pyearth/toolbox/slurm/slurm_prepare_job_script_python.py
+-rw-r--r--   0 liao313  (231954) users      (100)     5441 2022-02-02 17:37:10.000000 pyearth-0.1.9/pyearth/toolbox/slurm/slurm_prepare_job_script_python_checkpoint.py
+-rw-r--r--   0 liao313  (231954) users      (100)      683 2022-02-02 00:40:32.000000 pyearth-0.1.9/pyearth/toolbox/slurm/slurm_update_checkpoint_file.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.228546 pyearth-0.1.9/pyearth/visual/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-12-05 18:41:52.000000 pyearth-0.1.9/pyearth/visual/__init__.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.262615 pyearth-0.1.9/pyearth/visual/barplot/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2020-12-22 05:55:12.000000 pyearth-0.1.9/pyearth/visual/barplot/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     4208 2021-04-19 17:01:35.000000 pyearth-0.1.9/pyearth/visual/barplot/barplot_data.py
+-rw-r--r--   0 liao313  (231954) users      (100)     4908 2022-02-13 19:34:12.000000 pyearth-0.1.9/pyearth/visual/barplot/barplot_data_with_reference.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.318969 pyearth-0.1.9/pyearth/visual/color/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:15:36.000000 pyearth-0.1.9/pyearth/visual/color/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     2953 2021-05-24 22:04:07.000000 pyearth-0.1.9/pyearth/visual/color/choose_n_color.py
+-rw-r--r--   0 liao313  (231954) users      (100)     3229 2021-08-20 22:11:01.000000 pyearth-0.1.9/pyearth/visual/color/create_diverge_rgb_color_hex.py
+-rw-r--r--   0 liao313  (231954) users      (100)     3547 2021-04-19 17:08:52.000000 pyearth-0.1.9/pyearth/visual/color/create_qualitative_rgb_color_hex.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.337388 pyearth-0.1.9/pyearth/visual/histogram/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2020-05-04 17:07:18.000000 pyearth-0.1.9/pyearth/visual/histogram/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     3019 2021-04-19 17:22:06.000000 pyearth-0.1.9/pyearth/visual/histogram/histogram_plot.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.354167 pyearth-0.1.9/pyearth/visual/map/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2021-05-24 21:15:02.000000 pyearth-0.1.9/pyearth/visual/map/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     3072 2021-12-10 18:20:20.000000 pyearth-0.1.9/pyearth/visual/map/map_raster_data.py
+-rw-r--r--   0 liao313  (231954) users      (100)     8775 2022-02-15 21:33:55.000000 pyearth-0.1.9/pyearth/visual/plot_xy_data.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.400272 pyearth-0.1.9/pyearth/visual/scatter/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:15:44.000000 pyearth-0.1.9/pyearth/visual/scatter/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     1480 2021-01-17 02:59:12.000000 pyearth-0.1.9/pyearth/visual/scatter/scatter_lowess.py
+-rw-r--r--   0 liao313  (231954) users      (100)    10975 2021-12-10 18:20:19.000000 pyearth-0.1.9/pyearth/visual/scatter/scatter_plot_data.py
+-rw-r--r--   0 liao313  (231954) users      (100)    10404 2021-04-19 17:40:51.000000 pyearth-0.1.9/pyearth/visual/scatter/scatter_plot_data_density.py
+-rw-r--r--   0 liao313  (231954) users      (100)    12203 2022-02-17 19:26:36.000000 pyearth-0.1.9/pyearth/visual/scatter/scatter_plot_multiple_data.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.417644 pyearth-0.1.9/pyearth/visual/surface/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2020-04-20 23:57:01.000000 pyearth-0.1.9/pyearth/visual/surface/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     4533 2021-04-19 17:44:41.000000 pyearth-0.1.9/pyearth/visual/surface/convert_array_to_vtk_polygon.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.454980 pyearth-0.1.9/pyearth/visual/timeseries/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2019-12-05 18:41:42.000000 pyearth-0.1.9/pyearth/visual/timeseries/__init__.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.473590 pyearth-0.1.9/pyearth/visual/timeseries/analysis/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:15:56.000000 pyearth-0.1.9/pyearth/visual/timeseries/analysis/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     7980 2022-02-16 00:23:55.000000 pyearth-0.1.9/pyearth/visual/timeseries/analysis/plot_time_series_analysis.py
+-rw-r--r--   0 liao313  (231954) users      (100)      881 2021-04-07 20:21:45.000000 pyearth-0.1.9/pyearth/visual/timeseries/calculate_ticks_space.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.527425 pyearth-0.1.9/pyearth/visual/timeseries/fill/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:15:55.000000 pyearth-0.1.9/pyearth/visual/timeseries/fill/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     5714 2021-04-16 16:05:07.000000 pyearth-0.1.9/pyearth/visual/timeseries/fill/plot3d_time_series_data_fill.py
+-rw-r--r--   0 liao313  (231954) users      (100)     4935 2021-04-16 16:04:59.000000 pyearth-0.1.9/pyearth/visual/timeseries/fill/plot_time_series_data_monthly_fill.py
+-rw-r--r--   0 liao313  (231954) users      (100)     5727 2021-04-16 16:05:03.000000 pyearth-0.1.9/pyearth/visual/timeseries/fill/plot_time_series_data_multiple_temporal_resolution_fill.py
+-rw-r--r--   0 liao313  (231954) users      (100)     9169 2021-05-24 22:14:46.000000 pyearth-0.1.9/pyearth/visual/timeseries/plot_time_series_data.py
+-rw-r--r--   0 liao313  (231954) users      (100)     6099 2021-04-19 17:47:11.000000 pyearth-0.1.9/pyearth/visual/timeseries/plot_time_series_data_with_two_y_axis.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:30.545514 pyearth-0.1.9/pyearth/visual/timeseries/zoom/
+-rwxr-xr-x   0 liao313  (231954) users      (100)        0 2022-02-16 00:15:52.000000 pyearth-0.1.9/pyearth/visual/timeseries/zoom/__init__.py
+-rw-r--r--   0 liao313  (231954) users      (100)     5744 2021-04-19 17:47:39.000000 pyearth-0.1.9/pyearth/visual/timeseries/zoom/plot_time_series_data_monthly_fill_with_zoom.py
+drwxr-sr-x   0 liao313  (231954) users      (100)        0 2022-02-24 07:27:29.697185 pyearth-0.1.9/pyearth.egg-info/
+-rw-r--r--   0 liao313  (231954) users      (100)     2243 2022-02-24 07:27:26.000000 pyearth-0.1.9/pyearth.egg-info/PKG-INFO
+-rw-r--r--   0 liao313  (231954) users      (100)     4050 2022-02-24 07:27:27.000000 pyearth-0.1.9/pyearth.egg-info/SOURCES.txt
+-rw-r--r--   0 liao313  (231954) users      (100)        1 2022-02-24 07:27:26.000000 pyearth-0.1.9/pyearth.egg-info/dependency_links.txt
+-rw-r--r--   0 liao313  (231954) users      (100)       69 2022-02-24 07:27:26.000000 pyearth-0.1.9/pyearth.egg-info/requires.txt
+-rw-r--r--   0 liao313  (231954) users      (100)        8 2022-02-24 07:27:27.000000 pyearth-0.1.9/pyearth.egg-info/top_level.txt
+-rw-r--r--   0 liao313  (231954) users      (100)      103 2021-04-05 21:04:48.000000 pyearth-0.1.9/pyproject.toml
+-rw-r--r--   0 liao313  (231954) users      (100)      378 2022-02-24 07:27:30.569686 pyearth-0.1.9/setup.cfg
+-rw-r--r--   0 liao313  (231954) users      (100)     1448 2022-02-24 07:24:08.000000 pyearth-0.1.9/setup.py
```

### Comparing `pyearth-0.1.8/LICENSE.md` & `pyearth-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/PKG-INFO` & `pyearth-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyearth
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python for Earth Science.
 Home-page: https://github.com/changliao1025/pyearth
 Author: Chang Liao
 Author-email: changliao.climate@gmail.com
 License: custom
 Keywords: Earth Science
 Platform: UNKNOWN
```

### Comparing `pyearth-0.1.8/README.md` & `pyearth-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/gis/envi/envi_write_header.py` & `pyearth-0.1.9/pyearth/gis/envi/envi_write_header.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/gis/gdal/gdal_function.py` & `pyearth-0.1.9/pyearth/gis/gdal/gdal_function.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/gis/gdal/read/gdal_read_envi_file.py` & `pyearth-0.1.9/pyearth/gis/gdal/read/gdal_read_envi_file.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/gis/gdal/read/gdal_read_geotiff_file.py` & `pyearth-0.1.9/pyearth/gis/gdal/read/gdal_read_geotiff_file.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/gis/gdal/read/gdal_read_shapefile.py` & `pyearth-0.1.9/pyearth/gis/gdal/read/gdal_read_shapefile.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/gis/gdal/world2Pixel.py` & `pyearth-0.1.9/pyearth/gis/gdal/world2Pixel.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/gis/gdal/write/gdal_write_envi_file.py` & `pyearth-0.1.9/pyearth/gis/gdal/write/gdal_write_envi_file.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/gis/gdal/write/gdal_write_geotiff_file.py` & `pyearth-0.1.9/pyearth/gis/gdal/write/gdal_write_geotiff_file.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/gis/location/calculate_distance_based_on_lon_lat.py` & `pyearth-0.1.9/pyearth/gis/location/calculate_distance_based_on_lon_lat.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/gis/location/calculate_polygon_area.py` & `pyearth-0.1.9/pyearth/gis/location/calculate_polygon_area.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/gis/location/convert_lat_lon_range.py` & `pyearth-0.1.9/pyearth/gis/location/convert_lat_lon_range.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/system/define_global_variables.py` & `pyearth-0.1.9/pyearth/system/define_global_variables.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/data/convert_time_series_daily_to_monthly.py` & `pyearth-0.1.9/pyearth/toolbox/data/convert_time_series_daily_to_monthly.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/data/remove_outliers.py` & `pyearth-0.1.9/pyearth/toolbox/data/remove_outliers.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/date/day_in_month.py` & `pyearth-0.1.9/pyearth/toolbox/date/day_in_month.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/date/day_of_year.py` & `pyearth-0.1.9/pyearth/toolbox/date/day_of_year.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/date/dt2cal.py` & `pyearth-0.1.9/pyearth/toolbox/date/dt2cal.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/math/gap_fill_by_window.py` & `pyearth-0.1.9/pyearth/toolbox/math/gap_fill_by_window.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/math/stat/scipy_bivariate_kde.py` & `pyearth-0.1.9/pyearth/toolbox/math/stat/scipy_bivariate_kde.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/reader/parse_xml_file.py` & `pyearth-0.1.9/pyearth/toolbox/reader/parse_xml_file.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/reader/read_configuration_file.py` & `pyearth-0.1.9/pyearth/toolbox/reader/read_configuration_file.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/reader/split_string_into_chunk.py` & `pyearth-0.1.9/pyearth/toolbox/reader/split_string_into_chunk.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/reader/text_reader_string.py` & `pyearth-0.1.9/pyearth/toolbox/reader/text_reader_string.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/slurm/parafly/prepare_parafly_python_command_file.py` & `pyearth-0.1.9/pyearth/toolbox/slurm/parafly/prepare_parafly_python_command_file.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/slurm/parafly/prepare_parafly_slurm_job_script.py` & `pyearth-0.1.9/pyearth/toolbox/slurm/parafly/prepare_parafly_slurm_job_script.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/slurm/slurm_prepare_job_script_python.py` & `pyearth-0.1.9/pyearth/toolbox/slurm/slurm_prepare_job_script_python.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/slurm/slurm_prepare_job_script_python_checkpoint.py` & `pyearth-0.1.9/pyearth/toolbox/slurm/slurm_prepare_job_script_python_checkpoint.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/toolbox/slurm/slurm_update_checkpoint_file.py` & `pyearth-0.1.9/pyearth/toolbox/slurm/slurm_update_checkpoint_file.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/barplot/barplot_data.py` & `pyearth-0.1.9/pyearth/visual/barplot/barplot_data.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/barplot/barplot_data_with_reference.py` & `pyearth-0.1.9/pyearth/visual/barplot/barplot_data_with_reference.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/color/choose_n_color.py` & `pyearth-0.1.9/pyearth/visual/color/choose_n_color.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/color/create_diverge_rgb_color_hex.py` & `pyearth-0.1.9/pyearth/visual/color/create_diverge_rgb_color_hex.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/color/create_qualitative_rgb_color_hex.py` & `pyearth-0.1.9/pyearth/visual/color/create_qualitative_rgb_color_hex.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/histogram/histogram_plot.py` & `pyearth-0.1.9/pyearth/visual/histogram/histogram_plot.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/map/map_raster_data.py` & `pyearth-0.1.9/pyearth/visual/map/map_raster_data.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/plot_xy_data.py` & `pyearth-0.1.9/pyearth/visual/plot_xy_data.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/scatter/scatter_lowess.py` & `pyearth-0.1.9/pyearth/visual/scatter/scatter_lowess.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/scatter/scatter_plot_data.py` & `pyearth-0.1.9/pyearth/visual/scatter/scatter_plot_data.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/scatter/scatter_plot_data_density.py` & `pyearth-0.1.9/pyearth/visual/scatter/scatter_plot_data_density.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/scatter/scatter_plot_multiple_data.py` & `pyearth-0.1.9/pyearth/visual/scatter/scatter_plot_multiple_data.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/surface/convert_array_to_vtk_polygon.py` & `pyearth-0.1.9/pyearth/visual/surface/convert_array_to_vtk_polygon.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/timeseries/analysis/plot_time_series_analysis.py` & `pyearth-0.1.9/pyearth/visual/timeseries/analysis/plot_time_series_analysis.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/timeseries/calculate_ticks_space.py` & `pyearth-0.1.9/pyearth/visual/timeseries/calculate_ticks_space.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/timeseries/fill/plot3d_time_series_data_fill.py` & `pyearth-0.1.9/pyearth/visual/timeseries/fill/plot3d_time_series_data_fill.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/timeseries/fill/plot_time_series_data_monthly_fill.py` & `pyearth-0.1.9/pyearth/visual/timeseries/fill/plot_time_series_data_monthly_fill.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/timeseries/fill/plot_time_series_data_multiple_temporal_resolution_fill.py` & `pyearth-0.1.9/pyearth/visual/timeseries/fill/plot_time_series_data_multiple_temporal_resolution_fill.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/timeseries/plot_time_series_data.py` & `pyearth-0.1.9/pyearth/visual/timeseries/plot_time_series_data.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/timeseries/plot_time_series_data_with_two_y_axis.py` & `pyearth-0.1.9/pyearth/visual/timeseries/plot_time_series_data_with_two_y_axis.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth/visual/timeseries/zoom/plot_time_series_data_monthly_fill_with_zoom.py` & `pyearth-0.1.9/pyearth/visual/timeseries/zoom/plot_time_series_data_monthly_fill_with_zoom.py`

 * *Files identical despite different names*

### Comparing `pyearth-0.1.8/pyearth.egg-info/PKG-INFO` & `pyearth-0.1.9/pyearth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyearth
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python for Earth Science.
 Home-page: https://github.com/changliao1025/pyearth
 Author: Chang Liao
 Author-email: changliao.climate@gmail.com
 License: custom
 Keywords: Earth Science
 Platform: UNKNOWN
```

### Comparing `pyearth-0.1.8/pyearth.egg-info/SOURCES.txt` & `pyearth-0.1.9/pyearth.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 pyearth/system/define_global_variables.py
 pyearth/toolbox/__init__.py
 pyearth/toolbox/data/__init__.py
 pyearth/toolbox/data/check_if_duplicates.py
 pyearth/toolbox/data/convert_time_series_daily_to_monthly.py
 pyearth/toolbox/data/remove_outliers.py
 pyearth/toolbox/data/shift_array.py
+pyearth/toolbox/data/beta/__init__.py
+pyearth/toolbox/data/beta/add_variable_to_netcdf.py
+pyearth/toolbox/data/beta/replace_variable_in_netcdf.py
 pyearth/toolbox/date/__init__.py
 pyearth/toolbox/date/day_in_month.py
 pyearth/toolbox/date/day_of_year.py
 pyearth/toolbox/date/dt2cal.py
 pyearth/toolbox/date/leap_year.py
 pyearth/toolbox/geometry/__init__.py
 pyearth/toolbox/geometry/calculate_hexagon_area.py
```

### Comparing `pyearth-0.1.8/setup.py` & `pyearth-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = "pyearth"
 DESCRIPTION = \
     "Python for Earth Science."
 AUTHOR = "Chang Liao"
 AUTHOR_EMAIL = "changliao.climate@gmail.com"
 URL = "https://github.com/changliao1025/pyearth"
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 REQUIRES_PYTHON = ">=3.8.0"
 KEYWORDS = "Earth Science"
 
 REQUIRED = [    
     "julian",
     "matplotlib",
     "netCDF4",
```

