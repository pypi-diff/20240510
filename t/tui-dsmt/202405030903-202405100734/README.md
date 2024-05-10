# Comparing `tmp/tui_dsmt-202405030903.tar.gz` & `tmp/tui_dsmt-202405100734.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsmt-202405030903.tar", last modified: Fri May  3 09:03:48 2024, max compression
+gzip compressed data, was "tui_dsmt-202405100734.tar", last modified: Fri May 10 07:34:48 2024, max compression
```

## Comparing `tui_dsmt-202405030903.tar` & `tui_dsmt-202405100734.tar`

### file list

```diff
@@ -1,65 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 09:03:48.347682 tui_dsmt-202405030903/
--rw-r--r--   0 root         (0) root         (0)      897 2024-05-03 09:03:48.347682 tui_dsmt-202405030903/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-03 09:03:48.347682 tui_dsmt-202405030903/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1291 2024-05-01 13:21:14.000000 tui_dsmt-202405030903/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 09:03:48.335682 tui_dsmt-202405030903/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 09:03:48.335682 tui_dsmt-202405030903/src/tui_dsmt/
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 09:03:48.339682 tui_dsmt-202405030903/src/tui_dsmt/clustering/
--rw-rw-rw-   0 root         (0) root         (0)     5223 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/clustering/PAM.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/clustering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2691 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/clustering/animation.py
--rw-rw-rw-   0 root         (0) root         (0)    19467 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/clustering/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/clustering/draw.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2024-04-28 07:42:19.000000 tui_dsmt-202405030903/src/tui_dsmt/clustering/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     4488 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/clustering/hierarchical.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/clustering/interactive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 09:03:48.339682 tui_dsmt-202405030903/src/tui_dsmt/fpm/
--rw-rw-rw-   0 root         (0) root         (0)    14098 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/fpm/BruteForceFI.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/fpm/ConditionalFPTree.py
--rw-rw-rw-   0 root         (0) root         (0)     5837 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/fpm/ConditionalPatternBase.py
--rw-rw-rw-   0 root         (0) root         (0)    11867 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/fpm/FPTree.py
--rw-rw-rw-   0 root         (0) root         (0)    18908 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/fpm/HashTree.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/fpm/Itemset.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/fpm/ItemsetGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     5942 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/fpm/ItemsetGridApriori.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/fpm/ItemsetGridECLAT.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2024-04-28 08:46:02.000000 tui_dsmt-202405030903/src/tui_dsmt/fpm/SequentialDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/fpm/SequentialItemset.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/fpm/TransactionDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)   112752 2024-04-28 08:46:02.000000 tui_dsmt-202405030903/src/tui_dsmt/fpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 09:03:48.343682 tui_dsmt-202405030903/src/tui_dsmt/graph/
--rw-rw-rw-   0 root         (0) root         (0)     3894 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/BFS.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/BipartiteFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/DFS.py
--rw-rw-rw-   0 root         (0) root         (0)     5843 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/Dijkstra.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/EdmondsKarp.py
--rw-rw-rw-   0 root         (0) root         (0)     4747 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/FordFulkerson.py
--rw-rw-rw-   0 root         (0) root         (0)     4461 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/Hall.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/InteractiveGraph.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/Kruskal.py
--rw-rw-rw-   0 root         (0) root         (0)     4877 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/LabelPropagation.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/MaximumFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     2705 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/RandomWalk.py
--rw-rw-rw-   0 root         (0) root         (0)   420228 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5267 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/game.py
--rw-rw-rw-   0 root         (0) root         (0)     5766 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/html.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/graph/representation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 09:03:48.343682 tui_dsmt-202405030903/src/tui_dsmt/jpanim/
--rw-rw-rw-   0 root         (0) root         (0)     2935 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/jpanim/JupyterAnimation.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/jpanim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 09:03:48.347682 tui_dsmt-202405030903/src/tui_dsmt/jpanim/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2002 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/jpanim/resources/controls-ff.html
--rw-rw-rw-   0 root         (0) root         (0)      797 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/jpanim/resources/controls.html
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/jpanim/resources/script.js
--rw-rw-rw-   0 root         (0) root         (0)      193 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/jpanim/resources/style.css
--rw-rw-rw-   0 root         (0) root         (0)   147897 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/jpanim/resources/vue-3.4.24.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 09:03:48.347682 tui_dsmt-202405030903/src/tui_dsmt/util/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-04-25 10:30:29.000000 tui_dsmt-202405030903/src/tui_dsmt/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 09:03:48.347682 tui_dsmt-202405030903/src/tui_dsmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      897 2024-05-03 09:03:48.000000 tui_dsmt-202405030903/src/tui_dsmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1828 2024-05-03 09:03:48.000000 tui_dsmt-202405030903/src/tui_dsmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 09:03:48.000000 tui_dsmt-202405030903/src/tui_dsmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      194 2024-05-03 09:03:48.000000 tui_dsmt-202405030903/src/tui_dsmt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-03 09:03:48.000000 tui_dsmt-202405030903/src/tui_dsmt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.455278 tui_dsmt-202405100734/
+-rw-r--r--   0 root         (0) root         (0)      897 2024-05-10 07:34:48.455278 tui_dsmt-202405100734/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 07:34:48.455278 tui_dsmt-202405100734/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1324 2024-05-08 12:12:17.000000 tui_dsmt-202405100734/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.415277 tui_dsmt-202405100734/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.419277 tui_dsmt-202405100734/src/tui_dsmt/
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.423277 tui_dsmt-202405100734/src/tui_dsmt/clustering/
+-rw-rw-rw-   0 root         (0) root         (0)     5223 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/PAM.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/animation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19467 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4488 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/hierarchical.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/interactive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.427277 tui_dsmt-202405100734/src/tui_dsmt/fpm/
+-rw-rw-rw-   0 root         (0) root         (0)    14098 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/BruteForceFI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/ConditionalFPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     5837 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/ConditionalPatternBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    11867 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/FPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)    18908 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/HashTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/Itemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/ItemsetGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/ItemsetGridApriori.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/ItemsetGridECLAT.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/SequentialDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/SequentialItemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/TransactionDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)   112752 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.435277 tui_dsmt-202405100734/src/tui_dsmt/graph/
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/BFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/BipartiteFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/DFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     5843 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/Dijkstra.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/EdmondsKarp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4747 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/FordFulkerson.py
+-rw-rw-rw-   0 root         (0) root         (0)     4860 2024-05-08 12:12:17.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/FruchtermanReingold.py
+-rw-rw-rw-   0 root         (0) root         (0)     4461 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/Hall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/InteractiveGraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/Kruskal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4877 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/LabelPropagation.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/MaximumFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/RandomWalk.py
+-rw-rw-rw-   0 root         (0) root         (0)   420281 2024-05-08 12:12:17.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-08 12:12:17.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)     5267 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/game.py
+-rw-rw-rw-   0 root         (0) root         (0)     6426 2024-05-08 12:12:17.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/html.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/representation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.435277 tui_dsmt-202405100734/src/tui_dsmt/graph/resources/
+-rw-rw-rw-   0 root         (0) root         (0)  8978701 2024-05-08 12:12:17.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/resources/dewiki_sample.pickle.bz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.451278 tui_dsmt-202405100734/src/tui_dsmt/jpanim/
+-rw-rw-rw-   0 root         (0) root         (0)     2935 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/JupyterAnimation.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.451278 tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/controls-ff.html
+-rw-rw-rw-   0 root         (0) root         (0)      797 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/controls.html
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/script.js
+-rw-rw-rw-   0 root         (0) root         (0)      193 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/style.css
+-rw-rw-rw-   0 root         (0) root         (0)   147897 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/vue-3.4.24.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.451278 tui_dsmt-202405100734/src/tui_dsmt/util/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.451278 tui_dsmt-202405100734/src/tui_dsmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      897 2024-05-10 07:34:48.000000 tui_dsmt-202405100734/src/tui_dsmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1955 2024-05-10 07:34:48.000000 tui_dsmt-202405100734/src/tui_dsmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 07:34:48.000000 tui_dsmt-202405100734/src/tui_dsmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      194 2024-05-10 07:34:48.000000 tui_dsmt-202405100734/src/tui_dsmt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-10 07:34:48.000000 tui_dsmt-202405100734/src/tui_dsmt.egg-info/top_level.txt
```

### Comparing `tui_dsmt-202405030903/PKG-INFO` & `tui_dsmt-202405100734/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202405030903
+Version: 202405100734
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202405030903/setup.py` & `tui_dsmt-202405100734/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,12 +34,13 @@
         'pyarrow~=15.0.2',
         'pyfpgrowth~=1.0',
         'scikit-learn~=1.4.2',
         'scikit-learn-extra~=0.3.0'
     ],
     package_data={
         'tui_dsmt': [
+            'graph/resources/*',
             'jpanim/resources/*'
         ]
     },
     include_package_data=True
 )
