# Comparing `tmp/apache-sedona-1.5.1.tar.gz` & `tmp/apache_sedona-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-sedona-1.5.1.tar", last modified: Wed Jan 17 18:11:20 2024, max compression
+gzip compressed data, was "apache_sedona-1.5.2.tar", last modified: Tue May  7 19:30:01 2024, max compression
```

## Comparing `apache-sedona-1.5.1.tar` & `apache_sedona-1.5.2.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.838199 apache-sedona-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-01-17 18:11:20.838199 apache-sedona-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.838199 apache-sedona-1.5.1/apache_sedona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-01-17 18:11:20.000000 apache-sedona-1.5.1/apache_sedona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-01-17 18:11:20.000000 apache-sedona-1.5.1/apache_sedona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 18:11:20.000000 apache-sedona-1.5.1/apache_sedona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-17 18:11:20.000000 apache-sedona-1.5.1/apache_sedona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-17 18:11:20.000000 apache-sedona-1.5.1/apache_sedona.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.826200 apache-sedona-1.5.1/sedona/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.826200 apache-sedona-1.5.1/sedona/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.826200 apache-sedona-1.5.1/sedona/core/SpatialRDD/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/SpatialRDD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/SpatialRDD/circle_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/SpatialRDD/linestring_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/SpatialRDD/point_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/SpatialRDD/polygon_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/SpatialRDD/rectangle_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/SpatialRDD/spatial_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/SpatialRDD/spatial_rdd_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.826200 apache-sedona-1.5.1/sedona/core/enums/
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/enums/file_data_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/enums/grid_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/enums/index_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/enums/join_build_side.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/enums/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.830200 apache-sedona-1.5.1/sedona/core/formatMapper/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/formatMapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/formatMapper/disc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/formatMapper/geo_json_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/formatMapper/geo_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.830200 apache-sedona-1.5.1/sedona/core/formatMapper/shapefileParser/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/formatMapper/shapefileParser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/formatMapper/shapefileParser/shape_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/formatMapper/wkb_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/formatMapper/wkt_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.830200 apache-sedona-1.5.1/sedona/core/geom/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/geom/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/geom/envelope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.830200 apache-sedona-1.5.1/sedona/core/jvm/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/jvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/jvm/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/jvm/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/jvm/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.830200 apache-sedona-1.5.1/sedona/core/spatialOperator/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/spatialOperator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/spatialOperator/join_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/spatialOperator/join_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/spatialOperator/join_query_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/spatialOperator/knn_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/spatialOperator/range_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/spatialOperator/range_query_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/spatialOperator/rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.830200 apache-sedona-1.5.1/sedona/maps/
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/maps/SedonaKepler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/maps/SedonaMapUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/maps/SedonaPyDeck.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/maps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.830200 apache-sedona-1.5.1/sedona/raster_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/raster_utils/SedonaUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/raster_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.834200 apache-sedona-1.5.1/sedona/register/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/register/geo_registrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/register/java_libs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.834200 apache-sedona-1.5.1/sedona/spark/
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/spark/SedonaContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.834200 apache-sedona-1.5.1/sedona/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/sql/dataframe_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/sql/st_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/sql/st_constructors.py
--rw-r--r--   0 runner    (1001) docker     (127)    63285 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/sql/st_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/sql/st_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/sql/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.834200 apache-sedona-1.5.1/sedona/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/abstract_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/binary_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/geometry_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/geometry_serde.py
--rw-r--r--   0 runner    (1001) docker     (127)    19092 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/geometry_serde_general.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/jvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/serde.py
--rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/spatial_rdd_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/sedona/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 18:11:20.838199 apache-sedona-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.838199 apache-sedona-1.5.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/src/geom_buf.c
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/src/geom_buf.h
--rw-r--r--   0 runner    (1001) docker     (127)    24131 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/src/geomserde.c
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/src/geomserde.h
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/src/geomserde_speedup_module.c
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/src/geos_c_dyn.c
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/src/geos_c_dyn.h
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/src/geos_c_dyn_funcs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.838199 apache-sedona-1.5.1/src/pygeos/
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/src/pygeos/c_api.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 18:11:20.838199 apache-sedona-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/tests/test_assign_raw_spatial_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/tests/test_circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/tests/test_multiple_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-01-17 18:11:11.000000 apache-sedona-1.5.1/tests/test_scala_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.200940 apache_sedona-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-07 19:30:01.200940 apache_sedona-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.200940 apache_sedona-1.5.2/apache_sedona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-07 19:30:01.000000 apache_sedona-1.5.2/apache_sedona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-07 19:30:01.000000 apache_sedona-1.5.2/apache_sedona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:30:01.000000 apache_sedona-1.5.2/apache_sedona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-07 19:30:01.000000 apache_sedona-1.5.2/apache_sedona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 19:30:01.000000 apache_sedona-1.5.2/apache_sedona.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.184940 apache_sedona-1.5.2/sedona/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.184940 apache_sedona-1.5.2/sedona/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.184940 apache_sedona-1.5.2/sedona/core/SpatialRDD/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/SpatialRDD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/SpatialRDD/circle_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/SpatialRDD/linestring_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/SpatialRDD/point_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/SpatialRDD/polygon_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/SpatialRDD/rectangle_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/SpatialRDD/spatial_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/SpatialRDD/spatial_rdd_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.188940 apache_sedona-1.5.2/sedona/core/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/enums/file_data_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/enums/grid_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/enums/index_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/enums/join_build_side.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/enums/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.188940 apache_sedona-1.5.2/sedona/core/formatMapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/formatMapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/formatMapper/disc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/formatMapper/geo_json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/formatMapper/geo_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.188940 apache_sedona-1.5.2/sedona/core/formatMapper/shapefileParser/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/formatMapper/shapefileParser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/formatMapper/shapefileParser/shape_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/formatMapper/wkb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/formatMapper/wkt_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.188940 apache_sedona-1.5.2/sedona/core/geom/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/geom/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/geom/envelope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.188940 apache_sedona-1.5.2/sedona/core/jvm/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/jvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/jvm/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/jvm/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/jvm/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.192940 apache_sedona-1.5.2/sedona/core/spatialOperator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/spatialOperator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/spatialOperator/join_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/spatialOperator/join_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/spatialOperator/join_query_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/spatialOperator/knn_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/spatialOperator/range_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/spatialOperator/range_query_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/spatialOperator/rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.192940 apache_sedona-1.5.2/sedona/maps/
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/maps/SedonaKepler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/maps/SedonaMapUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/maps/SedonaPyDeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/maps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.192940 apache_sedona-1.5.2/sedona/raster_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/raster_utils/SedonaUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/raster_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.192940 apache_sedona-1.5.2/sedona/register/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/register/geo_registrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/register/java_libs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.192940 apache_sedona-1.5.2/sedona/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/spark/SedonaContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.192940 apache_sedona-1.5.2/sedona/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/sql/dataframe_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/sql/st_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/sql/st_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61309 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/sql/st_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/sql/st_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/sql/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.196940 apache_sedona-1.5.2/sedona/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/abstract_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/binary_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/geometry_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/geometry_serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19092 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/geometry_serde_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/spatial_rdd_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/sedona/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:30:01.200940 apache_sedona-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.196940 apache_sedona-1.5.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/src/geom_buf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/src/geom_buf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24131 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/src/geomserde.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/src/geomserde.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/src/geomserde_speedup_module.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/src/geos_c_dyn.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/src/geos_c_dyn.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/src/geos_c_dyn_funcs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.196940 apache_sedona-1.5.2/src/pygeos/
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/src/pygeos/c_api.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:30:01.200940 apache_sedona-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/tests/test_assign_raw_spatial_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/tests/test_circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/tests/test_multiple_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-07 19:29:58.000000 apache_sedona-1.5.2/tests/test_scala_example.py
```

### Comparing `apache-sedona-1.5.1/apache_sedona.egg-info/SOURCES.txt` & `apache_sedona-1.5.2/apache_sedona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/__init__.py` & `apache_sedona-1.5.2/sedona/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/SpatialRDD/__init__.py` & `apache_sedona-1.5.2/sedona/core/SpatialRDD/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/SpatialRDD/circle_rdd.py` & `apache_sedona-1.5.2/sedona/core/SpatialRDD/circle_rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/SpatialRDD/linestring_rdd.py` & `apache_sedona-1.5.2/sedona/core/SpatialRDD/linestring_rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/SpatialRDD/point_rdd.py` & `apache_sedona-1.5.2/sedona/core/SpatialRDD/point_rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/SpatialRDD/polygon_rdd.py` & `apache_sedona-1.5.2/sedona/core/SpatialRDD/polygon_rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/SpatialRDD/rectangle_rdd.py` & `apache_sedona-1.5.2/sedona/core/SpatialRDD/rectangle_rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/SpatialRDD/spatial_rdd.py` & `apache_sedona-1.5.2/sedona/core/SpatialRDD/spatial_rdd.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from pyspark import StorageLevel
 
 from sedona.core.SpatialRDD.spatial_rdd_factory import SpatialRDDFactory
 from sedona.core.enums.grid_type import GridTypeJvm, GridType
 from sedona.core.enums.index_type import IndexTypeJvm, IndexType
 from sedona.core.enums.spatial import SpatialType
 from sedona.core.geom.envelope import Envelope
