# Comparing `tmp/pyflowline-0.3.8.tar.gz` & `tmp/pyflowline-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflowline-0.3.8.tar", last modified: Wed Apr 17 04:03:29 2024, max compression
+gzip compressed data, was "pyflowline-0.3.9.tar", last modified: Tue May  7 17:00:14 2024, max compression
```

## Comparing `pyflowline-0.3.8.tar` & `pyflowline-0.3.9.tar`

### file list

```diff
@@ -1,175 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.277315 pyflowline-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-17 04:03:19.000000 pyflowline-0.3.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-17 04:03:19.000000 pyflowline-0.3.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-17 04:03:19.000000 pyflowline-0.3.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-17 04:03:19.000000 pyflowline-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 04:03:19.000000 pyflowline-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 04:03:29.277315 pyflowline-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-17 04:03:19.000000 pyflowline-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.245315 pyflowline-0.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.253315 pyflowline-0.3.8/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    67244 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/after_loop.png
--rw-r--r--   0 runner    (1001) docker     (127)    64320 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/after_merge.png
--rw-r--r--   0 runner    (1001) docker     (127)    68901 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/basic_element.png
--rw-r--r--   0 runner    (1001) docker     (127)    76858 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/before_loop.png
--rw-r--r--   0 runner    (1001) docker     (127)    68959 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/before_merge.png
--rw-r--r--   0 runner    (1001) docker     (127)    16482 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/disconnect_flowline.png
--rw-r--r--   0 runner    (1001) docker     (127)   146717 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/find_vertex.png
--rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/flow_direction.png
--rw-r--r--   0 runner    (1001) docker     (127)   252712 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/flow_direction_matrix.png
--rw-r--r--   0 runner    (1001) docker     (127)   525380 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/hexagon.png
--rw-r--r--   0 runner    (1001) docker     (127)   628942 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/hexagon_intersect.png
--rw-r--r--   0 runner    (1001) docker     (127)   524174 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/lat_lon.png
--rw-r--r--   0 runner    (1001) docker     (127)   734342 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/lat_lon_intersect.png
--rw-r--r--   0 runner    (1001) docker     (127)    45168 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/merge_flowline.png
--rw-r--r--   0 runner    (1001) docker     (127)  1191889 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/meshes.png
--rw-r--r--   0 runner    (1001) docker     (127)    47724 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/remove_loop.png
--rw-r--r--   0 runner    (1001) docker     (127)   596253 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/remove_loop_matrix.png
--rw-r--r--   0 runner    (1001) docker     (127)    93563 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/simplification01.png
--rw-r--r--   0 runner    (1001) docker     (127)    21317 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/small_river.png
--rw-r--r--   0 runner    (1001) docker     (127)   148387 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/sqaure_intersect.png
--rw-r--r--   0 runner    (1001) docker     (127)    61180 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/square.png
--rw-r--r--   0 runner    (1001) docker     (127)    46783 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/structure_pyflowline.png
--rw-r--r--   0 runner    (1001) docker     (127)   160993 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/figures/workflow.png
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.257315 pyflowline-0.3.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.257315 pyflowline-0.3.8/docs/source/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/algorithm/algorithm.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.257315 pyflowline-0.3.8/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/api/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.257315 pyflowline-0.3.8/docs/source/application/
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/application/application.rst
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.257315 pyflowline-0.3.8/docs/source/data/
--rw-r--r--   0 runner    (1001) docker     (127)    29917 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/data/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.257315 pyflowline-0.3.8/docs/source/installation/
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/installation/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/references.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/support.rst
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-17 04:03:19.000000 pyflowline-0.3.8/docs/source/visualization.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.257315 pyflowline-0.3.8/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-17 04:03:19.000000 pyflowline-0.3.8/examples/create_model_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.257315 pyflowline-0.3.8/pyflowline/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.261315 pyflowline-0.3.8/pyflowline/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.261315 pyflowline-0.3.8/pyflowline/algorithms/auxiliary/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/auxiliary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16311 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/auxiliary/check_head_water.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/auxiliary/find_index_in_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/auxiliary/find_vertex_in_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.261315 pyflowline-0.3.8/pyflowline/algorithms/connection/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/connection/connect_disconnect_flowline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.261315 pyflowline-0.3.8/pyflowline/algorithms/cython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/cython/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.261315 pyflowline-0.3.8/pyflowline/algorithms/direction/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/direction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/direction/correct_flowline_direction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.261315 pyflowline-0.3.8/pyflowline/algorithms/index/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/index/define_stream_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/index/define_stream_segment_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/index/define_stream_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.265315 pyflowline-0.3.8/pyflowline/algorithms/intersect/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/intersect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.265315 pyflowline-0.3.8/pyflowline/algorithms/loop/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/loop/remove_flowline_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.265315 pyflowline-0.3.8/pyflowline/algorithms/merge/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/merge/merge_flowline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.265315 pyflowline-0.3.8/pyflowline/algorithms/simplification/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/simplification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/simplification/remove_duplicate_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/simplification/remove_duplicate_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/simplification/remove_returning_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/simplification/remove_small_river.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.265315 pyflowline-0.3.8/pyflowline/algorithms/split/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/split/find_flowline_confluence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/split/find_flowline_vertex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/split/split_by_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/split/split_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/algorithms/split/split_flowline_to_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/change_json_key_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.269315 pyflowline-0.3.8/pyflowline/classes/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/_hpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/_visual_basin.py
--rw-r--r--   0 runner    (1001) docker     (127)    62019 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/basin.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/confluence.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/dggrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/hexagon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/latlon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/mpas.py
--rw-r--r--   0 runner    (1001) docker     (127)    60711 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/pycase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/square.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/tin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/classes/vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.273315 pyflowline-0.3.8/pyflowline/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/formats/convert_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/formats/convert_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/formats/convert_flowline_to_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/formats/export_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/formats/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/formats/export_vertex.py
--rw-r--r--   0 runner    (1001) docker     (127)    11769 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/formats/read_flowline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/formats/read_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/formats/read_nhdplus_flowline_shapefile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.273315 pyflowline-0.3.8/pyflowline/mesh/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.273315 pyflowline-0.3.8/pyflowline/mesh/dggrid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/mesh/dggrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/mesh/dggrid/create_dggrid_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.273315 pyflowline-0.3.8/pyflowline/mesh/hexagon/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/mesh/hexagon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28451 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/mesh/hexagon/create_hexagon_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.273315 pyflowline-0.3.8/pyflowline/mesh/latlon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/mesh/latlon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/mesh/latlon/create_latlon_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.273315 pyflowline-0.3.8/pyflowline/mesh/mpas/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/mesh/mpas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/mesh/mpas/create_mpas_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.273315 pyflowline-0.3.8/pyflowline/mesh/square/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/mesh/square/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/mesh/square/create_square_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.273315 pyflowline-0.3.8/pyflowline/mesh/tin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/mesh/tin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/mesh/tin/create_tin_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/pyflowline_create_template_configuration_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyflowline/pyflowline_read_model_configuration_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.277315 pyflowline-0.3.8/pyflowline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 04:03:29.000000 pyflowline-0.3.8/pyflowline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-17 04:03:29.000000 pyflowline-0.3.8/pyflowline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 04:03:29.000000 pyflowline-0.3.8/pyflowline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-17 04:03:29.000000 pyflowline-0.3.8/pyflowline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 04:03:29.000000 pyflowline-0.3.8/pyflowline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 04:03:19.000000 pyflowline-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-17 04:03:29.277315 pyflowline-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-17 04:03:19.000000 pyflowline-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:03:29.273315 pyflowline-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 04:03:19.000000 pyflowline-0.3.8/tests/test_installation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.794669 pyflowline-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-07 17:00:08.000000 pyflowline-0.3.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-07 17:00:08.000000 pyflowline-0.3.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 17:00:08.000000 pyflowline-0.3.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-07 17:00:08.000000 pyflowline-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 17:00:08.000000 pyflowline-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-05-07 17:00:14.794669 pyflowline-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-07 17:00:08.000000 pyflowline-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.758669 pyflowline-0.3.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.770669 pyflowline-0.3.9/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    67244 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/after_loop.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64320 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/after_merge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68901 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/basic_element.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76858 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/before_loop.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68959 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/before_merge.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16482 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/disconnect_flowline.png
+-rw-r--r--   0 runner    (1001) docker     (127)   146717 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/find_vertex.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/flow_direction.png
+-rw-r--r--   0 runner    (1001) docker     (127)   252712 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/flow_direction_matrix.png
+-rw-r--r--   0 runner    (1001) docker     (127)   525380 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/hexagon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   628942 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/hexagon_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (127)   524174 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/lat_lon.png
+-rw-r--r--   0 runner    (1001) docker     (127)   734342 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/lat_lon_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45168 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/merge_flowline.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1191889 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/meshes.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47724 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/remove_loop.png
+-rw-r--r--   0 runner    (1001) docker     (127)   596253 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/remove_loop_matrix.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93563 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/simplification01.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21317 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/small_river.png
+-rw-r--r--   0 runner    (1001) docker     (127)   148387 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/sqaure_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61180 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46783 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/structure_pyflowline.png
+-rw-r--r--   0 runner    (1001) docker     (127)   160993 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/figures/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.774670 pyflowline-0.3.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.774670 pyflowline-0.3.9/docs/source/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/algorithm/algorithm.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.774670 pyflowline-0.3.9/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/api/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.774670 pyflowline-0.3.9/docs/source/application/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/application/application.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.774670 pyflowline-0.3.9/docs/source/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/data/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.774670 pyflowline-0.3.9/docs/source/installation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/installation/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/support.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-07 17:00:08.000000 pyflowline-0.3.9/docs/source/visualization.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.774670 pyflowline-0.3.9/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:08.000000 pyflowline-0.3.9/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-07 17:00:08.000000 pyflowline-0.3.9/examples/create_model_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.774670 pyflowline-0.3.9/pyflowline/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:08.000000 pyflowline-0.3.9/pyflowline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.774670 pyflowline-0.3.9/pyflowline/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:08.000000 pyflowline-0.3.9/pyflowline/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.774670 pyflowline-0.3.9/pyflowline/algorithms/auxiliary/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:08.000000 pyflowline-0.3.9/pyflowline/algorithms/auxiliary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16311 2024-05-07 17:00:08.000000 pyflowline-0.3.9/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-07 17:00:08.000000 pyflowline-0.3.9/pyflowline/algorithms/auxiliary/check_head_water.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-07 17:00:08.000000 pyflowline-0.3.9/pyflowline/algorithms/auxiliary/find_index_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-07 17:00:08.000000 pyflowline-0.3.9/pyflowline/algorithms/auxiliary/find_vertex_in_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.774670 pyflowline-0.3.9/pyflowline/algorithms/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:08.000000 pyflowline-0.3.9/pyflowline/algorithms/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-07 17:00:08.000000 pyflowline-0.3.9/pyflowline/algorithms/connection/connect_disconnect_flowline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.778669 pyflowline-0.3.9/pyflowline/algorithms/cython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:08.000000 pyflowline-0.3.9/pyflowline/algorithms/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/cython/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.778669 pyflowline-0.3.9/pyflowline/algorithms/direction/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/direction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/direction/correct_flowline_direction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.778669 pyflowline-0.3.9/pyflowline/algorithms/index/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/index/define_stream_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/index/define_stream_segment_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/index/define_stream_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.778669 pyflowline-0.3.9/pyflowline/algorithms/intersect/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/intersect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.778669 pyflowline-0.3.9/pyflowline/algorithms/loop/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/loop/remove_flowline_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.778669 pyflowline-0.3.9/pyflowline/algorithms/merge/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/merge/merge_flowline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.778669 pyflowline-0.3.9/pyflowline/algorithms/simplification/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/simplification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/simplification/remove_duplicate_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/simplification/remove_duplicate_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/simplification/remove_returning_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/simplification/remove_small_river.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.782669 pyflowline-0.3.9/pyflowline/algorithms/split/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/split/find_flowline_confluence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/split/find_flowline_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/split/split_by_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/split/split_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/algorithms/split/split_flowline_to_edge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.786669 pyflowline-0.3.9/pyflowline/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/_hpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/_visual_basin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62019 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/basin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/dggrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/hexagon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/latlon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/mpas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59416 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/pycase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/square.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/tin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/classes/vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.786669 pyflowline-0.3.9/pyflowline/configuration/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/configuration/change_json_key_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/configuration/create_template_configuration_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/configuration/path_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/configuration/read_configuration_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.790669 pyflowline-0.3.9/pyflowline/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/formats/convert_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/formats/convert_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/formats/convert_flowline_to_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/formats/export_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/formats/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/formats/export_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11769 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/formats/read_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/formats/read_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/formats/read_nhdplus_flowline_shapefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.790669 pyflowline-0.3.9/pyflowline/mesh/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.790669 pyflowline-0.3.9/pyflowline/mesh/dggrid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/mesh/dggrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/mesh/dggrid/create_dggrid_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.790669 pyflowline-0.3.9/pyflowline/mesh/hexagon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/mesh/hexagon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28451 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/mesh/hexagon/create_hexagon_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.790669 pyflowline-0.3.9/pyflowline/mesh/latlon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/mesh/latlon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/mesh/latlon/create_latlon_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.790669 pyflowline-0.3.9/pyflowline/mesh/mpas/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/mesh/mpas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23224 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/mesh/mpas/create_mpas_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.790669 pyflowline-0.3.9/pyflowline/mesh/square/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/mesh/square/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15367 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/mesh/square/create_square_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.790669 pyflowline-0.3.9/pyflowline/mesh/tin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/mesh/tin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyflowline/mesh/tin/create_tin_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.790669 pyflowline-0.3.9/pyflowline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-05-07 17:00:14.000000 pyflowline-0.3.9/pyflowline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-07 17:00:14.000000 pyflowline-0.3.9/pyflowline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:00:14.000000 pyflowline-0.3.9/pyflowline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 17:00:14.000000 pyflowline-0.3.9/pyflowline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 17:00:14.000000 pyflowline-0.3.9/pyflowline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 17:00:09.000000 pyflowline-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-07 17:00:14.794669 pyflowline-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-07 17:00:09.000000 pyflowline-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:00:14.790669 pyflowline-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-07 17:00:09.000000 pyflowline-0.3.9/tests/TestPathManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-07 17:00:09.000000 pyflowline-0.3.9/tests/test_installation.py
```

### Comparing `pyflowline-0.3.8/CONTRIBUTING.rst` & `pyflowline-0.3.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/LICENSE` & `pyflowline-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/PKG-INFO` & `pyflowline-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflowline
-Version: 0.3.8
+Version: 0.3.9
 Summary: A mesh-independent river network generator for hydrologic models
 Home-page: https://github.com/changliao1025/pyflowline
 Author: Chang Liao
 Author-email: chang.liao@pnnl.gov
 License: custom
 Keywords: Earth Science
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyflowline-0.3.8/README.md` & `pyflowline-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/Makefile` & `pyflowline-0.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/after_loop.png` & `pyflowline-0.3.9/docs/figures/after_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/after_merge.png` & `pyflowline-0.3.9/docs/figures/after_merge.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/basic_element.png` & `pyflowline-0.3.9/docs/figures/basic_element.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/before_loop.png` & `pyflowline-0.3.9/docs/figures/before_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/before_merge.png` & `pyflowline-0.3.9/docs/figures/before_merge.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/disconnect_flowline.png` & `pyflowline-0.3.9/docs/figures/disconnect_flowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/find_vertex.png` & `pyflowline-0.3.9/docs/figures/find_vertex.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/flow_direction.png` & `pyflowline-0.3.9/docs/figures/flow_direction.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/flow_direction_matrix.png` & `pyflowline-0.3.9/docs/figures/flow_direction_matrix.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/hexagon.png` & `pyflowline-0.3.9/docs/figures/hexagon.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/hexagon_intersect.png` & `pyflowline-0.3.9/docs/figures/hexagon_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/lat_lon.png` & `pyflowline-0.3.9/docs/figures/lat_lon.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/lat_lon_intersect.png` & `pyflowline-0.3.9/docs/figures/lat_lon_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/merge_flowline.png` & `pyflowline-0.3.9/docs/figures/merge_flowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/meshes.png` & `pyflowline-0.3.9/docs/figures/meshes.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/remove_loop.png` & `pyflowline-0.3.9/docs/figures/remove_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/remove_loop_matrix.png` & `pyflowline-0.3.9/docs/figures/remove_loop_matrix.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/simplification01.png` & `pyflowline-0.3.9/docs/figures/simplification01.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/small_river.png` & `pyflowline-0.3.9/docs/figures/small_river.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/sqaure_intersect.png` & `pyflowline-0.3.9/docs/figures/sqaure_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/square.png` & `pyflowline-0.3.9/docs/figures/square.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/structure_pyflowline.png` & `pyflowline-0.3.9/docs/figures/structure_pyflowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/figures/workflow.png` & `pyflowline-0.3.9/docs/figures/workflow.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/make.bat` & `pyflowline-0.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/source/algorithm/algorithm.rst` & `pyflowline-0.3.9/docs/source/algorithm/algorithm.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/source/api/api.rst` & `pyflowline-0.3.9/docs/source/api/api.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/source/application/application.rst` & `pyflowline-0.3.9/docs/source/application/application.rst`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 The example `run_simulation_mpas.py` script import a few packages and functions.
 
 ::
 
     import os, sys
     from pathlib import Path
     from os.path import realpath
-    from pyflowline.pyflowline_read_model_configuration_file import pyflowline_read_model_configuration_file
+    from pyflowline.configuration.read_configuration_file import pyflowline_read_configuration_file
 
-The `pyflowline_read_model_configuration_file` function reads in a JSON configuration file and loads all the necessary model parameters. 
+The `pyflowline_read_configuration_file` function reads in a JSON configuration file and loads all the necessary model parameters. 
 
 
 ================
 Step 2
 ================
 
 The script sets up some paths, which should be adjusted based on a real case and your local directory structure.
@@ -51,30 +51,30 @@
 
 ::   
 
     sFilename_configuration_in = realpath( sPath_parent +  '/examples/susquehanna/pyflowline_susquehanna_mpas.json' )
     if os.path.isfile(sFilename_configuration_in):
         pass
     else:
-        print('This configuration does not exist: ', sFilename_configuration_in )
+        print('The domain configuration file does not exist: ',sFilename_configuration_in )
 
 ================
 Step 4
 ================
 
 Set up case information and read the configuration file.
 
 ::   
 
     iCase_index = 17
     Mesh = 'mpas'
     Date='20220901'
 
 
-    oPyflowline = pyflowline_read_model_configuration_file(sFilename_configuration_in, \
+    oPyflowline = pyflowline_read_configuration_file(sFilename_configuration_in, \
        iCase_index_in=iCase_index, sDate_in=sDate)
     oPyflowline.aBasin[0].dLatitude_outlet_degree=39.462000
     oPyflowline.aBasin[0].dLongitude_outlet_degree=-76.009300
 
 ================
 Step 5
 ================
```

