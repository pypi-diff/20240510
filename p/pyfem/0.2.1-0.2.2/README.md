# Comparing `tmp/pyfem-0.2.1.tar.gz` & `tmp/pyfem-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.2.1.tar", last modified: Mon Apr 22 08:34:00 2024, max compression
+gzip compressed data, was "pyfem-0.2.2.tar", last modified: Fri May 10 04:00:01 2024, max compression
```

## Comparing `pyfem-0.2.1.tar` & `pyfem-0.2.2.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 08:34:00.221618 pyfem-0.2.1/
--rw-rw-rw-   0        0        0     1190 2024-04-22 05:18:42.000000 pyfem-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     3686 2024-04-22 08:34:00.220623 pyfem-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-22 08:34:00.221618 pyfem-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1115 2023-08-17 09:47:32.000000 pyfem-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.625612 pyfem-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.634595 pyfem-0.2.1/src/pyfem/
--rw-rw-rw-   0        0        0     2804 2023-11-01 09:09:41.000000 pyfem-0.2.1/src/pyfem/Job.py
--rw-rw-rw-   0        0        0       23 2024-04-22 08:32:37.000000 pyfem-0.2.1/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0     1388 2023-11-02 07:31:58.000000 pyfem-0.2.1/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.687406 pyfem-0.2.1/src/pyfem/amplitude/
--rw-rw-rw-   0        0        0     1403 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/amplitude/BaseAmplitude.py
--rw-rw-rw-   0        0        0     1892 2023-11-02 07:24:23.000000 pyfem-0.2.1/src/pyfem/amplitude/TabularAmplitude.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/amplitude/__init__.py
--rw-rw-rw-   0        0        0     1112 2023-11-02 07:24:12.000000 pyfem-0.2.1/src/pyfem/amplitude/get_amplitude_data.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.690396 pyfem-0.2.1/src/pyfem/assembly/
--rw-rw-rw-   0        0        0    14782 2024-04-18 07:46:32.000000 pyfem-0.2.1/src/pyfem/assembly/Assembly.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.747204 pyfem-0.2.1/src/pyfem/bc/
--rw-rw-rw-   0        0        0     4148 2024-04-15 03:43:05.000000 pyfem-0.2.1/src/pyfem/bc/BaseBC.py
--rw-rw-rw-   0        0        0     3003 2024-04-18 05:44:17.000000 pyfem-0.2.1/src/pyfem/bc/DirichletBC.py
--rw-rw-rw-   0        0        0     2984 2024-04-18 05:43:15.000000 pyfem-0.2.1/src/pyfem/bc/NeumannBCConcentrated.py
--rw-rw-rw-   0        0        0    27073 2024-04-18 05:15:08.000000 pyfem-0.2.1/src/pyfem/bc/NeumannBCDistributed.py
--rw-rw-rw-   0        0        0    13073 2024-04-18 07:30:11.000000 pyfem-0.2.1/src/pyfem/bc/NeumannBCPressure.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/bc/__init__.py
--rw-rw-rw-   0        0        0     1049 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/bc/derive_surface_integral.py
--rw-rw-rw-   0        0        0     2087 2023-11-02 07:24:23.000000 pyfem-0.2.1/src/pyfem/bc/get_bc_data.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.770208 pyfem-0.2.1/src/pyfem/elements/
--rw-rw-rw-   0        0        0    20958 2024-04-22 08:22:10.000000 pyfem-0.2.1/src/pyfem/elements/BaseElement.py
--rw-rw-rw-   0        0        0    10270 2024-04-22 06:34:05.000000 pyfem-0.2.1/src/pyfem/elements/Diffusion.py
--rw-rw-rw-   0        0        0    76446 2024-01-17 03:37:48.000000 pyfem-0.2.1/src/pyfem/elements/SolidFiniteStrain.py
--rw-rw-rw-   0        0        0    18134 2024-04-22 06:52:14.000000 pyfem-0.2.1/src/pyfem/elements/SolidPhaseDamageSmallStrain.py
--rw-rw-rw-   0        0        0    12134 2024-04-22 08:23:28.000000 pyfem-0.2.1/src/pyfem/elements/SolidSmallStrain.py
--rw-rw-rw-   0        0        0    16046 2024-04-22 06:32:26.000000 pyfem-0.2.1/src/pyfem/elements/SolidThermalSmallStrain.py
--rw-rw-rw-   0        0        0     8255 2024-04-22 05:25:42.000000 pyfem-0.2.1/src/pyfem/elements/Thermal.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/elements/__init__.py
--rw-rw-rw-   0        0        0     3324 2024-04-08 03:47:57.000000 pyfem-0.2.1/src/pyfem/elements/get_element_data.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.783088 pyfem-0.2.1/src/pyfem/fem/
--rw-rw-rw-   0        0        0     2085 2023-09-07 09:41:11.000000 pyfem-0.2.1/src/pyfem/fem/Timer.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/fem/__init__.py
--rw-rw-rw-   0        0        0      344 2024-04-15 03:43:05.000000 pyfem-0.2.1/src/pyfem/fem/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.877771 pyfem-0.2.1/src/pyfem/io/
--rw-rw-rw-   0        0        0     1124 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/io/Amplitude.py
--rw-rw-rw-   0        0        0     2136 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/io/BC.py
--rw-rw-rw-   0        0        0     1781 2023-11-02 07:24:37.000000 pyfem-0.2.1/src/pyfem/io/BaseIO.py
--rw-rw-rw-   0        0        0      994 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/io/Dof.py
--rw-rw-rw-   0        0        0     3071 2024-04-08 03:47:57.000000 pyfem-0.2.1/src/pyfem/io/Material.py
--rw-rw-rw-   0        0        0      802 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/io/Mesh.py
--rw-rw-rw-   0        0        0     1573 2023-09-19 07:05:17.000000 pyfem-0.2.1/src/pyfem/io/Module.py
--rw-rw-rw-   0        0        0     1065 2023-09-21 04:09:47.000000 pyfem-0.2.1/src/pyfem/io/Output.py
--rw-rw-rw-   0        0        0      672 2023-10-30 08:41:09.000000 pyfem-0.2.1/src/pyfem/io/Parameter.py
--rw-rw-rw-   0        0        0    12038 2024-04-11 06:14:41.000000 pyfem-0.2.1/src/pyfem/io/Properties.py
--rw-rw-rw-   0        0        0     2149 2023-09-15 03:47:33.000000 pyfem-0.2.1/src/pyfem/io/Section.py
--rw-rw-rw-   0        0        0     1952 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/io/Solver.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/io/__init__.py
--rw-rw-rw-   0        0        0     1647 2023-12-20 04:03:58.000000 pyfem-0.2.1/src/pyfem/io/arguments.py
--rw-rw-rw-   0        0        0     5213 2023-11-03 06:49:39.000000 pyfem-0.2.1/src/pyfem/io/write_hdf5.py
--rw-rw-rw-   0        0        0     5839 2024-01-15 09:02:18.000000 pyfem-0.2.1/src/pyfem/io/write_vtk.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.918631 pyfem-0.2.1/src/pyfem/isoelements/
--rw-rw-rw-   0        0        0     2320 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/isoelements/IsoElementDiagram.py
--rw-rw-rw-   0        0        0    21867 2024-03-28 07:30:52.000000 pyfem-0.2.1/src/pyfem/isoelements/IsoElementShape.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/isoelements/__init__.py
--rw-rw-rw-   0        0        0     1297 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/isoelements/derive_shape_functions.py
--rw-rw-rw-   0        0        0     2153 2023-11-02 07:24:49.000000 pyfem-0.2.1/src/pyfem/isoelements/get_iso_element_type.py
--rw-rw-rw-   0        0        0    27934 2024-03-28 07:20:41.000000 pyfem-0.2.1/src/pyfem/isoelements/shape_functions.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:34:00.026271 pyfem-0.2.1/src/pyfem/materials/
--rw-rw-rw-   0        0        0     3385 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/materials/BaseMaterial.py
--rw-rw-rw-   0        0        0     3135 2024-04-17 07:21:32.000000 pyfem-0.2.1/src/pyfem/materials/DiffusionIsotropic.py
--rw-rw-rw-   0        0        0     8776 2024-03-11 03:57:52.000000 pyfem-0.2.1/src/pyfem/materials/ElasticIsotropic.py
--rw-rw-rw-   0        0        0     3135 2023-11-02 07:24:49.000000 pyfem-0.2.1/src/pyfem/materials/MechanicalThermalExpansion.py
--rw-rw-rw-   0        0        0     2174 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/materials/PhaseFieldDamage.py
--rw-rw-rw-   0        0        0    79933 2024-01-17 03:37:48.000000 pyfem-0.2.1/src/pyfem/materials/PlasticCrystal.py
--rw-rw-rw-   0        0        0    91044 2024-01-17 03:37:48.000000 pyfem-0.2.1/src/pyfem/materials/PlasticCrystalGNDs.py
--rw-rw-rw-   0        0        0     8404 2023-09-21 06:20:49.000000 pyfem-0.2.1/src/pyfem/materials/PlasticKinematicHardening.py
--rw-rw-rw-   0        0        0     2773 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/materials/ThermalIsotropic.py
--rw-rw-rw-   0        0        0     6137 2023-09-19 06:25:05.000000 pyfem-0.2.1/src/pyfem/materials/UMAT.py
--rw-rw-rw-   0        0        0    10058 2023-10-27 05:19:05.000000 pyfem-0.2.1/src/pyfem/materials/ViscoElasticMaxwell.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/materials/__init__.py
--rw-rw-rw-   0        0        0    41881 2023-09-26 03:18:28.000000 pyfem-0.2.1/src/pyfem/materials/crystal_slip_system.py
--rw-rw-rw-   0        0        0     2613 2024-04-08 03:47:57.000000 pyfem-0.2.1/src/pyfem/materials/get_material_data.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:34:00.029261 pyfem-0.2.1/src/pyfem/mesh/
--rw-rw-rw-   0        0        0     8071 2024-04-18 04:24:18.000000 pyfem-0.2.1/src/pyfem/mesh/MeshData.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:34:00.116971 pyfem-0.2.1/src/pyfem/quadrature/
--rw-rw-rw-   0        0        0     1657 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/quadrature/BaseQuadrature.py
--rw-rw-rw-   0        0        0     2824 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/quadrature/GaussLegendreQuadrature.py
--rw-rw-rw-   0        0        0     1129 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/quadrature/PyramidQuadrature.py
--rw-rw-rw-   0        0        0    22842 2024-03-28 07:28:06.000000 pyfem-0.2.1/src/pyfem/quadrature/TetrahedronQuadrature.py
--rw-rw-rw-   0        0        0    27075 2024-03-28 07:27:55.000000 pyfem-0.2.1/src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py
--rw-rw-rw-   0        0        0    25700 2024-03-28 04:13:23.000000 pyfem-0.2.1/src/pyfem/quadrature/TriangleQuadrature.py
--rw-rw-rw-   0        0        0    31453 2024-03-28 04:11:40.000000 pyfem-0.2.1/src/pyfem/quadrature/TriangleQuadratureBarycentric.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/quadrature/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:34:00.163811 pyfem-0.2.1/src/pyfem/solvers/
--rw-rw-rw-   0        0        0    15033 2024-04-18 07:31:18.000000 pyfem-0.2.1/src/pyfem/solvers/ArcLengthSolver.py
--rw-rw-rw-   0        0        0     1450 2023-11-01 04:20:15.000000 pyfem-0.2.1/src/pyfem/solvers/BaseSolver.py
--rw-rw-rw-   0        0        0     2225 2024-04-18 04:22:23.000000 pyfem-0.2.1/src/pyfem/solvers/LinearSolver.py
--rw-rw-rw-   0        0        0    16305 2024-04-22 08:32:01.000000 pyfem-0.2.1/src/pyfem/solvers/NonlinearSolver.py
--rw-rw-rw-   0        0        0    17321 2024-04-18 07:30:42.000000 pyfem-0.2.1/src/pyfem/solvers/TimeIntegrationNonlinearSolver.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/solvers/__init__.py
--rw-rw-rw-   0        0        0     1618 2024-04-15 07:19:03.000000 pyfem-0.2.1/src/pyfem/solvers/get_solver_data.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:34:00.218628 pyfem-0.2.1/src/pyfem/utils/
--rw-rw-rw-   0        0        0     2443 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/utils/IntKeyDict.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/utils/__init__.py
--rw-rw-rw-   0        0        0      957 2023-11-02 07:37:35.000000 pyfem-0.2.1/src/pyfem/utils/colors.py
--rw-rw-rw-   0        0        0     3374 2023-11-02 07:09:57.000000 pyfem-0.2.1/src/pyfem/utils/logger.py
--rw-rw-rw-   0        0        0    28928 2024-01-17 03:42:50.000000 pyfem-0.2.1/src/pyfem/utils/mechanics.py
--rw-rw-rw-   0        0        0     3941 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/utils/visualization.py
--rw-rw-rw-   0        0        0     1183 2023-11-01 09:41:59.000000 pyfem-0.2.1/src/pyfem/utils/wrappers.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.663484 pyfem-0.2.1/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0     3686 2024-04-22 08:33:59.000000 pyfem-0.2.1/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3243 2024-04-22 08:33:59.000000 pyfem-0.2.1/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 08:33:59.000000 pyfem-0.2.1/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-22 08:33:59.000000 pyfem-0.2.1/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-22 08:33:59.000000 pyfem-0.2.1/src/pyfem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-22 08:33:59.000000 pyfem-0.2.1/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.688399 pyfem-0.2.2/
+-rw-rw-rw-   0        0        0     1190 2024-04-22 05:18:42.000000 pyfem-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3846 2024-05-10 04:00:01.687426 pyfem-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-10 04:00:01.688399 pyfem-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2024-05-10 03:47:32.000000 pyfem-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.031399 pyfem-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.059628 pyfem-0.2.2/src/pyfem/
+-rw-rw-rw-   0        0        0     2804 2023-11-01 09:09:41.000000 pyfem-0.2.2/src/pyfem/Job.py
+-rw-rw-rw-   0        0        0       23 2024-05-10 03:47:11.000000 pyfem-0.2.2/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0     1388 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.113162 pyfem-0.2.2/src/pyfem/amplitude/
+-rw-rw-rw-   0        0        0     1403 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/amplitude/BaseAmplitude.py
+-rw-rw-rw-   0        0        0     1892 2023-11-02 07:24:23.000000 pyfem-0.2.2/src/pyfem/amplitude/TabularAmplitude.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/amplitude/__init__.py
+-rw-rw-rw-   0        0        0     1112 2023-11-02 07:24:12.000000 pyfem-0.2.2/src/pyfem/amplitude/get_amplitude_data.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.117052 pyfem-0.2.2/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0    14827 2024-05-09 08:43:30.000000 pyfem-0.2.2/src/pyfem/assembly/Assembly.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.175452 pyfem-0.2.2/src/pyfem/bc/
+-rw-rw-rw-   0        0        0     4148 2024-04-15 03:43:05.000000 pyfem-0.2.2/src/pyfem/bc/BaseBC.py
+-rw-rw-rw-   0        0        0     3003 2024-04-18 05:44:17.000000 pyfem-0.2.2/src/pyfem/bc/DirichletBC.py
+-rw-rw-rw-   0        0        0     2984 2024-04-18 05:43:15.000000 pyfem-0.2.2/src/pyfem/bc/NeumannBCConcentrated.py
+-rw-rw-rw-   0        0        0    27073 2024-04-18 05:15:08.000000 pyfem-0.2.2/src/pyfem/bc/NeumannBCDistributed.py
+-rw-rw-rw-   0        0        0    13067 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/bc/NeumannBCPressure.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/bc/__init__.py
+-rw-rw-rw-   0        0        0     1049 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/bc/derive_surface_integral.py
+-rw-rw-rw-   0        0        0     2087 2023-11-02 07:24:23.000000 pyfem-0.2.2/src/pyfem/bc/get_bc_data.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.186159 pyfem-0.2.2/src/pyfem/database/
+-rw-rw-rw-   0        0        0    11040 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/database/Database.py
+-rw-rw-rw-   0        0        0        0 2024-05-06 06:45:32.000000 pyfem-0.2.2/src/pyfem/database/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.263052 pyfem-0.2.2/src/pyfem/elements/
+-rw-rw-rw-   0        0        0    20942 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/elements/BaseElement.py
+-rw-rw-rw-   0        0        0    10277 2024-05-06 08:03:52.000000 pyfem-0.2.2/src/pyfem/elements/Diffusion.py
+-rw-rw-rw-   0        0        0    76454 2024-05-06 08:03:40.000000 pyfem-0.2.2/src/pyfem/elements/SolidFiniteStrain.py
+-rw-rw-rw-   0        0        0    18076 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/elements/SolidPhaseDamageSmallStrain.py
+-rw-rw-rw-   0        0        0    12097 2024-05-06 07:59:24.000000 pyfem-0.2.2/src/pyfem/elements/SolidSmallStrain.py
+-rw-rw-rw-   0        0        0    16068 2024-05-06 08:04:12.000000 pyfem-0.2.2/src/pyfem/elements/SolidThermalSmallStrain.py
+-rw-rw-rw-   0        0        0     8266 2024-05-06 08:04:41.000000 pyfem-0.2.2/src/pyfem/elements/Thermal.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/elements/__init__.py
+-rw-rw-rw-   0        0        0     3324 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/elements/get_element_data.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.275708 pyfem-0.2.2/src/pyfem/fem/
+-rw-rw-rw-   0        0        0     2085 2023-09-07 09:41:11.000000 pyfem-0.2.2/src/pyfem/fem/Timer.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/fem/__init__.py
+-rw-rw-rw-   0        0        0      344 2024-04-15 03:43:05.000000 pyfem-0.2.2/src/pyfem/fem/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.358439 pyfem-0.2.2/src/pyfem/io/
+-rw-rw-rw-   0        0        0     1124 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/io/Amplitude.py
+-rw-rw-rw-   0        0        0     2136 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/io/BC.py
+-rw-rw-rw-   0        0        0     2242 2024-05-10 03:46:13.000000 pyfem-0.2.2/src/pyfem/io/BaseIO.py
+-rw-rw-rw-   0        0        0      994 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/io/Dof.py
+-rw-rw-rw-   0        0        0     3289 2024-05-06 07:17:36.000000 pyfem-0.2.2/src/pyfem/io/Material.py
+-rw-rw-rw-   0        0        0      802 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/io/Mesh.py
+-rw-rw-rw-   0        0        0     1065 2023-09-21 04:09:47.000000 pyfem-0.2.2/src/pyfem/io/Output.py
+-rw-rw-rw-   0        0        0      672 2023-10-30 08:41:09.000000 pyfem-0.2.2/src/pyfem/io/Parameter.py
+-rw-rw-rw-   0        0        0    13127 2024-05-10 03:41:51.000000 pyfem-0.2.2/src/pyfem/io/Properties.py
+-rw-rw-rw-   0        0        0     2149 2023-09-15 03:47:33.000000 pyfem-0.2.2/src/pyfem/io/Section.py
+-rw-rw-rw-   0        0        0     1952 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/io/Solver.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1647 2023-12-20 04:03:58.000000 pyfem-0.2.2/src/pyfem/io/arguments.py
+-rw-rw-rw-   0        0        0     5839 2024-01-15 09:02:18.000000 pyfem-0.2.2/src/pyfem/io/write_vtk.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.402241 pyfem-0.2.2/src/pyfem/isoelements/
+-rw-rw-rw-   0        0        0     2320 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/isoelements/IsoElementDiagram.py
+-rw-rw-rw-   0        0        0    21673 2024-05-06 09:08:36.000000 pyfem-0.2.2/src/pyfem/isoelements/IsoElementShape.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/isoelements/__init__.py
+-rw-rw-rw-   0        0        0     1297 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/isoelements/derive_shape_functions.py
+-rw-rw-rw-   0        0        0     2153 2023-11-02 07:24:49.000000 pyfem-0.2.2/src/pyfem/isoelements/get_iso_element_type.py
+-rw-rw-rw-   0        0        0    27934 2024-03-28 07:20:41.000000 pyfem-0.2.2/src/pyfem/isoelements/shape_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.501520 pyfem-0.2.2/src/pyfem/materials/
+-rw-rw-rw-   0        0        0     3385 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/materials/BaseMaterial.py
+-rw-rw-rw-   0        0        0     3177 2024-05-09 08:36:01.000000 pyfem-0.2.2/src/pyfem/materials/DiffusionIsotropic.py
+-rw-rw-rw-   0        0        0     8772 2024-05-09 08:28:32.000000 pyfem-0.2.2/src/pyfem/materials/ElasticIsotropic.py
+-rw-rw-rw-   0        0        0     3177 2024-05-09 08:29:14.000000 pyfem-0.2.2/src/pyfem/materials/MechanicalThermalExpansion.py
+-rw-rw-rw-   0        0        0     2211 2024-05-09 08:34:27.000000 pyfem-0.2.2/src/pyfem/materials/PhaseFieldDamage.py
+-rw-rw-rw-   0        0        0    80110 2024-05-09 08:51:21.000000 pyfem-0.2.2/src/pyfem/materials/PlasticCrystal.py
+-rw-rw-rw-   0        0        0    91328 2024-05-10 03:46:13.000000 pyfem-0.2.2/src/pyfem/materials/PlasticCrystalGNDs.py
+-rw-rw-rw-   0        0        0     8446 2024-05-09 08:34:27.000000 pyfem-0.2.2/src/pyfem/materials/PlasticKinematicHardening.py
+-rw-rw-rw-   0        0        0     3399 2024-05-09 08:35:00.000000 pyfem-0.2.2/src/pyfem/materials/ThermalIsotropic.py
+-rw-rw-rw-   0        0        0    10100 2024-05-09 08:35:55.000000 pyfem-0.2.2/src/pyfem/materials/ViscoElasticMaxwell.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/materials/__init__.py
+-rw-rw-rw-   0        0        0    41870 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/materials/crystal_slip_system.py
+-rw-rw-rw-   0        0        0     2984 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/materials/get_material_data.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.511309 pyfem-0.2.2/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0     8071 2024-04-18 04:24:18.000000 pyfem-0.2.2/src/pyfem/mesh/MeshData.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.604692 pyfem-0.2.2/src/pyfem/quadrature/
+-rw-rw-rw-   0        0        0     1657 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/quadrature/BaseQuadrature.py
+-rw-rw-rw-   0        0        0     2824 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/quadrature/GaussLegendreQuadrature.py
+-rw-rw-rw-   0        0        0     1129 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/quadrature/PyramidQuadrature.py
+-rw-rw-rw-   0        0        0    22842 2024-03-28 07:28:06.000000 pyfem-0.2.2/src/pyfem/quadrature/TetrahedronQuadrature.py
+-rw-rw-rw-   0        0        0    27075 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py
+-rw-rw-rw-   0        0        0    25700 2024-03-28 04:13:23.000000 pyfem-0.2.2/src/pyfem/quadrature/TriangleQuadrature.py
+-rw-rw-rw-   0        0        0    31453 2024-03-28 04:11:40.000000 pyfem-0.2.2/src/pyfem/quadrature/TriangleQuadratureBarycentric.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/quadrature/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.649466 pyfem-0.2.2/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0    15057 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/solvers/ArcLengthSolver.py
+-rw-rw-rw-   0        0        0     1633 2024-05-06 06:45:32.000000 pyfem-0.2.2/src/pyfem/solvers/BaseSolver.py
+-rw-rw-rw-   0        0        0     2225 2024-04-18 04:22:23.000000 pyfem-0.2.2/src/pyfem/solvers/LinearSolver.py
+-rw-rw-rw-   0        0        0    16486 2024-05-06 09:22:48.000000 pyfem-0.2.2/src/pyfem/solvers/NonlinearSolver.py
+-rw-rw-rw-   0        0        0    17330 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/solvers/TimeIntegrationNonlinearSolver.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/solvers/__init__.py
+-rw-rw-rw-   0        0        0     1618 2024-05-06 09:04:40.000000 pyfem-0.2.2/src/pyfem/solvers/get_solver_data.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.685479 pyfem-0.2.2/src/pyfem/utils/
+-rw-rw-rw-   0        0        0     2443 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/utils/IntKeyDict.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/utils/__init__.py
+-rw-rw-rw-   0        0        0      983 2024-05-10 03:46:13.000000 pyfem-0.2.2/src/pyfem/utils/colors.py
+-rw-rw-rw-   0        0        0     3374 2023-11-02 07:09:57.000000 pyfem-0.2.2/src/pyfem/utils/logger.py
+-rw-rw-rw-   0        0        0    28928 2024-05-10 03:46:38.000000 pyfem-0.2.2/src/pyfem/utils/mechanics.py
+-rw-rw-rw-   0        0        0     3941 2023-08-17 09:47:32.000000 pyfem-0.2.2/src/pyfem/utils/visualization.py
+-rw-rw-rw-   0        0        0     1183 2024-05-10 03:46:42.000000 pyfem-0.2.2/src/pyfem/utils/wrappers.py
+drwxrwxrwx   0        0        0        0 2024-05-10 04:00:01.085906 pyfem-0.2.2/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0     3846 2024-05-10 04:00:00.000000 pyfem-0.2.2/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3227 2024-05-10 04:00:00.000000 pyfem-0.2.2/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 04:00:00.000000 pyfem-0.2.2/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-10 04:00:00.000000 pyfem-0.2.2/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-05-10 04:00:00.000000 pyfem-0.2.2/src/pyfem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-10 04:00:00.000000 pyfem-0.2.2/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.2.1/LICENSE` & `pyfem-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/PKG-INFO` & `pyfem-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Finite Element Method
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: meshio
+Requires-Dist: tomli
+Requires-Dist: colorlog
+Requires-Dist: sympy
+Requires-Dist: tomli_w
 
 # pyfem
 
 pyfem是一个完全基于python语言实现的极简有限元求解器。依赖的第三方库包括numpy、scipy和meshio等，主要用于有限元方法的学习、有限元算法验证和快速建立材料本构模型的程序原型。
 
 Github仓库：https://github.com/sunwhale/pyfem
 
