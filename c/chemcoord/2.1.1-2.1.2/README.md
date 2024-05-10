# Comparing `tmp/chemcoord-2.1.1.tar.gz` & `tmp/chemcoord-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemcoord-2.1.1.tar", last modified: Tue May  7 13:59:41 2024, max compression
+gzip compressed data, was "chemcoord-2.1.2.tar", last modified: Fri May 10 11:31:49 2024, max compression
```

## Comparing `chemcoord-2.1.1.tar` & `chemcoord-2.1.2.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.052855 chemcoord-2.1.1/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      309 2024-05-06 18:47:43.000000 chemcoord-2.1.1/CHANGELOG.md
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7644 2023-06-19 10:17:01.000000 chemcoord-2.1.1/LICENSE.md
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       77 2023-06-19 10:17:01.000000 chemcoord-2.1.1/MANIFEST.in
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     6577 2024-05-07 13:59:41.052855 chemcoord-2.1.1/PKG-INFO
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5169 2024-05-07 13:52:06.000000 chemcoord-2.1.1/README.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.032854 chemcoord-2.1.1/docs/
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.032854 chemcoord-2.1.1/docs/source/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      858 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/bugs_and_contributors.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      965 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/cartesian_coordinates.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1081 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/configuration.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      190 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/documentation.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      275 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/exceptions.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3157 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/index.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1079 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/installation.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      690 2023-08-02 12:14:08.000000 chemcoord-2.1.1/docs/source/internal_coordinates.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7445 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/license.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1381 2023-08-02 12:14:08.000000 chemcoord-2.1.1/docs/source/references.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.032854 chemcoord-2.1.1/docs/source/src_AsymmetricUnitCartesian/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3330 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.036855 chemcoord-2.1.1/docs/source/src_AsymmetricUnitCartesian/src_AsymmetricUnitCartesian/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      196 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_AsymmetricUnitCartesian/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.get_cartesian.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.036855 chemcoord-2.1.1/docs/source/src_Cartesian/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2291 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/chemcoord.Cartesian.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.040855 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.__init__.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._divide_et_impera.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      162 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._preserve_bonds.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.add_data.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      128 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.align.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      155 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.basistransform.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      163 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.change_numbering.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      174 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_absolute_refs.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      157 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_dihedral.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      136 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.columns.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      125 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.copy.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.correct_absolute_refs.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      163 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.correct_dihedral.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.cut_cuboid.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.cut_sphere.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      146 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.fragmentate.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      159 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.from_ase_atoms.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      183 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.from_pymatgen_molecule.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      168 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_angle_degrees.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      156 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_ase_atoms.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      174 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_asymmetric_unit.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      157 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_barycenter.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      165 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_bond_lengths.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_bonds.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      151 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_centroid.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      183 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_construction_table.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      186 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_coordination_sphere.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      177 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_dihedral_degrees.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      162 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_distance_to.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      174 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_electron_number.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      177 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_equivalent_atoms.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      151 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_fragment.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      156 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_grad_zmat.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_inertia.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      157 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_pointgroup.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_pymatgen_molecule.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_shortest_distance.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      159 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_total_mass.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_without.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_zmat.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.iloc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      130 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.index.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      131 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.insert.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      124 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.loc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      171 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.partition_chem_env.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.read_cjson.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.read_xyz.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      160 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.reindex_similar.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      134 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.replace.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      171 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.restrict_bond_dict.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.set_index.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.sort_index.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.sort_values.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      125 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.subs.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      143 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.symmetrize.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_cjson.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_latex.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_string.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      133 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_xyz.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      136 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_zmat.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      125 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.view.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.write_xyz.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.040855 chemcoord-2.1.1/docs/source/src_PointGroupOperations/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      651 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_PointGroupOperations/chemcoord.PointGroupOperations.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.040855 chemcoord-2.1.1/docs/source/src_Zmat/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1050 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/chemcoord.Zmat.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.044855 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      130 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.__init__.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      124 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.add_data.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.change_numbering.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.columns.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      110 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.copy.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      118 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.dtypes.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_cartesian.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      159 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_electron_number.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      156 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_grad_cartesian.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      144 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_total_mass.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      160 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.has_same_sumformula.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      112 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.iloc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.index.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      116 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.insert.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      122 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.iupacify.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      109 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.loc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      154 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.minimize_dihedrals.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.read_zmat.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.safe_iloc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      126 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.safe_loc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.shape.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      130 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.sort_index.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      133 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.sort_values.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      110 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.subs.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      124 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_latex.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_string.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      118 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_xyz.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_zmat.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.unsafe_iloc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.unsafe_loc.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      113 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.write.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.044855 chemcoord-2.1.1/docs/source/src_configuration/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      189 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_configuration/chemcoord.configuration.read_configuration_file.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      192 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_configuration/chemcoord.configuration.write_configuration_file.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.044855 chemcoord-2.1.1/docs/source/src_exceptions/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      183 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/src_exceptions/chemcoord.exceptions.IllegalArgumentCombination.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/src_exceptions/chemcoord.exceptions.InvalidReference.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      150 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/src_exceptions/chemcoord.exceptions.PhysicalMeaning.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2023-06-19 10:17:01.000000 chemcoord-2.1.1/docs/source/src_exceptions/chemcoord.exceptions.UndefinedCoordinateSystem.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.048855 chemcoord-2.1.1/docs/source/src_xyz_functions/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.allclose.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      190 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.apply_grad_zmat_tensor.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      136 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.concat.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.dot.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.isclose.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.read_molden.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      147 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.to_molden.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      130 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.view.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      156 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_xyz_functions/chemcoord.xyz_functions.write_molden.rst
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.048855 chemcoord-2.1.1/docs/source/src_zmat_functions/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      310 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_zmat_functions/chemcoord.zmat_functions.DummyManipulation.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      322 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_zmat_functions/chemcoord.zmat_functions.PureInternalMovement.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      294 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_zmat_functions/chemcoord.zmat_functions.TestOperators.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      208 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/src_zmat_functions/chemcoord.zmat_functions.apply_grad_cartesian_tensor.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      896 2024-05-06 18:47:43.000000 chemcoord-2.1.1/docs/source/tutorial.rst
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       38 2024-05-07 13:59:41.052855 chemcoord-2.1.1/setup.cfg
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2122 2024-05-07 12:40:00.000000 chemcoord-2.1.1/setup.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.032854 chemcoord-2.1.1/src/
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.048855 chemcoord-2.1.1/src/chemcoord/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1187 2023-08-04 15:24:20.000000 chemcoord-2.1.1/src/chemcoord/__init__.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.048855 chemcoord-2.1.1/src/chemcoord/_generic_classes/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/_generic_classes/__init__.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      490 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/_generic_classes/generic_IO.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3058 2023-08-04 15:24:20.000000 chemcoord-2.1.1/src/chemcoord/_generic_classes/generic_core.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.052855 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/__init__.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    49629 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cart_transformation.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    52118 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_core.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    32242 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_get_zmat.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    14356 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_io.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    10567 2023-08-04 15:24:20.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_pandas_wrapper.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4657 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_symmetry.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4092 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_indexers.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1411 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/asymmetric_unit_cartesian_class.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3277 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/cartesian_class_main.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      989 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/point_group.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    16476 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/xyz_functions.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3385 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/configuration.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    67997 2023-08-04 15:24:20.000000 chemcoord-2.1.1/src/chemcoord/constants.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2257 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/exceptions.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.052855 chemcoord-2.1.1/src/chemcoord/internal_coordinates/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/__init__.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4134 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/_indexers.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    31099 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_class_core.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7583 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_class_io.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3027 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_class_pandas_wrapper.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5573 2023-08-04 15:24:20.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_transformation.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3182 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/zmat_class_main.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4390 2023-08-02 12:14:08.000000 chemcoord-2.1.1/src/chemcoord/internal_coordinates/zmat_functions.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.052855 chemcoord-2.1.1/src/chemcoord/utilities/
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/utilities/__init__.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3365 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/utilities/_decorators.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4591 2023-06-19 10:17:01.000000 chemcoord-2.1.1/src/chemcoord/utilities/_print_versions.py
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      850 2024-05-06 18:47:43.000000 chemcoord-2.1.1/src/chemcoord/utilities/_temporary_deprecation_workarounds.py
-drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-07 13:59:41.052855 chemcoord-2.1.1/src/chemcoord.egg-info/
--rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     6577 2024-05-07 13:59:41.000000 chemcoord-2.1.1/src/chemcoord.egg-info/PKG-INFO
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    10525 2024-05-07 13:59:41.000000 chemcoord-2.1.1/src/chemcoord.egg-info/SOURCES.txt
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        1 2024-05-07 13:59:41.000000 chemcoord-2.1.1/src/chemcoord.egg-info/dependency_links.txt
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       77 2024-05-07 13:59:41.000000 chemcoord-2.1.1/src/chemcoord.egg-info/requires.txt
--rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       10 2024-05-07 13:59:41.000000 chemcoord-2.1.1/src/chemcoord.egg-info/top_level.txt
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.913784 chemcoord-2.1.2/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      324 2024-05-10 11:30:37.000000 chemcoord-2.1.2/CHANGELOG.md
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7644 2023-06-19 10:17:01.000000 chemcoord-2.1.2/LICENSE.md
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       77 2023-06-19 10:17:01.000000 chemcoord-2.1.2/MANIFEST.in
+-rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     6612 2024-05-10 11:31:49.913784 chemcoord-2.1.2/PKG-INFO
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5225 2024-05-10 11:30:37.000000 chemcoord-2.1.2/README.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.797781 chemcoord-2.1.2/docs/
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.809781 chemcoord-2.1.2/docs/source/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      858 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/bugs_and_contributors.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      965 2023-06-19 10:17:01.000000 chemcoord-2.1.2/docs/source/cartesian_coordinates.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1081 2023-06-19 10:17:01.000000 chemcoord-2.1.2/docs/source/configuration.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      190 2023-06-19 10:17:01.000000 chemcoord-2.1.2/docs/source/documentation.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      275 2023-06-19 10:17:01.000000 chemcoord-2.1.2/docs/source/exceptions.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3157 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1079 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/installation.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      690 2023-08-02 12:14:08.000000 chemcoord-2.1.2/docs/source/internal_coordinates.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7445 2023-06-19 10:17:01.000000 chemcoord-2.1.2/docs/source/license.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1381 2023-08-02 12:14:08.000000 chemcoord-2.1.2/docs/source/references.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.809781 chemcoord-2.1.2/docs/source/src_AsymmetricUnitCartesian/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3330 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.809781 chemcoord-2.1.2/docs/source/src_AsymmetricUnitCartesian/src_AsymmetricUnitCartesian/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      196 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_AsymmetricUnitCartesian/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.get_cartesian.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.809781 chemcoord-2.1.2/docs/source/src_Cartesian/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2291 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/chemcoord.Cartesian.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.869783 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.__init__.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      170 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._divide_et_impera.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      162 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian._preserve_bonds.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.add_data.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      128 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.align.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      155 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.basistransform.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      163 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.change_numbering.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      174 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_absolute_refs.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      157 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.check_dihedral.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      136 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.columns.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      125 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.copy.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.correct_absolute_refs.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      163 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.correct_dihedral.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.cut_cuboid.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.cut_sphere.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      146 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.fragmentate.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      159 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.from_ase_atoms.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      183 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.from_pymatgen_molecule.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      168 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_angle_degrees.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      156 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_ase_atoms.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      174 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_asymmetric_unit.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      157 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_barycenter.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      165 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_bond_lengths.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_bonds.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      151 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_centroid.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      183 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_construction_table.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      186 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_coordination_sphere.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      177 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_dihedral_degrees.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      162 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_distance_to.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      174 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_electron_number.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      177 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_equivalent_atoms.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      151 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_fragment.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      156 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_grad_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_inertia.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      157 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_pointgroup.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_pymatgen_molecule.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_shortest_distance.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      159 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_total_mass.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_without.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.get_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.iloc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      130 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      131 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.insert.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      124 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.loc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      171 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.partition_chem_env.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.read_cjson.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.read_xyz.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      160 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.reindex_similar.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      134 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.replace.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      171 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.restrict_bond_dict.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.set_index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      145 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.sort_index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.sort_values.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      125 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.subs.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      143 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.symmetrize.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_cjson.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_latex.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_string.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      133 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_xyz.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      136 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.to_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      125 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.view.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Cartesian/src_Cartesian/chemcoord.Cartesian.write_xyz.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.869783 chemcoord-2.1.2/docs/source/src_PointGroupOperations/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      651 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_PointGroupOperations/chemcoord.PointGroupOperations.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.869783 chemcoord-2.1.2/docs/source/src_Zmat/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1050 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/chemcoord.Zmat.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.881783 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      130 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.__init__.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      124 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.add_data.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      148 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.change_numbering.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.columns.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      110 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.copy.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      118 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.dtypes.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_cartesian.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      159 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_electron_number.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      156 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_grad_cartesian.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      144 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.get_total_mass.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      160 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.has_same_sumformula.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      112 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.iloc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      116 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.insert.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      122 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.iupacify.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      109 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.loc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      154 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.minimize_dihedrals.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.read_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      129 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.safe_iloc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      126 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.safe_loc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      115 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.shape.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      130 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.sort_index.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      133 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.sort_values.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      110 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.subs.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      124 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_latex.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_string.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      118 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_xyz.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      121 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.to_zmat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      135 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.unsafe_iloc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      132 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.unsafe_loc.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      113 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_Zmat/src_Zmat/chemcoord.Zmat.write.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.881783 chemcoord-2.1.2/docs/source/src_configuration/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      189 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_configuration/chemcoord.configuration.read_configuration_file.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      192 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_configuration/chemcoord.configuration.write_configuration_file.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.881783 chemcoord-2.1.2/docs/source/src_exceptions/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      183 2023-06-19 10:17:01.000000 chemcoord-2.1.2/docs/source/src_exceptions/chemcoord.exceptions.IllegalArgumentCombination.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2023-06-19 10:17:01.000000 chemcoord-2.1.2/docs/source/src_exceptions/chemcoord.exceptions.InvalidReference.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      150 2023-06-19 10:17:01.000000 chemcoord-2.1.2/docs/source/src_exceptions/chemcoord.exceptions.PhysicalMeaning.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      180 2023-06-19 10:17:01.000000 chemcoord-2.1.2/docs/source/src_exceptions/chemcoord.exceptions.UndefinedCoordinateSystem.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.885783 chemcoord-2.1.2/docs/source/src_xyz_functions/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      142 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_xyz_functions/chemcoord.xyz_functions.allclose.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      190 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_xyz_functions/chemcoord.xyz_functions.apply_grad_zmat_tensor.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      136 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_xyz_functions/chemcoord.xyz_functions.concat.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      127 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_xyz_functions/chemcoord.xyz_functions.dot.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      139 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_xyz_functions/chemcoord.xyz_functions.isclose.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      153 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_xyz_functions/chemcoord.xyz_functions.read_molden.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      147 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_xyz_functions/chemcoord.xyz_functions.to_molden.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      130 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_xyz_functions/chemcoord.xyz_functions.view.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      156 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_xyz_functions/chemcoord.xyz_functions.write_molden.rst
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.889783 chemcoord-2.1.2/docs/source/src_zmat_functions/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      310 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_zmat_functions/chemcoord.zmat_functions.DummyManipulation.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      322 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_zmat_functions/chemcoord.zmat_functions.PureInternalMovement.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      294 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_zmat_functions/chemcoord.zmat_functions.TestOperators.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      208 2024-05-06 18:47:43.000000 chemcoord-2.1.2/docs/source/src_zmat_functions/chemcoord.zmat_functions.apply_grad_cartesian_tensor.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      896 2024-05-10 11:30:37.000000 chemcoord-2.1.2/docs/source/tutorial.rst
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       38 2024-05-10 11:31:49.913784 chemcoord-2.1.2/setup.cfg
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2113 2024-05-10 11:30:37.000000 chemcoord-2.1.2/setup.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.801781 chemcoord-2.1.2/src/
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.893783 chemcoord-2.1.2/src/chemcoord/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1187 2023-08-04 15:24:20.000000 chemcoord-2.1.2/src/chemcoord/__init__.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.897783 chemcoord-2.1.2/src/chemcoord/_generic_classes/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.2/src/chemcoord/_generic_classes/__init__.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      490 2023-08-02 12:14:08.000000 chemcoord-2.1.2/src/chemcoord/_generic_classes/generic_IO.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3058 2023-08-04 15:24:20.000000 chemcoord-2.1.2/src/chemcoord/_generic_classes/generic_core.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.905784 chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/__init__.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    49629 2024-05-06 18:47:43.000000 chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_cart_transformation.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    52118 2024-05-06 18:47:43.000000 chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_cartesian_class_core.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    32242 2024-05-06 18:47:43.000000 chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_cartesian_class_get_zmat.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    14356 2024-05-06 18:47:43.000000 chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_cartesian_class_io.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    10567 2023-08-04 15:24:20.000000 chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_cartesian_class_pandas_wrapper.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4657 2024-05-06 18:47:43.000000 chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_cartesian_class_symmetry.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4092 2024-05-06 18:47:43.000000 chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_indexers.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     1411 2023-08-02 12:14:08.000000 chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/asymmetric_unit_cartesian_class.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3277 2023-08-02 12:14:08.000000 chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/cartesian_class_main.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      989 2023-08-02 12:14:08.000000 chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/point_group.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    16476 2024-05-06 18:47:43.000000 chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/xyz_functions.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3385 2023-06-19 10:17:01.000000 chemcoord-2.1.2/src/chemcoord/configuration.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    67997 2023-08-04 15:24:20.000000 chemcoord-2.1.2/src/chemcoord/constants.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     2257 2023-06-19 10:17:01.000000 chemcoord-2.1.2/src/chemcoord/exceptions.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.909784 chemcoord-2.1.2/src/chemcoord/internal_coordinates/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.2/src/chemcoord/internal_coordinates/__init__.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4134 2024-05-06 18:47:43.000000 chemcoord-2.1.2/src/chemcoord/internal_coordinates/_indexers.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    31099 2024-05-06 18:47:43.000000 chemcoord-2.1.2/src/chemcoord/internal_coordinates/_zmat_class_core.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     7583 2024-05-06 18:47:43.000000 chemcoord-2.1.2/src/chemcoord/internal_coordinates/_zmat_class_io.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3027 2023-08-02 12:14:08.000000 chemcoord-2.1.2/src/chemcoord/internal_coordinates/_zmat_class_pandas_wrapper.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     5573 2023-08-04 15:24:20.000000 chemcoord-2.1.2/src/chemcoord/internal_coordinates/_zmat_transformation.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3182 2023-08-02 12:14:08.000000 chemcoord-2.1.2/src/chemcoord/internal_coordinates/zmat_class_main.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4390 2023-08-02 12:14:08.000000 chemcoord-2.1.2/src/chemcoord/internal_coordinates/zmat_functions.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.909784 chemcoord-2.1.2/src/chemcoord/utilities/
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        0 2023-06-19 10:17:01.000000 chemcoord-2.1.2/src/chemcoord/utilities/__init__.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     3365 2023-06-19 10:17:01.000000 chemcoord-2.1.2/src/chemcoord/utilities/_decorators.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)     4539 2024-05-10 11:30:37.000000 chemcoord-2.1.2/src/chemcoord/utilities/_print_versions.py
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)      850 2024-05-06 18:47:43.000000 chemcoord-2.1.2/src/chemcoord/utilities/_temporary_deprecation_workarounds.py
+drwxrwxr-x   0 mcocdawc  (1000) mcocdawc  (1000)        0 2024-05-10 11:31:49.913784 chemcoord-2.1.2/src/chemcoord.egg-info/
+-rw-r--r--   0 mcocdawc  (1000) mcocdawc  (1000)     6612 2024-05-10 11:31:49.000000 chemcoord-2.1.2/src/chemcoord.egg-info/PKG-INFO
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)    10525 2024-05-10 11:31:49.000000 chemcoord-2.1.2/src/chemcoord.egg-info/SOURCES.txt
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)        1 2024-05-10 11:31:49.000000 chemcoord-2.1.2/src/chemcoord.egg-info/dependency_links.txt
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       71 2024-05-10 11:31:49.000000 chemcoord-2.1.2/src/chemcoord.egg-info/requires.txt
+-rw-rw-r--   0 mcocdawc  (1000) mcocdawc  (1000)       10 2024-05-10 11:31:49.000000 chemcoord-2.1.2/src/chemcoord.egg-info/top_level.txt
```

### Comparing `chemcoord-2.1.1/LICENSE.md` & `chemcoord-2.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/PKG-INFO` & `chemcoord-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemcoord
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python module for dealing with chemical coordinates.
 Home-page: https://github.com/mcocdawc/chemcoord
 Author: Oskar Weser
 Author-email: oskar.weser@gmail.com
 License: LGPLv3
 Keywords: chemcoord,transformation,cartesian,internal,chemistry,zmatrix,xyz,zmat,coordinates,coordinate system
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 Requires-Dist: numpy>=1.0
-Requires-Dist: scipy
 Requires-Dist: pandas>=1.0
 Requires-Dist: numba>=0.35
 Requires-Dist: sortedcontainers
 Requires-Dist: sympy
 Requires-Dist: six
 Requires-Dist: pymatgen
 