### Comparing `pyflowline-0.3.8/docs/source/conf.py` & `pyflowline-0.3.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/source/data/data.rst` & `pyflowline-0.3.9/docs/source/data/data.rst`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 PyFlowline uses two JSON-format configuration files to manage all input information, where major model input parameters and paths are specified. These configuration files have a parent-child relationship:
 
 1. The parent configuration file stores parameters for the entire domain.
 2. The child configuration file stores parameters for each individual watershed.
 
 These files serve as the entry point for setting up and running a PyFlowline case. They can exist wherever the user prefers, but PyFlowline uses the paths specified in these files to locate model inputs and write outputs. Model inputs, outputs, and a recommended directory structure are described in the following two sections.
 
-To create a new PyFlowline case, pass the full path to the parent configuration file to the `pyflowline_read_model_configuration_file` function. This will return a PyFlowline object configured with the values from the file, and it can be used to run the model. See the example notebooks for a demonstration.
+To create a new PyFlowline case, pass the full path to the parent configuration file to the `pyflowline_read_configuration_file` function. This will return a PyFlowline object configured with the values from the file, and it can be used to run the model. See the example notebooks for a demonstration.
 
 Note that the "parent" configuration file contains one block of parameter-value pairs that apply to the entire domain. In contrast, the "child" configuration file contains one block of parameter-value pairs for each watershed. A domain with a single watershed will have a single block in the "child" configuration file, while a domain with multiple watersheds will have multiple blocks.
 
 An example parent JSON file for the Susquehanna River Basin domain (with <domain_name> as "susquehanna") is provided below:
 
 ::