@@ -106,15 +113,15 @@
 
 
 ## Development 开发
 
 ### ToDo list
 
 - [ ] 增加如何建立toml算例文件的帮助文档
-- [ ] 增加hdf5计算结果输出格式
+- [x] 增加hdf5计算结果输出格式
 - [ ] 处理平面应力状态的面外应力平衡
 - [ ] 增加内聚区单元
 - [ ] 增加动力学求解器
 - [ ] 建立前处理界面
 
 ### Bug list
```

### Comparing `pyfem-0.2.1/setup.py` & `pyfem-0.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,10 +31,11 @@
     },
     install_requires=[
         'numpy',
         'scipy',
         'meshio',
         'tomli',
         'colorlog',
-        'sympy'
+        'sympy',
+        'tomli_w'
     ],
 )
```

### Comparing `pyfem-0.2.1/src/pyfem/Job.py` & `pyfem-0.2.2/src/pyfem/Job.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/__main__.py` & `pyfem-0.2.2/src/pyfem/__main__.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from pathlib import Path
 import traceback
+from pathlib import Path
 
+from pyfem import __version__
 from pyfem.Job import Job
 from pyfem.io.arguments import get_arguments
 from pyfem.utils.logger import logger, set_logger, logger_sta, set_logger_sta
 from pyfem.utils.wrappers import show_running_time
