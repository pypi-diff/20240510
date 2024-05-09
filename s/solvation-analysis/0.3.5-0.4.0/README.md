# Comparing `tmp/solvation-analysis-0.3.5.tar.gz` & `tmp/solvation_analysis-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solvation-analysis-0.3.5.tar", last modified: Mon Feb 12 22:38:58 2024, max compression
+gzip compressed data, was "solvation_analysis-0.4.0.tar", last modified: Thu May  9 23:36:01 2024, max compression
```

## Comparing `solvation-analysis-0.3.5.tar` & `solvation_analysis-0.4.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:58.729450 solvation-analysis-0.3.5/
--rw-r--r--   0 orioncohen   (505) staff       (20)     8081 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 orioncohen   (505) staff       (20)    34684 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/LICENSE
--rw-r--r--   0 orioncohen   (505) staff       (20)      234 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/MANIFEST.in
--rw-r--r--   0 orioncohen   (505) staff       (20)    45171 2024-02-12 22:38:58.729267 solvation-analysis-0.3.5/PKG-INFO
--rw-r--r--   0 orioncohen   (505) staff       (20)     4014 2023-08-14 16:59:31.000000 solvation-analysis-0.3.5/README.md
--rw-r--r--   0 orioncohen   (505) staff       (20)     1949 2024-02-12 21:26:16.000000 solvation-analysis-0.3.5/pyproject.toml
--rw-r--r--   0 orioncohen   (505) staff       (20)      112 2024-02-12 21:26:16.000000 solvation-analysis-0.3.5/requirements.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)      381 2024-02-12 22:38:58.730046 solvation-analysis-0.3.5/setup.cfg
--rw-r--r--   0 orioncohen   (505) staff       (20)     2400 2023-04-05 15:18:21.000000 solvation-analysis-0.3.5/setup.py
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:58.730327 solvation-analysis-0.3.5/solvation_analysis/
--rw-r--r--   0 orioncohen   (505) staff       (20)      335 2022-10-28 18:42:42.000000 solvation-analysis-0.3.5/solvation_analysis/__init__.py
--rw-r--r--   0 orioncohen   (505) staff       (20)      728 2022-10-28 18:42:42.000000 solvation-analysis-0.3.5/solvation_analysis/_column_names.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     8016 2024-02-12 20:31:32.000000 solvation-analysis-0.3.5/solvation_analysis/_utils.py
--rw-r--r--   0 orioncohen   (505) staff       (20)      498 2024-02-12 22:38:58.730421 solvation-analysis-0.3.5/solvation_analysis/_version.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     6570 2023-04-09 17:43:35.000000 solvation-analysis-0.3.5/solvation_analysis/coordination.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    10777 2023-04-02 16:08:07.000000 solvation-analysis-0.3.5/solvation_analysis/networking.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     5709 2023-04-02 16:08:07.000000 solvation-analysis-0.3.5/solvation_analysis/pairing.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    13759 2023-08-14 16:58:21.000000 solvation-analysis-0.3.5/solvation_analysis/plotting.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    11231 2022-10-28 18:42:42.000000 solvation-analysis-0.3.5/solvation_analysis/rdf_parser.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    11027 2024-02-12 20:32:42.000000 solvation-analysis-0.3.5/solvation_analysis/residence.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    38245 2023-02-14 18:50:22.000000 solvation-analysis-0.3.5/solvation_analysis/solute.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     8972 2023-08-14 16:59:31.000000 solvation-analysis-0.3.5/solvation_analysis/speciation.py
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:58.717171 solvation-analysis-0.3.5/solvation_analysis/tests/
--rw-r--r--   0 orioncohen   (505) staff       (20)      112 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/__init__.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     9536 2024-02-06 20:15:50.000000 solvation-analysis-0.3.5/solvation_analysis/tests/conftest.py
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:25.452445 solvation-analysis-0.3.5/solvation_analysis/tests/data/
--rw-r--r--   0 orioncohen   (505) staff       (20)     8196 2022-10-02 21:12:27.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/.DS_Store
--rw-r--r--   0 orioncohen   (505) staff       (20)     2848 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/README.md
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:58.718067 solvation-analysis-0.3.5/solvation_analysis/tests/data/bn_fec_data/
--rw-r--r--   0 orioncohen   (505) staff       (20)  1418421 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/bn_fec_data/bn_fec.data
--rw-r--r--   0 orioncohen   (505) staff       (20)    14285 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/bn_fec_data/bn_fec_elements.csv
--rw-r--r--   0 orioncohen   (505) staff       (20)   855316 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_unwrap.dcd
--rw-r--r--   0 orioncohen   (505) staff       (20)   855316 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_wrap.dcd
--rw-r--r--   0 orioncohen   (505) staff       (20)  5563748 2022-10-28 18:42:42.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/bn_fec_data/bn_solv_df_large.csv
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:25.473664 solvation-analysis-0.3.5/solvation_analysis/tests/data/ea_fec_data/
--rw-r--r--   0 orioncohen   (505) staff       (20)   892516 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/ea_fec_data/ea_fec.dcd
--rw-r--r--   0 orioncohen   (505) staff       (20)   761309 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/ea_fec_data/ea_fec.pdb
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:25.429978 solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:25.477855 solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/ea/
--rw-r--r--   0 orioncohen   (505) staff       (20)   871090 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/ea/topology.pdb
--rw-r--r--   0 orioncohen   (505) staff       (20)  1023556 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/ea/trajectory_equil.dcd
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:25.480636 solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/eaf/
--rw-r--r--   0 orioncohen   (505) staff       (20)   874261 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/eaf/topology.pdb
--rw-r--r--   0 orioncohen   (505) staff       (20)  1027396 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/eaf/trajectory_equil.dcd
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:25.484806 solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/fea/
--rw-r--r--   0 orioncohen   (505) staff       (20)   875050 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/fea/topology.pdb
--rw-r--r--   0 orioncohen   (505) staff       (20)  1028356 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/fea/trajectory_equil.dcd
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:25.489335 solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/feaf/
--rw-r--r--   0 orioncohen   (505) staff       (20)   876623 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/feaf/topology.pdb
--rw-r--r--   0 orioncohen   (505) staff       (20)  1030276 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/feaf/trajectory_equil.dcd
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:25.493161 solvation-analysis-0.3.5/solvation_analysis/tests/data/iba_data/
--rw-r--r--   0 orioncohen   (505) staff       (20)   721156 2022-09-27 18:34:04.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/iba_data/isobutyric_acid.dcd
--rw-r--r--   0 orioncohen   (505) staff       (20)   610100 2022-09-27 18:34:04.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/iba_data/isobutyric_acid.pdb
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:25.507712 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_data.npz
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:25.512726 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_data.npz
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:25.517469 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_bins.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_data.npz
--rw-r--r--   0 orioncohen   (505) staff       (20)     2601 2022-09-27 18:34:04.000000 solvation-analysis-0.3.5/solvation_analysis/tests/datafiles.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     1596 2023-04-09 17:25:23.000000 solvation-analysis-0.3.5/solvation_analysis/tests/test_coordination.py
--rw-r--r--   0 orioncohen   (505) staff       (20)      867 2023-02-14 18:28:50.000000 solvation-analysis-0.3.5/solvation_analysis/tests/test_networking.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     1516 2023-04-02 16:08:07.000000 solvation-analysis-0.3.5/solvation_analysis/tests/test_pairing.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    10037 2023-08-14 16:58:27.000000 solvation-analysis-0.3.5/solvation_analysis/tests/test_plotting.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     6317 2022-10-28 18:42:42.000000 solvation-analysis-0.3.5/solvation_analysis/tests/test_rdf_parser.py
--rw-r--r--   0 orioncohen   (505) staff       (20)      961 2023-02-14 18:28:50.000000 solvation-analysis-0.3.5/solvation_analysis/tests/test_residence.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     4012 2022-10-28 18:42:42.000000 solvation-analysis-0.3.5/solvation_analysis/tests/test_selection.py
--rw-r--r--   0 orioncohen   (505) staff       (20)    12563 2023-04-02 16:08:07.000000 solvation-analysis-0.3.5/solvation_analysis/tests/test_solute.py
--rw-r--r--   0 orioncohen   (505) staff       (20)     1572 2023-04-06 16:18:52.000000 solvation-analysis-0.3.5/solvation_analysis/tests/test_speciation.py
-drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-02-12 22:38:58.728482 solvation-analysis-0.3.5/solvation_analysis.egg-info/
--rw-r--r--   0 orioncohen   (505) staff       (20)    45171 2024-02-12 22:38:58.000000 solvation-analysis-0.3.5/solvation_analysis.egg-info/PKG-INFO
--rw-r--r--   0 orioncohen   (505) staff       (20)     7068 2024-02-12 22:38:58.000000 solvation-analysis-0.3.5/solvation_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)        1 2024-02-12 22:38:58.000000 solvation-analysis-0.3.5/solvation_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)      104 2024-02-12 22:38:58.000000 solvation-analysis-0.3.5/solvation_analysis.egg-info/requires.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)       19 2024-02-12 22:38:58.000000 solvation-analysis-0.3.5/solvation_analysis.egg-info/top_level.txt
--rw-r--r--   0 orioncohen   (505) staff       (20)    78254 2022-08-17 22:41:48.000000 solvation-analysis-0.3.5/versioneer.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:36:01.783509 solvation_analysis-0.4.0/
+-rw-r--r--   0 orioncohen   (505) staff       (20)     8081 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 orioncohen   (505) staff       (20)    34684 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/LICENSE
+-rw-r--r--   0 orioncohen   (505) staff       (20)      234 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/MANIFEST.in
+-rw-r--r--   0 orioncohen   (505) staff       (20)    45786 2024-05-09 23:36:01.783335 solvation_analysis-0.4.0/PKG-INFO
+-rw-r--r--   0 orioncohen   (505) staff       (20)     4621 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/README.md
+-rw-r--r--   0 orioncohen   (505) staff       (20)     1957 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/pyproject.toml
+-rw-r--r--   0 orioncohen   (505) staff       (20)      120 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/requirements.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)      381 2024-05-09 23:36:01.784040 solvation_analysis-0.4.0/setup.cfg
+-rw-r--r--   0 orioncohen   (505) staff       (20)     2412 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/setup.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:36:01.784360 solvation_analysis-0.4.0/solvation_analysis/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      404 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/__init__.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)      730 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/_column_names.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     8908 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/_utils.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)      498 2024-05-09 23:36:01.784424 solvation_analysis-0.4.0/solvation_analysis/_version.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     7089 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/coordination.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    11472 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/networking.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     6319 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/pairing.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    24851 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/plotting.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    12166 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/rdf_parser.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    11892 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/residence.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    41247 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/solute.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     9444 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/speciation.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:36:01.765573 solvation_analysis-0.4.0/solvation_analysis/tests/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      112 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/__init__.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     9690 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/tests/conftest.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:36:01.765948 solvation_analysis-0.4.0/solvation_analysis/tests/data/
+-rw-r--r--   0 orioncohen   (505) staff       (20)     8196 2022-10-02 21:12:27.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/.DS_Store
+-rw-r--r--   0 orioncohen   (505) staff       (20)     2848 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/README.md
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:36:01.766730 solvation_analysis-0.4.0/solvation_analysis/tests/data/bn_fec_data/
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1418421 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/bn_fec_data/bn_fec.data
+-rw-r--r--   0 orioncohen   (505) staff       (20)    14285 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/bn_fec_data/bn_fec_elements.csv
+-rw-r--r--   0 orioncohen   (505) staff       (20)   855316 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_unwrap.dcd
+-rw-r--r--   0 orioncohen   (505) staff       (20)   855316 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_wrap.dcd
+-rw-r--r--   0 orioncohen   (505) staff       (20)  5563748 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/bn_fec_data/bn_solv_df_large.csv
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:36:01.773140 solvation_analysis-0.4.0/solvation_analysis/tests/data/ea_fec_data/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   892516 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/ea_fec_data/ea_fec.dcd
+-rw-r--r--   0 orioncohen   (505) staff       (20)   761309 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/ea_fec_data/ea_fec.pdb
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:35:36.177697 solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:36:01.774356 solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/ea/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   871090 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/ea/topology.pdb
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1023556 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/ea/trajectory_equil.dcd
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:36:01.775862 solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/eaf/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   874261 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/eaf/topology.pdb
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1027396 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/eaf/trajectory_equil.dcd
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:36:01.777213 solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/fea/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   875050 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/fea/topology.pdb
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1028356 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/fea/trajectory_equil.dcd
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:36:01.778590 solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/feaf/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   876623 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/feaf/topology.pdb
+-rw-r--r--   0 orioncohen   (505) staff       (20)  1030276 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/feaf/trajectory_equil.dcd
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:36:01.779939 solvation_analysis-0.4.0/solvation_analysis/tests/data/iba_data/
+-rw-r--r--   0 orioncohen   (505) staff       (20)   721156 2022-09-27 18:34:04.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/iba_data/isobutyric_acid.dcd
+-rw-r--r--   0 orioncohen   (505) staff       (20)   610100 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/iba_data/isobutyric_acid.pdb
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:35:36.280293 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_data.npz
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:35:36.286997 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_data.npz
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:35:36.294036 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_bins.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)      864 2022-08-17 22:41:48.000000 solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_data.npz
+-rw-r--r--   0 orioncohen   (505) staff       (20)     2601 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/datafiles.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     1596 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/test_coordination.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)      867 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/test_networking.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     1516 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/test_pairing.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    10253 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/tests/test_plotting.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     6381 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/test_rdf_parser.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)      974 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/tests/test_residence.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     4012 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/test_selection.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)    12117 2024-05-09 23:34:09.000000 solvation_analysis-0.4.0/solvation_analysis/tests/test_solute.py
+-rw-r--r--   0 orioncohen   (505) staff       (20)     1572 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/solvation_analysis/tests/test_speciation.py
+drwxr-xr-x   0 orioncohen   (505) staff       (20)        0 2024-05-09 23:36:01.782612 solvation_analysis-0.4.0/solvation_analysis.egg-info/
+-rw-r--r--   0 orioncohen   (505) staff       (20)    45786 2024-05-09 23:36:01.000000 solvation_analysis-0.4.0/solvation_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 orioncohen   (505) staff       (20)     7068 2024-05-09 23:36:01.000000 solvation_analysis-0.4.0/solvation_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)        1 2024-05-09 23:36:01.000000 solvation_analysis-0.4.0/solvation_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)      112 2024-05-09 23:36:01.000000 solvation_analysis-0.4.0/solvation_analysis.egg-info/requires.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)       19 2024-05-09 23:36:01.000000 solvation_analysis-0.4.0/solvation_analysis.egg-info/top_level.txt
+-rw-r--r--   0 orioncohen   (505) staff       (20)    78254 2024-05-07 17:54:07.000000 solvation_analysis-0.4.0/versioneer.py
```

### Comparing `solvation-analysis-0.3.5/CODE_OF_CONDUCT.md` & `solvation_analysis-0.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/LICENSE` & `solvation_analysis-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/PKG-INFO` & `solvation_analysis-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvation-analysis
-Version: 0.3.5
+Version: 0.4.0
 Summary: A toolkit to analyze solvation structure in molecular dynamics trajectories.
 Author: Orion Cohen
 Author-email: Orion Cohen <orioncohen@berkeley.edu>
 Maintainer-email: Orion Cohen <orioncohen@berkeley.edu>, Hugo MacDermott-Opeskin <hugomacdermott@gmail.com>
 License:                         GNU GENERAL PUBLIC LICENSE 
                                   Version 3, 29 June 2007
         
@@ -604,15 +604,15 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pandas>=2.2
 Requires-Dist: mdanalysis>=2.0.0
 Requires-Dist: pytest
 Requires-Dist: matplotlib
 Requires-Dist: setuptools
