# Comparing `tmp/csp_cryspy-1.2.4.tar.gz` & `tmp/csp_cryspy-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csp_cryspy-1.2.4.tar", last modified: Tue May  7 08:17:08 2024, max compression
+gzip compressed data, was "csp_cryspy-1.2.5.tar", last modified: Fri May 10 04:58:33 2024, max compression
```

## Comparing `csp_cryspy-1.2.4.tar` & `csp_cryspy-1.2.5.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.369386 csp_cryspy-1.2.4/
--rw-r--r--   0 yamashita06   (501) staff       (20)     1080 2018-02-20 06:34:19.000000 csp_cryspy-1.2.4/LICENSE
--rw-r--r--   0 yamashita06   (501) staff       (20)     6226 2024-05-07 08:17:08.369116 csp_cryspy-1.2.4/PKG-INFO
--rw-r--r--   0 yamashita06   (501) staff       (20)     4291 2024-05-07 08:08:08.000000 csp_cryspy-1.2.4/README.md
--rw-r--r--   0 yamashita06   (501) staff       (20)      991 2023-03-16 13:18:20.000000 csp_cryspy-1.2.4/pyproject.toml
--rw-r--r--   0 yamashita06   (501) staff       (20)       38 2024-05-07 08:17:08.369426 csp_cryspy-1.2.4/setup.cfg
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.344656 csp_cryspy-1.2.4/src/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.345396 csp_cryspy-1.2.4/src/cryspy/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.347514 csp_cryspy-1.2.4/src/cryspy/BO/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/BO/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2651 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/BO/bo_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     7087 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/BO/bo_next_select.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      726 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/BO/bo_restart.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4907 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/BO/combo_cryspy.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      757 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/BO/select_descriptor.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.349009 csp_cryspy-1.2.4/src/cryspy/EA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/EA/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      823 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/EA/calc_ef.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4834 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/EA/calc_hull.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4042 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/EA/ea_append.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     8211 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/EA/ea_child.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4107 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/EA/ea_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     7725 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/EA/ea_next_gen.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.351202 csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1963 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/addition.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    14110 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/adj_comp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    30058 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/crossover.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    14404 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/ea_generation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1299 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/elimination.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     8444 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/permutation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2849 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/rotation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     9549 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/select_parents.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6428 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/strain.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2688 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/substitution.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.352320 csp_cryspy-1.2.4/src/cryspy/IO/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/IO/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      452 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/IO/change_input.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1794 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/IO/io_stat.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6219 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/IO/out_results.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     5079 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/IO/pkl_data.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    78090 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/IO/read_input.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.354184 csp_cryspy-1.2.4/src/cryspy/LAQA/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/LAQA/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      900 2023-05-16 07:40:54.000000 csp_cryspy-1.2.4/src/cryspy/LAQA/calc_score.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1475 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/LAQA/laqa_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1929 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/LAQA/laqa_next_selection.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1116 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/LAQA/laqa_restart.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.355127 csp_cryspy-1.2.4/src/cryspy/RS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/RS/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.356051 csp_cryspy-1.2.4/src/cryspy/RS/gen_struc_RS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/RS/gen_struc_RS/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    25584 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    19080 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/RS/gen_struc_RS/random_generation.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      437 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/RS/rs_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      669 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/RS/rs_restart.py
--rw-r--r--   0 yamashita06   (501) staff       (20)       65 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.356244 csp_cryspy-1.2.4/src/cryspy/calc_dscrpt/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.356829 csp_cryspy-1.2.4/src/cryspy/calc_dscrpt/FP/
--rw-r--r--   0 yamashita06   (501) staff       (20)       22 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/calc_dscrpt/FP/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2821 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/calc_dscrpt/FP/calc_FP.py
--rw-r--r--   0 yamashita06   (501) staff       (20)       17 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/calc_dscrpt/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.358224 csp_cryspy-1.2.4/src/cryspy/interactive/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:03:15.000000 csp_cryspy-1.2.4/src/cryspy/interactive/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1026 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interactive/action.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1839 2023-10-18 03:35:51.000000 csp_cryspy-1.2.4/src/cryspy/interactive/energy_plot.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     6479 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interactive/restart_intract.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      505 2023-10-18 03:35:51.000000 csp_cryspy-1.2.4/src/cryspy/interactive/rslt_energy.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      452 2023-10-18 03:35:51.000000 csp_cryspy-1.2.4/src/cryspy/interactive/view_atom.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.358855 csp_cryspy-1.2.4/src/cryspy/interface/
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.359614 csp_cryspy-1.2.4/src/cryspy/interface/ASE/
--rw-r--r--   0 yamashita06   (501) staff       (20)      818 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/interface/ASE/calc_files_ase.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1156 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/ASE/collect_ase.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1838 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/ASE/ctrl_job_ase.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.360509 csp_cryspy-1.2.4/src/cryspy/interface/LAMMPS/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/interface/LAMMPS/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      988 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/interface/LAMMPS/calc_files_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     1621 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/LAMMPS/collect_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2281 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2955 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/LAMMPS/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.361413 csp_cryspy-1.2.4/src/cryspy/interface/OMX/
--rw-r--r--   0 yamashita06   (501) staff       (20)      886 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/interface/OMX/calc_files_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2851 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/OMX/collect_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4616 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/OMX/ctrl_job_OMX.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3205 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/OMX/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.362419 csp_cryspy-1.2.4/src/cryspy/interface/QE/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/interface/QE/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      836 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/interface/QE/calc_files_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    11391 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/QE/collect_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4484 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/QE/ctrl_job_qe.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2945 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/QE/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.363476 csp_cryspy-1.2.4/src/cryspy/interface/VASP/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/interface/VASP/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      795 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/interface/VASP/calc_files_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     9130 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/VASP/collect_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3606 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/VASP/ctrl_job_vasp.py
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/interface/__init__.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.364067 csp_cryspy-1.2.4/src/cryspy/interface/ext/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/interface/ext/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      513 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/interface/ext/collect_ext.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     8681 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/select_code.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.365155 csp_cryspy-1.2.4/src/cryspy/interface/soiap/
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/interface/soiap/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)      839 2023-07-10 10:34:05.000000 csp_cryspy-1.2.4/src/cryspy/interface/soiap/calc_files_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     7519 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/soiap/collect_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2358 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/soiap/ctrl_job_soiap.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     2416 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/interface/soiap/structure.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.365599 csp_cryspy-1.2.4/src/cryspy/job/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/job/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    13495 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/job/ctrl_ext.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    33247 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/job/ctrl_job.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.366289 csp_cryspy-1.2.4/src/cryspy/scripts/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/scripts/__init__.py
--rwxr-xr-x   0 yamashita06   (501) staff       (20)     4416 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/scripts/cryspy.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.366880 csp_cryspy-1.2.4/src/cryspy/start/
--rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/start/__init__.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     5544 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/start/cryspy_init.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     4701 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/start/cryspy_restart.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     7376 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/start/gen_init_struc.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.367548 csp_cryspy-1.2.4/src/cryspy/util/
--rw-r--r--   0 yamashita06   (501) staff       (20)      106 2023-03-16 12:21:45.000000 csp_cryspy-1.2.4/src/cryspy/util/constants.py
--rw-r--r--   0 yamashita06   (501) staff       (20)    15905 2024-05-07 06:33:41.000000 csp_cryspy-1.2.4/src/cryspy/util/struc_util.py
--rw-r--r--   0 yamashita06   (501) staff       (20)     3825 2024-05-07 06:55:30.000000 csp_cryspy-1.2.4/src/cryspy/util/utility.py
-drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-07 08:17:08.368806 csp_cryspy-1.2.4/src/csp_cryspy.egg-info/
--rw-r--r--   0 yamashita06   (501) staff       (20)     6226 2024-05-07 08:17:08.000000 csp_cryspy-1.2.4/src/csp_cryspy.egg-info/PKG-INFO
--rw-r--r--   0 yamashita06   (501) staff       (20)     3543 2024-05-07 08:17:08.000000 csp_cryspy-1.2.4/src/csp_cryspy.egg-info/SOURCES.txt
--rw-r--r--   0 yamashita06   (501) staff       (20)        1 2024-05-07 08:17:08.000000 csp_cryspy-1.2.4/src/csp_cryspy.egg-info/dependency_links.txt
--rw-r--r--   0 yamashita06   (501) staff       (20)       54 2024-05-07 08:17:08.000000 csp_cryspy-1.2.4/src/csp_cryspy.egg-info/entry_points.txt
--rw-r--r--   0 yamashita06   (501) staff       (20)       14 2024-05-07 08:17:08.000000 csp_cryspy-1.2.4/src/csp_cryspy.egg-info/requires.txt
--rw-r--r--   0 yamashita06   (501) staff       (20)        7 2024-05-07 08:17:08.000000 csp_cryspy-1.2.4/src/csp_cryspy.egg-info/top_level.txt
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.923330 csp_cryspy-1.2.5/
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1080 2018-02-20 06:34:19.000000 csp_cryspy-1.2.5/LICENSE
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6311 2024-05-10 04:58:33.923096 csp_cryspy-1.2.5/PKG-INFO
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4376 2024-05-10 04:52:57.000000 csp_cryspy-1.2.5/README.md
+-rw-------   0 yamashita06   (501) staff       (20)      991 2023-03-16 13:18:20.000000 csp_cryspy-1.2.5/pyproject.toml
+-rw-r--r--   0 yamashita06   (501) staff       (20)       38 2024-05-10 04:58:33.923373 csp_cryspy-1.2.5/setup.cfg
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.894028 csp_cryspy-1.2.5/src/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.894792 csp_cryspy-1.2.5/src/cryspy/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.896642 csp_cryspy-1.2.5/src/cryspy/BO/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/BO/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2651 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/BO/bo_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     7087 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/BO/bo_next_select.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      726 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/BO/bo_restart.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4907 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/BO/combo_cryspy.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      757 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/BO/select_descriptor.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.898662 csp_cryspy-1.2.5/src/cryspy/EA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/EA/__init__.py
+-rw-------   0 yamashita06   (501) staff       (20)      823 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/calc_ef.py
+-rw-------   0 yamashita06   (501) staff       (20)     4834 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/calc_hull.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4042 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/EA/ea_append.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     8211 2024-05-06 04:10:37.000000 csp_cryspy-1.2.5/src/cryspy/EA/ea_child.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4107 2024-05-07 01:16:55.000000 csp_cryspy-1.2.5/src/cryspy/EA/ea_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     7725 2024-05-07 04:29:17.000000 csp_cryspy-1.2.5/src/cryspy/EA/ea_next_gen.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.902115 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/__init__.py
+-rw-------   0 yamashita06   (501) staff       (20)     1963 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/addition.py
+-rw-------   0 yamashita06   (501) staff       (20)    14110 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/adj_comp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    30058 2024-05-07 01:18:49.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/crossover.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    14404 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/ea_generation.py
+-rw-------   0 yamashita06   (501) staff       (20)     1299 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/elimination.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     8444 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/permutation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2849 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/rotation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     9549 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/select_parents.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6428 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/strain.py
+-rw-------   0 yamashita06   (501) staff       (20)     2688 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/substitution.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.903709 csp_cryspy-1.2.5/src/cryspy/IO/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/IO/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      452 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/IO/change_input.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1794 2023-11-17 03:52:02.000000 csp_cryspy-1.2.5/src/cryspy/IO/io_stat.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6223 2024-05-10 04:42:44.000000 csp_cryspy-1.2.5/src/cryspy/IO/out_results.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5079 2024-04-30 07:56:08.000000 csp_cryspy-1.2.5/src/cryspy/IO/pkl_data.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    78090 2024-05-02 13:30:51.000000 csp_cryspy-1.2.5/src/cryspy/IO/read_input.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.905768 csp_cryspy-1.2.5/src/cryspy/LAQA/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/LAQA/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      900 2023-05-16 07:40:54.000000 csp_cryspy-1.2.5/src/cryspy/LAQA/calc_score.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1475 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/LAQA/laqa_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1929 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/LAQA/laqa_next_selection.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1116 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/LAQA/laqa_restart.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.906721 csp_cryspy-1.2.5/src/cryspy/RS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/RS/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.907603 csp_cryspy-1.2.5/src/cryspy/RS/gen_struc_RS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/RS/gen_struc_RS/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    25584 2024-05-10 04:40:12.000000 csp_cryspy-1.2.5/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    19080 2023-11-11 11:29:31.000000 csp_cryspy-1.2.5/src/cryspy/RS/gen_struc_RS/random_generation.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      437 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/RS/rs_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      669 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/RS/rs_restart.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)       65 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.908072 csp_cryspy-1.2.5/src/cryspy/calc_dscrpt/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.908918 csp_cryspy-1.2.5/src/cryspy/calc_dscrpt/FP/
+-rw-r--r--   0 yamashita06   (501) staff       (20)       22 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/calc_dscrpt/FP/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2821 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/calc_dscrpt/FP/calc_FP.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)       17 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/calc_dscrpt/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.910492 csp_cryspy-1.2.5/src/cryspy/interactive/
+-rw-------   0 yamashita06   (501) staff       (20)        0 2023-06-14 14:03:15.000000 csp_cryspy-1.2.5/src/cryspy/interactive/__init__.py
+-rw-------   0 yamashita06   (501) staff       (20)     1026 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/interactive/action.py
+-rw-------   0 yamashita06   (501) staff       (20)     1839 2023-10-18 03:35:51.000000 csp_cryspy-1.2.5/src/cryspy/interactive/energy_plot.py
+-rw-------   0 yamashita06   (501) staff       (20)     6479 2023-11-17 03:50:43.000000 csp_cryspy-1.2.5/src/cryspy/interactive/restart_intract.py
+-rw-------   0 yamashita06   (501) staff       (20)      505 2023-10-18 03:35:51.000000 csp_cryspy-1.2.5/src/cryspy/interactive/rslt_energy.py
+-rw-------   0 yamashita06   (501) staff       (20)      452 2023-10-18 03:35:51.000000 csp_cryspy-1.2.5/src/cryspy/interactive/view_atom.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.911077 csp_cryspy-1.2.5/src/cryspy/interface/
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.912036 csp_cryspy-1.2.5/src/cryspy/interface/ASE/
+-rw-------   0 yamashita06   (501) staff       (20)      818 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/ASE/calc_files_ase.py
+-rw-------   0 yamashita06   (501) staff       (20)     1156 2023-12-24 01:43:02.000000 csp_cryspy-1.2.5/src/cryspy/interface/ASE/collect_ase.py
+-rw-------   0 yamashita06   (501) staff       (20)     1838 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/interface/ASE/ctrl_job_ase.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.913103 csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      988 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/calc_files_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     1621 2023-11-17 03:46:18.000000 csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/collect_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2281 2023-11-17 03:46:25.000000 csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2955 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.914182 csp_cryspy-1.2.5/src/cryspy/interface/OMX/
+-rw-r--r--   0 yamashita06   (501) staff       (20)      886 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/OMX/calc_files_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2851 2023-11-17 03:46:43.000000 csp_cryspy-1.2.5/src/cryspy/interface/OMX/collect_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4616 2024-04-24 09:10:55.000000 csp_cryspy-1.2.5/src/cryspy/interface/OMX/ctrl_job_OMX.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3205 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/interface/OMX/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.915461 csp_cryspy-1.2.5/src/cryspy/interface/QE/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/interface/QE/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      836 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/QE/calc_files_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    11391 2023-11-17 03:47:37.000000 csp_cryspy-1.2.5/src/cryspy/interface/QE/collect_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4484 2024-04-24 08:59:19.000000 csp_cryspy-1.2.5/src/cryspy/interface/QE/ctrl_job_qe.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2945 2024-04-24 09:06:06.000000 csp_cryspy-1.2.5/src/cryspy/interface/QE/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.916551 csp_cryspy-1.2.5/src/cryspy/interface/VASP/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/interface/VASP/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      795 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/VASP/calc_files_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     9130 2023-11-17 03:50:43.000000 csp_cryspy-1.2.5/src/cryspy/interface/VASP/collect_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3606 2024-05-07 06:33:41.000000 csp_cryspy-1.2.5/src/cryspy/interface/VASP/ctrl_job_vasp.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/interface/__init__.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.917192 csp_cryspy-1.2.5/src/cryspy/interface/ext/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/interface/ext/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      513 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/ext/collect_ext.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     8681 2023-11-17 03:44:32.000000 csp_cryspy-1.2.5/src/cryspy/interface/select_code.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.918354 csp_cryspy-1.2.5/src/cryspy/interface/soiap/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        1 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/interface/soiap/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)      839 2023-07-10 10:34:05.000000 csp_cryspy-1.2.5/src/cryspy/interface/soiap/calc_files_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     7519 2023-11-17 03:50:43.000000 csp_cryspy-1.2.5/src/cryspy/interface/soiap/collect_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2358 2023-11-17 03:50:43.000000 csp_cryspy-1.2.5/src/cryspy/interface/soiap/ctrl_job_soiap.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     2416 2023-11-15 04:16:43.000000 csp_cryspy-1.2.5/src/cryspy/interface/soiap/structure.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.919006 csp_cryspy-1.2.5/src/cryspy/job/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/job/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    13495 2024-05-10 04:40:12.000000 csp_cryspy-1.2.5/src/cryspy/job/ctrl_ext.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    33247 2024-05-10 04:40:12.000000 csp_cryspy-1.2.5/src/cryspy/job/ctrl_job.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.920026 csp_cryspy-1.2.5/src/cryspy/scripts/
+-rw-------   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/scripts/__init__.py
+-rwx------   0 yamashita06   (501) staff       (20)     4416 2023-11-10 02:37:20.000000 csp_cryspy-1.2.5/src/cryspy/scripts/cryspy.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.921019 csp_cryspy-1.2.5/src/cryspy/start/
+-rw-r--r--   0 yamashita06   (501) staff       (20)        0 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/start/__init__.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     5544 2024-04-27 15:01:58.000000 csp_cryspy-1.2.5/src/cryspy/start/cryspy_init.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     4701 2024-04-27 20:49:23.000000 csp_cryspy-1.2.5/src/cryspy/start/cryspy_restart.py
+-rw-------   0 yamashita06   (501) staff       (20)     7376 2023-11-11 09:28:31.000000 csp_cryspy-1.2.5/src/cryspy/start/gen_init_struc.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.921861 csp_cryspy-1.2.5/src/cryspy/util/
+-rw-------   0 yamashita06   (501) staff       (20)      106 2023-03-16 12:21:45.000000 csp_cryspy-1.2.5/src/cryspy/util/constants.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)    15905 2023-11-11 04:14:25.000000 csp_cryspy-1.2.5/src/cryspy/util/struc_util.py
+-rw-r--r--   0 yamashita06   (501) staff       (20)     3825 2024-05-10 04:48:14.000000 csp_cryspy-1.2.5/src/cryspy/util/utility.py
+drwxr-xr-x   0 yamashita06   (501) staff       (20)        0 2024-05-10 04:58:33.922833 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/
+-rw-r--r--   0 yamashita06   (501) staff       (20)     6311 2024-05-10 04:58:33.000000 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/PKG-INFO
+-rw-------   0 yamashita06   (501) staff       (20)     3543 2024-05-10 04:58:33.000000 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/SOURCES.txt
+-rw-------   0 yamashita06   (501) staff       (20)        1 2024-05-10 04:58:33.000000 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/dependency_links.txt
+-rw-------   0 yamashita06   (501) staff       (20)       54 2024-05-10 04:58:33.000000 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/entry_points.txt
+-rw-------   0 yamashita06   (501) staff       (20)       14 2024-05-10 04:58:33.000000 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/requires.txt
+-rw-------   0 yamashita06   (501) staff       (20)        7 2024-05-10 04:58:33.000000 csp_cryspy-1.2.5/src/csp_cryspy.egg-info/top_level.txt
```

### Comparing `csp_cryspy-1.2.4/LICENSE` & `csp_cryspy-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/PKG-INFO` & `csp_cryspy-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csp-cryspy
-Version: 1.2.4
+Version: 1.2.5
 Summary: CrySPY is a crystal structure prediction tool written in Python.
 Author-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 Maintainer-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 License: MIT License
         
         Copyright (c) 2018 CrySPY Development Team
         