-from pyfem import __version__
 
 
 @show_running_time
 def main() -> None:
     args = get_arguments()
 
     input_file = Path(args.i)
```

### Comparing `pyfem-0.2.1/src/pyfem/amplitude/BaseAmplitude.py` & `pyfem-0.2.2/src/pyfem/amplitude/BaseAmplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/amplitude/TabularAmplitude.py` & `pyfem-0.2.2/src/pyfem/amplitude/TabularAmplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/amplitude/get_amplitude_data.py` & `pyfem-0.2.2/src/pyfem/amplitude/get_amplitude_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/assembly/Assembly.py` & `pyfem-0.2.2/src/pyfem/assembly/Assembly.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-import time
 
 from numpy import repeat, array, ndarray, empty, zeros
 from scipy.sparse import coo_matrix, csc_matrix  # type: ignore
 
 from pyfem.bc.get_bc_data import get_bc_data, BCData
 from pyfem.elements.get_element_data import get_element_data, ElementData
 from pyfem.fem.Timer import Timer
@@ -248,15 +247,16 @@
                 element_dof_ids = element_data.element_dof_ids
                 element_dof_number = element_data.element_dof_number
                 row += [r for r in repeat(element_dof_ids, element_dof_number)]
                 for _ in range(element_dof_number):
                     col += [c for c in element_dof_ids]
                 val += [v for v in element_data.element_stiffness.reshape(element_dof_number * element_dof_number)]
 
-            self.global_stiffness = coo_matrix((array(val, dtype=DTYPE), (array(row, dtype=DTYPE), array(col, dtype=DTYPE))), shape=(self.total_dof_number, self.total_dof_number)).tocsr()
+            self.global_stiffness = coo_matrix((array(val, dtype=DTYPE), (array(row, dtype=DTYPE), array(col, dtype=DTYPE))),
+                                               shape=(self.total_dof_number, self.total_dof_number)).tocsr()
 
     # @show_running_time
     def assembly_fint(self) -> None:
         self.fint = zeros(self.total_dof_number, dtype=DTYPE)
         for element_data in self.element_data_list:
             self.fint[element_data.element_dof_ids] += element_data.element_fint
 
@@ -297,15 +297,15 @@
         for element_data in self.element_data_list:
             element_data.update_element_field_variables()
 
     def assembly_field_variables(self) -> None:
         nodes_number = len(self.props.mesh_data.nodes)
 
         for output in self.props.outputs:
-            if output.type == 'vtk':
+            if output.type in ['vtk', 'hdf5']:
                 for field_name in output.field_outputs:
                     self.field_variables[field_name] = zeros(nodes_number)
                     nodes_count = zeros(nodes_number)
                     for element_data in self.element_data_list:
                         assembly_conn = element_data.assembly_conn
                         self.field_variables[field_name][assembly_conn] += \
                             element_data.element_average_field_variables[field_name]
