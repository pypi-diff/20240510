# Comparing `tmp/geoh5py-0.9.0rc2.tar.gz` & `tmp/geoh5py-0.9.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoh5py-0.9.0rc2.tar", max compression
+gzip compressed data, was "geoh5py-0.9.0rc3.tar", max compression
```

## Comparing `geoh5py-0.9.0rc2.tar` & `geoh5py-0.9.0rc3.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0    35823 2024-04-23 21:09:09.940960 geoh5py-0.9.0rc2/COPYING
--rw-r--r--   0        0        0     7817 2024-04-23 21:09:09.940960 geoh5py-0.9.0rc2/COPYING.LESSER
--rw-r--r--   0        0        0      838 2024-05-02 19:52:20.263627 geoh5py-0.9.0rc2/geoh5py/__init__.py
--rw-r--r--   0        0        0     1574 2024-04-23 21:09:10.033237 geoh5py-0.9.0rc2/geoh5py/data/__init__.py
--rw-r--r--   0        0        0     1311 2024-04-23 21:09:10.034242 geoh5py-0.9.0rc2/geoh5py/data/blob_data.py
--rw-r--r--   0        0        0     2005 2024-04-23 21:09:10.034314 geoh5py-0.9.0rc2/geoh5py/data/boolean_data.py
--rw-r--r--   0        0        0     3756 2024-04-23 21:09:10.034314 geoh5py-0.9.0rc2/geoh5py/data/color_map.py
--rw-r--r--   0        0        0     8914 2024-04-23 21:09:50.491132 geoh5py-0.9.0rc2/geoh5py/data/data.py
--rw-r--r--   0        0        0     1138 2024-04-23 21:09:10.035431 geoh5py-0.9.0rc2/geoh5py/data/data_association_enum.py
--rw-r--r--   0        0        0    13377 2024-04-23 21:09:50.491940 geoh5py-0.9.0rc2/geoh5py/data/data_type.py
--rw-r--r--   0        0        0     1138 2024-04-23 21:09:10.035431 geoh5py-0.9.0rc2/geoh5py/data/data_unit.py
--rw-r--r--   0        0        0     1340 2024-04-23 21:09:10.036503 geoh5py-0.9.0rc2/geoh5py/data/datetime_data.py
--rw-r--r--   0        0        0     3690 2024-04-23 21:09:10.036503 geoh5py-0.9.0rc2/geoh5py/data/filename_data.py
--rw-r--r--   0        0        0     1787 2024-04-23 21:09:10.036503 geoh5py-0.9.0rc2/geoh5py/data/float_data.py
--rw-r--r--   0        0        0     1625 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc2/geoh5py/data/geometric_data_constants.py
--rw-r--r--   0        0        0     1709 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc2/geoh5py/data/integer_data.py
--rw-r--r--   0        0        0     4001 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc2/geoh5py/data/numeric_data.py
--rw-r--r--   0        0        0     1121 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc2/geoh5py/data/primitive_type_enum.py
--rw-r--r--   0        0        0     2896 2024-04-23 21:09:50.493092 geoh5py-0.9.0rc2/geoh5py/data/reference_value_map.py
--rw-r--r--   0        0        0     1531 2024-04-23 21:09:10.038674 geoh5py-0.9.0rc2/geoh5py/data/referenced_data.py
--rw-r--r--   0        0        0     5093 2024-04-23 21:09:10.038674 geoh5py-0.9.0rc2/geoh5py/data/text_data.py
--rw-r--r--   0        0        0     1573 2024-04-23 21:09:10.039753 geoh5py-0.9.0rc2/geoh5py/data/unknown_data.py
--rw-r--r--   0        0        0     4559 2024-04-23 21:09:10.039753 geoh5py-0.9.0rc2/geoh5py/data/visual_parameters.py
--rw-r--r--   0        0        0     1587 2024-04-23 21:09:10.039753 geoh5py-0.9.0rc2/geoh5py/groups/__init__.py
--rw-r--r--   0        0        0     1441 2024-04-23 21:09:10.040830 geoh5py-0.9.0rc2/geoh5py/groups/container_group.py
--rw-r--r--   0        0        0     1474 2024-04-23 21:09:10.040830 geoh5py-0.9.0rc2/geoh5py/groups/custom_group.py
--rw-r--r--   0        0        0     1797 2024-04-23 21:09:10.040830 geoh5py-0.9.0rc2/geoh5py/groups/drillhole_group.py
--rw-r--r--   0        0        0     1444 2024-04-23 21:09:10.041866 geoh5py-0.9.0rc2/geoh5py/groups/giftools_group.py
--rw-r--r--   0        0        0     7068 2024-04-23 21:09:50.493092 geoh5py-0.9.0rc2/geoh5py/groups/group.py
--rw-r--r--   0        0        0     2517 2024-04-23 21:09:10.041938 geoh5py-0.9.0rc2/geoh5py/groups/group_type.py
--rw-r--r--   0        0        0     6714 2024-04-23 21:09:10.043010 geoh5py-0.9.0rc2/geoh5py/groups/integrator_group.py
--rw-r--r--   0        0        0     1295 2024-04-23 21:09:10.043010 geoh5py-0.9.0rc2/geoh5py/groups/maps_group.py
--rw-r--r--   0        0        0     1414 2024-04-23 21:09:10.043010 geoh5py-0.9.0rc2/geoh5py/groups/notype_group.py
--rw-r--r--   0        0        0     7843 2024-04-23 21:09:50.494180 geoh5py-0.9.0rc2/geoh5py/groups/property_group.py
--rw-r--r--   0        0        0     1593 2024-04-23 21:09:10.044089 geoh5py-0.9.0rc2/geoh5py/groups/root_group.py
--rw-r--r--   0        0        0     2053 2024-04-23 21:09:10.044089 geoh5py-0.9.0rc2/geoh5py/groups/simpeg_group.py
--rw-r--r--   0        0        0     1322 2024-04-23 21:09:10.044089 geoh5py-0.9.0rc2/geoh5py/groups/survey_group.py
--rw-r--r--   0        0        0      866 2024-04-23 21:09:10.049503 geoh5py-0.9.0rc2/geoh5py/io/__init__.py
--rw-r--r--   0        0        0    17355 2024-04-23 21:09:50.495268 geoh5py-0.9.0rc2/geoh5py/io/h5_reader.py
--rw-r--r--   0        0        0    34805 2024-04-23 21:09:50.495268 geoh5py-0.9.0rc2/geoh5py/io/h5_writer.py
--rw-r--r--   0        0        0     2403 2024-04-23 21:09:10.051610 geoh5py-0.9.0rc2/geoh5py/objects/__init__.py
--rw-r--r--   0        0        0     9440 2024-04-23 21:09:10.051957 geoh5py-0.9.0rc2/geoh5py/objects/block_model.py
--rw-r--r--   0        0        0     7873 2024-04-23 21:09:50.496387 geoh5py-0.9.0rc2/geoh5py/objects/cell_object.py
--rw-r--r--   0        0        0     6300 2024-04-23 21:09:50.497531 geoh5py-0.9.0rc2/geoh5py/objects/curve.py
--rw-r--r--   0        0        0     6204 2024-04-23 21:09:10.053010 geoh5py-0.9.0rc2/geoh5py/objects/drape_model.py
--rw-r--r--   0        0        0    26674 2024-04-23 21:09:10.053010 geoh5py-0.9.0rc2/geoh5py/objects/drillhole.py
--rw-r--r--   0        0        0    21867 2024-04-23 21:09:50.498540 geoh5py-0.9.0rc2/geoh5py/objects/geo_image.py
--rw-r--r--   0        0        0    14054 2024-04-23 21:09:10.053963 geoh5py-0.9.0rc2/geoh5py/objects/grid2d.py
--rw-r--r--   0        0        0     4879 2024-04-23 21:09:10.053963 geoh5py-0.9.0rc2/geoh5py/objects/grid_object.py
--rw-r--r--   0        0        0     1957 2024-04-23 21:09:10.053963 geoh5py-0.9.0rc2/geoh5py/objects/integrator.py
--rw-r--r--   0        0        0     2921 2024-04-23 21:09:10.055218 geoh5py-0.9.0rc2/geoh5py/objects/label.py
--rw-r--r--   0        0        0     2686 2024-04-23 21:09:10.055218 geoh5py-0.9.0rc2/geoh5py/objects/notype_object.py
--rw-r--r--   0        0        0    21991 2024-04-23 21:09:50.498666 geoh5py-0.9.0rc2/geoh5py/objects/object_base.py
--rw-r--r--   0        0        0     1098 2024-04-23 21:09:10.056303 geoh5py-0.9.0rc2/geoh5py/objects/object_type.py
--rw-r--r--   0        0        0    13455 2024-04-23 21:09:50.499764 geoh5py-0.9.0rc2/geoh5py/objects/octree.py
--rw-r--r--   0        0        0     5353 2024-04-23 21:09:50.500917 geoh5py-0.9.0rc2/geoh5py/objects/points.py
--rw-r--r--   0        0        0     2588 2024-04-23 21:09:10.057382 geoh5py-0.9.0rc2/geoh5py/objects/surface.py
--rw-r--r--   0        0        0      747 2024-04-23 21:09:10.057382 geoh5py-0.9.0rc2/geoh5py/objects/surveys/__init__.py
--rw-r--r--   0        0        0    14521 2024-04-23 21:09:10.058382 geoh5py-0.9.0rc2/geoh5py/objects/surveys/direct_current.py
--rw-r--r--   0        0        0      747 2024-04-23 21:09:10.058382 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/__init__.py
--rw-r--r--   0        0        0     3660 2024-04-23 21:09:10.058382 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/airborne_fem.py
--rw-r--r--   0        0        0     3629 2024-04-23 21:09:10.059469 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
--rw-r--r--   0        0        0    36522 2024-04-23 21:09:10.059469 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/base.py
--rw-r--r--   0        0        0     6925 2024-04-23 21:09:10.059469 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/ground_fem.py
--rw-r--r--   0        0        0     6937 2024-04-23 21:09:10.060547 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/ground_tem.py
--rw-r--r--   0        0        0     2615 2024-04-23 21:09:10.060547 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
--rw-r--r--   0        0        0     6605 2024-04-23 21:09:10.060547 geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/tipper.py
--rw-r--r--   0        0        0     1247 2024-04-23 21:09:10.061666 geoh5py-0.9.0rc2/geoh5py/objects/surveys/magnetics.py
--rw-r--r--   0        0        0        0 2024-04-23 21:09:10.061666 geoh5py-0.9.0rc2/geoh5py/py.typed
--rw-r--r--   0        0        0     1013 2024-04-23 21:09:10.061666 geoh5py-0.9.0rc2/geoh5py/shared/__init__.py
--rw-r--r--   0        0        0     1057 2024-04-23 21:09:10.062721 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/__init__.py
--rw-r--r--   0        0        0     1847 2024-04-23 21:09:10.062721 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/concatenated.py
--rw-r--r--   0        0        0    25972 2024-04-23 21:09:50.500917 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/concatenator.py
--rw-r--r--   0        0        0     3029 2024-04-23 21:09:10.063809 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/data.py
--rw-r--r--   0        0        0    14282 2024-04-23 21:09:50.502000 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/drillhole.py
--rw-r--r--   0        0        0    15847 2024-04-23 21:09:50.503139 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/drillholes_group_table.py
--rw-r--r--   0        0        0     6729 2024-04-23 21:09:50.503139 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/object.py
--rw-r--r--   0        0        0     5193 2024-04-23 21:09:50.504046 geoh5py-0.9.0rc2/geoh5py/shared/concatenation/property_group.py
--rw-r--r--   0        0        0      937 2024-04-23 21:09:10.066045 geoh5py-0.9.0rc2/geoh5py/shared/conversion/__init__.py
--rw-r--r--   0        0        0     4426 2024-04-23 21:09:10.067142 geoh5py-0.9.0rc2/geoh5py/shared/conversion/base.py
--rw-r--r--   0        0        0     5629 2024-04-23 21:09:50.504628 geoh5py-0.9.0rc2/geoh5py/shared/conversion/geo_image.py
--rw-r--r--   0        0        0    10840 2024-04-23 21:09:10.068311 geoh5py-0.9.0rc2/geoh5py/shared/conversion/grid2d.py
--rw-r--r--   0        0        0    10730 2024-04-23 21:09:10.068311 geoh5py-0.9.0rc2/geoh5py/shared/entity.py
--rw-r--r--   0        0        0     7630 2024-04-23 21:09:50.505726 geoh5py-0.9.0rc2/geoh5py/shared/entity_container.py
--rw-r--r--   0        0        0     8632 2024-04-23 21:09:10.069420 geoh5py-0.9.0rc2/geoh5py/shared/entity_type.py
--rw-r--r--   0        0        0     8353 2024-04-23 21:09:10.070423 geoh5py-0.9.0rc2/geoh5py/shared/exceptions.py
--rw-r--r--   0        0        0      923 2024-04-23 21:09:10.070423 geoh5py-0.9.0rc2/geoh5py/shared/merging/__init__.py
--rw-r--r--   0        0        0     7734 2024-04-23 21:09:10.071533 geoh5py-0.9.0rc2/geoh5py/shared/merging/base.py
--rw-r--r--   0        0        0     2336 2024-04-23 21:09:10.071533 geoh5py-0.9.0rc2/geoh5py/shared/merging/cell.py
--rw-r--r--   0        0        0     6105 2024-04-23 21:09:10.072628 geoh5py-0.9.0rc2/geoh5py/shared/merging/drape_model.py
--rw-r--r--   0        0        0     1845 2024-04-23 21:09:10.072628 geoh5py-0.9.0rc2/geoh5py/shared/merging/points.py
--rw-r--r--   0        0        0    21424 2024-04-23 21:09:50.506831 geoh5py-0.9.0rc2/geoh5py/shared/utils.py
--rw-r--r--   0        0        0     8847 2024-04-23 21:09:10.073740 geoh5py-0.9.0rc2/geoh5py/shared/validators.py
--rw-r--r--   0        0        0     2647 2024-04-23 21:09:10.074842 geoh5py-0.9.0rc2/geoh5py/shared/weakref_utils.py
--rw-r--r--   0        0        0      959 2024-04-23 21:09:10.074842 geoh5py-0.9.0rc2/geoh5py/ui_json/__init__.py
--rw-r--r--   0        0        0     2991 2024-04-23 21:09:10.076022 geoh5py-0.9.0rc2/geoh5py/ui_json/constants.py
--rw-r--r--   0        0        0     1983 2024-04-23 21:09:10.076022 geoh5py-0.9.0rc2/geoh5py/ui_json/descriptors.py
--rw-r--r--   0        0        0    11461 2024-04-23 21:09:10.077023 geoh5py-0.9.0rc2/geoh5py/ui_json/enforcers.py
--rw-r--r--   0        0        0    18309 2024-04-23 21:09:10.077147 geoh5py-0.9.0rc2/geoh5py/ui_json/forms.py
--rw-r--r--   0        0        0    18789 2024-04-23 21:09:50.508030 geoh5py-0.9.0rc2/geoh5py/ui_json/input_file.py
--rw-r--r--   0        0        0     4939 2024-04-26 17:53:29.560114 geoh5py-0.9.0rc2/geoh5py/ui_json/parameters.py
--rw-r--r--   0        0        0    15250 2024-04-23 21:09:50.508030 geoh5py-0.9.0rc2/geoh5py/ui_json/templates.py
--rw-r--r--   0        0        0     5076 2024-04-23 21:09:10.079354 geoh5py-0.9.0rc2/geoh5py/ui_json/ui_json.py
--rw-r--r--   0        0        0    11199 2024-04-23 21:09:50.509027 geoh5py-0.9.0rc2/geoh5py/ui_json/utils.py
--rw-r--r--   0        0        0    11402 2024-04-26 17:53:43.697719 geoh5py-0.9.0rc2/geoh5py/ui_json/validation.py
--rw-r--r--   0        0        0      852 2024-04-23 21:09:10.081557 geoh5py-0.9.0rc2/geoh5py/workspace/__init__.py
--rw-r--r--   0        0        0    51060 2024-04-23 21:09:50.511214 geoh5py-0.9.0rc2/geoh5py/workspace/workspace.py
--rw-r--r--   0        0        0     2111 2024-04-23 21:09:10.082662 geoh5py-0.9.0rc2/package.rst
--rw-r--r--   0        0        0     2432 2024-05-02 19:52:20.268477 geoh5py-0.9.0rc2/pyproject.toml
--rw-r--r--   0        0        0     5600 2024-04-23 21:09:09.940960 geoh5py-0.9.0rc2/README.rst
--rw-r--r--   0        0        0    54566 2024-04-23 21:09:09.942022 geoh5py-0.9.0rc2/THIRD_PARTY_SOFTWARE.rst
--rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 geoh5py-0.9.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-04-23 21:09:09.940960 geoh5py-0.9.0rc3/COPYING
+-rw-r--r--   0        0        0     7817 2024-04-23 21:09:09.940960 geoh5py-0.9.0rc3/COPYING.LESSER
+-rw-r--r--   0        0        0      838 2024-05-09 21:46:02.524044 geoh5py-0.9.0rc3/geoh5py/__init__.py
+-rw-r--r--   0        0        0     1574 2024-04-23 21:09:10.033237 geoh5py-0.9.0rc3/geoh5py/data/__init__.py
+-rw-r--r--   0        0        0     1311 2024-04-23 21:09:10.034242 geoh5py-0.9.0rc3/geoh5py/data/blob_data.py
+-rw-r--r--   0        0        0     2005 2024-04-23 21:09:10.034314 geoh5py-0.9.0rc3/geoh5py/data/boolean_data.py
+-rw-r--r--   0        0        0     3756 2024-04-23 21:09:10.034314 geoh5py-0.9.0rc3/geoh5py/data/color_map.py
+-rw-r--r--   0        0        0     8914 2024-04-23 21:09:50.491132 geoh5py-0.9.0rc3/geoh5py/data/data.py
+-rw-r--r--   0        0        0     1138 2024-04-23 21:09:10.035431 geoh5py-0.9.0rc3/geoh5py/data/data_association_enum.py
+-rw-r--r--   0        0        0    13377 2024-04-23 21:09:50.491940 geoh5py-0.9.0rc3/geoh5py/data/data_type.py
+-rw-r--r--   0        0        0     1138 2024-04-23 21:09:10.035431 geoh5py-0.9.0rc3/geoh5py/data/data_unit.py
+-rw-r--r--   0        0        0     1340 2024-04-23 21:09:10.036503 geoh5py-0.9.0rc3/geoh5py/data/datetime_data.py
+-rw-r--r--   0        0        0     3690 2024-04-23 21:09:10.036503 geoh5py-0.9.0rc3/geoh5py/data/filename_data.py
+-rw-r--r--   0        0        0     1787 2024-04-23 21:09:10.036503 geoh5py-0.9.0rc3/geoh5py/data/float_data.py
+-rw-r--r--   0        0        0     1625 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc3/geoh5py/data/geometric_data_constants.py
+-rw-r--r--   0        0        0     1709 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc3/geoh5py/data/integer_data.py
+-rw-r--r--   0        0        0     4001 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc3/geoh5py/data/numeric_data.py
+-rw-r--r--   0        0        0     1121 2024-04-23 21:09:10.037592 geoh5py-0.9.0rc3/geoh5py/data/primitive_type_enum.py
+-rw-r--r--   0        0        0     2896 2024-04-23 21:09:50.493092 geoh5py-0.9.0rc3/geoh5py/data/reference_value_map.py
+-rw-r--r--   0        0        0     1531 2024-04-23 21:09:10.038674 geoh5py-0.9.0rc3/geoh5py/data/referenced_data.py
+-rw-r--r--   0        0        0     5093 2024-04-23 21:09:10.038674 geoh5py-0.9.0rc3/geoh5py/data/text_data.py
+-rw-r--r--   0        0        0     1573 2024-04-23 21:09:10.039753 geoh5py-0.9.0rc3/geoh5py/data/unknown_data.py
+-rw-r--r--   0        0        0     4559 2024-04-23 21:09:10.039753 geoh5py-0.9.0rc3/geoh5py/data/visual_parameters.py
+-rw-r--r--   0        0        0     1587 2024-04-23 21:09:10.039753 geoh5py-0.9.0rc3/geoh5py/groups/__init__.py
+-rw-r--r--   0        0        0     1441 2024-04-23 21:09:10.040830 geoh5py-0.9.0rc3/geoh5py/groups/container_group.py
+-rw-r--r--   0        0        0     1474 2024-04-23 21:09:10.040830 geoh5py-0.9.0rc3/geoh5py/groups/custom_group.py
+-rw-r--r--   0        0        0     1797 2024-04-23 21:09:10.040830 geoh5py-0.9.0rc3/geoh5py/groups/drillhole_group.py
+-rw-r--r--   0        0        0     1444 2024-04-23 21:09:10.041866 geoh5py-0.9.0rc3/geoh5py/groups/giftools_group.py
+-rw-r--r--   0        0        0     7068 2024-04-23 21:09:50.493092 geoh5py-0.9.0rc3/geoh5py/groups/group.py
+-rw-r--r--   0        0        0     2517 2024-04-23 21:09:10.041938 geoh5py-0.9.0rc3/geoh5py/groups/group_type.py
+-rw-r--r--   0        0        0     6714 2024-04-23 21:09:10.043010 geoh5py-0.9.0rc3/geoh5py/groups/integrator_group.py
+-rw-r--r--   0        0        0     1295 2024-04-23 21:09:10.043010 geoh5py-0.9.0rc3/geoh5py/groups/maps_group.py
+-rw-r--r--   0        0        0     1414 2024-04-23 21:09:10.043010 geoh5py-0.9.0rc3/geoh5py/groups/notype_group.py
+-rw-r--r--   0        0        0     7843 2024-04-23 21:09:50.494180 geoh5py-0.9.0rc3/geoh5py/groups/property_group.py
+-rw-r--r--   0        0        0     1593 2024-04-23 21:09:10.044089 geoh5py-0.9.0rc3/geoh5py/groups/root_group.py
+-rw-r--r--   0        0        0     2053 2024-04-23 21:09:10.044089 geoh5py-0.9.0rc3/geoh5py/groups/simpeg_group.py
+-rw-r--r--   0        0        0     1322 2024-04-23 21:09:10.044089 geoh5py-0.9.0rc3/geoh5py/groups/survey_group.py
+-rw-r--r--   0        0        0      866 2024-04-23 21:09:10.049503 geoh5py-0.9.0rc3/geoh5py/io/__init__.py
+-rw-r--r--   0        0        0    17462 2024-05-09 21:45:23.764341 geoh5py-0.9.0rc3/geoh5py/io/h5_reader.py
+-rw-r--r--   0        0        0    34805 2024-04-23 21:09:50.495268 geoh5py-0.9.0rc3/geoh5py/io/h5_writer.py
+-rw-r--r--   0        0        0     2403 2024-05-02 19:58:37.031626 geoh5py-0.9.0rc3/geoh5py/objects/__init__.py
+-rw-r--r--   0        0        0     9440 2024-04-23 21:09:10.051957 geoh5py-0.9.0rc3/geoh5py/objects/block_model.py
+-rw-r--r--   0        0        0     7873 2024-04-23 21:09:50.496387 geoh5py-0.9.0rc3/geoh5py/objects/cell_object.py
+-rw-r--r--   0        0        0     6300 2024-04-23 21:09:50.497531 geoh5py-0.9.0rc3/geoh5py/objects/curve.py
+-rw-r--r--   0        0        0     6204 2024-04-23 21:09:10.053010 geoh5py-0.9.0rc3/geoh5py/objects/drape_model.py
+-rw-r--r--   0        0        0    26674 2024-04-23 21:09:10.053010 geoh5py-0.9.0rc3/geoh5py/objects/drillhole.py
+-rw-r--r--   0        0        0    21867 2024-04-23 21:09:50.498540 geoh5py-0.9.0rc3/geoh5py/objects/geo_image.py
+-rw-r--r--   0        0        0    14054 2024-04-23 21:09:10.053963 geoh5py-0.9.0rc3/geoh5py/objects/grid2d.py
+-rw-r--r--   0        0        0     4879 2024-04-23 21:09:10.053963 geoh5py-0.9.0rc3/geoh5py/objects/grid_object.py
+-rw-r--r--   0        0        0     1957 2024-04-23 21:09:10.053963 geoh5py-0.9.0rc3/geoh5py/objects/integrator.py
+-rw-r--r--   0        0        0     2921 2024-04-23 21:09:10.055218 geoh5py-0.9.0rc3/geoh5py/objects/label.py
+-rw-r--r--   0        0        0     2686 2024-04-23 21:09:10.055218 geoh5py-0.9.0rc3/geoh5py/objects/notype_object.py
+-rw-r--r--   0        0        0    22388 2024-05-09 21:45:23.766343 geoh5py-0.9.0rc3/geoh5py/objects/object_base.py
+-rw-r--r--   0        0        0     1098 2024-04-23 21:09:10.056303 geoh5py-0.9.0rc3/geoh5py/objects/object_type.py
+-rw-r--r--   0        0        0    13455 2024-04-23 21:09:50.499764 geoh5py-0.9.0rc3/geoh5py/objects/octree.py
+-rw-r--r--   0        0        0     5353 2024-04-23 21:09:50.500917 geoh5py-0.9.0rc3/geoh5py/objects/points.py
+-rw-r--r--   0        0        0     2588 2024-04-23 21:09:10.057382 geoh5py-0.9.0rc3/geoh5py/objects/surface.py
+-rw-r--r--   0        0        0      747 2024-04-23 21:09:10.057382 geoh5py-0.9.0rc3/geoh5py/objects/surveys/__init__.py
+-rw-r--r--   0        0        0    14521 2024-04-23 21:09:10.058382 geoh5py-0.9.0rc3/geoh5py/objects/surveys/direct_current.py
+-rw-r--r--   0        0        0      747 2024-04-23 21:09:10.058382 geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/__init__.py
+-rw-r--r--   0        0        0     3660 2024-04-23 21:09:10.058382 geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/airborne_fem.py
+-rw-r--r--   0        0        0     3629 2024-04-23 21:09:10.059469 geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
+-rw-r--r--   0        0        0    36522 2024-04-23 21:09:10.059469 geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/base.py
+-rw-r--r--   0        0        0     6925 2024-04-23 21:09:10.059469 geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/ground_fem.py
+-rw-r--r--   0        0        0     6937 2024-04-23 21:09:10.060547 geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/ground_tem.py
+-rw-r--r--   0        0        0     2615 2024-04-23 21:09:10.060547 geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
+-rw-r--r--   0        0        0     6605 2024-04-23 21:09:10.060547 geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/tipper.py
+-rw-r--r--   0        0        0     1247 2024-04-23 21:09:10.061666 geoh5py-0.9.0rc3/geoh5py/objects/surveys/magnetics.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:09:10.061666 geoh5py-0.9.0rc3/geoh5py/py.typed
+-rw-r--r--   0        0        0     1013 2024-04-23 21:09:10.061666 geoh5py-0.9.0rc3/geoh5py/shared/__init__.py
+-rw-r--r--   0        0        0     1057 2024-04-23 21:09:10.062721 geoh5py-0.9.0rc3/geoh5py/shared/concatenation/__init__.py
+-rw-r--r--   0        0        0     1847 2024-04-23 21:09:10.062721 geoh5py-0.9.0rc3/geoh5py/shared/concatenation/concatenated.py
+-rw-r--r--   0        0        0    26016 2024-05-09 21:45:23.768356 geoh5py-0.9.0rc3/geoh5py/shared/concatenation/concatenator.py
+-rw-r--r--   0        0        0     3029 2024-04-23 21:09:10.063809 geoh5py-0.9.0rc3/geoh5py/shared/concatenation/data.py
+-rw-r--r--   0        0        0    14282 2024-04-23 21:09:50.502000 geoh5py-0.9.0rc3/geoh5py/shared/concatenation/drillhole.py
+-rw-r--r--   0        0        0    15847 2024-04-23 21:09:50.503139 geoh5py-0.9.0rc3/geoh5py/shared/concatenation/drillholes_group_table.py
+-rw-r--r--   0        0        0     6584 2024-05-09 21:45:23.770342 geoh5py-0.9.0rc3/geoh5py/shared/concatenation/object.py
+-rw-r--r--   0        0        0     5263 2024-05-09 21:45:23.771343 geoh5py-0.9.0rc3/geoh5py/shared/concatenation/property_group.py
+-rw-r--r--   0        0        0      937 2024-04-23 21:09:10.066045 geoh5py-0.9.0rc3/geoh5py/shared/conversion/__init__.py
+-rw-r--r--   0        0        0     4426 2024-04-23 21:09:10.067142 geoh5py-0.9.0rc3/geoh5py/shared/conversion/base.py
+-rw-r--r--   0        0        0     5629 2024-04-23 21:09:50.504628 geoh5py-0.9.0rc3/geoh5py/shared/conversion/geo_image.py
+-rw-r--r--   0        0        0    10840 2024-04-23 21:09:10.068311 geoh5py-0.9.0rc3/geoh5py/shared/conversion/grid2d.py
+-rw-r--r--   0        0        0    10730 2024-04-23 21:09:10.068311 geoh5py-0.9.0rc3/geoh5py/shared/entity.py
+-rw-r--r--   0        0        0     7630 2024-04-23 21:09:50.505726 geoh5py-0.9.0rc3/geoh5py/shared/entity_container.py
+-rw-r--r--   0        0        0     8632 2024-04-23 21:09:10.069420 geoh5py-0.9.0rc3/geoh5py/shared/entity_type.py
+-rw-r--r--   0        0        0     8353 2024-04-23 21:09:10.070423 geoh5py-0.9.0rc3/geoh5py/shared/exceptions.py
+-rw-r--r--   0        0        0      923 2024-04-23 21:09:10.070423 geoh5py-0.9.0rc3/geoh5py/shared/merging/__init__.py
+-rw-r--r--   0        0        0     7734 2024-04-23 21:09:10.071533 geoh5py-0.9.0rc3/geoh5py/shared/merging/base.py
+-rw-r--r--   0        0        0     2336 2024-04-23 21:09:10.071533 geoh5py-0.9.0rc3/geoh5py/shared/merging/cell.py
+-rw-r--r--   0        0        0     6105 2024-04-23 21:09:10.072628 geoh5py-0.9.0rc3/geoh5py/shared/merging/drape_model.py
+-rw-r--r--   0        0        0     1845 2024-04-23 21:09:10.072628 geoh5py-0.9.0rc3/geoh5py/shared/merging/points.py
+-rw-r--r--   0        0        0    21424 2024-04-23 21:09:50.506831 geoh5py-0.9.0rc3/geoh5py/shared/utils.py
+-rw-r--r--   0        0        0     8847 2024-04-23 21:09:10.073740 geoh5py-0.9.0rc3/geoh5py/shared/validators.py
+-rw-r--r--   0        0        0     2647 2024-04-23 21:09:10.074842 geoh5py-0.9.0rc3/geoh5py/shared/weakref_utils.py
+-rw-r--r--   0        0        0      959 2024-04-23 21:09:10.074842 geoh5py-0.9.0rc3/geoh5py/ui_json/__init__.py
+-rw-r--r--   0        0        0     2991 2024-04-23 21:09:10.076022 geoh5py-0.9.0rc3/geoh5py/ui_json/constants.py
+-rw-r--r--   0        0        0     1983 2024-04-23 21:09:10.076022 geoh5py-0.9.0rc3/geoh5py/ui_json/descriptors.py
+-rw-r--r--   0        0        0    11461 2024-04-23 21:09:10.077023 geoh5py-0.9.0rc3/geoh5py/ui_json/enforcers.py
+-rw-r--r--   0        0        0    18309 2024-04-23 21:09:10.077147 geoh5py-0.9.0rc3/geoh5py/ui_json/forms.py
+-rw-r--r--   0        0        0    18789 2024-04-23 21:09:50.508030 geoh5py-0.9.0rc3/geoh5py/ui_json/input_file.py
+-rw-r--r--   0        0        0     4939 2024-04-26 17:53:29.560114 geoh5py-0.9.0rc3/geoh5py/ui_json/parameters.py
+-rw-r--r--   0        0        0    15250 2024-04-23 21:09:50.508030 geoh5py-0.9.0rc3/geoh5py/ui_json/templates.py
+-rw-r--r--   0        0        0     5076 2024-04-23 21:09:10.079354 geoh5py-0.9.0rc3/geoh5py/ui_json/ui_json.py
+-rw-r--r--   0        0        0    11199 2024-04-23 21:09:50.509027 geoh5py-0.9.0rc3/geoh5py/ui_json/utils.py
+-rw-r--r--   0        0        0    11402 2024-04-26 17:53:43.697719 geoh5py-0.9.0rc3/geoh5py/ui_json/validation.py
+-rw-r--r--   0        0        0      852 2024-04-23 21:09:10.081557 geoh5py-0.9.0rc3/geoh5py/workspace/__init__.py
+-rw-r--r--   0        0        0    51060 2024-04-23 21:09:50.511214 geoh5py-0.9.0rc3/geoh5py/workspace/workspace.py
+-rw-r--r--   0        0        0     2111 2024-04-23 21:09:10.082662 geoh5py-0.9.0rc3/package.rst
+-rw-r--r--   0        0        0     2432 2024-05-09 21:46:02.510065 geoh5py-0.9.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     5600 2024-05-09 22:43:23.269959 geoh5py-0.9.0rc3/README.rst
+-rw-r--r--   0        0        0    54566 2024-04-23 21:09:09.942022 geoh5py-0.9.0rc3/THIRD_PARTY_SOFTWARE.rst
+-rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 geoh5py-0.9.0rc3/PKG-INFO
```

### Comparing `geoh5py-0.9.0rc2/COPYING` & `geoh5py-0.9.0rc3/COPYING`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/COPYING.LESSER` & `geoh5py-0.9.0rc3/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/__init__.py` & `geoh5py-0.9.0rc3/geoh5py/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 # flake8: noqa
 
-__version__ = "0.9.0-rc.2"
+__version__ = "0.9.0-rc.3"
 
 from geoh5py.workspace import Workspace
```

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/__init__.py` & `geoh5py-0.9.0rc3/geoh5py/data/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/blob_data.py` & `geoh5py-0.9.0rc3/geoh5py/data/blob_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/boolean_data.py` & `geoh5py-0.9.0rc3/geoh5py/data/boolean_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/color_map.py` & `geoh5py-0.9.0rc3/geoh5py/data/color_map.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/data.py` & `geoh5py-0.9.0rc3/geoh5py/data/data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/data_association_enum.py` & `geoh5py-0.9.0rc3/geoh5py/data/data_association_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/data_type.py` & `geoh5py-0.9.0rc3/geoh5py/data/data_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/data_unit.py` & `geoh5py-0.9.0rc3/geoh5py/data/data_unit.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/datetime_data.py` & `geoh5py-0.9.0rc3/geoh5py/data/datetime_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/filename_data.py` & `geoh5py-0.9.0rc3/geoh5py/data/filename_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/float_data.py` & `geoh5py-0.9.0rc3/geoh5py/data/float_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/geometric_data_constants.py` & `geoh5py-0.9.0rc3/geoh5py/data/geometric_data_constants.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/integer_data.py` & `geoh5py-0.9.0rc3/geoh5py/data/integer_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/numeric_data.py` & `geoh5py-0.9.0rc3/geoh5py/data/numeric_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/primitive_type_enum.py` & `geoh5py-0.9.0rc3/geoh5py/data/primitive_type_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/reference_value_map.py` & `geoh5py-0.9.0rc3/geoh5py/data/reference_value_map.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/referenced_data.py` & `geoh5py-0.9.0rc3/geoh5py/data/referenced_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/text_data.py` & `geoh5py-0.9.0rc3/geoh5py/data/text_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/unknown_data.py` & `geoh5py-0.9.0rc3/geoh5py/data/unknown_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/data/visual_parameters.py` & `geoh5py-0.9.0rc3/geoh5py/data/visual_parameters.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/__init__.py` & `geoh5py-0.9.0rc3/geoh5py/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/container_group.py` & `geoh5py-0.9.0rc3/geoh5py/groups/container_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/custom_group.py` & `geoh5py-0.9.0rc3/geoh5py/groups/custom_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/drillhole_group.py` & `geoh5py-0.9.0rc3/geoh5py/groups/drillhole_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/giftools_group.py` & `geoh5py-0.9.0rc3/geoh5py/groups/giftools_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/group.py` & `geoh5py-0.9.0rc3/geoh5py/groups/group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/group_type.py` & `geoh5py-0.9.0rc3/geoh5py/groups/group_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/integrator_group.py` & `geoh5py-0.9.0rc3/geoh5py/groups/integrator_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/maps_group.py` & `geoh5py-0.9.0rc3/geoh5py/groups/maps_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/notype_group.py` & `geoh5py-0.9.0rc3/geoh5py/groups/notype_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/property_group.py` & `geoh5py-0.9.0rc3/geoh5py/groups/property_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/root_group.py` & `geoh5py-0.9.0rc3/geoh5py/groups/root_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/simpeg_group.py` & `geoh5py-0.9.0rc3/geoh5py/groups/simpeg_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/groups/survey_group.py` & `geoh5py-0.9.0rc3/geoh5py/groups/survey_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/io/__init__.py` & `geoh5py-0.9.0rc3/geoh5py/io/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/io/h5_reader.py` & `geoh5py-0.9.0rc3/geoh5py/io/h5_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,19 @@
                     array = group.get(label.replace("/", "\u2044"))
 
                 attribute = array[:]
 
                 if attribute.dtype in [float, "float64", "float32"]:
                     attribute[attribute == FLOAT_NDV] = np.nan
 
