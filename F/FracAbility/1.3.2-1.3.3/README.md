# Comparing `tmp/fracability-1.3.2.tar.gz` & `tmp/fracability-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fracability-1.3.2.tar", last modified: Thu May  9 17:30:16 2024, max compression
+gzip compressed data, was "fracability-1.3.3.tar", last modified: Fri May 10 18:00:33 2024, max compression
```

## Comparing `fracability-1.3.2.tar` & `fracability-1.3.3.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.814038 fracability-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34503 2024-05-09 17:30:10.000000 fracability-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-09 17:30:16.814038 fracability-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-09 17:30:10.000000 fracability-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.786038 fracability-1.3.2/fracability/
--rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/AbstractClasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/Adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)    50373 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/Entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    32612 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/Plotters.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.786038 fracability-1.3.2/fracability/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.782038 fracability-1.3.2/fracability/examples/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.790038 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.cpg
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.prj
--rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.shp
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.shx
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_a.cpg
--rw-r--r--   0 runner    (1001) docker     (127)    81684 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_a.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_a.prj
--rw-r--r--   0 runner    (1001) docker     (127)   444908 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_a.shp
--rw-r--r--   0 runner    (1001) docker     (127)    15628 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_a.shx
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_b.cpg
--rw-r--r--   0 runner    (1001) docker     (127)    77682 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_b.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_b.prj
--rw-r--r--   0 runner    (1001) docker     (127)   224724 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_b.shp
--rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_b.shx
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_c.cpg
--rw-r--r--   0 runner    (1001) docker     (127)    25147 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_c.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_c.prj
--rw-r--r--   0 runner    (1001) docker     (127)   149084 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_c.shp
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_c.shx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.782038 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.790038 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/lengths/
--rw-r--r--   0 runner    (1001) docker     (127)   783657 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/lengths/Fractures_Length_set1_Pontrelli.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.790038 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/lengths/figures/
--rw-r--r--   0 runner    (1001) docker     (127)   112302 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/lengths/figures/cens.png
--rw-r--r--   0 runner    (1001) docker     (127)   116031 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/lengths/figures/no_cens.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.790038 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/spacing/
--rw-r--r--   0 runner    (1001) docker     (127)   166787 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/spacing/Fractures_Spacing_pontrelli.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.782038 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.802038 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.cpg
--rw-r--r--   0 runner    (1001) docker     (127)   273642 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.prj
--rw-r--r--   0 runner    (1001) docker     (127)   322948 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.shp
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.shx
--rw-r--r--   0 runner    (1001) docker     (127)   146225 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.zip
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.cpg
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.prj
--rw-r--r--   0 runner    (1001) docker     (127)    25396 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.shp
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.shx
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.cpg
--rw-r--r--   0 runner    (1001) docker     (127)  1267982 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.prj
--rw-r--r--   0 runner    (1001) docker     (127)   861844 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.shp
--rw-r--r--   0 runner    (1001) docker     (127)    34244 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.shx
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.cpg
--rw-r--r--   0 runner    (1001) docker     (127)  1855508 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.prj
--rw-r--r--   0 runner    (1001) docker     (127)   339148 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.shp
--rw-r--r--   0 runner    (1001) docker     (127)    75444 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.shx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.806038 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Interpretation_boundary.cpg
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Interpretation_boundary.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Interpretation_boundary.prj
--rw-r--r--   0 runner    (1001) docker     (127)   145016 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Interpretation_boundary.shp
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Interpretation_boundary.shx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.810038 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/
--rw-r--r--   0 runner    (1001) docker     (127)   358643 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/Salza_output.zip
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.cpg
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.prj
--rw-r--r--   0 runner    (1001) docker     (127)   150100 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.shp
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.shx
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.cpg
--rw-r--r--   0 runner    (1001) docker     (127)   428104 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.prj
--rw-r--r--   0 runner    (1001) docker     (127)   301908 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.shp
--rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.shx
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.cpg
--rw-r--r--   0 runner    (1001) docker     (127)   706998 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.prj
--rw-r--r--   0 runner    (1001) docker     (127)   129268 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.shp
--rw-r--r--   0 runner    (1001) docker     (127)    28804 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.shx
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_1.cpg
--rw-r--r--   0 runner    (1001) docker     (127)    13159 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)    32962 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_1.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_1.prj
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_1.qmd
--rw-r--r--   0 runner    (1001) docker     (127)   177796 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_1.shp
--rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_1.shx
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_2.cpg
--rw-r--r--   0 runner    (1001) docker     (127)    21455 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    22274 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_2.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_2.prj
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_2.qmd
--rw-r--r--   0 runner    (1001) docker     (127)   109732 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_2.shp
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_2.shx
--rw-r--r--   0 runner    (1001) docker     (127)    34826 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/length_dist.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.814038 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.cpg
--rw-r--r--   0 runner    (1001) docker     (127)    68687 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.prj
--rw-r--r--   0 runner    (1001) docker     (127)    13888 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.shp
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.shx
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.cpg
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.prj
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.shp
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.shx
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.cpg
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.prj
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.shp
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.shx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.814038 fracability-1.3.2/fracability/examples/datasets/qgis_styles/
--rw-r--r--   0 runner    (1001) docker     (127)    29047 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/qgis_styles/Boundary_style.qml
--rw-r--r--   0 runner    (1001) docker     (127)    38424 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/examples/datasets/qgis_styles/Nodes_style.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.814038 fracability-1.3.2/fracability/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/operations/Geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    27871 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/operations/Statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/operations/Topology.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.814038 fracability-1.3.2/fracability/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.814038 fracability-1.3.2/fracability/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/utils/general_use.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-09 17:30:10.000000 fracability-1.3.2/fracability/utils/shp_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:30:16.814038 fracability-1.3.2/fracability.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-09 17:30:16.000000 fracability-1.3.2/fracability.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-05-09 17:30:16.000000 fracability-1.3.2/fracability.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:30:16.000000 fracability-1.3.2/fracability.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-09 17:30:16.000000 fracability-1.3.2/fracability.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 17:30:16.000000 fracability-1.3.2/fracability.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-05-09 17:30:10.000000 fracability-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 17:30:16.814038 fracability-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-09 17:30:10.000000 fracability-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.652966 fracability-1.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.652966 fracability-1.3.3/FracAbility.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-05-10 18:00:33.000000 fracability-1.3.3/FracAbility.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-05-10 18:00:33.000000 fracability-1.3.3/FracAbility.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 18:00:33.000000 fracability-1.3.3/FracAbility.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-10 18:00:33.000000 fracability-1.3.3/FracAbility.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 18:00:33.000000 fracability-1.3.3/FracAbility.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34503 2024-05-10 18:00:27.000000 fracability-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-05-10 18:00:33.652966 fracability-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-10 18:00:27.000000 fracability-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.620966 fracability-1.3.3/fracability/
+-rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/AbstractClasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/Adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50373 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/Entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31609 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/Plotters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28706 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/Statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.620966 fracability-1.3.3/fracability/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.616966 fracability-1.3.3/fracability/examples/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.624966 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.prj
+-rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.shx
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_a.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)    81684 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_a.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_a.prj
+-rw-r--r--   0 runner    (1001) docker     (127)   444908 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_a.shp
+-rw-r--r--   0 runner    (1001) docker     (127)    15628 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_a.shx
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_b.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)    77682 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_b.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_b.prj
+-rw-r--r--   0 runner    (1001) docker     (127)   224724 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_b.shp
+-rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_b.shx
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_c.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)    25147 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_c.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_c.prj
+-rw-r--r--   0 runner    (1001) docker     (127)   149084 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_c.shp
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_c.shx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.616966 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.624966 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/lengths/
+-rw-r--r--   0 runner    (1001) docker     (127)   783657 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/lengths/Fractures_Length_set1_Pontrelli.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.624966 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/lengths/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)   112302 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/lengths/figures/cens.png
+-rw-r--r--   0 runner    (1001) docker     (127)   116031 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/lengths/figures/no_cens.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.624966 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/spacing/
+-rw-r--r--   0 runner    (1001) docker     (127)   166787 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/spacing/Fractures_Spacing_pontrelli.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.616966 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.636966 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)   273642 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.prj
+-rw-r--r--   0 runner    (1001) docker     (127)   322948 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.shp
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.shx
+-rw-r--r--   0 runner    (1001) docker     (127)   146225 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.zip
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.prj
+-rw-r--r--   0 runner    (1001) docker     (127)    25396 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.shx
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)  1267982 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.prj
+-rw-r--r--   0 runner    (1001) docker     (127)   861844 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.shp
+-rw-r--r--   0 runner    (1001) docker     (127)    34244 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.shx
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 18:00:27.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)  1855508 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.prj
+-rw-r--r--   0 runner    (1001) docker     (127)   339148 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.shp
+-rw-r--r--   0 runner    (1001) docker     (127)    75444 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.shx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.640966 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Interpretation_boundary.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Interpretation_boundary.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Interpretation_boundary.prj
+-rw-r--r--   0 runner    (1001) docker     (127)   145016 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Interpretation_boundary.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Interpretation_boundary.shx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.644966 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/
+-rw-r--r--   0 runner    (1001) docker     (127)   358643 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/Salza_output.zip
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.prj
+-rw-r--r--   0 runner    (1001) docker     (127)   150100 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.shx
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)   428104 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.prj
+-rw-r--r--   0 runner    (1001) docker     (127)   301908 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.shp
+-rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.shx
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)   706998 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.prj
+-rw-r--r--   0 runner    (1001) docker     (127)   129268 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.shp
+-rw-r--r--   0 runner    (1001) docker     (127)    28804 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.shx
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_1.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)    13159 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    32962 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_1.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_1.prj
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_1.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)   177796 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_1.shp
+-rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_1.shx
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_2.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)    21455 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    22274 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_2.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_2.prj
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_2.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)   109732 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_2.shp
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_2.shx
+-rw-r--r--   0 runner    (1001) docker     (127)    34826 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/length_dist.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.648966 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)    68687 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.prj
+-rw-r--r--   0 runner    (1001) docker     (127)    13888 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.shp
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.shx
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.prj
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.shx
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.prj
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.shp
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.shx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.648966 fracability-1.3.3/fracability/examples/datasets/qgis_styles/
+-rw-r--r--   0 runner    (1001) docker     (127)    29047 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/qgis_styles/Boundary_style.qml
+-rw-r--r--   0 runner    (1001) docker     (127)    38424 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/examples/datasets/qgis_styles/Nodes_style.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.652966 fracability-1.3.3/fracability/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/operations/Geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/operations/Topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.652966 fracability-1.3.3/fracability/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:33.652966 fracability-1.3.3/fracability/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/utils/general_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-10 18:00:28.000000 fracability-1.3.3/fracability/utils/shp_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-10 18:00:28.000000 fracability-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 18:00:33.652966 fracability-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-10 18:00:28.000000 fracability-1.3.3/setup.py
```

### Comparing `fracability-1.3.2/LICENSE` & `fracability-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/PKG-INFO` & `fracability-1.3.3/FracAbility.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: fracability
-Version: 1.3.2
+Name: FracAbility
+Version: 1.3.3
 Summary: Analyse fracture networks for digitalized rock outcrops. 