-from sedona.core.jvm.config import since
 from sedona.core.jvm.translate import SedonaPythonConverter, JvmSedonaPythonConverter
 from sedona.utils.decorators import require
 from sedona.utils.jvm import JvmStorageLevel
 from sedona.utils.spatial_rdd_parser import SedonaPickler
 from sedona.utils.types import crs
 
 
@@ -189,15 +188,14 @@
         """
 
         :return:
         """
         return self._srdd.countWithoutDuplicatesSPRDD()
 
     @property
-    @since("1.0.0")
     def fieldNames(self) -> List[str]:
         """
 
         :return:
         """
         try:
             field_names = list(get_field(self._srdd, "fieldNames"))
```

### Comparing `apache-sedona-1.5.1/sedona/core/SpatialRDD/spatial_rdd_factory.py` & `apache_sedona-1.5.2/sedona/core/SpatialRDD/spatial_rdd_factory.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/__init__.py` & `apache_sedona-1.5.2/sedona/core/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/enums/__init__.py` & `apache_sedona-1.5.2/sedona/core/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/enums/file_data_splitter.py` & `apache_sedona-1.5.2/sedona/core/enums/file_data_splitter.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/enums/grid_type.py` & `apache_sedona-1.5.2/sedona/core/enums/grid_type.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/enums/index_type.py` & `apache_sedona-1.5.2/sedona/core/enums/index_type.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/enums/join_build_side.py` & `apache_sedona-1.5.2/sedona/core/enums/join_build_side.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/enums/spatial.py` & `apache_sedona-1.5.2/sedona/core/enums/spatial.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/formatMapper/__init__.py` & `apache_sedona-1.5.2/sedona/core/formatMapper/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/formatMapper/disc_utils.py` & `apache_sedona-1.5.2/sedona/core/formatMapper/disc_utils.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/formatMapper/geo_json_reader.py` & `apache_sedona-1.5.2/sedona/core/formatMapper/geo_json_reader.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/formatMapper/geo_reader.py` & `apache_sedona-1.5.2/sedona/core/formatMapper/geo_reader.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/formatMapper/shapefileParser/__init__.py` & `apache_sedona-1.5.2/sedona/core/formatMapper/shapefileParser/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/formatMapper/shapefileParser/shape_file_reader.py` & `apache_sedona-1.5.2/sedona/core/formatMapper/shapefileParser/shape_file_reader.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/formatMapper/wkb_reader.py` & `apache_sedona-1.5.2/sedona/core/formatMapper/wkb_reader.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/formatMapper/wkt_reader.py` & `apache_sedona-1.5.2/sedona/core/formatMapper/wkt_reader.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/geom/__init__.py` & `apache_sedona-1.5.2/sedona/core/geom/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/geom/circle.py` & `apache_sedona-1.5.2/sedona/core/geom/circle.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/geom/envelope.py` & `apache_sedona-1.5.2/sedona/core/geom/envelope.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/jvm/__init__.py` & `apache_sedona-1.5.2/sedona/core/jvm/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/jvm/abstract.py` & `apache_sedona-1.5.2/sedona/core/jvm/abstract.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/jvm/config.py` & `apache_sedona-1.5.2/sedona/core/jvm/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
 import logging
 import os
 from re import findall