```

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/__init__.py` & `tui_dsmt-202405100734/src/tui_dsmt/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/clustering/PAM.py` & `tui_dsmt-202405100734/src/tui_dsmt/clustering/PAM.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/clustering/animation.py` & `tui_dsmt-202405100734/src/tui_dsmt/clustering/animation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/clustering/datasets.py` & `tui_dsmt-202405100734/src/tui_dsmt/clustering/datasets.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/clustering/evaluation.py` & `tui_dsmt-202405100734/src/tui_dsmt/clustering/evaluation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/clustering/hierarchical.py` & `tui_dsmt-202405100734/src/tui_dsmt/clustering/hierarchical.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/clustering/interactive.py` & `tui_dsmt-202405100734/src/tui_dsmt/clustering/interactive.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/fpm/BruteForceFI.py` & `tui_dsmt-202405100734/src/tui_dsmt/fpm/BruteForceFI.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/fpm/ConditionalFPTree.py` & `tui_dsmt-202405100734/src/tui_dsmt/fpm/ConditionalFPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/fpm/ConditionalPatternBase.py` & `tui_dsmt-202405100734/src/tui_dsmt/fpm/ConditionalPatternBase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/fpm/FPTree.py` & `tui_dsmt-202405100734/src/tui_dsmt/fpm/FPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/fpm/HashTree.py` & `tui_dsmt-202405100734/src/tui_dsmt/fpm/HashTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/fpm/Itemset.py` & `tui_dsmt-202405100734/src/tui_dsmt/fpm/Itemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/fpm/ItemsetGrid.py` & `tui_dsmt-202405100734/src/tui_dsmt/fpm/ItemsetGrid.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/fpm/ItemsetGridApriori.py` & `tui_dsmt-202405100734/src/tui_dsmt/fpm/ItemsetGridApriori.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/fpm/ItemsetGridECLAT.py` & `tui_dsmt-202405100734/src/tui_dsmt/fpm/ItemsetGridECLAT.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/fpm/SequentialDatabase.py` & `tui_dsmt-202405100734/src/tui_dsmt/fpm/SequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/fpm/SequentialItemset.py` & `tui_dsmt-202405100734/src/tui_dsmt/fpm/SequentialItemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/fpm/TransactionDatabase.py` & `tui_dsmt-202405100734/src/tui_dsmt/fpm/TransactionDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/fpm/__init__.py` & `tui_dsmt-202405100734/src/tui_dsmt/fpm/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/BFS.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/BFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/BipartiteFlow.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/BipartiteFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/DFS.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/DFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/Dijkstra.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/Dijkstra.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/FordFulkerson.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/FordFulkerson.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/Hall.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/Hall.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/InteractiveGraph.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/InteractiveGraph.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/Kruskal.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/Kruskal.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/LabelPropagation.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/LabelPropagation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/MaximumFlow.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/MaximumFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/RandomWalk.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/RandomWalk.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/__init__.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from .BFS import BFS
 from .BipartiteFlow import BipartiteFlow
 from .DFS import DFS
 from .Dijkstra import Dijkstra
 from .EdmondsKarp import EdmondsKarp
 from .FordFulkerson import FordFulkerson
+from .FruchtermanReingold import FruchtermanReingold
 from .Hall import Hall
 from .InteractiveGraph import InteractiveGraph
 from .Kruskal import Kruskal
 from .LabelPropagation import LabelPropagation
 from .MaximumFlow import MaximumFlow
 from .game import guess_adj_list, guess_adj_matrix
 from .RandomWalk import RandomWalk
```

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/game.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/game.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/html.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/html.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     num, unit = _split_measure(value)
     return f'`${{{num} / ({attr}.size * {scale}) + {offset}}}{unit}`'
 
 
 def graph_to_html(graph: nx.Graph, layout: Dict,
                   weights: str = None,
                   display_height: str = '40rem', max_width: str = '100%',
-                  node_width: str = '10rem', node_height: str = '2rem') -> Tuple[str, str]:
+                  node_width: str = '10rem', node_height: str = '2rem',
+                  animated_positions: bool = False) -> Tuple[str, str]:
     nodes = list(graph.nodes())
     adj = nx.to_numpy_array(graph)
 
     min_x, max_x, min_y, max_y = None, None, None, None
     for (px, py) in layout.values():
         if min_x is None or px < min_x:
             min_x = px