-Requires-Dist: scipy
+Requires-Dist: scipy==1.12.0
 Requires-Dist: statsmodels
 Requires-Dist: plotly
 Requires-Dist: rdkit
 
 SolvationAnalysis
 ==============================
 [//]: # (Badges)
@@ -626,47 +626,65 @@
 
 [//]: # ([![DOI]&#40;https://zenodo.org/badge/371804402.svg&#41;]&#40;https://zenodo.org/badge/latestdoi/371804402&#41;)
 
 
 ---
 
 Solvation analysis implements a robust, cohesive, and fast set of methods
-for analyzing the solvation structure of a liquid. It seamlessly integrates with
-[MDAnalysis](https://www.mdanalysis.org/), making use of the core AtomGroup
-and Universe data structures to parse solvation information. If you are interested
-in understanding the solvation structure of a liquid, this package is for you!
+for analyzing the solvation structure of a liquid. It integrates with
+[MDAnalysis](https://www.mdanalysis.org/) to seamlessly calculate, query,
+and visualize solvation information.
 
-
-Find documentation and tutorials on [readthedocs].
+Find documentation and tutorials on [readthedocs](https://solvation-analysis.readthedocs.io/en/latest/).
 
 ### Installing SolvationAnalysis
 
 SolvationAnalysis is available on PyPI and conda-forge can be installed with pip or conda:
 
 ```bash
 pip install solvation-analysis
 
 # or
 
 conda install -c conda-forge solvation_analysis
 ```
 
+### Solvation Analysis Summarized
+
+![summary](docs/tutorials/images/summary_figure.png)
+
+
+### Visualization
+
+With just a few lines of code, solvation analysis can calculate detailed
+properties within and between solvent systems. A few examples are shown below.
+
+![solvation_analysis.plotting.compare_coordination_numbers](docs/tutorials/images/coordination_plot.png)
+
+![solvation_analysis.plotting.plot_speciation](docs/tutorials/images/speciation_plot.png)
+
+![solvation_analysis.plotting.plot_rdfs](docs/tutorials/images/rdf_plot.png)
+
+
 ### Contributing
 
-Contributions, both issues and PRs, are welcome. If you'd like to contribute, we ask that you 
+Contributions, both issues and PRs, are welcome. If you'd like to contribute, we ask that you
 follow the community guidelines outlined in the [MDAnalysis Code of Conduct](https://www.mdanalysis.org/pages/conduct/).
 
+Solvation Analysis uses [pre-commit](https://pre-commit.com/) for linting. Make sure to install
+the pre-commit hooks if you are working on a contribution.
+
 ### Citation
 
 This work is described in [JOSS](https://doi.org/10.21105/joss.05183), please cite it if you make
 use of this package in published work.
 
 ---
 
-Project based on the 
+Project based on the
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.5.
 
 
 
 [readthedocs]: (https://solvation-analysis.readthedocs.io/en/latest/)
 [robust, cohesive, and fast set of methods]:(https://summerofcode.withgoogle.com/projects/#6227159028334592)
 [Google Summer of Code]: https://summerofcode.withgoogle.com/
```

### Comparing `solvation-analysis-0.3.5/README.md` & `solvation_analysis-0.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -11,47 +11,65 @@
 
 [//]: # ([![DOI]&#40;https://zenodo.org/badge/371804402.svg&#41;]&#40;https://zenodo.org/badge/latestdoi/371804402&#41;)
 
 
 ---
 
 Solvation analysis implements a robust, cohesive, and fast set of methods
-for analyzing the solvation structure of a liquid. It seamlessly integrates with
-[MDAnalysis](https://www.mdanalysis.org/), making use of the core AtomGroup
-and Universe data structures to parse solvation information. If you are interested
-in understanding the solvation structure of a liquid, this package is for you!
+for analyzing the solvation structure of a liquid. It integrates with
+[MDAnalysis](https://www.mdanalysis.org/) to seamlessly calculate, query,
+and visualize solvation information.
 
-
-Find documentation and tutorials on [readthedocs].
+Find documentation and tutorials on [readthedocs](https://solvation-analysis.readthedocs.io/en/latest/).
 
 ### Installing SolvationAnalysis
 
 SolvationAnalysis is available on PyPI and conda-forge can be installed with pip or conda:
 
 ```bash
 pip install solvation-analysis
 
 # or
 
 conda install -c conda-forge solvation_analysis
 ```
 
+### Solvation Analysis Summarized
+
+![summary](docs/tutorials/images/summary_figure.png)
+
+
+### Visualization
+
+With just a few lines of code, solvation analysis can calculate detailed
+properties within and between solvent systems. A few examples are shown below.
+
+![solvation_analysis.plotting.compare_coordination_numbers](docs/tutorials/images/coordination_plot.png)
+
+![solvation_analysis.plotting.plot_speciation](docs/tutorials/images/speciation_plot.png)
+
+![solvation_analysis.plotting.plot_rdfs](docs/tutorials/images/rdf_plot.png)
+
+
 ### Contributing
 
-Contributions, both issues and PRs, are welcome. If you'd like to contribute, we ask that you 
+Contributions, both issues and PRs, are welcome. If you'd like to contribute, we ask that you
 follow the community guidelines outlined in the [MDAnalysis Code of Conduct](https://www.mdanalysis.org/pages/conduct/).
 
+Solvation Analysis uses [pre-commit](https://pre-commit.com/) for linting. Make sure to install
+the pre-commit hooks if you are working on a contribution.
+
 ### Citation
 
 This work is described in [JOSS](https://doi.org/10.21105/joss.05183), please cite it if you make
 use of this package in published work.
 
 ---
 
-Project based on the 
+Project based on the
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.5.
 
 
 
 [readthedocs]: (https://solvation-analysis.readthedocs.io/en/latest/)
 [robust, cohesive, and fast set of methods]:(https://summerofcode.withgoogle.com/projects/#6227159028334592)
 [Google Summer of Code]: https://summerofcode.withgoogle.com/
```

### Comparing `solvation-analysis-0.3.5/pyproject.toml` & `solvation_analysis-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 dependencies = [
     'numpy>=1.20.0',
     'pandas>=2.2',
     'mdanalysis>=2.0.0',
     'pytest',
     'matplotlib',
     'setuptools',
-    'scipy',
+    'scipy==1.12.0',
     'statsmodels',
     'plotly',
     'rdkit'
 ]
 
 classifiers = [
     'Development Status :: 3 - Alpha',
```

### Comparing `solvation-analysis-0.3.5/setup.py` & `solvation_analysis-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,64 @@
 """
 SolvationAnalysis
 An MDAnalysis rmodule for solvation analysis.
 """
+
 import sys
 from setuptools import setup, find_packages
 import versioneer
 
 short_description = __doc__.split("\n")
 
 # from https://github.com/pytest-dev/pytest-runner#conditional-requirement
-needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
-pytest_runner = ['pytest-runner'] if needs_pytest else []
+needs_pytest = {"pytest", "test", "ptr"}.intersection(sys.argv)
+pytest_runner = ["pytest-runner"] if needs_pytest else []
 
 try:
     with open("README.md", "r") as handle:
         long_description = handle.read()
-except:
+except:  # noqa
     long_description = "\n".join(short_description[2:])
 
 
 setup(
     # Self-descriptive entries which should always be present
-    name='solvation_analysis',
-    author='Orion Cohen',
-    author_email='orioncohen@gmail.com',
+    name="solvation_analysis",
+    author="Orion Cohen",
+    author_email="orioncohen@gmail.com",
     description=short_description[0],
     long_description=long_description,
     long_description_content_type="text/markdown",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
-    license='GNU Public License v3',
-
+    license="GNU Public License v3",
     # Which Python importable modules should be included when your package is installed
     # Handled automatically by setuptools. Use 'exclude' to prevent some specific
     # subpackage(s) from being added, if needed
     packages=find_packages(),
-
     # Optional include package data to ship with your package
     # Customize MANIFEST.in if the general case does not suit your needs
     # Comment out this line to prevent the files from being packaged with your software
     include_package_data=True,
-
     # Allows `setup.py test` to work correctly with pytest
     setup_requires=[] + pytest_runner,
-
     install_requires=[
-        'numpy>=1.20.0',
-        'mdanalysis>=2.0.0',
-        'pandas',
-        'matplotlib',
-        'scipy',
-        'statsmodels',
-        'plotly',
-        'rdkit'
+        "numpy>=1.20.0",
+        "mdanalysis>=2.7.0",
+        "pandas",
+        "matplotlib",
+        "scipy==1.12.0",
+        "statsmodels",
+        "plotly",
+        "rdkit",
     ],
     # Additional entries you may want simply uncomment the lines you want and fill in the data
     # url='http://www.my_package.com',  # Website
     # install_requires=[],              # Required packages, pulls from pip if needed; do not use for Conda deployment
     # platforms=['Linux',
     #            'Mac OS-X',
     #            'Unix',
     #            'Windows'],            # Valid platforms your code works on, adjust to your flavor
     # python_requires=">=3.5",          # Python version restrictions
-
     # Manual control if final package is compressible or not, set False to prevent the .egg from being made
     # zip_safe=False,
-
 )
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/_column_names.py` & `solvation_analysis-0.4.0/solvation_analysis/_column_names.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 2. search through the documentation and change the string name wherever it appears
 3. change the name in the bn_solve_df_large dataframe
 
 To change the variable name of a variable:
 1. change the variable name in all files
 """
 
-
 # for solvation_data
 FRAME = "frame"
 SOLUTE_IX = "solute_ix"
 SOLUTE_ATOM_IX = "solute_atom_ix"
 SOLVENT_ATOM_IX = "solvent_atom_ix"
 DISTANCE = "distance"
 SOLUTE = "solute"
@@ -26,8 +25,8 @@
 # for networking
 NETWORK = "network"
 ISOLATED = "isolated"
 PAIRED = "paired"
 NETWORKED = "networked"
 
 # for speciation
-COUNT = "count"
+COUNT = "fraction"
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/_utils.py` & `solvation_analysis-0.4.0/solvation_analysis/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,93 @@
-import numpy as np
 from collections import defaultdict
 from functools import reduce
+from typing import Union
+
+import numpy as np
+import pandas as pd
 import MDAnalysis as mda
 from MDAnalysis.analysis import distances
 
-from solvation_analysis._column_names import *
+from solvation_analysis._column_names import FRAME, SOLUTE_IX, SOLVENT_IX, DISTANCE
 
 
-def verify_solute_atoms(solute_atom_group):
+def verify_solute_atoms(solute_atom_group: mda.AtomGroup) -> dict[int, mda.AtomGroup]:
     # we presume that the solute_atoms has the same number of atoms on each residue
     # and that they all have the same indices on those residues
     # and that the residues are all the same length
     # then this should work
     all_res_len = np.array([res.atoms.n_atoms for res in solute_atom_group.residues])
-    assert np.all(all_res_len[0] == all_res_len), (
-        "All residues must be the same length."
-    )
+    assert np.all(
+        all_res_len[0] == all_res_len
+    ), "All residues must be the same length."
     res_atom_local_ix = defaultdict(list)
     res_atom_ix = defaultdict(list)
 
     for atom in solute_atom_group.atoms:
         res_atom_local_ix[atom.resindex].append(atom.ix - atom.residue.atoms[0].ix)
         res_atom_ix[atom.resindex].append(atom.index)
     res_occupancy = np.array([len(ix) for ix in res_atom_local_ix.values()])
-    assert np.all(res_occupancy[0] == res_occupancy), (
-        "All residues must have the same number of solute_atoms atoms on them."
-    )
+    assert np.all(
+        res_occupancy[0] == res_occupancy
+    ), "All residues must have the same number of solute_atoms atoms on them."
 
     res_atom_array = np.array(list(res_atom_local_ix.values()))
-    assert np.all(res_atom_array[0] == res_atom_array), (
-        "All residues must have the same solute_atoms atoms on them."
-    )
+    assert np.all(
+        res_atom_array[0] == res_atom_array
+    ), "All residues must have the same solute_atoms atoms on them."
 
     res_atom_ix_array = np.array(list(res_atom_ix.values()))
     solute_atom_group_dict = {}
     for i in range(0, res_atom_ix_array.shape[1]):
-        solute_atom_group_dict[i] = solute_atom_group.universe.atoms[res_atom_ix_array[:, i]]
+        solute_atom_group_dict[i] = solute_atom_group.universe.atoms[
+            res_atom_ix_array[:, i]
+        ]
     return solute_atom_group_dict
 
 
-def verify_solute_atoms_dict(solute_atoms_dict):
+def verify_solute_atoms_dict(
+    solute_atoms_dict: dict[str, mda.AtomGroup],
+) -> mda.AtomGroup:
     # first we verify the input format
     atom_group_lengths = []
     for solute_name, solute_atom_group in solute_atoms_dict.items():
-        assert isinstance(solute_name, str), (
-            "The keys of solutes_dict must be strings."
-        )
+        assert isinstance(solute_name, str), "The keys of solutes_dict must be strings."
         assert isinstance(solute_atom_group, mda.AtomGroup), (
             f"The values of solutes_dict must be MDAnalysis.AtomGroups. But the value"
             f"for {solute_name} is a {type(solute_atom_group)}."
         )
-        assert len(solute_atom_group) == len(solute_atom_group.residues), (
-            "The solute_atom_group must have a single atom on each residue."
-        )
+        assert len(solute_atom_group) == len(
+            solute_atom_group.residues
+        ), "The solute_atom_group must have a single atom on each residue."
         atom_group_lengths.append(len(solute_atom_group))
     assert np.all(np.array(atom_group_lengths) == atom_group_lengths[0]), (
         "AtomGroups in solutes_dict must have the same length because there should be"
         "one atom per solute residue."
     )
 
     # verify that the solute_atom_groups have no overlap
-    solute_atom_group = reduce(lambda x, y: x | y, [atoms for atoms in solute_atoms_dict.values()])
-    assert solute_atom_group.n_atoms == sum([atoms.n_atoms for atoms in solute_atoms_dict.values()]), (
-        "The solute_atom_groups must not overlap."
+    solute_atom_group = reduce(
+        lambda x, y: x | y, [atoms for atoms in solute_atoms_dict.values()]
     )
+    assert solute_atom_group.n_atoms == sum(
+        [atoms.n_atoms for atoms in solute_atoms_dict.values()]
+    ), "The solute_atom_groups must not overlap."
     verify_solute_atoms(solute_atom_group)
 
     return solute_atom_group
 
 
-def get_atom_group(selection):
+def get_atom_group(
+    selection: Union[
+        mda.core.groups.Residue,
+        mda.core.groups.ResidueGroup,
+        mda.core.groups.Atom,
+        mda.core.groups.AtomGroup,
+    ],
+) -> mda.AtomGroup:
     """
     Cast an MDAnalysis.Atom, MDAnalysis.Residue, or MDAnalysis.ResidueGroup to AtomGroup.
 
     Parameters
     ----------
     selection: MDAnalysis.Atom, MDAnalysis.Residue or MDAnalysis.ResidueGroup
         atoms to cast
@@ -97,20 +111,29 @@
         selection = selection.atoms
     if isinstance(selection, mda.core.groups.Atom):
         selection = u.select_atoms(f"index {selection.index}")
     return selection
 
 
 def get_closest_n_mol(
-    central_species,
-    n_mol,
-    guess_radius=3,
-    return_ordered_resix=False,
-    return_radii=False,
-):
+    central_species: Union[
+        mda.core.groups.Residue,
+        mda.core.groups.ResidueGroup,
+        mda.core.groups.Atom,
+        mda.core.groups.AtomGroup,
+    ],
+    n_mol: int,
+    guess_radius: Union[float, int] = 3,
+    return_ordered_resix: bool = False,
+    return_radii: bool = False,
+) -> Union[
+    mda.AtomGroup,
+    tuple[mda.AtomGroup, np.ndarray],
+    tuple[mda.AtomGroup, np.ndarray, np.ndarray],
+]:
     """
     Returns the closest n molecules to the central species, an array of their resix,
     and an array of the distance of the closest atom in each molecule.
 
     Parameters
     ----------
     central_species : MDAnalysis.Atom, MDAnalysis.AtomGroup, MDAnalysis.Residue or MDAnalysis.ResidueGroup
@@ -144,23 +167,23 @@
     shell_resix = partial_shell.resindices
     if len(np.unique(shell_resix)) < n_mol + 1:
         return get_closest_n_mol(
             central_species,
             n_mol,
             guess_radius + 1,
             return_ordered_resix=return_ordered_resix,
-            return_radii=return_radii
+            return_radii=return_radii,
         )
     radii = distances.distance_array(coords, partial_shell.positions, box=u.dimensions)[
         0
     ]
     ordering = np.argsort(radii)
     ordered_resix = shell_resix[ordering]
     closest_n_resix = np.sort(np.unique(ordered_resix, return_index=True)[1])[
-        0: n_mol + 1
+        0 : n_mol + 1
     ]
     str_resix = " ".join(str(resix) for resix in ordered_resix[closest_n_resix])
     full_shell = u.select_atoms(f"resindex {str_resix}")
     if return_ordered_resix and return_radii:
         return (
             full_shell,
             ordered_resix[closest_n_resix],
@@ -170,15 +193,23 @@
         return full_shell, ordered_resix[closest_n_resix]
     elif return_radii:
         return full_shell, radii[ordering][closest_n_resix]
     else:
         return full_shell
 
 
-def get_radial_shell(central_species, radius):
+def get_radial_shell(
+    central_species: Union[
+        mda.core.groups.Residue,
+        mda.core.groups.ResidueGroup,
+        mda.core.groups.Atom,
+        mda.core.groups.AtomGroup,
+    ],
+    radius: Union[float, int],
+) -> mda.AtomGroup:
     """
     Returns all molecules with atoms within the radius of the central species.
     (specifically, within the radius of the COM of central species).
 
     Parameters
     ----------
     central_species : MDAnalysis.Atom, MDAnalysis.AtomGroup, MDAnalysis.Residue, or MDAnalysis.ResidueGroup
@@ -195,15 +226,15 @@
     coords = central_species.center_of_mass()
     str_coords = " ".join(str(coord) for coord in coords)
     partial_shell = u.select_atoms(f"point {str_coords} {radius}")
     full_shell = partial_shell.residues.atoms
     return full_shell
 
 
-def calculate_adjacency_dataframe(solvation_data):
+def calculate_adjacency_dataframe(solvation_data: pd.DataFrame) -> pd.DataFrame:
     """
     Calculate a frame-by-frame adjacency matrix from the solvation data.
 
     This will calculate the adjacency matrix of the solute and all possible
     solvents. It will maintain an index of ["frame", "solute_atom", "solvent"]
     where each "frame" is a sparse adjacency matrix between solvated atom ix
     and residue ix.
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/coordination.py` & `solvation_analysis-0.4.0/solvation_analysis/coordination.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,26 @@
 
 While ``coordination`` can be used in isolation, it is meant to be used
 as an attribute of the Solute class. This makes instantiating it and calculating the
 solvation data a non-issue.
 """
 
 import pandas as pd
+import MDAnalysis as mda
+import solvation_analysis
 
-from solvation_analysis._column_names import *
+from solvation_analysis._column_names import (
+    FRAME,
+    SOLUTE_IX,
+    SOLVENT,
+    SOLVENT_IX,
+    SOLVENT_ATOM_IX,
+    ATOM_TYPE,
+    FRACTION,
+)
 
 
 class Coordination:
     """
     Calculate the coordination number for each solvent.
 
     Coordination calculates the coordination number by averaging the number of
@@ -35,15 +45,15 @@
 
     The coordination numbers are made available as an mean over the whole
     simulation and by frame.
 
     Parameters
     ----------
     solvation_data : pandas.DataFrame
-        The solvation data frame output by Solute.
+        The solvation dataframe output by Solute.
     n_frames : int
         The number of frames in solvation_data.
     n_solutes : int
         The number of solutes in solvation_data.
     solvent_counts: Dict[str, int]
         A dictionary of the number of residues for each solvent.
     atom_group : MDAnalysis.core.groups.AtomGroup
@@ -58,26 +68,33 @@
         >>> solute = Solute(Li, {'BN': BN, 'FEC': FEC, 'PF6': PF6})
         >>> solute.run()
         >>> solute.coordination.coordination_numbers
         {'BN': 4.328, 'FEC': 0.253, 'PF6': 0.128}
 
     """
 
-    def __init__(self, solvation_data, n_frames, n_solutes, solvent_counts, atom_group):
+    def __init__(
+        self,
+        solvation_data: pd.DataFrame,
+        n_frames: int,
+        n_solutes: int,
+        solvent_counts: dict[str, int],
+        atom_group: mda.core.groups.AtomGroup,
+    ) -> None:
         self.solvation_data = solvation_data
         self.n_frames = n_frames
         self.n_solutes = n_solutes
         self._cn_dict, self._cn_dict_by_frame = self._mean_cn()
         self.atom_group = atom_group
         self._coordinating_atoms = self._calculate_coordinating_atoms()
         self.solvent_counts = solvent_counts
         self._coordination_vs_random = self._calculate_coordination_vs_random()
 
     @staticmethod
-    def from_solute(solute):
+    def from_solute(solute: "solvation_analysis.Solute") -> "Coordination":
         """
         Generate a Coordination object from a solute.
 
         Parameters
         ----------
         solute : Solute
 
@@ -90,52 +107,55 @@
             solute.solvation_data,
             solute.n_frames,
             solute.n_solutes,
             solute.solvent_counts,
             solute.u.atoms,
         )
 
-    def _mean_cn(self):
-        counts = self.solvation_data.groupby([FRAME, SOLUTE_IX, SOLVENT]).count()[SOLVENT_IX]
+    def _mean_cn(self) -> tuple[dict[str, float], pd.DataFrame]:
+        counts = self.solvation_data.groupby([FRAME, SOLUTE_IX, SOLVENT]).count()[
+            SOLVENT_IX
+        ]
         cn_series = counts.groupby([SOLVENT, FRAME]).sum() / (
-                self.n_solutes * self.n_frames
+            self.n_solutes * self.n_frames
         )
         cn_by_frame = cn_series.unstack()
         cn_dict = cn_series.groupby([SOLVENT]).sum().to_dict()
         return cn_dict, cn_by_frame
 
-    def _calculate_coordinating_atoms(self, tol=0.005):
+    def _calculate_coordinating_atoms(self, tol: float = 0.005) -> pd.DataFrame:
         """
         Determine which atom types are actually coordinating
         return the types of those atoms
         """
         # lookup atom types
         atom_types = self.solvation_data.reset_index([SOLVENT_ATOM_IX])
-        atom_types[ATOM_TYPE] = self.atom_group[atom_types[SOLVENT_ATOM_IX].values].types
+        atom_types[ATOM_TYPE] = self.atom_group[
+            atom_types[SOLVENT_ATOM_IX].values
+        ].types
         # count atom types
         atoms_by_type = atom_types[[ATOM_TYPE, SOLVENT, SOLVENT_ATOM_IX]]
         type_counts = atoms_by_type.groupby([SOLVENT, ATOM_TYPE]).count()
         solvent_counts = type_counts.groupby([SOLVENT]).sum()[SOLVENT_ATOM_IX]
         # calculate fraction of each
         solvent_counts_list = [
-            solvent_counts[solvent] for solvent in
-            type_counts.index.get_level_values(SOLVENT)
+            solvent_counts[solvent]
+            for solvent in type_counts.index.get_level_values(SOLVENT)
         ]
         type_fractions = type_counts[SOLVENT_ATOM_IX] / solvent_counts_list
         type_fractions.name = FRACTION
         # change index type
         type_fractions = (
-            type_fractions
-            .reset_index(ATOM_TYPE)
+            type_fractions.reset_index(ATOM_TYPE)
             .astype({ATOM_TYPE: str})
             .set_index(ATOM_TYPE, append=True)
         )
         return type_fractions[type_fractions[FRACTION] > tol]
 
-    def _calculate_coordination_vs_random(self):
+    def _calculate_coordination_vs_random(self) -> dict[str, float]:
         """
         Calculate the coordination number relative to random coordination.
 
         Values higher than 1 imply a higher coordination than expected from
         random distribution of solvents. Values lower than 1 imply a lower
         coordination than expected from random distribution of solvents.
         """
@@ -146,37 +166,37 @@
             count = self.solvent_counts[solvent]
             random = count * average_shell_size / total_solvents
             vs_random = cn / random
             coordination_vs_random[solvent] = vs_random
         return coordination_vs_random
 
     @property
-    def coordination_numbers(self):
+    def coordination_numbers(self) -> dict[str, float]:
         """
         A dictionary where keys are residue names (str) and values are the
         mean coordination number of that residue (float).
         """
         return self._cn_dict
 
     @property
-    def coordination_numbers_by_frame(self):
+    def coordination_numbers_by_frame(self) -> pd.DataFrame:
         """
         A DataFrame of the mean coordination number of in each frame of the trajectory.
         """
         return self._cn_dict_by_frame
 
     @property
-    def coordinating_atoms(self):
+    def coordinating_atoms(self) -> pd.DataFrame:
         """
         Fraction of each atom_type participating in solvation, calculated for each solvent.
         """
         return self._coordinating_atoms
 
     @property
-    def coordination_vs_random(self):
+    def coordination_vs_random(self) -> dict[str, float]:
         """
         Coordination number relative to random coordination.
 
         Values higher than 1 imply a higher coordination than expected from
         random distribution of solvents. Values lower than 1 imply a lower
         coordination than expected from random distribution of solvents.
         """
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/networking.py` & `solvation_analysis-0.4.0/solvation_analysis/networking.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,34 @@
 in the solute, regardless of identify. This could include cation-anion networks
 or hydrogen bond networks.
 
 While ``networking`` can be used in isolation, it is meant to be used
 as an attribute of the Solute class. This makes instantiating it and calculating the
 solvation data a non-issue.
 """
+
+from typing import Union
+
 import pandas as pd
 import numpy as np
 from scipy.sparse import csr_matrix
 from scipy.sparse.csgraph import connected_components
 
+import solvation_analysis
 from solvation_analysis._utils import calculate_adjacency_dataframe
-from solvation_analysis._column_names import *
+from solvation_analysis._column_names import (
+    FRAME,
+    SOLVENT,
+    SOLVENT_IX,
+    SOLUTE_IX,
+    NETWORK,
+    PAIRED,
+    NETWORKED,
+    ISOLATED,
+)
 
 
 class Networking:
     """
     Calculate the number and size of solute-solvent networks.
 
     A network is defined as a bipartite graph of solutes and solvents, where edges
@@ -57,31 +70,41 @@
      .. code-block:: python
 
         # first define Li, BN, and FEC AtomGroups
         >>> solute = Solute.from_atoms(Li, {'BN': BN, 'FEC': FEC, 'PF6': PF6})
         >>> networking = Networking.from_solute(solute, 'PF6')
     """
 
-    def __init__(self, solvents, solvation_data, solute_res_ix, res_name_map):
+    def __init__(
+        self,
+        solvents: Union[str, list[str]],
+        solvation_data: pd.DataFrame,
+        solute_res_ix: np.ndarray,
+        res_name_map: pd.Series,
+    ) -> None:
         self.solvents = solvents
         self.solvation_data = solvation_data
-        solvent_present = np.isin(self.solvents, self.solvation_data[SOLVENT].unique())
         # TODO: we need all analysis classes to run when there is no solvation_data
+        # solvent_present = np.isin(self.solvents, self.solvation_data[SOLVENT].unique())
         # if not solvent_present.all():
         #     raise Exception(f"Solvent(s) {np.array(self.solvents)[~solvent_present]} not found in solvation data.")
         self.solute_res_ix = solute_res_ix
         self.res_name_map = res_name_map
         self.n_solute = len(solute_res_ix)
         self._network_df = self._generate_networks()
         self._network_sizes = self._calculate_network_sizes()
-        self._solute_status, self._solute_status_by_frame = self._calculate_solute_status()
+        self._solute_status, self._solute_status_by_frame = (
+            self._calculate_solute_status()
+        )
         self._solute_status = self._solute_status.to_dict()
 
     @staticmethod
-    def from_solute(solute, solvents):
+    def from_solute(
+        solute: "solvation_analysis.Solute", solvents: Union[str, list[str]]
+    ) -> "Networking":
         """
         Generate a Networking object from a solute and solvent names.
 
         Parameters
         ----------
         solute : Solute
         solvents : str or list of str
@@ -98,95 +121,103 @@
             solvents,
             solute.solvation_data,
             solute.solute_res_ix,
             solute.res_name_map,
         )
 
     @staticmethod
-    def _unwrap_adjacency_dataframe(df):
+    def _unwrap_adjacency_dataframe(df: pd.DataFrame) -> csr_matrix:
         # this class will transform the biadjacency matrix into a proper adjacency matrix
         connections = df.reset_index(FRAME).drop(columns=FRAME)
         idx = connections.columns.append(connections.index)
         directed = connections.reindex(index=idx, columns=idx, fill_value=0)
         undirected = directed.values + directed.values.T
         adjacency_matrix = csr_matrix(undirected)
         return adjacency_matrix
 
-    def _generate_networks(self):
+    def _generate_networks(self) -> pd.DataFrame:
         """
         This function generates a dataframe containing all the solute-solvent networks
         in every frame of the simulation. The rough approach is as follows:
 
         1. transform the solvation_data DataFrame into an adjacency matrix
         2. determine the connected subgraphs in the adjacency matrix
         3. tabulate the solvent involved in each network and store in a DataFrame
         """
         solvents = [self.solvents] if isinstance(self.solvents, str) else self.solvents
-        solvation_subset = self.solvation_data[np.isin(self.solvation_data[SOLVENT], solvents)]
+        solvation_subset = self.solvation_data[
+            np.isin(self.solvation_data[SOLVENT], solvents)
+        ]
         # create adjacency matrix from solvation_subset
         graph = calculate_adjacency_dataframe(solvation_subset)
         network_arrays = []
         # loop through each time step / frame
         for frame, df in graph.groupby(FRAME):
             # drop empty columns
             df = df.loc[:, (df != 0).any(axis=0)]
             # save map from local index to residue index
             solute_map = df.index.get_level_values(SOLUTE_IX).values
             solvent_map = df.columns.values
             ix_to_res_ix = np.concatenate([solvent_map, solute_map])
             adjacency_df = Networking._unwrap_adjacency_dataframe(df)
             _, network = connected_components(
-                csgraph=adjacency_df,
-                directed=False,
-                return_labels=True
+                csgraph=adjacency_df, directed=False, return_labels=True
             )
-            network_array = np.vstack([
-                np.full(len(network), frame),  # frame
-                network,  # network
-                self.res_name_map[ix_to_res_ix],  # res_names
-                ix_to_res_ix,  # res index
-            ]).T
+            network_array = np.vstack(
+                [
+                    np.full(len(network), frame),  # frame
+                    network,  # network
+                    self.res_name_map[ix_to_res_ix],  # res_names
+                    ix_to_res_ix,  # res index
+                ]
+            ).T
             network_arrays.append(network_array)
         # create and return network dataframe
         if len(network_arrays) == 0:
             all_clusters = []
         else:
             all_clusters = np.concatenate(network_arrays)
         cluster_df = (
             pd.DataFrame(all_clusters, columns=[FRAME, NETWORK, SOLVENT, SOLVENT_IX])
-                .set_index([FRAME, NETWORK])
-                .sort_values([FRAME, NETWORK])
+            .set_index([FRAME, NETWORK])
+            .sort_values([FRAME, NETWORK])
         )
         return cluster_df
 
-    def _calculate_network_sizes(self):
+    def _calculate_network_sizes(self) -> pd.DataFrame:
         # This utility calculates the network sizes and returns a convenient dataframe.
         cluster_df = self.network_df
         cluster_sizes = cluster_df.groupby([FRAME, NETWORK]).count()
-        size_counts = cluster_sizes.groupby([FRAME, SOLVENT]).count().unstack(fill_value=0)
-        size_counts.columns = size_counts.columns.droplevel(None)  # the column value is None
+        size_counts = (
+            cluster_sizes.groupby([FRAME, SOLVENT]).count().unstack(fill_value=0)
+        )
+        size_counts.columns = size_counts.columns.droplevel(
+            None
+        )  # the column value is None
         return size_counts
 
-    def _calculate_solute_status(self):
+    def _calculate_solute_status(self) -> tuple[pd.Series, pd.DataFrame]:
         """
         This utility calculates the fraction of each solute with a given "status".
         Namely, whether the solvent is "isolated", "paired" (with a single solvent), or
         "networked" of > 2 species.
         """
         # an empty df with the right index
         status = self.network_sizes.iloc[:, 0:0]
         status[PAIRED] = self.network_sizes.iloc[:, 0:1].sum(axis=1).astype(int)
         status[NETWORKED] = self.network_sizes.iloc[:, 1:].sum(axis=1).astype(int)
-        status[ISOLATED] = self.n_solute - status.loc[:, [PAIRED, NETWORKED]].sum(axis=1)
+        status[ISOLATED] = self.n_solute - status.loc[:, [PAIRED, NETWORKED]].sum(
+            axis=1
+        )
         status = status.loc[:, [ISOLATED, PAIRED, NETWORKED]]
         solute_status_by_frame = status / self.n_solute
         solute_status = solute_status_by_frame.mean()
         return solute_status, solute_status_by_frame
 
-    def get_network_res_ix(self, network_index, frame):
+    def get_network_res_ix(self, network_index: int, frame: int) -> np.ndarray:
         """
         Return the indexes of all residues in a selected network.
 
         The network_index and frame must be provided to fully specify the network.
         Once the indexes are returned, they can be used to select an AtomGroup with
         the species of interest, see Examples.
 
@@ -209,50 +240,52 @@
             >>> solute = Solute(Li, {'BN': BN, 'FEC': FEC, 'PF6': PF6})
             >>> networking = Networking.from_solute(solute, 'PF6')
             >>> res_ix = networking.get_network_res_ix(1, 5)
             >>> solute.u.residues[res_ix].atoms
             <AtomGroup with 126 Atoms>
 
         """
-        res_ix = self.network_df.loc[pd.IndexSlice[frame, network_index], SOLVENT_IX].values
+        res_ix = self.network_df.loc[
+            pd.IndexSlice[frame, network_index], SOLVENT_IX
+        ].values
         return res_ix.astype(int)
 
     @property
-    def network_df(self):
+    def network_df(self) -> pd.DataFrame:
         """
         The dataframe containing all networking data. the indices are the frame and
         network index, respectively. the columns are the solvent_name and res_ix.
         """
         return self._network_df
 
     @property
-    def network_sizes(self):
+    def network_sizes(self) -> pd.DataFrame:
         """
         A dataframe of network sizes. the index is the frame. the column headers
         are network sizes, or the number of solutes + solvents in the network, so
         the columns might be [2, 3, 4, ...]. the values in each column are the
         number of networks with that size in each frame.
         """
         return self._network_sizes
 
     @property
-    def solute_status(self):
+    def solute_status(self) -> dict[str, float]:
         """
         A dictionary where the keys are the "status" of the solute and the values
         are the fraction of solute with that status, averaged over all frames.
         "isolated" means that the solute not coordinated with any of the networking
         solvents, network size is 1.
         "paired" means the solute and is coordinated with a single networking
         solvent and that solvent is not coordinated to any other solutes, network
         size is 2.
         "networked" means that the solute is coordinated to more than one solvent
         or its solvent is coordinated to more than one solute, network size >= 3.
         """
         return self._solute_status
 
     @property
-    def solute_status_by_frame(self):
+    def solute_status_by_frame(self) -> pd.DataFrame:
         """
         As described above, except organized into a dataframe where each
         row is a unique frame and the columns are "isolated", "paired", and "networked".
         """
         return self._solute_status_by_frame
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/pairing.py` & `solvation_analysis-0.4.0/solvation_analysis/pairing.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,15 +15,22 @@
 as an attribute of the Solute class. This makes instantiating it and calculating the
 solvation data a non-issue.
 """
 
 import pandas as pd
 import numpy as np
 
-from solvation_analysis._column_names import *
+import solvation_analysis
+from solvation_analysis._column_names import (
+    FRAME,
+    SOLUTE_IX,
+    SOLVENT,
+    SOLVENT_IX,
+    DISTANCE,
+)
 
 
 class Pairing:
     """
     Calculate the fraction of solutes that are coordinated with each solvent.
 
     The pairing fraction is the fraction of solutes that are coordinated with
@@ -32,15 +39,15 @@
 
     The pairing fractions are made available as an mean over the whole
     simulation and by frame.
 
     Parameters
     ----------
     solvation_data : pandas.DataFrame
-        The solvation data frame output by Solute.
+        The solvation dataframe output by Solute.
     n_frames : int
         The number of frames in solvation_data.
     n_solutes : int
         The number of solutes in solvation_data.
     n_solvents : dict of {str: int}
         The number of each kind of solvent.
 
@@ -52,25 +59,35 @@
         # first define Li, BN, and FEC AtomGroups
         >>> solute = Solute(Li, {'BN': BN, 'FEC': FEC, 'PF6': PF6})
         >>> solute.run()
         >>> solute.pairing.solvent_pairing
         {'BN': 1.0, 'FEC': 0.210, 'PF6': 0.120}
     """
 
-    def __init__(self, solvation_data, n_frames, n_solutes, n_solvents):
+    def __init__(
+        self,
+        solvation_data: pd.DataFrame,
+        n_frames: int,
+        n_solutes: int,
+        n_solvents: dict[str, int],
+    ) -> None:
         self.solvation_data = solvation_data
         self.n_frames = n_frames
         self.n_solutes = n_solutes
         self.solvent_counts = n_solvents
         self._solvent_pairing, self._pairing_by_frame = self._fraction_coordinated()
         self._fraction_free_solvents = self._fraction_free_solvent()
-        self._diluent_composition, self._diluent_composition_by_frame, self._diluent_counts = self._diluent_composition()
+        (
+            self._diluent_composition,
+            self._diluent_composition_by_frame,
+            self._diluent_counts,
+        ) = self._diluent_composition()
 
     @staticmethod
-    def from_solute(solute):
+    def from_solute(solute: "solvation_analysis.Solute") -> "Pairing":
         """
         Generate a Pairing object from a solute.
 
         Parameters
         ----------
         solute : Solute
 
@@ -79,84 +96,94 @@
         Pairing
         """
         assert solute.has_run, "The solute must be run before calling from_solute"
         return Pairing(
             solute.solvation_data,
             solute.n_frames,
             solute.n_solutes,
-            solute.solvent_counts
+            solute.solvent_counts,
         )
 
-    def _fraction_coordinated(self):
+    def _fraction_coordinated(self) -> tuple[dict[str, float], pd.DataFrame]:
         # calculate the fraction of solute coordinated with each solvent
-        counts = self.solvation_data.groupby([FRAME, SOLUTE_IX, SOLVENT]).count()[SOLVENT_IX]
+        counts = self.solvation_data.groupby([FRAME, SOLUTE_IX, SOLVENT]).count()[
+            SOLVENT_IX
+        ]
         pairing_series = counts.astype(bool).groupby([SOLVENT, FRAME]).sum() / (
             self.n_solutes
         )  # mean coordinated overall
         pairing_by_frame = pairing_series.unstack()
         pairing_normalized = pairing_series / self.n_frames
         pairing_dict = pairing_normalized.groupby([SOLVENT]).sum().to_dict()
         return pairing_dict, pairing_by_frame
 
-    def _fraction_free_solvent(self):
+    def _fraction_free_solvent(self) -> dict[str, float]:
         # calculate the fraction of each solvent NOT coordinated with the solute
-        counts = self.solvation_data.groupby([FRAME, SOLVENT_IX, SOLVENT]).count()[DISTANCE]
+        counts = self.solvation_data.groupby([FRAME, SOLVENT_IX, SOLVENT]).count()[
+            DISTANCE
+        ]
         totals = counts.groupby([SOLVENT]).count() / self.n_frames
-        n_solvents = np.array([self.solvent_counts[name] for name in totals.index.values])
+        n_solvents = np.array(
+            [self.solvent_counts[name] for name in totals.index.values]
+        )
         free_solvents = np.ones(len(totals)) - totals / n_solvents
         return free_solvents.to_dict()
 
-    def _diluent_composition(self):
-        coordinated_solvents = self.solvation_data.groupby([FRAME, SOLVENT]).nunique()[SOLVENT_IX]
+    def _diluent_composition(
+        self,
+    ) -> tuple[dict[str, float], pd.DataFrame, pd.DataFrame]:
+        coordinated_solvents = self.solvation_data.groupby([FRAME, SOLVENT]).nunique()[
+            SOLVENT_IX
+        ]
         solvent_counts = pd.Series(self.solvent_counts)
         total_solvents = solvent_counts.reindex(coordinated_solvents.index, level=1)
         diluent_solvents = total_solvents - coordinated_solvents
         diluent_series = diluent_solvents / diluent_solvents.groupby([FRAME]).sum()
         diluent_by_frame = diluent_series.unstack().T
         diluent_counts = diluent_solvents.unstack().T
         diluent_dict = diluent_by_frame.mean(axis=1).to_dict()
         return diluent_dict, diluent_by_frame, diluent_counts
 
     @property
-    def solvent_pairing(self):
+    def solvent_pairing(self) -> dict[str, float]:
         """
         A dictionary where keys are residue names (str) and values are the
         fraction of solutes that contain that residue (float).
         """
         return self._solvent_pairing
 
     @property
-    def pairing_by_frame(self):
+    def pairing_by_frame(self) -> pd.DataFrame:
         """
         A pd.Dataframe tracking the mean fraction of each residue across frames.
         """
         return self._pairing_by_frame
 
     @property
-    def fraction_free_solvents(self):
+    def fraction_free_solvents(self) -> dict[str, float]:
         """
         A dictionary containing the fraction of each solvent that is free. e.g.
         not coordinated to a solute.
         """
         return self._fraction_free_solvents
 
     @property
-    def diluent_composition(self):
+    def diluent_composition(self) -> dict[str, float]:
         """
         The fraction of the diluent constituted by each solvent. The diluent is
         defined as everything that is not coordinated with the solute.
         """
         return self._diluent_composition
 
     @property
-    def diluent_composition_by_frame(self):
+    def diluent_composition_by_frame(self) -> pd.DataFrame:
         """
         A DataFrame of the diluent composition in each frame of the trajectory.
         """
         return self._diluent_composition_by_frame
 
     @property
-    def diluent_counts(self):
+    def diluent_counts(self) -> pd.DataFrame:
         """
         A DataFrame of the raw solvent counts in the diluent in each frame of the trajectory.
         """
         return self._diluent_counts
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/rdf_parser.py` & `solvation_analysis-0.4.0/solvation_analysis/rdf_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 :Year: 2021
 :Copyright: GNU Public License v3
 
 RDF Parser defines several functions for finding the solvation cutoff
 from an RDF.
 """
 
+from typing import Any, Optional, Union
+
 import numpy as np
 from scipy.interpolate import UnivariateSpline
 import scipy
 import matplotlib.pyplot as plt
 import warnings
 from scipy.signal import find_peaks, gaussian
 
-from solvation_analysis._column_names import *
-
 
-def interpolate_rdf(bins, rdf, floor=0.05, cutoff=5):
+def interpolate_rdf(
+    bins: np.ndarray, rdf: np.ndarray, floor: float = 0.05, cutoff: float = 5
+) -> tuple[UnivariateSpline, tuple[float, float]]:
     """
     Fits a sciply.interpolate.UnivariateSpline to the starting region of
     the RDF. The floor and cutoff control the region of the RDF that the
     spline is fit to.
 
     Parameters
     ----------
@@ -45,15 +47,15 @@
     start = np.argmax(rdf > floor)  # will return first index > rdf
     end = np.argmax(bins > cutoff)  # will return first index > cutoff
     bounds = (bins[start], bins[end - 1])
     f = UnivariateSpline(bins[start:end], rdf[start:end], k=4, s=0)
     return f, bounds
 
 
-def identify_minima(f):
+def identify_minima(f: UnivariateSpline) -> tuple[np.ndarray, np.ndarray]:
     """
     Identifies the extrema of a interpolated polynomial.
 
     Parameters
     ----------
     f : sciply.interpolate.UnivariateSpline
 
@@ -71,15 +73,17 @@
             " scipy.interpolate.UnivariateSpline output by interpolate_rdf.",
         )
     cr_pts = f.derivative().roots()
     cr_vals = f(cr_pts)
     return cr_pts, cr_vals
 
 
-def plot_interpolation_fit(bins, rdf, **kwargs):
+def plot_interpolation_fit(
+    bins: np.ndarray, rdf: np.ndarray, **kwargs: Any
+) -> tuple[plt.Figure, plt.Axes]:
     """
     Calls interpolate_rdf and identify_minima to identify the extrema of an RDF.
     Plots the original rdf, the interpolated spline, and the extrema of the
     interpolated spline.
 
     Parameters
     ----------
@@ -105,15 +109,17 @@
     ax.set_xlabel("Radial Distance (A)")
     ax.set_ylabel("Probability Density")
     ax.set_title("Interpolation of RDF with quartic spline")
     ax.legend()
     return fig, ax
 
 
-def good_cutoff(cutoff_region, cr_pts, cr_vals):
+def good_cutoff(
+    cutoff_region: tuple[float, float], cr_pts: np.ndarray, cr_vals: np.ndarray
+) -> bool:
     """
     Uses several heuristics to determine if the a solvation cutoff is valid
     solvation cutoff. This fails if there is no solvation shell.
 
     Parameters
     ----------
     f : an interpolated RDF function
@@ -135,30 +141,37 @@
         or abs(cr_vals[1] - cr_vals[0]) < 0.15  # peak too small
     ):
         return False
     else:
         return True
 
 
-def good_cutoff_scipy(cutoff_region, min_trough_depth, peaks, troughs, rdf, bins):
+def good_cutoff_scipy(
+    cutoff_region: tuple[float, float],
+    min_trough_depth: float,
+    peaks: np.ndarray,
+    troughs: np.ndarray,
+    rdf: np.ndarray,
+    bins: np.ndarray,
+) -> bool:
     """
     Uses several heuristics to determine if the solvation cutoff is valid
     solvation cutoff. This fails if there is no solvation shell.
 
     Heuristics:
-      -  trough follows peak
+      -  troughs follows peaks
       -  in `Solute.cutoff_region` (specified by kwarg)
       -  normalized peak height > 0.05
 
     Parameters
     ----------
     cutoff_region : tuple
         boundaries in which to search for a solvation shell cutoff, i.e. (1.5, 4)
     min_trough_depth : float
-        the minimum depth of a trough to be considered a valid solvation cutoff
+        the minimum depth to be considered a valid solvation cutoff
     peaks : np.array
         the indices of the peaks in the bins array
     troughs : np.array
         the indices of the troughs in the bins array
     bins : np.array
         the x-axis bins of the rdf
     rdf : np.array
@@ -167,24 +180,30 @@
     -------
     boolean : True if good cutoff, False if bad cutoff
 
     """
     # normalize rdf
     norm_rdf = rdf / np.max(rdf)
     if (
-        len(peaks) == 0 or len(troughs) == 0  # insufficient critical points
+        len(peaks) == 0
+        or len(troughs) == 0  # insufficient critical points
         or troughs[0] < peaks[0]  # not a min and max
-        or not (cutoff_region[0] < bins[troughs[0]] < cutoff_region[1])  # min not in cutoff
-        or abs(norm_rdf[peaks[0]] - norm_rdf[troughs[0]]) < min_trough_depth  # peak too small
+        or not (
+            cutoff_region[0] < bins[troughs[0]] < cutoff_region[1]
+        )  # min not in cutoff
+        or abs(norm_rdf[peaks[0]] - norm_rdf[troughs[0]])
+        < min_trough_depth  # peak too small
     ):
         return False
     return True
 
 
-def scipy_find_peaks_troughs(bins, rdf, return_rdf=False, **kwargs):
+def scipy_find_peaks_troughs(
+    bins: np.ndarray, rdf: np.ndarray, return_rdf: bool = False, **kwargs: Any
+) -> Union[tuple[np.ndarray, np.ndarray], tuple[np.ndarray, np.ndarray, np.ndarray]]:
     """
     Finds the indices of the peaks and troughs of an RDF.
 
     This function applies the following procedure to identify peaks.
         1. normalize the RDF
         2. apply a gaussian convolution (std=1.1) to the RDF
         3. call scipy.signal.find_peaks on the RDF and -1*RDF to find the peaks and troughs, respectively.
@@ -219,21 +238,22 @@
     peaks, _ = find_peaks(smooth_rdf)
     if return_rdf:
         return peaks, troughs, smooth_rdf * np.max(rdf)
     return peaks, troughs
 
 
 def identify_cutoff_scipy(
-    bins,
-    rdf,
-    cutoff_region=(1.5, 4),
-    failure_behavior="warn",
-    min_trough_depth=0.02,
-    **kwargs
-):
+    bins: np.ndarray,
+    rdf: np.ndarray,
+    cutoff_region: tuple[float, float] = (1.5, 4),
+    failure_behavior: str = "warn",
+    min_trough_depth: float = 0.02,
+    default: Optional[float] = None,
+    **kwargs: Any,
+) -> Optional[float]:
     """
     Identifies the solvation cutoff of an RDF.
 
     This function is a thin wrapper on scipy_find_peaks_trough, see the documentation
     of that function for more detail. It applies a few simple heuristics, specified in
     good_cutoff_scipy, to determine if the solvation cutoff is valid.
 
@@ -244,43 +264,49 @@
     rdf : np.array
         RDF data matching the bins
     cutoff_region : tuple
         boundaries in which to search for a solvation shell cutoff, i.e. (1.5, 4)
     failure_behavior : str
         specifies the behavior of the function if no solvation shell is found, can
         be set to "silent", "warn", or "exception"
+    default : float, optional
+        the value to return if no solvation shell is found
     min_trough_depth : float
-        the minimum depth of a trough to be considered a valid solvation cutoff
+        the minimum depth of troughs to be considered a valid solvation cutoff
     kwargs : passed to the scipy.find_peaks function
 
     Returns
     -------
     cutoff : float
         the solvation cutoff of the RDF
     """
     peaks, troughs = scipy_find_peaks_troughs(bins, rdf, **kwargs)
-    if not good_cutoff_scipy(cutoff_region, min_trough_depth, peaks, troughs, rdf, bins):
+    if not good_cutoff_scipy(
+        cutoff_region, min_trough_depth, peaks, troughs, rdf, bins
+    ):
         if failure_behavior == "silent":
-            return np.NaN
+            return default
         if failure_behavior == "warn":
             warnings.warn("No solvation shell detected.")
-            return np.NaN
+            return default
         if failure_behavior == "exception":
-            raise RuntimeError("Solute could not identify a solvation radius for at least one solvent. "
-                               "Please enter the missing radii manually by adding them to the radii dict"
-                               "and rerun the analysis.")
+            raise RuntimeError(
+                "Solute could not identify a solvation radius for at least one solvent. "
+                "Please enter the missing radii manually by adding them to the radii dict"
+                "and rerun the analysis."
+            )
     cutoff = bins[troughs[0]]
     return cutoff
 
 
 def plot_scipy_find_peaks_troughs(
-    bins,
-    rdf,
-    **kwargs,
-):
+    bins: np.ndarray,
+    rdf: np.ndarray,
+    **kwargs: Any,
+) -> tuple[plt.Figure, plt.Axes]:
     """
     Plot the original and smoothed RDF with the peaks and troughs located.
 
     This function is a thin wrapper on scipy_find_peaks_trough, see the documentation
     of that function for more detail.
 
     Parameters
@@ -293,30 +319,37 @@
         passed to scipy.signal.find_peaks
 
     Returns
     -------
     fig, ax : matplotlib pyplot Figure and Axis for the fit
 
     """
-    peaks, troughs, smooth_rdf = scipy_find_peaks_troughs(bins, rdf, return_rdf=True, **kwargs)
+    peaks, troughs, smooth_rdf = scipy_find_peaks_troughs(
+        bins, rdf, return_rdf=True, **kwargs
+    )
     fig, ax = plt.subplots()
     ax.plot(bins, rdf, "b--", label="rdf")
     ax.plot(bins, smooth_rdf, "g-", label="smooth_rdf")
     ax.plot(bins[troughs], rdf[troughs], "go", label="troughs")
     ax.plot(bins[peaks], rdf[peaks], "ro", label="peaks")
     ax.set_xlabel("Radial Distance (A)")
     ax.set_ylabel("Probability Density")
     ax.set_title("RDF minima using scipy.find_peaks")
     ax.legend()
     return fig, ax
 
 
 def identify_cutoff_poly(
-    bins, rdf, failure_behavior="warn", cutoff_region=(1.5, 4), floor=0.05, cutoff=5
-):
+    bins: np.ndarray,
+    rdf: np.ndarray,
+    failure_behavior: str = "warn",
+    cutoff_region: tuple[float, float] = (1.5, 4),
+    floor: float = 0.05,
+    cutoff: float = 5,
+) -> float:
     """
     Identifies the solvation cutoff of an RDF using a polynomial interpolation.
 
     Parameters
     ----------
     bins : np.array
         the x-axis bins of the rdf
@@ -342,11 +375,13 @@
     if not good_cutoff(cutoff_region, cr_pts, cr_vals):
         if failure_behavior == "silent":
             return np.NaN
         if failure_behavior == "warn":
             warnings.warn("No solvation shell detected.")
             return np.NaN
         if failure_behavior == "exception":
-            raise RuntimeError("Solute could not identify a solvation radius for at least one solvent. "
-                               "Please enter the missing radii manually by adding them to the radii dict"
-                               "and rerun the analysis.")
+            raise RuntimeError(
+                "Solute could not identify a solvation radius for at least one solvent. "
+                "Please enter the missing radii manually by adding them to the radii dict"
+                "and rerun the analysis."
+            )
     return cr_pts[1]
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/residence.py` & `solvation_analysis-0.4.0/solvation_analysis/residence.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,24 +11,31 @@
 Residence times for all solvents are automatically calculated from autocovariance
 of the solvent-solute adjacency matrix.
 
 While ``residence`` can be used in isolation, it is meant to be used
 as an attribute of the Solute class. This makes instantiating it and calculating the
 solvation data a non-issue.
 """
+
 import math
 import warnings
 
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 from statsmodels.tsa.stattools import acovf
 from scipy.optimize import curve_fit
 
-from solvation_analysis._column_names import *
+import solvation_analysis
+from solvation_analysis._column_names import (
+    SOLVENT,
+    SOLUTE_ATOM_IX,
+    SOLVENT_ATOM_IX,
+    SOLUTE_IX,
+)
 from solvation_analysis._utils import calculate_adjacency_dataframe
 
 
 class Residence:
     """
     Calculate the residence times of solvents.
 
@@ -79,88 +86,99 @@
         # first define Li, BN, and FEC AtomGroups
         >>> solute = Solute(Li, {'BN': BN, 'FEC': FEC, 'PF6': PF6})
         >>> residence = Residence.from_solute(solute)
         >>> residence.residence_times_cutoff
         {'BN': 4.02, 'FEC': 3.79, 'PF6': 1.15}
     """
 
-    def __init__(self, solvation_data, step):
+    def __init__(self, solvation_data: pd.DataFrame, step: int) -> None:
         self.solvation_data = solvation_data
         self._auto_covariances = self._calculate_auto_covariance_dict()
-        self._residence_times_cutoff = self._calculate_residence_times_with_cutoff(self._auto_covariances, step)
-        self._residence_times_fit, self._fit_parameters = self._calculate_residence_times_with_fit(
-            self._auto_covariances,
-            step
+        self._residence_times_cutoff = self._calculate_residence_times_with_cutoff(
+            self._auto_covariances, step
+        )
+        self._residence_times_fit, self._fit_parameters = (
+            self._calculate_residence_times_with_fit(self._auto_covariances, step)
         )
 
     @staticmethod
-    def from_solute(solute):
+    def from_solute(solute: "solvation_analysis.Solute") -> "Residence":
         """
         Generate a Residence object from a solute.
 
         Parameters
         ----------
         solute : Solute
 
         Returns
         -------
         Residence
         """
         assert solute.has_run, "The solute must be run before calling from_solute"
-        return Residence(
-            solute.solvation_data,
-            solute.step
-        )
+        return Residence(solute.solvation_data, solute.step)
 
-    def _calculate_auto_covariance_dict(self):
+    def _calculate_auto_covariance_dict(self) -> dict[str, np.ndarray]:
         partial_index = self.solvation_data.index.droplevel(SOLVENT_ATOM_IX)
         unique_indices = np.unique(partial_index)
-        frame_solute_index = pd.MultiIndex.from_tuples(unique_indices, names=partial_index.names)
+        frame_solute_index = pd.MultiIndex.from_tuples(
+            unique_indices, names=partial_index.names
+        )
         auto_covariance_dict = {}
         for res_name, res_solvation_data in self.solvation_data.groupby([SOLVENT]):
             if isinstance(res_name, tuple):
                 res_name = res_name[0]
             adjacency_mini = calculate_adjacency_dataframe(res_solvation_data)
             adjacency_df = adjacency_mini.reindex(frame_solute_index, fill_value=0)
             auto_covariance = Residence._calculate_auto_covariance(adjacency_df)
             # normalize
             auto_covariance = auto_covariance / np.max(auto_covariance)
             auto_covariance_dict[res_name] = auto_covariance
         return auto_covariance_dict
 
     @staticmethod
-    def _calculate_residence_times_with_cutoff(auto_covariances, step, convergence_cutoff=0.1):
+    def _calculate_residence_times_with_cutoff(
+        auto_covariances: dict[str, np.ndarray],
+        step: int,
+        convergence_cutoff: float = 0.1,
+    ) -> dict[str, float]:
         residence_times = {}
         for res_name, auto_covariance in auto_covariances.items():
             if np.min(auto_covariance) > convergence_cutoff:
                 residence_times[res_name] = np.nan
-                warnings.warn(f'the autocovariance for {res_name} does not converge to zero '
-                              'so a residence time cannot be calculated. A longer simulation '
-                              'is required to get a valid estimate of the residence time.')
+                warnings.warn(
+                    f"the autocovariance for {res_name} does not converge to zero "
+                    "so a residence time cannot be calculated. A longer simulation "
+                    "is required to get a valid estimate of the residence time."
+                )
             unassigned = True
             for frame, val in enumerate(auto_covariance):
                 if val < 1 / math.e:
                     residence_times[res_name] = frame * step
                     unassigned = False
                     break
             if unassigned:
                 residence_times[res_name] = np.nan
         return residence_times
 
     @staticmethod
-    def _calculate_residence_times_with_fit(auto_covariances, step):
+    def _calculate_residence_times_with_fit(
+        auto_covariances: dict[str, np.ndarray], step: int
+    ) -> tuple[dict[str, float], dict[str, tuple[float, float, float]]]:
         # calculate the residence times
         residence_times = {}
         fit_parameters = {}
         for res_name, auto_covariance in auto_covariances.items():
             res_time, params = Residence._fit_exponential(auto_covariance, res_name)
-            residence_times[res_name], fit_parameters[res_name] = round(res_time * step, 2), params
+            residence_times[res_name], fit_parameters[res_name] = (
+                round(res_time * step, 2),
+                params,
+            )
         return residence_times, fit_parameters
 
-    def plot_auto_covariance(self, res_name):
+    def plot_auto_covariance(self, res_name: str) -> tuple[plt.Figure, plt.Axes]:
         """
         Plot the autocovariance of a solvent on the solute.
 
         See the discussion in the class docstring for more information.
 
         Parameters
         ----------
@@ -171,32 +189,37 @@
         -------
         fig : matplotlib.Figure
         ax : matplotlib.Axes
         """
         auto_covariance = self.auto_covariances[res_name]
         frames = np.arange(len(auto_covariance))
         params = self.fit_parameters[res_name]
-        exp_func = lambda x: self._exponential_decay(x, *params)
+
+        def exp_func(x):
+            return self._exponential_decay(x, *params)
+
         exp_fit = np.array(map(exp_func, frames))
         fig, ax = plt.subplots()
         ax.plot(frames, auto_covariance, "b-", label="auto covariance")
         try:
             ax.scatter(frames, exp_fit, label="exponential fit")
-        except:
-            warnings.warn(f'The fit for {res_name} failed so the exponential '
-                          f'fit will not be plotted.')
-        ax.hlines(y=1/math.e, xmin=frames[0], xmax=frames[-1], label='1/e cutoff')
+        except RuntimeError:
+            warnings.warn(
+                f"The fit for {res_name} failed so the exponential "
+                f"fit will not be plotted."
+            )
+        ax.hlines(y=1 / math.e, xmin=frames[0], xmax=frames[-1], label="1/e cutoff")
         ax.set_xlabel("Timestep (frames)")
         ax.set_ylabel("Normalized Autocovariance")
         ax.set_ylim(0, 1)
         ax.legend()
         return fig, ax
 
     @staticmethod
-    def _exponential_decay(x, a, b, c):
+    def _exponential_decay(x: np.ndarray, a: float, b: float, c: float) -> np.ndarray:
         """
         An exponential decay function.
 
         Args:
             x: Independent variable.
             a: Initial quantity.
             b: Exponential decay constant.
@@ -204,80 +227,88 @@
 
         Returns:
             The acf
         """
         return a * np.exp(-b * x) + c
 
     @staticmethod
-    def _fit_exponential(auto_covariance, res_name):
+    def _fit_exponential(
+        auto_covariance: np.ndarray, res_name: str
+    ) -> tuple[float, tuple[float, float, float]]:
         auto_covariance_norm = auto_covariance / auto_covariance[0]
         try:
             params, param_covariance = curve_fit(
                 Residence._exponential_decay,
                 np.arange(len(auto_covariance_norm)),
                 auto_covariance_norm,
                 p0=(1, 0.1, 0.01),
             )
             tau = 1 / params[1]  # p
         except RuntimeError:
-            warnings.warn(f'The fit for {res_name} failed so its values in'
-                          f'residence_time_fits and fit_parameters will be'
-                          f'set to np.nan.')
+            warnings.warn(
+                f"The fit for {res_name} failed so its values in"
+                f"residence_time_fits and fit_parameters will be"
+                f"set to np.nan."
+            )
             tau, params = np.nan, (np.nan, np.nan, np.nan)
         return tau, params
 
     @staticmethod
-    def _calculate_auto_covariance(adjacency_matrix):
+    def _calculate_auto_covariance(adjacency_matrix: pd.DataFrame) -> np.ndarray:
         auto_covariances = []
         timesteps = adjacency_matrix.index.levels[0]
 
-        for solute_ix, solute_df in adjacency_matrix.groupby([SOLUTE_IX, SOLUTE_ATOM_IX]):
+        for solute_ix, solute_df in adjacency_matrix.groupby(
+            [SOLUTE_IX, SOLUTE_ATOM_IX]
+        ):
             # this is needed to make sure auto-covariances can be concatenated later
-            new_solute_df = solute_df.droplevel([SOLUTE_IX, SOLUTE_ATOM_IX]).reindex(timesteps, fill_value=0)
+            new_solute_df = solute_df.droplevel([SOLUTE_IX, SOLUTE_ATOM_IX]).reindex(
+                timesteps, fill_value=0
+            )
             non_zero_cols = new_solute_df.loc[:, (solute_df != 0).any(axis=0)]
             auto_covariance_df = non_zero_cols.apply(
                 acovf,
                 axis=0,
-                result_type='expand',
+                result_type="expand",
                 demean=False,
                 adjusted=True,
-                fft=True
+                fft=True,
             )
             # timesteps with no binding are getting skipped, we need to make sure to include all timesteps
             auto_covariances.append(auto_covariance_df.values)
 
         auto_covariance = np.mean(np.concatenate(auto_covariances, axis=1), axis=1)
         return auto_covariance
 
     @property
-    def auto_covariances(self):
+    def auto_covariances(self) -> dict[str, np.ndarray]:
         """
         A dictionary where keys are residue names and values are the
         autocovariance of the that residue on the solute.
         """
         return self._auto_covariances
 
     @property
-    def residence_times_cutoff(self):
+    def residence_times_cutoff(self) -> dict[str, float]:
         """
         A dictionary where keys are residue names and values are the
         residence times of the that residue on the solute, calculated
         with the 1/e cutoff method.
         """
         return self._residence_times_cutoff
 
     @property
-    def residence_times_fit(self):
+    def residence_times_fit(self) -> dict[str, float]:
         """
         A dictionary where keys are residue names and values are the
         residence times of the that residue on the solute, calculated
         with the exponential fit method.
         """
         return self._residence_times_fit
 
     @property
-    def fit_parameters(self):
+    def fit_parameters(self) -> dict[str, tuple[float, float, float]]:
         """
         A dictionary where keys are residue names and values are the
-        arameters for the exponential fit to the autocorrelation function.
+        parameters for the exponential fit to the autocorrelation function.
         """
         return self._fit_parameters
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/solute.py` & `solvation_analysis-0.4.0/solvation_analysis/solute.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,36 +101,61 @@
 as attributes of the ``Solute``. ``Networking`` and ``Residence`` can also be
 added. These are covered in greater detail in their respective API pages.
 
 Solute also provides several functions to select a particular solute and its
 solvation shell, returning an AtomGroup for visualization or further analysis.
 This is covered in the visualization tutorial.
 """
+
 from collections import defaultdict
 from functools import reduce
+from typing import Any, Callable, Optional, Union
 
-import matplotlib.pyplot as plt
 import pandas as pd
 import warnings
 
 import MDAnalysis as mda
 from MDAnalysis.analysis.base import AnalysisBase
 from MDAnalysis.analysis.rdf import InterRDF
 from MDAnalysis.lib.distances import capped_distance
 import numpy as np
+import plotly.graph_objects as go
 
-from solvation_analysis._utils import verify_solute_atoms, verify_solute_atoms_dict, get_closest_n_mol, get_radial_shell
+from solvation_analysis._utils import (
+    verify_solute_atoms,
+    verify_solute_atoms_dict,
+    get_closest_n_mol,
+    get_radial_shell,
+)
 from solvation_analysis.rdf_parser import identify_cutoff_scipy
 from solvation_analysis.coordination import Coordination
 from solvation_analysis.networking import Networking
 from solvation_analysis.pairing import Pairing
 from solvation_analysis.residence import Residence
 from solvation_analysis.speciation import Speciation
 
-from solvation_analysis._column_names import *
+from solvation_analysis._column_names import (
+    FRAME,
+    DISTANCE,
+    SOLUTE,
+    SOLUTE_IX,
+    SOLVENT,
+    SOLVENT_IX,
+    SOLVENT_ATOM_IX,
+    SOLUTE_ATOM_IX,
+)
+
+try:
+    import rdkit
+    from rdkit.Chem import Draw
+    from rdkit.Chem import rdCoordGen
+    from rdkit.Chem.Draw.MolDrawing import DrawingOptions
+
+except ImportError:
+    rdkit = None
 
 
 class Solute(AnalysisBase):
     """
     Analyze the solvation structure of a solute.
 
     Solute determines the coordination between the solute and solvents,
@@ -156,24 +181,29 @@
     radii : dict of {str: float}, optional
         an optional dictionary of solvent names and associated solvation radii
         e.g. {"name_2": radius_2, "name_5": radius_5} Any radii not given will
         be calculated. The solvent names should match the solvents parameter.
     rdf_kernel : function, optional
         this function must take RDF bins and data as input and return
         a solvation radius as output. e.g. rdf_kernel(bins, data) -> 3.2. By default,
-        the rdf_kernel is solvation_analysis.rdf_parser.identify_solvation_cutoff.
+        the rdf_kernel is `solvation_analysis.rdf_parser.identify_cutoff_scipy`.
     kernel_kwargs : dict, optional
-        kwargs passed to rdf_kernel
+        kwargs passed to rdf_kernel. See `identify_cutoff_scipy` for options. This can
+        be used to set a default fallback radius for all solvents.
     rdf_init_kwargs : dict, optional
         kwargs passed to the initialization of the MDAnalysis.InterRDF used to plot
         the solute-solvent RDFs. By default, ``range`` will be set to (0, 7.5).
     rdf_run_kwargs : dict, optional
         kwargs passed to the internal MDAnalysis.InterRDF.run() command
         e.g. ``inner_rdf.run(**rdf_run_kwargs)``. By default, step, start, and
         stop will use any kwargs provided to ``solute.run(**kwargs)``.
+    skip_rdf : bool, optional
+        skip the RDF generation step. This is useful if you have already
+        calculated the RDFs and have the radii. If True, all radii must be
+        specified in the radii parameter.
     solute_name: str, optional
         the name of the solute, used for labeling.
     analysis_classes : List[str] or str, optional
         a list of the analysis classes to be instantiated, current options are:
         "pairing", "coordination", "speciation", "residence", and "networking".
         By default, only "pairing", "coordination", and "residence" are instantiated.
         If networking is included, the networking_solvents kwarg must be specified.
@@ -227,77 +257,100 @@
     networking : networking.Networking (optional)
         networking analyses the connectivity of solute-solvent networks. Only instantiated
         if 'networking' is included in the analysis_classes kwarg. the networking_solvents
         kwarg must be specified.
     """
 
     def __init__(
-            self,
-            solute_atoms,
-            solvents,
-            atom_solutes=None,
-            radii=None,
-            rdf_kernel=None,
-            kernel_kwargs=None,
-            rdf_init_kwargs=None,
-            rdf_run_kwargs=None,
-            solute_name="solute_0",
-            analysis_classes=None,
-            networking_solvents=None,
-            verbose=False,
-            internal_call=False,
+        self,
+        solute_atoms: mda.AtomGroup,
+        solvents: dict[str, mda.AtomGroup],
+        atom_solutes: Optional[dict[str, "Solute"]] = None,
+        radii: Optional[dict[str, float]] = None,
+        rdf_kernel: Optional[Callable[[np.ndarray, np.ndarray], float]] = None,
+        kernel_kwargs: Optional[dict[str, Any]] = None,
+        rdf_init_kwargs: Optional[dict[str, Any]] = None,
+        rdf_run_kwargs: Optional[dict[str, Any]] = None,
+        skip_rdf: bool = False,
+        solute_name: str = "solute_0",
+        analysis_classes: Optional[list[str]] = None,
+        networking_solvents: Optional[str] = None,
+        verbose: bool = False,
+        internal_call: bool = False,
     ):
         """
         This method is not intended to be called directly. Instead, use
         ``from_atoms``, ``from_atoms_dict`` or ``from_solute_list`` to create a Solute.
         """
         if not internal_call:
-            raise RuntimeError("Please use Solute.from_atoms, Solute.from_atoms_dict, or "
-                               "Solute.from_solute_list instead of the default constructor.")
+            raise RuntimeError(
+                "Please use Solute.from_atoms, Solute.from_atoms_dict, or "
+                "Solute.from_solute_list instead of the default constructor."
+            )
         super(Solute, self).__init__(solute_atoms.universe.trajectory, verbose=verbose)
 
         self.solute_atoms = solute_atoms  # TODO: this shit!
         self.atom_solutes = atom_solutes
         if self.atom_solutes is None or len(atom_solutes) <= 1:
             self.atom_solutes = {solute_name: self}
         self.radii = radii or {}
-        self.solvent_counts = {name: atoms.n_residues for name, atoms in solvents.items()}
+        self.solvent_counts = {
+            name: atoms.n_residues for name, atoms in solvents.items()
+        }
         self.kernel = rdf_kernel or identify_cutoff_scipy
         self.kernel_kwargs = kernel_kwargs or {}
         self.rdf_init_kwargs = rdf_init_kwargs or {}
         self.rdf_run_kwargs = rdf_run_kwargs or {}
         self.has_run = False
         self.u = solute_atoms.universe
         self.n_solutes = solute_atoms.n_residues
-        self.solute_res_ix = pd.Series(solute_atoms.atoms.resindices, solute_atoms.atoms.ix)
+        self.solute_res_ix = pd.Series(
+            solute_atoms.atoms.resindices, solute_atoms.atoms.ix
+        )
         self.solute_name = solute_name
         self.solvents = solvents
+        if skip_rdf:
+            assert set(self.radii.keys()) >= set(
+                self.solvents.keys()
+            ), "To skip RDF generation, all solvent radii must be specified."
+        self.skip_rdf = skip_rdf
 
         # instantiate the res_name_map
-        self.res_name_map = pd.Series(['none'] * len(self.u.residues))
+        self.res_name_map = pd.Series(["none"] * len(self.u.residues))
         self.res_name_map[solute_atoms.residues.ix] = self.solute_name
         for name, solvent in solvents.items():
             self.res_name_map[solvent.residues.ix] = name
 
         # instantiate analysis classes.
         if analysis_classes is None:
             self.analysis_classes = ["pairing", "coordination", "speciation"]
-        elif analysis_classes == 'all':
-            self.analysis_classes = ["pairing", "coordination", "speciation", "residence", "networking"]
+        elif analysis_classes == "all":
+            self.analysis_classes = [
+                "pairing",
+                "coordination",
+                "speciation",
+                "residence",
+                "networking",
+            ]
         else:
             self.analysis_classes = [cls.lower() for cls in analysis_classes]
         if "networking" in self.analysis_classes and networking_solvents is None:
             raise ValueError(
                 "networking analysis requires networking_solvents to be provided."
             )
         else:
             self.networking_solvents = networking_solvents
 
     @staticmethod
-    def from_atoms(solute_atoms, solvents, rename_solutes=None, **kwargs):
+    def from_atoms(
+        solute_atoms: mda.AtomGroup,
+        solvents: dict[str, mda.AtomGroup],
+        rename_solutes: Optional[dict[str, str]] = None,
+        **kwargs: Any,
+    ) -> "Solute":
         """
         Create a Solute from a single AtomGroup. The solute_atoms AtomGroup must
         should contain identical residues and identical atoms on each residue.
         For example, if one wanted to look at the O and H atoms of an ethanol molecule,
         solute_atoms should contain the O and H atoms of all ethanol molecules. It
         could not contain C atoms from some ethanol or include residues
         that were not ethanol.
@@ -329,18 +382,24 @@
         # a dict with keys as integers and values as AtomGroups
         # this will get called again later on with the same input, but for now, it's fine
         solute_atom_group_dict = verify_solute_atoms(solute_atoms)
         solute_atom_group_dict_renamed = {
             rename_solutes.get(f"solute_{i}") or f"solute_{i}": atom_group
             for i, atom_group in solute_atom_group_dict.items()
         }
-        return Solute.from_atoms_dict(solute_atom_group_dict_renamed, solvents, **kwargs)
+        return Solute.from_atoms_dict(
+            solute_atom_group_dict_renamed, solvents, **kwargs
+        )
 
     @staticmethod
-    def from_atoms_dict(solute_atoms_dict, solvents, **kwargs):
+    def from_atoms_dict(
+        solute_atoms_dict: dict[str, mda.AtomGroup],
+        solvents: dict[str, mda.AtomGroup],
+        **kwargs: Any,
+    ) -> "Solute":
         """
         Create a Solute object from a dictionary of solute atoms.
 
         Parameters
         ----------
         solute_atoms_dict: dict of {str: MDAnalysis.AtomGroup}
             a dictionary of solute atoms, e.g. {"name_1": solute_1, "name_2": solute_2}.
@@ -354,40 +413,42 @@
 
         Returns
         -------
         Solute
 
         """
         # all solute AtomGroups in one AtomGroup + verification
-        assert isinstance(solute_atoms_dict, dict), ("Solute_atoms_dict must be a dict.")
+        assert isinstance(solute_atoms_dict, dict), "Solute_atoms_dict must be a dict."
         solute_atom_group = verify_solute_atoms_dict(solute_atoms_dict)
 
         # create the solutes for each atom
         atom_solutes = {}
         for solute_name, atoms in solute_atoms_dict.items():
             atom_solutes[solute_name] = Solute(
                 atoms,
                 solvents,
                 internal_call=True,
-                **{**kwargs, "solute_name": solute_name}
+                **{**kwargs, "solute_name": solute_name},
             )
         # create the solute for the whole solute
         solute = Solute(
             solute_atom_group,
             solvents,
             atom_solutes=atom_solutes,
             internal_call=True,
-            **kwargs
+            **kwargs,
         )
         if len(atom_solutes) > 1:
-           solute.run = solute._run_solute_atoms
+            solute.run = solute._run_solute_atoms
         return solute
 
     @staticmethod
-    def from_solute_list(solutes, solvents, **kwargs):
+    def from_solute_list(
+        solutes: list["Solute"], solvents: dict[str, mda.AtomGroup], **kwargs: Any
+    ) -> "Solute":
         """
         Create a Solute from a list of Solutes. All Solutes must have only a
         single solute atom on each solute residue. Essentially, from_solute_list
         allows you to preconstruct the ``atom_solutes`` dictionary. This is useful
         if you want to individually specify initialization parameters for each
         atom Solute, otherwise, a different constructor is recommended.
 
@@ -406,124 +467,143 @@
         -------
         Solute
 
         """
         # check types and name uniqueness
         for solute in solutes:
             assert type(solute) == Solute, "solutes must be a list of Solute objects."
-            assert len(solute.solute_atoms.atoms) == len(solute.solute_atoms.atoms.residues), (
-                "Each Solute in solutes must have only a single atom per residue."
-            )
+            assert len(solute.solute_atoms.atoms) == len(
+                solute.solute_atoms.atoms.residues
+            ), "Each Solute in solutes must have only a single atom per residue."
         solute_names = [solute.solute_name for solute in solutes]
-        assert len(np.unique(solute_names)) == len(solute_names), (
-            "The solute_name for each solute must be unique."
-        )
+        assert len(np.unique(solute_names)) == len(
+            solute_names
+        ), "The solute_name for each solute must be unique."
 
-        solute_atom_group = reduce(lambda x, y: x | y, [solute.solute_atoms for solute in solutes])
+        solute_atom_group = reduce(
+            lambda x, y: x | y, [solute.solute_atoms for solute in solutes]
+        )
         verify_solute_atoms(solute_atom_group)
 
         atom_solutes = {solute.solute_name: solute for solute in solutes}
         solute = Solute(
             solute_atom_group,
             solvents,
             atom_solutes=atom_solutes,
             internal_call=True,
-            **kwargs
+            **kwargs,
         )
         if len(atom_solutes) > 1:
-           solute.run = solute._run_solute_atoms
+            solute.run = solute._run_solute_atoms
         return solute
 
-    def _run_solute_atoms(self, start=None, stop=None, step=None, verbose=None):
+    def _run_solute_atoms(
+        self,
+        start: Optional[int] = None,
+        stop: Optional[int] = None,
+        step: Optional[int] = None,
+        verbose: Optional[bool] = None,
+    ):
         # like prepare
         atom_solutes = {}
         rdf_data = {}
         solvation_datas = []
         solvation_data_dups = []
         start, stop, step = self.u.trajectory.check_slice_indices(start, stop, step)
         self.start, self.stop, self.step = start, stop, step
         self.n_frames = len(range(start, stop, step))
 
         # like run
         for solute in self.atom_solutes.values():
             if not solute.has_run:
                 solute.run(start=start, stop=stop, step=step, verbose=verbose)
             if (start, stop, step) != (solute.start, solute.stop, solute.step):
-                warnings.warn(f"The start, stop, or step for {solute.solute_name} do not"
-                              f"match the start, stop, or step for the run command so it "
-                              f"is being re-run.")
+                warnings.warn(
+                    f"The start, stop, or step for {solute.solute_name} do not"
+                    f"match the start, stop, or step for the run command so it "
+                    f"is being re-run."
+                )
                 solute.run(start=start, stop=stop, step=step, verbose=verbose)
             if self.solvents != solute.solvents:
-                warnings.warn(f"The solvents for {solute.solute_name} do not match the "
-                              f"solvents for the run command so it is being re-run.")
+                warnings.warn(
+                    f"The solvents for {solute.solute_name} do not match the "
+                    f"solvents for the run command so it is being re-run."
+                )
                 solute.run(start=start, stop=stop, step=step, verbose=verbose)
             atom_solutes[solute.solute_name] = solute
             rdf_data[solute.solute_name] = solute.rdf_data[solute.solute_name]
             solvation_datas.append(solute.solvation_data)
             solvation_data_dups.append(solute.solvation_data_duplicates)
 
         self.rdf_data = rdf_data
         self.solvation_data = pd.concat(solvation_datas).sort_index()
         self.solvation_data_duplicates = pd.concat(solvation_data_dups)
         self.has_run = True
 
         # like conclude
         analysis_classes = {
-            'speciation': Speciation,
-            'pairing': Pairing,
-            'coordination': Coordination,
-            'residence': Residence,
-            'networking': Networking,
+            "speciation": Speciation,
+            "pairing": Pairing,
+            "coordination": Coordination,
+            "residence": Residence,
+            "networking": Networking,
         }
         for analysis_class in self.analysis_classes:
-            if analysis_class == 'networking':
-                setattr(self, 'networking', Networking.from_solute(self, self.networking_solvents))
+            if analysis_class == "networking":
+                setattr(
+                    self,
+                    "networking",
+                    Networking.from_solute(self, self.networking_solvents),
+                )
             else:
-                setattr(self, analysis_class, analysis_classes[analysis_class].from_solute(self))
+                setattr(
+                    self,
+                    analysis_class,
+                    analysis_classes[analysis_class].from_solute(self),
+                )
 
     def _prepare(self):
         """
         This function identifies the solvation radii and saves the associated RDF data.
         """
         self.rdf_data = defaultdict(dict)
         self.solvation_data = None
         self.solvation_data_duplicates = None
         self._solvation_frames = []
         for name, solvent in self.solvents.items():
+            if self.skip_rdf:
+                self.rdf_data = None
+                break
             # set kwargs with defaults
-            self.rdf_init_kwargs["range"] = self.rdf_init_kwargs.get("range") or (0, 7.5)
+            self.rdf_init_kwargs["range"] = self.rdf_init_kwargs.get("range") or (
+                0,
+                7.5,
+            )
             self.rdf_init_kwargs["norm"] = self.rdf_init_kwargs.get("norm") or "density"
             self.rdf_run_kwargs["stop"] = self.rdf_run_kwargs.get("stop") or self.stop
             self.rdf_run_kwargs["step"] = self.rdf_run_kwargs.get("step") or self.step
-            self.rdf_run_kwargs["start"] = self.rdf_run_kwargs.get("start") or self.start
+            self.rdf_run_kwargs["start"] = (
+                self.rdf_run_kwargs.get("start") or self.start
+            )
             # generate and save RDFs
-            if self.solute_atoms.intersection(solvent).n_atoms == 0:
-                # the solute IS NOT in a solvent, the usual case
-                rdf = InterRDF(self.solute_atoms, solvent, **self.rdf_init_kwargs)
-                rdf.run(**self.rdf_run_kwargs)
-                bins, data = rdf.results.bins, rdf.results.rdf
-            else:
-                # the solute IS in a solvent
-                # we divide the solute and solvent into two groups, so that the rdfs
-                # are not contaminated by the solute-solvent pairs.
-                halfway_point = self.solute_atoms.n_residues // 2
-                solute_half = self.solute_atoms[halfway_point:]
-                solvent_half = (solvent.residues - solute_half.residues).atoms
-                # this is hacky and will make our rdf noisier but it was easy to implement
-                rdf = InterRDF(solute_half, solvent_half, **self.rdf_init_kwargs)
-                rdf.run(**self.rdf_run_kwargs)
-                bins, data = rdf.results.bins, rdf.results.rdf
+            rdf = InterRDF(
+                self.solute_atoms,
+                solvent,
+                **self.rdf_init_kwargs,
+                exclude_same="residue",
+            )
+            rdf.run(**self.rdf_run_kwargs)
+            bins, data = rdf.results.bins, rdf.results.rdf
             self.rdf_data[self.solute_name][name] = (bins, data)
             # generate and save plots
             if name not in self.radii.keys():
                 self.radii[name] = self.kernel(bins, data, **self.kernel_kwargs)
-        calculated_radii = set([name for name, radius in self.radii.items()
-                                if not np.isnan(radius)])
+        calculated_radii = set([name for name, radius in self.radii.items() if radius])
         missing_solvents = set(self.solvents.keys()) - calculated_radii
-        missing_solvents_str = ' '.join([str(i) for i in missing_solvents])
+        missing_solvents_str = " ".join([str(i) for i in missing_solvents])
         assert len(missing_solvents) == 0, (
             f"Solute could not identify a solvation radius for "
             f"{missing_solvents_str}. Please manually enter missing radii "
             f"by editing the radii dict and rerun the analysis."
         )
 
     def _single_frame(self):
@@ -539,15 +619,18 @@
             pairs, dist = capped_distance(
                 self.solute_atoms.positions,
                 solvent.positions,
                 self.radii[name],
                 box=self.u.dimensions,
             )
             # make sure pairs don't include intra-molecular interactions
-            filter = self.solute_atoms.resindices[pairs[:, 0]] == solvent.resindices[pairs[:, 1]]
+            filter = (
+                self.solute_atoms.resindices[pairs[:, 0]]
+                == solvent.resindices[pairs[:, 1]]
+            )
             pairs = pairs[~filter]
             dist = dist[~filter]
             # replace local ids with absolute ids
             pairs[:, 0] = self.solute_atoms.atoms.ix[tuple([pairs[:, 0]])]
             pairs[:, 1] = solvent.ix[tuple([pairs[:, 1]])]
             # extend
             pairs_list.append(pairs)
@@ -567,15 +650,15 @@
                 frame_number_array,
                 solute_res_ix_array,
                 pairs_array[:, 0],
                 pairs_array[:, 1],
                 dist_array,
                 solute_res_name_array,
                 solvent_res_name_array,
-                solvent_res_ix_array
+                solvent_res_ix_array,
             )
         )
         # add the current frame to the growing list of solvation arrays
         self._solvation_frames.append(solvation_data_np)
 
     def _conclude(self):
         """
@@ -589,143 +672,205 @@
                 FRAME,
                 SOLUTE_IX,
                 SOLUTE_ATOM_IX,
                 SOLVENT_ATOM_IX,
                 DISTANCE,
                 SOLUTE,
                 SOLVENT,
-                SOLVENT_IX
-            ]
+                SOLVENT_IX,
+            ],
         )
         # clean up solvation_data df
-        for column in [FRAME, SOLUTE_IX, SOLUTE_ATOM_IX, SOLVENT_ATOM_IX, DISTANCE, SOLVENT_IX]:
+        for column in [
+            FRAME,
+            SOLUTE_IX,
+            SOLUTE_ATOM_IX,
+            SOLVENT_ATOM_IX,
+            DISTANCE,
+            SOLVENT_IX,
+        ]:
             solvation_data_df[column] = pd.to_numeric(solvation_data_df[column])
-        solvation_data_df = solvation_data_df.sort_values([FRAME, SOLUTE_ATOM_IX, DISTANCE])
-        solvation_data_duplicates = solvation_data_df.duplicated(subset=[FRAME, SOLUTE_ATOM_IX, SOLVENT_IX])
+        solvation_data_df = solvation_data_df.sort_values(
+            [FRAME, SOLUTE_ATOM_IX, DISTANCE]
+        )
+        solvation_data_duplicates = solvation_data_df.duplicated(
+            subset=[FRAME, SOLUTE_ATOM_IX, SOLVENT_IX]
+        )
         solvation_data = solvation_data_df[~solvation_data_duplicates]
-        self.solvation_data = solvation_data.set_index([FRAME, SOLUTE_IX, SOLUTE_ATOM_IX, SOLVENT_ATOM_IX])
+        self.solvation_data = solvation_data.set_index(
+            [FRAME, SOLUTE_IX, SOLUTE_ATOM_IX, SOLVENT_ATOM_IX]
+        )
         duplicates = solvation_data_df[solvation_data_duplicates]
-        self.solvation_data_duplicates = duplicates.set_index([FRAME, SOLUTE_IX, SOLUTE_ATOM_IX, SOLVENT_ATOM_IX])
+        self.solvation_data_duplicates = duplicates.set_index(
+            [FRAME, SOLUTE_IX, SOLUTE_ATOM_IX, SOLVENT_ATOM_IX]
+        )
         # instantiate analysis classes
         self.has_run = True
         analysis_classes = {
-            'speciation': Speciation,
-            'pairing': Pairing,
-            'coordination': Coordination,
-            'residence': Residence,
-            'networking': Networking,
+            "speciation": Speciation,
+            "pairing": Pairing,
+            "coordination": Coordination,
+            "residence": Residence,
+            "networking": Networking,
         }
         for analysis_class in self.analysis_classes:
-            if analysis_class == 'networking':
-                setattr(self, 'networking', Networking.from_solute(self, self.networking_solvents))
+            if analysis_class == "networking":
+                setattr(
+                    self,
+                    "networking",
+                    Networking.from_solute(self, self.networking_solvents),
+                )
             else:
-                setattr(self, analysis_class, analysis_classes[analysis_class].from_solute(self))
+                setattr(
+                    self,
+                    analysis_class,
+                    analysis_classes[analysis_class].from_solute(self),
+                )
 
     @staticmethod
-    def _plot_solvation_radius(bins, data, radius):
+    def _plot_solvation_radius(
+        bins: np.ndarray, data: np.ndarray, radius: float
+    ) -> go.Figure:
         """
-        Plot a solvation radius on an RDF.
+        Plot a solvation radius on an RDF using Plotly.
 
         Includes a vertical line at the radius of interest.
 
         Parameters
         ----------
         bins : np.array
             the RDF bins
         data : np.array
             the RDF data
         radius : float
             the cutoff radius to draw on the plot
 
         Returns
         -------
-        fig : matplotlib.Figure
-        ax : matplotlib.Axes
+        fig : plotly.graph_objects.Figure
         """
-        fig, ax = plt.subplots()
-        ax.plot(bins, data, "b-", label="rdf")
-        ax.axvline(radius, color="r", label="solvation radius")
-        ax.set_xlabel("Radial Distance (A)")
-        ax.set_ylabel("Probability Density")
-        ax.legend()
-        return fig, ax
 
-    def plot_solvation_radius(self, solute_name, solvent_name):
+        fig = go.Figure()
+
+        # Add the RDF trace
+        fig.add_trace(go.Scatter(x=bins, y=data, mode="lines", name="RDF"))
+
+        # Add the vertical line for the solvation radius
+        fig.add_vline(
+            x=radius,
+            line_width=4,
+            line_dash="dash",
+            line_color="red",
+            annotation_text="Solvation Radius",
+            annotation_position="top right",
+        )
+
+        # Update the layout
+        fig.update_layout(
+            title="Solvation Radius on RDF",
+            xaxis_title="Radial Distance (Å)",
+            yaxis_title="Probability Density",
+            template="plotly_white",
+        )
+
+        return fig
+
+    def plot_solvation_radius(self, solute_name: str, solvent_name: str) -> go.Figure:
         """
         Plot the RDF of a solvent molecule
 
         Specified by the residue name in the solvents dict. Includes a vertical
         line at the radius of interest.
 
         Parameters
         ----------
         solvent_name : str
             the name of the residue of interest, as written in the solvents dict
 
         Returns
         -------
-        fig : matplotlib.Figure
-        ax : matplotlib.Axes
+        fig : go.Figure
         """
         if len(self.atom_solutes) == 1:
             solute_name = self.solute_name
         assert self.has_run, "Solute.run() must be called first."
+        assert not self.skip_rdf, "RDFs were skipped, so no RDFs are available."
         bins, data = self.rdf_data[solute_name][solvent_name]
         radius = self.atom_solutes[solute_name].radii[solvent_name]
-        fig, ax = self._plot_solvation_radius(bins, data, radius)
-        ax.set_title(f"{self.solute_name} solvation distance for {solvent_name}")
-        return fig, ax
+        fig = self._plot_solvation_radius(bins, data, radius)
+        fig.update_layout(
+            title=f"{self.solute_name} solvation radius for {solvent_name}"
+        )
+        return fig
 
-    def draw_molecule(self, residue, filename=None):
+    def draw_molecule(
+        self,
+        residue: Union[str, mda.core.groups.Residue],
+        filename: Optional[str] = None,
+    ) -> "rdkit.Chem.rdchem.Mol":
         """
         Returns
 
         Parameters
         ----------
         residue: the str name of the solute or any electrolytes or a MDAnalysis.Residue
         filename: If true, writes a file using the RDKit backend.
 
         Returns
         -------
         RDKit.Chem.rdchem.Mol
 
         """
-        from rdkit.Chem import Draw
-        from rdkit.Chem import rdCoordGen
-        from rdkit.Chem.Draw.MolDrawing import DrawingOptions
+        if rdkit is None:
+            raise ImportError(
+                "The RDKit package is required to use this function. "
+                "Please install RDKit with `conda install -c conda-forge rdkit`."
+            )
+
         DrawingOptions.atomLabelFontSize = 100
 
         if isinstance(residue, str):
             if residue in [self.solute_name, "solute"]:
                 mol = self.solute_atoms.residues[0].atoms.convert_to("RDKIT")
                 mol_mda_ix = self.solute_atoms.residues[0].atoms.ix
-                solute_atoms_ix0 = {solute.solute_atoms.atoms.ix[0]: solute_name
-                                    for solute_name, solute in self.atom_solutes.items()}
+                solute_atoms_ix0 = {
+                    solute.solute_atoms.atoms.ix[0]: solute_name
+                    for solute_name, solute in self.atom_solutes.items()
+                }
                 for i, atom in enumerate(mol.GetAtoms()):
                     atom_name = solute_atoms_ix0.get(mol_mda_ix[i])
                     label = f"{i}, " + atom_name if atom_name else str(i)
                     atom.SetProp("atomNote", label)
             elif residue in self.solvents.keys():
                 mol = self.solvents[residue].residues[0].atoms.convert_to("RDKIT")
                 for i, atom in enumerate(mol.GetAtoms()):
                     atom.SetProp("atomNote", str(i))
             else:
-                raise ValueError("If the residue is a string, it must be the name of a solute, "
-                             "the name of a solvent, or 'solute'.")
+                raise ValueError(
+                    "If the residue is a string, it must be the name of a solute, "
+                    "the name of a solvent, or 'solute'."
+                )
         else:
             assert isinstance(residue, mda.core.groups.Residue)
             mol = residue.atoms.convert_to("RDKIT")
             for i, atom in enumerate(mol.GetAtoms()):
                 atom.SetProp("atomNote", str(i))
         if filename:
             Draw.MolToFile(mol, filename=filename)
         rdCoordGen.AddCoords(mol)
         return mol
 
-    def get_shell(self, solute_index, frame, as_df=False, remove_mols=None, closest_n_only=None):
+    def get_shell(
+        self,
+        solute_index: int,
+        frame: int,
+        as_df: bool = False,
+        remove_mols: Optional[dict[str, int]] = None,
+        closest_n_only: Optional[int] = None,
+    ) -> Union[mda.AtomGroup, pd.DataFrame]:
         """
         Select the solvation shell of the solute.
 
         The solvation shell can be returned either as an
         AtomGroup, to be visualized or passed to other routines,
         or as a pandas.DataFrame for convenient inspection.
 
@@ -754,53 +899,58 @@
 
         Returns
         -------
         MDAnalysis.AtomGroup or pandas.DataFrame
 
         """
         assert self.has_run, "Solute.run() must be called first."
-        assert frame in self.frames, ("The requested frame must be one "
-                                      "of an analyzed frames in self.frames.")
+        assert (
+            frame in self.frames
+        ), "The requested frame must be one of the analyzed frames in self.frames."
         remove_mols = {} if remove_mols is None else remove_mols
         # select shell of interest
         shell = self.solvation_data.xs((frame, solute_index), level=(FRAME, SOLUTE_IX))
         # remove mols
         for mol_name, n_remove in remove_mols.items():
             # first, filter for only mols of type mol_name
             is_mol = shell[SOLVENT] == mol_name
             res_ix = shell[is_mol][SOLVENT_IX]
             mol_count = len(res_ix)
             n_remove = min(mol_count, n_remove)
             # then truncate resnames to remove mols
-            remove_ix = res_ix[(mol_count - n_remove):]
+            remove_ix = res_ix[(mol_count - n_remove) :]
             # then apply to original shell
             remove = shell[SOLVENT_IX].isin(remove_ix)
             shell = shell[np.invert(remove)]
         # filter based on length
         if closest_n_only:
             assert closest_n_only > 0, "closest_n_only must be at least 1"
             closest_n_only = min(len(shell), closest_n_only)
-            shell = shell[0: closest_n_only]
+            shell = shell[0:closest_n_only]
         if as_df:
             return shell
         else:
             return self._df_to_atom_group(shell, solute_index=solute_index)
 
     def get_closest_n_mol(
-            self,
-            solute_atom_ix,
-            n_mol,
-            guess_radius=3,
-            return_ordered_resix=False,
-            return_radii=False,
-    ):
+        self,
+        solute_atom_ix: int,
+        n_mol: int,
+        guess_radius: Union[float, int] = 3,
+        return_ordered_resix: bool = False,
+        return_radii: bool = False,
+    ) -> Union[
+        mda.AtomGroup,
+        tuple[mda.AtomGroup, np.ndarray],
+        tuple[mda.AtomGroup, np.ndarray, np.ndarray],
+    ]:
         """
         Select the n closest mols to the solute.
 
-        The solute is specified by it's index within solvation_data.
+        The solute is specified by its index within solvation_data.
         n is specified with the n_mol argument. Optionally returns
         an array of their resids and an array of the distance of
         the closest atom in each molecule.
 
         Parameters
         ----------
         solute_atom_ix : int
@@ -829,15 +979,17 @@
             self.u.atoms[solute_atom_ix],
             n_mol,
             guess_radius,
             return_ordered_resix,
             return_radii,
         )
 
-    def radial_shell(self, solute_atom_ix, radius):
+    def radial_shell(
+        self, solute_atom_ix: int, radius: Union[float, int]
+    ) -> mda.AtomGroup:
         """
         Select all residues with atoms within r of the solute.
 
         The solute is specified by it's index within solvation_data. r is
         specified with the radius argument. Thin wrapper around
         solvation.get_radial_shell.
 
@@ -850,15 +1002,17 @@
 
         Returns
         -------
         MDAnalysis.AtomGroup
         """
         return get_radial_shell(self.solute_atoms[solute_atom_ix], radius)
 
-    def _df_to_atom_group(self, df, solute_index=None):
+    def _df_to_atom_group(
+        self, df: pd.DataFrame, solute_index: Optional[int] = None
+    ) -> mda.AtomGroup:
         """
         Selects an MDAnalysis.AtomGroup from a pandas.DataFrame with solvent.
 
         Parameters
         ----------
         df : pandas.DataFrame
             a df with a "solvent" column
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/speciation.py` & `solvation_analysis-0.4.0/solvation_analysis/speciation.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,22 @@
 While ``speciation`` can be used in isolation, it is meant to be used
 as an attribute of the Solute class. This makes instantiating it and calculating the
 solvation data a non-issue.
 """
 
 import pandas as pd
 
-from solvation_analysis._column_names import *
+import solvation_analysis
+from solvation_analysis._column_names import (
+    FRAME,
+    SOLUTE_IX,
+    SOLVENT,
+    SOLVENT_IX,
+    COUNT,
+)
 
 
 class Speciation:
     """
     Calculate the solvation shells of every solute.
 
     Speciation organizes the solvation data by the type of residue
@@ -40,30 +47,32 @@
 
     Additionally, there are methods for finding solvation shells of
     interest and computing how common certain shell configurations are.
 
     Parameters
     ----------
     solvation_data : pandas.DataFrame
-        The solvation data frame output by Solute.
+        The solvation dataframe output by Solute.
     n_frames : int
         The number of frames in solvation_data.
     n_solutes : int
         The number of solutes in solvation_data.
     """
 
-    def __init__(self, solvation_data, n_frames, n_solutes):
+    def __init__(
+        self, solvation_data: pd.DataFrame, n_frames: int, n_solutes: int
+    ) -> None:
         self.solvation_data = solvation_data
         self.n_frames = n_frames
         self.n_solutes = n_solutes
         self._speciation_df, self._speciation_fraction = self._compute_speciation()
         self._solvent_co_occurrence = self._solvent_co_occurrence()
 
     @staticmethod
-    def from_solute(solute):
+    def from_solute(solute: "solvation_analysis.Solute") -> "Speciation":
         """
         Generate a Speciation object from a solute.
 
         Parameters
         ----------
         solute : Solute
 
@@ -74,32 +83,38 @@
         assert solute.has_run, "The solute must be run before calling from_solute"
         return Speciation(
             solute.solvation_data,
             solute.n_frames,
             solute.n_solutes,
         )
 
-    def _compute_speciation(self):
-        counts = self.solvation_data.groupby([FRAME, SOLUTE_IX, SOLVENT]).count()[SOLVENT_IX]
+    def _compute_speciation(self) -> tuple[pd.DataFrame, pd.DataFrame]:
+        counts = self.solvation_data.groupby([FRAME, SOLUTE_IX, SOLVENT]).count()[
+            SOLVENT_IX
+        ]
         counts_re = counts.reset_index([SOLVENT])
         speciation_data = counts_re.pivot(columns=[SOLVENT]).fillna(0).astype(int)
         res_names = speciation_data.columns.levels[1]
         speciation_data.columns = res_names
         sum_series = speciation_data.groupby(speciation_data.columns.to_list()).size()
         sum_sorted = sum_series.sort_values(ascending=False)
         speciation_fraction = sum_sorted.reset_index().rename(columns={0: COUNT})
-        speciation_fraction[COUNT] = speciation_fraction[COUNT] / (self.n_frames * self.n_solutes)
+        speciation_fraction[COUNT] = speciation_fraction[COUNT] / (
+            self.n_frames * self.n_solutes
+        )
         return speciation_data, speciation_fraction
 
     @classmethod
-    def _mean_speciation(cls, speciation_frames, solute_number, frame_number):
+    def _mean_speciation(
+        cls, speciation_frames: pd.DataFrame, solute_number: int, frame_number: int
+    ) -> pd.Series:
         means = speciation_frames.sum(axis=1) / (solute_number * frame_number)
         return means
 
-    def calculate_shell_fraction(self, shell_dict):
+    def calculate_shell_fraction(self, shell_dict: dict[str, int]) -> float:
         """
         Calculate the fraction of shells matching shell_dict.
 
         This function computes the fraction of solvation shells that exist with a particular
         composition. The composition is specified by the shell_dict. The fraction
         will be of all shells that match that specification.
 
@@ -130,15 +145,15 @@
             0.0898
         """
         query_list = [f"{name} == {str(count)}" for name, count in shell_dict.items()]
         query = " and ".join(query_list)
         query_counts = self.speciation_fraction.query(query)
         return query_counts[COUNT].sum()
 
-    def get_shells(self, shell_dict):
+    def get_shells(self, shell_dict: dict[str, int]) -> pd.DataFrame:
         """
         Find all solvation shells that match shell_dict.
 
         This returns the frame, solute index, and composition of all solutes
         that match the composition given in shell_dict.
 
         Attributes
@@ -157,25 +172,27 @@
             the index and composition of all shells that match shell_dict
         """
         query_list = [f"{name} == {str(count)}" for name, count in shell_dict.items()]
         query = " and ".join(query_list)
         query_counts = self.speciation_data.query(query)
         return query_counts
 
-    def _solvent_co_occurrence(self):
+    def _solvent_co_occurrence(self) -> pd.DataFrame:
         # calculate the co-occurrence of solvent molecules.
         expected_solvents_list = []
         actual_solvents_list = []
         for solvent in self.speciation_data.columns.values:
             # calculate number of available coordinating solvent slots
-            shells_w_solvent = self.speciation_data.query(f'`{solvent}` > 0')
+            shells_w_solvent = self.speciation_data.query(f"`{solvent}` > 0")
             n_solvents = shells_w_solvent.sum()
             # calculate expected number of coordinating solvents
             n_coordination_slots = n_solvents.sum() - len(shells_w_solvent)
-            coordination_fraction = self.speciation_data.sum() / self.speciation_data.sum().sum()
+            coordination_fraction = (
+                self.speciation_data.sum() / self.speciation_data.sum().sum()
+            )
             expected_solvents = coordination_fraction * n_coordination_slots
             # calculate actual number of coordinating solvents
             actual_solvents = n_solvents.copy()
             actual_solvents[solvent] = actual_solvents[solvent] - len(shells_w_solvent)
             # name series and append to list
             expected_solvents.name = solvent
             actual_solvents.name = solvent
@@ -188,35 +205,35 @@
         actual_df = pd.concat(actual_solvents_list, axis=1)
         expected_df = pd.concat(expected_solvents_list, axis=1)
         # calculate correlation matrix
         correlation = actual_df / expected_df
         return correlation
 
     @property
-    def speciation_data(self):
+    def speciation_data(self) -> pd.DataFrame:
         """
         A dataframe containing the speciation of every solute at
-        every trajectory frame. Indexed by frame and solute numbers.
+        every trajectory frame. Indexed by timestep and solute numbers.
         Columns are the solvent molecules and values are the number
         of solvent in the shell.
         """
         return self._speciation_df
 
     @property
-    def speciation_fraction(self):
+    def speciation_fraction(self) -> pd.DataFrame:
         """
         The fraction of shells of each type. Columns are the solvent
         molecules and values are the number of solvent in the shell.
         The final column is the fraction of total shell of that
         particular composition.
         """
         return self._speciation_fraction
 
     @property
-    def solvent_co_occurrence(self):
+    def solvent_co_occurrence(self) -> pd.DataFrame:
         """
         The actual co-occurrence of solvents divided by the expected co-occurrence.
         In other words, given one molecule of solvent i in the shell, what is the
         probability of finding a solvent j relative to choosing a solvent at random
         from the pool of all coordinated solvents. This matrix will
         likely not be symmetric.
         """
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/conftest.py` & `solvation_analysis-0.4.0/solvation_analysis/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from solvation_analysis.networking import Networking
 from solvation_analysis.residence import Residence
 
 from solvation_analysis.rdf_parser import identify_cutoff_poly
 from solvation_analysis.tests.datafiles import (
     bn_fec_data,
     bn_fec_dcd_wrap,
-    bn_fec_dcd_unwrap,
     bn_fec_atom_types,
     eax_data,
     iba_data,
     iba_dcd,
 )
 from solvation_analysis.tests.datafiles import (
     easy_rdf_bins,
@@ -46,15 +45,15 @@
     residue_size - size of mda residues
     n_frames - number of frames
 
     Returns
     -------
     A constructed MDanalysis.Universe
     """
-    n_particles = n_grid ** 3
+    n_particles = n_grid**3
     assert (
         n_particles % residue_size == 0
     ), "residue_size must be a factor of n_particles"
     n_residues = n_particles // residue_size
     atom_residues = np.array(range(0, n_particles)) // residue_size
 
     grid = np.mgrid[0:n_grid, 0:n_grid, 0:n_grid]  # make the grid
@@ -80,51 +79,47 @@
 
 @pytest.fixture
 def u_grid_1():
     """Creates a 6x6x6 grid with residues containing 1 atom"""
     return make_grid_universe(6, 1)
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def u_real():
     """Returns a universe of a BN FEC trajectory"""
     return mda.Universe(bn_fec_data, bn_fec_dcd_wrap)
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def u_real_named(u_real):
     """Returns a universe of a BN FEC trajectory with residues and atoms named"""
     types = np.loadtxt(bn_fec_atom_types, dtype=str)
     u_real.add_TopologyAttr("name", values=types)
     resnames = ["BN"] * 363 + ["FEC"] * 237 + ["PF6"] * 49 + ["Li"] * 49
     u_real.add_TopologyAttr("resnames", values=resnames)
     return u_real
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def atom_groups(u_real):
     """Returns pre-selected atom groups in the BN FEC universe"""
     li_atoms = u_real.atoms.select_atoms("type 22")
     pf6_atoms = u_real.atoms.select_atoms("byres type 20")
     bn_atoms = u_real.atoms.select_atoms("byres type 5")
     fec_atoms = u_real.atoms.select_atoms("byres type 19")
     atom_groups = {"li": li_atoms, "pf6": pf6_atoms, "bn": bn_atoms, "fec": fec_atoms}
     return atom_groups
 
 
 def rdf_loading_helper(bins_files, data_files):
     """
     Creates dictionary of bin and data arrays with a rdf tag as key
     """
-    rdf_bins = {
-        key: list(np.load(npz).values())[0] for key, npz in bins_files.items()
-    }
-    rdf_data = {
-        key: list(np.load(npz).values())[0] for key, npz in data_files.items()
-    }
+    rdf_bins = {key: list(np.load(npz).values())[0] for key, npz in bins_files.items()}
+    rdf_data = {key: list(np.load(npz).values())[0] for key, npz in data_files.items()}
     shared_keys = set(rdf_data.keys()) & set(rdf_bins.keys())
     rdf_bins_and_data = {key: (rdf_bins[key], rdf_data[key]) for key in shared_keys}
     return rdf_bins_and_data
 
 
 @pytest.fixture
 def rdf_bins_and_data_easy():
@@ -137,164 +132,174 @@
 
 
 @pytest.fixture
 def rdf_bins_and_data_non_solv():
     return rdf_loading_helper(non_solv_rdf_bins, non_solv_rdf_data)
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def pre_solute(atom_groups):
-    li = atom_groups['li']
-    pf6 = atom_groups['pf6']
-    bn = atom_groups['bn']
-    fec = atom_groups['fec']
+    li = atom_groups["li"]
+    pf6 = atom_groups["pf6"]
+    bn = atom_groups["bn"]
+    fec = atom_groups["fec"]
     return Solute.from_atoms(
         li,
-        {'pf6': pf6, 'bn': bn, 'fec': fec},
-        radii={'pf6': 2.8, 'bn': 2.61468, 'fec': 2.43158},
+        {"pf6": pf6, "bn": bn, "fec": fec},
+        radii={"pf6": 2.8, "bn": 2.61468, "fec": 2.43158},
         rdf_init_kwargs={"range": (0, 8.0)},
     )
 
 
-@pytest.fixture(scope='function')
+@pytest.fixture(scope="function")
 def pre_solute_mutable(atom_groups):
-    li = atom_groups['li']
-    pf6 = atom_groups['pf6']
-    bn = atom_groups['bn']
-    fec = atom_groups['fec']
+    li = atom_groups["li"]
+    pf6 = atom_groups["pf6"]
+    bn = atom_groups["bn"]
+    fec = atom_groups["fec"]
     return Solute.from_atoms(
         li,
-        {'pf6': pf6, 'bn': bn, 'fec': fec},
-        radii={'pf6': 2.8, 'bn': 2.61468, 'fec': 2.43158},
+        {"pf6": pf6, "bn": bn, "fec": fec},
+        radii={"pf6": 2.8, "bn": 2.61468, "fec": 2.43158},
         rdf_init_kwargs={"range": (0, 8.0)},
         rdf_kernel=identify_cutoff_poly,
     )
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def run_solute(pre_solute):
     pre_solute.run(step=1)
     return pre_solute
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def u_eax_series():
     boxes = {
-        'ea': [45.760393, 45.760393, 45.760393, 90, 90, 90],
-        'eaf': [47.844380, 47.844380, 47.844380, 90, 90, 90],
-        'fea': [48.358954, 48.358954, 48.358954, 90, 90, 90],
-        'feaf': [50.023129, 50.023129, 50.023129, 90, 90, 90],
+        "ea": [45.760393, 45.760393, 45.760393, 90, 90, 90],
+        "eaf": [47.844380, 47.844380, 47.844380, 90, 90, 90],
+        "fea": [48.358954, 48.358954, 48.358954, 90, 90, 90],
+        "feaf": [50.023129, 50.023129, 50.023129, 90, 90, 90],
     }
     us = {}
     for solvent_dir in pathlib.Path(eax_data).iterdir():
         u_solv = mda.Universe(
-            str(solvent_dir / 'topology.pdb'),
-            str(solvent_dir / 'trajectory_equil.dcd')
+            str(solvent_dir / "topology.pdb"), str(solvent_dir / "trajectory_equil.dcd")
         )
         # our dcd lacks dimensions so we must manually set them
         box = boxes[solvent_dir.stem]
         set_dim = transformations.boxdimensions.set_dimensions(box)
         u_solv.trajectory.add_transformations(set_dim)
         us[solvent_dir.stem] = u_solv
     return us
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def u_eax_atom_groups(u_eax_series):
     atom_groups_dict = {}
     for name, u in u_eax_series.items():
         atom_groups = {}
-        atom_groups['li'] = u.atoms.select_atoms("element Li")
-        atom_groups['pf6'] = u.atoms.select_atoms("byres element P")
+        atom_groups["li"] = u.atoms.select_atoms("element Li")
+        atom_groups["pf6"] = u.atoms.select_atoms("byres element P")
         residue_lengths = np.array([len(elements) for elements in u.residues.elements])
         eax_fec_cutoff = np.unique(residue_lengths, return_index=True)[1][2]
         atom_groups[name] = u.atoms.select_atoms(f"resid 1:{eax_fec_cutoff}")
-        atom_groups['fec'] = u.atoms.select_atoms(f"resid {eax_fec_cutoff + 1}:600")
+        atom_groups["fec"] = u.atoms.select_atoms(f"resid {eax_fec_cutoff + 1}:600")
         atom_groups_dict[name] = atom_groups
     return atom_groups_dict
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def eax_solutes(u_eax_atom_groups):
     solutes = {}
     for name, atom_groups in u_eax_atom_groups.items():
         solute = Solute.from_atoms(
-            atom_groups['li'],
-            {'pf6': atom_groups['pf6'], name: atom_groups[name], 'fec': atom_groups['fec']},
+            atom_groups["li"],
+            {
+                "pf6": atom_groups["pf6"],
+                name: atom_groups[name],
+                "fec": atom_groups["fec"],
+            },
+            analysis_classes=["pairing", "coordination", "speciation", "networking"],
+            networking_solvents=["pf6"],
         )
         solute.run()
         solutes[name] = solute
     return solutes
 
-@pytest.fixture(scope='module')
+
+@pytest.fixture(scope="module")
 def iba_u():
     return mda.Universe(iba_data, iba_dcd)
 
-@pytest.fixture(scope='module')
+
+@pytest.fixture(scope="module")
 def iba_solvents(iba_u):
     iba = iba_u.select_atoms("byres element C")
     H2O = iba_u.atoms - iba
-    return {'iba': iba, 'H2O': H2O}
+    return {"iba": iba, "H2O": H2O}
+
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def iba_atom_groups(iba_solvents):
-    iba = iba_solvents['iba']
+    iba = iba_solvents["iba"]
     return {
-        'iba_alcohol_O': iba[5::12],
-        'iba_alcohol_H': iba[11::12],
-        'iba_ketone': iba[4::12],
-        'iba_C0': iba[0::12],
-        'iba_C1': iba[1::12],
-        'iba_C2': iba[2::12],
-        'iba_C3': iba[3::12],
-        'iba_H6': iba[6::12],
-        'iba_H7': iba[7::12],
-        'iba_H8': iba[8::12],
-        'iba_H9': iba[9::12],
-        'iba_H10': iba[10::12],
+        "iba_alcohol_O": iba[5::12],
+        "iba_alcohol_H": iba[11::12],
+        "iba_ketone": iba[4::12],
+        "iba_C0": iba[0::12],
+        "iba_C1": iba[1::12],
+        "iba_C2": iba[2::12],
+        "iba_C3": iba[3::12],
+        "iba_H6": iba[6::12],
+        "iba_H7": iba[7::12],
+        "iba_H8": iba[8::12],
+        "iba_H9": iba[9::12],
+        "iba_H10": iba[10::12],
     }
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def H2O_atom_groups(iba_solvents):
-    H2O = iba_solvents['H2O']
+    H2O = iba_solvents["H2O"]
     return {
-        'H2O_O': H2O[0::3],
-        'H2O_H1': H2O[1::3],
-        'H2O_H2': H2O[2::3],
+        "H2O_O": H2O[0::3],
+        "H2O_H1": H2O[1::3],
+        "H2O_H2": H2O[2::3],
     }
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def iba_solutes(iba_atom_groups, iba_solvents):
     solutes = {}
     for name, atom_group in iba_atom_groups.items():
-        radii = {'iba': 1.9, 'H2O': 1.9} if ('iba_H' in name or 'iba_C' in name) else None
+        radii = (
+            {"iba": 1.9, "H2O": 1.9} if ("iba_H" in name or "iba_C" in name) else None
+        )
         solute = Solute.from_atoms(
             atom_group,
             iba_solvents,
             solute_name=name,
             radii=radii,
         )
         solute.run()
         solutes[name] = solute
     return solutes
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def iba_small_solute(iba_atom_groups, iba_solvents):
     solute_atoms = {
-        'iba_ketone': iba_atom_groups['iba_ketone'],
-        'iba_alcohol_O': iba_atom_groups['iba_alcohol_O'],
-        'iba_alcohol_H': iba_atom_groups['iba_alcohol_H']
+        "iba_ketone": iba_atom_groups["iba_ketone"],
+        "iba_alcohol_O": iba_atom_groups["iba_alcohol_O"],
+        "iba_alcohol_H": iba_atom_groups["iba_alcohol_H"],
     }
     solute = Solute.from_atoms_dict(
         solute_atoms,
         iba_solvents,
-        solute_name='iba',
+        solute_name="iba",
     )
     solute.run()
     return solute
 
 
 @pytest.fixture
 def solvation_results(run_solute):
@@ -302,26 +307,26 @@
 
 
 @pytest.fixture
 def solvation_data(run_solute):
     return run_solute.solvation_data
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def solvation_data_large():
     return pd.read_csv(bn_fec_solv_df_large, index_col=[0, 1, 2, 3])
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def solvation_data_sparse(solvation_data_large):
     step = 10
     return solvation_data_large.loc[pd.IndexSlice[::step, :, :], :]
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def residence(solvation_data_sparse):
     return Residence(solvation_data_sparse, step=10)
 
 
-@pytest.fixture(scope='module')
+@pytest.fixture(scope="module")
 def networking(run_solute):
-    return Networking.from_solute(run_solute, 'pf6')
+    return Networking.from_solute(run_solute, "pf6")
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/.DS_Store` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/README.md` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/README.md`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/bn_fec_data/bn_fec.data` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/bn_fec_data/bn_fec.data`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_unwrap.dcd` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_unwrap.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_wrap.dcd` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/bn_fec_data/bn_fec_short_wrap.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/bn_fec_data/bn_solv_df_large.csv` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/bn_fec_data/bn_solv_df_large.csv`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/ea_fec_data/ea_fec.dcd` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/ea_fec_data/ea_fec.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/ea_fec_data/ea_fec.pdb` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/ea_fec_data/ea_fec.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/ea/topology.pdb` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/ea/topology.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/ea/trajectory_equil.dcd` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/ea/trajectory_equil.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/eaf/topology.pdb` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/eaf/topology.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/eaf/trajectory_equil.dcd` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/eaf/trajectory_equil.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/fea/topology.pdb` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/fea/topology.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/fea/trajectory_equil.dcd` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/fea/trajectory_equil.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/feaf/topology.pdb` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/feaf/topology.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/eax_data/feaf/trajectory_equil.dcd` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/eax_data/feaf/trajectory_equil.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/iba_data/isobutyric_acid.dcd` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/iba_data/isobutyric_acid.dcd`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/iba_data/isobutyric_acid.pdb` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/iba_data/isobutyric_acid.pdb`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_O_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_fec_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_bn_N_vs_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_F_vs_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_fec_O_vs_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_O_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_non_solvated/rdf_pf6_F_vs_fec_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_O_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_fec_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_easy/rdf_universe_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_N_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_bn_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_O_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_fec_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_F_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_pf6_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_bins.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_bins.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_data.npz` & `solvation_analysis-0.4.0/solvation_analysis/tests/data/rdf_vs_li_hard/rdf_universe_all_data.npz`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/datafiles.py` & `solvation_analysis-0.4.0/solvation_analysis/tests/datafiles.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/test_coordination.py` & `solvation_analysis-0.4.0/solvation_analysis/tests/test_coordination.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/test_networking.py` & `solvation_analysis-0.4.0/solvation_analysis/tests/test_networking.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/test_pairing.py` & `solvation_analysis-0.4.0/solvation_analysis/tests/test_pairing.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/test_plotting.py` & `solvation_analysis-0.4.0/solvation_analysis/tests/test_plotting.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,67 @@
 import pytest
 from solvation_analysis.plotting import (
     plot_network_size_histogram,
     plot_shell_composition_by_size,
     plot_co_occurrence,
+    plot_speciation,
+    plot_rdfs,
     _compare_function_generator,
     compare_free_solvents,
     compare_pairing,
     compare_coordination_numbers,
     compare_residence_times_cutoff,
     compare_residence_times_fit,
     compare_diluent,
+    compare_networking,
 )
 
 from solvation_analysis.networking import Networking
 from solvation_analysis.residence import Residence
 from solvation_analysis.speciation import Speciation
 
 
 def test_plot_network_size_histogram(run_solute):
-    run_solute.networking = Networking.from_solute(run_solute, 'pf6')
+    run_solute.networking = Networking.from_solute(run_solute, "pf6")
     plot_network_size_histogram(run_solute)
     plot_network_size_histogram(run_solute.networking)
     assert True
 
 
 def test_plot_shell_size_histogram(run_solute):
     plot_shell_composition_by_size(run_solute)
     plot_shell_composition_by_size(run_solute.speciation)
     assert True
 
 
+def test_plot_speciation(run_solute):
+    plot_speciation(run_solute)
+    plot_speciation(run_solute.speciation)
+    assert True
+
+
+def test_plot_rdfs(run_solute, iba_small_solute):
+    plot_rdfs(iba_small_solute)
+    plot_rdfs(iba_small_solute, merge_on_x=True)
+    plot_rdfs(iba_small_solute, merge_on_y=True)
+    plot_rdfs(iba_small_solute, merge_on_x=True, merge_on_y=True)
+    plot_rdfs(iba_small_solute, x_axis_solute=True)
+    plot_rdfs(iba_small_solute, x_axis_solute=True, merge_on_y=True)
+    plot_rdfs(iba_small_solute, x_axis_solute=True, merge_on_x=True)
+    plot_rdfs(iba_small_solute, x_axis_solute=True, merge_on_x=True, merge_on_y=True)
+    plot_rdfs(run_solute)
+
+
 # compare_solvent_dicts tests
 def test_compare_solvent_dicts_rename_exception(eax_solutes):
     # invalid solvents_to_plot because solvent names were already renamed to the generic "EAx" form
     # solvents_to_plot here references the former names of solvents, which is wrong
     # this test should handle an exception
     with pytest.raises(Exception):
-        fig = compare_pairing(
+        compare_pairing(
             eax_solutes,
             rename_solvent_dict={
                 "ea": "EAx",
                 "fea": "EAx",
                 "eaf": "EAx",
                 "feaf": "EAx",
             },
@@ -51,133 +72,124 @@
         )
 
 
 def test_compare_solvent_dicts_sensitivity(eax_solutes):
     # solvent names are case-sensitive, so names in solvents_to_plot and rename_solvent_dict should be consistent
     # this test should handle an exception
     with pytest.raises(Exception):
-        fig = compare_pairing(
+        compare_pairing(
             eax_solutes,
             rename_solvent_dict={
                 "EA": "EAx",
                 "fEA": "EAx",
                 "EAf": "EAx",
                 "fEAf": "EAx",
             },
             solvents_to_plot=["PF6", "FEC", "EAx"],
             x_label="Species",
             y_label="Pairing",
             title="Graph",
         )
 
 
+def test_compare_networking(eax_solutes):
+    compare_networking(eax_solutes)
+
+
 # compare_pairing tests
 def test_compare_pairing_default_eax(eax_solutes):
     # call compare_pairing with only one required argument
     # also tests how the code handles eax systems
     fig = compare_pairing(eax_solutes)
-    assert len(fig.data) == 4
-    # fig.show()
+    assert len(fig.data) == 6
 
 
 def test_compare_pairing_case1(eax_solutes):
     # solvents_to_plot on x axis, each bar is a solute
     fig = compare_pairing(
         eax_solutes,
         solvents_to_plot=["fec", "pf6"],
         x_label="Species",
         y_label="Pairing",
         title="Bar Graph of Solvent Pairing",
     )
-    assert len(fig.data) == 4
-    for bar in fig.data:
-        assert set(bar.x) == {"fec", "pf6"}
-    # fig.show()
+    assert len(fig.data) == 2
 
 
 def test_compare_pairing_case2(eax_solutes):
     # solutes on x axis, each bar is an element of solvents_to_plot
     fig = compare_pairing(
         eax_solutes,
         solvents_to_plot=["pf6", "fec"],
         x_label="Solute",
         y_label="Pairing",
         title="Bar Graph of Solvent Pairing",
-        x_axis="solute",
+        x_axis_solute=True,
     )
     assert len(fig.data) == 2
     for bar in fig.data:
         assert set(bar.x) == {"feaf", "eaf", "fea", "ea"}
-    # fig.show()
 
 
 def test_compare_pairing_case3(eax_solutes):
     # solvents_to_plot on x axis, each line is a solute
     fig = compare_pairing(
         eax_solutes,
         solvents_to_plot=["pf6", "fec"],
         x_label="Solute",
         y_label="Pairing",
         title="Line Graph of Solvent Pairing",
         series=True,
     )
-    assert len(fig.data) == 4
-    for line in fig.data:
-        assert set(line.x) == {"fec", "pf6"}
-    # fig.show()
+    assert len(fig.data) == 2
 
 
 def test_compare_pairing_case4(eax_solutes):
     # solutes on x axis, each line is an element of solvents_to_plot
     fig = compare_pairing(
         eax_solutes,
         solvents_to_plot=["pf6", "fec"],
         x_label="Solute",
         y_label="Pairing",
         title="Line Graph of Solvent Pairing",
-        x_axis="solute",
+        x_axis_solute=True,
         series=True,
     )
     assert len(fig.data) == 2
     for line in fig.data:
         assert set(line.x) == {"feaf", "eaf", "fea", "ea"}
-    # fig.show()
 
 
 def test_compare_pairing_switch_solvents_to_plot_order(eax_solutes):
     # same test as test_compare_pairing_case4, except order for solvents_to_plot is switched
     fig = compare_pairing(
         eax_solutes,
         solvents_to_plot=["fec", "pf6"],
         x_label="Solute",
         y_label="Pairing",
         title="Line Graph of Solvent Pairing",
-        x_axis="solute",
+        x_axis_solute=True,
         series=True,
     )
     assert len(fig.data) == 2
     for line in fig.data:
         assert set(line.x) == {"feaf", "eaf", "fea", "ea"}
-    # fig.show()
 
 
 def test_compare_pairing_rename_solvent_dict(eax_solutes):
     # rename solvent names into the generic "EAx" form
     fig = compare_pairing(
         eax_solutes,
         rename_solvent_dict={"ea": "EAx", "fea": "EAx", "eaf": "EAx", "feaf": "EAx"},
         solvents_to_plot=["pf6", "fec", "EAx"],
         x_label="Species",
         y_label="Pairing",
         title="Bar Graph of Solvent Pairing",
     )
-    assert len(fig.data) == 4
-    for bar in fig.data:
-        assert set(bar.x) == {"pf6", "fec", "EAx"}
-    # fig.show()
+    assert len(fig.data) == 3
 
 
 def test_compare_free_solvents(eax_solutes):
     compare_free_solvents(eax_solutes, solvents_to_plot=["fec", "pf6"])
 
 
 def test_compare_diluent(eax_solutes):
@@ -185,109 +197,107 @@
 
 
 # compare_coordination_numbers tests
 def test_compare_coordination_numbers_default_eax(eax_solutes):
     # call compare_coordination_numbers with only one required argument
     # also tests how the code handles eax systems
     fig = compare_coordination_numbers(eax_solutes)
-    assert len(fig.data) == 4
-    # fig.show()
+    assert len(fig.data) == 6
 
 
 def test_compare_coordination_numbers_solute_four_cases(eax_solutes):
-    fig = compare_coordination_numbers(eax_solutes, x_axis='solute')
+    fig = compare_coordination_numbers(eax_solutes, x_axis_solute=True)
     assert len(fig.data) == 6
 
-    fig = compare_coordination_numbers(eax_solutes, x_axis='solute', series=True)
+    fig = compare_coordination_numbers(eax_solutes, x_axis_solute=True, series=True)
     assert len(fig.data) == 6
 
     rename = {
         "ea": "EAx",
         "fea": "EAx",
         "eaf": "EAx",
         "feaf": "EAx",
     }
-    fig = compare_coordination_numbers(eax_solutes, x_axis='solute', rename_solvent_dict=rename)
+    fig = compare_coordination_numbers(
+        eax_solutes, x_axis_solute=True, rename_solvent_dict=rename
+    )
     assert len(fig.data) == 3
 
-    fig = compare_coordination_numbers(eax_solutes, x_axis='solute', series=True, rename_solvent_dict=rename)
+    fig = compare_coordination_numbers(
+        eax_solutes,
+        x_axis_solute=True,
+        series=True,
+        rename_solvent_dict=rename,
+    )
     assert len(fig.data) == 3
 
     fig = compare_coordination_numbers(
         eax_solutes,
-        x_axis='solute',
+        x_axis_solute=True,
         rename_solvent_dict=rename,
         series=True,
-        solvents_to_plot=['EAx', 'pf6'],
+        solvents_to_plot=["EAx", "pf6"],
     )
     assert len(fig.data) == 2
 
 
 def test_compare_coordination_numbers_case1(eax_solutes):
     # solvents_to_plot on x axis, each bar is a solute
     fig = compare_coordination_numbers(
         eax_solutes,
         solvents_to_plot=["fec", "pf6"],
         x_label="Species",
         y_label="Coordination",
         title="Bar Graph of Coordination Numbers",
     )
-    assert len(fig.data) == 4
-    for bar in fig.data:
-        assert set(bar.x) == {"fec", "pf6"}
-    # fig.show()
+    assert len(fig.data) == 2
 
 
 def test_compare_coordination_numbers_case2(eax_solutes):
     # solutes on x axis, each bar is an element of solvents_to_plot
     fig = compare_coordination_numbers(
         eax_solutes,
         solvents_to_plot=["pf6", "fec"],
         x_label="solute",
         y_label="Coordination",
         title="Bar Graph of Coordination Numbers",
-        x_axis="solute",
+        x_axis_solute=True,
     )
     assert len(fig.data) == 2
     for bar in fig.data:
         assert set(bar.x) == {"feaf", "eaf", "fea", "ea"}
-    # fig.show()
 
 
 def test_compare_coordination_numbers_case3(eax_solutes):
     # solvents_to_plot on x axis, each line is a solute
     fig = compare_coordination_numbers(
         eax_solutes,
         solvents_to_plot=["pf6", "fec"],
         x_label="solute",
         y_label="Coordination",
         title="Line Graph of Coordination Numbers",
         series=True,
     )
-    assert len(fig.data) == 4
-    for line in fig.data:
-        assert set(line.x) == {"fec", "pf6"}
-    # fig.show()
+    assert len(fig.data) == 2
 
 
 def test_compare_coordination_numbers_case4(eax_solutes):
     # solutes on x axis, each line is an element of solvents_to_plot
     fig = compare_coordination_numbers(
         eax_solutes,
         solvents_to_plot=["pf6", "fec"],
         x_label="solute",
         y_label="Coordination",
         title="Line Graph of Coordination Numbers",
-        x_axis="solute",
+        x_axis_solute=True,
         series=True,
     )
     assert len(fig.data) == 2
     for line in fig.data:
         assert set(line.x) == {"feaf", "eaf", "fea", "ea"}
-    # fig.show()
 
 
 # compare_residence_times tests
 def test_compare_residence_times(eax_solutes):
     # this test should handle an exception relating to the acceptable arguments for res_type
     for solute in eax_solutes.values():
         residence = Residence.from_solute(solute)
@@ -306,17 +316,13 @@
         eax_solutes,
         rename_solvent_dict={"ea": "EAx", "fea": "EAx", "eaf": "EAx", "feaf": "EAx"},
         solvents_to_plot=["pf6", "fec", "EAx"],
         x_label="Species",
         y_label="Pairing",
         title="Bar Graph of Solvent Pairing",
     )
-    assert len(fig.data) == 4
-    for bar in fig.data:
-        assert set(bar.x) == {"pf6", "fec", "EAx"}
-    # fig.show()
+    assert len(fig.data) == 3
 
 
 def test_plot_co_occurrence(solvation_data):
     speciation = Speciation(solvation_data, 10, 49)
-    fig = plot_co_occurrence(speciation)
-    # fig.show()
+    plot_co_occurrence(speciation)
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/test_rdf_parser.py` & `solvation_analysis-0.4.0/solvation_analysis/tests/test_rdf_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     ],  # the above values are not real
 )
 def test_identify_cutoff_scipy_easy(
     rdf_tag, cutoff, rdf_bins_and_data_easy, rdf_bins_and_data_hard
 ):
     bins, rdf = rdf_bins_and_data_easy[rdf_tag]
     np.testing.assert_allclose(
-        identify_cutoff_scipy(bins, rdf, failure_behavior="warn"),
+        identify_cutoff_scipy(bins, rdf, failure_behavior="warn", default=np.NaN),
         cutoff,
         atol=0.2,
         equal_nan=True,
     )
 
 @pytest.mark.parametrize("rdf_tag", ["fec_F", "fec_all", "bn_all", "pf6_all", "pf6_F"])
 def test_identify_cutoff_poly_hard(
@@ -144,16 +144,16 @@
 @pytest.mark.parametrize("rdf_tag", ["fec_F", "fec_all", "bn_all", "pf6_all", "pf6_F"])
 def test_identify_scipy_hard(
         rdf_tag, rdf_bins_and_data_easy, rdf_bins_and_data_hard
 ):
     bins_ez, rdf_ez = rdf_bins_and_data_easy[rdf_tag]
     bins_hd, rdf_hd = rdf_bins_and_data_hard[rdf_tag]
     np.testing.assert_allclose(
-        identify_cutoff_scipy(bins_hd, rdf_hd, failure_behavior="warn"),
-        identify_cutoff_scipy(bins_ez, rdf_ez, failure_behavior="warn"),
+        identify_cutoff_scipy(bins_hd, rdf_hd, failure_behavior="warn", default=np.NaN),
+        identify_cutoff_scipy(bins_ez, rdf_ez, failure_behavior="warn", default=np.NaN),
         atol=0.2,
         equal_nan=True,
     )
 
 
 @pytest.mark.parametrize(
     "rdf_tag",
@@ -201,11 +201,11 @@
     bins, rdf = rdf_bins_and_data_non_solv[rdf_tag]
     np.testing.assert_allclose(
         identify_cutoff_poly(bins, rdf, failure_behavior="warn"),
         np.NaN,
         equal_nan=True,
     )
     np.testing.assert_allclose(
-        identify_cutoff_scipy(bins, rdf, failure_behavior="warn"),
+        identify_cutoff_scipy(bins, rdf, failure_behavior="warn", default=np.NaN),
         np.NaN,
         equal_nan=True,
     )
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/test_residence.py` & `solvation_analysis-0.4.0/solvation_analysis/tests/test_residence.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,18 @@
         ("pf6", np.nan),
     ],
 )
 def test_residence_times(name, res_time, residence):
     np.testing.assert_almost_equal(residence.residence_times_cutoff[name], res_time, 3)
 
 
-@pytest.mark.parametrize("name", ['fec', 'bn', 'pf6'])
+@pytest.mark.parametrize("name", ["fec", "bn", "pf6"])
 def test_plot_auto_covariance(name, residence):
     residence.plot_auto_covariance(name)
 
 
 def test_residence_time_warning(solvation_data_sparse):
-    # we step through the data frame to speed up the tests
-    with pytest.warns(UserWarning, match="the autocovariance for pf6 does not converge"):
+    # we step through the dataframe to speed up the tests
+    with pytest.warns(
+        UserWarning, match="the autocovariance for pf6 does not converge"
+    ):
         Residence(solvation_data_sparse, step=10)
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/test_selection.py` & `solvation_analysis-0.4.0/solvation_analysis/tests/test_selection.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/test_solute.py` & `solvation_analysis-0.4.0/solvation_analysis/tests/test_solute.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,166 +1,160 @@
 from functools import reduce
 
-import matplotlib.pyplot as plt
-import warnings
 import pytest
 from solvation_analysis.solute import Solute
 import numpy as np
 from MDAnalysis import Universe
 
-from solvation_analysis.tests.conftest import u_eax_series, u_eax_atom_groups
-
 
 def test_instantiate_solute_from_atoms(pre_solute):
     # these check basic properties of the instantiation
     assert len(pre_solute.radii) == 3
     assert callable(pre_solute.kernel)
     assert pre_solute.solute_atoms.n_residues == 49
-    assert pre_solute.solvents['pf6'].n_residues == 49
-    assert pre_solute.solvents['fec'].n_residues == 237
-    assert pre_solute.solvents['bn'].n_residues == 363
+    assert pre_solute.solvents["pf6"].n_residues == 49
+    assert pre_solute.solvents["fec"].n_residues == 237
+    assert pre_solute.solvents["bn"].n_residues == 363
 
 
 def test_init_fail(atom_groups):
     with pytest.raises(RuntimeError):
-        Solute(atom_groups['li'], {'pf6': atom_groups['pf6']})
+        Solute(atom_groups["li"], {"pf6": atom_groups["pf6"]})
 
 
 def test_networking_instantiation_error(atom_groups):
-    li = atom_groups['li']
-    pf6 = atom_groups['pf6']
-    bn = atom_groups['bn']
-    fec = atom_groups['fec']
+    li = atom_groups["li"]
+    pf6 = atom_groups["pf6"]
+    bn = atom_groups["bn"]
+    fec = atom_groups["fec"]
     with pytest.raises(Exception):
         Solute.from_atoms(
-            li, {'pf6': pf6, 'bn': bn, 'fec': fec}, analysis_classes=['networking']
+            li, {"pf6": pf6, "bn": bn, "fec": fec}, analysis_classes=["networking"]
         )
 
 
 def test_plot_solvation_distance(rdf_bins_and_data_easy):
-    bins, data = rdf_bins_and_data_easy['pf6_all']
-    fig, ax = Solute._plot_solvation_radius(bins, data, 2)
-    # fig.show()  # comment out for global testing
+    bins, data = rdf_bins_and_data_easy["pf6_all"]
+    Solute._plot_solvation_radius(bins, data, 2)
 
 
 def test_radii_finding(run_solute):
     # checks that the solvation radii are plotted
     assert len(run_solute.radii) == 3
     assert len(run_solute.rdf_data["solute_0"]) == 3
     # checks that the identified solvation radii are approximately correct
-    assert 2 < run_solute.radii['pf6'] < 3
-    assert 2 < run_solute.radii['fec'] < 3
-    assert 2 < run_solute.radii['bn'] < 3
-    # for fig, ax in run_solute.rdf_plots.values():
-    # plt.show()  # comment out for global testing
-
-
-def test_run_warning(pre_solute_mutable):
-    # checks that an error is thrown if there are not enough radii
-    pre_solute_mutable.radii = {'pf6': 2.8}
-    with pytest.raises(AssertionError):
-        pre_solute_mutable.run(step=1)
+    assert 2 < run_solute.radii["pf6"] < 3
+    assert 2 < run_solute.radii["fec"] < 3
+    assert 2 < run_solute.radii["bn"] < 3
 
 
 def test_run(pre_solute_mutable):
     # checks that run is run correctly
     pre_solute_mutable.run(step=1)
     assert len(pre_solute_mutable._solvation_frames) == 10
     assert len(pre_solute_mutable._solvation_frames[0]) == 228
     assert len(pre_solute_mutable.solvation_data) == 2312
 
 
 def test_run_w_all(pre_solute_mutable):
     # checks that run is run correctly
     pre_solute_mutable.analysis_classes = [
-        "pairing", "coordination", "speciation", "residence", "networking"
+        "pairing",
+        "coordination",
+        "speciation",
+        "residence",
+        "networking",
     ]
-    pre_solute_mutable.networking_solvents = 'pf6'
+    pre_solute_mutable.networking_solvents = "pf6"
     pre_solute_mutable.run(step=1)
     assert len(pre_solute_mutable._solvation_frames) == 10
     assert len(pre_solute_mutable._solvation_frames[0]) == 228
     assert len(pre_solute_mutable.solvation_data) == 2312
 
 
 @pytest.mark.parametrize(
     "solute_index, radius, frame, expected_res_ids",
     [
         (1, 3, 5, [46, 100, 171, 255, 325, 521, 650]),
         (2, 3, 6, [13, 59, 177, 264, 314, 651]),
-        (40, 3.5, 0, [101, 126, 127, 360, 368, 305, 689])
+        (40, 3.5, 0, [101, 126, 127, 360, 368, 305, 689]),
     ],
 )
 def test_radial_shell(solute_index, radius, frame, expected_res_ids, run_solute):
     run_solute.u.trajectory[frame]
     shell = run_solute.radial_shell(solute_index, radius)
     assert set(shell.resindices) == set(expected_res_ids)
 
 
 @pytest.mark.parametrize(
     "solute_index, n_mol, frame, expected_res_ids",
     [
         (6741, 4, 5, [46, 100, 171, 255, 650]),
         (6749, 5, 6, [13, 59, 177, 264, 314, 651]),
-        (7053, 6, 0, [101, 126, 127, 360, 368, 305, 689])
+        (7053, 6, 0, [101, 126, 127, 360, 368, 305, 689]),
     ],
 )
 def test_closest_n_mol(solute_index, n_mol, frame, expected_res_ids, run_solute):
     run_solute.u.trajectory[frame]
     shell = run_solute.get_closest_n_mol(solute_index, n_mol)
     assert set(shell.resindices) == set(expected_res_ids)
 
 
 @pytest.mark.parametrize(
     "solute_index, step, expected_res_ids",
     [
         (650, 5, [46, 100, 171, 255, 650]),
         (651, 6, [13, 59, 177, 264, 314, 651]),
-        (689, 0, [101, 126, 127, 360, 689])
+        (689, 0, [101, 126, 127, 360, 689]),
     ],
 )
 def test_solvation_shell(solute_index, step, expected_res_ids, run_solute):
     # TODO: something is broken in the tutorial here
     shell = run_solute.get_shell(solute_index, step)
     assert set(shell.resindices) == set(expected_res_ids)
 
 
 @pytest.mark.parametrize(
     "solute_index, step, remove, expected_res_ids",
     [
-        (650, 5, {'bn': 1}, [46, 171, 255, 650]),
-        (651, 6, {'bn': 2, 'fec': 1}, [13, 177, 314, 651]),
-        (689, 0, {'fec': 1}, [101, 126, 127, 360, 689])
+        (650, 5, {"bn": 1}, [46, 171, 255, 650]),
+        (651, 6, {"bn": 2, "fec": 1}, [13, 177, 314, 651]),
+        (689, 0, {"fec": 1}, [101, 126, 127, 360, 689]),
     ],
 )
-def test_solvation_shell_remove_mols(solute_index, step, remove, expected_res_ids, run_solute):
+def test_solvation_shell_remove_mols(
+    solute_index, step, remove, expected_res_ids, run_solute
+):
     shell = run_solute.get_shell(solute_index, step, remove_mols=remove)
     assert set(shell.resindices) == set(expected_res_ids)
 
 
 @pytest.mark.parametrize(
     "solute_index, step, n, expected_res_ids",
     [
         (650, 5, 3, [46, 171, 255, 650]),
         (651, 6, 3, [13, 177, 314, 651]),
         (689, 0, 4, [101, 126, 127, 360, 689]),
-        (689, 0, 1, [101, 689])
+        (689, 0, 1, [101, 689]),
     ],
 )
-def test_solvation_shell_remove_closest(solute_index, step, n, expected_res_ids, run_solute):
+def test_solvation_shell_remove_closest(
+    solute_index, step, n, expected_res_ids, run_solute
+):
     shell = run_solute.get_shell(solute_index, step, closest_n_only=n)
     assert set(shell.resindices) == set(expected_res_ids)
 
 
 @pytest.mark.parametrize(
     "shell, n_shells",
     [
-        ({'bn': 5, 'fec': 0, 'pf6': 0}, 175),
-        ({'bn': 3, 'fec': 3, 'pf6': 0}, 2),
-        ({'bn': 3, 'fec': 0, 'pf6': 1}, 13),
-        ({'bn': 4}, 260),
+        ({"bn": 5, "fec": 0, "pf6": 0}, 175),
+        ({"bn": 3, "fec": 3, "pf6": 0}, 2),
+        ({"bn": 3, "fec": 0, "pf6": 1}, 13),
+        ({"bn": 4}, 260),
     ],
 )
 def test_speciation_find_shells(shell, n_shells, run_solute):
     # duplicated to test in solute
     df = run_solute.speciation.get_shells(shell)
     assert len(df) == n_shells
 
@@ -189,180 +183,188 @@
 )
 def test_pairing(name, fraction, run_solute):
     # duplicated to test in solute
     pairing_dict = run_solute.pairing.solvent_pairing
     np.testing.assert_allclose([fraction], pairing_dict[name], atol=0.05)
 
 
-@pytest.mark.parametrize("name", ['ea', 'eaf', 'fea', 'feaf'])
+@pytest.mark.parametrize("name", ["ea", "eaf", "fea", "feaf"])
 def test_instantiate_eax_solvents(name, u_eax_series):
     assert isinstance(u_eax_series[name], Universe)
 
 
-@pytest.mark.parametrize("name", ['ea', 'eaf', 'fea', 'feaf'])
+@pytest.mark.parametrize("name", ["ea", "eaf", "fea", "feaf"])
 def test_instantiate_eax_atom_groups(name, u_eax_atom_groups):
-    all_atoms = len(u_eax_atom_groups[name]['li'].universe.atoms)
+    all_atoms = len(u_eax_atom_groups[name]["li"].universe.atoms)
     all_atoms_in_groups = sum([len(ag) for ag in u_eax_atom_groups[name].values()])
     assert all_atoms_in_groups == all_atoms
 
 
-@pytest.mark.parametrize("name", ['ea', 'eaf', 'fea', 'feaf'])
+@pytest.mark.parametrize("name", ["ea", "eaf", "fea", "feaf"])
 def test_instantiate_eax_solutes(name, eax_solutes):
     assert isinstance(eax_solutes[name], Solute)
 
 
 def test_plot_solvation_radius(run_solute, iba_small_solute):
-    run_solute.plot_solvation_radius('solute_0', 'fec')
-    iba_small_solute.plot_solvation_radius('iba_ketone', 'iba')
+    run_solute.plot_solvation_radius("solute_0", "fec")
+    iba_small_solute.plot_solvation_radius("iba_ketone", "iba")
 
 
-@pytest.mark.parametrize("residue", ['iba_ketone', 'solute', 'H2O', 'iba'])
+@pytest.mark.parametrize("residue", ["iba_ketone", "solute", "H2O", "iba"])
 def test_draw_molecule_string(iba_solutes, residue):
-    iba_solutes['iba_ketone'].draw_molecule(residue)
+    iba_solutes["iba_ketone"].draw_molecule(residue)
 
 
 def test_draw_molecule_residue(iba_solutes):
-    solute = iba_solutes['iba_ketone']
+    solute = iba_solutes["iba_ketone"]
     residue = solute.u.atoms.residues[0]
     solute.draw_molecule(residue)
 
 
 def test_iba_solutes(iba_solutes):
     for solute in iba_solutes.values():
         assert isinstance(solute, Solute)
 
 
 def test_from_atoms(iba_atom_groups, iba_solvents):
     solute_atoms = (
-            iba_atom_groups['iba_ketone'] +
-            iba_atom_groups['iba_alcohol_O'] +
-            iba_atom_groups['iba_alcohol_H']
+        iba_atom_groups["iba_ketone"]
+        + iba_atom_groups["iba_alcohol_O"]
+        + iba_atom_groups["iba_alcohol_H"]
     )
     solute = Solute.from_atoms(solute_atoms, iba_solvents)
     solute.run()
-    assert set(solute.atom_solutes.keys()) == {'solute_0', 'solute_1', 'solute_2'}
+    assert set(solute.atom_solutes.keys()) == {"solute_0", "solute_1", "solute_2"}
 
 
 def test_from_atoms_errors(iba_atom_groups, H2O_atom_groups, iba_solvents):
     solute_atoms = (
-            iba_atom_groups['iba_ketone'] +
-            iba_atom_groups['iba_alcohol_O'] +
-            iba_atom_groups['iba_alcohol_H']
+        iba_atom_groups["iba_ketone"]
+        + iba_atom_groups["iba_alcohol_O"]
+        + iba_atom_groups["iba_alcohol_H"]
     )
     with pytest.raises(AssertionError):
         bad_atoms = solute_atoms[:-2]
         Solute.from_atoms(bad_atoms, iba_solvents)
 
     with pytest.raises(AssertionError):
-        bad_atoms = solute_atoms + H2O_atom_groups['H2O_O']
+        bad_atoms = solute_atoms + H2O_atom_groups["H2O_O"]
         Solute.from_atoms(bad_atoms, iba_solvents)
 
 
 def test_from_atoms_dict(iba_atom_groups, iba_solvents):
     solute_atoms = {
-        'iba_ketone': iba_atom_groups['iba_ketone'],
-        'iba_alcohol_O': iba_atom_groups['iba_alcohol_O'],
-        'iba_alcohol_H': iba_atom_groups['iba_alcohol_H']
+        "iba_ketone": iba_atom_groups["iba_ketone"],
+        "iba_alcohol_O": iba_atom_groups["iba_alcohol_O"],
+        "iba_alcohol_H": iba_atom_groups["iba_alcohol_H"],
     }
     solute = Solute.from_atoms_dict(solute_atoms, iba_solvents)
-    assert set(solute.atom_solutes.keys()) == {'iba_ketone', 'iba_alcohol_O', 'iba_alcohol_H'}
+    assert set(solute.atom_solutes.keys()) == {
+        "iba_ketone",
+        "iba_alcohol_O",
+        "iba_alcohol_H",
+    }
     solute.run()
 
 
 def test_from_atoms_dict_errors(iba_atom_groups, H2O_atom_groups, iba_solvents):
     solute_atoms = {
-        'iba_ketone': iba_atom_groups['iba_ketone'],
-        'iba_alcohol_O': iba_atom_groups['iba_alcohol_O'],
-        'iba_alcohol_H': iba_atom_groups['iba_alcohol_H']
+        "iba_ketone": iba_atom_groups["iba_ketone"],
+        "iba_alcohol_O": iba_atom_groups["iba_alcohol_O"],
+        "iba_alcohol_H": iba_atom_groups["iba_alcohol_H"],
     }
     with pytest.raises(AssertionError):
         bad_atoms = {**solute_atoms}
-        bad_atoms['iba_ketone'] = bad_atoms['iba_ketone'][:-2]
+        bad_atoms["iba_ketone"] = bad_atoms["iba_ketone"][:-2]
         Solute.from_atoms_dict(bad_atoms, iba_solvents)
 
     with pytest.raises(AssertionError):
         bad_atoms = {**solute_atoms}
-        bad_atoms['iba_ketone'] = bad_atoms['iba_ketone'] + bad_atoms['iba_alcohol_O']
+        bad_atoms["iba_ketone"] = bad_atoms["iba_ketone"] + bad_atoms["iba_alcohol_O"]
         Solute.from_atoms_dict(bad_atoms, iba_solvents)
 
     with pytest.raises(AssertionError):
         bad_atoms = {**solute_atoms}
-        bad_atoms['iba_ketone'] = bad_atoms['iba_alcohol_O']
+        bad_atoms["iba_ketone"] = bad_atoms["iba_alcohol_O"]
         Solute.from_atoms_dict(bad_atoms, iba_solvents)
 
     with pytest.raises(AssertionError):
         bad_atoms = {**solute_atoms}
-        bad_atoms['H2O_O'] = H2O_atom_groups['H2O_O']
+        bad_atoms["H2O_O"] = H2O_atom_groups["H2O_O"]
         Solute.from_atoms_dict(bad_atoms, iba_solvents)
 
 
 def test_from_solute_list(iba_solutes, iba_solvents):
     solute_list = [
-            iba_solutes['iba_ketone'],
-            iba_solutes['iba_alcohol_O'],
-            iba_solutes['iba_alcohol_H']
+        iba_solutes["iba_ketone"],
+        iba_solutes["iba_alcohol_O"],
+        iba_solutes["iba_alcohol_H"],
     ]
     solute = Solute.from_solute_list(solute_list, iba_solvents)
     solute.run()
-    assert set(solute.atom_solutes.keys()) == {'iba_ketone', 'iba_alcohol_O', 'iba_alcohol_H'}
+    assert set(solute.atom_solutes.keys()) == {
+        "iba_ketone",
+        "iba_alcohol_O",
+        "iba_alcohol_H",
+    }
 
 
 def test_from_solute_list_restepped(iba_solutes, iba_atom_groups, iba_solvents):
     new_solvent = {"H2O": iba_solvents["H2O"]}
     new_ketone = Solute.from_atoms(
-        iba_atom_groups['iba_ketone'],
-        new_solvent,
-        solute_name='iba_ketone'
+        iba_atom_groups["iba_ketone"], new_solvent, solute_name="iba_ketone"
     )
     new_ketone.run(step=2)
-    solute_list = [iba_solutes['iba_alcohol_O'], new_ketone]
+    solute_list = [iba_solutes["iba_alcohol_O"], new_ketone]
     solute = Solute.from_solute_list(solute_list, iba_solvents)
-    with pytest.warns(UserWarning, match='re-run') as record:
+    with pytest.warns(UserWarning, match="re-run") as record:
         solute.run(step=2)
         user_warnings = 0
         for warning in record:
             if warning.category == UserWarning:
                 user_warnings += 1
         assert user_warnings == 2
-    assert set(solute.atom_solutes.keys()) == {'iba_ketone', 'iba_alcohol_O'}
+    assert set(solute.atom_solutes.keys()) == {"iba_ketone", "iba_alcohol_O"}
 
 
 def test_from_solute_list_errors(iba_solutes, H2O_atom_groups, iba_solvents):
     solute_list = [
-        iba_solutes['iba_ketone'],
-        iba_solutes['iba_alcohol_O'],
-        iba_solutes['iba_alcohol_H']
+        iba_solutes["iba_ketone"],
+        iba_solutes["iba_alcohol_O"],
+        iba_solutes["iba_alcohol_H"],
     ]
 
-    H2O_solute = Solute.from_atoms(H2O_atom_groups['H2O_O'], iba_solvents)
+    H2O_solute = Solute.from_atoms(H2O_atom_groups["H2O_O"], iba_solvents)
     with pytest.raises(AssertionError):
         bad_solute_list = [*solute_list]
         bad_solute_list.append(H2O_solute)
         Solute.from_solute_list(bad_solute_list, iba_solvents)
 
     iba_ketone_renamed = Solute.from_atoms(
-        iba_solutes['iba_ketone'].solute_atoms,
+        iba_solutes["iba_ketone"].solute_atoms,
         iba_solvents,
-        solute_name='iba_alcohol_O'
+        solute_name="iba_alcohol_O",
     )
     with pytest.raises(AssertionError):
         bad_solute_list = [*solute_list]
         bad_solute_list[0] = iba_ketone_renamed
         Solute.from_solute_list(bad_solute_list, iba_solvents)
 
     with pytest.raises(AssertionError):
         bad_solute_list = [1, 2, 3]
         Solute.from_solute_list(bad_solute_list, iba_solvents)
 
 
 def test_iba_all_analysis(iba_atom_groups, iba_solvents):
-    solute_atoms = reduce(lambda x, y: x | y, [solute for solute in iba_atom_groups.values()])
+    solute_atoms = reduce(
+        lambda x, y: x | y, [solute for solute in iba_atom_groups.values()]
+    )
     solute = Solute.from_atoms(
         solute_atoms,
         iba_solvents,
-        networking_solvents=['iba'],
-        analysis_classes='all',
-        radii={'iba': 1.9, 'H2O': 1.9},
+        networking_solvents=["iba"],
+        analysis_classes="all",
+        radii={"iba": 1.9, "H2O": 1.9},
     )
     # TODO: get this passing
     solute.run(step=4)
     return
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis/tests/test_speciation.py` & `solvation_analysis-0.4.0/solvation_analysis/tests/test_speciation.py`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/solvation_analysis.egg-info/PKG-INFO` & `solvation_analysis-0.4.0/solvation_analysis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solvation-analysis
-Version: 0.3.5
+Version: 0.4.0
 Summary: A toolkit to analyze solvation structure in molecular dynamics trajectories.
 Author: Orion Cohen
 Author-email: Orion Cohen <orioncohen@berkeley.edu>
 Maintainer-email: Orion Cohen <orioncohen@berkeley.edu>, Hugo MacDermott-Opeskin <hugomacdermott@gmail.com>
 License:                         GNU GENERAL PUBLIC LICENSE 
                                   Version 3, 29 June 2007
         
@@ -604,15 +604,15 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: pandas>=2.2
 Requires-Dist: mdanalysis>=2.0.0
 Requires-Dist: pytest
 Requires-Dist: matplotlib
 Requires-Dist: setuptools
-Requires-Dist: scipy
+Requires-Dist: scipy==1.12.0
 Requires-Dist: statsmodels
 Requires-Dist: plotly
 Requires-Dist: rdkit
 
 SolvationAnalysis
 ==============================
 [//]: # (Badges)
@@ -626,47 +626,65 @@
 
 [//]: # ([![DOI]&#40;https://zenodo.org/badge/371804402.svg&#41;]&#40;https://zenodo.org/badge/latestdoi/371804402&#41;)
 
 
 ---
 
 Solvation analysis implements a robust, cohesive, and fast set of methods
-for analyzing the solvation structure of a liquid. It seamlessly integrates with
-[MDAnalysis](https://www.mdanalysis.org/), making use of the core AtomGroup
-and Universe data structures to parse solvation information. If you are interested
-in understanding the solvation structure of a liquid, this package is for you!
+for analyzing the solvation structure of a liquid. It integrates with
+[MDAnalysis](https://www.mdanalysis.org/) to seamlessly calculate, query,
+and visualize solvation information.
 
-
-Find documentation and tutorials on [readthedocs].
+Find documentation and tutorials on [readthedocs](https://solvation-analysis.readthedocs.io/en/latest/).
 
 ### Installing SolvationAnalysis
 
 SolvationAnalysis is available on PyPI and conda-forge can be installed with pip or conda:
 
 ```bash
 pip install solvation-analysis
 
 # or
 
 conda install -c conda-forge solvation_analysis
 ```
 
+### Solvation Analysis Summarized
+
+![summary](docs/tutorials/images/summary_figure.png)
+
+
+### Visualization
+
+With just a few lines of code, solvation analysis can calculate detailed
+properties within and between solvent systems. A few examples are shown below.
+
+![solvation_analysis.plotting.compare_coordination_numbers](docs/tutorials/images/coordination_plot.png)
+
+![solvation_analysis.plotting.plot_speciation](docs/tutorials/images/speciation_plot.png)
+
+![solvation_analysis.plotting.plot_rdfs](docs/tutorials/images/rdf_plot.png)
+
+
 ### Contributing
 
-Contributions, both issues and PRs, are welcome. If you'd like to contribute, we ask that you 
+Contributions, both issues and PRs, are welcome. If you'd like to contribute, we ask that you
 follow the community guidelines outlined in the [MDAnalysis Code of Conduct](https://www.mdanalysis.org/pages/conduct/).
 
+Solvation Analysis uses [pre-commit](https://pre-commit.com/) for linting. Make sure to install
+the pre-commit hooks if you are working on a contribution.
+
 ### Citation
 
 This work is described in [JOSS](https://doi.org/10.21105/joss.05183), please cite it if you make
 use of this package in published work.
 
 ---
 
-Project based on the 
+Project based on the
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.5.
 
 
 
 [readthedocs]: (https://solvation-analysis.readthedocs.io/en/latest/)
 [robust, cohesive, and fast set of methods]:(https://summerofcode.withgoogle.com/projects/#6227159028334592)
 [Google Summer of Code]: https://summerofcode.withgoogle.com/
```

### Comparing `solvation-analysis-0.3.5/solvation_analysis.egg-info/SOURCES.txt` & `solvation_analysis-0.4.0/solvation_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solvation-analysis-0.3.5/versioneer.py` & `solvation_analysis-0.4.0/versioneer.py`

 * *Files identical despite different names*