```

### Comparing `pyfem-0.2.1/src/pyfem/bc/BaseBC.py` & `pyfem-0.2.2/src/pyfem/bc/BaseBC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/bc/DirichletBC.py` & `pyfem-0.2.2/src/pyfem/bc/DirichletBC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/bc/NeumannBCConcentrated.py` & `pyfem-0.2.2/src/pyfem/bc/NeumannBCConcentrated.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/bc/NeumannBCDistributed.py` & `pyfem-0.2.2/src/pyfem/bc/NeumannBCDistributed.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/bc/NeumannBCPressure.py` & `pyfem-0.2.2/src/pyfem/bc/NeumannBCPressure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from typing import Optional
 
-from numpy import array, delete, dot, logical_and, ndarray, in1d, all, zeros, sign, cross, sum, sqrt
+from numpy import array, delete, dot, logical_and, ndarray, in1d, all, zeros, sign, cross, sum
 from numpy.linalg import det, norm
 
 from pyfem.bc.BaseBC import BaseBC
 from pyfem.io.Amplitude import Amplitude
 from pyfem.io.BC import BC
 from pyfem.io.Dof import Dof
 from pyfem.io.Solver import Solver
```

### Comparing `pyfem-0.2.1/src/pyfem/bc/derive_surface_integral.py` & `pyfem-0.2.2/src/pyfem/bc/derive_surface_integral.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/bc/get_bc_data.py` & `pyfem-0.2.2/src/pyfem/bc/get_bc_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/elements/BaseElement.py` & `pyfem-0.2.2/src/pyfem/elements/BaseElement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from copy import deepcopy
 
-from numpy import dot, ndarray, array, ones, concatenate, transpose, einsum
-from numpy.linalg import det, inv
+from numpy import dot, ndarray, array, ones, concatenate, einsum
+from numpy.linalg import det
 
 from pyfem.fem.Timer import Timer
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.isoelements.IsoElementShape import IsoElementShape
 from pyfem.materials.get_material_data import MaterialData
```

### Comparing `pyfem-0.2.1/src/pyfem/elements/Diffusion.py` & `pyfem-0.2.2/src/pyfem/elements/Diffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                  materials: list[Material],
                  section: Section,
                  material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = [('DiffusionIsotropic',)]
+        self.allowed_material_data_list = [('DiffusionIsotropic', 'User')]
         self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
```

### Comparing `pyfem-0.2.1/src/pyfem/elements/SolidFiniteStrain.py` & `pyfem-0.2.2/src/pyfem/elements/SolidFiniteStrain.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                  section: Section,
                  material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
         self.allowed_material_data_list = [
-            ('ElasticIsotropic', 'PlasticKinematicHardening', 'PlasticCrystal', 'PlasticCrystalGNDs', 'ViscoElasticMaxwell')]
+            ('ElasticIsotropic', 'PlasticKinematicHardening', 'PlasticCrystal', 'PlasticCrystalGNDs', 'ViscoElasticMaxwell', 'User')]
         self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
```

### Comparing `pyfem-0.2.1/src/pyfem/elements/SolidPhaseDamageSmallStrain.py` & `pyfem-0.2.2/src/pyfem/elements/SolidPhaseDamageSmallStrain.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.isoelements.IsoElementShape import IsoElementShape
 from pyfem.materials.get_material_data import MaterialData
 from pyfem.utils.colors import error_style
-from pyfem.utils.mechanics import get_decompose_energy
 
 
 class SolidPhaseDamageSmallStrain(BaseElement):
     r"""
     固体相场断裂单元。
 
     :ivar qp_b_matrices: 积分点处的B矩阵列表
@@ -89,16 +88,17 @@
                  materials: list[Material],
                  section: Section,
                  material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell', 'PlasticCrystal', 'PlasticCrystalGNDs'),
-                                           ('PhaseFieldDamage',)]
+        self.allowed_material_data_list = [
+            ('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell', 'PlasticCrystal', 'PlasticCrystalGNDs', 'User'),
+            ('PhaseFieldDamage', 'User')]
         self.allowed_material_number = len(self.allowed_material_data_list)
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
```

### Comparing `pyfem-0.2.1/src/pyfem/elements/SolidSmallStrain.py` & `pyfem-0.2.2/src/pyfem/elements/SolidSmallStrain.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                  section: Section,
                  material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
         self.allowed_material_data_list = [
-            ('ElasticIsotropic', 'PlasticKinematicHardening', 'PlasticCrystal', 'PlasticCrystalGNDs', 'ViscoElasticMaxwell')]
+            ('ElasticIsotropic', 'PlasticKinematicHardening', 'PlasticCrystal', 'PlasticCrystalGNDs', 'ViscoElasticMaxwell', 'User')]
         self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
@@ -202,16 +202,15 @@
                 qp_b_matrix_transpose = qp_b_matrices_transpose[i]
                 qp_b_matrix = qp_b_matrices[i]
                 qp_weight_times_jacobi_det = qp_weight_times_jacobi_dets[i]
                 qp_ddsdde = self.qp_ddsddes[i]
                 qp_stress = self.qp_stresses[i]
 
             if is_update_stiffness:
-                self.element_stiffness += dot(qp_b_matrix_transpose, dot(qp_ddsdde, qp_b_matrix)) * \
-                                          qp_weight_times_jacobi_det
+                self.element_stiffness += dot(qp_b_matrix_transpose, dot(qp_ddsdde, qp_b_matrix)) * qp_weight_times_jacobi_det
 
             if is_update_fint:
                 self.element_fint += dot(qp_b_matrix_transpose, qp_stress) * qp_weight_times_jacobi_det
 
     def update_element_field_variables(self) -> None:
         qp_stresses = self.qp_stresses
         qp_strains = self.qp_strains
```

### Comparing `pyfem-0.2.1/src/pyfem/elements/SolidThermalSmallStrain.py` & `pyfem-0.2.2/src/pyfem/elements/SolidThermalSmallStrain.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,17 +66,17 @@
                  materials: list[Material],
                  section: Section,
                  material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell'),
-                                           ('ThermalIsotropic',),
-                                           ('MechanicalThermalExpansion',)]
+        self.allowed_material_data_list = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell', 'User'),
+                                           ('ThermalIsotropic', 'User'),
+                                           ('MechanicalThermalExpansion', 'User')]
         self.allowed_material_number = len(self.allowed_material_data_list)
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
```

### Comparing `pyfem-0.2.1/src/pyfem/elements/Thermal.py` & `pyfem-0.2.2/src/pyfem/elements/Thermal.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                  materials: list[Material],
                  section: Section,
                  material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = [('ThermalIsotropic',)]
+        self.allowed_material_data_list = [('ThermalIsotropic', 'User')]
         self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
@@ -168,18 +168,18 @@
     def update_element_field_variables(self) -> None:
         qp_temperatures = self.qp_temperatures
         qp_heat_fluxes = self.qp_heat_fluxes
 
         average_temperatures = average(qp_temperatures, axis=0)
         average_heat_fluxes = average(qp_heat_fluxes, axis=0)
 
-        self.qp_field_variables['temperature'] = array(qp_temperatures, dtype=DTYPE)
+        # self.qp_field_variables['temperature'] = array(qp_temperatures, dtype=DTYPE)
         self.qp_field_variables['heat_flux'] = array(qp_heat_fluxes, dtype=DTYPE)
 
-        self.element_average_field_variables['T'] = average_temperatures
+        # self.element_average_field_variables['T'] = average_temperatures
         if len(average_heat_fluxes) >= 1:
             self.element_average_field_variables['HFL1'] = average_heat_fluxes[0]
         if len(average_heat_fluxes) >= 2:
             self.element_average_field_variables['HFL2'] = average_heat_fluxes[1]
         if len(average_heat_fluxes) >= 3:
             self.element_average_field_variables['HFL3'] = average_heat_fluxes[2]
```

### Comparing `pyfem-0.2.1/src/pyfem/elements/get_element_data.py` & `pyfem-0.2.2/src/pyfem/elements/get_element_data.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 """
 from typing import Union
 
 from numpy import ndarray
 
 from pyfem.elements.BaseElement import BaseElement
+from pyfem.elements.Diffusion import Diffusion
+from pyfem.elements.SolidFiniteStrain import SolidFiniteStrain
 from pyfem.elements.SolidPhaseDamageSmallStrain import SolidPhaseDamageSmallStrain
 from pyfem.elements.SolidSmallStrain import SolidSmallStrain
-from pyfem.elements.SolidFiniteStrain import SolidFiniteStrain
 from pyfem.elements.SolidThermalSmallStrain import SolidThermalSmallStrain
 from pyfem.elements.Thermal import Thermal
-from pyfem.elements.Diffusion import Diffusion
 from pyfem.fem.Timer import Timer
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.isoelements.IsoElementShape import IsoElementShape
 from pyfem.materials.get_material_data import MaterialData
 from pyfem.utils.colors import error_style
```

### Comparing `pyfem-0.2.1/src/pyfem/fem/Timer.py` & `pyfem-0.2.2/src/pyfem/fem/Timer.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/io/Amplitude.py` & `pyfem-0.2.2/src/pyfem/io/Amplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/io/BC.py` & `pyfem-0.2.2/src/pyfem/io/BC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/io/BaseIO.py` & `pyfem-0.2.2/src/pyfem/io/BaseIO.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from typing import Dict, List
 