@@ -92,20 +93,28 @@
                     lines_svg.append(f'''
                         <line id="{id}" 
                               x1="{x1}%" y1="{y1}%" x2="{x2}%" y2="{y2}%"
                               :stroke-width="{attr}.size ?? 2" :stroke="{attr}.backgroundColor"
                               {arrow}="url(#head-{marker_id})" />
                     ''')
                 else:
-                    lines_svg.append(f'''
-                        <line id="{id}" 
-                              x1="{x1}%" y1="{y1}%" x2="{x2}%" y2="{y2}%"
-                              :stroke-width="{attr}.size ?? 2" :stroke="{attr}.backgroundColor"
-                              :stroke-dasharray="{attr}.dash" />
-                    ''')
+                    if animated_positions:
+                        lines_svg.append(f'''
+                            <line id="{id}" 
+                                  :x1="frame.edge_{source_node}_{target_node}.x1" :y1="frame.edge_{source_node}_{target_node}.y1" :x2="frame.edge_{source_node}_{target_node}.x2" :y2="frame.edge_{source_node}_{target_node}.y2"
+                                  :stroke-width="{attr}.size ?? 2" :stroke="{attr}.backgroundColor"
+                                  :stroke-dasharray="{attr}.dash" />
+                        ''')
+                    else:
+                        lines_svg.append(f'''
+                            <line id="{id}" 
+                                  x1="{x1}%" y1="{y1}%" x2="{x2}%" y2="{y2}%"
+                                  :stroke-width="{attr}.size ?? 2" :stroke="{attr}.backgroundColor"
+                                  :stroke-dasharray="{attr}.dash" />
+                        ''')
 
                 if weights is not None:
                     weight = graph.get_edge_data(source_node, target_node)[weights]
                 else:
                     weight = f'{{{{{attr}.text}}}}'
 
                 lines_svg.append(f'''
```

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/graph/representation.py` & `tui_dsmt-202405100734/src/tui_dsmt/graph/representation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/jpanim/JupyterAnimation.py` & `tui_dsmt-202405100734/src/tui_dsmt/jpanim/JupyterAnimation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/jpanim/resources/controls-ff.html` & `tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/controls-ff.html`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/jpanim/resources/controls.html` & `tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/controls.html`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/jpanim/resources/script.js` & `tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/script.js`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt/jpanim/resources/vue-3.4.24.js` & `tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/vue-3.4.24.js`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405030903/src/tui_dsmt.egg-info/PKG-INFO` & `tui_dsmt-202405100734/src/tui_dsmt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202405030903
+Version: 202405100734
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202405030903/src/tui_dsmt.egg-info/SOURCES.txt` & `tui_dsmt-202405100734/src/tui_dsmt.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -28,25 +28,28 @@
 src/tui_dsmt/fpm/__init__.py
 src/tui_dsmt/graph/BFS.py
 src/tui_dsmt/graph/BipartiteFlow.py
 src/tui_dsmt/graph/DFS.py
 src/tui_dsmt/graph/Dijkstra.py
 src/tui_dsmt/graph/EdmondsKarp.py
 src/tui_dsmt/graph/FordFulkerson.py
+src/tui_dsmt/graph/FruchtermanReingold.py
 src/tui_dsmt/graph/Hall.py
 src/tui_dsmt/graph/InteractiveGraph.py
 src/tui_dsmt/graph/Kruskal.py
 src/tui_dsmt/graph/LabelPropagation.py
 src/tui_dsmt/graph/MarkovClusterAlgorithm.py
 src/tui_dsmt/graph/MaximumFlow.py
 src/tui_dsmt/graph/RandomWalk.py
 src/tui_dsmt/graph/__init__.py
+src/tui_dsmt/graph/datasets.py
 src/tui_dsmt/graph/game.py
 src/tui_dsmt/graph/html.py
 src/tui_dsmt/graph/representation.py
+src/tui_dsmt/graph/resources/dewiki_sample.pickle.bz2
 src/tui_dsmt/jpanim/JupyterAnimation.py
 src/tui_dsmt/jpanim/__init__.py
 src/tui_dsmt/jpanim/resources/controls-ff.html
 src/tui_dsmt/jpanim/resources/controls.html
 src/tui_dsmt/jpanim/resources/script.js
 src/tui_dsmt/jpanim/resources/style.css
 src/tui_dsmt/jpanim/resources/vue-3.4.24.js
```