-from typing import Any, Optional, Tuple
+from typing import Optional, Tuple
 
 from py4j.protocol import Py4JJavaError
 from pyspark.sql import SparkSession
 from sedona.utils.decorators import classproperty
 import functools
 import inspect
 import warnings
@@ -85,21 +85,19 @@
             if inspect.isclass(func1):
                 fmt1 = "Call to deprecated class {name} ({reason})."
             else:
                 fmt1 = "Call to deprecated function {name} ({reason})."
 
             @functools.wraps(func1)
             def new_func1(*args, **kwargs):
-                warnings.simplefilter('always', DeprecationWarning)
                 warnings.warn(
                     fmt1.format(name=func1.__name__, reason=reason),
                     category=DeprecationWarning,
                     stacklevel=2
                 )
-                warnings.simplefilter('default', DeprecationWarning)
                 return func1(*args, **kwargs)
 
             return new_func1
 
         return decorator
 
     elif inspect.isclass(reason) or inspect.isfunction(reason):
@@ -117,21 +115,19 @@
         if inspect.isclass(func2):
             fmt2 = "Call to deprecated class {name}."
         else:
             fmt2 = "Call to deprecated function {name}."
 
         @functools.wraps(func2)
         def new_func2(*args, **kwargs):
-            warnings.simplefilter('always', DeprecationWarning)
             warnings.warn(
                 fmt2.format(name=func2.__name__),
                 category=DeprecationWarning,
                 stacklevel=2
             )
-            warnings.simplefilter('default', DeprecationWarning)
             return func2(*args, **kwargs)
 
         return new_func2
 
     else:
         raise TypeError(repr(type(reason)))
 
@@ -187,28 +183,27 @@
 
         java_spark_conf = spark_conf._jconf
         used_jar_files = None
         error_message = None
 
         try:
             used_jar_files = java_spark_conf.get(value)
-        except Py4JJavaError as java_error:
-            error_message = "Failed to get the value of {} from SparkConf: {}".format(
-                value, java_error
-            )
+        except Py4JJavaError:
+            error_message = "Didn't find the value of {} from SparkConf".format(value)
+            logging.info(error_message)
 
         return used_jar_files, error_message
 
 
 class SedonaMeta:
     @classmethod
     def get_version(cls, spark_jars: str) -> Optional[str]:
         # Find Spark version, Scala version and Sedona version.
         versions = findall(
-            r"sedona-(?:python-adapter|spark-shaded)-([^,\n]{3})_([^,\n]{4})-([^,\n]{5})",
+            r"sedona-(?:python-adapter|spark-shaded|spark)-([^,\n]{3})_([^,\n]{4})-([^,\n]{5})",
             spark_jars,
         )
         print(versions)
         try:
             sedona_version = versions[0][2]
         except IndexError:
             sedona_version = None
```

### Comparing `apache-sedona-1.5.1/sedona/core/jvm/translate.py` & `apache_sedona-1.5.2/sedona/core/jvm/translate.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/spatialOperator/__init__.py` & `apache_sedona-1.5.2/sedona/core/spatialOperator/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/spatialOperator/join_params.py` & `apache_sedona-1.5.2/sedona/core/spatialOperator/join_params.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/spatialOperator/join_query.py` & `apache_sedona-1.5.2/sedona/core/spatialOperator/join_query.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/spatialOperator/join_query_raw.py` & `apache_sedona-1.5.2/sedona/core/spatialOperator/join_query_raw.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/spatialOperator/knn_query.py` & `apache_sedona-1.5.2/sedona/core/spatialOperator/knn_query.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/spatialOperator/range_query.py` & `apache_sedona-1.5.2/sedona/core/spatialOperator/range_query.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/spatialOperator/range_query_raw.py` & `apache_sedona-1.5.2/sedona/core/spatialOperator/range_query_raw.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/spatialOperator/rdd.py` & `apache_sedona-1.5.2/sedona/core/spatialOperator/rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/core/utils.py` & `apache_sedona-1.5.2/sedona/core/utils.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/exceptions.py` & `apache_sedona-1.5.2/sedona/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/maps/SedonaKepler.py` & `apache_sedona-1.5.2/sedona/maps/SedonaKepler.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,29 +11,35 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-from keplergl import KeplerGl
 from sedona.maps.SedonaMapUtils import SedonaMapUtils
 
 
 class SedonaKepler:
 
     @classmethod
     def create_map(cls, df=None, name="unnamed", config=None):
         """
         Creates a map visualization using kepler, optionally taking a sedona dataFrame as data input
         :param df: [Optional] SedonaDataFrame to plot on the map
         :param name: [Optional] Name to be associated with the given
         dataframe, if a df is passed with no name, a default name of 'unnamed' is set for it.
         param config: [Optional] A map config to be applied to the rendered map :return: A map object
         """
+
+        try:
+            from keplergl import KeplerGl
+        except ImportError:
+            msg = "Install sedona[kepler-map] to convert sedona dataframes to kepler maps."
+            raise ImportError(msg) from None
+
         kepler_map = KeplerGl()
         if df is not None:
             SedonaKepler.add_df(kepler_map, df, name)
 
         if config is not None:
             kepler_map.config = config
 
@@ -44,9 +50,9 @@
         """
         Adds a SedonaDataFrame to a given map object.
         :param kepler_map: Map object to add SedonaDataFrame to
         :param df: SedonaDataFrame to add
         :param name: [Optional] Name to assign to the dataframe, default name assigned is 'unnamed'
         :return: Does not return anything, adds df directly to the given map object
         """
-        geo_df = SedonaMapUtils.__convert_to_gdf__(df)
+        geo_df = SedonaMapUtils.__convert_to_gdf_or_pdf__(df)
         kepler_map.add_data(geo_df, name=name)