+import tomli_w
+
+try:
+    import tomllib  # type: ignore
+except ModuleNotFoundError:
+    import tomli as tomllib  # type: ignore
+
 from pyfem.utils.colors import error_style
 from pyfem.utils.visualization import object_slots_to_string
 
 
 class BaseIO:
     """
     属性配置基类。
@@ -48,11 +55,22 @@
     def show(self) -> None:
         print(self.to_string())
 
     def set_io_values(self, io_dict: Dict) -> None:
         for key, item in io_dict.items():
             self.__setattr__(key, item)
 
+    def to_dict(self) -> dict:
+        object_dict = {}
+        for key in self.__slots__:
+            item = self.__getattribute__(key)
+            if item is not None:
+                object_dict[key] = item
+        return object_dict
+
+    def to_toml(self) -> str:
+        return tomli_w.dumps(self.to_dict())
+
 
 if __name__ == "__main__":
     io = BaseIO()
     io.show()
```

### Comparing `pyfem-0.2.1/src/pyfem/io/Dof.py` & `pyfem-0.2.2/src/pyfem/io/Dof.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/io/Material.py` & `pyfem-0.2.2/src/pyfem/io/Material.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,35 +20,40 @@
     :vartype type: str
 
     :ivar data: 材料数据列表
     :vartype data: list[float]
 
     :ivar data_dict: 材料数据字典
     :vartype data_dict: dict[str, any]
+
+    :ivar user_path: 用户自定义材料路径
+    :vartype user_path: str
     """
 
     __slots_dict__: dict = {
         'name': ('str', '材料名称'),
         'category': ('str', '材料类别'),
         'type': ('str', '材料类型'),
         'data': ('list[float]', '材料数据列表'),
-        'data_dict': ('dict[str, any]', '材料数据字典')
+        'data_dict': ('dict[str, any]', '材料数据字典'),
+        'user_path': ('str', '用户自定义材料路径')
     }
 
     __slots__: list = [slot for slot in __slots_dict__.keys()]
 
     allowed_categories_types: dict = {
         None: [None],
         'Elastic': ['Isotropic'],
         'Plastic': ['KinematicHardening', 'Crystal', 'CrystalGNDs'],
         'ViscoElastic': ['Maxwell'],
         'Thermal': ['Isotropic'],
         'PhaseField': ['Damage'],
         'MechanicalThermal': ['Expansion'],
         'Diffusion': ['Isotropic'],
+        'User': [''],
     }
 
     allowed_keys_values: dict = {
         'category': allowed_categories_types.keys(),
         'type': []
     }
 
@@ -58,14 +63,15 @@
     def __init__(self) -> None:
         super().__init__()
         self.name: str = None  # type: ignore
         self.category: str = None  # type: ignore
         self.type: str = None  # type: ignore
         self.data: list[float] = None  # type: ignore
         self.data_dict: dict = None  # type: ignore
+        self.user_path: str = None  # type: ignore
 
     def __setattr__(self, key, value) -> None:
         if self.is_read_only:
             if key not in self.__slots__:
                 error_msg = f'{key} is not an allowable attribute keyword of {type(self).__name__}'
                 raise AttributeError(error_style(error_msg))
```

### Comparing `pyfem-0.2.1/src/pyfem/io/Mesh.py` & `pyfem-0.2.2/src/pyfem/io/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/io/Output.py` & `pyfem-0.2.2/src/pyfem/io/Output.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/io/Parameter.py` & `pyfem-0.2.2/src/pyfem/io/Parameter.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/io/Properties.py` & `pyfem-0.2.2/src/pyfem/io/Properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -286,14 +286,29 @@
 
         if 'outputs' in toml_keys:
             outputs_dict = self.toml['outputs']
             self.set_outputs(outputs_dict)
 
         self.verify()
 
+    def to_dict(self) -> dict:
+        prop_dict = {}
+        prop_dict['title'] = str(self.__getattribute__('title'))
+        prop_dict['mesh'] = self.__getattribute__('mesh').to_dict()
+        prop_dict['dof'] = self.__getattribute__('dof').to_dict()
+        prop_dict['materials'] = [material.to_dict() for material in self.__getattribute__('materials')]
+        prop_dict['sections'] = [material.to_dict() for material in self.__getattribute__('sections')]
+        prop_dict['amplitudes'] = [material.to_dict() for material in self.__getattribute__('amplitudes')]
+        prop_dict['bcs'] = [material.to_dict() for material in self.__getattribute__('bcs')]
+        prop_dict['solver'] = self.__getattribute__('solver').to_dict()
+        prop_dict['outputs'] = [material.to_dict() for material in self.__getattribute__('outputs')]
+        prop_dict['parameter_filename'] = self.__getattribute__('parameter_filename')
+        prop_dict['parameters'] = self.__getattribute__('parameters')
+        return prop_dict
+
 
 def extract_parameter_label(string: str) -> str:
     """
     从带有<>的字符串中提取参数标签
     """
     pattern = r'<(.*?)>'
     matches = re.findall(pattern, string)
@@ -323,8 +338,10 @@
 if __name__ == "__main__":
     # from pyfem.utils.visualization import print_slots_dict
     #
     # print_slots_dict(Properties.__slots_dict__)
 
     props = Properties()
     props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
-    props.show()
+    # props.show()
+    print(props.to_dict())
+    print(props.to_toml())
```

### Comparing `pyfem-0.2.1/src/pyfem/io/Section.py` & `pyfem-0.2.2/src/pyfem/io/Section.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/io/Solver.py` & `pyfem-0.2.2/src/pyfem/io/Solver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/io/arguments.py` & `pyfem-0.2.2/src/pyfem/io/arguments.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/io/write_vtk.py` & `pyfem-0.2.2/src/pyfem/io/write_vtk.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/isoelements/IsoElementDiagram.py` & `pyfem-0.2.2/src/pyfem/isoelements/IsoElementDiagram.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/isoelements/IsoElementShape.py` & `pyfem-0.2.2/src/pyfem/isoelements/IsoElementShape.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 
 """
 from typing import Callable
 
 from numpy import empty, array, ndarray, insert, in1d, sqrt
 
 from pyfem.isoelements.IsoElementDiagram import IsoElementDiagram
-from pyfem.isoelements.shape_functions import get_shape_line2, get_shape_tetra4, get_shape_tetra4_barycentric, get_shape_empty, get_shape_hex20, get_shape_quad4, \
-    get_shape_tria3, get_shape_tria3_barycentric, get_shape_line3, get_shape_quad8, get_shape_tria6, get_shape_tria6_barycentric, get_shape_hex8
+from pyfem.isoelements.shape_functions import get_shape_line2, get_shape_tetra4_barycentric, get_shape_empty, get_shape_hex20, \
+    get_shape_quad4, get_shape_tria3_barycentric, get_shape_line3, get_shape_quad8, get_shape_tria6_barycentric, get_shape_hex8
 from pyfem.quadrature.GaussLegendreQuadrature import GaussLegendreQuadrature
-from pyfem.quadrature.TetrahedronQuadrature import TetrahedronQuadrature
 from pyfem.quadrature.TetrahedronQuadratureBarycentric import TetrahedronQuadratureBarycentric
-from pyfem.quadrature.TriangleQuadrature import TriangleQuadrature
 from pyfem.quadrature.TriangleQuadratureBarycentric import TriangleQuadratureBarycentric
 from pyfem.utils.colors import error_style
 from pyfem.utils.visualization import object_slots_to_string_ndarray
 
 
 class IsoElementShape:
     """
```

### Comparing `pyfem-0.2.1/src/pyfem/isoelements/derive_shape_functions.py` & `pyfem-0.2.2/src/pyfem/isoelements/derive_shape_functions.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/isoelements/get_iso_element_type.py` & `pyfem-0.2.2/src/pyfem/isoelements/get_iso_element_type.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/isoelements/shape_functions.py` & `pyfem-0.2.2/src/pyfem/isoelements/shape_functions.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/materials/BaseMaterial.py` & `pyfem-0.2.2/src/pyfem/materials/BaseMaterial.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/materials/DiffusionIsotropic.py` & `pyfem-0.2.2/src/pyfem/materials/DiffusionIsotropic.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,19 +26,21 @@
 
     __slots_dict__: dict = {
         'd': ('float', 'Diffusion coefficient d'),
     }
 
     __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __data_keys__ = ['Diffusion coefficient d']
+
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('', 'Volume', 'PlaneStress', 'PlaneStrain')
 
-        self.data_keys = ['Diffusion coefficient d']
+        self.data_keys = self.__data_keys__
 
         if len(self.material.data) != len(self.data_keys):
             raise NotImplementedError(error_style(self.get_data_length_error_msg()))
         else:
             for i, key in enumerate(self.data_keys):
                 self.data_dict[key] = material.data[i]
```

### Comparing `pyfem-0.2.1/src/pyfem/materials/ElasticIsotropic.py` & `pyfem-0.2.2/src/pyfem/materials/ElasticIsotropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from copy import deepcopy
+
 from numpy import array, ndarray, dot, zeros
 
 from pyfem.fem.Timer import Timer
-from pyfem.io.Material import Material
 from pyfem.fem.constants import DTYPE
+from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
 
 class ElasticIsotropic(BaseMaterial):
     """
@@ -29,19 +30,21 @@
     __slots_dict__: dict = {
         'E': ('float', 'Young\'s modulus E'),
         'nu': ('float', 'Poisson\'s ratio nu'),
     }
 
     __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __data_keys__ = ['Young\'s modulus E', 'Poisson\'s ratio nu']
+
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
 
-        self.data_keys = ['Young\'s modulus E', 'Poisson\'s ratio nu']
+        self.data_keys = self.__data_keys__
 
         if len(self.material.data) != len(self.data_keys):
             raise NotImplementedError(error_style(self.get_data_length_error_msg()))
         else:
             for i, key in enumerate(self.data_keys):
                 self.data_dict[key] = material.data[i]
 
@@ -61,25 +64,28 @@
                     state_variable_new: dict[str, ndarray],
                     element_id: int,
                     iqp: int,
                     ntens: int,
                     ndi: int,
                     nshr: int,
                     timer: Timer) -> tuple[ndarray, dict[str, ndarray]]:
-        """
-        注：这里没有使用增量格式。对于线性问题，全量和增量格式得到的结果相同。
-        """
+
+        # 全量格式
+        # strain = variable['strain']
+        # stress = dot(self.tangent, strain)
+
+        # 增量格式
         strain = variable['strain']
         dstrain = variable['dstrain']
         if state_variable == {} or timer.time0 == 0.0:
             state_variable['stress'] = zeros(len(strain), dtype=DTYPE)
         stress = deepcopy(state_variable['stress'])
         stress += dot(self.tangent, dstrain)
         state_variable_new['stress'] = stress
-        # stress = dot(self.tangent, strain)
+
         strain_energy = 0.5 * sum(stress * strain)
         output = {'stress': stress, 'strain_energy': strain_energy}
         return self.tangent, output
 
 
 def get_lame_from_young_poisson(E: float, nu: float, plane: str) -> tuple[float, float]:
     r"""