@@ -43,17 +43,19 @@
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
 Document: https://tomoki-yamashita.github.io/CrySPY_doc  
 Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.2.4 (2024 May 7)
+version 1.2.5 (2024 May 10)
 
 ## News
+- [2024 May 10] CrySPY 1.2.5 released.
+    + bug fix for order_ef in out_results.py
 - [2024 May 7] CrySPY 1.2.4 released.
     + bug fix
 - [2023 October 21] CrySPY 1.2.3 released.
     + bug fix for MPI
 - [2023 October 18] CrySPY 1.2.2 released.
     + [Enthalpy](https://tomoki-yamashita.github.io/CrySPY_doc/features/enthalpy/index.html)
 - [2023 September 27] CrySPY 1.2.1 released.
```

### Comparing `csp_cryspy-1.2.4/README.md` & `csp_cryspy-1.2.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
 Document: https://tomoki-yamashita.github.io/CrySPY_doc  
 Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.2.4 (2024 May 7)
+version 1.2.5 (2024 May 10)
 
 ## News
+- [2024 May 10] CrySPY 1.2.5 released.
+    + bug fix for order_ef in out_results.py
 - [2024 May 7] CrySPY 1.2.4 released.
     + bug fix
 - [2023 October 21] CrySPY 1.2.3 released.
     + bug fix for MPI
 - [2023 October 18] CrySPY 1.2.2 released.
     + [Enthalpy](https://tomoki-yamashita.github.io/CrySPY_doc/features/enthalpy/index.html)
 - [2023 September 27] CrySPY 1.2.1 released.
```

### Comparing `csp_cryspy-1.2.4/pyproject.toml` & `csp_cryspy-1.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/BO/bo_init.py` & `csp_cryspy-1.2.5/src/cryspy/BO/bo_init.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/BO/bo_next_select.py` & `csp_cryspy-1.2.5/src/cryspy/BO/bo_next_select.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/BO/bo_restart.py` & `csp_cryspy-1.2.5/src/cryspy/BO/bo_restart.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/BO/combo_cryspy.py` & `csp_cryspy-1.2.5/src/cryspy/BO/combo_cryspy.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/BO/select_descriptor.py` & `csp_cryspy-1.2.5/src/cryspy/BO/select_descriptor.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/calc_ef.py` & `csp_cryspy-1.2.5/src/cryspy/EA/calc_ef.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/calc_hull.py` & `csp_cryspy-1.2.5/src/cryspy/EA/calc_hull.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/ea_append.py` & `csp_cryspy-1.2.5/src/cryspy/EA/ea_append.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/ea_child.py` & `csp_cryspy-1.2.5/src/cryspy/EA/ea_child.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/ea_init.py` & `csp_cryspy-1.2.5/src/cryspy/EA/ea_init.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/ea_next_gen.py` & `csp_cryspy-1.2.5/src/cryspy/EA/ea_next_gen.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/addition.py` & `csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/addition.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/adj_comp.py` & `csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/adj_comp.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/crossover.py` & `csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/crossover.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/ea_generation.py` & `csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/ea_generation.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/elimination.py` & `csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/elimination.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/permutation.py` & `csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/permutation.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/rotation.py` & `csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/rotation.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/select_parents.py` & `csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/select_parents.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/strain.py` & `csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/strain.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/EA/gen_struc_EA/substitution.py` & `csp_cryspy-1.2.5/src/cryspy/EA/gen_struc_EA/substitution.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/IO/io_stat.py` & `csp_cryspy-1.2.5/src/cryspy/IO/io_stat.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/IO/out_results.py` & `csp_cryspy-1.2.5/src/cryspy/IO/out_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def out_rslt(rslt_data, order_ef=False):
     # ---------- asc in Struc_ID or (Gen or Select)
     with open('./data/cryspy_rslt', 'w') as f:
         f.write(rslt_data.to_string())
 
     # ---------- asc in energy
     with open('./data/cryspy_rslt_energy_asc', 'w') as f:
-        if order_ef:
+        if not order_ef:
             order = 'E_eV_atom'
         else:
             order = 'Ef_eV_atom'
         f.write(rslt_data.sort_values(
             by=[order], ascending=True).to_string())
```

### Comparing `csp_cryspy-1.2.4/src/cryspy/IO/pkl_data.py` & `csp_cryspy-1.2.5/src/cryspy/IO/pkl_data.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/IO/read_input.py` & `csp_cryspy-1.2.5/src/cryspy/IO/read_input.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/LAQA/calc_score.py` & `csp_cryspy-1.2.5/src/cryspy/LAQA/calc_score.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/LAQA/laqa_init.py` & `csp_cryspy-1.2.5/src/cryspy/LAQA/laqa_init.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/LAQA/laqa_next_selection.py` & `csp_cryspy-1.2.5/src/cryspy/LAQA/laqa_next_selection.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/LAQA/laqa_restart.py` & `csp_cryspy-1.2.5/src/cryspy/LAQA/laqa_restart.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py` & `csp_cryspy-1.2.5/src/cryspy/RS/gen_struc_RS/gen_pyxtal.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/RS/gen_struc_RS/random_generation.py` & `csp_cryspy-1.2.5/src/cryspy/RS/gen_struc_RS/random_generation.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/RS/rs_restart.py` & `csp_cryspy-1.2.5/src/cryspy/RS/rs_restart.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/calc_dscrpt/FP/calc_FP.py` & `csp_cryspy-1.2.5/src/cryspy/calc_dscrpt/FP/calc_FP.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interactive/action.py` & `csp_cryspy-1.2.5/src/cryspy/interactive/action.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interactive/energy_plot.py` & `csp_cryspy-1.2.5/src/cryspy/interactive/energy_plot.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interactive/restart_intract.py` & `csp_cryspy-1.2.5/src/cryspy/interactive/restart_intract.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/ASE/calc_files_ase.py` & `csp_cryspy-1.2.5/src/cryspy/interface/ASE/calc_files_ase.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/ASE/collect_ase.py` & `csp_cryspy-1.2.5/src/cryspy/interface/ASE/collect_ase.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/ASE/ctrl_job_ase.py` & `csp_cryspy-1.2.5/src/cryspy/interface/ASE/ctrl_job_ase.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/LAMMPS/calc_files_lammps.py` & `csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/calc_files_lammps.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/LAMMPS/collect_lammps.py` & `csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/collect_lammps.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py` & `csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/ctrl_job_lammps.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/LAMMPS/structure.py` & `csp_cryspy-1.2.5/src/cryspy/interface/LAMMPS/structure.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/OMX/calc_files_OMX.py` & `csp_cryspy-1.2.5/src/cryspy/interface/OMX/calc_files_OMX.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/OMX/collect_OMX.py` & `csp_cryspy-1.2.5/src/cryspy/interface/OMX/collect_OMX.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/OMX/ctrl_job_OMX.py` & `csp_cryspy-1.2.5/src/cryspy/interface/OMX/ctrl_job_OMX.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/OMX/structure.py` & `csp_cryspy-1.2.5/src/cryspy/interface/OMX/structure.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/QE/calc_files_qe.py` & `csp_cryspy-1.2.5/src/cryspy/interface/QE/calc_files_qe.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/QE/collect_qe.py` & `csp_cryspy-1.2.5/src/cryspy/interface/QE/collect_qe.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/QE/ctrl_job_qe.py` & `csp_cryspy-1.2.5/src/cryspy/interface/QE/ctrl_job_qe.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/QE/structure.py` & `csp_cryspy-1.2.5/src/cryspy/interface/QE/structure.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/VASP/calc_files_vasp.py` & `csp_cryspy-1.2.5/src/cryspy/interface/VASP/calc_files_vasp.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/VASP/collect_vasp.py` & `csp_cryspy-1.2.5/src/cryspy/interface/VASP/collect_vasp.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/VASP/ctrl_job_vasp.py` & `csp_cryspy-1.2.5/src/cryspy/interface/VASP/ctrl_job_vasp.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/ext/collect_ext.py` & `csp_cryspy-1.2.5/src/cryspy/interface/ext/collect_ext.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/select_code.py` & `csp_cryspy-1.2.5/src/cryspy/interface/select_code.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/soiap/calc_files_soiap.py` & `csp_cryspy-1.2.5/src/cryspy/interface/soiap/calc_files_soiap.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/soiap/collect_soiap.py` & `csp_cryspy-1.2.5/src/cryspy/interface/soiap/collect_soiap.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/soiap/ctrl_job_soiap.py` & `csp_cryspy-1.2.5/src/cryspy/interface/soiap/ctrl_job_soiap.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/interface/soiap/structure.py` & `csp_cryspy-1.2.5/src/cryspy/interface/soiap/structure.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/job/ctrl_ext.py` & `csp_cryspy-1.2.5/src/cryspy/job/ctrl_ext.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/job/ctrl_job.py` & `csp_cryspy-1.2.5/src/cryspy/job/ctrl_job.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/scripts/cryspy.py` & `csp_cryspy-1.2.5/src/cryspy/scripts/cryspy.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/start/cryspy_init.py` & `csp_cryspy-1.2.5/src/cryspy/start/cryspy_init.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/start/cryspy_restart.py` & `csp_cryspy-1.2.5/src/cryspy/start/cryspy_restart.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/start/gen_init_struc.py` & `csp_cryspy-1.2.5/src/cryspy/start/gen_init_struc.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/util/struc_util.py` & `csp_cryspy-1.2.5/src/cryspy/util/struc_util.py`

 * *Files identical despite different names*

### Comparing `csp_cryspy-1.2.4/src/cryspy/util/utility.py` & `csp_cryspy-1.2.5/src/cryspy/util/utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import subprocess
 import sys
 
 
 logger = getLogger('cryspy')
 
 def get_version():
-    return '1.2.4'
+    return '1.2.5'
 
 
 def set_logger(noprint=False, debug=False):
     # ---------- level and formatter
     logger.setLevel(DEBUG)
     fmt = Formatter("[%(asctime)s][%(module)s][%(levelname)s] %(message)s")
```

### Comparing `csp_cryspy-1.2.4/src/csp_cryspy.egg-info/PKG-INFO` & `csp_cryspy-1.2.5/src/csp_cryspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csp-cryspy
-Version: 1.2.4
+Version: 1.2.5
 Summary: CrySPY is a crystal structure prediction tool written in Python.
 Author-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 Maintainer-email: Tomoki Yamashita <yamashita06@vos.nagaokaut.ac.jp>
 License: MIT License
         
         Copyright (c) 2018 CrySPY Development Team
         
@@ -43,17 +43,19 @@
 
 # CrySPY
 CrySPY (pronounced as crispy) is a crystal structure prediction tool written in Python.  
 Document: https://tomoki-yamashita.github.io/CrySPY_doc  
 Questions and comments: https://github.com/Tomoki-YAMASHITA/CrySPY/discussions
 
 ## Latest version
-version 1.2.4 (2024 May 7)
+version 1.2.5 (2024 May 10)
 
 ## News
+- [2024 May 10] CrySPY 1.2.5 released.
+    + bug fix for order_ef in out_results.py
 - [2024 May 7] CrySPY 1.2.4 released.
     + bug fix
 - [2023 October 21] CrySPY 1.2.3 released.
     + bug fix for MPI
 - [2023 October 18] CrySPY 1.2.2 released.
     + [Enthalpy](https://tomoki-yamashita.github.io/CrySPY_doc/features/enthalpy/index.html)
 - [2023 September 27] CrySPY 1.2.1 released.
```

### Comparing `csp_cryspy-1.2.4/src/csp_cryspy.egg-info/SOURCES.txt` & `csp_cryspy-1.2.5/src/csp_cryspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