```

### Comparing `pyflowline-0.3.8/docs/source/faq.rst` & `pyflowline-0.3.9/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/source/glossary.rst` & `pyflowline-0.3.9/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/source/index.rst` & `pyflowline-0.3.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/source/installation/installation.rst` & `pyflowline-0.3.9/docs/source/installation/installation.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/source/quickstart.rst` & `pyflowline-0.3.9/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/docs/source/readme.rst` & `pyflowline-0.3.9/docs/source/readme.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/examples/create_model_configuration.py` & `pyflowline-0.3.9/examples/create_model_configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from pathlib import Path
 from os.path import realpath
 import argparse
 
-from pyflowline.pyflowline_create_template_configuration_file import pyflowline_create_template_configuration_file
+from pyflowline.configuration.pyflowline_create_template_configuration_file import pyflowline_create_template_configuration_file
 
 parser = argparse.ArgumentParser()
 parser.add_argument("--sMesh_type", help = "sMesh_type",  type = str)
 parser.add_argument("--iCase_index", help = "iCase_index",  type = int)
 parser.add_argument("--dResolution_meter", help = "dResolution_meter",  type = float)
 parser.add_argument("--sDate", help = "sDate",  type = str)
 
@@ -33,15 +33,15 @@
 sPath = str( Path().resolve() )
 
 sWorkspace_data = realpath( sPath +  '/data/susquehanna' )
 sWorkspace_input =  str(Path(sWorkspace_data)  /  'input')
 sWorkspace_output=  str(Path(sWorkspace_data)  /  'output')
 
 sFilename_configuration_in = realpath( sPath +  '/tests/configurations/template.json' )
-    
+
 oPyflowline = pyflowline_create_template_configuration_file(sFilename_configuration_in,\
          sWorkspace_input, sWorkspace_output, iFlag_use_mesh_dem_in = 1,sMesh_type_in=sMesh_type, iCase_index_in = iCase_index, sDate_in = sDate)
-    
+
 print(oPyflowline.tojson())
 
 print('Finished')
```

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py` & `pyflowline-0.3.9/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/auxiliary/check_head_water.py` & `pyflowline-0.3.9/pyflowline/algorithms/auxiliary/check_head_water.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/auxiliary/find_index_in_list.py` & `pyflowline-0.3.9/pyflowline/algorithms/auxiliary/find_index_in_list.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/auxiliary/find_vertex_in_list.py` & `pyflowline-0.3.9/pyflowline/algorithms/auxiliary/find_vertex_in_list.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/connection/connect_disconnect_flowline.py` & `pyflowline-0.3.9/pyflowline/algorithms/connection/connect_disconnect_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/direction/correct_flowline_direction.py` & `pyflowline-0.3.9/pyflowline/algorithms/direction/correct_flowline_direction.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/index/define_stream_order.py` & `pyflowline-0.3.9/pyflowline/algorithms/index/define_stream_order.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/index/define_stream_segment_index.py` & `pyflowline-0.3.9/pyflowline/algorithms/index/define_stream_segment_index.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/index/define_stream_topology.py` & `pyflowline-0.3.9/pyflowline/algorithms/index/define_stream_topology.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py` & `pyflowline-0.3.9/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py` & `pyflowline-0.3.9/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py` & `pyflowline-0.3.9/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/loop/remove_flowline_loop.py` & `pyflowline-0.3.9/pyflowline/algorithms/loop/remove_flowline_loop.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/merge/merge_flowline.py` & `pyflowline-0.3.9/pyflowline/algorithms/merge/merge_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/simplification/remove_returning_flowline.py` & `pyflowline-0.3.9/pyflowline/algorithms/simplification/remove_returning_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/simplification/remove_small_river.py` & `pyflowline-0.3.9/pyflowline/algorithms/simplification/remove_small_river.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/split/find_flowline_confluence.py` & `pyflowline-0.3.9/pyflowline/algorithms/split/find_flowline_confluence.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/split/find_flowline_vertex.py` & `pyflowline-0.3.9/pyflowline/algorithms/split/find_flowline_vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/split/split_by_length.py` & `pyflowline-0.3.9/pyflowline/algorithms/split/split_by_length.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/split/split_flowline.py` & `pyflowline-0.3.9/pyflowline/algorithms/split/split_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/algorithms/split/split_flowline_to_edge.py` & `pyflowline-0.3.9/pyflowline/algorithms/split/split_flowline_to_edge.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/_hpc.py` & `pyflowline-0.3.9/pyflowline/classes/_hpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 
     sFilename_pyflowline = os.path.join(
         str(Path(self.sWorkspace_output)), "run_pyflowline.py")
     ofs_pyflowline = open(sFilename_pyflowline, 'w')
 
     sLine = '#!/qfs/people/liao313/.conda/envs/pyflowline/bin/' + 'python3' + '\n'
     ofs_pyflowline.write(sLine)
-    sLine = 'from pyflowline.pyflowline_read_model_configuration_file import pyflowline_read_model_configuration_file' + '\n'
+    sLine = 'from pyflowline.configuration.read_configuration_file import pyflowline_read_configuration_file' + '\n'
     ofs_pyflowline.write(sLine)
     sLine = 'sFilename_configuration_in = ' + '"' + \
         self.sFilename_model_configuration + '"\n'
     ofs_pyflowline.write(sLine)
-    sLine = 'oPyflowline = pyflowline_read_model_configuration_file(sFilename_configuration_in,'\
+    sLine = 'oPyflowline = pyflowline_read_configuration_file(sFilename_configuration_in,'\
         + 'iCase_index_in=' + str(self.iCase_index) + ','\
         + 'iResolution_index_in=' + str(self.iResolution_index) + ','\
         + 'dResolution_meter_in=' + "{:0f}".format(self.dResolution_meter) + ','\
         + 'sDggrid_type_in="'+ str(self.sDggrid_type) + '",' \
         + 'sDate_in="' + str(self.sDate) + '",'\
         + 'sMesh_type_in="' + str(self.sMesh_type) + '"' + ')' + '\n'
     ofs_pyflowline.write(sLine)
```

### Comparing `pyflowline-0.3.8/pyflowline/classes/_visual.py` & `pyflowline-0.3.9/pyflowline/classes/_visual.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,35 +30,35 @@
 
     if iFlag_title_in is None:
         iFlag_title_in = 1
 
     if sVariable_in is None:
         sVariable_in = 'flowline_conceptual'
     else:
-        if sVariable_in == 'mesh': 
+        if sVariable_in == 'mesh':
             iFlag_type_in = 3
         else:
             if sVariable_in == 'overlap':
                 iFlag_type_in = 4
-    
+
 
     if iFlag_type_in == 1: #point based, such as dam
         #currently, this feature is not supported
         pass
     else:
         if iFlag_type_in == 2:
             #polyline based, only flowline
             aLegend = list()
-            sText = 'Case: ' + "{:0d}".format( int(self.iCase_index) ) 
+            sText = 'Case: ' + "{:0d}".format( int(self.iCase_index) )
             aLegend.append(sText)
             sText = 'Mesh type: ' + self.sMesh_type.title()
             aLegend.append(sText)
             sResolution =  'Resolution: ' + "{:0d}".format( int(self.dResolution_meter) ) + 'm'