```

### Comparing `pyfem-0.2.1/src/pyfem/materials/MechanicalThermalExpansion.py` & `pyfem-0.2.2/src/pyfem/materials/MechanicalThermalExpansion.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,21 @@
 
     __slots_dict__: dict = {
         'alpha': ('float', 'Coefficient of thermal expansion alpha')
     }
 
     __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __data_keys__ = ['Coefficient of thermal expansion alpha']
+
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
 
-        self.data_keys = ['Coefficient of thermal expansion alpha']
+        self.data_keys = self.__data_keys__
 
         if len(self.material.data) != len(self.data_keys):
             raise NotImplementedError(error_style(self.get_data_length_error_msg()))
         else:
             for i, key in enumerate(self.data_keys):
                 self.data_dict[key] = material.data[i]
```

### Comparing `pyfem-0.2.1/src/pyfem/materials/PhaseFieldDamage.py` & `pyfem-0.2.2/src/pyfem/materials/PhaseFieldDamage.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,20 +24,22 @@
     __slots_dict__: dict = {
         'gc': ('float', 'surface energy to create a unit fracture surface gc'),
         'lc': ('float', 'length scale parameter to measure the damage diffusion lc'),
     }
 
     __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __data_keys__ = ['surface energy to create a unit fracture surface gc',
+                     'length scale parameter to measure the damage diffusion lc']
+
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
 
-        self.data_keys = ['surface energy to create a unit fracture surface gc',
-                          'length scale parameter to measure the damage diffusion lc']
+        self.data_keys = self.__data_keys__
 
         if len(self.material.data) != len(self.data_keys):
             raise NotImplementedError(error_style(self.get_data_length_error_msg()))
         else:
             for i, key in enumerate(self.data_keys):
                 self.data_dict[key] = material.data[i]
```

### Comparing `pyfem-0.2.1/src/pyfem/materials/PlasticCrystal.py` & `pyfem-0.2.2/src/pyfem/materials/PlasticCrystal.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,16 @@
         'm_s': ('ndarray', '特征滑移系滑移方向'),
         'n_s': ('ndarray', '特征滑移系滑移面法向'),
         'MAX_NITER': ('ndarray', '硬化系数矩阵'),
     }
 
     __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __data_keys__ = ['elastic', 'theta', 'slip_system_name', 'c_over_a', 'K', 'dot_gamma_0', 'p_s', 'c_1', 'c_2', 'r_0', 'b_s', 'Q_s']
+
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('Volume', 'PlaneStrain')
 
         self.data_keys = []
 
         if len(self.material.data) != len(self.data_keys):
@@ -1297,8 +1299,8 @@
     print_slots_dict(PlasticCrystal.__slots_dict__)
 
     from pyfem.Job import Job
 
     # job = Job(r'..\..\..\examples\mechanical\1element\hex20_crystal\Job-1.toml')
     job = Job(r'..\..\..\examples\mechanical\4_grains_crystal\Job-1.toml')
 
-    job.run()
+    print(job.props.materials[0].data_dict.keys())
```

### Comparing `pyfem-0.2.1/src/pyfem/materials/PlasticCrystalGNDs.py` & `pyfem-0.2.2/src/pyfem/materials/PlasticCrystalGNDs.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,17 @@
         'm_s': ('ndarray', '特征滑移系滑移方向'),
         'n_s': ('ndarray', '特征滑移系滑移面法向'),
         'MAX_NITER': ('ndarray', '最大迭代次数'),
     }
 
     __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __data_keys__ = ['elastic', 'theta', 'temperature', 'k_b', 'G', 'slip_system_name', 'c_over_a', 'v_0', 'tau_sol', 'b_s', 'Q_s', 'p_s', 'q_s', 'd_grain',
+                     'i_slip', 'c_anni', 'Q_climb', 'Omega_climb_coefficient', 'D_0']
+
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('Volume', 'PlaneStrain')
 
         self.data_keys = []
 
         if len(self.material.data) != len(self.data_keys):
@@ -1504,8 +1507,8 @@
 
     print_slots_dict(PlasticCrystalGNDs.__slots_dict__)
 
     from pyfem.Job import Job
 
     job = Job(r'..\..\..\examples\mechanical\1element\hex20_crystal_GNDs\Job-1.toml')
 
-    job.run()
+    print(job.props.materials[0].data_dict.keys())
```

### Comparing `pyfem-0.2.1/src/pyfem/materials/PlasticKinematicHardening.py` & `pyfem-0.2.2/src/pyfem/materials/PlasticKinematicHardening.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,19 +63,21 @@
         'EG3': ('float', '3倍剪切模量'),
         'ELAM': ('float', '拉梅常数'),
         'tolerance': ('float', '判断屈服的误差容限'),
     }
 
     __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __data_keys__ = ['Young\'s modulus E', 'Poisson\'s ratio nu', 'Yield stress', 'Hardening coefficient']
+
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
 
-        self.data_keys = ['Young\'s modulus E', 'Poisson\'s ratio nu', 'Yield stress', 'Hardening coefficient']
+        self.data_keys = self.__data_keys__
 
         if len(self.material.data) != len(self.data_keys):
             raise NotImplementedError(error_style(self.get_data_length_error_msg()))
         else:
             for i, key in enumerate(self.data_keys):
                 self.data_dict[key] = material.data[i]
```

### Comparing `pyfem-0.2.1/src/pyfem/materials/ViscoElasticMaxwell.py` & `pyfem-0.2.2/src/pyfem/materials/ViscoElasticMaxwell.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,19 +100,21 @@
         'TAU2': ('float', '第2个粘弹性单元的时间系数'),
         'TAU3': ('float', '第3个粘弹性单元的时间系数'),
         'nu': ('float', '泊松比')
     }
 
     __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
+    __data_keys__ = ['E0', 'Poisson\'s ratio nu', 'E1', 'TAU1', 'E2', 'TAU2', 'E3', 'TAU3']
+
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
 
-        self.data_keys = ['E0', 'Poisson\'s ratio nu', 'E1', 'TAU1', 'E2', 'TAU2', 'E3', 'TAU3']
+        self.data_keys = self.__data_keys__
 
         if len(self.material.data) != len(self.data_keys):
             raise NotImplementedError(error_style(self.get_data_length_error_msg()))
         else:
             for i, key in enumerate(self.data_keys):
                 self.data_dict[key] = material.data[i]
```

### Comparing `pyfem-0.2.1/src/pyfem/materials/crystal_slip_system.py` & `pyfem-0.2.2/src/pyfem/materials/crystal_slip_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,14 @@
 
 将 :math:`D_{{\text{HCP}}}` 乘以 :math:`{{a}^2}` ，即得到与三轴坐标系晶面法向指数和三轴坐标系平面指数转换矩阵 :math:`T` 相同的形式。
 
 **参考书：材料科学基础-第2版-余永宁，P35-48**
 
 """
 
-import re
 from math import sqrt
 
 from numpy import array, ndarray, zeros, dot, transpose
 from numpy.linalg import norm
 
 from pyfem.fem.constants import DTYPE
 from pyfem.utils.colors import error_style
```

### Comparing `pyfem-0.2.1/src/pyfem/materials/get_material_data.py` & `pyfem-0.2.2/src/pyfem/materials/get_material_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,22 +43,30 @@
         dimension(int): 空间维度
         section(Section): 截面属性
 
     :return: 材料对象
     :rtype: MaterialData
     """
 
-    class_name = f'{material.category}{material.type}'.strip().replace(' ', '')
+    if material.user_path is not None:
+        import importlib.util
+        spec = importlib.util.spec_from_file_location('User', material.user_path)
+        user_material = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(user_material)
+        return user_material.User(material, dimension, section)
 
-    if class_name in material_data_dict:
-        return material_data_dict[class_name](material, dimension, section)
     else:
-        error_msg = f'{class_name} material is not supported.\n'
-        error_msg += f'The allowed material types are {list(material_data_dict.keys())}.'
-        raise NotImplementedError(error_style(error_msg))
+        class_name = f'{material.category}{material.type}'.strip().replace(' ', '')
+
+        if class_name in material_data_dict:
+            return material_data_dict[class_name](material, dimension, section)
+        else:
+            error_msg = f'{class_name} material is not supported.\n'
+            error_msg += f'The allowed material types are {list(material_data_dict.keys())}.'
+            raise NotImplementedError(error_style(error_msg))
 
 
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
     props = Properties()
     props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
```

### Comparing `pyfem-0.2.1/src/pyfem/mesh/MeshData.py` & `pyfem-0.2.2/src/pyfem/mesh/MeshData.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/quadrature/BaseQuadrature.py` & `pyfem-0.2.2/src/pyfem/quadrature/BaseQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/quadrature/GaussLegendreQuadrature.py` & `pyfem-0.2.2/src/pyfem/quadrature/GaussLegendreQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/quadrature/PyramidQuadrature.py` & `pyfem-0.2.2/src/pyfem/quadrature/PyramidQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/quadrature/TetrahedronQuadrature.py` & `pyfem-0.2.2/src/pyfem/quadrature/TetrahedronQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py` & `pyfem-0.2.2/src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     __slots__ = BaseQuadrature.__slots__ + []
 
     def __init__(self, order: int, dimension: int) -> None:
         dimension = 3
         super().__init__(order, dimension)
         if order == 1:  # order 1, qp_number 1
             qp_coords_and_weights = array([
-                [0.2500000000000000,	0.2500000000000000,	0.2500000000000000,	0.2500000000000000,	1.0000000000000000]], dtype=DTYPE)
+                [0.2500000000000000, 0.2500000000000000, 0.2500000000000000, 0.2500000000000000, 1.0000000000000000]], dtype=DTYPE)
         elif order == 2:  # order 2, qp_number 4
             qp_coords_and_weights = array([
                 [0.5854101966249680, 0.1381966011250110, 0.1381966011250110, 0.1381966011250110, 0.2500000000000000],
                 [0.1381966011250110, 0.5854101966249680, 0.1381966011250110, 0.1381966011250110, 0.2500000000000000],
                 [0.1381966011250110, 0.1381966011250110, 0.5854101966249680, 0.1381966011250110, 0.2500000000000000],
                 [0.1381966011250110, 0.1381966011250110, 0.1381966011250110, 0.5854101966249680, 0.2500000000000000]], dtype=DTYPE)
         elif order == 3:  # order 3, qp_number 10