@@ -38,15 +37,15 @@
 =======================================================
 
 
 .. list-table::
    :widths: 25 25
    :header-rows: 0
 
-   * - .. image:: https://github.com/mcocdawc/chemcoord/blob/v2.1.1/docs/source/_static/logo/chemcoord_logo.png
+   * - .. image:: https://raw.githubusercontent.com/mcocdawc/chemcoord/v2.1.2/docs/source/_static/logo/chemcoord_logo.png
               :align: center
               :width: 140
               :alt: Chemcoord logo
      -
    * - Latest Release
      - .. image:: https://img.shields.io/pypi/v/chemcoord.svg
             :target: https://pypi.python.org/pypi/chemcoord
@@ -170,14 +169,14 @@
 
 
 
 Acknowledgement
 ~~~~~~~~~~~~~~~
 
 
-.. image:: https://github.com/zulip/zulip/blob/main/static/images/logo/zulip-icon-circle.svg
+.. image:: https://raw.githubusercontent.com/zulip/zulip/982097f0a7fe2ecf46edc8756fc19f2a5c354ad7/static/images/logo/zulip-icon-circle.svg
    :width: 80
    :align: left
    :target: https://zulip.com/
 
 Zulip is an open-source modern team chat app designed to keep both live and asynchronous conversations organized,
 that supports the development of chemcoord with a free plan.
