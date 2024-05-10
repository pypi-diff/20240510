# Comparing `tmp/cspdk-0.8.0.tar.gz` & `tmp/cspdk-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cspdk-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cspdk-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cspdk-0.8.0.tar` & `cspdk-0.8.1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0     1077 2024-05-04 23:51:20.740936 cspdk-0.8.0/LICENSE
--rw-r--r--   0        0        0     1178 2024-05-04 23:51:20.740936 cspdk-0.8.0/README.md
--rw-r--r--   0        0        0       22 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/__init__.py
--rw-r--r--   0        0        0      971 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/__init__.py
--rw-r--r--   0        0        0    40171 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/cells.py
--rw-r--r--   0        0        0      474 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/config.py
--rw-r--r--   0        0        0    90112 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/CORNERSTONE MPW SOI 220nm GDSII Template.gds
--rw-r--r--   0        0        0      192 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Cell0_Institution_Name.gds
--rw-r--r--   0        0        0    27216 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Cell0_SOI220_Full_1550nm_Packaging_Template.gds
--rw-r--r--   0        0        0      202 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Cell0_SOI_Full_Institution_Name.gds
--rw-r--r--   0        0        0      202 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Cell0_SOI_Half_Institution_Name.gds
--rw-r--r--   0        0        0     1156 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Flip_Chip_Bonding_Example.gds
--rw-r--r--   0        0        0      688 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Heater.gds
--rw-r--r--   0        0        0    20356 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/Layer_Designations.gds
--rw-r--r--   0        0        0      504 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_2x1_MMI.gds
--rw-r--r--   0        0        0      872 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_2x2_MMI.gds
--rw-r--r--   0        0        0     2240 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_90_Degree_Bend.gds
--rw-r--r--   0        0        0     5472 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Grating_Coupler.gds
--rw-r--r--   0        0        0      266 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Waveguide.gds
--rw-r--r--   0        0        0     1108 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Waveguide_Crossing.gds
--rw-r--r--   0        0        0      586 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_2x1_MMI.gds
--rw-r--r--   0        0        0      714 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_2x2_MMI.gds
--rw-r--r--   0        0        0      650 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_90_Degree_Bend.gds
--rw-r--r--   0        0        0     5394 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Grating_Coupler.gds
--rw-r--r--   0        0        0      204 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Waveguide.gds
--rw-r--r--   0        0        0      726 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Waveguide_Crossing.gds
--rw-r--r--   0        0        0      744 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_2x1_MMI.gds
--rw-r--r--   0        0        0      872 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_2x2_MMI.gds
--rw-r--r--   0        0        0     2272 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_90_Degree_Bend.gds
--rw-r--r--   0        0        0     4192 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Grating_Coupler.gds
--rw-r--r--   0        0        0      266 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Waveguide.gds
--rw-r--r--   0        0        0     1108 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Waveguide_Crossing.gds
--rw-r--r--   0        0        0      586 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_2x1_MMI.gds
--rw-r--r--   0        0        0      714 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_2x2_MMI.gds
--rw-r--r--   0        0        0      650 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_90_Degree_Bend.gds
--rw-r--r--   0        0        0      204 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_Waveguide.gds
--rw-r--r--   0        0        0      854 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_Waveguide_Crossing.gds
--rw-r--r--   0        0        0      217 2024-05-04 23:51:20.740936 cspdk-0.8.0/cspdk/si220/import_pdk.py
--rw-r--r--   0        0        0     1004 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/klayout/d25/Cornerstone.lyd25
--rw-r--r--   0        0        0      809 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/klayout/d25/Cornerstone_si220.lyd25
--rw-r--r--   0        0        0     4201 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/klayout/layers.lyp
--rw-r--r--   0        0        0     5740 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/klayout/tech.lyt
--rw-r--r--   0        0        0     1051 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/layers.yaml
--rw-r--r--   0        0        0     5823 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/models.py
--rw-r--r--   0        0        0      589 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/samples/circuit_simulations_sc.py
--rw-r--r--   0        0        0      929 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/samples/circuit_simulations_sc_with_routing.py
--rw-r--r--   0        0        0      825 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/samples/component_from_yaml_sc.py
--rw-r--r--   0        0        0      416 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/samples/get_route_sc.py
--rw-r--r--   0        0        0      736 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/samples/mode_solver_r.py
--rw-r--r--   0        0        0      733 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/samples/mode_solver_s.py
--rw-r--r--   0        0        0     6987 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si220/tech.py
--rw-r--r--   0        0        0      971 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/__init__.py
--rw-r--r--   0        0        0    19676 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/cells.py
--rw-r--r--   0        0        0      474 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/config.py
--rw-r--r--   0        0        0      217 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/import_pdk.py
--rw-r--r--   0        0        0     1004 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/klayout/d25/Cornerstone.lyd25
--rw-r--r--   0        0        0      809 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/klayout/d25/Cornerstone_si220.lyd25
--rw-r--r--   0        0        0     4201 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/klayout/layers.lyp
--rw-r--r--   0        0        0     5740 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/klayout/tech.lyt
--rw-r--r--   0        0        0     1051 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/layers.yaml
--rw-r--r--   0        0        0     5823 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/models.py
--rw-r--r--   0        0        0      589 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/samples/circuit_simulations_rc500.py
--rw-r--r--   0        0        0      929 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/samples/circuit_simulations_rc500_with_routing.py
--rw-r--r--   0        0        0      825 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/samples/component_from_yaml_rc500.py
--rw-r--r--   0        0        0      416 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/samples/get_route_rc500.py
--rw-r--r--   0        0        0      734 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/samples/mode_solver_r500.py
--rw-r--r--   0        0        0     4853 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/si500/tech.py
--rw-r--r--   0        0        0      977 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/__init__.py
--rw-r--r--   0        0        0    27490 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/cells.py
--rw-r--r--   0        0        0      474 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/config.py
--rw-r--r--   0        0        0    90112 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/CORNERSTONE MPW SOI 220nm GDSII Template.gds
--rw-r--r--   0        0        0      192 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Cell0_Institution_Name.gds
--rw-r--r--   0        0        0    27216 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Cell0_SOI220_Full_1550nm_Packaging_Template.gds
--rw-r--r--   0        0        0      202 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Cell0_SOI_Full_Institution_Name.gds
--rw-r--r--   0        0        0      202 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Cell0_SOI_Half_Institution_Name.gds
--rw-r--r--   0        0        0     1156 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Flip_Chip_Bonding_Example.gds
--rw-r--r--   0        0        0      688 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Heater.gds
--rw-r--r--   0        0        0    20356 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/Layer_Designations.gds
--rw-r--r--   0        0        0      504 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_2x1_MMI.gds
--rw-r--r--   0        0        0      872 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_2x2_MMI.gds
--rw-r--r--   0        0        0     2240 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_90_Degree_Bend.gds
--rw-r--r--   0        0        0     5472 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_Grating_Coupler.gds
--rw-r--r--   0        0        0      266 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_Waveguide.gds
--rw-r--r--   0        0        0     1108 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_Waveguide_Crossing.gds
--rw-r--r--   0        0        0      586 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_2x1_MMI.gds
--rw-r--r--   0        0        0      714 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_2x2_MMI.gds
--rw-r--r--   0        0        0      650 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_90_Degree_Bend.gds
--rw-r--r--   0        0        0     5394 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_Grating_Coupler.gds
--rw-r--r--   0        0        0      204 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_Waveguide.gds
--rw-r--r--   0        0        0      726 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_Waveguide_Crossing.gds
--rw-r--r--   0        0        0      744 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_2x1_MMI.gds
--rw-r--r--   0        0        0      872 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_2x2_MMI.gds
--rw-r--r--   0        0        0     2272 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_90_Degree_Bend.gds
--rw-r--r--   0        0        0     4192 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_Grating_Coupler.gds
--rw-r--r--   0        0        0      266 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_Waveguide.gds
--rw-r--r--   0        0        0     1108 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_Waveguide_Crossing.gds
--rw-r--r--   0        0        0      586 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_2x1_MMI.gds
--rw-r--r--   0        0        0      714 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_2x2_MMI.gds
--rw-r--r--   0        0        0      650 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_90_Degree_Bend.gds
--rw-r--r--   0        0        0      204 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_Waveguide.gds
--rw-r--r--   0        0        0      854 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_Waveguide_Crossing.gds
--rw-r--r--   0        0        0      394 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_2x1_MMI.gds
--rw-r--r--   0        0        0      458 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_2x2_MMI.gds
--rw-r--r--   0        0        0     1626 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_90_Degr.gds
--rw-r--r--   0        0        0     2570 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_Grating.gds
--rw-r--r--   0        0        0      202 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_Wavegui.gds
--rw-r--r--   0        0        0      650 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_2x1_MMI.gds
--rw-r--r--   0        0        0      458 2024-05-04 23:51:20.744936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_2x2_MMI.gds
--rw-r--r--   0        0        0     1626 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_90_Degr.gds
--rw-r--r--   0        0        0     1674 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_Grating.gds
--rw-r--r--   0        0        0      202 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_Wavegui.gds
--rw-r--r--   0        0        0      211 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/import_pdk.py
--rw-r--r--   0        0        0     1004 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/klayout/d25/Cornerstone.lyd25
--rw-r--r--   0        0        0      852 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/klayout/d25/Cornerstone_sin300.lyd25
--rw-r--r--   0        0        0     3295 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/klayout/layers.lyp
--rw-r--r--   0        0        0     5741 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/klayout/tech.lyt
--rw-r--r--   0        0        0      800 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/layers.yaml
--rw-r--r--   0        0        0     3711 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/models.py
--rw-r--r--   0        0        0      590 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/samples/circuit_simulations_nc.py
--rw-r--r--   0        0        0      930 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/samples/circuit_simulations_nc_with_routing.py
--rw-r--r--   0        0        0      826 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/samples/component_from_yaml_nc.py
--rw-r--r--   0        0        0      417 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/samples/get_route_nc.py
--rw-r--r--   0        0        0      733 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/samples/mode_solver_n.py
--rw-r--r--   0        0        0     5441 2024-05-04 23:51:20.748936 cspdk-0.8.0/cspdk/sin300/tech.py
--rw-r--r--   0        0        0     2270 2024-05-04 23:51:20.748936 cspdk-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 cspdk-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-10 16:26:58.361097 cspdk-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1178 2024-05-10 16:26:58.361097 cspdk-0.8.1/README.md
+-rw-r--r--   0        0        0       22 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/__init__.py
+-rw-r--r--   0        0        0      971 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/__init__.py
+-rw-r--r--   0        0        0    40171 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/cells.py
+-rw-r--r--   0        0        0      474 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/config.py
+-rw-r--r--   0        0        0    90112 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/CORNERSTONE MPW SOI 220nm GDSII Template.gds
+-rw-r--r--   0        0        0      192 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/Cell0_Institution_Name.gds
+-rw-r--r--   0        0        0    27216 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/Cell0_SOI220_Full_1550nm_Packaging_Template.gds
+-rw-r--r--   0        0        0      202 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/Cell0_SOI_Full_Institution_Name.gds
+-rw-r--r--   0        0        0      202 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/Cell0_SOI_Half_Institution_Name.gds
+-rw-r--r--   0        0        0     1156 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/Flip_Chip_Bonding_Example.gds
+-rw-r--r--   0        0        0      688 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/Heater.gds
+-rw-r--r--   0        0        0    20356 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/Layer_Designations.gds
+-rw-r--r--   0        0        0      504 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_2x1_MMI.gds
+-rw-r--r--   0        0        0      872 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_2x2_MMI.gds
+-rw-r--r--   0        0        0     2240 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_90_Degree_Bend.gds
+-rw-r--r--   0        0        0     5472 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Grating_Coupler.gds
+-rw-r--r--   0        0        0      266 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Waveguide.gds
+-rw-r--r--   0        0        0     1108 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      586 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_2x1_MMI.gds
+-rw-r--r--   0        0        0      714 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_2x2_MMI.gds
+-rw-r--r--   0        0        0      650 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_90_Degree_Bend.gds
+-rw-r--r--   0        0        0     5394 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Grating_Coupler.gds
+-rw-r--r--   0        0        0      204 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Waveguide.gds
+-rw-r--r--   0        0        0      726 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      744 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_2x1_MMI.gds
+-rw-r--r--   0        0        0      872 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_2x2_MMI.gds
+-rw-r--r--   0        0        0     2272 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_90_Degree_Bend.gds
+-rw-r--r--   0        0        0     4192 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Grating_Coupler.gds
+-rw-r--r--   0        0        0      266 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Waveguide.gds
+-rw-r--r--   0        0        0     1108 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      586 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_2x1_MMI.gds
+-rw-r--r--   0        0        0      714 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_2x2_MMI.gds
+-rw-r--r--   0        0        0      650 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_90_Degree_Bend.gds
+-rw-r--r--   0        0        0      204 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_Waveguide.gds
+-rw-r--r--   0        0        0      854 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      217 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/import_pdk.py
+-rw-r--r--   0        0        0     1004 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/klayout/d25/Cornerstone.lyd25
+-rw-r--r--   0        0        0      809 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/klayout/d25/Cornerstone_si220.lyd25
+-rw-r--r--   0        0        0     4201 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/klayout/layers.lyp
+-rw-r--r--   0        0        0     5740 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/klayout/tech.lyt
+-rw-r--r--   0        0        0     1051 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/layers.yaml
+-rw-r--r--   0        0        0     5823 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/models.py
+-rw-r--r--   0        0        0      589 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/samples/circuit_simulations_sc.py
+-rw-r--r--   0        0        0      929 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/samples/circuit_simulations_sc_with_routing.py
+-rw-r--r--   0        0        0      825 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/samples/component_from_yaml_sc.py
+-rw-r--r--   0        0        0      416 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/samples/get_route_sc.py
+-rw-r--r--   0        0        0      736 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/samples/mode_solver_r.py
+-rw-r--r--   0        0        0      733 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/samples/mode_solver_s.py
+-rw-r--r--   0        0        0     6987 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si220/tech.py
+-rw-r--r--   0        0        0      971 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si500/__init__.py
+-rw-r--r--   0        0        0    19676 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si500/cells.py
+-rw-r--r--   0        0        0      474 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si500/config.py
+-rw-r--r--   0        0        0      217 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si500/import_pdk.py
+-rw-r--r--   0        0        0     1004 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si500/klayout/d25/Cornerstone.lyd25
+-rw-r--r--   0        0        0      809 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si500/klayout/d25/Cornerstone_si220.lyd25
+-rw-r--r--   0        0        0     4201 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si500/klayout/layers.lyp
+-rw-r--r--   0        0        0     5740 2024-05-10 16:26:58.361097 cspdk-0.8.1/cspdk/si500/klayout/tech.lyt
+-rw-r--r--   0        0        0     1051 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/si500/layers.yaml
+-rw-r--r--   0        0        0     5823 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/si500/models.py
+-rw-r--r--   0        0        0      589 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/si500/samples/circuit_simulations_rc500.py
+-rw-r--r--   0        0        0      929 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/si500/samples/circuit_simulations_rc500_with_routing.py
+-rw-r--r--   0        0        0      825 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/si500/samples/component_from_yaml_rc500.py
+-rw-r--r--   0        0        0      416 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/si500/samples/get_route_rc500.py
+-rw-r--r--   0        0        0      734 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/si500/samples/mode_solver_r500.py
+-rw-r--r--   0        0        0     4853 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/si500/tech.py
+-rw-r--r--   0        0        0      977 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/__init__.py
+-rw-r--r--   0        0        0    27490 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/cells.py
+-rw-r--r--   0        0        0      474 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/config.py
+-rw-r--r--   0        0        0    90112 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/CORNERSTONE MPW SOI 220nm GDSII Template.gds
+-rw-r--r--   0        0        0      192 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/Cell0_Institution_Name.gds
+-rw-r--r--   0        0        0    27216 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/Cell0_SOI220_Full_1550nm_Packaging_Template.gds
+-rw-r--r--   0        0        0      202 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/Cell0_SOI_Full_Institution_Name.gds
+-rw-r--r--   0        0        0      202 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/Cell0_SOI_Half_Institution_Name.gds
+-rw-r--r--   0        0        0     1156 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/Flip_Chip_Bonding_Example.gds
+-rw-r--r--   0        0        0      688 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/Heater.gds
+-rw-r--r--   0        0        0    20356 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/Layer_Designations.gds
+-rw-r--r--   0        0        0      504 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_2x1_MMI.gds
+-rw-r--r--   0        0        0      872 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_2x2_MMI.gds
+-rw-r--r--   0        0        0     2240 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_90_Degree_Bend.gds
+-rw-r--r--   0        0        0     5472 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_Grating_Coupler.gds
+-rw-r--r--   0        0        0      266 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_Waveguide.gds
+-rw-r--r--   0        0        0     1108 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      586 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_2x1_MMI.gds
+-rw-r--r--   0        0        0      714 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_2x2_MMI.gds
+-rw-r--r--   0        0        0      650 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_90_Degree_Bend.gds
+-rw-r--r--   0        0        0     5394 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_Grating_Coupler.gds
+-rw-r--r--   0        0        0      204 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_Waveguide.gds
+-rw-r--r--   0        0        0      726 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      744 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_2x1_MMI.gds
+-rw-r--r--   0        0        0      872 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_2x2_MMI.gds
+-rw-r--r--   0        0        0     2272 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_90_Degree_Bend.gds
+-rw-r--r--   0        0        0     4192 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_Grating_Coupler.gds
+-rw-r--r--   0        0        0      266 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_Waveguide.gds
+-rw-r--r--   0        0        0     1108 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      586 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_2x1_MMI.gds
+-rw-r--r--   0        0        0      714 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_2x2_MMI.gds
+-rw-r--r--   0        0        0      650 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_90_Degree_Bend.gds
+-rw-r--r--   0        0        0      204 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_Waveguide.gds
+-rw-r--r--   0        0        0      854 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_Waveguide_Crossing.gds
+-rw-r--r--   0        0        0      394 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_2x1_MMI.gds
+-rw-r--r--   0        0        0      458 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_2x2_MMI.gds
+-rw-r--r--   0        0        0     1626 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_90_Degr.gds
+-rw-r--r--   0        0        0     2570 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_Grating.gds
+-rw-r--r--   0        0        0      202 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_Wavegui.gds
+-rw-r--r--   0        0        0      650 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_2x1_MMI.gds
+-rw-r--r--   0        0        0      458 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_2x2_MMI.gds
+-rw-r--r--   0        0        0     1626 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_90_Degr.gds
+-rw-r--r--   0        0        0     1674 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_Grating.gds
+-rw-r--r--   0        0        0      202 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_Wavegui.gds
+-rw-r--r--   0        0        0      211 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/import_pdk.py
+-rw-r--r--   0        0        0     1004 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/klayout/d25/Cornerstone.lyd25
+-rw-r--r--   0        0        0      852 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/klayout/d25/Cornerstone_sin300.lyd25
+-rw-r--r--   0        0        0     3295 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/klayout/layers.lyp
+-rw-r--r--   0        0        0     5741 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/klayout/tech.lyt
+-rw-r--r--   0        0        0      800 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/layers.yaml
+-rw-r--r--   0        0        0     3711 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/models.py
+-rw-r--r--   0        0        0      590 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/samples/circuit_simulations_nc.py
+-rw-r--r--   0        0        0      930 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/samples/circuit_simulations_nc_with_routing.py
+-rw-r--r--   0        0        0      826 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/samples/component_from_yaml_nc.py
+-rw-r--r--   0        0        0      417 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/samples/get_route_nc.py
+-rw-r--r--   0        0        0      733 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/samples/mode_solver_n.py
+-rw-r--r--   0        0        0     5441 2024-05-10 16:26:58.365097 cspdk-0.8.1/cspdk/sin300/tech.py
+-rw-r--r--   0        0        0     2270 2024-05-10 16:26:58.369097 cspdk-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 cspdk-0.8.1/PKG-INFO
```

### Comparing `cspdk-0.8.0/LICENSE` & `cspdk-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/README.md` & `cspdk-0.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CornerStone PDK 0.8.0
+# CornerStone PDK 0.8.1
 
 ![](https://i.imgur.com/V5Ukc6j.png)
 
 [CornerStone](https://www.cornerstone.sotonfab.co.uk/) Photonics PDK.
 
 ## Installation
```

### Comparing `cspdk-0.8.0/cspdk/si220/__init__.py` & `cspdk-0.8.1/cspdk/si220/__init__.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/cells.py` & `cspdk-0.8.1/cspdk/si220/cells.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/CORNERSTONE MPW SOI 220nm GDSII Template.gds` & `cspdk-0.8.1/cspdk/si220/gds/CORNERSTONE MPW SOI 220nm GDSII Template.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/Cell0_SOI220_Full_1550nm_Packaging_Template.gds` & `cspdk-0.8.1/cspdk/si220/gds/Cell0_SOI220_Full_1550nm_Packaging_Template.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/Flip_Chip_Bonding_Example.gds` & `cspdk-0.8.1/cspdk/si220/gds/Flip_Chip_Bonding_Example.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/Heater.gds` & `cspdk-0.8.1/cspdk/si220/gds/Heater.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/Layer_Designations.gds` & `cspdk-0.8.1/cspdk/si220/gds/Layer_Designations.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_2x2_MMI.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_2x2_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_90_Degree_Bend.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_90_Degree_Bend.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Grating_Coupler.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Grating_Coupler.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Waveguide_Crossing.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_RIB_Waveguide_Crossing.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_2x1_MMI.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_2x1_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_2x2_MMI.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_2x2_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_90_Degree_Bend.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_90_Degree_Bend.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Grating_Coupler.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Grating_Coupler.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Waveguide_Crossing.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1310nm_TE_STRIP_Waveguide_Crossing.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_2x1_MMI.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_2x1_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_2x2_MMI.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_2x2_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_90_Degree_Bend.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_90_Degree_Bend.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Grating_Coupler.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Grating_Coupler.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Waveguide_Crossing.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_RIB_Waveguide_Crossing.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_2x1_MMI.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_2x1_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_2x2_MMI.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_2x2_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_90_Degree_Bend.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_90_Degree_Bend.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_Waveguide_Crossing.gds` & `cspdk-0.8.1/cspdk/si220/gds/SOI220nm_1550nm_TE_STRIP_Waveguide_Crossing.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/klayout/d25/Cornerstone.lyd25` & `cspdk-0.8.1/cspdk/si220/klayout/d25/Cornerstone.lyd25`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/klayout/d25/Cornerstone_si220.lyd25` & `cspdk-0.8.1/cspdk/si220/klayout/d25/Cornerstone_si220.lyd25`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/klayout/layers.lyp` & `cspdk-0.8.1/cspdk/si220/klayout/layers.lyp`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/klayout/tech.lyt` & `cspdk-0.8.1/cspdk/si220/klayout/tech.lyt`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/layers.yaml` & `cspdk-0.8.1/cspdk/si220/layers.yaml`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/models.py` & `cspdk-0.8.1/cspdk/si220/models.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/samples/circuit_simulations_sc.py` & `cspdk-0.8.1/cspdk/si220/samples/circuit_simulations_sc.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/samples/circuit_simulations_sc_with_routing.py` & `cspdk-0.8.1/cspdk/si220/samples/circuit_simulations_sc_with_routing.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/samples/component_from_yaml_sc.py` & `cspdk-0.8.1/cspdk/si220/samples/component_from_yaml_sc.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/samples/mode_solver_r.py` & `cspdk-0.8.1/cspdk/si220/samples/mode_solver_r.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/samples/mode_solver_s.py` & `cspdk-0.8.1/cspdk/si220/samples/mode_solver_s.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si220/tech.py` & `cspdk-0.8.1/cspdk/si220/tech.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si500/__init__.py` & `cspdk-0.8.1/cspdk/si500/__init__.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si500/cells.py` & `cspdk-0.8.1/cspdk/si500/cells.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si500/klayout/d25/Cornerstone.lyd25` & `cspdk-0.8.1/cspdk/si500/klayout/d25/Cornerstone.lyd25`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si500/klayout/d25/Cornerstone_si220.lyd25` & `cspdk-0.8.1/cspdk/si500/klayout/d25/Cornerstone_si220.lyd25`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si500/klayout/layers.lyp` & `cspdk-0.8.1/cspdk/si500/klayout/layers.lyp`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si500/klayout/tech.lyt` & `cspdk-0.8.1/cspdk/si500/klayout/tech.lyt`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si500/layers.yaml` & `cspdk-0.8.1/cspdk/si500/layers.yaml`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si500/models.py` & `cspdk-0.8.1/cspdk/si500/models.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si500/samples/circuit_simulations_rc500.py` & `cspdk-0.8.1/cspdk/si500/samples/circuit_simulations_rc500.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si500/samples/circuit_simulations_rc500_with_routing.py` & `cspdk-0.8.1/cspdk/si500/samples/circuit_simulations_rc500_with_routing.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si500/samples/component_from_yaml_rc500.py` & `cspdk-0.8.1/cspdk/si500/samples/component_from_yaml_rc500.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si500/samples/mode_solver_r500.py` & `cspdk-0.8.1/cspdk/si500/samples/mode_solver_r500.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/si500/tech.py` & `cspdk-0.8.1/cspdk/si500/tech.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/__init__.py` & `cspdk-0.8.1/cspdk/sin300/__init__.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/cells.py` & `cspdk-0.8.1/cspdk/sin300/cells.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/CORNERSTONE MPW SOI 220nm GDSII Template.gds` & `cspdk-0.8.1/cspdk/sin300/gds/CORNERSTONE MPW SOI 220nm GDSII Template.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/Cell0_SOI220_Full_1550nm_Packaging_Template.gds` & `cspdk-0.8.1/cspdk/sin300/gds/Cell0_SOI220_Full_1550nm_Packaging_Template.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/Flip_Chip_Bonding_Example.gds` & `cspdk-0.8.1/cspdk/sin300/gds/Flip_Chip_Bonding_Example.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/Heater.gds` & `cspdk-0.8.1/cspdk/sin300/gds/Heater.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/Layer_Designations.gds` & `cspdk-0.8.1/cspdk/sin300/gds/Layer_Designations.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_2x2_MMI.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_2x2_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_90_Degree_Bend.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_90_Degree_Bend.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_Grating_Coupler.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_Grating_Coupler.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_Waveguide_Crossing.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_RIB_Waveguide_Crossing.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_2x1_MMI.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_2x1_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_2x2_MMI.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_2x2_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_90_Degree_Bend.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_90_Degree_Bend.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_Grating_Coupler.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_Grating_Coupler.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_Waveguide_Crossing.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1310nm_TE_STRIP_Waveguide_Crossing.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_2x1_MMI.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_2x1_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_2x2_MMI.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_2x2_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_90_Degree_Bend.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_90_Degree_Bend.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_Grating_Coupler.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_Grating_Coupler.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_Waveguide_Crossing.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_RIB_Waveguide_Crossing.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_2x1_MMI.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_2x1_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_2x2_MMI.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_2x2_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_90_Degree_Bend.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_90_Degree_Bend.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_Waveguide_Crossing.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SOI220nm_1550nm_TE_STRIP_Waveguide_Crossing.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_90_Degr.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_90_Degr.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_Grating.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1310nm_TE_STRIP_Grating.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_2x1_MMI.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_2x1_MMI.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_90_Degr.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_90_Degr.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_Grating.gds` & `cspdk-0.8.1/cspdk/sin300/gds/SiN300nm_1550nm_TE_STRIP_Grating.gds`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/klayout/d25/Cornerstone.lyd25` & `cspdk-0.8.1/cspdk/sin300/klayout/d25/Cornerstone.lyd25`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/klayout/d25/Cornerstone_sin300.lyd25` & `cspdk-0.8.1/cspdk/sin300/klayout/d25/Cornerstone_sin300.lyd25`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/klayout/layers.lyp` & `cspdk-0.8.1/cspdk/sin300/klayout/layers.lyp`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/klayout/tech.lyt` & `cspdk-0.8.1/cspdk/sin300/klayout/tech.lyt`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/layers.yaml` & `cspdk-0.8.1/cspdk/sin300/layers.yaml`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/models.py` & `cspdk-0.8.1/cspdk/sin300/models.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/samples/circuit_simulations_nc.py` & `cspdk-0.8.1/cspdk/sin300/samples/circuit_simulations_nc.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/samples/circuit_simulations_nc_with_routing.py` & `cspdk-0.8.1/cspdk/sin300/samples/circuit_simulations_nc_with_routing.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/samples/component_from_yaml_nc.py` & `cspdk-0.8.1/cspdk/sin300/samples/component_from_yaml_nc.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/samples/mode_solver_n.py` & `cspdk-0.8.1/cspdk/sin300/samples/mode_solver_n.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/cspdk/sin300/tech.py` & `cspdk-0.8.1/cspdk/sin300/tech.py`

 * *Files identical despite different names*

### Comparing `cspdk-0.8.0/pyproject.toml` & `cspdk-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 ]
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: OS Independent"
 ]
 dependencies = [
-  "gdsfactory==7.25.1",
+  "gdsfactory==7.26.1",
   "gplugins[sax]>=0.13,<0.14"
 ]
 description = "CornerStone PDK"
 keywords = ["python"]
 license = {file = "LICENSE"}
 name = "cspdk"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.8.0"
