# Comparing `tmp/libmoon-0.1.9.tar.gz` & `tmp/libmoon-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmoon-0.1.9.tar", last modified: Wed Feb 28 08:02:20 2024, max compression
+gzip compressed data, was "libmoon-0.2.1.tar", last modified: Fri May 10 13:24:47 2024, max compression
```

## Comparing `libmoon-0.1.9.tar` & `libmoon-0.2.1.tar`

### file list

```diff
@@ -1,116 +1,95 @@
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.877366 libmoon-0.1.9/
--rw-r--r--   0 yuan       (501) staff       (20)     1073 2024-02-22 12:26:36.000000 libmoon-0.1.9/LICENSE
--rw-r--r--   0 yuan       (501) staff       (20)    10659 2024-02-28 08:02:20.876989 libmoon-0.1.9/PKG-INFO
--rw-r--r--   0 yuan       (501) staff       (20)    10172 2024-02-28 07:52:18.000000 libmoon-0.1.9/README.md
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.856137 libmoon-0.1.9/libmoon/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-23 13:12:49.000000 libmoon-0.1.9/libmoon/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)       45 2024-02-23 13:01:09.000000 libmoon-0.1.9/libmoon/example.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.857229 libmoon-0.1.9/libmoon/problem/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-24 12:57:10.000000 libmoon-0.1.9/libmoon/problem/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)     2386 2024-02-24 13:05:45.000000 libmoon-0.1.9/libmoon/problem/mop.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.858280 libmoon-0.1.9/libmoon/problem/mtl/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-24 12:57:10.000000 libmoon-0.1.9/libmoon/problem/mtl/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/problem/mtl/fair_classify.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.859694 libmoon-0.1.9/libmoon/problem/mtl/loaders/
--rw-r--r--   0 yuan       (501) staff       (20)       45 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/problem/mtl/loaders/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)     4262 2024-02-26 07:56:37.000000 libmoon-0.1.9/libmoon/problem/mtl/loaders/adult_loader.py
--rw-r--r--   0 yuan       (501) staff       (20)     3528 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/problem/mtl/loaders/compas_loader.py
--rw-r--r--   0 yuan       (501) staff       (20)     2458 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/problem/mtl/loaders/credit_loader.py
--rw-r--r--   0 yuan       (501) staff       (20)     3249 2024-02-26 07:56:37.000000 libmoon-0.1.9/libmoon/problem/mtl/loaders/multimnist_loader.py
--rw-r--r--   0 yuan       (501) staff       (20)     8237 2024-02-26 07:56:37.000000 libmoon-0.1.9/libmoon/problem/mtl/mnist.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.860149 libmoon-0.1.9/libmoon/problem/mtl/model/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-24 12:57:10.000000 libmoon-0.1.9/libmoon/problem/mtl/model/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)     1827 2024-02-26 07:56:37.000000 libmoon-0.1.9/libmoon/problem/mtl/model/simple.py
--rw-r--r--   0 yuan       (501) staff       (20)     5488 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/problem/mtl/objectives.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.862819 libmoon-0.1.9/libmoon/problem/synthetic/
--rw-r--r--   0 yuan       (501) staff       (20)      107 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/problem/synthetic/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)     5182 2024-02-24 13:04:08.000000 libmoon-0.1.9/libmoon/problem/synthetic/dtlz.py
--rw-r--r--   0 yuan       (501) staff       (20)      856 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/problem/synthetic/maf.py
--rw-r--r--   0 yuan       (501) staff       (20)    20790 2024-02-24 13:04:44.000000 libmoon-0.1.9/libmoon/problem/synthetic/re.py
--rw-r--r--   0 yuan       (501) staff       (20)    46001 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/problem/synthetic/re_original.py
--rw-r--r--   0 yuan       (501) staff       (20)     2311 2024-02-24 13:05:14.000000 libmoon-0.1.9/libmoon/problem/synthetic/vlmop.py
--rw-r--r--   0 yuan       (501) staff       (20)        3 2024-02-24 12:57:41.000000 libmoon-0.1.9/libmoon/problem/synthetic/wfg.py
--rw-r--r--   0 yuan       (501) staff       (20)     5951 2024-02-27 07:42:37.000000 libmoon-0.1.9/libmoon/problem/synthetic/zdt.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.863115 libmoon-0.1.9/libmoon/solver/
--rw-r--r--   0 yuan       (501) staff       (20)       44 2024-02-24 08:17:53.000000 libmoon-0.1.9/libmoon/solver/__init__.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.866985 libmoon-0.1.9/libmoon/solver/gradient/
--rw-r--r--   0 yuan       (501) staff       (20)      734 2024-02-24 08:57:22.000000 libmoon-0.1.9/libmoon/solver/gradient/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)     1948 2024-02-27 12:10:35.000000 libmoon-0.1.9/libmoon/solver/gradient/base_solver.py
--rw-r--r--   0 yuan       (501) staff       (20)     1776 2024-02-24 12:41:38.000000 libmoon-0.1.9/libmoon/solver/gradient/core_solver.py
--rw-r--r--   0 yuan       (501) staff       (20)     6494 2024-02-27 13:54:25.000000 libmoon-0.1.9/libmoon/solver/gradient/epo_solver.py
--rw-r--r--   0 yuan       (501) staff       (20)     4513 2024-02-27 03:50:56.000000 libmoon-0.1.9/libmoon/solver/gradient/functions_evaluation.py
--rw-r--r--   0 yuan       (501) staff       (20)    11637 2024-02-27 08:58:41.000000 libmoon-0.1.9/libmoon/solver/gradient/functions_hv_grad_3d.py
--rw-r--r--   0 yuan       (501) staff       (20)    10125 2024-02-27 08:57:51.000000 libmoon-0.1.9/libmoon/solver/gradient/functions_hv_python3.py
--rw-r--r--   0 yuan       (501) staff       (20)     4917 2024-02-27 09:03:38.000000 libmoon-0.1.9/libmoon/solver/gradient/gradhv.py
--rw-r--r--   0 yuan       (501) staff       (20)     1704 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/gradient/mgda_core.py
--rw-r--r--   0 yuan       (501) staff       (20)     2522 2024-02-27 14:04:05.000000 libmoon-0.1.9/libmoon/solver/gradient/mgda_solver.py
--rw-r--r--   0 yuan       (501) staff       (20)    14773 2024-02-27 14:31:31.000000 libmoon-0.1.9/libmoon/solver/gradient/min_norm_solvers_numpy.py
--rw-r--r--   0 yuan       (501) staff       (20)     3411 2024-02-27 08:15:31.000000 libmoon-0.1.9/libmoon/solver/gradient/moosvgd.py
--rw-r--r--   0 yuan       (501) staff       (20)      304 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/gradient/pmgda.py
--rw-r--r--   0 yuan       (501) staff       (20)     5049 2024-02-27 14:36:50.000000 libmoon-0.1.9/libmoon/solver/gradient/pmtl.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.867384 libmoon-0.1.9/libmoon/solver/gradient/run/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-24 16:53:24.000000 libmoon-0.1.9/libmoon/solver/gradient/run/__init__.py
--rwxrwxrwx   0 yuan       (501) staff       (20)     3607 2024-02-28 04:38:01.000000 libmoon-0.1.9/libmoon/solver/gradient/run/run_grad.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.867751 libmoon-0.1.9/libmoon/solver/gradient/utils/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/gradient/utils/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)      706 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/gradient/utils/util.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.868412 libmoon-0.1.9/libmoon/solver/mobo/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-24 02:26:49.000000 libmoon-0.1.9/libmoon/solver/mobo/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)     4419 2024-02-26 07:56:37.000000 libmoon-0.1.9/libmoon/solver/mobo/dirhvego.py
--rw-r--r--   0 yuan       (501) staff       (20)     7855 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/mobo/mobod.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.868956 libmoon-0.1.9/libmoon/solver/mobo/utils/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-24 02:26:49.000000 libmoon-0.1.9/libmoon/solver/mobo/utils/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)      673 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/mobo/utils/termination.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.869681 libmoon-0.1.9/libmoon/solver/moea/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-24 02:26:49.000000 libmoon-0.1.9/libmoon/solver/moea/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)     8747 2024-02-27 03:50:51.000000 libmoon-0.1.9/libmoon/solver/moea/moead.py
--rw-r--r--   0 yuan       (501) staff       (20)     7172 2024-02-26 07:56:37.000000 libmoon-0.1.9/libmoon/solver/moea/moead_pfl.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.871499 libmoon-0.1.9/libmoon/solver/moea/utils/
--rw-r--r--   0 yuan       (501) staff       (20)      587 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/moea/utils/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)     1136 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/moea/utils/decomposition.py
--rw-r--r--   0 yuan       (501) staff       (20)     3943 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/moea/utils/genetic_operator.py
--rw-r--r--   0 yuan       (501) staff       (20)     2312 2024-02-26 07:56:37.000000 libmoon-0.1.9/libmoon/solver/moea/utils/population.py
--rw-r--r--   0 yuan       (501) staff       (20)      685 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/moea/utils/termination.py
--rw-r--r--   0 yuan       (501) staff       (20)     2686 2024-02-26 07:56:37.000000 libmoon-0.1.9/libmoon/solver/moea/utils/utils_ea.py
--rw-r--r--   0 yuan       (501) staff       (20)       21 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/moea/utils/weight_vector.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.871850 libmoon-0.1.9/libmoon/solver/pfl/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/pfl/__init__.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.872084 libmoon-0.1.9/libmoon/solver/pfl/model/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-24 02:26:49.000000 libmoon-0.1.9/libmoon/solver/pfl/model/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)      781 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/pfl/model/simple.py
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/pfl/run.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.873501 libmoon-0.1.9/libmoon/solver/psl/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-24 02:26:49.000000 libmoon-0.1.9/libmoon/solver/psl/__init__.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.874099 libmoon-0.1.9/libmoon/solver/psl/model/
--rw-r--r--   0 yuan       (501) staff       (20)       73 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/psl/model/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)     5725 2024-02-26 07:56:37.000000 libmoon-0.1.9/libmoon/solver/psl/model/mtl.py
--rw-r--r--   0 yuan       (501) staff       (20)     1227 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/psl/model/simple.py
--rw-r--r--   0 yuan       (501) staff       (20)     2587 2024-02-26 07:56:37.000000 libmoon-0.1.9/libmoon/solver/psl/run_mtl_condition.py
--rw-r--r--   0 yuan       (501) staff       (20)     2587 2024-02-26 07:56:37.000000 libmoon-0.1.9/libmoon/solver/psl/run_mtl_psl.py
--rw-r--r--   0 yuan       (501) staff       (20)     2096 2024-02-26 07:56:37.000000 libmoon-0.1.9/libmoon/solver/psl/run_simple_psl.py
--rw-r--r--   0 yuan       (501) staff       (20)      206 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/solver/psl/util.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.874601 libmoon-0.1.9/libmoon/util_global/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-24 11:10:42.000000 libmoon-0.1.9/libmoon/util_global/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)     1822 2024-02-24 13:02:55.000000 libmoon-0.1.9/libmoon/util_global/constant.py
--rw-r--r--   0 yuan       (501) staff       (20)     1987 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/util_global/scalarization.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.875184 libmoon-0.1.9/libmoon/util_global/weight_factor/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-24 11:10:42.000000 libmoon-0.1.9/libmoon/util_global/weight_factor/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)      735 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/util_global/weight_factor/das_dennis.py
--rw-r--r--   0 yuan       (501) staff       (20)      469 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/util_global/weight_factor/funs.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.876012 libmoon-0.1.9/libmoon/visulization/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-27 03:50:06.000000 libmoon-0.1.9/libmoon/visulization/__init__.py
--rw-r--r--   0 yuan       (501) staff       (20)      807 2024-02-22 09:25:31.000000 libmoon-0.1.9/libmoon/visulization/util.py
--rw-r--r--   0 yuan       (501) staff       (20)     4634 2024-02-27 13:59:04.000000 libmoon-0.1.9/libmoon/visulization/view_res.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.856966 libmoon-0.1.9/libmoon.egg-info/
--rw-r--r--   0 yuan       (501) staff       (20)    10659 2024-02-28 08:02:20.000000 libmoon-0.1.9/libmoon.egg-info/PKG-INFO
--rw-r--r--   0 yuan       (501) staff       (20)     3060 2024-02-28 08:02:20.000000 libmoon-0.1.9/libmoon.egg-info/SOURCES.txt
--rw-r--r--   0 yuan       (501) staff       (20)        1 2024-02-28 08:02:20.000000 libmoon-0.1.9/libmoon.egg-info/dependency_links.txt
--rw-r--r--   0 yuan       (501) staff       (20)      121 2024-02-28 08:02:20.000000 libmoon-0.1.9/libmoon.egg-info/requires.txt
--rw-r--r--   0 yuan       (501) staff       (20)       12 2024-02-28 08:02:20.000000 libmoon-0.1.9/libmoon.egg-info/top_level.txt
--rw-r--r--   0 yuan       (501) staff       (20)       38 2024-02-28 08:02:20.877415 libmoon-0.1.9/setup.cfg
--rw-r--r--   0 yuan       (501) staff       (20)     1223 2024-02-28 07:57:40.000000 libmoon-0.1.9/setup.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.876302 libmoon-0.1.9/src/
--rw-r--r--   0 yuan       (501) staff       (20)        0 2024-02-24 02:26:49.000000 libmoon-0.1.9/src/__init__.py
-drwxr-xr-x   0 yuan       (501) staff       (20)        0 2024-02-28 08:02:20.876592 libmoon-0.1.9/test/
--rw-r--r--   0 yuan       (501) staff       (20)      318 2024-02-22 09:25:31.000000 libmoon-0.1.9/test/test2.py
--rw-r--r--   0 yuan       (501) staff       (20)      243 2024-02-22 09:25:31.000000 libmoon-0.1.9/test/test_kernel.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.590094 libmoon-0.2.1/
+-rw-rw-rw-   0        0        0     1091 2024-04-30 06:01:28.000000 libmoon-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0    11708 2024-05-10 13:24:47.589422 libmoon-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11302 2024-04-30 07:51:24.000000 libmoon-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.321298 libmoon-0.2.1/libmoon/
+-rw-rw-rw-   0        0        0        0 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.343239 libmoon-0.2.1/libmoon/metrics/
+-rw-rw-rw-   0        0        0        0 2024-05-07 10:15:45.000000 libmoon-0.2.1/libmoon/metrics/__init__.py
+-rw-rw-rw-   0        0        0     4673 2024-05-10 13:04:48.000000 libmoon-0.2.1/libmoon/metrics/metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.344236 libmoon-0.2.1/libmoon/problem/
+-rw-rw-rw-   0        0        0        0 2024-05-08 06:07:09.000000 libmoon-0.2.1/libmoon/problem/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.366125 libmoon-0.2.1/libmoon/problem/mtl/
+-rw-rw-rw-   0        0        0        0 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/problem/mtl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.391982 libmoon-0.2.1/libmoon/problem/mtl/loaders/
+-rw-rw-rw-   0        0        0      101 2024-05-08 06:30:53.000000 libmoon-0.2.1/libmoon/problem/mtl/loaders/__init__.py
+-rw-rw-rw-   0        0        0     4289 2024-05-08 12:08:33.000000 libmoon-0.2.1/libmoon/problem/mtl/loaders/adult_loader.py
+-rw-rw-rw-   0        0        0     3865 2024-05-08 06:11:05.000000 libmoon-0.2.1/libmoon/problem/mtl/loaders/compas_loader.py
+-rw-rw-rw-   0        0        0     2488 2024-05-08 06:11:23.000000 libmoon-0.2.1/libmoon/problem/mtl/loaders/credit_loader.py
+-rw-rw-rw-   0        0        0     3249 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/problem/mtl/loaders/multimnist_loader.py
+-rw-rw-rw-   0        0        0     9174 2024-05-08 06:44:40.000000 libmoon-0.2.1/libmoon/problem/mtl/mnist.py
+-rw-rw-rw-   0        0        0      673 2024-05-08 08:38:21.000000 libmoon-0.2.1/libmoon/problem/mtl/model_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.403315 libmoon-0.2.1/libmoon/problem/mtl/models/
+-rw-rw-rw-   0        0        0       69 2024-05-08 07:56:33.000000 libmoon-0.2.1/libmoon/problem/mtl/models/__init__.py
+-rw-rw-rw-   0        0        0      437 2024-05-08 08:32:29.000000 libmoon-0.2.1/libmoon/problem/mtl/models/fair_model.py
+-rw-rw-rw-   0        0        0     1407 2024-05-08 07:58:28.000000 libmoon-0.2.1/libmoon/problem/mtl/models/lenet.py
+-rw-rw-rw-   0        0        0     4198 2024-05-08 08:26:51.000000 libmoon-0.2.1/libmoon/problem/mtl/objectives.py
+-rw-rw-rw-   0        0        0     6460 2024-05-10 05:18:40.000000 libmoon-0.2.1/libmoon/problem/mtl/run_fair_pref.py
+-rw-rw-rw-   0        0        0     6687 2024-05-10 10:59:07.000000 libmoon-0.2.1/libmoon/problem/mtl/run_fair_set.py
+-rw-rw-rw-   0        0        0     3931 2024-05-08 08:35:58.000000 libmoon-0.2.1/libmoon/problem/mtl/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.455799 libmoon-0.2.1/libmoon/problem/synthetic/
+-rw-rw-rw-   0        0        0      107 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/problem/synthetic/__init__.py
+-rw-rw-rw-   0        0        0     5206 2024-05-08 06:07:21.000000 libmoon-0.2.1/libmoon/problem/synthetic/dtlz.py
+-rw-rw-rw-   0        0        0      866 2024-04-30 11:42:42.000000 libmoon-0.2.1/libmoon/problem/synthetic/maf.py
+-rw-rw-rw-   0        0        0     2478 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/problem/synthetic/mop.py
+-rw-rw-rw-   0        0        0    21433 2024-05-08 06:07:21.000000 libmoon-0.2.1/libmoon/problem/synthetic/re.py
+-rw-rw-rw-   0        0        0    47335 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/problem/synthetic/re_original.py
+-rw-rw-rw-   0        0        0     2335 2024-05-08 06:07:21.000000 libmoon-0.2.1/libmoon/problem/synthetic/vlmop.py
+-rw-rw-rw-   0        0        0        6 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/problem/synthetic/wfg.py
+-rw-rw-rw-   0        0        0     6057 2024-05-08 06:07:21.000000 libmoon-0.2.1/libmoon/problem/synthetic/zdt.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.459788 libmoon-0.2.1/libmoon/solver/
+-rw-rw-rw-   0        0        0       45 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.472677 libmoon-0.2.1/libmoon/solver/mobo/
+-rw-rw-rw-   0        0        0        0 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/mobo/__init__.py
+-rw-rw-rw-   0        0        0     4553 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/mobo/dirhvego.py
+-rw-rw-rw-   0        0        0     8056 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/mobo/mobod.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.477590 libmoon-0.2.1/libmoon/solver/mobo/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/mobo/utils/__init__.py
+-rw-rw-rw-   0        0        0      703 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/mobo/utils/termination.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.491586 libmoon-0.2.1/libmoon/solver/moea/
+-rw-rw-rw-   0        0        0        0 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/moea/__init__.py
+-rw-rw-rw-   0        0        0     8982 2024-05-07 10:27:32.000000 libmoon-0.2.1/libmoon/solver/moea/moead.py
+-rw-rw-rw-   0        0        0     7397 2024-05-07 10:27:32.000000 libmoon-0.2.1/libmoon/solver/moea/moead_pfl.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.530615 libmoon-0.2.1/libmoon/solver/moea/utils/
+-rw-rw-rw-   0        0        0      605 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/moea/utils/__init__.py
+-rw-rw-rw-   0        0        0     1173 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/moea/utils/decomposition.py
+-rw-rw-rw-   0        0        0     4098 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/moea/utils/genetic_operator.py
+-rw-rw-rw-   0        0        0     2404 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/moea/utils/population.py
+-rw-rw-rw-   0        0        0      717 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/moea/utils/termination.py
+-rw-rw-rw-   0        0        0     2795 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/moea/utils/utils_ea.py
+-rw-rw-rw-   0        0        0       23 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/moea/utils/weight_vector.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.532613 libmoon-0.2.1/libmoon/solver/pfl/
+-rw-rw-rw-   0        0        0        0 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/pfl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.538596 libmoon-0.2.1/libmoon/solver/pfl/model/
+-rw-rw-rw-   0        0        0        0 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/pfl/model/__init__.py
+-rw-rw-rw-   0        0        0      686 2024-05-08 02:45:17.000000 libmoon-0.2.1/libmoon/solver/pfl/model/simple.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/pfl/run.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.552586 libmoon-0.2.1/libmoon/solver/psl/
+-rw-rw-rw-   0        0        0        0 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/psl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.560537 libmoon-0.2.1/libmoon/solver/psl/model/
+-rw-rw-rw-   0        0        0       74 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/psl/model/__init__.py
+-rw-rw-rw-   0        0        0     5906 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/psl/model/mtl.py
+-rw-rw-rw-   0        0        0     1747 2024-05-07 08:44:18.000000 libmoon-0.2.1/libmoon/solver/psl/model/simple.py
+-rw-rw-rw-   0        0        0     2667 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/psl/run_mtl_condition.py
+-rw-rw-rw-   0        0        0     2667 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/psl/run_mtl_psl.py
+-rw-rw-rw-   0        0        0     8182 2024-05-10 13:00:33.000000 libmoon-0.2.1/libmoon/solver/psl/run_simple_psl.py
+-rw-rw-rw-   0        0        0      218 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/solver/psl/util.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.576009 libmoon-0.2.1/libmoon/util_global/
+-rw-rw-rw-   0        0        0        0 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/util_global/__init__.py
+-rw-rw-rw-   0        0        0     2487 2024-05-09 14:52:18.000000 libmoon-0.2.1/libmoon/util_global/constant.py
+-rw-rw-rw-   0        0        0     1530 2024-05-09 07:30:31.000000 libmoon-0.2.1/libmoon/util_global/grad_util.py
+-rw-rw-rw-   0        0        0     2775 2024-05-10 12:50:32.000000 libmoon-0.2.1/libmoon/util_global/scalarization.py
+-rw-rw-rw-   0        0        0     1229 2024-05-08 11:00:10.000000 libmoon-0.2.1/libmoon/util_global/weight_factor.py
+-rw-rw-rw-   0        0        0     1122 2024-05-08 13:41:45.000000 libmoon-0.2.1/libmoon/util_global/zero_order.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.588475 libmoon-0.2.1/libmoon/visulization/
+-rw-rw-rw-   0        0        0        0 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/visulization/__init__.py
+-rw-rw-rw-   0        0        0      830 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/visulization/util.py
+-rw-rw-rw-   0        0        0     4758 2024-04-30 06:01:28.000000 libmoon-0.2.1/libmoon/visulization/view_res.py
+drwxrwxrwx   0        0        0        0 2024-05-10 13:24:47.342241 libmoon-0.2.1/libmoon.egg-info/
+-rw-rw-rw-   0        0        0    11708 2024-05-10 13:24:47.000000 libmoon-0.2.1/libmoon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2453 2024-05-10 13:24:47.000000 libmoon-0.2.1/libmoon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 13:24:47.000000 libmoon-0.2.1/libmoon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-10 13:24:47.000000 libmoon-0.2.1/libmoon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-10 13:24:47.000000 libmoon-0.2.1/libmoon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 13:24:47.590094 libmoon-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1260 2024-05-10 13:22:59.000000 libmoon-0.2.1/setup.py
```

### Comparing `libmoon-0.1.9/LICENSE` & `libmoon-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `libmoon-0.1.9/PKG-INFO` & `libmoon-0.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,184 +1,212 @@
-Metadata-Version: 2.1
-Name: libmoon
-Version: 0.1.9
-Summary: Moon, Make MOO great again
-Author: Xiaoyuan Zhang et al.
-Author-email: xzhang2523-c@my.cityu.edu.hk
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy==1.26.4
-Requires-Dist: torch==2.2.1
-Requires-Dist: matplotlib==3.8.3
-Requires-Dist: tqdm==4.66.2
-Requires-Dist: pymoo==0.6.1.1
-Requires-Dist: cvxopt==1.3.2
-Requires-Dist: cvxpy==1.4.2
-Requires-Dist: ffmpeg-python
-Requires-Dist: ffmpeg
-
-### Moon: A Standardized/Flexible Framework for MultiObjective OptimizatioN
-<img src="moon.png" alt="Moon" width="200">
-
-''
-    I raise my cup to invite the moon.
-    With my shadow we become three from one.
-''
--- Li Bai.
-
-Moon: is a multiobjective optimization framework, from single-objective optimization to multiobjective optimization, towards a better understanding of optimization problems and fair comparasions between MOO algorithms.
-
-
-
-Main contributors: Xiaoyuan Zhang (project leader), Ji Cheng, Liao Zhang, Weiduo Liao, Zhe Zhao, Xi Lin, Cheng Gong, Longcan Chen.
-
-Advised by: Prof. Yifan Chen, Prof. Zhichao Lu, Prof. Ke Shang, Prof. Tao Qin. 
-
-Corresponding to: Prof. Qingfu Zhang (CityU HK).
-
-
-
-(1) A standardlized gradient based framework. 
-
-- **Problem** class. For more problem details, please also check the Readme_problem.md file. 
-  (i) For synthetic problems,
-- 
-  | Problem                                                      | Paper                                                                | Project/Code                                         |
-  |--------------------------------------------------------------|----------------------------------------------------------------------|------------------------------------------------------|
-  | ZDT                                                          | [paper](https://ieeexplore.ieee.org/document/996017)                 | [project](https://pymoo.org/problems/multi/zdt.html) |
-  | DTLZ                                                         | [paper] | [project](https://pymoo.org/problems/many/dtlz.html) |Y                                        |
-  | MAF                                                          | [paper](https://link.springer.com/article/10.1007/s40747-017-0039-7) | [project]                         |
-  | [WFG](https://ieeexplore.ieee.org/document/996017) [code]()  | Real world problems.                                                 | Y                                                    |
-  | [Fi's](https://ieeexplore.ieee.org/document/996017) [code]() | Real world problems.                                                 | Y                                                    |
-  | RE                                                           | [paper](https://arxiv.org/abs/2009.12867)                            | [code](https://github.com/ryojitanabe/reproblems)    |
-
-
-(2) For multitask learning problems,
-
-| Problem                 | Paper | Project/Code |
-|-------------------------|------|--------------|
-| MO-MNISTs               | [PMTL](https://proceedings.neurips.cc/paper_files/paper/2019/file/685bfde03eb646c27ed565881917c71c-Paper.pdf)     | [COSMOS](https://github.com/ruchtem/cosmos)     |
-| Fairness Classification |[COSMOS](https://arxiv.org/pdf/2103.13392.pdf) |[COSMOS](https://github.com/ruchtem/cosmos) |
-| Federated Learning      | | |
-
-(3) For MORL problems,
-
-| Problem                 | Paper                                                                                                            | Project/Code                              |
-|-------------------------|------------------------------------------------------------------------------------------------------------------|-------------------------------------------|
-| Synthetic (DST FTS...)  | [Envelop](https://proceedings.neurips.cc/paper_files/paper/2019/file/4a46fbfca3f1465a27b210f4bdfe6ab3-Paper.pdf) | [code]()                                  |
-| Robotics (MO-MuJoCo...) | [PGMORL](http://proceedings.mlr.press/v119/xu20h/xu20h.pdf)                                                      | [code](https://github.com/mit-gfx/PGMORL) |
-
-
-
-
-- **Gradient-based Solver**.
-
-    | Method                                                                                                                                                                                | Property                                                              | #Obj               | Support | Published | Complexity      |
-    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------|--------------------|---------|----------|-----------------|
-    | [EPO](https://proceedings.mlr.press/v119/mahapatra20a/mahapatra20a.pdf) [code](https://github.com/dbmptr/EPOSearch)                                                                   | Exact solution.                                                       | Any                | Y       | ICML 2020 | $O(m^2 n K )$   |
-    | [COSMOS](https://arxiv.org/pdf/2103.13392.pdf) [code](https://github.com/ruchtem/cosmos)                                                                                              | Approximated exact solution.                                          | Any                | Y       | ICDM 2021| $O(m n K )$     |
-    | [MOO-SVGD](https://openreview.net/pdf?id=S2-j0ZegyrE) [code](https://github.com/gnobitab/MultiObjectiveSampling)                                                                      | A set of diverse Pareto solution.                                     | Any                | Y       | NeurIPS 2021 | $O(m^2 n K^2 )$ |
-    | [MGDA](https://proceedings.neurips.cc/paper/2018/file/432aca3a1e345e339f35a30c8f65edce-Paper.pdf) [code](https://github.com/intel-isl/MultiObjectiveOptimization)                     | Arbitray Pareto solutions. Location affected highly by initialization. | Any                | Y       | NeurIPS 2018 | $O(m^2 n K )$   |
-    | [PMTL](https://proceedings.neurips.cc/paper_files/paper/2019/file/685bfde03eb646c27ed565881917c71c-Paper.pdf) [code](https://github.com/Xi-L/ParetoMTL)                               | Pareto solutions in sectors.                                          | 2. 3 is difficult. | Y       | NeurIPS 2019 | $O(m^2 n K^2 )$ |
-    | [PMGDA](http://arxiv.org/abs/2402.09492)                                                                                                                                              | Pareto solutions satisfying any preference.                           | Any                | Y       | Under review | $O(m^2 n K )$   |
-    | [GradienHV](https://arxiv.org/abs/2102.04523) [WangHao](https://link.springer.com/chapter/10.1007/978-3-319-54157-0_44) [code](https://github.com/timodeist/multi_objective_learning) | It is a gradient-based HV method.| 2/3                | Y       | CEC 2023| $O(m^2 n K^2 )$ |   
-    | Aggregation fun. based, e.g. Tche,mTche,LS,PBI,...                                                                                                                                    | Pareto solution with aggregations.    | Any                | Y       |
-
-
-    Here, $m$ is the number of objectives, $K$ is the number of samples, and $n$ is the number of decision variables.
-    For neural network based methods, $n$ is the number of parameters; hence $n$ is very large (>10000), K is also large (e.g., 20-50), while $m$ is small (2.g., 2-4).
-
-    As a result, m^2 is not a big problem. n^2 is a big problem. K^2 is a big problem.
-
-    Time complexity of gradient based methods are as follows,
-        -1 Tier 1. GradAggSolver.
-        -2 Tier 2. MGDASolver, EPOSolver, PMTLSolver. 
-        -3 Tier 3. GradHVSolver
-        -4 Tier 4. MOOSVGDSolver
-
-    Current support:
-        GradAggSolver, MGDASolver, EPOSolver, MOOSVGDSolver, GradHVSolver, PMTLSolver.
-
-    Important things to notice:
-        The original code MOO-SVGD does not offer a MTL implement. Our code is the first open source code for MTL MOO-SVGD.
-
-
-- **PSL solvers**
-    - EPO-based
-    - Agg-based
-    - Hypernetwork-based
-    - ConditionalNet-based
-    - Simple PSL model
-    - Generative PSL model     
-    
-- **MOEA/D**
-    Current supported:
-    - Vanilla [MOEA/D](https://ieeexplore.ieee.org/document/4358754)
-    
-    - Will be released soon:
-    - [MOEA/D AWA](https://pubmed.ncbi.nlm.nih.gov/23777254/). 
-    - [MOEA/D neural AWA](https://openreview.net/pdf?id=W3T9rql5eo).
-
-    
-
-
-- **ML pretrained methods.** 
-    - HV net (https://arxiv.org/abs/2203.02185).  
-
-
-
-
-
-Example code:
-```
-from libmoon.solver.gradient import GradAggSolver
-from libmoon.util_global.constant import problem_dict
-from libmoon.util_global.weight_factor.funs import uniform_pref
-import torch
-import numpy as np
-from matplotlib import pyplot as plt
-import argparse
-
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='example')
-    parser.add_argument('--n-partition', type=int, default=10)
-    parser.add_argument('--agg', type=str, default='tche')  # If solve is agg, then choose a specific agg method.
-    parser.add_argument('--solver', type=str, default='agg')
-    parser.add_argument('--problem-name', type=str, default='VLMOP2')
-    parser.add_argument('--iter', type=int, default=1000)
-    parser.add_argument('--step-size', type=float, default=1e-2)
-    parser.add_argument('--tol', type=float, default=1e-6)
-    args = parser.parse_args()
-    
-    
-    # Init the solver, problem and prefs. 
-    solver = GradAggSolver(args.step_size, args.iter, args.tol)
-    problem = problem_dict[args.problem_name]
-    prefs = uniform_pref(args.n_partition, problem.n_obj, clip_eps=1e-2)
-    args.n_prob = len(prefs)
-
-    # Initialize the initial solution 
-    if 'lbound' in dir(problem):
-        if args.problem_name == 'VLMOP1':
-            x0 = torch.rand(args.n_prob, problem.n_var) * 2 / np.sqrt(problem.n_var) - 1 / np.sqrt(problem.n_var)
-        else:
-            x0 = torch.rand(args.n_prob, problem.n_var)
-    else:
-        x0 = torch.rand( args.n_prob, problem.n_var )*20 - 10
-
-
-    # Solve results
-    res = solver.solve(problem, x=x0, prefs=prefs, args=args)
-    
-    # Visualize results
-    y_arr = res['y']
-    plt.scatter(y_arr[:,0], y_arr[:,1], s=50)
-    plt.xlabel('$f_1$', fontsize=20)
-    plt.ylabel('$f_2$', fontsize=20)
-    plt.show()
-
-    
-
+### Moon: A Standardized/Flexible Framework for MultiObjective OptimizatioN
+
+
+<img src="moon.png" alt="Moon" width="200">
+
+# Moon: A Multiobjective Optimization Framework
+
+## Introduction
+**Moon** is a multiobjective optimization framework that spans from single-objective optimization to multiobjective optimization. It aims to enhance the understanding of optimization problems and facilitate fair comparisons between MOO algorithms.
+
+> "I raise my cup to invite the moon.  
+> With my shadow we become three from one."  
+> -- Li Bai
+
+## Main Contributors
+- **Xiaoyuan Zhang** (Project Leader)
+- Ji Cheng
+- Liao Zhao
+- Weiduo Liao
+- Zhe Zhao
+- Xi Lin
+- Cheng Gong
+- Longcan Chen
+- YingYing Yu
+
+## Advisory Board
+- **Prof. Yifan Chen** (Hong Kong Baptist University)
+- **Prof. Zhichao Lu** (City University of Hong Kong)
+- **Prof. Ke Shang** (Shenzhen University)
+- **Prof. Tao Qin** (Microsoft Research)
+- **Prof. Han Zhao** (University of Illinois at Urbana-Champaign)
+
+## Correspondence
+For any inquiries, please contact **Prof. Qingfu Zhang** (City University of Hong Kong) at the corresponding address.
+
+## Resources
+For more information on methodologies, please visit our [GitHub repository](https://github.com/xzhang2523/awesome-moo-ml-papers). Contributions and stars are welcome!
+
+
+
+(1) A standardlized gradient based framework. 
+# Optimization Problem Classes
+
+## **Problem Class Details**
+For more information on problem specifics, please refer to the `Readme_problem.md` file.
+
+### Synthetic Problems
+Here's a list of synthetic problems along with relevant research papers and project/code links:
+
+| Problem | Paper | Project/Code |
+|---------|-------|--------------|
+| ZDT     | [Paper](https://ieeexplore.ieee.org/document/996017) | [Project](https://pymoo.org/problems/multi/zdt.html) |
+| DTLZ    | [Paper](https://ieeexplore.ieee.org/document/996017) | [Project](https://pymoo.org/problems/many/dtlz.html) |
+| MAF     | [Paper](https://link.springer.com/article/10.1007/s40747-017-0039-7) | [Project](https://pymoo.org/problems/multi/maf.html) |
+| WFG     | [Paper](https://ieeexplore.ieee.org/document/996017) | [Code](https://github.com/sample-repo/wfg-code) |
+| Fi's    | [Paper](https://ieeexplore.ieee.org/document/996017) | [Code](https://github.com/sample-repo/fis-code) |
+| RE      | [Paper](https://arxiv.org/abs/2009.12867) | [Code](https://github.com/ryojitanabe/reproblems) |
+
+### Multitask Learning Problems
+
+This section details problems related to multitask learning, along with their corresponding papers and project/code references:
+
+| Problem              | Paper                                                                                                           | Project/Code                                   |
+|----------------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------------|
+| MO-MNISTs            | [PMTL](https://proceedings.neurips.cc/paper_files/paper/2019/file/685bfde03eb646c27ed565881917c71c-Paper.pdf) | [COSMOS](https://github.com/ruchtem/cosmos)    |
+| Fairness Classification | [COSMOS](https://arxiv.org/pdf/2103.13392.pdf)                                                                  | [COSMOS](https://github.com/ruchtem/cosmos)    |
+| Federated Learning   | [Federal MTL](https://proceedings.neurips.cc/paper_files/paper/2023/file/7cb2c2a8d35576c00078b6591ec26a7d-Paper.pdf) | [COSMOS](https://github.com/ruchtem/cosmos) |
+| Synthetic (DST, FTS...) | [Envelop](https://proceedings.neurips.cc/paper_files/paper/2019/file/4a46fbfca3f1465a27b210f4bdfe6ab3-Paper.pdf) | [Project](https://github.com/sample-repo/envelop-code) |
+| Robotics (MO-MuJoCo...) | [PGMORL](http://proceedings.mlr.press/v119/xu20h/xu20h.pdf)                                                      | [Code](https://github.com/mit-gfx/PGMORL)     |
+
+
+
+- **Gradient-based Solver**.
+
+    | Method                                                                                                                                                                                | Property                                                              | #Obj               | Support | Published | Complexity      |
+    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------|--------------------|---------|----------|-----------------|
+    | [EPO](https://proceedings.mlr.press/v119/mahapatra20a/mahapatra20a.pdf) [code](https://github.com/dbmptr/EPOSearch)                                                                   | Exact solution.                                                       | Any                | Y       | ICML 2020 | $O(m^2 n K )$   |
+    | [COSMOS](https://arxiv.org/pdf/2103.13392.pdf) [code](https://github.com/ruchtem/cosmos)                                                                                              | Approximated exact solution.                                          | Any                | Y       | ICDM 2021| $O(m n K )$     |
+    | [MOO-SVGD](https://openreview.net/pdf?id=S2-j0ZegyrE) [code](https://github.com/gnobitab/MultiObjectiveSampling)                                                                      | A set of diverse Pareto solution.                                     | Any                | Y       | NeurIPS 2021 | $O(m^2 n K^2 )$ |
+    | [MGDA](https://proceedings.neurips.cc/paper/2018/file/432aca3a1e345e339f35a30c8f65edce-Paper.pdf) [code](https://github.com/intel-isl/MultiObjectiveOptimization)                     | Arbitray Pareto solutions. Location affected highly by initialization. | Any                | Y       | NeurIPS 2018 | $O(m^2 n K )$   |
+    | [PMTL](https://proceedings.neurips.cc/paper_files/paper/2019/file/685bfde03eb646c27ed565881917c71c-Paper.pdf) [code](https://github.com/Xi-L/ParetoMTL)                               | Pareto solutions in sectors.                                          | 2. 3 is difficult. | Y       | NeurIPS 2019 | $O(m^2 n K^2 )$ |
+    | [PMGDA](http://arxiv.org/abs/2402.09492)                                                                                                                                              | Pareto solutions satisfying any preference.                           | Any                | Y       | Under review | $O(m^2 n K )$   |
+    | [GradienHV](https://arxiv.org/abs/2102.04523) [WangHao](https://link.springer.com/chapter/10.1007/978-3-319-54157-0_44) [code](https://github.com/timodeist/multi_objective_learning) | It is a gradient-based HV method.| 2/3                | Y       | CEC 2023| $O(m^2 n K^2 )$ |   
+    | Aggregation fun. based, e.g. Tche,mTche,LS,PBI,...                                                                                                                                    | Pareto solution with aggregations.    | Any                | Y       |
+
+
+    Here, $m$ is the number of objectives, $K$ is the number of samples, and $n$ is the number of decision variables.
+    For neural network based methods, $n$ is the number of parameters; hence $n$ is very large (>10000), K is also large (e.g., 20-50), while $m$ is small (2.g., 2-4).
+
+    As a result, m^2 is not a big problem. n^2 is a big problem. K^2 is a big problem.
+
+    Time complexity of gradient based methods are as follows,
+        -1 Tier 1. GradAggSolver.
+        -2 Tier 2. MGDASolver, EPOSolver, PMTLSolver. 
+        -3 Tier 3. GradHVSolver
+        -4 Tier 4. MOOSVGDSolver
+
+    Current support:
+        GradAggSolver, MGDASolver, EPOSolver, MOOSVGDSolver, GradHVSolver, PMTLSolver.
+
+    Important things to notice:
+        The original code MOO-SVGD does not offer a MTL implement. Our code is the first open source code for MTL MOO-SVGD.
+
+## Supported Solvers
+
+### Current Support
+Libmoon includes a variety of solvers tailored for different needs:
+- GradAggSolver
+- MGDASolver
+- EPOSolver
+- MOOSVGDSolver (*)
+- GradHVSolver
+- PMTLSolver
+
+(*) The original MOO-SVGD code does not include an implementation for Multitask Learning (MTL). Our release of MOO-SVGD is the first open-source code that supports MTL.
+
+## PSL (Pareto set learning) Solvers
+
+Libmoon supports various models of PSL solvers, categorized as follows:
+- EPO-based PSL model
+- Agg-based PSL model 
+- Hypernetwork-based PSL model 
+- ConditionalNet-based PSL model 
+- Simple PSL model
+- Generative PSL model
+
+
+
+
+## MOEA/D Framework
+
+### Currently Supported
+- Vanilla [MOEA/D](https://ieeexplore.ieee.org/document/4358754)
+
+### Upcoming Releases
+- [MOEA/D AWA](https://pubmed.ncbi.nlm.nih.gov/23777254/)
+- [MOEA/D Neural AWA](https://openreview.net/pdf?id=W3T9rql5eo)
+
+## ML Pretrained Methods
+- HV Net, a model for handling high-volume data, available [here](https://arxiv.org/abs/2203.02185).
+
+## Installation
+
+Libmoon is available on PyPI. You can install it using pip:
+
+```bash
+pip install libmoon==0.1.11
+
+
+Example code for a synthetic problem,
+```
+from libmoon.solver.gradient import GradAggSolver
+from libmoon.util_global.constant import problem_dict
+from libmoon.util_global.weight_factor.funs import uniform_pref
+import torch
+import numpy as np
+from matplotlib import pyplot as plt
+import argparse
+from libmoon.visulization.view_res import vedio_res
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser(description='example')
+    parser.add_argument('--n-partition', type=int, default=10)
+    parser.add_argument('--agg', type=str, default='tche')  # If solve is agg, then choose a specific agg method.
+    parser.add_argument('--solver', type=str, default='agg')
+    parser.add_argument('--problem-name', type=str, default='VLMOP2')
+    parser.add_argument('--iter', type=int, default=1000)
+    parser.add_argument('--step-size', type=float, default=1e-2)
+    parser.add_argument('--tol', type=float, default=1e-6)
+    args = parser.parse_args()
+    
+    
+    # Init the solver, problem and prefs. 
+    solver = GradAggSolver(args.step_size, args.iter, args.tol)
+    problem = problem_dict[args.problem_name]
+    prefs = uniform_pref(args.n_partition, problem.n_obj, clip_eps=1e-2)
+    args.n_prob = len(prefs)
+
+    # Initialize the initial solution 
+    if 'lbound' in dir(problem):
+        if args.problem_name == 'VLMOP1':
+            x0 = torch.rand(args.n_prob, problem.n_var) * 2 / np.sqrt(problem.n_var) - 1 / np.sqrt(problem.n_var)
+        else:
+            x0 = torch.rand(args.n_prob, problem.n_var)
+    else:
+        x0 = torch.rand( args.n_prob, problem.n_var )*20 - 10
+
+
+    # Solve results
+    res = solver.solve(problem, x=x0, prefs=prefs, args=args)
+    
+    # Visualize results
+    y_arr = res['y']
+    plt.scatter(y_arr[:,0], y_arr[:,1], s=50)
+    plt.xlabel('$f_1$', fontsize=20)
+    plt.ylabel('$f_2$', fontsize=20)
+    plt.show()
+    
+    # If use vedio
+    use_vedio=True
+    if use_vedio:
+        vedio_res(res, problem, prefs, args)     
+```
+        
+Example of MTL
+```
+
+
+```
+
+    
+
```

### Comparing `libmoon-0.1.9/README.md` & `libmoon-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,89 @@
+Metadata-Version: 2.1
+Name: libmoon
+Version: 0.2.1
+Summary: Moon, Make MOO great again
+Author: Xiaoyuan Zhang et al.
+Author-email: xzhang2523-c@my.cityu.edu.hk
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ### Moon: A Standardized/Flexible Framework for MultiObjective OptimizatioN
-<img src="moon.png" alt="Moon" width="200">
 
-''
-    I raise my cup to invite the moon.
-    With my shadow we become three from one.
-''
--- Li Bai.
 
-Moon: is a multiobjective optimization framework, from single-objective optimization to multiobjective optimization, towards a better understanding of optimization problems and fair comparasions between MOO algorithms.
+<img src="moon.png" alt="Moon" width="200">
 
+# Moon: A Multiobjective Optimization Framework
 
+## Introduction
+**Moon** is a multiobjective optimization framework that spans from single-objective optimization to multiobjective optimization. It aims to enhance the understanding of optimization problems and facilitate fair comparisons between MOO algorithms.
 
-Main contributors: Xiaoyuan Zhang (project leader), Ji Cheng, Liao Zhang, Weiduo Liao, Zhe Zhao, Xi Lin, Cheng Gong, Longcan Chen.
+> "I raise my cup to invite the moon.  
+> With my shadow we become three from one."  
+> -- Li Bai
+
+## Main Contributors
+- **Xiaoyuan Zhang** (Project Leader)
+- Ji Cheng
+- Liao Zhao
+- Weiduo Liao
+- Zhe Zhao
+- Xi Lin
+- Cheng Gong
+- Longcan Chen
+- YingYing Yu
+
+## Advisory Board
+- **Prof. Yifan Chen** (Hong Kong Baptist University)
+- **Prof. Zhichao Lu** (City University of Hong Kong)
+- **Prof. Ke Shang** (Shenzhen University)
+- **Prof. Tao Qin** (Microsoft Research)
+- **Prof. Han Zhao** (University of Illinois at Urbana-Champaign)
 
-Advised by: Prof. Yifan Chen, Prof. Zhichao Lu, Prof. Ke Shang, Prof. Tao Qin. 
+## Correspondence
+For any inquiries, please contact **Prof. Qingfu Zhang** (City University of Hong Kong) at the corresponding address.
 
-Corresponding to: Prof. Qingfu Zhang (CityU HK).
+## Resources
+For more information on methodologies, please visit our [GitHub repository](https://github.com/xzhang2523/awesome-moo-ml-papers). Contributions and stars are welcome!
 
 
 
 (1) A standardlized gradient based framework. 
+# Optimization Problem Classes
 
-- **Problem** class. For more problem details, please also check the Readme_problem.md file. 
-  (i) For synthetic problems,
-- 
-  | Problem                                                      | Paper                                                                | Project/Code                                         |
-  |--------------------------------------------------------------|----------------------------------------------------------------------|------------------------------------------------------|
-  | ZDT                                                          | [paper](https://ieeexplore.ieee.org/document/996017)                 | [project](https://pymoo.org/problems/multi/zdt.html) |
-  | DTLZ                                                         | [paper] | [project](https://pymoo.org/problems/many/dtlz.html) |Y                                        |
-  | MAF                                                          | [paper](https://link.springer.com/article/10.1007/s40747-017-0039-7) | [project]                         |
-  | [WFG](https://ieeexplore.ieee.org/document/996017) [code]()  | Real world problems.                                                 | Y                                                    |
-  | [Fi's](https://ieeexplore.ieee.org/document/996017) [code]() | Real world problems.                                                 | Y                                                    |
-  | RE                                                           | [paper](https://arxiv.org/abs/2009.12867)                            | [code](https://github.com/ryojitanabe/reproblems)    |
-
-
-(2) For multitask learning problems,
-
-| Problem                 | Paper | Project/Code |
-|-------------------------|------|--------------|
-| MO-MNISTs               | [PMTL](https://proceedings.neurips.cc/paper_files/paper/2019/file/685bfde03eb646c27ed565881917c71c-Paper.pdf)     | [COSMOS](https://github.com/ruchtem/cosmos)     |
-| Fairness Classification |[COSMOS](https://arxiv.org/pdf/2103.13392.pdf) |[COSMOS](https://github.com/ruchtem/cosmos) |
-| Federated Learning      | | |
-
-(3) For MORL problems,
-
-| Problem                 | Paper                                                                                                            | Project/Code                              |
-|-------------------------|------------------------------------------------------------------------------------------------------------------|-------------------------------------------|
-| Synthetic (DST FTS...)  | [Envelop](https://proceedings.neurips.cc/paper_files/paper/2019/file/4a46fbfca3f1465a27b210f4bdfe6ab3-Paper.pdf) | [code]()                                  |
-| Robotics (MO-MuJoCo...) | [PGMORL](http://proceedings.mlr.press/v119/xu20h/xu20h.pdf)                                                      | [code](https://github.com/mit-gfx/PGMORL) |
+## **Problem Class Details**
+For more information on problem specifics, please refer to the `Readme_problem.md` file.
 
+### Synthetic Problems
+Here's a list of synthetic problems along with relevant research papers and project/code links:
+
+| Problem | Paper | Project/Code |
+|---------|-------|--------------|
+| ZDT     | [Paper](https://ieeexplore.ieee.org/document/996017) | [Project](https://pymoo.org/problems/multi/zdt.html) |
+| DTLZ    | [Paper](https://ieeexplore.ieee.org/document/996017) | [Project](https://pymoo.org/problems/many/dtlz.html) |
+| MAF     | [Paper](https://link.springer.com/article/10.1007/s40747-017-0039-7) | [Project](https://pymoo.org/problems/multi/maf.html) |
+| WFG     | [Paper](https://ieeexplore.ieee.org/document/996017) | [Code](https://github.com/sample-repo/wfg-code) |
+| Fi's    | [Paper](https://ieeexplore.ieee.org/document/996017) | [Code](https://github.com/sample-repo/fis-code) |
+| RE      | [Paper](https://arxiv.org/abs/2009.12867) | [Code](https://github.com/ryojitanabe/reproblems) |
+
+### Multitask Learning Problems
+
+This section details problems related to multitask learning, along with their corresponding papers and project/code references:
+
+| Problem              | Paper                                                                                                           | Project/Code                                   |
+|----------------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------------|
+| MO-MNISTs            | [PMTL](https://proceedings.neurips.cc/paper_files/paper/2019/file/685bfde03eb646c27ed565881917c71c-Paper.pdf) | [COSMOS](https://github.com/ruchtem/cosmos)    |
+| Fairness Classification | [COSMOS](https://arxiv.org/pdf/2103.13392.pdf)                                                                  | [COSMOS](https://github.com/ruchtem/cosmos)    |
+| Federated Learning   | [Federal MTL](https://proceedings.neurips.cc/paper_files/paper/2023/file/7cb2c2a8d35576c00078b6591ec26a7d-Paper.pdf) | [COSMOS](https://github.com/ruchtem/cosmos) |
+| Synthetic (DST, FTS...) | [Envelop](https://proceedings.neurips.cc/paper_files/paper/2019/file/4a46fbfca3f1465a27b210f4bdfe6ab3-Paper.pdf) | [Project](https://github.com/sample-repo/envelop-code) |
+| Robotics (MO-MuJoCo...) | [PGMORL](http://proceedings.mlr.press/v119/xu20h/xu20h.pdf)                                                      | [Code](https://github.com/mit-gfx/PGMORL)     |
 
 
 
 - **Gradient-based Solver**.
 
     | Method                                                                                                                                                                                | Property                                                              | #Obj               | Support | Published | Complexity      |
     |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------|--------------------|---------|----------|-----------------|
@@ -79,50 +110,70 @@
 
     Current support:
         GradAggSolver, MGDASolver, EPOSolver, MOOSVGDSolver, GradHVSolver, PMTLSolver.
 
     Important things to notice:
         The original code MOO-SVGD does not offer a MTL implement. Our code is the first open source code for MTL MOO-SVGD.
 
+## Supported Solvers
 
-- **PSL solvers**
-    - EPO-based
-    - Agg-based
-    - Hypernetwork-based
-    - ConditionalNet-based
-    - Simple PSL model
-    - Generative PSL model     
-    
-- **MOEA/D**
-    Current supported:
-    - Vanilla [MOEA/D](https://ieeexplore.ieee.org/document/4358754)
-    
-    - Will be released soon:
-    - [MOEA/D AWA](https://pubmed.ncbi.nlm.nih.gov/23777254/). 
-    - [MOEA/D neural AWA](https://openreview.net/pdf?id=W3T9rql5eo).
+### Current Support
+Libmoon includes a variety of solvers tailored for different needs:
+- GradAggSolver
+- MGDASolver
+- EPOSolver
+- MOOSVGDSolver (*)
+- GradHVSolver
+- PMTLSolver
+
+(*) The original MOO-SVGD code does not include an implementation for Multitask Learning (MTL). Our release of MOO-SVGD is the first open-source code that supports MTL.
+
+## PSL (Pareto set learning) Solvers
+
+Libmoon supports various models of PSL solvers, categorized as follows:
+- EPO-based PSL model
+- Agg-based PSL model 
+- Hypernetwork-based PSL model 
+- ConditionalNet-based PSL model 
+- Simple PSL model
+- Generative PSL model
 
-    
 
 
-- **ML pretrained methods.** 
-    - HV net (https://arxiv.org/abs/2203.02185).  
 
+## MOEA/D Framework
 
+### Currently Supported
+- Vanilla [MOEA/D](https://ieeexplore.ieee.org/document/4358754)
 
+### Upcoming Releases
+- [MOEA/D AWA](https://pubmed.ncbi.nlm.nih.gov/23777254/)
+- [MOEA/D Neural AWA](https://openreview.net/pdf?id=W3T9rql5eo)
 
+## ML Pretrained Methods
+- HV Net, a model for handling high-volume data, available [here](https://arxiv.org/abs/2203.02185).
 
-Example code:
+## Installation
+
+Libmoon is available on PyPI. You can install it using pip:
+
+```bash
+pip install libmoon==0.1.11
+
+
+Example code for a synthetic problem,
 ```
 from libmoon.solver.gradient import GradAggSolver
 from libmoon.util_global.constant import problem_dict
 from libmoon.util_global.weight_factor.funs import uniform_pref
 import torch
 import numpy as np
 from matplotlib import pyplot as plt
 import argparse
+from libmoon.visulization.view_res import vedio_res
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='example')
     parser.add_argument('--n-partition', type=int, default=10)
     parser.add_argument('--agg', type=str, default='tche')  # If solve is agg, then choose a specific agg method.
     parser.add_argument('--solver', type=str, default='agg')
     parser.add_argument('--problem-name', type=str, default='VLMOP2')
@@ -153,10 +204,22 @@
     
     # Visualize results
     y_arr = res['y']
     plt.scatter(y_arr[:,0], y_arr[:,1], s=50)
     plt.xlabel('$f_1$', fontsize=20)
     plt.ylabel('$f_2$', fontsize=20)
     plt.show()
+    
+    # If use vedio
+    use_vedio=True
+    if use_vedio:
+        vedio_res(res, problem, prefs, args)     
+```
+        
+Example of MTL
+```
+
+
+```
```

### Comparing `libmoon-0.1.9/libmoon/problem/mop.py` & `libmoon-0.2.1/libmoon/problem/synthetic/mop.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import numpy as np
-import torch
-
-class mop():
-    def __init__(self,
-                 n_var: int,
-                 n_obj: int,
-                 lbound: np.ndarray,
-                 ubound: np.ndarray,
-                 n_cons: int=0,
-                 ) -> None:
-
-        self.n_var = n_var
-        self.n_obj = n_obj
-        self.n_cons = n_cons
-
-        self.lbound=lbound
-        self.ubound=ubound
-
-
-    @property
-    def get_number_variable(self) -> int:
-        return self.n_var
-
-    @property
-    def get_number_objective(self) -> int:
-        return self.n_obj
-
-    @property
-    def get_lower_bound(self) -> np.ndarray:
-        return self.lbound
-
-    @property
-    def get_upper_bound(self) -> np.ndarray:
-        return self.ubound
-
-    @property
-    def has_constraint(self) -> bool:
-        return self.n_cons > 0
-
-    def evaluate(self, x):
-        raise NotImplementedError("Subclasses should implement this method.")
-
-    def __call__(self, x):
-        return self.evaluate(x)
-
-    def evaluate(self, x: any) -> any:
-        """
-            Evaluate the objectives for x
-            Parameters
-            ----------
-            x : any
-                Tensor or ndarray
-            Returns
-            -------
-            any
-                Tensor or ndarray correspondingly
-            Raises
-            ------
-            ValueError
-                wrong type of x
-        """
-
-        if type(x) == torch.Tensor:
-            return self._evaluate_torch(torch.atleast_2d(x))
-        elif isinstance(x, np.ndarray):
-            return self._evaluate_numpy(np.atleast_2d(x))
-        else:
-            raise ValueError("Input has to be in the form of Tensor or ndarray!")
-
-    def get_pf(self, n_points: int=100) -> np.ndarray:
-        """
-        Get Pareto front
-        Parameters
-        ----------
-        num_points : int, optional
-            _description_, by default 100
-        Returns
-        -------
-        np.ndarray
-            _description_
-        """
-        # TODO
-        # if method=='uniform':
-        if hasattr(self, "_get_pf"): return self._get_pf(n_points)
-        else: raise NotImplementedError("Subclasses should implement this method.")
-
-
-
-class mop_noCons(mop):
-
-    def __init__(self, n_var: int, n_obj: int, lbound: np.ndarray, ubound: np.ndarray, n_cons: int = 0) -> None:
+import numpy as np
+import torch
+
+class mop():
+    def __init__(self,
+                 n_var: int,
+                 n_obj: int,
+                 lbound: np.ndarray,
+                 ubound: np.ndarray,
+                 n_cons: int=0,
+                 ) -> None:
+
+        self.n_var = n_var
+        self.n_obj = n_obj
+        self.n_cons = n_cons
+
+        self.lbound=lbound
+        self.ubound=ubound
+
+
+    @property
+    def get_number_variable(self) -> int:
+        return self.n_var
+
+    @property
+    def get_number_objective(self) -> int:
+        return self.n_obj
+
+    @property
+    def get_lower_bound(self) -> np.ndarray:
+        return self.lbound
+
+    @property
+    def get_upper_bound(self) -> np.ndarray:
+        return self.ubound
+
+    @property
+    def has_constraint(self) -> bool:
+        return self.n_cons > 0
+
+    def evaluate(self, x):
+        raise NotImplementedError("Subclasses should implement this method.")
+
+    def __call__(self, x):
+        return self.evaluate(x)
+
+    def evaluate(self, x: any) -> any:
+        """
+            Evaluate the objectives for x
+            Parameters
+            ----------
+            x : any
+                Tensor or ndarray
+            Returns
+            -------
+            any
+                Tensor or ndarray correspondingly
+            Raises
+            ------
+            ValueError
+                wrong type of x
+        """
+
+        if type(x) == torch.Tensor:
+            return self._evaluate_torch(torch.atleast_2d(x))
+        elif isinstance(x, np.ndarray):
+            return self._evaluate_numpy(np.atleast_2d(x))
+        else:
+            raise ValueError("Input has to be in the form of Tensor or ndarray!")
+
+    def get_pf(self, n_points: int=100) -> np.ndarray:
+        """
+        Get Pareto front
+        Parameters
+        ----------
+        num_points : int, optional
+            _description_, by default 100
+        Returns
+        -------
+        np.ndarray
+            _description_
+        """
+        # TODO
+        # if method=='uniform':
+        if hasattr(self, "_get_pf"): return self._get_pf(n_points)
+        else: raise NotImplementedError("Subclasses should implement this method.")
+
+
+
+class mop_noCons(mop):
+
+    def __init__(self, n_var: int, n_obj: int, lbound: np.ndarray, ubound: np.ndarray, n_cons: int = 0) -> None:
         super().__init__(n_var, n_obj, lbound, ubound, n_cons)
```

### Comparing `libmoon-0.1.9/libmoon/problem/mtl/loaders/adult_loader.py` & `libmoon-0.2.1/libmoon/problem/mtl/loaders/adult_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,22 +60,17 @@
 
 
 class ADULT(data.Dataset):
 
 
     def __init__(self, split="train", sensible_attribute="gender"):
         assert split in ["train", "val", "test"]
-
         # folder_name = os.path.dirname( os.path.dirname(__file__) )
 
-
-
-
-        path = os.path.join(root_name, 'mtldata', "adult.csv")
-
+        path = os.path.join(root_name, 'libmoon', 'problem', 'mtl', 'mtl_data', 'adult', "adult.csv")
         x, y, s1 = load_dataset(path, sensible_attribute)
 
 
         x = torch.from_numpy(x).float()
         y = torch.from_numpy(y).long()
         s1 = torch.from_numpy(s1).long()
         # s2 = torch.from_numpy(s2).long()
@@ -111,14 +106,14 @@
     def __getitem__(self, index):
         return dict(data=self.x[index], labels=self.y[index], sensible_attribute=self.s1[index])
 
     def task_names(self):
         return None
 
 
-    
+
 if __name__ == "__main__":
     dataset = ADULT(split="train")
     trainloader = data.DataLoader(dataset, batch_size=256, num_workers=0)
 
     for i, data in enumerate(trainloader):
-        break
+        print()
```

### Comparing `libmoon-0.1.9/libmoon/problem/mtl/loaders/compas_loader.py` & `libmoon-0.2.1/libmoon/problem/mtl/loaders/compas_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,28 +48,28 @@
     data1 = data.copy()
     data1 = data1.drop(['two_year_recid', 'sex'], axis=1)
     data1 = pd.get_dummies(data1)
 
     x = StandardScaler().fit(data1).transform(data1)
     y = data['two_year_recid'].values
     s = data['sex'].values
-
     return x, y, s
 
 
+
 class Compas(torch.utils.data.Dataset):
 
     def __init__(self, split, sensible_attribute='sex'):
         assert split in ['train', 'val', 'test']
 
-        folder_name = os.path.dirname(os.path.dirname(__file__))
-        path = os.path.join(folder_name, 'mtldata', "compas.csv")
+        from libmoon.util_global.constant import root_name
+        # folder_name = os.path.dirname(os.path.dirname(__file__))
+        path = os.path.join(root_name, 'libmoon', 'problem', 'mtl', 'mtl_data', 'compas', "compas.csv")
 
         x, y, s = load_dataset(path, sensible_attribute)
-
         x = torch.from_numpy(x).float()
         y = torch.from_numpy(y).long()
         s = torch.from_numpy(s).long()
 
         # train/val/test split: 70/10/20 %
         x_train, x_test, y_train, y_test, s_train, s_test = train_test_split(x, y, s, test_size=.2, random_state=1)
         x_train, x_val, y_train, y_val, s_train, s_val = train_test_split(x_train, y_train, s_train, test_size=.125, random_state=1)
@@ -94,8 +94,16 @@
     def __len__(self):
         return len(self.y)
     
     def __getitem__(self, index):
         return dict(data=self.x[index], labels=self.y[index], sensible_attribute=self.s[index])
     
     def task_names(self):
-        return None
+        return None
+
+
+if __name__ == "__main__":
+    from torch.utils import data
+    dataset = Compas(split="train")
+    trainloader = data.DataLoader(dataset, batch_size=256, num_workers=0)
+    for i, data in enumerate(trainloader):
+        print()
```

### Comparing `libmoon-0.1.9/libmoon/problem/mtl/loaders/credit_loader.py` & `libmoon-0.2.1/libmoon/problem/mtl/loaders/credit_loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,28 +25,27 @@
     data1 = data.copy()
     data1 = data1.drop(['default.payment.next.month', s_label], axis=1)
     data1 = pd.get_dummies(data1)
 
     x = StandardScaler().fit(data1).transform(data1)
     y = data['default.payment.next.month'].values
     s = data[s_label].values
-
     return x, y, s
 
 
+
 class Credit(torch.utils.data.Dataset):
 
     def __init__(self, split, sensible_attribute='SEX'):
         assert split in ['train', 'val', 'test']
 
-        folder_name = os.path.dirname(os.path.dirname(__file__))
-        path = os.path.join(folder_name, 'mtldata', "credit.csv")
+        from libmoon.util_global.constant import root_name
+        path = os.path.join(root_name, 'libmoon', 'problem', 'mtl', 'mtl_data', 'credit', "credit.csv")
 
         x, y, s = load_dataset(path, sensible_attribute)
-
         x = torch.from_numpy(x).float()
         y = torch.from_numpy(y).long()
         s = torch.from_numpy(s).long()
 
         # train/val/test split: 70/10/20 %
         x_train, x_test, y_train, y_test, s_train, s_test = train_test_split(x, y, s, test_size=.2, random_state=1)
         x_train, x_val, y_train, y_val, s_train, s_val = train_test_split(x_train, y_train, s_train, test_size=.125, random_state=1)
```

### Comparing `libmoon-0.1.9/libmoon/problem/mtl/loaders/multimnist_loader.py` & `libmoon-0.2.1/libmoon/problem/mtl/loaders/multimnist_loader.py`

 * *Files identical despite different names*

### Comparing `libmoon-0.1.9/libmoon/problem/mtl/mnist.py` & `libmoon-0.2.1/libmoon/problem/mtl/mnist.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,189 +1,222 @@
+'''
+    This file define the MO-Mnist problem as first proposed in Pareto multitask learning in Section 6.1.
+'''
 import matplotlib.pyplot as plt
-from libmoon.util_global.constant import root_name
-from libmoon.problem.mtl.loaders.multimnist_loader import MultiMNISTData
 import torch
 
+
+from libmoon.util_global.constant import root_name
+from libmoon.problem.mtl.loaders.multimnist_loader import MultiMNISTData
 from libmoon.problem.mtl.objectives import CrossEntropyLoss
-from libmoon.problem.mtl.model.simple import MultiLeNet
-from libmoon.util_global.weight_factor.funs import uniform_pref
+from libmoon.problem.mtl.model.lenet import MultiLeNet
+from libmoon.util_global.weight_factor import uniform_pref
 from libmoon.util_global.constant import FONT_SIZE
 
+from libmoon.solver.gradient import get_core_solver
+from libmoon.solver.gradient import get_grads_from_model, numel_params
+
+
+from libmoon.util_global.constant import is_pref_based
+
+
 loss_1 = CrossEntropyLoss(label_name='labels_l', logits_name='logits_l')
 loss_2 = CrossEntropyLoss(label_name='labels_r', logits_name='logits_r')
 
+
+
+
 from tqdm import tqdm
 import numpy as np
 from numpy import array
 import os
-from solver.gradient import get_core_solver
-from solver.gradient.utils.util import get_grads_from_model, numel_params
-from libmoon.util_global.constant import is_pref_based
+
 import itertools
 
+
 class MultiMnistProblem:
 
     # How to train at the same time.
-    def __init__(self, args, prefs):
+    def __init__(self, args):
         self.dataset = MultiMNISTData('mnist', 'train')
         self.args = args
         self.loader = torch.utils.data.DataLoader(self.dataset, batch_size=self.args.batch_size, shuffle=True,
                                                   num_workers=0)
         self.dataset_test = MultiMNISTData('mnist', 'test')
         self.loader_test = torch.utils.data.DataLoader(self.dataset_test, batch_size=args.batch_size, shuffle=True,
                                                        num_workers=0)
 
         self.lr = args.lr
-        self.prefs = prefs
-        self.n_prob = len(prefs)
-
-        self.model_arr = [MultiLeNet([1, 36, 36]) for _ in range(self.n_prob)]
-
+        self.model_arr = [MultiLeNet([1, 36, 36]) for _ in range(self.args.n_prob)]
         num_params = numel_params(self.model_arr[0])
         print('num_params: ', num_params)
-
         for model in self.model_arr:
             model.to(args.device)
 
-        self.is_pref_flag = is_pref_based(args.mtd)
-
+        self.is_pref_flag = is_pref_based(args.solver)
         if self.is_pref_flag:
             self.core_solver_arr = [get_core_solver(args, pref) for pref in prefs]
             self.optimizer_arr = [torch.optim.Adam(self.model_arr[idx].parameters(), lr=self.lr) for idx in
                                   range(self.n_prob)]
         else:
             self.set_core_solver = get_core_solver(args)
-
             params = [model.parameters() for model in self.model_arr]
             self.set_optimizer = torch.optim.Adam(itertools.chain(*params), lr=0.01)
 
 
-    def optimize(self):
+    def optimize(self, prefs=[]):
+
+        self.prefs = prefs
+        self.n_prob = len(prefs)
+
         loss_all = []
         for _ in tqdm(range(self.args.num_epoch)):
             if self.is_pref_flag:
-                loss_hostory = [[] for i in range(self.n_prob)]
+                loss_hostory = [ [] for i in range(self.n_prob) ]
             else:
                 loss_hostory = []
 
             for data in self.loader:
                 data_ = {k: v.to(self.args.device) for k, v in data.items()}
-
                 # pref based mtd
                 if self.is_pref_flag:
                     for pref_idx, (pref, model, optimizer) in enumerate(
                             zip(self.prefs, self.model_arr, self.optimizer_arr)):
+
                         logits_dict = self.model_arr[pref_idx](data_)
                         logits_dict['labels_l'] = data_['labels_l']
                         logits_dict['labels_r'] = data_['labels_r']
+
                         l1 = loss_1(**logits_dict)
                         l2 = loss_2(**logits_dict)
 
                         l_contains_grad = [l1, l2]
-                        G = get_grads_from_model(l_contains_grad, model)
 
-                        l1_np = np.array(l1.cpu().detach().numpy(), copy=True)
-                        l2_np = np.array(l2.cpu().detach().numpy(), copy=True)
-                        losses = array([l1_np, l2_np])
-                        alpha = self.core_solver_arr[pref_idx].get_alpha(G = G, losses=losses)
+                        # here for different methods, the needed information is not enough.
+                        if args.solver == 'agg':
+                            pass
+                        else:
+                            G = get_grads_from_model(l_contains_grad, model)
+                            l1_np = np.array(l1.cpu().detach().numpy(), copy=True)
+                            l2_np = np.array(l2.cpu().detach().numpy(), copy=True)
+                            losses = array([l1_np, l2_np])
+
+                        if args.solver == 'agg':
+                            if args.agg_mtd == 'ls':
+                                alpha = self.core_solver_arr[pref_idx].get_alpha(G = None, losses=None)
+                            else:
+                                assert False, 'mtd not implemented'
+
+                        else:
+                            alpha = self.core_solver_arr[pref_idx].get_alpha(G = G, losses=losses)
+
                         self.optimizer_arr[pref_idx].zero_grad()
                         (alpha[0] * l1 + alpha[1] * l2).backward()
                         self.optimizer_arr[pref_idx].step()
                         l1_np = np.array(l1.cpu().detach().numpy(), copy=True)
                         l2_np = np.array(l2.cpu().detach().numpy(), copy=True)
                         loss_hostory[pref_idx].append([l1_np, l2_np])
+
                 else:
                     # set based method is more complicated.
                     losses = [0,] * self.n_prob
                     losses_ts = [0] * self.n_prob
 
                     for model_idx, model in enumerate(self.model_arr):
                         logits_dict = self.model_arr[model_idx](data_)
                         logits_dict['labels_l'] = data_['labels_l']
                         logits_dict['labels_r'] = data_['labels_r']
                         l1 = loss_1(**logits_dict)
                         l2 = loss_2(**logits_dict)
 
                         losses_ts[model_idx] = torch.stack([l1, l2])
-
                         l1_np, l2_np = np.array(l1.cpu().detach().numpy(), copy=True), np.array(l2.cpu().detach().numpy(), copy=True)
                         losses[model_idx] = [l1_np, l2_np]
 
                     losses_ts = torch.stack(losses_ts)
                     losses = np.array(losses)
                     alpha = self.set_core_solver.get_alpha(losses).to(self.args.device)
                     self.set_optimizer.zero_grad()
                     torch.sum(alpha * losses_ts).backward()
                     self.set_optimizer.step()
                     loss_hostory.append(losses)
+
             loss_hostory = np.array(loss_hostory)
             if args.is_pref_based:
                 loss_history_mean = np.mean(loss_hostory, axis=1)
             else:
                 loss_history_mean = np.mean(loss_hostory, axis=0)
             loss_all.append(loss_history_mean)
+
         return loss_all
 
 
 
+
+
 if __name__ == '__main__':
+
     import argparse
     parser = argparse.ArgumentParser()
-
     parser.add_argument('--problem', default='mnist', type=str)  # For attribute in args, we all call problem.
     parser.add_argument('--split', default='train', type=str)
     parser.add_argument('--batch_size', default=512, type=int)
     parser.add_argument('--shuffle', default=True, type=bool)
     parser.add_argument('--lr', default=1e-2, type=float)
-    parser.add_argument('--num_epoch', default=10, type=int)
+    parser.add_argument('--num_epoch', default=1, type=int)
     parser.add_argument('--use-cuda', default=True, type=bool)
-
-    parser.add_argument('--mtd', default='hvgrad', type=str)
-    parser.add_argument('--agg-mtd', default='ls', type=str)   # This att is only valid when args.mtd=agg.
-    parser.add_argument('--n-obj', default=2, type=int)   # This att is only valid when args.mtd=agg.
+    parser.add_argument('--agg-mtd', default='ls', type=str)   # This att is only valid when args.solver=agg.
+    parser.add_argument('--solver', default='agg', type=str)
+    parser.add_argument('--n-obj', default=2, type=int)   # This att is only valid when args.solver=agg.
+    parser.add_argument('--debug', default=True, type=bool)   # This att is only valid when args.solver=agg.
 
     args = parser.parse_args()
-    args.is_pref_based = is_pref_based(args.mtd)
+    args.is_pref_based = is_pref_based(args.solver)
     if torch.cuda.is_available() and args.use_cuda:
         args.device = torch.device("cuda")  # Use the GPU
         print('cuda is available')
     else:
         args.device = torch.device("cpu")  # Use the CPU
         print('cuda is not available')
 
+
     prefs = uniform_pref(n_partition=10, n_obj=2, clip_eps=0.1)
     args.n_prob = len(prefs)
-
     problem = MultiMnistProblem(args, prefs)
-    # args.n_obj = problem.n_obj
 
     loss_history = problem.optimize()
     loss_history = np.array(loss_history)
-
     final_solution = loss_history[-1,:,:]
-    # plt.scatter(final_solution[:,0], final_solution[:,1], label='final solution')
-    for idx in range(loss_history.shape[1]):
-        plt.plot(loss_history[:,idx,0], loss_history[:,idx,1], 'o-', label='pref {}'.format(idx))
 
-    plt.plot(final_solution[:,0], final_solution[:,1], color='k', linewidth=3)
+    for idx in range(loss_history.shape[0]):
+        if idx==0:
+            plt.plot(loss_history[:,idx,0], loss_history[:,idx,1], 'o-', label='pref {}'.format(idx))
+        else:
+            plt.plot(loss_history[:,idx,0], loss_history[:,idx,1], 'o-')
+
 
+
+    plt.plot(final_solution[:,0], final_solution[:,1], color='k', linewidth=3)
     plt.legend(fontsize=FONT_SIZE)
     # draw pref
     solution_norm = np.linalg.norm(final_solution, axis=1, keepdims=True)
-    prefs_norm = prefs / np.linalg.norm(prefs, axis=1, keepdims=True) * solution_norm
+    prefs_norm = prefs / np.linalg.norm(prefs, axis=1, keepdims=True) * np.max(solution_norm)
 
     if args.is_pref_based:
         for pref in prefs_norm:
             plt.plot([0, pref[0]], [0, pref[1]], color='k')
 
 
     plt.xlabel('$L_1$', fontsize=FONT_SIZE)
     plt.ylabel('$L_2$', fontsize=FONT_SIZE)
 
-
-    folder_name = os.path.join( root_name, 'output', args.problem, args.mtd)
+    folder_name = os.path.join( root_name, 'output', args.problem, args.solver)
     os.makedirs(folder_name, exist_ok=True)
     fig_name = os.path.join(folder_name, 'final_solution.svg')
     plt.savefig(fig_name)
+
+
+    plt.title('{}_{}'.format(args.problem, args.solver), fontsize= FONT_SIZE )
+
     print('saved in ', fig_name)
 
     plt.show()
```

### Comparing `libmoon-0.1.9/libmoon/problem/mtl/model/simple.py` & `libmoon-0.2.1/libmoon/problem/mtl/models/lenet.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import torch.nn as nn
 
 '''
     MTL problems need . 
 '''
-
-
-
 class MultiLeNet(nn.Module):
 
     def __init__(self, dim, **kwargs):
-
         '''
             :param dim: a 3d-array. [chanel, height, width]
             :param kwargs:
         '''
         super().__init__()
         self.shared = nn.Sequential(
             nn.Conv2d(dim[0], 10, kernel_size=5),
@@ -36,42 +32,18 @@
         return dict(logits_l=self.private_left(x), logits_r=self.private_right(x))
 
     def private_params(self):
         return ['private_left.weight', 'private_left.bias', 'private_right.weight', 'private_right.bias']
 
 
 
-
-
-class FullyConnected(nn.Module):
-    def __init__(self, dim, **kwargs):
-        super().__init__()
-        self.f = nn.Sequential(
-            nn.Linear(dim[0], 60),
-            nn.ReLU(),
-            nn.Linear(60, 25),
-            nn.ReLU(),
-            nn.Linear(25, 1),
-        )
-
-    def forward(self, batch):
-        x = batch['data']
-        return dict(logits=self.f(x))
-
-
-
-
-
 if __name__ == '__main__':
     from libmoon.util_global.constant import root_name
     import os
     import pickle
 
-
-
-
     pickle_name = os.path.join(root_name, 'problem', 'mtl', 'data', 'multimnist', 'mnist.pickle')
     with open(pickle_name, 'rb') as f:
         data = pickle.load(f)
 
     model = MultiLeNet([3, 32, 32])
     print('hello world')
```

### Comparing `libmoon-0.1.9/libmoon/problem/synthetic/dtlz.py` & `libmoon-0.2.1/libmoon/problem/synthetic/dtlz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import numpy as np
 import torch
-from ..mop import mop
+from libmoon.problem.synthetic.mop import mop
 
 
 
 
 class DTLZ1(mop):
 
     def __init__(self, n_var=30, n_obj=3, lbound=np.zeros(30),
```

### Comparing `libmoon-0.1.9/libmoon/problem/synthetic/maf.py` & `libmoon-0.2.1/libmoon/problem/synthetic/maf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 
 from numpy import array
 import torch
 
 
 
 class MAF1:
-    def __init__(self):
+    def __init__(self, n_var):
         '''
             n_obj can be set as any number. For simlicity, we set it as 3.
         '''
         self.n_obj = 3
-        self.n_var = 30
+        self.n_var = n_var
         self.lb = 0
         self.ub = 1
 
     def evaluate(self, x):
         if type(x) == torch.Tensor:
 
             g = torch.sum( torch.pow(x[:, 2:] - 0.5, 2), dim=1 )
```

### Comparing `libmoon-0.1.9/libmoon/problem/synthetic/re.py` & `libmoon-0.2.1/libmoon/problem/synthetic/re.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,619 +1,619 @@
-
-import numpy as np
-import torch
-from ..mop import mop
-
-from numpy import array
-
-
-class RE21(mop):
-    def __init__(self, n_var=4, n_obj=2, lbound=np.zeros(4), ubound=np.ones(4)):
-        self.problem_name = 'RE21'
-        self.n_var = n_var
-        self.n_obj = n_obj
-        self.n_cons = 0
-
-        self.n_original_constraints = 0
-
-        self.ideal = array([1237.8414230005742, 0.002761423749158419])
-        # self.nadir = array([2086.36956042, 0.00341421356237])
-        self.nadir = np.array([2886.3695604236013, 0.039999999999998245])
-
-        F = 10.0
-        sigma = 10.0
-        tmp_val = F / sigma
-        self.ubound = np.full(self.n_var, 3 * tmp_val)
-        self.lbound = np.zeros(self.n_var)
-        self.lbound[0] = tmp_val
-        self.lbound[1] = np.sqrt(2.0) * tmp_val
-        self.lbound[2] = np.sqrt(2.0) * tmp_val
-        self.lbound[3] = tmp_val
-
-
-    def _evaluate_numpy(self, x):
-        n_sub = len(x)
-
-        x1 = x[:,0]
-        x2 = x[:,1]
-        x3 = x[:,2]
-        x4 = x[:,3]
-        f = np.zeros((n_sub, self.n_obj) )
-
-        F = 10.0
-        sigma = 10.0
-        E = 2.0 * 1e5
-        L = 200.0
-
-        f[:,0] = L * ((2 * x1) + np.sqrt(2.0) * x2 + np.sqrt(x3) + x4)
-        f[:,1] = ((F * L) / E) * ((2.0 / x1) + (2.0 * np.sqrt(2.0) / x2) - (2.0 * np.sqrt(2.0) / x3) + (2.0 / x4))
-
-        # f_arr = np.stack((f1,f2), axis=1)
-
-        f_arr_norm = (f - self.ideal) / (self.nadir - self.ideal)
-        # f_arr_norm =
-        f_arr_norm[:, 0] = 0.5 * f_arr_norm[:, 0]
-
-        return f_arr_norm
-
-
-    def _evaluate_torch(self, x):
-        x1 = x[:, 0]
-        x2 = x[:, 1]
-        x3 = x[:, 2]
-        x4 = x[:, 3]
-
-        F = 10.0
-        sigma = 10.0
-        E = 2.0 * 1e5
-        L = 200.0
-
-        f1 = L * ( (2 * x1) + np.sqrt(2.0) * x2 + torch.sqrt(x3) + x4 )
-        f2 = ((F * L) / E) * ((2.0 / x1) + (2.0 * np.sqrt(2.0) / x2) - (2.0 * np.sqrt(2.0) / x3) + (2.0 / x4))
-        f_arr = torch.stack((f1, f2), dim=1)
-        f_arr_norm = (f_arr - self.ideal) / (self.nadir - self.ideal)
-        f_arr_norm[:, 0] = 0.5 * f_arr_norm[:, 0]
-        return f_arr_norm
-
-
-class RE22(mop):
-    def __init__(self, n_var=3, n_obj=2, lbound=np.zeros(30),
-                 ubound=np.ones(30)):
-
-
-        self.n_var=n_var
-        self.n_obj=n_obj
-        self.problem_name = 'RE22'
-        self.n_cons = 0
-        self.n_original_constraints = 2
-
-        self.ideal = np.array([5.88, 0.0])
-        self.nadir = np.array([361.262944647, 180.01547])
-
-
-        self.ubound = np.zeros(self.n_var)
-        self.lbound = np.zeros(self.n_var)
-
-        self.lbound[0] = 0.2
-        self.lbound[1] = 0.0
-        self.lbound[2] = 0.0
-        self.ubound[0] = 15
-        self.ubound[1] = 20
-        self.ubound[2] = 40
-
-        self.n_var = n_var
-        self.n_obj = n_obj
-
-        self.feasible_vals = np.array(
-            [0.20, 0.31, 0.40, 0.44, 0.60, 0.62, 0.79, 0.80, 0.88, 0.93, 1.0, 1.20, 1.24, 1.32, 1.40, 1.55, 1.58, 1.60,
-             1.76, 1.80, 1.86, 2.0, 2.17, 2.20, 2.37, 2.40, 2.48, 2.60, 2.64, 2.79, 2.80, 3.0, 3.08, 3, 10, 3.16, 3.41,
-             3.52, 3.60, 3.72, 3.95, 3.96, 4.0, 4.03, 4.20, 4.34, 4.40, 4.65, 4.74, 4.80, 4.84, 5.0, 5.28, 5.40, 5.53,
-             5.72, 6.0, 6.16, 6.32, 6.60, 7.11, 7.20, 7.80, 7.90, 8.0, 8.40, 8.69, 9.0, 9.48, 10.27, 11.0, 11.06, 11.85,
-             12.0, 13.0, 14.0, 15.0])
-
-
-    def _evaluate_numpy(self, x):
-        n_sub = len(x)
-
-        f = np.zeros( (n_sub, self.n_obj) )
-        g = np.zeros( (n_sub, self.n_original_constraints)  )
-        # Reference: getNearestValue_sample2.py (https://gist.github.com/icchi-h/1d0bb1c52ebfdd31f14b3e811328390a)
-        idx_arr = [np.abs(np.asarray(self.feasible_vals) - x0).argmin() for x0 in x[:,0]]
-        x1 = array([self.feasible_vals[idx] for idx in idx_arr])
-        x2 = x[:,1]
-        x3 = x[:,2]
-
-        # First original objective function
-        f[:,0] = (29.4 * x1) + (0.6 * x2 * x3)
-        # Original constraint functions
-        g[:,0] = (x1 * x3) - 7.735 * ((x1 * x1) / x2) - 180.0
-        g[:,1] = 4.0 - (x3 / x2)
-        g = np.where(g < 0, -g, 0)
-        f[:,1] = g[:,0] + g[:,1]
-        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
-        f_norm[:, 0] = 0.5 * f_norm[:, 0]
-
-        return f_norm
-
-    def _evaluate_torch(self, x):
-        pass
-
-
-class RE23(mop):
-    def __init__(self, n_var=4, n_obj=2, lbound=np.zeros(2),
-                 ubound=np.ones(2)):
-        self.problem_name = 'RE23'
-        self.n_obj = n_obj
-        self.n_var = n_var
-        self.n_cons = 0
-        self.n_original_constraints = 3
-
-        self.ideal = array([15.9018007813, 0.0])
-        self.nadir = array([481.608088535, 44.2819047619])
-
-        self.ubound = np.zeros(self.n_var)
-        self.lbound = np.zeros(self.n_var)
-        self.lbound[0] = 1
-        self.lbound[1] = 1
-        self.lbound[2] = 10
-        self.lbound[3] = 10
-        self.ubound[0] = 100
-        self.ubound[1] = 100
-        self.ubound[2] = 200
-        self.ubound[3] = 240
-
-    def _evaluate_numpy(self, x):
-
-        f = np.zeros( (len(x), self.n_obj) )
-        g = np.zeros( (len(x), self.n_original_constraints))
-
-        x1 = 0.0625 * np.round(x[:,0]).astype(np.int32)
-        x2 = 0.0625 * np.round(x[:,1]).astype(np.int32)
-
-        x3 = x[:,2]
-        x4 = x[:,3]
-
-        # First original objective function
-        f[:,0] = (0.6224 * x1 * x3 * x4) + (1.7781 * x2 * x3 * x3) + (3.1661 * x1 * x1 * x4) + (19.84 * x1 * x1 * x3)
-
-        # Original constraint functions
-        g[:,0] = x1 - (0.0193 * x3)
-        g[:,1] = x2 - (0.00954 * x3)
-        g[:,2] = (np.pi * x3 * x3 * x4) + ((4.0 / 3.0) * (np.pi * x3 * x3 * x3)) - 1296000
-        g = np.where(g < 0, -g, 0)
-        f[:,1] = g[:,0] + g[:,1] + g[:,2]
-
-        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
-
-        return f_norm
-
-
-
-
-
-class RE24(mop):
-    def __init__(self, n_var=2, n_obj=2, lbound=np.zeros(2),
-                 ubound=np.ones(2)):
-        super().__init__(n_var=n_var,
-                         n_obj=n_obj,
-                         lbound=lbound,
-                         ubound=ubound, )
-
-        self.problem_name = 'RE24'
-        self.n_obj = 2
-        self.n_var = 2
-
-        self.n_cons = 0
-        self.n_original_constraints = 4
-
-        self.ubound = np.zeros(self.n_var)
-        self.lbound = np.zeros(self.n_var)
-
-        self.lbound[0] = 0.5
-        self.lbound[1] = 0.5
-
-        self.ubound[0] = 4
-        self.ubound[1] = 50
-
-        self.ideal = np.array([60.5, 0.0])
-        self.nadir = np.array([481.608088535, 44.2819047619])
-
-
-
-
-    def _evaluate_numpy(self, x):
-        n_sub = len(x)
-        # f = np.zeros(self.n_objectives)
-        g = np.zeros( (n_sub, self.n_original_constraints) )
-
-        x1 = x[:,0]
-        x2 = x[:,1]
-
-        # First original objective function
-        f1 = x1 + (120 * x2)
-
-        E = 700000
-        sigma_b_max = 700
-        tau_max = 450
-        delta_max = 1.5
-        sigma_k = (E * x1 * x1) / 100
-        sigma_b = 4500 / (x1 * x2)
-        tau = 1800 / x2
-        delta = (56.2 * 10000) / (E * x1 * x2 * x2)
-
-        g[:,0] = 1 - (sigma_b / sigma_b_max)
-        g[:,1] = 1 - (tau / tau_max)
-        g[:,2] = 1 - (delta / delta_max)
-        g[:,3] = 1 - (sigma_b / sigma_k)
-        g = np.where(g < 0, -g, 0)
-        f2 = g[:,0] + g[:,1] + g[:,2] + g[:,3]
-
-        f_arr = np.stack((f1, f2), axis=1)
-        f_norm = (f_arr - self.ideal) / (self.nadir - self.ideal)
-
-        return f_norm
-
-
-    def _evaluate_torch(self, x):
-        pass
-
-
-class RE25(mop):
-    def __init__(self, n_var=3, n_obj=2):
-        self.problem_name = 'RE25'
-        self.n_obj = n_obj
-        self.n_var = n_var
-
-        self.n_cons = 0
-        self.n_original_constraints = 6
-
-        self.ideal = array([0.037591349242869145, 0.0])
-        self.nadir = array([0.40397042546, 2224669.22419])
-
-        self.ubound = np.zeros( self.n_var )
-        self.lbound = np.zeros( self.n_var )
-        self.lbound[0] = 1
-        self.lbound[1] = 0.6
-        self.lbound[2] = 0.09
-        self.ubound[0] = 70
-        self.ubound[1] = 3
-        self.ubound[2] = 0.5
-
-        self.feasible_vals = np.array(
-            [0.009, 0.0095, 0.0104, 0.0118, 0.0128, 0.0132, 0.014, 0.015, 0.0162, 0.0173, 0.018, 0.02, 0.023, 0.025,
-             0.028, 0.032, 0.035, 0.041, 0.047, 0.054, 0.063, 0.072, 0.08, 0.092, 0.105, 0.12, 0.135, 0.148, 0.162,
-             0.177, 0.192, 0.207, 0.225, 0.244, 0.263, 0.283, 0.307, 0.331, 0.362, 0.394, 0.4375, 0.5])
-
-    def _evaluate_numpy(self, x):
-        n_sub = len(x)
-        f = np.zeros( (n_sub, self.n_obj) )
-        g = np.zeros( (n_sub, self.n_original_constraints) )
-        x1 = np.round(x[:,0])
-        x2 = x[:,1]
-
-        # Reference: getNearestValue_sample2.py (https://gist.github.com/icchi-h/1d0bb1c52ebfdd31f14b3e811328390a)
-        idx_array = array([np.abs(np.asarray(self.feasible_vals) - x2).argmin() for x2 in x[:,2]])
-
-        x3 = array( [self.feasible_vals[idx] for idx in idx_array] )
-
-        # first original objective function
-        f[:,0] = (np.pi * np.pi * x2 * x3 * x3 * (x1 + 2)) / 4.0
-
-        # constraint functions
-        Cf = ((4.0 * (x2 / x3) - 1) / (4.0 * (x2 / x3) - 4)) + (0.615 * x3 / x2)
-        Fmax = 1000.0
-        S = 189000.0
-        G = 11.5 * 1e+6
-        K = (G * x3 * x3 * x3 * x3) / (8 * x1 * x2 * x2 * x2)
-        lmax = 14.0
-        lf = (Fmax / K) + 1.05 * (x1 + 2) * x3
-        dmin = 0.2
-        Dmax = 3
-        Fp = 300.0
-        sigmaP = Fp / K
-        sigmaPM = 6
-        sigmaW = 1.25
-
-        g[:,0] = -((8 * Cf * Fmax * x2) / (np.pi * x3 * x3 * x3)) + S
-        g[:,1] = -lf + lmax
-        g[:,2] = -3 + (x2 / x3)
-        g[:,3] = -sigmaP + sigmaPM
-        g[:,4] = -sigmaP - ((Fmax - Fp) / K) - 1.05 * (x1 + 2) * x3 + lf
-        g[:,5] = sigmaW - ((Fmax - Fp) / K)
-
-        g = np.where(g < 0, -g, 0)
-        f[:,1] = g[:,0] + g[:,1] + g[:,2] + g[:,3] + g[:,4] + g[:,5]
-
-        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
-        return f_norm
-
-    def _evaluate_torch(self, x):
-        pass
-
-
-class RE31(mop):
-    def __init__(self, n_obj=3, n_var=3):
-        self.problem_name = 'RE31'
-        self.n_obj = n_obj
-        self.n_var = n_var
-        self.n_cons = 0
-        self.n_original_constraints = 3
-
-        self.ubound = np.zeros(self.n_var)
-        self.lbound = np.zeros(self.n_var)
-        self.lbound[0] = 0.00001
-        self.lbound[1] = 0.00001
-        self.lbound[2] = 1.0
-        self.ubound[0] = 100.0
-        self.ubound[1] = 100.0
-        self.ubound[2] = 3.0
-
-        self.ideal = np.array([5.53731918799e-05, 0.333333333333, 0.0])
-        self.nadir = np.array([500.002668442, 8246211.25124, 19359919.7502])
-
-
-    def _evaluate_numpy(self, x):
-        n_sub = len(x)
-        f = np.zeros( (n_sub, self.n_obj) )
-        g = np.zeros( (n_sub, self.n_original_constraints) )
-
-        x1 = x[:,0]
-        x2 = x[:,1]
-        x3 = x[:,2]
-
-        # First original objective function
-        f[:,0] = x1 * np.sqrt(16.0 + (x3 * x3)) + x2 * np.sqrt(1.0 + x3 * x3)
-        # Second original objective function
-        f[:,1] = (20.0 * np.sqrt(16.0 + (x3 * x3))) / (x1 * x3)
-
-        # Constraint functions
-        g[:,0] = 0.1 - f[:,0]
-        g[:,1] = 100000.0 - f[:,1]
-        g[:,2] = 100000 - ((80.0 * np.sqrt(1.0 + x3 * x3)) / (x3 * x2))
-        g = np.where(g < 0, -g, 0)
-        f[:,2] = g[:,0] + g[:,1] + g[:,2]
-
-        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
-        return f_norm
-
-    def _evaluate_torch(self, x):
-        pass
-
-
-class RE37(mop):
-    def __init__(self, n_obj=3, n_var=4):
-        self.problem_name = 'RE37'
-        self.n_obj = n_obj
-        self.n_var = n_var
-        self.n_cons = 0
-        self.n_original_constraints = 0
-
-        self.lbound = np.full(self.n_var, 0)
-        self.ubound = np.full(self.n_var, 1)
-
-        self.ideal = np.array([0.00889341391106, 0.00488, -0.431499999825])
-        self.nadir = np.array([0.98949120096, 0.956587924661, 0.987530948586])
-
-
-    def _evaluate_numpy(self, x):
-        n_sub = len(x)
-        f = np.zeros( (n_sub, self.n_obj) )
-
-        xAlpha = x[:,0]
-        xHA = x[:,1]
-        xOA = x[:,2]
-        xOPTT = x[:,3]
-
-        # f1 (TF_max)
-        f[:,0] = 0.692 + (0.477 * xAlpha) - (0.687 * xHA) - (0.080 * xOA) - (0.0650 * xOPTT) - (
-                    0.167 * xAlpha * xAlpha) - (0.0129 * xHA * xAlpha) + (0.0796 * xHA * xHA) - (
-                           0.0634 * xOA * xAlpha) - (0.0257 * xOA * xHA) + (0.0877 * xOA * xOA) - (
-                           0.0521 * xOPTT * xAlpha) + (0.00156 * xOPTT * xHA) + (0.00198 * xOPTT * xOA) + (
-                           0.0184 * xOPTT * xOPTT)
-        # f2 (X_cc)
-        f[:,1] = 0.153 - (0.322 * xAlpha) + (0.396 * xHA) + (0.424 * xOA) + (0.0226 * xOPTT) + (
-                    0.175 * xAlpha * xAlpha) + (0.0185 * xHA * xAlpha) - (0.0701 * xHA * xHA) - (
-                           0.251 * xOA * xAlpha) + (0.179 * xOA * xHA) + (0.0150 * xOA * xOA) + (
-                           0.0134 * xOPTT * xAlpha) + (0.0296 * xOPTT * xHA) + (0.0752 * xOPTT * xOA) + (
-                           0.0192 * xOPTT * xOPTT)
-        # f3 (TT_max)
-        f[:,2] = 0.370 - (0.205 * xAlpha) + (0.0307 * xHA) + (0.108 * xOA) + (1.019 * xOPTT) - (
-                    0.135 * xAlpha * xAlpha) + (0.0141 * xHA * xAlpha) + (0.0998 * xHA * xHA) + (
-                           0.208 * xOA * xAlpha) - (0.0301 * xOA * xHA) - (0.226 * xOA * xOA) + (
-                           0.353 * xOPTT * xAlpha) - (0.0497 * xOPTT * xOA) - (0.423 * xOPTT * xOPTT) + (
-                           0.202 * xHA * xAlpha * xAlpha) - (0.281 * xOA * xAlpha * xAlpha) - (
-                           0.342 * xHA * xHA * xAlpha) - (0.245 * xHA * xHA * xOA) + (0.281 * xOA * xOA * xHA) - (
-                           0.184 * xOPTT * xOPTT * xAlpha) - (0.281 * xHA * xAlpha * xOA)
-
-        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
-        return f_norm
-
-
-
-class RE41(mop):
-    def __init__(self, n_obj=4, n_var=7):
-        self.problem_name = 'RE41'
-        self.n_obj = n_obj
-        self.n_var = n_var
-        self.n_cons = 0
-        self.n_original_constraints = 10
-
-        self.lbound = np.zeros(self.n_var)
-        self.ubound = np.zeros(self.n_var)
-        self.lbound[0] = 0.5
-        self.lbound[1] = 0.45
-        self.lbound[2] = 0.5
-        self.lbound[3] = 0.5
-        self.lbound[4] = 0.875
-        self.lbound[5] = 0.4
-        self.lbound[6] = 0.4
-        self.ubound[0] = 1.5
-        self.ubound[1] = 1.35
-        self.ubound[2] = 1.5
-        self.ubound[3] = 1.5
-        self.ubound[4] = 2.625
-        self.ubound[5] = 1.2
-        self.ubound[6] = 1.2
-
-        self.ideal = np.array([15.576004, 3.58525, 10.61064375, 0.0])
-        self.nadir = np.array([39.2905121788, 4.42725, 13.09138125, 9.49401929991])
-
-
-    def _evaluate_numpy(self, x):
-        n_sub = len(x)
-
-        f = np.zeros( (n_sub, self.n_obj) )
-        g = np.zeros( (n_sub, self.n_original_constraints) )
-
-        x1 = x[:,0]
-        x2 = x[:,1]
-        x3 = x[:,2]
-        x4 = x[:,3]
-        x5 = x[:,4]
-        x6 = x[:,5]
-        x7 = x[:,6]
-
-        # First original objective function
-        f[:,0] = 1.98 + 4.9 * x1 + 6.67 * x2 + 6.98 * x3 + 4.01 * x4 + 1.78 * x5 + 0.00001 * x6 + 2.73 * x7
-        # Second original objective function
-        f[:,1] = 4.72 - 0.5 * x4 - 0.19 * x2 * x3
-        # Third original objective function
-        Vmbp = 10.58 - 0.674 * x1 * x2 - 0.67275 * x2
-        Vfd = 16.45 - 0.489 * x3 * x7 - 0.843 * x5 * x6
-        f[:,2] = 0.5 * (Vmbp + Vfd)
-
-        # Constraint functions
-        g[:,0] = 1 - (1.16 - 0.3717 * x2 * x4 - 0.0092928 * x3)
-        g[:,1] = 0.32 - (0.261 - 0.0159 * x1 * x2 - 0.06486 * x1 - 0.019 * x2 * x7 + 0.0144 * x3 * x5 + 0.0154464 * x6)
-        g[:,2] = 0.32 - (
-                    0.214 + 0.00817 * x5 - 0.045195 * x1 - 0.0135168 * x1 + 0.03099 * x2 * x6 - 0.018 * x2 * x7 + 0.007176 * x3 + 0.023232 * x3 - 0.00364 * x5 * x6 - 0.018 * x2 * x2)
-        g[:,3] = 0.32 - (0.74 - 0.61 * x2 - 0.031296 * x3 - 0.031872 * x7 + 0.227 * x2 * x2)
-        g[:,4] = 32 - (28.98 + 3.818 * x3 - 4.2 * x1 * x2 + 1.27296 * x6 - 2.68065 * x7)
-        g[:,5] = 32 - (33.86 + 2.95 * x3 - 5.057 * x1 * x2 - 3.795 * x2 - 3.4431 * x7 + 1.45728)
-        g[:,6] = 32 - (46.36 - 9.9 * x2 - 4.4505 * x1)
-        g[:,7] = 4 - f[:,1]
-        g[:,8] = 9.9 - Vmbp
-        g[:,9] = 15.7 - Vfd
-        g = np.where(g < 0, -g, 0)
-        f[:,3] = g[:,0] + g[:,1] + g[:,2] + g[:,3] + g[:,4] + g[:,5] + g[:,6] + g[:,7] + g[:,8] + g[:,9]
-        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
-        return f_norm
-
-    def _evaluate_torch(self, x):
-        pass
-
-
-class RE42(mop):
-    def __init__(self):
-        self.problem_name = 'RE42'
-
-        self.n_obj = 4
-        self.n_var = 6
-        self.n_cons = 0
-        self.n_original_constraints = 9
-
-        self.lbound = np.zeros(self.n_var )
-        self.ubound = np.zeros(self.n_var )
-        self.lbound[0] = 150.0
-        self.lbound[1] = 20.0
-        self.lbound[2] = 13.0
-        self.lbound[3] = 10.0
-        self.lbound[4] = 14.0
-        self.lbound[5] = 0.63
-        self.ubound[0] = 274.32
-        self.ubound[1] = 32.31
-        self.ubound[2] = 25.0
-        self.ubound[3] = 11.71
-        self.ubound[4] = 18.0
-        self.ubound[5] = 0.75
-
-        self.ideal = np.array([-2756.2590400638524, 3962.557843228888, 1947.880856925791, 0.0])
-        self.nadir = np.array([-1010.5229595219643, 13827.138456300128, 2611.9668107424536, 12.437669929732023 ])
-
-
-
-    def _evaluate_numpy(self, x):
-        n_sub = len(x)
-
-        f = np.zeros( (n_sub, self.n_obj) )
-        # NOT g
-        constraintFuncs = np.zeros( (n_sub, self.n_original_constraints) )
-
-        x_L = x[:,0]
-        x_B = x[:,1]
-        x_D = x[:,2]
-        x_T = x[:,3]
-        x_Vk = x[:,4]
-        x_CB = x[:,5]
-
-        displacement = 1.025 * x_L * x_B * x_T * x_CB
-        V = 0.5144 * x_Vk
-        g = 9.8065
-        Fn = V / np.power(g * x_L, 0.5)
-        a = (4977.06 * x_CB * x_CB) - (8105.61 * x_CB) + 4456.51
-        b = (-10847.2 * x_CB * x_CB) + (12817.0 * x_CB) - 6960.32
-
-        power = (np.power(displacement, 2.0 / 3.0) * np.power(x_Vk, 3.0)) / (a + (b * Fn))
-        outfit_weight = 1.0 * np.power(x_L, 0.8) * np.power(x_B, 0.6) * np.power(x_D, 0.3) * np.power(x_CB, 0.1)
-        steel_weight = 0.034 * np.power(x_L, 1.7) * np.power(x_B, 0.7) * np.power(x_D, 0.4) * np.power(x_CB, 0.5)
-        machinery_weight = 0.17 * np.power(power, 0.9)
-        light_ship_weight = steel_weight + outfit_weight + machinery_weight
-
-        ship_cost = 1.3 * ((2000.0 * np.power(steel_weight, 0.85)) + (3500.0 * outfit_weight) + (
-                    2400.0 * np.power(power, 0.8)))
-        capital_costs = 0.2 * ship_cost
-
-        DWT = displacement - light_ship_weight
-
-        running_costs = 40000.0 * np.power(DWT, 0.3)
-
-        round_trip_miles = 5000.0
-        sea_days = (round_trip_miles / 24.0) * x_Vk
-        handling_rate = 8000.0
-
-        daily_consumption = ((0.19 * power * 24.0) / 1000.0) + 0.2
-        fuel_price = 100.0
-        fuel_cost = 1.05 * daily_consumption * sea_days * fuel_price
-        port_cost = 6.3 * np.power(DWT, 0.8)
-
-        fuel_carried = daily_consumption * (sea_days + 5.0)
-        miscellaneous_DWT = 2.0 * np.power(DWT, 0.5)
-
-        cargo_DWT = DWT - fuel_carried - miscellaneous_DWT
-        port_days = 2.0 * ((cargo_DWT / handling_rate) + 0.5)
-        RTPA = 350.0 / (sea_days + port_days)
-
-        voyage_costs = (fuel_cost + port_cost) * RTPA
-        annual_costs = capital_costs + running_costs + voyage_costs
-        annual_cargo = cargo_DWT * RTPA
-
-        f[:,0] = annual_costs / annual_cargo
-        f[:,1] = light_ship_weight
-        # f_2 is dealt as a minimization problem
-        f[:,2] = -annual_cargo
-
-        # Reformulated objective functions
-        constraintFuncs[:,0] = (x_L / x_B) - 6.0
-        constraintFuncs[:,1] = -(x_L / x_D) + 15.0
-        constraintFuncs[:,2] = -(x_L / x_T) + 19.0
-        constraintFuncs[:,3] = 0.45 * np.power(DWT, 0.31) - x_T
-        constraintFuncs[:,4] = 0.7 * x_D + 0.7 - x_T
-        constraintFuncs[:,5] = 500000.0 - DWT
-        constraintFuncs[:,6] = DWT - 3000.0
-        constraintFuncs[:,7] = 0.32 - Fn
-
-        KB = 0.53 * x_T
-        BMT = ((0.085 * x_CB - 0.002) * x_B * x_B) / (x_T * x_CB)
-        KG = 1.0 + 0.52 * x_D
-        constraintFuncs[:,8] = (KB + BMT - KG) - (0.07 * x_B)
-
-        constraintFuncs = np.where(constraintFuncs < 0, -constraintFuncs, 0)
-        f[:,3] = constraintFuncs[:,0] + constraintFuncs[:,1] + constraintFuncs[:,2] + constraintFuncs[:,3] + constraintFuncs[:,4] + \
-               constraintFuncs[:,5] + constraintFuncs[:,6] + constraintFuncs[:,7] + constraintFuncs[:,8]
-
-        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
-        return f
-
-
-
-
-
+
+import numpy as np
+import torch
+from libmoon.problem.synthetic.mop import mop
+
+from numpy import array
+
+
+class RE21(mop):
+    def __init__(self, n_var=4, n_obj=2, lbound=np.zeros(4), ubound=np.ones(4)):
+        self.problem_name = 'RE21'
+        self.n_var = n_var
+        self.n_obj = n_obj
+        self.n_cons = 0
+
+        self.n_original_constraints = 0
+
+        self.ideal = array([1237.8414230005742, 0.002761423749158419])
+        # self.nadir = array([2086.36956042, 0.00341421356237])
+        self.nadir = np.array([2886.3695604236013, 0.039999999999998245])
+
+        F = 10.0
+        sigma = 10.0
+        tmp_val = F / sigma
+        self.ubound = np.full(self.n_var, 3 * tmp_val)
+        self.lbound = np.zeros(self.n_var)
+        self.lbound[0] = tmp_val
+        self.lbound[1] = np.sqrt(2.0) * tmp_val
+        self.lbound[2] = np.sqrt(2.0) * tmp_val
+        self.lbound[3] = tmp_val
+
+
+    def _evaluate_numpy(self, x):
+        n_sub = len(x)
+
+        x1 = x[:,0]
+        x2 = x[:,1]
+        x3 = x[:,2]
+        x4 = x[:,3]
+        f = np.zeros((n_sub, self.n_obj) )
+
+        F = 10.0
+        sigma = 10.0
+        E = 2.0 * 1e5
+        L = 200.0
+
+        f[:,0] = L * ((2 * x1) + np.sqrt(2.0) * x2 + np.sqrt(x3) + x4)
+        f[:,1] = ((F * L) / E) * ((2.0 / x1) + (2.0 * np.sqrt(2.0) / x2) - (2.0 * np.sqrt(2.0) / x3) + (2.0 / x4))
+
+        # f_arr = np.stack((f1,f2), axis=1)
+
+        f_arr_norm = (f - self.ideal) / (self.nadir - self.ideal)
+        # f_arr_norm =
+        f_arr_norm[:, 0] = 0.5 * f_arr_norm[:, 0]
+
+        return f_arr_norm
+
+
+    def _evaluate_torch(self, x):
+        x1 = x[:, 0]
+        x2 = x[:, 1]
+        x3 = x[:, 2]
+        x4 = x[:, 3]
+
+        F = 10.0
+        sigma = 10.0
+        E = 2.0 * 1e5
+        L = 200.0
+
+        f1 = L * ( (2 * x1) + np.sqrt(2.0) * x2 + torch.sqrt(x3) + x4 )
+        f2 = ((F * L) / E) * ((2.0 / x1) + (2.0 * np.sqrt(2.0) / x2) - (2.0 * np.sqrt(2.0) / x3) + (2.0 / x4))
+        f_arr = torch.stack((f1, f2), dim=1)
+        f_arr_norm = (f_arr - self.ideal) / (self.nadir - self.ideal)
+        f_arr_norm[:, 0] = 0.5 * f_arr_norm[:, 0]
+        return f_arr_norm
+
+
+class RE22(mop):
+    def __init__(self, n_var=3, n_obj=2, lbound=np.zeros(30),
+                 ubound=np.ones(30)):
+
+
+        self.n_var=n_var
+        self.n_obj=n_obj
+        self.problem_name = 'RE22'
+        self.n_cons = 0
+        self.n_original_constraints = 2
+
+        self.ideal = np.array([5.88, 0.0])
+        self.nadir = np.array([361.262944647, 180.01547])
+
+
+        self.ubound = np.zeros(self.n_var)
+        self.lbound = np.zeros(self.n_var)
+
+        self.lbound[0] = 0.2
+        self.lbound[1] = 0.0
+        self.lbound[2] = 0.0
+        self.ubound[0] = 15
+        self.ubound[1] = 20
+        self.ubound[2] = 40
+
+        self.n_var = n_var
+        self.n_obj = n_obj
+
+        self.feasible_vals = np.array(
+            [0.20, 0.31, 0.40, 0.44, 0.60, 0.62, 0.79, 0.80, 0.88, 0.93, 1.0, 1.20, 1.24, 1.32, 1.40, 1.55, 1.58, 1.60,
+             1.76, 1.80, 1.86, 2.0, 2.17, 2.20, 2.37, 2.40, 2.48, 2.60, 2.64, 2.79, 2.80, 3.0, 3.08, 3, 10, 3.16, 3.41,
+             3.52, 3.60, 3.72, 3.95, 3.96, 4.0, 4.03, 4.20, 4.34, 4.40, 4.65, 4.74, 4.80, 4.84, 5.0, 5.28, 5.40, 5.53,
+             5.72, 6.0, 6.16, 6.32, 6.60, 7.11, 7.20, 7.80, 7.90, 8.0, 8.40, 8.69, 9.0, 9.48, 10.27, 11.0, 11.06, 11.85,
+             12.0, 13.0, 14.0, 15.0])
+
+
+    def _evaluate_numpy(self, x):
+        n_sub = len(x)
+
+        f = np.zeros( (n_sub, self.n_obj) )
+        g = np.zeros( (n_sub, self.n_original_constraints)  )
+        # Reference: getNearestValue_sample2.py (https://gist.github.com/icchi-h/1d0bb1c52ebfdd31f14b3e811328390a)
+        idx_arr = [np.abs(np.asarray(self.feasible_vals) - x0).argmin() for x0 in x[:,0]]
+        x1 = array([self.feasible_vals[idx] for idx in idx_arr])
+        x2 = x[:,1]
+        x3 = x[:,2]
+
+        # First original objective function
+        f[:,0] = (29.4 * x1) + (0.6 * x2 * x3)
+        # Original constraint functions
+        g[:,0] = (x1 * x3) - 7.735 * ((x1 * x1) / x2) - 180.0
+        g[:,1] = 4.0 - (x3 / x2)
+        g = np.where(g < 0, -g, 0)
+        f[:,1] = g[:,0] + g[:,1]
+        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
+        f_norm[:, 0] = 0.5 * f_norm[:, 0]
+
+        return f_norm
+
+    def _evaluate_torch(self, x):
+        pass
+
+
+class RE23(mop):
+    def __init__(self, n_var=4, n_obj=2, lbound=np.zeros(2),
+                 ubound=np.ones(2)):
+        self.problem_name = 'RE23'
+        self.n_obj = n_obj
+        self.n_var = n_var
+        self.n_cons = 0
+        self.n_original_constraints = 3
+
+        self.ideal = array([15.9018007813, 0.0])
+        self.nadir = array([481.608088535, 44.2819047619])
+
+        self.ubound = np.zeros(self.n_var)
+        self.lbound = np.zeros(self.n_var)
+        self.lbound[0] = 1
+        self.lbound[1] = 1
+        self.lbound[2] = 10
+        self.lbound[3] = 10
+        self.ubound[0] = 100
+        self.ubound[1] = 100
+        self.ubound[2] = 200
+        self.ubound[3] = 240
+
+    def _evaluate_numpy(self, x):
+
+        f = np.zeros( (len(x), self.n_obj) )
+        g = np.zeros( (len(x), self.n_original_constraints))
+
+        x1 = 0.0625 * np.round(x[:,0]).astype(np.int32)
+        x2 = 0.0625 * np.round(x[:,1]).astype(np.int32)
+
+        x3 = x[:,2]
+        x4 = x[:,3]
+
+        # First original objective function
+        f[:,0] = (0.6224 * x1 * x3 * x4) + (1.7781 * x2 * x3 * x3) + (3.1661 * x1 * x1 * x4) + (19.84 * x1 * x1 * x3)
+
+        # Original constraint functions
+        g[:,0] = x1 - (0.0193 * x3)
+        g[:,1] = x2 - (0.00954 * x3)
+        g[:,2] = (np.pi * x3 * x3 * x4) + ((4.0 / 3.0) * (np.pi * x3 * x3 * x3)) - 1296000
+        g = np.where(g < 0, -g, 0)
+        f[:,1] = g[:,0] + g[:,1] + g[:,2]
+
+        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
+
+        return f_norm
+
+
+
+
+
+class RE24(mop):
+    def __init__(self, n_var=2, n_obj=2, lbound=np.zeros(2),
+                 ubound=np.ones(2)):
+        super().__init__(n_var=n_var,
+                         n_obj=n_obj,
+                         lbound=lbound,
+                         ubound=ubound, )
+
+        self.problem_name = 'RE24'
+        self.n_obj = 2
+        self.n_var = 2
+
+        self.n_cons = 0
+        self.n_original_constraints = 4
+
+        self.ubound = np.zeros(self.n_var)
+        self.lbound = np.zeros(self.n_var)
+
+        self.lbound[0] = 0.5
+        self.lbound[1] = 0.5
+
+        self.ubound[0] = 4
+        self.ubound[1] = 50
+
+        self.ideal = np.array([60.5, 0.0])
+        self.nadir = np.array([481.608088535, 44.2819047619])
+
+
+
+
+    def _evaluate_numpy(self, x):
+        n_sub = len(x)
+        # f = np.zeros(self.n_objectives)
+        g = np.zeros( (n_sub, self.n_original_constraints) )
+
+        x1 = x[:,0]
+        x2 = x[:,1]
+
+        # First original objective function
+        f1 = x1 + (120 * x2)
+
+        E = 700000
+        sigma_b_max = 700
+        tau_max = 450
+        delta_max = 1.5
+        sigma_k = (E * x1 * x1) / 100
+        sigma_b = 4500 / (x1 * x2)
+        tau = 1800 / x2
+        delta = (56.2 * 10000) / (E * x1 * x2 * x2)
+
+        g[:,0] = 1 - (sigma_b / sigma_b_max)
+        g[:,1] = 1 - (tau / tau_max)
+        g[:,2] = 1 - (delta / delta_max)
+        g[:,3] = 1 - (sigma_b / sigma_k)
+        g = np.where(g < 0, -g, 0)
+        f2 = g[:,0] + g[:,1] + g[:,2] + g[:,3]
+
+        f_arr = np.stack((f1, f2), axis=1)
+        f_norm = (f_arr - self.ideal) / (self.nadir - self.ideal)
+
+        return f_norm
+
+
+    def _evaluate_torch(self, x):
+        pass
+
+
+class RE25(mop):
+    def __init__(self, n_var=3, n_obj=2):
+        self.problem_name = 'RE25'
+        self.n_obj = n_obj
+        self.n_var = n_var
+
+        self.n_cons = 0
+        self.n_original_constraints = 6
+
+        self.ideal = array([0.037591349242869145, 0.0])
+        self.nadir = array([0.40397042546, 2224669.22419])
+
+        self.ubound = np.zeros( self.n_var )
+        self.lbound = np.zeros( self.n_var )
+        self.lbound[0] = 1
+        self.lbound[1] = 0.6
+        self.lbound[2] = 0.09
+        self.ubound[0] = 70
+        self.ubound[1] = 3
+        self.ubound[2] = 0.5
+
+        self.feasible_vals = np.array(
+            [0.009, 0.0095, 0.0104, 0.0118, 0.0128, 0.0132, 0.014, 0.015, 0.0162, 0.0173, 0.018, 0.02, 0.023, 0.025,
+             0.028, 0.032, 0.035, 0.041, 0.047, 0.054, 0.063, 0.072, 0.08, 0.092, 0.105, 0.12, 0.135, 0.148, 0.162,
+             0.177, 0.192, 0.207, 0.225, 0.244, 0.263, 0.283, 0.307, 0.331, 0.362, 0.394, 0.4375, 0.5])
+
+    def _evaluate_numpy(self, x):
+        n_sub = len(x)
+        f = np.zeros( (n_sub, self.n_obj) )
+        g = np.zeros( (n_sub, self.n_original_constraints) )
+        x1 = np.round(x[:,0])
+        x2 = x[:,1]
+
+        # Reference: getNearestValue_sample2.py (https://gist.github.com/icchi-h/1d0bb1c52ebfdd31f14b3e811328390a)
+        idx_array = array([np.abs(np.asarray(self.feasible_vals) - x2).argmin() for x2 in x[:,2]])
+
+        x3 = array( [self.feasible_vals[idx] for idx in idx_array] )
+
+        # first original objective function
+        f[:,0] = (np.pi * np.pi * x2 * x3 * x3 * (x1 + 2)) / 4.0
+
+        # constraint functions
+        Cf = ((4.0 * (x2 / x3) - 1) / (4.0 * (x2 / x3) - 4)) + (0.615 * x3 / x2)
+        Fmax = 1000.0
+        S = 189000.0
+        G = 11.5 * 1e+6
+        K = (G * x3 * x3 * x3 * x3) / (8 * x1 * x2 * x2 * x2)
+        lmax = 14.0
+        lf = (Fmax / K) + 1.05 * (x1 + 2) * x3
+        dmin = 0.2
+        Dmax = 3
+        Fp = 300.0
+        sigmaP = Fp / K
+        sigmaPM = 6
+        sigmaW = 1.25
+
+        g[:,0] = -((8 * Cf * Fmax * x2) / (np.pi * x3 * x3 * x3)) + S
+        g[:,1] = -lf + lmax
+        g[:,2] = -3 + (x2 / x3)
+        g[:,3] = -sigmaP + sigmaPM
+        g[:,4] = -sigmaP - ((Fmax - Fp) / K) - 1.05 * (x1 + 2) * x3 + lf
+        g[:,5] = sigmaW - ((Fmax - Fp) / K)
+
+        g = np.where(g < 0, -g, 0)
+        f[:,1] = g[:,0] + g[:,1] + g[:,2] + g[:,3] + g[:,4] + g[:,5]
+
+        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
+        return f_norm
+
+    def _evaluate_torch(self, x):
+        pass
+
+
+class RE31(mop):
+    def __init__(self, n_obj=3, n_var=3):
+        self.problem_name = 'RE31'
+        self.n_obj = n_obj
+        self.n_var = n_var
+        self.n_cons = 0
+        self.n_original_constraints = 3
+
+        self.ubound = np.zeros(self.n_var)
+        self.lbound = np.zeros(self.n_var)
+        self.lbound[0] = 0.00001
+        self.lbound[1] = 0.00001
+        self.lbound[2] = 1.0
+        self.ubound[0] = 100.0
+        self.ubound[1] = 100.0
+        self.ubound[2] = 3.0
+
+        self.ideal = np.array([5.53731918799e-05, 0.333333333333, 0.0])
+        self.nadir = np.array([500.002668442, 8246211.25124, 19359919.7502])
+
+
+    def _evaluate_numpy(self, x):
+        n_sub = len(x)
+        f = np.zeros( (n_sub, self.n_obj) )
+        g = np.zeros( (n_sub, self.n_original_constraints) )
+
+        x1 = x[:,0]
+        x2 = x[:,1]
+        x3 = x[:,2]
+
+        # First original objective function
+        f[:,0] = x1 * np.sqrt(16.0 + (x3 * x3)) + x2 * np.sqrt(1.0 + x3 * x3)
+        # Second original objective function
+        f[:,1] = (20.0 * np.sqrt(16.0 + (x3 * x3))) / (x1 * x3)
+
+        # Constraint functions
+        g[:,0] = 0.1 - f[:,0]
+        g[:,1] = 100000.0 - f[:,1]
+        g[:,2] = 100000 - ((80.0 * np.sqrt(1.0 + x3 * x3)) / (x3 * x2))
+        g = np.where(g < 0, -g, 0)
+        f[:,2] = g[:,0] + g[:,1] + g[:,2]
+
+        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
+        return f_norm
+
+    def _evaluate_torch(self, x):
+        pass
+
+
+class RE37(mop):
+    def __init__(self, n_obj=3, n_var=4):
+        self.problem_name = 'RE37'
+        self.n_obj = n_obj
+        self.n_var = n_var
+        self.n_cons = 0
+        self.n_original_constraints = 0
+
+        self.lbound = np.full(self.n_var, 0)
+        self.ubound = np.full(self.n_var, 1)
+
+        self.ideal = np.array([0.00889341391106, 0.00488, -0.431499999825])
+        self.nadir = np.array([0.98949120096, 0.956587924661, 0.987530948586])
+
+
+    def _evaluate_numpy(self, x):
+        n_sub = len(x)
+        f = np.zeros( (n_sub, self.n_obj) )
+
+        xAlpha = x[:,0]
+        xHA = x[:,1]
+        xOA = x[:,2]
+        xOPTT = x[:,3]
+
+        # f1 (TF_max)
+        f[:,0] = 0.692 + (0.477 * xAlpha) - (0.687 * xHA) - (0.080 * xOA) - (0.0650 * xOPTT) - (
+                    0.167 * xAlpha * xAlpha) - (0.0129 * xHA * xAlpha) + (0.0796 * xHA * xHA) - (
+                           0.0634 * xOA * xAlpha) - (0.0257 * xOA * xHA) + (0.0877 * xOA * xOA) - (
+                           0.0521 * xOPTT * xAlpha) + (0.00156 * xOPTT * xHA) + (0.00198 * xOPTT * xOA) + (
+                           0.0184 * xOPTT * xOPTT)
+        # f2 (X_cc)
+        f[:,1] = 0.153 - (0.322 * xAlpha) + (0.396 * xHA) + (0.424 * xOA) + (0.0226 * xOPTT) + (
+                    0.175 * xAlpha * xAlpha) + (0.0185 * xHA * xAlpha) - (0.0701 * xHA * xHA) - (
+                           0.251 * xOA * xAlpha) + (0.179 * xOA * xHA) + (0.0150 * xOA * xOA) + (
+                           0.0134 * xOPTT * xAlpha) + (0.0296 * xOPTT * xHA) + (0.0752 * xOPTT * xOA) + (
+                           0.0192 * xOPTT * xOPTT)
+        # f3 (TT_max)
+        f[:,2] = 0.370 - (0.205 * xAlpha) + (0.0307 * xHA) + (0.108 * xOA) + (1.019 * xOPTT) - (
+                    0.135 * xAlpha * xAlpha) + (0.0141 * xHA * xAlpha) + (0.0998 * xHA * xHA) + (
+                           0.208 * xOA * xAlpha) - (0.0301 * xOA * xHA) - (0.226 * xOA * xOA) + (
+                           0.353 * xOPTT * xAlpha) - (0.0497 * xOPTT * xOA) - (0.423 * xOPTT * xOPTT) + (
+                           0.202 * xHA * xAlpha * xAlpha) - (0.281 * xOA * xAlpha * xAlpha) - (
+                           0.342 * xHA * xHA * xAlpha) - (0.245 * xHA * xHA * xOA) + (0.281 * xOA * xOA * xHA) - (
+                           0.184 * xOPTT * xOPTT * xAlpha) - (0.281 * xHA * xAlpha * xOA)
+
+        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
+        return f_norm
+
+
+
+class RE41(mop):
+    def __init__(self, n_obj=4, n_var=7):
+        self.problem_name = 'RE41'
+        self.n_obj = n_obj
+        self.n_var = n_var
+        self.n_cons = 0
+        self.n_original_constraints = 10
+
+        self.lbound = np.zeros(self.n_var)
+        self.ubound = np.zeros(self.n_var)
+        self.lbound[0] = 0.5
+        self.lbound[1] = 0.45
+        self.lbound[2] = 0.5
+        self.lbound[3] = 0.5
+        self.lbound[4] = 0.875
+        self.lbound[5] = 0.4
+        self.lbound[6] = 0.4
+        self.ubound[0] = 1.5
+        self.ubound[1] = 1.35
+        self.ubound[2] = 1.5
+        self.ubound[3] = 1.5
+        self.ubound[4] = 2.625
+        self.ubound[5] = 1.2
+        self.ubound[6] = 1.2
+
+        self.ideal = np.array([15.576004, 3.58525, 10.61064375, 0.0])
+        self.nadir = np.array([39.2905121788, 4.42725, 13.09138125, 9.49401929991])
+
+
+    def _evaluate_numpy(self, x):
+        n_sub = len(x)
+
+        f = np.zeros( (n_sub, self.n_obj) )
+        g = np.zeros( (n_sub, self.n_original_constraints) )
+
+        x1 = x[:,0]
+        x2 = x[:,1]
+        x3 = x[:,2]
+        x4 = x[:,3]
+        x5 = x[:,4]
+        x6 = x[:,5]
+        x7 = x[:,6]
+
+        # First original objective function
+        f[:,0] = 1.98 + 4.9 * x1 + 6.67 * x2 + 6.98 * x3 + 4.01 * x4 + 1.78 * x5 + 0.00001 * x6 + 2.73 * x7
+        # Second original objective function
+        f[:,1] = 4.72 - 0.5 * x4 - 0.19 * x2 * x3
+        # Third original objective function
+        Vmbp = 10.58 - 0.674 * x1 * x2 - 0.67275 * x2
+        Vfd = 16.45 - 0.489 * x3 * x7 - 0.843 * x5 * x6
+        f[:,2] = 0.5 * (Vmbp + Vfd)
+
+        # Constraint functions
+        g[:,0] = 1 - (1.16 - 0.3717 * x2 * x4 - 0.0092928 * x3)
+        g[:,1] = 0.32 - (0.261 - 0.0159 * x1 * x2 - 0.06486 * x1 - 0.019 * x2 * x7 + 0.0144 * x3 * x5 + 0.0154464 * x6)
+        g[:,2] = 0.32 - (
+                    0.214 + 0.00817 * x5 - 0.045195 * x1 - 0.0135168 * x1 + 0.03099 * x2 * x6 - 0.018 * x2 * x7 + 0.007176 * x3 + 0.023232 * x3 - 0.00364 * x5 * x6 - 0.018 * x2 * x2)
+        g[:,3] = 0.32 - (0.74 - 0.61 * x2 - 0.031296 * x3 - 0.031872 * x7 + 0.227 * x2 * x2)
+        g[:,4] = 32 - (28.98 + 3.818 * x3 - 4.2 * x1 * x2 + 1.27296 * x6 - 2.68065 * x7)
+        g[:,5] = 32 - (33.86 + 2.95 * x3 - 5.057 * x1 * x2 - 3.795 * x2 - 3.4431 * x7 + 1.45728)
+        g[:,6] = 32 - (46.36 - 9.9 * x2 - 4.4505 * x1)
+        g[:,7] = 4 - f[:,1]
+        g[:,8] = 9.9 - Vmbp
+        g[:,9] = 15.7 - Vfd
+        g = np.where(g < 0, -g, 0)
+        f[:,3] = g[:,0] + g[:,1] + g[:,2] + g[:,3] + g[:,4] + g[:,5] + g[:,6] + g[:,7] + g[:,8] + g[:,9]
+        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
+        return f_norm
+
+    def _evaluate_torch(self, x):
+        pass
+
+
+class RE42(mop):
+    def __init__(self):
+        self.problem_name = 'RE42'
+
+        self.n_obj = 4
+        self.n_var = 6
+        self.n_cons = 0
+        self.n_original_constraints = 9
+
+        self.lbound = np.zeros(self.n_var )
+        self.ubound = np.zeros(self.n_var )
+        self.lbound[0] = 150.0
+        self.lbound[1] = 20.0
+        self.lbound[2] = 13.0
+        self.lbound[3] = 10.0
+        self.lbound[4] = 14.0
+        self.lbound[5] = 0.63
+        self.ubound[0] = 274.32
+        self.ubound[1] = 32.31
+        self.ubound[2] = 25.0
+        self.ubound[3] = 11.71
+        self.ubound[4] = 18.0
+        self.ubound[5] = 0.75
+
+        self.ideal = np.array([-2756.2590400638524, 3962.557843228888, 1947.880856925791, 0.0])
+        self.nadir = np.array([-1010.5229595219643, 13827.138456300128, 2611.9668107424536, 12.437669929732023 ])
+
+
+
+    def _evaluate_numpy(self, x):
+        n_sub = len(x)
+
+        f = np.zeros( (n_sub, self.n_obj) )
+        # NOT g
+        constraintFuncs = np.zeros( (n_sub, self.n_original_constraints) )
+
+        x_L = x[:,0]
+        x_B = x[:,1]
+        x_D = x[:,2]
+        x_T = x[:,3]
+        x_Vk = x[:,4]
+        x_CB = x[:,5]
+
+        displacement = 1.025 * x_L * x_B * x_T * x_CB
+        V = 0.5144 * x_Vk
+        g = 9.8065
+        Fn = V / np.power(g * x_L, 0.5)
+        a = (4977.06 * x_CB * x_CB) - (8105.61 * x_CB) + 4456.51
+        b = (-10847.2 * x_CB * x_CB) + (12817.0 * x_CB) - 6960.32
+
+        power = (np.power(displacement, 2.0 / 3.0) * np.power(x_Vk, 3.0)) / (a + (b * Fn))
+        outfit_weight = 1.0 * np.power(x_L, 0.8) * np.power(x_B, 0.6) * np.power(x_D, 0.3) * np.power(x_CB, 0.1)
+        steel_weight = 0.034 * np.power(x_L, 1.7) * np.power(x_B, 0.7) * np.power(x_D, 0.4) * np.power(x_CB, 0.5)
+        machinery_weight = 0.17 * np.power(power, 0.9)
+        light_ship_weight = steel_weight + outfit_weight + machinery_weight
+
+        ship_cost = 1.3 * ((2000.0 * np.power(steel_weight, 0.85)) + (3500.0 * outfit_weight) + (
+                    2400.0 * np.power(power, 0.8)))
+        capital_costs = 0.2 * ship_cost
+
+        DWT = displacement - light_ship_weight
+
+        running_costs = 40000.0 * np.power(DWT, 0.3)
+
+        round_trip_miles = 5000.0
+        sea_days = (round_trip_miles / 24.0) * x_Vk
+        handling_rate = 8000.0
+
+        daily_consumption = ((0.19 * power * 24.0) / 1000.0) + 0.2
+        fuel_price = 100.0
+        fuel_cost = 1.05 * daily_consumption * sea_days * fuel_price
+        port_cost = 6.3 * np.power(DWT, 0.8)
+
+        fuel_carried = daily_consumption * (sea_days + 5.0)
+        miscellaneous_DWT = 2.0 * np.power(DWT, 0.5)
+
+        cargo_DWT = DWT - fuel_carried - miscellaneous_DWT
+        port_days = 2.0 * ((cargo_DWT / handling_rate) + 0.5)
+        RTPA = 350.0 / (sea_days + port_days)
+
+        voyage_costs = (fuel_cost + port_cost) * RTPA
+        annual_costs = capital_costs + running_costs + voyage_costs
+        annual_cargo = cargo_DWT * RTPA
+
+        f[:,0] = annual_costs / annual_cargo
+        f[:,1] = light_ship_weight
+        # f_2 is dealt as a minimization problem
+        f[:,2] = -annual_cargo
+
+        # Reformulated objective functions
+        constraintFuncs[:,0] = (x_L / x_B) - 6.0
+        constraintFuncs[:,1] = -(x_L / x_D) + 15.0
+        constraintFuncs[:,2] = -(x_L / x_T) + 19.0
+        constraintFuncs[:,3] = 0.45 * np.power(DWT, 0.31) - x_T
+        constraintFuncs[:,4] = 0.7 * x_D + 0.7 - x_T
+        constraintFuncs[:,5] = 500000.0 - DWT
+        constraintFuncs[:,6] = DWT - 3000.0
+        constraintFuncs[:,7] = 0.32 - Fn
+
+        KB = 0.53 * x_T
+        BMT = ((0.085 * x_CB - 0.002) * x_B * x_B) / (x_T * x_CB)
+        KG = 1.0 + 0.52 * x_D
+        constraintFuncs[:,8] = (KB + BMT - KG) - (0.07 * x_B)
+
+        constraintFuncs = np.where(constraintFuncs < 0, -constraintFuncs, 0)
+        f[:,3] = constraintFuncs[:,0] + constraintFuncs[:,1] + constraintFuncs[:,2] + constraintFuncs[:,3] + constraintFuncs[:,4] + \
+               constraintFuncs[:,5] + constraintFuncs[:,6] + constraintFuncs[:,7] + constraintFuncs[:,8]
+
+        f_norm = (f - self.ideal) / (self.nadir - self.ideal)
+        return f
+
+
+
+
+
```

### Comparing `libmoon-0.1.9/libmoon/problem/synthetic/re_original.py` & `libmoon-0.2.1/libmoon/problem/synthetic/re_original.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,1335 +1,1335 @@
-#!/usr/bin/env python
-"""
-  A real-world multimnist-objective problem suite (the RE benchmark set)
-  Reference:
-  Ryoji Tanabe, Hisao Ishibuchi, "An Easy-to-use Real-world Multi-objective Problem Suite" Applied Soft Computing. 89: 106078 (2020)
-   Copyright (c) 2020 Ryoji Tanabe
-
-  I re-implemented the RE problem set by referring to its C source code (reproblem.c). While variables directly copied from the C source code are written in CamelCase, the other variables are written in snake_case. It is somewhat awkward.
-
-  This program is free software: you can redistribute it and/or modify
-  it under the terms of the GNU General Public License as published by
-  the Free Software Foundation, either version 3 of the License, or
-  (at your option) any later version.
-
-  This program is distributed in the hope that it will be useful,
-  but WITHOUT ANY WARRANTY; without even the implied warranty of
-  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-  GNU General Public License for more details.
-
-  You should have received a copy of the GNU General Public License
-  along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import numpy as np
-
-class RE21():
-    def __init__(self, n_var=4, n_obj=2, lower_bound=np.zeros(30),
-                 upper_bound=np.ones(30)):
-        self.problem_name = 'RE21'
-        self.n_constraints = 0
-        self.n_original_constraints = 0
-
-        F = 10.0
-        sigma = 10.0
-        tmp_val = F / sigma
-
-        self.ubound = np.full(self.n_variables, 3 * tmp_val)
-        self.lbound = np.zeros(self.n_variables)
-        self.lbound[0] = tmp_val
-        self.lbound[1] = np.sqrt(2.0) * tmp_val
-        self.lbound[2] = np.sqrt(2.0) * tmp_val
-        self.lbound[3] = tmp_val
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        x1 = x[0]
-        x2 = x[1]
-        x3 = x[2]
-        x4 = x[3]
-
-        F = 10.0
-        sigma = 10.0
-        E = 2.0 * 1e5
-        L = 200.0
-
-        f[0] = L * ((2 * x1) + np.sqrt(2.0) * x2 + np.sqrt(x3) + x4)
-        f[1] = ((F * L) / E) * ((2.0 / x1) + (2.0 * np.sqrt(2.0) / x2) - (2.0 * np.sqrt(2.0) / x3) + (2.0 / x4))
-
-        return f
-
-
-class RE22():
-    def __init__(self):
-        self.problem_name = 'RE22'
-        self.n_objectives = 2
-        self.n_variables = 3
-
-        self.n_constraints = 0
-        self.n_original_constraints = 2
-
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound = np.zeros(self.n_variables)
-        self.lbound[0] = 0.2
-        self.lbound[1] = 0.0
-        self.lbound[2] = 0.0
-        self.ubound[0] = 15
-        self.ubound[1] = 20
-        self.ubound[2] = 40
-
-        self.feasible_vals = np.array(
-            [0.20, 0.31, 0.40, 0.44, 0.60, 0.62, 0.79, 0.80, 0.88, 0.93, 1.0, 1.20, 1.24, 1.32, 1.40, 1.55, 1.58, 1.60,
-             1.76, 1.80, 1.86, 2.0, 2.17, 2.20, 2.37, 2.40, 2.48, 2.60, 2.64, 2.79, 2.80, 3.0, 3.08, 3, 10, 3.16, 3.41,
-             3.52, 3.60, 3.72, 3.95, 3.96, 4.0, 4.03, 4.20, 4.34, 4.40, 4.65, 4.74, 4.80, 4.84, 5.0, 5.28, 5.40, 5.53,
-             5.72, 6.0, 6.16, 6.32, 6.60, 7.11, 7.20, 7.80, 7.90, 8.0, 8.40, 8.69, 9.0, 9.48, 10.27, 11.0, 11.06, 11.85,
-             12.0, 13.0, 14.0, 15.0])
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_original_constraints)
-        # Reference: getNearestValue_sample2.py (https://gist.github.com/icchi-h/1d0bb1c52ebfdd31f14b3e811328390a)
-        idx = np.abs(np.asarray(self.feasible_vals) - x[0]).argmin()
-        x1 = self.feasible_vals[idx]
-        x2 = x[1]
-        x3 = x[2]
-
-        # First original objective function
-        f[0] = (29.4 * x1) + (0.6 * x2 * x3)
-
-        # Original constraint functions
-        g[0] = (x1 * x3) - 7.735 * ((x1 * x1) / x2) - 180.0
-        g[1] = 4.0 - (x3 / x2)
-        g = np.where(g < 0, -g, 0)
-        f[1] = g[0] + g[1]
-
-        return f
-
-
-class RE23():
-    def __init__(self):
-        self.problem_name = 'RE23'
-        self.n_objectives = 2
-        self.n_variables = 4
-        self.n_constraints = 0
-        self.n_original_constraints = 3
-
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound = np.zeros(self.n_variables)
-        self.lbound[0] = 1
-        self.lbound[1] = 1
-        self.lbound[2] = 10
-        self.lbound[3] = 10
-        self.ubound[0] = 100
-        self.ubound[1] = 100
-        self.ubound[2] = 200
-        self.ubound[3] = 240
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_original_constraints)
-
-        x1 = 0.0625 * int(np.round(x[0]))
-        x2 = 0.0625 * int(np.round(x[1]))
-        x3 = x[2]
-        x4 = x[3]
-
-        # First original objective function
-        f[0] = (0.6224 * x1 * x3 * x4) + (1.7781 * x2 * x3 * x3) + (3.1661 * x1 * x1 * x4) + (19.84 * x1 * x1 * x3)
-
-        # Original constraint functions
-        g[0] = x1 - (0.0193 * x3)
-        g[1] = x2 - (0.00954 * x3)
-        g[2] = (np.pi * x3 * x3 * x4) + ((4.0 / 3.0) * (np.pi * x3 * x3 * x3)) - 1296000
-        g = np.where(g < 0, -g, 0)
-        f[1] = g[0] + g[1] + g[2]
-
-        return f
-
-
-class RE24():
-    def __init__(self):
-        self.problem_name = 'RE24'
-        self.n_objectives = 2
-        self.n_variables = 2
-        self.n_constraints = 0
-        self.n_original_constraints = 4
-
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound = np.zeros(self.n_variables)
-        self.lbound[0] = 0.5
-        self.lbound[1] = 0.5
-        self.ubound[0] = 4
-        self.ubound[1] = 50
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_original_constraints)
-
-        x1 = x[0]
-        x2 = x[1]
-
-        # First original objective function
-        f[0] = x1 + (120 * x2)
-
-        E = 700000
-        sigma_b_max = 700
-        tau_max = 450
-        delta_max = 1.5
-        sigma_k = (E * x1 * x1) / 100
-        sigma_b = 4500 / (x1 * x2)
-        tau = 1800 / x2
-        delta = (56.2 * 10000) / (E * x1 * x2 * x2)
-
-        g[0] = 1 - (sigma_b / sigma_b_max)
-        g[1] = 1 - (tau / tau_max)
-        g[2] = 1 - (delta / delta_max)
-        g[3] = 1 - (sigma_b / sigma_k)
-        g = np.where(g < 0, -g, 0)
-        f[1] = g[0] + g[1] + g[2] + g[3]
-
-        return f
-
-
-class RE25():
-    def __init__(self):
-        self.problem_name = 'RE25'
-        self.n_objectives = 2
-        self.n_variables = 3
-        self.n_constraints = 0
-        self.n_original_constraints = 6
-
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound = np.zeros(self.n_variables)
-        self.lbound[0] = 1
-        self.lbound[1] = 0.6
-        self.lbound[2] = 0.09
-        self.ubound[0] = 70
-        self.ubound[1] = 3
-        self.ubound[2] = 0.5
-
-        self.feasible_vals = np.array(
-            [0.009, 0.0095, 0.0104, 0.0118, 0.0128, 0.0132, 0.014, 0.015, 0.0162, 0.0173, 0.018, 0.02, 0.023, 0.025,
-             0.028, 0.032, 0.035, 0.041, 0.047, 0.054, 0.063, 0.072, 0.08, 0.092, 0.105, 0.12, 0.135, 0.148, 0.162,
-             0.177, 0.192, 0.207, 0.225, 0.244, 0.263, 0.283, 0.307, 0.331, 0.362, 0.394, 0.4375, 0.5])
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_original_constraints)
-
-        x1 = np.round(x[0])
-        x2 = x[1]
-        # Reference: getNearestValue_sample2.py (https://gist.github.com/icchi-h/1d0bb1c52ebfdd31f14b3e811328390a)
-        idx = np.abs(np.asarray(self.feasible_vals) - x[2]).argmin()
-        x3 = self.feasible_vals[idx]
-
-        # first original objective function
-        f[0] = (np.pi * np.pi * x2 * x3 * x3 * (x1 + 2)) / 4.0
-
-        # constraint functions
-        Cf = ((4.0 * (x2 / x3) - 1) / (4.0 * (x2 / x3) - 4)) + (0.615 * x3 / x2)
-        Fmax = 1000.0
-        S = 189000.0
-        G = 11.5 * 1e+6
-        K = (G * x3 * x3 * x3 * x3) / (8 * x1 * x2 * x2 * x2)
-        lmax = 14.0
-        lf = (Fmax / K) + 1.05 * (x1 + 2) * x3
-        dmin = 0.2
-        Dmax = 3
-        Fp = 300.0
-        sigmaP = Fp / K
-        sigmaPM = 6
-        sigmaW = 1.25
-
-        g[0] = -((8 * Cf * Fmax * x2) / (np.pi * x3 * x3 * x3)) + S
-        g[1] = -lf + lmax
-        g[2] = -3 + (x2 / x3)
-        g[3] = -sigmaP + sigmaPM
-        g[4] = -sigmaP - ((Fmax - Fp) / K) - 1.05 * (x1 + 2) * x3 + lf
-        g[5] = sigmaW - ((Fmax - Fp) / K)
-
-        g = np.where(g < 0, -g, 0)
-        f[1] = g[0] + g[1] + g[2] + g[3] + g[4] + g[5]
-
-        return f
-
-
-class RE31():
-    def __init__(self):
-        self.problem_name = 'RE31'
-        self.n_objectives = 3
-        self.n_variables = 3
-        self.n_constraints = 0
-        self.n_original_constraints = 3
-
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound = np.zeros(self.n_variables)
-        self.lbound[0] = 0.00001
-        self.lbound[1] = 0.00001
-        self.lbound[2] = 1.0
-        self.ubound[0] = 100.0
-        self.ubound[1] = 100.0
-        self.ubound[2] = 3.0
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_original_constraints)
-
-        x1 = x[0]
-        x2 = x[1]
-        x3 = x[2]
-
-        # First original objective function
-        f[0] = x1 * np.sqrt(16.0 + (x3 * x3)) + x2 * np.sqrt(1.0 + x3 * x3)
-        # Second original objective function
-        f[1] = (20.0 * np.sqrt(16.0 + (x3 * x3))) / (x1 * x3)
-
-        # Constraint functions
-        g[0] = 0.1 - f[0]
-        g[1] = 100000.0 - f[1]
-        g[2] = 100000 - ((80.0 * np.sqrt(1.0 + x3 * x3)) / (x3 * x2))
-        g = np.where(g < 0, -g, 0)
-        f[2] = g[0] + g[1] + g[2]
-
-        return f
-
-
-class RE32():
-    def __init__(self):
-        self.problem_name = 'RE32'
-        self.n_objectives = 3
-        self.n_variables = 4
-        self.n_constraints = 0
-        self.n_original_constraints = 4
-
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound = np.zeros(self.n_variables)
-        self.lbound[0] = 0.125
-        self.lbound[1] = 0.1
-        self.lbound[2] = 0.1
-        self.lbound[3] = 0.125
-        self.ubound[0] = 5.0
-        self.ubound[1] = 10.0
-        self.ubound[2] = 10.0
-        self.ubound[3] = 5.0
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_original_constraints)
-
-        x1 = x[0]
-        x2 = x[1]
-        x3 = x[2]
-        x4 = x[3]
-
-        P = 6000
-        L = 14
-        E = 30 * 1e6
-
-        # // deltaMax = 0.25
-        G = 12 * 1e6
-        tauMax = 13600
-        sigmaMax = 30000
-
-        # First original objective function
-        f[0] = (1.10471 * x1 * x1 * x2) + (0.04811 * x3 * x4) * (14.0 + x2)
-        # Second original objective function
-        f[1] = (4 * P * L * L * L) / (E * x4 * x3 * x3 * x3)
-
-        # Constraint functions
-        M = P * (L + (x2 / 2))
-        tmpVar = ((x2 * x2) / 4.0) + np.power((x1 + x3) / 2.0, 2)
-        R = np.sqrt(tmpVar)
-        tmpVar = ((x2 * x2) / 12.0) + np.power((x1 + x3) / 2.0, 2)
-        J = 2 * np.sqrt(2) * x1 * x2 * tmpVar
-
-        tauDashDash = (M * R) / J
-        tauDash = P / (np.sqrt(2) * x1 * x2)
-        tmpVar = tauDash * tauDash + ((2 * tauDash * tauDashDash * x2) / (2 * R)) + (tauDashDash * tauDashDash)
-        tau = np.sqrt(tmpVar)
-        sigma = (6 * P * L) / (x4 * x3 * x3)
-        tmpVar = 4.013 * E * np.sqrt((x3 * x3 * x4 * x4 * x4 * x4 * x4 * x4) / 36.0) / (L * L)
-        tmpVar2 = (x3 / (2 * L)) * np.sqrt(E / (4 * G))
-        PC = tmpVar * (1 - tmpVar2)
-
-        g[0] = tauMax - tau
-        g[1] = sigmaMax - sigma
-        g[2] = x4 - x1
-        g[3] = PC - P
-        g = np.where(g < 0, -g, 0)
-        f[2] = g[0] + g[1] + g[2] + g[3]
-
-        return f
-
-
-class RE33():
-    def __init__(self):
-        self.problem_name = 'RE33'
-        self.n_objectives = 3
-        self.n_variables = 4
-        self.n_constraints = 0
-        self.n_original_constraints = 4
-
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound = np.zeros(self.n_variables)
-        self.lbound[0] = 55
-        self.lbound[1] = 75
-        self.lbound[2] = 1000
-        self.lbound[3] = 11
-        self.ubound[0] = 80
-        self.ubound[1] = 110
-        self.ubound[2] = 3000
-        self.ubound[3] = 20
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_original_constraints)
-
-        x1 = x[0]
-        x2 = x[1]
-        x3 = x[2]
-        x4 = x[3]
-
-        # First original objective function
-        f[0] = 4.9 * 1e-5 * (x2 * x2 - x1 * x1) * (x4 - 1.0)
-        # Second original objective function
-        f[1] = ((9.82 * 1e6) * (x2 * x2 - x1 * x1)) / (x3 * x4 * (x2 * x2 * x2 - x1 * x1 * x1))
-
-        # Reformulated objective functions
-        g[0] = (x2 - x1) - 20.0
-        g[1] = 0.4 - (x3 / (3.14 * (x2 * x2 - x1 * x1)))
-        g[2] = 1.0 - (2.22 * 1e-3 * x3 * (x2 * x2 * x2 - x1 * x1 * x1)) / np.power((x2 * x2 - x1 * x1), 2)
-        g[3] = (2.66 * 1e-2 * x3 * x4 * (x2 * x2 * x2 - x1 * x1 * x1)) / (x2 * x2 - x1 * x1) - 900.0
-        g = np.where(g < 0, -g, 0)
-        f[2] = g[0] + g[1] + g[2] + g[3]
-
-        return f
-
-
-class RE34():
-    def __init__(self):
-        self.problem_name = 'RE34'
-        self.n_objectives = 3
-        self.n_variables = 5
-        self.n_constraints = 0
-        self.n_original_constraints = 0
-
-        self.lbound = np.full(self.n_variables, 1)
-        self.ubound = np.full(self.n_variables, 3)
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_original_constraints)
-
-        x1 = x[0]
-        x2 = x[1]
-        x3 = x[2]
-        x4 = x[3]
-        x5 = x[4]
-
-        f[0] = 1640.2823 + (2.3573285 * x1) + (2.3220035 * x2) + (4.5688768 * x3) + (7.7213633 * x4) + (4.4559504 * x5)
-        f[1] = 6.5856 + (1.15 * x1) - (1.0427 * x2) + (0.9738 * x3) + (0.8364 * x4) - (0.3695 * x1 * x4) + (
-                    0.0861 * x1 * x5) + (0.3628 * x2 * x4) - (0.1106 * x1 * x1) - (0.3437 * x3 * x3) + (
-                           0.1764 * x4 * x4)
-        f[2] = -0.0551 + (0.0181 * x1) + (0.1024 * x2) + (0.0421 * x3) - (0.0073 * x1 * x2) + (0.024 * x2 * x3) - (
-                    0.0118 * x2 * x4) - (0.0204 * x3 * x4) - (0.008 * x3 * x5) - (0.0241 * x2 * x2) + (0.0109 * x4 * x4)
-
-        return f
-
-
-class RE35():
-    def __init__(self):
-        self.problem_name = 'RE35'
-        self.n_objectives = 3
-        self.n_variables = 7
-        self.n_constraints = 0
-        self.n_original_constraints = 11
-
-        self.lbound = np.zeros(self.n_variables)
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound[0] = 2.6
-        self.lbound[1] = 0.7
-        self.lbound[2] = 17
-        self.lbound[3] = 7.3
-        self.lbound[4] = 7.3
-        self.lbound[5] = 2.9
-        self.lbound[6] = 5.0
-        self.ubound[0] = 3.6
-        self.ubound[1] = 0.8
-        self.ubound[2] = 28
-        self.ubound[3] = 8.3
-        self.ubound[4] = 8.3
-        self.ubound[5] = 3.9
-        self.ubound[6] = 5.5
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_original_constraints)
-
-        x1 = x[0]
-        x2 = x[1]
-        x3 = np.round(x[2])
-        x4 = x[3]
-        x5 = x[4]
-        x6 = x[5]
-        x7 = x[6]
-
-        # First original objective function (weight)
-        f[0] = 0.7854 * x1 * (x2 * x2) * (((10.0 * x3 * x3) / 3.0) + (14.933 * x3) - 43.0934) - 1.508 * x1 * (
-                    x6 * x6 + x7 * x7) + 7.477 * (x6 * x6 * x6 + x7 * x7 * x7) + 0.7854 * (x4 * x6 * x6 + x5 * x7 * x7)
-
-        # Second original objective function (stress)
-        tmpVar = np.power((745.0 * x4) / (x2 * x3), 2.0) + 1.69 * 1e7
-        f[1] = np.sqrt(tmpVar) / (0.1 * x6 * x6 * x6)
-
-        # Constraint functions
-        g[0] = -(1.0 / (x1 * x2 * x2 * x3)) + 1.0 / 27.0
-        g[1] = -(1.0 / (x1 * x2 * x2 * x3 * x3)) + 1.0 / 397.5
-        g[2] = -(x4 * x4 * x4) / (x2 * x3 * x6 * x6 * x6 * x6) + 1.0 / 1.93
-        g[3] = -(x5 * x5 * x5) / (x2 * x3 * x7 * x7 * x7 * x7) + 1.0 / 1.93
-        g[4] = -(x2 * x3) + 40.0
-        g[5] = -(x1 / x2) + 12.0
-        g[6] = -5.0 + (x1 / x2)
-        g[7] = -1.9 + x4 - 1.5 * x6
-        g[8] = -1.9 + x5 - 1.1 * x7
-        g[9] = -f[1] + 1300.0
-        tmpVar = np.power((745.0 * x5) / (x2 * x3), 2.0) + 1.575 * 1e8
-        g[10] = -np.sqrt(tmpVar) / (0.1 * x7 * x7 * x7) + 1100.0
-        g = np.where(g < 0, -g, 0)
-        f[2] = g[0] + g[1] + g[2] + g[3] + g[4] + g[5] + g[6] + g[7] + g[8] + g[9] + g[10]
-
-        return f
-
-
-class RE36():
-    def __init__(self):
-        self.problem_name = 'RE36'
-        self.n_objectives = 3
-        self.n_variables = 4
-        self.n_constraints = 0
-        self.n_original_constraints = 1
-
-        self.lbound = np.full(self.n_variables, 12)
-        self.ubound = np.full(self.n_variables, 60)
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_original_constraints)
-
-        # all the four variables must be inverger values
-        x1 = np.round(x[0])
-        x2 = np.round(x[1])
-        x3 = np.round(x[2])
-        x4 = np.round(x[3])
-
-        # First original objective function
-        f[0] = np.abs(6.931 - ((x3 / x1) * (x4 / x2)))
-        # Second original objective function (the maximum value among the four variables)
-        l = [x1, x2, x3, x4]
-        f[1] = max(l)
-
-        g[0] = 0.5 - (f[0] / 6.931)
-        g = np.where(g < 0, -g, 0)
-        f[2] = g[0]
-
-        return f
-
-
-class RE37():
-    def __init__(self):
-        self.problem_name = 'RE37'
-        self.n_objectives = 3
-        self.n_variables = 4
-        self.n_constraints = 0
-        self.n_original_constraints = 0
-
-        self.lbound = np.full(self.n_variables, 0)
-        self.ubound = np.full(self.n_variables, 1)
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-
-        xAlpha = x[0]
-        xHA = x[1]
-        xOA = x[2]
-        xOPTT = x[3]
-
-        # f1 (TF_max)
-        f[0] = 0.692 + (0.477 * xAlpha) - (0.687 * xHA) - (0.080 * xOA) - (0.0650 * xOPTT) - (
-                    0.167 * xAlpha * xAlpha) - (0.0129 * xHA * xAlpha) + (0.0796 * xHA * xHA) - (
-                           0.0634 * xOA * xAlpha) - (0.0257 * xOA * xHA) + (0.0877 * xOA * xOA) - (
-                           0.0521 * xOPTT * xAlpha) + (0.00156 * xOPTT * xHA) + (0.00198 * xOPTT * xOA) + (
-                           0.0184 * xOPTT * xOPTT)
-        # f2 (X_cc)
-        f[1] = 0.153 - (0.322 * xAlpha) + (0.396 * xHA) + (0.424 * xOA) + (0.0226 * xOPTT) + (
-                    0.175 * xAlpha * xAlpha) + (0.0185 * xHA * xAlpha) - (0.0701 * xHA * xHA) - (
-                           0.251 * xOA * xAlpha) + (0.179 * xOA * xHA) + (0.0150 * xOA * xOA) + (
-                           0.0134 * xOPTT * xAlpha) + (0.0296 * xOPTT * xHA) + (0.0752 * xOPTT * xOA) + (
-                           0.0192 * xOPTT * xOPTT)
-        # f3 (TT_max)
-        f[2] = 0.370 - (0.205 * xAlpha) + (0.0307 * xHA) + (0.108 * xOA) + (1.019 * xOPTT) - (
-                    0.135 * xAlpha * xAlpha) + (0.0141 * xHA * xAlpha) + (0.0998 * xHA * xHA) + (
-                           0.208 * xOA * xAlpha) - (0.0301 * xOA * xHA) - (0.226 * xOA * xOA) + (
-                           0.353 * xOPTT * xAlpha) - (0.0497 * xOPTT * xOA) - (0.423 * xOPTT * xOPTT) + (
-                           0.202 * xHA * xAlpha * xAlpha) - (0.281 * xOA * xAlpha * xAlpha) - (
-                           0.342 * xHA * xHA * xAlpha) - (0.245 * xHA * xHA * xOA) + (0.281 * xOA * xOA * xHA) - (
-                           0.184 * xOPTT * xOPTT * xAlpha) - (0.281 * xHA * xAlpha * xOA)
-
-        return f
-
-
-class RE41():
-    def __init__(self):
-        self.problem_name = 'RE41'
-        self.n_objectives = 4
-        self.n_variables = 7
-        self.n_constraints = 0
-        self.n_original_constraints = 10
-
-        self.lbound = np.zeros(self.n_variables)
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound[0] = 0.5
-        self.lbound[1] = 0.45
-        self.lbound[2] = 0.5
-        self.lbound[3] = 0.5
-        self.lbound[4] = 0.875
-        self.lbound[5] = 0.4
-        self.lbound[6] = 0.4
-        self.ubound[0] = 1.5
-        self.ubound[1] = 1.35
-        self.ubound[2] = 1.5
-        self.ubound[3] = 1.5
-        self.ubound[4] = 2.625
-        self.ubound[5] = 1.2
-        self.ubound[6] = 1.2
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_original_constraints)
-
-        x1 = x[0]
-        x2 = x[1]
-        x3 = x[2]
-        x4 = x[3]
-        x5 = x[4]
-        x6 = x[5]
-        x7 = x[6]
-
-        # First original objective function
-        f[0] = 1.98 + 4.9 * x1 + 6.67 * x2 + 6.98 * x3 + 4.01 * x4 + 1.78 * x5 + 0.00001 * x6 + 2.73 * x7
-        # Second original objective function
-        f[1] = 4.72 - 0.5 * x4 - 0.19 * x2 * x3
-        # Third original objective function
-        Vmbp = 10.58 - 0.674 * x1 * x2 - 0.67275 * x2
-        Vfd = 16.45 - 0.489 * x3 * x7 - 0.843 * x5 * x6
-        f[2] = 0.5 * (Vmbp + Vfd)
-
-        # Constraint functions
-        g[0] = 1 - (1.16 - 0.3717 * x2 * x4 - 0.0092928 * x3)
-        g[1] = 0.32 - (0.261 - 0.0159 * x1 * x2 - 0.06486 * x1 - 0.019 * x2 * x7 + 0.0144 * x3 * x5 + 0.0154464 * x6)
-        g[2] = 0.32 - (
-                    0.214 + 0.00817 * x5 - 0.045195 * x1 - 0.0135168 * x1 + 0.03099 * x2 * x6 - 0.018 * x2 * x7 + 0.007176 * x3 + 0.023232 * x3 - 0.00364 * x5 * x6 - 0.018 * x2 * x2)
-        g[3] = 0.32 - (0.74 - 0.61 * x2 - 0.031296 * x3 - 0.031872 * x7 + 0.227 * x2 * x2)
-        g[4] = 32 - (28.98 + 3.818 * x3 - 4.2 * x1 * x2 + 1.27296 * x6 - 2.68065 * x7)
-        g[5] = 32 - (33.86 + 2.95 * x3 - 5.057 * x1 * x2 - 3.795 * x2 - 3.4431 * x7 + 1.45728)
-        g[6] = 32 - (46.36 - 9.9 * x2 - 4.4505 * x1)
-        g[7] = 4 - f[1]
-        g[8] = 9.9 - Vmbp
-        g[9] = 15.7 - Vfd
-
-        g = np.where(g < 0, -g, 0)
-        f[3] = g[0] + g[1] + g[2] + g[3] + g[4] + g[5] + g[6] + g[7] + g[8] + g[9]
-
-        return f
-
-
-class RE42():
-    def __init__(self):
-        self.problem_name = 'RE42'
-        self.n_objectives = 4
-        self.n_variables = 6
-        self.n_constraints = 0
-        self.n_original_constraints = 9
-
-        self.lbound = np.zeros(self.n_variables)
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound[0] = 150.0
-        self.lbound[1] = 20.0
-        self.lbound[2] = 13.0
-        self.lbound[3] = 10.0
-        self.lbound[4] = 14.0
-        self.lbound[5] = 0.63
-        self.ubound[0] = 274.32
-        self.ubound[1] = 32.31
-        self.ubound[2] = 25.0
-        self.ubound[3] = 11.71
-        self.ubound[4] = 18.0
-        self.ubound[5] = 0.75
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        # NOT g
-        constraintFuncs = np.zeros(self.n_original_constraints)
-
-        x_L = x[0]
-        x_B = x[1]
-        x_D = x[2]
-        x_T = x[3]
-        x_Vk = x[4]
-        x_CB = x[5]
-
-        displacement = 1.025 * x_L * x_B * x_T * x_CB
-        V = 0.5144 * x_Vk
-        g = 9.8065
-        Fn = V / np.power(g * x_L, 0.5)
-        a = (4977.06 * x_CB * x_CB) - (8105.61 * x_CB) + 4456.51
-        b = (-10847.2 * x_CB * x_CB) + (12817.0 * x_CB) - 6960.32
-
-        power = (np.power(displacement, 2.0 / 3.0) * np.power(x_Vk, 3.0)) / (a + (b * Fn))
-        outfit_weight = 1.0 * np.power(x_L, 0.8) * np.power(x_B, 0.6) * np.power(x_D, 0.3) * np.power(x_CB, 0.1)
-        steel_weight = 0.034 * np.power(x_L, 1.7) * np.power(x_B, 0.7) * np.power(x_D, 0.4) * np.power(x_CB, 0.5)
-        machinery_weight = 0.17 * np.power(power, 0.9)
-        light_ship_weight = steel_weight + outfit_weight + machinery_weight
-
-        ship_cost = 1.3 * ((2000.0 * np.power(steel_weight, 0.85)) + (3500.0 * outfit_weight) + (
-                    2400.0 * np.power(power, 0.8)))
-        capital_costs = 0.2 * ship_cost
-
-        DWT = displacement - light_ship_weight
-
-        running_costs = 40000.0 * np.power(DWT, 0.3)
-
-        round_trip_miles = 5000.0
-        sea_days = (round_trip_miles / 24.0) * x_Vk
-        handling_rate = 8000.0
-
-        daily_consumption = ((0.19 * power * 24.0) / 1000.0) + 0.2
-        fuel_price = 100.0
-        fuel_cost = 1.05 * daily_consumption * sea_days * fuel_price
-        port_cost = 6.3 * np.power(DWT, 0.8)
-
-        fuel_carried = daily_consumption * (sea_days + 5.0)
-        miscellaneous_DWT = 2.0 * np.power(DWT, 0.5)
-
-        cargo_DWT = DWT - fuel_carried - miscellaneous_DWT
-        port_days = 2.0 * ((cargo_DWT / handling_rate) + 0.5)
-        RTPA = 350.0 / (sea_days + port_days)
-
-        voyage_costs = (fuel_cost + port_cost) * RTPA
-        annual_costs = capital_costs + running_costs + voyage_costs
-        annual_cargo = cargo_DWT * RTPA
-
-        f[0] = annual_costs / annual_cargo
-        f[1] = light_ship_weight
-        # f_2 is dealt as a minimization problem
-        f[2] = -annual_cargo
-
-        # Reformulated objective functions
-        constraintFuncs[0] = (x_L / x_B) - 6.0
-        constraintFuncs[1] = -(x_L / x_D) + 15.0
-        constraintFuncs[2] = -(x_L / x_T) + 19.0
-        constraintFuncs[3] = 0.45 * np.power(DWT, 0.31) - x_T
-        constraintFuncs[4] = 0.7 * x_D + 0.7 - x_T
-        constraintFuncs[5] = 500000.0 - DWT
-        constraintFuncs[6] = DWT - 3000.0
-        constraintFuncs[7] = 0.32 - Fn
-
-        KB = 0.53 * x_T
-        BMT = ((0.085 * x_CB - 0.002) * x_B * x_B) / (x_T * x_CB)
-        KG = 1.0 + 0.52 * x_D
-        constraintFuncs[8] = (KB + BMT - KG) - (0.07 * x_B)
-
-        constraintFuncs = np.where(constraintFuncs < 0, -constraintFuncs, 0)
-        f[3] = constraintFuncs[0] + constraintFuncs[1] + constraintFuncs[2] + constraintFuncs[3] + constraintFuncs[4] + \
-               constraintFuncs[5] + constraintFuncs[6] + constraintFuncs[7] + constraintFuncs[8]
-
-        return f
-
-
-class RE61():
-    def __init__(self):
-        self.problem_name = 'RE61'
-        self.n_objectives = 6
-        self.n_variables = 3
-        self.n_constraints = 0
-        self.n_original_constraints = 7
-
-        self.lbound = np.zeros(self.n_variables)
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound[0] = 0.01
-        self.lbound[1] = 0.01
-        self.lbound[2] = 0.01
-        self.ubound[0] = 0.45
-        self.ubound[1] = 0.10
-        self.ubound[2] = 0.10
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_original_constraints)
-
-        # First original objective function
-        f[0] = 106780.37 * (x[1] + x[2]) + 61704.67
-        # Second original objective function
-        f[1] = 3000 * x[0]
-        # Third original objective function
-        f[2] = 305700 * 2289 * x[1] / np.power(0.06 * 2289, 0.65)
-        # Fourth original objective function
-        f[3] = 250 * 2289 * np.exp(-39.75 * x[1] + 9.9 * x[2] + 2.74)
-        # Fifth original objective function
-        f[4] = 25 * (1.39 / (x[0] * x[1]) + 4940 * x[2] - 80)
-
-        # Constraint functions
-        g[0] = 1 - (0.00139 / (x[0] * x[1]) + 4.94 * x[2] - 0.08)
-        g[1] = 1 - (0.000306 / (x[0] * x[1]) + 1.082 * x[2] - 0.0986)
-        g[2] = 50000 - (12.307 / (x[0] * x[1]) + 49408.24 * x[2] + 4051.02)
-        g[3] = 16000 - (2.098 / (x[0] * x[1]) + 8046.33 * x[2] - 696.71)
-        g[4] = 10000 - (2.138 / (x[0] * x[1]) + 7883.39 * x[2] - 705.04)
-        g[5] = 2000 - (0.417 * x[0] * x[1] + 1721.26 * x[2] - 136.54)
-        g[6] = 550 - (0.164 / (x[0] * x[1]) + 631.13 * x[2] - 54.48)
-
-        g = np.where(g < 0, -g, 0)
-        f[5] = g[0] + g[1] + g[2] + g[3] + g[4] + g[5] + g[6]
-
-        return f
-
-
-class RE91():
-    def __init__(self):
-        self.problem_name = 'RE91'
-        self.n_objectives = 9
-        self.n_variables = 7
-        self.n_constraints = 0
-        self.n_original_constraints = 0
-
-        self.lbound = np.zeros(self.n_variables)
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound[0] = 0.5
-        self.lbound[1] = 0.45
-        self.lbound[2] = 0.5
-        self.lbound[3] = 0.5
-        self.lbound[4] = 0.875
-        self.lbound[5] = 0.4
-        self.lbound[6] = 0.4
-        self.ubound[0] = 1.5
-        self.ubound[1] = 1.35
-        self.ubound[2] = 1.5
-        self.ubound[3] = 1.5
-        self.ubound[4] = 2.625
-        self.ubound[5] = 1.2
-        self.ubound[6] = 1.2
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_original_constraints)
-
-        x1 = x[0]
-        x2 = x[1]
-        x3 = x[2]
-        x4 = x[3]
-        x5 = x[4]
-        x6 = x[5]
-        x7 = x[6]
-        # stochastic variables
-        x8 = 0.006 * (np.random.normal(0, 1)) + 0.345
-        x9 = 0.006 * (np.random.normal(0, 1)) + 0.192
-        x10 = 10 * (np.random.normal(0, 1)) + 0.0
-        x11 = 10 * (np.random.normal(0, 1)) + 0.0
-
-        # First function
-        f[0] = 1.98 + 4.9 * x1 + 6.67 * x2 + 6.98 * x3 + 4.01 * x4 + 1.75 * x5 + 0.00001 * x6 + 2.73 * x7
-        # Second function
-        f[1] = max(0.0, (1.16 - 0.3717 * x2 * x4 - 0.00931 * x2 * x10 - 0.484 * x3 * x9 + 0.01343 * x6 * x10) / 1.0)
-        # Third function
-        f[2] = max(0.0, (
-                    0.261 - 0.0159 * x1 * x2 - 0.188 * x1 * x8 - 0.019 * x2 * x7 + 0.0144 * x3 * x5 + 0.87570001 * x5 * x10 + 0.08045 * x6 * x9 + 0.00139 * x8 * x11 + 0.00001575 * x10 * x11) / 0.32)
-        # Fourth function
-        f[3] = max(0.0, (
-                    0.214 + 0.00817 * x5 - 0.131 * x1 * x8 - 0.0704 * x1 * x9 + 0.03099 * x2 * x6 - 0.018 * x2 * x7 + 0.0208 * x3 * x8 + 0.121 * x3 * x9 - 0.00364 * x5 * x6 + 0.0007715 * x5 * x10 - 0.0005354 * x6 * x10 + 0.00121 * x8 * x11 + 0.00184 * x9 * x10 - 0.018 * x2 * x2) / 0.32)
-        # Fifth function
-        f[4] = max(0.0, (
-                    0.74 - 0.61 * x2 - 0.163 * x3 * x8 + 0.001232 * x3 * x10 - 0.166 * x7 * x9 + 0.227 * x2 * x2) / 0.32)
-        # Sixth function
-        tmp = ((
-                           28.98 + 3.818 * x3 - 4.2 * x1 * x2 + 0.0207 * x5 * x10 + 6.63 * x6 * x9 - 7.77 * x7 * x8 + 0.32 * x9 * x10) + (
-                           33.86 + 2.95 * x3 + 0.1792 * x10 - 5.057 * x1 * x2 - 11 * x2 * x8 - 0.0215 * x5 * x10 - 9.98 * x7 * x8 + 22 * x8 * x9) + (
-                           46.36 - 9.9 * x2 - 12.9 * x1 * x8 + 0.1107 * x3 * x10)) / 3
-        f[5] = max(0.0, tmp / 32)
-        # Seventh function
-        f[6] = max(0.0, (
-                    4.72 - 0.5 * x4 - 0.19 * x2 * x3 - 0.0122 * x4 * x10 + 0.009325 * x6 * x10 + 0.000191 * x11 * x11) / 4.0)
-        # EighthEighth function
-        f[7] = max(0.0, (
-                    10.58 - 0.674 * x1 * x2 - 1.95 * x2 * x8 + 0.02054 * x3 * x10 - 0.0198 * x4 * x10 + 0.028 * x6 * x10) / 9.9)
-        # Ninth function
-        f[8] = max(0.0, (
-                    16.45 - 0.489 * x3 * x7 - 0.843 * x5 * x6 + 0.0432 * x9 * x10 - 0.0556 * x9 * x11 - 0.000786 * x11 * x11) / 15.7)
-
-        return f
-
-
-class CRE21():
-    def __init__(self):
-        self.problem_name = 'CRE21'
-        self.n_objectives = 2
-        self.n_variables = 3
-        self.n_constraints = 3
-
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound = np.zeros(self.n_variables)
-        self.lbound[0] = 0.00001
-        self.lbound[1] = 0.00001
-        self.lbound[2] = 1.0
-        self.ubound[0] = 100.0
-        self.ubound[1] = 100.0
-        self.ubound[2] = 3.0
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_constraints)
-
-        x1 = x[0]
-        x2 = x[1]
-        x3 = x[2]
-
-        # First original objective function
-        f[0] = x1 * np.sqrt(16.0 + (x3 * x3)) + x2 * np.sqrt(1.0 + x3 * x3)
-        # Second original objective function
-        f[1] = (20.0 * np.sqrt(16.0 + (x3 * x3))) / (x1 * x3)
-
-        # Constraint functions
-        g[0] = 0.1 - f[0]
-        g[1] = 100000.0 - f[1]
-        g[2] = 100000 - ((80.0 * np.sqrt(1.0 + x3 * x3)) / (x3 * x2))
-        g = np.where(g < 0, -g, 0)
-
-        return f, g
-
-
-class CRE22():
-    def __init__(self):
-        self.problem_name = 'CRE22'
-        self.n_objectives = 2
-        self.n_variables = 4
-        self.n_constraints = 4
-
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound = np.zeros(self.n_variables)
-        self.lbound[0] = 0.125
-        self.lbound[1] = 0.1
-        self.lbound[2] = 0.1
-        self.lbound[3] = 0.125
-        self.ubound[0] = 5.0
-        self.ubound[1] = 10.0
-        self.ubound[2] = 10.0
-        self.ubound[3] = 5.0
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_constraints)
-
-        x1 = x[0]
-        x2 = x[1]
-        x3 = x[2]
-        x4 = x[3]
-
-        P = 6000
-        L = 14
-        E = 30 * 1e6
-
-        # // deltaMax = 0.25
-        G = 12 * 1e6
-        tauMax = 13600
-        sigmaMax = 30000
-
-        # First original objective function
-        f[0] = (1.10471 * x1 * x1 * x2) + (0.04811 * x3 * x4) * (14.0 + x2)
-        # Second original objective function
-        f[1] = (4 * P * L * L * L) / (E * x4 * x3 * x3 * x3)
-
-        # Constraint functions
-        M = P * (L + (x2 / 2))
-        tmpVar = ((x2 * x2) / 4.0) + np.power((x1 + x3) / 2.0, 2)
-        R = np.sqrt(tmpVar)
-        tmpVar = ((x2 * x2) / 12.0) + np.power((x1 + x3) / 2.0, 2)
-        J = 2 * np.sqrt(2) * x1 * x2 * tmpVar
-
-        tauDashDash = (M * R) / J
-        tauDash = P / (np.sqrt(2) * x1 * x2)
-        tmpVar = tauDash * tauDash + ((2 * tauDash * tauDashDash * x2) / (2 * R)) + (tauDashDash * tauDashDash)
-        tau = np.sqrt(tmpVar)
-        sigma = (6 * P * L) / (x4 * x3 * x3)
-        tmpVar = 4.013 * E * np.sqrt((x3 * x3 * x4 * x4 * x4 * x4 * x4 * x4) / 36.0) / (L * L)
-        tmpVar2 = (x3 / (2 * L)) * np.sqrt(E / (4 * G))
-        PC = tmpVar * (1 - tmpVar2)
-
-        g[0] = tauMax - tau
-        g[1] = sigmaMax - sigma
-        g[2] = x4 - x1
-        g[3] = PC - P
-        g = np.where(g < 0, -g, 0)
-
-        return f, g
-
-
-class CRE23():
-    def __init__(self):
-        self.problem_name = 'CRE23'
-        self.n_objectives = 2
-        self.n_variables = 4
-        self.n_constraints = 4
-
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound = np.zeros(self.n_variables)
-        self.lbound[0] = 55
-        self.lbound[1] = 75
-        self.lbound[2] = 1000
-        self.lbound[3] = 11
-        self.ubound[0] = 80
-        self.ubound[1] = 110
-        self.ubound[2] = 3000
-        self.ubound[3] = 20
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_constraints)
-
-        x1 = x[0]
-        x2 = x[1]
-        x3 = x[2]
-        x4 = x[3]
-
-        # First original objective function
-        f[0] = 4.9 * 1e-5 * (x2 * x2 - x1 * x1) * (x4 - 1.0)
-        # Second original objective function
-        f[1] = ((9.82 * 1e6) * (x2 * x2 - x1 * x1)) / (x3 * x4 * (x2 * x2 * x2 - x1 * x1 * x1))
-
-        # Reformulated objective functions
-        g[0] = (x2 - x1) - 20.0
-        g[1] = 0.4 - (x3 / (3.14 * (x2 * x2 - x1 * x1)))
-        g[2] = 1.0 - (2.22 * 1e-3 * x3 * (x2 * x2 * x2 - x1 * x1 * x1)) / np.power((x2 * x2 - x1 * x1), 2)
-        g[3] = (2.66 * 1e-2 * x3 * x4 * (x2 * x2 * x2 - x1 * x1 * x1)) / (x2 * x2 - x1 * x1) - 900.0
-        g = np.where(g < 0, -g, 0)
-
-        return f, g
-
-
-class CRE24():
-    def __init__(self):
-        self.problem_name = 'CRE24'
-        self.n_objectives = 2
-        self.n_variables = 7
-        self.n_constraints = 11
-
-        self.lbound = np.zeros(self.n_variables)
-        self.ubound = np.zeros(self.n_variables)
-
-        self.lbound[0] = 2.6
-        self.lbound[1] = 0.7
-        self.lbound[2] = 17
-        self.lbound[3] = 7.3
-        self.lbound[4] = 7.3
-        self.lbound[5] = 2.9
-        self.lbound[6] = 5.0
-        self.ubound[0] = 3.6
-        self.ubound[1] = 0.8
-        self.ubound[2] = 28
-        self.ubound[3] = 8.3
-        self.ubound[4] = 8.3
-        self.ubound[5] = 3.9
-        self.ubound[6] = 5.5
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_constraints)
-
-        x1 = x[0]
-        x2 = x[1]
-        x3 = np.round(x[2])
-        x4 = x[3]
-        x5 = x[4]
-        x6 = x[5]
-        x7 = x[6]
-
-        # First original objective function (weight)
-        f[0] = 0.7854 * x1 * (x2 * x2) * (((10.0 * x3 * x3) / 3.0) + (14.933 * x3) - 43.0934) - 1.508 * x1 * (
-                    x6 * x6 + x7 * x7) + 7.477 * (x6 * x6 * x6 + x7 * x7 * x7) + 0.7854 * (x4 * x6 * x6 + x5 * x7 * x7)
-
-        # Second original objective function (stress)
-        tmpVar = np.power((745.0 * x4) / (x2 * x3), 2.0) + 1.69 * 1e7
-        f[1] = np.sqrt(tmpVar) / (0.1 * x6 * x6 * x6)
-
-        # Constraint functions
-        g[0] = -(1.0 / (x1 * x2 * x2 * x3)) + 1.0 / 27.0
-        g[1] = -(1.0 / (x1 * x2 * x2 * x3 * x3)) + 1.0 / 397.5
-        g[2] = -(x4 * x4 * x4) / (x2 * x3 * x6 * x6 * x6 * x6) + 1.0 / 1.93
-        g[3] = -(x5 * x5 * x5) / (x2 * x3 * x7 * x7 * x7 * x7) + 1.0 / 1.93
-        g[4] = -(x2 * x3) + 40.0
-        g[5] = -(x1 / x2) + 12.0
-        g[6] = -5.0 + (x1 / x2)
-        g[7] = -1.9 + x4 - 1.5 * x6
-        g[8] = -1.9 + x5 - 1.1 * x7
-        g[9] = -f[1] + 1300.0
-        tmpVar = np.power((745.0 * x5) / (x2 * x3), 2.0) + 1.575 * 1e8
-        g[10] = -np.sqrt(tmpVar) / (0.1 * x7 * x7 * x7) + 1100.0
-        g = np.where(g < 0, -g, 0)
-
-        return f, g
-
-
-class CRE25():
-    def __init__(self):
-        self.problem_name = 'CRE25'
-        self.n_objectives = 2
-        self.n_variables = 4
-        self.n_constraints = 1
-
-        self.lbound = np.full(self.n_variables, 12)
-        self.ubound = np.full(self.n_variables, 60)
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_constraints)
-
-        # all the four variables must be inverger values
-        x1 = np.round(x[0])
-        x2 = np.round(x[1])
-        x3 = np.round(x[2])
-        x4 = np.round(x[3])
-
-        # First original objective function
-        f[0] = np.abs(6.931 - ((x3 / x1) * (x4 / x2)))
-        # Second original objective function (the maximum value among the four variables)
-        l = [x1, x2, x3, x4]
-        f[1] = max(l)
-
-        g[0] = 0.5 - (f[0] / 6.931)
-        g = np.where(g < 0, -g, 0)
-
-        return f, g
-
-
-class CRE31():
-    def __init__(self):
-        self.problem_name = 'CRE31'
-        self.n_objectives = 3
-        self.n_variables = 7
-        self.n_constraints = 10
-
-        self.lbound = np.zeros(self.n_variables)
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound[0] = 0.5
-        self.lbound[1] = 0.45
-        self.lbound[2] = 0.5
-        self.lbound[3] = 0.5
-        self.lbound[4] = 0.875
-        self.lbound[5] = 0.4
-        self.lbound[6] = 0.4
-        self.ubound[0] = 1.5
-        self.ubound[1] = 1.35
-        self.ubound[2] = 1.5
-        self.ubound[3] = 1.5
-        self.ubound[4] = 2.625
-        self.ubound[5] = 1.2
-        self.ubound[6] = 1.2
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_constraints)
-
-        x1 = x[0]
-        x2 = x[1]
-        x3 = x[2]
-        x4 = x[3]
-        x5 = x[4]
-        x6 = x[5]
-        x7 = x[6]
-
-        # First original objective function
-        f[0] = 1.98 + 4.9 * x1 + 6.67 * x2 + 6.98 * x3 + 4.01 * x4 + 1.78 * x5 + 0.00001 * x6 + 2.73 * x7
-        # Second original objective function
-        f[1] = 4.72 - 0.5 * x4 - 0.19 * x2 * x3
-        # Third original objective function
-        Vmbp = 10.58 - 0.674 * x1 * x2 - 0.67275 * x2
-        Vfd = 16.45 - 0.489 * x3 * x7 - 0.843 * x5 * x6
-        f[2] = 0.5 * (Vmbp + Vfd)
-
-        # Constraint functions
-        g[0] = 1 - (1.16 - 0.3717 * x2 * x4 - 0.0092928 * x3)
-        g[1] = 0.32 - (0.261 - 0.0159 * x1 * x2 - 0.06486 * x1 - 0.019 * x2 * x7 + 0.0144 * x3 * x5 + 0.0154464 * x6)
-        g[2] = 0.32 - (
-                    0.214 + 0.00817 * x5 - 0.045195 * x1 - 0.0135168 * x1 + 0.03099 * x2 * x6 - 0.018 * x2 * x7 + 0.007176 * x3 + 0.023232 * x3 - 0.00364 * x5 * x6 - 0.018 * x2 * x2)
-        g[3] = 0.32 - (0.74 - 0.61 * x2 - 0.031296 * x3 - 0.031872 * x7 + 0.227 * x2 * x2)
-        g[4] = 32 - (28.98 + 3.818 * x3 - 4.2 * x1 * x2 + 1.27296 * x6 - 2.68065 * x7)
-        g[5] = 32 - (33.86 + 2.95 * x3 - 5.057 * x1 * x2 - 3.795 * x2 - 3.4431 * x7 + 1.45728)
-        g[6] = 32 - (46.36 - 9.9 * x2 - 4.4505 * x1)
-        g[7] = 4 - f[1]
-        g[8] = 9.9 - Vmbp
-        g[9] = 15.7 - Vfd
-        g = np.where(g < 0, -g, 0)
-
-        return f, g
-
-
-class CRE32():
-    def __init__(self):
-        self.problem_name = 'CRE32'
-        self.n_objectives = 3
-        self.n_variables = 6
-        self.n_constraints = 9
-
-        self.lbound = np.zeros(self.n_variables)
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound[0] = 150.0
-        self.lbound[1] = 20.0
-        self.lbound[2] = 13.0
-        self.lbound[3] = 10.0
-        self.lbound[4] = 14.0
-        self.lbound[5] = 0.63
-        self.ubound[0] = 274.32
-        self.ubound[1] = 32.31
-        self.ubound[2] = 25.0
-        self.ubound[3] = 11.71
-        self.ubound[4] = 18.0
-        self.ubound[5] = 0.75
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        # NOT g
-        constraintFuncs = np.zeros(self.n_constraints)
-
-        x_L = x[0]
-        x_B = x[1]
-        x_D = x[2]
-        x_T = x[3]
-        x_Vk = x[4]
-        x_CB = x[5]
-
-        displacement = 1.025 * x_L * x_B * x_T * x_CB
-        V = 0.5144 * x_Vk
-        g = 9.8065
-        Fn = V / np.power(g * x_L, 0.5)
-        a = (4977.06 * x_CB * x_CB) - (8105.61 * x_CB) + 4456.51
-        b = (-10847.2 * x_CB * x_CB) + (12817.0 * x_CB) - 6960.32
-
-        power = (np.power(displacement, 2.0 / 3.0) * np.power(x_Vk, 3.0)) / (a + (b * Fn))
-        outfit_weight = 1.0 * np.power(x_L, 0.8) * np.power(x_B, 0.6) * np.power(x_D, 0.3) * np.power(x_CB, 0.1)
-        steel_weight = 0.034 * np.power(x_L, 1.7) * np.power(x_B, 0.7) * np.power(x_D, 0.4) * np.power(x_CB, 0.5)
-        machinery_weight = 0.17 * np.power(power, 0.9)
-        light_ship_weight = steel_weight + outfit_weight + machinery_weight
-
-        ship_cost = 1.3 * ((2000.0 * np.power(steel_weight, 0.85)) + (3500.0 * outfit_weight) + (
-                    2400.0 * np.power(power, 0.8)))
-        capital_costs = 0.2 * ship_cost
-
-        DWT = displacement - light_ship_weight
-
-        running_costs = 40000.0 * np.power(DWT, 0.3)
-
-        round_trip_miles = 5000.0
-        sea_days = (round_trip_miles / 24.0) * x_Vk
-        handling_rate = 8000.0
-
-        daily_consumption = ((0.19 * power * 24.0) / 1000.0) + 0.2
-        fuel_price = 100.0
-        fuel_cost = 1.05 * daily_consumption * sea_days * fuel_price
-        port_cost = 6.3 * np.power(DWT, 0.8)
-
-        fuel_carried = daily_consumption * (sea_days + 5.0)
-        miscellaneous_DWT = 2.0 * np.power(DWT, 0.5)
-
-        cargo_DWT = DWT - fuel_carried - miscellaneous_DWT
-        port_days = 2.0 * ((cargo_DWT / handling_rate) + 0.5)
-        RTPA = 350.0 / (sea_days + port_days)
-
-        voyage_costs = (fuel_cost + port_cost) * RTPA
-        annual_costs = capital_costs + running_costs + voyage_costs
-        annual_cargo = cargo_DWT * RTPA
-
-        f[0] = annual_costs / annual_cargo
-        f[1] = light_ship_weight
-        # f_2 is dealt as a minimization problem
-        f[2] = -annual_cargo
-
-        # Reformulated objective functions
-        constraintFuncs[0] = (x_L / x_B) - 6.0
-        constraintFuncs[1] = -(x_L / x_D) + 15.0
-        constraintFuncs[2] = -(x_L / x_T) + 19.0
-        constraintFuncs[3] = 0.45 * np.power(DWT, 0.31) - x_T
-        constraintFuncs[4] = 0.7 * x_D + 0.7 - x_T
-        constraintFuncs[5] = 500000.0 - DWT
-        constraintFuncs[6] = DWT - 3000.0
-        constraintFuncs[7] = 0.32 - Fn
-
-        KB = 0.53 * x_T
-        BMT = ((0.085 * x_CB - 0.002) * x_B * x_B) / (x_T * x_CB)
-        KG = 1.0 + 0.52 * x_D
-        constraintFuncs[8] = (KB + BMT - KG) - (0.07 * x_B)
-        constraintFuncs = np.where(constraintFuncs < 0, -constraintFuncs, 0)
-
-        return f, constraintFuncs
-
-
-class CRE51():
-    def __init__(self):
-        self.problem_name = 'CRE51'
-        self.n_objectives = 5
-        self.n_variables = 3
-        self.n_constraints = 7
-
-        self.lbound = np.zeros(self.n_variables)
-        self.ubound = np.zeros(self.n_variables)
-        self.lbound[0] = 0.01
-        self.lbound[1] = 0.01
-        self.lbound[2] = 0.01
-        self.ubound[0] = 0.45
-        self.ubound[1] = 0.10
-        self.ubound[2] = 0.10
-
-    def evaluate(self, x):
-        f = np.zeros(self.n_objectives)
-        g = np.zeros(self.n_constraints)
-
-        # First original objective function
-        f[0] = 106780.37 * (x[1] + x[2]) + 61704.67
-        # Second original objective function
-        f[1] = 3000 * x[0]
-        # Third original objective function
-        f[2] = 305700 * 2289 * x[1] / np.power(0.06 * 2289, 0.65)
-        # Fourth original objective function
-        f[3] = 250 * 2289 * np.exp(-39.75 * x[1] + 9.9 * x[2] + 2.74)
-        # Fifth original objective function
-        f[4] = 25 * (1.39 / (x[0] * x[1]) + 4940 * x[2] - 80)
-
-        # Constraint functions
-        g[0] = 1 - (0.00139 / (x[0] * x[1]) + 4.94 * x[2] - 0.08)
-        g[1] = 1 - (0.000306 / (x[0] * x[1]) + 1.082 * x[2] - 0.0986)
-        g[2] = 50000 - (12.307 / (x[0] * x[1]) + 49408.24 * x[2] + 4051.02)
-        g[3] = 16000 - (2.098 / (x[0] * x[1]) + 8046.33 * x[2] - 696.71)
-        g[4] = 10000 - (2.138 / (x[0] * x[1]) + 7883.39 * x[2] - 705.04)
-        g[5] = 2000 - (0.417 * x[0] * x[1] + 1721.26 * x[2] - 136.54)
-        g[6] = 550 - (0.164 / (x[0] * x[1]) + 631.13 * x[2] - 54.48)
-        g = np.where(g < 0, -g, 0)
-
-        return f, g
-
-
-
-
-if __name__ == '__main__':
-    np.random.seed(seed=1)
-    fun = RE21()
-
-    x = fun.lbound + (fun.ubound - fun.lbound) * np.random.rand(fun.n_variables)
-    print("Problem = {}".format(fun.problem_name))
-    print("Number of objectives = {}".format(fun.n_objectives))
-    print("Number of variables = {}".format(fun.n_variables))
-    print("Number of constraints = {}".format(fun.n_constraints))
-    print("Lower bounds = ", fun.lbound)
-    print("Upper bounds = ", fun.ubound)
-    print("x = ", x)
-
-    if 'CRE' in fun.problem_name:
-        f, g = fun.evaluate(x)
-        print("f(x) = {}".format(f))
-        print("g(x) = {}".format(g))
-    else:
-        f = fun.evaluate(x)
+#!/usr/bin/env python
+"""
+  A real-world multimnist-objective problem suite (the RE benchmark set)
+  Reference:
+  Ryoji Tanabe, Hisao Ishibuchi, "An Easy-to-use Real-world Multi-objective Problem Suite" Applied Soft Computing. 89: 106078 (2020)
+   Copyright (c) 2020 Ryoji Tanabe
+
+  I re-implemented the RE problem set by referring to its C source code (reproblem.c). While variables directly copied from the C source code are written in CamelCase, the other variables are written in snake_case. It is somewhat awkward.
+
+  This program is free software: you can redistribute it and/or modify
+  it under the terms of the GNU General Public License as published by
+  the Free Software Foundation, either version 3 of the License, or
+  (at your option) any later version.
+
+  This program is distributed in the hope that it will be useful,
+  but WITHOUT ANY WARRANTY; without even the implied warranty of
+  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+  GNU General Public License for more details.
+
+  You should have received a copy of the GNU General Public License
+  along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+import numpy as np
+
+class RE21():
+    def __init__(self, n_var=4, n_obj=2, lower_bound=np.zeros(30),
+                 upper_bound=np.ones(30)):
+        self.problem_name = 'RE21'
+        self.n_constraints = 0
+        self.n_original_constraints = 0
+
+        F = 10.0
+        sigma = 10.0
+        tmp_val = F / sigma
+
+        self.ubound = np.full(self.n_variables, 3 * tmp_val)
+        self.lbound = np.zeros(self.n_variables)
+        self.lbound[0] = tmp_val
+        self.lbound[1] = np.sqrt(2.0) * tmp_val
+        self.lbound[2] = np.sqrt(2.0) * tmp_val
+        self.lbound[3] = tmp_val
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        x1 = x[0]
+        x2 = x[1]
+        x3 = x[2]
+        x4 = x[3]
+
+        F = 10.0
+        sigma = 10.0
+        E = 2.0 * 1e5
+        L = 200.0
+
+        f[0] = L * ((2 * x1) + np.sqrt(2.0) * x2 + np.sqrt(x3) + x4)
+        f[1] = ((F * L) / E) * ((2.0 / x1) + (2.0 * np.sqrt(2.0) / x2) - (2.0 * np.sqrt(2.0) / x3) + (2.0 / x4))
+
+        return f
+
+
+class RE22():
+    def __init__(self):
+        self.problem_name = 'RE22'
+        self.n_objectives = 2
+        self.n_variables = 3
+
+        self.n_constraints = 0
+        self.n_original_constraints = 2
+
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound = np.zeros(self.n_variables)
+        self.lbound[0] = 0.2
+        self.lbound[1] = 0.0
+        self.lbound[2] = 0.0
+        self.ubound[0] = 15
+        self.ubound[1] = 20
+        self.ubound[2] = 40
+
+        self.feasible_vals = np.array(
+            [0.20, 0.31, 0.40, 0.44, 0.60, 0.62, 0.79, 0.80, 0.88, 0.93, 1.0, 1.20, 1.24, 1.32, 1.40, 1.55, 1.58, 1.60,
+             1.76, 1.80, 1.86, 2.0, 2.17, 2.20, 2.37, 2.40, 2.48, 2.60, 2.64, 2.79, 2.80, 3.0, 3.08, 3, 10, 3.16, 3.41,
+             3.52, 3.60, 3.72, 3.95, 3.96, 4.0, 4.03, 4.20, 4.34, 4.40, 4.65, 4.74, 4.80, 4.84, 5.0, 5.28, 5.40, 5.53,
+             5.72, 6.0, 6.16, 6.32, 6.60, 7.11, 7.20, 7.80, 7.90, 8.0, 8.40, 8.69, 9.0, 9.48, 10.27, 11.0, 11.06, 11.85,
+             12.0, 13.0, 14.0, 15.0])
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_original_constraints)
+        # Reference: getNearestValue_sample2.py (https://gist.github.com/icchi-h/1d0bb1c52ebfdd31f14b3e811328390a)
+        idx = np.abs(np.asarray(self.feasible_vals) - x[0]).argmin()
+        x1 = self.feasible_vals[idx]
+        x2 = x[1]
+        x3 = x[2]
+
+        # First original objective function
+        f[0] = (29.4 * x1) + (0.6 * x2 * x3)
+
+        # Original constraint functions
+        g[0] = (x1 * x3) - 7.735 * ((x1 * x1) / x2) - 180.0
+        g[1] = 4.0 - (x3 / x2)
+        g = np.where(g < 0, -g, 0)
+        f[1] = g[0] + g[1]
+
+        return f
+
+
+class RE23():
+    def __init__(self):
+        self.problem_name = 'RE23'
+        self.n_objectives = 2
+        self.n_variables = 4
+        self.n_constraints = 0
+        self.n_original_constraints = 3
+
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound = np.zeros(self.n_variables)
+        self.lbound[0] = 1
+        self.lbound[1] = 1
+        self.lbound[2] = 10
+        self.lbound[3] = 10
+        self.ubound[0] = 100
+        self.ubound[1] = 100
+        self.ubound[2] = 200
+        self.ubound[3] = 240
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_original_constraints)
+
+        x1 = 0.0625 * int(np.round(x[0]))
+        x2 = 0.0625 * int(np.round(x[1]))
+        x3 = x[2]
+        x4 = x[3]
+
+        # First original objective function
+        f[0] = (0.6224 * x1 * x3 * x4) + (1.7781 * x2 * x3 * x3) + (3.1661 * x1 * x1 * x4) + (19.84 * x1 * x1 * x3)
+
+        # Original constraint functions
+        g[0] = x1 - (0.0193 * x3)
+        g[1] = x2 - (0.00954 * x3)
+        g[2] = (np.pi * x3 * x3 * x4) + ((4.0 / 3.0) * (np.pi * x3 * x3 * x3)) - 1296000
+        g = np.where(g < 0, -g, 0)
+        f[1] = g[0] + g[1] + g[2]
+
+        return f
+
+
+class RE24():
+    def __init__(self):
+        self.problem_name = 'RE24'
+        self.n_objectives = 2
+        self.n_variables = 2
+        self.n_constraints = 0
+        self.n_original_constraints = 4
+
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound = np.zeros(self.n_variables)
+        self.lbound[0] = 0.5
+        self.lbound[1] = 0.5
+        self.ubound[0] = 4
+        self.ubound[1] = 50
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_original_constraints)
+
+        x1 = x[0]
+        x2 = x[1]
+
+        # First original objective function
+        f[0] = x1 + (120 * x2)
+
+        E = 700000
+        sigma_b_max = 700
+        tau_max = 450
+        delta_max = 1.5
+        sigma_k = (E * x1 * x1) / 100
+        sigma_b = 4500 / (x1 * x2)
+        tau = 1800 / x2
+        delta = (56.2 * 10000) / (E * x1 * x2 * x2)
+
+        g[0] = 1 - (sigma_b / sigma_b_max)
+        g[1] = 1 - (tau / tau_max)
+        g[2] = 1 - (delta / delta_max)
+        g[3] = 1 - (sigma_b / sigma_k)
+        g = np.where(g < 0, -g, 0)
+        f[1] = g[0] + g[1] + g[2] + g[3]
+
+        return f
+
+
+class RE25():
+    def __init__(self):
+        self.problem_name = 'RE25'
+        self.n_objectives = 2
+        self.n_variables = 3
+        self.n_constraints = 0
+        self.n_original_constraints = 6
+
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound = np.zeros(self.n_variables)
+        self.lbound[0] = 1
+        self.lbound[1] = 0.6
+        self.lbound[2] = 0.09
+        self.ubound[0] = 70
+        self.ubound[1] = 3
+        self.ubound[2] = 0.5
+
+        self.feasible_vals = np.array(
+            [0.009, 0.0095, 0.0104, 0.0118, 0.0128, 0.0132, 0.014, 0.015, 0.0162, 0.0173, 0.018, 0.02, 0.023, 0.025,
+             0.028, 0.032, 0.035, 0.041, 0.047, 0.054, 0.063, 0.072, 0.08, 0.092, 0.105, 0.12, 0.135, 0.148, 0.162,
+             0.177, 0.192, 0.207, 0.225, 0.244, 0.263, 0.283, 0.307, 0.331, 0.362, 0.394, 0.4375, 0.5])
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_original_constraints)
+
+        x1 = np.round(x[0])
+        x2 = x[1]
+        # Reference: getNearestValue_sample2.py (https://gist.github.com/icchi-h/1d0bb1c52ebfdd31f14b3e811328390a)
+        idx = np.abs(np.asarray(self.feasible_vals) - x[2]).argmin()
+        x3 = self.feasible_vals[idx]
+
+        # first original objective function
+        f[0] = (np.pi * np.pi * x2 * x3 * x3 * (x1 + 2)) / 4.0
+
+        # constraint functions
+        Cf = ((4.0 * (x2 / x3) - 1) / (4.0 * (x2 / x3) - 4)) + (0.615 * x3 / x2)
+        Fmax = 1000.0
+        S = 189000.0
+        G = 11.5 * 1e+6
+        K = (G * x3 * x3 * x3 * x3) / (8 * x1 * x2 * x2 * x2)
+        lmax = 14.0
+        lf = (Fmax / K) + 1.05 * (x1 + 2) * x3
+        dmin = 0.2
+        Dmax = 3
+        Fp = 300.0
+        sigmaP = Fp / K
+        sigmaPM = 6
+        sigmaW = 1.25
+
+        g[0] = -((8 * Cf * Fmax * x2) / (np.pi * x3 * x3 * x3)) + S
+        g[1] = -lf + lmax
+        g[2] = -3 + (x2 / x3)
+        g[3] = -sigmaP + sigmaPM
+        g[4] = -sigmaP - ((Fmax - Fp) / K) - 1.05 * (x1 + 2) * x3 + lf
+        g[5] = sigmaW - ((Fmax - Fp) / K)
+
+        g = np.where(g < 0, -g, 0)
+        f[1] = g[0] + g[1] + g[2] + g[3] + g[4] + g[5]
+
+        return f
+
+
+class RE31():
+    def __init__(self):
+        self.problem_name = 'RE31'
+        self.n_objectives = 3
+        self.n_variables = 3
+        self.n_constraints = 0
+        self.n_original_constraints = 3
+
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound = np.zeros(self.n_variables)
+        self.lbound[0] = 0.00001
+        self.lbound[1] = 0.00001
+        self.lbound[2] = 1.0
+        self.ubound[0] = 100.0
+        self.ubound[1] = 100.0
+        self.ubound[2] = 3.0
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_original_constraints)
+
+        x1 = x[0]
+        x2 = x[1]
+        x3 = x[2]
+
+        # First original objective function
+        f[0] = x1 * np.sqrt(16.0 + (x3 * x3)) + x2 * np.sqrt(1.0 + x3 * x3)
+        # Second original objective function
+        f[1] = (20.0 * np.sqrt(16.0 + (x3 * x3))) / (x1 * x3)
+
+        # Constraint functions
+        g[0] = 0.1 - f[0]
+        g[1] = 100000.0 - f[1]
+        g[2] = 100000 - ((80.0 * np.sqrt(1.0 + x3 * x3)) / (x3 * x2))
+        g = np.where(g < 0, -g, 0)
+        f[2] = g[0] + g[1] + g[2]
+
+        return f
+
+
+class RE32():
+    def __init__(self):
+        self.problem_name = 'RE32'
+        self.n_objectives = 3
+        self.n_variables = 4
+        self.n_constraints = 0
+        self.n_original_constraints = 4
+
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound = np.zeros(self.n_variables)
+        self.lbound[0] = 0.125
+        self.lbound[1] = 0.1
+        self.lbound[2] = 0.1
+        self.lbound[3] = 0.125
+        self.ubound[0] = 5.0
+        self.ubound[1] = 10.0
+        self.ubound[2] = 10.0
+        self.ubound[3] = 5.0
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_original_constraints)
+
+        x1 = x[0]
+        x2 = x[1]
+        x3 = x[2]
+        x4 = x[3]
+
+        P = 6000
+        L = 14
+        E = 30 * 1e6
+
+        # // deltaMax = 0.25
+        G = 12 * 1e6
+        tauMax = 13600
+        sigmaMax = 30000
+
+        # First original objective function
+        f[0] = (1.10471 * x1 * x1 * x2) + (0.04811 * x3 * x4) * (14.0 + x2)
+        # Second original objective function
+        f[1] = (4 * P * L * L * L) / (E * x4 * x3 * x3 * x3)
+
+        # Constraint functions
+        M = P * (L + (x2 / 2))
+        tmpVar = ((x2 * x2) / 4.0) + np.power((x1 + x3) / 2.0, 2)
+        R = np.sqrt(tmpVar)
+        tmpVar = ((x2 * x2) / 12.0) + np.power((x1 + x3) / 2.0, 2)
+        J = 2 * np.sqrt(2) * x1 * x2 * tmpVar
+
+        tauDashDash = (M * R) / J
+        tauDash = P / (np.sqrt(2) * x1 * x2)
+        tmpVar = tauDash * tauDash + ((2 * tauDash * tauDashDash * x2) / (2 * R)) + (tauDashDash * tauDashDash)
+        tau = np.sqrt(tmpVar)
+        sigma = (6 * P * L) / (x4 * x3 * x3)
+        tmpVar = 4.013 * E * np.sqrt((x3 * x3 * x4 * x4 * x4 * x4 * x4 * x4) / 36.0) / (L * L)
+        tmpVar2 = (x3 / (2 * L)) * np.sqrt(E / (4 * G))
+        PC = tmpVar * (1 - tmpVar2)
+
+        g[0] = tauMax - tau
+        g[1] = sigmaMax - sigma
+        g[2] = x4 - x1
+        g[3] = PC - P
+        g = np.where(g < 0, -g, 0)
+        f[2] = g[0] + g[1] + g[2] + g[3]
+
+        return f
+
+
+class RE33():
+    def __init__(self):
+        self.problem_name = 'RE33'
+        self.n_objectives = 3
+        self.n_variables = 4
+        self.n_constraints = 0
+        self.n_original_constraints = 4
+
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound = np.zeros(self.n_variables)
+        self.lbound[0] = 55
+        self.lbound[1] = 75
+        self.lbound[2] = 1000
+        self.lbound[3] = 11
+        self.ubound[0] = 80
+        self.ubound[1] = 110
+        self.ubound[2] = 3000
+        self.ubound[3] = 20
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_original_constraints)
+
+        x1 = x[0]
+        x2 = x[1]
+        x3 = x[2]
+        x4 = x[3]
+
+        # First original objective function
+        f[0] = 4.9 * 1e-5 * (x2 * x2 - x1 * x1) * (x4 - 1.0)
+        # Second original objective function
+        f[1] = ((9.82 * 1e6) * (x2 * x2 - x1 * x1)) / (x3 * x4 * (x2 * x2 * x2 - x1 * x1 * x1))
+
+        # Reformulated objective functions
+        g[0] = (x2 - x1) - 20.0
+        g[1] = 0.4 - (x3 / (3.14 * (x2 * x2 - x1 * x1)))
+        g[2] = 1.0 - (2.22 * 1e-3 * x3 * (x2 * x2 * x2 - x1 * x1 * x1)) / np.power((x2 * x2 - x1 * x1), 2)
+        g[3] = (2.66 * 1e-2 * x3 * x4 * (x2 * x2 * x2 - x1 * x1 * x1)) / (x2 * x2 - x1 * x1) - 900.0
+        g = np.where(g < 0, -g, 0)
+        f[2] = g[0] + g[1] + g[2] + g[3]
+
+        return f
+
+
+class RE34():
+    def __init__(self):
+        self.problem_name = 'RE34'
+        self.n_objectives = 3
+        self.n_variables = 5
+        self.n_constraints = 0
+        self.n_original_constraints = 0
+
+        self.lbound = np.full(self.n_variables, 1)
+        self.ubound = np.full(self.n_variables, 3)
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_original_constraints)
+
+        x1 = x[0]
+        x2 = x[1]
+        x3 = x[2]
+        x4 = x[3]
+        x5 = x[4]
+
+        f[0] = 1640.2823 + (2.3573285 * x1) + (2.3220035 * x2) + (4.5688768 * x3) + (7.7213633 * x4) + (4.4559504 * x5)
+        f[1] = 6.5856 + (1.15 * x1) - (1.0427 * x2) + (0.9738 * x3) + (0.8364 * x4) - (0.3695 * x1 * x4) + (
+                    0.0861 * x1 * x5) + (0.3628 * x2 * x4) - (0.1106 * x1 * x1) - (0.3437 * x3 * x3) + (
+                           0.1764 * x4 * x4)
+        f[2] = -0.0551 + (0.0181 * x1) + (0.1024 * x2) + (0.0421 * x3) - (0.0073 * x1 * x2) + (0.024 * x2 * x3) - (
+                    0.0118 * x2 * x4) - (0.0204 * x3 * x4) - (0.008 * x3 * x5) - (0.0241 * x2 * x2) + (0.0109 * x4 * x4)
+
+        return f
+
+
+class RE35():
+    def __init__(self):
+        self.problem_name = 'RE35'
+        self.n_objectives = 3
+        self.n_variables = 7
+        self.n_constraints = 0
+        self.n_original_constraints = 11
+
+        self.lbound = np.zeros(self.n_variables)
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound[0] = 2.6
+        self.lbound[1] = 0.7
+        self.lbound[2] = 17
+        self.lbound[3] = 7.3
+        self.lbound[4] = 7.3
+        self.lbound[5] = 2.9
+        self.lbound[6] = 5.0
+        self.ubound[0] = 3.6
+        self.ubound[1] = 0.8
+        self.ubound[2] = 28
+        self.ubound[3] = 8.3
+        self.ubound[4] = 8.3
+        self.ubound[5] = 3.9
+        self.ubound[6] = 5.5
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_original_constraints)
+
+        x1 = x[0]
+        x2 = x[1]
+        x3 = np.round(x[2])
+        x4 = x[3]
+        x5 = x[4]
+        x6 = x[5]
+        x7 = x[6]
+
+        # First original objective function (weight)
+        f[0] = 0.7854 * x1 * (x2 * x2) * (((10.0 * x3 * x3) / 3.0) + (14.933 * x3) - 43.0934) - 1.508 * x1 * (
+                    x6 * x6 + x7 * x7) + 7.477 * (x6 * x6 * x6 + x7 * x7 * x7) + 0.7854 * (x4 * x6 * x6 + x5 * x7 * x7)
+
+        # Second original objective function (stress)
+        tmpVar = np.power((745.0 * x4) / (x2 * x3), 2.0) + 1.69 * 1e7
+        f[1] = np.sqrt(tmpVar) / (0.1 * x6 * x6 * x6)
+
+        # Constraint functions
+        g[0] = -(1.0 / (x1 * x2 * x2 * x3)) + 1.0 / 27.0
+        g[1] = -(1.0 / (x1 * x2 * x2 * x3 * x3)) + 1.0 / 397.5
+        g[2] = -(x4 * x4 * x4) / (x2 * x3 * x6 * x6 * x6 * x6) + 1.0 / 1.93
+        g[3] = -(x5 * x5 * x5) / (x2 * x3 * x7 * x7 * x7 * x7) + 1.0 / 1.93
+        g[4] = -(x2 * x3) + 40.0
+        g[5] = -(x1 / x2) + 12.0
+        g[6] = -5.0 + (x1 / x2)
+        g[7] = -1.9 + x4 - 1.5 * x6
+        g[8] = -1.9 + x5 - 1.1 * x7
+        g[9] = -f[1] + 1300.0
+        tmpVar = np.power((745.0 * x5) / (x2 * x3), 2.0) + 1.575 * 1e8
+        g[10] = -np.sqrt(tmpVar) / (0.1 * x7 * x7 * x7) + 1100.0
+        g = np.where(g < 0, -g, 0)
+        f[2] = g[0] + g[1] + g[2] + g[3] + g[4] + g[5] + g[6] + g[7] + g[8] + g[9] + g[10]
+
+        return f
+
+
+class RE36():
+    def __init__(self):
+        self.problem_name = 'RE36'
+        self.n_objectives = 3
+        self.n_variables = 4
+        self.n_constraints = 0
+        self.n_original_constraints = 1
+
+        self.lbound = np.full(self.n_variables, 12)
+        self.ubound = np.full(self.n_variables, 60)
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_original_constraints)
+
+        # all the four variables must be inverger values
+        x1 = np.round(x[0])
+        x2 = np.round(x[1])
+        x3 = np.round(x[2])
+        x4 = np.round(x[3])
+
+        # First original objective function
+        f[0] = np.abs(6.931 - ((x3 / x1) * (x4 / x2)))
+        # Second original objective function (the maximum value among the four variables)
+        l = [x1, x2, x3, x4]
+        f[1] = max(l)
+
+        g[0] = 0.5 - (f[0] / 6.931)
+        g = np.where(g < 0, -g, 0)
+        f[2] = g[0]
+
+        return f
+
+
+class RE37():
+    def __init__(self):
+        self.problem_name = 'RE37'
+        self.n_objectives = 3
+        self.n_variables = 4
+        self.n_constraints = 0
+        self.n_original_constraints = 0
+
+        self.lbound = np.full(self.n_variables, 0)
+        self.ubound = np.full(self.n_variables, 1)
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+
+        xAlpha = x[0]
+        xHA = x[1]
+        xOA = x[2]
+        xOPTT = x[3]
+
+        # f1 (TF_max)
+        f[0] = 0.692 + (0.477 * xAlpha) - (0.687 * xHA) - (0.080 * xOA) - (0.0650 * xOPTT) - (
+                    0.167 * xAlpha * xAlpha) - (0.0129 * xHA * xAlpha) + (0.0796 * xHA * xHA) - (
+                           0.0634 * xOA * xAlpha) - (0.0257 * xOA * xHA) + (0.0877 * xOA * xOA) - (
+                           0.0521 * xOPTT * xAlpha) + (0.00156 * xOPTT * xHA) + (0.00198 * xOPTT * xOA) + (
+                           0.0184 * xOPTT * xOPTT)
+        # f2 (X_cc)
+        f[1] = 0.153 - (0.322 * xAlpha) + (0.396 * xHA) + (0.424 * xOA) + (0.0226 * xOPTT) + (
+                    0.175 * xAlpha * xAlpha) + (0.0185 * xHA * xAlpha) - (0.0701 * xHA * xHA) - (
+                           0.251 * xOA * xAlpha) + (0.179 * xOA * xHA) + (0.0150 * xOA * xOA) + (
+                           0.0134 * xOPTT * xAlpha) + (0.0296 * xOPTT * xHA) + (0.0752 * xOPTT * xOA) + (
+                           0.0192 * xOPTT * xOPTT)
+        # f3 (TT_max)
+        f[2] = 0.370 - (0.205 * xAlpha) + (0.0307 * xHA) + (0.108 * xOA) + (1.019 * xOPTT) - (
+                    0.135 * xAlpha * xAlpha) + (0.0141 * xHA * xAlpha) + (0.0998 * xHA * xHA) + (
+                           0.208 * xOA * xAlpha) - (0.0301 * xOA * xHA) - (0.226 * xOA * xOA) + (
+                           0.353 * xOPTT * xAlpha) - (0.0497 * xOPTT * xOA) - (0.423 * xOPTT * xOPTT) + (
+                           0.202 * xHA * xAlpha * xAlpha) - (0.281 * xOA * xAlpha * xAlpha) - (
+                           0.342 * xHA * xHA * xAlpha) - (0.245 * xHA * xHA * xOA) + (0.281 * xOA * xOA * xHA) - (
+                           0.184 * xOPTT * xOPTT * xAlpha) - (0.281 * xHA * xAlpha * xOA)
+
+        return f
+
+
+class RE41():
+    def __init__(self):
+        self.problem_name = 'RE41'
+        self.n_objectives = 4
+        self.n_variables = 7
+        self.n_constraints = 0
+        self.n_original_constraints = 10
+
+        self.lbound = np.zeros(self.n_variables)
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound[0] = 0.5
+        self.lbound[1] = 0.45
+        self.lbound[2] = 0.5
+        self.lbound[3] = 0.5
+        self.lbound[4] = 0.875
+        self.lbound[5] = 0.4
+        self.lbound[6] = 0.4
+        self.ubound[0] = 1.5
+        self.ubound[1] = 1.35
+        self.ubound[2] = 1.5
+        self.ubound[3] = 1.5
+        self.ubound[4] = 2.625
+        self.ubound[5] = 1.2
+        self.ubound[6] = 1.2
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_original_constraints)
+
+        x1 = x[0]
+        x2 = x[1]
+        x3 = x[2]
+        x4 = x[3]
+        x5 = x[4]
+        x6 = x[5]
+        x7 = x[6]
+
+        # First original objective function
+        f[0] = 1.98 + 4.9 * x1 + 6.67 * x2 + 6.98 * x3 + 4.01 * x4 + 1.78 * x5 + 0.00001 * x6 + 2.73 * x7
+        # Second original objective function
+        f[1] = 4.72 - 0.5 * x4 - 0.19 * x2 * x3
+        # Third original objective function
+        Vmbp = 10.58 - 0.674 * x1 * x2 - 0.67275 * x2
+        Vfd = 16.45 - 0.489 * x3 * x7 - 0.843 * x5 * x6
+        f[2] = 0.5 * (Vmbp + Vfd)
+
+        # Constraint functions
+        g[0] = 1 - (1.16 - 0.3717 * x2 * x4 - 0.0092928 * x3)
+        g[1] = 0.32 - (0.261 - 0.0159 * x1 * x2 - 0.06486 * x1 - 0.019 * x2 * x7 + 0.0144 * x3 * x5 + 0.0154464 * x6)
+        g[2] = 0.32 - (
+                    0.214 + 0.00817 * x5 - 0.045195 * x1 - 0.0135168 * x1 + 0.03099 * x2 * x6 - 0.018 * x2 * x7 + 0.007176 * x3 + 0.023232 * x3 - 0.00364 * x5 * x6 - 0.018 * x2 * x2)
+        g[3] = 0.32 - (0.74 - 0.61 * x2 - 0.031296 * x3 - 0.031872 * x7 + 0.227 * x2 * x2)
+        g[4] = 32 - (28.98 + 3.818 * x3 - 4.2 * x1 * x2 + 1.27296 * x6 - 2.68065 * x7)
+        g[5] = 32 - (33.86 + 2.95 * x3 - 5.057 * x1 * x2 - 3.795 * x2 - 3.4431 * x7 + 1.45728)
+        g[6] = 32 - (46.36 - 9.9 * x2 - 4.4505 * x1)
+        g[7] = 4 - f[1]
+        g[8] = 9.9 - Vmbp
+        g[9] = 15.7 - Vfd
+
+        g = np.where(g < 0, -g, 0)
+        f[3] = g[0] + g[1] + g[2] + g[3] + g[4] + g[5] + g[6] + g[7] + g[8] + g[9]
+
+        return f
+
+
+class RE42():
+    def __init__(self):
+        self.problem_name = 'RE42'
+        self.n_objectives = 4
+        self.n_variables = 6
+        self.n_constraints = 0
+        self.n_original_constraints = 9
+
+        self.lbound = np.zeros(self.n_variables)
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound[0] = 150.0
+        self.lbound[1] = 20.0
+        self.lbound[2] = 13.0
+        self.lbound[3] = 10.0
+        self.lbound[4] = 14.0
+        self.lbound[5] = 0.63
+        self.ubound[0] = 274.32
+        self.ubound[1] = 32.31
+        self.ubound[2] = 25.0
+        self.ubound[3] = 11.71
+        self.ubound[4] = 18.0
+        self.ubound[5] = 0.75
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        # NOT g
+        constraintFuncs = np.zeros(self.n_original_constraints)
+
+        x_L = x[0]
+        x_B = x[1]
+        x_D = x[2]
+        x_T = x[3]
+        x_Vk = x[4]
+        x_CB = x[5]
+
+        displacement = 1.025 * x_L * x_B * x_T * x_CB
+        V = 0.5144 * x_Vk
+        g = 9.8065
+        Fn = V / np.power(g * x_L, 0.5)
+        a = (4977.06 * x_CB * x_CB) - (8105.61 * x_CB) + 4456.51
+        b = (-10847.2 * x_CB * x_CB) + (12817.0 * x_CB) - 6960.32
+
+        power = (np.power(displacement, 2.0 / 3.0) * np.power(x_Vk, 3.0)) / (a + (b * Fn))
+        outfit_weight = 1.0 * np.power(x_L, 0.8) * np.power(x_B, 0.6) * np.power(x_D, 0.3) * np.power(x_CB, 0.1)
+        steel_weight = 0.034 * np.power(x_L, 1.7) * np.power(x_B, 0.7) * np.power(x_D, 0.4) * np.power(x_CB, 0.5)
+        machinery_weight = 0.17 * np.power(power, 0.9)
+        light_ship_weight = steel_weight + outfit_weight + machinery_weight
+
+        ship_cost = 1.3 * ((2000.0 * np.power(steel_weight, 0.85)) + (3500.0 * outfit_weight) + (
+                    2400.0 * np.power(power, 0.8)))
+        capital_costs = 0.2 * ship_cost
+
+        DWT = displacement - light_ship_weight
+
+        running_costs = 40000.0 * np.power(DWT, 0.3)
+
+        round_trip_miles = 5000.0
+        sea_days = (round_trip_miles / 24.0) * x_Vk
+        handling_rate = 8000.0
+
+        daily_consumption = ((0.19 * power * 24.0) / 1000.0) + 0.2
+        fuel_price = 100.0
+        fuel_cost = 1.05 * daily_consumption * sea_days * fuel_price
+        port_cost = 6.3 * np.power(DWT, 0.8)
+
+        fuel_carried = daily_consumption * (sea_days + 5.0)
+        miscellaneous_DWT = 2.0 * np.power(DWT, 0.5)
+
+        cargo_DWT = DWT - fuel_carried - miscellaneous_DWT
+        port_days = 2.0 * ((cargo_DWT / handling_rate) + 0.5)
+        RTPA = 350.0 / (sea_days + port_days)
+
+        voyage_costs = (fuel_cost + port_cost) * RTPA
+        annual_costs = capital_costs + running_costs + voyage_costs
+        annual_cargo = cargo_DWT * RTPA
+
+        f[0] = annual_costs / annual_cargo
+        f[1] = light_ship_weight
+        # f_2 is dealt as a minimization problem
+        f[2] = -annual_cargo
+
+        # Reformulated objective functions
+        constraintFuncs[0] = (x_L / x_B) - 6.0
+        constraintFuncs[1] = -(x_L / x_D) + 15.0
+        constraintFuncs[2] = -(x_L / x_T) + 19.0
+        constraintFuncs[3] = 0.45 * np.power(DWT, 0.31) - x_T
+        constraintFuncs[4] = 0.7 * x_D + 0.7 - x_T
+        constraintFuncs[5] = 500000.0 - DWT
+        constraintFuncs[6] = DWT - 3000.0
+        constraintFuncs[7] = 0.32 - Fn
+
+        KB = 0.53 * x_T
+        BMT = ((0.085 * x_CB - 0.002) * x_B * x_B) / (x_T * x_CB)
+        KG = 1.0 + 0.52 * x_D
+        constraintFuncs[8] = (KB + BMT - KG) - (0.07 * x_B)
+
+        constraintFuncs = np.where(constraintFuncs < 0, -constraintFuncs, 0)
+        f[3] = constraintFuncs[0] + constraintFuncs[1] + constraintFuncs[2] + constraintFuncs[3] + constraintFuncs[4] + \
+               constraintFuncs[5] + constraintFuncs[6] + constraintFuncs[7] + constraintFuncs[8]
+
+        return f
+
+
+class RE61():
+    def __init__(self):
+        self.problem_name = 'RE61'
+        self.n_objectives = 6
+        self.n_variables = 3
+        self.n_constraints = 0
+        self.n_original_constraints = 7
+
+        self.lbound = np.zeros(self.n_variables)
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound[0] = 0.01
+        self.lbound[1] = 0.01
+        self.lbound[2] = 0.01
+        self.ubound[0] = 0.45
+        self.ubound[1] = 0.10
+        self.ubound[2] = 0.10
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_original_constraints)
+
+        # First original objective function
+        f[0] = 106780.37 * (x[1] + x[2]) + 61704.67
+        # Second original objective function
+        f[1] = 3000 * x[0]
+        # Third original objective function
+        f[2] = 305700 * 2289 * x[1] / np.power(0.06 * 2289, 0.65)
+        # Fourth original objective function
+        f[3] = 250 * 2289 * np.exp(-39.75 * x[1] + 9.9 * x[2] + 2.74)
+        # Fifth original objective function
+        f[4] = 25 * (1.39 / (x[0] * x[1]) + 4940 * x[2] - 80)
+
+        # Constraint functions
+        g[0] = 1 - (0.00139 / (x[0] * x[1]) + 4.94 * x[2] - 0.08)
+        g[1] = 1 - (0.000306 / (x[0] * x[1]) + 1.082 * x[2] - 0.0986)
+        g[2] = 50000 - (12.307 / (x[0] * x[1]) + 49408.24 * x[2] + 4051.02)
+        g[3] = 16000 - (2.098 / (x[0] * x[1]) + 8046.33 * x[2] - 696.71)
+        g[4] = 10000 - (2.138 / (x[0] * x[1]) + 7883.39 * x[2] - 705.04)
+        g[5] = 2000 - (0.417 * x[0] * x[1] + 1721.26 * x[2] - 136.54)
+        g[6] = 550 - (0.164 / (x[0] * x[1]) + 631.13 * x[2] - 54.48)
+
+        g = np.where(g < 0, -g, 0)
+        f[5] = g[0] + g[1] + g[2] + g[3] + g[4] + g[5] + g[6]
+
+        return f
+
+
+class RE91():
+    def __init__(self):
+        self.problem_name = 'RE91'
+        self.n_objectives = 9
+        self.n_variables = 7
+        self.n_constraints = 0
+        self.n_original_constraints = 0
+
+        self.lbound = np.zeros(self.n_variables)
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound[0] = 0.5
+        self.lbound[1] = 0.45
+        self.lbound[2] = 0.5
+        self.lbound[3] = 0.5
+        self.lbound[4] = 0.875
+        self.lbound[5] = 0.4
+        self.lbound[6] = 0.4
+        self.ubound[0] = 1.5
+        self.ubound[1] = 1.35
+        self.ubound[2] = 1.5
+        self.ubound[3] = 1.5
+        self.ubound[4] = 2.625
+        self.ubound[5] = 1.2
+        self.ubound[6] = 1.2
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_original_constraints)
+
+        x1 = x[0]
+        x2 = x[1]
+        x3 = x[2]
+        x4 = x[3]
+        x5 = x[4]
+        x6 = x[5]
+        x7 = x[6]
+        # stochastic variables
+        x8 = 0.006 * (np.random.normal(0, 1)) + 0.345
+        x9 = 0.006 * (np.random.normal(0, 1)) + 0.192
+        x10 = 10 * (np.random.normal(0, 1)) + 0.0
+        x11 = 10 * (np.random.normal(0, 1)) + 0.0
+
+        # First function
+        f[0] = 1.98 + 4.9 * x1 + 6.67 * x2 + 6.98 * x3 + 4.01 * x4 + 1.75 * x5 + 0.00001 * x6 + 2.73 * x7
+        # Second function
+        f[1] = max(0.0, (1.16 - 0.3717 * x2 * x4 - 0.00931 * x2 * x10 - 0.484 * x3 * x9 + 0.01343 * x6 * x10) / 1.0)
+        # Third function
+        f[2] = max(0.0, (
+                    0.261 - 0.0159 * x1 * x2 - 0.188 * x1 * x8 - 0.019 * x2 * x7 + 0.0144 * x3 * x5 + 0.87570001 * x5 * x10 + 0.08045 * x6 * x9 + 0.00139 * x8 * x11 + 0.00001575 * x10 * x11) / 0.32)
+        # Fourth function
+        f[3] = max(0.0, (
+                    0.214 + 0.00817 * x5 - 0.131 * x1 * x8 - 0.0704 * x1 * x9 + 0.03099 * x2 * x6 - 0.018 * x2 * x7 + 0.0208 * x3 * x8 + 0.121 * x3 * x9 - 0.00364 * x5 * x6 + 0.0007715 * x5 * x10 - 0.0005354 * x6 * x10 + 0.00121 * x8 * x11 + 0.00184 * x9 * x10 - 0.018 * x2 * x2) / 0.32)
+        # Fifth function
+        f[4] = max(0.0, (
+                    0.74 - 0.61 * x2 - 0.163 * x3 * x8 + 0.001232 * x3 * x10 - 0.166 * x7 * x9 + 0.227 * x2 * x2) / 0.32)
+        # Sixth function
+        tmp = ((
+                           28.98 + 3.818 * x3 - 4.2 * x1 * x2 + 0.0207 * x5 * x10 + 6.63 * x6 * x9 - 7.77 * x7 * x8 + 0.32 * x9 * x10) + (
+                           33.86 + 2.95 * x3 + 0.1792 * x10 - 5.057 * x1 * x2 - 11 * x2 * x8 - 0.0215 * x5 * x10 - 9.98 * x7 * x8 + 22 * x8 * x9) + (
+                           46.36 - 9.9 * x2 - 12.9 * x1 * x8 + 0.1107 * x3 * x10)) / 3
+        f[5] = max(0.0, tmp / 32)
+        # Seventh function
+        f[6] = max(0.0, (
+                    4.72 - 0.5 * x4 - 0.19 * x2 * x3 - 0.0122 * x4 * x10 + 0.009325 * x6 * x10 + 0.000191 * x11 * x11) / 4.0)
+        # EighthEighth function
+        f[7] = max(0.0, (
+                    10.58 - 0.674 * x1 * x2 - 1.95 * x2 * x8 + 0.02054 * x3 * x10 - 0.0198 * x4 * x10 + 0.028 * x6 * x10) / 9.9)
+        # Ninth function
+        f[8] = max(0.0, (
+                    16.45 - 0.489 * x3 * x7 - 0.843 * x5 * x6 + 0.0432 * x9 * x10 - 0.0556 * x9 * x11 - 0.000786 * x11 * x11) / 15.7)
+
+        return f
+
+
+class CRE21():
+    def __init__(self):
+        self.problem_name = 'CRE21'
+        self.n_objectives = 2
+        self.n_variables = 3
+        self.n_constraints = 3
+
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound = np.zeros(self.n_variables)
+        self.lbound[0] = 0.00001
+        self.lbound[1] = 0.00001
+        self.lbound[2] = 1.0
+        self.ubound[0] = 100.0
+        self.ubound[1] = 100.0
+        self.ubound[2] = 3.0
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_constraints)
+
+        x1 = x[0]
+        x2 = x[1]
+        x3 = x[2]
+
+        # First original objective function
+        f[0] = x1 * np.sqrt(16.0 + (x3 * x3)) + x2 * np.sqrt(1.0 + x3 * x3)
+        # Second original objective function
+        f[1] = (20.0 * np.sqrt(16.0 + (x3 * x3))) / (x1 * x3)
+
+        # Constraint functions
+        g[0] = 0.1 - f[0]
+        g[1] = 100000.0 - f[1]
+        g[2] = 100000 - ((80.0 * np.sqrt(1.0 + x3 * x3)) / (x3 * x2))
+        g = np.where(g < 0, -g, 0)
+
+        return f, g
+
+
+class CRE22():
+    def __init__(self):
+        self.problem_name = 'CRE22'
+        self.n_objectives = 2
+        self.n_variables = 4
+        self.n_constraints = 4
+
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound = np.zeros(self.n_variables)
+        self.lbound[0] = 0.125
+        self.lbound[1] = 0.1
+        self.lbound[2] = 0.1
+        self.lbound[3] = 0.125
+        self.ubound[0] = 5.0
+        self.ubound[1] = 10.0
+        self.ubound[2] = 10.0
+        self.ubound[3] = 5.0
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_constraints)
+
+        x1 = x[0]
+        x2 = x[1]
+        x3 = x[2]
+        x4 = x[3]
+
+        P = 6000
+        L = 14
+        E = 30 * 1e6
+
+        # // deltaMax = 0.25
+        G = 12 * 1e6
+        tauMax = 13600
+        sigmaMax = 30000
+
+        # First original objective function
+        f[0] = (1.10471 * x1 * x1 * x2) + (0.04811 * x3 * x4) * (14.0 + x2)
+        # Second original objective function
+        f[1] = (4 * P * L * L * L) / (E * x4 * x3 * x3 * x3)
+
+        # Constraint functions
+        M = P * (L + (x2 / 2))
+        tmpVar = ((x2 * x2) / 4.0) + np.power((x1 + x3) / 2.0, 2)
+        R = np.sqrt(tmpVar)
+        tmpVar = ((x2 * x2) / 12.0) + np.power((x1 + x3) / 2.0, 2)
+        J = 2 * np.sqrt(2) * x1 * x2 * tmpVar
+
+        tauDashDash = (M * R) / J
+        tauDash = P / (np.sqrt(2) * x1 * x2)
+        tmpVar = tauDash * tauDash + ((2 * tauDash * tauDashDash * x2) / (2 * R)) + (tauDashDash * tauDashDash)
+        tau = np.sqrt(tmpVar)
+        sigma = (6 * P * L) / (x4 * x3 * x3)
+        tmpVar = 4.013 * E * np.sqrt((x3 * x3 * x4 * x4 * x4 * x4 * x4 * x4) / 36.0) / (L * L)
+        tmpVar2 = (x3 / (2 * L)) * np.sqrt(E / (4 * G))
+        PC = tmpVar * (1 - tmpVar2)
+
+        g[0] = tauMax - tau
+        g[1] = sigmaMax - sigma
+        g[2] = x4 - x1
+        g[3] = PC - P
+        g = np.where(g < 0, -g, 0)
+
+        return f, g
+
+
+class CRE23():
+    def __init__(self):
+        self.problem_name = 'CRE23'
+        self.n_objectives = 2
+        self.n_variables = 4
+        self.n_constraints = 4
+
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound = np.zeros(self.n_variables)
+        self.lbound[0] = 55
+        self.lbound[1] = 75
+        self.lbound[2] = 1000
+        self.lbound[3] = 11
+        self.ubound[0] = 80
+        self.ubound[1] = 110
+        self.ubound[2] = 3000
+        self.ubound[3] = 20
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_constraints)
+
+        x1 = x[0]
+        x2 = x[1]
+        x3 = x[2]
+        x4 = x[3]
+
+        # First original objective function
+        f[0] = 4.9 * 1e-5 * (x2 * x2 - x1 * x1) * (x4 - 1.0)
+        # Second original objective function
+        f[1] = ((9.82 * 1e6) * (x2 * x2 - x1 * x1)) / (x3 * x4 * (x2 * x2 * x2 - x1 * x1 * x1))
+
+        # Reformulated objective functions
+        g[0] = (x2 - x1) - 20.0
+        g[1] = 0.4 - (x3 / (3.14 * (x2 * x2 - x1 * x1)))
+        g[2] = 1.0 - (2.22 * 1e-3 * x3 * (x2 * x2 * x2 - x1 * x1 * x1)) / np.power((x2 * x2 - x1 * x1), 2)
+        g[3] = (2.66 * 1e-2 * x3 * x4 * (x2 * x2 * x2 - x1 * x1 * x1)) / (x2 * x2 - x1 * x1) - 900.0
+        g = np.where(g < 0, -g, 0)
+
+        return f, g
+
+
+class CRE24():
+    def __init__(self):
+        self.problem_name = 'CRE24'
+        self.n_objectives = 2
+        self.n_variables = 7
+        self.n_constraints = 11
+
+        self.lbound = np.zeros(self.n_variables)
+        self.ubound = np.zeros(self.n_variables)
+
+        self.lbound[0] = 2.6
+        self.lbound[1] = 0.7
+        self.lbound[2] = 17
+        self.lbound[3] = 7.3
+        self.lbound[4] = 7.3
+        self.lbound[5] = 2.9
+        self.lbound[6] = 5.0
+        self.ubound[0] = 3.6
+        self.ubound[1] = 0.8
+        self.ubound[2] = 28
+        self.ubound[3] = 8.3
+        self.ubound[4] = 8.3
+        self.ubound[5] = 3.9
+        self.ubound[6] = 5.5
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_constraints)
+
+        x1 = x[0]
+        x2 = x[1]
+        x3 = np.round(x[2])
+        x4 = x[3]
+        x5 = x[4]
+        x6 = x[5]
+        x7 = x[6]
+
+        # First original objective function (weight)
+        f[0] = 0.7854 * x1 * (x2 * x2) * (((10.0 * x3 * x3) / 3.0) + (14.933 * x3) - 43.0934) - 1.508 * x1 * (
+                    x6 * x6 + x7 * x7) + 7.477 * (x6 * x6 * x6 + x7 * x7 * x7) + 0.7854 * (x4 * x6 * x6 + x5 * x7 * x7)
+
+        # Second original objective function (stress)
+        tmpVar = np.power((745.0 * x4) / (x2 * x3), 2.0) + 1.69 * 1e7
+        f[1] = np.sqrt(tmpVar) / (0.1 * x6 * x6 * x6)
+
+        # Constraint functions
+        g[0] = -(1.0 / (x1 * x2 * x2 * x3)) + 1.0 / 27.0
+        g[1] = -(1.0 / (x1 * x2 * x2 * x3 * x3)) + 1.0 / 397.5
+        g[2] = -(x4 * x4 * x4) / (x2 * x3 * x6 * x6 * x6 * x6) + 1.0 / 1.93
+        g[3] = -(x5 * x5 * x5) / (x2 * x3 * x7 * x7 * x7 * x7) + 1.0 / 1.93
+        g[4] = -(x2 * x3) + 40.0
+        g[5] = -(x1 / x2) + 12.0
+        g[6] = -5.0 + (x1 / x2)
+        g[7] = -1.9 + x4 - 1.5 * x6
+        g[8] = -1.9 + x5 - 1.1 * x7
+        g[9] = -f[1] + 1300.0
+        tmpVar = np.power((745.0 * x5) / (x2 * x3), 2.0) + 1.575 * 1e8
+        g[10] = -np.sqrt(tmpVar) / (0.1 * x7 * x7 * x7) + 1100.0
+        g = np.where(g < 0, -g, 0)
+
+        return f, g
+
+
+class CRE25():
+    def __init__(self):
+        self.problem_name = 'CRE25'
+        self.n_objectives = 2
+        self.n_variables = 4
+        self.n_constraints = 1
+
+        self.lbound = np.full(self.n_variables, 12)
+        self.ubound = np.full(self.n_variables, 60)
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_constraints)
+
+        # all the four variables must be inverger values
+        x1 = np.round(x[0])
+        x2 = np.round(x[1])
+        x3 = np.round(x[2])
+        x4 = np.round(x[3])
+
+        # First original objective function
+        f[0] = np.abs(6.931 - ((x3 / x1) * (x4 / x2)))
+        # Second original objective function (the maximum value among the four variables)
+        l = [x1, x2, x3, x4]
+        f[1] = max(l)
+
+        g[0] = 0.5 - (f[0] / 6.931)
+        g = np.where(g < 0, -g, 0)
+
+        return f, g
+
+
+class CRE31():
+    def __init__(self):
+        self.problem_name = 'CRE31'
+        self.n_objectives = 3
+        self.n_variables = 7
+        self.n_constraints = 10
+
+        self.lbound = np.zeros(self.n_variables)
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound[0] = 0.5
+        self.lbound[1] = 0.45
+        self.lbound[2] = 0.5
+        self.lbound[3] = 0.5
+        self.lbound[4] = 0.875
+        self.lbound[5] = 0.4
+        self.lbound[6] = 0.4
+        self.ubound[0] = 1.5
+        self.ubound[1] = 1.35
+        self.ubound[2] = 1.5
+        self.ubound[3] = 1.5
+        self.ubound[4] = 2.625
+        self.ubound[5] = 1.2
+        self.ubound[6] = 1.2
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_constraints)
+
+        x1 = x[0]
+        x2 = x[1]
+        x3 = x[2]
+        x4 = x[3]
+        x5 = x[4]
+        x6 = x[5]
+        x7 = x[6]
+
+        # First original objective function
+        f[0] = 1.98 + 4.9 * x1 + 6.67 * x2 + 6.98 * x3 + 4.01 * x4 + 1.78 * x5 + 0.00001 * x6 + 2.73 * x7
+        # Second original objective function
+        f[1] = 4.72 - 0.5 * x4 - 0.19 * x2 * x3
+        # Third original objective function
+        Vmbp = 10.58 - 0.674 * x1 * x2 - 0.67275 * x2
+        Vfd = 16.45 - 0.489 * x3 * x7 - 0.843 * x5 * x6
+        f[2] = 0.5 * (Vmbp + Vfd)
+
+        # Constraint functions
+        g[0] = 1 - (1.16 - 0.3717 * x2 * x4 - 0.0092928 * x3)
+        g[1] = 0.32 - (0.261 - 0.0159 * x1 * x2 - 0.06486 * x1 - 0.019 * x2 * x7 + 0.0144 * x3 * x5 + 0.0154464 * x6)
+        g[2] = 0.32 - (
+                    0.214 + 0.00817 * x5 - 0.045195 * x1 - 0.0135168 * x1 + 0.03099 * x2 * x6 - 0.018 * x2 * x7 + 0.007176 * x3 + 0.023232 * x3 - 0.00364 * x5 * x6 - 0.018 * x2 * x2)
+        g[3] = 0.32 - (0.74 - 0.61 * x2 - 0.031296 * x3 - 0.031872 * x7 + 0.227 * x2 * x2)
+        g[4] = 32 - (28.98 + 3.818 * x3 - 4.2 * x1 * x2 + 1.27296 * x6 - 2.68065 * x7)
+        g[5] = 32 - (33.86 + 2.95 * x3 - 5.057 * x1 * x2 - 3.795 * x2 - 3.4431 * x7 + 1.45728)
+        g[6] = 32 - (46.36 - 9.9 * x2 - 4.4505 * x1)
+        g[7] = 4 - f[1]
+        g[8] = 9.9 - Vmbp
+        g[9] = 15.7 - Vfd
+        g = np.where(g < 0, -g, 0)
+
+        return f, g
+
+
+class CRE32():
+    def __init__(self):
+        self.problem_name = 'CRE32'
+        self.n_objectives = 3
+        self.n_variables = 6
+        self.n_constraints = 9
+
+        self.lbound = np.zeros(self.n_variables)
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound[0] = 150.0
+        self.lbound[1] = 20.0
+        self.lbound[2] = 13.0
+        self.lbound[3] = 10.0
+        self.lbound[4] = 14.0
+        self.lbound[5] = 0.63
+        self.ubound[0] = 274.32
+        self.ubound[1] = 32.31
+        self.ubound[2] = 25.0
+        self.ubound[3] = 11.71
+        self.ubound[4] = 18.0
+        self.ubound[5] = 0.75
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        # NOT g
+        constraintFuncs = np.zeros(self.n_constraints)
+
+        x_L = x[0]
+        x_B = x[1]
+        x_D = x[2]
+        x_T = x[3]
+        x_Vk = x[4]
+        x_CB = x[5]
+
+        displacement = 1.025 * x_L * x_B * x_T * x_CB
+        V = 0.5144 * x_Vk
+        g = 9.8065
+        Fn = V / np.power(g * x_L, 0.5)
+        a = (4977.06 * x_CB * x_CB) - (8105.61 * x_CB) + 4456.51
+        b = (-10847.2 * x_CB * x_CB) + (12817.0 * x_CB) - 6960.32
+
+        power = (np.power(displacement, 2.0 / 3.0) * np.power(x_Vk, 3.0)) / (a + (b * Fn))
+        outfit_weight = 1.0 * np.power(x_L, 0.8) * np.power(x_B, 0.6) * np.power(x_D, 0.3) * np.power(x_CB, 0.1)
+        steel_weight = 0.034 * np.power(x_L, 1.7) * np.power(x_B, 0.7) * np.power(x_D, 0.4) * np.power(x_CB, 0.5)
+        machinery_weight = 0.17 * np.power(power, 0.9)
+        light_ship_weight = steel_weight + outfit_weight + machinery_weight
+
+        ship_cost = 1.3 * ((2000.0 * np.power(steel_weight, 0.85)) + (3500.0 * outfit_weight) + (
+                    2400.0 * np.power(power, 0.8)))
+        capital_costs = 0.2 * ship_cost
+
+        DWT = displacement - light_ship_weight
+
+        running_costs = 40000.0 * np.power(DWT, 0.3)
+
+        round_trip_miles = 5000.0
+        sea_days = (round_trip_miles / 24.0) * x_Vk
+        handling_rate = 8000.0
+
+        daily_consumption = ((0.19 * power * 24.0) / 1000.0) + 0.2
+        fuel_price = 100.0
+        fuel_cost = 1.05 * daily_consumption * sea_days * fuel_price
+        port_cost = 6.3 * np.power(DWT, 0.8)
+
+        fuel_carried = daily_consumption * (sea_days + 5.0)
+        miscellaneous_DWT = 2.0 * np.power(DWT, 0.5)
+
+        cargo_DWT = DWT - fuel_carried - miscellaneous_DWT
+        port_days = 2.0 * ((cargo_DWT / handling_rate) + 0.5)
+        RTPA = 350.0 / (sea_days + port_days)
+
+        voyage_costs = (fuel_cost + port_cost) * RTPA
+        annual_costs = capital_costs + running_costs + voyage_costs
+        annual_cargo = cargo_DWT * RTPA
+
+        f[0] = annual_costs / annual_cargo
+        f[1] = light_ship_weight
+        # f_2 is dealt as a minimization problem
+        f[2] = -annual_cargo
+
+        # Reformulated objective functions
+        constraintFuncs[0] = (x_L / x_B) - 6.0
+        constraintFuncs[1] = -(x_L / x_D) + 15.0
+        constraintFuncs[2] = -(x_L / x_T) + 19.0
+        constraintFuncs[3] = 0.45 * np.power(DWT, 0.31) - x_T
+        constraintFuncs[4] = 0.7 * x_D + 0.7 - x_T
+        constraintFuncs[5] = 500000.0 - DWT
+        constraintFuncs[6] = DWT - 3000.0
+        constraintFuncs[7] = 0.32 - Fn
+
+        KB = 0.53 * x_T
+        BMT = ((0.085 * x_CB - 0.002) * x_B * x_B) / (x_T * x_CB)
+        KG = 1.0 + 0.52 * x_D
+        constraintFuncs[8] = (KB + BMT - KG) - (0.07 * x_B)
+        constraintFuncs = np.where(constraintFuncs < 0, -constraintFuncs, 0)
+
+        return f, constraintFuncs
+
+
+class CRE51():
+    def __init__(self):
+        self.problem_name = 'CRE51'
+        self.n_objectives = 5
+        self.n_variables = 3
+        self.n_constraints = 7
+
+        self.lbound = np.zeros(self.n_variables)
+        self.ubound = np.zeros(self.n_variables)
+        self.lbound[0] = 0.01
+        self.lbound[1] = 0.01
+        self.lbound[2] = 0.01
+        self.ubound[0] = 0.45
+        self.ubound[1] = 0.10
+        self.ubound[2] = 0.10
+
+    def evaluate(self, x):
+        f = np.zeros(self.n_objectives)
+        g = np.zeros(self.n_constraints)
+
+        # First original objective function
+        f[0] = 106780.37 * (x[1] + x[2]) + 61704.67
+        # Second original objective function
+        f[1] = 3000 * x[0]
+        # Third original objective function
+        f[2] = 305700 * 2289 * x[1] / np.power(0.06 * 2289, 0.65)
+        # Fourth original objective function
+        f[3] = 250 * 2289 * np.exp(-39.75 * x[1] + 9.9 * x[2] + 2.74)
+        # Fifth original objective function
+        f[4] = 25 * (1.39 / (x[0] * x[1]) + 4940 * x[2] - 80)
+
+        # Constraint functions
+        g[0] = 1 - (0.00139 / (x[0] * x[1]) + 4.94 * x[2] - 0.08)
+        g[1] = 1 - (0.000306 / (x[0] * x[1]) + 1.082 * x[2] - 0.0986)
+        g[2] = 50000 - (12.307 / (x[0] * x[1]) + 49408.24 * x[2] + 4051.02)
+        g[3] = 16000 - (2.098 / (x[0] * x[1]) + 8046.33 * x[2] - 696.71)
+        g[4] = 10000 - (2.138 / (x[0] * x[1]) + 7883.39 * x[2] - 705.04)
+        g[5] = 2000 - (0.417 * x[0] * x[1] + 1721.26 * x[2] - 136.54)
+        g[6] = 550 - (0.164 / (x[0] * x[1]) + 631.13 * x[2] - 54.48)
+        g = np.where(g < 0, -g, 0)
+
+        return f, g
+
+
+
+
+if __name__ == '__main__':
+    np.random.seed(seed=1)
+    fun = RE21()
+
+    x = fun.lbound + (fun.ubound - fun.lbound) * np.random.rand(fun.n_variables)
+    print("Problem = {}".format(fun.problem_name))
+    print("Number of objectives = {}".format(fun.n_objectives))
+    print("Number of variables = {}".format(fun.n_variables))
+    print("Number of constraints = {}".format(fun.n_constraints))
+    print("Lower bounds = ", fun.lbound)
+    print("Upper bounds = ", fun.ubound)
+    print("x = ", x)
+
+    if 'CRE' in fun.problem_name:
+        f, g = fun.evaluate(x)
+        print("f(x) = {}".format(f))
+        print("g(x) = {}".format(g))
+    else:
+        f = fun.evaluate(x)
         print("f(x) = {}".format(f))
```

### Comparing `libmoon-0.1.9/libmoon/problem/synthetic/vlmop.py` & `libmoon-0.2.1/libmoon/problem/synthetic/vlmop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import matplotlib.pyplot as plt
 import torch
 import numpy as np
 
-from ..mop import mop
+from libmoon.problem.synthetic.mop import mop
 
 
 
 class VLMOP1(mop):
     def __init__( self, n_var=10, n_obj=2, lbound=-np.ones(10), ubound=np.ones(10) ):
         super().__init__(n_var=n_var,
                          n_obj=n_obj,
```

### Comparing `libmoon-0.1.9/libmoon/problem/synthetic/zdt.py` & `libmoon-0.2.1/libmoon/problem/synthetic/zdt.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,51 +6,58 @@
     Zitzler, E., Deb, K., & Thiele, L. (2000). Comparison of multiobjective
     evolutionary algorithms: Empirical results. Evolutionary computation,
     8(2), 173-195. DOI: 10.1162/106365600568202
 """
 import numpy as np
 import torch
 from matplotlib import pyplot as plt
-from ..mop import mop
+from libmoon.problem.synthetic.mop import mop
 
 class ZDT1(mop):
 
-    def __init__(self, n_var=30, n_obj=2, lbound=np.zeros(30),
-                 ubound=np.ones(30)):
+    def __init__(self, n_var=30, n_obj=2):
+        lbound = np.zeros(n_var)
+        ubound = np.ones(n_var)
         super().__init__(n_var=n_var,
                          n_obj=n_obj,
                          lbound=lbound,
                          ubound=ubound, )
         self.problem_name = 'ZDT1'
 
 
     def _evaluate_torch(self, x: torch.Tensor):
         f1 = x[:, 0]
-        n = len(x)
+        n = x.shape[-1]
         g = 1 + 9/(n-1) * torch.sum(x[:, 1:], dim=1)
         h = 1 - torch.sqrt(f1 / g)
         f2 = g * h
         return torch.stack((f1, f2), dim=1)
 
     def _evaluate_numpy(self, x: np.ndarray):
-        n = len(x)
+        assert len(x.shape)==2
+        n = x.shape[-1]
+
         f1 = x[:, 0]
         g = 1 + 9 / (n-1) * np.sum(x[:, 1:], axis=1)
         f2 = 1 - np.sqrt(f1 / g)
         return np.stack((f1, f2), axis=1)
 
+
     def _get_pf(self, n_points: int = 100):
         f1 = np.linspace(0, 1, n_points)
         f2 = 1 - np.sqrt(f1)
         return np.stack((f1, f2), axis=1)
 
 
 class ZDT2(mop):
 
-    def __init__(self, n_var=30, n_obj=2, lbound=np.zeros(30), ubound=np.ones(30)):
+    def __init__(self, n_var=30, n_obj=2):
+        lbound = np.zeros(n_var)
+        ubound = np.ones(n_var)
+
         super().__init__(n_var=n_var,
                          n_obj=n_obj,
                          lbound=lbound,
                          ubound=ubound)
         self.problem_name = 'ZDT2'
 
     def _evaluate_torch(self, x: torch.Tensor):
```

### Comparing `libmoon-0.1.9/libmoon/solver/mobo/dirhvego.py` & `libmoon-0.2.1/libmoon/solver/mobo/dirhvego.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-# -*- coding: utf-8 -*-
-"""
-------------------------------- Reference --------------------------------
- L. Zhao and Q. Zhang, Hypervolume-Guided Decomposition for Parallel
- Expensive Multiobjective Optimization. IEEE Transactions on Evolutionary
- Computation, 2023.
-"""
-import numpy as np
-from scipy import stats
-from sklearn.preprocessing import MinMaxScaler
-import matplotlib.pyplot as plt
-from solver.mobo.mobod import MOBOD
-
-
-class DirHVEGO(MOBOD):
-    def __init__(self,
-                 mop: any = None,
-                 ref_vecs: np.ndarray = None,
-                 max_iter: int = None,
-                 batch_size: int = 5
-                 ) -> None:
-        super().__init__(mop, ref_vecs, max_iter, batch_size)
-
-    def evaluator_acquisition(self, u, sigma, ref_vec, pref_inc):
-        '''
-        Parameters:
-        ----------
-        u :
-        sigma :
-        ref_vec: direction vector
-        pref_inc :  preference-conditional incumbent
-
-        Returns
-        -------
-        EI_D : preference-conditional EI: DirHV-EI(X|pref_vec)
-
-        '''
-        xi_minus_u = pref_inc - u  # N*M
-        tau = xi_minus_u / sigma  # N*M
-        temp = xi_minus_u * stats.norm(0, 1).cdf(tau) + sigma * stats.norm(0, 1).pdf(tau)  # N*M
-        EI_D = np.prod(temp, axis=1)
-        return EI_D
-
-    def step(self):
-        #  normalization
-        X_norm = self.X.copy()
-        Y_scaler = MinMaxScaler(feature_range=(0, 1))
-        Y_norm = Y_scaler.fit_transform(self.Y)
-
-        # GP modeling
-        self.construct_model(X_norm, Y_norm)
-
-        # Utopian point
-        Z = -0.01 * np.ones(shape=[1, self.n_obj])
-        # Calculate the Intersection points and Direction vectors
-        Xi, Lambda = self.get_Xi(Y_norm[self.pf_idx[0]], self.ref_vecs, Z)
-        # Use MOEA/D to maximize DirHV-EI
-        Pop_Dec, Pop_u, Pop_s = self.MOEAD_GR_(Lambda, Xi)
-        # Discard duplicate candidates
-        PopDec, ia = np.unique(Pop_Dec, axis=0, return_index=True)
-        Pop_u = Pop_u[ia, :]
-        Pop_s = Pop_s[ia, :]
-        N = self.ref_vecs.shape[0]  # pop size
-
-        # Compute EI_D for all the points in Q
-        L = PopDec.shape[0]
-        EIDs = np.zeros((L, N))
-        for j in range(L):
-            EIDs[j, :] = self.evaluator_acquisition(np.tile(Pop_u[j], (N, 1)), np.tile(Pop_s[j], (N, 1)), Lambda, Xi)
-
-        # Find q solutions with the greedy algorithm
-        # Batch_size = np.min(Problem.maxFE - Problem.FE, q)  # the total budget is Problem.maxFE
-        Qb = self.batchSelection(EIDs, self.batch_size)
-
-        return PopDec[Qb, :]
-
-    def batchSelection(self, EIDs, q):
-        # Algorithm 3: Submodularity-based Batch Selection
-        L, N = EIDs.shape
-        Qb = []
-        temp = EIDs.copy()
-        beta = np.zeros(N)
-        for i in range(q):
-            index = np.argmax(np.sum(temp, axis=1))
-            Qb.append(index)
-            beta = beta + temp[index, :]
-            # temp: [EI_D(x|\lambda) - beta]_+
-            temp = EIDs - np.repeat(beta[None, :], L, axis=0)
-            temp[temp < 0] = 0
-        return Qb
-
-    def get_Xi(self, A, W, Z):
-        N = self.ref_vecs.shape[0]
-        W_ = 1.1 * self.ref_vecs - Z
-        Lambda = W_ / np.linalg.norm(W_, axis=1, keepdims=True)
-        # Eq. 11, compute the intersection points
-        Lambda_ = 1.0 / Lambda
-        A = A - Z  # L*M
-        G = np.outer(Lambda_[:, 0], A[:, 0])  # N*L, f1
-        for j in range(1, self.n_obj):
-            G = np.maximum(G, np.outer(Lambda_[:, j], A[:, j]))  # N*L, max(fi,fj)
-
-        # minimum of mTch for each direction vector
-        Lmin = np.min(G, axis=1, keepdims=True)  # N*1  one for each direction vector
-
-        # N*M  Intersection points
-        Xi = Z + np.multiply(Lmin, Lambda)
-
-        return Xi, Lambda
-
-
-
-
-
-if __name__ == '__main__':
-    from libmoon.problem.synthetic.zdt import ZDT1
-    from pyDOE3 import lhs
-
-    prob = ZDT1(n_var=8,
-                n_obj=2,
-                lower_bound=np.array([.0] * 8),
-                upper_bound=np.array([1.] * 8))
-    alg = DirHVEGO()
-    alg.setup(prob, max_iter=10, batch_size=5)
-
-    xdoe = (prob.ub - prob.lb) * lhs(prob.n_var, samples=11 * prob.n_var - 1,
-                                     criterion='maximin', iterations=10) + prob.lb
-
-
-    ydoe = prob.evaluate(xdoe)
-
-    alg.solve(xdoe, ydoe)
-
-    plt.scatter(alg.Y[alg.pf_idx[0], 0], alg.Y[alg.pf_idx[0], 1], c='none', edgecolors='r')
+# -*- coding: utf-8 -*-
+"""
+------------------------------- Reference --------------------------------
+ L. Zhao and Q. Zhang, Hypervolume-Guided Decomposition for Parallel
+ Expensive Multiobjective Optimization. IEEE Transactions on Evolutionary
+ Computation, 2023.
+"""
+import numpy as np
+from scipy import stats
+from sklearn.preprocessing import MinMaxScaler
+import matplotlib.pyplot as plt
+from solver.mobo.mobod import MOBOD
+
+
+class DirHVEGO(MOBOD):
+    def __init__(self,
+                 mop: any = None,
+                 ref_vecs: np.ndarray = None,
+                 max_iter: int = None,
+                 batch_size: int = 5
+                 ) -> None:
+        super().__init__(mop, ref_vecs, max_iter, batch_size)
+
+    def evaluator_acquisition(self, u, sigma, ref_vec, pref_inc):
+        '''
+        Parameters:
+        ----------
+        u :
+        sigma :
+        ref_vec: direction vector
+        pref_inc :  preference-conditional incumbent
+
+        Returns
+        -------
+        EI_D : preference-conditional EI: DirHV-EI(X|pref_vec)
+
+        '''
+        xi_minus_u = pref_inc - u  # N*M
+        tau = xi_minus_u / sigma  # N*M
+        temp = xi_minus_u * stats.norm(0, 1).cdf(tau) + sigma * stats.norm(0, 1).pdf(tau)  # N*M
+        EI_D = np.prod(temp, axis=1)
+        return EI_D
+
+    def step(self):
+        #  normalization
+        X_norm = self.X.copy()
+        Y_scaler = MinMaxScaler(feature_range=(0, 1))
+        Y_norm = Y_scaler.fit_transform(self.Y)
+
+        # GP modeling
+        self.construct_model(X_norm, Y_norm)
+
+        # Utopian point
+        Z = -0.01 * np.ones(shape=[1, self.n_obj])
+        # Calculate the Intersection points and Direction vectors
+        Xi, Lambda = self.get_Xi(Y_norm[self.pf_idx[0]], self.ref_vecs, Z)
+        # Use MOEA/D to maximize DirHV-EI
+        Pop_Dec, Pop_u, Pop_s = self.MOEAD_GR_(Lambda, Xi)
+        # Discard duplicate candidates
+        PopDec, ia = np.unique(Pop_Dec, axis=0, return_index=True)
+        Pop_u = Pop_u[ia, :]
+        Pop_s = Pop_s[ia, :]
+        N = self.ref_vecs.shape[0]  # pop size
+
+        # Compute EI_D for all the points in Q
+        L = PopDec.shape[0]
+        EIDs = np.zeros((L, N))
+        for j in range(L):
+            EIDs[j, :] = self.evaluator_acquisition(np.tile(Pop_u[j], (N, 1)), np.tile(Pop_s[j], (N, 1)), Lambda, Xi)
+
+        # Find q solutions with the greedy algorithm
+        # Batch_size = np.min(Problem.maxFE - Problem.FE, q)  # the total budget is Problem.maxFE
+        Qb = self.batchSelection(EIDs, self.batch_size)
+
+        return PopDec[Qb, :]
+
+    def batchSelection(self, EIDs, q):
+        # Algorithm 3: Submodularity-based Batch Selection
+        L, N = EIDs.shape
+        Qb = []
+        temp = EIDs.copy()
+        beta = np.zeros(N)
+        for i in range(q):
+            index = np.argmax(np.sum(temp, axis=1))
+            Qb.append(index)
+            beta = beta + temp[index, :]
+            # temp: [EI_D(x|\lambda) - beta]_+
+            temp = EIDs - np.repeat(beta[None, :], L, axis=0)
+            temp[temp < 0] = 0
+        return Qb
+
+    def get_Xi(self, A, W, Z):
+        N = self.ref_vecs.shape[0]
+        W_ = 1.1 * self.ref_vecs - Z
+        Lambda = W_ / np.linalg.norm(W_, axis=1, keepdims=True)
+        # Eq. 11, compute the intersection points
+        Lambda_ = 1.0 / Lambda
+        A = A - Z  # L*M
+        G = np.outer(Lambda_[:, 0], A[:, 0])  # N*L, f1
+        for j in range(1, self.n_obj):
+            G = np.maximum(G, np.outer(Lambda_[:, j], A[:, j]))  # N*L, max(fi,fj)
+
+        # minimum of mTch for each direction vector
+        Lmin = np.min(G, axis=1, keepdims=True)  # N*1  one for each direction vector
+
+        # N*M  Intersection points
+        Xi = Z + np.multiply(Lmin, Lambda)
+
+        return Xi, Lambda
+
+
+
+
+
+if __name__ == '__main__':
+    from libmoon.problem.synthetic.zdt import ZDT1
+    from pyDOE3 import lhs
+
+    prob = ZDT1(n_var=8,
+                n_obj=2,
+                lower_bound=np.array([.0] * 8),
+                upper_bound=np.array([1.] * 8))
+    alg = DirHVEGO()
+    alg.setup(prob, max_iter=10, batch_size=5)
+
+    xdoe = (prob.ub - prob.lb) * lhs(prob.n_var, samples=11 * prob.n_var - 1,
+                                     criterion='maximin', iterations=10) + prob.lb
+
+
+    ydoe = prob.evaluate(xdoe)
+
+    alg.solve(xdoe, ydoe)
+
+    plt.scatter(alg.Y[alg.pf_idx[0], 0], alg.Y[alg.pf_idx[0], 1], c='none', edgecolors='r')
     plt.show()
```

### Comparing `libmoon-0.1.9/libmoon/solver/mobo/mobod.py` & `libmoon-0.2.1/libmoon/solver/mobo/mobod.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-import numpy as np
-from smt.surrogate_models import KRG
-
-from scipy.spatial.distance import cdist
-
-from pymoo.indicators.hv import HV
-from pymoo.util.nds.non_dominated_sorting import NonDominatedSorting
-from pymoo.util.ref_dirs import get_reference_directions
-from pyDOE3 import lhs
-
-from solver.mobo.utils.termination import termination
-
-
-'''
-    Main algorithm framework for  Decomposition-based Multi-objective Bayesian Optimization.
-'''
-
-
-
-class MOBOD(object):
-    def __init__(self,
-                 mop: any = None,
-                 ref_vecs: np.ndarray = None,
-                 max_iter: int = None,
-                 batch_size: int = 5,
-                 ):
-        self.mop = mop
-        self.ref_vecs = ref_vecs
-        self.max_iter = max_iter
-        self.batch_size = batch_size
-        self.termina = termination()
-
-    def setup(self,
-              mop: any = None,
-              ref_vec: np.ndarray = None,
-              max_iter: int = None,
-              batch_size: int = 5,
-              ) -> None:
-        if mop is not None:
-            self.mop = mop
-            self.n_var, self.n_obj = mop.n_var, mop.n_obj
-        assert not mop.has_constraint
-        self.termina.setup(max_gen=max_iter)
-
-        if self.ref_vecs is None:
-            self.ref_vecs = get_reference_directions("uniform", mop.get_number_objective, n_partitions=199)
-        self.pop_size = len(self.ref_vecs)
-        # to keep track of data
-        self.X = None
-        self.Y = None
-        self.sample_num = 0
-        self.i_iter = 0
-        self.pf_idx = None  # idx of nondominated solutions
-        self.ref_point = None
-        self.hv_all_value = np.zeros([max_iter + 1, 1])
-
-    def construct_model(self, X_obs, Y_obs):
-        # build surrogate models
-        theta = [self.sample_num ** (-1. / self.sample_num)] * self.n_var
-        self.surrogate_model = [KRG(theta0=theta) for i in range(self.n_obj)]
-        for i in range(self.n_obj):
-            self.surrogate_model[i].options.__setitem__('print_global', False)
-            self.surrogate_model[i].set_training_values(X_obs, Y_obs[:, i])
-            self.surrogate_model[i].train()
-
-    def predict_model(self, X):
-        N = X.shape[0]
-        u = np.zeros(shape=(N, self.n_obj), dtype=float)
-        MSE = np.zeros(shape=(N, self.n_obj), dtype=float)
-
-        for j in range(self.n_obj):
-            u[:, j] = self.surrogate_model[j].predict_values(X)[:, 0]
-            # MSE[:,j] = np.sqrt(model[j].predict_variances(PopDec))
-            MSE[:, j] = self.surrogate_model[j].predict_variances(X)[:, 0]
-
-        MSE[MSE < 0] = 0
-        s = np.sqrt(MSE)
-        return u, s
-
-    def evaluator_acquisition(self, u, sigma, ref_vec, pref_inc):
-        pass
-
-    def aggregate_data(self, X_new, Y_new):
-        if self.sample_num == 0:
-            self.X = X_new.copy()
-            self.Y = Y_new.copy()
-        else:
-            self.X = np.vstack([self.X, X_new])
-            self.Y = np.vstack([self.Y, Y_new])
-        self.sample_num += len(X_new)
-
-        # nondominated X, Y
-        nds = NonDominatedSorting()
-        self.pf_idx = nds.do(self.Y)
-        # X_nds = self.X[self.pf_idx[0]]
-        Y_nds = self.Y[self.pf_idx[0]]
-
-        hv = HV(ref_point=self.ref_point)
-        hv_value = hv(Y_nds)
-        self.hv_all_value[self.i_iter, 0] = hv_value
-
-    def step(self):
-        pass
-
-    def solve(self, X_init, Y_init):
-        if self.ref_point is None:
-            self.ref_point = np.max(Y_init, axis=0)
-        self.aggregate_data(X_init, Y_init)
-
-        s = str('n_iter').center(12) + " | " + str('n_eval').center(12) + " | " + str('HV').center(12)
-        print("=" * len(s))
-        print(s)
-        print("=" * len(s))
-        print(str(self.i_iter).center(12), "|", str(self.sample_num).center(12), "| ",
-              f"%.{10}f" % self.hv_all_value[self.i_iter, 0])
-
-        while self.termina.has_next:
-            self.i_iter += 1
-            # generate new samples
-            X_next = self.step()  # check
-            Y_next = self.mop.evaluate(X_next)
-            self.termina(nfe=self.batch_size, gen=1)
-            self.aggregate_data(X_next, Y_next)
-            print(str(self.i_iter).center(12), "|", str(self.sample_num).center(12), "| ",
-                  f"%.{10}f" % self.hv_all_value[self.i_iter, 0])
-
-        print("=" * len(s))
-
-    def MOEAD_GR_(self, ref_vecs, pref_incs):
-        # using MOEA/D-GR to solve subproblems
-        maxIter = 50
-        N = self.pop_size
-        T = int(np.ceil(N / 10))  # size of neighbourhood: 0.1*N
-        B = np.argsort(cdist(ref_vecs, ref_vecs), axis=1, kind='quicksort')[:, :T]
-
-        # the initial population for MOEA/D
-
-        Pop_Dec = (self.mop.get_upper_bound - self.mop.get_lower_bound) * lhs(self.n_var,
-                                                                              samples=N) + self.mop.get_lower_bound
-        Pop_u, Pop_sigma = self.predict_model(Pop_Dec)
-        Pop_EID = self.evaluator_acquisition(Pop_u, Pop_sigma, ref_vecs, pref_incs)
-
-        # optimization
-        for gen in range(maxIter - 1):
-            for i in range(N):
-                if np.random.random() < 0.8:  # delta
-                    P = B[i, np.random.permutation(B.shape[1])]
-                else:
-                    P = np.random.permutation(N)
-                # generate an offspring 1*d
-                Off_Dec = self._OperatorDE(Pop_Dec[i, :][None, :], Pop_Dec[P[0], :][None, :], Pop_Dec[P[1], :][None, :])
-                Off_u, Off_sigma = self.predict_model(Off_Dec)
-                # Global Replacement  MOEA/D-GR
-                # Find the most approprite subproblem and its neighbourhood
-                EID_all = self.evaluator_acquisition(np.repeat(Off_u, N, axis=0), np.repeat(Off_sigma, N, axis=0),
-                                                     ref_vecs, pref_incs)
-                best_index = np.argmax(EID_all)
-                P = B[best_index, :]  # replacement neighborhood
-
-                offindex = P[Pop_EID[P] < EID_all[P]]
-                if len(offindex) > 0:
-                    Pop_Dec[offindex, :] = np.repeat(Off_Dec, len(offindex), axis=0)
-                    Pop_u[offindex, :] = np.repeat(Off_u, len(offindex), axis=0)
-                    Pop_sigma[offindex, :] = np.repeat(Off_sigma, len(offindex), axis=0)
-                    Pop_EID[offindex] = EID_all[offindex]
-
-        return Pop_Dec, Pop_u, Pop_sigma
-
-    def _OperatorDE(self, Parent1, Parent2, Parent3):
-        '''
-            generate one offspring by P1 + 0.5*(P2-P3) and polynomial mutation.
-        '''
-        # Parameter
-        CR = 1
-        F = 0.5
-        proM = 1
-        disM = 20
-        #
-        N, D = Parent1.shape
-        # Differental evolution
-        Site = np.random.rand(N, D) < CR
-        Offspring = Parent1.copy()
-        Offspring[Site] = Offspring[Site] + F * (Parent2[Site] - Parent3[Site])
-        # Polynomial mutation
-        Lower = np.atleast_2d(self.mop.get_lower_bound)  # numpy  Upper=np.array(Upper)[None,:]
-        Upper = np.atleast_2d(self.mop.get_upper_bound)  # Lower = np.atleast_2d(Lower)
-        U_L = Upper - Lower
-        Site = np.random.rand(N, D) < proM / D
-        mu = np.random.rand(N, D)
-        temp = np.logical_and(Site, mu <= 0.5)
-        Offspring = np.minimum(np.maximum(Offspring, Lower), Upper)
-        delta1 = (Offspring - Lower) / U_L
-        delta2 = (Upper - Offspring) / U_L
-        #  mu <= 0.5
-        val = 2. * mu + (1 - 2. * mu) * (np.power(1. - delta1, disM + 1))
-        Offspring[temp] = Offspring[temp] + (np.power(val[temp], 1.0 / (disM + 1)) - 1.) * U_L[temp]
-        # mu > 0.5
-        temp = np.logical_and(Site, mu > 0.5)
-        val = 2. * (1.0 - mu) + 2. * (mu - 0.5) * (np.power(1. - delta2, disM + 1))
-        Offspring[temp] = Offspring[temp] + (1.0 - np.power(val[temp], 1.0 / (disM + 1))) * U_L[temp]
-
+import numpy as np
+from smt.surrogate_models import KRG
+
+from scipy.spatial.distance import cdist
+
+from pymoo.indicators.hv import HV
+from pymoo.util.nds.non_dominated_sorting import NonDominatedSorting
+from pymoo.util.ref_dirs import get_reference_directions
+from pyDOE3 import lhs
+
+from solver.mobo.utils.termination import termination
+
+
+'''
+    Main algorithm framework for  Decomposition-based Multi-objective Bayesian Optimization.
+'''
+
+
+
+class MOBOD(object):
+    def __init__(self,
+                 mop: any = None,
+                 ref_vecs: np.ndarray = None,
+                 max_iter: int = None,
+                 batch_size: int = 5,
+                 ):
+        self.mop = mop
+        self.ref_vecs = ref_vecs
+        self.max_iter = max_iter
+        self.batch_size = batch_size
+        self.termina = termination()
+
+    def setup(self,
+              mop: any = None,
+              ref_vec: np.ndarray = None,
+              max_iter: int = None,
+              batch_size: int = 5,
+              ) -> None:
+        if mop is not None:
+            self.mop = mop
+            self.n_var, self.n_obj = mop.n_var, mop.n_obj
+        assert not mop.has_constraint
+        self.termina.setup(max_gen=max_iter)
+
+        if self.ref_vecs is None:
+            self.ref_vecs = get_reference_directions("uniform", mop.get_number_objective, n_partitions=199)
+        self.pop_size = len(self.ref_vecs)
+        # to keep track of data
+        self.X = None
+        self.Y = None
+        self.sample_num = 0
+        self.i_iter = 0
+        self.pf_idx = None  # idx of nondominated solutions
+        self.ref_point = None
+        self.hv_all_value = np.zeros([max_iter + 1, 1])
+
+    def construct_model(self, X_obs, Y_obs):
+        # build surrogate models
+        theta = [self.sample_num ** (-1. / self.sample_num)] * self.n_var
+        self.surrogate_model = [KRG(theta0=theta) for i in range(self.n_obj)]
+        for i in range(self.n_obj):
+            self.surrogate_model[i].options.__setitem__('print_global', False)
+            self.surrogate_model[i].set_training_values(X_obs, Y_obs[:, i])
+            self.surrogate_model[i].train()
+
+    def predict_model(self, X):
+        N = X.shape[0]
+        u = np.zeros(shape=(N, self.n_obj), dtype=float)
+        MSE = np.zeros(shape=(N, self.n_obj), dtype=float)
+
+        for j in range(self.n_obj):
+            u[:, j] = self.surrogate_model[j].predict_values(X)[:, 0]
+            # MSE[:,j] = np.sqrt(model[j].predict_variances(PopDec))
+            MSE[:, j] = self.surrogate_model[j].predict_variances(X)[:, 0]
+
+        MSE[MSE < 0] = 0
+        s = np.sqrt(MSE)
+        return u, s
+
+    def evaluator_acquisition(self, u, sigma, ref_vec, pref_inc):
+        pass
+
+    def aggregate_data(self, X_new, Y_new):
+        if self.sample_num == 0:
+            self.X = X_new.copy()
+            self.Y = Y_new.copy()
+        else:
+            self.X = np.vstack([self.X, X_new])
+            self.Y = np.vstack([self.Y, Y_new])
+        self.sample_num += len(X_new)
+
+        # nondominated X, Y
+        nds = NonDominatedSorting()
+        self.pf_idx = nds.do(self.Y)
+        # X_nds = self.X[self.pf_idx[0]]
+        Y_nds = self.Y[self.pf_idx[0]]
+
+        hv = HV(ref_point=self.ref_point)
+        hv_value = hv(Y_nds)
+        self.hv_all_value[self.i_iter, 0] = hv_value
+
+    def step(self):
+        pass
+
+    def solve(self, X_init, Y_init):
+        if self.ref_point is None:
+            self.ref_point = np.max(Y_init, axis=0)
+        self.aggregate_data(X_init, Y_init)
+
+        s = str('n_iter').center(12) + " | " + str('n_eval').center(12) + " | " + str('HV').center(12)
+        print("=" * len(s))
+        print(s)
+        print("=" * len(s))
+        print(str(self.i_iter).center(12), "|", str(self.sample_num).center(12), "| ",
+              f"%.{10}f" % self.hv_all_value[self.i_iter, 0])
+
+        while self.termina.has_next:
+            self.i_iter += 1
+            # generate new samples
+            X_next = self.step()  # check
+            Y_next = self.mop.evaluate(X_next)
+            self.termina(nfe=self.batch_size, gen=1)
+            self.aggregate_data(X_next, Y_next)
+            print(str(self.i_iter).center(12), "|", str(self.sample_num).center(12), "| ",
+                  f"%.{10}f" % self.hv_all_value[self.i_iter, 0])
+
+        print("=" * len(s))
+
+    def MOEAD_GR_(self, ref_vecs, pref_incs):
+        # using MOEA/D-GR to solve subproblems
+        maxIter = 50
+        N = self.pop_size
+        T = int(np.ceil(N / 10))  # size of neighbourhood: 0.1*N
+        B = np.argsort(cdist(ref_vecs, ref_vecs), axis=1, kind='quicksort')[:, :T]
+
+        # the initial population for MOEA/D
+
+        Pop_Dec = (self.mop.get_upper_bound - self.mop.get_lower_bound) * lhs(self.n_var,
+                                                                              samples=N) + self.mop.get_lower_bound
+        Pop_u, Pop_sigma = self.predict_model(Pop_Dec)
+        Pop_EID = self.evaluator_acquisition(Pop_u, Pop_sigma, ref_vecs, pref_incs)
+
+        # optimization
+        for gen in range(maxIter - 1):
+            for i in range(N):
+                if np.random.random() < 0.8:  # delta
+                    P = B[i, np.random.permutation(B.shape[1])]
+                else:
+                    P = np.random.permutation(N)
+                # generate an offspring 1*d
+                Off_Dec = self._OperatorDE(Pop_Dec[i, :][None, :], Pop_Dec[P[0], :][None, :], Pop_Dec[P[1], :][None, :])
+                Off_u, Off_sigma = self.predict_model(Off_Dec)
+                # Global Replacement  MOEA/D-GR
+                # Find the most approprite subproblem and its neighbourhood
+                EID_all = self.evaluator_acquisition(np.repeat(Off_u, N, axis=0), np.repeat(Off_sigma, N, axis=0),
+                                                     ref_vecs, pref_incs)
+                best_index = np.argmax(EID_all)
+                P = B[best_index, :]  # replacement neighborhood
+
+                offindex = P[Pop_EID[P] < EID_all[P]]
+                if len(offindex) > 0:
+                    Pop_Dec[offindex, :] = np.repeat(Off_Dec, len(offindex), axis=0)
+                    Pop_u[offindex, :] = np.repeat(Off_u, len(offindex), axis=0)
+                    Pop_sigma[offindex, :] = np.repeat(Off_sigma, len(offindex), axis=0)
+                    Pop_EID[offindex] = EID_all[offindex]
+
+        return Pop_Dec, Pop_u, Pop_sigma
+
+    def _OperatorDE(self, Parent1, Parent2, Parent3):
+        '''
+            generate one offspring by P1 + 0.5*(P2-P3) and polynomial mutation.
+        '''
+        # Parameter
+        CR = 1
+        F = 0.5
+        proM = 1
+        disM = 20
+        #
+        N, D = Parent1.shape
+        # Differental evolution
+        Site = np.random.rand(N, D) < CR
+        Offspring = Parent1.copy()
+        Offspring[Site] = Offspring[Site] + F * (Parent2[Site] - Parent3[Site])
+        # Polynomial mutation
+        Lower = np.atleast_2d(self.mop.get_lower_bound)  # numpy  Upper=np.array(Upper)[None,:]
+        Upper = np.atleast_2d(self.mop.get_upper_bound)  # Lower = np.atleast_2d(Lower)
+        U_L = Upper - Lower
+        Site = np.random.rand(N, D) < proM / D
+        mu = np.random.rand(N, D)
+        temp = np.logical_and(Site, mu <= 0.5)
+        Offspring = np.minimum(np.maximum(Offspring, Lower), Upper)
+        delta1 = (Offspring - Lower) / U_L
+        delta2 = (Upper - Offspring) / U_L
+        #  mu <= 0.5
+        val = 2. * mu + (1 - 2. * mu) * (np.power(1. - delta1, disM + 1))
+        Offspring[temp] = Offspring[temp] + (np.power(val[temp], 1.0 / (disM + 1)) - 1.) * U_L[temp]
+        # mu > 0.5
+        temp = np.logical_and(Site, mu > 0.5)
+        val = 2. * (1.0 - mu) + 2. * (mu - 0.5) * (np.power(1. - delta2, disM + 1))
+        Offspring[temp] = Offspring[temp] + (1.0 - np.power(val[temp], 1.0 / (disM + 1))) * U_L[temp]
+
         return Offspring
```

### Comparing `libmoon-0.1.9/libmoon/solver/mobo/utils/termination.py` & `libmoon-0.2.1/libmoon/solver/mobo/utils/termination.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Any
-import numpy as np
-
-
-class termination:
-
-    def __init__(self) -> None:
-        pass
-
-    def __call__(self,
-                 nfe: int = 0,
-                 gen: int = 0,
-                 ) -> bool:
-        self.nfe += nfe
-        self.gen += gen
-
-    def setup(self,
-              nfe: int = 0,
-              gen: int = 0,
-              max_nfe: int = np.inf,
-              max_gen: int = np.inf,
-              ) -> None:
-        self.nfe = nfe
-        self.gen = gen
-        self.max_nfe = max_nfe
-        self.max_gen = max_gen
-
-    @property
-    def has_next(self) -> bool:
-        return (self.nfe < self.max_nfe) and (self.gen < self.max_gen)
+from typing import Any
+import numpy as np
+
+
+class termination:
+
+    def __init__(self) -> None:
+        pass
+
+    def __call__(self,
+                 nfe: int = 0,
+                 gen: int = 0,
+                 ) -> bool:
+        self.nfe += nfe
+        self.gen += gen
+
+    def setup(self,
+              nfe: int = 0,
+              gen: int = 0,
+              max_nfe: int = np.inf,
+              max_gen: int = np.inf,
+              ) -> None:
+        self.nfe = nfe
+        self.gen = gen
+        self.max_nfe = max_nfe
+        self.max_gen = max_gen
+
+    @property
+    def has_next(self) -> bool:
+        return (self.nfe < self.max_nfe) and (self.gen < self.max_gen)
```

### Comparing `libmoon-0.1.9/libmoon/solver/moea/moead_pfl.py` & `libmoon-0.2.1/libmoon/solver/moea/moead_pfl.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,221 +1,221 @@
-import os.path
-
-from solver.moea.moead import MOEAD
-import numpy as np
-import argparse
-import time
-from pymoo.indicators.hv import HV
-from libmoon.util_global.constant import FONT_SIZE, problem_dict, root_name
-
-from solver.moea.utils.genetic_operator import cross_sbx, mut_pm
-from solver.moea.utils.utils_ea import neighborhood_selection, OperatorDE
-
-from matplotlib import pyplot as plt
-from solver.pfl.model.simple import PFLModel
-import torch
-from torch import Tensor
-from torch.optim import Adam
-
-from torch.autograd import Variable
-from indicator.indicator import get_MMS, pref2angle, angle2pref
-
-import pickle
-
-
-
-class MOEAD_PFL(MOEAD):
-    def __init__(self,
-                 mop: any = None,
-                 ref_vec: np.ndarray = None,
-                 n_neighbors: int = 10,
-                 ):
-        super().__init__(mop, ref_vec, n_neighbors)
-        # self.pfl_update_num = 100
-        self.name = 'MOEAD_PFL'
-        # self.pfl_model = PFLModel(self.mop.n_obj)
-
-    def setup(self,
-              mop: any = None,
-              args: argparse.Namespace = None,
-              max_gen: int = 100,
-              pop_size: int = 100,
-              ) -> None:
-
-        super().setup(mop, args, max_gen, pop_size)
-        self.pfl_model = PFLModel(self.mop.n_obj)
-
-        self.optimizer = Adam(self.pfl_model.parameters(), lr=0.001)
-        self.pfl_update_num = args.n_pfl_update
-
-
-    def pfl_update(self):
-        loss_arr = []
-
-        angle_ts = pref2angle(self.ref_vec, self.mop.n_obj)
-        angle_ts = torch.Tensor( angle_ts )
-
-        for idx in range(500):
-            pred_y = self.pfl_model.forward( angle_ts )
-            loss = torch.sum( torch.pow(pred_y - Tensor(self.pop.F), 2) )
-            # print()
-            self.optimizer.zero_grad()
-            loss.backward()
-            loss_arr.append(loss.item())
-            self.optimizer.step()
-
-
-        use_plot = False
-        if use_plot:
-            plt.plot(loss_arr)
-            plt.xlabel('iteration')
-            plt.ylabel('loss')
-            plt.show()
-            assert False
-
-
-    def pref_adjust(self):
-        pref = self.ref_vec
-        pref_old = np.copy(pref)
-        angle = pref2angle(pref, self.mop.n_obj)
-        angle_ts = Variable( Tensor(angle), requires_grad=True )
-        angle_optimizer = Adam([angle_ts], lr=0.01)
-
-        loss_arr = []
-        for idx in range(1000):
-            pred_y = self.pfl_model.forward(angle_ts)
-            mms = get_MMS( pred_y )
-            angle_optimizer.zero_grad()
-            mms.backward()
-            loss_arr.append(mms.item())
-
-            angle_optimizer.step()
-            angle_ts.data = torch.clip(angle_ts.data, 1e-3, np.pi/2-1e-3)
-
-        pref_ts = angle2pref(angle_ts, self.mop.n_obj)
-        self.ref_vec = pref_ts.detach().numpy()
-
-
-        use_plot = False
-        if use_plot:
-            plt.plot(loss_arr)
-            plt.xlabel('iteration')
-            plt.ylabel('mms')
-            plt.show()
-            assert False
-
-        return pref_old
-
-
-
-
-    def step(self):
-        # print('using PFL updation')
-        self.gen += 1
-
-        if self.gen % self.pfl_update_num == 0:
-
-            # for idx, ref in enumerate(self.ref_vec):
-            #     if idx == 0:
-            #         plt.scatter(ref[0], ref[1], label='old', color='r')
-            #     else:
-            #         plt.scatter(ref[0], ref[1], color='r')
-
-            self.pfl_update()
-            pref_old = self.pref_adjust()
-            print('adjust at {}'.format(self.gen))
-
-            use_plt=False
-            if use_plt:
-                plt.scatter(pref_old[:,0], pref_old[:,1], label='old', color='r')
-                plt.scatter(self.ref_vec[:,0], self.ref_vec[:,1], label='new', color='b')
-                plt.legend()
-                plt.show()
-
-        for k in np.random.permutation(self.n_pop):
-            if self.args.crossover == 'sbx':
-                P = neighborhood_selection(self.n_pop, self.neighbors[k])
-                X = self.pop.parent_select(P)
-                off_cross = cross_sbx(X, self.mop.get_lower_bound, self.mop.get_upper_bound)
-            else:
-                P = neighborhood_selection(self.n_pop, self.neighbors[k], n_selects=3)
-                X = self.pop.parent_select(P)
-                off_cross = OperatorDE(np.atleast_2d(X[0]), np.atleast_2d(X[1]), np.atleast_2d(X[2]), self.mop)
-            off = mut_pm(off_cross, self.mop.get_lower_bound, self.mop.get_upper_bound)
-            off_f = self.mop(off).squeeze()
-            self.z_star = np.minimum(self.z_star, off_f)
-            self._update_neighbor(off, off_f, self.neighbors[k])
-            self.ep(off, off_f)
-        self.termina(nfe=self.n_pop, gen=1)
-
-
-
-
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser()
-    parser.add_argument('--n-gen', type=int, default=2000)
-    parser.add_argument('--n-pfl-update', type=int, default=500)
-
-    parser.add_argument('--crossover', type=str, default='sbx')  # crossover operator ['de', 'sbx']
-    parser.add_argument('--problem-name', type=str, default='RE24')  # should be in lowwer case
-
-    args = parser.parse_args()
-    problem = problem_dict[args.problem_name]
-    ref_point = np.array(1.2 * np.ones(problem.n_obj))
-    ind = HV(ref_point=ref_point)
-
-    alg = MOEAD_PFL()
-    print('{} on {}'.format(alg.name, problem.problem_name))
-    alg.setup(problem, args, max_gen=args.n_gen, pop_size=10)
-
-    ref_vec = alg.ref_vec
-    ts = time.time()
-    alg.solve()
-    print('solving over {:.2f}m'.format((time.time() - ts) / 60))
-
-    # statistics and save.
-    hv_val = ind.do(alg.pop.F)
-    mms = get_MMS(alg.pop.F)
-
-    print('hv: {:.4f}'.format(hv_val))
-    print('mms: {:.4f}'.format(mms))
-
-
-    pickle_folder = os.path.join(root_name, 'output', problem.problem_name, alg.name)
-    os.makedirs(pickle_folder, exist_ok=True)
-    pickle_name = os.path.join(pickle_folder, 'res.pkl')
-    with open(pickle_name, 'wb') as f:
-        pickle.dump(alg.pop.F, f)
-
-    txt_name = os.path.join(pickle_folder, 'res.txt')
-    with open(txt_name, 'w') as f:
-        f.write('hv: {:.4f}\n'.format(hv_val))
-        f.write('mms: {:.4f}\n'.format(mms))
-
-
-    if problem.n_obj == 2:
-        plt.scatter(alg.pop.F[:, 0], alg.pop.F[:, 1], c='none', edgecolors='r', label='solution')
-        plt.plot(alg.pop.F[:, 0], alg.pop.F[:, 1], c='r')
-
-        if not problem.problem_name.startswith('RE'):
-            pf = problem.get_pf()
-            plt.plot(pf[:, 0], pf[:, 1], c='b')
-
-        plt.legend()
-        plt.xlabel('$f_1$', fontsize=FONT_SIZE )
-        plt.ylabel('$f_2$', fontsize=FONT_SIZE )
-
-        ref_vec_norm = ref_vec / np.linalg.norm(ref_vec, axis=1, keepdims=True)
-        for ref in ref_vec_norm:
-            plt.plot([0, ref[0]], [0, ref[1]], c='k')
-    elif problem.n_obj == 3:
-        fig = plt.figure()
-        ax = fig.add_subplot(projection='3d')
-        ax.scatter(alg.pop.F[:, 0], alg.pop.F[:, 1], alg.pop.F[:, 2], c='none', edgecolors='r')
-        ax.set_xlabel('$f_1$', fontsize=FONT_SIZE)
-        ax.set_ylabel('$f_2$', fontsize=FONT_SIZE)
-        ax.set_zlabel('$f_3$', fontsize=FONT_SIZE)
-    else:
-        assert False, 'n_obj should be 2 or 3'
-
-    plt.show()
-
+import os.path
+
+from solver.moea.moead import MOEAD
+import numpy as np
+import argparse
+import time
+from pymoo.indicators.hv import HV
+from libmoon.util_global.constant import FONT_SIZE, problem_dict, root_name
+
+from solver.moea.utils.genetic_operator import cross_sbx, mut_pm
+from solver.moea.utils.utils_ea import neighborhood_selection, OperatorDE
+
+from matplotlib import pyplot as plt
+from solver.pfl.model.simple import PFLModel
+import torch
+from torch import Tensor
+from torch.optim import Adam
+
+from torch.autograd import Variable
+from libmoon.metrics.metrics import get_MMS, pref2angle, angle2pref
+
+import pickle
+
+
+
+class MOEAD_PFL(MOEAD):
+    def __init__(self,
+                 mop: any = None,
+                 ref_vec: np.ndarray = None,
+                 n_neighbors: int = 10,
+                 ):
+        super().__init__(mop, ref_vec, n_neighbors)
+        # self.pfl_update_num = 100
+        self.name = 'MOEAD_PFL'
+        # self.pfl_model = PFLModel(self.mop.n_obj)
+
+    def setup(self,
+              mop: any = None,
+              args: argparse.Namespace = None,
+              max_gen: int = 100,
+              pop_size: int = 100,
+              ) -> None:
+
+        super().setup(mop, args, max_gen, pop_size)
+        self.pfl_model = PFLModel(self.mop.n_obj)
+
+        self.optimizer = Adam(self.pfl_model.parameters(), lr=0.001)
+        self.pfl_update_num = args.n_pfl_update
+
+
+    def pfl_update(self):
+        loss_arr = []
+
+        angle_ts = pref2angle(self.ref_vec, self.mop.n_obj)
+        angle_ts = torch.Tensor( angle_ts )
+
+        for idx in range(500):
+            pred_y = self.pfl_model.forward( angle_ts )
+            loss = torch.sum( torch.pow(pred_y - Tensor(self.pop.F), 2) )
+            # print()
+            self.optimizer.zero_grad()
+            loss.backward()
+            loss_arr.append(loss.item())
+            self.optimizer.step()
+
+
+        use_plot = False
+        if use_plot:
+            plt.plot(loss_arr)
+            plt.xlabel('iteration')
+            plt.ylabel('loss')
+            plt.show()
+            assert False
+
+
+    def pref_adjust(self):
+        pref = self.ref_vec
+        pref_old = np.copy(pref)
+        angle = pref2angle(pref, self.mop.n_obj)
+        angle_ts = Variable( Tensor(angle), requires_grad=True )
+        angle_optimizer = Adam([angle_ts], lr=0.01)
+
+        loss_arr = []
+        for idx in range(1000):
+            pred_y = self.pfl_model.forward(angle_ts)
+            mms = get_MMS( pred_y )
+            angle_optimizer.zero_grad()
+            mms.backward()
+            loss_arr.append(mms.item())
+
+            angle_optimizer.step()
+            angle_ts.data = torch.clip(angle_ts.data, 1e-3, np.pi/2-1e-3)
+
+        pref_ts = angle2pref(angle_ts, self.mop.n_obj)
+        self.ref_vec = pref_ts.detach().numpy()
+
+
+        use_plot = False
+        if use_plot:
+            plt.plot(loss_arr)
+            plt.xlabel('iteration')
+            plt.ylabel('mms')
+            plt.show()
+            assert False
+
+        return pref_old
+
+
+
+
+    def step(self):
+        # print('using PFL updation')
+        self.gen += 1
+
+        if self.gen % self.pfl_update_num == 0:
+
+            # for idx, ref in enumerate(self.ref_vec):
+            #     if idx == 0:
+            #         plt.scatter(ref[0], ref[1], label='old', color='r')
+            #     else:
+            #         plt.scatter(ref[0], ref[1], color='r')
+
+            self.pfl_update()
+            pref_old = self.pref_adjust()
+            print('adjust at {}'.format(self.gen))
+
+            use_plt=False
+            if use_plt:
+                plt.scatter(pref_old[:,0], pref_old[:,1], label='old', color='r')
+                plt.scatter(self.ref_vec[:,0], self.ref_vec[:,1], label='new', color='b')
+                plt.legend()
+                plt.show()
+
+        for k in np.random.permutation(self.n_pop):
+            if self.args.crossover == 'sbx':
+                P = neighborhood_selection(self.n_pop, self.neighbors[k])
+                X = self.pop.parent_select(P)
+                off_cross = cross_sbx(X, self.mop.get_lower_bound, self.mop.get_upper_bound)
+            else:
+                P = neighborhood_selection(self.n_pop, self.neighbors[k], n_selects=3)
+                X = self.pop.parent_select(P)
+                off_cross = OperatorDE(np.atleast_2d(X[0]), np.atleast_2d(X[1]), np.atleast_2d(X[2]), self.mop)
+            off = mut_pm(off_cross, self.mop.get_lower_bound, self.mop.get_upper_bound)
+            off_f = self.mop(off).squeeze()
+            self.z_star = np.minimum(self.z_star, off_f)
+            self._update_neighbor(off, off_f, self.neighbors[k])
+            self.ep(off, off_f)
+        self.termina(nfe=self.n_pop, gen=1)
+
+
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser()
+    parser.add_argument('--n-gen', type=int, default=2000)
+    parser.add_argument('--n-pfl-update', type=int, default=500)
+
+    parser.add_argument('--crossover', type=str, default='sbx')  # crossover operator ['de', 'sbx']
+    parser.add_argument('--problem-name', type=str, default='RE24')  # should be in lowwer case
+
+    args = parser.parse_args()
+    problem = problem_dict[args.problem_name]
+    ref_point = np.array(1.2 * np.ones(problem.n_obj))
+    ind = HV(ref_point=ref_point)
+
+    alg = MOEAD_PFL()
+    print('{} on {}'.format(alg.name, problem.problem_name))
+    alg.setup(problem, args, max_gen=args.n_gen, pop_size=10)
+
+    ref_vec = alg.ref_vec
+    ts = time.time()
+    alg.solve()
+    print('solving over {:.2f}m'.format((time.time() - ts) / 60))
+
+    # statistics and save.
+    hv_val = ind.do(alg.pop.F)
+    mms = get_MMS(alg.pop.F)
+
+    print('hv: {:.4f}'.format(hv_val))
+    print('mms: {:.4f}'.format(mms))
+
+
+    pickle_folder = os.path.join(root_name, 'output', problem.problem_name, alg.name)
+    os.makedirs(pickle_folder, exist_ok=True)
+    pickle_name = os.path.join(pickle_folder, 'res.pkl')
+    with open(pickle_name, 'wb') as f:
+        pickle.dump(alg.pop.F, f)
+
+    txt_name = os.path.join(pickle_folder, 'res.txt')
+    with open(txt_name, 'w') as f:
+        f.write('hv: {:.4f}\n'.format(hv_val))
+        f.write('mms: {:.4f}\n'.format(mms))
+
+
+    if problem.n_obj == 2:
+        plt.scatter(alg.pop.F[:, 0], alg.pop.F[:, 1], c='none', edgecolors='r', label='solution')
+        plt.plot(alg.pop.F[:, 0], alg.pop.F[:, 1], c='r')
+
+        if not problem.problem_name.startswith('RE'):
+            pf = problem.get_pf()
+            plt.plot(pf[:, 0], pf[:, 1], c='b')
+
+        plt.legend()
+        plt.xlabel('$f_1$', fontsize=FONT_SIZE )
+        plt.ylabel('$f_2$', fontsize=FONT_SIZE )
+
+        ref_vec_norm = ref_vec / np.linalg.norm(ref_vec, axis=1, keepdims=True)
+        for ref in ref_vec_norm:
+            plt.plot([0, ref[0]], [0, ref[1]], c='k')
+    elif problem.n_obj == 3:
+        fig = plt.figure()
+        ax = fig.add_subplot(projection='3d')
+        ax.scatter(alg.pop.F[:, 0], alg.pop.F[:, 1], alg.pop.F[:, 2], c='none', edgecolors='r')
+        ax.set_xlabel('$f_1$', fontsize=FONT_SIZE)
+        ax.set_ylabel('$f_2$', fontsize=FONT_SIZE)
+        ax.set_zlabel('$f_3$', fontsize=FONT_SIZE)
+    else:
+        assert False, 'n_obj should be 2 or 3'
+
+    plt.show()
+
```

### Comparing `libmoon-0.1.9/libmoon/solver/moea/utils/__init__.py` & `libmoon-0.2.1/libmoon/solver/moea/utils/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from solver.moea.utils.decomposition import weighted_sum
-from solver.moea.utils.decomposition import Tchebycheff, modified_Tchebycheff
-
-from solver.moea.utils.decomposition import penalty_boundary_intersection
-from solver.moea.utils.utils_ea import dominance_min
-
-def get_decomposition(name):
-
-    decom_methods = {
-        "ws": weighted_sum,
-        "tch": Tchebycheff,
-        "mtch": modified_Tchebycheff,
-        "pbi": penalty_boundary_intersection,
-    }
-
-    if name not in decom_methods:
-        raise Exception("Decomposition method not found.")
-
+from solver.moea.utils.decomposition import weighted_sum
+from solver.moea.utils.decomposition import Tchebycheff, modified_Tchebycheff
+
+from solver.moea.utils.decomposition import penalty_boundary_intersection
+from solver.moea.utils.utils_ea import dominance_min
+
+def get_decomposition(name):
+
+    decom_methods = {
+        "ws": weighted_sum,
+        "tch": Tchebycheff,
+        "mtch": modified_Tchebycheff,
+        "pbi": penalty_boundary_intersection,
+    }
+
+    if name not in decom_methods:
+        raise Exception("Decomposition method not found.")
+
     return decom_methods[name]
```

### Comparing `libmoon-0.1.9/libmoon/solver/moea/utils/decomposition.py` & `libmoon-0.2.1/libmoon/solver/moea/utils/decomposition.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import numpy as np 
-from numpy import linalg as LA
-
-
-def weighted_sum(f: np.ndarray, 
-                 lamda: np.ndarray
-                 ) -> np.ndarray: 
-
-    assert f.ndim * lamda.ndim == 1 
-    return np.sum(f * lamda)
-
-def Tchebycheff(f: np.ndarray, 
-                lamda: np.ndarray, 
-                ref_point: np.ndarray, 
-                ) -> np.ndarray: 
-    
-    assert f.ndim * lamda.ndim * ref_point.ndim == 1 
-    return np.max(lamda * (f-ref_point))
-
-def modified_Tchebycheff(f: np.ndarray,
-                         lamda: np.ndarray,
-                         ref_point: np.ndarray,
-                         ) -> np.ndarray:
-
-    return Tchebycheff(f, 1/lamda, ref_point)
-
-
-
-def penalty_boundary_intersection(f: np.ndarray, 
-                                  lamda: np.ndarray, 
-                                  ref_point: np.ndarray, 
-                                  theta: float, 
-                                  ) -> np.ndarray: 
-    
-    assert f.ndim * lamda.ndim * ref_point.ndim == 1 
-    d1 = np.dot(f-ref_point, lamda) / LA.norm(lamda) 
-    d2 = LA.norm(f - (ref_point+d1*lamda))
+import numpy as np 
+from numpy import linalg as LA
+
+
+def weighted_sum(f: np.ndarray, 
+                 lamda: np.ndarray
+                 ) -> np.ndarray: 
+
+    assert f.ndim * lamda.ndim == 1 
+    return np.sum(f * lamda)
+
+def Tchebycheff(f: np.ndarray, 
+                lamda: np.ndarray, 
+                ref_point: np.ndarray, 
+                ) -> np.ndarray: 
+    
+    assert f.ndim * lamda.ndim * ref_point.ndim == 1 
+    return np.max(lamda * (f-ref_point))
+
+def modified_Tchebycheff(f: np.ndarray,
+                         lamda: np.ndarray,
+                         ref_point: np.ndarray,
+                         ) -> np.ndarray:
+
+    return Tchebycheff(f, 1/lamda, ref_point)
+
+
+
+def penalty_boundary_intersection(f: np.ndarray, 
+                                  lamda: np.ndarray, 
+                                  ref_point: np.ndarray, 
+                                  theta: float, 
+                                  ) -> np.ndarray: 
+    
+    assert f.ndim * lamda.ndim * ref_point.ndim == 1 
+    d1 = np.dot(f-ref_point, lamda) / LA.norm(lamda) 
+    d2 = LA.norm(f - (ref_point+d1*lamda))
     return d1 + theta * d2
```

### Comparing `libmoon-0.1.9/libmoon/solver/moea/utils/genetic_operator.py` & `libmoon-0.2.1/libmoon/solver/moea/utils/genetic_operator.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-import numpy as np 
-
-from solver.moea.utils.utils_ea import repair_clamp
-
-
-
-
-
-def cross_sbx(X, xl, xu, eta=15, prob_var=0.5, prob_bin=0.5, eps=1.0e-14, n_offsprings=1):
-    n_parents, n_var = X.shape
-
-    # the probability of a crossover for each of the variables
-    cross = np.random.random((n_var)) < prob_var
-
-    # when solutions are too close -> do not apply sbx crossover
-    too_close = np.abs(X[0] - X[1]) <= eps
-
-    # disable if two individuals are already too close
-    cross[too_close] = False
-    # disable crossover when lower and upper bound are identical
-    cross[xl == xu] = False
-
-    # assign y1 the smaller and y2 the larger value
-    y1 = np.min(X, axis=0)[cross]
-    y2 = np.max(X, axis=0)[cross]
-
-    # mask all the values that should be crossovered
-    _xl = xl[cross]
-    _xu = xu[cross]
-    eta = np.full((n_var, ), eta)[cross]
-    prob_bin = np.full((n_var, ), prob_bin)[cross]
-
-
-    # random values for each individual
-    rand = np.random.random(len(eta))
-    def calc_betaq(beta):
-        alpha = 2.0 - np.power(beta, -(eta + 1.0))
-
-        mask, mask_not = (rand <= (1.0 / alpha)), (rand > (1.0 / alpha))
-
-        betaq = np.zeros(mask.shape)
-        betaq[mask] = np.power((rand * alpha), (1.0 / (eta + 1.0)))[mask]
-        betaq[mask_not] = np.power((1.0 / (2.0 - rand * alpha)), (1.0 / (eta + 1.0)))[mask_not]
-
-        return betaq
-
-    # difference between all variables
-    delta = (y2 - y1)
-
-    beta = 1.0 + (2.0 * (y1 - _xl) / delta)
-    betaq = calc_betaq(beta)
-    c1 = 0.5 * ((y1 + y2) - betaq * delta)
-
-    beta = 1.0 + (2.0 * (_xu - y2) / delta)
-    betaq = calc_betaq(beta)
-    c2 = 0.5 * ((y1 + y2) + betaq * delta)
-
-    # with the given probability either assign the value from the first or second parent
-    b = np.random.random(len(prob_bin)) < prob_bin
-    tmp = np.copy(c1[b])
-    c1[b] = c2[b]
-    c2[b] = tmp
-
-    # first copy the unmodified parents
-    Q = np.copy(X)
-
-    # copy the positions where the crossover was done
-    Q[0, cross] = c1
-    Q[1, cross] = c2
-
-    Q[0] = repair_clamp(Q[0], xl, xu)
-    Q[1] = repair_clamp(Q[1], xl, xu)
-
-    if n_offsprings == 1:
-        rand = np.random.random() < 0.5
-        Q[0, rand] = Q[1, rand]
-        Q = Q[[0]]
-
-    return Q
-
-
-def mut_pm(X, xl, xu, eta=15, prob=None, at_least_once=False):
-    n, n_var = X.shape
-    if prob is None: prob = min(0.5, 1 / n_var) 
-
-    eta = np.full((n,), eta)
-    prob = np.full((n,), prob)
-
-    Xp = np.full(X.shape, np.inf)
-
-    mut = mut_binomial(n, n_var, prob, at_least_once=at_least_once)
-    mut[:, xl == xu] = False
-
-    Xp[:, :] = X
-
-    _xl = np.repeat(xl[None, :], X.shape[0], axis=0)[mut]
-    _xu = np.repeat(xu[None, :], X.shape[0], axis=0)[mut]
-
-    X = X[mut]
-    eta = np.tile(eta[:, None], (1, n_var))[mut]
-
-    delta1 = (X - _xl) / (_xu - _xl)
-    delta2 = (_xu - X) / (_xu - _xl)
-
-    mut_pow = 1.0 / (eta + 1.0)
-
-    rand = np.random.random(X.shape)
-    mask = rand <= 0.5
-    mask_not = np.logical_not(mask)
-
-    deltaq = np.zeros(X.shape)
-
-    xy = 1.0 - delta1
-    val = 2.0 * rand + (1.0 - 2.0 * rand) * (np.power(xy, (eta + 1.0)))
-    d = np.power(val, mut_pow) - 1.0
-    deltaq[mask] = d[mask]
-
-    xy = 1.0 - delta2
-    val = 2.0 * (1.0 - rand) + 2.0 * (rand - 0.5) * (np.power(xy, (eta + 1.0)))
-    d = 1.0 - (np.power(val, mut_pow))
-    deltaq[mask_not] = d[mask_not]
-
-    # mutated values
-    _Y = X + deltaq * (_xu - _xl)
-
-    # back in bounds if necessary (floating point issues)
-    _Y[_Y < _xl] = _xl[_Y < _xl]
-    _Y[_Y > _xu] = _xu[_Y > _xu]
-
-    # set the values for output
-    Xp[mut] = _Y
-
-    return Xp
-
-
-def row_at_least_once_true(M):
-    _, d = M.shape
-    for k in np.where(~np.any(M, axis=1))[0]:
-        M[k, np.random.randint(d)] = True
-    return M
-
-
-def mut_binomial(n, m, prob, at_least_once=True):
-    prob = np.ones(n) * prob
-    M = np.random.random((n, m)) < prob[:, None]
-
-    if at_least_once:
-        M = row_at_least_once_true(M)
-
-    return M
-
-
-
-
-
+import numpy as np 
+
+from solver.moea.utils.utils_ea import repair_clamp
+
+
+
+
+
+def cross_sbx(X, xl, xu, eta=15, prob_var=0.5, prob_bin=0.5, eps=1.0e-14, n_offsprings=1):
+    n_parents, n_var = X.shape
+
+    # the probability of a crossover for each of the variables
+    cross = np.random.random((n_var)) < prob_var
+
+    # when solutions are too close -> do not apply sbx crossover
+    too_close = np.abs(X[0] - X[1]) <= eps
+
+    # disable if two individuals are already too close
+    cross[too_close] = False
+    # disable crossover when lower and upper bound are identical
+    cross[xl == xu] = False
+
+    # assign y1 the smaller and y2 the larger value
+    y1 = np.min(X, axis=0)[cross]
+    y2 = np.max(X, axis=0)[cross]
+
+    # mask all the values that should be crossovered
+    _xl = xl[cross]
+    _xu = xu[cross]
+    eta = np.full((n_var, ), eta)[cross]
+    prob_bin = np.full((n_var, ), prob_bin)[cross]
+
+
+    # random values for each individual
+    rand = np.random.random(len(eta))
+    def calc_betaq(beta):
+        alpha = 2.0 - np.power(beta, -(eta + 1.0))
+
+        mask, mask_not = (rand <= (1.0 / alpha)), (rand > (1.0 / alpha))
+
+        betaq = np.zeros(mask.shape)
+        betaq[mask] = np.power((rand * alpha), (1.0 / (eta + 1.0)))[mask]
+        betaq[mask_not] = np.power((1.0 / (2.0 - rand * alpha)), (1.0 / (eta + 1.0)))[mask_not]
+
+        return betaq
+
+    # difference between all variables
+    delta = (y2 - y1)
+
+    beta = 1.0 + (2.0 * (y1 - _xl) / delta)
+    betaq = calc_betaq(beta)
+    c1 = 0.5 * ((y1 + y2) - betaq * delta)
+
+    beta = 1.0 + (2.0 * (_xu - y2) / delta)
+    betaq = calc_betaq(beta)
+    c2 = 0.5 * ((y1 + y2) + betaq * delta)
+
+    # with the given probability either assign the value from the first or second parent
+    b = np.random.random(len(prob_bin)) < prob_bin
+    tmp = np.copy(c1[b])
+    c1[b] = c2[b]
+    c2[b] = tmp
+
+    # first copy the unmodified parents
+    Q = np.copy(X)
+
+    # copy the positions where the crossover was done
+    Q[0, cross] = c1
+    Q[1, cross] = c2
+
+    Q[0] = repair_clamp(Q[0], xl, xu)
+    Q[1] = repair_clamp(Q[1], xl, xu)
+
+    if n_offsprings == 1:
+        rand = np.random.random() < 0.5
+        Q[0, rand] = Q[1, rand]
+        Q = Q[[0]]
+
+    return Q
+
+
+def mut_pm(X, xl, xu, eta=15, prob=None, at_least_once=False):
+    n, n_var = X.shape
+    if prob is None: prob = min(0.5, 1 / n_var) 
+
+    eta = np.full((n,), eta)
+    prob = np.full((n,), prob)
+
+    Xp = np.full(X.shape, np.inf)
+
+    mut = mut_binomial(n, n_var, prob, at_least_once=at_least_once)
+    mut[:, xl == xu] = False
+
+    Xp[:, :] = X
+
+    _xl = np.repeat(xl[None, :], X.shape[0], axis=0)[mut]
+    _xu = np.repeat(xu[None, :], X.shape[0], axis=0)[mut]
+
+    X = X[mut]
+    eta = np.tile(eta[:, None], (1, n_var))[mut]
+
+    delta1 = (X - _xl) / (_xu - _xl)
+    delta2 = (_xu - X) / (_xu - _xl)
+
+    mut_pow = 1.0 / (eta + 1.0)
+
+    rand = np.random.random(X.shape)
+    mask = rand <= 0.5
+    mask_not = np.logical_not(mask)
+
+    deltaq = np.zeros(X.shape)
+
+    xy = 1.0 - delta1
+    val = 2.0 * rand + (1.0 - 2.0 * rand) * (np.power(xy, (eta + 1.0)))
+    d = np.power(val, mut_pow) - 1.0
+    deltaq[mask] = d[mask]
+
+    xy = 1.0 - delta2
+    val = 2.0 * (1.0 - rand) + 2.0 * (rand - 0.5) * (np.power(xy, (eta + 1.0)))
+    d = 1.0 - (np.power(val, mut_pow))
+    deltaq[mask_not] = d[mask_not]
+
+    # mutated values
+    _Y = X + deltaq * (_xu - _xl)
+
+    # back in bounds if necessary (floating point issues)
+    _Y[_Y < _xl] = _xl[_Y < _xl]
+    _Y[_Y > _xu] = _xu[_Y > _xu]
+
+    # set the values for output
+    Xp[mut] = _Y
+
+    return Xp
+
+
+def row_at_least_once_true(M):
+    _, d = M.shape
+    for k in np.where(~np.any(M, axis=1))[0]:
+        M[k, np.random.randint(d)] = True
+    return M
+
+
+def mut_binomial(n, m, prob, at_least_once=True):
+    prob = np.ones(n) * prob
+    M = np.random.random((n, m)) < prob[:, None]
+
+    if at_least_once:
+        M = row_at_least_once_true(M)
+
+    return M
+
+
+
+
+
```

### Comparing `libmoon-0.1.9/libmoon/solver/moea/utils/utils_ea.py` & `libmoon-0.2.1/libmoon/solver/moea/utils/utils_ea.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-import numpy as np 
-
-
-
-
-def population_initialization(n_pop, 
-                              problem, 
-                              method: str='random'): 
-    
-    lb = problem.get_lower_bound
-    ub = problem.get_upper_bound 
-    dim = problem.get_number_variable
-    if method == 'random': 
-        return lb + (ub - lb) * np.random.rand(n_pop, dim)
-
-
-def repair_clamp(Xp, xl, xu):
-
-    I = np.where(Xp < xl)
-    Xp[I] = xl[I]
-
-    I = np.where(Xp > xu)
-    Xp[I] = xu[I]
-
-    return Xp
-
-
-def dominance_min(u, v): 
-    assert u.ndim * v.ndim == 1
-    assert len(u) == len(v) 
-    for i in range(len(u)):
-        if v[i] < u[i]: return False
-    if (u==v).all(): return False
-    return True
-
-
-
-def neighborhood_selection(n_pop, neighbors, n_selects=2, prob=.9): 
-
-    assert neighbors.ndim == 1 
-
-    if np.random.random() < prob:
-        P = np.random.choice(neighbors, n_selects, replace=False)
-    else:
-        P = np.random.permutation(n_pop)[:n_selects]
-
-    return P
-
-
-
-def OperatorDE(Parent1, Parent2, Parent3, mop):
-    '''
-        generate one offspring by P1 + 0.5*(P2-P3) and polynomial mutation.
-    '''
-    # Parameter
-    CR = 1
-    F = 0.5
-    proM = 1
-    disM = 20
-    #
-    N, D = Parent1.shape
-    # Differental evolution
-    Site = np.random.rand(N, D) < CR
-    Offspring = Parent1.copy()
-    Offspring[Site] = Offspring[Site] + F * (Parent2[Site] - Parent3[Site])
-    # Polynomial mutation
-    Lower = np.atleast_2d( mop.get_lower_bound )  # numpy  Upper=np.array(Upper)[None,:]
-    Upper = np.atleast_2d( mop.get_upper_bound)  # Lower = np.atleast_2d(Lower)
-    U_L = Upper - Lower
-    Site = np.random.rand(N, D) < proM / D
-    mu = np.random.rand(N, D)
-    temp = np.logical_and(Site, mu <= 0.5)
-    Offspring = np.minimum(np.maximum(Offspring, Lower), Upper)
-    delta1 = (Offspring - Lower) / U_L
-    delta2 = (Upper - Offspring) / U_L
-    #  mu <= 0.5
-    val = 2. * mu + (1 - 2. * mu) * (np.power(1. - delta1, disM + 1))
-    Offspring[temp] = Offspring[temp] + (np.power(val[temp], 1.0 / (disM + 1)) - 1.) * U_L[temp]
-    # mu > 0.5
-    temp = np.logical_and(Site, mu > 0.5)
-    val = 2. * (1.0 - mu) + 2. * (mu - 0.5) * (np.power(1. - delta2, disM + 1))
-    Offspring[temp] = Offspring[temp] + (1.0 - np.power(val[temp], 1.0 / (disM + 1))) * U_L[temp]
-
-    return Offspring
-
-
-
-
-
-
-if __name__ == '__main__':
-    from libmoon.problem.synthetic.zdt import ZDT1
-
-    problem = ZDT1()
-
-    # p1 = np.array( [[1,2,3],] )
-    # p2 = np.array( [[2,3,4],] )
-
-    p1 = np.random.random( (1, 30) )
-    p2 = np.random.random( (1, 30) )
-    p3 = np.random.random( (1, 30) )
-
-
-    print(p1)
-    print(p2)
-
-    res = _OperatorDE(p1, p2, p1, problem)
-    print( res )
-
+import numpy as np 
+
+
+
+
+def population_initialization(n_pop, 
+                              problem, 
+                              method: str='random'): 
+    
+    lb = problem.get_lower_bound
+    ub = problem.get_upper_bound 
+    dim = problem.get_number_variable
+    if method == 'random': 
+        return lb + (ub - lb) * np.random.rand(n_pop, dim)
+
+
+def repair_clamp(Xp, xl, xu):
+
+    I = np.where(Xp < xl)
+    Xp[I] = xl[I]
+
+    I = np.where(Xp > xu)
+    Xp[I] = xu[I]
+
+    return Xp
+
+
+def dominance_min(u, v): 
+    assert u.ndim * v.ndim == 1
+    assert len(u) == len(v) 
+    for i in range(len(u)):
+        if v[i] < u[i]: return False
+    if (u==v).all(): return False
+    return True
+
+
+
+def neighborhood_selection(n_pop, neighbors, n_selects=2, prob=.9): 
+
+    assert neighbors.ndim == 1 
+
+    if np.random.random() < prob:
+        P = np.random.choice(neighbors, n_selects, replace=False)
+    else:
+        P = np.random.permutation(n_pop)[:n_selects]
+
+    return P
+
+
+
+def OperatorDE(Parent1, Parent2, Parent3, mop):
+    '''
+        generate one offspring by P1 + 0.5*(P2-P3) and polynomial mutation.
+    '''
+    # Parameter
+    CR = 1
+    F = 0.5
+    proM = 1
+    disM = 20
+    #
+    N, D = Parent1.shape
+    # Differental evolution
+    Site = np.random.rand(N, D) < CR
+    Offspring = Parent1.copy()
+    Offspring[Site] = Offspring[Site] + F * (Parent2[Site] - Parent3[Site])
+    # Polynomial mutation
+    Lower = np.atleast_2d( mop.get_lower_bound )  # numpy  Upper=np.array(Upper)[None,:]
+    Upper = np.atleast_2d( mop.get_upper_bound)  # Lower = np.atleast_2d(Lower)
+    U_L = Upper - Lower
+    Site = np.random.rand(N, D) < proM / D
+    mu = np.random.rand(N, D)
+    temp = np.logical_and(Site, mu <= 0.5)
+    Offspring = np.minimum(np.maximum(Offspring, Lower), Upper)
+    delta1 = (Offspring - Lower) / U_L
+    delta2 = (Upper - Offspring) / U_L
+    #  mu <= 0.5
+    val = 2. * mu + (1 - 2. * mu) * (np.power(1. - delta1, disM + 1))
+    Offspring[temp] = Offspring[temp] + (np.power(val[temp], 1.0 / (disM + 1)) - 1.) * U_L[temp]
+    # mu > 0.5
+    temp = np.logical_and(Site, mu > 0.5)
+    val = 2. * (1.0 - mu) + 2. * (mu - 0.5) * (np.power(1. - delta2, disM + 1))
+    Offspring[temp] = Offspring[temp] + (1.0 - np.power(val[temp], 1.0 / (disM + 1))) * U_L[temp]
+
+    return Offspring
+
+
+
+
+
+
+if __name__ == '__main__':
+    from libmoon.problem.synthetic.zdt import ZDT1
+
+    problem = ZDT1()
+
+    # p1 = np.array( [[1,2,3],] )
+    # p2 = np.array( [[2,3,4],] )
+
+    p1 = np.random.random( (1, 30) )
+    p2 = np.random.random( (1, 30) )
+    p3 = np.random.random( (1, 30) )
+
+
+    print(p1)
+    print(p2)
+
+    res = _OperatorDE(p1, p2, p1, problem)
+    print( res )
+
```

### Comparing `libmoon-0.1.9/libmoon/solver/psl/model/mtl.py` & `libmoon-0.2.1/libmoon/solver/psl/model/mtl.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-import torch
-from torch import nn
-from libmoon.util_global.constant import get_param_num
-
-import torch.nn.functional as F
-
-
-class HyperNet(nn.Module):
-    def __init__(self,
-        kernel_size,
-        ray_hidden_dim=100,
-        out_dim=10,
-        target_hidden_dim=50,
-        n_kernels=10,
-        n_conv_layers=2,
-        n_hidden=1,
-        n_tasks=2):
-
-        super().__init__()
-        self.n_conv_layers = n_conv_layers
-        self.n_hidden = n_hidden
-        self.n_tasks = n_tasks
-
-        assert len(kernel_size) == n_conv_layers, (
-            'kernel size should be the same as the number of conv layers'
-            'conv layers holding kernel size for earch conv layer'
-        )
-
-        self.ray_mlp = nn.Sequential(
-            nn.Linear(2, ray_hidden_dim),
-            nn.ReLU(inplace=True),
-            nn.Linear(ray_hidden_dim, ray_hidden_dim),
-            nn.ReLU(inplace=True),
-            nn.Linear(ray_hidden_dim, ray_hidden_dim)
-        )
-
-        self.conv_0_weights = nn.Linear(
-            ray_hidden_dim, n_kernels * kernel_size[0] * kernel_size[0]     # n_kernel : 10
-        )
-        # output_size: 10*9*9
-
-        self.conv_0_bias = nn.Linear(ray_hidden_dim, n_kernels)
-        for i in range(1, n_conv_layers):
-            # previous number of kernels.
-            p = 2**(i-1) * n_kernels
-            # current number of kernels
-            c = 2**i*n_kernels
-            setattr(
-                self, f"conv_{i}_weights", nn.Linear(ray_hidden_dim, c*p*kernel_size[i]*kernel_size[i]),
-            )
-            setattr(self, f"conv_{i}_bias", nn.Linear(ray_hidden_dim, c))
-
-        latent = 25
-        self.hidden_0_weights = nn.Linear(
-            ray_hidden_dim, target_hidden_dim * 2 ** i * n_kernels * latent   # self.hidden_0_weights: 100 -> 25000
-        )
-
-        self.hidden_0_bias = nn.Linear(ray_hidden_dim, target_hidden_dim)
-        for j in range(n_tasks):
-            setattr(
-                self,
-                f"task_{j}_weights",
-                nn.Linear(ray_hidden_dim, target_hidden_dim * out_dim)
-            )
-            setattr(self, f"task_{j}_bias", nn.Linear(ray_hidden_dim, out_dim))
-
-    def shared_parameters(self):
-        return list([p for n,p in self.named_parameters() if 'task' not in n])
-
-    def forward(self, ray):
-        features = self.ray_mlp(ray)
-        # features.shape: (batch_size, ray_hidden_dim)
-        out_dict={}  # task 1, task 2. Task specfic parameters.
-        # features.shape : [128, 100]
-
-        layer_types = ['conv', 'hidden', 'task']
-        for i in layer_types:
-            # Sequential layers. Two convs, two hiddens, two tasks.
-            if i == 'conv':
-                n_layers = self.n_conv_layers
-            elif i == 'hidden':
-                n_layers = self.n_hidden
-            elif i == 'task':
-                n_layers = self.n_tasks
-
-            for j in range( n_layers ):
-                out_dict[f"{i}{j}.weights"] = getattr(self, f"{i}_{j}_weights")(
-                    features
-                )
-
-                out_dict[f"{i}{j}.bias"] = getattr(self, f"{i}_{j}_bias")(
-                    features
-                ).flatten()
-
-        return out_dict
-
-
-
-class LeNetTarget(nn.Module):
-    '''
-        LeNet target network
-    '''
-    def __init__(self,
-                 kernel_size,
-                 n_kernels=10,
-                 out_dim=10,
-                 target_hidden_dim=50,
-                 n_conv_layers=2,
-                 n_tasks=2
-                 ):
-
-        super().__init__()
-        assert len(kernel_size) == n_conv_layers, (
-            'kernel size should be the same as the number of conv layers'
-            'conv layers holding kernel size for earch conv layer'
-        )
-        self.n_kernels = n_kernels
-        self.kernel_size= kernel_size
-        self.out_dim = out_dim
-        self.n_conv_layers = n_conv_layers
-        self.n_tasks = n_tasks
-        self.target_hidden_dim= target_hidden_dim
-
-    def forward(self, x, weights=None):
-        # weights['conv0.weights'].shape : (bs, 810)
-        x = F.conv2d(
-            x,
-            weight = weights['conv0.weights'].reshape(
-                self.n_kernels, 1, self.kernel_size[0], self.kernel_size[0]
-            ),
-            bias=weights['conv0.bias'],
-            stride=1,
-        )
-
-        x = F.relu(x)
-        x = F.max_pool2d(x, 2)
-
-        for i in range(1, self.n_conv_layers):
-            x = F.conv2d(
-                x,
-                weight = weights[f"conv{i}.weights"].reshape(
-                    int(2**i * self.n_kernels), int(2**(i-1) * self.n_kernels), self.kernel_size[i], self.kernel_size[i]
-                ),
-                bias=weights[f"conv{i}.bias"],
-                stride=1,
-            )
-            x = F.relu(x)
-            x = F.max_pool2d(x, 2)
-
-        x = torch.flatten(x, 1)
-
-        x = F.linear(
-            x,
-            weight = weights['hidden0.weights'].reshape(
-                self.target_hidden_dim, x.shape[-1]
-            ),
-            bias=weights['hidden0.bias'],
-        )
-
-        logits = []
-        for j in range(self.n_tasks):
-            logits.append(
-                F.linear(
-                    x,
-                    weight = weights[f"task{j}.weights"].reshape(
-                        self.out_dim, self.target_hidden_dim
-                    ),
-                    bias=weights[f"task{j}.bias"],
-                )
-            )
-
-        return logits
-
-
-
-if __name__ == '__main__':
-    prefs = torch.rand(10, 2)
-    hyper_model = HyperNet(kernel_size=[5,5])
-    model_num = get_param_num(hyper_model)   #model num: 3,186,850. It is too large, unacceptable.
-    print('model_num', model_num)
-    out_dict = hyper_model(prefs)
+import torch
+from torch import nn
+from libmoon.util_global.constant import get_param_num
+
+import torch.nn.functional as F
+
+
+class HyperNet(nn.Module):
+    def __init__(self,
+        kernel_size,
+        ray_hidden_dim=100,
+        out_dim=10,
+        target_hidden_dim=50,
+        n_kernels=10,
+        n_conv_layers=2,
+        n_hidden=1,
+        n_tasks=2):
+
+        super().__init__()
+        self.n_conv_layers = n_conv_layers
+        self.n_hidden = n_hidden
+        self.n_tasks = n_tasks
+
+        assert len(kernel_size) == n_conv_layers, (
+            'kernel size should be the same as the number of conv layers'
+            'conv layers holding kernel size for earch conv layer'
+        )
+
+        self.ray_mlp = nn.Sequential(
+            nn.Linear(2, ray_hidden_dim),
+            nn.ReLU(inplace=True),
+            nn.Linear(ray_hidden_dim, ray_hidden_dim),
+            nn.ReLU(inplace=True),
+            nn.Linear(ray_hidden_dim, ray_hidden_dim)
+        )
+
+        self.conv_0_weights = nn.Linear(
+            ray_hidden_dim, n_kernels * kernel_size[0] * kernel_size[0]     # n_kernel : 10
+        )
+        # output_size: 10*9*9
+
+        self.conv_0_bias = nn.Linear(ray_hidden_dim, n_kernels)
+        for i in range(1, n_conv_layers):
+            # previous number of kernels.
+            p = 2**(i-1) * n_kernels
+            # current number of kernels
+            c = 2**i*n_kernels
+            setattr(
+                self, f"conv_{i}_weights", nn.Linear(ray_hidden_dim, c*p*kernel_size[i]*kernel_size[i]),
+            )
+            setattr(self, f"conv_{i}_bias", nn.Linear(ray_hidden_dim, c))
+
+        latent = 25
+        self.hidden_0_weights = nn.Linear(
+            ray_hidden_dim, target_hidden_dim * 2 ** i * n_kernels * latent   # self.hidden_0_weights: 100 -> 25000
+        )
+
+        self.hidden_0_bias = nn.Linear(ray_hidden_dim, target_hidden_dim)
+        for j in range(n_tasks):
+            setattr(
+                self,
+                f"task_{j}_weights",
+                nn.Linear(ray_hidden_dim, target_hidden_dim * out_dim)
+            )
+            setattr(self, f"task_{j}_bias", nn.Linear(ray_hidden_dim, out_dim))
+
+    def shared_parameters(self):
+        return list([p for n,p in self.named_parameters() if 'task' not in n])
+
+    def forward(self, ray):
+        features = self.ray_mlp(ray)
+        # features.shape: (batch_size, ray_hidden_dim)
+        out_dict={}  # task 1, task 2. Task specfic parameters.
+        # features.shape : [128, 100]
+
+        layer_types = ['conv', 'hidden', 'task']
+        for i in layer_types:
+            # Sequential layers. Two convs, two hiddens, two tasks.
+            if i == 'conv':
+                n_layers = self.n_conv_layers
+            elif i == 'hidden':
+                n_layers = self.n_hidden
+            elif i == 'task':
+                n_layers = self.n_tasks
+
+            for j in range( n_layers ):
+                out_dict[f"{i}{j}.weights"] = getattr(self, f"{i}_{j}_weights")(
+                    features
+                )
+
+                out_dict[f"{i}{j}.bias"] = getattr(self, f"{i}_{j}_bias")(
+                    features
+                ).flatten()
+
+        return out_dict
+
+
+
+class LeNetTarget(nn.Module):
+    '''
+        LeNet target network
+    '''
+    def __init__(self,
+                 kernel_size,
+                 n_kernels=10,
+                 out_dim=10,
+                 target_hidden_dim=50,
+                 n_conv_layers=2,
+                 n_tasks=2
+                 ):
+
+        super().__init__()
+        assert len(kernel_size) == n_conv_layers, (
+            'kernel size should be the same as the number of conv layers'
+            'conv layers holding kernel size for earch conv layer'
+        )
+        self.n_kernels = n_kernels
+        self.kernel_size= kernel_size
+        self.out_dim = out_dim
+        self.n_conv_layers = n_conv_layers
+        self.n_tasks = n_tasks
+        self.target_hidden_dim= target_hidden_dim
+
+    def forward(self, x, weights=None):
+        # weights['conv0.weights'].shape : (bs, 810)
+        x = F.conv2d(
+            x,
+            weight = weights['conv0.weights'].reshape(
+                self.n_kernels, 1, self.kernel_size[0], self.kernel_size[0]
+            ),
+            bias=weights['conv0.bias'],
+            stride=1,
+        )
+
+        x = F.relu(x)
+        x = F.max_pool2d(x, 2)
+
+        for i in range(1, self.n_conv_layers):
+            x = F.conv2d(
+                x,
+                weight = weights[f"conv{i}.weights"].reshape(
+                    int(2**i * self.n_kernels), int(2**(i-1) * self.n_kernels), self.kernel_size[i], self.kernel_size[i]
+                ),
+                bias=weights[f"conv{i}.bias"],
+                stride=1,
+            )
+            x = F.relu(x)
+            x = F.max_pool2d(x, 2)
+
+        x = torch.flatten(x, 1)
+
+        x = F.linear(
+            x,
+            weight = weights['hidden0.weights'].reshape(
+                self.target_hidden_dim, x.shape[-1]
+            ),
+            bias=weights['hidden0.bias'],
+        )
+
+        logits = []
+        for j in range(self.n_tasks):
+            logits.append(
+                F.linear(
+                    x,
+                    weight = weights[f"task{j}.weights"].reshape(
+                        self.out_dim, self.target_hidden_dim
+                    ),
+                    bias=weights[f"task{j}.bias"],
+                )
+            )
+
+        return logits
+
+
+
+if __name__ == '__main__':
+    prefs = torch.rand(10, 2)
+    hyper_model = HyperNet(kernel_size=[5,5])
+    model_num = get_param_num(hyper_model)   #model num: 3,186,850. It is too large, unacceptable.
+    print('model_num', model_num)
+    out_dict = hyper_model(prefs)
     # print()
```

### Comparing `libmoon-0.1.9/libmoon/solver/psl/run_mtl_condition.py` & `libmoon-0.2.1/libmoon/solver/psl/run_mtl_condition.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import torch
-import argparse
-import numpy as np
-# from util_global.constant import get_device
-from libmoon.problem.mtl.objectives import from_name
-from libmoon.util_global.constant import get_device
-
-loss_func_arr = from_name( names=['CrossEntropyLoss', 'CrossEntropyLoss'], task_names=['l', 'r'] )
-from model.mtl import HyperNet, LeNetTarget
-from libmoon.problem.mtl.loaders import MultiMNISTData
-from tqdm import tqdm
-
-from matplotlib import pyplot as plt
-
-
-
-if __name__ == '__main__':
-    parse = argparse.ArgumentParser()
-    parse.add_argument('--n-epoch', type=int, default=5)
-    parse.add_argument('--batch-size', type=int, default=128)
-    parse.add_argument('--lr', type=float, default=1e-3)
-    parse.add_argument('--n-obj', type=int, default=2)
-    parse.add_argument('--model', type=str, default='lenet')
-    parse.add_argument('--ray-hidden', type=int, default=100)
-
-    dataset = MultiMNISTData('mnist', 'train')
-    args = parse.parse_args()
-    loader = torch.utils.data.DataLoader(dataset, batch_size=args.batch_size, shuffle=True,
-                                              num_workers=0)
-    dataset_test = MultiMNISTData('mnist', 'test')
-    loader_test = torch.utils.data.DataLoader(dataset_test, batch_size=args.batch_size, shuffle=True,
-                                                   num_workers=0)
-
-    args.device = get_device()
-    if args.model == 'lenet':
-        hnet = HyperNet( [9,5] )
-        net = LeNetTarget( [9,5] )
-    else:
-        assert False, 'model not supported'
-
-    hnet.to(args.device)
-    optimizer = torch.optim.Adam(hnet.parameters(), lr=args.lr)
-
-
-
-    loss_history = []
-
-    for idx in tqdm(range( args.n_epoch)):
-        for i, batch in enumerate(loader):
-
-            ray = torch.from_numpy(
-                np.random.dirichlet((1, 1), 1).astype(np.float32).flatten()
-            ).to(args.device)  # ray.shape (1,2)
-
-            batch_ = {}
-            for k, v in batch.items():
-                batch_[k] = v.to(args.device)
-
-            hnet.train()
-            weights = hnet( ray )
-            logits_l, logits_r = net(batch_['data'], weights)
-
-            batch_['logits_l'] = logits_l
-            batch_['logits_r'] = logits_r
-
-            loss_arr = torch.stack([loss(**batch_) for loss in loss_func_arr])
-            # print()
-            optimizer.zero_grad()
-            loss = ray@loss_arr
-            (loss).backward()
-            loss_item = loss.cpu().detach().numpy()
-            loss_history.append(loss_item)
-
-            optimizer.step()
-
-
-    plt.plot( np.log( np.array(loss_history) )  )
-    plt.show()
-
-
+import torch
+import argparse
+import numpy as np
+# from util_global.constant import get_device
+from libmoon.problem.mtl.objectives import from_name
+from libmoon.util_global.constant import get_device
+
+loss_func_arr = from_name( names=['CrossEntropyLoss', 'CrossEntropyLoss'], task_names=['l', 'r'] )
+from model.mtl import HyperNet, LeNetTarget
+from libmoon.problem.mtl.loaders import MultiMNISTData
+from tqdm import tqdm
+
+from matplotlib import pyplot as plt
+
+
+
+if __name__ == '__main__':
+    parse = argparse.ArgumentParser()
+    parse.add_argument('--n-epoch', type=int, default=5)
+    parse.add_argument('--batch-size', type=int, default=128)
+    parse.add_argument('--lr', type=float, default=1e-3)
+    parse.add_argument('--n-obj', type=int, default=2)
+    parse.add_argument('--model', type=str, default='lenet')
+    parse.add_argument('--ray-hidden', type=int, default=100)
+
+    dataset = MultiMNISTData('mnist', 'train')
+    args = parse.parse_args()
+    loader = torch.utils.data.DataLoader(dataset, batch_size=args.batch_size, shuffle=True,
+                                              num_workers=0)
+    dataset_test = MultiMNISTData('mnist', 'test')
+    loader_test = torch.utils.data.DataLoader(dataset_test, batch_size=args.batch_size, shuffle=True,
+                                                   num_workers=0)
+
+    args.device = get_device()
+    if args.model == 'lenet':
+        hnet = HyperNet( [9,5] )
+        net = LeNetTarget( [9,5] )
+    else:
+        assert False, 'model not supported'
+
+    hnet.to(args.device)
+    optimizer = torch.optim.Adam(hnet.parameters(), lr=args.lr)
+
+
+
+    loss_history = []
+
+    for idx in tqdm(range( args.n_epoch)):
+        for i, batch in enumerate(loader):
+
+            ray = torch.from_numpy(
+                np.random.dirichlet((1, 1), 1).astype(np.float32).flatten()
+            ).to(args.device)  # ray.shape (1,2)
+
+            batch_ = {}
+            for k, v in batch.items():
+                batch_[k] = v.to(args.device)
+
+            hnet.train()
+            weights = hnet( ray )
+            logits_l, logits_r = net(batch_['data'], weights)
+
+            batch_['logits_l'] = logits_l
+            batch_['logits_r'] = logits_r
+
+            loss_arr = torch.stack([loss(**batch_) for loss in loss_func_arr])
+            # print()
+            optimizer.zero_grad()
+            loss = ray@loss_arr
+            (loss).backward()
+            loss_item = loss.cpu().detach().numpy()
+            loss_history.append(loss_item)
+
+            optimizer.step()
+
+
+    plt.plot( np.log( np.array(loss_history) )  )
+    plt.show()
+
+
```

### Comparing `libmoon-0.1.9/libmoon/solver/psl/run_mtl_psl.py` & `libmoon-0.2.1/libmoon/solver/psl/run_mtl_psl.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-import torch
-import argparse
-import numpy as np
-# from util_global.constant import get_device
-from libmoon.problem.mtl.objectives import from_name
-from libmoon.util_global.constant import get_device
-
-loss_func_arr = from_name( names=['CrossEntropyLoss', 'CrossEntropyLoss'], task_names=['l', 'r'] )
-from model.mtl import HyperNet, LeNetTarget
-from libmoon.problem.mtl.loaders import MultiMNISTData
-from tqdm import tqdm
-
-from matplotlib import pyplot as plt
-
-
-
-if __name__ == '__main__':
-    parse = argparse.ArgumentParser()
-    parse.add_argument('--n-epoch', type=int, default=5)
-    parse.add_argument('--batch-size', type=int, default=128)
-    parse.add_argument('--lr', type=float, default=1e-3)
-    parse.add_argument('--n-obj', type=int, default=2)
-    parse.add_argument('--model', type=str, default='lenet')
-    parse.add_argument('--ray-hidden', type=int, default=100)
-
-    dataset = MultiMNISTData('mnist', 'train')
-    args = parse.parse_args()
-    loader = torch.utils.data.DataLoader(dataset, batch_size=args.batch_size, shuffle=True,
-                                              num_workers=0)
-    dataset_test = MultiMNISTData('mnist', 'test')
-    loader_test = torch.utils.data.DataLoader(dataset_test, batch_size=args.batch_size, shuffle=True,
-                                                   num_workers=0)
-
-    args.device = get_device()
-    if args.model == 'lenet':
-        hnet = HyperNet( [9,5] )
-        net = LeNetTarget( [9,5] )
-    else:
-        assert False, 'model not supported'
-
-    hnet.to(args.device)
-    optimizer = torch.optim.Adam(hnet.parameters(), lr=args.lr)
-
-
-
-    loss_history = []
-
-    for idx in tqdm(range( args.n_epoch)):
-        for i, batch in enumerate(loader):
-
-            ray = torch.from_numpy(
-                np.random.dirichlet((1, 1), 1).astype(np.float32).flatten()
-            ).to(args.device)  # ray.shape (1,2)
-
-            batch_ = {}
-            for k, v in batch.items():
-                batch_[k] = v.to(args.device)
-
-            hnet.train()
-            weights = hnet( ray )
-            logits_l, logits_r = net(batch_['data'], weights)
-
-            batch_['logits_l'] = logits_l
-            batch_['logits_r'] = logits_r
-
-            loss_arr = torch.stack([loss(**batch_) for loss in loss_func_arr])
-            # print()
-            optimizer.zero_grad()
-            loss = ray@loss_arr
-            (loss).backward()
-            loss_item = loss.cpu().detach().numpy()
-            loss_history.append(loss_item)
-
-            optimizer.step()
-
-
-    plt.plot( np.log( np.array(loss_history) )  )
-    plt.show()
-
-
+import torch
+import argparse
+import numpy as np
+# from util_global.constant import get_device
+from libmoon.problem.mtl.objectives import from_name
+from libmoon.util_global.constant import get_device
+
+loss_func_arr = from_name( names=['CrossEntropyLoss', 'CrossEntropyLoss'], task_names=['l', 'r'] )
+from model.mtl import HyperNet, LeNetTarget
+from libmoon.problem.mtl.loaders import MultiMNISTData
+from tqdm import tqdm
+
+from matplotlib import pyplot as plt
+
+
+
+if __name__ == '__main__':
+    parse = argparse.ArgumentParser()
+    parse.add_argument('--n-epoch', type=int, default=5)
+    parse.add_argument('--batch-size', type=int, default=128)
+    parse.add_argument('--lr', type=float, default=1e-3)
+    parse.add_argument('--n-obj', type=int, default=2)
+    parse.add_argument('--model', type=str, default='lenet')
+    parse.add_argument('--ray-hidden', type=int, default=100)
+
+    dataset = MultiMNISTData('mnist', 'train')
+    args = parse.parse_args()
+    loader = torch.utils.data.DataLoader(dataset, batch_size=args.batch_size, shuffle=True,
+                                              num_workers=0)
+    dataset_test = MultiMNISTData('mnist', 'test')
+    loader_test = torch.utils.data.DataLoader(dataset_test, batch_size=args.batch_size, shuffle=True,
+                                                   num_workers=0)
+
+    args.device = get_device()
+    if args.model == 'lenet':
+        hnet = HyperNet( [9,5] )
+        net = LeNetTarget( [9,5] )
+    else:
+        assert False, 'model not supported'
+
+    hnet.to(args.device)
+    optimizer = torch.optim.Adam(hnet.parameters(), lr=args.lr)
+
+
+
+    loss_history = []
+
+    for idx in tqdm(range( args.n_epoch)):
+        for i, batch in enumerate(loader):
+
+            ray = torch.from_numpy(
+                np.random.dirichlet((1, 1), 1).astype(np.float32).flatten()
+            ).to(args.device)  # ray.shape (1,2)
+
+            batch_ = {}
+            for k, v in batch.items():
+                batch_[k] = v.to(args.device)
+
+            hnet.train()
+            weights = hnet( ray )
+            logits_l, logits_r = net(batch_['data'], weights)
+
+            batch_['logits_l'] = logits_l
+            batch_['logits_r'] = logits_r
+
+            loss_arr = torch.stack([loss(**batch_) for loss in loss_func_arr])
+            # print()
+            optimizer.zero_grad()
+            loss = ray@loss_arr
+            (loss).backward()
+            loss_item = loss.cpu().detach().numpy()
+            loss_history.append(loss_item)
+
+            optimizer.step()
+
+
+    plt.plot( np.log( np.array(loss_history) )  )
+    plt.show()
+
+
```

### Comparing `libmoon-0.1.9/libmoon/visulization/util.py` & `libmoon-0.2.1/libmoon/visulization/util.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import numpy as np
-from matplotlib import pyplot as plt
-from mpl_toolkits.mplot3d.art3d import Poly3DCollection
-
-
-def plot_simplex(ax, p1, p2, p3, color='k'):
-    # x1 = np.array([0, 0, 2])
-    # y1 = np.array([0, 2, 0])
-    # z1 = np.array([2, 0, 0])  # z1 should have 3 coordinates, right?
-    # ax.scatter(x1, y1, z1)
-    # 1. create vertices from points
-    verts = [list(zip(p1, p2, p3))]
-    # 2. create 3d polygons and specify parameters
-    srf = Poly3DCollection(verts, alpha=.25, facecolor='#800000')
-    # 3. add polygon to the figure (current axes)
-    plt.gca().add_collection3d(srf)
-
-
-def plot_unit_sphere(ax):
-    u, v = np.mgrid[0:np.pi / 2:30j, 0:np.pi / 2:20j]
-    x = np.cos(u) * np.sin(v)
-    y = np.sin(u) * np.sin(v)
-    z = np.cos(v)
+import numpy as np
+from matplotlib import pyplot as plt
+from mpl_toolkits.mplot3d.art3d import Poly3DCollection
+
+
+def plot_simplex(ax, p1, p2, p3, color='k'):
+    # x1 = np.array([0, 0, 2])
+    # y1 = np.array([0, 2, 0])
+    # z1 = np.array([2, 0, 0])  # z1 should have 3 coordinates, right?
+    # ax.scatter(x1, y1, z1)
+    # 1. create vertices from points
+    verts = [list(zip(p1, p2, p3))]
+    # 2. create 3d polygons and specify parameters
+    srf = Poly3DCollection(verts, alpha=.25, facecolor='#800000')
+    # 3. add polygon to the figure (current axes)
+    plt.gca().add_collection3d(srf)
+
+
+def plot_unit_sphere(ax):
+    u, v = np.mgrid[0:np.pi / 2:30j, 0:np.pi / 2:20j]
+    x = np.cos(u) * np.sin(v)
+    y = np.sin(u) * np.sin(v)
+    z = np.cos(v)
     ax.plot_surface(x, y, z, color='b', alpha=0.2)
```

### Comparing `libmoon-0.1.9/libmoon/visulization/view_res.py` & `libmoon-0.2.1/libmoon/visulization/view_res.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 from matplotlib import pyplot as plt
-from libmoon.util_global.constant import FONT_SIZE
+from libmoon.util_global.constant import FONT_SIZE, root_name
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
 
 
-
 def vis_res(res, problem, prefs, args):
     if args.n_obj == 2:
         fig = plt.figure(figsize=(8, 20))
         plt.subplot(3,1,1)
         plt.title(args.solver, fontsize=FONT_SIZE)
         plt.scatter(res['y'][:, 0], res['y'][:, 1], label='solution')
         pf = problem.get_pf()
@@ -71,20 +70,14 @@
 import matplotlib.animation as manimation
 from matplotlib.animation import PillowWriter
 
 from libmoon.util_global.constant import FONT_SIZE
 
 def vedio_res(res, problem, prefs, args):
     print('vedio making')
-    # print()
-    # FFMpegWriter = manimation.writers['ffmpeg']
-    metadata = dict(title='Movie Test', artist='Matplotlib',
-                    comment='a red circle following a blue sine wave')
-    # writer = PillowWriter(fps=15, metadata=metadata)
-    fps=15
     from matplotlib.animation import FuncAnimation
     from matplotlib.animation import FFMpegWriter
 
     # Create some data
     # x = np.linspace(0, 2 * np.pi, 100)
     # y = np.sin(x)
     subsample = 20
@@ -95,42 +88,55 @@
     fig, ax = plt.subplots()
     ax.set_xlim(0, 1.2)
     ax.set_ylim(0, 1.2)
 
     ax.set_xlabel('$f_1$', fontsize=FONT_SIZE)
     ax.set_ylabel('$f_2$', fontsize=FONT_SIZE)
 
-
     # Create a function to update the plot for each frame of the animation
+    if args.solver == 'agg':
+        file_name = '{}_{}_{}'.format(args.problem_name, args.solver, args.agg)
+    else:
+        file_name = '{}_{}'.format(args.problem_name, args.solver)
     def update(frame):
         ax.clear()
         ax.scatter(y_arr[frame][:,0], y_arr[frame][:,1])
+
+        pf = problem.get_pf()
+
+        ax.plot(pf[:,0], pf[:,1], 'k', linewidth=1)
+
         ax.set_xlim(0, 1.2)
         ax.set_ylim(0, 1.2)
-
         ax.set_xlabel('$f_1$', fontsize=FONT_SIZE)
         ax.set_ylabel('$f_2$', fontsize=FONT_SIZE)
 
+        ax.set_title(file_name, fontsize=FONT_SIZE)
+
+
     # Create the animation
     ani = FuncAnimation(fig, update, frames=n_frame, interval=100)
 
     # Define the writer for the animation using FFMpegWriter
     writer = FFMpegWriter(fps=15, metadata=dict(artist='Me'), bitrate=1800)
 
 
-    if args.solver == 'agg':
-        file_name = '{}_{}_{}.mp4'.format(args.problem_name, args.solver, args.agg)
-    else:
-        file_name = '{}_{}.mp4'.format(args.problem_name, args.solver)
+
+    import os
+    folder_name = os.path.join(root_name, 'solver', 'gradient', 'output')
+    mp4_file_name = os.path.join(folder_name, file_name + '.mp4')
+
 
 
     # Save the animation as a video file
-    ani.save(file_name, writer=writer)
+    ani.save(mp4_file_name, writer=writer)
+    print('Vedio saved: {}'.format(mp4_file_name))
 
-    plt.show()
+    if args.use_plt=='Y':
+        plt.show()
```

### Comparing `libmoon-0.1.9/libmoon.egg-info/PKG-INFO` & `libmoon-0.2.1/libmoon.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,184 +1,225 @@
-Metadata-Version: 2.1
-Name: libmoon
-Version: 0.1.9
-Summary: Moon, Make MOO great again
-Author: Xiaoyuan Zhang et al.
-Author-email: xzhang2523-c@my.cityu.edu.hk
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy==1.26.4
-Requires-Dist: torch==2.2.1
-Requires-Dist: matplotlib==3.8.3
-Requires-Dist: tqdm==4.66.2
-Requires-Dist: pymoo==0.6.1.1
-Requires-Dist: cvxopt==1.3.2
-Requires-Dist: cvxpy==1.4.2
-Requires-Dist: ffmpeg-python
-Requires-Dist: ffmpeg
-
-### Moon: A Standardized/Flexible Framework for MultiObjective OptimizatioN
-<img src="moon.png" alt="Moon" width="200">
-
-''
-    I raise my cup to invite the moon.
-    With my shadow we become three from one.
-''
--- Li Bai.
-
-Moon: is a multiobjective optimization framework, from single-objective optimization to multiobjective optimization, towards a better understanding of optimization problems and fair comparasions between MOO algorithms.
-
-
-
-Main contributors: Xiaoyuan Zhang (project leader), Ji Cheng, Liao Zhang, Weiduo Liao, Zhe Zhao, Xi Lin, Cheng Gong, Longcan Chen.
-
-Advised by: Prof. Yifan Chen, Prof. Zhichao Lu, Prof. Ke Shang, Prof. Tao Qin. 
-
-Corresponding to: Prof. Qingfu Zhang (CityU HK).
-
-
-
-(1) A standardlized gradient based framework. 
-
-- **Problem** class. For more problem details, please also check the Readme_problem.md file. 
-  (i) For synthetic problems,
-- 
-  | Problem                                                      | Paper                                                                | Project/Code                                         |
-  |--------------------------------------------------------------|----------------------------------------------------------------------|------------------------------------------------------|
-  | ZDT                                                          | [paper](https://ieeexplore.ieee.org/document/996017)                 | [project](https://pymoo.org/problems/multi/zdt.html) |
-  | DTLZ                                                         | [paper] | [project](https://pymoo.org/problems/many/dtlz.html) |Y                                        |
-  | MAF                                                          | [paper](https://link.springer.com/article/10.1007/s40747-017-0039-7) | [project]                         |
-  | [WFG](https://ieeexplore.ieee.org/document/996017) [code]()  | Real world problems.                                                 | Y                                                    |
-  | [Fi's](https://ieeexplore.ieee.org/document/996017) [code]() | Real world problems.                                                 | Y                                                    |
-  | RE                                                           | [paper](https://arxiv.org/abs/2009.12867)                            | [code](https://github.com/ryojitanabe/reproblems)    |
-
-
-(2) For multitask learning problems,
-
-| Problem                 | Paper | Project/Code |
-|-------------------------|------|--------------|
-| MO-MNISTs               | [PMTL](https://proceedings.neurips.cc/paper_files/paper/2019/file/685bfde03eb646c27ed565881917c71c-Paper.pdf)     | [COSMOS](https://github.com/ruchtem/cosmos)     |
-| Fairness Classification |[COSMOS](https://arxiv.org/pdf/2103.13392.pdf) |[COSMOS](https://github.com/ruchtem/cosmos) |
-| Federated Learning      | | |
-
-(3) For MORL problems,
-
-| Problem                 | Paper                                                                                                            | Project/Code                              |
-|-------------------------|------------------------------------------------------------------------------------------------------------------|-------------------------------------------|
-| Synthetic (DST FTS...)  | [Envelop](https://proceedings.neurips.cc/paper_files/paper/2019/file/4a46fbfca3f1465a27b210f4bdfe6ab3-Paper.pdf) | [code]()                                  |
-| Robotics (MO-MuJoCo...) | [PGMORL](http://proceedings.mlr.press/v119/xu20h/xu20h.pdf)                                                      | [code](https://github.com/mit-gfx/PGMORL) |
-
-
-
-
-- **Gradient-based Solver**.
-
-    | Method                                                                                                                                                                                | Property                                                              | #Obj               | Support | Published | Complexity      |
-    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------|--------------------|---------|----------|-----------------|
-    | [EPO](https://proceedings.mlr.press/v119/mahapatra20a/mahapatra20a.pdf) [code](https://github.com/dbmptr/EPOSearch)                                                                   | Exact solution.                                                       | Any                | Y       | ICML 2020 | $O(m^2 n K )$   |
-    | [COSMOS](https://arxiv.org/pdf/2103.13392.pdf) [code](https://github.com/ruchtem/cosmos)                                                                                              | Approximated exact solution.                                          | Any                | Y       | ICDM 2021| $O(m n K )$     |
-    | [MOO-SVGD](https://openreview.net/pdf?id=S2-j0ZegyrE) [code](https://github.com/gnobitab/MultiObjectiveSampling)                                                                      | A set of diverse Pareto solution.                                     | Any                | Y       | NeurIPS 2021 | $O(m^2 n K^2 )$ |
-    | [MGDA](https://proceedings.neurips.cc/paper/2018/file/432aca3a1e345e339f35a30c8f65edce-Paper.pdf) [code](https://github.com/intel-isl/MultiObjectiveOptimization)                     | Arbitray Pareto solutions. Location affected highly by initialization. | Any                | Y       | NeurIPS 2018 | $O(m^2 n K )$   |
-    | [PMTL](https://proceedings.neurips.cc/paper_files/paper/2019/file/685bfde03eb646c27ed565881917c71c-Paper.pdf) [code](https://github.com/Xi-L/ParetoMTL)                               | Pareto solutions in sectors.                                          | 2. 3 is difficult. | Y       | NeurIPS 2019 | $O(m^2 n K^2 )$ |
-    | [PMGDA](http://arxiv.org/abs/2402.09492)                                                                                                                                              | Pareto solutions satisfying any preference.                           | Any                | Y       | Under review | $O(m^2 n K )$   |
-    | [GradienHV](https://arxiv.org/abs/2102.04523) [WangHao](https://link.springer.com/chapter/10.1007/978-3-319-54157-0_44) [code](https://github.com/timodeist/multi_objective_learning) | It is a gradient-based HV method.| 2/3                | Y       | CEC 2023| $O(m^2 n K^2 )$ |   
-    | Aggregation fun. based, e.g. Tche,mTche,LS,PBI,...                                                                                                                                    | Pareto solution with aggregations.    | Any                | Y       |
-
-
-    Here, $m$ is the number of objectives, $K$ is the number of samples, and $n$ is the number of decision variables.
-    For neural network based methods, $n$ is the number of parameters; hence $n$ is very large (>10000), K is also large (e.g., 20-50), while $m$ is small (2.g., 2-4).
-
-    As a result, m^2 is not a big problem. n^2 is a big problem. K^2 is a big problem.
-
-    Time complexity of gradient based methods are as follows,
-        -1 Tier 1. GradAggSolver.
-        -2 Tier 2. MGDASolver, EPOSolver, PMTLSolver. 
-        -3 Tier 3. GradHVSolver
-        -4 Tier 4. MOOSVGDSolver
-
-    Current support:
-        GradAggSolver, MGDASolver, EPOSolver, MOOSVGDSolver, GradHVSolver, PMTLSolver.
-
-    Important things to notice:
-        The original code MOO-SVGD does not offer a MTL implement. Our code is the first open source code for MTL MOO-SVGD.
-
-
-- **PSL solvers**
-    - EPO-based
-    - Agg-based
-    - Hypernetwork-based
-    - ConditionalNet-based
-    - Simple PSL model
-    - Generative PSL model     
-    
-- **MOEA/D**
-    Current supported:
-    - Vanilla [MOEA/D](https://ieeexplore.ieee.org/document/4358754)
-    
-    - Will be released soon:
-    - [MOEA/D AWA](https://pubmed.ncbi.nlm.nih.gov/23777254/). 
-    - [MOEA/D neural AWA](https://openreview.net/pdf?id=W3T9rql5eo).
-
-    
-
-
-- **ML pretrained methods.** 
-    - HV net (https://arxiv.org/abs/2203.02185).  
-
-
-
-
-
-Example code:
-```
-from libmoon.solver.gradient import GradAggSolver
-from libmoon.util_global.constant import problem_dict
-from libmoon.util_global.weight_factor.funs import uniform_pref
-import torch
-import numpy as np
-from matplotlib import pyplot as plt
-import argparse
-
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='example')
-    parser.add_argument('--n-partition', type=int, default=10)
-    parser.add_argument('--agg', type=str, default='tche')  # If solve is agg, then choose a specific agg method.
-    parser.add_argument('--solver', type=str, default='agg')
-    parser.add_argument('--problem-name', type=str, default='VLMOP2')
-    parser.add_argument('--iter', type=int, default=1000)
-    parser.add_argument('--step-size', type=float, default=1e-2)
-    parser.add_argument('--tol', type=float, default=1e-6)
-    args = parser.parse_args()
-    
-    
-    # Init the solver, problem and prefs. 
-    solver = GradAggSolver(args.step_size, args.iter, args.tol)
-    problem = problem_dict[args.problem_name]
-    prefs = uniform_pref(args.n_partition, problem.n_obj, clip_eps=1e-2)
-    args.n_prob = len(prefs)
-
-    # Initialize the initial solution 
-    if 'lbound' in dir(problem):
-        if args.problem_name == 'VLMOP1':
-            x0 = torch.rand(args.n_prob, problem.n_var) * 2 / np.sqrt(problem.n_var) - 1 / np.sqrt(problem.n_var)
-        else:
-            x0 = torch.rand(args.n_prob, problem.n_var)
-    else:
-        x0 = torch.rand( args.n_prob, problem.n_var )*20 - 10
-
-
-    # Solve results
-    res = solver.solve(problem, x=x0, prefs=prefs, args=args)
-    
-    # Visualize results
-    y_arr = res['y']
-    plt.scatter(y_arr[:,0], y_arr[:,1], s=50)
-    plt.xlabel('$f_1$', fontsize=20)
-    plt.ylabel('$f_2$', fontsize=20)
-    plt.show()
-
-    
-
+Metadata-Version: 2.1
+Name: libmoon
+Version: 0.2.1
+Summary: Moon, Make MOO great again
+Author: Xiaoyuan Zhang et al.
+Author-email: xzhang2523-c@my.cityu.edu.hk
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+### Moon: A Standardized/Flexible Framework for MultiObjective OptimizatioN
+
+
+<img src="moon.png" alt="Moon" width="200">
+
+# Moon: A Multiobjective Optimization Framework
+
+## Introduction
+**Moon** is a multiobjective optimization framework that spans from single-objective optimization to multiobjective optimization. It aims to enhance the understanding of optimization problems and facilitate fair comparisons between MOO algorithms.
+
+> "I raise my cup to invite the moon.  
+> With my shadow we become three from one."  
+> -- Li Bai
+
+## Main Contributors
+- **Xiaoyuan Zhang** (Project Leader)
+- Ji Cheng
+- Liao Zhao
+- Weiduo Liao
+- Zhe Zhao
+- Xi Lin
+- Cheng Gong
+- Longcan Chen
+- YingYing Yu
+
+## Advisory Board
+- **Prof. Yifan Chen** (Hong Kong Baptist University)
+- **Prof. Zhichao Lu** (City University of Hong Kong)
+- **Prof. Ke Shang** (Shenzhen University)
+- **Prof. Tao Qin** (Microsoft Research)
+- **Prof. Han Zhao** (University of Illinois at Urbana-Champaign)
+
+## Correspondence
+For any inquiries, please contact **Prof. Qingfu Zhang** (City University of Hong Kong) at the corresponding address.
+
+## Resources
+For more information on methodologies, please visit our [GitHub repository](https://github.com/xzhang2523/awesome-moo-ml-papers). Contributions and stars are welcome!
+
+
+
+(1) A standardlized gradient based framework. 
+# Optimization Problem Classes
+
+## **Problem Class Details**
+For more information on problem specifics, please refer to the `Readme_problem.md` file.
+
+### Synthetic Problems
+Here's a list of synthetic problems along with relevant research papers and project/code links:
+
+| Problem | Paper | Project/Code |
+|---------|-------|--------------|
+| ZDT     | [Paper](https://ieeexplore.ieee.org/document/996017) | [Project](https://pymoo.org/problems/multi/zdt.html) |
+| DTLZ    | [Paper](https://ieeexplore.ieee.org/document/996017) | [Project](https://pymoo.org/problems/many/dtlz.html) |
+| MAF     | [Paper](https://link.springer.com/article/10.1007/s40747-017-0039-7) | [Project](https://pymoo.org/problems/multi/maf.html) |
+| WFG     | [Paper](https://ieeexplore.ieee.org/document/996017) | [Code](https://github.com/sample-repo/wfg-code) |
+| Fi's    | [Paper](https://ieeexplore.ieee.org/document/996017) | [Code](https://github.com/sample-repo/fis-code) |
+| RE      | [Paper](https://arxiv.org/abs/2009.12867) | [Code](https://github.com/ryojitanabe/reproblems) |
+
+### Multitask Learning Problems
+
+This section details problems related to multitask learning, along with their corresponding papers and project/code references:
+
+| Problem              | Paper                                                                                                           | Project/Code                                   |
+|----------------------|-----------------------------------------------------------------------------------------------------------------|------------------------------------------------|
+| MO-MNISTs            | [PMTL](https://proceedings.neurips.cc/paper_files/paper/2019/file/685bfde03eb646c27ed565881917c71c-Paper.pdf) | [COSMOS](https://github.com/ruchtem/cosmos)    |
+| Fairness Classification | [COSMOS](https://arxiv.org/pdf/2103.13392.pdf)                                                                  | [COSMOS](https://github.com/ruchtem/cosmos)    |
+| Federated Learning   | [Federal MTL](https://proceedings.neurips.cc/paper_files/paper/2023/file/7cb2c2a8d35576c00078b6591ec26a7d-Paper.pdf) | [COSMOS](https://github.com/ruchtem/cosmos) |
+| Synthetic (DST, FTS...) | [Envelop](https://proceedings.neurips.cc/paper_files/paper/2019/file/4a46fbfca3f1465a27b210f4bdfe6ab3-Paper.pdf) | [Project](https://github.com/sample-repo/envelop-code) |
+| Robotics (MO-MuJoCo...) | [PGMORL](http://proceedings.mlr.press/v119/xu20h/xu20h.pdf)                                                      | [Code](https://github.com/mit-gfx/PGMORL)     |
+
+
+
+- **Gradient-based Solver**.
+
+    | Method                                                                                                                                                                                | Property                                                              | #Obj               | Support | Published | Complexity      |
+    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------|--------------------|---------|----------|-----------------|
+    | [EPO](https://proceedings.mlr.press/v119/mahapatra20a/mahapatra20a.pdf) [code](https://github.com/dbmptr/EPOSearch)                                                                   | Exact solution.                                                       | Any                | Y       | ICML 2020 | $O(m^2 n K )$   |
+    | [COSMOS](https://arxiv.org/pdf/2103.13392.pdf) [code](https://github.com/ruchtem/cosmos)                                                                                              | Approximated exact solution.                                          | Any                | Y       | ICDM 2021| $O(m n K )$     |
+    | [MOO-SVGD](https://openreview.net/pdf?id=S2-j0ZegyrE) [code](https://github.com/gnobitab/MultiObjectiveSampling)                                                                      | A set of diverse Pareto solution.                                     | Any                | Y       | NeurIPS 2021 | $O(m^2 n K^2 )$ |
+    | [MGDA](https://proceedings.neurips.cc/paper/2018/file/432aca3a1e345e339f35a30c8f65edce-Paper.pdf) [code](https://github.com/intel-isl/MultiObjectiveOptimization)                     | Arbitray Pareto solutions. Location affected highly by initialization. | Any                | Y       | NeurIPS 2018 | $O(m^2 n K )$   |
+    | [PMTL](https://proceedings.neurips.cc/paper_files/paper/2019/file/685bfde03eb646c27ed565881917c71c-Paper.pdf) [code](https://github.com/Xi-L/ParetoMTL)                               | Pareto solutions in sectors.                                          | 2. 3 is difficult. | Y       | NeurIPS 2019 | $O(m^2 n K^2 )$ |
+    | [PMGDA](http://arxiv.org/abs/2402.09492)                                                                                                                                              | Pareto solutions satisfying any preference.                           | Any                | Y       | Under review | $O(m^2 n K )$   |
+    | [GradienHV](https://arxiv.org/abs/2102.04523) [WangHao](https://link.springer.com/chapter/10.1007/978-3-319-54157-0_44) [code](https://github.com/timodeist/multi_objective_learning) | It is a gradient-based HV method.| 2/3                | Y       | CEC 2023| $O(m^2 n K^2 )$ |   
+    | Aggregation fun. based, e.g. Tche,mTche,LS,PBI,...                                                                                                                                    | Pareto solution with aggregations.    | Any                | Y       |
+
+
+    Here, $m$ is the number of objectives, $K$ is the number of samples, and $n$ is the number of decision variables.
+    For neural network based methods, $n$ is the number of parameters; hence $n$ is very large (>10000), K is also large (e.g., 20-50), while $m$ is small (2.g., 2-4).
+
+    As a result, m^2 is not a big problem. n^2 is a big problem. K^2 is a big problem.
+
+    Time complexity of gradient based methods are as follows,
+        -1 Tier 1. GradAggSolver.
+        -2 Tier 2. MGDASolver, EPOSolver, PMTLSolver. 
+        -3 Tier 3. GradHVSolver
+        -4 Tier 4. MOOSVGDSolver
+
+    Current support:
+        GradAggSolver, MGDASolver, EPOSolver, MOOSVGDSolver, GradHVSolver, PMTLSolver.
+
+    Important things to notice:
+        The original code MOO-SVGD does not offer a MTL implement. Our code is the first open source code for MTL MOO-SVGD.
+
+## Supported Solvers
+
+### Current Support
+Libmoon includes a variety of solvers tailored for different needs:
+- GradAggSolver
+- MGDASolver
+- EPOSolver
+- MOOSVGDSolver (*)
+- GradHVSolver
+- PMTLSolver
+
+(*) The original MOO-SVGD code does not include an implementation for Multitask Learning (MTL). Our release of MOO-SVGD is the first open-source code that supports MTL.
+
+## PSL (Pareto set learning) Solvers
+
+Libmoon supports various models of PSL solvers, categorized as follows:
+- EPO-based PSL model
+- Agg-based PSL model 
+- Hypernetwork-based PSL model 
+- ConditionalNet-based PSL model 
+- Simple PSL model
+- Generative PSL model
+
+
+
+
+## MOEA/D Framework
+
+### Currently Supported
+- Vanilla [MOEA/D](https://ieeexplore.ieee.org/document/4358754)
+
+### Upcoming Releases
+- [MOEA/D AWA](https://pubmed.ncbi.nlm.nih.gov/23777254/)
+- [MOEA/D Neural AWA](https://openreview.net/pdf?id=W3T9rql5eo)
+
+## ML Pretrained Methods
+- HV Net, a model for handling high-volume data, available [here](https://arxiv.org/abs/2203.02185).
+
+## Installation
+
+Libmoon is available on PyPI. You can install it using pip:
+
+```bash
+pip install libmoon==0.1.11
+
+
+Example code for a synthetic problem,
+```
+from libmoon.solver.gradient import GradAggSolver
+from libmoon.util_global.constant import problem_dict
+from libmoon.util_global.weight_factor.funs import uniform_pref
+import torch
+import numpy as np
+from matplotlib import pyplot as plt
+import argparse
+from libmoon.visulization.view_res import vedio_res
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser(description='example')
+    parser.add_argument('--n-partition', type=int, default=10)
+    parser.add_argument('--agg', type=str, default='tche')  # If solve is agg, then choose a specific agg method.
+    parser.add_argument('--solver', type=str, default='agg')
+    parser.add_argument('--problem-name', type=str, default='VLMOP2')
+    parser.add_argument('--iter', type=int, default=1000)
+    parser.add_argument('--step-size', type=float, default=1e-2)
+    parser.add_argument('--tol', type=float, default=1e-6)
+    args = parser.parse_args()
+    
+    
+    # Init the solver, problem and prefs. 
+    solver = GradAggSolver(args.step_size, args.iter, args.tol)
+    problem = problem_dict[args.problem_name]
+    prefs = uniform_pref(args.n_partition, problem.n_obj, clip_eps=1e-2)
+    args.n_prob = len(prefs)
+
+    # Initialize the initial solution 
+    if 'lbound' in dir(problem):
+        if args.problem_name == 'VLMOP1':
+            x0 = torch.rand(args.n_prob, problem.n_var) * 2 / np.sqrt(problem.n_var) - 1 / np.sqrt(problem.n_var)
+        else:
+            x0 = torch.rand(args.n_prob, problem.n_var)
+    else:
+        x0 = torch.rand( args.n_prob, problem.n_var )*20 - 10
+
+
+    # Solve results
+    res = solver.solve(problem, x=x0, prefs=prefs, args=args)
+    
+    # Visualize results
+    y_arr = res['y']
+    plt.scatter(y_arr[:,0], y_arr[:,1], s=50)
+    plt.xlabel('$f_1$', fontsize=20)
+    plt.ylabel('$f_2$', fontsize=20)
+    plt.show()
+    
+    # If use vedio
+    use_vedio=True
+    if use_vedio:
+        vedio_res(res, problem, prefs, args)     
+```
+        
+Example of MTL
+```
+
+
+```
+
+    
+
```

### Comparing `libmoon-0.1.9/libmoon.egg-info/SOURCES.txt` & `libmoon-0.2.1/libmoon.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,44 @@
 LICENSE
 README.md
 setup.py
 libmoon/__init__.py
-libmoon/example.py
 libmoon.egg-info/PKG-INFO
 libmoon.egg-info/SOURCES.txt
 libmoon.egg-info/dependency_links.txt
 libmoon.egg-info/requires.txt
 libmoon.egg-info/top_level.txt
+libmoon/metrics/__init__.py
+libmoon/metrics/metrics.py
 libmoon/problem/__init__.py
-libmoon/problem/mop.py
 libmoon/problem/mtl/__init__.py
-libmoon/problem/mtl/fair_classify.py
 libmoon/problem/mtl/mnist.py
+libmoon/problem/mtl/model_utils.py
 libmoon/problem/mtl/objectives.py
+libmoon/problem/mtl/run_fair_pref.py
+libmoon/problem/mtl/run_fair_set.py
+libmoon/problem/mtl/settings.py
 libmoon/problem/mtl/loaders/__init__.py
 libmoon/problem/mtl/loaders/adult_loader.py
 libmoon/problem/mtl/loaders/compas_loader.py
 libmoon/problem/mtl/loaders/credit_loader.py
 libmoon/problem/mtl/loaders/multimnist_loader.py
-libmoon/problem/mtl/model/__init__.py
-libmoon/problem/mtl/model/simple.py
+libmoon/problem/mtl/models/__init__.py
+libmoon/problem/mtl/models/fair_model.py
+libmoon/problem/mtl/models/lenet.py
 libmoon/problem/synthetic/__init__.py
 libmoon/problem/synthetic/dtlz.py
 libmoon/problem/synthetic/maf.py
+libmoon/problem/synthetic/mop.py
 libmoon/problem/synthetic/re.py
 libmoon/problem/synthetic/re_original.py
 libmoon/problem/synthetic/vlmop.py
 libmoon/problem/synthetic/wfg.py
 libmoon/problem/synthetic/zdt.py
 libmoon/solver/__init__.py
-libmoon/solver/gradient/__init__.py
-libmoon/solver/gradient/base_solver.py
-libmoon/solver/gradient/core_solver.py
-libmoon/solver/gradient/epo_solver.py
-libmoon/solver/gradient/functions_evaluation.py
-libmoon/solver/gradient/functions_hv_grad_3d.py
-libmoon/solver/gradient/functions_hv_python3.py
-libmoon/solver/gradient/gradhv.py
-libmoon/solver/gradient/mgda_core.py
-libmoon/solver/gradient/mgda_solver.py
-libmoon/solver/gradient/min_norm_solvers_numpy.py
-libmoon/solver/gradient/moosvgd.py
-libmoon/solver/gradient/pmgda.py
-libmoon/solver/gradient/pmtl.py
-libmoon/solver/gradient/run/__init__.py
-libmoon/solver/gradient/run/run_grad.py
-libmoon/solver/gradient/utils/__init__.py
-libmoon/solver/gradient/utils/util.py
 libmoon/solver/mobo/__init__.py
 libmoon/solver/mobo/dirhvego.py
 libmoon/solver/mobo/mobod.py
 libmoon/solver/mobo/utils/__init__.py
 libmoon/solver/mobo/utils/termination.py
 libmoon/solver/moea/__init__.py
 libmoon/solver/moea/moead.py
@@ -73,17 +60,14 @@
 libmoon/solver/psl/run_simple_psl.py
 libmoon/solver/psl/util.py
 libmoon/solver/psl/model/__init__.py
 libmoon/solver/psl/model/mtl.py
 libmoon/solver/psl/model/simple.py
 libmoon/util_global/__init__.py
 libmoon/util_global/constant.py
+libmoon/util_global/grad_util.py
 libmoon/util_global/scalarization.py
-libmoon/util_global/weight_factor/__init__.py
-libmoon/util_global/weight_factor/das_dennis.py
-libmoon/util_global/weight_factor/funs.py
+libmoon/util_global/weight_factor.py
+libmoon/util_global/zero_order.py
 libmoon/visulization/__init__.py
 libmoon/visulization/util.py
-libmoon/visulization/view_res.py
-src/__init__.py
-test/test2.py
-test/test_kernel.py
+libmoon/visulization/view_res.py
```

### Comparing `libmoon-0.1.9/setup.py` & `libmoon-0.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='libmoon',
-    version='0.1.9',
+    version='0.2.1',
     author='Xiaoyuan Zhang et al.',
     author_email='xzhang2523-c@my.cityu.edu.hk',
     description='Moon, Make MOO great again',
     packages=find_packages(
         # include=['solver.gradient.epo_solver',
         #          'solver.gradient',
         #          'src.libmoon']
@@ -27,12 +27,13 @@
                     'torch==2.2.1',
                     'matplotlib==3.8.3',
                     'tqdm==4.66.2',
                     'pymoo==0.6.1.1',
                     'cvxopt==1.3.2',
                     'cvxpy==1.4.2',
                     'ffmpeg-python',
-                      'ffmpeg'
+                      'ffmpeg',
+                    'scikit-learn'
                       ],
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