```

### Comparing `chemcoord-2.1.1/README.rst` & `chemcoord-2.1.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 =======================================================
 
 
 .. list-table::
    :widths: 25 25
    :header-rows: 0
 
-   * - .. image:: https://github.com/mcocdawc/chemcoord/blob/v2.1.1/docs/source/_static/logo/chemcoord_logo.png
+   * - .. image:: https://raw.githubusercontent.com/mcocdawc/chemcoord/v2.1.2/docs/source/_static/logo/chemcoord_logo.png
               :align: center
               :width: 140
               :alt: Chemcoord logo
      -
    * - Latest Release
      - .. image:: https://img.shields.io/pypi/v/chemcoord.svg
             :target: https://pypi.python.org/pypi/chemcoord
@@ -134,14 +134,14 @@
 
 
 
 Acknowledgement
 ~~~~~~~~~~~~~~~
 
 
-.. image:: https://github.com/zulip/zulip/blob/main/static/images/logo/zulip-icon-circle.svg
+.. image:: https://raw.githubusercontent.com/zulip/zulip/982097f0a7fe2ecf46edc8756fc19f2a5c354ad7/static/images/logo/zulip-icon-circle.svg
    :width: 80
    :align: left
    :target: https://zulip.com/
 
 Zulip is an open-source modern team chat app designed to keep both live and asynchronous conversations organized,
 that supports the development of chemcoord with a free plan.