```

### Comparing `apache-sedona-1.5.1/sedona/maps/SedonaMapUtils.py` & `apache_sedona-1.5.2/sedona/maps/SedonaMapUtils.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,35 +20,41 @@
 import json
 from sedona.sql.types import GeometryType
 
 
 class SedonaMapUtils:
 
     @classmethod
-    def __convert_to_gdf__(cls, df, rename=True, geometry_col=None):
+    def __convert_to_gdf_or_pdf__(cls, df, rename=True, geometry_col=None):
         """
         Converts a SedonaDataFrame to a GeoPandasDataFrame and also renames geometry column to a standard name of
-        'geometry' :param df: SedonaDataFrame to convert :param geometry_col: [Optional] :return:
+        'geometry'
+        However, if no geometry column is found even after traversing schema, returns a Pandas Dataframe
+        :param df: SedonaDataFrame to convert
+        :param geometry_col: [Optional]
+        :return: GeoPandas Dataframe or Pandas Dataframe
         """
         if geometry_col is None:
             geometry_col = SedonaMapUtils.__get_geometry_col__(df)
         pandas_df = df.toPandas()
+        if geometry_col is None:  # No geometry column found even after searching schema, return Pandas Dataframe
+            return pandas_df
         geo_df = gpd.GeoDataFrame(pandas_df, geometry=geometry_col)
         if geometry_col != "geometry" and rename is True:
             geo_df.rename_geometry("geometry", inplace=True)
         return geo_df
 
     @classmethod
     def __convert_to_geojson__(cls, df):
         """
         Converts a SedonaDataFrame to GeoJSON
         :param df: SedonaDataFrame to convert
         :return: GeoJSON object
         """
-        gdf = SedonaMapUtils.__convert_to_gdf__(df)
+        gdf = SedonaMapUtils.__convert_to_gdf_or_pdf__(df)
         gjson_str = gdf.to_json()
         gjson = json.loads(gjson_str)
         return gjson
 
     @classmethod
     def __get_geometry_col__(cls, df):
         schema = df.schema
```

### Comparing `apache-sedona-1.5.1/sedona/maps/SedonaPyDeck.py` & `apache_sedona-1.5.2/sedona/maps/SedonaPyDeck.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-import pydeck as pdk
+from types import ModuleType
 from sedona.maps.SedonaMapUtils import SedonaMapUtils
 
 
 class SedonaPyDeck:
 
     # User Facing APIs
     @classmethod
@@ -33,14 +33,15 @@
                 If no color scheme is given, a default color scheme is created using the 'plot_col' column as the quantizing column
         :param plot_col: Column to be used to create a default color scheme. If fill_color is provided, this parameter is ignored.
         :param initial_view_state:
         :param map_style:
         :param map_provider:
         :return: A pydeck Map object with choropleth layer added:
         """
+        pdk = _try_import_pydeck()
 
         if initial_view_state is None:
             gdf = SedonaPyDeck._prepare_df_(df, add_coords=True)
             initial_view_state = pdk.data_utils.compute_view(gdf['coordinate_array_sedona'])
         else:
             gdf = SedonaPyDeck._prepare_df_(df)
 
@@ -75,14 +76,16 @@
         :param fill_color: Optional color for the plotted polygons
         :param elevation_col: Optional column/numeric value to determine elevation for plotted polygons
         :param initial_view_state: optional initial view state of the pydeck map
         :param map_style: optional map_style of the pydeck map
         :param map_provider: optional map_provider of the pydeck map
         :return: A pydeck map with a GeoJsonLayer map added
         """
+        pdk = _try_import_pydeck()
+
         geometry_col = SedonaMapUtils.__get_geometry_col__(df)
         gdf = SedonaPyDeck._prepare_df_(df, geometry_col=geometry_col)
         geom_type = gdf[geometry_col][0].geom_type
         SedonaPyDeck._create_coord_column_(gdf, geometry_col=geometry_col)
         # if len(type_list) >= 2:  # change line colors if any to make it more visible.
         #     if line_color == "[85, 183, 177, 255]":
         #         line_color = "[237, 119, 79]"
@@ -112,14 +115,16 @@
         :param df: SedonaDataFrame to plot
         :param fill_color: color of the points
         :param initial_view_state: optional initial view state of a pydeck map
         :param map_style: optional map_style to be added to the pydeck map
         :param map_provider: optional map_provider to be added to the pydeck map
         :return: A pydeck map object with a scatterplot layer added
         """
+        pdk = _try_import_pydeck()
+
         gdf = SedonaPyDeck._prepare_df_(df, add_coords=True)
         layer = pdk.Layer(
             "ScatterplotLayer",
             data=gdf,
             pickable=True,
             opacity=0.8,
             filled=True,
@@ -148,14 +153,15 @@
         :param weight: Optional column to determine weight of each point while plotting the heatmap
         :param aggregation: Optional aggregation to use for the heatmap (used when rendering a zoomed out heatmap)
         :param initial_view_state: Optional initial view state of the pydeck map
         :param map_style: Optional map_style of the pydeck map
         :param map_provider: Optional map_provider for the pydeck map
         :return: A pydeck map with a heatmap layer added
         """