-                if attribute.dtype == object and isinstance(attribute[0], bytes):
+                if (
+                    attribute.dtype == object
+                    and len(attribute) > 0
+                    and isinstance(attribute[0], bytes)
+                ):
                     attribute = np.char.decode(attribute.astype(np.bytes_), "UTF-8")
 
                 return attribute, indices[:]
 
             except KeyError:
                 return None
```

### Comparing `geoh5py-0.9.0rc2/geoh5py/io/h5_writer.py` & `geoh5py-0.9.0rc3/geoh5py/io/h5_writer.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/__init__.py` & `geoh5py-0.9.0rc3/geoh5py/objects/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 from .notype_object import NoTypeObject
 from .object_base import ObjectBase
 from .object_type import ObjectType
 from .octree import Octree
 from .points import Points
 from .surface import Surface
 from .surveys.direct_current import CurrentElectrode, PotentialElectrode
-from .surveys.electromagnetics.base import (
-    AirborneEMSurvey,
-    FEMSurvey,
-    LargeLoopGroundEMSurvey,
-    MovingLoopGroundEMSurvey,
-    TEMSurvey,
-)
 from .surveys.electromagnetics.airborne_fem import (
     AirborneFEMReceivers,
     AirborneFEMTransmitters,
 )
 from .surveys.electromagnetics.airborne_tem import (
     AirborneTEMReceivers,
     AirborneTEMTransmitters,
 )