-Author-email: Gabriele Benedetti <gabri.benedetti@gmail.com>
+Author-email: Gabriele Benedetti <gabri.benedetti@gmail.com>, Stefano Casiraghi <s.casiraghi21@campus.unimib.it>, Daniela Bertacchi <daniela.bertacchi@unimib.it>, Andrea Bistacchi <andrea.bistacchi@unimib.it>
 License: AGPL-3.0 license 
 Project-URL: Documentation, https://fracability.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/gbene/FracAbility/issues
 Project-URL: Source Code, https://github.com/gbene/FracAbility
 Keywords: DOM,censoring,fractures,fracture-networks,survival-analysis,reliability
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
@@ -31,107 +31,72 @@
 Requires-Dist: pyperclip
 Requires-Dist: pyqt5
 Requires-Dist: openpyxl
 Requires-Dist: seaborn
 Provides-Extra: all
 Requires-Dist: fracability[jupyter]; extra == "all"
 Provides-Extra: jupyter
-Requires-Dist: ipywidgets; extra == "jupyter"
-Requires-Dist: jupyter-server-proxy; extra == "jupyter"
-Requires-Dist: nest_asyncio; extra == "jupyter"
-Requires-Dist: trame>=2.5.2; extra == "jupyter"
-Requires-Dist: trame-client>=2.12.7; extra == "jupyter"
-Requires-Dist: trame-server>=2.11.7; extra == "jupyter"
-Requires-Dist: trame-vtk>=2.5.8; extra == "jupyter"
-Requires-Dist: trame-vuetify>=2.3.1; extra == "jupyter"
+Requires-Dist: jupyter; extra == "jupyter"
 
 
 <div align="center">
 
 ![](./docs/images/logo_small_small.png)
 
 [![GitHub release](https://img.shields.io/github/release/gbene/FracAbility?&sort=semver&color=orange)](https://github.com/gbene/FracAbility/releases/)
 [![License](https://img.shields.io/badge/License-AGPL--3.0-orange)](#license)
 [![issues - FracAbility](https://img.shields.io/github/issues/gbene/FracAbility)](https://github.com/gbene/FracAbility/issues)
 [![Made with Python](https://img.shields.io/badge/Python->=3.8-orange?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 ![maintained - yes](https://img.shields.io/badge/maintained-yes-green)
 </div>
 
-**FracAbility** is a Python toolbox that can be used to analyse fracture networks in digitalized rock
-outcrops. This package provides tools to:
-
-1. Define the topology of fracture networks 
-2. Statistically analyze fracture length distributions while taking into consideration 
-right censoring effects ([survival analysis](https://en.wikipedia.org/wiki/Survival_analysis)). 
-
-The name Frac**Ability** recalls the [reliability](https://github.com/MatthewReid854/reliability/tree/master)<sup>1</sup> 
-library that inspired and helped in the creation of this project. 
-
-
 ## Quick introduction ⚡
 
+![](./docs/images/oniscent_view.png)
+
 Fracture networks are essential for the analysis and modelling of mechanical and hydraulic properties 
 of rock masses. Recently, the use of Digital Outcrop Models (**DOMs**) provided a solid framework for the collection 
 of large and quantitative datasets from which different properties can be extracted.
 Because of the complex nature of exposed rock outcrops, statistical model fitting can sometimes be challenging. 
 Areas covered by rock debree, vegetation patches or simply the outer boundaries of the outcrop can 
-introduce right-censoring bias and can often lead to parameter underestimation.
-
-The following diagram represents an idealized rock outcrop. We can define the wider rectangle as the entire 
-fractured object while the smaller one as the outcrop that we can see and measure. We can immediately 
-see what is going wrong; many of the fractures that we can measure are incomplete thus leading to underestimate 
-fracture length. 
-
-![](./docs/images/example_diagram.png)
-
-Tools are needed to correct for this bias. Survival analysis techniques, although usually applied  
-in function of time and not space, accomplishes exactly this.
-
-## Features 📋
+introduce right-censoring bias and can often lead to parameter underestimation. Tools are needed to correct for estimating the correct distribution parameters while taking into account this bias. Survival analysis techniques, although usually applied in function of time and not length, accomplishes exactly this.
 
-- **Shapefile importing support**
-
-
-- **Rapid topology analysis and identification of I,Y,X and U nodes**
-
-
-- **Backbone(s) identification**
-
-
-- **Statistical analysis tools:**
-    + Empirical CDF and SF calculation
-    + Distribution fitting
-    + Statistical model testing
+**FracAbility** is a Python toolbox that can be used to analyse fracture networks and estimate length distributions considering and correcting the effect of right-censoring using survival analysis. This package provides tools to:
 
+1. Define the topology of fracture networks 
+2. Estimate multiple fracture length distributions while taking into consideration 
+right censoring effects. 
+3. Provide methods to choose the most representative distribution using both a visual and a quantitative approach  
 
-- **Plotting tools:**
-    + Network objects plotting using matplotlib or vtk
-    + Ternary node plot 
-    + Rose diagram
-    + Statistical plotting
+Please refer to the [Docs](https://fracability.readthedocs.io/en/latest/) for a more in depth introduction to the problem, theoretical background, examples and API overview. 
 
 ## Installation 🔧
 
-To install fracability pip can be used:
+To install FracAbility **pip** can be used:
 
 ```bash
 pip install fracability
 ```
 
-## Documentation
+Please refer to the [Docs](https://fracability.readthedocs.io/en/latest/Quickstart.html) for further guidance
 
-For usage details please refer to the documentation:
+## Documentation 📚
 
-[![View - Online docs](https://img.shields.io/badge/View-Online_docs-blue?style=for-the-badge)](https://fracability.readthedocs.io/en/latest/index.html "Go to online documentation")
+Click here to view the online documentation:
 
-[![view - Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](/docs/ "Go to project documentation")
+[![View - Online docs](https://img.shields.io/badge/View-Online_docs-blue?style=for-the-badge)](https://fracability.readthedocs.io/en/latest/index.html "Go to online documentation")
 
+Click here to view the source code for the documentation:
 
+[![view - Source documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](/docs/ "Go to project documentation")
 
-## References 🎓
 
-1. Reid, M. (2020). MatthewReid854/reliability: v0. 5.1. version v0, 5.
+## Authors 💎✨
 
+ + **Gabriele Benedetti** ([gabri.benedetti@gmail.com](mailto:gabri.benedetti@gmail.com))
+ + Stefano Casiraghi ([s.casiraghi21@campus.unimib.it](mailto:s.casiraghi21@campus.unimib.it))
+ + Daniela Bertacchi ([daniela.bertacchi@unimib.it](mailto:daniela.bertacchi@unimib.it))
+ + Andrea Bistacchi ([andrea.bistacchi@unimib.it](mailto:andrea.bistacchi@unimib.it))
 
-## License
+## License 📄
 
 Released under [AGPL-3.0](/LICENSE) by [@gbene](https://github.com/gbene)
```

### Comparing `fracability-1.3.2/README.md` & `fracability-1.3.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -6,86 +6,58 @@
 [![GitHub release](https://img.shields.io/github/release/gbene/FracAbility?&sort=semver&color=orange)](https://github.com/gbene/FracAbility/releases/)
 [![License](https://img.shields.io/badge/License-AGPL--3.0-orange)](#license)
 [![issues - FracAbility](https://img.shields.io/github/issues/gbene/FracAbility)](https://github.com/gbene/FracAbility/issues)
 [![Made with Python](https://img.shields.io/badge/Python->=3.8-orange?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 ![maintained - yes](https://img.shields.io/badge/maintained-yes-green)
 </div>
 
-**FracAbility** is a Python toolbox that can be used to analyse fracture networks in digitalized rock
-outcrops. This package provides tools to:
-
-1. Define the topology of fracture networks 
-2. Statistically analyze fracture length distributions while taking into consideration 
-right censoring effects ([survival analysis](https://en.wikipedia.org/wiki/Survival_analysis)). 
-
-The name Frac**Ability** recalls the [reliability](https://github.com/MatthewReid854/reliability/tree/master)<sup>1</sup> 
-library that inspired and helped in the creation of this project. 
-
-
 ## Quick introduction ⚡
 
+![](./docs/images/oniscent_view.png)
+
 Fracture networks are essential for the analysis and modelling of mechanical and hydraulic properties 
 of rock masses. Recently, the use of Digital Outcrop Models (**DOMs**) provided a solid framework for the collection 
 of large and quantitative datasets from which different properties can be extracted.
 Because of the complex nature of exposed rock outcrops, statistical model fitting can sometimes be challenging. 
 Areas covered by rock debree, vegetation patches or simply the outer boundaries of the outcrop can 
-introduce right-censoring bias and can often lead to parameter underestimation.
-
-The following diagram represents an idealized rock outcrop. We can define the wider rectangle as the entire 
-fractured object while the smaller one as the outcrop that we can see and measure. We can immediately 
-see what is going wrong; many of the fractures that we can measure are incomplete thus leading to underestimate 
-fracture length. 
-
-![](./docs/images/example_diagram.png)
-
-Tools are needed to correct for this bias. Survival analysis techniques, although usually applied  
-in function of time and not space, accomplishes exactly this.
-
-## Features 📋
+introduce right-censoring bias and can often lead to parameter underestimation. Tools are needed to correct for estimating the correct distribution parameters while taking into account this bias. Survival analysis techniques, although usually applied in function of time and not length, accomplishes exactly this.
 
-- **Shapefile importing support**
-
-
-- **Rapid topology analysis and identification of I,Y,X and U nodes**
-
-
-- **Backbone(s) identification**
-
-
-- **Statistical analysis tools:**
-    + Empirical CDF and SF calculation
-    + Distribution fitting
-    + Statistical model testing
+**FracAbility** is a Python toolbox that can be used to analyse fracture networks and estimate length distributions considering and correcting the effect of right-censoring using survival analysis. This package provides tools to:
 
+1. Define the topology of fracture networks 
+2. Estimate multiple fracture length distributions while taking into consideration 
+right censoring effects. 
+3. Provide methods to choose the most representative distribution using both a visual and a quantitative approach  
 
-- **Plotting tools:**
-    + Network objects plotting using matplotlib or vtk
-    + Ternary node plot 
-    + Rose diagram
-    + Statistical plotting
+Please refer to the [Docs](https://fracability.readthedocs.io/en/latest/) for a more in depth introduction to the problem, theoretical background, examples and API overview. 
 
 ## Installation 🔧
 
-To install fracability pip can be used:
+To install FracAbility **pip** can be used:
 
 ```bash
 pip install fracability
 ```
 
-## Documentation
+Please refer to the [Docs](https://fracability.readthedocs.io/en/latest/Quickstart.html) for further guidance
 
-For usage details please refer to the documentation:
+## Documentation 📚
 
-[![View - Online docs](https://img.shields.io/badge/View-Online_docs-blue?style=for-the-badge)](https://fracability.readthedocs.io/en/latest/index.html "Go to online documentation")
+Click here to view the online documentation:
 
-[![view - Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](/docs/ "Go to project documentation")
+[![View - Online docs](https://img.shields.io/badge/View-Online_docs-blue?style=for-the-badge)](https://fracability.readthedocs.io/en/latest/index.html "Go to online documentation")
 
+Click here to view the source code for the documentation:
 
+[![view - Source documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](/docs/ "Go to project documentation")
 
-## References 🎓
 
-1. Reid, M. (2020). MatthewReid854/reliability: v0. 5.1. version v0, 5.
+## Authors 💎✨
 
+ + **Gabriele Benedetti** ([gabri.benedetti@gmail.com](mailto:gabri.benedetti@gmail.com))
+ + Stefano Casiraghi ([s.casiraghi21@campus.unimib.it](mailto:s.casiraghi21@campus.unimib.it))
+ + Daniela Bertacchi ([daniela.bertacchi@unimib.it](mailto:daniela.bertacchi@unimib.it))
+ + Andrea Bistacchi ([andrea.bistacchi@unimib.it](mailto:andrea.bistacchi@unimib.it))
 
-## License
+## License 📄
 
 Released under [AGPL-3.0](/LICENSE) by [@gbene](https://github.com/gbene)
```

### Comparing `fracability-1.3.2/fracability/AbstractClasses.py` & `fracability-1.3.3/fracability/AbstractClasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,14 @@
 
 class BaseOperator(ABC):
     """
     Abstract class for Operators such as:
 
     1. Geometry operations
     2. Topology operations
-    3. Statistics operations
 
     This class provides a unified input for the different operators since all are based on the BaseObj and associated
     entity_df
     """
 
     def __init__(self, obj: BaseEntity):
         self.df = obj.entity_df.loc[obj.entity_df['active_set'] == 1].copy()
```

### Comparing `fracability-1.3.2/fracability/Adapters.py` & `fracability-1.3.3/fracability/Adapters.py`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/Entities.py` & `fracability-1.3.3/fracability/Entities.py`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/Plotters.py` & `fracability-1.3.3/fracability/Plotters.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 import matplotlib.pyplot as plt
 import pandas as pd
 import seaborn as sns
 from pyvista import Plotter
 import ternary
 from vtkmodules.vtkFiltersCore import vtkConnectivityFilter
 
-from fracability.operations.Statistics import NetworkDistribution, NetworkFitter
+from fracability.Statistics import NetworkDistribution, NetworkFitter
 from fracability.utils.general_use import KM, setFigLinesBW
 
 import numpy as np
 from scipy.stats import uniform
 
 
 def matplot_nodes(entity,
@@ -106,14 +106,87 @@
     if return_plot:
         return ax
     else:
         if show_plot:
             plt.show()
 
 
+def matplot_ternary(entity,
+                    return_plot: bool = False,
+                    show_plot: bool = True):
+
+    """
+    Plot the ternary diagram for nodes
+
+    Parameters
+    ----------
+
+    entity: The fracability Nodes entity
+
+    return_plot: Bool. If true return the plot. By default, false
+
+    show_plot: Bool. If true show the plot. By default, true.
+
+
+    """
+
+    figure, tax = ternary.figure(scale=100)
+    figure.set_size_inches(10, 10)
+
+    if entity.name == 'FractureNetwork':
+        nodes = entity.nodes
+    elif entity.name == 'Nodes':
+        nodes = entity
+
+    PI, PY, PX, _, CI = nodes.ternary_node_count
+    points = [(PX, PI, PY)]
+
+    tax.scatter(points, marker='o', color='red', label='Classification')
+    tax.annotate(f'{np.round(CI,2)}', position=[PX, PI, PY])
+
+    for n in range(8):
+        n += 1
+        A1 = np.array([[1, 1, 1], [0, 0, 1], [-n, 4, 0]])
+        B = np.array([1, 0, 4 - n])
+
+        X1 = np.linalg.inv(A1).dot(B) * 100
+        if n < 4:
+            side = [1, 0, 0]
+        else:
+            side = [0, 1, 0]
+        A2 = np.array([[1, 1, 1], side, [-n, 4, 0]])
+
+        X2 = np.linalg.inv(A2).dot(B) * 100
+
+        tax.line(X1, X2, color='black', linewidth=1, alpha=n / 8)
+
+    ax = tax.get_axes()
+    ax.text(76.8, 21.3, 8)
+    ax.text(74.8, 23.8, 7)
+    ax.text(73.5, 27.9, 6)
+    ax.text(71, 32.3, 5)
+    ax.text(69.1, 38, 4)
+    ax.text(65.8, 45, 3)
+    ax.text(62.7, 54, 2)
+    ax.text(57, 66.5, 1)
+
+    tax.right_corner_label("X", fontsize=15)
+    tax.top_corner_label("I", fontsize=15)
+    tax.left_corner_label("Y", fontsize=15)
+
+    tax.get_axes().set_aspect(1)  # This is used to avoid deformation when rescaling the plotter window
+    # tax.clear_matplotlib_ticks()
+    tax.get_axes().axis('off')
+    if return_plot:
+        return tax
+    else:
+        if show_plot:
+            plt.show()
+
+
 def matplot_fractures(entity,
                       linewidth=1,
                       color='black',
                       color_set=False,
                       return_plot=False,
                       show_plot=True):
     """
@@ -769,57 +842,19 @@
     # ran_table.auto_set_font_size(False)
     # ran_table.auto_set_column_width(col=list(range(len(rank_df.columns))))
 
     if show_plot:
         plt.show()
 
 
-# def matplot_stats_model_selection(fitter: NetworkFitter,
-#                                   vertical: bool= False,
-#                                   show_plot: bool = True,
-#                                   sort_by: str = 'Akaike'):
-#     """
-#     Plot the stats summary table for the chosen models
-#
-#     Parameters
-#     -----------
-#     fitter: Network fitter object
-#     vertical: Bool. If true the table is vertical. By default, is False
-#     show_plot: Bool. If true show the plot. By default, is True
-#     sort_by: Sort the model based on a selection parameter. Available keys:
-#         1. Akaike
-#         2. KS_distance
-#         3. KG_distance
-#         4. AD_distance
-#     """
-#
-#     if show_plot:
-#         fig = plt.figure(num=f'Model selection summary table')
-#         fig.text(0.5, 0.95, f'Model selection summary table (sorted by {sort_by})', ha='center')
-#
-#     plt.axis('off')
-#     data_frame = fitter.fit_records(sort_by)
-#     the_table = plt.table(cellText=data_frame.round(decimals=2).values[:, 1:13],
-#                           rowLabels=data_frame['name'],
-#                           colLabels=data_frame.columns[1:13],
-#                           loc='center')
-#
-#     the_table.auto_set_font_size(False)
-#     the_table.auto_set_column_width(col=list(range(len(data_frame.columns))))
-#     the_table.set_fontsize(14)
-#
-#     if show_plot:
-#         plt.show()
-
-
 def matplot_stats_summary(fitter: NetworkFitter,
                           function_list: list = ['pdf', 'cdf', 'sf'],
                           table: bool = True,
                           show_plot: bool = True,
-                          position: int = 1,
+                          position: list = [],
                           sort_by: str = 'Akaike'):
     """
     Summarize PDF, CDF and SF functions and display summary table all
     in a single plot.
 
 
     Parameters
@@ -828,23 +863,26 @@
 
     function_list: List of function to calculate (cdf, pdf etc.). By default pdf, cdf and sf functions are calculated
 
     table: Bool. If true the summary table is shown. By default is true
 
     show_plot: Bool. If true show the plot. By default, is True
     
-    position: int. Show the summary plot for the model at the indicated position (1 indexed) sorted by the sort_by field. If False show the plots for each fit.  By default is 1.
+    position: List.  Plot the models at the given position (1 indexed) in the ordered sorted by the sort_by field. If None show the plots for each fit. By default is [1].
 
     sort_by: str. If best is True, show the best fit using the indicated column name. By default is Akaike
 
     """
     sns.set_theme()
-    
+
+    # This distribution selection process could be probably optimized
+    names = []
     if position:
-        names = [fitter.get_fitted_distribution_names(sort_by)[position-1]]
+        for pos in position:
+            names.append(fitter.get_fitted_distribution_names(sort_by)[pos-1])
     else:
         names = fitter.get_fitted_distribution_names(sort_by)
 
     for name in names:
         network_distribution = fitter.get_fitted_distribution(name)
         fig = plt.figure(num=f'{name} summary plot', figsize=(13, 7))
         # fig.text(0.5, 0.02, 'Length [m]', ha='center')
@@ -873,34 +911,40 @@
 
         if show_plot:
             plt.show()
 
 
 def matplot_stats_uniform(fitter: NetworkFitter,
                           show_plot: bool = True,
-                          position: int = 0,
-                          sort_by: str = 'Akaike'):
+                          position: list = None,
+                          sort_by: str = 'Akaike',
+                          bw: bool = False):
     """
     Confront the fitted data with the standard uniform 0,1. Following Kim 2019
 
     Parameters
     -------
     fitter: Input NetworkFitter object
 
     show_plot: Bool. If true show the plot. By default, is True
 
-    position: int. Show the summary plot for the model at the indicated position (1 indexed) sorted by the sort_by field. If False show the plots for each fit.  By default is False.
+    position: List.  Plot the models at the given position (1 indexed) in the ordered fit_records dataframe sorted by the sort_by field. If None show the plots for each fit. Default is None
 
     sort_by: str. If best is True, show the best fit using the indicated column name. By default is Akaike
 
+    bw: Bool. If true turn the plot color-blind friendly (black lines with different patterns). Max 7 lines (i.e. models). Default is False
+
     """
-    #sns.set_theme()
 
+    # This distribution selection process could be probably optimized
+
+    names = []
     if position:
-        names = [fitter.get_fitted_distribution_names(sort_by)[position-1]]
+        for pos in position:
+            names.append(fitter.get_fitted_distribution_names(sort_by)[pos-1])
     else:
         names = fitter.get_fitted_distribution_names(sort_by)
 
     fig = plt.figure(num=f'Comparison plot', figsize=(13, 7))
 
     uniform_list = np.linspace(0, 1, num=10)
     uniform_cdf = uniform.cdf(uniform_list)
@@ -908,89 +952,17 @@
     for name in names:
         network_distribution = fitter.get_fitted_distribution(name)
         Z = network_distribution.cdf()
         delta = network_distribution.fit_data.delta
         G_n = KM(Z, Z, delta)
         plt.plot(Z, G_n, label=f'G_n {name}') # plot the Kaplan-Meier curves with steps
 
-    setFigLinesBW(fig)
+    if bw:
+        setFigLinesBW(fig)
 
     if show_plot:
         plt.plot(uniform_list, uniform_cdf, 'r', label='U(0, 1)')
         plt.title('Distance to Uniform comparison')
         plt.grid(False)
         plt.legend()
         plt.show()
 
-
-
-def matplot_ternary(entity,
-                    return_plot: bool = False,
-                    show_plot: bool = True):
-
-    """
-    Plot the ternary diagram for nodes
-
-    Parameters
-    ----------
-
-    entity: The fracability Nodes entity
-
-    return_plot: Bool. If true return the plot. By default, false
-
-    show_plot: Bool. If true show the plot. By default, true.
-
-
-    """
-
-    figure, tax = ternary.figure(scale=100)
-    figure.set_size_inches(10, 10)
-
-    if entity.name == 'FractureNetwork':
-        nodes = entity.nodes
-    elif entity.name == 'Nodes':
-        nodes = entity
-
-    PI, PY, PX, _, CI = nodes.ternary_node_count
-    points = [(PX, PI, PY)]
-
-    tax.scatter(points, marker='o', color='red', label='Classification')
-    tax.annotate(f'{np.round(CI,2)}', position=[PX, PI, PY])
-
-    for n in range(8):
-        n += 1
-        A1 = np.array([[1, 1, 1], [0, 0, 1], [-n, 4, 0]])
-        B = np.array([1, 0, 4 - n])
-
-        X1 = np.linalg.inv(A1).dot(B) * 100
-        if n < 4:
-            side = [1, 0, 0]
-        else:
-            side = [0, 1, 0]
-        A2 = np.array([[1, 1, 1], side, [-n, 4, 0]])
-
-        X2 = np.linalg.inv(A2).dot(B) * 100
-
-        tax.line(X1, X2, color='black', linewidth=1, alpha=n / 8)
-
-    ax = tax.get_axes()
-    ax.text(76.8, 21.3, 8)
-    ax.text(74.8, 23.8, 7)
-    ax.text(73.5, 27.9, 6)
-    ax.text(71, 32.3, 5)
-    ax.text(69.1, 38, 4)
-    ax.text(65.8, 45, 3)
-    ax.text(62.7, 54, 2)
-    ax.text(57, 66.5, 1)
-
-    tax.right_corner_label("X", fontsize=15)
-    tax.top_corner_label("I", fontsize=15)
-    tax.left_corner_label("Y", fontsize=15)
-
-    tax.get_axes().set_aspect(1)  # This is used to avoid deformation when rescaling the plotter window
-    # tax.clear_matplotlib_ticks()
-    tax.get_axes().axis('off')
-    if return_plot:
-        return tax
-    else:
-        if show_plot:
-            plt.show()
```

### Comparing `fracability-1.3.2/fracability/examples/data.py` & `fracability-1.3.3/fracability/examples/data.py`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.shp` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_a.dbf` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_a.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_a.shp` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_a.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_a.shx` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_a.shx`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_b.dbf` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_b.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_b.shp` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_b.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_b.shx` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_b.shx`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_c.dbf` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_c.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_c.shp` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_c.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/Set_c.shx` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/Set_c.shx`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/lengths/Fractures_Length_set1_Pontrelli.csv` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/lengths/Fractures_Length_set1_Pontrelli.csv`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/lengths/figures/cens.png` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/lengths/figures/cens.png`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/lengths/figures/no_cens.png` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/lengths/figures/no_cens.png`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/spacing/Fractures_Spacing_pontrelli.csv` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/spacing/Fractures_Spacing_pontrelli.csv`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.dbf` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.shp` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.shx` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.shx`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.zip` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/backbone.zip`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.dbf` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.shp` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/boundaries_Pontrelli.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.dbf` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.shp` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.shx` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/fractures_Pontrelli.shx`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.dbf` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.shp` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.shx` & `fracability-1.3.3/fracability/examples/datasets/cava_pontrelli/output/topology/output_Pontrelli/nodes_Pontrelli.shx`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Interpretation_boundary.shp` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Interpretation_boundary.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/Salza_output.zip` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/Salza_output.zip`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.dbf` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.shp` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/boundaries_Salza.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.dbf` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.shp` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.shx` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/fractures_Salza.shx`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.dbf` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.shp` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.shx` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Output/nodes_Salza.shx`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_1.csv` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_1.csv`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_1.dbf` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_1.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_1.qmd` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_1.qmd`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_1.shp` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_1.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_1.shx` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_1.shx`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_2.csv` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_2.csv`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_2.dbf` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_2.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_2.qmd` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_2.qmd`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_2.shp` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_2.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/Set_2.shx` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/Set_2.shx`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/length_dist.csv` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/length_dist.csv`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.dbf` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.shp` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.shx` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/nodes_subset.shx`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.dbf` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.qmd` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.qmd`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.shp` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.shx` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_1_subset.shx`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.dbf` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.dbf`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.qmd` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.qmd`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.shp` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.shp`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.shx` & `fracability-1.3.3/fracability/examples/datasets/laghetto_salza/subset/set_2_subset.shx`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/qgis_styles/Boundary_style.qml` & `fracability-1.3.3/fracability/examples/datasets/qgis_styles/Boundary_style.qml`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/examples/datasets/qgis_styles/Nodes_style.qml` & `fracability-1.3.3/fracability/examples/datasets/qgis_styles/Nodes_style.qml`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/operations/Geometry.py` & `fracability-1.3.3/fracability/operations/Geometry.py`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/operations/Statistics.py` & `fracability-1.3.3/fracability/Statistics.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 
 from numpy import exp
 from numpy import log as ln
 import pandas as pd
 from pandas import DataFrame
 import scipy.stats as ss
 from scipy.optimize import minimize
-import ast
-import pyperclip
 
 from fracability.utils.general_use import KM
+import fracability.Plotters as plotter
 
 
 class NetworkData:
 
     """ Class used to represent fracture or fracture network data.
     It acts as a wrapper for the scipy CensoredData class
 
@@ -214,18 +213,14 @@
 
     def __init__(self, parent, obj: ss.rv_continuous = None, parameters: tuple = None, fit_data: NetworkData = None):
 
         self.parent: NetworkFitter = parent
         self._distribution = obj.freeze(*parameters)
         self.fit_data = fit_data
 
-    # @property
-    # def parent(self) -> NetworkFitter:
-    #     return self._parent
-
     @property
     def distribution(self) -> ss.rv_continuous:
         """
         Property that returns or sets a *frozen* ss.rv_continuous class
         :return:
         """
         return self._distribution
@@ -538,14 +533,16 @@
         return fitter_records.loc[fitter_records['name'] == name, 'AD_rank'].values[0]
 
     @property
     def Mean_rank(self):
         fitter_records = self.parent.fit_records()
         name = self.distribution_name
         return fitter_records.loc[fitter_records['name'] == name, 'Mean_rank'].values[0]
+
+
 class NetworkFitter:
 
     """
     Class used to fit a Fracture or Fracture network object
 
     :param obj: fracture/fracture network object
     :param use_survival: Boolean flag to use survival (True) or treat the data as if there were no censoring (False). Default is True.
@@ -582,20 +579,14 @@
         """
         return self._net_data
 
     @network_data.setter
     def network_data(self, data: NetworkData):
         self._net_data = data
 
-    def fit_records(self, sort_by='Akaike') -> DataFrame:
-
-        """ Return the sorted fit dataframe"""
-
-        return self._fit_dataframe.sort_values(by=sort_by, ignore_index=True)
-
     def fit(self, distribution_name: str):
 
         """
         Fit the data of the entity_df using scipy available distributions
         :param distribution_name: Name of the distribution to fit
         :return:
         """
@@ -643,126 +634,132 @@
         self._fit_dataframe['AD_rank'] = ss.rankdata(self._fit_dataframe['AD_distance'], nan_policy='omit').astype(int)
         self._fit_dataframe['Mean_rank'] = self._fit_dataframe.iloc[:, 8:12].mean(axis=1)
 
         self._fit_dataframe.loc[last_pos, 'distribution'] = distribution
 
         # self._fit_dataframe.loc[last_pos, 'params'] = params  # this gives out an error for setting the df, I do not know why
 
-    def get_fitted_parameters(self, distribution_name: str, sort_by='Akaike') -> tuple:
-        """
-        Get the fitted distributions parameters in the fit records df
-        :param distribution_name: Name of the distribution
-        """
-        fit_records = self.fit_records(sort_by)
-        dist = fit_records.loc[fit_records['name'] == distribution_name, 'distribution'].values[0]
-        parameters = dist.distribution_parameters
-        return parameters
-
-    def get_fitted_parameters_list(self, distribution_names: list = None, sort_by='Akaike') -> list:
-
-        """
-        Get the parameters of the computed fit(s)
-        :return: Pandas DataFrame
-        """
-
-        fit_records = self.fit_records(sort_by)
-
-        if distribution_names is None:
-            distribution_names = fit_records['name'].tolist()
-
-        parameter_list = []
+    def fit_records(self, sort_by='Akaike') -> DataFrame:
 
-        for name in distribution_names:
-            parameter_list.append(self.get_fitted_parameters(name))
+        """ Return the sorted fit dataframe"""
 
-        return parameter_list
+        return self._fit_dataframe.sort_values(by=sort_by, ignore_index=True)
 
     def get_fitted_distribution(self, distribution_name: str, sort_by='Akaike') -> NetworkDistribution:
 
         """
         get the fitted NetworkDistribution object
         :param distribution_name: name of the distribution
+        :param sort_by: Column name to sort the output order
         :return:
         """
         fit_records = self.fit_records(sort_by)
         distribution = fit_records.loc[fit_records['name'] == distribution_name, 'distribution'].values[0]
 
         return distribution
 
     def get_fitted_distribution_names(self, sort_by='Akaike') -> list:
 
         """
         get the names of the fitted NetworkDistribution object
-        :param distribution_name: name of the distribution
+        :param sort_by: Column name to sort the output order
         :return:
         """
 
         return self.fit_records(sort_by)['name'].values
 
     def get_fitted_distribution_list(self, distribution_names: list = None, sort_by='Akaike') -> list:
         """
-        Get a list of NetworkDistribution objects  fot the given distribution name
+        Get a list of NetworkDistribution objects for the given distribution name
         :param distribution_names:
+        :param sort_by: Column name to sort the output order
         :return:
         """
         fit_records = self.fit_records(sort_by)
         if distribution_names is None:
             distribution_names = fit_records['name'].tolist()
 
         distribution_list = []
 
         for name in distribution_names:
             distribution = fit_records.loc[fit_records['name'] == name, 'distribution'].values[0]
             distribution_list.append(distribution)
 
         return distribution_list
 
-    def best_fit(self, sort_by='Akaike') -> pd.Series:
+    def get_fitted_parameters(self, distribution_name: str, sort_by='Akaike') -> tuple:
+        """
+        Get the fitted distributions parameters in the fit records df
+        :param distribution_name: Name of the distribution
+        :param sort_by: Column name to sort the output order
+        """
+        fit_records = self.fit_records(sort_by)
+        dist = fit_records.loc[fit_records['name'] == distribution_name, 'distribution'].values[0]
+        parameters = dist.distribution_parameters
+        return parameters
+
+    def get_fitted_parameters_list(self, distribution_names: list = None, sort_by='Akaike') -> list:
 
         """
-        Return the best fit in the fit records dataframe
-        :return:
+        Get the parameters of the computed fit(s)
+        :return: Pandas DataFrame
         """
 
-        df = self.fit_records(sort_by)
+        fit_records = self.fit_records(sort_by)
 
-        return df.loc[0]
+        if distribution_names is None:
+            distribution_names = fit_records['name'].tolist()
+
+        parameter_list = []
+
+        for name in distribution_names:
+            parameter_list.append(self.get_fitted_parameters(name))
+
+        return parameter_list
 
-    def rejected_fit(self, sort_by='Akaike') -> pd.DataFrame:
+    def best_fit(self, sort_by='Akaike') -> pd.Series:
 
         """
-        Return the fit records dataframe without the best fit
+        Return the best fit in the fit records dataframe sorted by sort_by
         :return:
         """
 
         df = self.fit_records(sort_by)
 
-        return df.loc[1:]
+        return df.loc[0]
 
-    def best_fit_name(self, distribution_list: list = None) -> pd.Series:
+    # ====================== Plot ==========================
+
+    def plot_PIT(self,  show_plot: bool = True,
+                 position: list = None, sort_by: str = 'Akaike',
+                 bw: bool = False):
         """
-        Method used to find the best distribution using BIC ranking
-        :param distribution_list: list of distribution to test
+        Method to plot the uniform comparison plot for the fitted models.
+        :param show_plot: Bool. If True, show the plot if False do not show. Default is True.
+        :param position: List. Plot the models at the given position in the ordered fit_records dataframe. If None (default) plot all models.
+        :param sort_by: String. Column name to sort the fit_records dataframe. Default is Akaike
+        :param bw: Bool. If true turn the plot color-blind friendly (black lines with different patterns). Max 7 lines (i.e. models). Default is False
+
         :return:
         """
 
-        if distribution_list is None:
+        plotter.matplot_stats_uniform(self, show_plot, position, sort_by, bw)
 
-            distribution_list = ['lognorm',
-                                 'norm',
-                                 'expon',
-                                 'burr12',
-                                 'gamma',
-                                 'logistic']
-
-        for distribution in distribution_list:
-            self.fit(distribution)
+    def plot_summary(self, show_plot:bool = True, position: list = None, sort_by: str = 'Akaike'):
+        """
+        Method to plot the summary plot for the given fitted model(s).
+        :param show_plot: Bool. If True, show the plot if False do not show. Default is True.
+        :param position: List. Plot the models at the given position in the ordered fit_records dataframe. If None (default) plot all models.
+        :param sort_by: String. Column name to sort the fit_records dataframe. Default is Akaike
+        :return:
+        """
 
-        return self.best_fit()
+        plotter.matplot_stats_summary(self, show_plot=show_plot, position=position, sort_by=sort_by)
 
+    # ====================== Export ==========================
     def fit_result_to_csv(self, path, sort_by='Akaike'):
         """
         Save the csv to a specified path
         :param path: Path of where to save the csv
         :param sort_by: Column name to sort the values
         :return:
         """
```

### Comparing `fracability-1.3.2/fracability/operations/Topology.py` & `fracability-1.3.3/fracability/operations/Topology.py`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/utils/general_use.py` & `fracability-1.3.3/fracability/utils/general_use.py`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability/utils/shp_operations.py` & `fracability-1.3.3/fracability/utils/shp_operations.py`

 * *Files identical despite different names*

### Comparing `fracability-1.3.2/fracability.egg-info/PKG-INFO` & `fracability-1.3.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: fracability
-Version: 1.3.2
+Name: FracAbility
+Version: 1.3.3
 Summary: Analyse fracture networks for digitalized rock outcrops. 
-Author-email: Gabriele Benedetti <gabri.benedetti@gmail.com>
+Author-email: Gabriele Benedetti <gabri.benedetti@gmail.com>, Stefano Casiraghi <s.casiraghi21@campus.unimib.it>, Daniela Bertacchi <daniela.bertacchi@unimib.it>, Andrea Bistacchi <andrea.bistacchi@unimib.it>
 License: AGPL-3.0 license 
 Project-URL: Documentation, https://fracability.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/gbene/FracAbility/issues
 Project-URL: Source Code, https://github.com/gbene/FracAbility
 Keywords: DOM,censoring,fractures,fracture-networks,survival-analysis,reliability
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
@@ -31,107 +31,72 @@
 Requires-Dist: pyperclip
 Requires-Dist: pyqt5
 Requires-Dist: openpyxl
 Requires-Dist: seaborn
 Provides-Extra: all
 Requires-Dist: fracability[jupyter]; extra == "all"
 Provides-Extra: jupyter
-Requires-Dist: ipywidgets; extra == "jupyter"
-Requires-Dist: jupyter-server-proxy; extra == "jupyter"
-Requires-Dist: nest_asyncio; extra == "jupyter"
-Requires-Dist: trame>=2.5.2; extra == "jupyter"
-Requires-Dist: trame-client>=2.12.7; extra == "jupyter"
-Requires-Dist: trame-server>=2.11.7; extra == "jupyter"
-Requires-Dist: trame-vtk>=2.5.8; extra == "jupyter"
-Requires-Dist: trame-vuetify>=2.3.1; extra == "jupyter"
+Requires-Dist: jupyter; extra == "jupyter"
 
 
 <div align="center">
 
 ![](./docs/images/logo_small_small.png)
 
 [![GitHub release](https://img.shields.io/github/release/gbene/FracAbility?&sort=semver&color=orange)](https://github.com/gbene/FracAbility/releases/)
 [![License](https://img.shields.io/badge/License-AGPL--3.0-orange)](#license)
 [![issues - FracAbility](https://img.shields.io/github/issues/gbene/FracAbility)](https://github.com/gbene/FracAbility/issues)
 [![Made with Python](https://img.shields.io/badge/Python->=3.8-orange?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 ![maintained - yes](https://img.shields.io/badge/maintained-yes-green)
 </div>
 
-**FracAbility** is a Python toolbox that can be used to analyse fracture networks in digitalized rock
-outcrops. This package provides tools to:
-
-1. Define the topology of fracture networks 
-2. Statistically analyze fracture length distributions while taking into consideration 
-right censoring effects ([survival analysis](https://en.wikipedia.org/wiki/Survival_analysis)). 
-
-The name Frac**Ability** recalls the [reliability](https://github.com/MatthewReid854/reliability/tree/master)<sup>1</sup> 
-library that inspired and helped in the creation of this project. 
-
-
 ## Quick introduction ⚡
 
+![](./docs/images/oniscent_view.png)
+
 Fracture networks are essential for the analysis and modelling of mechanical and hydraulic properties 
 of rock masses. Recently, the use of Digital Outcrop Models (**DOMs**) provided a solid framework for the collection 
 of large and quantitative datasets from which different properties can be extracted.
 Because of the complex nature of exposed rock outcrops, statistical model fitting can sometimes be challenging. 
 Areas covered by rock debree, vegetation patches or simply the outer boundaries of the outcrop can 
-introduce right-censoring bias and can often lead to parameter underestimation.
-
-The following diagram represents an idealized rock outcrop. We can define the wider rectangle as the entire 
-fractured object while the smaller one as the outcrop that we can see and measure. We can immediately 
-see what is going wrong; many of the fractures that we can measure are incomplete thus leading to underestimate 
-fracture length. 
-
-![](./docs/images/example_diagram.png)
-
-Tools are needed to correct for this bias. Survival analysis techniques, although usually applied  
-in function of time and not space, accomplishes exactly this.
-
-## Features 📋
+introduce right-censoring bias and can often lead to parameter underestimation. Tools are needed to correct for estimating the correct distribution parameters while taking into account this bias. Survival analysis techniques, although usually applied in function of time and not length, accomplishes exactly this.
 
-- **Shapefile importing support**
-
-
-- **Rapid topology analysis and identification of I,Y,X and U nodes**
-
-
-- **Backbone(s) identification**
-
-
-- **Statistical analysis tools:**
-    + Empirical CDF and SF calculation
-    + Distribution fitting
-    + Statistical model testing
+**FracAbility** is a Python toolbox that can be used to analyse fracture networks and estimate length distributions considering and correcting the effect of right-censoring using survival analysis. This package provides tools to:
 
+1. Define the topology of fracture networks 
+2. Estimate multiple fracture length distributions while taking into consideration 
+right censoring effects. 
+3. Provide methods to choose the most representative distribution using both a visual and a quantitative approach  
 
-- **Plotting tools:**
-    + Network objects plotting using matplotlib or vtk
-    + Ternary node plot 
-    + Rose diagram
-    + Statistical plotting
+Please refer to the [Docs](https://fracability.readthedocs.io/en/latest/) for a more in depth introduction to the problem, theoretical background, examples and API overview. 
 
 ## Installation 🔧
 
-To install fracability pip can be used:
+To install FracAbility **pip** can be used:
 
 ```bash
 pip install fracability
 ```
 
-## Documentation
+Please refer to the [Docs](https://fracability.readthedocs.io/en/latest/Quickstart.html) for further guidance
 
-For usage details please refer to the documentation:
+## Documentation 📚
 
-[![View - Online docs](https://img.shields.io/badge/View-Online_docs-blue?style=for-the-badge)](https://fracability.readthedocs.io/en/latest/index.html "Go to online documentation")
+Click here to view the online documentation:
 
-[![view - Documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](/docs/ "Go to project documentation")
+[![View - Online docs](https://img.shields.io/badge/View-Online_docs-blue?style=for-the-badge)](https://fracability.readthedocs.io/en/latest/index.html "Go to online documentation")
 
+Click here to view the source code for the documentation:
 
+[![view - Source documentation](https://img.shields.io/badge/view-Documentation-blue?style=for-the-badge)](/docs/ "Go to project documentation")
 
-## References 🎓
 
-1. Reid, M. (2020). MatthewReid854/reliability: v0. 5.1. version v0, 5.
+## Authors 💎✨
 
+ + **Gabriele Benedetti** ([gabri.benedetti@gmail.com](mailto:gabri.benedetti@gmail.com))
+ + Stefano Casiraghi ([s.casiraghi21@campus.unimib.it](mailto:s.casiraghi21@campus.unimib.it))
+ + Daniela Bertacchi ([daniela.bertacchi@unimib.it](mailto:daniela.bertacchi@unimib.it))
+ + Andrea Bistacchi ([andrea.bistacchi@unimib.it](mailto:andrea.bistacchi@unimib.it))
 
-## License
+## License 📄
 
 Released under [AGPL-3.0](/LICENSE) by [@gbene](https://github.com/gbene)
```

### Comparing `fracability-1.3.2/fracability.egg-info/SOURCES.txt` & `fracability-1.3.3/FracAbility.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+FracAbility.egg-info/PKG-INFO
+FracAbility.egg-info/SOURCES.txt
+FracAbility.egg-info/dependency_links.txt
+FracAbility.egg-info/requires.txt
+FracAbility.egg-info/top_level.txt
 fracability/AbstractClasses.py
 fracability/Adapters.py
 fracability/Entities.py
 fracability/Plotters.py
+fracability/Statistics.py
 fracability/__init__.py
-fracability.egg-info/PKG-INFO
-fracability.egg-info/SOURCES.txt
-fracability.egg-info/dependency_links.txt
-fracability.egg-info/requires.txt
-fracability.egg-info/top_level.txt
 fracability/examples/__init__.py
 fracability/examples/data.py
 fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.cpg
 fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.dbf
 fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.prj
 fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.shp
 fracability/examples/datasets/cava_pontrelli/Interpretation_boundary.shx
@@ -111,14 +112,13 @@
 fracability/examples/datasets/laghetto_salza/subset/set_2_subset.prj
 fracability/examples/datasets/laghetto_salza/subset/set_2_subset.qmd
 fracability/examples/datasets/laghetto_salza/subset/set_2_subset.shp
 fracability/examples/datasets/laghetto_salza/subset/set_2_subset.shx
 fracability/examples/datasets/qgis_styles/Boundary_style.qml
 fracability/examples/datasets/qgis_styles/Nodes_style.qml
 fracability/operations/Geometry.py
-fracability/operations/Statistics.py
 fracability/operations/Topology.py
 fracability/operations/__init__.py
 fracability/tests/__init__.py
 fracability/utils/__init__.py
 fracability/utils/general_use.py
 fracability/utils/shp_operations.py
```

### Comparing `fracability-1.3.2/pyproject.toml` & `fracability-1.3.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
-name = 'fracability'
+name = 'FracAbility'
 description = 'Analyse fracture networks for digitalized rock outcrops. '
 authors = [
     {name = 'Gabriele Benedetti', email = 'gabri.benedetti@gmail.com'},
+    {name = 'Stefano Casiraghi', email = 's.casiraghi21@campus.unimib.it'},
+    {name = 'Daniela Bertacchi', email = 'daniela.bertacchi@unimib.it'},
+    {name = 'Andrea Bistacchi', email = 'andrea.bistacchi@unimib.it'},
 ]
 readme = 'README.md'
 requires-python = '>=3.8'
 keywords = ['DOM', 'censoring', 'fractures','fracture-networks', 'survival-analysis', 'reliability']
 license = {text = 'AGPL-3.0 license '}
 classifiers = [
     'Intended Audience :: Science/Research',
@@ -40,22 +43,15 @@
 
 dynamic = ['version']
 
 [project.optional-dependencies]
 all = ['fracability[jupyter]']
 
 jupyter = [
-    'ipywidgets',
-    'jupyter-server-proxy',
-    'nest_asyncio',
-    'trame>=2.5.2',
-    'trame-client>=2.12.7',
-    'trame-server>=2.11.7',
-    'trame-vtk>=2.5.8',
-    'trame-vuetify>=2.3.1',
+    'jupyter'
 ]
 
 [project.urls]
 Documentation = 'https://fracability.readthedocs.io/en/latest/index.html'
 "Bug Tracker" = 'https://github.com/gbene/FracAbility/issues'
 "Source Code" = 'https://github.com/gbene/FracAbility'
```

### Comparing `fracability-1.3.2/setup.py` & `fracability-1.3.3/setup.py`

 * *Files identical despite different names*