+        pdk = _try_import_pydeck()
 
         gdf = SedonaPyDeck._prepare_df_(df, add_coords=True)
 
         if color_range is None:
             color_range = [
                 [255, 255, 178],
                 [254, 217, 118],
@@ -191,15 +197,15 @@
         Convert a SedonaDataFrame to a GeoPandas DataFrame without renaming the column (as it is not necessary while rendering a pydeck map)
         :param df: SedonaDataFrame
         :param add_coords: Used to decide if a coordinate column containing lists of point coordinates is to be added to the resultant gdf.
         :return: GeoPandas DataFrame
         """
         if geometry_col is None:
             geometry_col = SedonaMapUtils.__get_geometry_col__(df=df)
-        gdf = SedonaMapUtils.__convert_to_gdf__(df, rename=False, geometry_col=geometry_col)
+        gdf = SedonaMapUtils.__convert_to_gdf_or_pdf__(df, rename=False, geometry_col=geometry_col)
         if add_coords is True:
             SedonaPyDeck._create_coord_column_(gdf=gdf, geometry_col=geometry_col)
         return gdf
 
     # Utility APIs specific to SedonaPyDeck
     @classmethod
     def _set_optional_parameters_(cls, p_map, map_style, map_provider):
@@ -235,14 +241,15 @@
         """
         type_list = []
         gdf['coordinate_array_sedona'] = gdf.apply(
             lambda val: list(SedonaMapUtils.__extract_coordinate__(val[geometry_col], type_list)), axis=1)
 
     @classmethod
     def _create_fat_layer_(cls, gdf, fill_color, line_color, elevation_col):
+        pdk = _try_import_pydeck()
         layer = pdk.Layer(
             'GeoJsonLayer',  # `type` positional argument is here
             data=gdf,
             auto_highlight=True,
             get_fill_color=fill_color,
             opacity=0.4,
             stroked=False,
@@ -250,7 +257,18 @@
             get_elevation=elevation_col,
             get_line_color=line_color,
             pickable=True,
             get_line_width=3
         )
 
         return layer
+
+
+def _try_import_pydeck() -> ModuleType:
+    try:
+        import pydeck as pdk
+
+    except ImportError:
+        msg = "Install sedona[pydeck-map] to convert sedona dataframes to pydeck maps."
+        raise ImportError(msg) from None
+
+    return pdk
```

### Comparing `apache-sedona-1.5.1/sedona/maps/__init__.py` & `apache_sedona-1.5.2/sedona/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/raster_utils/SedonaUtils.py` & `apache_sedona-1.5.2/sedona/raster_utils/SedonaUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,12 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-from IPython.display import display, HTML
-
 class SedonaUtils:
     @classmethod
     def display_image(cls, df):
+        from IPython.display import display, HTML
         display(HTML(df.toPandas().to_html(escape=False)))
```

### Comparing `apache-sedona-1.5.1/sedona/raster_utils/__init__.py` & `apache_sedona-1.5.2/sedona/raster_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/register/__init__.py` & `apache_sedona-1.5.2/sedona/register/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/register/geo_registrator.py` & `apache_sedona-1.5.2/sedona/register/geo_registrator.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/register/java_libs.py` & `apache_sedona-1.5.2/sedona/register/java_libs.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/spark/SedonaContext.py` & `apache_sedona-1.5.2/sedona/spark/SedonaContext.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         and register the core logics of Apache Sedona, for this SparkSession.
 
         :param spark: pyspark.sql.SparkSession, spark session instance
         :return: SedonaContext which is an instance of SparkSession
         """
         spark.sql("SELECT 1 as geom").count()
         PackageImporter.import_jvm_lib(spark._jvm)
-        spark._jvm.SedonaContext.create(spark._jsparkSession)
+        spark._jvm.SedonaContext.create(spark._jsparkSession, "python")
         return spark
 
     @classmethod
     def builder(cls) -> SparkSession.builder:
         """
         This method adds the basic Sedona configuration to the SparkSession builder.
         Usually the user does not need to call this method directly, as it is configured when a cluster is created.
```

### Comparing `apache-sedona-1.5.1/sedona/sql/__init__.py` & `apache_sedona-1.5.2/sedona/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/sql/dataframe_api.py` & `apache_sedona-1.5.2/sedona/sql/dataframe_api.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/sql/exceptions.py` & `apache_sedona-1.5.2/sedona/sql/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/sql/st_aggregates.py` & `apache_sedona-1.5.2/sedona/sql/st_aggregates.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 #
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
+import inspect
+import sys
 
 from functools import partial
 
 from pyspark.sql import Column
 
 from sedona.sql.dataframe_api import ColumnOrName, call_sedona_function, validate_argument_types
 
 _call_aggregate_function = partial(call_sedona_function, "st_aggregates")
 
-__all__ = [
-    "ST_Envelope_Aggr",
-    "ST_Intersection_Aggr",
-    "ST_Union_Aggr",
-]
+# Automatically populate __all__
+__all__ = [name for name, obj in inspect.getmembers(sys.modules[__name__])
+           if inspect.isfunction(obj)]
 
 
 @validate_argument_types
 def ST_Envelope_Aggr(geometry: ColumnOrName) -> Column:
     """Aggregate Function: Get the aggregate envelope of a geometry column.
 
     :param geometry: Geometry column to aggregate.
```

### Comparing `apache-sedona-1.5.1/sedona/sql/st_constructors.py` & `apache_sedona-1.5.2/sedona/sql/st_constructors.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,42 +10,28 @@
 #
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
+import inspect
+import sys
 
 from functools import partial
 from typing import Optional, Union
 
 from pyspark.sql import Column
 
 from sedona.sql.dataframe_api import ColumnOrName, ColumnOrNameOrNumber, call_sedona_function, validate_argument_types
 
 
-__all__ = [
-    "ST_GeomFromGeoHash",
-    "ST_GeomFromGeoJSON",
-    "ST_GeomFromGML",
-    "ST_GeomFromKML",
-    "ST_GeomFromText",
-    "ST_GeomFromWKB",
-    "ST_GeomFromWKT",
-    "ST_GeomFromEWKT",
-    "ST_LineFromText",
-    "ST_LineStringFromText",
-    "ST_Point",
-    "ST_PointFromText",
-    "ST_MakePoint"
-    "ST_PolygonFromEnvelope",
-    "ST_PolygonFromText",
-    "ST_MLineFromText",
-    "ST_MPolyFromText"
-]
+# Automatically populate __all__
+__all__ = [name for name, obj in inspect.getmembers(sys.modules[__name__])
+           if inspect.isfunction(obj)]
 
 
 _call_constructor_function = partial(call_sedona_function, "st_constructors")
 
 
 @validate_argument_types
 def ST_GeomFromGeoHash(geohash: ColumnOrName, precision: Union[ColumnOrName, int]) -> Column:
@@ -94,24 +80,26 @@
     :return: Geometry column representing the KML string.
     :rtype: Column
     """
     return _call_constructor_function("ST_GeomFromKML", kml_string)
 
 
 @validate_argument_types
-def ST_GeomFromText(wkt: ColumnOrName) -> Column:
+def ST_GeomFromText(wkt: ColumnOrName, srid: Optional[ColumnOrNameOrNumber] = None) -> Column:
     """Generate a geometry column from a Well-Known Text (WKT) string column.
     This is an alias of ST_GeomFromWKT.
 
     :param wkt: WKT string column to generate from.
     :type wkt: ColumnOrName
     :return: Geometry column representing the WKT string.
     :rtype: Column
     """
-    return _call_constructor_function("ST_GeomFromText", wkt)
+    args = (wkt) if srid is None else (wkt, srid)
+
+    return _call_constructor_function("ST_GeomFromText", args)
 
 
 @validate_argument_types
 def ST_GeomFromWKB(wkb: ColumnOrName) -> Column:
     """Generate a geometry column from a Well-Known Binary (WKB) binary column.
 
     :param wkb: WKB binary column to generate from.
@@ -119,24 +107,26 @@
     :return: Geometry column representing the WKB binary.
     :rtype: Column
     """
     return _call_constructor_function("ST_GeomFromWKB", wkb)
 
 
 @validate_argument_types
-def ST_GeomFromWKT(wkt: ColumnOrName) -> Column:
+def ST_GeomFromWKT(wkt: ColumnOrName, srid: Optional[ColumnOrNameOrNumber] = None) -> Column:
     """Generate a geometry column from a Well-Known Text (WKT) string column.
     This is an alias of ST_GeomFromText.
 
     :param wkt: WKT string column to generate from.
     :type wkt: ColumnOrName
     :return: Geometry column representing the WKT string.
     :rtype: Column
     """
-    return _call_constructor_function("ST_GeomFromWKT", wkt)
+    args = (wkt) if srid is None else (wkt, srid)
+
+    return _call_constructor_function("ST_GeomFromWKT", args)
 
 @validate_argument_types
 def ST_GeomFromEWKT(ewkt: ColumnOrName) -> Column:
     """Generate a geometry column from a OGC Extended Well-Known Text (WKT) string column.
 
     :param ewkt: OGC Extended WKT string column to generate from.
     :type ewkt: ColumnOrName
@@ -271,27 +261,31 @@
     :type delimiter: ColumnOrName
     :return: Polygon geometry column generated from the list of coordinates.
     :rtype: Column
     """
     return _call_constructor_function("ST_PolygonFromText", (coords, delimiter))
 
 @validate_argument_types
-def ST_MPolyFromText(wkt: ColumnOrName) -> Column:
+def ST_MPolyFromText(wkt: ColumnOrName, srid: Optional[ColumnOrNameOrNumber] = None) -> Column:
     """Generate multiPolygon geometry from a multiPolygon WKT representation.
 
     :param wkt: multiPolygon WKT string column to generate from.
     :type wkt: ColumnOrName
     :return: multiPolygon geometry generated from the wkt column.
     :rtype: Column
     """
-    return _call_constructor_function("ST_MPolyFromText", wkt)
+    args = (wkt) if srid is None else (wkt, srid)
+
+    return _call_constructor_function("ST_MPolyFromText", args)
 
 @validate_argument_types
-def ST_MLineFromText(wkt: ColumnOrName) -> Column:
+def ST_MLineFromText(wkt: ColumnOrName, srid: Optional[ColumnOrNameOrNumber] = None) -> Column:
     """Generate multiLineString geometry from a multiLineString WKT representation.
 
     :param wkt: multiLineString WKT string column to generate from.
     :type wkt: ColumnOrName
     :return: multiLineString geometry generated from the wkt column.
     :rtype: Column
     """
-    return _call_constructor_function("ST_MLineFromText", wkt)
+    args = (wkt) if srid is None else (wkt, srid)
+
+    return _call_constructor_function("ST_MLineFromText", args)
```

### Comparing `apache-sedona-1.5.1/sedona/sql/st_functions.py` & `apache_sedona-1.5.2/sedona/sql/st_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,132 +10,28 @@
 #
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
+import inspect
+import sys
 
 from functools import partial
 from typing import Optional, Union
 
 from pyspark.sql import Column
 
 from sedona.sql.dataframe_api import call_sedona_function, ColumnOrName, ColumnOrNameOrNumber, validate_argument_types
 
 
-__all__ = [
-    "GeometryType",
-    "ST_3DDistance",
-    "ST_AddPoint",
-    "ST_Area",
-    "ST_AreaSpheroid",
-    "ST_AsBinary",
-    "ST_AsEWKB",
-    "ST_AsEWKT",
-    "ST_AsGeoJSON",
-    "ST_AsGML",
-    "ST_AsKML",
-    "ST_AsText",
-    "ST_Azimuth",
-    "ST_Boundary",
-    "ST_Buffer",
-    "ST_BuildArea",
-    "ST_Centroid",
-    "ST_Collect",
-    "ST_CollectionExtract",
-    "ST_ClosestPoint",
-    "ST_ConcaveHull",
-    "ST_ConvexHull",
-    "ST_Difference",
-    "ST_Dimension",
-    "ST_Distance",
-    "ST_DistanceSphere",
-    "ST_DistanceSpheroid",
-    "ST_Dump",
-    "ST_DumpPoints",
-    "ST_EndPoint",
-    "ST_Envelope",
-    "ST_ExteriorRing",
-    "ST_FlipCoordinates",
-    "ST_Force_2D",
-    "ST_GeoHash",
-    "ST_GeometricMedian",
-    "ST_GeometryN",
-    "ST_GeometryType",
-    "ST_H3CellDistance",
-    "ST_H3CellIDs",
-    "ST_H3KRing",
-    "ST_H3ToGeom",
-    "ST_InteriorRingN",
-    "ST_Intersection",
-    "ST_IsClosed",
-    "ST_IsEmpty",
-    "ST_IsRing",
-    "ST_IsSimple",
-    "ST_IsValid",
-    "ST_IsValidReason",
-    "ST_Length",
-    "ST_LengthSpheroid",
-    "ST_LineFromMultiPoint",
-    "ST_LineInterpolatePoint",
-    "ST_LineLocatePoint",
-    "ST_LineMerge",
-    "ST_LineSubstring",
-    "ST_MakeLine",
-    "ST_Polygon"
-    "ST_MakePolygon",
-    "ST_MakeValid",
-    "ST_MinimumBoundingCircle",
-    "ST_MinimumBoundingRadius",
-    "ST_Multi",
-    "ST_Normalize",
-    "ST_NPoints",
-    "ST_NDims",
-    "ST_NumGeometries",
-    "ST_NumInteriorRings",
-    "ST_PointN",
-    "ST_PointOnSurface",
-    "ST_ReducePrecision",
-    "ST_RemovePoint",
-    "ST_Reverse",
-    "ST_S2CellIDs",
-    "ST_SetPoint",
-    "ST_SetSRID",
-    "ST_SRID",
-    "ST_Split",
-    "ST_StartPoint",
-    "ST_SubDivide",
-    "ST_SubDivideExplode",
-    "ST_SimplifyPreserveTopology",
-    "ST_SymDifference",
-    "ST_Transform",
-    "ST_Union",
-    "ST_X",
-    "ST_XMax",
-    "ST_XMin",
-    "ST_Y",
-    "ST_YMax",
-    "ST_YMin",
-    "ST_Z",
-    "ST_ZMax",
-    "ST_ZMin",
-    "ST_NumPoints",
-    "ST_Force3D",
-    "ST_NRings",
-    "ST_Translate",
-    "ST_VoronoiPolygons",
-    "ST_Angle",
-    "ST_Degrees",
-    "ST_FrechetDistance",
-    "ST_CoordDim",
-    "ST_IsCollection",
-    "ST_Affine",
-    "ST_BoundingDiagonal"
-]
+# Automatically populate __all__
+__all__ = [name for name, obj in inspect.getmembers(sys.modules[__name__])
+           if inspect.isfunction(obj)]
 
 
 _call_st_function = partial(call_sedona_function, "st_functions")
 
 @validate_argument_types
 def GeometryType(geometry: ColumnOrName):
     """Return the type of the geometry as a string.
@@ -1253,15 +1149,15 @@
     :param input: One geometry column to use.
     :type input: ColumnOrName
     :param blade: Other geometry column to use.
     :type blase: ColumnOrName
     :return: Multi-geometry representing the split of input by blade.
     :rtype: Column
     """
-    return _call_st_function("ST_SymDifference", (input, blade))
+    return _call_st_function("ST_Split", (input, blade))
 
 
 @validate_argument_types
 def ST_SymDifference(a: ColumnOrName, b: ColumnOrName) -> Column:
     """Calculate the symmetric difference of two geometries (the regions that are only in one of them).
 
     :param a: One geometry column to use.
@@ -1476,14 +1372,15 @@
     :param extendTo: If a geometry is supplied as the "extend_to" parameter, the diagram will be extended to cover the envelope of the "extend_to" geometry, unless that envelope is smaller than the default envelope
     (default = NULL, default envelope is boundingbox of input geometry extended by about 50% in each direction).
     :return: The two-dimensional Voronoi diagram geometry.
     """
     args = (geometry, tolerance, extendTo)
     return _call_st_function("ST_VoronoiPolygons", args)
 
+@validate_argument_types
 def ST_FrechetDistance(g1: ColumnOrName, g2: ColumnOrName) -> Column:
     """
     Computes discrete frechet distance between the two geometries.
     If any of the geometry is empty, ST_FrechetDistance returns 0
     :param g1:
     :param g2:
     :return: Computed Discrete Frechet Distance between g1 and g2
@@ -1518,15 +1415,15 @@
     :return: Geometry with affine transformation applied
     """
     args = (geometry, a, b, d, e, xOff, yOff)
     if not [x for x in (c, f, g, h, i, zOff) if x is None]:
         args = (geometry, a, b, c, d, e, f, g, h, i, xOff, yOff, zOff)
     return _call_st_function("ST_Affine", args)
 
-
+@validate_argument_types
 def ST_BoundingDiagonal(geometry: ColumnOrName) -> Column:
     """
     Returns a LineString with the min/max values of each dimension of the bounding box of the given geometry as its
     start/end coordinates.
     :param geometry: Geometry to return bounding diagonal of.
     :return: LineString spanning min and max values of each dimension of the given geometry
     """
```

### Comparing `apache-sedona-1.5.1/sedona/sql/st_predicates.py` & `apache_sedona-1.5.2/sedona/sql/st_predicates.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,35 +10,28 @@
 #
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
+import inspect
+import sys
 
 from functools import partial
 
 from pyspark.sql import Column
 from typing import Union
 
 from sedona.sql.dataframe_api import ColumnOrName, call_sedona_function, validate_argument_types
 
 
-__all__ = [
-    "ST_Contains",
-    "ST_Crosses",
-    "ST_Disjoint",
-    "ST_Equals",
-    "ST_Intersects",
-    "ST_OrderingEquals",
-    "ST_Overlaps",
-    "ST_Touches",
-    "ST_Within",
-    "ST_DWithin"
-]
+# Automatically populate __all__
+__all__ = [name for name, obj in inspect.getmembers(sys.modules[__name__])
+           if inspect.isfunction(obj)]
 
 
 _call_predicate_function = partial(call_sedona_function, "st_predicates")
 
 
 @validate_argument_types
 def ST_Contains(a: ColumnOrName, b: ColumnOrName) -> Column:
```

### Comparing `apache-sedona-1.5.1/sedona/sql/types.py` & `apache_sedona-1.5.2/sedona/sql/types.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/__init__.py` & `apache_sedona-1.5.2/sedona/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/abstract_parser.py` & `apache_sedona-1.5.2/sedona/utils/abstract_parser.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/adapter.py` & `apache_sedona-1.5.2/sedona/utils/adapter.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/binary_parser.py` & `apache_sedona-1.5.2/sedona/utils/binary_parser.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/decorators.py` & `apache_sedona-1.5.2/sedona/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/geometry_adapter.py` & `apache_sedona-1.5.2/sedona/utils/geometry_adapter.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/geometry_serde.py` & `apache_sedona-1.5.2/sedona/utils/geometry_serde.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/geometry_serde_general.py` & `apache_sedona-1.5.2/sedona/utils/geometry_serde_general.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/jvm.py` & `apache_sedona-1.5.2/sedona/utils/jvm.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/meta.py` & `apache_sedona-1.5.2/sedona/utils/meta.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/prep.py` & `apache_sedona-1.5.2/sedona/utils/prep.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/serde.py` & `apache_sedona-1.5.2/sedona/utils/serde.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/spatial_rdd_parser.py` & `apache_sedona-1.5.2/sedona/utils/spatial_rdd_parser.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/utils/types.py` & `apache_sedona-1.5.2/sedona/utils/types.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/sedona/version.py` & `apache_sedona-1.5.2/sedona/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-version = "1.5.1"
+version = "1.5.2"
```

### Comparing `apache-sedona-1.5.1/setup.py` & `apache_sedona-1.5.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -49,15 +49,20 @@
     author_email='dev@sedona.apache.org',
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     ext_modules=ext_modules,
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires='>=3.6',
     install_requires=['attrs', "shapely>=1.7.0"],
-    extras_require={"spark": ['pyspark>=2.3.0']},
+    extras_require={
+        "spark": ["pyspark>=2.3.0"],
+        "pydeck-map": ["pandas<=1.3.5", "geopandas<=0.10.2", "pydeck==0.8.0"],
+        "kepler-map": ["pandas<=1.3.5", "geopandas<=0.10.2", "keplergl==0.3.2"],
+        "all": ["pyspark>=2.3.0", "pandas<=1.3.5", "geopandas<=0.10.2","pydeck==0.8.0", "keplergl==0.3.2"],
+    },
     project_urls={
         'Documentation': 'https://sedona.apache.org',
         'Source code': 'https://github.com/apache/sedona',
         'Bug Reports': 'https://issues.apache.org/jira/projects/SEDONA'
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `apache-sedona-1.5.1/src/geom_buf.c` & `apache_sedona-1.5.2/src/geom_buf.c`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/src/geom_buf.h` & `apache_sedona-1.5.2/src/geom_buf.h`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/src/geomserde.c` & `apache_sedona-1.5.2/src/geomserde.c`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/src/geomserde.h` & `apache_sedona-1.5.2/src/geomserde.h`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/src/geomserde_speedup_module.c` & `apache_sedona-1.5.2/src/geomserde_speedup_module.c`

 * *Files 5% similar despite different names*

```diff
@@ -188,29 +188,41 @@
   *out_handle = handle;
   return geom;
 }
 
 /* serialize/deserialize functions for Shapely 2.x */
 
 static PyObject *serialize(PyObject *self, PyObject *args) {
-  PyObject *pygeos_geom = NULL;
-  if (!PyArg_ParseTuple(args, "O", &pygeos_geom)) {
-    return NULL;
-  }
-
-  GEOSGeometry *geos_geom = NULL;
-  char success = PyGEOS_GetGEOSGeometry(pygeos_geom, &geos_geom);
-  if (success == 0) {
-    PyErr_SetString(
-        PyExc_TypeError,
-        "Argument is of incorrect type. Please provide only Geometry objects.");
-    return NULL;
-  }
+    PyObject *pygeos_geom = NULL;
+    if (!PyArg_ParseTuple(args, "O", &pygeos_geom)) {
+        return NULL;  // Argument parsing failed; error already set by PyArg_ParseTuple
+    }
 
-  return do_serialize(geos_geom);
+    GEOSGeometry *geos_geom = NULL;
+    char success = PyGEOS_GetGEOSGeometry(pygeos_geom, &geos_geom);
+    if (success == 0) {
+        // Retrieve the type of the supplied object
+        PyObject *type = (PyObject *)Py_TYPE(pygeos_geom);
+        PyObject *type_name = PyObject_GetAttrString(type, "__name__");
+        if (type_name == NULL) {
+            // Fallback error if we can't get the type name
+            PyErr_SetString(PyExc_TypeError, "Argument is of incorrect type.");
+        } else {
+            // Construct the error message with the type name
+            const char *type_str = PyUnicode_AsUTF8(type_name);
+            char error_msg[256];
+            snprintf(error_msg, sizeof(error_msg), "Argument is of incorrect type: '%s'. Please provide only Geometry objects.", type_str);
+
+            PyErr_SetString(PyExc_TypeError, error_msg);
+            Py_DECREF(type_name);  // Cleanup the reference to type_name
+        }
+        return NULL;
+    }
+
+    return do_serialize(geos_geom);
 }
 
 static PyObject *deserialize(PyObject *self, PyObject *args) {
   GEOSContextHandle_t handle = NULL;
   int length = 0;
   GEOSGeometry *geom = do_deserialize(args, &handle, &length);
   if (geom == NULL) {
```

### Comparing `apache-sedona-1.5.1/src/geos_c_dyn.c` & `apache_sedona-1.5.2/src/geos_c_dyn.c`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/src/geos_c_dyn.h` & `apache_sedona-1.5.2/src/geos_c_dyn.h`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/src/geos_c_dyn_funcs.h` & `apache_sedona-1.5.2/src/geos_c_dyn_funcs.h`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/src/pygeos/c_api.h` & `apache_sedona-1.5.2/src/pygeos/c_api.h`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/tests/test_assign_raw_spatial_rdd.py` & `apache_sedona-1.5.2/tests/test_assign_raw_spatial_rdd.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/tests/test_base.py` & `apache_sedona-1.5.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/tests/test_circle.py` & `apache_sedona-1.5.2/tests/test_circle.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/tests/test_multiple_meta.py` & `apache_sedona-1.5.2/tests/test_multiple_meta.py`

 * *Files identical despite different names*

### Comparing `apache-sedona-1.5.1/tests/test_scala_example.py` & `apache_sedona-1.5.2/tests/test_scala_example.py`

 * *Files identical despite different names*