```

### Comparing `chemcoord-2.1.1/docs/source/bugs_and_contributors.rst` & `chemcoord-2.1.2/docs/source/bugs_and_contributors.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/docs/source/cartesian_coordinates.rst` & `chemcoord-2.1.2/docs/source/cartesian_coordinates.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/docs/source/configuration.rst` & `chemcoord-2.1.2/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/docs/source/index.rst` & `chemcoord-2.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/docs/source/installation.rst` & `chemcoord-2.1.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/docs/source/internal_coordinates.rst` & `chemcoord-2.1.2/docs/source/internal_coordinates.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/docs/source/license.rst` & `chemcoord-2.1.2/docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/docs/source/references.rst` & `chemcoord-2.1.2/docs/source/references.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/docs/source/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.rst` & `chemcoord-2.1.2/docs/source/src_AsymmetricUnitCartesian/chemcoord.AsymmetricUnitCartesian.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/docs/source/src_Cartesian/chemcoord.Cartesian.rst` & `chemcoord-2.1.2/docs/source/src_Cartesian/chemcoord.Cartesian.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/docs/source/src_PointGroupOperations/chemcoord.PointGroupOperations.rst` & `chemcoord-2.1.2/docs/source/src_PointGroupOperations/chemcoord.PointGroupOperations.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/docs/source/src_Zmat/chemcoord.Zmat.rst` & `chemcoord-2.1.2/docs/source/src_Zmat/chemcoord.Zmat.rst`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/docs/source/tutorial.rst` & `chemcoord-2.1.2/docs/source/tutorial.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Tutorial
 ==================
 
 Just follow the link to the example notebooks.
 
 
-  * `Cartesian <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.1/Tutorial/Cartesian.ipynb>`_
-  * `Zmat <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.1/Tutorial/Zmat.ipynb>`_
-  * `Transformation <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.1/Tutorial/Transformation.ipynb>`_
-  * `Gradients <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.1/Tutorial/Gradients.ipynb>`_
-  * `Advanced customisation <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.1/Tutorial/Advanced_customisation.ipynb>`_
+  * `Cartesian <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.2/Tutorial/Cartesian.ipynb>`_
+  * `Zmat <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.2/Tutorial/Zmat.ipynb>`_
+  * `Transformation <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.2/Tutorial/Transformation.ipynb>`_
+  * `Gradients <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.2/Tutorial/Gradients.ipynb>`_
+  * `Advanced customisation <http://nbviewer.jupyter.org/github/mcocdawc/chemcoord/blob/v2.1.2/Tutorial/Advanced_customisation.ipynb>`_
 
 If you want to have an interactive session, just download the following