```

### Comparing `pyfem-0.2.1/src/pyfem/quadrature/TriangleQuadrature.py` & `pyfem-0.2.2/src/pyfem/quadrature/TriangleQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/quadrature/TriangleQuadratureBarycentric.py` & `pyfem-0.2.2/src/pyfem/quadrature/TriangleQuadratureBarycentric.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/solvers/ArcLengthSolver.py` & `pyfem-0.2.2/src/pyfem/solvers/ArcLengthSolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,16 @@
 
                 if f_residual < self.FORCE_TOL:
                     is_convergence = True
                     break
 
             if is_convergence:
                 logger.info(f'  increment {increment} is convergence')
-                logger_sta.info(f'{1:4}  {increment:9}  {attempt:3}  {0:6}  {niter:5}  {niter:5}  {timer.time1:14.6f}  {timer.time1:14.6f}  {timer.dtime:14.6f}')
+                logger_sta.info(
+                    f'{1:4}  {increment:9}  {attempt:3}  {0:6}  {niter:5}  {niter:5}  {timer.time1:14.6f}  {timer.time1:14.6f}  {timer.dtime:14.6f}')
 
                 self.assembly.update_element_data()
                 self.assembly.dof_solution += self.assembly.ddof_solution
                 # 调换了上面两行代码的顺序，基于t时刻的自由度值及t+dt时刻的自由度增量值对单元信息进行更新，之后在将所有单元的自由度值更新为t+dt时刻。
 
                 self.assembly.update_element_state_variables()
                 self.assembly.update_element_field_variables()
@@ -294,14 +295,15 @@
     from pyfem.utils.visualization import print_slots_dict
 
     print_slots_dict(ArcLengthSolver.__slots_dict__)
 
     from pyfem.Job import Job
 
     import numpy as np
+
     np.set_printoptions(precision=5, suppress=True, linewidth=10000)
 
     job = Job(r'..\..\..\examples\mechanical\beam\Job-1.toml')
     # job = Job(r'..\..\..\examples\mechanical\1element\quad4\Job-1.toml')
     # solver = NonlinearSolver(job.assembly, job.props.solver)
     # solver.show()
     job.run()
```

### Comparing `pyfem-0.2.1/src/pyfem/solvers/BaseSolver.py` & `pyfem-0.2.2/src/pyfem/solvers/BaseSolver.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from numpy import ndarray, empty
 
 from pyfem.assembly.Assembly import Assembly
+from pyfem.database.Database import Database
 from pyfem.io.Solver import Solver
 from pyfem.utils.visualization import object_slots_to_string_ndarray
 
 
 class BaseSolver:
     """
     求解器基类。
@@ -22,23 +23,25 @@
     :ivar dof_solution: 求解得到自由度的值
     :vartype dof_solution: ndarray
     """
 
     __slots_dict__: dict = {
         'assembly': ('Assembly', '装配体对象'),
         'solver': ('Solver', '求解器属性'),
-        'dof_solution': ('ndarray', '求解得到自由度的值')
+        'dof_solution': ('ndarray', '求解得到自由度的值'),
+        'database': ('Database', '数据库对象，用于输出计算结果')
     }
 
     __slots__: list = [slot for slot in __slots_dict__.keys()]
 
     def __init__(self) -> None:
         self.assembly: Assembly = None  # type: ignore
         self.solver: Solver = None  # type: ignore
         self.dof_solution: ndarray = empty(0)
+        self.database: Database = None  # type: ignore
 
     def to_string(self, level: int = 1) -> str:
         return object_slots_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
```

### Comparing `pyfem-0.2.1/src/pyfem/solvers/LinearSolver.py` & `pyfem-0.2.2/src/pyfem/solvers/LinearSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/solvers/NonlinearSolver.py` & `pyfem-0.2.2/src/pyfem/solvers/NonlinearSolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-import time
 from copy import deepcopy
 
 from numpy import zeros
 from numpy.linalg import norm
 from scipy.sparse.linalg import splu  # type: ignore
 
 from pyfem.assembly.Assembly import Assembly
+from pyfem.database.Database import Database
 from pyfem.fem.constants import DTYPE, IS_PETSC
 from pyfem.io.Solver import Solver
 from pyfem.io.write_vtk import write_vtk, write_pvd
 from pyfem.solvers.BaseSolver import BaseSolver
 from pyfem.utils.colors import error_style
 from pyfem.utils.logger import logger, logger_sta
 
@@ -60,14 +60,15 @@
     __slots__ = BaseSolver.__slots__ + [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, assembly: Assembly, solver: Solver) -> None:
         super().__init__()
         self.assembly = assembly
         self.solver = solver
         self.dof_solution = zeros(self.assembly.total_dof_number)
+        self.database = Database(self.assembly)
         self.PENALTY: float = 1.0e128
         self.FORCE_TOL: float = 1.0e-3
         self.MAX_NITER: int = 16
         self.BC_METHOD: str = '01'
 
     def run(self) -> int:
         if self.assembly.props.solver.option in [None, '', 'NR', 'NewtonRaphson']:
@@ -84,14 +85,15 @@
         timer.dtime = self.solver.initial_dtime
         timer.time0 = self.solver.start_time
         timer.increment = 0
         timer.frame_ids.append(0)
 
         self.assembly.update_element_field_variables()
         self.assembly.assembly_field_variables()
+        self.database.init_hdf5()
         for output in self.assembly.props.outputs:
             if output.is_save:
                 if output.type == 'vtk':
                     write_vtk(self.assembly)
 
         increment: int = 1
         attempt: int = 1
@@ -159,15 +161,15 @@
                                         rhs[bc_dof_id] = bc_dof_value * amplitude_increment + fint[bc_dof_id]
                                     # rhs -= sum((self.assembly.A.getValues(range(self.assembly.total_dof_number), bc_data.bc_dof_ids) * bc_data.bc_dof_values * amplitude_increment), axis=1)
                                     # rhs[bc_data.bc_dof_ids] = bc_data.bc_dof_values * amplitude_increment + fint[bc_data.bc_dof_ids]
                             elif bc_data.bc.category == 'NeumannBC':
                                 if IS_PETSC:
                                     b.setValues(bc_data.bc_dof_ids, bc_data.bc_fext * amplitude_increment, addv=True)
                                     self.assembly.fext[bc_data.bc_dof_ids] += bc_data.bc_fext * amplitude_increment
-                                # else:
+                                else:
                                     for bc_dof_id, bc_fext in zip(bc_data.bc_dof_ids, bc_data.bc_fext):
                                         rhs[bc_dof_id] += bc_fext * amplitude_increment
                                         self.assembly.fext[bc_dof_id] += bc_fext * amplitude_increment
 
                     else:
                         for bc_data in self.assembly.bc_data_list:
                             if bc_data.bc.category == 'DirichletBC':
@@ -234,25 +236,27 @@
 
                 if f_residual < self.FORCE_TOL:
                     is_convergence = True
                     break
 
             if is_convergence:
                 logger.info(f'  increment {increment} is convergence')
-                logger_sta.info(f'{1:4}  {increment:9}  {attempt:3}  {0:6}  {niter:5}  {niter:5}  {timer.time1:14.6f}  {timer.time1:14.6f}  {timer.dtime:14.6f}')
+                logger_sta.info(
+                    f'{1:4}  {increment:9}  {attempt:3}  {0:6}  {niter:5}  {niter:5}  {timer.time1:14.6f}  {timer.time1:14.6f}  {timer.dtime:14.6f}')
 
                 self.assembly.update_element_data()
                 self.assembly.dof_solution += self.assembly.ddof_solution
                 # 调换了上面两行代码的顺序，基于t时刻的自由度值及t+dt时刻的自由度增量值对单元信息进行更新，之后在将所有单元的自由度值更新为t+dt时刻。
 
                 self.assembly.update_element_state_variables()
                 self.assembly.update_element_field_variables()
                 self.assembly.assembly_field_variables()
 
                 # time0 = time.time()
+                self.database.add_hdf5()
                 for output in self.assembly.props.outputs:
                     if output.is_save:
                         if output.type == 'vtk':
                             write_vtk(self.assembly)
                 # time1 = time.time()
                 # print('write_vtk: ', time1 - time0)
 
@@ -302,14 +306,15 @@
     from pyfem.utils.visualization import print_slots_dict
 
     print_slots_dict(NonlinearSolver.__slots_dict__)
 
     from pyfem.Job import Job
 
     import numpy as np
+
     np.set_printoptions(precision=5, suppress=True, linewidth=10000)
 
     job = Job(r'..\..\..\examples\mechanical\beam\Job-1.toml')
     # job = Job(r'..\..\..\examples\mechanical\1element\quad4\Job-1.toml')
     # solver = NonlinearSolver(job.assembly, job.props.solver)
     # solver.show()
     job.run()
```

### Comparing `pyfem-0.2.1/src/pyfem/solvers/TimeIntegrationNonlinearSolver.py` & `pyfem-0.2.2/src/pyfem/solvers/TimeIntegrationNonlinearSolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-import time
 from copy import deepcopy
 
 from numpy import zeros
-from numpy.linalg import norm, det
+from numpy.linalg import norm
 from scipy.sparse.linalg import splu  # type: ignore
 
 from pyfem.assembly.Assembly import Assembly
 from pyfem.fem.constants import DTYPE, IS_PETSC
 from pyfem.io.Solver import Solver
 from pyfem.io.write_vtk import write_vtk, write_pvd
 from pyfem.solvers.BaseSolver import BaseSolver
@@ -110,15 +109,15 @@
             is_convergence = False
 
             for niter in range(self.MAX_NITER):
                 self.assembly.assembly_global_stiffness()
                 fint = deepcopy(self.assembly.fint)
                 fext = deepcopy(self.assembly.fext)
                 ftime = deepcopy(self.assembly.ftime)
-                rhs = fext + ftime
+                rhs = fext
                 # print(ftime)
 
                 # import numpy as np
                 # np.set_printoptions(precision=5, suppress=True, linewidth=10000)
                 # print(self.assembly.global_stiffness.A)
                 # print(rhs)
 