+from .surveys.electromagnetics.base import (
+    AirborneEMSurvey,
+    FEMSurvey,
+    LargeLoopGroundEMSurvey,
+    MovingLoopGroundEMSurvey,
+    TEMSurvey,
+)
 from .surveys.electromagnetics.ground_fem import (
     LargeLoopGroundFEMReceivers,
     LargeLoopGroundFEMTransmitters,
     MovingLoopGroundFEMReceivers,
     MovingLoopGroundFEMTransmitters,
 )
 from .surveys.electromagnetics.ground_tem import (
```

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/block_model.py` & `geoh5py-0.9.0rc3/geoh5py/objects/block_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/cell_object.py` & `geoh5py-0.9.0rc3/geoh5py/objects/cell_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/curve.py` & `geoh5py-0.9.0rc3/geoh5py/objects/curve.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/drape_model.py` & `geoh5py-0.9.0rc3/geoh5py/objects/drape_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/drillhole.py` & `geoh5py-0.9.0rc3/geoh5py/objects/drillhole.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/geo_image.py` & `geoh5py-0.9.0rc3/geoh5py/objects/geo_image.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/grid2d.py` & `geoh5py-0.9.0rc3/geoh5py/objects/grid2d.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/grid_object.py` & `geoh5py-0.9.0rc3/geoh5py/objects/grid_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/integrator.py` & `geoh5py-0.9.0rc3/geoh5py/objects/integrator.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/label.py` & `geoh5py-0.9.0rc3/geoh5py/objects/label.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/notype_object.py` & `geoh5py-0.9.0rc3/geoh5py/objects/notype_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/object_base.py` & `geoh5py-0.9.0rc3/geoh5py/objects/object_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,15 +509,15 @@
             children = [children]
 
         for child in children:
             if child not in self._children:
                 continue
 
             if isinstance(child, PropertyGroup) and self._property_groups:
-                self._property_groups.remove(child)
+                self.remove_property_group(child)
             elif isinstance(child, Data):
                 self.remove_data_from_groups(child)
 
             self._children.remove(child)
 
         self.workspace.remove_children(self, children)
 
@@ -543,14 +543,26 @@
                 values = getattr(child, "_values", None)
                 if values is None:
                     values = child.workspace.fetch_values(child)
                 child.values = np.delete(values, indices, axis=0)
                 if clear_cache:
                     clear_array_attributes(child)
 
+    def remove_property_group(self, property_group: PropertyGroup):
+        """
+        Remove a property group from the object.
+
+        :param property_group: The property group to remove.
+        """
+        if (
+            self._property_groups is not None
+            and property_group in self._property_groups
+        ):
+            self._property_groups.remove(property_group)
+
     @property
     def vertices(self) -> np.ndarray:
         r"""
         :obj:`numpy.array` of :obj:`float`, shape (\*, 3): Array of x, y, z coordinates
         defining the position of points in 3D space.
         """
```

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/object_type.py` & `geoh5py-0.9.0rc3/geoh5py/objects/object_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/octree.py` & `geoh5py-0.9.0rc3/geoh5py/objects/octree.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/points.py` & `geoh5py-0.9.0rc3/geoh5py/objects/points.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/surface.py` & `geoh5py-0.9.0rc3/geoh5py/objects/surface.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/surveys/__init__.py` & `geoh5py-0.9.0rc3/geoh5py/objects/surveys/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/surveys/direct_current.py` & `geoh5py-0.9.0rc3/geoh5py/objects/surveys/direct_current.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/__init__.py` & `geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/airborne_fem.py` & `geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/airborne_fem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/airborne_tem.py` & `geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/airborne_tem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/base.py` & `geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/ground_fem.py` & `geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/ground_fem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/ground_tem.py` & `geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/ground_tem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py` & `geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/surveys/electromagnetics/tipper.py` & `geoh5py-0.9.0rc3/geoh5py/objects/surveys/electromagnetics/tipper.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/objects/surveys/magnetics.py` & `geoh5py-0.9.0rc3/geoh5py/objects/surveys/magnetics.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/__init__.py` & `geoh5py-0.9.0rc3/geoh5py/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/__init__.py` & `geoh5py-0.9.0rc3/geoh5py/shared/concatenation/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/concatenated.py` & `geoh5py-0.9.0rc3/geoh5py/shared/concatenation/concatenated.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/concatenator.py` & `geoh5py-0.9.0rc3/geoh5py/shared/concatenation/concatenator.py`

 * *Files 1% similar despite different names*

```diff
@@ -504,15 +504,16 @@
 
         elif isinstance(entity, ConcatenatedPropertyGroup):
             # Remove all data within the group
             if entity.properties is not None and len(entity.properties) > 0:
                 data = [entity.parent.get_entity(uid)[0] for uid in entity.properties]
                 entity.parent.remove_children(data)
 
-            self.update_array_attribute(parent, "property_groups", remove=True)
+            entity.parent.remove_property_group(entity)
+            self.update_array_attribute(parent, "property_groups")
 
         if (
             self.concatenated_attributes is not None
             and self.attributes_keys is not None
         ):
             attr_handle = self.get_concatenated_attributes(entity.uid)
             self.attributes_keys.remove(as_str_if_uuid(entity.uid))
```

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/data.py` & `geoh5py-0.9.0rc3/geoh5py/shared/concatenation/data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/drillhole.py` & `geoh5py-0.9.0rc3/geoh5py/shared/concatenation/drillhole.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/drillholes_group_table.py` & `geoh5py-0.9.0rc3/geoh5py/shared/concatenation/drillholes_group_table.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/object.py` & `geoh5py-0.9.0rc3/geoh5py/shared/concatenation/object.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,12 +177,8 @@
             children = [children]
 
         for child in children:
             if child not in self._children:
                 continue
 
             self.concatenator.remove_entity(child)
-
-            if isinstance(child, ConcatenatedPropertyGroup) and self._property_groups:
-                self._property_groups.remove(child)
-
             self._children.remove(child)
```

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/concatenation/property_group.py` & `geoh5py-0.9.0rc3/geoh5py/shared/concatenation/property_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,18 +150,19 @@
 
         if (
             self._properties is not None
             and len(self._properties) == 1
             and self.depth_ is not None
         ):
             self.depth_.allow_delete = True
-            self.parent.remove_children(self)
+            self.parent.remove_children([self.depth_])
 
         elif (
             self._properties is not None
             and len(self._properties) == 2
             and self.from_ is not None
             and self.to_ is not None
         ):
-            self.from_.allow_delete = True
             self.to_.allow_delete = True
-            self.parent.remove_children(self)
+            self.parent.remove_children([self.to_])
+            self.from_.allow_delete = True
+            self.parent.remove_children([self.from_])
```

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/conversion/__init__.py` & `geoh5py-0.9.0rc3/geoh5py/shared/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/conversion/base.py` & `geoh5py-0.9.0rc3/geoh5py/shared/conversion/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/conversion/geo_image.py` & `geoh5py-0.9.0rc3/geoh5py/shared/conversion/geo_image.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/conversion/grid2d.py` & `geoh5py-0.9.0rc3/geoh5py/shared/conversion/grid2d.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/entity.py` & `geoh5py-0.9.0rc3/geoh5py/shared/entity.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/entity_container.py` & `geoh5py-0.9.0rc3/geoh5py/shared/entity_container.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/entity_type.py` & `geoh5py-0.9.0rc3/geoh5py/shared/entity_type.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/exceptions.py` & `geoh5py-0.9.0rc3/geoh5py/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/merging/__init__.py` & `geoh5py-0.9.0rc3/geoh5py/shared/merging/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/merging/base.py` & `geoh5py-0.9.0rc3/geoh5py/shared/merging/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/merging/cell.py` & `geoh5py-0.9.0rc3/geoh5py/shared/merging/cell.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/merging/drape_model.py` & `geoh5py-0.9.0rc3/geoh5py/shared/merging/drape_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/merging/points.py` & `geoh5py-0.9.0rc3/geoh5py/shared/merging/points.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/utils.py` & `geoh5py-0.9.0rc3/geoh5py/shared/utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/validators.py` & `geoh5py-0.9.0rc3/geoh5py/shared/validators.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/shared/weakref_utils.py` & `geoh5py-0.9.0rc3/geoh5py/shared/weakref_utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/ui_json/__init__.py` & `geoh5py-0.9.0rc3/geoh5py/ui_json/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/ui_json/constants.py` & `geoh5py-0.9.0rc3/geoh5py/ui_json/constants.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/ui_json/descriptors.py` & `geoh5py-0.9.0rc3/geoh5py/ui_json/descriptors.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/ui_json/enforcers.py` & `geoh5py-0.9.0rc3/geoh5py/ui_json/enforcers.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/ui_json/forms.py` & `geoh5py-0.9.0rc3/geoh5py/ui_json/forms.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/ui_json/input_file.py` & `geoh5py-0.9.0rc3/geoh5py/ui_json/input_file.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/ui_json/parameters.py` & `geoh5py-0.9.0rc3/geoh5py/ui_json/parameters.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/ui_json/templates.py` & `geoh5py-0.9.0rc3/geoh5py/ui_json/templates.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/ui_json/ui_json.py` & `geoh5py-0.9.0rc3/geoh5py/ui_json/ui_json.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/ui_json/utils.py` & `geoh5py-0.9.0rc3/geoh5py/ui_json/utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/ui_json/validation.py` & `geoh5py-0.9.0rc3/geoh5py/ui_json/validation.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/workspace/__init__.py` & `geoh5py-0.9.0rc3/geoh5py/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/geoh5py/workspace/workspace.py` & `geoh5py-0.9.0rc3/geoh5py/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/package.rst` & `geoh5py-0.9.0rc3/package.rst`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/pyproject.toml` & `geoh5py-0.9.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geoh5py"
-version = "0.9.0-rc.2"
+version = "0.9.0-rc.3"
 license = "LGPL-3.0-or-later"
 description = "Python API for geoh5, an open file format for geoscientific data"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/geoh5py"
 maintainers = [
     "Benjamin Kary <benjamink@mirageoscience.com>",
     "Dominique Fournier <dominiquef@mirageoscience.com>",
```

### Comparing `geoh5py-0.9.0rc2/README.rst` & `geoh5py-0.9.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/THIRD_PARTY_SOFTWARE.rst` & `geoh5py-0.9.0rc3/THIRD_PARTY_SOFTWARE.rst`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0rc2/PKG-INFO` & `geoh5py-0.9.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoh5py
-Version: 0.9.0rc2
+Version: 0.9.0rc3
 Summary: Python API for geoh5, an open file format for geoscientific data
 Home-page: https://www.mirageoscience.com/mining-industry-software/python-integration/
 License: LGPL-3.0-or-later
 Keywords: geology,geophysics,data,interoperability
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Maintainer: Benjamin Kary
```