-`zip file <https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/mcocdawc/chemcoord/tree/v2.1.1/Tutorial>`_,
+`zip file <https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/mcocdawc/chemcoord/tree/v2.1.2/Tutorial>`_,
 which contains all notebooks and coordinates.
```

### Comparing `chemcoord-2.1.1/setup.py` & `chemcoord-2.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 MAIN_PACKAGE = 'chemcoord'
 DESCRIPTION = "Python module for dealing with chemical coordinates."
 LICENSE = 'LGPLv3'
 AUTHOR = 'Oskar Weser'
 EMAIL = 'oskar.weser@gmail.com'
 URL = 'https://github.com/mcocdawc/chemcoord'
-INSTALL_REQUIRES = ['numpy>=1.0', 'scipy', 'pandas>=1.0', 'numba>=0.35',
+INSTALL_REQUIRES = ['numpy>=1.0', 'pandas>=1.0', 'numba>=0.35',
                     'sortedcontainers', 'sympy', 'six', 'pymatgen']
 KEYWORDS = ['chemcoord', 'transformation', 'cartesian', 'internal',
             'chemistry', 'zmatrix', 'xyz', 'zmat', 'coordinates',
             'coordinate system']
 CLASSIFIERS = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
@@ -31,15 +31,15 @@
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Topic :: Scientific/Engineering :: Chemistry',
     'Topic :: Scientific/Engineering :: Physics']
