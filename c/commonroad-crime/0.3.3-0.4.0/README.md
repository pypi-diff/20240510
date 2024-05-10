# Comparing `tmp/commonroad-crime-0.3.3.tar.gz` & `tmp/commonroad_crime-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonroad-crime-0.3.3.tar", last modified: Sat Mar 16 10:54:54 2024, max compression
+gzip compressed data, was "commonroad_crime-0.4.0.tar", last modified: Fri May 10 15:30:48 2024, max compression
```

## Comparing `commonroad-crime-0.3.3.tar` & `commonroad_crime-0.4.0.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.384432 commonroad-crime-0.3.3/
--rw-rw-rw-   0 root         (0) root         (0)     1570 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6307 2024-03-16 10:54:54.384432 commonroad-crime-0.3.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4892 2024-03-16 10:40:37.000000 commonroad-crime-0.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.376433 commonroad-crime-0.3.3/commonroad_crime/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-16 10:54:01.000000 commonroad-crime-0.3.3/commonroad_crime/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-03-16 10:31:51.000000 commonroad-crime-0.3.3/commonroad_crime/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.376433 commonroad-crime-0.3.3/commonroad_crime/data_structure/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-16 10:54:01.000000 commonroad-crime-0.3.3/commonroad_crime/data_structure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9358 2024-03-16 10:23:27.000000 commonroad-crime-0.3.3/commonroad_crime/data_structure/base.py
--rw-rw-rw-   0 root         (0) root         (0)    16248 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/data_structure/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2024-03-16 09:37:51.000000 commonroad-crime-0.3.3/commonroad_crime/data_structure/crime_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/data_structure/scene.py
--rw-rw-rw-   0 root         (0) root         (0)     2692 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/data_structure/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.376433 commonroad-crime-0.3.3/commonroad_crime/measure/
--rw-rw-rw-   0 root         (0) root         (0)     1273 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.376433 commonroad-crime-0.3.3/commonroad_crime/measure/acceleration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-16 10:54:01.000000 commonroad-crime-0.3.3/commonroad_crime/measure/acceleration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5421 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/acceleration/a_lat_req.py
--rw-rw-rw-   0 root         (0) root         (0)     4478 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/acceleration/a_long_req.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/acceleration/a_req.py
--rw-rw-rw-   0 root         (0) root         (0)     2852 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/acceleration/dst.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.376433 commonroad-crime-0.3.3/commonroad_crime/measure/distance/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-16 10:54:01.000000 commonroad-crime-0.3.3/commonroad_crime/measure/distance/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4738 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/distance/dce.py
--rw-rw-rw-   0 root         (0) root         (0)     3473 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/distance/hw.py
--rw-rw-rw-   0 root         (0) root         (0)     4539 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/distance/msd.py
--rw-rw-rw-   0 root         (0) root         (0)     7101 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/distance/psd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.376433 commonroad-crime-0.3.3/commonroad_crime/measure/index/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-16 10:54:01.000000 commonroad-crime-0.3.3/commonroad_crime/measure/index/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/index/aci.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/index/btn.py
--rw-rw-rw-   0 root         (0) root         (0)     8391 2024-03-16 09:37:51.000000 commonroad-crime-0.3.3/commonroad_crime/measure/index/ci.py
--rw-rw-rw-   0 root         (0) root         (0)     5266 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/index/cpi.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/index/pri.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/index/rss.py
--rw-rw-rw-   0 root         (0) root         (0)    10360 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/index/soi.py
--rw-rw-rw-   0 root         (0) root         (0)     2103 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/index/stn.py
--rw-rw-rw-   0 root         (0) root         (0)     2855 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/index/tci.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.376433 commonroad-crime-0.3.3/commonroad_crime/measure/jerk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-16 10:54:01.000000 commonroad-crime-0.3.3/commonroad_crime/measure/jerk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1929 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/jerk/lat_j.py
--rw-rw-rw-   0 root         (0) root         (0)     2042 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/jerk/long_j.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.380432 commonroad-crime-0.3.3/commonroad_crime/measure/potential/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-16 10:54:01.000000 commonroad-crime-0.3.3/commonroad_crime/measure/potential/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15926 2024-03-16 09:37:51.000000 commonroad-crime-0.3.3/commonroad_crime/measure/potential/pf.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/potential/sp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.380432 commonroad-crime-0.3.3/commonroad_crime/measure/probability/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-16 10:54:01.000000 commonroad-crime-0.3.3/commonroad_crime/measure/probability/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7308 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/probability/p_mc.py
--rw-rw-rw-   0 root         (0) root         (0)      997 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/probability/p_smh.py
--rw-rw-rw-   0 root         (0) root         (0)      997 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/probability/p_srs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.380432 commonroad-crime-0.3.3/commonroad_crime/measure/reachable_set/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-16 10:54:01.000000 commonroad-crime-0.3.3/commonroad_crime/measure/reachable_set/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4834 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/reachable_set/drivable_area.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.380432 commonroad-crime-0.3.3/commonroad_crime/measure/time/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-16 10:54:01.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/ags.py
--rw-rw-rw-   0 root         (0) root         (0)    16392 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/et.py
--rw-rw-rw-   0 root         (0) root         (0)    11308 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/pet.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/pttc.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/tc.py
--rw-rw-rw-   0 root         (0) root         (0)     2027 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/tet.py
--rw-rw-rw-   0 root         (0) root         (0)     4531 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/thw.py
--rw-rw-rw-   0 root         (0) root         (0)     3877 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/tit.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/ttb.py
--rw-rw-rw-   0 root         (0) root         (0)     5649 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/ttc.py
--rw-rw-rw-   0 root         (0) root         (0)     6565 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/ttc_star.py
--rw-rw-rw-   0 root         (0) root         (0)     2437 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/ttce.py
--rw-rw-rw-   0 root         (0) root         (0)      693 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/ttk.py
--rw-rw-rw-   0 root         (0) root         (0)     7196 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/ttm.py
--rw-rw-rw-   0 root         (0) root         (0)     2764 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/ttr.py
--rw-rw-rw-   0 root         (0) root         (0)     2555 2024-03-16 09:37:51.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/tts.py
--rw-rw-rw-   0 root         (0) root         (0)     6570 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/ttz.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/tv.py
--rw-rw-rw-   0 root         (0) root         (0)     5618 2024-03-16 09:37:51.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/wttc.py
--rw-rw-rw-   0 root         (0) root         (0)     6552 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/time/wttr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.380432 commonroad-crime-0.3.3/commonroad_crime/measure/velocity/
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/velocity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      987 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/velocity/cs.py
--rw-rw-rw-   0 root         (0) root         (0)     3148 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/measure/velocity/delta_v.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.380432 commonroad-crime-0.3.3/commonroad_crime/utility/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-16 10:54:01.000000 commonroad-crime-0.3.3/commonroad_crime/utility/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10350 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/utility/batch_evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     8195 2024-03-16 08:57:32.000000 commonroad-crime-0.3.3/commonroad_crime/utility/general.py
--rw-rw-rw-   0 root         (0) root         (0)     1843 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/utility/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    10662 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/utility/optimization.py
--rw-rw-rw-   0 root         (0) root         (0)    34806 2024-03-16 09:37:51.000000 commonroad-crime-0.3.3/commonroad_crime/utility/simulation.py
--rw-rw-rw-   0 root         (0) root         (0)    14082 2024-03-16 10:23:27.000000 commonroad-crime-0.3.3/commonroad_crime/utility/solver.py
--rw-rw-rw-   0 root         (0) root         (0)     9483 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/commonroad_crime/utility/visualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.384432 commonroad-crime-0.3.3/commonroad_crime.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6307 2024-03-16 10:54:54.000000 commonroad-crime-0.3.3/commonroad_crime.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3520 2024-03-16 10:54:54.000000 commonroad-crime-0.3.3/commonroad_crime.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-16 10:54:54.000000 commonroad-crime-0.3.3/commonroad_crime.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      300 2024-03-16 10:54:54.000000 commonroad-crime-0.3.3/commonroad_crime.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-16 10:54:54.000000 commonroad-crime-0.3.3/commonroad_crime.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-16 10:54:54.384432 commonroad-crime-0.3.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1922 2024-03-16 08:54:41.000000 commonroad-crime-0.3.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-16 10:54:54.384432 commonroad-crime-0.3.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1709 2024-03-14 18:08:10.000000 commonroad-crime-0.3.3/tests/test_acceleration_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     1659 2024-03-16 08:32:01.000000 commonroad-crime-0.3.3/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1915 2024-03-14 18:08:10.000000 commonroad-crime-0.3.3/tests/test_distance_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     3509 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/tests/test_index_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     1428 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/tests/test_jerk_domain.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/tests/test_potential_domain.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/tests/test_probability_domain.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/tests/test_reachable_set_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     9902 2024-03-16 09:37:51.000000 commonroad-crime-0.3.3/tests/test_time_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     6816 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/tests/test_utils_simulation.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2024-03-14 17:14:19.000000 commonroad-crime-0.3.3/tests/test_velocity_domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.724271 commonroad_crime-0.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6805 2024-05-10 15:30:48.724271 commonroad_crime-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5386 2024-05-10 15:23:42.000000 commonroad_crime-0.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.632274 commonroad_crime-0.4.0/commonroad_crime/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-10 14:43:51.000000 commonroad_crime-0.4.0/commonroad_crime/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.640273 commonroad_crime-0.4.0/commonroad_crime/data_structure/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/data_structure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11885 2024-04-23 13:52:54.000000 commonroad_crime-0.4.0/commonroad_crime/data_structure/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    16249 2024-03-22 09:23:05.000000 commonroad_crime-0.4.0/commonroad_crime/data_structure/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     7182 2024-05-09 05:22:09.000000 commonroad_crime-0.4.0/commonroad_crime/data_structure/crime_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/data_structure/scene.py
+-rw-rw-rw-   0 root         (0) root         (0)     2692 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/data_structure/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.644273 commonroad_crime-0.4.0/commonroad_crime/measure/
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.648273 commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5873 2024-04-08 15:17:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/a_lat_req.py
+-rw-rw-rw-   0 root         (0) root         (0)     5015 2024-04-08 15:17:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/a_long_req.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/a_req.py
+-rw-rw-rw-   0 root         (0) root         (0)     2731 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/dst.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.652273 commonroad_crime-0.4.0/commonroad_crime/measure/distance/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/distance/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4732 2024-05-10 14:43:51.000000 commonroad_crime-0.4.0/commonroad_crime/measure/distance/dce.py
+-rw-rw-rw-   0 root         (0) root         (0)     3882 2024-05-10 14:43:51.000000 commonroad_crime-0.4.0/commonroad_crime/measure/distance/hw.py
+-rw-rw-rw-   0 root         (0) root         (0)     4444 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/distance/msd.py
+-rw-rw-rw-   0 root         (0) root         (0)     6952 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/distance/psd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.664273 commonroad_crime-0.4.0/commonroad_crime/measure/index/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/aci.py
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/btn.py
+-rw-rw-rw-   0 root         (0) root         (0)     8272 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     5110 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/cpi.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/pri.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/rss.py
+-rw-rw-rw-   0 root         (0) root         (0)    10267 2024-04-28 15:00:45.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/soi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1983 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/stn.py
+-rw-rw-rw-   0 root         (0) root         (0)     2779 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/tci.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.664273 commonroad_crime-0.4.0/commonroad_crime/measure/jerk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/jerk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1853 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/jerk/lat_j.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/jerk/long_j.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.668273 commonroad_crime-0.4.0/commonroad_crime/measure/potential/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/potential/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16293 2024-04-15 08:47:41.000000 commonroad_crime-0.4.0/commonroad_crime/measure/potential/pf.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/potential/sp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.672273 commonroad_crime-0.4.0/commonroad_crime/measure/probability/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/probability/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7488 2024-05-10 14:43:51.000000 commonroad_crime-0.4.0/commonroad_crime/measure/probability/p_mc.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/probability/p_smh.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/probability/p_srs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.676272 commonroad_crime-0.4.0/commonroad_crime/measure/reachable_set/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/reachable_set/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4945 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/reachable_set/drivable_area.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.696272 commonroad_crime-0.4.0/commonroad_crime/measure/time/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ags.py
+-rw-rw-rw-   0 root         (0) root         (0)    16262 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/et.py
+-rw-rw-rw-   0 root         (0) root         (0)    11178 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/pet.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/pttc.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/tc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/tet.py
+-rw-rw-rw-   0 root         (0) root         (0)     5928 2024-05-08 22:38:38.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/thw.py
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/tit.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttb.py
+-rw-rw-rw-   0 root         (0) root         (0)     6677 2024-04-08 15:29:07.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6490 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttc_star.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2024-04-28 15:03:44.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttce.py
+-rw-rw-rw-   0 root         (0) root         (0)      693 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttk.py
+-rw-rw-rw-   0 root         (0) root         (0)     7121 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2024-03-19 15:06:10.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttr.py
+-rw-rw-rw-   0 root         (0) root         (0)     2630 2024-03-19 15:06:10.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/tts.py
+-rw-rw-rw-   0 root         (0) root         (0)     6606 2024-05-08 22:38:38.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttz.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/tv.py
+-rw-rw-rw-   0 root         (0) root         (0)     5479 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/wttc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6475 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/wttr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.700272 commonroad_crime-0.4.0/commonroad_crime/measure/velocity/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/velocity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/velocity/cs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3009 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/velocity/delta_v.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.708272 commonroad_crime-0.4.0/commonroad_crime/utility/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/utility/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10350 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/utility/batch_evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8463 2024-03-19 12:50:18.000000 commonroad_crime-0.4.0/commonroad_crime/utility/general.py
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/utility/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    10662 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/utility/optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)    34806 2024-03-16 09:37:51.000000 commonroad_crime-0.4.0/commonroad_crime/utility/simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)    14569 2024-05-08 22:38:38.000000 commonroad_crime-0.4.0/commonroad_crime/utility/solver.py
+-rw-rw-rw-   0 root         (0) root         (0)    11746 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/utility/visualization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.720271 commonroad_crime-0.4.0/commonroad_crime.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6805 2024-05-10 15:30:48.000000 commonroad_crime-0.4.0/commonroad_crime.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3538 2024-05-10 15:30:48.000000 commonroad_crime-0.4.0/commonroad_crime.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 15:30:48.000000 commonroad_crime-0.4.0/commonroad_crime.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      296 2024-05-10 15:30:48.000000 commonroad_crime-0.4.0/commonroad_crime.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-10 15:30:48.000000 commonroad_crime-0.4.0/commonroad_crime.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 15:30:48.724271 commonroad_crime-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-05-10 15:12:38.000000 commonroad_crime-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.720271 commonroad_crime-0.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2024-04-29 15:24:25.000000 commonroad_crime-0.4.0/tests/test_acceleration_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3614 2024-05-09 05:22:09.000000 commonroad_crime-0.4.0/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1915 2024-03-14 18:08:10.000000 commonroad_crime-0.4.0/tests/test_distance_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3794 2024-04-29 15:24:25.000000 commonroad_crime-0.4.0/tests/test_index_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2024-04-29 15:24:25.000000 commonroad_crime-0.4.0/tests/test_jerk_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      936 2024-04-29 15:24:25.000000 commonroad_crime-0.4.0/tests/test_potential_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2024-04-29 15:24:25.000000 commonroad_crime-0.4.0/tests/test_probability_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/tests/test_reachable_set_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     9902 2024-03-16 09:37:51.000000 commonroad_crime-0.4.0/tests/test_time_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     6816 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/tests/test_utils_simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-29 15:24:25.000000 commonroad_crime-0.4.0/tests/test_velocity_domain.py
```

### Comparing `commonroad-crime-0.3.3/LICENSE` & `commonroad_crime-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/PKG-INFO` & `commonroad_crime-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 636f 6d6d  : 2.1.Name: comm
 00000020: 6f6e 726f 6164 2d63 7269 6d65 0a56 6572  onroad-crime.Ver
-00000030: 7369 6f6e 3a20 302e 332e 330a 5375 6d6d  sion: 0.3.3.Summ
+00000030: 7369 6f6e 3a20 302e 342e 300a 5375 6d6d  sion: 0.4.0.Summ
 00000040: 6172 793a 2063 7269 7469 6361 6c69 7479  ary: criticality
 00000050: 206d 6561 7375 7265 7320 6f66 2061 7574   measures of aut
 00000060: 6f6d 6174 6564 2076 6568 6963 6c65 730a  omated vehicles.
 00000070: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
 00000080: 3a2f 2f63 6f6d 6d6f 6e72 6f61 642e 696e  ://commonroad.in
 00000090: 2e74 756d 2e64 652f 746f 6f6c 732f 636f  .tum.de/tools/co
 000000a0: 6d6d 6f6e 726f 6164 2d63 7269 6d65 0a41  mmonroad-crime.A
@@ -15,381 +15,412 @@
 000000e0: 696c 3a20 636f 6d6d 6f6e 726f 6164 406c  il: commonroad@l
 000000f0: 6973 7473 2e6c 727a 2e64 650a 4c69 6365  ists.lrz.de.Lice
 00000100: 6e73 653a 2042 5344 2033 2d43 6c61 7573  nse: BSD 3-Claus
 00000110: 650a 5072 6f6a 6563 742d 5552 4c3a 2044  e.Project-URL: D
 00000120: 6f63 756d 656e 7461 7469 6f6e 2c20 6874  ocumentation, ht
 00000130: 7470 733a 2f2f 6370 732e 7061 6765 732e  tps://cps.pages.
 00000140: 6769 746c 6162 2e6c 727a 2e64 652f 636f  gitlab.lrz.de/co
-00000150: 6d6d 6f6e 726f 6164 2d63 7269 7469 6361  mmonroad-critica
-00000160: 6c69 7479 2d6d 6561 7375 7265 732f 0a50  lity-measures/.P
-00000170: 726f 6a65 6374 2d55 524c 3a20 466f 7275  roject-URL: Foru
-00000180: 6d2c 2068 7474 7073 3a2f 2f63 6f6d 6d6f  m, https://commo
-00000190: 6e72 6f61 642e 696e 2e74 756d 2e64 652f  nroad.in.tum.de/
-000001a0: 666f 7275 6d2f 632f 636f 6d6d 6f6e 726f  forum/c/commonro
-000001b0: 6164 2d63 7269 6d65 2f32 300a 5072 6f6a  ad-crime/20.Proj
-000001c0: 6563 742d 5552 4c3a 2053 6f75 7263 652c  ect-URL: Source,
-000001d0: 2068 7474 7073 3a2f 2f67 6974 6c61 622e   https://gitlab.
-000001e0: 6c72 7a2e 6465 2f74 756d 2d63 7073 2f63  lrz.de/tum-cps/c
-000001f0: 6f6d 6d6f 6e72 6f61 642d 6372 696d 650a  ommonroad-crime.
-00000200: 4b65 7977 6f72 6473 3a20 6372 6974 6963  Keywords: critic
-00000210: 616c 6974 792c 6175 746f 6e6f 6d6f 7573  ality,autonomous
-00000220: 2064 7269 7669 6e67 0a43 6c61 7373 6966   driving.Classif
-00000230: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000240: 204c 616e 6775 6167 6520 3a3a 2043 2b2b   Language :: C++
-00000250: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000260: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000270: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000280: 2e38 0a43 6c61 7373 6966 6965 723a 2050  .8.Classifier: P
-00000290: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002b0: 2033 2e39 0a43 6c61 7373 6966 6965 723a   3.9.Classifier:
-000002c0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000002d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002e0: 3a3a 2033 2e31 300a 436c 6173 7369 6669  :: 3.10.Classifi
-000002f0: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
-00000300: 5349 2041 7070 726f 7665 6420 3a3a 2042  SI Approved :: B
-00000310: 5344 204c 6963 656e 7365 0a43 6c61 7373  SD License.Class
-00000320: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-00000330: 2053 7973 7465 6d20 3a3a 2050 4f53 4958   System :: POSIX
-00000340: 203a 3a20 4c69 6e75 780a 4465 7363 7269   :: Linux.Descri
-00000350: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000360: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000370: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
-00000380: 4c49 4345 4e53 450a 5265 7175 6972 6573  LICENSE.Requires
-00000390: 2d44 6973 743a 2063 6f6d 6d6f 6e72 6f61  -Dist: commonroa
-000003a0: 642d 696f 3e3d 3230 3233 2e34 0a52 6571  d-io>=2023.4.Req
-000003b0: 7569 7265 732d 4469 7374 3a20 636f 6d6d  uires-Dist: comm
-000003c0: 6f6e 726f 6164 2d76 6568 6963 6c65 2d6d  onroad-vehicle-m
-000003d0: 6f64 656c 733e 3d33 2e30 2e30 0a52 6571  odels>=3.0.0.Req
-000003e0: 7569 7265 732d 4469 7374 3a20 636f 6d6d  uires-Dist: comm
-000003f0: 6f6e 726f 6164 2d72 6f75 7465 2d70 6c61  onroad-route-pla
-00000400: 6e6e 6572 3c32 3032 342e 312c 3e3d 3230  nner<2024.1,>=20
-00000410: 3232 2e33 0a52 6571 7569 7265 732d 4469  22.3.Requires-Di
-00000420: 7374 3a20 636f 6d6d 6f6e 726f 6164 2d64  st: commonroad-d
-00000430: 7269 7661 6269 6c69 7479 2d63 6865 636b  rivability-check
-00000440: 6572 3e3d 3230 3233 2e31 0a52 6571 7569  er>=2023.1.Requi
-00000450: 7265 732d 4469 7374 3a20 636f 6d6d 6f6e  res-Dist: common
-00000460: 726f 6164 2d72 6561 6368 3e3d 3230 3233  road-reach>=2023
-00000470: 2e31 0a52 6571 7569 7265 732d 4469 7374  .1.Requires-Dist
-00000480: 3a20 6d61 7470 6c6f 746c 6962 3e3d 332e  : matplotlib>=3.
-00000490: 352e 320a 5265 7175 6972 6573 2d44 6973  5.2.Requires-Dis
-000004a0: 743a 206e 756d 7079 3e3d 312e 3139 2e30  t: numpy>=1.19.0
-000004b0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000004c0: 7363 6970 793e 3d31 2e37 2e33 0a52 6571  scipy>=1.7.3.Req
-000004d0: 7569 7265 732d 4469 7374 3a20 7368 6170  uires-Dist: shap
-000004e0: 656c 793c 332e 302e 302c 3e3d 322e 302e  ely<3.0.0,>=2.0.
-000004f0: 310a 5265 7175 6972 6573 2d44 6973 743a  1.Requires-Dist:
-00000500: 206f 6d65 6761 636f 6e66 3e3d 322e 312e   omegaconf>=2.1.
-00000510: 310a 5265 7175 6972 6573 2d44 6973 743a  1.Requires-Dist:
-00000520: 2063 6173 6164 693e 3d33 2e36 2e33 0a52   casadi>=3.6.3.R
-00000530: 6571 7569 7265 732d 4469 7374 3a20 7471  equires-Dist: tq
-00000540: 646d 3e3d 342e 3635 2e30 0a52 6571 7569  dm>=4.65.0.Requi
-00000550: 7265 732d 4469 7374 3a20 696d 6167 6569  res-Dist: imagei
-00000560: 6f3e 3d32 2e39 2e30 0a52 6571 7569 7265  o>=2.9.0.Require
-00000570: 732d 4469 7374 3a20 7079 7465 7374 3e3d  s-Dist: pytest>=
-00000580: 372e 342e 300a 0a23 2043 6f6d 6d6f 6e52  7.4.0..# CommonR
-00000590: 6f61 642d 4372 694d 650a 215b 696d 6167  oad-CriMe.![imag
-000005a0: 6520 696e 666f 5d28 6874 7470 733a 2f2f  e info](https://
-000005b0: 6769 746c 6162 2e6c 727a 2e64 652f 7475  gitlab.lrz.de/tu
-000005c0: 6d2d 6370 732f 636f 6d6d 6f6e 726f 6164  m-cps/commonroad
-000005d0: 2d63 7269 6d65 2f2d 2f72 6177 2f6d 6173  -crime/-/raw/mas
-000005e0: 7465 722f 646f 6373 2f66 6967 7572 6573  ter/docs/figures
-000005f0: 2f43 7269 4d65 2d62 616e 6e65 722e 706e  /CriMe-banner.pn
-00000600: 6729 0a5b 215b 4c69 6e75 785d 2868 7474  g).[![Linux](htt
-00000610: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000620: 2e69 6f2f 6261 6467 652f 6f73 2d6c 696e  .io/badge/os-lin
-00000630: 7578 3f26 6c6f 676f 3d4c 696e 7578 266c  ux?&logo=Linux&l
-00000640: 6f67 6f43 6f6c 6f72 3d77 6869 7465 266c  ogoColor=white&l
-00000650: 6162 656c 436f 6c6f 723d 6772 6179 295d  abelColor=gray)]
-00000660: 2868 7474 7073 3a2f 2f70 7970 692e 7079  (https://pypi.py
-00000670: 7468 6f6e 2e6f 7267 2f70 7970 692f 636f  thon.org/pypi/co
-00000680: 6d6d 6f6e 726f 6164 2d6f 7065 6e73 6365  mmonroad-opensce
-00000690: 6e61 7269 6f2d 636f 6e76 6572 7465 722f  nario-converter/
-000006a0: 290a 5b21 5b50 7950 4920 7665 7273 696f  ).[![PyPI versio
-000006b0: 6e20 6675 7279 2e69 6f5d 2868 7474 7073  n fury.io](https
-000006c0: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
-000006d0: 2f70 792f 636f 6d6d 6f6e 726f 6164 2d63  /py/commonroad-c
-000006e0: 7269 6d65 2e73 7667 3f73 7479 6c65 3d70  rime.svg?style=p
-000006f0: 6c61 7374 6963 295d 2868 7474 7073 3a2f  lastic)](https:/
-00000700: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
-00000710: 2f70 7970 692f 636f 6d6d 6f6e 726f 6164  /pypi/commonroad
-00000720: 2d63 7269 6d65 2f29 0a5b 215b 5079 5049  -crime/).[![PyPI
-00000730: 206c 6963 656e 7365 5d28 6874 7470 733a   license](https:
-00000740: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000750: 2f70 7970 692f 6c2f 636f 6d6d 6f6e 726f  /pypi/l/commonro
-00000760: 6164 2d63 7269 6d65 2e73 7667 3f73 7479  ad-crime.svg?sty
-00000770: 6c65 3d70 6c61 7374 6963 295d 2868 7474  le=plastic)](htt
-00000780: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
-00000790: 2e6f 7267 2f70 7970 692f 636f 6d6d 6f6e  .org/pypi/common
-000007a0: 726f 6164 2d63 7269 6d65 2f29 3c62 723e  road-crime/)<br>
-000007b0: 0a5b 215b 5079 5049 2064 6f77 6e6c 6f61  .[![PyPI downloa
-000007c0: 6420 6d6f 6e74 685d 2868 7474 7073 3a2f  d month](https:/
-000007d0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000007e0: 7079 7069 2f64 6d2f 636f 6d6d 6f6e 726f  pypi/dm/commonro
-000007f0: 6164 2d63 7269 6d65 2e73 7667 3f73 7479  ad-crime.svg?sty
-00000800: 6c65 3d70 6c61 7374 6963 266c 6162 656c  le=plastic&label
-00000810: 3d50 7950 4925 3230 646f 776e 6c6f 6164  =PyPI%20download
-00000820: 7329 5d28 6874 7470 733a 2f2f 7079 7069  s)](https://pypi
-00000830: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
-00000840: 2f63 6f6d 6d6f 6e72 6f61 642d 6372 696d  /commonroad-crim
-00000850: 652f 2920 0a5b 215b 5079 5049 2064 6f77  e/) .[![PyPI dow
-00000860: 6e6c 6f61 6420 7765 656b 5d28 6874 7470  nload week](http
-00000870: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000880: 696f 2f70 7970 692f 6477 2f63 6f6d 6d6f  io/pypi/dw/commo
-00000890: 6e72 6f61 642d 6372 696d 652e 7376 673f  nroad-crime.svg?
-000008a0: 7374 796c 653d 706c 6173 7469 6326 6c61  style=plastic&la
-000008b0: 6265 6c3d 5079 5049 2532 3064 6f77 6e6c  bel=PyPI%20downl
-000008c0: 6f61 6473 295d 2868 7474 7073 3a2f 2f70  oads)](https://p
-000008d0: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
-000008e0: 7970 692f 636f 6d6d 6f6e 726f 6164 2d63  ypi/commonroad-c
-000008f0: 7269 6d65 2f29 3c62 723e 0a0a 546f 6f6c  rime/)<br>..Tool
-00000900: 626f 7820 746f 2063 6f6d 7075 7465 202a  box to compute *
-00000910: 2a43 7269 2a2a 7469 6361 6c69 7479 202a  *Cri**ticality *
-00000920: 2a4d 652a 2a61 7375 7265 7320 0a28 652e  *Me**asures .(e.
-00000930: 672e 2074 696d 652d 746f 2d63 6f6c 6c69  g. time-to-colli
-00000940: 7369 6f6e 2c20 7469 6d65 2d74 6f2d 7265  sion, time-to-re
-00000950: 6163 742c 2e2e 2e29 2e20 5375 6368 206d  act,...). Such m
-00000960: 6561 7375 7265 730a 6361 6e20 6265 2075  easures.can be u
-00000970: 7365 6420 746f 2074 7269 6767 6572 2077  sed to trigger w
-00000980: 6172 6e69 6e67 7320 616e 6420 656d 6572  arnings and emer
-00000990: 6765 6e63 7920 6d61 6e65 7576 6572 7320  gency maneuvers 
-000009a0: 0a69 6e20 6472 6976 6572 2061 7373 6973  .in driver assis
-000009b0: 7461 6e63 6520 7379 7374 656d 7320 6f72  tance systems or
-000009c0: 2072 6570 6169 7220 616e 2069 6e66 6561   repair an infea
-000009d0: 7369 626c 6520 0a74 7261 6a65 6374 6f72  sible .trajector
-000009e0: 792e 200a 0a2d 2049 6620 796f 7520 6861  y. ..- If you ha
-000009f0: 7665 2071 7565 7374 696f 6e73 206f 7220  ve questions or 
-00000a00: 7761 6e74 2074 6f20 7265 706f 7274 2070  want to report p
-00000a10: 726f 626c 656d 7320 6f72 2073 7567 6765  roblems or sugge
-00000a20: 7374 696f 6e73 2c20 706c 6561 7365 2073  stions, please s
-00000a30: 7461 7274 2061 205b 4769 7468 7562 2064  tart a [Github d
-00000a40: 6973 6375 7373 696f 6e5d 2868 7474 7073  iscussion](https
-00000a50: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f72  ://github.com/or
-00000a60: 6773 2f43 6f6d 6d6f 6e52 6f61 642f 6469  gs/CommonRoad/di
-00000a70: 7363 7573 7369 6f6e 7329 2e20 0a0a 2323  scussions). ..##
-00000a80: 2320 f09f 9aa7 2057 6520 4d65 6173 7572  # .... We Measur
-00000a90: 6520 f09d 95ae 6f6d 6d6f 6e20 f09d 95bd  e ....ommon ....
-00000aa0: 6f61 6420 f09d 95ae 7269 f09d 95b8 6521  oad ....ri....e!
-00000ab0: 20f0 9f9a 940a 0a0a 2323 2049 6e73 7461   .......## Insta
-00000ac0: 6c6c 6174 696f 6e20 4775 6964 650a 0a60  llation Guide..`
-00000ad0: 636f 6d6d 6f6e 726f 6164 2d63 7269 6d65  commonroad-crime
-00000ae0: 6020 6361 6e20 6265 2069 6e73 7461 6c6c  ` can be install
-00000af0: 6564 2077 6974 683a 0a0a 6060 6020 6261  ed with:..``` ba
-00000b00: 7368 0a24 2070 6970 2069 6e73 7461 6c6c  sh.$ pip install
-00000b10: 2063 6f6d 6d6f 6e72 6f61 642d 6372 696d   commonroad-crim
-00000b20: 650a 6060 600a 466f 7220 6164 6469 6e67  e.```.For adding
-00000b30: 206e 6577 206d 6561 7375 7265 732c 2077   new measures, w
-00000b40: 6520 7265 636f 6d6d 656e 6420 7573 696e  e recommend usin
-00000b50: 6720 5b41 6e61 636f 6e64 615d 2868 7474  g [Anaconda](htt
-00000b60: 7073 3a2f 2f77 7777 2e61 6e61 636f 6e64  ps://www.anacond
-00000b70: 612e 636f 6d2f 2920 746f 206d 616e 6167  a.com/) to manag
-00000b80: 6520 796f 7572 2065 6e76 6972 6f6e 6d65  e your environme
-00000b90: 6e74 2073 6f20 7468 6174 2065 7665 6e20  nt so that even 
-00000ba0: 6966 2079 6f75 206d 6573 7320 736f 6d65  if you mess some
-00000bb0: 7468 696e 6720 7570 2c20 796f 7520 6361  thing up, you ca
-00000bc0: 6e20 616c 7761 7973 2068 6176 6520 6120  n always have a 
-00000bd0: 7361 6665 2061 6e64 2063 6c65 616e 2072  safe and clean r
-00000be0: 6573 7461 7274 2e20 4120 6775 6964 6520  estart. A guide 
-00000bf0: 666f 7220 6d61 6e61 6769 6e67 2070 7974  for managing pyt
-00000c00: 686f 6e20 656e 7669 726f 6e6d 656e 7473  hon environments
-00000c10: 2077 6974 6820 416e 6163 6f6e 6461 2063   with Anaconda c
-00000c20: 616e 2062 6520 666f 756e 6420 5b68 6572  an be found [her
-00000c30: 655d 2868 7474 7073 3a2f 2f63 6f6e 6461  e](https://conda
-00000c40: 2e69 6f2f 7072 6f6a 6563 7473 2f63 6f6e  .io/projects/con
-00000c50: 6461 2f65 6e2f 6c61 7465 7374 2f75 7365  da/en/latest/use
-00000c60: 722d 6775 6964 652f 7461 736b 732f 6d61  r-guide/tasks/ma
-00000c70: 6e61 6765 2d65 6e76 6972 6f6e 6d65 6e74  nage-environment
-00000c80: 732e 6874 6d6c 292e 0a0a 4166 7465 7220  s.html)...After 
-00000c90: 696e 7374 616c 6c69 6e67 2041 6e61 636f  installing Anaco
-00000ca0: 6e64 612c 2063 7265 6174 6520 6120 6e65  nda, create a ne
-00000cb0: 7720 656e 7669 726f 6e6d 656e 7420 7769  w environment wi
-00000cc0: 7468 3a0a 6060 6020 6261 7368 0a24 2063  th:.``` bash.$ c
-00000cd0: 6f6e 6461 2063 7265 6174 6520 2d6e 2063  onda create -n c
-00000ce0: 6f6d 6d6f 6e72 6f61 642d 7079 3338 2070  ommonroad-py38 p
-00000cf0: 7974 686f 6e3d 332e 3820 2d79 0a60 6060  ython=3.8 -y.```
-00000d00: 0a0a 4865 7265 2074 6865 206e 616d 6520  ..Here the name 
-00000d10: 6f66 2074 6865 2065 6e76 6972 6f6e 6d65  of the environme
-00000d20: 6e74 2069 7320 6361 6c6c 6564 202a 2a63  nt is called **c
-00000d30: 6f6d 6d6f 6e72 6f61 642d 7079 3338 2a2a  ommonroad-py38**
-00000d40: 2e20 596f 7520 6d61 7920 616c 736f 2063  . You may also c
-00000d50: 6861 6e67 6520 7468 6973 206e 616d 6520  hange this name 
-00000d60: 6173 2079 6f75 2077 6973 682e 2049 6e20  as you wish. In 
-00000d70: 7375 6368 2063 6173 652c 2064 6f6e 2774  such case, don't
-00000d80: 2066 6f72 6765 7420 746f 2063 6861 6e67   forget to chang
-00000d90: 6520 6974 2069 6e20 7468 6520 666f 6c6c  e it in the foll
-00000da0: 6f77 696e 6720 636f 6d6d 616e 6473 2061  owing commands a
-00000db0: 7320 7765 6c6c 2e20 2a2a 416c 7761 7973  s well. **Always
-00000dc0: 2061 6374 6976 6174 652a 2a20 7468 6973   activate** this
-00000dd0: 2065 6e76 6972 6f6e 6d65 6e74 2062 6566   environment bef
-00000de0: 6f72 6520 796f 7520 646f 2061 6e79 7468  ore you do anyth
-00000df0: 696e 6720 7265 6c61 7465 643a 0a0a 6060  ing related:..``
-00000e00: 6073 680a 2420 636f 6e64 6120 6163 7469  `sh.$ conda acti
-00000e10: 7661 7465 2063 6f6d 6d6f 6e72 6f61 642d  vate commonroad-
-00000e20: 7079 3338 0a6f 720a 2420 736f 7572 6365  py38.or.$ source
-00000e30: 2061 6374 6976 6174 6520 636f 6d6d 6f6e   activate common
-00000e40: 726f 6164 2d70 7933 380a 6060 600a 5468  road-py38.```.Th
-00000e50: 656e 2c20 696e 7374 616c 6c20 7468 6520  en, install the 
-00000e60: 6465 7065 6e64 656e 6369 6573 2077 6974  dependencies wit
-00000e70: 683a 0a0a 6060 6073 680a 2420 6364 203c  h:..```sh.$ cd <
-00000e80: 7061 7468 2d74 6f2d 7468 6973 2d72 6570  path-to-this-rep
-00000e90: 6f3e 0a24 2070 6970 2069 6e73 7461 6c6c  o>.$ pip install
-00000ea0: 202d 6520 2e0a 2420 636f 6e64 6120 6465   -e ..$ conda de
-00000eb0: 7665 6c6f 7020 2e0a 6060 600a 0a54 6f20  velop ..```..To 
-00000ec0: 7465 7374 2074 6865 2069 6e73 7461 6c6c  test the install
-00000ed0: 6974 696f 6e2c 2072 756e 2075 6e69 7474  ition, run unitt
-00000ee0: 6573 743a 0a60 6060 6261 7368 0a24 2063  est:.```bash.$ c
-00000ef0: 6420 7465 7374 730a 2420 7079 7468 6f6e  d tests.$ python
-00000f00: 202d 6d20 756e 6974 7465 7374 202d 760a   -m unittest -v.
-00000f10: 6060 600a 0a0a 546f 2067 6574 2073 7461  ```...To get sta
-00000f20: 7274 6564 2079 6f75 7220 6a6f 7572 6e65  rted your journe
-00000f30: 7920 7769 7468 206f 7572 2063 7269 7469  y with our criti
-00000f40: 6361 6c69 7479 206d 6561 7375 7265 732c  cality measures,
-00000f50: 2063 6865 636b 2074 6865 2060 7475 746f   check the `tuto
-00000f60: 7269 616c 7360 2061 6e64 2074 6865 2066  rials` and the f
-00000f70: 6f6c 6c6f 7769 6e67 2074 6970 732e 0a0a  ollowing tips...
-00000f80: 2323 2320 486f 7720 746f 2061 6464 206e  ### How to add n
-00000f90: 6577 2063 7269 7469 6361 6c69 7479 206d  ew criticality m
-00000fa0: 6561 7375 7265 0a31 2e20 6372 6561 7465  easure.1. create
-00000fb0: 2061 206e 6577 2062 7261 6e63 6820 7769   a new branch wi
-00000fc0: 7468 2060 6665 6174 7572 652d 3c6d 6561  th `feature-<mea
-00000fd0: 7375 7265 2d6e 616d 653e 6020 616e 6420  sure-name>` and 
-00000fe0: 6368 6563 6b6f 7574 2074 6865 2062 7261  checkout the bra
-00000ff0: 6e63 680a 322e 206e 6176 6967 6174 6520  nch.2. navigate 
-00001000: 746f 2060 636f 6d6d 6f6e 726f 6164 5f63  to `commonroad_c
-00001010: 7269 6d65 2f64 6174 615f 7374 7275 6374  rime/data_struct
-00001020: 7572 652f 7479 7065 2e70 7960 2074 6f20  ure/type.py` to 
-00001030: 6669 6e64 2074 6865 2063 6f72 7265 6374  find the correct
-00001040: 2063 6174 6567 6f72 7920 6f66 2074 6865   category of the
-00001050: 206d 6561 7375 7265 2061 6e64 2061 6464   measure and add
-00001060: 2061 6e20 0a65 6e75 6d65 7261 7469 6f6e   an .enumeration
-00001070: 2065 6e74 7279 2060 3c61 6262 7265 7669   entry `<abbrevi
-00001080: 6174 696f 6e3e 3a20 3c65 7870 6c61 6e61  ation>: <explana
-00001090: 7469 6f6e 3e60 0a33 2e20 6e61 7669 6761  tion>`.3. naviga
-000010a0: 7465 2074 6f20 6063 6f6d 6d6f 6e72 6f61  te to `commonroa
-000010b0: 645f 6372 696d 652f 6d65 6173 7572 6560  d_crime/measure`
-000010c0: 2074 6f20 6669 6e64 2074 6865 2061 626f   to find the abo
-000010d0: 7665 2d6d 656e 7469 6f6e 6564 2063 6174  ve-mentioned cat
-000010e0: 6567 6f72 7920 616e 6420 6372 6561 7465  egory and create
-000010f0: 2061 2070 7974 686f 6e20 6669 6c65 206e   a python file n
-00001100: 616d 6564 0a60 3c61 6262 7265 7669 6174  amed.`<abbreviat
-00001110: 696f 6e3e 2e70 7960 2e20 5468 656e 2063  ion>.py`. Then c
-00001120: 7265 6174 6520 6120 636c 6173 7320 696e  reate a class in
-00001130: 6865 7269 7469 6e67 2074 6865 2060 4372  heriting the `Cr
-00001140: 694d 6542 6173 6560 2075 6e64 6572 2060  iMeBase` under `
-00001150: 636f 6d6d 6f6e 726f 6164 5f63 7269 6d65  commonroad_crime
-00001160: 2f64 6174 615f 7374 7275 6374 7572 652f  /data_structure/
-00001170: 6261 7365 2e70 7960 0a34 2e20 7369 6d69  base.py`.4. simi
-00001180: 6c61 7220 746f 206f 7468 6572 206d 6561  lar to other mea
-00001190: 7375 7265 732c 2079 6f75 206e 6565 6420  sures, you need 
-000011a0: 746f 2069 6d70 6c65 6d65 6e74 2074 6865  to implement the
-000011b0: 2060 636f 6d70 7574 6528 2960 2061 6e64   `compute()` and
-000011c0: 2060 7669 7375 616c 697a 6528 2960 2066   `visualize()` f
-000011d0: 756e 6374 696f 6e73 0a0a 2323 2320 486f  unctions..### Ho
-000011e0: 7720 746f 2064 6566 696e 6520 636f 6e66  w to define conf
-000011f0: 6967 7572 6174 696f 6e20 7061 7261 6d65  iguration parame
-00001200: 7465 7273 206f 6620 7468 6520 6d65 6173  ters of the meas
-00001210: 7572 650a 312e 206e 6176 6967 6174 6520  ure.1. navigate 
-00001220: 746f 2060 636f 6d6d 6f6e 726f 6164 5f63  to `commonroad_c
-00001230: 7269 6d65 2f64 6174 615f 7374 7275 6374  rime/data_struct
-00001240: 7572 652f 636f 6e66 6967 7561 7469 6f6e  ure/configuation
-00001250: 2e70 7960 2074 6f20 6669 6e64 2074 6865  .py` to find the
-00001260: 2061 626f 7665 2d6d 656e 7469 6f6e 6564   above-mentioned
-00001270: 2063 6174 6567 6f72 7920 616e 6420 6164   category and ad
-00001280: 6420 6120 6e65 7720 0a69 6e73 7461 6e63  d a new .instanc
-00001290: 6520 746f 2074 6865 2063 6c61 7373 2061  e to the class a
-000012a0: 7320 6073 656c 662e 3c70 6172 616d 6574  s `self.<paramet
-000012b0: 6572 3e20 3d20 636f 6e66 6967 5f72 656c  er> = config_rel
-000012c0: 6576 616e 742e 3c70 6172 616d 6574 6572  evant.<parameter
-000012d0: 3e60 0a32 2e20 796f 7520 6361 6e20 7468  >`.2. you can th
-000012e0: 656e 2064 6972 6563 746c 7920 6361 6c6c  en directly call
-000012f0: 2074 6865 2076 616c 7565 7320 7573 696e   the values usin
-00001300: 6720 6073 656c 662e 636f 6e66 6967 7572  g `self.configur
-00001310: 6174 696f 6e2e 3c63 6174 6567 6f72 793e  ation.<category>
-00001320: 2e3c 7061 7261 6d65 7465 723e 6020 696e  .<parameter>` in
-00001330: 2079 6f75 7220 6d65 6173 7572 6520 636c   your measure cl
-00001340: 6173 730a 332e 2074 6f20 6f76 6572 7269  ass.3. to overri
-00001350: 6465 2074 6865 2064 6566 6175 6c74 2070  de the default p
-00001360: 6172 616d 6574 6572 2076 616c 7565 732c  arameter values,
-00001370: 2063 7265 6174 6520 6120 6079 616d 6c60   create a `yaml`
-00001380: 2066 696c 6520 286e 616d 6520 6974 2074   file (name it t
-00001390: 6865 2073 616d 6520 6173 2074 6865 2073  he same as the s
-000013a0: 6365 6e61 7269 6f29 2069 6e20 602e 2f63  cenario) in `./c
-000013b0: 6f6e 6669 675f 6669 6c65 7360 2061 6e64  onfig_files` and
-000013c0: 206d 6f64 6966 7920 7468 6520 7661 6c75   modify the valu
-000013d0: 6573 2074 6865 7265 0a23 2320 446f 6375  es there.## Docu
-000013e0: 6d65 6e74 6174 696f 6e0a 0a54 6865 2064  mentation..The d
-000013f0: 6f63 756d 656e 7461 7469 6f6e 206f 6620  ocumentation of 
-00001400: 6f75 7220 746f 6f6c 626f 7820 6973 2061  our toolbox is a
-00001410: 7661 696c 6162 6c65 206f 6e20 6f75 7220  vailable on our 
-00001420: 7765 6273 6974 653a 2068 7474 7073 3a2f  website: https:/
-00001430: 2f63 7073 2e70 6167 6573 2e67 6974 6c61  /cps.pages.gitla
-00001440: 622e 6c72 7a2e 6465 2f63 6f6d 6d6f 6e72  b.lrz.de/commonr
-00001450: 6f61 642f 636f 6d6d 6f6e 726f 6164 2d63  oad/commonroad-c
-00001460: 7269 7469 6361 6c69 7479 2d6d 6561 7375  riticality-measu
-00001470: 7265 732f 2e0a 0a49 6e20 6f72 6465 7220  res/...In order 
-00001480: 746f 2067 656e 6572 6174 6520 7468 6520  to generate the 
-00001490: 646f 6375 6d65 6e74 6174 696f 6e20 7669  documentation vi
-000014a0: 6120 5370 6869 6e78 206c 6f63 616c 6c79  a Sphinx locally
-000014b0: 2c20 7275 6e20 7468 6520 666f 6c6c 6f77  , run the follow
-000014c0: 696e 6720 636f 6d6d 616e 6473 2069 6e20  ing commands in 
-000014d0: 7468 6520 726f 6f74 2064 6972 6563 746f  the root directo
-000014e0: 7279 3a0a 0a60 6060 6261 7368 0a24 2070  ry:..```bash.$ p
-000014f0: 6970 2069 6e73 7461 6c6c 202d 7220 2e2f  ip install -r ./
-00001500: 646f 6373 2f72 6571 7569 7265 6d65 6e74  docs/requirement
-00001510: 735f 646f 632e 7478 740a 2420 6364 2064  s_doc.txt.$ cd d
-00001520: 6f63 732f 7370 6869 6e78 0a24 206d 616b  ocs/sphinx.$ mak
-00001530: 6520 6874 6d6c 0a60 6060 0a0a 5468 6520  e html.```..The 
-00001540: 646f 6375 6d65 6e74 6174 696f 6e20 6361  documentation ca
-00001550: 6e20 7468 656e 2062 6520 6c61 756e 6368  n then be launch
-00001560: 6564 2062 7920 6272 6f77 7369 6e67 2060  ed by browsing `
-00001570: 602e 2f64 6f63 732f 7370 6869 6e78 2f62  `./docs/sphinx/b
-00001580: 7569 6c64 2f68 746d 6c2f 696e 6465 782e  uild/html/index.
-00001590: 6874 6d6c 2f60 602e 0a0a 2323 2320 436f  html/``...### Co
-000015a0: 6e74 7269 6275 746f 7273 2028 696e 2061  ntributors (in a
-000015b0: 6c70 6861 6265 7469 6361 6c20 6f72 6465  lphabetical orde
-000015c0: 7220 6279 206c 6173 7420 6e61 6d65 290a  r by last name).
-000015d0: 2d20 4c69 6775 6f20 4368 656e 0a2d 2059  - Liguo Chen.- Y
-000015e0: 7561 6e66 6569 204c 696e 0a2d 2053 6562  uanfei Lin.- Seb
-000015f0: 6173 7469 616e 204d 6169 6572 686f 6665  astian Maierhofe
-00001600: 720a 2d20 4976 616e 6120 5065 6e65 7661  r.- Ivana Peneva
-00001610: 0a2d 204b 756e 2051 6961 6e0a 2d20 4f6c  .- Kun Qian.- Ol
-00001620: 6976 6572 2053 7065 6368 740a 2d20 5369  iver Specht.- Si
-00001630: 6368 656e 6720 5761 6e67 0a2d 2059 6f75  cheng Wang.- You
-00001640: 7261 6e20 5761 6e67 0a2d 205a 656b 756e  ran Wang.- Zekun
-00001650: 2058 696e 670a 2d20 5a69 7169 616e 2058   Xing.- Ziqian X
-00001660: 750a 0a23 2323 2043 6974 6174 696f 6e0a  u..### Citation.
-00001670: 4966 2079 6f75 2075 7365 2060 636f 6d6d  If you use `comm
-00001680: 6f6e 726f 6164 2d63 7269 6d65 6020 666f  onroad-crime` fo
-00001690: 7220 6163 6164 656d 6963 2077 6f72 6b2c  r academic work,
-000016a0: 2077 6520 6869 6768 6c79 2065 6e63 6f75   we highly encou
-000016b0: 7261 6765 2079 6f75 2074 6f20 6369 7465  rage you to cite
-000016c0: 206f 7572 2070 6170 6572 3a0a 6060 6074   our paper:.```t
-000016d0: 6578 740a 4049 6e50 726f 6365 6564 696e  ext.@InProceedin
-000016e0: 6773 7b6c 696e 3230 3233 6372 696d 652c  gs{lin2023crime,
-000016f0: 0a20 2020 2020 2074 6974 6c65 2020 2020  .      title    
-00001700: 203d 207b 7b43 6f6d 6d6f 6e52 6f61 642d   = {{CommonRoad-
-00001710: 4372 694d 657d 3a20 7b41 7d20 546f 6f6c  CriMe}: {A} Tool
-00001720: 626f 7820 666f 7220 4372 6974 6963 616c  box for Critical
-00001730: 6974 7920 4d65 6173 7572 6573 206f 6620  ity Measures of 
-00001740: 4175 746f 6e6f 6d6f 7573 2056 6568 6963  Autonomous Vehic
-00001750: 6c65 737d 2c0a 2020 2020 2020 6175 7468  les},.      auth
-00001760: 6f72 2020 2020 3d20 7b59 7561 6e66 6569  or    = {Yuanfei
-00001770: 204c 696e 2061 6e64 204d 6174 7468 6961   Lin and Matthia
-00001780: 7320 416c 7468 6f66 667d 2c0a 2020 2020  s Althoff},.    
-00001790: 2020 626f 6f6b 7469 746c 6520 3d20 7b50    booktitle = {P
-000017a0: 726f 632e 206f 6620 7468 6520 4945 4545  roc. of the IEEE
-000017b0: 2049 6e74 656c 6c2e 2056 6568 2e20 5379   Intell. Veh. Sy
-000017c0: 6d70 2e7d 2c20 2020 2020 0a20 2020 2020  mp.},     .     
-000017d0: 2070 6167 6573 2020 2020 203d 207b 312d   pages     = {1-
-000017e0: 387d 2c20 0a20 2020 2020 2079 6561 7220  8}, .      year 
-000017f0: 2020 2020 203d 207b 3230 3233 7d2c 0a7d       = {2023},.}
-00001800: 0a60 6060 0a49 6620 796f 7520 7573 6520  .```.If you use 
-00001810: 7468 6973 2070 726f 6a65 6374 2773 2063  this project's c
-00001820: 6f64 6520 696e 2069 6e64 7573 7472 792c  ode in industry,
-00001830: 2077 6527 6420 6c6f 7665 2074 6f20 6865   we'd love to he
-00001840: 6172 2066 726f 6d20 796f 7520 6173 2077  ar from you as w
-00001850: 656c 6c3b 200a 6665 656c 2066 7265 6520  ell; .feel free 
-00001860: 746f 2072 6561 6368 206f 7574 2074 6f20  to reach out to 
-00001870: 5b59 7561 6e66 6569 204c 696e 5d28 6d61  [Yuanfei Lin](ma
-00001880: 696c 746f 3a79 7561 6e66 6569 2e6c 696e  ilto:yuanfei.lin
-00001890: 4074 756d 2e64 6529 2064 6972 6563 746c  @tum.de) directl
-000018a0: 792e 0a                                  y..
+00000150: 6d6d 6f6e 726f 6164 2f63 6f6d 6d6f 6e72  mmonroad/commonr
+00000160: 6f61 642d 6372 6974 6963 616c 6974 792d  oad-criticality-
+00000170: 6d65 6173 7572 6573 2f0a 5072 6f6a 6563  measures/.Projec
+00000180: 742d 5552 4c3a 2046 6f72 756d 2c20 6874  t-URL: Forum, ht
+00000190: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000001a0: 2f43 6f6d 6d6f 6e52 6f61 642f 636f 6d6d  /CommonRoad/comm
+000001b0: 6f6e 726f 6164 2d63 7269 6d65 2f69 7373  onroad-crime/iss
+000001c0: 7565 730a 5072 6f6a 6563 742d 5552 4c3a  ues.Project-URL:
+000001d0: 2053 6f75 7263 652c 2068 7474 7073 3a2f   Source, https:/
+000001e0: 2f67 6974 6875 622e 636f 6d2f 436f 6d6d  /github.com/Comm
+000001f0: 6f6e 526f 6164 2f63 6f6d 6d6f 6e72 6f61  onRoad/commonroa
+00000200: 642d 6372 696d 650a 4b65 7977 6f72 6473  d-crime.Keywords
+00000210: 3a20 6372 6974 6963 616c 6974 792c 6175  : criticality,au
+00000220: 746f 6e6f 6d6f 7573 2064 7269 7669 6e67  tonomous driving
+00000230: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000240: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000250: 6520 3a3a 2043 2b2b 0a43 6c61 7373 6966  e :: C++.Classif
+00000260: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000270: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000280: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+00000290: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000002a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002b0: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+000002c0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002e0: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+000002f0: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
+00000300: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000310: 7665 6420 3a3a 2042 5344 204c 6963 656e  ved :: BSD Licen
+00000320: 7365 0a43 6c61 7373 6966 6965 723a 204f  se.Classifier: O
+00000330: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000340: 3a3a 2050 4f53 4958 203a 3a20 4c69 6e75  :: POSIX :: Linu
+00000350: 780a 4465 7363 7269 7074 696f 6e2d 436f  x.Description-Co
+00000360: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+00000370: 2f6d 6172 6b64 6f77 6e0a 4c69 6365 6e73  /markdown.Licens
+00000380: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
+00000390: 5265 7175 6972 6573 2d44 6973 743a 2063  Requires-Dist: c
+000003a0: 6f6d 6d6f 6e72 6f61 642d 696f 3e3d 3230  ommonroad-io>=20
+000003b0: 3233 2e34 0a52 6571 7569 7265 732d 4469  23.4.Requires-Di
+000003c0: 7374 3a20 636f 6d6d 6f6e 726f 6164 2d76  st: commonroad-v
+000003d0: 6568 6963 6c65 2d6d 6f64 656c 733e 3d33  ehicle-models>=3
+000003e0: 2e30 2e30 0a52 6571 7569 7265 732d 4469  .0.0.Requires-Di
+000003f0: 7374 3a20 636f 6d6d 6f6e 726f 6164 2d72  st: commonroad-r
+00000400: 6f75 7465 2d70 6c61 6e6e 6572 3e3d 3230  oute-planner>=20
+00000410: 3234 2e32 2e30 0a52 6571 7569 7265 732d  24.2.0.Requires-
+00000420: 4469 7374 3a20 636f 6d6d 6f6e 726f 6164  Dist: commonroad
+00000430: 2d64 7269 7661 6269 6c69 7479 2d63 6865  -drivability-che
+00000440: 636b 6572 3e3d 3230 3233 2e31 0a52 6571  cker>=2023.1.Req
+00000450: 7569 7265 732d 4469 7374 3a20 636f 6d6d  uires-Dist: comm
+00000460: 6f6e 726f 6164 2d72 6561 6368 3e3d 3230  onroad-reach>=20
+00000470: 3234 2e31 2e32 0a52 6571 7569 7265 732d  24.1.2.Requires-
+00000480: 4469 7374 3a20 6d61 7470 6c6f 746c 6962  Dist: matplotlib
+00000490: 3e3d 332e 352e 320a 5265 7175 6972 6573  >=3.5.2.Requires
+000004a0: 2d44 6973 743a 206e 756d 7079 3e3d 312e  -Dist: numpy>=1.
+000004b0: 3139 2e30 0a52 6571 7569 7265 732d 4469  19.0.Requires-Di
+000004c0: 7374 3a20 7363 6970 793e 3d31 2e37 2e33  st: scipy>=1.7.3
+000004d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000004e0: 7368 6170 656c 793c 332e 302e 302c 3e3d  shapely<3.0.0,>=
+000004f0: 322e 302e 310a 5265 7175 6972 6573 2d44  2.0.1.Requires-D
+00000500: 6973 743a 206f 6d65 6761 636f 6e66 3e3d  ist: omegaconf>=
+00000510: 322e 312e 310a 5265 7175 6972 6573 2d44  2.1.1.Requires-D
+00000520: 6973 743a 2063 6173 6164 693e 3d33 2e36  ist: casadi>=3.6
+00000530: 2e33 0a52 6571 7569 7265 732d 4469 7374  .3.Requires-Dist
+00000540: 3a20 7471 646d 3e3d 342e 3635 2e30 0a52  : tqdm>=4.65.0.R
+00000550: 6571 7569 7265 732d 4469 7374 3a20 696d  equires-Dist: im
+00000560: 6167 6569 6f3e 3d32 2e39 2e30 0a52 6571  ageio>=2.9.0.Req
+00000570: 7569 7265 732d 4469 7374 3a20 7079 7465  uires-Dist: pyte
+00000580: 7374 3e3d 372e 342e 300a 0a23 2043 6f6d  st>=7.4.0..# Com
+00000590: 6d6f 6e52 6f61 642d 4372 694d 650a 215b  monRoad-CriMe.![
+000005a0: 696d 6167 6520 696e 666f 5d28 6874 7470  image info](http
+000005b0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+000005c0: 6572 636f 6e74 656e 742e 636f 6d2f 436f  ercontent.com/Co
+000005d0: 6d6d 6f6e 526f 6164 2f63 6f6d 6d6f 6e72  mmonRoad/commonr
+000005e0: 6f61 642d 6372 696d 652f 6465 7665 6c6f  oad-crime/develo
+000005f0: 702f 646f 6373 2f66 6967 7572 6573 2f43  p/docs/figures/C
+00000600: 7269 4d65 2d62 616e 6e65 722e 706e 6729  riMe-banner.png)
+00000610: 0a5b 215b 4c69 6e75 785d 2868 7474 7073  .[![Linux](https
+00000620: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000630: 6f2f 6261 6467 652f 6f73 2d6c 696e 7578  o/badge/os-linux
+00000640: 3f26 6c6f 676f 3d4c 696e 7578 266c 6f67  ?&logo=Linux&log
+00000650: 6f43 6f6c 6f72 3d77 6869 7465 266c 6162  oColor=white&lab
+00000660: 656c 436f 6c6f 723d 6772 6179 295d 2868  elColor=gray)](h
+00000670: 7474 7073 3a2f 2f70 7970 692e 7079 7468  ttps://pypi.pyth
+00000680: 6f6e 2e6f 7267 2f70 7970 692f 636f 6d6d  on.org/pypi/comm
+00000690: 6f6e 726f 6164 2d6f 7065 6e73 6365 6e61  onroad-openscena
+000006a0: 7269 6f2d 636f 6e76 6572 7465 722f 290a  rio-converter/).
+000006b0: 5b21 5b50 7950 4920 7665 7273 696f 6e20  [![PyPI version 
+000006c0: 6675 7279 2e69 6f5d 2868 7474 7073 3a2f  fury.io](https:/
+000006d0: 2f62 6164 6765 2e66 7572 792e 696f 2f70  /badge.fury.io/p
+000006e0: 792f 636f 6d6d 6f6e 726f 6164 2d63 7269  y/commonroad-cri
+000006f0: 6d65 2e73 7667 3f73 7479 6c65 3d70 6c61  me.svg?style=pla
+00000700: 7374 6963 295d 2868 7474 7073 3a2f 2f70  stic)](https://p
+00000710: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
+00000720: 7970 692f 636f 6d6d 6f6e 726f 6164 2d63  ypi/commonroad-c
+00000730: 7269 6d65 2f29 0a5b 215b 5079 5049 206c  rime/).[![PyPI l
+00000740: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
+00000750: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000760: 7970 692f 6c2f 636f 6d6d 6f6e 726f 6164  ypi/l/commonroad
+00000770: 2d63 7269 6d65 2e73 7667 3f73 7479 6c65  -crime.svg?style
+00000780: 3d70 6c61 7374 6963 295d 2868 7474 7073  =plastic)](https
+00000790: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+000007a0: 7267 2f70 7970 692f 636f 6d6d 6f6e 726f  rg/pypi/commonro
+000007b0: 6164 2d63 7269 6d65 2f29 3c62 723e 0a5b  ad-crime/)<br>.[
+000007c0: 215b 5079 5049 2064 6f77 6e6c 6f61 6420  ![PyPI download 
+000007d0: 6d6f 6e74 685d 2868 7474 7073 3a2f 2f69  month](https://i
+000007e0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000007f0: 7069 2f64 6d2f 636f 6d6d 6f6e 726f 6164  pi/dm/commonroad
+00000800: 2d63 7269 6d65 2e73 7667 3f73 7479 6c65  -crime.svg?style
+00000810: 3d70 6c61 7374 6963 266c 6162 656c 3d50  =plastic&label=P
+00000820: 7950 4925 3230 646f 776e 6c6f 6164 7329  yPI%20downloads)
+00000830: 5d28 6874 7470 733a 2f2f 7079 7069 2e70  ](https://pypi.p
+00000840: 7974 686f 6e2e 6f72 672f 7079 7069 2f63  ython.org/pypi/c
+00000850: 6f6d 6d6f 6e72 6f61 642d 6372 696d 652f  ommonroad-crime/
+00000860: 2920 0a5b 215b 5079 5049 2064 6f77 6e6c  ) .[![PyPI downl
+00000870: 6f61 6420 7765 656b 5d28 6874 7470 733a  oad week](https:
+00000880: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000890: 2f70 7970 692f 6477 2f63 6f6d 6d6f 6e72  /pypi/dw/commonr
+000008a0: 6f61 642d 6372 696d 652e 7376 673f 7374  oad-crime.svg?st
+000008b0: 796c 653d 706c 6173 7469 6326 6c61 6265  yle=plastic&labe
+000008c0: 6c3d 5079 5049 2532 3064 6f77 6e6c 6f61  l=PyPI%20downloa
+000008d0: 6473 295d 2868 7474 7073 3a2f 2f70 7970  ds)](https://pyp
+000008e0: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
+000008f0: 692f 636f 6d6d 6f6e 726f 6164 2d63 7269  i/commonroad-cri
+00000900: 6d65 2f29 3c62 723e 0a0a 546f 6f6c 626f  me/)<br>..Toolbo
+00000910: 7820 746f 2063 6f6d 7075 7465 202a 2a43  x to compute **C
+00000920: 7269 2a2a 7469 6361 6c69 7479 202a 2a4d  ri**ticality **M
+00000930: 652a 2a61 7375 7265 7320 0a28 652e 672e  e**asures .(e.g.
+00000940: 2074 696d 652d 746f 2d63 6f6c 6c69 7369   time-to-collisi
+00000950: 6f6e 2c20 7469 6d65 2d74 6f2d 7265 6163  on, time-to-reac
+00000960: 742c 2e2e 2e29 2e20 5375 6368 206d 6561  t,...). Such mea
+00000970: 7375 7265 730a 6361 6e20 6265 2075 7365  sures.can be use
+00000980: 6420 746f 2074 7269 6767 6572 2077 6172  d to trigger war
+00000990: 6e69 6e67 7320 616e 6420 656d 6572 6765  nings and emerge
+000009a0: 6e63 7920 6d61 6e65 7576 6572 7320 0a69  ncy maneuvers .i
+000009b0: 6e20 6472 6976 6572 2061 7373 6973 7461  n driver assista
+000009c0: 6e63 6520 7379 7374 656d 7320 6f72 2072  nce systems or r
+000009d0: 6570 6169 7220 616e 2069 6e66 6561 7369  epair an infeasi
+000009e0: 626c 6520 0a74 7261 6a65 6374 6f72 792e  ble .trajectory.
+000009f0: 2049 6620 796f 7520 6861 7665 2071 7565   If you have que
+00000a00: 7374 696f 6e73 206f 7220 7761 6e74 2074  stions or want t
+00000a10: 6f20 7265 706f 7274 2070 726f 626c 656d  o report problem
+00000a20: 7320 6f72 2073 7567 6765 7374 696f 6e73  s or suggestions
+00000a30: 2c20 706c 6561 7365 2073 7461 7274 2061  , please start a
+00000a40: 205b 4769 7468 7562 2064 6973 6375 7373   [Github discuss
+00000a50: 696f 6e5d 2868 7474 7073 3a2f 2f67 6974  ion](https://git
+00000a60: 6875 622e 636f 6d2f 6f72 6773 2f43 6f6d  hub.com/orgs/Com
+00000a70: 6d6f 6e52 6f61 642f 6469 7363 7573 7369  monRoad/discussi
+00000a80: 6f6e 7329 202f 0a5b 4769 7468 7562 2069  ons) /.[Github i
+00000a90: 7373 7565 5d28 6874 7470 733a 2f2f 6769  ssue](https://gi
+00000aa0: 7468 7562 2e63 6f6d 2f43 6f6d 6d6f 6e52  thub.com/CommonR
+00000ab0: 6f61 642f 636f 6d6d 6f6e 726f 6164 2d63  oad/commonroad-c
+00000ac0: 7269 6d65 2f69 7373 7565 732f 292e 200a  rime/issues/). .
+00000ad0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000ae0: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+00000af0: 2e67 6f6f 676c 652e 636f 6d2f 6472 6976  .google.com/driv
+00000b00: 652f 3154 374d 6253 5671 5535 5843 445a  e/1T7MbSVqU5XCDZ
+00000b10: 6750 5444 4552 4b4e 4b59 4662 4149 6e58  gPTDERKNKYFbAInX
+00000b20: 526a 7922 3e0a 2020 3c69 6d67 2073 7263  Rjy">.  <img src
+00000b30: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+00000b40: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000b50: 636f 6d2f 436f 6d6d 6f6e 526f 6164 2f63  com/CommonRoad/c
+00000b60: 6f6d 6d6f 6e72 6f61 642d 6372 696d 652f  ommonroad-crime/
+00000b70: 6465 7665 6c6f 702f 646f 6373 2f66 6967  develop/docs/fig
+00000b80: 7572 6573 2f6c 6976 655f 6465 6d6f 2e70  ures/live_demo.p
+00000b90: 6e67 2220 616c 743d 224c 6976 6520 4465  ng" alt="Live De
+00000ba0: 6d6f 223e 0a3c 2f61 3e0a 0a23 2320 f09f  mo">.</a>..## ..
+00000bb0: 9a80 2049 6e73 7461 6c6c 6174 696f 6e20  .. Installation 
+00000bc0: 4775 6964 650a 0a60 636f 6d6d 6f6e 726f  Guide..`commonro
+00000bd0: 6164 2d63 7269 6d65 6020 6361 6e20 6265  ad-crime` can be
+00000be0: 2069 6e73 7461 6c6c 6564 2077 6974 683a   installed with:
+00000bf0: 0a0a 6060 6020 6261 7368 0a24 2070 6970  ..``` bash.$ pip
+00000c00: 2069 6e73 7461 6c6c 2063 6f6d 6d6f 6e72   install commonr
+00000c10: 6f61 642d 6372 696d 650a 6060 600a 3c64  oad-crime.```.<d
+00000c20: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00000c30: 3e3c 623e 4465 7665 6c6f 7020 4372 694d  ><b>Develop CriM
+00000c40: 6520 6c6f 6361 6c6c 793c 2f62 3e3c 2f73  e locally</b></s
+00000c50: 756d 6d61 7279 3e0a 0a46 6f72 2061 6464  ummary>..For add
+00000c60: 696e 6720 6e65 7720 6d65 6173 7572 6573  ing new measures
+00000c70: 2c20 7765 2072 6563 6f6d 6d65 6e64 2075  , we recommend u
+00000c80: 7369 6e67 205b 416e 6163 6f6e 6461 5d28  sing [Anaconda](
+00000c90: 6874 7470 733a 2f2f 7777 772e 616e 6163  https://www.anac
+00000ca0: 6f6e 6461 2e63 6f6d 2f29 2074 6f20 6d61  onda.com/) to ma
+00000cb0: 6e61 6765 2079 6f75 7220 656e 7669 726f  nage your enviro
+00000cc0: 6e6d 656e 7420 736f 2074 6861 7420 6576  nment so that ev
+00000cd0: 656e 2069 6620 796f 7520 6d65 7373 2073  en if you mess s
+00000ce0: 6f6d 6574 6869 6e67 2075 702c 2079 6f75  omething up, you
+00000cf0: 2063 616e 2061 6c77 6179 7320 6861 7665   can always have
+00000d00: 2061 2073 6166 6520 616e 6420 636c 6561   a safe and clea
+00000d10: 6e20 7265 7374 6172 742e 2041 2067 7569  n restart. A gui
+00000d20: 6465 2066 6f72 206d 616e 6167 696e 6720  de for managing 
+00000d30: 7079 7468 6f6e 2065 6e76 6972 6f6e 6d65  python environme
+00000d40: 6e74 7320 7769 7468 2041 6e61 636f 6e64  nts with Anacond
+00000d50: 6120 6361 6e20 6265 2066 6f75 6e64 205b  a can be found [
+00000d60: 6865 7265 5d28 6874 7470 733a 2f2f 636f  here](https://co
+00000d70: 6e64 612e 696f 2f70 726f 6a65 6374 732f  nda.io/projects/
+00000d80: 636f 6e64 612f 656e 2f6c 6174 6573 742f  conda/en/latest/
+00000d90: 7573 6572 2d67 7569 6465 2f74 6173 6b73  user-guide/tasks
+00000da0: 2f6d 616e 6167 652d 656e 7669 726f 6e6d  /manage-environm
+00000db0: 656e 7473 2e68 746d 6c29 2e0a 0a41 6674  ents.html)...Aft
+00000dc0: 6572 2069 6e73 7461 6c6c 696e 6720 416e  er installing An
+00000dd0: 6163 6f6e 6461 2c20 6372 6561 7465 2061  aconda, create a
+00000de0: 206e 6577 2065 6e76 6972 6f6e 6d65 6e74   new environment
+00000df0: 2077 6974 683a 0a60 6060 2062 6173 680a   with:.``` bash.
+00000e00: 2420 636f 6e64 6120 6372 6561 7465 202d  $ conda create -
+00000e10: 6e20 636f 6d6d 6f6e 726f 6164 2d70 7933  n commonroad-py3
+00000e20: 3820 7079 7468 6f6e 3d33 2e38 202d 790a  8 python=3.8 -y.
+00000e30: 6060 600a 0a48 6572 6520 7468 6520 6e61  ```..Here the na
+00000e40: 6d65 206f 6620 7468 6520 656e 7669 726f  me of the enviro
+00000e50: 6e6d 656e 7420 6973 2063 616c 6c65 6420  nment is called 
+00000e60: 2a2a 636f 6d6d 6f6e 726f 6164 2d70 7933  **commonroad-py3
+00000e70: 382a 2a2e 2059 6f75 206d 6179 2061 6c73  8**. You may als
+00000e80: 6f20 6368 616e 6765 2074 6869 7320 6e61  o change this na
+00000e90: 6d65 2061 7320 796f 7520 7769 7368 2e20  me as you wish. 
+00000ea0: 496e 2073 7563 6820 6361 7365 2c20 646f  In such case, do
+00000eb0: 6e27 7420 666f 7267 6574 2074 6f20 6368  n't forget to ch
+00000ec0: 616e 6765 2069 7420 696e 2074 6865 2066  ange it in the f
+00000ed0: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00000ee0: 7320 6173 2077 656c 6c2e 202a 2a41 6c77  s as well. **Alw
+00000ef0: 6179 7320 6163 7469 7661 7465 2a2a 2074  ays activate** t
+00000f00: 6869 7320 656e 7669 726f 6e6d 656e 7420  his environment 
+00000f10: 6265 666f 7265 2079 6f75 2064 6f20 616e  before you do an
+00000f20: 7974 6869 6e67 2072 656c 6174 6564 3a0a  ything related:.
+00000f30: 0a60 6060 7368 0a24 2063 6f6e 6461 2061  .```sh.$ conda a
+00000f40: 6374 6976 6174 6520 636f 6d6d 6f6e 726f  ctivate commonro
+00000f50: 6164 2d70 7933 380a 6f72 0a24 2073 6f75  ad-py38.or.$ sou
+00000f60: 7263 6520 6163 7469 7661 7465 2063 6f6d  rce activate com
+00000f70: 6d6f 6e72 6f61 642d 7079 3338 0a60 6060  monroad-py38.```
+00000f80: 0a54 6865 6e2c 2069 6e73 7461 6c6c 2074  .Then, install t
+00000f90: 6865 2064 6570 656e 6465 6e63 6965 7320  he dependencies 
+00000fa0: 7769 7468 3a0a 0a60 6060 7368 0a24 2063  with:..```sh.$ c
+00000fb0: 6420 3c70 6174 682d 746f 2d74 6869 732d  d <path-to-this-
+00000fc0: 7265 706f 3e0a 2420 7069 7020 696e 7374  repo>.$ pip inst
+00000fd0: 616c 6c20 2d65 202e 0a24 2063 6f6e 6461  all -e ..$ conda
+00000fe0: 2064 6576 656c 6f70 202e 0a60 6060 0a0a   develop ..```..
+00000ff0: 546f 2074 6573 7420 7468 6520 696e 7374  To test the inst
+00001000: 616c 6c69 7469 6f6e 2c20 7275 6e20 756e  allition, run un
+00001010: 6974 7465 7374 3a0a 6060 6062 6173 680a  ittest:.```bash.
+00001020: 2420 6364 2074 6573 7473 0a24 2070 7974  $ cd tests.$ pyt
+00001030: 686f 6e20 2d6d 2075 6e69 7474 6573 7420  hon -m unittest 
+00001040: 2d76 0a60 6060 0a0a 3c2f 6465 7461 696c  -v.```..</detail
+00001050: 733e 0a0a 546f 2067 6574 2073 7461 7274  s>..To get start
+00001060: 6564 2079 6f75 7220 6a6f 7572 6e65 7920  ed your journey 
+00001070: 7769 7468 206f 7572 2063 7269 7469 6361  with our critica
+00001080: 6c69 7479 206d 6561 7375 7265 732c 2063  lity measures, c
+00001090: 6865 636b 2074 6865 2060 7475 746f 7269  heck the `tutori
+000010a0: 616c 7360 2061 6e64 2074 6865 2066 6f6c  als` and the fol
+000010b0: 6c6f 7769 6e67 2074 6970 732e 0a0a 3c64  lowing tips...<d
+000010c0: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+000010d0: 3e3c 623e 4164 6420 6e65 7720 6372 6974  ><b>Add new crit
+000010e0: 6963 616c 6974 7920 6d65 6173 7572 653c  icality measure<
+000010f0: 2f62 3e3c 2f73 756d 6d61 7279 3e0a 0a31  /b></summary>..1
+00001100: 2e20 6372 6561 7465 2061 206e 6577 2062  . create a new b
+00001110: 7261 6e63 6820 7769 7468 2060 6665 6174  ranch with `feat
+00001120: 7572 652d 3c6d 6561 7375 7265 2d6e 616d  ure-<measure-nam
+00001130: 653e 6020 616e 6420 6368 6563 6b6f 7574  e>` and checkout
+00001140: 2074 6865 2062 7261 6e63 680a 322e 206e   the branch.2. n
+00001150: 6176 6967 6174 6520 746f 2060 636f 6d6d  avigate to `comm
+00001160: 6f6e 726f 6164 5f63 7269 6d65 2f64 6174  onroad_crime/dat
+00001170: 615f 7374 7275 6374 7572 652f 7479 7065  a_structure/type
+00001180: 2e70 7960 2074 6f20 6669 6e64 2074 6865  .py` to find the
+00001190: 2063 6f72 7265 6374 2063 6174 6567 6f72   correct categor
+000011a0: 7920 6f66 2074 6865 206d 6561 7375 7265  y of the measure
+000011b0: 2061 6e64 2061 6464 2061 6e20 0a65 6e75   and add an .enu
+000011c0: 6d65 7261 7469 6f6e 2065 6e74 7279 2060  meration entry `
+000011d0: 3c61 6262 7265 7669 6174 696f 6e3e 3a20  <abbreviation>: 
+000011e0: 3c65 7870 6c61 6e61 7469 6f6e 3e60 0a33  <explanation>`.3
+000011f0: 2e20 6e61 7669 6761 7465 2074 6f20 6063  . navigate to `c
+00001200: 6f6d 6d6f 6e72 6f61 645f 6372 696d 652f  ommonroad_crime/
+00001210: 6d65 6173 7572 6560 2074 6f20 6669 6e64  measure` to find
+00001220: 2074 6865 2061 626f 7665 2d6d 656e 7469   the above-menti
+00001230: 6f6e 6564 2063 6174 6567 6f72 7920 616e  oned category an
+00001240: 6420 6372 6561 7465 2061 2070 7974 686f  d create a pytho
+00001250: 6e20 6669 6c65 206e 616d 6564 0a60 3c61  n file named.`<a
+00001260: 6262 7265 7669 6174 696f 6e3e 2e70 7960  bbreviation>.py`
+00001270: 2e20 5468 656e 2063 7265 6174 6520 6120  . Then create a 
+00001280: 636c 6173 7320 696e 6865 7269 7469 6e67  class inheriting
+00001290: 2074 6865 2060 4372 694d 6542 6173 6560   the `CriMeBase`
+000012a0: 2075 6e64 6572 2060 636f 6d6d 6f6e 726f   under `commonro
+000012b0: 6164 5f63 7269 6d65 2f64 6174 615f 7374  ad_crime/data_st
+000012c0: 7275 6374 7572 652f 6261 7365 2e70 7960  ructure/base.py`
+000012d0: 0a34 2e20 7369 6d69 6c61 7220 746f 206f  .4. similar to o
+000012e0: 7468 6572 206d 6561 7375 7265 732c 2079  ther measures, y
+000012f0: 6f75 206e 6565 6420 746f 2069 6d70 6c65  ou need to imple
+00001300: 6d65 6e74 2074 6865 2060 636f 6d70 7574  ment the `comput
+00001310: 6528 2960 2061 6e64 2060 7669 7375 616c  e()` and `visual
+00001320: 697a 6528 2960 2066 756e 6374 696f 6e73  ize()` functions
+00001330: 0a0a 3c2f 6465 7461 696c 733e 0a0a 3c64  ..</details>..<d
+00001340: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00001350: 3e3c 623e 4465 6669 6e65 2063 6f6e 6669  ><b>Define confi
+00001360: 6775 7261 7469 6f6e 2070 6172 616d 6574  guration paramet
+00001370: 6572 7320 6f66 2074 6865 206d 6561 7375  ers of the measu
+00001380: 7265 3c2f 623e 3c2f 7375 6d6d 6172 793e  re</b></summary>
+00001390: 0a0a 312e 206e 6176 6967 6174 6520 746f  ..1. navigate to
+000013a0: 2060 636f 6d6d 6f6e 726f 6164 5f63 7269   `commonroad_cri
+000013b0: 6d65 2f64 6174 615f 7374 7275 6374 7572  me/data_structur
+000013c0: 652f 636f 6e66 6967 7561 7469 6f6e 2e70  e/configuation.p
+000013d0: 7960 2074 6f20 6669 6e64 2074 6865 2061  y` to find the a
+000013e0: 626f 7665 2d6d 656e 7469 6f6e 6564 2063  bove-mentioned c
+000013f0: 6174 6567 6f72 7920 616e 6420 6164 6420  ategory and add 
+00001400: 6120 6e65 7720 0a69 6e73 7461 6e63 6520  a new .instance 
+00001410: 746f 2074 6865 2063 6c61 7373 2061 7320  to the class as 
+00001420: 6073 656c 662e 3c70 6172 616d 6574 6572  `self.<parameter
+00001430: 3e20 3d20 636f 6e66 6967 5f72 656c 6576  > = config_relev
+00001440: 616e 742e 3c70 6172 616d 6574 6572 3e60  ant.<parameter>`
+00001450: 0a32 2e20 796f 7520 6361 6e20 7468 656e  .2. you can then
+00001460: 2064 6972 6563 746c 7920 6361 6c6c 2074   directly call t
+00001470: 6865 2076 616c 7565 7320 7573 696e 6720  he values using 
+00001480: 6073 656c 662e 636f 6e66 6967 7572 6174  `self.configurat
+00001490: 696f 6e2e 3c63 6174 6567 6f72 793e 2e3c  ion.<category>.<
+000014a0: 7061 7261 6d65 7465 723e 6020 696e 2079  parameter>` in y
+000014b0: 6f75 7220 6d65 6173 7572 6520 636c 6173  our measure clas
+000014c0: 730a 332e 2074 6f20 6f76 6572 7269 6465  s.3. to override
+000014d0: 2074 6865 2064 6566 6175 6c74 2070 6172   the default par
+000014e0: 616d 6574 6572 2076 616c 7565 732c 2063  ameter values, c
+000014f0: 7265 6174 6520 6120 6079 616d 6c60 2066  reate a `yaml` f
+00001500: 696c 6520 286e 616d 6520 6974 2074 6865  ile (name it the
+00001510: 2073 616d 6520 6173 2074 6865 2073 6365   same as the sce
+00001520: 6e61 7269 6f29 2069 6e20 602e 2f63 6f6e  nario) in `./con
+00001530: 6669 675f 6669 6c65 7360 2061 6e64 206d  fig_files` and m
+00001540: 6f64 6966 7920 7468 6520 7661 6c75 6573  odify the values
+00001550: 2074 6865 7265 0a0a 3c2f 6465 7461 696c   there..</detail
+00001560: 733e 0a0a 2323 20f0 9f9a a720 446f 6375  s>..## .... Docu
+00001570: 6d65 6e74 6174 696f 6e0a 0a54 6865 2064  mentation..The d
+00001580: 6f63 756d 656e 7461 7469 6f6e 206f 6620  ocumentation of 
+00001590: 6f75 7220 746f 6f6c 626f 7820 6973 2061  our toolbox is a
+000015a0: 7661 696c 6162 6c65 206f 6e20 6f75 7220  vailable on our 
+000015b0: 7765 6273 6974 653a 2068 7474 7073 3a2f  website: https:/
+000015c0: 2f63 7073 2e70 6167 6573 2e67 6974 6c61  /cps.pages.gitla
+000015d0: 622e 6c72 7a2e 6465 2f63 6f6d 6d6f 6e72  b.lrz.de/commonr
+000015e0: 6f61 642f 636f 6d6d 6f6e 726f 6164 2d63  oad/commonroad-c
+000015f0: 7269 7469 6361 6c69 7479 2d6d 6561 7375  riticality-measu
+00001600: 7265 732f 2e0a 3c64 6574 6169 6c73 3e0a  res/..<details>.
+00001610: 3c73 756d 6d61 7279 3e3c 623e 4275 696c  <summary><b>Buil
+00001620: 6420 646f 6375 6d65 6e74 6174 696f 6e20  d documentation 
+00001630: 6c6f 6361 6c6c 793c 2f62 3e3c 2f73 756d  locally</b></sum
+00001640: 6d61 7279 3e0a 496e 206f 7264 6572 2074  mary>.In order t
+00001650: 6f20 6765 6e65 7261 7465 2074 6865 2064  o generate the d
+00001660: 6f63 756d 656e 7461 7469 6f6e 2076 6961  ocumentation via
+00001670: 2053 7068 696e 7820 6c6f 6361 6c6c 792c   Sphinx locally,
+00001680: 2072 756e 2074 6865 2066 6f6c 6c6f 7769   run the followi
+00001690: 6e67 2063 6f6d 6d61 6e64 7320 696e 2074  ng commands in t
+000016a0: 6865 2072 6f6f 7420 6469 7265 6374 6f72  he root director
+000016b0: 793a 0a0a 6060 6062 6173 680a 2420 7069  y:..```bash.$ pi
+000016c0: 7020 696e 7374 616c 6c20 2d72 202e 2f64  p install -r ./d
+000016d0: 6f63 732f 7265 7175 6972 656d 656e 7473  ocs/requirements
+000016e0: 5f64 6f63 2e74 7874 0a24 2063 6420 646f  _doc.txt.$ cd do
+000016f0: 6373 2f73 7068 696e 780a 2420 6d61 6b65  cs/sphinx.$ make
+00001700: 2068 746d 6c0a 6060 600a 0a54 6865 2064   html.```..The d
+00001710: 6f63 756d 656e 7461 7469 6f6e 2063 616e  ocumentation can
+00001720: 2074 6865 6e20 6265 206c 6175 6e63 6865   then be launche
+00001730: 6420 6279 2062 726f 7773 696e 6720 6060  d by browsing ``
+00001740: 2e2f 646f 6373 2f73 7068 696e 782f 6275  ./docs/sphinx/bu
+00001750: 696c 642f 6874 6d6c 2f69 6e64 6578 2e68  ild/html/index.h
+00001760: 746d 6c2f 6060 2e0a 3c2f 6465 7461 696c  tml/``..</detail
+00001770: 733e 0a0a 2323 20f0 9f8c 9f20 436f 6e74  s>..## .... Cont
+00001780: 7269 6275 746f 7273 2028 696e 2061 6c70  ributors (in alp
+00001790: 6861 6265 7469 6361 6c20 6f72 6465 7220  habetical order 
+000017a0: 6279 206c 6173 7420 6e61 6d65 290a 0a2d  by last name)..-
+000017b0: 204c 6967 756f 2043 6865 6e0a 2d20 4d61   Liguo Chen.- Ma
+000017c0: 7269 7573 2045 7261 7468 0a2d 2059 7561  rius Erath.- Yua
+000017d0: 6e66 6569 204c 696e 0a2d 2053 6562 6173  nfei Lin.- Sebas
+000017e0: 7469 616e 204d 6169 6572 686f 6665 720a  tian Maierhofer.
+000017f0: 2d20 4976 616e 6120 5065 6e65 7661 0a2d  - Ivana Peneva.-
+00001800: 204b 756e 2051 6961 6e0a 2d20 4f6c 6976   Kun Qian.- Oliv
+00001810: 6572 2053 7065 6368 740a 2d20 5369 6368  er Specht.- Sich
+00001820: 656e 6720 5761 6e67 0a2d 2059 6f75 7261  eng Wang.- Youra
+00001830: 6e20 5761 6e67 0a2d 205a 656b 756e 2058  n Wang.- Zekun X
+00001840: 696e 670a 2d20 5a69 7169 616e 2058 750a  ing.- Ziqian Xu.
+00001850: 0a23 2320 f09f 9496 2043 6974 6174 696f  .## .... Citatio
+00001860: 6e0a 4966 2079 6f75 2075 7365 2060 636f  n.If you use `co
+00001870: 6d6d 6f6e 726f 6164 2d63 7269 6d65 6020  mmonroad-crime` 
+00001880: 666f 7220 6163 6164 656d 6963 2077 6f72  for academic wor
+00001890: 6b2c 2077 6520 6869 6768 6c79 2065 6e63  k, we highly enc
+000018a0: 6f75 7261 6765 2079 6f75 2074 6f20 6369  ourage you to ci
+000018b0: 7465 206f 7572 2070 6170 6572 3a0a 6060  te our paper:.``
+000018c0: 6074 6578 740a 4049 6e50 726f 6365 6564  `text.@InProceed
+000018d0: 696e 6773 7b6c 696e 3230 3233 6372 696d  ings{lin2023crim
+000018e0: 652c 0a20 2020 2020 2074 6974 6c65 2020  e,.      title  
+000018f0: 2020 203d 207b 7b43 6f6d 6d6f 6e52 6f61     = {{CommonRoa
+00001900: 642d 4372 694d 657d 3a20 7b41 7d20 546f  d-CriMe}: {A} To
+00001910: 6f6c 626f 7820 666f 7220 4372 6974 6963  olbox for Critic
+00001920: 616c 6974 7920 4d65 6173 7572 6573 206f  ality Measures o
+00001930: 6620 4175 746f 6e6f 6d6f 7573 2056 6568  f Autonomous Veh
+00001940: 6963 6c65 737d 2c0a 2020 2020 2020 6175  icles},.      au
+00001950: 7468 6f72 2020 2020 3d20 7b59 7561 6e66  thor    = {Yuanf
+00001960: 6569 204c 696e 2061 6e64 204d 6174 7468  ei Lin and Matth
+00001970: 6961 7320 416c 7468 6f66 667d 2c0a 2020  ias Althoff},.  
+00001980: 2020 2020 626f 6f6b 7469 746c 6520 3d20      booktitle = 
+00001990: 7b50 726f 632e 206f 6620 7468 6520 4945  {Proc. of the IE
+000019a0: 4545 2049 6e74 656c 6c2e 2056 6568 2e20  EE Intell. Veh. 
+000019b0: 5379 6d70 2e7d 2c20 2020 2020 0a20 2020  Symp.},     .   
+000019c0: 2020 2070 6167 6573 2020 2020 203d 207b     pages     = {
+000019d0: 312d 387d 2c20 0a20 2020 2020 2079 6561  1-8}, .      yea
+000019e0: 7220 2020 2020 203d 207b 3230 3233 7d2c  r      = {2023},
+000019f0: 0a7d 0a60 6060 0a49 6620 796f 7520 7573  .}.```.If you us
+00001a00: 6520 7468 6973 2070 726f 6a65 6374 2773  e this project's
+00001a10: 2063 6f64 6520 696e 2069 6e64 7573 7472   code in industr
+00001a20: 792c 2077 6527 6420 6c6f 7665 2074 6f20  y, we'd love to 
+00001a30: 6865 6172 2066 726f 6d20 796f 7520 6173  hear from you as
+00001a40: 2077 656c 6c3b 200a 6665 656c 2066 7265   well; .feel fre
+00001a50: 6520 746f 2072 6561 6368 206f 7574 2074  e to reach out t
+00001a60: 6f20 5b59 7561 6e66 6569 204c 696e 5d28  o [Yuanfei Lin](
+00001a70: 6d61 696c 746f 3a79 7561 6e66 6569 2e6c  mailto:yuanfei.l
+00001a80: 696e 4074 756d 2e64 6529 2064 6972 6563  in@tum.de) direc
+00001a90: 746c 792e 0a                             tly..
```

### Comparing `commonroad-crime-0.3.3/README.md` & `commonroad_crime-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,306 +1,337 @@
 00000000: 2320 436f 6d6d 6f6e 526f 6164 2d43 7269  # CommonRoad-Cri
 00000010: 4d65 0a21 5b69 6d61 6765 2069 6e66 6f5d  Me.![image info]
-00000020: 2868 7474 7073 3a2f 2f67 6974 6c61 622e  (https://gitlab.
-00000030: 6c72 7a2e 6465 2f74 756d 2d63 7073 2f63  lrz.de/tum-cps/c
-00000040: 6f6d 6d6f 6e72 6f61 642d 6372 696d 652f  ommonroad-crime/
-00000050: 2d2f 7261 772f 6d61 7374 6572 2f64 6f63  -/raw/master/doc
-00000060: 732f 6669 6775 7265 732f 4372 694d 652d  s/figures/CriMe-
-00000070: 6261 6e6e 6572 2e70 6e67 290a 5b21 5b4c  banner.png).[![L
-00000080: 696e 7578 5d28 6874 7470 733a 2f2f 696d  inux](https://im
-00000090: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000000a0: 6765 2f6f 732d 6c69 6e75 783f 266c 6f67  ge/os-linux?&log
-000000b0: 6f3d 4c69 6e75 7826 6c6f 676f 436f 6c6f  o=Linux&logoColo
-000000c0: 723d 7768 6974 6526 6c61 6265 6c43 6f6c  r=white&labelCol
-000000d0: 6f72 3d67 7261 7929 5d28 6874 7470 733a  or=gray)](https:
-000000e0: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
-000000f0: 672f 7079 7069 2f63 6f6d 6d6f 6e72 6f61  g/pypi/commonroa
-00000100: 642d 6f70 656e 7363 656e 6172 696f 2d63  d-openscenario-c
-00000110: 6f6e 7665 7274 6572 2f29 0a5b 215b 5079  onverter/).[![Py
-00000120: 5049 2076 6572 7369 6f6e 2066 7572 792e  PI version fury.
-00000130: 696f 5d28 6874 7470 733a 2f2f 6261 6467  io](https://badg
-00000140: 652e 6675 7279 2e69 6f2f 7079 2f63 6f6d  e.fury.io/py/com
-00000150: 6d6f 6e72 6f61 642d 6372 696d 652e 7376  monroad-crime.sv
-00000160: 673f 7374 796c 653d 706c 6173 7469 6329  g?style=plastic)
-00000170: 5d28 6874 7470 733a 2f2f 7079 7069 2e70  ](https://pypi.p
-00000180: 7974 686f 6e2e 6f72 672f 7079 7069 2f63  ython.org/pypi/c
-00000190: 6f6d 6d6f 6e72 6f61 642d 6372 696d 652f  ommonroad-crime/
-000001a0: 290a 5b21 5b50 7950 4920 6c69 6365 6e73  ).[![PyPI licens
-000001b0: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
-000001c0: 6869 656c 6473 2e69 6f2f 7079 7069 2f6c  hields.io/pypi/l
-000001d0: 2f63 6f6d 6d6f 6e72 6f61 642d 6372 696d  /commonroad-crim
-000001e0: 652e 7376 673f 7374 796c 653d 706c 6173  e.svg?style=plas
-000001f0: 7469 6329 5d28 6874 7470 733a 2f2f 7079  tic)](https://py
-00000200: 7069 2e70 7974 686f 6e2e 6f72 672f 7079  pi.python.org/py
-00000210: 7069 2f63 6f6d 6d6f 6e72 6f61 642d 6372  pi/commonroad-cr
-00000220: 696d 652f 293c 6272 3e0a 5b21 5b50 7950  ime/)<br>.[![PyP
-00000230: 4920 646f 776e 6c6f 6164 206d 6f6e 7468  I download month
-00000240: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000250: 6965 6c64 732e 696f 2f70 7970 692f 646d  ields.io/pypi/dm
-00000260: 2f63 6f6d 6d6f 6e72 6f61 642d 6372 696d  /commonroad-crim
-00000270: 652e 7376 673f 7374 796c 653d 706c 6173  e.svg?style=plas
-00000280: 7469 6326 6c61 6265 6c3d 5079 5049 2532  tic&label=PyPI%2
-00000290: 3064 6f77 6e6c 6f61 6473 295d 2868 7474  0downloads)](htt
-000002a0: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
-000002b0: 2e6f 7267 2f70 7970 692f 636f 6d6d 6f6e  .org/pypi/common
-000002c0: 726f 6164 2d63 7269 6d65 2f29 200a 5b21  road-crime/) .[!
-000002d0: 5b50 7950 4920 646f 776e 6c6f 6164 2077  [PyPI download w
-000002e0: 6565 6b5d 2868 7474 7073 3a2f 2f69 6d67  eek](https://img
-000002f0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000300: 2f64 772f 636f 6d6d 6f6e 726f 6164 2d63  /dw/commonroad-c
-00000310: 7269 6d65 2e73 7667 3f73 7479 6c65 3d70  rime.svg?style=p
-00000320: 6c61 7374 6963 266c 6162 656c 3d50 7950  lastic&label=PyP
-00000330: 4925 3230 646f 776e 6c6f 6164 7329 5d28  I%20downloads)](
-00000340: 6874 7470 733a 2f2f 7079 7069 2e70 7974  https://pypi.pyt
-00000350: 686f 6e2e 6f72 672f 7079 7069 2f63 6f6d  hon.org/pypi/com
-00000360: 6d6f 6e72 6f61 642d 6372 696d 652f 293c  monroad-crime/)<
-00000370: 6272 3e0a 0a54 6f6f 6c62 6f78 2074 6f20  br>..Toolbox to 
-00000380: 636f 6d70 7574 6520 2a2a 4372 692a 2a74  compute **Cri**t
-00000390: 6963 616c 6974 7920 2a2a 4d65 2a2a 6173  icality **Me**as
-000003a0: 7572 6573 200a 2865 2e67 2e20 7469 6d65  ures .(e.g. time
-000003b0: 2d74 6f2d 636f 6c6c 6973 696f 6e2c 2074  -to-collision, t
-000003c0: 696d 652d 746f 2d72 6561 6374 2c2e 2e2e  ime-to-react,...
-000003d0: 292e 2053 7563 6820 6d65 6173 7572 6573  ). Such measures
-000003e0: 0a63 616e 2062 6520 7573 6564 2074 6f20  .can be used to 
-000003f0: 7472 6967 6765 7220 7761 726e 696e 6773  trigger warnings
-00000400: 2061 6e64 2065 6d65 7267 656e 6379 206d   and emergency m
-00000410: 616e 6575 7665 7273 200a 696e 2064 7269  aneuvers .in dri
-00000420: 7665 7220 6173 7369 7374 616e 6365 2073  ver assistance s
-00000430: 7973 7465 6d73 206f 7220 7265 7061 6972  ystems or repair
-00000440: 2061 6e20 696e 6665 6173 6962 6c65 200a   an infeasible .
-00000450: 7472 616a 6563 746f 7279 2e20 0a0a 2d20  trajectory. ..- 
-00000460: 4966 2079 6f75 2068 6176 6520 7175 6573  If you have ques
-00000470: 7469 6f6e 7320 6f72 2077 616e 7420 746f  tions or want to
-00000480: 2072 6570 6f72 7420 7072 6f62 6c65 6d73   report problems
-00000490: 206f 7220 7375 6767 6573 7469 6f6e 732c   or suggestions,
-000004a0: 2070 6c65 6173 6520 7374 6172 7420 6120   please start a 
-000004b0: 5b47 6974 6875 6220 6469 7363 7573 7369  [Github discussi
-000004c0: 6f6e 5d28 6874 7470 733a 2f2f 6769 7468  on](https://gith
-000004d0: 7562 2e63 6f6d 2f6f 7267 732f 436f 6d6d  ub.com/orgs/Comm
-000004e0: 6f6e 526f 6164 2f64 6973 6375 7373 696f  onRoad/discussio
-000004f0: 6e73 292e 200a 0a23 2323 20f0 9f9a a720  ns). ..### .... 
-00000500: 5765 204d 6561 7375 7265 20f0 9d95 ae6f  We Measure ....o
-00000510: 6d6d 6f6e 20f0 9d95 bd6f 6164 20f0 9d95  mmon ....oad ...
-00000520: ae72 69f0 9d95 b865 2120 f09f 9a94 0a0a  .ri....e! ......
-00000530: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-00000540: 2047 7569 6465 0a0a 6063 6f6d 6d6f 6e72   Guide..`commonr
-00000550: 6f61 642d 6372 696d 6560 2063 616e 2062  oad-crime` can b
-00000560: 6520 696e 7374 616c 6c65 6420 7769 7468  e installed with
-00000570: 3a0a 0a60 6060 2062 6173 680a 2420 7069  :..``` bash.$ pi
-00000580: 7020 696e 7374 616c 6c20 636f 6d6d 6f6e  p install common
-00000590: 726f 6164 2d63 7269 6d65 0a60 6060 0a46  road-crime.```.F
-000005a0: 6f72 2061 6464 696e 6720 6e65 7720 6d65  or adding new me
-000005b0: 6173 7572 6573 2c20 7765 2072 6563 6f6d  asures, we recom
-000005c0: 6d65 6e64 2075 7369 6e67 205b 416e 6163  mend using [Anac
-000005d0: 6f6e 6461 5d28 6874 7470 733a 2f2f 7777  onda](https://ww
-000005e0: 772e 616e 6163 6f6e 6461 2e63 6f6d 2f29  w.anaconda.com/)
-000005f0: 2074 6f20 6d61 6e61 6765 2079 6f75 7220   to manage your 
-00000600: 656e 7669 726f 6e6d 656e 7420 736f 2074  environment so t
-00000610: 6861 7420 6576 656e 2069 6620 796f 7520  hat even if you 
-00000620: 6d65 7373 2073 6f6d 6574 6869 6e67 2075  mess something u
-00000630: 702c 2079 6f75 2063 616e 2061 6c77 6179  p, you can alway
-00000640: 7320 6861 7665 2061 2073 6166 6520 616e  s have a safe an
-00000650: 6420 636c 6561 6e20 7265 7374 6172 742e  d clean restart.
-00000660: 2041 2067 7569 6465 2066 6f72 206d 616e   A guide for man
-00000670: 6167 696e 6720 7079 7468 6f6e 2065 6e76  aging python env
-00000680: 6972 6f6e 6d65 6e74 7320 7769 7468 2041  ironments with A
-00000690: 6e61 636f 6e64 6120 6361 6e20 6265 2066  naconda can be f
-000006a0: 6f75 6e64 205b 6865 7265 5d28 6874 7470  ound [here](http
-000006b0: 733a 2f2f 636f 6e64 612e 696f 2f70 726f  s://conda.io/pro
-000006c0: 6a65 6374 732f 636f 6e64 612f 656e 2f6c  jects/conda/en/l
-000006d0: 6174 6573 742f 7573 6572 2d67 7569 6465  atest/user-guide
-000006e0: 2f74 6173 6b73 2f6d 616e 6167 652d 656e  /tasks/manage-en
-000006f0: 7669 726f 6e6d 656e 7473 2e68 746d 6c29  vironments.html)
-00000700: 2e0a 0a41 6674 6572 2069 6e73 7461 6c6c  ...After install
-00000710: 696e 6720 416e 6163 6f6e 6461 2c20 6372  ing Anaconda, cr
-00000720: 6561 7465 2061 206e 6577 2065 6e76 6972  eate a new envir
-00000730: 6f6e 6d65 6e74 2077 6974 683a 0a60 6060  onment with:.```
-00000740: 2062 6173 680a 2420 636f 6e64 6120 6372   bash.$ conda cr
-00000750: 6561 7465 202d 6e20 636f 6d6d 6f6e 726f  eate -n commonro
-00000760: 6164 2d70 7933 3820 7079 7468 6f6e 3d33  ad-py38 python=3
-00000770: 2e38 202d 790a 6060 600a 0a48 6572 6520  .8 -y.```..Here 
-00000780: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
-00000790: 656e 7669 726f 6e6d 656e 7420 6973 2063  environment is c
-000007a0: 616c 6c65 6420 2a2a 636f 6d6d 6f6e 726f  alled **commonro
-000007b0: 6164 2d70 7933 382a 2a2e 2059 6f75 206d  ad-py38**. You m
-000007c0: 6179 2061 6c73 6f20 6368 616e 6765 2074  ay also change t
-000007d0: 6869 7320 6e61 6d65 2061 7320 796f 7520  his name as you 
-000007e0: 7769 7368 2e20 496e 2073 7563 6820 6361  wish. In such ca
-000007f0: 7365 2c20 646f 6e27 7420 666f 7267 6574  se, don't forget
-00000800: 2074 6f20 6368 616e 6765 2069 7420 696e   to change it in
-00000810: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00000820: 6f6d 6d61 6e64 7320 6173 2077 656c 6c2e  ommands as well.
-00000830: 202a 2a41 6c77 6179 7320 6163 7469 7661   **Always activa
-00000840: 7465 2a2a 2074 6869 7320 656e 7669 726f  te** this enviro
-00000850: 6e6d 656e 7420 6265 666f 7265 2079 6f75  nment before you
-00000860: 2064 6f20 616e 7974 6869 6e67 2072 656c   do anything rel
-00000870: 6174 6564 3a0a 0a60 6060 7368 0a24 2063  ated:..```sh.$ c
-00000880: 6f6e 6461 2061 6374 6976 6174 6520 636f  onda activate co
-00000890: 6d6d 6f6e 726f 6164 2d70 7933 380a 6f72  mmonroad-py38.or
-000008a0: 0a24 2073 6f75 7263 6520 6163 7469 7661  .$ source activa
-000008b0: 7465 2063 6f6d 6d6f 6e72 6f61 642d 7079  te commonroad-py
-000008c0: 3338 0a60 6060 0a54 6865 6e2c 2069 6e73  38.```.Then, ins
-000008d0: 7461 6c6c 2074 6865 2064 6570 656e 6465  tall the depende
-000008e0: 6e63 6965 7320 7769 7468 3a0a 0a60 6060  ncies with:..```
-000008f0: 7368 0a24 2063 6420 3c70 6174 682d 746f  sh.$ cd <path-to
-00000900: 2d74 6869 732d 7265 706f 3e0a 2420 7069  -this-repo>.$ pi
-00000910: 7020 696e 7374 616c 6c20 2d65 202e 0a24  p install -e ..$
-00000920: 2063 6f6e 6461 2064 6576 656c 6f70 202e   conda develop .
-00000930: 0a60 6060 0a0a 546f 2074 6573 7420 7468  .```..To test th
-00000940: 6520 696e 7374 616c 6c69 7469 6f6e 2c20  e installition, 
-00000950: 7275 6e20 756e 6974 7465 7374 3a0a 6060  run unittest:.``
-00000960: 6062 6173 680a 2420 6364 2074 6573 7473  `bash.$ cd tests
-00000970: 0a24 2070 7974 686f 6e20 2d6d 2075 6e69  .$ python -m uni
-00000980: 7474 6573 7420 2d76 0a60 6060 0a0a 0a54  ttest -v.```...T
-00000990: 6f20 6765 7420 7374 6172 7465 6420 796f  o get started yo
-000009a0: 7572 206a 6f75 726e 6579 2077 6974 6820  ur journey with 
-000009b0: 6f75 7220 6372 6974 6963 616c 6974 7920  our criticality 
-000009c0: 6d65 6173 7572 6573 2c20 6368 6563 6b20  measures, check 
-000009d0: 7468 6520 6074 7574 6f72 6961 6c73 6020  the `tutorials` 
-000009e0: 616e 6420 7468 6520 666f 6c6c 6f77 696e  and the followin
-000009f0: 6720 7469 7073 2e0a 0a23 2323 2048 6f77  g tips...### How
-00000a00: 2074 6f20 6164 6420 6e65 7720 6372 6974   to add new crit
-00000a10: 6963 616c 6974 7920 6d65 6173 7572 650a  icality measure.
-00000a20: 312e 2063 7265 6174 6520 6120 6e65 7720  1. create a new 
-00000a30: 6272 616e 6368 2077 6974 6820 6066 6561  branch with `fea
-00000a40: 7475 7265 2d3c 6d65 6173 7572 652d 6e61  ture-<measure-na
-00000a50: 6d65 3e60 2061 6e64 2063 6865 636b 6f75  me>` and checkou
-00000a60: 7420 7468 6520 6272 616e 6368 0a32 2e20  t the branch.2. 
-00000a70: 6e61 7669 6761 7465 2074 6f20 6063 6f6d  navigate to `com
-00000a80: 6d6f 6e72 6f61 645f 6372 696d 652f 6461  monroad_crime/da
-00000a90: 7461 5f73 7472 7563 7475 7265 2f74 7970  ta_structure/typ
-00000aa0: 652e 7079 6020 746f 2066 696e 6420 7468  e.py` to find th
-00000ab0: 6520 636f 7272 6563 7420 6361 7465 676f  e correct catego
-00000ac0: 7279 206f 6620 7468 6520 6d65 6173 7572  ry of the measur
-00000ad0: 6520 616e 6420 6164 6420 616e 200a 656e  e and add an .en
-00000ae0: 756d 6572 6174 696f 6e20 656e 7472 7920  umeration entry 
-00000af0: 603c 6162 6272 6576 6961 7469 6f6e 3e3a  `<abbreviation>:
-00000b00: 203c 6578 706c 616e 6174 696f 6e3e 600a   <explanation>`.
-00000b10: 332e 206e 6176 6967 6174 6520 746f 2060  3. navigate to `
-00000b20: 636f 6d6d 6f6e 726f 6164 5f63 7269 6d65  commonroad_crime
-00000b30: 2f6d 6561 7375 7265 6020 746f 2066 696e  /measure` to fin
-00000b40: 6420 7468 6520 6162 6f76 652d 6d65 6e74  d the above-ment
-00000b50: 696f 6e65 6420 6361 7465 676f 7279 2061  ioned category a
-00000b60: 6e64 2063 7265 6174 6520 6120 7079 7468  nd create a pyth
-00000b70: 6f6e 2066 696c 6520 6e61 6d65 640a 603c  on file named.`<
-00000b80: 6162 6272 6576 6961 7469 6f6e 3e2e 7079  abbreviation>.py
-00000b90: 602e 2054 6865 6e20 6372 6561 7465 2061  `. Then create a
-00000ba0: 2063 6c61 7373 2069 6e68 6572 6974 696e   class inheritin
-00000bb0: 6720 7468 6520 6043 7269 4d65 4261 7365  g the `CriMeBase
-00000bc0: 6020 756e 6465 7220 6063 6f6d 6d6f 6e72  ` under `commonr
-00000bd0: 6f61 645f 6372 696d 652f 6461 7461 5f73  oad_crime/data_s
-00000be0: 7472 7563 7475 7265 2f62 6173 652e 7079  tructure/base.py
-00000bf0: 600a 342e 2073 696d 696c 6172 2074 6f20  `.4. similar to 
-00000c00: 6f74 6865 7220 6d65 6173 7572 6573 2c20  other measures, 
-00000c10: 796f 7520 6e65 6564 2074 6f20 696d 706c  you need to impl
-00000c20: 656d 656e 7420 7468 6520 6063 6f6d 7075  ement the `compu
-00000c30: 7465 2829 6020 616e 6420 6076 6973 7561  te()` and `visua
-00000c40: 6c69 7a65 2829 6020 6675 6e63 7469 6f6e  lize()` function
-00000c50: 730a 0a23 2323 2048 6f77 2074 6f20 6465  s..### How to de
-00000c60: 6669 6e65 2063 6f6e 6669 6775 7261 7469  fine configurati
-00000c70: 6f6e 2070 6172 616d 6574 6572 7320 6f66  on parameters of
-00000c80: 2074 6865 206d 6561 7375 7265 0a31 2e20   the measure.1. 
-00000c90: 6e61 7669 6761 7465 2074 6f20 6063 6f6d  navigate to `com
-00000ca0: 6d6f 6e72 6f61 645f 6372 696d 652f 6461  monroad_crime/da
-00000cb0: 7461 5f73 7472 7563 7475 7265 2f63 6f6e  ta_structure/con
-00000cc0: 6669 6775 6174 696f 6e2e 7079 6020 746f  figuation.py` to
-00000cd0: 2066 696e 6420 7468 6520 6162 6f76 652d   find the above-
-00000ce0: 6d65 6e74 696f 6e65 6420 6361 7465 676f  mentioned catego
-00000cf0: 7279 2061 6e64 2061 6464 2061 206e 6577  ry and add a new
-00000d00: 200a 696e 7374 616e 6365 2074 6f20 7468   .instance to th
-00000d10: 6520 636c 6173 7320 6173 2060 7365 6c66  e class as `self
-00000d20: 2e3c 7061 7261 6d65 7465 723e 203d 2063  .<parameter> = c
-00000d30: 6f6e 6669 675f 7265 6c65 7661 6e74 2e3c  onfig_relevant.<
-00000d40: 7061 7261 6d65 7465 723e 600a 322e 2079  parameter>`.2. y
-00000d50: 6f75 2063 616e 2074 6865 6e20 6469 7265  ou can then dire
-00000d60: 6374 6c79 2063 616c 6c20 7468 6520 7661  ctly call the va
-00000d70: 6c75 6573 2075 7369 6e67 2060 7365 6c66  lues using `self
-00000d80: 2e63 6f6e 6669 6775 7261 7469 6f6e 2e3c  .configuration.<
-00000d90: 6361 7465 676f 7279 3e2e 3c70 6172 616d  category>.<param
-00000da0: 6574 6572 3e60 2069 6e20 796f 7572 206d  eter>` in your m
-00000db0: 6561 7375 7265 2063 6c61 7373 0a33 2e20  easure class.3. 
-00000dc0: 746f 206f 7665 7272 6964 6520 7468 6520  to override the 
-00000dd0: 6465 6661 756c 7420 7061 7261 6d65 7465  default paramete
-00000de0: 7220 7661 6c75 6573 2c20 6372 6561 7465  r values, create
-00000df0: 2061 2060 7961 6d6c 6020 6669 6c65 2028   a `yaml` file (
-00000e00: 6e61 6d65 2069 7420 7468 6520 7361 6d65  name it the same
-00000e10: 2061 7320 7468 6520 7363 656e 6172 696f   as the scenario
-00000e20: 2920 696e 2060 2e2f 636f 6e66 6967 5f66  ) in `./config_f
-00000e30: 696c 6573 6020 616e 6420 6d6f 6469 6679  iles` and modify
-00000e40: 2074 6865 2076 616c 7565 7320 7468 6572   the values ther
-00000e50: 650a 2323 2044 6f63 756d 656e 7461 7469  e.## Documentati
-00000e60: 6f6e 0a0a 5468 6520 646f 6375 6d65 6e74  on..The document
-00000e70: 6174 696f 6e20 6f66 206f 7572 2074 6f6f  ation of our too
-00000e80: 6c62 6f78 2069 7320 6176 6169 6c61 626c  lbox is availabl
-00000e90: 6520 6f6e 206f 7572 2077 6562 7369 7465  e on our website
-00000ea0: 3a20 6874 7470 733a 2f2f 6370 732e 7061  : https://cps.pa
-00000eb0: 6765 732e 6769 746c 6162 2e6c 727a 2e64  ges.gitlab.lrz.d
-00000ec0: 652f 636f 6d6d 6f6e 726f 6164 2f63 6f6d  e/commonroad/com
-00000ed0: 6d6f 6e72 6f61 642d 6372 6974 6963 616c  monroad-critical
-00000ee0: 6974 792d 6d65 6173 7572 6573 2f2e 0a0a  ity-measures/...
-00000ef0: 496e 206f 7264 6572 2074 6f20 6765 6e65  In order to gene
-00000f00: 7261 7465 2074 6865 2064 6f63 756d 656e  rate the documen
-00000f10: 7461 7469 6f6e 2076 6961 2053 7068 696e  tation via Sphin
-00000f20: 7820 6c6f 6361 6c6c 792c 2072 756e 2074  x locally, run t
-00000f30: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-00000f40: 6d61 6e64 7320 696e 2074 6865 2072 6f6f  mands in the roo
-00000f50: 7420 6469 7265 6374 6f72 793a 0a0a 6060  t directory:..``
-00000f60: 6062 6173 680a 2420 7069 7020 696e 7374  `bash.$ pip inst
-00000f70: 616c 6c20 2d72 202e 2f64 6f63 732f 7265  all -r ./docs/re
-00000f80: 7175 6972 656d 656e 7473 5f64 6f63 2e74  quirements_doc.t
-00000f90: 7874 0a24 2063 6420 646f 6373 2f73 7068  xt.$ cd docs/sph
-00000fa0: 696e 780a 2420 6d61 6b65 2068 746d 6c0a  inx.$ make html.
-00000fb0: 6060 600a 0a54 6865 2064 6f63 756d 656e  ```..The documen
-00000fc0: 7461 7469 6f6e 2063 616e 2074 6865 6e20  tation can then 
-00000fd0: 6265 206c 6175 6e63 6865 6420 6279 2062  be launched by b
-00000fe0: 726f 7773 696e 6720 6060 2e2f 646f 6373  rowsing ``./docs
-00000ff0: 2f73 7068 696e 782f 6275 696c 642f 6874  /sphinx/build/ht
-00001000: 6d6c 2f69 6e64 6578 2e68 746d 6c2f 6060  ml/index.html/``
-00001010: 2e0a 0a23 2323 2043 6f6e 7472 6962 7574  ...### Contribut
-00001020: 6f72 7320 2869 6e20 616c 7068 6162 6574  ors (in alphabet
-00001030: 6963 616c 206f 7264 6572 2062 7920 6c61  ical order by la
-00001040: 7374 206e 616d 6529 0a2d 204c 6967 756f  st name).- Liguo
-00001050: 2043 6865 6e0a 2d20 5975 616e 6665 6920   Chen.- Yuanfei 
-00001060: 4c69 6e0a 2d20 5365 6261 7374 6961 6e20  Lin.- Sebastian 
-00001070: 4d61 6965 7268 6f66 6572 0a2d 2049 7661  Maierhofer.- Iva
-00001080: 6e61 2050 656e 6576 610a 2d20 4b75 6e20  na Peneva.- Kun 
-00001090: 5169 616e 0a2d 204f 6c69 7665 7220 5370  Qian.- Oliver Sp
-000010a0: 6563 6874 0a2d 2053 6963 6865 6e67 2057  echt.- Sicheng W
-000010b0: 616e 670a 2d20 596f 7572 616e 2057 616e  ang.- Youran Wan
-000010c0: 670a 2d20 5a65 6b75 6e20 5869 6e67 0a2d  g.- Zekun Xing.-
-000010d0: 205a 6971 6961 6e20 5875 0a0a 2323 2320   Ziqian Xu..### 
-000010e0: 4369 7461 7469 6f6e 0a49 6620 796f 7520  Citation.If you 
-000010f0: 7573 6520 6063 6f6d 6d6f 6e72 6f61 642d  use `commonroad-
-00001100: 6372 696d 6560 2066 6f72 2061 6361 6465  crime` for acade
-00001110: 6d69 6320 776f 726b 2c20 7765 2068 6967  mic work, we hig
-00001120: 686c 7920 656e 636f 7572 6167 6520 796f  hly encourage yo
-00001130: 7520 746f 2063 6974 6520 6f75 7220 7061  u to cite our pa
-00001140: 7065 723a 0a60 6060 7465 7874 0a40 496e  per:.```text.@In
-00001150: 5072 6f63 6565 6469 6e67 737b 6c69 6e32  Proceedings{lin2
-00001160: 3032 3363 7269 6d65 2c0a 2020 2020 2020  023crime,.      
-00001170: 7469 746c 6520 2020 2020 3d20 7b7b 436f  title     = {{Co
-00001180: 6d6d 6f6e 526f 6164 2d43 7269 4d65 7d3a  mmonRoad-CriMe}:
-00001190: 207b 417d 2054 6f6f 6c62 6f78 2066 6f72   {A} Toolbox for
-000011a0: 2043 7269 7469 6361 6c69 7479 204d 6561   Criticality Mea
-000011b0: 7375 7265 7320 6f66 2041 7574 6f6e 6f6d  sures of Autonom
-000011c0: 6f75 7320 5665 6869 636c 6573 7d2c 0a20  ous Vehicles},. 
-000011d0: 2020 2020 2061 7574 686f 7220 2020 203d       author    =
-000011e0: 207b 5975 616e 6665 6920 4c69 6e20 616e   {Yuanfei Lin an
-000011f0: 6420 4d61 7474 6869 6173 2041 6c74 686f  d Matthias Altho
-00001200: 6666 7d2c 0a20 2020 2020 2062 6f6f 6b74  ff},.      bookt
-00001210: 6974 6c65 203d 207b 5072 6f63 2e20 6f66  itle = {Proc. of
-00001220: 2074 6865 2049 4545 4520 496e 7465 6c6c   the IEEE Intell
-00001230: 2e20 5665 682e 2053 796d 702e 7d2c 2020  . Veh. Symp.},  
-00001240: 2020 200a 2020 2020 2020 7061 6765 7320     .      pages 
-00001250: 2020 2020 3d20 7b31 2d38 7d2c 200a 2020      = {1-8}, .  
-00001260: 2020 2020 7965 6172 2020 2020 2020 3d20      year      = 
-00001270: 7b32 3032 337d 2c0a 7d0a 6060 600a 4966  {2023},.}.```.If
-00001280: 2079 6f75 2075 7365 2074 6869 7320 7072   you use this pr
-00001290: 6f6a 6563 7427 7320 636f 6465 2069 6e20  oject's code in 
-000012a0: 696e 6475 7374 7279 2c20 7765 2764 206c  industry, we'd l
-000012b0: 6f76 6520 746f 2068 6561 7220 6672 6f6d  ove to hear from
-000012c0: 2079 6f75 2061 7320 7765 6c6c 3b20 0a66   you as well; .f
-000012d0: 6565 6c20 6672 6565 2074 6f20 7265 6163  eel free to reac
-000012e0: 6820 6f75 7420 746f 205b 5975 616e 6665  h out to [Yuanfe
-000012f0: 6920 4c69 6e5d 286d 6169 6c74 6f3a 7975  i Lin](mailto:yu
-00001300: 616e 6665 692e 6c69 6e40 7475 6d2e 6465  anfei.lin@tum.de
-00001310: 2920 6469 7265 6374 6c79 2e0a            ) directly..
+00000020: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
+00000030: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000040: 6f6d 2f43 6f6d 6d6f 6e52 6f61 642f 636f  om/CommonRoad/co
+00000050: 6d6d 6f6e 726f 6164 2d63 7269 6d65 2f64  mmonroad-crime/d
+00000060: 6576 656c 6f70 2f64 6f63 732f 6669 6775  evelop/docs/figu
+00000070: 7265 732f 4372 694d 652d 6261 6e6e 6572  res/CriMe-banner
+00000080: 2e70 6e67 290a 5b21 5b4c 696e 7578 5d28  .png).[![Linux](
+00000090: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000000a0: 6c64 732e 696f 2f62 6164 6765 2f6f 732d  lds.io/badge/os-
+000000b0: 6c69 6e75 783f 266c 6f67 6f3d 4c69 6e75  linux?&logo=Linu
+000000c0: 7826 6c6f 676f 436f 6c6f 723d 7768 6974  x&logoColor=whit
+000000d0: 6526 6c61 6265 6c43 6f6c 6f72 3d67 7261  e&labelColor=gra
+000000e0: 7929 5d28 6874 7470 733a 2f2f 7079 7069  y)](https://pypi
+000000f0: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
+00000100: 2f63 6f6d 6d6f 6e72 6f61 642d 6f70 656e  /commonroad-open
+00000110: 7363 656e 6172 696f 2d63 6f6e 7665 7274  scenario-convert
+00000120: 6572 2f29 0a5b 215b 5079 5049 2076 6572  er/).[![PyPI ver
+00000130: 7369 6f6e 2066 7572 792e 696f 5d28 6874  sion fury.io](ht
+00000140: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
+00000150: 2e69 6f2f 7079 2f63 6f6d 6d6f 6e72 6f61  .io/py/commonroa
+00000160: 642d 6372 696d 652e 7376 673f 7374 796c  d-crime.svg?styl
+00000170: 653d 706c 6173 7469 6329 5d28 6874 7470  e=plastic)](http
+00000180: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
+00000190: 6f72 672f 7079 7069 2f63 6f6d 6d6f 6e72  org/pypi/commonr
+000001a0: 6f61 642d 6372 696d 652f 290a 5b21 5b50  oad-crime/).[![P
+000001b0: 7950 4920 6c69 6365 6e73 655d 2868 7474  yPI license](htt
+000001c0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000001d0: 2e69 6f2f 7079 7069 2f6c 2f63 6f6d 6d6f  .io/pypi/l/commo
+000001e0: 6e72 6f61 642d 6372 696d 652e 7376 673f  nroad-crime.svg?
+000001f0: 7374 796c 653d 706c 6173 7469 6329 5d28  style=plastic)](
+00000200: 6874 7470 733a 2f2f 7079 7069 2e70 7974  https://pypi.pyt
+00000210: 686f 6e2e 6f72 672f 7079 7069 2f63 6f6d  hon.org/pypi/com
+00000220: 6d6f 6e72 6f61 642d 6372 696d 652f 293c  monroad-crime/)<
+00000230: 6272 3e0a 5b21 5b50 7950 4920 646f 776e  br>.[![PyPI down
+00000240: 6c6f 6164 206d 6f6e 7468 5d28 6874 7470  load month](http
+00000250: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000260: 696f 2f70 7970 692f 646d 2f63 6f6d 6d6f  io/pypi/dm/commo
+00000270: 6e72 6f61 642d 6372 696d 652e 7376 673f  nroad-crime.svg?
+00000280: 7374 796c 653d 706c 6173 7469 6326 6c61  style=plastic&la
+00000290: 6265 6c3d 5079 5049 2532 3064 6f77 6e6c  bel=PyPI%20downl
+000002a0: 6f61 6473 295d 2868 7474 7073 3a2f 2f70  oads)](https://p
+000002b0: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
+000002c0: 7970 692f 636f 6d6d 6f6e 726f 6164 2d63  ypi/commonroad-c
+000002d0: 7269 6d65 2f29 200a 5b21 5b50 7950 4920  rime/) .[![PyPI 
+000002e0: 646f 776e 6c6f 6164 2077 6565 6b5d 2868  download week](h
+000002f0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000300: 6473 2e69 6f2f 7079 7069 2f64 772f 636f  ds.io/pypi/dw/co
+00000310: 6d6d 6f6e 726f 6164 2d63 7269 6d65 2e73  mmonroad-crime.s
+00000320: 7667 3f73 7479 6c65 3d70 6c61 7374 6963  vg?style=plastic
+00000330: 266c 6162 656c 3d50 7950 4925 3230 646f  &label=PyPI%20do
+00000340: 776e 6c6f 6164 7329 5d28 6874 7470 733a  wnloads)](https:
+00000350: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
+00000360: 672f 7079 7069 2f63 6f6d 6d6f 6e72 6f61  g/pypi/commonroa
+00000370: 642d 6372 696d 652f 293c 6272 3e0a 0a54  d-crime/)<br>..T
+00000380: 6f6f 6c62 6f78 2074 6f20 636f 6d70 7574  oolbox to comput
+00000390: 6520 2a2a 4372 692a 2a74 6963 616c 6974  e **Cri**ticalit
+000003a0: 7920 2a2a 4d65 2a2a 6173 7572 6573 200a  y **Me**asures .
+000003b0: 2865 2e67 2e20 7469 6d65 2d74 6f2d 636f  (e.g. time-to-co
+000003c0: 6c6c 6973 696f 6e2c 2074 696d 652d 746f  llision, time-to
+000003d0: 2d72 6561 6374 2c2e 2e2e 292e 2053 7563  -react,...). Suc
+000003e0: 6820 6d65 6173 7572 6573 0a63 616e 2062  h measures.can b
+000003f0: 6520 7573 6564 2074 6f20 7472 6967 6765  e used to trigge
+00000400: 7220 7761 726e 696e 6773 2061 6e64 2065  r warnings and e
+00000410: 6d65 7267 656e 6379 206d 616e 6575 7665  mergency maneuve
+00000420: 7273 200a 696e 2064 7269 7665 7220 6173  rs .in driver as
+00000430: 7369 7374 616e 6365 2073 7973 7465 6d73  sistance systems
+00000440: 206f 7220 7265 7061 6972 2061 6e20 696e   or repair an in
+00000450: 6665 6173 6962 6c65 200a 7472 616a 6563  feasible .trajec
+00000460: 746f 7279 2e20 4966 2079 6f75 2068 6176  tory. If you hav
+00000470: 6520 7175 6573 7469 6f6e 7320 6f72 2077  e questions or w
+00000480: 616e 7420 746f 2072 6570 6f72 7420 7072  ant to report pr
+00000490: 6f62 6c65 6d73 206f 7220 7375 6767 6573  oblems or sugges
+000004a0: 7469 6f6e 732c 2070 6c65 6173 6520 7374  tions, please st
+000004b0: 6172 7420 6120 5b47 6974 6875 6220 6469  art a [Github di
+000004c0: 7363 7573 7369 6f6e 5d28 6874 7470 733a  scussion](https:
+000004d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 7267  //github.com/org
+000004e0: 732f 436f 6d6d 6f6e 526f 6164 2f64 6973  s/CommonRoad/dis
+000004f0: 6375 7373 696f 6e73 2920 2f0a 5b47 6974  cussions) /.[Git
+00000500: 6875 6220 6973 7375 655d 2868 7474 7073  hub issue](https
+00000510: 3a2f 2f67 6974 6875 622e 636f 6d2f 436f  ://github.com/Co
+00000520: 6d6d 6f6e 526f 6164 2f63 6f6d 6d6f 6e72  mmonRoad/commonr
+00000530: 6f61 642d 6372 696d 652f 6973 7375 6573  oad-crime/issues
+00000540: 2f29 2e20 0a0a 3c61 2068 7265 663d 2268  /). ..<a href="h
+00000550: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
+00000560: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
+00000570: 2f64 7269 7665 2f31 5437 4d62 5356 7155  /drive/1T7MbSVqU
+00000580: 3558 4344 5a67 5054 4445 524b 4e4b 5946  5XCDZgPTDERKNKYF
+00000590: 6241 496e 5852 6a79 223e 0a20 203c 696d  bAInXRjy">.  <im
+000005a0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+000005b0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
+000005c0: 7465 6e74 2e63 6f6d 2f43 6f6d 6d6f 6e52  tent.com/CommonR
+000005d0: 6f61 642f 636f 6d6d 6f6e 726f 6164 2d63  oad/commonroad-c
+000005e0: 7269 6d65 2f64 6576 656c 6f70 2f64 6f63  rime/develop/doc
+000005f0: 732f 6669 6775 7265 732f 6c69 7665 5f64  s/figures/live_d
+00000600: 656d 6f2e 706e 6722 2061 6c74 3d22 4c69  emo.png" alt="Li
+00000610: 7665 2044 656d 6f22 3e0a 3c2f 613e 0a0a  ve Demo">.</a>..
+00000620: 2323 20f0 9f9a 8020 496e 7374 616c 6c61  ## .... Installa
+00000630: 7469 6f6e 2047 7569 6465 0a0a 6063 6f6d  tion Guide..`com
+00000640: 6d6f 6e72 6f61 642d 6372 696d 6560 2063  monroad-crime` c
+00000650: 616e 2062 6520 696e 7374 616c 6c65 6420  an be installed 
+00000660: 7769 7468 3a0a 0a60 6060 2062 6173 680a  with:..``` bash.
+00000670: 2420 7069 7020 696e 7374 616c 6c20 636f  $ pip install co
+00000680: 6d6d 6f6e 726f 6164 2d63 7269 6d65 0a60  mmonroad-crime.`
+00000690: 6060 0a3c 6465 7461 696c 733e 0a3c 7375  ``.<details>.<su
+000006a0: 6d6d 6172 793e 3c62 3e44 6576 656c 6f70  mmary><b>Develop
+000006b0: 2043 7269 4d65 206c 6f63 616c 6c79 3c2f   CriMe locally</
+000006c0: 623e 3c2f 7375 6d6d 6172 793e 0a0a 466f  b></summary>..Fo
+000006d0: 7220 6164 6469 6e67 206e 6577 206d 6561  r adding new mea
+000006e0: 7375 7265 732c 2077 6520 7265 636f 6d6d  sures, we recomm
+000006f0: 656e 6420 7573 696e 6720 5b41 6e61 636f  end using [Anaco
+00000700: 6e64 615d 2868 7474 7073 3a2f 2f77 7777  nda](https://www
+00000710: 2e61 6e61 636f 6e64 612e 636f 6d2f 2920  .anaconda.com/) 
+00000720: 746f 206d 616e 6167 6520 796f 7572 2065  to manage your e
+00000730: 6e76 6972 6f6e 6d65 6e74 2073 6f20 7468  nvironment so th
+00000740: 6174 2065 7665 6e20 6966 2079 6f75 206d  at even if you m
+00000750: 6573 7320 736f 6d65 7468 696e 6720 7570  ess something up
+00000760: 2c20 796f 7520 6361 6e20 616c 7761 7973  , you can always
+00000770: 2068 6176 6520 6120 7361 6665 2061 6e64   have a safe and
+00000780: 2063 6c65 616e 2072 6573 7461 7274 2e20   clean restart. 
+00000790: 4120 6775 6964 6520 666f 7220 6d61 6e61  A guide for mana
+000007a0: 6769 6e67 2070 7974 686f 6e20 656e 7669  ging python envi
+000007b0: 726f 6e6d 656e 7473 2077 6974 6820 416e  ronments with An
+000007c0: 6163 6f6e 6461 2063 616e 2062 6520 666f  aconda can be fo
+000007d0: 756e 6420 5b68 6572 655d 2868 7474 7073  und [here](https
+000007e0: 3a2f 2f63 6f6e 6461 2e69 6f2f 7072 6f6a  ://conda.io/proj
+000007f0: 6563 7473 2f63 6f6e 6461 2f65 6e2f 6c61  ects/conda/en/la
+00000800: 7465 7374 2f75 7365 722d 6775 6964 652f  test/user-guide/
+00000810: 7461 736b 732f 6d61 6e61 6765 2d65 6e76  tasks/manage-env
+00000820: 6972 6f6e 6d65 6e74 732e 6874 6d6c 292e  ironments.html).
+00000830: 0a0a 4166 7465 7220 696e 7374 616c 6c69  ..After installi
+00000840: 6e67 2041 6e61 636f 6e64 612c 2063 7265  ng Anaconda, cre
+00000850: 6174 6520 6120 6e65 7720 656e 7669 726f  ate a new enviro
+00000860: 6e6d 656e 7420 7769 7468 3a0a 6060 6020  nment with:.``` 
+00000870: 6261 7368 0a24 2063 6f6e 6461 2063 7265  bash.$ conda cre
+00000880: 6174 6520 2d6e 2063 6f6d 6d6f 6e72 6f61  ate -n commonroa
+00000890: 642d 7079 3338 2070 7974 686f 6e3d 332e  d-py38 python=3.
+000008a0: 3820 2d79 0a60 6060 0a0a 4865 7265 2074  8 -y.```..Here t
+000008b0: 6865 206e 616d 6520 6f66 2074 6865 2065  he name of the e
+000008c0: 6e76 6972 6f6e 6d65 6e74 2069 7320 6361  nvironment is ca
+000008d0: 6c6c 6564 202a 2a63 6f6d 6d6f 6e72 6f61  lled **commonroa
+000008e0: 642d 7079 3338 2a2a 2e20 596f 7520 6d61  d-py38**. You ma
+000008f0: 7920 616c 736f 2063 6861 6e67 6520 7468  y also change th
+00000900: 6973 206e 616d 6520 6173 2079 6f75 2077  is name as you w
+00000910: 6973 682e 2049 6e20 7375 6368 2063 6173  ish. In such cas
+00000920: 652c 2064 6f6e 2774 2066 6f72 6765 7420  e, don't forget 
+00000930: 746f 2063 6861 6e67 6520 6974 2069 6e20  to change it in 
+00000940: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
+00000950: 6d6d 616e 6473 2061 7320 7765 6c6c 2e20  mmands as well. 
+00000960: 2a2a 416c 7761 7973 2061 6374 6976 6174  **Always activat
+00000970: 652a 2a20 7468 6973 2065 6e76 6972 6f6e  e** this environ
+00000980: 6d65 6e74 2062 6566 6f72 6520 796f 7520  ment before you 
+00000990: 646f 2061 6e79 7468 696e 6720 7265 6c61  do anything rela
+000009a0: 7465 643a 0a0a 6060 6073 680a 2420 636f  ted:..```sh.$ co
+000009b0: 6e64 6120 6163 7469 7661 7465 2063 6f6d  nda activate com
+000009c0: 6d6f 6e72 6f61 642d 7079 3338 0a6f 720a  monroad-py38.or.
+000009d0: 2420 736f 7572 6365 2061 6374 6976 6174  $ source activat
+000009e0: 6520 636f 6d6d 6f6e 726f 6164 2d70 7933  e commonroad-py3
+000009f0: 380a 6060 600a 5468 656e 2c20 696e 7374  8.```.Then, inst
+00000a00: 616c 6c20 7468 6520 6465 7065 6e64 656e  all the dependen
+00000a10: 6369 6573 2077 6974 683a 0a0a 6060 6073  cies with:..```s
+00000a20: 680a 2420 6364 203c 7061 7468 2d74 6f2d  h.$ cd <path-to-
+00000a30: 7468 6973 2d72 6570 6f3e 0a24 2070 6970  this-repo>.$ pip
+00000a40: 2069 6e73 7461 6c6c 202d 6520 2e0a 2420   install -e ..$ 
+00000a50: 636f 6e64 6120 6465 7665 6c6f 7020 2e0a  conda develop ..
+00000a60: 6060 600a 0a54 6f20 7465 7374 2074 6865  ```..To test the
+00000a70: 2069 6e73 7461 6c6c 6974 696f 6e2c 2072   installition, r
+00000a80: 756e 2075 6e69 7474 6573 743a 0a60 6060  un unittest:.```
+00000a90: 6261 7368 0a24 2063 6420 7465 7374 730a  bash.$ cd tests.
+00000aa0: 2420 7079 7468 6f6e 202d 6d20 756e 6974  $ python -m unit
+00000ab0: 7465 7374 202d 760a 6060 600a 0a3c 2f64  test -v.```..</d
+00000ac0: 6574 6169 6c73 3e0a 0a54 6f20 6765 7420  etails>..To get 
+00000ad0: 7374 6172 7465 6420 796f 7572 206a 6f75  started your jou
+00000ae0: 726e 6579 2077 6974 6820 6f75 7220 6372  rney with our cr
+00000af0: 6974 6963 616c 6974 7920 6d65 6173 7572  iticality measur
+00000b00: 6573 2c20 6368 6563 6b20 7468 6520 6074  es, check the `t
+00000b10: 7574 6f72 6961 6c73 6020 616e 6420 7468  utorials` and th
+00000b20: 6520 666f 6c6c 6f77 696e 6720 7469 7073  e following tips
+00000b30: 2e0a 0a3c 6465 7461 696c 733e 0a3c 7375  ...<details>.<su
+00000b40: 6d6d 6172 793e 3c62 3e41 6464 206e 6577  mmary><b>Add new
+00000b50: 2063 7269 7469 6361 6c69 7479 206d 6561   criticality mea
+00000b60: 7375 7265 3c2f 623e 3c2f 7375 6d6d 6172  sure</b></summar
+00000b70: 793e 0a0a 312e 2063 7265 6174 6520 6120  y>..1. create a 
+00000b80: 6e65 7720 6272 616e 6368 2077 6974 6820  new branch with 
+00000b90: 6066 6561 7475 7265 2d3c 6d65 6173 7572  `feature-<measur
+00000ba0: 652d 6e61 6d65 3e60 2061 6e64 2063 6865  e-name>` and che
+00000bb0: 636b 6f75 7420 7468 6520 6272 616e 6368  ckout the branch
+00000bc0: 0a32 2e20 6e61 7669 6761 7465 2074 6f20  .2. navigate to 
+00000bd0: 6063 6f6d 6d6f 6e72 6f61 645f 6372 696d  `commonroad_crim
+00000be0: 652f 6461 7461 5f73 7472 7563 7475 7265  e/data_structure
+00000bf0: 2f74 7970 652e 7079 6020 746f 2066 696e  /type.py` to fin
+00000c00: 6420 7468 6520 636f 7272 6563 7420 6361  d the correct ca
+00000c10: 7465 676f 7279 206f 6620 7468 6520 6d65  tegory of the me
+00000c20: 6173 7572 6520 616e 6420 6164 6420 616e  asure and add an
+00000c30: 200a 656e 756d 6572 6174 696f 6e20 656e   .enumeration en
+00000c40: 7472 7920 603c 6162 6272 6576 6961 7469  try `<abbreviati
+00000c50: 6f6e 3e3a 203c 6578 706c 616e 6174 696f  on>: <explanatio
+00000c60: 6e3e 600a 332e 206e 6176 6967 6174 6520  n>`.3. navigate 
+00000c70: 746f 2060 636f 6d6d 6f6e 726f 6164 5f63  to `commonroad_c
+00000c80: 7269 6d65 2f6d 6561 7375 7265 6020 746f  rime/measure` to
+00000c90: 2066 696e 6420 7468 6520 6162 6f76 652d   find the above-
+00000ca0: 6d65 6e74 696f 6e65 6420 6361 7465 676f  mentioned catego
+00000cb0: 7279 2061 6e64 2063 7265 6174 6520 6120  ry and create a 
+00000cc0: 7079 7468 6f6e 2066 696c 6520 6e61 6d65  python file name
+00000cd0: 640a 603c 6162 6272 6576 6961 7469 6f6e  d.`<abbreviation
+00000ce0: 3e2e 7079 602e 2054 6865 6e20 6372 6561  >.py`. Then crea
+00000cf0: 7465 2061 2063 6c61 7373 2069 6e68 6572  te a class inher
+00000d00: 6974 696e 6720 7468 6520 6043 7269 4d65  iting the `CriMe
+00000d10: 4261 7365 6020 756e 6465 7220 6063 6f6d  Base` under `com
+00000d20: 6d6f 6e72 6f61 645f 6372 696d 652f 6461  monroad_crime/da
+00000d30: 7461 5f73 7472 7563 7475 7265 2f62 6173  ta_structure/bas
+00000d40: 652e 7079 600a 342e 2073 696d 696c 6172  e.py`.4. similar
+00000d50: 2074 6f20 6f74 6865 7220 6d65 6173 7572   to other measur
+00000d60: 6573 2c20 796f 7520 6e65 6564 2074 6f20  es, you need to 
+00000d70: 696d 706c 656d 656e 7420 7468 6520 6063  implement the `c
+00000d80: 6f6d 7075 7465 2829 6020 616e 6420 6076  ompute()` and `v
+00000d90: 6973 7561 6c69 7a65 2829 6020 6675 6e63  isualize()` func
+00000da0: 7469 6f6e 730a 0a3c 2f64 6574 6169 6c73  tions..</details
+00000db0: 3e0a 0a3c 6465 7461 696c 733e 0a3c 7375  >..<details>.<su
+00000dc0: 6d6d 6172 793e 3c62 3e44 6566 696e 6520  mmary><b>Define 
+00000dd0: 636f 6e66 6967 7572 6174 696f 6e20 7061  configuration pa
+00000de0: 7261 6d65 7465 7273 206f 6620 7468 6520  rameters of the 
+00000df0: 6d65 6173 7572 653c 2f62 3e3c 2f73 756d  measure</b></sum
+00000e00: 6d61 7279 3e0a 0a31 2e20 6e61 7669 6761  mary>..1. naviga
+00000e10: 7465 2074 6f20 6063 6f6d 6d6f 6e72 6f61  te to `commonroa
+00000e20: 645f 6372 696d 652f 6461 7461 5f73 7472  d_crime/data_str
+00000e30: 7563 7475 7265 2f63 6f6e 6669 6775 6174  ucture/configuat
+00000e40: 696f 6e2e 7079 6020 746f 2066 696e 6420  ion.py` to find 
+00000e50: 7468 6520 6162 6f76 652d 6d65 6e74 696f  the above-mentio
+00000e60: 6e65 6420 6361 7465 676f 7279 2061 6e64  ned category and
+00000e70: 2061 6464 2061 206e 6577 200a 696e 7374   add a new .inst
+00000e80: 616e 6365 2074 6f20 7468 6520 636c 6173  ance to the clas
+00000e90: 7320 6173 2060 7365 6c66 2e3c 7061 7261  s as `self.<para
+00000ea0: 6d65 7465 723e 203d 2063 6f6e 6669 675f  meter> = config_
+00000eb0: 7265 6c65 7661 6e74 2e3c 7061 7261 6d65  relevant.<parame
+00000ec0: 7465 723e 600a 322e 2079 6f75 2063 616e  ter>`.2. you can
+00000ed0: 2074 6865 6e20 6469 7265 6374 6c79 2063   then directly c
+00000ee0: 616c 6c20 7468 6520 7661 6c75 6573 2075  all the values u
+00000ef0: 7369 6e67 2060 7365 6c66 2e63 6f6e 6669  sing `self.confi
+00000f00: 6775 7261 7469 6f6e 2e3c 6361 7465 676f  guration.<catego
+00000f10: 7279 3e2e 3c70 6172 616d 6574 6572 3e60  ry>.<parameter>`
+00000f20: 2069 6e20 796f 7572 206d 6561 7375 7265   in your measure
+00000f30: 2063 6c61 7373 0a33 2e20 746f 206f 7665   class.3. to ove
+00000f40: 7272 6964 6520 7468 6520 6465 6661 756c  rride the defaul
+00000f50: 7420 7061 7261 6d65 7465 7220 7661 6c75  t parameter valu
+00000f60: 6573 2c20 6372 6561 7465 2061 2060 7961  es, create a `ya
+00000f70: 6d6c 6020 6669 6c65 2028 6e61 6d65 2069  ml` file (name i
+00000f80: 7420 7468 6520 7361 6d65 2061 7320 7468  t the same as th
+00000f90: 6520 7363 656e 6172 696f 2920 696e 2060  e scenario) in `
+00000fa0: 2e2f 636f 6e66 6967 5f66 696c 6573 6020  ./config_files` 
+00000fb0: 616e 6420 6d6f 6469 6679 2074 6865 2076  and modify the v
+00000fc0: 616c 7565 7320 7468 6572 650a 0a3c 2f64  alues there..</d
+00000fd0: 6574 6169 6c73 3e0a 0a23 2320 f09f 9aa7  etails>..## ....
+00000fe0: 2044 6f63 756d 656e 7461 7469 6f6e 0a0a   Documentation..
+00000ff0: 5468 6520 646f 6375 6d65 6e74 6174 696f  The documentatio
+00001000: 6e20 6f66 206f 7572 2074 6f6f 6c62 6f78  n of our toolbox
+00001010: 2069 7320 6176 6169 6c61 626c 6520 6f6e   is available on
+00001020: 206f 7572 2077 6562 7369 7465 3a20 6874   our website: ht
+00001030: 7470 733a 2f2f 6370 732e 7061 6765 732e  tps://cps.pages.
+00001040: 6769 746c 6162 2e6c 727a 2e64 652f 636f  gitlab.lrz.de/co
+00001050: 6d6d 6f6e 726f 6164 2f63 6f6d 6d6f 6e72  mmonroad/commonr
+00001060: 6f61 642d 6372 6974 6963 616c 6974 792d  oad-criticality-
+00001070: 6d65 6173 7572 6573 2f2e 0a3c 6465 7461  measures/..<deta
+00001080: 696c 733e 0a3c 7375 6d6d 6172 793e 3c62  ils>.<summary><b
+00001090: 3e42 7569 6c64 2064 6f63 756d 656e 7461  >Build documenta
+000010a0: 7469 6f6e 206c 6f63 616c 6c79 3c2f 623e  tion locally</b>
+000010b0: 3c2f 7375 6d6d 6172 793e 0a49 6e20 6f72  </summary>.In or
+000010c0: 6465 7220 746f 2067 656e 6572 6174 6520  der to generate 
+000010d0: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
+000010e0: 6e20 7669 6120 5370 6869 6e78 206c 6f63  n via Sphinx loc
+000010f0: 616c 6c79 2c20 7275 6e20 7468 6520 666f  ally, run the fo
+00001100: 6c6c 6f77 696e 6720 636f 6d6d 616e 6473  llowing commands
+00001110: 2069 6e20 7468 6520 726f 6f74 2064 6972   in the root dir
+00001120: 6563 746f 7279 3a0a 0a60 6060 6261 7368  ectory:..```bash
+00001130: 0a24 2070 6970 2069 6e73 7461 6c6c 202d  .$ pip install -
+00001140: 7220 2e2f 646f 6373 2f72 6571 7569 7265  r ./docs/require
+00001150: 6d65 6e74 735f 646f 632e 7478 740a 2420  ments_doc.txt.$ 
+00001160: 6364 2064 6f63 732f 7370 6869 6e78 0a24  cd docs/sphinx.$
+00001170: 206d 616b 6520 6874 6d6c 0a60 6060 0a0a   make html.```..
+00001180: 5468 6520 646f 6375 6d65 6e74 6174 696f  The documentatio
+00001190: 6e20 6361 6e20 7468 656e 2062 6520 6c61  n can then be la
+000011a0: 756e 6368 6564 2062 7920 6272 6f77 7369  unched by browsi
+000011b0: 6e67 2060 602e 2f64 6f63 732f 7370 6869  ng ``./docs/sphi
+000011c0: 6e78 2f62 7569 6c64 2f68 746d 6c2f 696e  nx/build/html/in
+000011d0: 6465 782e 6874 6d6c 2f60 602e 0a3c 2f64  dex.html/``..</d
+000011e0: 6574 6169 6c73 3e0a 0a23 2320 f09f 8c9f  etails>..## ....
+000011f0: 2043 6f6e 7472 6962 7574 6f72 7320 2869   Contributors (i
+00001200: 6e20 616c 7068 6162 6574 6963 616c 206f  n alphabetical o
+00001210: 7264 6572 2062 7920 6c61 7374 206e 616d  rder by last nam
+00001220: 6529 0a0a 2d20 4c69 6775 6f20 4368 656e  e)..- Liguo Chen
+00001230: 0a2d 204d 6172 6975 7320 4572 6174 680a  .- Marius Erath.
+00001240: 2d20 5975 616e 6665 6920 4c69 6e0a 2d20  - Yuanfei Lin.- 
+00001250: 5365 6261 7374 6961 6e20 4d61 6965 7268  Sebastian Maierh
+00001260: 6f66 6572 0a2d 2049 7661 6e61 2050 656e  ofer.- Ivana Pen
+00001270: 6576 610a 2d20 4b75 6e20 5169 616e 0a2d  eva.- Kun Qian.-
+00001280: 204f 6c69 7665 7220 5370 6563 6874 0a2d   Oliver Specht.-
+00001290: 2053 6963 6865 6e67 2057 616e 670a 2d20   Sicheng Wang.- 
+000012a0: 596f 7572 616e 2057 616e 670a 2d20 5a65  Youran Wang.- Ze
+000012b0: 6b75 6e20 5869 6e67 0a2d 205a 6971 6961  kun Xing.- Ziqia
+000012c0: 6e20 5875 0a0a 2323 20f0 9f94 9620 4369  n Xu..## .... Ci
+000012d0: 7461 7469 6f6e 0a49 6620 796f 7520 7573  tation.If you us
+000012e0: 6520 6063 6f6d 6d6f 6e72 6f61 642d 6372  e `commonroad-cr
+000012f0: 696d 6560 2066 6f72 2061 6361 6465 6d69  ime` for academi
+00001300: 6320 776f 726b 2c20 7765 2068 6967 686c  c work, we highl
+00001310: 7920 656e 636f 7572 6167 6520 796f 7520  y encourage you 
+00001320: 746f 2063 6974 6520 6f75 7220 7061 7065  to cite our pape
+00001330: 723a 0a60 6060 7465 7874 0a40 496e 5072  r:.```text.@InPr
+00001340: 6f63 6565 6469 6e67 737b 6c69 6e32 3032  oceedings{lin202
+00001350: 3363 7269 6d65 2c0a 2020 2020 2020 7469  3crime,.      ti
+00001360: 746c 6520 2020 2020 3d20 7b7b 436f 6d6d  tle     = {{Comm
+00001370: 6f6e 526f 6164 2d43 7269 4d65 7d3a 207b  onRoad-CriMe}: {
+00001380: 417d 2054 6f6f 6c62 6f78 2066 6f72 2043  A} Toolbox for C
+00001390: 7269 7469 6361 6c69 7479 204d 6561 7375  riticality Measu
+000013a0: 7265 7320 6f66 2041 7574 6f6e 6f6d 6f75  res of Autonomou
+000013b0: 7320 5665 6869 636c 6573 7d2c 0a20 2020  s Vehicles},.   
+000013c0: 2020 2061 7574 686f 7220 2020 203d 207b     author    = {
+000013d0: 5975 616e 6665 6920 4c69 6e20 616e 6420  Yuanfei Lin and 
+000013e0: 4d61 7474 6869 6173 2041 6c74 686f 6666  Matthias Althoff
+000013f0: 7d2c 0a20 2020 2020 2062 6f6f 6b74 6974  },.      booktit
+00001400: 6c65 203d 207b 5072 6f63 2e20 6f66 2074  le = {Proc. of t
+00001410: 6865 2049 4545 4520 496e 7465 6c6c 2e20  he IEEE Intell. 
+00001420: 5665 682e 2053 796d 702e 7d2c 2020 2020  Veh. Symp.},    
+00001430: 200a 2020 2020 2020 7061 6765 7320 2020   .      pages   
+00001440: 2020 3d20 7b31 2d38 7d2c 200a 2020 2020    = {1-8}, .    
+00001450: 2020 7965 6172 2020 2020 2020 3d20 7b32    year      = {2
+00001460: 3032 337d 2c0a 7d0a 6060 600a 4966 2079  023},.}.```.If y
+00001470: 6f75 2075 7365 2074 6869 7320 7072 6f6a  ou use this proj
+00001480: 6563 7427 7320 636f 6465 2069 6e20 696e  ect's code in in
+00001490: 6475 7374 7279 2c20 7765 2764 206c 6f76  dustry, we'd lov
+000014a0: 6520 746f 2068 6561 7220 6672 6f6d 2079  e to hear from y
+000014b0: 6f75 2061 7320 7765 6c6c 3b20 0a66 6565  ou as well; .fee
+000014c0: 6c20 6672 6565 2074 6f20 7265 6163 6820  l free to reach 
+000014d0: 6f75 7420 746f 205b 5975 616e 6665 6920  out to [Yuanfei 
+000014e0: 4c69 6e5d 286d 6169 6c74 6f3a 7975 616e  Lin](mailto:yuan
+000014f0: 6665 692e 6c69 6e40 7475 6d2e 6465 2920  fei.lin@tum.de) 
+00001500: 6469 7265 6374 6c79 2e0a                 directly..
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/data_structure/base.py` & `commonroad_crime-0.4.0/commonroad_crime/data_structure/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import time
 from enum import Enum
 from abc import abstractmethod
 import copy
 import logging
 from typing import Union
 
+import numpy as np
+
 # CommonRoad packages
 from commonroad.scenario.obstacle import Obstacle, DynamicObstacle, StaticObstacle
 from commonroad.prediction.prediction import TrajectoryPrediction
 from commonroad.visualization.mp_renderer import MPRenderer
 from commonroad.prediction.prediction import SetBasedPrediction
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
@@ -77,15 +79,16 @@
         )
         if not isinstance(self.ego_vehicle, StaticObstacle) and not isinstance(
             self.ego_vehicle.prediction, SetBasedPrediction
         ):
             utils_gen.check_elements_state_list(
                 [self.ego_vehicle.initial_state]
                 + self.ego_vehicle.prediction.trajectory.states_in_time_interval(
-                    time_begin=1, time_end=self.ego_vehicle.prediction.final_time_step
+                    time_begin=self.ego_vehicle.initial_state.time_step + 1,
+                    time_end=self.ego_vehicle.prediction.final_time_step,
                 ),
                 self.dt,
             )
             self._update_clcs()
         self.other_vehicle: Union[Obstacle, DynamicObstacle, StaticObstacle, None] = (
             None  # optional
         )
@@ -119,15 +122,17 @@
     def _update_clcs(self):
         """
         Updates the curvilinear coordinate system in the configuration setting using the reference path from the lanelet
         where the ego vehicle is currently located to the end of the lanelet.
         """
         # default setting of ego vehicle's curvilinear coordinate system
         ego_initial_lanelet_id = list(
-            self.ego_vehicle.prediction.center_lanelet_assignment[0]
+            self.ego_vehicle.prediction.center_lanelet_assignment[
+                self.ego_vehicle.initial_state.time_step
+            ]
         )[0]
         reference_path = utils_gen.generate_reference_path(
             ego_initial_lanelet_id, self.sce.lanelet_network
         )
         clcs = CurvilinearCoordinateSystem(reference_path)
         self.configuration.update(CLCS=clcs)
 
@@ -143,17 +148,55 @@
         if plot_limit is None:
             plot_limit = self.configuration.debug.plot_limits
         self.rnd = MPRenderer(figsize=figsize, plot_limits=plot_limit)
         utils_vis.draw_sce_at_time_step(
             self.rnd, self.configuration, self.sce, self.time_step
         )
 
+    def validate_update_states_log(
+        self, vehicle_id: int = None, time_step: int = 0, verbose: bool = True
+    ) -> bool:
+        """
+        Validates the presence of vehicle states at a given time step and updates internal states accordingly.
+
+        This function checks if both the ego vehicle and another specified vehicle have valid states at the specified
+        time step. It updates the internal time step and other vehicle states if valid. It logs the process and any
+        warnings encountered.
+        """
+        if time_step is not None:
+            if not self.ego_vehicle.state_at_time(time_step):
+                utils_log.print_and_log_warning(
+                    logger,
+                    f"<{self.measure_name}>:"
+                    f" The ego vehicle does NOT have the state at time step {time_step}",
+                    verbose,
+                )
+                return False
+            self.time_step = time_step
+
+        if vehicle_id is not None:
+            self.set_other_vehicles(vehicle_id)
+            if not self.other_vehicle.state_at_time(self.time_step):
+                utils_log.print_and_log_warning(
+                    logger,
+                    f"* <{self.measure_name}>:"
+                    f" The vehicle {self.other_vehicle.obstacle_id} does NOT have the state at time step {time_step}",
+                    verbose,
+                )
+                return False
+        utils_log.print_and_log_info(
+            logger,
+            f"* Computing the {self.measure_name} at time step {time_step}",
+            verbose,
+        )
+        return True
+
     def set_other_vehicles(self, vehicle_id: int):
         """
-        Sets up the id for other measure-related vehicle.
+        Sets up the id for other measure-related vehicles.
         """
         # if already being set, do not have to reset again
         if self.other_vehicle:
             if vehicle_id == self.other_vehicle.obstacle_id:
                 return
 
         if not self.sce.obstacle_by_id(vehicle_id):
@@ -205,26 +248,35 @@
 
     def compute_criticality(
         self, time_step: int, vehicle_id: Union[int, None] = None, verbose: bool = True
     ):
         """
         Wrapper for computing the criticality, i.e., the value of the measure.
         """
+        if self.ego_vehicle.state_at_time(time_step) is None:
+            utils_log.print_and_log_warning(
+                logger,
+                f"* The ego vehicle doesn't have state at time step {time_step}",
+            )
+            return np.nan
+
         utils_log.print_and_log_info(
             logger, "*********************************", verbose
         )
 
         self.time_step = time_step
+
         if vehicle_id:
             other_veh_ids = [vehicle_id]
         else:
             other_veh_ids = [
                 veh.obstacle_id
                 for veh in self.sce.obstacles
                 if veh.obstacle_id is not self.ego_vehicle.obstacle_id
+                and veh.state_at_time(self.time_step) is not None
             ]
 
         time_start = time.time()
         criti_list = []
         if self.measure_name in [
             TypeTime.TTR,
             TypeTime.TTM,
@@ -238,20 +290,28 @@
             criti = self.compute(time_step=time_step, vehicle_id=None, verbose=verbose)
         else:
             for v_id in other_veh_ids:
                 criti_list.append(
                     self.compute(time_step=time_step, vehicle_id=v_id, verbose=verbose)
                 )
             if len([c for c in criti_list if c is not None]) > 0:
+                if np.all(np.isnan(criti_list)):
+                    utils_log.print_and_log_warning(
+                        logger,
+                        f"* Due to the missing entries, all elements are NaN, "
+                        f"the result for time step {time_step} is NaN",
+                    )
+                    return np.nan
+                # Not all elements are NaN, return the max/min of the non-NaN values
                 if self.monotone == TypeMonotone.POS:
-                    criti = max(criti_list)
+                    criti = np.nanmax(criti_list)
                 else:
-                    criti = min(criti_list)
+                    criti = np.nanmin(criti_list)
             else:
-                criti = None
+                return None
         time_computation = time.time() - time_start
         utils_log.print_and_log_info(
             logger, f"*\t\t {self.measure_name} of the scenario: {criti}", verbose
         )
         utils_log.print_and_log_info(
             logger, f"\tTook: \t{time_computation:.3f}s", verbose
         )
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/data_structure/configuration.py` & `commonroad_crime-0.4.0/commonroad_crime/data_structure/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
 
 
 @dataclass
 class DebugConfiguration(BaseConfig):
     save_plots: bool = True
     plot_limits: Union[List[float], None] = None
     # visualization settings
-    draw_visualization: bool = True
+    draw_visualization: bool = False
     # visualize dynamic obstacles with icons
     draw_icons: bool = True
 
 
 @dataclass
 class CriMeConfiguration(BaseConfig):
     """Class to hold criticality-measures-related configurations"""
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/data_structure/scene.py` & `commonroad_crime-0.4.0/commonroad_crime/data_structure/scene.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/data_structure/type.py` & `commonroad_crime-0.4.0/commonroad_crime/data_structure/type.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/__init__.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/acceleration/a_lat_req.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/a_lat_req.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
 import logging
+import numpy as np
 
 from commonroad.geometry.shape import Circle
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.type import TypeAcceleration, TypeMonotone
 from commonroad_crime.measure.time.ttc import TTC
@@ -70,68 +71,77 @@
                 + sign * (other_width + self.ego_vehicle.obstacle_shape.width / 2)
                 - v_rel_lat * ttc
             )
             / ttc**2
         )
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.set_other_vehicles(vehicle_id)
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
+
         if self._except_obstacle_in_same_lanelet(expected_value=0.0, verbose=verbose):
             # no negative acceleration is needed for avoiding a collision
             return self.value
+
         lanelet_id = self.sce.lanelet_network.find_lanelet_by_position(
             [self.ego_vehicle.state_at_time(time_step).position]
         )[0]
         # orientation of the ego vehicle and the other vehicle
         ego_orientation = utils_sol.compute_lanelet_width_orientation(
             self.sce.lanelet_network.find_lanelet_by_id(lanelet_id[0]),
             self.ego_vehicle.state_at_time(time_step).position,
         )[1]
-        other_orientation = utils_sol.compute_lanelet_width_orientation(
-            self.sce.lanelet_network.find_lanelet_by_id(lanelet_id[0]),
-            self.other_vehicle.state_at_time(time_step).position,
-        )[1]
-        ttc = self._ttc_object.compute(vehicle_id, time_step, verbose=verbose)
-        utils_log.print_and_log_info(logger, f"*\t\t TTC is equal to {ttc}", verbose)
-        if ttc == math.inf:
-            # no lateral acceleration is needed for avoiding a collision
+        try:
+            other_orientation = utils_sol.compute_lanelet_width_orientation(
+                self.sce.lanelet_network.find_lanelet_by_id(lanelet_id[0]),
+                self.other_vehicle.state_at_time(time_step).position,
+            )[1]
+        except ValueError as e:
+            utils_log.print_and_log_warning(
+                logger,
+                f"* <A_LAT_REQ> During the projection of the vehicle {self.other_vehicle.obstacle_id} "
+                f"at time step {self.time_step}: {e}",
+            )
+            # out of projection domain: the other vehicle is far away
             self.value = 0.0
-            return self.value
-        a_obj_lat = math.sqrt(
-            self.other_vehicle.state_at_time(time_step).acceleration_y ** 2
-            + self.other_vehicle.state_at_time(time_step).acceleration ** 2
-        ) * math.sin(other_orientation)
-
-        # compute the headway distance
-        d_rel_lat = utils_sol.compute_clcs_distance(
-            self.clcs,
-            self.ego_vehicle.state_at_time(time_step).position,
-            self.ego_vehicle.state_at_time(time_step).position,
-        )[1]
-        v_rel_lat = (
-            math.sqrt(
-                self.other_vehicle.state_at_time(time_step).velocity ** 2
-                + self.other_vehicle.state_at_time(time_step).velocity_y ** 2
+        else:
+            ttc = self._ttc_object.compute(vehicle_id, time_step, verbose=verbose)
+            utils_log.print_and_log_info(
+                logger, f"*\t\t TTC is equal to {ttc}", verbose
             )
-            * math.sin(other_orientation)
-            - math.sqrt(
-                self.ego_vehicle.state_at_time(time_step).velocity ** 2
-                + self.ego_vehicle.state_at_time(time_step).velocity_y ** 2
+            if ttc == math.inf:
+                # no lateral acceleration is needed for avoiding a collision
+                self.value = 0.0
+                return self.value
+            a_obj_lat = math.sqrt(
+                self.other_vehicle.state_at_time(time_step).acceleration_y ** 2
+                + self.other_vehicle.state_at_time(time_step).acceleration ** 2
+            ) * math.sin(other_orientation)
+
+            # compute the headway distance
+            d_rel_lat = utils_sol.compute_clcs_distance(
+                self.clcs,
+                self.ego_vehicle.state_at_time(time_step).position,
+                self.ego_vehicle.state_at_time(time_step).position,
+            )[1]
+            v_rel_lat = (
+                math.sqrt(
+                    self.other_vehicle.state_at_time(time_step).velocity ** 2
+                    + self.other_vehicle.state_at_time(time_step).velocity_y ** 2
+                )
+                * math.sin(other_orientation)
+                - math.sqrt(
+                    self.ego_vehicle.state_at_time(time_step).velocity ** 2
+                    + self.ego_vehicle.state_at_time(time_step).velocity_y ** 2
+                )
+            ) * math.sin(ego_orientation)
+            self.value = min(
+                abs(self._compute_a_lat(a_obj_lat, d_rel_lat, v_rel_lat, ttc, "left")),
+                abs(self._compute_a_lat(a_obj_lat, d_rel_lat, v_rel_lat, ttc, "right")),
             )
-        ) * math.sin(ego_orientation)
-        self.value = min(
-            abs(self._compute_a_lat(a_obj_lat, d_rel_lat, v_rel_lat, ttc, "left")),
-            abs(self._compute_a_lat(a_obj_lat, d_rel_lat, v_rel_lat, ttc, "right")),
-        )
         if self.value != math.inf:
             self.value = utils_gen.int_round(self.value, 2)
 
         utils_log.print_and_log_info(
             logger, f"*\t\t {self.measure_name} = {self.value}", verbose
         )
         return self.value
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/acceleration/a_long_req.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/a_long_req.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
+import numpy as np
 import logging
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.type import TypeAcceleration, TypeMonotone
 from commonroad_crime.measure.distance.hw import HW
 import commonroad_crime.utility.general as utils_gen
@@ -33,64 +34,72 @@
     monotone = TypeMonotone.NEG
 
     def __init__(self, config: CriMeConfiguration):
         super(ALongReq, self).__init__(config)
         self._hw_object = HW(config)
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.set_other_vehicles(vehicle_id)
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         if self._except_obstacle_in_same_lanelet(expected_value=0.0, verbose=verbose):
             # no negative acceleration is needed for avoiding a collision
+            utils_log.print_and_log_info(
+                logger, f"*\t\t {self.measure_name} = {self.value}", verbose
+            )
             return self.value
         lanelet_id = self.sce.lanelet_network.find_lanelet_by_position(
             [self.ego_vehicle.state_at_time(time_step).position]
         )[0]
         # orientation of the ego vehicle and the other vehicle
         ego_orientation = utils_sol.compute_lanelet_width_orientation(
             self.sce.lanelet_network.find_lanelet_by_id(lanelet_id[0]),
             self.ego_vehicle.state_at_time(time_step).position,
         )[1]
-        other_orientation = utils_sol.compute_lanelet_width_orientation(
-            self.sce.lanelet_network.find_lanelet_by_id(lanelet_id[0]),
-            self.other_vehicle.state_at_time(time_step).position,
-        )[1]
-        # acceleration of the other vehicle along the lanelet
-        a_obj = math.sqrt(
-            self.other_vehicle.state_at_time(time_step).acceleration ** 2
-            + self.other_vehicle.state_at_time(time_step).acceleration_y ** 2
-        ) * math.cos(other_orientation)
-        # compute the headway (relative distance) along the lanelet
-        x_rel = self._hw_object.compute(vehicle_id, time_step, verbose=verbose)
-        # compute the vehicles' velocity along the lanelet direction
-        v_ego_long = math.sqrt(
-            self.ego_vehicle.state_at_time(time_step).velocity ** 2
-            + self.ego_vehicle.state_at_time(time_step).velocity_y ** 2
-        ) * math.cos(ego_orientation)
-        v_other_long = math.sqrt(
-            self.other_vehicle.state_at_time(time_step).velocity ** 2
-            + self.other_vehicle.state_at_time(time_step).velocity_y ** 2
-        ) * math.cos(other_orientation)
-        if self.configuration.acceleration.acceleration_mode == 1:
-            # constant acceleration using (8) in "Using extreme value theory for vehicle level safety validation and
-            # implications for autonomous vehicles." is in correct
-            v_rel = v_other_long - v_ego_long
-            utils_log.print_and_log_info(
-                logger, f"*\t\t relative velocity is {v_rel}", verbose
+        try:
+            other_orientation = utils_sol.compute_lanelet_width_orientation(
+                self.sce.lanelet_network.find_lanelet_by_id(lanelet_id[0]),
+                self.other_vehicle.state_at_time(time_step).position,
+            )[1]
+        except ValueError as e:
+            utils_log.print_and_log_warning(
+                logger,
+                f"* <A_LONG_REQ> During the projection of the vehicle {self.other_vehicle.obstacle_id} "
+                f"at time step {self.time_step}: {e}",
             )
-            a_req = min(a_obj - v_rel**2 / (2 * x_rel), 0.0)
+            # out of projection domain: the other vehicle is far away
+            a_req = 0.0
         else:
-            # piecewise constant motion using (5.39) in "Collision Avoidance Theory with Application to Automotive
-            # Collision Mitigation"
-            a_req = -(v_ego_long**2) / (2 * (x_rel - v_other_long**2 / 2 * a_obj))
+            # acceleration of the other vehicle along the lanelet
+            a_obj = math.sqrt(
+                self.other_vehicle.state_at_time(time_step).acceleration ** 2
+                + self.other_vehicle.state_at_time(time_step).acceleration_y ** 2
+            ) * math.cos(other_orientation)
+            # compute the headway (relative distance) along the lanelet
+            x_rel = self._hw_object.compute(vehicle_id, time_step, verbose=verbose)
+            # compute the vehicles' velocity along the lanelet direction
+            v_ego_long = math.sqrt(
+                self.ego_vehicle.state_at_time(time_step).velocity ** 2
+                + self.ego_vehicle.state_at_time(time_step).velocity_y ** 2
+            ) * math.cos(ego_orientation)
+            v_other_long = math.sqrt(
+                self.other_vehicle.state_at_time(time_step).velocity ** 2
+                + self.other_vehicle.state_at_time(time_step).velocity_y ** 2
+            ) * math.cos(other_orientation)
+            if self.configuration.acceleration.acceleration_mode == 1:
+                # constant acceleration using (8) in "Using extreme value theory for vehicle level safety validation and
+                # implications for autonomous vehicles." is in correct
+                v_rel = v_other_long - v_ego_long
+                utils_log.print_and_log_info(
+                    logger, f"*\t\t relative velocity is {v_rel}", verbose
+                )
+                a_req = min(a_obj - v_rel**2 / (2 * x_rel), 0.0)
+            else:
+                # piecewise constant motion using (5.39) in "Collision Avoidance Theory with Application to Automotive
+                # Collision Mitigation"
+                a_req = -(v_ego_long**2) / (2 * (x_rel - v_other_long**2 / 2 * a_obj))
         if a_req > 0:  # the object is non-closing
             self.value = 0.0
         else:
             self.value = utils_gen.int_round(a_req, 2)
         utils_log.print_and_log_info(
             logger, f"*\t\t {self.measure_name} = {self.value}", verbose
         )
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/acceleration/a_req.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/a_req.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
 import logging
+import numpy as np
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.type import TypeAcceleration, TypeMonotone
 from commonroad_crime.measure.acceleration.a_lat_req import ALatReq
 from commonroad_crime.measure.acceleration.a_long_req import ALongReq
 import commonroad_crime.utility.general as utils_gen
@@ -33,21 +34,16 @@
 
     def __init__(self, config: CriMeConfiguration):
         super(AReq, self).__init__(config)
         self._a_long_object = ALongReq(config)
         self._a_lat_object = ALatReq(config)
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.set_other_vehicles(vehicle_id)
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         self.value = math.sqrt(
             self._a_long_object.compute(vehicle_id, time_step, verbose) ** 2
             + self._a_lat_object.compute(vehicle_id, time_step, verbose) ** 2
         )
         self.value = utils_gen.int_round(self.value, 2)
         utils_log.print_and_log_info(
             logger, f"*\t\t {self.measure_name} = {self.value}", verbose
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/acceleration/dst.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/dst.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
-
+import numpy as np
 import matplotlib.pyplot as plt
 import logging
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.type import TypeAcceleration, TypeMonotone
 from commonroad_crime.measure.distance.hw import HW
@@ -33,21 +33,16 @@
     monotone = TypeMonotone.POS
 
     def __init__(self, config: CriMeConfiguration):
         super(DST, self).__init__(config)
         self._hw_solver = HW(config)
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.set_other_vehicles(vehicle_id)
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         # under the assumption that the velocity of the other object remains constant
         headway = self._hw_solver.compute(vehicle_id, time_step)
         if headway < 0:
             return -math.inf
         v_ego = self.ego_vehicle.state_at_time(time_step).velocity
         v_otr = self.other_vehicle.state_at_time(time_step).velocity
         # from (17) in Schubert, Robin, Karsten Schulze, and Gerd Wanielik. "Situation assessment for automatic
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/distance/dce.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/distance/dce.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Oliver Specht, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 import math
 import matplotlib.pyplot as plt
 import logging
@@ -31,29 +31,23 @@
     """
 
     measure_name = TypeDistance.DCE
     monotone = TypeMonotone.NEG
 
     def __init__(self, config: CriMeConfiguration):
         super(DCE, self).__init__(config)
-        self.time_dce = None
+        self.time_dce = math.inf
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
         """
         Computed the shortest distance of ego-vehicle and obstacle by calculating the distance between both polygons
         (boundaries of both objects) for each time step and returning the minimum.
         """
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.set_other_vehicles(vehicle_id)
-        self.time_step = time_step
-
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         state_list = self.ego_vehicle.prediction.trajectory.state_list
         dce = math.inf
         for i in range(time_step, len(state_list)):
             if self.other_vehicle.occupancy_at_time(i) is not None:
                 ego_poly = self.ego_vehicle.occupancy_at_time(i).shape.shapely_object
                 other_shape = self.other_vehicle.occupancy_at_time(i).shape
                 if isinstance(other_shape, ShapeGroup):
@@ -83,22 +77,24 @@
             logger,
             f"*\t\t {self.measure_name} with vehicle id {vehicle_id} = {self.value}",
             verbose,
         )
         return self.value
 
     def visualize(self, figsize: tuple = (25, 15)):
-        self._initialize_vis(
-            figsize=figsize,
-            plot_limit=utils_vis.plot_limits_from_state_list(
+        if self.configuration.debug.plot_limits:
+            plot_limits = self.configuration.debug.plot_limits
+        else:
+            plot_limits = utils_vis.plot_limits_from_state_list(
                 self.time_step,
                 self.ego_vehicle.prediction.trajectory.state_list,
                 margin=10,
-            ),
-        )
+            )
+
+        self._initialize_vis(figsize=figsize, plot_limit=plot_limits)
         self.rnd.render()
         utils_vis.draw_reference_path(self.rnd, np.array(self.clcs.reference_path()))
         utils_vis.draw_state_list(
             self.rnd,
             self.ego_vehicle.prediction.trajectory.state_list[self.time_step :],
             color=TUMcolor.TUMblue,
             linewidth=5,
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/distance/hw.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/distance/hw.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import matplotlib.pyplot as plt
 import logging
 import math
@@ -13,14 +13,15 @@
 import numpy as np
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.type import TypeDistance, TypeMonotone
 from commonroad_crime.measure.time.thw import THW
 import commonroad_crime.utility.visualization as utils_vis
 import commonroad_crime.utility.solver as utils_sol
+import commonroad_crime.utility.logger as utils_log
 from commonroad_crime.utility.visualization import TUMcolor
 
 from commonroad.geometry.shape import Polygon, Circle
 
 logger = logging.getLogger(__name__)
 
 
@@ -51,31 +52,39 @@
                     self.other_vehicle.state_at_time(self.time_step).position
                     - self.other_vehicle.obstacle_shape.length / 2
                 )
         ego_position = (
             self.ego_vehicle.state_at_time(self.time_step).position
             + self.ego_vehicle.obstacle_shape.length / 2
         )
-        headway = utils_sol.compute_clcs_distance(
-            self.clcs, ego_position, other_position
-        )[0]
+        try:
+            headway = utils_sol.compute_clcs_distance(
+                self.clcs, ego_position, other_position
+            )[0]
+        except ValueError as e:
+            utils_log.print_and_log_warning(
+                logger, f"<HW> During the projection of the other vehicle: {e}"
+            )
+            headway = math.inf
         if headway < 0:
             return math.inf
         else:
             return headway
 
     def visualize(self, figsize: tuple = (25, 15)):
-        self._initialize_vis(
-            figsize=figsize,
-            plot_limit=utils_vis.plot_limits_from_state_list(
+        if self.configuration.debug.plot_limits:
+            plot_limits = self.configuration.debug.plot_limits
+        else:
+            plot_limits = utils_vis.plot_limits_from_state_list(
                 self.time_step,
                 self.ego_vehicle.prediction.trajectory.state_list,
                 margin=10,
-            ),
-        )
+            )
+
+        self._initialize_vis(figsize=figsize, plot_limit=plot_limits)
         self.rnd.render()
         utils_vis.draw_reference_path(self.rnd, np.array(self.clcs.reference_path()))
         utils_vis.draw_state_list(
             self.rnd,
             self.ego_vehicle.prediction.trajectory.state_list[self.time_step :],
             color=TUMcolor.TUMblue,
             linewidth=5,
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/distance/msd.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/distance/msd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin, Ziqian Xu"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
 import matplotlib.pyplot as plt
 import logging
@@ -34,20 +34,16 @@
     measure_name = TypeDistance.MSD
     monotone = TypeMonotone.POS
 
     def __init__(self, config: CriMeConfiguration):
         super(MSD, self).__init__(config)
 
     def compute(self, vehicle_id: int = None, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         state = self.ego_vehicle.state_at_time(time_step)
         lanelet_id = self.sce.lanelet_network.find_lanelet_by_position(
             [self.ego_vehicle.state_at_time(time_step).position]
         )[0]
 
         # compute the orientation of ego-vehicle
         ego_orientation = utils_sol.compute_lanelet_width_orientation(
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/distance/psd.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/distance/psd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin, Ziqian Xu"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
 from commonroad.scenario.obstacle import DynamicObstacle
 from commonroad_crime.data_structure.base import CriMeBase
@@ -39,21 +39,16 @@
 
     def __init__(self, config: CriMeConfiguration):
         super(PSD, self).__init__(config)
         self._msd_object = MSD(config)
         self._et_object = ET(config)
 
     def compute(self, vehicle_id: int = None, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} beginning at time step {time_step}",
-            verbose,
-        )
-        self.time_step = time_step
-        self.set_other_vehicles(vehicle_id)
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         # compute MSD
         if isinstance(self.other_vehicle, DynamicObstacle):
             self._et_object.ca = self._et_object.get_ca(
                 self.time_step, self.other_vehicle
             )
             if self._et_object.ca is not None:
                 # check when the ego vehicle enters the conflict area
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/index/aci.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/index/aci.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/index/btn.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/index/btn.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import logging
-import matplotlib.pyplot as plt
+import numpy as np
 
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.type import TypeIndex, TypeMonotone
 from commonroad_crime.measure.acceleration.a_long_req import ALongReq
 import commonroad_crime.utility.general as utils_gen
 import commonroad_crime.utility.logger as utils_log
-import commonroad_crime.utility.visualization as utils_vis
 
 logger = logging.getLogger(__name__)
 
 
 class BTN(CriMeBase):
     """
     the relation between the negative acceleration needed to marginally avoid a collision and the maximum deceleration
@@ -33,21 +32,16 @@
     monotone = TypeMonotone.POS
 
     def __init__(self, config: CriMeConfiguration):
         super(BTN, self).__init__(config)
         self._a_long_req_object = ALongReq(config)
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.set_other_vehicles(vehicle_id)
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         a_long_req = self._a_long_req_object.compute(
             vehicle_id, time_step, verbose=verbose
         )
         # (9) in "Using extreme value theory for vehicle level safety validation and implications
         # for autonomous vehicles."
         # maximum deceleration
         self.value = utils_gen.int_round(
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/index/ci.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/index/ci.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 __author__ = "Yuanfei Lin and Kun Qian"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import logging
 import matplotlib.pyplot as plt
 import math
+import numpy as np
+
 from commonroad.scenario.scenario import Tag
 
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.type import TypeIndex, TypeMonotone
 import commonroad_crime.utility.logger as utils_log
 from commonroad_crime.measure.time.pet import PET
@@ -35,21 +37,16 @@
 
     def __init__(self, config: CriMeConfiguration):
         super(CI, self).__init__(config)
         self._pet_object = PET(config)
         self.ci_config = config.index.ci
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.set_other_vehicles(vehicle_id)
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
 
         # Only for scenarios with intersection tag
         if (Tag.INTERSECTION not in self.sce.tags) or (
             len(self.sce.lanelet_network.intersections) == 0
         ):
             utils_log.print_and_log_info(
                 logger,
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/index/cpi.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/index/cpi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin, Sicheng Wang"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import logging
 import math
 
@@ -53,22 +53,17 @@
             a, b, self.cpi_config.madr_mean, self.cpi_config.madr_devi
         )
         self.dr_lon_req_list = []
         self.value = 0
         self.end_time_step = self.ego_vehicle.prediction.final_time_step
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} between ego vehicle"
-            f" and vehicle {vehicle_id} at timestep {time_step}.",
-            verbose,
-        )
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
 
-        self.time_step = time_step
         self.end_time_step = self.ego_vehicle.prediction.final_time_step
         self.value = 0.0
 
         for ts in range(self.time_step, self.end_time_step):
             try:
                 dr_lon_req = -self._a_lon_req_object.compute(vehicle_id, ts)
                 self.dr_lon_req_list.append(dr_lon_req)
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/index/pri.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/index/pri.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/index/rss.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/index/rss.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/index/soi.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/index/soi.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 __version__ = "0.3.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import logging
 import math
+import numpy as np
 
 from commonroad.scenario.obstacle import DynamicObstacle
 from matplotlib import pyplot as plt
 
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.type import TypeIndex, TypeMonotone
@@ -118,33 +119,29 @@
             )
         return personal_space
 
     def compute(self, time_step: int = 0, vehicle_id: int = None, verbose: bool = True):
         """
         Calculates how often the personal space of the ego-vehicle is violated by obstacles in the observed time
         """
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         self.value = 0
         self.value_list.clear()
-        self.time_step = time_step
 
         for ts in range(
             self.time_step, len(self.ego_vehicle.prediction.trajectory.state_list)
         ):
             ego_poly = self.create_sp_polygon(self.ego_vehicle, ts)
 
             for obstacle in self.sce.obstacles:
                 # Skip ego-vehicle and obstacles out of scope (e.g. timeline ended for this obstacle)
                 if (
                     isinstance(obstacle, DynamicObstacle)
-                    and len(obstacle.prediction.trajectory.state_list) < ts
+                    and obstacle.state_at_time(ts) is None
                 ):
                     continue
                 if obstacle.obstacle_id == self.ego_vehicle.obstacle_id:
                     continue
 
                 other_poly = utils_sol.create_polygon(obstacle, ts)
                 if ego_poly.intersects(other_poly):
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/index/stn.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/index/stn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import logging
+import numpy as np
 
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.type import TypeIndex, TypeMonotone
 from commonroad_crime.measure.acceleration.a_lat_req import ALatReq
 import commonroad_crime.utility.general as utils_gen
 import commonroad_crime.utility.logger as utils_log
@@ -31,21 +32,16 @@
     monotone = TypeMonotone.POS
 
     def __init__(self, config: CriMeConfiguration):
         super(STN, self).__init__(config)
         self._a_lat_req_object = ALatReq(config)
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.set_other_vehicles(vehicle_id)
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         a_lat_req = self._a_lat_req_object.compute(
             vehicle_id, time_step, verbose=verbose
         )
         # (1) in "Adaptive forward collision warning algorithm for automotive applications."
         self.value = utils_gen.int_round(
             abs(a_lat_req / self.configuration.vehicle.curvilinear.a_lat_max), 4
         )
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/index/tci.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/index/tci.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import logging
+import numpy as np
 import matplotlib.pyplot as plt
 
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.type import TypeIndex
 import commonroad_crime.utility.general as utils_gen
 import commonroad_crime.utility.logger as utils_log
@@ -36,20 +37,16 @@
 
     def __init__(self, config: CriMeConfiguration):
         super(TCI, self).__init__(config)
         self._optimizer = utils_opt.TCIOptimizer(config, self.sce)
         self._sol = None
 
     def compute(self, time_step: int = 0, vehicle_id: int = None, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
 
         self._sol, self.value = self._optimizer.optimize(self.ego_vehicle, time_step)
         self.value = utils_gen.int_round(self.value, 2)
         utils_log.print_and_log_info(
             logger, f"*\t\t {self.measure_name} = {self.value}", verbose
         )
         return self.value
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/jerk/lat_j.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/jerk/long_j.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
 import logging
+import numpy as np
 
-from commonroad_crime.data_structure.base import CriMeBase
+from commonroad_crime.measure.jerk.lat_j import LatJ
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.type import TypeJerk, TypeMonotone
 import commonroad_crime.utility.general as utils_gen
 import commonroad_crime.utility.logger as utils_log
 import commonroad_crime.utility.solver as utils_sol
 
 logger = logging.getLogger(__name__)
 
 
-class LatJ(CriMeBase):
+class LongJ(LatJ):
     """
     Jerk is the rate of change in acceleration, and thus quantifies over the abruptness of a maneuver.
     """
 
-    measure_name = TypeJerk.LatJ
+    measure_name = TypeJerk.LongJ
     monotone = TypeMonotone.POS
 
     def __init__(self, config: CriMeConfiguration):
-        super(LatJ, self).__init__(config)
+        super(LongJ, self).__init__(config)
 
     def compute(self, time_step: int, vehicle_id: int = None, verbose: bool = True):
-        self.time_step = time_step
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
+        evaluated_state = self.ego_vehicle.state_at_time(self.time_step)
         lanelet_id = self.sce.lanelet_network.find_lanelet_by_position(
             [self.ego_vehicle.state_at_time(time_step).position]
         )[0]
         # orientation of the ego vehicle and the other vehicle
         ego_orientation = utils_sol.compute_lanelet_width_orientation(
             self.sce.lanelet_network.find_lanelet_by_id(lanelet_id[0]),
             self.ego_vehicle.state_at_time(time_step).position,
         )[1]
-        evaluated_state = self.ego_vehicle.state_at_time(self.time_step)
         self.value = utils_gen.int_round(
-            abs(evaluated_state.jerk * math.sin(ego_orientation)), 2
+            abs(evaluated_state.jerk * math.cos(ego_orientation)), 2
+        )
+        utils_log.print_and_log_info(
+            logger, f"*\t\t {self.measure_name} = {self.value}", verbose
         )
         return self.value
 
     def visualize(self):
         pass
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/jerk/long_j.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttr.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,76 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
-import math
 import logging
+import numpy as np
+from typing import Union
 
-from commonroad_crime.measure.jerk.lat_j import LatJ
+from commonroad_crime.measure.time.ttb import TTB
+from commonroad_crime.measure.time.ttk import TTK
+from commonroad_crime.measure.time.tts import TTS
+from commonroad_crime.measure.time.ttm import TTM
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
-from commonroad_crime.data_structure.type import TypeJerk, TypeMonotone
-import commonroad_crime.utility.general as utils_gen
+from commonroad_crime.data_structure.type import TypeTime
+from commonroad_crime.utility.simulation import Maneuver
 import commonroad_crime.utility.logger as utils_log
-import commonroad_crime.utility.solver as utils_sol
 
 logger = logging.getLogger(__name__)
 
 
-class LongJ(LatJ):
+class TTR(TTM):
     """
-    Jerk is the rate of change in acceleration, and thus quantifies over the abruptness of a maneuver.
+    Time-to-react: latest possible time before the TTC, at which an evasive maneuver still exists. This
+    under-approximative approach is obtained from Tamke, Andreas, Thao Dang, and Gabi Breuel.
+    "A flexible method for criticality assessment in driver assistance systems." 2011 IEEE intelligent
+     vehicles symposium (IV). IEEE, 2011.
     """
 
-    measure_name = TypeJerk.LongJ
-    monotone = TypeMonotone.POS
+    measure_name = TypeTime.TTR
 
     def __init__(self, config: CriMeConfiguration):
-        super(LongJ, self).__init__(config)
+        super(TTR, self).__init__(config, Maneuver.NONE)
+        self._evaluator = None
 
-    def compute(self, time_step: int, vehicle_id: int = None, verbose: bool = True):
+    def initialize_evaluator(self, time_step: int, verbose: bool):
+        """
+        Initializes the evaluators for underestimating the ttr.
+        """
+        self._evaluator = [
+            TTB(self.configuration),
+            TTK(self.configuration),
+            TTS(self.configuration),
+        ]
         self.time_step = time_step
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        evaluated_state = self.ego_vehicle.state_at_time(self.time_step)
-        lanelet_id = self.sce.lanelet_network.find_lanelet_by_position(
-            [self.ego_vehicle.state_at_time(time_step).position]
-        )[0]
-        # orientation of the ego vehicle and the other vehicle
-        ego_orientation = utils_sol.compute_lanelet_width_orientation(
-            self.sce.lanelet_network.find_lanelet_by_id(lanelet_id[0]),
-            self.ego_vehicle.state_at_time(time_step).position,
-        )[1]
-        self.value = utils_gen.int_round(
-            abs(evaluated_state.jerk * math.cos(ego_orientation)), 2
-        )
+        self.state_list_set = []
+        self.ttc = self.ttc_object.compute(time_step, verbose=verbose)
+
+    def compute(
+        self,
+        time_step: int = 0,
+        vehicle_id: Union[int, None] = None,
+        ttc: float = None,
+        verbose: bool = True,
+    ):
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
+        self.initialize_evaluator(self.time_step, verbose)
+        ttm = dict()
+        for evl in self._evaluator:
+            ttm[evl] = evl.compute(
+                time_step=self.time_step, ttc=self.ttc, verbose=False
+            )
+            self.state_list_set += evl.state_list_set
+        self.value = max(ttm.values())
+        # plots the selected state list as the last evasive maneuver.
+        self.selected_state_list = max(ttm, key=ttm.get).selected_state_list
+        self.maneuver = max(ttm, key=ttm.get).maneuver
+        utils_log.print_and_log_info(logger, "*\t maximum of the values")
         utils_log.print_and_log_info(
             logger, f"*\t\t {self.measure_name} = {self.value}", verbose
         )
         return self.value
-
-    def visualize(self):
-        pass
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/potential/pf.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/potential/pf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import logging
 
 from shapely.geometry import Polygon, Point, LineString
@@ -37,20 +37,16 @@
 
     def __init__(self, config: CriMeConfiguration):
         super(PF, self).__init__(config)
         self._s_ego = None
         self._d_ego = None
 
     def compute(self, time_step: int, vehicle_id: int = None, verbose: bool = True):
-        self.time_step = time_step
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         evaluated_state = self.ego_vehicle.state_at_time(self.time_step)
         try:
             self._s_ego, self._d_ego = self.clcs.convert_to_curvilinear_coords(
                 evaluated_state.position[0], evaluated_state.position[1]
             )
         except ValueError as err:
             utils_log.print_and_log_error(logger, err)
@@ -177,50 +173,60 @@
             return xi_m
 
         config_pot = self.configuration.potential
         u_car = 0
         for obs in self.sce.obstacles:
             if obs is not self.ego_vehicle:
                 # shape in curvilinear coordinate system
-                obs_clcs_shape = self.clcs.convert_list_of_polygons_to_curvilinear_coords_and_rasterize(
-                    [
-                        obs.occupancy_at_time(
-                            self.time_step
-                        ).shape.shapely_object.exterior.coords
-                    ],
-                    [0],
-                    1,
-                    4,
-                )[
-                    0
-                ]
-                if len(obs_clcs_shape[0]) == 0:
+                if obs.occupancy_at_time(self.time_step) is not None:
+                    obs_clcs_shape = self.clcs.convert_list_of_polygons_to_curvilinear_coords_and_rasterize(
+                        [
+                            obs.occupancy_at_time(
+                                self.time_step
+                            ).shape.shapely_object.exterior.coords
+                        ],
+                        [0],
+                        1,
+                        4,
+                    )[
+                        0
+                    ][
+                        0
+                    ]
+                else:
+                    utils_log.print_and_log_warning(
+                        logger,
+                        f"At Time step {self.time_step}: the obstable {obs.obstacle_id} does not exist",
+                        verbose,
+                    )
+                    obs_clcs_shape = []
+                if len(obs_clcs_shape) == 0:
                     utils_log.print_and_log_warning(
                         logger,
                         f"At Time step {self.time_step}: the conversion of the polygon to the "
                         f"curvilinear coordinates failed, u_car is set to 0",
                         verbose,
                     )
                     u_car += 0
                     continue
-                obs_clcs_poly = Polygon(obs_clcs_shape[0][0])
+                obs_clcs_poly = Polygon(obs_clcs_shape[0])
                 obs_s_min = np.min(obs_clcs_poly.exterior.xy[0])
                 if isinstance(obs, StaticObstacle) or (
                     isinstance(obs, DynamicObstacle) and (s_veh > obs_s_min).any()
                 ):
                     # static obstacle or forward/side of obstacle ->
                     # Euclidean distance to the nearest point on the obstacle
                     if obs_clcs_poly.contains(Point(s_veh, d_veh)):
                         K = 0.0
                     else:
                         K = Point(s_veh, d_veh).distance(obs_clcs_poly)
                 else:
                     # behind dynamic obstacle
-                    minx, miny = np.array(obs_clcs_shape[0][0]).min(axis=0)
-                    maxx, maxy = np.array(obs_clcs_shape[0][0]).max(axis=0)
+                    minx, miny = np.array(obs_clcs_shape[0]).min(axis=0)
+                    maxx, maxy = np.array(obs_clcs_shape[0]).max(axis=0)
                     bottommost_then_leftmost_point = np.array([minx, maxy])
                     topmost_then_leftmost_point = np.array([minx, miny])
                     # * previous option: the sort of the orders but doesn't work for some scenarios
                     # topmost_then_leftmost_point = min(obs_clcs_shape[0][0], key=lambda pt: (-pt[0], pt[1]))
                     # bottommost_then_leftmost_point = min(obs_clcs_shape[0][0], key=lambda pt: (-pt[1], pt[0]))
                     wedge_point_l = (
                         LineString(
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/potential/sp.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/potential/sp.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/probability/p_mc.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/probability/p_mc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import numpy as np
 import matplotlib.pyplot as plt
 import logging
@@ -69,26 +69,23 @@
         )
         self.ego_state_list_set_cf = []  # collision-free
         self.ego_state_list_set_wc = []  # with collisions
         self.sim_time_steps = int(config_mc.prediction_horizon / self.sce.dt)
         self.ttc_object = TTCStar(self.configuration)
 
     def compute(self, time_step: int = 0, vehicle_id=None, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         utils_log.print_and_log_info(
             logger,
             f"* \t\t nr of samples "
             f"{self.configuration.probability.monte_carlo.nr_samples}",
             verbose,
         )
-        self.time_step = time_step
+
         colliding_prob_list = []
         self.ego_state_list_set_cf = []  # collision-free
         self.ego_state_list_set_wc = []  # with collisions
         for i in range(len(self.maneuver_list)):
             maneuver = self.maneuver_list[i]
             # randomly rounding to integer
             nr_sample_maneuver = int(
@@ -96,17 +93,19 @@
             )
             ego_sl_bundle, pdf_bundle = self.monte_carlo_simulation(
                 self.ego_vehicle, maneuver, nr_sample_maneuver
             )
             for j in range(len(ego_sl_bundle)):
                 if self.ttc_object.detect_collision(ego_sl_bundle[j]):
                     colliding_prob_list.append(pdf_bundle[j])
-                    self.ego_state_list_set_wc.append(ego_sl_bundle[j])
+                    if self.configuration.debug.draw_visualization:
+                        self.ego_state_list_set_wc.append(ego_sl_bundle[j])
                 else:
-                    self.ego_state_list_set_cf.append(ego_sl_bundle[j])
+                    if self.configuration.debug.draw_visualization:
+                        self.ego_state_list_set_cf.append(ego_sl_bundle[j])
         # (14) in Broadhurst, Adrian, Simon Baker, and Takeo Kanade. "Monte Carlo road safety reasoning." IEEE
         # Proceedings of Intelligent Vehicles Symposium, IEEE, 2005.
         if colliding_prob_list:
             p_mc = np.average(np.array(colliding_prob_list))
             self.value = utils_gen.int_round(p_mc, 4)
         else:
             utils_log.print_and_log_error(
@@ -148,22 +147,24 @@
             state_list_bundle.append(
                 simulator.simulate_state_list(self.time_step, self.sim_time_steps)
             )
             pdf_bundle.append(simulator.pdf)
         return state_list_bundle, pdf_bundle
 
     def visualize(self, figsize: tuple = (25, 15)):
-        self._initialize_vis(
-            figsize=figsize,
-            plot_limit=utils_vis.plot_limits_from_state_list(
+        if self.configuration.debug.plot_limits:
+            plot_limits = self.configuration.debug.plot_limits
+        else:
+            plot_limits = utils_vis.plot_limits_from_state_list(
                 self.time_step,
                 self.ego_vehicle.prediction.trajectory.state_list,
                 margin=20,
-            ),
-        )
+            )
+
+        self._initialize_vis(figsize=figsize, plot_limit=plot_limits)
         self.rnd.render()
         for sl in self.ego_state_list_set_wc:
             utils_vis.draw_state_list(self.rnd, sl, color=TUMcolor.TUMred)
         for sl in self.ego_state_list_set_cf:
             utils_vis.draw_state_list(self.rnd, sl, color=TUMcolor.TUMblue)
         plt.title(f"{self.measure_name} at time step {self.time_step} is {self.value}")
         if self.configuration.debug.save_plots:
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/probability/p_smh.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/probability/p_smh.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/probability/p_srs.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/probability/p_srs.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/reachable_set/drivable_area.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/reachable_set/drivable_area.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.1"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import copy
 import numpy as np
 import logging
@@ -75,16 +75,18 @@
             target_state.orientation
         )
         self.reach_config.planning_problem.initial_state.time_step = (
             target_state.time_step
         )
 
     def compute(self, time_step: int = 0, vehicle_id: int = None, verbose: bool = True):
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         self.value = 0.0
-        evaluated_state = copy.deepcopy(self.ego_vehicle.state_at_time(time_step))
+        evaluated_state = copy.deepcopy(self.ego_vehicle.state_at_time(self.time_step))
         self._update_initial_state(target_state=evaluated_state)
         self.reach_config.update(planning_problem=self.reach_config.planning_problem)
         self.reach_config.scenario.remove_obstacle(
             self.reach_config.scenario.obstacle_by_id(self.ego_vehicle.obstacle_id)
         )
         self.reach_interface.reset(self.reach_config)
         self.reach_interface.compute_reachable_sets(verbose=verbose)
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/ags.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/ags.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/et.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/et.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 __author__ = "Yuanfei Lin, Liguo Chen"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
 import matplotlib.pyplot as plt
 import logging
+import numpy as np
 from typing import Union
 from shapely.geometry import Polygon
 
 from commonroad.scenario.scenario import Tag
 from commonroad.scenario.lanelet import LaneletType, Lanelet
 from commonroad.scenario.obstacle import DynamicObstacle
 
@@ -42,21 +43,16 @@
         # Conflict area
         self.ca = None
         # The time points when the ego vehicle enters and leaves the conflict area
         self.enter_time: Union[int, float] = math.inf
         self.exit_time: Union[int, float] = math.inf
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} beginning at time step {time_step}",
-            verbose,
-        )
-        self.time_step = time_step
-        self.set_other_vehicles(vehicle_id)
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         # check whether there is an intersection
         if (Tag.INTERSECTION not in self.sce.tags) or (
             len(self.sce.lanelet_network.intersections) == 0
         ):
             utils_log.print_and_log_info(
                 logger,
                 f"* \t\tMeasure only for intersection. {self.measure_name} is set to inf.",
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/pet.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/pet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 __author__ = "Yuanfei Lin, Liguo Chen"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import matplotlib.pyplot as plt
+import numpy as np
 import logging
 from typing import Union
 import math
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.type import TypeTime, TypeMonotone
 from commonroad_crime.measure.time.et import ET
@@ -40,21 +41,16 @@
         self.other_vehicle_exit_time: Union[float, int] = math.inf
         self.other_vehicle_enter_time: Union[float, int] = math.inf
         self.ego_vehicle_exit_time: Union[float, int] = math.inf
         self.ego_vehicle_enter_time: Union[float, int] = math.inf
         self.case_one: bool = False
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} beginning at time step {time_step}",
-            verbose,
-        )
-        self.time_step = time_step
-        self.set_other_vehicles(vehicle_id)
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         if (Tag.INTERSECTION not in self.sce.tags) or (
             len(self.sce.lanelet_network.intersections) == 0
         ):
             utils_log.print_and_log_info(
                 logger,
                 f"*\t\t There is no intersection. \n*\t\t {self.measure_name} = {self.value}",
                 verbose,
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/pttc.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/pttc.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/tc.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/tc.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/tet.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/tet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 __author__ = "Oliver Specht, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import logging
+import numpy as np
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.type import TypeTime, TypeMonotone
 from commonroad_crime.measure.time.tit import TIT
 import commonroad_crime.utility.logger as utils_log
 import commonroad_crime.utility.general as utils_gen
 
@@ -30,21 +31,16 @@
         super(TET, self).__init__(config)
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
         """
         Iterate through all states, calculate ttc, compare it to tau and then add dt to the result
         if ttc is smaller than tau
         """
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} beginning at time step {time_step}",
-            verbose,
-        )
-        # init
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         tau = self.configuration.time.tau
         state_list = self.ego_vehicle.prediction.trajectory.state_list
 
         self.value = 0
         for i in range(time_step, len(state_list)):
             ttc_result = self.ttc_object.compute(vehicle_id, i, verbose=verbose)
             self._ttc_cache[i] = ttc_result
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/thw.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/thw.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import matplotlib.pyplot as plt
 import logging
 import math
+import numpy as np
+
+from commonroad.geometry.shape import Rectangle, Circle
+from commonroad.scenario.obstacle import Obstacle
 
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.type import TypeTime, TypeMonotone
 import commonroad_crime.utility.visualization as utils_vis
 import commonroad_crime.utility.general as utils_gen
 import commonroad_crime.utility.logger as utils_log
@@ -28,54 +32,78 @@
 
     measure_name = TypeTime.THW
     monotone = TypeMonotone.NEG
 
     def __init__(self, config: CriMeConfiguration):
         super(THW, self).__init__(config)
 
+    def _compute_vehicle_add_on(self, vehicle: Obstacle):
+        if isinstance(vehicle.obstacle_shape, Rectangle):
+            add_on = vehicle.obstacle_shape.length / 2
+        elif isinstance(vehicle.obstacle_shape, Circle):
+            add_on = vehicle.obstacle_shape.radius
+        else:
+            raise ValueError(
+                f"<{self.measure_name}>: obstacle shape {type(vehicle.obstacle_shape).__name__} not supported."
+            )
+        return add_on
+
     def cal_headway(self):
-        other_position = self.other_vehicle.state_at_time(self.time_step).position
-        other_s, _ = self.clcs.convert_to_curvilinear_coords(
-            other_position[0], other_position[1]
-        )
-        ego_position = self.ego_vehicle.state_at_time(self.time_step).position
-        ego_s, _ = self.clcs.convert_to_curvilinear_coords(
-            ego_position[0], ego_position[1]
-        )
+        try:
+            other_position = self.other_vehicle.state_at_time(self.time_step).position
+            other_s, _ = self.clcs.convert_to_curvilinear_coords(
+                other_position[0], other_position[1]
+            )
+        except ValueError as e:
+            utils_log.print_and_log_warning(
+                logger,
+                f"* <THW> During the projection of the vehicle {self.other_vehicle.obstacle_id} "
+                f"at time step {self.time_step}: {e}",
+            )
+            # out of projection domain: the other vehicle is far away
+            return math.inf
+        try:
+            ego_position = self.ego_vehicle.state_at_time(self.time_step).position
+            ego_s, _ = self.clcs.convert_to_curvilinear_coords(
+                ego_position[0], ego_position[1]
+            )
+        except ValueError as e:
+            utils_log.print_and_log_warning(
+                logger,
+                f"* <THW> During the projection of the ego vehicle with id {self.ego_vehicle.obstacle_id} "
+                f"at time step {self.time_step}: {e}",
+            )
+            # out of projection domain: the ref path should be problematic
+            return math.nan
 
-        # bump position
-        ego_s += self.ego_vehicle.obstacle_shape.length / 2
-        other_s -= self.other_vehicle.obstacle_shape.length / 2
+        # additional position for the vehicles
+        ego_s += self._compute_vehicle_add_on(self.ego_vehicle)
+        other_s -= self._compute_vehicle_add_on(self.other_vehicle)
 
         if ego_s > other_s:
             return math.inf
         # another option is (other_s-ego_s)/self.ego_vehicle.state_at_time(self.time_step).velocity
         # here since the predicted trajectory is given, we use it to make the result more accurate
         for ts in range(
             self.time_step + 1, self.ego_vehicle.prediction.final_time_step + 1
         ):
             ego_position = self.ego_vehicle.state_at_time(ts).position
             ego_s, _ = self.clcs.convert_to_curvilinear_coords(
                 ego_position[0], ego_position[1]
             )
-            ego_s += self.ego_vehicle.obstacle_shape.length / 2
+            ego_s += self._compute_vehicle_add_on(self.ego_vehicle)
             if ego_s > other_s:
                 return utils_gen.int_round(
                     (ts - self.time_step) * self.dt, str(self.dt)[::-1].find(".")
                 )
         return math.inf
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.set_other_vehicles(vehicle_id)
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
 
         if self._except_obstacle_in_same_lanelet(
             expected_value=math.inf, verbose=verbose
         ):
             return self.value
         self.value = self.cal_headway()
         if self.value is not math.inf:
@@ -84,32 +112,31 @@
             logger,
             f"*\t\t {self.measure_name} with vehicle id {vehicle_id} = {self.value}",
             verbose,
         )
         return self.value
 
     def visualize(self, figsize: tuple = (25, 15)):
-        self._initialize_vis(
-            figsize=figsize,
-            plot_limit=utils_vis.plot_limits_from_state_list(
+        if self.configuration.debug.plot_limits:
+            plot_limits = self.configuration.debug.plot_limits
+        else:
+            plot_limits = utils_vis.plot_limits_from_state_list(
                 self.time_step,
                 self.ego_vehicle.prediction.trajectory.state_list,
-                margin=10,
-            ),
-        )
+                margin=50,
+            )
+        self._initialize_vis(figsize=figsize, plot_limit=plot_limits)
         self.rnd.render()
         utils_vis.draw_state_list(
             self.rnd,
             self.ego_vehicle.prediction.trajectory.state_list[self.time_step :],
             color=TUMcolor.TUMblue,
             linewidth=5,
         )
         if self.value > 0 and self.value is not math.inf:
-            print(self.value)
-
             tshw = int(utils_gen.int_round(self.value / self.dt, 0))
             utils_vis.draw_state(
                 self.rnd, self.ego_vehicle.state_at_time(tshw + self.time_step)
             )
             utils_vis.draw_dyn_vehicle_shape(
                 self.rnd, self.ego_vehicle, tshw + self.time_step
             )
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/tit.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/tit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Oliver Specht, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import matplotlib.pyplot as plt
 import numpy as np
 import logging
@@ -37,26 +37,23 @@
         self._ttc_cache = dict()
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
         """
         Iterate through all states, calculate ttc, compare it to tau and then add dt to the result
         if ttc is smaller than tau
         """
-        # init
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} beginning at time step {time_step}",
-            verbose,
-        )
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
+
         tau = self.configuration.time.tau
         state_list = self.ego_vehicle.prediction.trajectory.state_list
         self._ttc_cache.clear()
 
         self.value = 0
-        for i in range(time_step, len(state_list)):
+        for i in range(self.time_step, len(state_list)):
             ttc_result = self.ttc_object.compute(vehicle_id, i, verbose=verbose)
             self._ttc_cache[i] = ttc_result
             if ttc_result <= tau:
                 self.value += (tau - ttc_result) * self.dt
         self.value = utils_gen.int_round(self.value, 4)
         utils_log.print_and_log_info(
             logger, f"*\t\t {self.measure_name} = {self.value}", verbose
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/ttb.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttb.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/ttc.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin, Oliver Specht"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import logging
 import math
 
@@ -37,21 +37,16 @@
     monotone = TypeMonotone.NEG
 
     def __init__(self, config: CriMeConfiguration):
         super(TTC, self).__init__(config)
         self._hw_object = HW(config)
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.set_other_vehicles(vehicle_id)
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         state = self.ego_vehicle.state_at_time(time_step)
         state_other = self.other_vehicle.state_at_time(time_step)
         lanelet_id = self.sce.lanelet_network.find_lanelet_by_position(
             [self.ego_vehicle.state_at_time(time_step).position]
         )[0]
         """
         Using https://www.diva-portal.org/smash/get/diva2:617438/FULLTEXT01.pdf 
@@ -61,57 +56,77 @@
         # distance along the lanelet
         delta_d = self._hw_object.compute(vehicle_id, time_step, verbose)
 
         if delta_d == math.inf:
             self.value = math.inf
         else:
             # orientation of the ego vehicle and the other vehicle
-            ego_orientation = utils_sol.compute_lanelet_width_orientation(
-                self.sce.lanelet_network.find_lanelet_by_id(lanelet_id[0]),
-                self.ego_vehicle.state_at_time(time_step).position,
-            )[1]
-            other_orientation = utils_sol.compute_lanelet_width_orientation(
-                self.sce.lanelet_network.find_lanelet_by_id(lanelet_id[0]),
-                self.other_vehicle.state_at_time(time_step).position,
-            )[1]
-            # actual velocity and acceleration of both vehicles along the lanelet
-            v_ego = (
-                np.sign(state.velocity)
-                * math.sqrt(state.velocity**2 + state.velocity_y**2)
-                * math.cos(ego_orientation)
-            )
-            # include the directions
-            a_ego = (
-                np.sign(state.acceleration)
-                * math.sqrt(state.acceleration**2 + state.acceleration_y**2)
-                * math.cos(ego_orientation)
-            )
-            if isinstance(self.other_vehicle, DynamicObstacle):
-                v_other = math.sqrt(
-                    state_other.velocity**2 + state_other.velocity_y**2
-                ) * math.cos(other_orientation)
-                a_other = math.sqrt(
-                    state_other.acceleration**2 + state_other.acceleration_y**2
-                ) * math.cos(other_orientation)
+
+            try:
+                ego_orientation = utils_sol.compute_lanelet_width_orientation(
+                    self.sce.lanelet_network.find_lanelet_by_id(lanelet_id[0]),
+                    self.ego_vehicle.state_at_time(time_step).position,
+                )[1]
+            except ValueError as e:
+                utils_log.print_and_log_warning(
+                    logger,
+                    f"* <TTC> During the projection of the ego vehicle {self.ego_vehicle.obstacle_id} "
+                    f"at time step {self.time_step}: {e}",
+                )
+                self.value = math.nan
             else:
-                v_other = 0.0
-                a_other = 0.0
-            delta_v = v_other - v_ego
-            delta_a = a_other - a_ego
-
-            if delta_v < 0 and abs(delta_a) <= 0.1:
-                self.value = utils_gen.int_round(-(delta_d / delta_v), 2)
-            elif delta_v**2 - 2 * delta_d * delta_a < 0:
-                self.value = math.inf
-            elif (delta_v < 0 and delta_a != 0) or (delta_v >= 0 > delta_a):
-                first = -(delta_v / delta_a)
-                second = np.sqrt(delta_v**2 - 2 * delta_d * delta_a) / delta_a
-                self.value = utils_gen.int_round(first - second, 2)
-            else:  # delta_v >= 0 and delta_a >= 0
-                self.value = math.inf
+                try:
+                    other_orientation = utils_sol.compute_lanelet_width_orientation(
+                        self.sce.lanelet_network.find_lanelet_by_id(lanelet_id[0]),
+                        self.other_vehicle.state_at_time(time_step).position,
+                    )[1]
+                except ValueError as e:
+                    utils_log.print_and_log_warning(
+                        logger,
+                        f"* <TTC> During the projection of the vehicle {self.other_vehicle.obstacle_id} "
+                        f"at time step {self.time_step}: {e}",
+                    )
+                    # out of projection domain: the other vehicle is far away
+                    self.value = math.inf
+                else:
+                    # actual velocity and acceleration of both vehicles along the lanelet
+                    v_ego = (
+                        np.sign(state.velocity)
+                        * math.sqrt(state.velocity**2 + state.velocity_y**2)
+                        * math.cos(ego_orientation)
+                    )
+                    # include the directions
+                    a_ego = (
+                        np.sign(state.acceleration)
+                        * math.sqrt(state.acceleration**2 + state.acceleration_y**2)
+                        * math.cos(ego_orientation)
+                    )
+                    if isinstance(self.other_vehicle, DynamicObstacle):
+                        v_other = math.sqrt(
+                            state_other.velocity**2 + state_other.velocity_y**2
+                        ) * math.cos(other_orientation)
+                        a_other = math.sqrt(
+                            state_other.acceleration**2 + state_other.acceleration_y**2
+                        ) * math.cos(other_orientation)
+                    else:
+                        v_other = 0.0
+                        a_other = 0.0
+                    delta_v = v_other - v_ego
+                    delta_a = a_other - a_ego
+
+                    if delta_v < 0 and abs(delta_a) <= 0.1:
+                        self.value = utils_gen.int_round(-(delta_d / delta_v), 2)
+                    elif delta_v**2 - 2 * delta_d * delta_a < 0:
+                        self.value = math.inf
+                    elif (delta_v < 0 and delta_a != 0) or (delta_v >= 0 > delta_a):
+                        first = -(delta_v / delta_a)
+                        second = np.sqrt(delta_v**2 - 2 * delta_d * delta_a) / delta_a
+                        self.value = utils_gen.int_round(first - second, 2)
+                    else:  # delta_v >= 0 and delta_a >= 0
+                        self.value = math.inf
 
         utils_log.print_and_log_info(
             logger, f"*\t\t {self.measure_name} = {self.value}", verbose
         )
         return self.value
 
     def visualize(self):
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/ttc_star.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttc_star.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import copy
 import math
 import logging
 from typing import List
+import numpy as np
 import matplotlib.pyplot as plt
 
 from commonroad.visualization.mp_renderer import MPRenderer
 from commonroad.scenario.state import CustomState, State
 from commonroad.scenario.scenario import TrajectoryPrediction
 from commonroad.scenario.trajectory import Trajectory
 
@@ -126,20 +127,17 @@
             plt.show()
 
     def compute(self, time_step: int = 0, vehicle_id: int = None, verbose: bool = True):
         """
         Detects the collision time given the trajectory of ego_vehicle using a for loop over
         the state list.
         """
-        self.time_step = time_step
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
+
         state_list = self.ego_vehicle.prediction.trajectory.state_list
         self.value = math.inf
         for i in range(time_step, len(state_list)):
             # i-th time step
             pos1 = self.ego_vehicle.state_at_time(i).position[0]
             pos2 = self.ego_vehicle.state_at_time(i).position[1]
             theta = self.ego_vehicle.state_at_time(i).orientation
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/ttce.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttce.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 __author__ = "Oliver Specht, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "beta"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 import matplotlib.pyplot as plt
+import numpy as np
 import logging
+import math
 
 from commonroad_crime.measure.distance.dce import DCE
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.type import TypeTime, TypeMonotone
 import commonroad_crime.utility.logger as utils_log
 import commonroad_crime.utility.general as utils_gen
@@ -35,23 +37,24 @@
         super(TTCE, self).__init__(config)
         self._dce_object = DCE(config)
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
         """
         Using DCE to calculate the TTCE value. DCE marks the time step when the minimal distance is reached.
         """
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self._dce_object.compute(vehicle_id, time_step)
-        self.value = utils_gen.int_round(
-            (self._dce_object.time_dce - time_step) * self.dt, 3
-        )
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
+
+        self._dce_object.compute(vehicle_id, self.time_step)
+        if self._dce_object.time_dce is not math.inf:
+            self.value = utils_gen.int_round(
+                (self._dce_object.time_dce - self.time_step) * self.dt, 3
+            )
+        else:
+            self.value = self._dce_object.time_dce
         utils_log.print_and_log_info(
             logger,
             f"*\t\t {self.measure_name} with vehicle id {vehicle_id} = {self.value}",
             verbose,
         )
         return self.value
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/ttk.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttk.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/ttm.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
 import matplotlib.pyplot as plt
 from typing import Union
 import logging
+import numpy as np
 
 from commonroad.scenario.state import CustomState
 
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.utility.simulation import SimulationLong, SimulationLat, Maneuver
 from commonroad_crime.measure.time.ttc_star import TTCStar
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
@@ -129,21 +130,18 @@
     def compute(
         self,
         time_step: int = 0,
         vehicle_id: Union[int, None] = None,
         ttc: float = None,
         verbose: bool = True,
     ):
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         self.state_list_set = []
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.time_step = time_step
+
         if ttc:
             self.ttc = ttc
         else:
             self.ttc = self.ttc_object.compute(time_step, verbose=verbose)
         if self.ttc == 0:
             self.value = -math.inf
         elif self.ttc == math.inf:
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/tts.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/tts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import logging
+import numpy as np
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.type import TypeTime
 from commonroad_crime.measure.time.ttm import TTM
 from commonroad_crime.utility.simulation import Maneuver
 import commonroad_crime.utility.logger as utils_log
@@ -40,22 +41,25 @@
     def compute(
         self,
         time_step: int = 0,
         vehicle_id: int = None,
         ttc: float = None,
         verbose: bool = True,
     ):
-        utils_log.print_and_log_info(
-            logger, f"* Computing the {self.measure_name} at time step {time_step}"
-        )
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
 
-        tts_left = self._left_evaluator.compute(time_step, ttc, verbose=False)
+        tts_left = self._left_evaluator.compute(
+            time_step=self.time_step, ttc=ttc, verbose=False
+        )
         self.state_list_set += self._left_evaluator.state_list_set
 
-        tts_right = self._right_evaluator.compute(time_step, ttc, verbose=False)
+        tts_right = self._right_evaluator.compute(
+            time_step=self.time_step, ttc=ttc, verbose=False
+        )
         self.state_list_set += self._right_evaluator.state_list_set
 
         # decide the specific maneuver for steering
         if tts_left > tts_right:
             self.maneuver = Maneuver.STEERLEFT
             self.selected_state_list = self._left_evaluator.selected_state_list
         else:
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/ttz.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttz.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import logging
 import math
 from shapely.geometry import Point
@@ -36,21 +36,17 @@
 
     measure_name = TypeTime.TTZ
 
     def __init__(self, config: CriMeConfiguration):
         super(TTZ, self).__init__(config)
         self._zebra_list = []
 
-    def compute(self, time_step: int = 0, other_id: int = None, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.time_step = time_step
+    def compute(self, time_step: int = 0, vehicle_id: int = None, verbose: bool = True):
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         zebra_list = []
         for ll in self.sce.lanelet_network.lanelets:
             if LaneletType.CROSSWALK in ll.lanelet_type:
                 zebra_list.append(ll)
         if zebra_list:
             ttz_list = []
             for zebra in zebra_list:
@@ -97,22 +93,23 @@
             self.value = math.inf
         utils_log.print_and_log_info(
             logger, f"*\t\t {self.measure_name} = {self.value}", verbose
         )
         return self.value
 
     def visualize(self, figsize: tuple = (25, 15)):
-        self._initialize_vis(
-            figsize=figsize,
-            plot_limit=utils_vis.plot_limits_from_state_list(
+        if self.configuration.debug.plot_limits:
+            plot_limits = self.configuration.debug.plot_limits
+        else:
+            plot_limits = utils_vis.plot_limits_from_state_list(
                 self.time_step,
                 self.ego_vehicle.prediction.trajectory.state_list,
-                margin=10,
-            ),
-        )
+                margin=50,
+            )
+        self._initialize_vis(figsize=figsize, plot_limit=plot_limits)
         self.rnd.render()
         # ------------- Plot zebra crossing ------------------
 
         def imshow_affine(ax, z, *args, **kwargs):
             im = ax.imshow(z, *args, **kwargs)
             x1, x2, y1, y2 = im.get_extent()
             im._image_skew_coordinate = (x2, y1)
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/tv.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/tv.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/wttc.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/wttc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import numpy as np
 import matplotlib.pyplot as plt
 import logging
@@ -33,21 +33,16 @@
     measure_name = TypeTime.WTTC
     monotone = TypeMonotone.NEG
 
     def __init__(self, config: CriMeConfiguration):
         super(WTTC, self).__init__(config)
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.time_step = time_step
-        self.set_other_vehicles(vehicle_id)
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         wttc_list = utils_sol.solver_wttc(
             self.ego_vehicle,
             self.other_vehicle,
             time_step,
             self.configuration.vehicle.params.longitudinal.a_max,
         )
         self.value = max(
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/time/wttr.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/time/wttr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
 import copy
 import logging
+import numpy as np
 
 from commonroad.scenario.state import State
 
 from commonroad_reach.data_structure.configuration_builder import ConfigurationBuilder
 from commonroad_reach.data_structure.reach.reach_interface import ReachableSetInterface
 from commonroad_reach.utility import visualization as util_visual
 
@@ -76,21 +77,16 @@
             target_state.orientation
         )
         self.reach_config.planning_problem.initial_state.time_step = (
             target_state.time_step
         )
 
     def compute(self, time_step: int = 0, vehicle_id=None, verbose: bool = True):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         self.ttc = self.ttc_object.compute(time_step)
         if self.ttc == 0:
             self.value = -math.inf
         elif self.ttc == math.inf:
             self.value = math.inf
         else:
             self.value = self.binary_search(time_step)
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/velocity/cs.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/velocity/cs.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/measure/velocity/delta_v.py` & `commonroad_crime-0.4.0/commonroad_crime/measure/velocity/delta_v.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 import numpy as np
 from typing import Union
 import logging
@@ -32,21 +32,16 @@
 
     def __init__(self, config: CriMeConfiguration):
         super(DeltaV, self).__init__(config)
 
     def compute(
         self, time_step: int, vehicle_id: Union[int, None], verbose: bool = True
     ):
-        utils_log.print_and_log_info(
-            logger,
-            f"* Computing the {self.measure_name} at time step {time_step}",
-            verbose,
-        )
-        self.set_other_vehicles(vehicle_id)
-        self.time_step = time_step
+        if not self.validate_update_states_log(vehicle_id, time_step, verbose):
+            return np.nan
         m_ego = self.configuration.vehicle.dynamic.parameters.m
         if self.configuration.velocity.m_b:
             m_b = self.configuration.velocity.m_b
         else:
             # assume that the vehicle b has the same mass as the ego vehicle
             m_b = m_ego
         if self.ego_vehicle.state_at_time(
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/utility/batch_evaluation.py` & `commonroad_crime-0.4.0/commonroad_crime/utility/batch_evaluation.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/utility/general.py` & `commonroad_crime-0.4.0/commonroad_crime/utility/general.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.2"
+__version__ = "0.3.4"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 from commonroad.scenario.lanelet import LaneletNetwork
 from commonroad.scenario.state import (
     State,
@@ -95,36 +95,40 @@
 
 def check_in_same_lanelet(
     lanelet_network: LaneletNetwork,
     vehicle_1: DynamicObstacle,
     vehicle_2: Union[DynamicObstacle, StaticObstacle],
     time_step: int,
 ):
-    if not vehicle_1.occupancy_at_time(time_step):
-        logger.info(
-            f"<utility> vehicle {vehicle_1.obstacle_id} doesn't have occupancies at time step {time_step}."
-        )
-        return False
-
-    if not vehicle_2.occupancy_at_time(time_step):
-        logger.info(
-            f"<utility> vehicle {vehicle_2.obstacle_id} doesn't have occupancies at time step {time_step}."
-        )
-        return False
-
-    # Proceed only if both vehicles have occupancies
-    lanelets_1 = lanelet_network.find_lanelet_by_shape(
-        vehicle_1.occupancy_at_time(time_step).shape
-    )
-    lanelets_2 = lanelet_network.find_lanelet_by_shape(
-        vehicle_2.occupancy_at_time(time_step).shape
-    )
+    # Helper function to get occupied lanelets along with their predecessors and successors
+    def get_occupied_lanelets(vehicle):
+        occupancy = vehicle.occupancy_at_time(time_step)
+        if not occupancy:
+            logger.info(
+                f"<utility> vehicle {vehicle.obstacle_id} doesn't have occupancies at time step {time_step}."
+            )
+            return set()
+
+        occupied_lanelets = set(lanelet_network.find_lanelet_by_shape(occupancy.shape))
+        for ll in list(
+            occupied_lanelets
+        ):  # Use a list copy to iterate over as we modify the set
+            occupied_lanelets.update(
+                lanelet_network.find_lanelet_by_id(ll).predecessor or []
+            )
+            occupied_lanelets.update(
+                lanelet_network.find_lanelet_by_id(ll).successor or []
+            )
+        return occupied_lanelets
+
+    lanelets_1 = get_occupied_lanelets(vehicle_1)
+    lanelets_2 = get_occupied_lanelets(vehicle_2)
 
-    # Check if there is an intersection between the sets of lanelets occupied by the vehicles
-    return len(set(lanelets_1).intersection(lanelets_2)) > 0
+    # Return True if there is any overlap between the sets of lanelets occupied by the two vehicles
+    return not lanelets_1.isdisjoint(lanelets_2)
 
 
 def check_elements_state_list(
     state_list: List[
         Union[LongitudinalState, KSState, CustomState, PMState, State, None]
     ],
     dt: float,
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/utility/logger.py` & `commonroad_crime-0.4.0/commonroad_crime/utility/logger.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/utility/optimization.py` & `commonroad_crime-0.4.0/commonroad_crime/utility/optimization.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/utility/simulation.py` & `commonroad_crime-0.4.0/commonroad_crime/utility/simulation.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/commonroad_crime/utility/solver.py` & `commonroad_crime-0.4.0/commonroad_crime/utility/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 from typing import Tuple, Union
 import numpy as np
 import logging
 import math
+from functools import lru_cache
 from shapely.geometry import Polygon
 from scipy.spatial.distance import cdist
 
+from commonroad.geometry.shape import Circle, Rectangle
+
 from commonroad.scenario.obstacle import (
     Obstacle,
     StaticObstacle,
     ObstacleType,
     DynamicObstacle,
 )
 from commonroad.scenario.state import State
@@ -120,14 +123,15 @@
     """
     Computes the closest coordinate from a list of points
     """
     vertices = resample_polyline(vertices)
     return vertices[np.argmin(cdist(np.array([state.position]), vertices, "euclidean"))]
 
 
+@lru_cache(maxsize=None)
 def compute_disc_radius_and_distance(
     length: float, width: float
 ) -> Tuple[float, float]:
     """
     Computes the radius of discs and their distances used as the approximation of the shape of the ego vehicle.
     """
     assert (
@@ -352,17 +356,26 @@
     :param l_back: extended length to the back, measured from the center
     :return: shapely-polygon of the obstacle
     """
     pos = obstacle.state_at_time(time_step).position
     angle = obstacle.state_at_time(time_step).orientation
     angle_cos = math.cos(angle)
     angle_sin = math.sin(angle)
-    width = max(obstacle.obstacle_shape.width * 0.5, w)
-    length_front = max(obstacle.obstacle_shape.length * 0.5, l_front)
-    length_back = max(obstacle.obstacle_shape.length * 0.5, l_back)
+    if isinstance(obstacle.obstacle_shape, Circle):
+        width_obs = length_obs = obstacle.obstacle_shape.radius * 2
+    elif isinstance(obstacle.obstacle_shape, Rectangle):
+        width_obs = obstacle.obstacle_shape.width
+        length_obs = obstacle.obstacle_shape.length
+    else:
+        raise ValueError(
+            f"<Criticality/Solver>: obstacle shape {type(obstacle.obstacle_shape).__name__} not supported."
+        )
+    width = max(width_obs * 0.5, w)
+    length_front = max(length_obs * 0.5, l_front)
+    length_back = max(length_obs * 0.5, l_back)
     coords = [
         (
             pos[0] + length_front * angle_cos - width * angle_sin,
             pos[1] + length_front * angle_sin + width * angle_cos,
         ),
         (
             pos[0] - length_back * angle_cos - width * angle_sin,
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime/utility/visualization.py` & `commonroad_crime-0.4.0/commonroad_crime/utility/visualization.py`

 * *Files 15% similar despite different names*

```diff
@@ -240,15 +240,71 @@
                     time_list.append(time_step)
             if nr_metrics == 1:
                 ax = axs
             elif nr_row == 1:
                 ax = axs[count_column]
             else:
                 ax = axs[count_row, count_column]
-            ax.plot(time_list, criticality_list)
+
+            # Create a mask to filter out NaN and infinity values
+            criticality_list = np.array(criticality_list)
+
+            # Apply the mask and find the maximum value among the remaining elements
+            if np.any(np.isinf(criticality_list)):
+                mask = ~np.isnan(criticality_list) & ~np.isinf(criticality_list)
+
+                if len(criticality_list[mask]) > 0:
+                    max_value = np.max(criticality_list[mask]) + 10
+                    min_value = np.min(criticality_list[mask]) - 10
+                else:
+                    max_value = 10
+                    min_value = 10
+
+                # First, replace np.inf with 1000
+                criticality_list_clean = np.where(
+                    criticality_list == np.inf, max_value, criticality_list
+                )
+
+                # Then, replace -np.inf with -1000
+                criticality_list_clean = np.where(
+                    criticality_list_clean == -np.inf, min_value, criticality_list_clean
+                )
+
+                ax.plot(time_list, criticality_list_clean)
+            else:
+                max_value = np.nanmax(criticality_list)
+                min_value = np.nanmin(criticality_list)
+                ax.plot(time_list, criticality_list)
+
+            # Customize y-axis
+            ticks, _ = plt.yticks()
+            # Update ticks and labels
+            new_ticks = [
+                tick for tick in ticks if min_value <= tick <= max_value
+            ]  # Keep ticks within the finite range
+            new_labels = [
+                "{:.4g}".format(tick) for tick in new_ticks
+            ]  # Limit to 4 significant digits
+
+            # Check for infinities and add custom labels
+            if np.any(np.isposinf(criticality_list)):
+                new_ticks.append(
+                    max_value
+                )  # Place at max finite value or a predefined position
+                new_labels.append("inf")
+
+            if np.any(np.isneginf(criticality_list)):
+                new_ticks = [
+                    min_value
+                ] + new_ticks  # Place at min finite value or a predefined position
+                new_labels = ["-inf"] + new_labels
+
+            # Apply the updated ticks and labels to the plot
+            plt.yticks(new_ticks, new_labels)
+
             ax.axis(xmin=time_list[0], xmax=time_list[-1])
             ax.title.set_text(measure.measure_name.value)
 
             if measure.monotone == TypeMonotone.NEG:
                 ax.invert_yaxis()
             count_column += 1
             if count_column > nr_per_row - 1:
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime.egg-info/PKG-INFO` & `commonroad_crime-0.4.0/commonroad_crime.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 636f 6d6d  : 2.1.Name: comm
 00000020: 6f6e 726f 6164 2d63 7269 6d65 0a56 6572  onroad-crime.Ver
-00000030: 7369 6f6e 3a20 302e 332e 330a 5375 6d6d  sion: 0.3.3.Summ
+00000030: 7369 6f6e 3a20 302e 342e 300a 5375 6d6d  sion: 0.4.0.Summ
 00000040: 6172 793a 2063 7269 7469 6361 6c69 7479  ary: criticality
 00000050: 206d 6561 7375 7265 7320 6f66 2061 7574   measures of aut
 00000060: 6f6d 6174 6564 2076 6568 6963 6c65 730a  omated vehicles.
 00000070: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
 00000080: 3a2f 2f63 6f6d 6d6f 6e72 6f61 642e 696e  ://commonroad.in
 00000090: 2e74 756d 2e64 652f 746f 6f6c 732f 636f  .tum.de/tools/co
 000000a0: 6d6d 6f6e 726f 6164 2d63 7269 6d65 0a41  mmonroad-crime.A
@@ -15,381 +15,412 @@
 000000e0: 696c 3a20 636f 6d6d 6f6e 726f 6164 406c  il: commonroad@l
 000000f0: 6973 7473 2e6c 727a 2e64 650a 4c69 6365  ists.lrz.de.Lice
 00000100: 6e73 653a 2042 5344 2033 2d43 6c61 7573  nse: BSD 3-Claus
 00000110: 650a 5072 6f6a 6563 742d 5552 4c3a 2044  e.Project-URL: D
 00000120: 6f63 756d 656e 7461 7469 6f6e 2c20 6874  ocumentation, ht
 00000130: 7470 733a 2f2f 6370 732e 7061 6765 732e  tps://cps.pages.
 00000140: 6769 746c 6162 2e6c 727a 2e64 652f 636f  gitlab.lrz.de/co
-00000150: 6d6d 6f6e 726f 6164 2d63 7269 7469 6361  mmonroad-critica
-00000160: 6c69 7479 2d6d 6561 7375 7265 732f 0a50  lity-measures/.P
-00000170: 726f 6a65 6374 2d55 524c 3a20 466f 7275  roject-URL: Foru
-00000180: 6d2c 2068 7474 7073 3a2f 2f63 6f6d 6d6f  m, https://commo
-00000190: 6e72 6f61 642e 696e 2e74 756d 2e64 652f  nroad.in.tum.de/
-000001a0: 666f 7275 6d2f 632f 636f 6d6d 6f6e 726f  forum/c/commonro
-000001b0: 6164 2d63 7269 6d65 2f32 300a 5072 6f6a  ad-crime/20.Proj
-000001c0: 6563 742d 5552 4c3a 2053 6f75 7263 652c  ect-URL: Source,
-000001d0: 2068 7474 7073 3a2f 2f67 6974 6c61 622e   https://gitlab.
-000001e0: 6c72 7a2e 6465 2f74 756d 2d63 7073 2f63  lrz.de/tum-cps/c
-000001f0: 6f6d 6d6f 6e72 6f61 642d 6372 696d 650a  ommonroad-crime.
-00000200: 4b65 7977 6f72 6473 3a20 6372 6974 6963  Keywords: critic
-00000210: 616c 6974 792c 6175 746f 6e6f 6d6f 7573  ality,autonomous
-00000220: 2064 7269 7669 6e67 0a43 6c61 7373 6966   driving.Classif
-00000230: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000240: 204c 616e 6775 6167 6520 3a3a 2043 2b2b   Language :: C++
-00000250: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
-00000260: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000270: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000280: 2e38 0a43 6c61 7373 6966 6965 723a 2050  .8.Classifier: P
-00000290: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002b0: 2033 2e39 0a43 6c61 7373 6966 6965 723a   3.9.Classifier:
-000002c0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000002d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002e0: 3a3a 2033 2e31 300a 436c 6173 7369 6669  :: 3.10.Classifi
-000002f0: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
-00000300: 5349 2041 7070 726f 7665 6420 3a3a 2042  SI Approved :: B
-00000310: 5344 204c 6963 656e 7365 0a43 6c61 7373  SD License.Class
-00000320: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
-00000330: 2053 7973 7465 6d20 3a3a 2050 4f53 4958   System :: POSIX
-00000340: 203a 3a20 4c69 6e75 780a 4465 7363 7269   :: Linux.Descri
-00000350: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000360: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000370: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
-00000380: 4c49 4345 4e53 450a 5265 7175 6972 6573  LICENSE.Requires
-00000390: 2d44 6973 743a 2063 6f6d 6d6f 6e72 6f61  -Dist: commonroa
-000003a0: 642d 696f 3e3d 3230 3233 2e34 0a52 6571  d-io>=2023.4.Req
-000003b0: 7569 7265 732d 4469 7374 3a20 636f 6d6d  uires-Dist: comm
-000003c0: 6f6e 726f 6164 2d76 6568 6963 6c65 2d6d  onroad-vehicle-m
-000003d0: 6f64 656c 733e 3d33 2e30 2e30 0a52 6571  odels>=3.0.0.Req
-000003e0: 7569 7265 732d 4469 7374 3a20 636f 6d6d  uires-Dist: comm
-000003f0: 6f6e 726f 6164 2d72 6f75 7465 2d70 6c61  onroad-route-pla
-00000400: 6e6e 6572 3c32 3032 342e 312c 3e3d 3230  nner<2024.1,>=20
-00000410: 3232 2e33 0a52 6571 7569 7265 732d 4469  22.3.Requires-Di
-00000420: 7374 3a20 636f 6d6d 6f6e 726f 6164 2d64  st: commonroad-d
-00000430: 7269 7661 6269 6c69 7479 2d63 6865 636b  rivability-check
-00000440: 6572 3e3d 3230 3233 2e31 0a52 6571 7569  er>=2023.1.Requi
-00000450: 7265 732d 4469 7374 3a20 636f 6d6d 6f6e  res-Dist: common
-00000460: 726f 6164 2d72 6561 6368 3e3d 3230 3233  road-reach>=2023
-00000470: 2e31 0a52 6571 7569 7265 732d 4469 7374  .1.Requires-Dist
-00000480: 3a20 6d61 7470 6c6f 746c 6962 3e3d 332e  : matplotlib>=3.
-00000490: 352e 320a 5265 7175 6972 6573 2d44 6973  5.2.Requires-Dis
-000004a0: 743a 206e 756d 7079 3e3d 312e 3139 2e30  t: numpy>=1.19.0
-000004b0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000004c0: 7363 6970 793e 3d31 2e37 2e33 0a52 6571  scipy>=1.7.3.Req
-000004d0: 7569 7265 732d 4469 7374 3a20 7368 6170  uires-Dist: shap
-000004e0: 656c 793c 332e 302e 302c 3e3d 322e 302e  ely<3.0.0,>=2.0.
-000004f0: 310a 5265 7175 6972 6573 2d44 6973 743a  1.Requires-Dist:
-00000500: 206f 6d65 6761 636f 6e66 3e3d 322e 312e   omegaconf>=2.1.
-00000510: 310a 5265 7175 6972 6573 2d44 6973 743a  1.Requires-Dist:
-00000520: 2063 6173 6164 693e 3d33 2e36 2e33 0a52   casadi>=3.6.3.R
-00000530: 6571 7569 7265 732d 4469 7374 3a20 7471  equires-Dist: tq
-00000540: 646d 3e3d 342e 3635 2e30 0a52 6571 7569  dm>=4.65.0.Requi
-00000550: 7265 732d 4469 7374 3a20 696d 6167 6569  res-Dist: imagei
-00000560: 6f3e 3d32 2e39 2e30 0a52 6571 7569 7265  o>=2.9.0.Require
-00000570: 732d 4469 7374 3a20 7079 7465 7374 3e3d  s-Dist: pytest>=
-00000580: 372e 342e 300a 0a23 2043 6f6d 6d6f 6e52  7.4.0..# CommonR
-00000590: 6f61 642d 4372 694d 650a 215b 696d 6167  oad-CriMe.![imag
-000005a0: 6520 696e 666f 5d28 6874 7470 733a 2f2f  e info](https://
-000005b0: 6769 746c 6162 2e6c 727a 2e64 652f 7475  gitlab.lrz.de/tu
-000005c0: 6d2d 6370 732f 636f 6d6d 6f6e 726f 6164  m-cps/commonroad
-000005d0: 2d63 7269 6d65 2f2d 2f72 6177 2f6d 6173  -crime/-/raw/mas
-000005e0: 7465 722f 646f 6373 2f66 6967 7572 6573  ter/docs/figures
-000005f0: 2f43 7269 4d65 2d62 616e 6e65 722e 706e  /CriMe-banner.pn
-00000600: 6729 0a5b 215b 4c69 6e75 785d 2868 7474  g).[![Linux](htt
-00000610: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000620: 2e69 6f2f 6261 6467 652f 6f73 2d6c 696e  .io/badge/os-lin
-00000630: 7578 3f26 6c6f 676f 3d4c 696e 7578 266c  ux?&logo=Linux&l
-00000640: 6f67 6f43 6f6c 6f72 3d77 6869 7465 266c  ogoColor=white&l
-00000650: 6162 656c 436f 6c6f 723d 6772 6179 295d  abelColor=gray)]
-00000660: 2868 7474 7073 3a2f 2f70 7970 692e 7079  (https://pypi.py
-00000670: 7468 6f6e 2e6f 7267 2f70 7970 692f 636f  thon.org/pypi/co
-00000680: 6d6d 6f6e 726f 6164 2d6f 7065 6e73 6365  mmonroad-opensce
-00000690: 6e61 7269 6f2d 636f 6e76 6572 7465 722f  nario-converter/
-000006a0: 290a 5b21 5b50 7950 4920 7665 7273 696f  ).[![PyPI versio
-000006b0: 6e20 6675 7279 2e69 6f5d 2868 7474 7073  n fury.io](https
-000006c0: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
-000006d0: 2f70 792f 636f 6d6d 6f6e 726f 6164 2d63  /py/commonroad-c
-000006e0: 7269 6d65 2e73 7667 3f73 7479 6c65 3d70  rime.svg?style=p
-000006f0: 6c61 7374 6963 295d 2868 7474 7073 3a2f  lastic)](https:/
-00000700: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
-00000710: 2f70 7970 692f 636f 6d6d 6f6e 726f 6164  /pypi/commonroad
-00000720: 2d63 7269 6d65 2f29 0a5b 215b 5079 5049  -crime/).[![PyPI
-00000730: 206c 6963 656e 7365 5d28 6874 7470 733a   license](https:
-00000740: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000750: 2f70 7970 692f 6c2f 636f 6d6d 6f6e 726f  /pypi/l/commonro
-00000760: 6164 2d63 7269 6d65 2e73 7667 3f73 7479  ad-crime.svg?sty
-00000770: 6c65 3d70 6c61 7374 6963 295d 2868 7474  le=plastic)](htt
-00000780: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
-00000790: 2e6f 7267 2f70 7970 692f 636f 6d6d 6f6e  .org/pypi/common
-000007a0: 726f 6164 2d63 7269 6d65 2f29 3c62 723e  road-crime/)<br>
-000007b0: 0a5b 215b 5079 5049 2064 6f77 6e6c 6f61  .[![PyPI downloa
-000007c0: 6420 6d6f 6e74 685d 2868 7474 7073 3a2f  d month](https:/
-000007d0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000007e0: 7079 7069 2f64 6d2f 636f 6d6d 6f6e 726f  pypi/dm/commonro
-000007f0: 6164 2d63 7269 6d65 2e73 7667 3f73 7479  ad-crime.svg?sty
-00000800: 6c65 3d70 6c61 7374 6963 266c 6162 656c  le=plastic&label
-00000810: 3d50 7950 4925 3230 646f 776e 6c6f 6164  =PyPI%20download
-00000820: 7329 5d28 6874 7470 733a 2f2f 7079 7069  s)](https://pypi
-00000830: 2e70 7974 686f 6e2e 6f72 672f 7079 7069  .python.org/pypi
-00000840: 2f63 6f6d 6d6f 6e72 6f61 642d 6372 696d  /commonroad-crim
-00000850: 652f 2920 0a5b 215b 5079 5049 2064 6f77  e/) .[![PyPI dow
-00000860: 6e6c 6f61 6420 7765 656b 5d28 6874 7470  nload week](http
-00000870: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000880: 696f 2f70 7970 692f 6477 2f63 6f6d 6d6f  io/pypi/dw/commo
-00000890: 6e72 6f61 642d 6372 696d 652e 7376 673f  nroad-crime.svg?
-000008a0: 7374 796c 653d 706c 6173 7469 6326 6c61  style=plastic&la
-000008b0: 6265 6c3d 5079 5049 2532 3064 6f77 6e6c  bel=PyPI%20downl
-000008c0: 6f61 6473 295d 2868 7474 7073 3a2f 2f70  oads)](https://p
-000008d0: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
-000008e0: 7970 692f 636f 6d6d 6f6e 726f 6164 2d63  ypi/commonroad-c
-000008f0: 7269 6d65 2f29 3c62 723e 0a0a 546f 6f6c  rime/)<br>..Tool
-00000900: 626f 7820 746f 2063 6f6d 7075 7465 202a  box to compute *
-00000910: 2a43 7269 2a2a 7469 6361 6c69 7479 202a  *Cri**ticality *
-00000920: 2a4d 652a 2a61 7375 7265 7320 0a28 652e  *Me**asures .(e.
-00000930: 672e 2074 696d 652d 746f 2d63 6f6c 6c69  g. time-to-colli
-00000940: 7369 6f6e 2c20 7469 6d65 2d74 6f2d 7265  sion, time-to-re
-00000950: 6163 742c 2e2e 2e29 2e20 5375 6368 206d  act,...). Such m
-00000960: 6561 7375 7265 730a 6361 6e20 6265 2075  easures.can be u
-00000970: 7365 6420 746f 2074 7269 6767 6572 2077  sed to trigger w
-00000980: 6172 6e69 6e67 7320 616e 6420 656d 6572  arnings and emer
-00000990: 6765 6e63 7920 6d61 6e65 7576 6572 7320  gency maneuvers 
-000009a0: 0a69 6e20 6472 6976 6572 2061 7373 6973  .in driver assis
-000009b0: 7461 6e63 6520 7379 7374 656d 7320 6f72  tance systems or
-000009c0: 2072 6570 6169 7220 616e 2069 6e66 6561   repair an infea
-000009d0: 7369 626c 6520 0a74 7261 6a65 6374 6f72  sible .trajector
-000009e0: 792e 200a 0a2d 2049 6620 796f 7520 6861  y. ..- If you ha
-000009f0: 7665 2071 7565 7374 696f 6e73 206f 7220  ve questions or 
-00000a00: 7761 6e74 2074 6f20 7265 706f 7274 2070  want to report p
-00000a10: 726f 626c 656d 7320 6f72 2073 7567 6765  roblems or sugge
-00000a20: 7374 696f 6e73 2c20 706c 6561 7365 2073  stions, please s
-00000a30: 7461 7274 2061 205b 4769 7468 7562 2064  tart a [Github d
-00000a40: 6973 6375 7373 696f 6e5d 2868 7474 7073  iscussion](https
-00000a50: 3a2f 2f67 6974 6875 622e 636f 6d2f 6f72  ://github.com/or
-00000a60: 6773 2f43 6f6d 6d6f 6e52 6f61 642f 6469  gs/CommonRoad/di
-00000a70: 7363 7573 7369 6f6e 7329 2e20 0a0a 2323  scussions). ..##
-00000a80: 2320 f09f 9aa7 2057 6520 4d65 6173 7572  # .... We Measur
-00000a90: 6520 f09d 95ae 6f6d 6d6f 6e20 f09d 95bd  e ....ommon ....
-00000aa0: 6f61 6420 f09d 95ae 7269 f09d 95b8 6521  oad ....ri....e!
-00000ab0: 20f0 9f9a 940a 0a0a 2323 2049 6e73 7461   .......## Insta
-00000ac0: 6c6c 6174 696f 6e20 4775 6964 650a 0a60  llation Guide..`
-00000ad0: 636f 6d6d 6f6e 726f 6164 2d63 7269 6d65  commonroad-crime
-00000ae0: 6020 6361 6e20 6265 2069 6e73 7461 6c6c  ` can be install
-00000af0: 6564 2077 6974 683a 0a0a 6060 6020 6261  ed with:..``` ba
-00000b00: 7368 0a24 2070 6970 2069 6e73 7461 6c6c  sh.$ pip install
-00000b10: 2063 6f6d 6d6f 6e72 6f61 642d 6372 696d   commonroad-crim
-00000b20: 650a 6060 600a 466f 7220 6164 6469 6e67  e.```.For adding
-00000b30: 206e 6577 206d 6561 7375 7265 732c 2077   new measures, w
-00000b40: 6520 7265 636f 6d6d 656e 6420 7573 696e  e recommend usin
-00000b50: 6720 5b41 6e61 636f 6e64 615d 2868 7474  g [Anaconda](htt
-00000b60: 7073 3a2f 2f77 7777 2e61 6e61 636f 6e64  ps://www.anacond
-00000b70: 612e 636f 6d2f 2920 746f 206d 616e 6167  a.com/) to manag
-00000b80: 6520 796f 7572 2065 6e76 6972 6f6e 6d65  e your environme
-00000b90: 6e74 2073 6f20 7468 6174 2065 7665 6e20  nt so that even 
-00000ba0: 6966 2079 6f75 206d 6573 7320 736f 6d65  if you mess some
-00000bb0: 7468 696e 6720 7570 2c20 796f 7520 6361  thing up, you ca
-00000bc0: 6e20 616c 7761 7973 2068 6176 6520 6120  n always have a 
-00000bd0: 7361 6665 2061 6e64 2063 6c65 616e 2072  safe and clean r
-00000be0: 6573 7461 7274 2e20 4120 6775 6964 6520  estart. A guide 
-00000bf0: 666f 7220 6d61 6e61 6769 6e67 2070 7974  for managing pyt
-00000c00: 686f 6e20 656e 7669 726f 6e6d 656e 7473  hon environments
-00000c10: 2077 6974 6820 416e 6163 6f6e 6461 2063   with Anaconda c
-00000c20: 616e 2062 6520 666f 756e 6420 5b68 6572  an be found [her
-00000c30: 655d 2868 7474 7073 3a2f 2f63 6f6e 6461  e](https://conda
-00000c40: 2e69 6f2f 7072 6f6a 6563 7473 2f63 6f6e  .io/projects/con
-00000c50: 6461 2f65 6e2f 6c61 7465 7374 2f75 7365  da/en/latest/use
-00000c60: 722d 6775 6964 652f 7461 736b 732f 6d61  r-guide/tasks/ma
-00000c70: 6e61 6765 2d65 6e76 6972 6f6e 6d65 6e74  nage-environment
-00000c80: 732e 6874 6d6c 292e 0a0a 4166 7465 7220  s.html)...After 
-00000c90: 696e 7374 616c 6c69 6e67 2041 6e61 636f  installing Anaco
-00000ca0: 6e64 612c 2063 7265 6174 6520 6120 6e65  nda, create a ne
-00000cb0: 7720 656e 7669 726f 6e6d 656e 7420 7769  w environment wi
-00000cc0: 7468 3a0a 6060 6020 6261 7368 0a24 2063  th:.``` bash.$ c
-00000cd0: 6f6e 6461 2063 7265 6174 6520 2d6e 2063  onda create -n c
-00000ce0: 6f6d 6d6f 6e72 6f61 642d 7079 3338 2070  ommonroad-py38 p
-00000cf0: 7974 686f 6e3d 332e 3820 2d79 0a60 6060  ython=3.8 -y.```
-00000d00: 0a0a 4865 7265 2074 6865 206e 616d 6520  ..Here the name 
-00000d10: 6f66 2074 6865 2065 6e76 6972 6f6e 6d65  of the environme
-00000d20: 6e74 2069 7320 6361 6c6c 6564 202a 2a63  nt is called **c
-00000d30: 6f6d 6d6f 6e72 6f61 642d 7079 3338 2a2a  ommonroad-py38**
-00000d40: 2e20 596f 7520 6d61 7920 616c 736f 2063  . You may also c
-00000d50: 6861 6e67 6520 7468 6973 206e 616d 6520  hange this name 
-00000d60: 6173 2079 6f75 2077 6973 682e 2049 6e20  as you wish. In 
-00000d70: 7375 6368 2063 6173 652c 2064 6f6e 2774  such case, don't
-00000d80: 2066 6f72 6765 7420 746f 2063 6861 6e67   forget to chang
-00000d90: 6520 6974 2069 6e20 7468 6520 666f 6c6c  e it in the foll
-00000da0: 6f77 696e 6720 636f 6d6d 616e 6473 2061  owing commands a
-00000db0: 7320 7765 6c6c 2e20 2a2a 416c 7761 7973  s well. **Always
-00000dc0: 2061 6374 6976 6174 652a 2a20 7468 6973   activate** this
-00000dd0: 2065 6e76 6972 6f6e 6d65 6e74 2062 6566   environment bef
-00000de0: 6f72 6520 796f 7520 646f 2061 6e79 7468  ore you do anyth
-00000df0: 696e 6720 7265 6c61 7465 643a 0a0a 6060  ing related:..``
-00000e00: 6073 680a 2420 636f 6e64 6120 6163 7469  `sh.$ conda acti
-00000e10: 7661 7465 2063 6f6d 6d6f 6e72 6f61 642d  vate commonroad-
-00000e20: 7079 3338 0a6f 720a 2420 736f 7572 6365  py38.or.$ source
-00000e30: 2061 6374 6976 6174 6520 636f 6d6d 6f6e   activate common
-00000e40: 726f 6164 2d70 7933 380a 6060 600a 5468  road-py38.```.Th
-00000e50: 656e 2c20 696e 7374 616c 6c20 7468 6520  en, install the 
-00000e60: 6465 7065 6e64 656e 6369 6573 2077 6974  dependencies wit
-00000e70: 683a 0a0a 6060 6073 680a 2420 6364 203c  h:..```sh.$ cd <
-00000e80: 7061 7468 2d74 6f2d 7468 6973 2d72 6570  path-to-this-rep
-00000e90: 6f3e 0a24 2070 6970 2069 6e73 7461 6c6c  o>.$ pip install
-00000ea0: 202d 6520 2e0a 2420 636f 6e64 6120 6465   -e ..$ conda de
-00000eb0: 7665 6c6f 7020 2e0a 6060 600a 0a54 6f20  velop ..```..To 
-00000ec0: 7465 7374 2074 6865 2069 6e73 7461 6c6c  test the install
-00000ed0: 6974 696f 6e2c 2072 756e 2075 6e69 7474  ition, run unitt
-00000ee0: 6573 743a 0a60 6060 6261 7368 0a24 2063  est:.```bash.$ c
-00000ef0: 6420 7465 7374 730a 2420 7079 7468 6f6e  d tests.$ python
-00000f00: 202d 6d20 756e 6974 7465 7374 202d 760a   -m unittest -v.
-00000f10: 6060 600a 0a0a 546f 2067 6574 2073 7461  ```...To get sta
-00000f20: 7274 6564 2079 6f75 7220 6a6f 7572 6e65  rted your journe
-00000f30: 7920 7769 7468 206f 7572 2063 7269 7469  y with our criti
-00000f40: 6361 6c69 7479 206d 6561 7375 7265 732c  cality measures,
-00000f50: 2063 6865 636b 2074 6865 2060 7475 746f   check the `tuto
-00000f60: 7269 616c 7360 2061 6e64 2074 6865 2066  rials` and the f
-00000f70: 6f6c 6c6f 7769 6e67 2074 6970 732e 0a0a  ollowing tips...
-00000f80: 2323 2320 486f 7720 746f 2061 6464 206e  ### How to add n
-00000f90: 6577 2063 7269 7469 6361 6c69 7479 206d  ew criticality m
-00000fa0: 6561 7375 7265 0a31 2e20 6372 6561 7465  easure.1. create
-00000fb0: 2061 206e 6577 2062 7261 6e63 6820 7769   a new branch wi
-00000fc0: 7468 2060 6665 6174 7572 652d 3c6d 6561  th `feature-<mea
-00000fd0: 7375 7265 2d6e 616d 653e 6020 616e 6420  sure-name>` and 
-00000fe0: 6368 6563 6b6f 7574 2074 6865 2062 7261  checkout the bra
-00000ff0: 6e63 680a 322e 206e 6176 6967 6174 6520  nch.2. navigate 
-00001000: 746f 2060 636f 6d6d 6f6e 726f 6164 5f63  to `commonroad_c
-00001010: 7269 6d65 2f64 6174 615f 7374 7275 6374  rime/data_struct
-00001020: 7572 652f 7479 7065 2e70 7960 2074 6f20  ure/type.py` to 
-00001030: 6669 6e64 2074 6865 2063 6f72 7265 6374  find the correct
-00001040: 2063 6174 6567 6f72 7920 6f66 2074 6865   category of the
-00001050: 206d 6561 7375 7265 2061 6e64 2061 6464   measure and add
-00001060: 2061 6e20 0a65 6e75 6d65 7261 7469 6f6e   an .enumeration
-00001070: 2065 6e74 7279 2060 3c61 6262 7265 7669   entry `<abbrevi
-00001080: 6174 696f 6e3e 3a20 3c65 7870 6c61 6e61  ation>: <explana
-00001090: 7469 6f6e 3e60 0a33 2e20 6e61 7669 6761  tion>`.3. naviga
-000010a0: 7465 2074 6f20 6063 6f6d 6d6f 6e72 6f61  te to `commonroa
-000010b0: 645f 6372 696d 652f 6d65 6173 7572 6560  d_crime/measure`
-000010c0: 2074 6f20 6669 6e64 2074 6865 2061 626f   to find the abo
-000010d0: 7665 2d6d 656e 7469 6f6e 6564 2063 6174  ve-mentioned cat
-000010e0: 6567 6f72 7920 616e 6420 6372 6561 7465  egory and create
-000010f0: 2061 2070 7974 686f 6e20 6669 6c65 206e   a python file n
-00001100: 616d 6564 0a60 3c61 6262 7265 7669 6174  amed.`<abbreviat
-00001110: 696f 6e3e 2e70 7960 2e20 5468 656e 2063  ion>.py`. Then c
-00001120: 7265 6174 6520 6120 636c 6173 7320 696e  reate a class in
-00001130: 6865 7269 7469 6e67 2074 6865 2060 4372  heriting the `Cr
-00001140: 694d 6542 6173 6560 2075 6e64 6572 2060  iMeBase` under `
-00001150: 636f 6d6d 6f6e 726f 6164 5f63 7269 6d65  commonroad_crime
-00001160: 2f64 6174 615f 7374 7275 6374 7572 652f  /data_structure/
-00001170: 6261 7365 2e70 7960 0a34 2e20 7369 6d69  base.py`.4. simi
-00001180: 6c61 7220 746f 206f 7468 6572 206d 6561  lar to other mea
-00001190: 7375 7265 732c 2079 6f75 206e 6565 6420  sures, you need 
-000011a0: 746f 2069 6d70 6c65 6d65 6e74 2074 6865  to implement the
-000011b0: 2060 636f 6d70 7574 6528 2960 2061 6e64   `compute()` and
-000011c0: 2060 7669 7375 616c 697a 6528 2960 2066   `visualize()` f
-000011d0: 756e 6374 696f 6e73 0a0a 2323 2320 486f  unctions..### Ho
-000011e0: 7720 746f 2064 6566 696e 6520 636f 6e66  w to define conf
-000011f0: 6967 7572 6174 696f 6e20 7061 7261 6d65  iguration parame
-00001200: 7465 7273 206f 6620 7468 6520 6d65 6173  ters of the meas
-00001210: 7572 650a 312e 206e 6176 6967 6174 6520  ure.1. navigate 
-00001220: 746f 2060 636f 6d6d 6f6e 726f 6164 5f63  to `commonroad_c
-00001230: 7269 6d65 2f64 6174 615f 7374 7275 6374  rime/data_struct
-00001240: 7572 652f 636f 6e66 6967 7561 7469 6f6e  ure/configuation
-00001250: 2e70 7960 2074 6f20 6669 6e64 2074 6865  .py` to find the
-00001260: 2061 626f 7665 2d6d 656e 7469 6f6e 6564   above-mentioned
-00001270: 2063 6174 6567 6f72 7920 616e 6420 6164   category and ad
-00001280: 6420 6120 6e65 7720 0a69 6e73 7461 6e63  d a new .instanc
-00001290: 6520 746f 2074 6865 2063 6c61 7373 2061  e to the class a
-000012a0: 7320 6073 656c 662e 3c70 6172 616d 6574  s `self.<paramet
-000012b0: 6572 3e20 3d20 636f 6e66 6967 5f72 656c  er> = config_rel
-000012c0: 6576 616e 742e 3c70 6172 616d 6574 6572  evant.<parameter
-000012d0: 3e60 0a32 2e20 796f 7520 6361 6e20 7468  >`.2. you can th
-000012e0: 656e 2064 6972 6563 746c 7920 6361 6c6c  en directly call
-000012f0: 2074 6865 2076 616c 7565 7320 7573 696e   the values usin
-00001300: 6720 6073 656c 662e 636f 6e66 6967 7572  g `self.configur
-00001310: 6174 696f 6e2e 3c63 6174 6567 6f72 793e  ation.<category>
-00001320: 2e3c 7061 7261 6d65 7465 723e 6020 696e  .<parameter>` in
-00001330: 2079 6f75 7220 6d65 6173 7572 6520 636c   your measure cl
-00001340: 6173 730a 332e 2074 6f20 6f76 6572 7269  ass.3. to overri
-00001350: 6465 2074 6865 2064 6566 6175 6c74 2070  de the default p
-00001360: 6172 616d 6574 6572 2076 616c 7565 732c  arameter values,
-00001370: 2063 7265 6174 6520 6120 6079 616d 6c60   create a `yaml`
-00001380: 2066 696c 6520 286e 616d 6520 6974 2074   file (name it t
-00001390: 6865 2073 616d 6520 6173 2074 6865 2073  he same as the s
-000013a0: 6365 6e61 7269 6f29 2069 6e20 602e 2f63  cenario) in `./c
-000013b0: 6f6e 6669 675f 6669 6c65 7360 2061 6e64  onfig_files` and
-000013c0: 206d 6f64 6966 7920 7468 6520 7661 6c75   modify the valu
-000013d0: 6573 2074 6865 7265 0a23 2320 446f 6375  es there.## Docu
-000013e0: 6d65 6e74 6174 696f 6e0a 0a54 6865 2064  mentation..The d
-000013f0: 6f63 756d 656e 7461 7469 6f6e 206f 6620  ocumentation of 
-00001400: 6f75 7220 746f 6f6c 626f 7820 6973 2061  our toolbox is a
-00001410: 7661 696c 6162 6c65 206f 6e20 6f75 7220  vailable on our 
-00001420: 7765 6273 6974 653a 2068 7474 7073 3a2f  website: https:/
-00001430: 2f63 7073 2e70 6167 6573 2e67 6974 6c61  /cps.pages.gitla
-00001440: 622e 6c72 7a2e 6465 2f63 6f6d 6d6f 6e72  b.lrz.de/commonr
-00001450: 6f61 642f 636f 6d6d 6f6e 726f 6164 2d63  oad/commonroad-c
-00001460: 7269 7469 6361 6c69 7479 2d6d 6561 7375  riticality-measu
-00001470: 7265 732f 2e0a 0a49 6e20 6f72 6465 7220  res/...In order 
-00001480: 746f 2067 656e 6572 6174 6520 7468 6520  to generate the 
-00001490: 646f 6375 6d65 6e74 6174 696f 6e20 7669  documentation vi
-000014a0: 6120 5370 6869 6e78 206c 6f63 616c 6c79  a Sphinx locally
-000014b0: 2c20 7275 6e20 7468 6520 666f 6c6c 6f77  , run the follow
-000014c0: 696e 6720 636f 6d6d 616e 6473 2069 6e20  ing commands in 
-000014d0: 7468 6520 726f 6f74 2064 6972 6563 746f  the root directo
-000014e0: 7279 3a0a 0a60 6060 6261 7368 0a24 2070  ry:..```bash.$ p
-000014f0: 6970 2069 6e73 7461 6c6c 202d 7220 2e2f  ip install -r ./
-00001500: 646f 6373 2f72 6571 7569 7265 6d65 6e74  docs/requirement
-00001510: 735f 646f 632e 7478 740a 2420 6364 2064  s_doc.txt.$ cd d
-00001520: 6f63 732f 7370 6869 6e78 0a24 206d 616b  ocs/sphinx.$ mak
-00001530: 6520 6874 6d6c 0a60 6060 0a0a 5468 6520  e html.```..The 
-00001540: 646f 6375 6d65 6e74 6174 696f 6e20 6361  documentation ca
-00001550: 6e20 7468 656e 2062 6520 6c61 756e 6368  n then be launch
-00001560: 6564 2062 7920 6272 6f77 7369 6e67 2060  ed by browsing `
-00001570: 602e 2f64 6f63 732f 7370 6869 6e78 2f62  `./docs/sphinx/b
-00001580: 7569 6c64 2f68 746d 6c2f 696e 6465 782e  uild/html/index.
-00001590: 6874 6d6c 2f60 602e 0a0a 2323 2320 436f  html/``...### Co
-000015a0: 6e74 7269 6275 746f 7273 2028 696e 2061  ntributors (in a
-000015b0: 6c70 6861 6265 7469 6361 6c20 6f72 6465  lphabetical orde
-000015c0: 7220 6279 206c 6173 7420 6e61 6d65 290a  r by last name).
-000015d0: 2d20 4c69 6775 6f20 4368 656e 0a2d 2059  - Liguo Chen.- Y
-000015e0: 7561 6e66 6569 204c 696e 0a2d 2053 6562  uanfei Lin.- Seb
-000015f0: 6173 7469 616e 204d 6169 6572 686f 6665  astian Maierhofe
-00001600: 720a 2d20 4976 616e 6120 5065 6e65 7661  r.- Ivana Peneva
-00001610: 0a2d 204b 756e 2051 6961 6e0a 2d20 4f6c  .- Kun Qian.- Ol
-00001620: 6976 6572 2053 7065 6368 740a 2d20 5369  iver Specht.- Si
-00001630: 6368 656e 6720 5761 6e67 0a2d 2059 6f75  cheng Wang.- You
-00001640: 7261 6e20 5761 6e67 0a2d 205a 656b 756e  ran Wang.- Zekun
-00001650: 2058 696e 670a 2d20 5a69 7169 616e 2058   Xing.- Ziqian X
-00001660: 750a 0a23 2323 2043 6974 6174 696f 6e0a  u..### Citation.
-00001670: 4966 2079 6f75 2075 7365 2060 636f 6d6d  If you use `comm
-00001680: 6f6e 726f 6164 2d63 7269 6d65 6020 666f  onroad-crime` fo
-00001690: 7220 6163 6164 656d 6963 2077 6f72 6b2c  r academic work,
-000016a0: 2077 6520 6869 6768 6c79 2065 6e63 6f75   we highly encou
-000016b0: 7261 6765 2079 6f75 2074 6f20 6369 7465  rage you to cite
-000016c0: 206f 7572 2070 6170 6572 3a0a 6060 6074   our paper:.```t
-000016d0: 6578 740a 4049 6e50 726f 6365 6564 696e  ext.@InProceedin
-000016e0: 6773 7b6c 696e 3230 3233 6372 696d 652c  gs{lin2023crime,
-000016f0: 0a20 2020 2020 2074 6974 6c65 2020 2020  .      title    
-00001700: 203d 207b 7b43 6f6d 6d6f 6e52 6f61 642d   = {{CommonRoad-
-00001710: 4372 694d 657d 3a20 7b41 7d20 546f 6f6c  CriMe}: {A} Tool
-00001720: 626f 7820 666f 7220 4372 6974 6963 616c  box for Critical
-00001730: 6974 7920 4d65 6173 7572 6573 206f 6620  ity Measures of 
-00001740: 4175 746f 6e6f 6d6f 7573 2056 6568 6963  Autonomous Vehic
-00001750: 6c65 737d 2c0a 2020 2020 2020 6175 7468  les},.      auth
-00001760: 6f72 2020 2020 3d20 7b59 7561 6e66 6569  or    = {Yuanfei
-00001770: 204c 696e 2061 6e64 204d 6174 7468 6961   Lin and Matthia
-00001780: 7320 416c 7468 6f66 667d 2c0a 2020 2020  s Althoff},.    
-00001790: 2020 626f 6f6b 7469 746c 6520 3d20 7b50    booktitle = {P
-000017a0: 726f 632e 206f 6620 7468 6520 4945 4545  roc. of the IEEE
-000017b0: 2049 6e74 656c 6c2e 2056 6568 2e20 5379   Intell. Veh. Sy
-000017c0: 6d70 2e7d 2c20 2020 2020 0a20 2020 2020  mp.},     .     
-000017d0: 2070 6167 6573 2020 2020 203d 207b 312d   pages     = {1-
-000017e0: 387d 2c20 0a20 2020 2020 2079 6561 7220  8}, .      year 
-000017f0: 2020 2020 203d 207b 3230 3233 7d2c 0a7d       = {2023},.}
-00001800: 0a60 6060 0a49 6620 796f 7520 7573 6520  .```.If you use 
-00001810: 7468 6973 2070 726f 6a65 6374 2773 2063  this project's c
-00001820: 6f64 6520 696e 2069 6e64 7573 7472 792c  ode in industry,
-00001830: 2077 6527 6420 6c6f 7665 2074 6f20 6865   we'd love to he
-00001840: 6172 2066 726f 6d20 796f 7520 6173 2077  ar from you as w
-00001850: 656c 6c3b 200a 6665 656c 2066 7265 6520  ell; .feel free 
-00001860: 746f 2072 6561 6368 206f 7574 2074 6f20  to reach out to 
-00001870: 5b59 7561 6e66 6569 204c 696e 5d28 6d61  [Yuanfei Lin](ma
-00001880: 696c 746f 3a79 7561 6e66 6569 2e6c 696e  ilto:yuanfei.lin
-00001890: 4074 756d 2e64 6529 2064 6972 6563 746c  @tum.de) directl
-000018a0: 792e 0a                                  y..
+00000150: 6d6d 6f6e 726f 6164 2f63 6f6d 6d6f 6e72  mmonroad/commonr
+00000160: 6f61 642d 6372 6974 6963 616c 6974 792d  oad-criticality-
+00000170: 6d65 6173 7572 6573 2f0a 5072 6f6a 6563  measures/.Projec
+00000180: 742d 5552 4c3a 2046 6f72 756d 2c20 6874  t-URL: Forum, ht
+00000190: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000001a0: 2f43 6f6d 6d6f 6e52 6f61 642f 636f 6d6d  /CommonRoad/comm
+000001b0: 6f6e 726f 6164 2d63 7269 6d65 2f69 7373  onroad-crime/iss
+000001c0: 7565 730a 5072 6f6a 6563 742d 5552 4c3a  ues.Project-URL:
+000001d0: 2053 6f75 7263 652c 2068 7474 7073 3a2f   Source, https:/
+000001e0: 2f67 6974 6875 622e 636f 6d2f 436f 6d6d  /github.com/Comm
+000001f0: 6f6e 526f 6164 2f63 6f6d 6d6f 6e72 6f61  onRoad/commonroa
+00000200: 642d 6372 696d 650a 4b65 7977 6f72 6473  d-crime.Keywords
+00000210: 3a20 6372 6974 6963 616c 6974 792c 6175  : criticality,au
+00000220: 746f 6e6f 6d6f 7573 2064 7269 7669 6e67  tonomous driving
+00000230: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000240: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000250: 6520 3a3a 2043 2b2b 0a43 6c61 7373 6966  e :: C++.Classif
+00000260: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000270: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000280: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+00000290: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000002a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002b0: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+000002c0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000002d0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002e0: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+000002f0: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
+00000300: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000310: 7665 6420 3a3a 2042 5344 204c 6963 656e  ved :: BSD Licen
+00000320: 7365 0a43 6c61 7373 6966 6965 723a 204f  se.Classifier: O
+00000330: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000340: 3a3a 2050 4f53 4958 203a 3a20 4c69 6e75  :: POSIX :: Linu
+00000350: 780a 4465 7363 7269 7074 696f 6e2d 436f  x.Description-Co
+00000360: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+00000370: 2f6d 6172 6b64 6f77 6e0a 4c69 6365 6e73  /markdown.Licens
+00000380: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
+00000390: 5265 7175 6972 6573 2d44 6973 743a 2063  Requires-Dist: c
+000003a0: 6f6d 6d6f 6e72 6f61 642d 696f 3e3d 3230  ommonroad-io>=20
+000003b0: 3233 2e34 0a52 6571 7569 7265 732d 4469  23.4.Requires-Di
+000003c0: 7374 3a20 636f 6d6d 6f6e 726f 6164 2d76  st: commonroad-v
+000003d0: 6568 6963 6c65 2d6d 6f64 656c 733e 3d33  ehicle-models>=3
+000003e0: 2e30 2e30 0a52 6571 7569 7265 732d 4469  .0.0.Requires-Di
+000003f0: 7374 3a20 636f 6d6d 6f6e 726f 6164 2d72  st: commonroad-r
+00000400: 6f75 7465 2d70 6c61 6e6e 6572 3e3d 3230  oute-planner>=20
+00000410: 3234 2e32 2e30 0a52 6571 7569 7265 732d  24.2.0.Requires-
+00000420: 4469 7374 3a20 636f 6d6d 6f6e 726f 6164  Dist: commonroad
+00000430: 2d64 7269 7661 6269 6c69 7479 2d63 6865  -drivability-che
+00000440: 636b 6572 3e3d 3230 3233 2e31 0a52 6571  cker>=2023.1.Req
+00000450: 7569 7265 732d 4469 7374 3a20 636f 6d6d  uires-Dist: comm
+00000460: 6f6e 726f 6164 2d72 6561 6368 3e3d 3230  onroad-reach>=20
+00000470: 3234 2e31 2e32 0a52 6571 7569 7265 732d  24.1.2.Requires-
+00000480: 4469 7374 3a20 6d61 7470 6c6f 746c 6962  Dist: matplotlib
+00000490: 3e3d 332e 352e 320a 5265 7175 6972 6573  >=3.5.2.Requires
+000004a0: 2d44 6973 743a 206e 756d 7079 3e3d 312e  -Dist: numpy>=1.
+000004b0: 3139 2e30 0a52 6571 7569 7265 732d 4469  19.0.Requires-Di
+000004c0: 7374 3a20 7363 6970 793e 3d31 2e37 2e33  st: scipy>=1.7.3
+000004d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000004e0: 7368 6170 656c 793c 332e 302e 302c 3e3d  shapely<3.0.0,>=
+000004f0: 322e 302e 310a 5265 7175 6972 6573 2d44  2.0.1.Requires-D
+00000500: 6973 743a 206f 6d65 6761 636f 6e66 3e3d  ist: omegaconf>=
+00000510: 322e 312e 310a 5265 7175 6972 6573 2d44  2.1.1.Requires-D
+00000520: 6973 743a 2063 6173 6164 693e 3d33 2e36  ist: casadi>=3.6
+00000530: 2e33 0a52 6571 7569 7265 732d 4469 7374  .3.Requires-Dist
+00000540: 3a20 7471 646d 3e3d 342e 3635 2e30 0a52  : tqdm>=4.65.0.R
+00000550: 6571 7569 7265 732d 4469 7374 3a20 696d  equires-Dist: im
+00000560: 6167 6569 6f3e 3d32 2e39 2e30 0a52 6571  ageio>=2.9.0.Req
+00000570: 7569 7265 732d 4469 7374 3a20 7079 7465  uires-Dist: pyte
+00000580: 7374 3e3d 372e 342e 300a 0a23 2043 6f6d  st>=7.4.0..# Com
+00000590: 6d6f 6e52 6f61 642d 4372 694d 650a 215b  monRoad-CriMe.![
+000005a0: 696d 6167 6520 696e 666f 5d28 6874 7470  image info](http
+000005b0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+000005c0: 6572 636f 6e74 656e 742e 636f 6d2f 436f  ercontent.com/Co
+000005d0: 6d6d 6f6e 526f 6164 2f63 6f6d 6d6f 6e72  mmonRoad/commonr
+000005e0: 6f61 642d 6372 696d 652f 6465 7665 6c6f  oad-crime/develo
+000005f0: 702f 646f 6373 2f66 6967 7572 6573 2f43  p/docs/figures/C
+00000600: 7269 4d65 2d62 616e 6e65 722e 706e 6729  riMe-banner.png)
+00000610: 0a5b 215b 4c69 6e75 785d 2868 7474 7073  .[![Linux](https
+00000620: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000630: 6f2f 6261 6467 652f 6f73 2d6c 696e 7578  o/badge/os-linux
+00000640: 3f26 6c6f 676f 3d4c 696e 7578 266c 6f67  ?&logo=Linux&log
+00000650: 6f43 6f6c 6f72 3d77 6869 7465 266c 6162  oColor=white&lab
+00000660: 656c 436f 6c6f 723d 6772 6179 295d 2868  elColor=gray)](h
+00000670: 7474 7073 3a2f 2f70 7970 692e 7079 7468  ttps://pypi.pyth
+00000680: 6f6e 2e6f 7267 2f70 7970 692f 636f 6d6d  on.org/pypi/comm
+00000690: 6f6e 726f 6164 2d6f 7065 6e73 6365 6e61  onroad-openscena
+000006a0: 7269 6f2d 636f 6e76 6572 7465 722f 290a  rio-converter/).
+000006b0: 5b21 5b50 7950 4920 7665 7273 696f 6e20  [![PyPI version 
+000006c0: 6675 7279 2e69 6f5d 2868 7474 7073 3a2f  fury.io](https:/
+000006d0: 2f62 6164 6765 2e66 7572 792e 696f 2f70  /badge.fury.io/p
+000006e0: 792f 636f 6d6d 6f6e 726f 6164 2d63 7269  y/commonroad-cri
+000006f0: 6d65 2e73 7667 3f73 7479 6c65 3d70 6c61  me.svg?style=pla
+00000700: 7374 6963 295d 2868 7474 7073 3a2f 2f70  stic)](https://p
+00000710: 7970 692e 7079 7468 6f6e 2e6f 7267 2f70  ypi.python.org/p
+00000720: 7970 692f 636f 6d6d 6f6e 726f 6164 2d63  ypi/commonroad-c
+00000730: 7269 6d65 2f29 0a5b 215b 5079 5049 206c  rime/).[![PyPI l
+00000740: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
+00000750: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000760: 7970 692f 6c2f 636f 6d6d 6f6e 726f 6164  ypi/l/commonroad
+00000770: 2d63 7269 6d65 2e73 7667 3f73 7479 6c65  -crime.svg?style
+00000780: 3d70 6c61 7374 6963 295d 2868 7474 7073  =plastic)](https
+00000790: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+000007a0: 7267 2f70 7970 692f 636f 6d6d 6f6e 726f  rg/pypi/commonro
+000007b0: 6164 2d63 7269 6d65 2f29 3c62 723e 0a5b  ad-crime/)<br>.[
+000007c0: 215b 5079 5049 2064 6f77 6e6c 6f61 6420  ![PyPI download 
+000007d0: 6d6f 6e74 685d 2868 7474 7073 3a2f 2f69  month](https://i
+000007e0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000007f0: 7069 2f64 6d2f 636f 6d6d 6f6e 726f 6164  pi/dm/commonroad
+00000800: 2d63 7269 6d65 2e73 7667 3f73 7479 6c65  -crime.svg?style
+00000810: 3d70 6c61 7374 6963 266c 6162 656c 3d50  =plastic&label=P
+00000820: 7950 4925 3230 646f 776e 6c6f 6164 7329  yPI%20downloads)
+00000830: 5d28 6874 7470 733a 2f2f 7079 7069 2e70  ](https://pypi.p
+00000840: 7974 686f 6e2e 6f72 672f 7079 7069 2f63  ython.org/pypi/c
+00000850: 6f6d 6d6f 6e72 6f61 642d 6372 696d 652f  ommonroad-crime/
+00000860: 2920 0a5b 215b 5079 5049 2064 6f77 6e6c  ) .[![PyPI downl
+00000870: 6f61 6420 7765 656b 5d28 6874 7470 733a  oad week](https:
+00000880: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000890: 2f70 7970 692f 6477 2f63 6f6d 6d6f 6e72  /pypi/dw/commonr
+000008a0: 6f61 642d 6372 696d 652e 7376 673f 7374  oad-crime.svg?st
+000008b0: 796c 653d 706c 6173 7469 6326 6c61 6265  yle=plastic&labe
+000008c0: 6c3d 5079 5049 2532 3064 6f77 6e6c 6f61  l=PyPI%20downloa
+000008d0: 6473 295d 2868 7474 7073 3a2f 2f70 7970  ds)](https://pyp
+000008e0: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
+000008f0: 692f 636f 6d6d 6f6e 726f 6164 2d63 7269  i/commonroad-cri
+00000900: 6d65 2f29 3c62 723e 0a0a 546f 6f6c 626f  me/)<br>..Toolbo
+00000910: 7820 746f 2063 6f6d 7075 7465 202a 2a43  x to compute **C
+00000920: 7269 2a2a 7469 6361 6c69 7479 202a 2a4d  ri**ticality **M
+00000930: 652a 2a61 7375 7265 7320 0a28 652e 672e  e**asures .(e.g.
+00000940: 2074 696d 652d 746f 2d63 6f6c 6c69 7369   time-to-collisi
+00000950: 6f6e 2c20 7469 6d65 2d74 6f2d 7265 6163  on, time-to-reac
+00000960: 742c 2e2e 2e29 2e20 5375 6368 206d 6561  t,...). Such mea
+00000970: 7375 7265 730a 6361 6e20 6265 2075 7365  sures.can be use
+00000980: 6420 746f 2074 7269 6767 6572 2077 6172  d to trigger war
+00000990: 6e69 6e67 7320 616e 6420 656d 6572 6765  nings and emerge
+000009a0: 6e63 7920 6d61 6e65 7576 6572 7320 0a69  ncy maneuvers .i
+000009b0: 6e20 6472 6976 6572 2061 7373 6973 7461  n driver assista
+000009c0: 6e63 6520 7379 7374 656d 7320 6f72 2072  nce systems or r
+000009d0: 6570 6169 7220 616e 2069 6e66 6561 7369  epair an infeasi
+000009e0: 626c 6520 0a74 7261 6a65 6374 6f72 792e  ble .trajectory.
+000009f0: 2049 6620 796f 7520 6861 7665 2071 7565   If you have que
+00000a00: 7374 696f 6e73 206f 7220 7761 6e74 2074  stions or want t
+00000a10: 6f20 7265 706f 7274 2070 726f 626c 656d  o report problem
+00000a20: 7320 6f72 2073 7567 6765 7374 696f 6e73  s or suggestions
+00000a30: 2c20 706c 6561 7365 2073 7461 7274 2061  , please start a
+00000a40: 205b 4769 7468 7562 2064 6973 6375 7373   [Github discuss
+00000a50: 696f 6e5d 2868 7474 7073 3a2f 2f67 6974  ion](https://git
+00000a60: 6875 622e 636f 6d2f 6f72 6773 2f43 6f6d  hub.com/orgs/Com
+00000a70: 6d6f 6e52 6f61 642f 6469 7363 7573 7369  monRoad/discussi
+00000a80: 6f6e 7329 202f 0a5b 4769 7468 7562 2069  ons) /.[Github i
+00000a90: 7373 7565 5d28 6874 7470 733a 2f2f 6769  ssue](https://gi
+00000aa0: 7468 7562 2e63 6f6d 2f43 6f6d 6d6f 6e52  thub.com/CommonR
+00000ab0: 6f61 642f 636f 6d6d 6f6e 726f 6164 2d63  oad/commonroad-c
+00000ac0: 7269 6d65 2f69 7373 7565 732f 292e 200a  rime/issues/). .
+00000ad0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000ae0: 2f2f 636f 6c61 622e 7265 7365 6172 6368  //colab.research
+00000af0: 2e67 6f6f 676c 652e 636f 6d2f 6472 6976  .google.com/driv
+00000b00: 652f 3154 374d 6253 5671 5535 5843 445a  e/1T7MbSVqU5XCDZ
+00000b10: 6750 5444 4552 4b4e 4b59 4662 4149 6e58  gPTDERKNKYFbAInX
+00000b20: 526a 7922 3e0a 2020 3c69 6d67 2073 7263  Rjy">.  <img src
+00000b30: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+00000b40: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000b50: 636f 6d2f 436f 6d6d 6f6e 526f 6164 2f63  com/CommonRoad/c
+00000b60: 6f6d 6d6f 6e72 6f61 642d 6372 696d 652f  ommonroad-crime/
+00000b70: 6465 7665 6c6f 702f 646f 6373 2f66 6967  develop/docs/fig
+00000b80: 7572 6573 2f6c 6976 655f 6465 6d6f 2e70  ures/live_demo.p
+00000b90: 6e67 2220 616c 743d 224c 6976 6520 4465  ng" alt="Live De
+00000ba0: 6d6f 223e 0a3c 2f61 3e0a 0a23 2320 f09f  mo">.</a>..## ..
+00000bb0: 9a80 2049 6e73 7461 6c6c 6174 696f 6e20  .. Installation 
+00000bc0: 4775 6964 650a 0a60 636f 6d6d 6f6e 726f  Guide..`commonro
+00000bd0: 6164 2d63 7269 6d65 6020 6361 6e20 6265  ad-crime` can be
+00000be0: 2069 6e73 7461 6c6c 6564 2077 6974 683a   installed with:
+00000bf0: 0a0a 6060 6020 6261 7368 0a24 2070 6970  ..``` bash.$ pip
+00000c00: 2069 6e73 7461 6c6c 2063 6f6d 6d6f 6e72   install commonr
+00000c10: 6f61 642d 6372 696d 650a 6060 600a 3c64  oad-crime.```.<d
+00000c20: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00000c30: 3e3c 623e 4465 7665 6c6f 7020 4372 694d  ><b>Develop CriM
+00000c40: 6520 6c6f 6361 6c6c 793c 2f62 3e3c 2f73  e locally</b></s
+00000c50: 756d 6d61 7279 3e0a 0a46 6f72 2061 6464  ummary>..For add
+00000c60: 696e 6720 6e65 7720 6d65 6173 7572 6573  ing new measures
+00000c70: 2c20 7765 2072 6563 6f6d 6d65 6e64 2075  , we recommend u
+00000c80: 7369 6e67 205b 416e 6163 6f6e 6461 5d28  sing [Anaconda](
+00000c90: 6874 7470 733a 2f2f 7777 772e 616e 6163  https://www.anac
+00000ca0: 6f6e 6461 2e63 6f6d 2f29 2074 6f20 6d61  onda.com/) to ma
+00000cb0: 6e61 6765 2079 6f75 7220 656e 7669 726f  nage your enviro
+00000cc0: 6e6d 656e 7420 736f 2074 6861 7420 6576  nment so that ev
+00000cd0: 656e 2069 6620 796f 7520 6d65 7373 2073  en if you mess s
+00000ce0: 6f6d 6574 6869 6e67 2075 702c 2079 6f75  omething up, you
+00000cf0: 2063 616e 2061 6c77 6179 7320 6861 7665   can always have
+00000d00: 2061 2073 6166 6520 616e 6420 636c 6561   a safe and clea
+00000d10: 6e20 7265 7374 6172 742e 2041 2067 7569  n restart. A gui
+00000d20: 6465 2066 6f72 206d 616e 6167 696e 6720  de for managing 
+00000d30: 7079 7468 6f6e 2065 6e76 6972 6f6e 6d65  python environme
+00000d40: 6e74 7320 7769 7468 2041 6e61 636f 6e64  nts with Anacond
+00000d50: 6120 6361 6e20 6265 2066 6f75 6e64 205b  a can be found [
+00000d60: 6865 7265 5d28 6874 7470 733a 2f2f 636f  here](https://co
+00000d70: 6e64 612e 696f 2f70 726f 6a65 6374 732f  nda.io/projects/
+00000d80: 636f 6e64 612f 656e 2f6c 6174 6573 742f  conda/en/latest/
+00000d90: 7573 6572 2d67 7569 6465 2f74 6173 6b73  user-guide/tasks
+00000da0: 2f6d 616e 6167 652d 656e 7669 726f 6e6d  /manage-environm
+00000db0: 656e 7473 2e68 746d 6c29 2e0a 0a41 6674  ents.html)...Aft
+00000dc0: 6572 2069 6e73 7461 6c6c 696e 6720 416e  er installing An
+00000dd0: 6163 6f6e 6461 2c20 6372 6561 7465 2061  aconda, create a
+00000de0: 206e 6577 2065 6e76 6972 6f6e 6d65 6e74   new environment
+00000df0: 2077 6974 683a 0a60 6060 2062 6173 680a   with:.``` bash.
+00000e00: 2420 636f 6e64 6120 6372 6561 7465 202d  $ conda create -
+00000e10: 6e20 636f 6d6d 6f6e 726f 6164 2d70 7933  n commonroad-py3
+00000e20: 3820 7079 7468 6f6e 3d33 2e38 202d 790a  8 python=3.8 -y.
+00000e30: 6060 600a 0a48 6572 6520 7468 6520 6e61  ```..Here the na
+00000e40: 6d65 206f 6620 7468 6520 656e 7669 726f  me of the enviro
+00000e50: 6e6d 656e 7420 6973 2063 616c 6c65 6420  nment is called 
+00000e60: 2a2a 636f 6d6d 6f6e 726f 6164 2d70 7933  **commonroad-py3
+00000e70: 382a 2a2e 2059 6f75 206d 6179 2061 6c73  8**. You may als
+00000e80: 6f20 6368 616e 6765 2074 6869 7320 6e61  o change this na
+00000e90: 6d65 2061 7320 796f 7520 7769 7368 2e20  me as you wish. 
+00000ea0: 496e 2073 7563 6820 6361 7365 2c20 646f  In such case, do
+00000eb0: 6e27 7420 666f 7267 6574 2074 6f20 6368  n't forget to ch
+00000ec0: 616e 6765 2069 7420 696e 2074 6865 2066  ange it in the f
+00000ed0: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00000ee0: 7320 6173 2077 656c 6c2e 202a 2a41 6c77  s as well. **Alw
+00000ef0: 6179 7320 6163 7469 7661 7465 2a2a 2074  ays activate** t
+00000f00: 6869 7320 656e 7669 726f 6e6d 656e 7420  his environment 
+00000f10: 6265 666f 7265 2079 6f75 2064 6f20 616e  before you do an
+00000f20: 7974 6869 6e67 2072 656c 6174 6564 3a0a  ything related:.
+00000f30: 0a60 6060 7368 0a24 2063 6f6e 6461 2061  .```sh.$ conda a
+00000f40: 6374 6976 6174 6520 636f 6d6d 6f6e 726f  ctivate commonro
+00000f50: 6164 2d70 7933 380a 6f72 0a24 2073 6f75  ad-py38.or.$ sou
+00000f60: 7263 6520 6163 7469 7661 7465 2063 6f6d  rce activate com
+00000f70: 6d6f 6e72 6f61 642d 7079 3338 0a60 6060  monroad-py38.```
+00000f80: 0a54 6865 6e2c 2069 6e73 7461 6c6c 2074  .Then, install t
+00000f90: 6865 2064 6570 656e 6465 6e63 6965 7320  he dependencies 
+00000fa0: 7769 7468 3a0a 0a60 6060 7368 0a24 2063  with:..```sh.$ c
+00000fb0: 6420 3c70 6174 682d 746f 2d74 6869 732d  d <path-to-this-
+00000fc0: 7265 706f 3e0a 2420 7069 7020 696e 7374  repo>.$ pip inst
+00000fd0: 616c 6c20 2d65 202e 0a24 2063 6f6e 6461  all -e ..$ conda
+00000fe0: 2064 6576 656c 6f70 202e 0a60 6060 0a0a   develop ..```..
+00000ff0: 546f 2074 6573 7420 7468 6520 696e 7374  To test the inst
+00001000: 616c 6c69 7469 6f6e 2c20 7275 6e20 756e  allition, run un
+00001010: 6974 7465 7374 3a0a 6060 6062 6173 680a  ittest:.```bash.
+00001020: 2420 6364 2074 6573 7473 0a24 2070 7974  $ cd tests.$ pyt
+00001030: 686f 6e20 2d6d 2075 6e69 7474 6573 7420  hon -m unittest 
+00001040: 2d76 0a60 6060 0a0a 3c2f 6465 7461 696c  -v.```..</detail
+00001050: 733e 0a0a 546f 2067 6574 2073 7461 7274  s>..To get start
+00001060: 6564 2079 6f75 7220 6a6f 7572 6e65 7920  ed your journey 
+00001070: 7769 7468 206f 7572 2063 7269 7469 6361  with our critica
+00001080: 6c69 7479 206d 6561 7375 7265 732c 2063  lity measures, c
+00001090: 6865 636b 2074 6865 2060 7475 746f 7269  heck the `tutori
+000010a0: 616c 7360 2061 6e64 2074 6865 2066 6f6c  als` and the fol
+000010b0: 6c6f 7769 6e67 2074 6970 732e 0a0a 3c64  lowing tips...<d
+000010c0: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+000010d0: 3e3c 623e 4164 6420 6e65 7720 6372 6974  ><b>Add new crit
+000010e0: 6963 616c 6974 7920 6d65 6173 7572 653c  icality measure<
+000010f0: 2f62 3e3c 2f73 756d 6d61 7279 3e0a 0a31  /b></summary>..1
+00001100: 2e20 6372 6561 7465 2061 206e 6577 2062  . create a new b
+00001110: 7261 6e63 6820 7769 7468 2060 6665 6174  ranch with `feat
+00001120: 7572 652d 3c6d 6561 7375 7265 2d6e 616d  ure-<measure-nam
+00001130: 653e 6020 616e 6420 6368 6563 6b6f 7574  e>` and checkout
+00001140: 2074 6865 2062 7261 6e63 680a 322e 206e   the branch.2. n
+00001150: 6176 6967 6174 6520 746f 2060 636f 6d6d  avigate to `comm
+00001160: 6f6e 726f 6164 5f63 7269 6d65 2f64 6174  onroad_crime/dat
+00001170: 615f 7374 7275 6374 7572 652f 7479 7065  a_structure/type
+00001180: 2e70 7960 2074 6f20 6669 6e64 2074 6865  .py` to find the
+00001190: 2063 6f72 7265 6374 2063 6174 6567 6f72   correct categor
+000011a0: 7920 6f66 2074 6865 206d 6561 7375 7265  y of the measure
+000011b0: 2061 6e64 2061 6464 2061 6e20 0a65 6e75   and add an .enu
+000011c0: 6d65 7261 7469 6f6e 2065 6e74 7279 2060  meration entry `
+000011d0: 3c61 6262 7265 7669 6174 696f 6e3e 3a20  <abbreviation>: 
+000011e0: 3c65 7870 6c61 6e61 7469 6f6e 3e60 0a33  <explanation>`.3
+000011f0: 2e20 6e61 7669 6761 7465 2074 6f20 6063  . navigate to `c
+00001200: 6f6d 6d6f 6e72 6f61 645f 6372 696d 652f  ommonroad_crime/
+00001210: 6d65 6173 7572 6560 2074 6f20 6669 6e64  measure` to find
+00001220: 2074 6865 2061 626f 7665 2d6d 656e 7469   the above-menti
+00001230: 6f6e 6564 2063 6174 6567 6f72 7920 616e  oned category an
+00001240: 6420 6372 6561 7465 2061 2070 7974 686f  d create a pytho
+00001250: 6e20 6669 6c65 206e 616d 6564 0a60 3c61  n file named.`<a
+00001260: 6262 7265 7669 6174 696f 6e3e 2e70 7960  bbreviation>.py`
+00001270: 2e20 5468 656e 2063 7265 6174 6520 6120  . Then create a 
+00001280: 636c 6173 7320 696e 6865 7269 7469 6e67  class inheriting
+00001290: 2074 6865 2060 4372 694d 6542 6173 6560   the `CriMeBase`
+000012a0: 2075 6e64 6572 2060 636f 6d6d 6f6e 726f   under `commonro
+000012b0: 6164 5f63 7269 6d65 2f64 6174 615f 7374  ad_crime/data_st
+000012c0: 7275 6374 7572 652f 6261 7365 2e70 7960  ructure/base.py`
+000012d0: 0a34 2e20 7369 6d69 6c61 7220 746f 206f  .4. similar to o
+000012e0: 7468 6572 206d 6561 7375 7265 732c 2079  ther measures, y
+000012f0: 6f75 206e 6565 6420 746f 2069 6d70 6c65  ou need to imple
+00001300: 6d65 6e74 2074 6865 2060 636f 6d70 7574  ment the `comput
+00001310: 6528 2960 2061 6e64 2060 7669 7375 616c  e()` and `visual
+00001320: 697a 6528 2960 2066 756e 6374 696f 6e73  ize()` functions
+00001330: 0a0a 3c2f 6465 7461 696c 733e 0a0a 3c64  ..</details>..<d
+00001340: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+00001350: 3e3c 623e 4465 6669 6e65 2063 6f6e 6669  ><b>Define confi
+00001360: 6775 7261 7469 6f6e 2070 6172 616d 6574  guration paramet
+00001370: 6572 7320 6f66 2074 6865 206d 6561 7375  ers of the measu
+00001380: 7265 3c2f 623e 3c2f 7375 6d6d 6172 793e  re</b></summary>
+00001390: 0a0a 312e 206e 6176 6967 6174 6520 746f  ..1. navigate to
+000013a0: 2060 636f 6d6d 6f6e 726f 6164 5f63 7269   `commonroad_cri
+000013b0: 6d65 2f64 6174 615f 7374 7275 6374 7572  me/data_structur
+000013c0: 652f 636f 6e66 6967 7561 7469 6f6e 2e70  e/configuation.p
+000013d0: 7960 2074 6f20 6669 6e64 2074 6865 2061  y` to find the a
+000013e0: 626f 7665 2d6d 656e 7469 6f6e 6564 2063  bove-mentioned c
+000013f0: 6174 6567 6f72 7920 616e 6420 6164 6420  ategory and add 
+00001400: 6120 6e65 7720 0a69 6e73 7461 6e63 6520  a new .instance 
+00001410: 746f 2074 6865 2063 6c61 7373 2061 7320  to the class as 
+00001420: 6073 656c 662e 3c70 6172 616d 6574 6572  `self.<parameter
+00001430: 3e20 3d20 636f 6e66 6967 5f72 656c 6576  > = config_relev
+00001440: 616e 742e 3c70 6172 616d 6574 6572 3e60  ant.<parameter>`
+00001450: 0a32 2e20 796f 7520 6361 6e20 7468 656e  .2. you can then
+00001460: 2064 6972 6563 746c 7920 6361 6c6c 2074   directly call t
+00001470: 6865 2076 616c 7565 7320 7573 696e 6720  he values using 
+00001480: 6073 656c 662e 636f 6e66 6967 7572 6174  `self.configurat
+00001490: 696f 6e2e 3c63 6174 6567 6f72 793e 2e3c  ion.<category>.<
+000014a0: 7061 7261 6d65 7465 723e 6020 696e 2079  parameter>` in y
+000014b0: 6f75 7220 6d65 6173 7572 6520 636c 6173  our measure clas
+000014c0: 730a 332e 2074 6f20 6f76 6572 7269 6465  s.3. to override
+000014d0: 2074 6865 2064 6566 6175 6c74 2070 6172   the default par
+000014e0: 616d 6574 6572 2076 616c 7565 732c 2063  ameter values, c
+000014f0: 7265 6174 6520 6120 6079 616d 6c60 2066  reate a `yaml` f
+00001500: 696c 6520 286e 616d 6520 6974 2074 6865  ile (name it the
+00001510: 2073 616d 6520 6173 2074 6865 2073 6365   same as the sce
+00001520: 6e61 7269 6f29 2069 6e20 602e 2f63 6f6e  nario) in `./con
+00001530: 6669 675f 6669 6c65 7360 2061 6e64 206d  fig_files` and m
+00001540: 6f64 6966 7920 7468 6520 7661 6c75 6573  odify the values
+00001550: 2074 6865 7265 0a0a 3c2f 6465 7461 696c   there..</detail
+00001560: 733e 0a0a 2323 20f0 9f9a a720 446f 6375  s>..## .... Docu
+00001570: 6d65 6e74 6174 696f 6e0a 0a54 6865 2064  mentation..The d
+00001580: 6f63 756d 656e 7461 7469 6f6e 206f 6620  ocumentation of 
+00001590: 6f75 7220 746f 6f6c 626f 7820 6973 2061  our toolbox is a
+000015a0: 7661 696c 6162 6c65 206f 6e20 6f75 7220  vailable on our 
+000015b0: 7765 6273 6974 653a 2068 7474 7073 3a2f  website: https:/
+000015c0: 2f63 7073 2e70 6167 6573 2e67 6974 6c61  /cps.pages.gitla
+000015d0: 622e 6c72 7a2e 6465 2f63 6f6d 6d6f 6e72  b.lrz.de/commonr
+000015e0: 6f61 642f 636f 6d6d 6f6e 726f 6164 2d63  oad/commonroad-c
+000015f0: 7269 7469 6361 6c69 7479 2d6d 6561 7375  riticality-measu
+00001600: 7265 732f 2e0a 3c64 6574 6169 6c73 3e0a  res/..<details>.
+00001610: 3c73 756d 6d61 7279 3e3c 623e 4275 696c  <summary><b>Buil
+00001620: 6420 646f 6375 6d65 6e74 6174 696f 6e20  d documentation 
+00001630: 6c6f 6361 6c6c 793c 2f62 3e3c 2f73 756d  locally</b></sum
+00001640: 6d61 7279 3e0a 496e 206f 7264 6572 2074  mary>.In order t
+00001650: 6f20 6765 6e65 7261 7465 2074 6865 2064  o generate the d
+00001660: 6f63 756d 656e 7461 7469 6f6e 2076 6961  ocumentation via
+00001670: 2053 7068 696e 7820 6c6f 6361 6c6c 792c   Sphinx locally,
+00001680: 2072 756e 2074 6865 2066 6f6c 6c6f 7769   run the followi
+00001690: 6e67 2063 6f6d 6d61 6e64 7320 696e 2074  ng commands in t
+000016a0: 6865 2072 6f6f 7420 6469 7265 6374 6f72  he root director
+000016b0: 793a 0a0a 6060 6062 6173 680a 2420 7069  y:..```bash.$ pi
+000016c0: 7020 696e 7374 616c 6c20 2d72 202e 2f64  p install -r ./d
+000016d0: 6f63 732f 7265 7175 6972 656d 656e 7473  ocs/requirements
+000016e0: 5f64 6f63 2e74 7874 0a24 2063 6420 646f  _doc.txt.$ cd do
+000016f0: 6373 2f73 7068 696e 780a 2420 6d61 6b65  cs/sphinx.$ make
+00001700: 2068 746d 6c0a 6060 600a 0a54 6865 2064   html.```..The d
+00001710: 6f63 756d 656e 7461 7469 6f6e 2063 616e  ocumentation can
+00001720: 2074 6865 6e20 6265 206c 6175 6e63 6865   then be launche
+00001730: 6420 6279 2062 726f 7773 696e 6720 6060  d by browsing ``
+00001740: 2e2f 646f 6373 2f73 7068 696e 782f 6275  ./docs/sphinx/bu
+00001750: 696c 642f 6874 6d6c 2f69 6e64 6578 2e68  ild/html/index.h
+00001760: 746d 6c2f 6060 2e0a 3c2f 6465 7461 696c  tml/``..</detail
+00001770: 733e 0a0a 2323 20f0 9f8c 9f20 436f 6e74  s>..## .... Cont
+00001780: 7269 6275 746f 7273 2028 696e 2061 6c70  ributors (in alp
+00001790: 6861 6265 7469 6361 6c20 6f72 6465 7220  habetical order 
+000017a0: 6279 206c 6173 7420 6e61 6d65 290a 0a2d  by last name)..-
+000017b0: 204c 6967 756f 2043 6865 6e0a 2d20 4d61   Liguo Chen.- Ma
+000017c0: 7269 7573 2045 7261 7468 0a2d 2059 7561  rius Erath.- Yua
+000017d0: 6e66 6569 204c 696e 0a2d 2053 6562 6173  nfei Lin.- Sebas
+000017e0: 7469 616e 204d 6169 6572 686f 6665 720a  tian Maierhofer.
+000017f0: 2d20 4976 616e 6120 5065 6e65 7661 0a2d  - Ivana Peneva.-
+00001800: 204b 756e 2051 6961 6e0a 2d20 4f6c 6976   Kun Qian.- Oliv
+00001810: 6572 2053 7065 6368 740a 2d20 5369 6368  er Specht.- Sich
+00001820: 656e 6720 5761 6e67 0a2d 2059 6f75 7261  eng Wang.- Youra
+00001830: 6e20 5761 6e67 0a2d 205a 656b 756e 2058  n Wang.- Zekun X
+00001840: 696e 670a 2d20 5a69 7169 616e 2058 750a  ing.- Ziqian Xu.
+00001850: 0a23 2320 f09f 9496 2043 6974 6174 696f  .## .... Citatio
+00001860: 6e0a 4966 2079 6f75 2075 7365 2060 636f  n.If you use `co
+00001870: 6d6d 6f6e 726f 6164 2d63 7269 6d65 6020  mmonroad-crime` 
+00001880: 666f 7220 6163 6164 656d 6963 2077 6f72  for academic wor
+00001890: 6b2c 2077 6520 6869 6768 6c79 2065 6e63  k, we highly enc
+000018a0: 6f75 7261 6765 2079 6f75 2074 6f20 6369  ourage you to ci
+000018b0: 7465 206f 7572 2070 6170 6572 3a0a 6060  te our paper:.``
+000018c0: 6074 6578 740a 4049 6e50 726f 6365 6564  `text.@InProceed
+000018d0: 696e 6773 7b6c 696e 3230 3233 6372 696d  ings{lin2023crim
+000018e0: 652c 0a20 2020 2020 2074 6974 6c65 2020  e,.      title  
+000018f0: 2020 203d 207b 7b43 6f6d 6d6f 6e52 6f61     = {{CommonRoa
+00001900: 642d 4372 694d 657d 3a20 7b41 7d20 546f  d-CriMe}: {A} To
+00001910: 6f6c 626f 7820 666f 7220 4372 6974 6963  olbox for Critic
+00001920: 616c 6974 7920 4d65 6173 7572 6573 206f  ality Measures o
+00001930: 6620 4175 746f 6e6f 6d6f 7573 2056 6568  f Autonomous Veh
+00001940: 6963 6c65 737d 2c0a 2020 2020 2020 6175  icles},.      au
+00001950: 7468 6f72 2020 2020 3d20 7b59 7561 6e66  thor    = {Yuanf
+00001960: 6569 204c 696e 2061 6e64 204d 6174 7468  ei Lin and Matth
+00001970: 6961 7320 416c 7468 6f66 667d 2c0a 2020  ias Althoff},.  
+00001980: 2020 2020 626f 6f6b 7469 746c 6520 3d20      booktitle = 
+00001990: 7b50 726f 632e 206f 6620 7468 6520 4945  {Proc. of the IE
+000019a0: 4545 2049 6e74 656c 6c2e 2056 6568 2e20  EE Intell. Veh. 
+000019b0: 5379 6d70 2e7d 2c20 2020 2020 0a20 2020  Symp.},     .   
+000019c0: 2020 2070 6167 6573 2020 2020 203d 207b     pages     = {
+000019d0: 312d 387d 2c20 0a20 2020 2020 2079 6561  1-8}, .      yea
+000019e0: 7220 2020 2020 203d 207b 3230 3233 7d2c  r      = {2023},
+000019f0: 0a7d 0a60 6060 0a49 6620 796f 7520 7573  .}.```.If you us
+00001a00: 6520 7468 6973 2070 726f 6a65 6374 2773  e this project's
+00001a10: 2063 6f64 6520 696e 2069 6e64 7573 7472   code in industr
+00001a20: 792c 2077 6527 6420 6c6f 7665 2074 6f20  y, we'd love to 
+00001a30: 6865 6172 2066 726f 6d20 796f 7520 6173  hear from you as
+00001a40: 2077 656c 6c3b 200a 6665 656c 2066 7265   well; .feel fre
+00001a50: 6520 746f 2072 6561 6368 206f 7574 2074  e to reach out t
+00001a60: 6f20 5b59 7561 6e66 6569 204c 696e 5d28  o [Yuanfei Lin](
+00001a70: 6d61 696c 746f 3a79 7561 6e66 6569 2e6c  mailto:yuanfei.l
+00001a80: 696e 4074 756d 2e64 6529 2064 6972 6563  in@tum.de) direc
+00001a90: 746c 792e 0a                             tly..
```

### Comparing `commonroad-crime-0.3.3/commonroad_crime.egg-info/SOURCES.txt` & `commonroad_crime-0.4.0/commonroad_crime.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 commonroad_crime/utility/batch_evaluation.py
 commonroad_crime/utility/general.py
 commonroad_crime/utility/logger.py
 commonroad_crime/utility/optimization.py
 commonroad_crime/utility/simulation.py
 commonroad_crime/utility/solver.py
 commonroad_crime/utility/visualization.py
+tests/__init__.py
 tests/test_acceleration_domain.py
 tests/test_base.py
 tests/test_distance_domain.py
 tests/test_index_domain.py
 tests/test_jerk_domain.py
 tests/test_potential_domain.py
 tests/test_probability_domain.py
```

### Comparing `commonroad-crime-0.3.3/setup.py` & `commonroad_crime-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,27 +19,27 @@
     keywords="criticality, autonomous driving",
     long_description_content_type="text/markdown",
     long_description=readme,
     author="Technical University of Munich",
     author_email="commonroad@lists.lrz.de",
     license="BSD 3-Clause",
     project_urls={
-        "Documentation": "https://cps.pages.gitlab.lrz.de/commonroad-criticality-measures/",
-        "Forum": "https://commonroad.in.tum.de/forum/c/commonroad-crime/20",
-        "Source": "https://gitlab.lrz.de/tum-cps/commonroad-crime",
+        "Documentation": "https://cps.pages.gitlab.lrz.de/commonroad/commonroad-criticality-measures/",
+        "Forum": "https://github.com/CommonRoad/commonroad-crime/issues",
+        "Source": "https://github.com/CommonRoad/commonroad-crime",
     },
     url="https://commonroad.in.tum.de/tools/commonroad-crime",
     packages=find_packages(),
     data_files=[(".", ["LICENSE"])],
     install_requires=[
         "commonroad-io>=2023.4",
         "commonroad-vehicle-models>=3.0.0",
-        "commonroad-route-planner>=2022.3,<2024.1",
+        "commonroad-route-planner>=2024.2.0",
         "commonroad-drivability-checker>=2023.1",
-        "commonroad-reach>=2023.1",
+        "commonroad-reach>=2024.1.2",
         "matplotlib>=3.5.2",
         "numpy>=1.19.0",
         "scipy>=1.7.3",
         "shapely<3.0.0,>=2.0.1",
         "omegaconf>=2.1.1",
         "casadi>=3.6.3",
         "tqdm>=4.65.0",
```

### Comparing `commonroad-crime-0.3.3/tests/test_acceleration_domain.py` & `commonroad_crime-0.4.0/tests/test_acceleration_domain.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """
 Unit tests of the module acceleration-scale measures
 """
 
+import os
 import unittest
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.measure import DST, ALongReq, ALatReq, AReq
 import commonroad_crime.utility.logger as util_logger
 
 
 class TestAccelerationDomain(unittest.TestCase):
     def setUp(self) -> None:
         super().setUp()
         scenario_id = "DEU_Gar-1_1_T-1"
+        current_dir = os.path.dirname(__file__)
         self.config = CriMeConfiguration.load(
-            f"../config_files/{scenario_id}.yaml", scenario_id
+            os.path.join(current_dir, "../config_files", f"{scenario_id}.yaml"),
+            scenario_id,
         )
+
         util_logger.initialize_logger(self.config)
         self.config.print_configuration_summary()
         self.config.update()
 
     def test_dst(self):
         dst_object = DST(self.config)
         dst_1 = dst_object.compute(201, 0)
```

### Comparing `commonroad-crime-0.3.3/tests/test_base.py` & `commonroad_crime-0.4.0/tests/test_distance_domain.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,58 @@
-import unittest
+"""
+Unit tests of the module distance-scale measures
+"""
 
-import numpy as np
-import pytest
+import unittest
 
-from commonroad_crime.data_structure.scene import Scene
-from commonroad_crime.data_structure.base import CriMeBase
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
+from commonroad_crime.measure import PSD, MSD, HW, DCE
 import commonroad_crime.utility.logger as util_logger
 
-from commonroad_dc.pycrccosy import CurvilinearCoordinateSystem
+from commonroad.common.file_reader import CommonRoadFileReader
 
 
-class TestBase(unittest.TestCase):
+class TestDistanceDomain(unittest.TestCase):
     def setUp(self) -> None:
         super().setUp()
-        scenario_id = "DEU_Test-1_1_T-1"
-        self.config = CriMeConfiguration.load(
-            f"../config_files/{scenario_id}.yaml", scenario_id
-        )
+        scenario_id = "ZAM_Urban-3_3_Repair"
+        self.config = CriMeConfiguration()
+        self.config.general.set_scenario_name(scenario_id)
+        self.config.vehicle.ego_id = 8
         util_logger.initialize_logger(self.config)
         self.config.print_configuration_summary()
-
-    def test_construction(self):
-        """
-        Test the construction of base classes.
-        """
         self.config.update()
-        base_1 = CriMeBase(self.config)
 
-        scene = Scene(0, self.config.scenario)
-        self.config.update(sce=scene)
-        base_2 = CriMeBase(self.config)
-
-        self.assertIsInstance(base_1, CriMeBase)
-        self.assertIsInstance(base_2, CriMeBase)
-
-    def test_clcs(self):
-        """
-        Test the update of the CLCS.
-        """
-        self.config.update()
-        base = CriMeBase(self.config)
-        with pytest.raises(AttributeError):
-            base.clcs = self.config.vehicle.curvilinear.clcs
-
-        example_list = [
-            np.array([1.0, 2.0]),
-            np.array([3.0, 4.0]),
-            np.array([5.0, 6.0]),
-        ]
-        new_clcs = CurvilinearCoordinateSystem(example_list)
-        self.config.update(CLCS=new_clcs)
-        self.assertEqual(base.clcs, new_clcs)
+    def test_MSD_PSD(self):
+        self.config.general.name_scenario = "BEL_Putte-8_2_T-1"
+        sce_crosswalk, _ = CommonRoadFileReader(self.config.general.path_scenario).open(
+            lanelet_assignment=True
+        )
+        self.config.update(ego_id=349, sce=sce_crosswalk)
+        msd_object = MSD(self.config)
+        msd = msd_object.compute(328, 0)
+        self.assertEqual(msd, 0.32)
+        self.config.debug.plot_limits = [-320, -380, 210, 290]
+        msd_object.visualize()
+
+        psd_object = PSD(self.config)
+        psd = psd_object.compute(328, 0)
+        self.assertEqual(psd, 38.49)
+        psd_object.visualize()
+
+    def test_hw(self):
+        hw_object = HW(self.config)
+        hw = hw_object.compute(6, 0)
+        self.assertGreater(hw, 0)
+        self.assertEqual(hw, 20.75)
+        hw_object.visualize()
+
+    def test_dce(self):
+        dce_object_1 = DCE(self.config)
+        dce_1 = dce_object_1.compute(6, 0)
+        dce_object_1.visualize()
+        self.assertEqual(dce_1, 0.00)
+
+        dce_object_2 = DCE(self.config)
+        dce_2 = dce_object_2.compute(7, 0)
+        dce_object_2.visualize()
+        self.assertEqual(dce_2, 0.98)
```

### Comparing `commonroad-crime-0.3.3/tests/test_distance_domain.py` & `commonroad_crime-0.4.0/tests/test_index_domain.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,117 @@
 """
-Unit tests of the module distance-scale measures
+Unit tests of the module index-scale measures
 """
 
 import unittest
+import os
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
-from commonroad_crime.measure import PSD, MSD, HW, DCE
+from commonroad_crime.measure import BTN, STN, TCI, CPI, CI, SOI
 import commonroad_crime.utility.logger as util_logger
 
 from commonroad.common.file_reader import CommonRoadFileReader
 
 
-class TestDistanceDomain(unittest.TestCase):
+class TestIndexDomain(unittest.TestCase):
     def setUp(self) -> None:
         super().setUp()
+        scenario_id = "ZAM_Zip-1_56_T-1"
+        current_dir = os.path.dirname(__file__)
+        self.config = CriMeConfiguration.load(
+            os.path.join(current_dir, "../config_files", f"{scenario_id}.yaml"),
+            scenario_id,
+        )
+
+        util_logger.initialize_logger(self.config)
+        self.config.print_configuration_summary()
+        self.config.update()
+
+    def test_bnt(self):
+        btn_object = BTN(self.config)
+        # vehicle in the same lanelet and in front
+        btn_1 = btn_object.compute(3, 0)
+        btn_object.visualize()
+        self.assertAlmostEqual(btn_1, 0.1043)
+
+        # vehicle in another lanelet
+        btn_2 = btn_object.compute(1, 0)
+        self.assertAlmostEqual(btn_2, 0.0)
+
+    def test_snt(self):
+        stn_object = STN(self.config)
+        # vehicle in the same lanelet and in front
+        stn_1 = stn_object.compute(3, 0)
+        self.assertAlmostEqual(stn_1, 0.0238)
+
+        # vehicle in another lanelet
+        stn_2 = stn_object.compute(1, 0)
+        self.assertAlmostEqual(stn_2, 0.0)
+
+    def test_tci(self):
+        self.config.vehicle.ego_id = 1
+        tci_object = TCI(self.config)
+        tci_1 = tci_object.compute(0)
+        tci_object.visualize()
+        self.assertEqual(tci_1, 0.0)
+
+    def test_cpi(self):
+        cpi_object = CPI(self.config)
+        cpi = cpi_object.compute_criticality(0)
+        cpi_object.visualize()
+        self.assertAlmostEqual(cpi, 4.4345e-06)
+
+    def test_ci(self):
+        ci_object = CI(self.config)
+        ci = ci_object.compute(3, 0)
+        self.assertEqual(ci, 0.0)
+
+        # test scenario with valid conflict area
+        self.config.general.name_scenario = "ZAM_Tjunction-1_97_T-1"
+        sce_pet, _ = CommonRoadFileReader(self.config.general.path_scenario).open(
+            lanelet_assignment=True
+        )
+        self.config.update(ego_id=5, sce=sce_pet)
+        ci_object = CI(self.config)
+        ci = ci_object.compute(1, 0)
+        self.assertAlmostEqual(ci, 2688.3)
+        self.config.debug.plot_limits = [-100, 100, -10, 80]
+        ci_object.visualize()
+
+    def test_soi(self):
         scenario_id = "ZAM_Urban-3_3_Repair"
         self.config = CriMeConfiguration()
         self.config.general.set_scenario_name(scenario_id)
         self.config.vehicle.ego_id = 8
-        util_logger.initialize_logger(self.config)
-        self.config.print_configuration_summary()
         self.config.update()
 
-    def test_MSD_PSD(self):
-        self.config.general.name_scenario = "BEL_Putte-8_2_T-1"
-        sce_crosswalk, _ = CommonRoadFileReader(self.config.general.path_scenario).open(
-            lanelet_assignment=True
+        soi_object_1 = SOI(self.config)
+        soi_1 = soi_object_1.compute()
+        soi_object_1.visualize()
+        self.assertEqual(soi_1, 39.0)
+
+        scenario_id = "USA_Lanker-1_3_T-1"
+        current_dir = os.path.dirname(__file__)
+        self.config = CriMeConfiguration.load(
+            os.path.join(current_dir, "../config_files", f"{scenario_id}.yaml"),
+            scenario_id,
         )
-        self.config.update(ego_id=349, sce=sce_crosswalk)
-        msd_object = MSD(self.config)
-        msd = msd_object.compute(328, 0)
-        self.assertEqual(msd, 0.32)
-        self.config.debug.plot_limits = [-320, -380, 210, 290]
-        msd_object.visualize()
-
-        psd_object = PSD(self.config)
-        psd = psd_object.compute(328, 0)
-        self.assertEqual(psd, 38.49)
-        psd_object.visualize()
-
-    def test_hw(self):
-        hw_object = HW(self.config)
-        hw = hw_object.compute(6, 0)
-        self.assertGreater(hw, 0)
-        self.assertEqual(hw, 20.75)
-        hw_object.visualize()
-
-    def test_dce(self):
-        dce_object_1 = DCE(self.config)
-        dce_1 = dce_object_1.compute(6, 0)
-        dce_object_1.visualize()
-        self.assertEqual(dce_1, 0.00)
-
-        dce_object_2 = DCE(self.config)
-        dce_2 = dce_object_2.compute(7, 0)
-        dce_object_2.visualize()
-        self.assertEqual(dce_2, 0.98)
+
+        self.config.update()
+
+        soi_object_2 = SOI(self.config)
+        soi_2 = soi_object_2.compute()
+        soi_object_2.visualize()
+        self.assertEqual(soi_2, 32.0)
+
+        scenario_id = "DEU_Moabit-4_1_T-1"
+        current_dir = os.path.dirname(__file__)
+        self.config = CriMeConfiguration.load(
+            os.path.join(current_dir, "../config_files", f"{scenario_id}.yaml"),
+            scenario_id,
+        )
+        self.config.update()
+
+        soi_object_3 = SOI(self.config)
+        soi_3 = soi_object_3.compute()
+        soi_object_3.visualize()
+        self.assertEqual(soi_3, 0.0)
```

### Comparing `commonroad-crime-0.3.3/tests/test_jerk_domain.py` & `commonroad_crime-0.4.0/tests/test_jerk_domain.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """
 Unit tests of the module jerk-scale measures
 """
 
 import unittest
+import os
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.measure import LatJ, LongJ
 import commonroad_crime.utility.logger as util_logger
 
 
 class TestJerkDomain(unittest.TestCase):
     def setUp(self) -> None:
         super().setUp()
         scenario_id = "ZAM_Zip-1_56_T-1"
+
+        current_dir = os.path.dirname(__file__)
         self.config = CriMeConfiguration.load(
-            f"../config_files/{scenario_id}.yaml", scenario_id
+            os.path.join(current_dir, "../config_files", f"{scenario_id}.yaml"),
+            scenario_id,
         )
+
         util_logger.initialize_logger(self.config)
         self.config.print_configuration_summary()
         self.config.update()
 
     def test_lat_j(self):
         lat_j_obj = LatJ(self.config)
         lat_j_1 = lat_j_obj.compute(0)
```

### Comparing `commonroad-crime-0.3.3/tests/test_potential_domain.py` & `commonroad_crime-0.4.0/tests/test_potential_domain.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """
 Unit tests of the module potential-scale measures
 """
 
 import unittest
+import os
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.measure.potential.pf import PF
 import commonroad_crime.utility.logger as util_logger
 
 
 class TestPotentialDomain(unittest.TestCase):
     def setUp(self) -> None:
         super().setUp()
         scenario_id = "DEU_Gar-1_1_T-1"
+        current_dir = os.path.dirname(__file__)
         self.config = CriMeConfiguration.load(
-            f"../config_files/{scenario_id}.yaml", scenario_id
+            os.path.join(current_dir, "../config_files", f"{scenario_id}.yaml"),
+            scenario_id,
         )
+
         util_logger.initialize_logger(self.config)
         self.config.print_configuration_summary()
         self.config.update()
 
     def test_pf(self):
         pf_object = PF(self.config)
         pf = pf_object.compute(20)
```

### Comparing `commonroad-crime-0.3.3/tests/test_probability_domain.py` & `commonroad_crime-0.4.0/tests/test_reachable_set_domain.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """
-Unit tests of the module probability-scale measures
+Unit tests of the module reachable set scale measures
 """
 
 import unittest
 
+from commonroad_crime.measure.reachable_set.drivable_area import DA
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
-from commonroad_crime.measure.probability.p_mc import P_MC
 import commonroad_crime.utility.logger as util_logger
 
 
-class TestProbabilityDomain(unittest.TestCase):
+class TestReachableSetDomain(unittest.TestCase):
     def setUp(self) -> None:
         super().setUp()
-        scenario_id = "DEU_Gar-1_1_T-1"
-        self.config = CriMeConfiguration.load(
-            f"../config_files/{scenario_id}.yaml", scenario_id
-        )
+        scenario_id = "ZAM_Urban-3_3_Repair"
+        self.config = CriMeConfiguration()
+        self.config.general.set_scenario_name(scenario_id)
+        self.config.vehicle.ego_id = 8
         util_logger.initialize_logger(self.config)
         self.config.print_configuration_summary()
         self.config.update()
 
-    def test_p_mc(self):
-        p_mc_object = P_MC(self.config)
-        p_mc = p_mc_object.compute(0)
-        p_mc_object.visualize()
-        self.assertLessEqual(abs(p_mc - 0.04), 0.05)
-        self.assertLessEqual(p_mc, 1.0)
+    def test_drivable_area(self):
+        da_solver = DA(self.config)
+        self.assertAlmostEqual(da_solver.compute(), 60.13)
+        da_solver.visualize()
```

### Comparing `commonroad-crime-0.3.3/tests/test_time_domain.py` & `commonroad_crime-0.4.0/tests/test_time_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/tests/test_utils_simulation.py` & `commonroad_crime-0.4.0/tests/test_utils_simulation.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.3.3/tests/test_velocity_domain.py` & `commonroad_crime-0.4.0/tests/test_velocity_domain.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """
 Unit tests of the module velocity-scale measures
 """
 
+import os
 import unittest
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 from commonroad_crime.measure.velocity.delta_v import DeltaV
 import commonroad_crime.utility.logger as util_logger
 
 
 class TestVelocityDomain(unittest.TestCase):
     def setUp(self) -> None:
         super().setUp()
         scenario_id = "DEU_Gar-1_1_T-1"
+
+        current_dir = os.path.dirname(__file__)
         self.config = CriMeConfiguration.load(
-            f"../config_files/{scenario_id}.yaml", scenario_id
+            os.path.join(current_dir, "../config_files", f"{scenario_id}.yaml"),
+            scenario_id,
         )
         util_logger.initialize_logger(self.config)
         self.config.print_configuration_summary()
         self.config.update()
 
     def test_delta_v(self):
         delta_v_object = DeltaV(self.config)
```