@@ -168,15 +167,15 @@
                                         rhs[bc_dof_id] = bc_dof_value * amplitude_increment + fint[bc_dof_id]
                                     # rhs -= sum((self.assembly.A.getValues(range(self.assembly.total_dof_number), bc_data.bc_dof_ids) * bc_data.bc_dof_values * amplitude_increment), axis=1)
                                     # rhs[bc_data.bc_dof_ids] = bc_data.bc_dof_values * amplitude_increment + fint[bc_data.bc_dof_ids]
                             elif bc_data.bc.category == 'NeumannBC':
                                 if IS_PETSC:
                                     b.setValues(bc_data.bc_dof_ids, bc_data.bc_fext * amplitude_increment, addv=True)
                                     self.assembly.fext[bc_data.bc_dof_ids] += bc_data.bc_fext * amplitude_increment
-                                # else:
+                                    # else:
                                     for bc_dof_id, bc_fext in zip(bc_data.bc_dof_ids, bc_data.bc_fext):
                                         rhs[bc_dof_id] += bc_fext * amplitude_increment
                                         self.assembly.fext[bc_dof_id] += bc_fext * amplitude_increment
 
                     else:
                         for bc_data in self.assembly.bc_data_list:
                             if bc_data.bc.category == 'DirichletBC':
@@ -213,15 +212,15 @@
                         self.assembly.global_stiffness = self.assembly.global_stiffness.tocsc()
 
                         # import numpy as np
                         # np.set_printoptions(precision=3, suppress=True, linewidth=10000)
                         # print(self.assembly.global_stiffness.A)
                         # print(rhs)
                         LU = splu(self.assembly.global_stiffness)
-                        da = LU.solve(rhs)
+                        da = LU.solve(rhs - fint)
                         # print(da)
                         # print(self.assembly.dof_solution)
                         # print(self.assembly.ddof_solution)
 
                 except RuntimeError as e:
                     is_convergence = False
                     print(error_style(f"Catch RuntimeError exception: {e}"))
@@ -256,15 +255,16 @@
                 break
                 # if f_residual < self.FORCE_TOL:
                 #     is_convergence = True
                 #     break
 
             if is_convergence:
                 logger.info(f'  increment {increment} is convergence')
-                logger_sta.info(f'{1:4}  {increment:9}  {attempt:3}  {0:6}  {niter:5}  {niter:5}  {timer.time1:14.6f}  {timer.time1:14.6f}  {timer.dtime:14.6f}')
+                logger_sta.info(
+                    f'{1:4}  {increment:9}  {attempt:3}  {0:6}  {niter:5}  {niter:5}  {timer.time1:14.6f}  {timer.time1:14.6f}  {timer.dtime:14.6f}')
 
                 self.assembly.update_element_data()
                 self.assembly.dof_solution += self.assembly.ddof_solution
                 # 调换了上面两行代码的顺序，基于t时刻的自由度值及t+dt时刻的自由度增量值对单元信息进行更新，之后在将所有单元的自由度值更新为t+dt时刻。
 
                 self.assembly.update_element_state_variables()
                 self.assembly.update_element_field_variables()
@@ -324,14 +324,15 @@
     from pyfem.utils.visualization import print_slots_dict
 
     print_slots_dict(TimeIntegrationNonlinearSolver.__slots_dict__)
 
     from pyfem.Job import Job
 
     import numpy as np
+
     np.set_printoptions(precision=5, suppress=True, linewidth=10000)
 
     job = Job(r'..\..\..\examples\mechanical\beam\Job-1.toml')
     # job = Job(r'..\..\..\examples\mechanical\1element\quad4\Job-1.toml')
     # solver = NonlinearSolver(job.assembly, job.props.solver)
     # solver.show()
     job.run()
```

### Comparing `pyfem-0.2.1/src/pyfem/solvers/get_solver_data.py` & `pyfem-0.2.2/src/pyfem/solvers/get_solver_data.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 """
 
 """
 from typing import Union
 
 from pyfem.assembly.Assembly import Assembly
 from pyfem.io.Solver import Solver
+from pyfem.solvers.ArcLengthSolver import ArcLengthSolver
 from pyfem.solvers.BaseSolver import BaseSolver
 from pyfem.solvers.LinearSolver import LinearSolver
 from pyfem.solvers.NonlinearSolver import NonlinearSolver
 from pyfem.solvers.TimeIntegrationNonlinearSolver import TimeIntegrationNonlinearSolver
-from pyfem.solvers.ArcLengthSolver import ArcLengthSolver
 from pyfem.utils.colors import error_style
 
 SolverData = Union[BaseSolver, LinearSolver, NonlinearSolver, ArcLengthSolver]
 
 solver_data_dict = {
     'LinearSolver': LinearSolver,
     'NonlinearSolver': NonlinearSolver,
```

### Comparing `pyfem-0.2.1/src/pyfem/utils/IntKeyDict.py` & `pyfem-0.2.2/src/pyfem/utils/IntKeyDict.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/utils/colors.py` & `pyfem-0.2.2/src/pyfem/utils/colors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 定义色彩关键字，用于对字符串着色。
 """
 import os
+
 import colorlog
 
 from pyfem.fem.constants import IS_DEBUG
 
 IS_COLORED = True
 
 if os.environ.get('TERM', '') != '' or IS_COLORED:
@@ -26,14 +27,16 @@
     GREEN = ''
     YELLOW = ''
     RED = ''
     BOLD = ''
     UNDERLINE = ''
     END = ''
 
+c = colorlog.__all__
+
 
 def error_style(error_msg: str) -> str:
     if IS_DEBUG:
         return RED + BOLD + '\nPYFEM ERROR:\n' + error_msg + END
     else:
         return '\nPYFEM ERROR:\n' + error_msg
```

### Comparing `pyfem-0.2.1/src/pyfem/utils/logger.py` & `pyfem-0.2.2/src/pyfem/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/utils/mechanics.py` & `pyfem-0.2.2/src/pyfem/utils/mechanics.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/utils/visualization.py` & `pyfem-0.2.2/src/pyfem/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem/utils/wrappers.py` & `pyfem-0.2.2/src/pyfem/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.1/src/pyfem.egg-info/PKG-INFO` & `pyfem-0.2.2/src/pyfem.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Finite Element Method
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: meshio
+Requires-Dist: tomli
+Requires-Dist: colorlog
+Requires-Dist: sympy
+Requires-Dist: tomli_w
 
 # pyfem
 
 pyfem是一个完全基于python语言实现的极简有限元求解器。依赖的第三方库包括numpy、scipy和meshio等，主要用于有限元方法的学习、有限元算法验证和快速建立材料本构模型的程序原型。
 
 Github仓库：https://github.com/sunwhale/pyfem
 
@@ -106,15 +113,15 @@
 
 
 ## Development 开发
 
 ### ToDo list
 
 - [ ] 增加如何建立toml算例文件的帮助文档
-- [ ] 增加hdf5计算结果输出格式
+- [x] 增加hdf5计算结果输出格式
 - [ ] 处理平面应力状态的面外应力平衡
 - [ ] 增加内聚区单元
 - [ ] 增加动力学求解器
 - [ ] 建立前处理界面
 
 ### Bug list
```

### Comparing `pyfem-0.2.1/src/pyfem.egg-info/SOURCES.txt` & `pyfem-0.2.2/src/pyfem.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 src/pyfem/bc/DirichletBC.py
 src/pyfem/bc/NeumannBCConcentrated.py
 src/pyfem/bc/NeumannBCDistributed.py
 src/pyfem/bc/NeumannBCPressure.py
 src/pyfem/bc/__init__.py
 src/pyfem/bc/derive_surface_integral.py
 src/pyfem/bc/get_bc_data.py
+src/pyfem/database/Database.py
+src/pyfem/database/__init__.py
 src/pyfem/elements/BaseElement.py
 src/pyfem/elements/Diffusion.py
 src/pyfem/elements/SolidFiniteStrain.py
 src/pyfem/elements/SolidPhaseDamageSmallStrain.py
 src/pyfem/elements/SolidSmallStrain.py
 src/pyfem/elements/SolidThermalSmallStrain.py
 src/pyfem/elements/Thermal.py
@@ -38,23 +40,21 @@
 src/pyfem/fem/constants.py
 src/pyfem/io/Amplitude.py
 src/pyfem/io/BC.py
 src/pyfem/io/BaseIO.py
 src/pyfem/io/Dof.py
 src/pyfem/io/Material.py
 src/pyfem/io/Mesh.py
-src/pyfem/io/Module.py
 src/pyfem/io/Output.py
 src/pyfem/io/Parameter.py
 src/pyfem/io/Properties.py
 src/pyfem/io/Section.py
 src/pyfem/io/Solver.py
 src/pyfem/io/__init__.py
 src/pyfem/io/arguments.py
-src/pyfem/io/write_hdf5.py
 src/pyfem/io/write_vtk.py
 src/pyfem/isoelements/IsoElementDiagram.py
 src/pyfem/isoelements/IsoElementShape.py
 src/pyfem/isoelements/__init__.py
 src/pyfem/isoelements/derive_shape_functions.py
 src/pyfem/isoelements/get_iso_element_type.py
 src/pyfem/isoelements/shape_functions.py
@@ -63,15 +63,14 @@
 src/pyfem/materials/ElasticIsotropic.py
 src/pyfem/materials/MechanicalThermalExpansion.py
 src/pyfem/materials/PhaseFieldDamage.py
 src/pyfem/materials/PlasticCrystal.py
 src/pyfem/materials/PlasticCrystalGNDs.py
 src/pyfem/materials/PlasticKinematicHardening.py
 src/pyfem/materials/ThermalIsotropic.py
-src/pyfem/materials/UMAT.py
 src/pyfem/materials/ViscoElasticMaxwell.py
 src/pyfem/materials/__init__.py
 src/pyfem/materials/crystal_slip_system.py
 src/pyfem/materials/get_material_data.py
 src/pyfem/mesh/MeshData.py
 src/pyfem/mesh/__init__.py
 src/pyfem/quadrature/BaseQuadrature.py
```