-            aLegend.append(sResolution)            
-            for pBasin in self.aBasin:                
+            aLegend.append(sResolution)
+            for pBasin in self.aBasin:
                 pBasin.basin_plot(iFlag_type_in,
                                   self.sMesh_type,
                                   iFlag_title_in= iFlag_title_in,
                                   sFilename_output_in=sFilename_output_in,
                                   sVariable_in= sVariable_in,
                                   aExtent_in = aExtent_in,
                                   aLegend_in = aLegend,
@@ -82,23 +82,23 @@
 
                     pass
                 else:
                     pass
 
         return
 
-def _plot_mesh(self, 
-               sFilename_output_in=None, 
-               aExtent_in=None, 
+def _plot_mesh(self,
+               sFilename_output_in=None,
+               aExtent_in=None,
                pProjection_map_in = None):
 
-    sFilename_in = self.sFilename_mesh 
+    sFilename_in = self.sFilename_mesh
     sMesh_type = self.sMesh_type
 
-    map_vector_polygon_data(sFilename_in,
+    map_vector_polygon_data(1, sFilename_in,
                             sFilename_output_in = sFilename_output_in,
                             sTitle_in = sMesh_type,
                             aExtent_in = aExtent_in,
                             pProjection_map_in = pProjection_map_in)
 
     return
 
@@ -112,15 +112,15 @@
     aFiletype_in = list()
     aFilename_in = list()
     aFlag_color = list()
     aVariable_in = list()
     aFilename_in.append(self.sFilename_mesh)
     aFiletype_in.append(3)
     aFlag_color.append(0)
-    
+
     aVariable_in.append(None)
 
     for pBasin in self.aBasin:
         aFiletype_in.append(2)
         dummy = pBasin.sFilename_flowline_conceptual
         sFilename_json = os.path.join(pBasin.sWorkspace_output_basin, dummy)
         aFilename_in.append(sFilename_json)
```

### Comparing `pyflowline-0.3.8/pyflowline/classes/_visual_basin.py` & `pyflowline-0.3.9/pyflowline/classes/_visual_basin.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/basin.py` & `pyflowline-0.3.9/pyflowline/classes/basin.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/confluence.py` & `pyflowline-0.3.9/pyflowline/classes/confluence.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/dggrid.py` & `pyflowline-0.3.9/pyflowline/classes/dggrid.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/edge.py` & `pyflowline-0.3.9/pyflowline/classes/edge.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/flowline.py` & `pyflowline-0.3.9/pyflowline/classes/flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/hexagon.py` & `pyflowline-0.3.9/pyflowline/classes/hexagon.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/latlon.py` & `pyflowline-0.3.9/pyflowline/classes/latlon.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/link.py` & `pyflowline-0.3.9/pyflowline/classes/link.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/mpas.py` & `pyflowline-0.3.9/pyflowline/classes/mpas.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/pycase.py` & `pyflowline-0.3.9/pyflowline/classes/pycase.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,48 +27,48 @@
 from pyearth.gis.spatialref.conversion_between_degree_and_meter  import degree_to_meter
 from pyearth.gis.spatialref.conversion_between_degree_and_meter  import meter_to_degree
 from pyearth.gis.gdal.read.raster.gdal_read_geotiff_file import gdal_read_geotiff_file
 from pyearth.gis.gdal.read.vector.gdal_read_geojson_boundary import gdal_read_geojson_boundary
 from pyearth.gis.spatialref.get_utm_spatial_reference import get_utm_spatial_reference
 from pyearth.toolbox.data.geoparquet.convert_geojson_to_geoparquet import convert_geojson_to_geoparquet
 
-iFlag_kml = importlib.util.find_spec("simplekml") 
+iFlag_kml = importlib.util.find_spec("simplekml")
 
 
-iFlag_cython = importlib.util.find_spec("cython") 
+iFlag_cython = importlib.util.find_spec("cython")
 if iFlag_cython is not None:
     from pyflowline.external.tinyr.tinyr.tinyr import RTree
     iFlag_use_rtree = 1
 else:
     iFlag_use_rtree =0
     pass
 
 from pyflowline.mesh.hexagon.create_hexagon_mesh import create_hexagon_mesh
 from pyflowline.mesh.latlon.create_latlon_mesh import create_latlon_mesh
 from pyflowline.mesh.square.create_square_mesh import create_square_mesh
 from pyflowline.mesh.mpas.create_mpas_mesh import create_mpas_mesh
 from pyflowline.mesh.dggrid.create_dggrid_mesh import create_dggrid_mesh
 from pyflowline.mesh.dggrid.create_dggrid_mesh import dggrid_find_resolution_by_index
 from pyflowline.mesh.tin.create_tin_mesh import create_tin_mesh
-gdal.UseExceptions()   
+gdal.UseExceptions()
 pDate = datetime.datetime.today()
 sDate_default = "{:04d}".format(pDate.year) + "{:02d}".format(pDate.month) + "{:02d}".format(pDate.day)
 
 class CaseClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         if isinstance(obj, list):
             pass
         if isinstance(obj, pyvertex):
-            return json.loads(obj.tojson()) 
+            return json.loads(obj.tojson())
         if isinstance(obj, pyedge):
             return obj.lEdgeID
         if isinstance(obj, pyflowline):
             return obj.lFlowlineID
         if isinstance(obj, pyhexagon):
             return obj.lCellID
         if isinstance(obj, pysquare):
@@ -244,15 +244,15 @@
             self.iFlag_rotation = int(aConfig_in['iFlag_rotation'])
 
 
         if 'iFlag_intersect' in aConfig_in:
             self.iFlag_intersect = int(aConfig_in['iFlag_intersect'])
         else:
             self.iFlag_intersect=1
-        
+
         if self.iFlag_flowline == 1:
             pass
         else:
             self.iFlag_intersect=0
 
         if 'iFlag_break_by_distance' in aConfig_in:
             self.iFlag_break_by_distance = int(aConfig_in['iFlag_break_by_distance'])
@@ -264,40 +264,40 @@
         else:
             self.iFlag_dggrid=0
 
         if 'iResolution_index' in aConfig_in:
             self.iResolution_index = int(aConfig_in['iResolution_index'])
         else:
             self.iResolution_index=10
-        
+
         if 'sDggrid_type' in aConfig_in:
             self.sDggrid_type = aConfig_in['sDggrid_type']
         else:
             self.sDggrid_type='ISEA3H'
 
         if 'nOutlet' in aConfig_in:
             self.nOutlet = int(aConfig_in['nOutlet'])
 
         if 'iCase_index' in aConfig_in:
             iCase_index = int(aConfig_in['iCase_index'])
         else:
             iCase_index = 1
-        
+
         sCase_index = "{:03d}".format( iCase_index )
         self.iCase_index =   iCase_index
 
         if 'dResolution_degree' in aConfig_in:
             self.dResolution_degree = float(aConfig_in['dResolution_degree'])
 
         if 'dResolution_meter' in aConfig_in:
             self.dResolution_meter = float(aConfig_in['dResolution_meter'])
         else:
             print('Please specify resolution.')
 
-        
+
 
         if 'dThreshold_break_by_distance' in aConfig_in:
             self.dThreshold_break_by_distance = float(aConfig_in['dThreshold_break_by_distance'])
 
         if 'dLongitude_left' in aConfig_in:
             self.dLongitude_left = float(aConfig_in['dLongitude_left'])
 
@@ -324,15 +324,15 @@
 
         if 'sFilename_spatial_reference' in aConfig_in:
             self.sFilename_spatial_reference = aConfig_in['sFilename_spatial_reference']
 
 
         if 'sFilename_dem' in aConfig_in:
             self.sFilename_dem = aConfig_in['sFilename_dem']
-        
+
         if self.iFlag_dggrid == 1:
             if 'sFilename_dggrid' in aConfig_in:
                 self.sFilename_dggrid = aConfig_in['sFilename_dggrid']
                 if not os.path.isfile(self.sFilename_dggrid ):
                     print("The dggrid binary file does not exist, you need to update this parameter before running the model!")
                     #exit()
                 pass
@@ -406,15 +406,15 @@
                                 self.iMesh_type = 6
                             else:
                                 print('Unsupported mesh type?')
 
         if self.iMesh_type == 5:
             #update resolution
             self.dResolution_meter = dggrid_find_resolution_by_index(self.sDggrid_type, self.iResolution_index)
-            
+
         #the model can be run as part of hexwatershed or standalone
         if self.iFlag_standalone == 1:
             #in standalone case, will add case information and update output path
             sPath = str(Path(self.sWorkspace_output)  /  sCase)
             self.sWorkspace_output = sPath
         else:
             #use specified output path, also do not add output or input tag
@@ -440,30 +440,30 @@
                     with open(self.sFilename_basins) as json_file:
                         dummy_data = json.load(json_file)
                         for i in range(self.nOutlet):
                             sBasin =  "{:08d}".format(i+1)
                             dummy_basin = dummy_data[i]
                             dummy_basin['sWorkspace_output_basin'] = str(Path(self.sWorkspace_output) / sBasin )
                             pBasin = pybasin(dummy_basin)
-                            self.aBasin.append(pBasin)    
+                            self.aBasin.append(pBasin)
                 else:
                     print('This basin configuration file does not exist: ', self.sFilename_basins )
                     print('Please update this parameter before running the model!')
                     #exit()
-                    
-                
+
+
             else:
                 pass
         else:
-            
+
             pass
 
 
         #model generated files
-        
+
         self.sFilename_mesh = os.path.join(str(Path(self.sWorkspace_output)  ) , sMesh_type + ".geojson" )
         self.sFilename_mesh_info= os.path.join(str(Path(self.sWorkspace_output)  ) , sMesh_type + "_mesh_info.json"  )
         self.sFilename_mesh_kml = os.path.join(str(Path(self.sWorkspace_output)  ) , sMesh_type + ".kml" ) #for google service
 
         return
 
 
@@ -500,45 +500,45 @@
         """
         print('Start mesh generation.')
         if iFlag_antarctic_in is None:
             iFlag_antarctic = 0
         else:
             iFlag_antarctic = iFlag_antarctic_in
 
-     
+
         if self.iFlag_create_mesh ==1:
             iFlag_global =  self.iFlag_global
             iMesh_type = self.iMesh_type
             iFlag_save_mesh = self.iFlag_save_mesh
             iFlag_rotation = self.iFlag_rotation
             iFlag_mesh_boundary = self.iFlag_mesh_boundary
             dResolution_degree = self.dResolution_degree
             dResolution_meter = self.dResolution_meter
             sFilename_dem = self.sFilename_dem
             sFilename_spatial_reference = self.sFilename_spatial_reference
-            sFilename_mesh = self.sFilename_mesh 
+            sFilename_mesh = self.sFilename_mesh
 
             if iFlag_global ==1: #a global mesh does not require boundary
                 pass
             else:
 
                 if iFlag_mesh_boundary ==1:
                     #create a polygon based on real boundary
-                    pBoundary_wkt, aExtent = gdal_read_geojson_boundary(self.sFilename_mesh_boundary)           
+                    pBoundary_wkt, aExtent = gdal_read_geojson_boundary(self.sFilename_mesh_boundary)
 
                     if iMesh_type != 4: #not mpas
                         spatial_reference_target = osr.SpatialReference()
                         spatial_reference_target.ImportFromEPSG(4326)
 
                         #check whether DEM exists
                         if os.path.isfile(sFilename_dem):
                             #dPixelWidth, pPixelHeight, dOriginX, dOriginY, nrow, ncolumn, pSpatialRef_dem, pProjection, pGeotransform\
                             #    = retrieve_geotiff_metadata(sFilename_dem)
                             dummy = gdal_read_geotiff_file(sFilename_dem, iFlag_metadata_only= 1)
-                            dPixelWidth = dummy['pixelWidth']                        
+                            dPixelWidth = dummy['pixelWidth']
                             pPixelHeight = dummy['pixelHeight']
                             dOriginX = dummy['originX']
                             dOriginY = dummy['originY']
                             nrow = dummy['nrow']
                             ncolumn = dummy['ncolumn']
                             pSpatialRef_dem = dummy['spatialReference']
                             #pProjection= dummy['projection']
@@ -617,15 +617,15 @@
                     if iMesh_type != 4: #mpas
                         spatial_reference_target = osr.SpatialReference()
                         spatial_reference_target.ImportFromEPSG(4326)
 
                         #check whether DEM exists
                         if os.path.isfile(sFilename_dem):
                             dummy = gdal_read_geotiff_file(sFilename_dem, iFlag_metadata_only= 1)
-                            dPixelWidth = dummy['pixelWidth']                        
+                            dPixelWidth = dummy['pixelWidth']
                             pPixelHeight = dummy['pixelHeight']
                             dOriginX = dummy['originX']
                             dOriginY = dummy['originY']
                             nrow = dummy['nrow']
                             ncolumn = dummy['ncolumn']
                             pSpatialRef_dem = dummy['spatialReference']
                             pProjection= dummy['projection']
@@ -690,15 +690,15 @@
                     ncolumn= int( (dX_lowerright - dX_lowerleft) / dX_spacing )+1
                     nrow= int( (dY_upperleft - dY_lowerleft) / dY_spacing )
 
                 if iFlag_mesh_boundary ==1:
                     #create a polygon based on real boundary
                     pBoundary_wkt, aExtent = gdal_read_geojson_boundary(self.sFilename_mesh_boundary)
 
-                    aHexagon = create_hexagon_mesh(iFlag_rotation, dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, 
+                    aHexagon = create_hexagon_mesh(iFlag_rotation, dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow,
                                                    sFilename_mesh, sFilename_spatial_reference, pBoundary_wkt)
                     pass
                 else:
                     pRing = ogr.Geometry(ogr.wkbLinearRing)
                     pRing.AddPoint(dLongitude_left, dLatitude_top)
                     pRing.AddPoint(dLongitude_right, dLatitude_top)
                     pRing.AddPoint(dLongitude_right, dLatitude_bot)
@@ -706,79 +706,79 @@
                     pRing.AddPoint(dLongitude_left, dLatitude_top)
                     pBoundary = ogr.Geometry(ogr.wkbPolygon)
                     pBoundary.AddGeometry(pRing)
                     pBoundary_wkt = pBoundary.ExportToWkt() #wkt format
 
                     aHexagon = create_hexagon_mesh(iFlag_rotation, dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow,
                                                    sFilename_mesh, sFilename_spatial_reference, pBoundary_wkt)
-                    
-                    
+
+
                     pass
 
-                
+
 
                 self.aCell = aHexagon
             else:
                 if iMesh_type ==2: #sqaure
                     ncolumn= int( (dX_lowerright - dX_lowerleft) / dResolution_meter )
                     nrow= int( (dY_upperleft - dY_lowerleft) / dResolution_meter )
                     if iFlag_mesh_boundary ==1:
                         #create a polygon based on real boundary
                         pBoundary_wkt, aExtent= gdal_read_geojson_boundary(self.sFilename_mesh_boundary)
 
-                        aSquare = create_square_mesh(dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, 
+                        aSquare = create_square_mesh(dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow,
                                                      sFilename_mesh, sFilename_spatial_reference, pBoundary_wkt)
                         pass
                     else:
                         pRing = ogr.Geometry(ogr.wkbLinearRing)
                         pRing.AddPoint(dLongitude_left, dLatitude_top)
                         pRing.AddPoint(dLongitude_right, dLatitude_top)
                         pRing.AddPoint(dLongitude_right, dLatitude_bot)
                         pRing.AddPoint(dLongitude_left, dLatitude_bot)
                         pRing.AddPoint(dLongitude_left, dLatitude_top)
                         pBoundary = ogr.Geometry(ogr.wkbPolygon)
                         pBoundary.AddGeometry(pRing)
-                        pBoundary_wkt = pBoundary.ExportToWkt() 
-                        aSquare = create_square_mesh(dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow, 
+                        pBoundary_wkt = pBoundary.ExportToWkt()
+                        aSquare = create_square_mesh(dX_lowerleft, dY_lowerleft, dResolution_meter, ncolumn, nrow,
                                                      sFilename_mesh, sFilename_spatial_reference, pBoundary_wkt)
                         pass
-                    
+
                     self.aCell = aSquare
                 else:
                     if iMesh_type ==3: #latlon
                         dResolution_meter = degree_to_meter(dLatitude_mean, dResolution_degree)
                         dArea = np.power(dResolution_meter,2.0)
                         ncolumn= int( (dLongitude_right - dLongitude_left) / dResolution_degree )
                         nrow= int( (dLatitude_top - dLatitude_bot) / dResolution_degree )
 
                         if iFlag_mesh_boundary ==1:
                             #create a polygon based on real boundary
                             #already produced
                             pBoundary_wkt , aExtent= gdal_read_geojson_boundary(self.sFilename_mesh_boundary)
-                            aLatlon = create_latlon_mesh(dLongitude_left, dLatitude_bot, dResolution_degree, ncolumn, nrow, 
+                            aLatlon = create_latlon_mesh(dLongitude_left, dLatitude_bot, dResolution_degree, ncolumn, nrow,
                                                          sFilename_mesh, pBoundary_wkt)
                             pass
                         else:
                             pRing = ogr.Geometry(ogr.wkbLinearRing)
                             pRing.AddPoint(dLongitude_left, dLatitude_top)
                             pRing.AddPoint(dLongitude_right, dLatitude_top)
                             pRing.AddPoint(dLongitude_right, dLatitude_bot)
                             pRing.AddPoint(dLongitude_left, dLatitude_bot)
                             pRing.AddPoint(dLongitude_left, dLatitude_top)
                             pBoundary = ogr.Geometry(ogr.wkbPolygon)
                             pBoundary.AddGeometry(pRing)
-                            pBoundary_wkt =  pBoundary.ExportToWkt() 
+                            pBoundary_wkt =  pBoundary.ExportToWkt()
                             aLatlon = create_latlon_mesh(dLongitude_left, dLatitude_bot, dResolution_degree, ncolumn, nrow, \
                                                          sFilename_mesh, pBoundary_wkt)
 
                             pass
-                    
+
                         self.aCell = aLatlon
 
-                        
+
                     else:
                         if iMesh_type == 4: #mpas
                             iFlag_use_mesh_dem = self.iFlag_use_mesh_dem
                             sFilename_mesh_netcdf = self.sFilename_mesh_netcdf
                             dLatitude_top    = self.dLatitude_top
                             dLatitude_bot    = self.dLatitude_bot
                             dLongitude_left  = self.dLongitude_left
@@ -803,65 +803,65 @@
                                     pRing.AddPoint(dLongitude_left, dLatitude_top)
                                     pRing.AddPoint(dLongitude_right, dLatitude_top)
                                     pRing.AddPoint(dLongitude_right, dLatitude_bot)
                                     pRing.AddPoint(dLongitude_left, dLatitude_bot)
                                     pRing.AddPoint(dLongitude_left, dLatitude_top)
                                     pBoundary = ogr.Geometry(ogr.wkbPolygon)
                                     pBoundary.AddGeometry(pRing)
-                                    pBoundary_wkt =  pBoundary.ExportToWkt() 
+                                    pBoundary_wkt =  pBoundary.ExportToWkt()
 
                                     #new method using polygon object
-                                    aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh, 
+                                    aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh,
                                                              sFilename_mesh_netcdf, sFilename_mesh, iFlag_antarctic_in= iFlag_antarctic_in, pBoundary_in = pBoundary_wkt  )
                                     pass
 
                             self.aCell = aMpas
                         else:
                             if iMesh_type == 5: #dggrid
                                 dLatitude_top    = self.dLatitude_top
                                 dLatitude_bot    = self.dLatitude_bot
                                 dLongitude_left  = self.dLongitude_left
-                                dLongitude_right = self.dLongitude_right                                
-                                
+                                dLongitude_right = self.dLongitude_right
+
 
                                 if self.iFlag_standalone == 1:
                                     sWorkspace_output = self.sWorkspace_output + slash + 'dggrid'
                                     pass
                                 else:
                                     sWorkspace_output = self.sWorkspace_output + slash + '..'+ slash + 'dggrid'
-                                    
+
                                     sWorkspace_output = os.path.abspath(sWorkspace_output)
                                     pass
 
                                 if not os.path.exists(sWorkspace_output):
                                     os.makedirs(sWorkspace_output)
-                                
+
                                 if iFlag_mesh_boundary ==1:
-                                        #create a polygon based on                                   
+                                        #create a polygon based on
 
                                     aDggrid = create_dggrid_mesh(iFlag_global,
                                                                      iFlag_save_mesh,
                                                                      sFilename_mesh,
                                                                      sWorkspace_output,
                                                                      iResolution_index_in= self.iResolution_index,
                                                                      iFlag_antarctic_in=iFlag_antarctic_in,
                                                                      sDggrid_type_in = self.sDggrid_type,
                                                                      sFilename_boundary_in = self.sFilename_mesh_boundary)
-                                    
-                                    
-                                                                     
+
+
+
                                     pass
-                                else:                                       
+                                else:
                                     aDggrid = create_dggrid_mesh(iFlag_global,
-                                                                     iFlag_save_mesh,                                                                   
+                                                                     iFlag_save_mesh,
                                                                      sFilename_mesh,
                                                                      sWorkspace_output,
                                                                       iResolution_index_in= self.iResolution_index,
                                                                           sDggrid_type_in = self.sDggrid_type)
-                                    
+
                                     pass
 
 
                                 self.aCell = aDggrid
 
                             else:
                                 if iMesh_type == 6: #tin this one need to be updated because central location issue
@@ -879,27 +879,27 @@
                                     self.aCell = aTin
                                 else:
 
                                     print('Unsupported mesh type?')
                                 return
 
             #no matter what type of mash, we will convert it to geoparquet for easy visualization
-            convert_geojson_to_geoparquet(sFilename_mesh, sFilename_mesh.replace('.geojson','.parquet'))    
-        else:            
+            convert_geojson_to_geoparquet(sFilename_mesh, sFilename_mesh.replace('.geojson','.parquet'))
+        else:
             pass
 
         #build rtree
         if iFlag_use_rtree == 1:
             interleaved = True
             self.pRTree_mesh = RTree(interleaved=interleaved, max_cap=5, min_cap=2)
-            for lCellIndex in range(len(self.aCell)):                
-                pBound = self.aCell[lCellIndex].pBound                                    
-                self.pRTree_mesh.insert(lCellIndex, pBound)  #  
+            for lCellIndex in range(len(self.aCell)):
+                pBound = self.aCell[lCellIndex].pBound
+                self.pRTree_mesh.insert(lCellIndex, pBound)  #
+
 
-        
         print('Finish mesh generation.')
         return self.aCell
 
     def pyflowline_reconstruct_topological_relationship(self):
         """
         The topological relationship reconstruction operation
 
@@ -908,46 +908,46 @@
 
         Returns:
             tuple [list [pycell], list [pyflowline], list [long]]: A list of cells, flowlines, and outlet cell IDs.
         """
         print('Start topology reconstruction.')
         iFlag_intersect = self.iFlag_intersect
         if iFlag_intersect == 1:
-            iMesh_type = self.iMesh_type 
-            sFilename_mesh=self.sFilename_mesh         
+            iMesh_type = self.iMesh_type
+            sFilename_mesh=self.sFilename_mesh
             aFlowline_conceptual = list()   #store all the flowline
             aCellID_outlet = list()
             aBasin = list()
             aCell_intersect=list()
             ncell=len(self.aCell)
-            #there is a one-to-one match between cell id and cell center because each cell has only one center                  
-            
+            #there is a one-to-one match between cell id and cell center because each cell has only one center
+
             for pBasin in self.aBasin:
                 aCell_intersect_basin = pBasin.basin_reconstruct_topological_relationship(iMesh_type,sFilename_mesh)
                 aFlowline_conceptual = aFlowline_conceptual + pBasin.aFlowline_basin_conceptual
                 aBasin.append(pBasin)
                 aCellID_outlet.append(pBasin.lCellID_outlet)
                 aCell_intersect = aCell_intersect + aCell_intersect_basin
                 if iFlag_use_rtree == 1:
                     #use rtree to update topology and length
-                    for pFlowline in pBasin.aFlowline_basin_conceptual:                    
+                    for pFlowline in pBasin.aFlowline_basin_conceptual:
                         iStream_segment = pFlowline.iStream_segment
-                        iStream_order = pFlowline.iStream_order                    
+                        iStream_order = pFlowline.iStream_order
                         for pEdge in pFlowline.aEdge:
                             pVertex_start = pEdge.pVertex_start
                             pVertex_end = pEdge.pVertex_end
                             pBound = pEdge.pBound
                             aIntersect = list(self.pRTree_mesh.search(pBound))
                             for k in aIntersect:
                                 pCell = self.aCell[k]
                                 if pVertex_start.calculate_distance(pCell.pVertex_center) < 1.0E-6:
                                     self.aCell[k].iStream_segment_burned = iStream_segment
                                     self.aCell[k].iStream_order_burned = iStream_order
                                     lCellIndex_upstream = k
-                                
+
                                 if pVertex_end.calculate_distance(pCell.pVertex_center) < 1.0E-6:
                                     self.aCell[k].iStream_segment_burned = iStream_segment
                                     self.aCell[k].iStream_order_burned = iStream_order
                                     lCellIndex_downstream = k
 
                             self.aCell[lCellIndex_upstream].lCellID_downstream_burned = self.aCell[lCellIndex_downstream].lCellID
 
@@ -956,20 +956,20 @@
                         aIntersect = list(self.pRTree_mesh.search(pBound))
                         for k in aIntersect:
                             pCell = self.aCell[k]
                             if pCell2.lCellID == pCell.lCellID:
                                 pCell.dLength_flowline = pCell2.dLength_flowline
                         pass
                 else:
-                    #set topology here               
-                    for pFlowline in pBasin.aFlowline_basin_conceptual:                    
+                    #set topology here
+                    for pFlowline in pBasin.aFlowline_basin_conceptual:
                         iStream_segment = pFlowline.iStream_segment
-                        iStream_order = pFlowline.iStream_order                    
+                        iStream_order = pFlowline.iStream_order
                         for pEdge in pFlowline.aEdge:
-                            try:                            
+                            try:
                                 pVertex_start = pEdge.pVertex_start
                                 pVertex_end = pEdge.pVertex_end
                                 iFlag_found_start = 0
                                 for k in range(ncell):
                                     pVertex_center = self.aCell[k].pVertex_center
                                     if pVertex_center == pVertex_start:
                                         iFlag_found_start = 1
@@ -996,15 +996,15 @@
                                 print("error in step")
                                 print(pFlowline.tojson())
                                 print(pEdge.tojson())
                                 print(pVertex_start.tojson())
                                 print(pVertex_end.tojson())
                                 pass
 
-                    #update length using rtree            
+                    #update length using rtree
                     for pCell in self.aCell:
                         for pCell2 in aCell_intersect_basin:
                             if pCell2.lCellID == pCell.lCellID:
                                 pCell.dLength_flowline = pCell2.dLength_flowline
 
             self.aFlowline_conceptual = aFlowline_conceptual
             self.aCellID_outlet = aCellID_outlet
@@ -1053,116 +1053,116 @@
         """
         Set up the flowlinecase
         """
         system = platform.system()
         if self.iFlag_flowline == 1:
             self.pyflowline_convert_flowline_to_geojson()
             pass
-        
+
         if self.iFlag_dggrid == 1:
             #create dggrid output folder
             if self.iFlag_standalone == 1:
                 sWorkspace_output = self.sWorkspace_output + slash + 'dggrid'
             else:
                 sWorkspace_output = self.sWorkspace_output + slash + '..'+ slash + 'dggrid'
                 sWorkspace_output = os.path.abspath(sWorkspace_output)
 
-         
+
             Path(sWorkspace_output).mkdir(parents=True, exist_ok=True)
             #then copy the binary file to the folder
             #copy execulate
             if self.iFlag_user_provided_binary == 1:
                 sFilename_new = sWorkspace_output + slash + 'dggrid'
                 copy2(self.sFilename_dggrid, sFilename_new)
                 os.chmod(sFilename_new, stat.S_IREAD | stat.S_IWRITE | stat.S_IXUSR)
                 pass
-            else:      
+            else:
                 if system == 'Windows':
                     sFilename_executable = 'dggrid.exe'
                 else:
-                    sFilename_executable = 'dggrid'     
+                    sFilename_executable = 'dggrid'
 
                 #search for system wide binary in the system path
                 iFlag_found_binary = 0
                 for folder in os.environ['PATH'].split(os.pathsep):
                     sFilename_dggrid_bin = os.path.join(folder, sFilename_executable)
                     if os.path.isfile(sFilename_dggrid_bin):
                         print('Found binary at:', sFilename_dggrid_bin)
                         iFlag_found_binary = 1
                         break
                 else:
                     print('Binary not found in system path.')
                 if iFlag_found_binary ==1:
                     sFilename_new = sWorkspace_output + slash + 'dggrid'
                     copy2(sFilename_dggrid_bin, sFilename_new)
-                    os.chmod(sFilename_new, stat.S_IREAD | stat.S_IWRITE | stat.S_IXUSR)    
+                    os.chmod(sFilename_new, stat.S_IREAD | stat.S_IWRITE | stat.S_IXUSR)
                 else:
                     print('Binary not found in system path.')
-                    return                            
-                    
-                       
+                    return
+
+
         return
 
     def pyflowline_change_model_parameter(self, sVariable_in, dValue, iFlag_basin_in = None):
         if iFlag_basin_in is None:
             if hasattr(self, sVariable_in):
-                #get default data type                
+                #get default data type
                 sType_default = type(getattr(self, sVariable_in))
                 #get the data type of the input value
                 sType_input = type(dValue)
-                if sType_default == sType_input:      
-                    setattr(self, sVariable_in, dValue)                    
-                    pass   
+                if sType_default == sType_input:
+                    setattr(self, sVariable_in, dValue)
+                    pass
                 else:
                     print('Incorrect data type for the input value: ' + sVariable_in)
                 return True
             else:
                 print("This model parameter is unknown, please check the full parameter list in the documentation: " + sVariable_in)
                 return False
-            
-            
+
+
 
         else:
             #this mean the variable is in the basin object
             for pBasin in self.aBasin:
                 if hasattr(pBasin, sVariable_in):
                     #get default data type
                     sType_default = type(getattr(pBasin, sVariable_in))
                     sType_input = type(dValue)
-                    if sType_default == sType_input:      
+                    if sType_default == sType_input:
                         setattr(pBasin, sVariable_in, dValue)
                     else:
-                        print('Incorrect data type for the input value: ' + sVariable_in)                       
+                        print('Incorrect data type for the input value: ' + sVariable_in)
                         return False
                 else:
                     print("This model parameter is unknown, please check the full parameter list in the documentation: " + sVariable_in)
                     return False
 
     def pyflowline_run(self):
         """
         Run the flowlinecase simulation
 
         Returns:
             list: A list of cell objects
         """
         aCell_out = None
         if self.iFlag_flowline == 1:
-            self.pyflowline_flowline_simplification()       
+            self.pyflowline_flowline_simplification()
         else:
-            pass            
+            pass
 
         if self.iFlag_create_mesh:
             self.aCell = self.pyflowline_mesh_generation(iFlag_antarctic_in= self.iFlag_antarctic)
             aCell_out = self.aCell
             pass
         else:
-            #may be read mesh           
+            #may be read mesh
             iMesh_type = self.iMesh_type
             #there must be some auxiliary file associated with the mesh file
-            self.aCell = read_mesh_json_w_topology(iMesh_type, self.sFilename_mesh)             
+            self.aCell = read_mesh_json_w_topology(iMesh_type, self.sFilename_mesh)
             aCell_out = self.aCell
             pass
 
         if self.iFlag_intersect == 1:
             self.aCell, a, b = self.pyflowline_reconstruct_topological_relationship()
             aCell_out = self.aCell
             pass
@@ -1202,17 +1202,17 @@
         return
 
     def pyflowline_export_mesh_info_to_json(self):
         """
         Export the mesh information to a json file
         """
 
-  
+
         sFilename_json = self.sFilename_mesh_info
-        
+
         #if iFlag_flowline == 1: #if there is conceptual flowline
         #    pass
         #else:
         #    #only mesh, no flowline
         #    pass
 
 
@@ -1234,15 +1234,15 @@
                  'aFlowline_simplified','aFlowline_conceptual','aCellID_outlet',
                  'aCell', 'pRTree_mesh']
 
         obj = self.__dict__.copy()
         for sKey in aSkip:
             obj.pop(sKey, None)
             pass
-        
+
         sJson = json.dumps(obj,\
                                sort_keys=True, \
                                indent = 4, \
                                ensure_ascii=True, \
                                cls=CaseClassEncoder)
         return sJson
 
@@ -1298,17 +1298,17 @@
                 f.write(sJson)
                 f.close()
                 #update for pyhexwatershed
             self.sFilename_basins = sFilename_configuration
             self.sWorkspace_output =   sPath.parent.absolute()
 
 
-        aSkip = ['aBasin', \
+        aSkip = ['aBasin',
                  'aFlowline_simplified','aFlowline_conceptual','aCellID_outlet',
-                 'aCell']
+                 'aCell', 'pRTree_mesh']
 
         obj = self.__dict__.copy()
         for sKey in aSkip:
             obj.pop(sKey, None)
 
         with open(sFilename_output, 'w', encoding='utf-8') as f:
             json.dump(obj, f,sort_keys=True, \
```

### Comparing `pyflowline-0.3.8/pyflowline/classes/square.py` & `pyflowline-0.3.9/pyflowline/classes/square.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/timer.py` & `pyflowline-0.3.9/pyflowline/classes/timer.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/tin.py` & `pyflowline-0.3.9/pyflowline/classes/tin.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/classes/vertex.py` & `pyflowline-0.3.9/pyflowline/classes/vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/formats/convert_attributes.py` & `pyflowline-0.3.9/pyflowline/formats/convert_attributes.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/formats/convert_coordinates.py` & `pyflowline-0.3.9/pyflowline/formats/convert_coordinates.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/formats/convert_flowline_to_geojson.py` & `pyflowline-0.3.9/pyflowline/formats/convert_flowline_to_geojson.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/formats/export_flowline.py` & `pyflowline-0.3.9/pyflowline/formats/export_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/formats/export_mesh.py` & `pyflowline-0.3.9/pyflowline/formats/export_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/formats/export_vertex.py` & `pyflowline-0.3.9/pyflowline/formats/export_vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/formats/read_flowline.py` & `pyflowline-0.3.9/pyflowline/formats/read_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/formats/read_mesh.py` & `pyflowline-0.3.9/pyflowline/formats/read_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/formats/read_nhdplus_flowline_shapefile.py` & `pyflowline-0.3.9/pyflowline/formats/read_nhdplus_flowline_shapefile.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/mesh/dggrid/create_dggrid_mesh.py` & `pyflowline-0.3.9/pyflowline/mesh/dggrid/create_dggrid_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/mesh/hexagon/create_hexagon_mesh.py` & `pyflowline-0.3.9/pyflowline/mesh/hexagon/create_hexagon_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/mesh/latlon/create_latlon_mesh.py` & `pyflowline-0.3.9/pyflowline/mesh/latlon/create_latlon_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/mesh/mpas/create_mpas_mesh.py` & `pyflowline-0.3.9/pyflowline/mesh/mpas/create_mpas_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/mesh/square/create_square_mesh.py` & `pyflowline-0.3.9/pyflowline/mesh/square/create_square_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/mesh/tin/create_tin_mesh.py` & `pyflowline-0.3.9/pyflowline/mesh/tin/create_tin_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.3.8/pyflowline/pyflowline_create_template_configuration_file.py` & `pyflowline-0.3.9/pyflowline/configuration/create_template_configuration_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,36 @@
 from pathlib import Path
 #use this function to generate an initial json file for hexwatershed
 import json
 #once it's generated, you can modify it and use it for different simulations
 from pyflowline.classes.pycase import flowlinecase
 from pyflowline.classes.basin import pybasin
 
-def pyflowline_create_basin_template_configuration_file(sFilename_basins_json, nBasin, sWorkspace_input_in, sWorkspace_output_in):
+def pyflowline_create_template_basin_configuration_file(
+        sFilename_basins_json,
+        nBasin,
+        sWorkspace_input_in,
+        sWorkspace_output_in):
     """generate basin configuration
 
     Args:
-        sFilename_basins_json (str): the filename
+        sFilename_basins_json (str or Path): the filename
         nBasin (int): the total number of basin
-        sWorkspace_input_in (str): the input data path
-        sWorkspace_output (str): the output path
+        sWorkspace_input_in (str or Path): the input data path
+        sWorkspace_output (str or Path): the output path
 
     Returns:
         basin: a basin object
     """
 
+    # Ensure input pathnames are strings
+    sFilename_basins_json = str(sFilename_basins_json)
+    sWorkspace_input_in = str(sWorkspace_input_in)
+    sWorkspace_output_in = str(sWorkspace_output_in)
+
     aBasin_out = list()
     for i in range(nBasin):
         sBasin =  "{:03d}".format(i+1)   
         aConfig_basin = {}
         aConfig_basin['iFlag_dam'] = 0
         aConfig_basin['iFlag_disconnected'] = 0
         aConfig_basin['lBasinID'] = i + 1
@@ -43,35 +52,50 @@
     with open(sFilename_basins_json, 'w', encoding='utf-8') as f:
         sJson = json.dumps([json.loads(ob.tojson()) for ob in aBasin_out], indent = 4)        
         f.write(sJson)    
         f.close()
 
     return aBasin_out
 
-def pyflowline_create_template_configuration_file(sFilename_json, \
-    sWorkspace_input, sWorkspace_output, iFlag_standalone_in=None, \
-        iFlag_use_mesh_dem_in=None,  iCase_index_in=None,  dResolution_degree_in = None, dResolution_meter_in = None,   sDate_in = None,  sMesh_type_in = None,    sModel_in = None):
+def pyflowline_create_template_configuration_file(
+        sFilename_json,
+        sWorkspace_input,
+        sWorkspace_output,
+        iFlag_standalone_in=None,
+        iFlag_use_mesh_dem_in=None,
+        iCase_index_in=None,
+        dResolution_degree_in=None,
+        dResolution_meter_in=None,
+        sDate_in=None,
+        sMesh_type_in=None,
+        sModel_in=None):
     """generate pyflowline config template file
 
     Args:
-        sFilename_json (str): _description_
-        sWorkspace_input (str): _description_
+        sFilename_json (str or Path): _description_.
+        sWorkspace_input (str or Path): _description_.
+        sWorkspace_output (str or Path): _description_.
         iFlag_standalone_in (int, optional): _description_. Defaults to None.
         iFlag_use_mesh_dem_in (int, optional): _description_. Defaults to None.        
         iCase_index_in (int, optional): _description_. Defaults to None.
         dResolution_degree_in (float, optional): _description_. Defaults to None.
         dResolution_meter_in (float, optional): _description_. Defaults to None.
         sDate_in (str, optional): _description_. Defaults to None.
         sMesh_type_in (str, optional): _description_. Defaults to None.
         sModel_in (str, optional): _description_. Defaults to None.
-        sWorkspace_output_in (str, optional): _description_. Defaults to None.
 
     Returns:
         _type_: _description_
     """
+
+    # Ensure input pathnames are strings
+    sFilename_json = str(sFilename_json)
+    sWorkspace_input = str(sWorkspace_input)
+    sWorkspace_output = str(sWorkspace_output)
+
     if os.path.exists(sFilename_json):         
         os.remove(sFilename_json)
 
     if iCase_index_in is not None:        
         iCase_index = iCase_index_in
     else:       
         iCase_index = 1
@@ -97,23 +121,20 @@
         sMesh_type = 'hexagon'
         pass
     if sDate_in is not None:
         sDate = sDate_in
     else:
         sDate = '20220202'
         pass
-    
-    
+
     nBasin = 1
 
- 
-    #use a dict to initialize the class
+    # Use a dict to initialize the class
     aConfig = {}
-    
-    
+
     #aConfig['iFlag_use_shapefile_extent'] = iFlag_use_shapefile_extent 
     aConfig['iFlag_use_mesh_dem'] = iFlag_use_mesh_dem
     aConfig['iFlag_save_mesh'] = 1
     aConfig['iFlag_simplification']=1
     aConfig['iFlag_create_mesh']=1
     aConfig['iFlag_intersect']=1
     aConfig['iFlag_resample_method']=1
@@ -126,15 +147,15 @@
     aConfig['nOutlet'] = nBasin
     aConfig['dResolution_degree'] = 0.5
     aConfig['dResolution_meter'] = 50000
     aConfig['dLongitude_left'] = -180
     aConfig['dLongitude_right'] = 180
     aConfig['dLatitude_bot'] = -90
     aConfig['dLatitude_top'] = 90
-    aConfig['sFilename_model_configuration']  = sFilename_json 
+    aConfig['sFilename_model_configuration'] = sFilename_json 
     aConfig['sWorkspace_input'] = sWorkspace_input    
     aConfig['sWorkspace_output'] = sWorkspace_output        
     aConfig['sRegion'] = 'susquehanna'
     aConfig['sModel'] = 'pyflowline'
     aConfig['iCase_index'] = iCase_index   
     aConfig['sMesh_type'] = sMesh_type
     aConfig['sJob'] = 'pyflowline'
@@ -143,18 +164,24 @@
     aConfig['sFilename_mesh_netcdf'] = str(Path(sWorkspace_input)  /  'lnd_cull_mesh.nc')
     aConfig['sFilename_spatial_reference'] =  str(Path(sWorkspace_input)  /  'boundary_proj.shp')   
     #relative path
     aConfig['flowline_info'] = 'flowline_info.json'
     aConfig['sFilename_mesh_info'] = 'mesh_info.json'
     aConfig['sFilename_elevation'] = 'elevation.json' 
     oModel = flowlinecase(aConfig)
-    #generate basin
+
+    # Generate basin
     sDirname = os.path.dirname(sFilename_json)
     sFilename =  Path(sFilename_json).stem + '_basins.json'
     sFilename_basins_json = os.path.join(sDirname, sFilename)   
-    aBasin = pyflowline_create_basin_template_configuration_file(sFilename_basins_json, nBasin, sWorkspace_input,  oModel.sWorkspace_output)
+
+    aBasin = pyflowline_create_template_basin_configuration_file(
+        sFilename_basins_json,
+        nBasin,
+        sWorkspace_input,
+        oModel.sWorkspace_output)
+
     oModel.aBasin = aBasin
     oModel.sFilename_basins = sFilename_basins_json
     oModel.export_config_to_json(sFilename_json)    
 
     return oModel
-
```

### Comparing `pyflowline-0.3.8/pyflowline/pyflowline_read_model_configuration_file.py` & `pyflowline-0.3.9/pyflowline/configuration/read_configuration_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,68 +1,75 @@
 import os
 from pathlib import Path
 import datetime
 import json
 from pyflowline.classes.pycase import flowlinecase
+
 pDate = datetime.datetime.today()
-sDate_default = "{:04d}".format(
-    pDate.year) + "{:02d}".format(pDate.month) + "{:02d}".format(pDate.day)
+sDate_default = "{:04d}".format(pDate.year) + \
+    "{:02d}".format(pDate.month) + "{:02d}".format(pDate.day)
 
 
-def pyflowline_read_model_configuration_file(sFilename_configuration_in,
-                                             iFlag_standalone_in=None,
+def pyflowline_read_configuration_file(sFilename_configuration_in,
+                                             iFlag_standalone_in=1,
                                              iFlag_use_mesh_dem_in=None,
                                              iCase_index_in=None,
                                              iResolution_index_in = None,
                                              dResolution_degree_in=None,
                                              dResolution_meter_in=None,
                                              sMesh_type_in=None,
-                                             sModel_in=None,
+                                             sModel_in='pyflowline',
                                              sDate_in=None,
-                                              sDggrid_type_in = None,
+                                             sDggrid_type_in = None,
                                              sWorkspace_output_in=None):
+
     """read a model configuration
 
     Args:
-        sFilename_configuration_in (str): _description_
+        sFilename_configuration_in (str or Path): _description_
         iFlag_standalone_in (int, optional): _description_. Defaults to None.
         iFlag_use_mesh_dem_in (int, optional): _description_. Defaults to None.
         iCase_index_in (int, optional): _description_. Defaults to None.
         dResolution_degree_in (float, optional): _description_. Defaults to None.
         dResolution_meter_in (float, optional): _description_. Defaults to None.
         sMesh_type_in (str, optional): _description_. Defaults to None.
         sModel_in (str, optional): _description_. Defaults to None.
         sDate_in (str, optional): _description_. Defaults to None.
-        sWorkspace_output_in (str, optional): _description_. Defaults to None.
+        sWorkspace_output_in (str or Path, optional): _description_. Defaults to None.
 
     Returns:
         _type_: _description_
     """
+    # Ensure input filenames are strings
+    if isinstance(sFilename_configuration_in, Path):
+        sFilename_configuration_in = str(sFilename_configuration_in)
+    if isinstance(sWorkspace_output_in, Path):
+        sWorkspace_output_in = str(sWorkspace_output_in)
 
     if not os.path.isfile(sFilename_configuration_in):
         print(sFilename_configuration_in + ' does not exist')
         return
 
     # Opening JSON file
     with open(sFilename_configuration_in) as json_file:
         aConfig = json.load(json_file)
 
     if iCase_index_in is not None:
         iCase_index = iCase_index_in
     else:
         iCase_index = int(aConfig['iCase_index'])
-    
-    if iResolution_index_in is not None:    
+
+    if iResolution_index_in is not None:
         iResolution_index = iResolution_index_in
     else:
-        if "iResolution_index" in aConfig:            
+        if "iResolution_index" in aConfig:
             iResolution_index =  int( aConfig['iResolution_index'])
         else:
             iResolution_index = 10
-      
+
         pass
 
     if iFlag_standalone_in is not None:
         iFlag_standalone = iFlag_standalone_in
     else:
         iFlag_standalone = int(aConfig['iFlag_standalone'])
 
@@ -76,15 +83,15 @@
     else:
         sMesh_type = aConfig['sMesh_type']
         pass
 
     if sDggrid_type_in is not None:
         sDggrid_type = sDggrid_type_in
     else:
-        if "sDggrid_type" in aConfig:            
+        if "sDggrid_type" in aConfig:
             sDggrid_type = aConfig["sDggrid_type"]
         else:
             sDggrid_type = 'ISEA3H'
 
     if sModel_in is not None:
         sModel = sModel_in
     else:
@@ -112,16 +119,17 @@
     if sWorkspace_output_in is not None:
         sWorkspace_output = sWorkspace_output_in
     else:
         sWorkspace_output = aConfig['sWorkspace_output']
         # try to create this output folder first using
 
     try:
-        print(sWorkspace_output)
+        print("Creating the specified output workspace (if it does not exist): \n", sWorkspace_output)
         Path(sWorkspace_output).mkdir(parents=True, exist_ok=True)
+        print("The specified output workspace is: \n", sWorkspace_output)
     except ValueError:
         print("The specified output workspace cannot be created!")
         exit
 
     aConfig['iCase_index'] = iCase_index
     aConfig['iFlag_standalone'] = iFlag_standalone
     aConfig['iFlag_use_mesh_dem'] = iFlag_use_mesh_dem
```

### Comparing `pyflowline-0.3.8/pyflowline.egg-info/PKG-INFO` & `pyflowline-0.3.9/pyflowline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflowline
-Version: 0.3.8
+Version: 0.3.9
 Summary: A mesh-independent river network generator for hydrologic models
 Home-page: https://github.com/changliao1025/pyflowline
 Author: Chang Liao
 Author-email: chang.liao@pnnl.gov
 License: custom
 Keywords: Earth Science
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyflowline-0.3.8/pyflowline.egg-info/SOURCES.txt` & `pyflowline-0.3.9/pyflowline.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,14 @@
 docs/source/api/api.rst
 docs/source/application/application.rst
 docs/source/data/data.rst
 docs/source/installation/installation.rst
 examples/__init__.py
 examples/create_model_configuration.py
 pyflowline/__init__.py
-pyflowline/change_json_key_value.py
-pyflowline/pyflowline_create_template_configuration_file.py
-pyflowline/pyflowline_read_model_configuration_file.py
 pyflowline.egg-info/PKG-INFO
 pyflowline.egg-info/SOURCES.txt
 pyflowline.egg-info/dependency_links.txt
 pyflowline.egg-info/requires.txt
 pyflowline.egg-info/top_level.txt
 pyflowline/algorithms/__init__.py
 pyflowline/algorithms/auxiliary/__init__.py
@@ -111,14 +108,19 @@
 pyflowline/classes/mesh.py
 pyflowline/classes/mpas.py
 pyflowline/classes/pycase.py
 pyflowline/classes/square.py
 pyflowline/classes/timer.py
 pyflowline/classes/tin.py
 pyflowline/classes/vertex.py
+pyflowline/configuration/__init__.py
+pyflowline/configuration/change_json_key_value.py
+pyflowline/configuration/create_template_configuration_file.py
+pyflowline/configuration/path_manager.py
+pyflowline/configuration/read_configuration_file.py
 pyflowline/formats/__init__.py
 pyflowline/formats/convert_attributes.py
 pyflowline/formats/convert_coordinates.py
 pyflowline/formats/convert_flowline_to_geojson.py
 pyflowline/formats/export_flowline.py
 pyflowline/formats/export_mesh.py
 pyflowline/formats/export_vertex.py
@@ -134,8 +136,9 @@
 pyflowline/mesh/latlon/create_latlon_mesh.py
 pyflowline/mesh/mpas/__init__.py
 pyflowline/mesh/mpas/create_mpas_mesh.py
 pyflowline/mesh/square/__init__.py
 pyflowline/mesh/square/create_square_mesh.py
 pyflowline/mesh/tin/__init__.py
 pyflowline/mesh/tin/create_tin_mesh.py
+tests/TestPathManager.py
 tests/test_installation.py
```

### Comparing `pyflowline-0.3.8/setup.py` & `pyflowline-0.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 NAME = "pyflowline"
 DESCRIPTION = \
     "A mesh-independent river network generator for hydrologic models"
 AUTHOR = "Chang Liao"
 AUTHOR_EMAIL = "chang.liao@pnnl.gov"
 URL = "https://github.com/changliao1025/pyflowline"
-VERSION = "0.3.8"
+VERSION = "0.3.9"
 REQUIRES_PYTHON = ">=3.8.0"
 KEYWORDS = "Earth Science"
 
 REQUIRED = [
-    "numpy", 
+    "numpy",
     "gdal",
     "netCDF4"
 ]
 
 CLASSIFY = [
     "Development Status :: 4 - Beta",
     "Operating System :: OS Independent",
```