+version = "0.8.1"
 
 [project.optional-dependencies]
 dev = [
   "pre-commit",
   "pytest",
   "pytest-cov",
   "pytest_regressions"
@@ -97,15 +97,15 @@
 src = "cspdk/__init__.py"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [tool.tbump.version]
-current = "0.8.0"
+current = "0.8.1"
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `cspdk-0.8.0/PKG-INFO` & `cspdk-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: cspdk
-Version: 0.8.0
+Version: 0.8.1
 Summary: CornerStone PDK
 Keywords: python
 Author-email: gdsfactory <contact@gdsfactory.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Dist: gdsfactory==7.25.1
+Requires-Dist: gdsfactory==7.26.1
 Requires-Dist: gplugins[sax]>=0.13,<0.14
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest_regressions ; extra == "dev"
 Requires-Dist: jupytext ; extra == "docs"
 Requires-Dist: matplotlib ; extra == "docs"
 Requires-Dist: jupyter-book==1.0.0 ; extra == "docs"
 Provides-Extra: dev
 Provides-Extra: docs
 
-# CornerStone PDK 0.8.0
+# CornerStone PDK 0.8.1
 
 ![](https://i.imgur.com/V5Ukc6j.png)
 
 [CornerStone](https://www.cornerstone.sotonfab.co.uk/) Photonics PDK.
 
 ## Installation
```