-VERSION = '2.1.1'
+VERSION = '2.1.2'
 
 
 def readme():
     '''Return the contents of the README.md file.'''
     with open('README.rst') as freadme:
         return freadme.read()
```

### Comparing `chemcoord-2.1.1/src/chemcoord/__init__.py` & `chemcoord-2.1.2/src/chemcoord/__init__.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/_generic_classes/generic_core.py` & `chemcoord-2.1.2/src/chemcoord/_generic_classes/generic_core.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cart_transformation.py` & `chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_cart_transformation.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_core.py` & `chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_cartesian_class_core.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_get_zmat.py` & `chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_cartesian_class_get_zmat.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_io.py` & `chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_cartesian_class_io.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_pandas_wrapper.py` & `chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_cartesian_class_pandas_wrapper.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_cartesian_class_symmetry.py` & `chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_cartesian_class_symmetry.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/_indexers.py` & `chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/_indexers.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/asymmetric_unit_cartesian_class.py` & `chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/asymmetric_unit_cartesian_class.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/cartesian_class_main.py` & `chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/cartesian_class_main.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/point_group.py` & `chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/point_group.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/cartesian_coordinates/xyz_functions.py` & `chemcoord-2.1.2/src/chemcoord/cartesian_coordinates/xyz_functions.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/configuration.py` & `chemcoord-2.1.2/src/chemcoord/configuration.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/constants.py` & `chemcoord-2.1.2/src/chemcoord/constants.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/exceptions.py` & `chemcoord-2.1.2/src/chemcoord/exceptions.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/internal_coordinates/_indexers.py` & `chemcoord-2.1.2/src/chemcoord/internal_coordinates/_indexers.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_class_core.py` & `chemcoord-2.1.2/src/chemcoord/internal_coordinates/_zmat_class_core.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_class_io.py` & `chemcoord-2.1.2/src/chemcoord/internal_coordinates/_zmat_class_io.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_class_pandas_wrapper.py` & `chemcoord-2.1.2/src/chemcoord/internal_coordinates/_zmat_class_pandas_wrapper.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/internal_coordinates/_zmat_transformation.py` & `chemcoord-2.1.2/src/chemcoord/internal_coordinates/_zmat_transformation.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/internal_coordinates/zmat_class_main.py` & `chemcoord-2.1.2/src/chemcoord/internal_coordinates/zmat_class_main.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/internal_coordinates/zmat_functions.py` & `chemcoord-2.1.2/src/chemcoord/internal_coordinates/zmat_functions.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/utilities/_decorators.py` & `chemcoord-2.1.2/src/chemcoord/utilities/_decorators.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord/utilities/_print_versions.py` & `chemcoord-2.1.2/src/chemcoord/utilities/_print_versions.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 def show_versions(as_json=False):
     sys_info = get_sys_info()
 
     deps = [
         # (MODULE_NAME, f(mod) -> mod version)
         ("chemcoord", lambda mod: mod.__version__),
         ("numpy", lambda mod: mod.version.version),
-        ("scipy", lambda mod: mod.version.version),
         ("pandas", lambda mod: mod.__version__),
         ("numba", lambda mod: mod.__version__),
         ("sortedcontainers", lambda mod: mod.__version__),
         ("sympy", lambda mod: mod.__version__),
         ("pytest", lambda mod: mod.__version__),
         ("pip", lambda mod: mod.__version__),
         ("setuptools", lambda mod: mod.__version__),
```

### Comparing `chemcoord-2.1.1/src/chemcoord/utilities/_temporary_deprecation_workarounds.py` & `chemcoord-2.1.2/src/chemcoord/utilities/_temporary_deprecation_workarounds.py`

 * *Files identical despite different names*

### Comparing `chemcoord-2.1.1/src/chemcoord.egg-info/PKG-INFO` & `chemcoord-2.1.2/src/chemcoord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemcoord
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python module for dealing with chemical coordinates.
 Home-page: https://github.com/mcocdawc/chemcoord
 Author: Oskar Weser
 Author-email: oskar.weser@gmail.com
 License: LGPLv3
 Keywords: chemcoord,transformation,cartesian,internal,chemistry,zmatrix,xyz,zmat,coordinates,coordinate system
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/x-rst
 License-File: LICENSE.md
 Requires-Dist: numpy>=1.0
-Requires-Dist: scipy
 Requires-Dist: pandas>=1.0
 Requires-Dist: numba>=0.35
 Requires-Dist: sortedcontainers
 Requires-Dist: sympy
 Requires-Dist: six
 Requires-Dist: pymatgen
 
@@ -38,15 +37,15 @@
 =======================================================
 
 
 .. list-table::
    :widths: 25 25
    :header-rows: 0
 
-   * - .. image:: https://github.com/mcocdawc/chemcoord/blob/v2.1.1/docs/source/_static/logo/chemcoord_logo.png
+   * - .. image:: https://raw.githubusercontent.com/mcocdawc/chemcoord/v2.1.2/docs/source/_static/logo/chemcoord_logo.png
               :align: center
               :width: 140
               :alt: Chemcoord logo
      -
    * - Latest Release
      - .. image:: https://img.shields.io/pypi/v/chemcoord.svg
             :target: https://pypi.python.org/pypi/chemcoord
@@ -170,14 +169,14 @@
 
 
 
 Acknowledgement
 ~~~~~~~~~~~~~~~
 
 
-.. image:: https://github.com/zulip/zulip/blob/main/static/images/logo/zulip-icon-circle.svg
+.. image:: https://raw.githubusercontent.com/zulip/zulip/982097f0a7fe2ecf46edc8756fc19f2a5c354ad7/static/images/logo/zulip-icon-circle.svg
    :width: 80
    :align: left
    :target: https://zulip.com/
 
 Zulip is an open-source modern team chat app designed to keep both live and asynchronous conversations organized,
 that supports the development of chemcoord with a free plan.
```

### Comparing `chemcoord-2.1.1/src/chemcoord.egg-info/SOURCES.txt` & `chemcoord-2.1.2/src/chemcoord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

